# Comparing `tmp/gun_scraper-0.2.0.tar.gz` & `tmp/gun_scraper-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gun_scraper-0.2.0.tar", max compression
+gzip compressed data, was "gun_scraper-0.2.1.tar", max compression
```

## Comparing `gun_scraper-0.2.0.tar` & `gun_scraper-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1068 2023-02-02 19:39:32.967706 gun_scraper-0.2.0/LICENSE
--rw-r--r--   0        0        0     1755 2023-04-11 19:37:56.337374 gun_scraper-0.2.0/README.md
--rw-r--r--   0        0        0       85 2023-02-02 19:39:32.968466 gun_scraper-0.2.0/gun_scraper/__init__.py
--rw-r--r--   0        0        0     6123 2023-04-11 19:37:56.337651 gun_scraper-0.2.0/gun_scraper/__main__.py
--rw-r--r--   0        0        0     3663 2023-03-16 20:34:59.883041 gun_scraper-0.2.0/gun_scraper/file_io.py
--rw-r--r--   0        0        0     3780 2023-04-11 19:37:56.337897 gun_scraper-0.2.0/gun_scraper/notifier.py
--rw-r--r--   0        0        0       23 2023-02-02 19:39:32.969092 gun_scraper-0.2.0/gun_scraper/scrapers/__init__.py
--rw-r--r--   0        0        0     4888 2023-04-11 19:37:56.338092 gun_scraper-0.2.0/gun_scraper/scrapers/jaktmarken.py
--rw-r--r--   0        0        0     8056 2023-04-11 19:37:56.338334 gun_scraper-0.2.0/gun_scraper/scrapers/jg.py
--rw-r--r--   0        0        0     3245 2023-04-11 19:37:56.338564 gun_scraper-0.2.0/gun_scraper/scrapers/scraper_abc.py
--rw-r--r--   0        0        0     6290 2023-02-02 19:39:32.969557 gun_scraper-0.2.0/gun_scraper/scrapers/torsbo.py
--rw-r--r--   0        0        0      576 2023-02-02 19:39:32.969694 gun_scraper-0.2.0/gun_scraper/utils.py
--rw-r--r--   0        0        0     1773 2023-04-11 19:57:44.369710 gun_scraper-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2748 1970-01-01 00:00:00.000000 gun_scraper-0.2.0/setup.py
--rw-r--r--   0        0        0     2646 1970-01-01 00:00:00.000000 gun_scraper-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-02-02 19:39:32.967706 gun_scraper-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1755 2023-04-11 19:37:56.337374 gun_scraper-0.2.1/README.md
+-rw-r--r--   0        0        0       85 2023-04-11 20:32:55.117536 gun_scraper-0.2.1/gun_scraper/__init__.py
+-rw-r--r--   0        0        0     6123 2023-04-11 20:32:55.117802 gun_scraper-0.2.1/gun_scraper/__main__.py
+-rw-r--r--   0        0        0     3663 2023-03-16 20:34:59.883041 gun_scraper-0.2.1/gun_scraper/file_io.py
+-rw-r--r--   0        0        0     3780 2023-04-11 19:37:56.337897 gun_scraper-0.2.1/gun_scraper/notifier.py
+-rw-r--r--   0        0        0       23 2023-02-02 19:39:32.969092 gun_scraper-0.2.1/gun_scraper/scrapers/__init__.py
+-rw-r--r--   0        0        0     4853 2023-04-11 20:32:55.118077 gun_scraper-0.2.1/gun_scraper/scrapers/jaktmarken.py
+-rw-r--r--   0        0        0     8056 2023-04-11 19:37:56.338334 gun_scraper-0.2.1/gun_scraper/scrapers/jg.py
+-rw-r--r--   0        0        0     3245 2023-04-11 19:37:56.338564 gun_scraper-0.2.1/gun_scraper/scrapers/scraper_abc.py
+-rw-r--r--   0        0        0     6290 2023-02-02 19:39:32.969557 gun_scraper-0.2.1/gun_scraper/scrapers/torsbo.py
+-rw-r--r--   0        0        0      576 2023-02-02 19:39:32.969694 gun_scraper-0.2.1/gun_scraper/utils.py
+-rw-r--r--   0        0        0     1774 2023-04-11 20:33:15.920213 gun_scraper-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2748 1970-01-01 00:00:00.000000 gun_scraper-0.2.1/setup.py
+-rw-r--r--   0        0        0     2646 1970-01-01 00:00:00.000000 gun_scraper-0.2.1/PKG-INFO
```

### Comparing `gun_scraper-0.2.0/LICENSE` & `gun_scraper-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gun_scraper-0.2.0/README.md` & `gun_scraper-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `gun_scraper-0.2.0/gun_scraper/__main__.py` & `gun_scraper-0.2.1/gun_scraper/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
     if len(new_guns) > 0:
         send_gun_notification(new_guns, config_file_path)
         write_notification_timestamp_to_file(data_file)
     else:
         logger.info("No new guns found. No notification sent")
         # Check if alive notification should be sent
         check_latest_notification(
-            config["email"]["alive_msg_interval"], data_file, config_file_path
+            config["email"]["alive_msg_interval"], config_file_path, data_file
         )
 
     write_guns_to_file(scraped_guns, data_file)
 
     logger.info("GunScraper finished")
```

### Comparing `gun_scraper-0.2.0/gun_scraper/file_io.py` & `gun_scraper-0.2.1/gun_scraper/file_io.py`

 * *Files identical despite different names*

### Comparing `gun_scraper-0.2.0/gun_scraper/notifier.py` & `gun_scraper-0.2.1/gun_scraper/notifier.py`

 * *Files identical despite different names*

### Comparing `gun_scraper-0.2.0/gun_scraper/scrapers/jaktmarken.py` & `gun_scraper-0.2.1/gun_scraper/scrapers/jaktmarken.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,14 @@
         while next_page_url:
             result_page_soup = soup_from_url(next_page_url)
             logger.debug("Result page successfully retrieved")
 
             gun_tags = result_page_soup.find_all(
                 "li", class_="product-small product-small-vertical-small"
             )
-            logger.debug(gun_tags)
             for tag in gun_tags:
                 matching_guns.append(self._parse_gun_tag(tag))
 
             # Check if next page exists
             next_page_tag = result_page_soup.find("a", class_="button next")
             if next_page_tag:
                 next_page_url = self._base_url + next_page_tag["href"]
```

### Comparing `gun_scraper-0.2.0/gun_scraper/scrapers/jg.py` & `gun_scraper-0.2.1/gun_scraper/scrapers/jg.py`

 * *Files identical despite different names*

### Comparing `gun_scraper-0.2.0/gun_scraper/scrapers/scraper_abc.py` & `gun_scraper-0.2.1/gun_scraper/scrapers/scraper_abc.py`

 * *Files identical despite different names*

### Comparing `gun_scraper-0.2.0/gun_scraper/scrapers/torsbo.py` & `gun_scraper-0.2.1/gun_scraper/scrapers/torsbo.py`

 * *Files identical despite different names*

### Comparing `gun_scraper-0.2.0/gun_scraper/utils.py` & `gun_scraper-0.2.1/gun_scraper/utils.py`

 * *Files identical despite different names*

### Comparing `gun_scraper-0.2.0/pyproject.toml` & `gun_scraper-0.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gun-scraper"
-version = "0.2.0"
+version = "0.2.1"
 description = "A simple scraper for finding guns, according to search criteria, from Swedish gun shops"
 authors = ["Erik Persson <erik.ao.persson@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -44,19 +44,19 @@
 bumpver = "^2022.1120"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bumpver]
-current_version = "0.2.0"
+current_version = "0.2.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
-tag = true
+tag = false
 push = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
 "gun_scraper/__init__.py" = ["{version}"]
 
 [tool.pytest.ini_options]
```

### Comparing `gun_scraper-0.2.0/setup.py` & `gun_scraper-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'requests>=2.28.1,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['gun_scraper = gun_scraper.__main__:main']}
 
 setup_kwargs = {
     'name': 'gun-scraper',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'A simple scraper for finding guns, according to search criteria, from Swedish gun shops',
     'long_description': "# GunScraper\n\nA simple scraper for finding guns, according to search criteria, from Swedish gun shops.\n\nCurrently three shops are supported: \n\n* [Torsbo Handels](https://torsbohandels.com/) \n* [JG Jakt](https://www.jgjakt.se/)\n* [Jaktmarken.se/Marks Jakt och Fiskecenter](https://www.jaktmarken.se)\n\n## Setup\n\nIn order to install and setup GunScraper, follow the steps below:\n\n1. Create a virtual environment\n1. Install GunScraper and dependencies: `pip install gun_scraper`\n1. Download the configuration template `misc/config.yaml`\n1. Update the configuration\n1. Download `misc/runner.sh` and edit it with the path to the virtual environment\n  and config file\n1. Create a Cron Job to run `runner.sh` at desired interval\n\nExample Cron Job, running every 12th hour:\n```\n0 */12 * * * <path-to-repo>/GunScraper/runner.sh >/tmp/stdout.log 2>/tmp/stderr.log\n```\n\n## Config\n\nThe `config.yaml` follows the following syntax:\n\n```yaml\nscraper:\n  filters:\n    # Dictionary defining which filters to apply\n    caliber: # Possible values: 22lr, 22WMR or 308win\n    handedness: # Possible values: left\n  sites:\n    - # List defining which sites to scrape. Supported values: 'torsbo', 'jg' and 'jaktmarken'\n\nemail:\n  sender: # email address that will appear as sender of the notification emails\n  receiver: # email that will receive notification emails\n  smtp_server: # hostname of smtp server used to send notifications\n  ssl_port: # SSL port of the 'smtp_server'\n  username: # username for the 'smtp_server'\n  password: # password for the 'smtp_server'\n  alive_msg_interval: # interval (in hours) to send notification in case no guns matching search criteria is found\n\ndata_folder: # folder to store persistent data in\nlogs_folder: # folder to store log output in\n```",
     'author': 'Erik Persson',
     'author_email': 'erik.ao.persson@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/95ep/GunScraper',
```

### Comparing `gun_scraper-0.2.0/PKG-INFO` & `gun_scraper-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gun-scraper
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple scraper for finding guns, according to search criteria, from Swedish gun shops
 Home-page: https://github.com/95ep/GunScraper
 License: MIT
 Author: Erik Persson
 Author-email: erik.ao.persson@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

