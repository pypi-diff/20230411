# Comparing `tmp/twitscrape-0.0.5.tar.gz` & `tmp/twitscrape-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitscrape-0.0.5.tar", last modified: Tue Apr 11 08:29:11 2023, max compression
+gzip compressed data, was "twitscrape-0.0.6.tar", last modified: Tue Apr 11 08:41:44 2023, max compression
```

## Comparing `twitscrape-0.0.5.tar` & `twitscrape-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 christianharrison   (501) staff       (20)        0 2023-04-11 08:29:11.612889 twitscrape-0.0.5/
--rw-r--r--   0 christianharrison   (501) staff       (20)     1072 2023-04-03 16:06:06.000000 twitscrape-0.0.5/LICENSE
--rw-r--r--   0 christianharrison   (501) staff       (20)     1049 2023-04-11 08:29:11.612420 twitscrape-0.0.5/PKG-INFO
--rw-r--r--   0 christianharrison   (501) staff       (20)      451 2023-04-03 16:06:06.000000 twitscrape-0.0.5/README.md
--rw-r--r--   0 christianharrison   (501) staff       (20)      779 2023-04-11 08:29:02.000000 twitscrape-0.0.5/pyproject.toml
--rw-r--r--   0 christianharrison   (501) staff       (20)       38 2023-04-11 08:29:11.613045 twitscrape-0.0.5/setup.cfg
-drwxr-xr-x   0 christianharrison   (501) staff       (20)        0 2023-04-11 08:29:11.607505 twitscrape-0.0.5/tests/
--rw-r--r--   0 christianharrison   (501) staff       (20)      352 2023-04-03 18:49:58.000000 twitscrape-0.0.5/tests/test_twitter_scraper.py
-drwxr-xr-x   0 christianharrison   (501) staff       (20)        0 2023-04-11 08:29:11.608303 twitscrape-0.0.5/twitscrape/
--rw-r--r--   0 christianharrison   (501) staff       (20)        0 2023-04-03 16:06:06.000000 twitscrape-0.0.5/twitscrape/__init__.py
--rw-r--r--   0 christianharrison   (501) staff       (20)    10878 2023-04-11 08:24:54.000000 twitscrape-0.0.5/twitscrape/twitter_scraper.py
-drwxr-xr-x   0 christianharrison   (501) staff       (20)        0 2023-04-11 08:29:11.611480 twitscrape-0.0.5/twitscrape.egg-info/
--rw-r--r--   0 christianharrison   (501) staff       (20)     1049 2023-04-11 08:29:11.000000 twitscrape-0.0.5/twitscrape.egg-info/PKG-INFO
--rw-r--r--   0 christianharrison   (501) staff       (20)      284 2023-04-11 08:29:11.000000 twitscrape-0.0.5/twitscrape.egg-info/SOURCES.txt
--rw-r--r--   0 christianharrison   (501) staff       (20)        1 2023-04-11 08:29:11.000000 twitscrape-0.0.5/twitscrape.egg-info/dependency_links.txt
--rw-r--r--   0 christianharrison   (501) staff       (20)       60 2023-04-11 08:29:11.000000 twitscrape-0.0.5/twitscrape.egg-info/requires.txt
--rw-r--r--   0 christianharrison   (501) staff       (20)       11 2023-04-11 08:29:11.000000 twitscrape-0.0.5/twitscrape.egg-info/top_level.txt
+drwxr-xr-x   0 christianharrison   (501) staff       (20)        0 2023-04-11 08:41:44.629407 twitscrape-0.0.6/
+-rw-r--r--   0 christianharrison   (501) staff       (20)     1072 2023-04-03 16:06:06.000000 twitscrape-0.0.6/LICENSE
+-rw-r--r--   0 christianharrison   (501) staff       (20)     1049 2023-04-11 08:41:44.628887 twitscrape-0.0.6/PKG-INFO
+-rw-r--r--   0 christianharrison   (501) staff       (20)      451 2023-04-03 16:06:06.000000 twitscrape-0.0.6/README.md
+-rw-r--r--   0 christianharrison   (501) staff       (20)      779 2023-04-11 08:41:24.000000 twitscrape-0.0.6/pyproject.toml
+-rw-r--r--   0 christianharrison   (501) staff       (20)       38 2023-04-11 08:41:44.629548 twitscrape-0.0.6/setup.cfg
+drwxr-xr-x   0 christianharrison   (501) staff       (20)        0 2023-04-11 08:41:44.624182 twitscrape-0.0.6/tests/
+-rw-r--r--   0 christianharrison   (501) staff       (20)      352 2023-04-03 18:49:58.000000 twitscrape-0.0.6/tests/test_twitter_scraper.py
+drwxr-xr-x   0 christianharrison   (501) staff       (20)        0 2023-04-11 08:41:44.625585 twitscrape-0.0.6/twitscrape/
+-rw-r--r--   0 christianharrison   (501) staff       (20)        0 2023-04-03 16:06:06.000000 twitscrape-0.0.6/twitscrape/__init__.py
+-rw-r--r--   0 christianharrison   (501) staff       (20)    10883 2023-04-11 08:40:34.000000 twitscrape-0.0.6/twitscrape/twitter_scraper.py
+drwxr-xr-x   0 christianharrison   (501) staff       (20)        0 2023-04-11 08:41:44.628234 twitscrape-0.0.6/twitscrape.egg-info/
+-rw-r--r--   0 christianharrison   (501) staff       (20)     1049 2023-04-11 08:41:44.000000 twitscrape-0.0.6/twitscrape.egg-info/PKG-INFO
+-rw-r--r--   0 christianharrison   (501) staff       (20)      284 2023-04-11 08:41:44.000000 twitscrape-0.0.6/twitscrape.egg-info/SOURCES.txt
+-rw-r--r--   0 christianharrison   (501) staff       (20)        1 2023-04-11 08:41:44.000000 twitscrape-0.0.6/twitscrape.egg-info/dependency_links.txt
+-rw-r--r--   0 christianharrison   (501) staff       (20)       60 2023-04-11 08:41:44.000000 twitscrape-0.0.6/twitscrape.egg-info/requires.txt
+-rw-r--r--   0 christianharrison   (501) staff       (20)       11 2023-04-11 08:41:44.000000 twitscrape-0.0.6/twitscrape.egg-info/top_level.txt
```

### Comparing `twitscrape-0.0.5/LICENSE` & `twitscrape-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `twitscrape-0.0.5/PKG-INFO` & `twitscrape-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitscrape
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simple package using Selenium to scrape tweet data based on geolocation and datetime
 Author-email: Christian Harrison <christywastakenwastaken@gmail.com>
 Project-URL: Homepage, https://github.com/christywastaken/twitscrape
 Project-URL: Bug Tracker, https://github.com/christywastaken/twitscrape/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `twitscrape-0.0.5/pyproject.toml` & `twitscrape-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 67"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "twitscrape"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Christian Harrison", email="christywastakenwastaken@gmail.com" },
 ]
 description = "Simple package using Selenium to scrape tweet data based on geolocation and datetime"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `twitscrape-0.0.5/twitscrape/twitter_scraper.py` & `twitscrape-0.0.6/twitscrape/twitter_scraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
         last_height = 0
         # Loop until the document.body.scrollHeight no longer increases - end of page reached. 
         while True:
             try:
                 # Destructure output of get_tweets()
                 tweet_df, rate_lim_remaining, rate_lim_reset_time = self.get_tweets()
                 all_tweets_df = pd.concat([all_tweets_df, tweet_df], ignore_index=True)
-                print(f'remaining rate limit: {rate_lim_remaining} | tweets scraped: {len(tweet_df)}') #TODO: edit this for better readout. Make activity spinner?
+                print(f'remaining rate limit: {rate_lim_remaining} | tweets scraped: {len(all_tweets_df)}') #TODO: edit this for better readout. Make activity spinner?
                 
                 time.sleep(0.3) #TODO: Work out a better implementation for this timeout. The scrolling should happen when the page is ready, so it doesn't error.
                 self.driver.execute_script("window.scrollTo(0, document.body.scrollHeight)")
                 new_height = self.driver.execute_script("return document.body.scrollHeight")
 
                 if rate_lim_remaining < 5:
                     # If we are getting close to the rate limit, sleep the app until the rate-limit has reset.
```

### Comparing `twitscrape-0.0.5/twitscrape.egg-info/PKG-INFO` & `twitscrape-0.0.6/twitscrape.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitscrape
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simple package using Selenium to scrape tweet data based on geolocation and datetime
 Author-email: Christian Harrison <christywastakenwastaken@gmail.com>
 Project-URL: Homepage, https://github.com/christywastaken/twitscrape
 Project-URL: Bug Tracker, https://github.com/christywastaken/twitscrape/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

