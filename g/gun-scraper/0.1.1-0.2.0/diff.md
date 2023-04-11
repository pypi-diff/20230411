# Comparing `tmp/gun-scraper-0.1.1.tar.gz` & `tmp/gun_scraper-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gun-scraper-0.1.1.tar", last modified: Sun Oct 30 15:30:22 2022, max compression
+gzip compressed data, was "gun_scraper-0.2.0.tar", max compression
```

## Comparing `gun-scraper-0.1.1.tar` & `gun_scraper-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,15 @@
-drwxr-xr-x   0 erikpersson   (501) staff       (20)        0 2022-10-30 15:30:22.143821 gun-scraper-0.1.1/
--rw-r--r--   0 erikpersson   (501) staff       (20)     1068 2022-05-16 19:55:26.000000 gun-scraper-0.1.1/LICENSE
--rw-r--r--   0 erikpersson   (501) staff       (20)     3404 2022-10-30 15:30:22.143985 gun-scraper-0.1.1/PKG-INFO
--rw-r--r--   0 erikpersson   (501) staff       (20)     1628 2022-10-30 15:27:51.000000 gun-scraper-0.1.1/README.md
--rw-r--r--   0 erikpersson   (501) staff       (20)     1069 2022-10-30 15:28:35.000000 gun-scraper-0.1.1/pyproject.toml
--rw-r--r--   0 erikpersson   (501) staff       (20)      186 2022-10-30 15:30:22.147818 gun-scraper-0.1.1/setup.cfg
-drwxr-xr-x   0 erikpersson   (501) staff       (20)        0 2022-10-30 15:30:22.004459 gun-scraper-0.1.1/src/
-drwxr-xr-x   0 erikpersson   (501) staff       (20)        0 2022-10-30 15:30:22.132313 gun-scraper-0.1.1/src/gun_scraper/
--rw-r--r--   0 erikpersson   (501) staff       (20)       85 2022-10-30 15:28:35.000000 gun-scraper-0.1.1/src/gun_scraper/__init__.py
--rw-r--r--   0 erikpersson   (501) staff       (20)     4846 2022-10-30 11:56:29.000000 gun-scraper-0.1.1/src/gun_scraper/__main__.py
--rw-r--r--   0 erikpersson   (501) staff       (20)     3683 2022-10-30 11:56:29.000000 gun-scraper-0.1.1/src/gun_scraper/file_io.py
--rw-r--r--   0 erikpersson   (501) staff       (20)     3742 2022-10-30 11:56:29.000000 gun-scraper-0.1.1/src/gun_scraper/notifier.py
-drwxr-xr-x   0 erikpersson   (501) staff       (20)        0 2022-10-30 15:30:22.142858 gun-scraper-0.1.1/src/gun_scraper/scrapers/
--rw-r--r--   0 erikpersson   (501) staff       (20)       23 2022-10-30 11:56:29.000000 gun-scraper-0.1.1/src/gun_scraper/scrapers/__init__.py
--rw-r--r--   0 erikpersson   (501) staff       (20)     8825 2022-10-30 11:56:29.000000 gun-scraper-0.1.1/src/gun_scraper/scrapers/jg.py
--rw-r--r--   0 erikpersson   (501) staff       (20)     1446 2022-10-30 11:56:29.000000 gun-scraper-0.1.1/src/gun_scraper/scrapers/scraper_abc.py
--rw-r--r--   0 erikpersson   (501) staff       (20)     6290 2022-10-30 11:56:29.000000 gun-scraper-0.1.1/src/gun_scraper/scrapers/torsbo.py
--rw-r--r--   0 erikpersson   (501) staff       (20)      576 2022-10-30 11:56:29.000000 gun-scraper-0.1.1/src/gun_scraper/utils.py
-drwxr-xr-x   0 erikpersson   (501) staff       (20)        0 2022-10-30 15:30:22.139623 gun-scraper-0.1.1/src/gun_scraper.egg-info/
--rw-r--r--   0 erikpersson   (501) staff       (20)     3404 2022-10-30 15:30:21.000000 gun-scraper-0.1.1/src/gun_scraper.egg-info/PKG-INFO
--rw-r--r--   0 erikpersson   (501) staff       (20)      557 2022-10-30 15:30:21.000000 gun-scraper-0.1.1/src/gun_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 erikpersson   (501) staff       (20)        1 2022-10-30 15:30:21.000000 gun-scraper-0.1.1/src/gun_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 erikpersson   (501) staff       (20)       58 2022-10-30 15:30:21.000000 gun-scraper-0.1.1/src/gun_scraper.egg-info/entry_points.txt
--rw-r--r--   0 erikpersson   (501) staff       (20)       66 2022-10-30 15:30:21.000000 gun-scraper-0.1.1/src/gun_scraper.egg-info/requires.txt
--rw-r--r--   0 erikpersson   (501) staff       (20)       12 2022-10-30 15:30:21.000000 gun-scraper-0.1.1/src/gun_scraper.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1068 2023-02-02 19:39:32.967706 gun_scraper-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1755 2023-04-11 19:37:56.337374 gun_scraper-0.2.0/README.md
+-rw-r--r--   0        0        0       85 2023-02-02 19:39:32.968466 gun_scraper-0.2.0/gun_scraper/__init__.py
+-rw-r--r--   0        0        0     6123 2023-04-11 19:37:56.337651 gun_scraper-0.2.0/gun_scraper/__main__.py
+-rw-r--r--   0        0        0     3663 2023-03-16 20:34:59.883041 gun_scraper-0.2.0/gun_scraper/file_io.py
+-rw-r--r--   0        0        0     3780 2023-04-11 19:37:56.337897 gun_scraper-0.2.0/gun_scraper/notifier.py
+-rw-r--r--   0        0        0       23 2023-02-02 19:39:32.969092 gun_scraper-0.2.0/gun_scraper/scrapers/__init__.py
+-rw-r--r--   0        0        0     4888 2023-04-11 19:37:56.338092 gun_scraper-0.2.0/gun_scraper/scrapers/jaktmarken.py
+-rw-r--r--   0        0        0     8056 2023-04-11 19:37:56.338334 gun_scraper-0.2.0/gun_scraper/scrapers/jg.py
+-rw-r--r--   0        0        0     3245 2023-04-11 19:37:56.338564 gun_scraper-0.2.0/gun_scraper/scrapers/scraper_abc.py
+-rw-r--r--   0        0        0     6290 2023-02-02 19:39:32.969557 gun_scraper-0.2.0/gun_scraper/scrapers/torsbo.py
+-rw-r--r--   0        0        0      576 2023-02-02 19:39:32.969694 gun_scraper-0.2.0/gun_scraper/utils.py
+-rw-r--r--   0        0        0     1773 2023-04-11 19:57:44.369710 gun_scraper-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2748 1970-01-01 00:00:00.000000 gun_scraper-0.2.0/setup.py
+-rw-r--r--   0        0        0     2646 1970-01-01 00:00:00.000000 gun_scraper-0.2.0/PKG-INFO
```

### Comparing `gun-scraper-0.1.1/LICENSE` & `gun_scraper-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gun-scraper-0.1.1/README.md` & `gun_scraper-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,50 @@
+Metadata-Version: 2.1
+Name: gun-scraper
+Version: 0.2.0
+Summary: A simple scraper for finding guns, according to search criteria, from Swedish gun shops
+Home-page: https://github.com/95ep/GunScraper
+License: MIT
+Author: Erik Persson
+Author-email: erik.ao.persson@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
+Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Description-Content-Type: text/markdown
+
 # GunScraper
 
 A simple scraper for finding guns, according to search criteria, from Swedish gun shops.
 
-Currently two shops are supported: [Torsbo Handels](https://torsbohandels.com/) and [JG Jakt](https://www.jgjakt.se/).
+Currently three shops are supported: 
+
+* [Torsbo Handels](https://torsbohandels.com/) 
+* [JG Jakt](https://www.jgjakt.se/)
+* [Jaktmarken.se/Marks Jakt och Fiskecenter](https://www.jaktmarken.se)
 
 ## Setup
 
 In order to install and setup GunScraper, follow the steps below:
 
 1. Create a virtual environment
-1. Install GunScraper: `pip install gun_scraper`
-1. Download `misc/runner.sh` and edit it with the path to the virtual environment
-1. Download the configuration template `misc/config.yaml` and place it in the same folder as `runner.sh`
+1. Install GunScraper and dependencies: `pip install gun_scraper`
+1. Download the configuration template `misc/config.yaml`
 1. Update the configuration
+1. Download `misc/runner.sh` and edit it with the path to the virtual environment
+  and config file
 1. Create a Cron Job to run `runner.sh` at desired interval
 
 Example Cron Job, running every 12th hour:
 ```
 0 */12 * * * <path-to-repo>/GunScraper/runner.sh >/tmp/stdout.log 2>/tmp/stderr.log
 ```
 
@@ -27,20 +55,21 @@
 ```yaml
 scraper:
   filters:
     # Dictionary defining which filters to apply
     caliber: # Possible values: 22lr, 22WMR or 308win
     handedness: # Possible values: left
   sites:
-    - # List defining which sites to scrape. Supported values: torsbo and jg
+    - # List defining which sites to scrape. Supported values: 'torsbo', 'jg' and 'jaktmarken'
 
 email:
   sender: # email address that will appear as sender of the notification emails
   receiver: # email that will receive notification emails
   smtp_server: # hostname of smtp server used to send notifications
   ssl_port: # SSL port of the 'smtp_server'
   username: # username for the 'smtp_server'
   password: # password for the 'smtp_server'
   alive_msg_interval: # interval (in hours) to send notification in case no guns matching search criteria is found
 
 data_folder: # folder to store persistent data in
-```
+logs_folder: # folder to store log output in
+```
```

### Comparing `gun-scraper-0.1.1/src/gun_scraper/file_io.py` & `gun_scraper-0.2.0/gun_scraper/file_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Module collecting functions for file I/O."""
 import json
 from pathlib import Path
-import time
+from time import time
 from typing import Dict, List
 
 from loguru import logger
 
 INDENT_LEVEL = 4
 
 
@@ -30,28 +30,28 @@
 
     Raises:
         GunScraperFileIOError: if the parent folder of the 'data_file' doesn't exist
 
     Returns:
         Dict: Content of the data file, or empty dict if it doesn't exist
     """
-    if data_file.exists():
-        logger.debug(f"Data file {data_file} exists")
-        with open(data_file) as fp:
-            data_content = json.load(fp)
-        logger.debug(f"The following content loaded from file: {data_content}")
-        return data_content
-    else:
+    if not data_file.exists():
         logger.warning(f"Data file {data_file} doesn't exist.")
         if not data_file.parent.is_dir():
             raise GunScraperFileIOError(
                 f"data_folder from config doesn't exist: {data_file.parent}"
             )
         return {}
 
+    logger.debug(f"Data file {data_file} exists")
+    with open(data_file) as fp:
+        data_content = json.load(fp)
+    logger.debug(f"The following content loaded from file: {data_content}")
+    return data_content
+
 
 def read_guns_from_file(data_file: Path) -> List[Dict]:
     """Read the guns stored in the data file.
 
     Args:
         data_file (Path): Path to file holding previously scraped guns
 
@@ -108,14 +108,14 @@
     """Write timestamp of latest notification to file.
 
     Args:
         data_file (Path): path to file holding scraped guns
     """
     data_content = load_data_file(data_file)
 
-    timestamp = time.time()
+    timestamp = time()
     logger.debug(f"Writing the following timestamp to file: {timestamp}")
     data_content["latest_notification_timestamp"] = timestamp
 
     with open(data_file, "w") as fp:
         logger.debug(f"New data file content: {data_content}")
         json.dump(data_content, fp, indent=INDENT_LEVEL)
```

### Comparing `gun-scraper-0.1.1/src/gun_scraper/notifier.py` & `gun_scraper-0.2.0/gun_scraper/notifier.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 from typing import Dict, List
 
 
 from loguru import logger
 import yaml
 
 
-def send_gun_notification(guns_list: List[Dict]):
+def send_gun_notification(guns_list: List[Dict], config_file: Path):
     """Take the list of guns and send an email notification.
 
     Args:
         guns_list (List[Dict]): List of matching guns
+        config_file: path to config file
     """
     logger.info("Sending notification for new guns")
     # Read config file with config for sending emails
-    config_file_path = Path("config.yaml")
-    with open(config_file_path) as f:
+    with open(config_file) as f:
         config = yaml.safe_load(f)
     email_config = config["email"]
     logger.debug(f"The following email config is read: {email_config}")
 
     email_body = "The following guns were found: \n"
     for gun in guns_list:
         email_body += (
@@ -45,20 +45,23 @@
         email_config["smtp_server"],
         email_config["ssl_port"],
         email_config["username"],
         email_config["password"],
     )
 
 
-def send_alive_notification():
-    """Send email notifying subscriber that the scraper is still alive."""
+def send_alive_notification(config_file: Path):
+    """Send email notifying subscriber that the scraper is still alive.
+
+    Args:
+        config_file: path to config file
+    """
     logger.info("Sending alive notification")
     # Read config file and extract config for sending emails
-    config_file_path = Path("config.yaml")
-    with open(config_file_path) as f:
+    with open(config_file) as f:
         config = yaml.safe_load(f)
     email_config = config["email"]
     logger.debug(f"The following email config is read: {email_config}")
 
     email_body = "No new gun matching the filter found, but I'm still looking!"
     message = MIMEText(email_body, "plain")  # TODO - use multipart and add HTML
     message["Subject"] = "GunScraper: No new guns found"
```

### Comparing `gun-scraper-0.1.1/src/gun_scraper/scrapers/jg.py` & `gun_scraper-0.2.0/gun_scraper/scrapers/jg.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 from gun_scraper.scrapers.scraper_abc import GunScraperABC
 from gun_scraper.utils import soup_from_url
 
 
 class JGScraperError(Exception):
-    """Exception to raise when something goes wrong in the JG module."""
+    """Exception to raise when something goes wrong in the JG scraper."""
 
     def __init__(self, message) -> None:
         """Create the error instance and log the error message.
 
         Args:
             message (str): the error message to log
         """
@@ -30,15 +30,15 @@
         "22lr": "22lr-56x15r",
         "22WMR": "22-wmr-56x26r",
         "308win": "308-win-762x51",
     }
     supported_handedness = {"left": "vänster"}
 
     def __init__(self, filter_input: Dict[str, str]):
-        """Initialize a scraper object for Torsbo.
+        """Initialize a scraper object for JG.
 
         Args:
             filter_input (Dict[str, str]): filter settings from config
         """
         logger.debug(f"Creating JGGunScraper object with filter input {filter_input}")
         self.handedness = None
         self.caliber = None
@@ -106,34 +106,14 @@
             else:
                 logger.debug(
                     f"The following gun doesn't match the handedness filter:\n{gun}"
                 )
 
         return guns_matching_handedness
 
-    def _parse_filters(self, filter_input: Dict[str, str]):
-        """Parse the filter input.
-
-        Args:
-            filter_input (Dict[str, str]): filter settings from config
-
-        Raises:
-            JGScraperError: if an unsupported filter key is included
-                in the input
-        """
-        logger.debug(f"Parsing filters: {filter_input}")
-        for filter_key, filter_value in filter_input.items():
-            if filter_key == "handedness":
-                self._set_handedness_filter(filter_value)
-            elif filter_key == "caliber":
-                self._set_caliber_filter(filter_value)
-            else:
-                raise JGScraperError(f"Filter type '{filter_key}' not supported!")
-        logger.debug("Filters parsed")
-
     def _build_url(self) -> None:
         """Build the query url."""
         self.query_url = self._base_url
         url_filters = []
         if self.caliber:
             url_filters.append(f"pa_kaliber={self.caliber}")
```

### Comparing `gun-scraper-0.1.1/src/gun_scraper/scrapers/torsbo.py` & `gun_scraper-0.2.0/gun_scraper/scrapers/torsbo.py`

 * *Files identical despite different names*

### Comparing `gun-scraper-0.1.1/src/gun_scraper/utils.py` & `gun_scraper-0.2.0/gun_scraper/utils.py`

 * *Files identical despite different names*

