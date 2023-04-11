# Comparing `tmp/twitscrape-0.0.3.tar.gz` & `tmp/twitscrape-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitscrape-0.0.3.tar", last modified: Tue Apr  4 22:31:24 2023, max compression
+gzip compressed data, was "twitscrape-0.0.4.tar", last modified: Tue Apr 11 08:00:35 2023, max compression
```

## Comparing `twitscrape-0.0.3.tar` & `twitscrape-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 christianharrison   (501) staff       (20)        0 2023-04-04 22:31:24.885893 twitscrape-0.0.3/
--rw-r--r--   0 christianharrison   (501) staff       (20)     1072 2023-04-03 16:06:06.000000 twitscrape-0.0.3/LICENSE
--rw-r--r--   0 christianharrison   (501) staff       (20)     1049 2023-04-04 22:31:24.885455 twitscrape-0.0.3/PKG-INFO
--rw-r--r--   0 christianharrison   (501) staff       (20)      451 2023-04-03 16:06:06.000000 twitscrape-0.0.3/README.md
--rw-r--r--   0 christianharrison   (501) staff       (20)      779 2023-04-04 22:30:58.000000 twitscrape-0.0.3/pyproject.toml
--rw-r--r--   0 christianharrison   (501) staff       (20)       38 2023-04-04 22:31:24.885985 twitscrape-0.0.3/setup.cfg
-drwxr-xr-x   0 christianharrison   (501) staff       (20)        0 2023-04-04 22:31:24.880342 twitscrape-0.0.3/tests/
--rw-r--r--   0 christianharrison   (501) staff       (20)      352 2023-04-03 18:49:58.000000 twitscrape-0.0.3/tests/test_twitter_scraper.py
-drwxr-xr-x   0 christianharrison   (501) staff       (20)        0 2023-04-04 22:31:24.881680 twitscrape-0.0.3/twitscrape/
--rw-r--r--   0 christianharrison   (501) staff       (20)        0 2023-04-03 16:06:06.000000 twitscrape-0.0.3/twitscrape/__init__.py
--rw-r--r--   0 christianharrison   (501) staff       (20)    10594 2023-04-04 22:26:58.000000 twitscrape-0.0.3/twitscrape/twitter_scraper.py
-drwxr-xr-x   0 christianharrison   (501) staff       (20)        0 2023-04-04 22:31:24.884784 twitscrape-0.0.3/twitscrape.egg-info/
--rw-r--r--   0 christianharrison   (501) staff       (20)     1049 2023-04-04 22:31:24.000000 twitscrape-0.0.3/twitscrape.egg-info/PKG-INFO
--rw-r--r--   0 christianharrison   (501) staff       (20)      284 2023-04-04 22:31:24.000000 twitscrape-0.0.3/twitscrape.egg-info/SOURCES.txt
--rw-r--r--   0 christianharrison   (501) staff       (20)        1 2023-04-04 22:31:24.000000 twitscrape-0.0.3/twitscrape.egg-info/dependency_links.txt
--rw-r--r--   0 christianharrison   (501) staff       (20)       60 2023-04-04 22:31:24.000000 twitscrape-0.0.3/twitscrape.egg-info/requires.txt
--rw-r--r--   0 christianharrison   (501) staff       (20)       11 2023-04-04 22:31:24.000000 twitscrape-0.0.3/twitscrape.egg-info/top_level.txt
+drwxr-xr-x   0 christianharrison   (501) staff       (20)        0 2023-04-11 08:00:35.414732 twitscrape-0.0.4/
+-rw-r--r--   0 christianharrison   (501) staff       (20)     1072 2023-04-03 16:06:06.000000 twitscrape-0.0.4/LICENSE
+-rw-r--r--   0 christianharrison   (501) staff       (20)     1049 2023-04-11 08:00:35.414271 twitscrape-0.0.4/PKG-INFO
+-rw-r--r--   0 christianharrison   (501) staff       (20)      451 2023-04-03 16:06:06.000000 twitscrape-0.0.4/README.md
+-rw-r--r--   0 christianharrison   (501) staff       (20)      779 2023-04-11 08:00:00.000000 twitscrape-0.0.4/pyproject.toml
+-rw-r--r--   0 christianharrison   (501) staff       (20)       38 2023-04-11 08:00:35.414871 twitscrape-0.0.4/setup.cfg
+drwxr-xr-x   0 christianharrison   (501) staff       (20)        0 2023-04-11 08:00:35.408810 twitscrape-0.0.4/tests/
+-rw-r--r--   0 christianharrison   (501) staff       (20)      352 2023-04-03 18:49:58.000000 twitscrape-0.0.4/tests/test_twitter_scraper.py
+drwxr-xr-x   0 christianharrison   (501) staff       (20)        0 2023-04-11 08:00:35.410562 twitscrape-0.0.4/twitscrape/
+-rw-r--r--   0 christianharrison   (501) staff       (20)        0 2023-04-03 16:06:06.000000 twitscrape-0.0.4/twitscrape/__init__.py
+-rw-r--r--   0 christianharrison   (501) staff       (20)    11519 2023-04-11 07:58:13.000000 twitscrape-0.0.4/twitscrape/twitter_scraper.py
+drwxr-xr-x   0 christianharrison   (501) staff       (20)        0 2023-04-11 08:00:35.413542 twitscrape-0.0.4/twitscrape.egg-info/
+-rw-r--r--   0 christianharrison   (501) staff       (20)     1049 2023-04-11 08:00:35.000000 twitscrape-0.0.4/twitscrape.egg-info/PKG-INFO
+-rw-r--r--   0 christianharrison   (501) staff       (20)      284 2023-04-11 08:00:35.000000 twitscrape-0.0.4/twitscrape.egg-info/SOURCES.txt
+-rw-r--r--   0 christianharrison   (501) staff       (20)        1 2023-04-11 08:00:35.000000 twitscrape-0.0.4/twitscrape.egg-info/dependency_links.txt
+-rw-r--r--   0 christianharrison   (501) staff       (20)       60 2023-04-11 08:00:35.000000 twitscrape-0.0.4/twitscrape.egg-info/requires.txt
+-rw-r--r--   0 christianharrison   (501) staff       (20)       11 2023-04-11 08:00:35.000000 twitscrape-0.0.4/twitscrape.egg-info/top_level.txt
```

### Comparing `twitscrape-0.0.3/LICENSE` & `twitscrape-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `twitscrape-0.0.3/PKG-INFO` & `twitscrape-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitscrape
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple package using Selenium to scrape tweet data based on geolocation and datetime
 Author-email: Christian Harrison <christywastakenwastaken@gmail.com>
 Project-URL: Homepage, https://github.com/christywastaken/twitscrape
 Project-URL: Bug Tracker, https://github.com/christywastaken/twitscrape/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `twitscrape-0.0.3/pyproject.toml` & `twitscrape-0.0.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 67"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "twitscrape"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Christian Harrison", email="christywastakenwastaken@gmail.com" },
 ]
 description = "Simple package using Selenium to scrape tweet data based on geolocation and datetime"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `twitscrape-0.0.3/twitscrape/twitter_scraper.py` & `twitscrape-0.0.4/twitscrape/twitter_scraper.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,15 +43,15 @@
           
         # Use ChromeDriverManager().install() to update driver for browser.
         print('-- TwitterGeolocationScraper running. This may take a minute to update the webdriver. --')
         self.driver = webdriver.Chrome(service=Service(ChromeDriverManager().install()), options=options)
         # Narrows the scope of to requests containing 'adaptive' (the requests containing tweets)
         self.driver.scopes= ['.*adaptive.*']
         # Tweet_df_model
-        self.tweet_df_schema = pd.DataFrame(columns=['tweet_id', 'created_at', 'tweet_text', 'hashtags', 'media_url', 'retweet_count', 'favourite_count', 'reply_count', 'views'])
+        self.tweet_df_schema = pd.DataFrame(columns=['tweet_id', 'user_id', 'created_at', 'tweet_text', 'hashtags', 'media_url', 'retweet_count', 'favourite_count', 'reply_count', 'views'])
       
 
 
 
     def create_twitter_url(self) -> str:
         # As default it uses Central Newcastle-Upon-Tyne with 10km radius, filters links and replies, sorted by latest. Start_date & end_date: current date.
         today = datetime.utcnow()
@@ -93,74 +93,90 @@
             # Decodes the byte data from the response
             body = decode(request.response.body, request.response.headers.get('Content-Encoding', 'identity')) 
             data = json.loads(body)
             tweets = data['globalObjects']['tweets']
             # Get rate limit info
             try:
                 rate_lim_remaining = int(request.response.headers.get('x-rate-limit-remaining'))
-            except:
+            except KeyError as err:
                 rate_lim_remaining = None
+                print(f'Error: {err}')
             try:
                 rate_lim_reset_time = int(request.response.headers.get('x-rate-limit-reset'))
-            except:
+            except KeyError as err:
                 rate_lim_reset_time = None
-
+                print(f'Error: {err}')
             for tweet_id, tweet_data in tweets.items():
-              try:
+                try:
+                    user_id = tweet_data['user_id']
+                except KeyError as err:
+                    user_id = None
+                    print(f'Error: {err}')
+                try:
                   created_at = tweet_data['created_at']
-              except:
-                  created_at = None
-              try:
-                  tweet_text = tweet_data['full_text']
-              except:
-                  tweet_text = None
-              try:
-                  hashtags_entity = tweet_data['entities']['hashtags']
-                  if not hashtags_entity:
-                      hashtags = None
-                  else:
-                      hashtags = '|'.join([x['text'] for x in hashtags_entity])
-              except:
-                  hashtags = None
-              try:
-                  media_entities = tweet_data['extended_entities']['media']
-                  if not media_entities:
+                except KeyError as err:
+                    created_at = None
+                    print(f'Error: {err}')
+                try:
+                    tweet_text = tweet_data['full_text']
+                except KeyError as err:
+                    tweet_text = None
+                    print(f'Error: {err}')
+                try:
+                    hashtags_entity = tweet_data['entities']['hashtags']
+                    if not hashtags_entity:
+                        hashtags = None
+                    else:
+                        hashtags = '|'.join([x['text'] for x in hashtags_entity])
+                except KeyError as err:
+                    hashtags = None
+                    print(f'Error: {err}')
+                try:
+                    media_entities = tweet_data['extended_entities']['media']
+                    if not media_entities:
                       media_urls = None
-                  else: 
-                      media_urls = '|'.join([x['media_url'] for x in media_entities])
-              except:
-                  media_urls = None
-              try:
-                  retweet_count = tweet_data['retweet_count']
-              except:
-                  retweet_count = None
-              try:
-                  reply_count = tweet_data['reply_count']
-              except:
-                  reply_count = None
-              try:
-                  favorite_count = tweet_data['favorite_count']
-              except:
-                  favorite_count = None
-              try:
-                  views = tweet_data['ext_views']['count']
-              except:
-                  views = None
+                    else: 
+                        media_urls = '|'.join([x['media_url'] for x in media_entities])
+                except KeyError as err:
+                    media_urls = None
+                    print(f'Error: {err}')
+                try:
+                    retweet_count = tweet_data['retweet_count']
+                except KeyError as err:
+                    retweet_count = None
+                    print(f'Error: {err}')
+                try:
+                    reply_count = tweet_data['reply_count']
+                except KeyError as err:
+                    reply_count = None
+                    print(f'Error: {err}')
+
+                try:
+                    favorite_count = tweet_data['favorite_count']
+                except KeyError as err:
+                    favorite_count = None
+                    print(f'Error: {err}')
+                try:
+                    views = tweet_data['ext_views']['count']
+                except KeyError as err:
+                    views = None
+                    print(f'Error: {err}')
                 
-              new_row_df = pd.DataFrame({'tweet_id': [tweet_id], 
+                new_row_df = pd.DataFrame({'tweet_id': [tweet_id],
+                                        'user_id': [user_id],
                                         'created_at': [created_at],
                                         'tweet_text': [tweet_text],
                                         'hashtags': [hashtags],
                                         'media_url': [media_urls],
                                         'retweet_count': [retweet_count],
                                         'reply_count': [reply_count],
                                         'favourite_count': [favorite_count],
                                         'views': [views]})
               
-              tweet_df = pd.concat([tweet_df, new_row_df], ignore_index=True)
+                tweet_df = pd.concat([tweet_df, new_row_df], ignore_index=True)
         except Exception as err:
             print(f'-- Error: {err} --')
         tweet_df.sort_values(by='created_at', ascending=False, inplace=True)
         # Deletes driver.requests so get_tweets() waits for the new request response 
         del self.driver.requests
         return (tweet_df, rate_lim_remaining, rate_lim_reset_time)
```

### Comparing `twitscrape-0.0.3/twitscrape.egg-info/PKG-INFO` & `twitscrape-0.0.4/twitscrape.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitscrape
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple package using Selenium to scrape tweet data based on geolocation and datetime
 Author-email: Christian Harrison <christywastakenwastaken@gmail.com>
 Project-URL: Homepage, https://github.com/christywastaken/twitscrape
 Project-URL: Bug Tracker, https://github.com/christywastaken/twitscrape/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

