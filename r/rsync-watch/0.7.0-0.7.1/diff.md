# Comparing `tmp/rsync_watch-0.7.0.tar.gz` & `tmp/rsync_watch-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rsync_watch-0.7.0.tar", max compression
+gzip compressed data, was "rsync_watch-0.7.1.tar", max compression
```

## Comparing `rsync_watch-0.7.0.tar` & `rsync_watch-0.7.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2022-07-24 13:06:43.891140 rsync_watch-0.7.0/LICENSE
--rw-r--r--   0        0        0     5887 2022-08-22 16:12:46.595787 rsync_watch-0.7.0/README.rst
--rw-r--r--   0        0        0      946 2022-08-22 19:09:09.128565 rsync_watch-0.7.0/pyproject.toml
--rwxr-xr-x   0        0        0     7677 2022-08-22 19:08:04.997359 rsync_watch-0.7.0/rsync_watch/__init__.py
--rw-r--r--   0        0        0     2868 2022-08-22 06:53:27.545146 rsync_watch-0.7.0/rsync_watch/check.py
--rw-r--r--   0        0        0     2746 2022-08-22 15:32:02.583584 rsync_watch-0.7.0/rsync_watch/cli.py
--rw-r--r--   0        0        0     6872 1970-01-01 00:00:00.000000 rsync_watch-0.7.0/setup.py
--rw-r--r--   0        0        0     6762 1970-01-01 00:00:00.000000 rsync_watch-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-07-13 18:22:50.968095 rsync_watch-0.7.1/LICENSE
+-rw-r--r--   0        0        0     5887 2022-08-22 18:46:37.179391 rsync_watch-0.7.1/README.rst
+-rw-r--r--   0        0        0      966 2023-04-11 18:27:53.792883 rsync_watch-0.7.1/pyproject.toml
+-rwxr-xr-x   0        0        0     8075 2023-04-11 18:19:23.257908 rsync_watch-0.7.1/rsync_watch/__init__.py
+-rw-r--r--   0        0        0     2868 2022-08-22 05:59:42.466791 rsync_watch-0.7.1/rsync_watch/check.py
+-rw-r--r--   0        0        0     2746 2022-08-22 18:46:37.179391 rsync_watch-0.7.1/rsync_watch/cli.py
+-rw-r--r--   0        0        0     6872 1970-01-01 00:00:00.000000 rsync_watch-0.7.1/setup.py
+-rw-r--r--   0        0        0     6813 1970-01-01 00:00:00.000000 rsync_watch-0.7.1/PKG-INFO
```

### Comparing `rsync_watch-0.7.0/LICENSE` & `rsync_watch-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rsync_watch-0.7.0/README.rst` & `rsync_watch-0.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `rsync_watch-0.7.0/pyproject.toml` & `rsync_watch-0.7.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rsync_watch"
-version = "0.7.0"
+version = "0.7.1"
 description = "A Python script to monitor the execution of a rsync task."
 authors = ["Josef Friedrich <josef@friedrich.rocks>"]
 readme = "README.rst"
 license = "GPL-3.0-only"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
@@ -13,23 +13,24 @@
 repository = "https://github.com/Josef-Friedrich/rsync-watch"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 command-watcher = "^0.4.0"
 conf2levels = "^0.5.0"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = "^5.2"
 mypy = "^0.961"
 autopep8 = "^1.6.0"
 stdout-stderr-capturing = "^0.2.0"
 black = "^22.6.0"
 isort = "^5.10.1"
+tox = "^3.25.1"
 readme-patcher = "^0.6.0"
 # readme-patcher = { path = "../readme_patcher" }
 
 [build-system]
-requires = ["poetry>=1.2.0b2"]
+requires = ["poetry>=1.4.2"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry.scripts]
 "rsync-watch.py" = "rsync_watch:main"
```

### Comparing `rsync_watch-0.7.0/rsync_watch/__init__.py` & `rsync_watch-0.7.1/rsync_watch/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,109 +15,119 @@
 from .cli import ArgumentsDefault, __version__, get_argparser  # noqa: F401
 
 
 class StatsNotFoundError(CommandWatcherError):
     """Raised when some stats regex couldn’t be found in stdout."""
 
 
-def convert_stat_number_to_int(comma_integer: str) -> int:
-    """Convert a integer containing commas to a integer without commas.
+def convert_number_to_int(formatted_number: str) -> int:
+    """Convert a integer containing commas or dots to a integer without commas or dots.
 
-    :param comma_integer: a integer containing commas
+    :param comma_integer: a integer containing commas or dots
 
-    :return: A integer without commas
+    :return: A integer without commas or dots
     """
-    return int(comma_integer.replace(",", ""))
+
+    formatted_number = formatted_number.replace(",", "")
+    formatted_number = formatted_number.replace(".", "")
+
+    return int(formatted_number)
+
+
+def convert_number_to_float(formatted_number: str) -> float:
+    return float(formatted_number.replace(",", "."))
 
 
 def parse_stats(stdout: str) -> typing.Dict[str, typing.Union[int, float]]:
     """Parse the standard output of the rsync process.
 
+    https://github.com/WayneD/rsync/blob/c69dc7a5ab473bb52a575b5803026c2694761084/main.c#L416-L465
+
     :param stdout: The standard output of the rsync process
 
     :return: A dictionary containing all the stats numbers.
     """
     result: typing.Dict[str, typing.Union[int, float]] = {}
 
     def search(regex: str, exception_msg: str) -> int:
         match = re.search(regex, stdout)
         if match:
-            return convert_stat_number_to_int(match.group(1))
+            return convert_number_to_int(match.group(1))
         else:
             raise StatsNotFoundError(exception_msg)
 
     result["num_files"] = search(
-        r"\nNumber of files: ([\d,]*)",
+        r"\nNumber of files: ([\d,\.]*)",
         "Number of files: X,XXX (reg: X,XXX, dir: X,XXX)",
     )
 
     result["num_created_files"] = search(
-        r"\nNumber of created files: ([\d,]*)",
+        r"\nNumber of created files: ([\d,\.]*)",
         "Number of created files: X,XXX (reg: X,XXX, dir: X,XXX)",
     )
 
     # num_deleted_files
     # This line is sometimes missing on rsync --version 3.1.2
     # raise no error
-    match = re.search(r"\nNumber of deleted files: ([\d,]*)", stdout)
+    match = re.search(r"\nNumber of deleted files: ([\d,\.]*)", stdout)
     if match:
-        result["num_deleted_files"] = convert_stat_number_to_int(match.group(1))
+        result["num_deleted_files"] = convert_number_to_int(match.group(1))
     else:
         result["num_deleted_files"] = 0
 
     result["num_files_transferred"] = search(
-        r"\nNumber of regular files transferred: ([\d,]*)\n",
+        r"\nNumber of regular files transferred: ([\d,\.]*)\n",
         "Number of regular files transferred: X,XXX",
     )
 
     result["total_size"] = search(
-        r"\nTotal file size: ([\d,]*) bytes\n",
+        r"\nTotal file size: ([\d,\.]*) bytes\n",
         "Total file size: X,XXX bytes",
     )
 
     result["transferred_size"] = search(
-        r"\nTotal transferred file size: ([\d,]*) bytes\n",
+        r"\nTotal transferred file size: ([\d,\.]*) bytes\n",
         "Total transferred file size: X,XXX bytes",
     )
 
     result["literal_data"] = search(
-        r"\nLiteral data: ([\d,]*) bytes\n",
+        r"\nLiteral data: ([\d,\.]*) bytes\n",
         "Literal data: X,XXX bytes",
     )
 
     result["matched_data"] = search(
-        r"\nMatched data: ([\d,]*) bytes\n",
+        r"\nMatched data: ([\d,\.]*) bytes\n",
         "Matched data: X,XXX bytes",
     )
 
     result["list_size"] = search(
-        r"\nFile list size: ([\d,]*)\n", "File list size: X,XXX"
+        r"\nFile list size: ([\d,\.]*)\n", "File list size: X,XXX"
     )
 
     # list_generation_time
-    match = re.search(r"\nFile list generation time: ([\d\.]*) seconds\n", stdout)
+    match = re.search(r"\nFile list generation time: ([\d,\.]*) seconds\n", stdout)
     if match:
-        result["list_generation_time"] = float(match.group(1))
+        result["list_generation_time"] = convert_number_to_float(match.group(1))
     else:
         raise StatsNotFoundError("File list generation time: X.XXX seconds")
 
     # list_transfer_time
-    match = re.search(r"\nFile list transfer time: ([\d\.]*) seconds\n", stdout)
+    match = re.search(r"\nFile list transfer time: ([\d,\.]*) seconds\n", stdout)
     if match:
-        result["list_transfer_time"] = float(match.group(1))
+        result["list_transfer_time"] = convert_number_to_float(match.group(1))
     else:
         raise StatsNotFoundError("File list transfer time: X.XXX seconds")
 
     result["bytes_sent"] = search(
-        r"\nTotal bytes sent: ([\d,]*)\n",
+        r"\nTotal bytes sent: ([\d,\.]*)\n",
         "Total bytes sent: X,XXX",
     )
 
     result["bytes_received"] = search(
-        r"\nTotal bytes received: ([\d,]*)\n",
+        r"\nTotal bytes received: ([\d,\.]*)\n",
         "Total bytes received: X,XXX",
     )
 
     return result
 
 
 def format_service_name(host_name: str, src: str, dest: str) -> str:
```

### Comparing `rsync_watch-0.7.0/rsync_watch/check.py` & `rsync_watch-0.7.1/rsync_watch/check.py`

 * *Files identical despite different names*

### Comparing `rsync_watch-0.7.0/rsync_watch/cli.py` & `rsync_watch-0.7.1/rsync_watch/cli.py`

 * *Files identical despite different names*

### Comparing `rsync_watch-0.7.0/setup.py` & `rsync_watch-0.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['command-watcher>=0.4.0,<0.5.0', 'conf2levels>=0.5.0,<0.6.0']
 
 entry_points = \
 {'console_scripts': ['rsync-watch.py = rsync_watch:main']}
 
 setup_kwargs = {
     'name': 'rsync-watch',
-    'version': '0.7.0',
+    'version': '0.7.1',
     'description': 'A Python script to monitor the execution of a rsync task.',
     'long_description': '.. image:: http://img.shields.io/pypi/v/rsync-watch.svg\n    :target: https://pypi.org/project/rsync-watch\n    :alt: This package on the Python Package Index\n\n.. image:: https://github.com/Josef-Friedrich/rsync-watch/actions/workflows/tests.yml/badge.svg\n    :target: https://github.com/Josef-Friedrich/rsync-watch/actions/workflows/tests.yml\n    :alt: Tests\n\n.. image:: https://readthedocs.org/projects/rsync-watch/badge/?version=latest\n    :target: https://rsync-watch.readthedocs.io/en/latest/?badge=latest\n    :alt: Documentation Status\n\nrsync-watch.py\n==============\n\nA Python script to monitor the execution of a rsync task.\n\nFeatures\n--------\n\n-  The script ``rsync-watch.py`` parses the ``rsync --stats`` output and\n   sends this statistics to a monitoring system like Nagios or Icinga\n   using the NSCA protocol.\n\n-  The script ``rsync-watch.py`` can be configured to perform various\n   checks before starting the rsync process.\n\n:: \n\n    usage: rsync-watch.py [-h] [--host-name HOST_NAME]\n                          [--dest-user-group USER_GROUP_NAME] [--exclude EXCLUDE]\n                          [--rsync-args RSYNC_ARGS]\n                          [--action-check-failed {exception,skip}]\n                          [--check-file FILE_PATH] [--check-ping DESTINATION]\n                          [--check-ssh-login SSH_LOGIN] [-v]\n                          [--email-from-addr EMAIL_FROM_ADDR]\n                          [--email-to-addr EMAIL_TO_ADDR]\n                          [--email-to-addr-critical EMAIL_TO_ADDR_CRITICAL]\n                          [--email-smtp-login EMAIL_SMTP_LOGIN]\n                          [--email-smtp-password EMAIL_SMTP_PASSWORD]\n                          [--email-smtp-server EMAIL_SMTP_SERVER]\n                          [--nsca-remote-host NSCA_REMOTE_HOST]\n                          [--nsca-password NSCA_PASSWORD]\n                          [--nsca-encryption-method NSCA_ENCRYPTION_METHOD]\n                          [--nsca-port NSCA_PORT] [--icinga-url ICINGA_URL]\n                          [--icinga-user ICINGA_USER]\n                          [--icinga-password ICINGA_PASSWORD]\n                          [--beep-activated BEEP_ACTIVATED]\n                          src dest\n\n    A Python script to monitor the execution of a rsync task.\n\n    positional arguments:\n      src                   The source ([[USER@]HOST:]SRC)\n      dest                  The destination ([[USER@]HOST:]DEST)\n\n    options:\n      -h, --help            show this help message and exit\n      --host-name HOST_NAME\n                            The hostname to submit over NSCA to the monitoring.\n      --dest-user-group USER_GROUP_NAME\n                            Both the user name and the group name of the\n                            destination will be set to this name.\n      --exclude EXCLUDE     See the documention of --exclude in the rsync manual.\n      --rsync-args RSYNC_ARGS\n                            Rsync CLI arguments. Insert some rsync command line\n                            arguments. Wrap all arguments in one string, for\n                            example: --rsync-args \'--exclude "this folder"\'\n      -v, --version         show program\'s version number and exit\n\n    checks:\n      Perform different checks before running the rsync task.\n\n      --action-check-failed {exception,skip}\n                            Select action what to do when a check failed.\n      --check-file FILE_PATH\n                            Check if a file exists on the local machine.\n      --check-ping DESTINATION\n                            Check if a remote host is reachable by pinging.\n                            DESTINATION can a IP address or a host name or a full\n                            qualified host name.\n      --check-ssh-login SSH_LOGIN\n                            Check if a remote host is reachable over the network\n                            by SSHing into it. SSH_LOGIN: “root@192.168.1.1” or\n                            “root@example.com” or “example.com”.\n\n    email:\n      Generated by the config_reader.\n\n      --email-from-addr EMAIL_FROM_ADDR\n                            The email address of the sender.\n      --email-to-addr EMAIL_TO_ADDR\n                            The email address of the recipient.\n      --email-to-addr-critical EMAIL_TO_ADDR_CRITICAL\n                            The email address of the recipient to send critical\n                            messages to.\n      --email-smtp-login EMAIL_SMTP_LOGIN\n                            The SMTP login name.\n      --email-smtp-password EMAIL_SMTP_PASSWORD\n                            The SMTP password.\n      --email-smtp-server EMAIL_SMTP_SERVER\n                            The URL of the SMTP server, for example:\n                            `smtp.example.com:587`.\n\n    nsca:\n      Generated by the config_reader.\n\n      --nsca-remote-host NSCA_REMOTE_HOST\n                            The IP address of the NSCA remote host.\n      --nsca-password NSCA_PASSWORD\n                            The NSCA password.\n      --nsca-encryption-method NSCA_ENCRYPTION_METHOD\n                            The NSCA encryption method. The supported encryption\n                            methods are: 0 1 2 3 4 8 11 14 15 16\n      --nsca-port NSCA_PORT\n                            The NSCA port.\n\n    icinga:\n      Generated by the config_reader.\n\n      --icinga-url ICINGA_URL\n                            The HTTP URL. /v1/actions/process-check-result is\n                            appended.\n      --icinga-user ICINGA_USER\n                            The user for the HTTP authentification.\n      --icinga-password ICINGA_PASSWORD\n                            The password for the HTTP authentification.\n\n    beep:\n      Generated by the config_reader.\n\n      --beep-activated BEEP_ACTIVATED\n                            Activate the beep channel to report auditive messages.\n\n',
     'author': 'Josef Friedrich',
     'author_email': 'josef@friedrich.rocks',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Josef-Friedrich/rsync-watch',
```

### Comparing `rsync_watch-0.7.0/PKG-INFO` & `rsync_watch-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: rsync-watch
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Python script to monitor the execution of a rsync task.
 Home-page: https://github.com/Josef-Friedrich/rsync-watch
 License: GPL-3.0-only
 Author: Josef Friedrich
 Author-email: josef@friedrich.rocks
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: command-watcher (>=0.4.0,<0.5.0)
 Requires-Dist: conf2levels (>=0.5.0,<0.6.0)
 Project-URL: Repository, https://github.com/Josef-Friedrich/rsync-watch
 Description-Content-Type: text/x-rst
 
 .. image:: http://img.shields.io/pypi/v/rsync-watch.svg
```

