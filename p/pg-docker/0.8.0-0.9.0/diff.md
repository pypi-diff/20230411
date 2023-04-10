# Comparing `tmp/pg_docker-0.8.0.tar.gz` & `tmp/pg_docker-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pg_docker-0.8.0.tar", max compression
+gzip compressed data, was "pg_docker-0.9.0.tar", max compression
```

## Comparing `pg_docker-0.8.0.tar` & `pg_docker-0.9.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2286 2022-12-19 20:16:34.229525 pg_docker-0.8.0/README.md
--rw-r--r--   0        0        0       88 2022-12-15 21:23:14.996919 pg_docker-0.8.0/pg_docker/__init__.py
--rw-r--r--   0        0        0     8213 2023-04-06 14:56:37.634490 pg_docker-0.8.0/pg_docker/_core.py
--rw-r--r--   0        0        0     1169 2022-12-15 22:40:13.976549 pg_docker-0.8.0/pg_docker/_plugin.py
--rw-r--r--   0        0        0        0 2022-12-19 18:30:52.443272 pg_docker-0.8.0/pg_docker/py.typed
--rw-r--r--   0        0        0      569 2023-04-06 15:01:40.631392 pg_docker-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     3046 1970-01-01 00:00:00.000000 pg_docker-0.8.0/setup.py
--rw-r--r--   0        0        0     2736 1970-01-01 00:00:00.000000 pg_docker-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     2286 2022-12-19 20:16:34.229525 pg_docker-0.9.0/README.md
+-rw-r--r--   0        0        0       88 2022-12-15 21:23:14.996919 pg_docker-0.9.0/pg_docker/__init__.py
+-rw-r--r--   0        0        0     9125 2023-04-10 22:54:37.860747 pg_docker-0.9.0/pg_docker/_core.py
+-rw-r--r--   0        0        0     1169 2022-12-15 22:40:13.976549 pg_docker-0.9.0/pg_docker/_plugin.py
+-rw-r--r--   0        0        0        0 2022-12-19 18:30:52.443272 pg_docker-0.9.0/pg_docker/py.typed
+-rw-r--r--   0        0        0      569 2023-04-10 22:56:24.865510 pg_docker-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3046 1970-01-01 00:00:00.000000 pg_docker-0.9.0/setup.py
+-rw-r--r--   0        0        0     2736 1970-01-01 00:00:00.000000 pg_docker-0.9.0/PKG-INFO
```

### Comparing `pg_docker-0.8.0/README.md` & `pg_docker-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pg_docker-0.8.0/pg_docker/_core.py` & `pg_docker-0.9.0/pg_docker/_core.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,18 @@
     pass
 
 
 def _noop_setup_db(db_params: DatabaseParams) -> None:
     return
 
 
+class _DBShuttingDownError(Exception):
+    pass
+
+
 class DatabaseCleaner:
     def __init__(
         self,
         root_params: DatabaseParams,
         clean_dbs: multiprocessing.Queue[DatabaseParams],
         dirty_dbs: multiprocessing.Queue[DatabaseParams],
         setup_db: Callable[[DatabaseParams], None] = _noop_setup_db,
@@ -42,51 +46,57 @@
 
     @functools.cached_property
     def _cursor(self) -> psycopg2.cursor:
         connection = psycopg2.connect(**self._root_params.connection_kwargs())
         cursor = connection.cursor()
         cursor.execute("COMMIT")
         return cursor
+    
+    def _execute_sql(self, sql: str) -> None:
+        try:
+            self._cursor.execute(sql)
+        except psycopg2.OperationalError as e:
+            raise _DBShuttingDownError() from e
 
     def create_db(self, db_params: DatabaseParams) -> None:
-        self._cursor.execute(
+        self._execute_sql(
             f"""
             CREATE USER {db_params.user}
                 PASSWORD '{db_params.password}'
             """
         )
-        self._cursor.execute(
+        self._execute_sql(
             f"""
             CREATE DATABASE {db_params.dbname}
                 OWNER = {db_params.user}
             """
         )
 
     def drop_db(self, db_params: DatabaseParams) -> None:
-        self._cursor.execute(
+        self._execute_sql(
             f"""
             SELECT pg_terminate_backend(pg_stat_activity.pid)
             FROM pg_stat_activity
             WHERE pid <> pg_backend_pid() 
             AND pg_stat_activity.datname = '{db_params.dbname}'
             """
         )
-        self._cursor.execute(
+        self._execute_sql(
             f"""
             DROP DATABASE IF EXISTS {db_params.dbname}
         """
         )
-        self._cursor.execute(
+        self._execute_sql(
             f"""
             DROP USER IF EXISTS {db_params.user}
             """
         )
 
     def drop_all_connections(self) -> None:
-        self._cursor.execute(
+        self._execute_sql(
             """
             SELECT pg_terminate_backend(pg_stat_activity.pid)
             FROM pg_stat_activity
             WHERE pid <> pg_backend_pid()
             """
         )
 
@@ -100,40 +110,47 @@
         self.setup_db(database_to_clean)
         self.clean_dbs.put(database_to_clean)
 
     def run_forever(
         self,
     ) -> None:
         while not self._stop_event.is_set():
-            self.maybe_clean_a_dirty_db()
+            try:
+                self.maybe_clean_a_dirty_db()
+            except _DBShuttingDownError:
+                break
         self.drop_all_connections()
         self._cursor.close()
         self._cursor.connection.close()
 
     def stop(self) -> None:
         self._stop_event.set()
 
 
 @dataclasses.dataclass()
 class DatabasePool:
     root_params: DatabaseParams
     max_pool_size: int
+    cleaning_workers: int
     setup_db: Callable[[DatabaseParams], None] = _noop_setup_db
 
     def __post_init__(self) -> None:
         self._dirty_dbs: multiprocessing.Queue[DatabaseParams] = multiprocessing.Queue()
         self._clean_dbs: multiprocessing.Queue[DatabaseParams] = multiprocessing.Queue()
-        self._cleaner = DatabaseCleaner(
-            self.root_params, self._clean_dbs, self._dirty_dbs, self.setup_db
-        )
+        self._cleaners = [
+            DatabaseCleaner(
+                self.root_params, self._clean_dbs, self._dirty_dbs, self.setup_db
+            )
+            for _ in range(self.cleaning_workers)
+        ]
 
         self._pool_size = 0
 
         self._wait_until_ready()
-        self._cleanup_process = self._launch_cleanup_process()
+        self._cleanup_processes = self._launch_cleanup_processes()
         self._saturate_pool()
 
     def _saturate_pool(self) -> None:
         while self._pool_size < self.max_pool_size:
             self._add_db_to_pool()
 
     def _add_db_to_pool(self) -> None:
@@ -141,22 +158,26 @@
         new_database = dataclasses.replace(
             self.root_params,
             dbname=f"__test_db_{self._pool_size}",
             user=f"__test_user_{self._pool_size}",
         )
         self._dirty_dbs.put(new_database)
 
-    def _launch_cleanup_process(self) -> multiprocessing.Process:
-        process = multiprocessing.Process(
-            target=self._cleaner.run_forever,
-            name="test-database-cleanup",
-            daemon=True,
-        )
-        process.start()
-        return process
+    def _launch_cleanup_processes(self) -> list[multiprocessing.Process]:
+        processes = [
+            multiprocessing.Process(
+                target=cleaner.run_forever,
+                name=f"test-database-cleaner-{i}",
+                daemon=True,
+            )
+            for i, cleaner in enumerate(self._cleaners)
+        ]
+        for process in processes:
+            process.start()
+        return processes
 
     def _wait_until_ready(self) -> None:
         while True:
             try:
                 psycopg2.connect(**self.root_params.connection_kwargs())
             except psycopg2.Error as e:
                 pass
@@ -164,29 +185,31 @@
                 return
 
     def _get_db_and_check_on_cleanup(self) -> DatabaseParams:
         while True:
             try:
                 return self._clean_dbs.get(timeout=_SHORT_TIMEOUT)
             except (queue.Empty, multiprocessing.TimeoutError):
-                if not self._cleanup_process.is_alive():
-                    raise CleanupProcessTerminatedError()
+                for process in self._cleanup_processes:
+                    if not process.is_alive():
+                        raise CleanupProcessTerminatedError()
 
     @contextlib.contextmanager
     def database(self) -> Generator[DatabaseParams, None, None]:
         """Returns the connection parameters to a clean database."""
 
         database = self._get_db_and_check_on_cleanup()
         try:
             yield database
         finally:
             self._dirty_dbs.put(database)
 
     def stop(self):
-        self._cleaner.stop()
+        for cleaner in self._cleaners:
+            cleaner.stop()
 
 
 class DatabaseParamsDict(TypedDict):
     host: str
     port: int
     dbname: str
     user: str
@@ -227,15 +250,16 @@
     return sock.getsockname()[1]
 
 
 @contextlib.contextmanager
 def database_pool(
     *,
     postgres_image_tag: str = "latest",
-    max_pool_size: int = 5,
+    max_pool_size: int = 10,
+    cleaning_workers: int = 5,
     docker_command: str = "docker",
     setup_db: Callable[[DatabaseParams], None] = _noop_setup_db,
 ) -> Generator[DatabasePool, None, None]:
     """A context manager to create a database pool.
 
     This will return an instance of `DatabasePool`.
 
@@ -250,32 +274,38 @@
         more info. 
     """
     port = get_free_port()
     docker_process = subprocess.Popen(
         [
             docker_command,
             "run",
+            "--tmpfs",
+            "/var/lib/postgresql/data"
             "--rm",
             "-t",
             f"-p{port}:5432",
             f"-ePOSTGRES_PASSWORD={_PG_PASSWORD}",
             f"postgres:{postgres_image_tag}",
+            "-c", "fsync=off",
+            "-c", "synchronous_commit=off",
+            "-c", "full_page_writes=off",
         ],
         stderr=subprocess.DEVNULL,
         stdout=subprocess.DEVNULL,
     )
     pool = DatabasePool(
         DatabaseParams(
             host="0.0.0.0",
             port=port,
             dbname=_PG_ROOT_DATABASE,
             user=_PG_ROOT_USER,
             password=_PG_PASSWORD,
         ),
         max_pool_size=max_pool_size,
+        cleaning_workers=cleaning_workers,
         setup_db=setup_db
     )
     try:
         yield pool
     finally:
         pool.stop()
         docker_process.terminate()
```

### Comparing `pg_docker-0.8.0/pg_docker/_plugin.py` & `pg_docker-0.9.0/pg_docker/_plugin.py`

 * *Files identical despite different names*

### Comparing `pg_docker-0.8.0/pyproject.toml` & `pg_docker-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pg-docker"
-version = "0.8.0"
+version = "0.9.0"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 packages = [{include = "pg_docker"}]
 classifiers = [
     "Framework :: Pytest"
 ]
```

### Comparing `pg_docker-0.8.0/setup.py` & `pg_docker-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['psycopg2>=2.9,<3.0']
 
 entry_points = \
 {'pytest11': ['pg_docker = pg_docker._plugin']}
 
 setup_kwargs = {
     'name': 'pg-docker',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': '',
     'long_description': '# PG Docker\n\nA python package to provide containerized postgres databases in python\n\n**Why would you need this?**\n\nIf you are using postgres and want to write tests that run against a real database, then this will make your life easier.\n\n## Installation\n\nInstall via pip:\n```\npip install pg-docker\n```\n\nYou will also need to have [docker](https://www.docker.com/).\n\n## Usage\n\nNote: *This package is mainly built with pytest in mind, but you can use the context managers documented below with other testing frameworks as well.*\n\n### Example\n\nWith pytest:\n```py\nimport psycopg2\n\n\npytest_plugins = ["pg_docker"]\n\n\ndef test_using_a_database(pg_database):\n    db_connection = psycopg2.connect(**pg_database.connection_kwargs())\n    cursor = db_connection.cursor()\n    cursor.execute("SELECT \'hello world!\'")\n\n    assert cursor.fetchone() == ("hello world!",)\n```\n\n### Usage with pytest\n\nYou first need to enable the plugin. To do this add a `conftest.py` to the root directory of your tests and add:\n```py\npytest_plugins = ["pg_docker"]\n```\nYou can find more details on how to activate plugins in the [pytest docs](https://docs.pytest.org/en/latest/how-to/plugins.html#requiring-loading-plugins-in-a-test-module-or-conftest-file)\n\nThe plugin The following fixtures:\n\n - `pg_database`: `DatabaseParams` for a clean database.\n - `pg_database_pool`: A `DatabasePool` instance. Use this if you need more than one database in your tests at a time.\n\n\n### Configuring Database Migrations\n\nUse the below template in your `conftest.py` to configure how your databases are set up. \n```py\ndef setup_db(pg_params):\n    """Add any setup logic for your database in here."""\n    pass\n\n@pytest.fixture(scope="session")\ndef pg_setup_db():\n    return setup_db\n```\nNote: *You might be inclined to edit the above code to nest the setup_db function inside of the fixture function. This will not work, because the fixture result needs to be [pickleable](https://docs.python.org/3/library/pickle.html#what-can-be-pickled-and-unpickled)!*\n\n\n### Advanced Usage (and other testing frameworks)\n\nFor other use cases you can use the `database_pool` context manager:\n```py\nwith database_pool() as db_pool:\n    with db_pool.database as db_params:\n        connection = psycopg2.connect(**db_params.connection_kwargs())\n```\n',
     'author': 'Your Name',
     'author_email': 'you@example.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pg_docker-0.8.0/PKG-INFO` & `pg_docker-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pg-docker
-Version: 0.8.0
+Version: 0.9.0
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

