# Comparing `tmp/fh_fablib-1.0.20230303.tar.gz` & `tmp/fh_fablib-1.0.20230411.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fh_fablib-1.0.20230303.tar", last modified: Fri Mar  3 08:47:42 2023, max compression
+gzip compressed data, was "fh_fablib-1.0.20230411.tar", last modified: Tue Apr 11 12:23:25 2023, max compression
```

## Comparing `fh_fablib-1.0.20230303.tar` & `fh_fablib-1.0.20230411.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-03-03 08:47:42.805658 fh_fablib-1.0.20230303/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1548 2022-02-08 07:07:00.000000 fh_fablib-1.0.20230303/LICENSE
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      198 2022-04-04 07:13:49.000000 fh_fablib-1.0.20230303/MANIFEST.in
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     7689 2023-03-03 08:47:42.805658 fh_fablib-1.0.20230303/PKG-INFO
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     7322 2023-03-03 08:47:35.000000 fh_fablib-1.0.20230303/README.rst
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-03-03 08:47:42.805658 fh_fablib-1.0.20230303/fh_fablib/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    25949 2023-03-03 08:47:35.000000 fh_fablib-1.0.20230303/fh_fablib/__init__.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-03-03 08:47:42.805658 fh_fablib-1.0.20230303/fh_fablib/dotfiles/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      200 2023-03-03 08:44:50.000000 fh_fablib-1.0.20230303/fh_fablib/dotfiles/.editorconfig
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      201 2023-01-16 12:43:58.000000 fh_fablib-1.0.20230303/fh_fablib/dotfiles/.eslintrc.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2400 2023-03-03 08:45:08.000000 fh_fablib-1.0.20230303/fh_fablib/dotfiles/.pre-commit-config.yaml
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     5820 2023-03-03 08:44:50.000000 fh_fablib-1.0.20230303/fh_fablib/dotfiles/webpack.library.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2091 2022-02-08 07:07:00.000000 fh_fablib-1.0.20230303/fh_fablib/extract_js_gettext_strings.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-03-03 08:47:42.805658 fh_fablib-1.0.20230303/fh_fablib.egg-info/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     7689 2023-03-03 08:47:42.000000 fh_fablib-1.0.20230303/fh_fablib.egg-info/PKG-INFO
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      489 2023-03-03 08:47:42.000000 fh_fablib-1.0.20230303/fh_fablib.egg-info/SOURCES.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2023-03-03 08:47:42.000000 fh_fablib-1.0.20230303/fh_fablib.egg-info/dependency_links.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       47 2023-03-03 08:47:42.000000 fh_fablib-1.0.20230303/fh_fablib.egg-info/entry_points.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2022-02-11 12:00:50.000000 fh_fablib-1.0.20230303/fh_fablib.egg-info/not-zip-safe
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       25 2023-03-03 08:47:42.000000 fh_fablib-1.0.20230303/fh_fablib.egg-info/requires.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       10 2023-03-03 08:47:42.000000 fh_fablib-1.0.20230303/fh_fablib.egg-info/top_level.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      694 2023-03-03 08:47:42.805658 fh_fablib-1.0.20230303/setup.cfg
--rwxrwxr-x   0 matthias  (1000) matthias  (1000)       62 2022-04-06 07:00:23.000000 fh_fablib-1.0.20230303/setup.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-04-11 12:23:25.927419 fh_fablib-1.0.20230411/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1548 2022-05-20 14:16:22.000000 fh_fablib-1.0.20230411/LICENSE
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      198 2022-05-20 14:16:22.000000 fh_fablib-1.0.20230411/MANIFEST.in
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     7689 2023-04-11 12:23:25.927419 fh_fablib-1.0.20230411/PKG-INFO
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     7322 2023-04-11 12:23:02.000000 fh_fablib-1.0.20230411/README.rst
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-04-11 12:23:25.926419 fh_fablib-1.0.20230411/fh_fablib/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    26437 2023-04-11 12:23:02.000000 fh_fablib-1.0.20230411/fh_fablib/__init__.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-04-11 12:23:25.926419 fh_fablib-1.0.20230411/fh_fablib/dotfiles/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      200 2022-05-20 14:16:22.000000 fh_fablib-1.0.20230411/fh_fablib/dotfiles/.editorconfig
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      201 2022-05-20 14:16:22.000000 fh_fablib-1.0.20230411/fh_fablib/dotfiles/.eslintrc.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     2013 2023-04-11 12:21:56.000000 fh_fablib-1.0.20230411/fh_fablib/dotfiles/.pre-commit-config.yaml
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      455 2023-04-11 12:21:56.000000 fh_fablib-1.0.20230411/fh_fablib/dotfiles/pyproject.toml
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5820 2023-03-07 08:46:55.000000 fh_fablib-1.0.20230411/fh_fablib/dotfiles/webpack.library.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2091 2022-05-20 14:16:22.000000 fh_fablib-1.0.20230411/fh_fablib/extract_js_gettext_strings.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-04-11 12:23:25.926419 fh_fablib-1.0.20230411/fh_fablib.egg-info/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     7689 2023-04-11 12:23:25.000000 fh_fablib-1.0.20230411/fh_fablib.egg-info/PKG-INFO
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      538 2023-04-11 12:23:25.000000 fh_fablib-1.0.20230411/fh_fablib.egg-info/SOURCES.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2023-04-11 12:23:25.000000 fh_fablib-1.0.20230411/fh_fablib.egg-info/dependency_links.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       47 2023-04-11 12:23:25.000000 fh_fablib-1.0.20230411/fh_fablib.egg-info/entry_points.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2022-05-20 14:16:27.000000 fh_fablib-1.0.20230411/fh_fablib.egg-info/not-zip-safe
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       24 2023-04-11 12:23:25.000000 fh_fablib-1.0.20230411/fh_fablib.egg-info/requires.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       10 2023-04-11 12:23:25.000000 fh_fablib-1.0.20230411/fh_fablib.egg-info/top_level.txt
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      465 2023-04-11 12:21:56.000000 fh_fablib-1.0.20230411/pyproject.toml
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      693 2023-04-11 12:23:25.927419 fh_fablib-1.0.20230411/setup.cfg
+-rwxrwxr-x   0 matthias  (1000) matthias  (1000)       62 2022-05-20 14:16:22.000000 fh_fablib-1.0.20230411/setup.py
```

### Comparing `fh_fablib-1.0.20230303/LICENSE` & `fh_fablib-1.0.20230411/LICENSE`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20230303/PKG-INFO` & `fh_fablib-1.0.20230411/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fh_fablib
-Version: 1.0.20230303
+Version: 1.0.20230411
 Summary: fh-fablib
 Home-page: https://github.com/feinheit/fh-fablib/
 Author: Matthias Kestenholz
 Author-email: mk@feinheit.ch
 License: BSD-3-Clause
 Platform: OS Independent
 Classifier: License :: OSI Approved :: BSD License
@@ -28,15 +28,15 @@
 
 3. Add a ``fabfile.py`` to your project. A minimal example follows:
 
    .. code-block:: python
 
        import fh_fablib as fl
 
-       fl.require("1.0.20230303")
+       fl.require("1.0.20230411")
        fl.config.update(host="www-data@feinheit06.nine.ch")
 
        environments = [
            fl.environment(
                "production",
                {
                    "domain": "example.com",
@@ -104,15 +104,15 @@
 
 If you need multiple environments, add environment tasks as follows:
 
 .. code-block:: python
 
     import fh_fablib as fl
 
-    fl.require("1.0.20230303")
+    fl.require("1.0.20230411")
     fl.config.update(host="www-data@feinheit06.nine.ch")
 
     environments = [
         fl.environment(
             "production",
             {
                 "domain": "example.com",
```

### Comparing `fh_fablib-1.0.20230303/README.rst` & `fh_fablib-1.0.20230411/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 3. Add a ``fabfile.py`` to your project. A minimal example follows:
 
    .. code-block:: python
 
        import fh_fablib as fl
 
-       fl.require("1.0.20230303")
+       fl.require("1.0.20230411")
        fl.config.update(host="www-data@feinheit06.nine.ch")
 
        environments = [
            fl.environment(
                "production",
                {
                    "domain": "example.com",
@@ -90,15 +90,15 @@
 
 If you need multiple environments, add environment tasks as follows:
 
 .. code-block:: python
 
     import fh_fablib as fl
 
-    fl.require("1.0.20230303")
+    fl.require("1.0.20230411")
     fl.config.update(host="www-data@feinheit06.nine.ch")
 
     environments = [
         fl.environment(
             "production",
             {
                 "domain": "example.com",
```

### Comparing `fh_fablib-1.0.20230303/fh_fablib/__init__.py` & `fh_fablib-1.0.20230411/fh_fablib/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from fabric import Connection, task
 from invoke import Collection  # noqa, re-export
 from speckenv_django import django_database_url
 
 from fh_fablib.extract_js_gettext_strings import generate_strings
 
 
-__version__ = "1.0.20230303"
+__version__ = "1.0.20230411"
 
 
 # I don't care, in this context.
 warnings.simplefilter("ignore", category=ResourceWarning)
 
 
 def ansi(code):
@@ -95,14 +95,23 @@
                 warning(
                     "The fabfile and dotfiles have been updated automatically.\n\nPlease check the result twice before committing!"
                 )
 
 
 def run(c, *a, **kw):
     """A Context.run or Connection.run with better defaults"""
+    kw.setdefault("pty", False)
+    kw.setdefault("replace_env", True)
+    if not kw.get("hide"):
+        progress(" ".join(str(part) for part in a))
+    return c.run(*a, **kw)
+
+
+def run_local(c, *a, **kw):
+    """A Context.run for local execution with better defaults"""
     kw.setdefault("pty", True)
     kw.setdefault("replace_env", False)
     if not kw.get("hide"):
         progress(" ".join(str(part) for part in a))
     return c.run(*a, **kw)
 
 
@@ -189,15 +198,15 @@
 {jobs}
 {{ set +x; }} 2>/dev/null
 
 for job in $(jobs -p); do wait $job; done
 """
         )
         f.flush()
-        run(ctx, f"bash {f.name}", replace_env=False)
+        run_local(ctx, f"bash {f.name}", replace_env=False)
 
 
 def _update_dotfiles(*, force):
     source = Path(__file__).parent / "dotfiles"
     target = config.base
     for s in sorted(source.glob("*")):
         t = target / s.name
@@ -207,15 +216,15 @@
 
 @task(auto_shortflags=False, help={"force": "Overwrite existing pre-commit files"})
 def hook(ctx, force=False):
     """
     Add default pre-commit configuration and install hook running coding style checks
     """
     _update_dotfiles(force=force)
-    run(ctx, "pre-commit install -f")
+    run_local(ctx, "pre-commit install -f")
 
 
 @task(auto_shortflags=False)
 def dev(ctx, host="127.0.0.1", port=8000):
     """Run the development server for the frontend and backend"""
     progress(f"Starting server at http://{host}:{port}/")
     backend = random.randint(50000, 60000)
@@ -246,50 +255,50 @@
     with Connection(config.host) as conn:
         e = _srv_env(conn, f"{config.domain}/.env")
 
     srv_dsn = e("DATABASE_URL")
     local_dsn = _local_env()("DATABASE_URL")
     dbname = _dbname_from_dsn(local_dsn)
 
-    run(ctx, f"dropdb --if-exists {dbname}", warn=True)
-    run(ctx, f"createdb {dbname}")
-    run(
+    run_local(ctx, f"dropdb --if-exists {dbname}", warn=True)
+    run_local(ctx, f"createdb {dbname}")
+    run_local(
         ctx,
         f"ssh {config.host} -C 'pg_dump -Ox {srv_dsn} {extra_dump_args}' | psql {local_dsn}",
     )
 
     reset_pw(ctx)
 
 
 @task(auto_shortflags=False)
 def pull_media(ctx, folder="media"):
     """Rsync a folder from the remote to the local environment"""
     flags = "-pthrz --stats"
     folder = folder.strip("/")
-    run(ctx, f"rsync {flags} {config.host}:{config.domain}/{folder}/ {folder}/")
+    run_local(ctx, f"rsync {flags} {config.host}:{config.domain}/{folder}/ {folder}/")
 
 
 @task
 def reset_pw(ctx):
     """Set all user passwords to "password" """
     # 'password' encoded with a constant salt. Does not force a login after pull_db
     pw = r"pbkdf2_sha256\$320000\$2Hz1pcncCTWtqEnr3uoBdD\$nVc9Fka1oYQHFgGRGLUC4Nw3w6+ZmdO0IDdZOow+kJ0="
-    run(
+    run_local(
         ctx,
         f"venv/bin/python manage.py shell -c \"pw='{pw}';"
         f"from django.contrib.auth import get_user_model as g;"
         f'g()._base_manager.update(password=pw)"',
     )
 
 
 @task
 def reset_sq(ctx):
     """Reset all PostgreSQL sequences"""
 
-    SQL = """
+    sql = """
 SELECT 'SELECT SETVAL(' ||
        quote_literal(quote_ident(PGT.schemaname) || '.' || quote_ident(S.relname)) ||
        ', COALESCE(MAX(' ||quote_ident(C.attname)|| '), 1) ) FROM ' ||
        quote_ident(PGT.schemaname)|| '.'||quote_ident(T.relname)|| ';'
 FROM pg_class AS S,
      pg_depend AS D,
      pg_class AS T,
@@ -303,17 +312,17 @@
     AND T.relname = PGT.tablename
 ORDER BY S.relname;
     """
 
     dsn = _local_env()("DATABASE_URL")
 
     with tempfile.NamedTemporaryFile("w") as f:
-        f.write(SQL)
+        f.write(sql)
         f.seek(0)
-        run(ctx, f"psql -Atq -f {f.name} {dsn} | psql -a {dsn}")
+        run_local(ctx, f"psql -Atq -f {f.name} {dsn} | psql -a {dsn}")
 
 
 def _local_env(path=".env"):
     mapping = {}
     speckenv.read_speckenv(config.base / path, mapping=mapping)
 
     return lambda *a, **kw: speckenv.env(*a, **kw, mapping=mapping)
@@ -337,33 +346,33 @@
     """Update the translation catalogs"""
 
     with open("conf/strings.js", "w", encoding="utf-8") as f:
         f.write("/* eslint-disable */\n")
         f.write("".join(f"{str}\n" for str in generate_strings()))
 
     language = f"-l {language}" if language else "-a"
-    run(
+    run_local(
         ctx,
         f"venv/bin/python manage.py makemessages {language} --add-location file"
         " -i venv -i htmlcov -i node_modules -i lib -i build -i dist --no-wrap",
         replace_env=False,
     )
-    run(
+    run_local(
         ctx,
         f"venv/bin/python manage.py makemessages {language} --add-location file"
         " -i venv -i htmlcov -i node_modules -i lib -i build -i dist --no-wrap"
         " -d djangojs",
         replace_env=False,
     )
 
 
 @task
 def cm(ctx):
     """Compile the translation catalogs"""
-    run(
+    run_local(
         ctx,
         "venv/bin/python manage.py compilemessages"
         " -i venv -i htmlcov -i node_modules -i lib -i build -i dist",
         replace_env=False,
     )
 
 
@@ -383,50 +392,52 @@
         "stable": "Avoid pre-release versions of packages",
     },
 )
 def upgrade(ctx, keep=False, stable=False):
     """Re-create the virtualenv with newest versions of all libraries"""
     venv = config.base / "venv"
     if not venv.exists() or not keep:
-        run(ctx, f"rm -rf venv && {_python3()} -m venv venv")
+        run_local(ctx, f"rm -rf venv && {_python3()} -m venv venv")
     _pip_up(ctx)
     extra = "" if stable else "--pre"
-    run(ctx, f"venv/bin/python -m pip install -U -r requirements-to-freeze.txt {extra}")
+    run_local(
+        ctx, f"venv/bin/python -m pip install -U -r requirements-to-freeze.txt {extra}"
+    )
     freeze(ctx)
     hook(ctx)
 
 
 @task
 def freeze(ctx):
     """Freeze the virtualenv's state"""
-    run(
+    run_local(
         ctx,
         '(printf "# AUTOGENERATED, DO NOT EDIT\n\n";' "venv/bin/python -m pip freeze -l"
         # Until Ubuntu gets its act together:
         ' | grep -vE "(^pkg.resources)"' ") > requirements.txt",
     )
 
 
 @task
 def update(ctx):
     """Update virtualenv and node_modules to match the lockfiles"""
     venv = config.base / "venv"
     if not venv.exists():
-        run(ctx, f"{_python3()} -m venv venv")
+        run_local(ctx, f"{_python3()} -m venv venv")
     _pip_up(ctx)
     _concurrently(
         ctx,
         [
             "venv/bin/python -m pip install -r requirements.txt",
             "git submodule update --init",
             'find . -name "*.pyc" -delete',
             "yarn",
         ],
     )
-    run(ctx, "venv/bin/python manage.py migrate", warn=True)
+    run_local(ctx, "venv/bin/python manage.py migrate", warn=True)
     hook(ctx)
 
 
 def _local_dotenv_if_not_exists():
     dotenv = config.base / ".env"
     if dotenv.exists():
         return
@@ -457,17 +468,17 @@
 @task(
     auto_shortflags=False,
     help={"clobber": "Clobber pre-existing node_modules and venv folders"},
 )
 def local(ctx, clobber=False):
     """Local environment setup"""
     if clobber:
-        run(ctx, "rm -rf node_modules venv")
+        run_local(ctx, "rm -rf node_modules venv")
     dbname = _local_dbname()
-    run(ctx, f"createdb {dbname}", warn=True)
+    run_local(ctx, f"createdb {dbname}", warn=True)
     update(ctx)
 
 
 @task
 def nine_vhost(ctx):
     """Create a virtual host using nine-manage-vhosts"""
     with Connection(config.host) as conn, conn.cd(config.domain):
@@ -764,67 +775,69 @@
     nine_vhost(ctx)
     nine_unit(ctx)
 
 
 @task
 def github(ctx):
     """Create a repository on GitHub and push the code"""
-    url = run(ctx, "git config remote.origin.url", hide=True, warn=True).stdout.strip()
+    url = run_local(
+        ctx, "git config remote.origin.url", hide=True, warn=True
+    ).stdout.strip()
     if url:
         terminate(f"The 'origin' remote already points to '{url}'")
 
     e = _local_env(Path.home() / ".box.env")
     organization = e("GITHUB_ORGANIZATION")
     repository = config.domain
 
     print(f"Organization [{organization}]: ", end="")
     organization = input() or organization
     print(f"Repository [{repository}]: ", end="")
     repository = input() or repository
 
-    run(
+    run_local(
         ctx,
         f"gh repo create {organization}/{repository} --private --source=. --remote=origin --push",
     )
-    run(ctx, f"git push -u origin {config.branch}")
+    run_local(ctx, f"git push -u origin {config.branch}")
 
 
 @task
 def fetch(ctx):
     """Ensure a remote exists for the server and fetch"""
-    run(
+    run_local(
         ctx,
         f"git remote add {config.remote} {config.host}:{config.domain}",
         warn=True,
         hide=True,
     )
-    run(ctx, f"git fetch {config.remote}")
+    run_local(ctx, f"git fetch {config.remote}")
 
 
 def _check_branch(ctx):
-    branch = run(ctx, "git rev-parse --abbrev-ref HEAD", hide=True).stdout.strip()
+    branch = run_local(ctx, "git rev-parse --abbrev-ref HEAD", hide=True).stdout.strip()
     if branch != config.branch:
         terminate(f"Current branch is '{branch}', should be '{config.branch}'")
 
 
 def _check_no_uncommitted_changes(ctx):
     with Connection(config.host) as conn, conn.cd(config.domain):
         result = run(conn, "git status --porcelain").stdout.strip()
         if result:
             terminate("Terminating because of uncommitted changes on server")
 
 
 @task
 def check(ctx):
     """Check the coding style of staged files"""
-    run(ctx, "pre-commit run")
+    run_local(ctx, "pre-commit run")
 
 
 def _deploy_sync_origin_url(ctx, conn):
-    url = run(ctx, "git remote get-url origin").stdout.strip()
+    url = run_local(ctx, "git remote get-url origin").stdout.strip()
     run(conn, f"git remote set-url origin {url}")
 
 
 def _deploy_django(conn):
     run(conn, "git fetch origin")
     run(conn, f"git checkout {config.branch}")
 
@@ -844,30 +857,32 @@
 def _deploy_staticfiles(conn):
     run(conn, "venv/bin/python manage.py collectstatic --noinput")
 
 
 def _rsync_static(ctx, *, delete=False):
     flags = "-pthrz --stats"
     delete = " --delete" if delete else ""
-    run(ctx, f"rsync {flags}{delete} static/ {config.host}:{config.domain}/static/")
+    run_local(
+        ctx, f"rsync {flags}{delete} static/ {config.host}:{config.domain}/static/"
+    )
 
 
 @task(
     auto_shortflags=False,
     help={"fast": "Skip the Webpack build", "force": "Force the git push"},
 )
 def deploy(ctx, fast=False, force=False):
     """Deploy once 🔥"""
     _check_branch(ctx)
     _check_no_uncommitted_changes(ctx)
     check(ctx)
     force = "--force-with-lease " if (force or config.force) else ""
-    run(ctx, f"git push origin {force}{config.branch}")
+    run_local(ctx, f"git push origin {force}{config.branch}")
     if not fast:
-        run(ctx, "NODE_ENV=production yarn run webpack --mode production --bail")
+        run_local(ctx, "NODE_ENV=production yarn run webpack --mode production --bail")
 
     with Connection(config.host) as conn, conn.cd(config.domain):
         _deploy_sync_origin_url(ctx, conn)
         _deploy_django(conn)
         if not fast:
             _rsync_static(ctx, delete=True)
         _deploy_staticfiles(conn)
```

### Comparing `fh_fablib-1.0.20230303/fh_fablib/dotfiles/.pre-commit-config.yaml` & `fh_fablib-1.0.20230411/fh_fablib/dotfiles/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -16,46 +16,33 @@
     hooks:
       - id: django-check
         name: django check
         entry: venv/bin/python manage.py check
         pass_filenames: false
         language: system
         always_run: true
-  - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
-    hooks:
-      - id: pyupgrade
-        args: [--py39-plus]
   - repo: https://github.com/adamchainz/django-upgrade
     rev: 1.13.0
     hooks:
       - id: django-upgrade
         args: [--target-version, "4.0"]
   - repo: https://github.com/MarcoGorelli/absolufy-imports
     rev: v0.3.1
     hooks:
       - id: absolufy-imports
-  - repo: https://github.com/pycqa/isort
-    rev: 5.12.0
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    rev: "v0.0.261"
     hooks:
-      - id: isort
-        args: [--profile=black, --lines-after-imports=2, --combine-as]
+      - id: ruff
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
-  - repo: https://github.com/pycqa/flake8
-    rev: 6.0.0
-    hooks:
-      - id: flake8
-        args: ["--ignore=E203,E501,W503", "--max-complexity=10"]
-        additional_dependencies:
-          - flake8-bugbear
   - repo: https://github.com/pre-commit/mirrors-eslint
-    rev: v8.35.0
+    rev: v8.38.0
     hooks:
       - id: eslint
         args: [--fix]
         types_or: [css, scss, javascript]
         verbose: true
         additional_dependencies:
           - eslint
```

### Comparing `fh_fablib-1.0.20230303/fh_fablib/dotfiles/webpack.library.js` & `fh_fablib-1.0.20230411/fh_fablib/dotfiles/webpack.library.js`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20230303/fh_fablib/extract_js_gettext_strings.py` & `fh_fablib-1.0.20230411/fh_fablib/extract_js_gettext_strings.py`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20230303/fh_fablib.egg-info/PKG-INFO` & `fh_fablib-1.0.20230411/fh_fablib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fh-fablib
-Version: 1.0.20230303
+Version: 1.0.20230411
 Summary: fh-fablib
 Home-page: https://github.com/feinheit/fh-fablib/
 Author: Matthias Kestenholz
 Author-email: mk@feinheit.ch
 License: BSD-3-Clause
 Platform: OS Independent
 Classifier: License :: OSI Approved :: BSD License
@@ -28,15 +28,15 @@
 
 3. Add a ``fabfile.py`` to your project. A minimal example follows:
 
    .. code-block:: python
 
        import fh_fablib as fl
 
-       fl.require("1.0.20230303")
+       fl.require("1.0.20230411")
        fl.config.update(host="www-data@feinheit06.nine.ch")
 
        environments = [
            fl.environment(
                "production",
                {
                    "domain": "example.com",
@@ -104,15 +104,15 @@
 
 If you need multiple environments, add environment tasks as follows:
 
 .. code-block:: python
 
     import fh_fablib as fl
 
-    fl.require("1.0.20230303")
+    fl.require("1.0.20230411")
     fl.config.update(host="www-data@feinheit06.nine.ch")
 
     environments = [
         fl.environment(
             "production",
             {
                 "domain": "example.com",
```

### Comparing `fh_fablib-1.0.20230303/setup.cfg` & `fh_fablib-1.0.20230411/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fh_fablib
-version = 1.0.20230303
+version = 1.0.20230411
 description = fh-fablib
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/feinheit/fh-fablib/
 author = Matthias Kestenholz
 author_email = mk@feinheit.ch
 license = BSD-3-Clause
@@ -12,15 +12,15 @@
 platforms = OS Independent
 classifiers = 
 	License :: OSI Approved :: BSD License
 
 [options]
 packages = find:
 install_requires = 
-	fabric<2.7
+	fabric>=3
 	speckenv>=3.3
 python_requires = >=3.9
 include_package_data = True
 zip_safe = False
 
 [options.packages.find]
 exclude =
```

