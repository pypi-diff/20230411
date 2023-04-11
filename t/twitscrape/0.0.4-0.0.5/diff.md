# Comparing `tmp/twitscrape-0.0.4.tar.gz` & `tmp/twitscrape-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitscrape-0.0.4.tar", last modified: Tue Apr 11 08:00:35 2023, max compression
+gzip compressed data, was "twitscrape-0.0.5.tar", last modified: Tue Apr 11 08:29:11 2023, max compression
```

## Comparing `twitscrape-0.0.4.tar` & `twitscrape-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 christianharrison   (501) staff       (20)        0 2023-04-11 08:00:35.414732 twitscrape-0.0.4/
--rw-r--r--   0 christianharrison   (501) staff       (20)     1072 2023-04-03 16:06:06.000000 twitscrape-0.0.4/LICENSE
--rw-r--r--   0 christianharrison   (501) staff       (20)     1049 2023-04-11 08:00:35.414271 twitscrape-0.0.4/PKG-INFO
--rw-r--r--   0 christianharrison   (501) staff       (20)      451 2023-04-03 16:06:06.000000 twitscrape-0.0.4/README.md
--rw-r--r--   0 christianharrison   (501) staff       (20)      779 2023-04-11 08:00:00.000000 twitscrape-0.0.4/pyproject.toml
--rw-r--r--   0 christianharrison   (501) staff       (20)       38 2023-04-11 08:00:35.414871 twitscrape-0.0.4/setup.cfg
-drwxr-xr-x   0 christianharrison   (501) staff       (20)        0 2023-04-11 08:00:35.408810 twitscrape-0.0.4/tests/
--rw-r--r--   0 christianharrison   (501) staff       (20)      352 2023-04-03 18:49:58.000000 twitscrape-0.0.4/tests/test_twitter_scraper.py
-drwxr-xr-x   0 christianharrison   (501) staff       (20)        0 2023-04-11 08:00:35.410562 twitscrape-0.0.4/twitscrape/
--rw-r--r--   0 christianharrison   (501) staff       (20)        0 2023-04-03 16:06:06.000000 twitscrape-0.0.4/twitscrape/__init__.py
--rw-r--r--   0 christianharrison   (501) staff       (20)    11519 2023-04-11 07:58:13.000000 twitscrape-0.0.4/twitscrape/twitter_scraper.py
-drwxr-xr-x   0 christianharrison   (501) staff       (20)        0 2023-04-11 08:00:35.413542 twitscrape-0.0.4/twitscrape.egg-info/
--rw-r--r--   0 christianharrison   (501) staff       (20)     1049 2023-04-11 08:00:35.000000 twitscrape-0.0.4/twitscrape.egg-info/PKG-INFO
--rw-r--r--   0 christianharrison   (501) staff       (20)      284 2023-04-11 08:00:35.000000 twitscrape-0.0.4/twitscrape.egg-info/SOURCES.txt
--rw-r--r--   0 christianharrison   (501) staff       (20)        1 2023-04-11 08:00:35.000000 twitscrape-0.0.4/twitscrape.egg-info/dependency_links.txt
--rw-r--r--   0 christianharrison   (501) staff       (20)       60 2023-04-11 08:00:35.000000 twitscrape-0.0.4/twitscrape.egg-info/requires.txt
--rw-r--r--   0 christianharrison   (501) staff       (20)       11 2023-04-11 08:00:35.000000 twitscrape-0.0.4/twitscrape.egg-info/top_level.txt
+drwxr-xr-x   0 christianharrison   (501) staff       (20)        0 2023-04-11 08:29:11.612889 twitscrape-0.0.5/
+-rw-r--r--   0 christianharrison   (501) staff       (20)     1072 2023-04-03 16:06:06.000000 twitscrape-0.0.5/LICENSE
+-rw-r--r--   0 christianharrison   (501) staff       (20)     1049 2023-04-11 08:29:11.612420 twitscrape-0.0.5/PKG-INFO
+-rw-r--r--   0 christianharrison   (501) staff       (20)      451 2023-04-03 16:06:06.000000 twitscrape-0.0.5/README.md
+-rw-r--r--   0 christianharrison   (501) staff       (20)      779 2023-04-11 08:29:02.000000 twitscrape-0.0.5/pyproject.toml
+-rw-r--r--   0 christianharrison   (501) staff       (20)       38 2023-04-11 08:29:11.613045 twitscrape-0.0.5/setup.cfg
+drwxr-xr-x   0 christianharrison   (501) staff       (20)        0 2023-04-11 08:29:11.607505 twitscrape-0.0.5/tests/
+-rw-r--r--   0 christianharrison   (501) staff       (20)      352 2023-04-03 18:49:58.000000 twitscrape-0.0.5/tests/test_twitter_scraper.py
+drwxr-xr-x   0 christianharrison   (501) staff       (20)        0 2023-04-11 08:29:11.608303 twitscrape-0.0.5/twitscrape/
+-rw-r--r--   0 christianharrison   (501) staff       (20)        0 2023-04-03 16:06:06.000000 twitscrape-0.0.5/twitscrape/__init__.py
+-rw-r--r--   0 christianharrison   (501) staff       (20)    10878 2023-04-11 08:24:54.000000 twitscrape-0.0.5/twitscrape/twitter_scraper.py
+drwxr-xr-x   0 christianharrison   (501) staff       (20)        0 2023-04-11 08:29:11.611480 twitscrape-0.0.5/twitscrape.egg-info/
+-rw-r--r--   0 christianharrison   (501) staff       (20)     1049 2023-04-11 08:29:11.000000 twitscrape-0.0.5/twitscrape.egg-info/PKG-INFO
+-rw-r--r--   0 christianharrison   (501) staff       (20)      284 2023-04-11 08:29:11.000000 twitscrape-0.0.5/twitscrape.egg-info/SOURCES.txt
+-rw-r--r--   0 christianharrison   (501) staff       (20)        1 2023-04-11 08:29:11.000000 twitscrape-0.0.5/twitscrape.egg-info/dependency_links.txt
+-rw-r--r--   0 christianharrison   (501) staff       (20)       60 2023-04-11 08:29:11.000000 twitscrape-0.0.5/twitscrape.egg-info/requires.txt
+-rw-r--r--   0 christianharrison   (501) staff       (20)       11 2023-04-11 08:29:11.000000 twitscrape-0.0.5/twitscrape.egg-info/top_level.txt
```

### Comparing `twitscrape-0.0.4/LICENSE` & `twitscrape-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `twitscrape-0.0.4/PKG-INFO` & `twitscrape-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitscrape
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple package using Selenium to scrape tweet data based on geolocation and datetime
 Author-email: Christian Harrison <christywastakenwastaken@gmail.com>
 Project-URL: Homepage, https://github.com/christywastaken/twitscrape
 Project-URL: Bug Tracker, https://github.com/christywastaken/twitscrape/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `twitscrape-0.0.4/pyproject.toml` & `twitscrape-0.0.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 67"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "twitscrape"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Christian Harrison", email="christywastakenwastaken@gmail.com" },
 ]
 description = "Simple package using Selenium to scrape tweet data based on geolocation and datetime"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `twitscrape-0.0.4/twitscrape/twitter_scraper.py` & `twitscrape-0.0.5/twitscrape/twitter_scraper.py`

 * *Files 8% similar despite different names*

```diff
@@ -93,77 +93,66 @@
             # Decodes the byte data from the response
             body = decode(request.response.body, request.response.headers.get('Content-Encoding', 'identity')) 
             data = json.loads(body)
             tweets = data['globalObjects']['tweets']
             # Get rate limit info
             try:
                 rate_lim_remaining = int(request.response.headers.get('x-rate-limit-remaining'))
-            except KeyError as err:
+            except:
                 rate_lim_remaining = None
-                print(f'Error: {err}')
             try:
                 rate_lim_reset_time = int(request.response.headers.get('x-rate-limit-reset'))
-            except KeyError as err:
+            except:
                 rate_lim_reset_time = None
-                print(f'Error: {err}')
             for tweet_id, tweet_data in tweets.items():
                 try:
                     user_id = tweet_data['user_id']
-                except KeyError as err:
+                except:
                     user_id = None
-                    print(f'Error: {err}')
                 try:
                   created_at = tweet_data['created_at']
-                except KeyError as err:
+                except:
                     created_at = None
-                    print(f'Error: {err}')
                 try:
                     tweet_text = tweet_data['full_text']
-                except KeyError as err:
+                except:
                     tweet_text = None
-                    print(f'Error: {err}')
                 try:
                     hashtags_entity = tweet_data['entities']['hashtags']
                     if not hashtags_entity:
                         hashtags = None
                     else:
                         hashtags = '|'.join([x['text'] for x in hashtags_entity])
-                except KeyError as err:
+                except:
                     hashtags = None
-                    print(f'Error: {err}')
                 try:
                     media_entities = tweet_data['extended_entities']['media']
                     if not media_entities:
                       media_urls = None
                     else: 
                         media_urls = '|'.join([x['media_url'] for x in media_entities])
-                except KeyError as err:
+                except:
                     media_urls = None
-                    print(f'Error: {err}')
                 try:
                     retweet_count = tweet_data['retweet_count']
-                except KeyError as err:
+                except:
                     retweet_count = None
-                    print(f'Error: {err}')
                 try:
                     reply_count = tweet_data['reply_count']
-                except KeyError as err:
+                except:
                     reply_count = None
-                    print(f'Error: {err}')
-
                 try:
                     favorite_count = tweet_data['favorite_count']
-                except KeyError as err:
+                except:
                     favorite_count = None
-                    print(f'Error: {err}')
                 try:
                     views = tweet_data['ext_views']['count']
-                except KeyError as err:
+                except:
                     views = None
-                    print(f'Error: {err}')
+
                 
                 new_row_df = pd.DataFrame({'tweet_id': [tweet_id],
                                         'user_id': [user_id],
                                         'created_at': [created_at],
                                         'tweet_text': [tweet_text],
                                         'hashtags': [hashtags],
                                         'media_url': [media_urls],
```

### Comparing `twitscrape-0.0.4/twitscrape.egg-info/PKG-INFO` & `twitscrape-0.0.5/twitscrape.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitscrape
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple package using Selenium to scrape tweet data based on geolocation and datetime
 Author-email: Christian Harrison <christywastakenwastaken@gmail.com>
 Project-URL: Homepage, https://github.com/christywastaken/twitscrape
 Project-URL: Bug Tracker, https://github.com/christywastaken/twitscrape/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

