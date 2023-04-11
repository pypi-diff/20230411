# Comparing `tmp/twitscrape-0.0.6.tar.gz` & `tmp/twitscrape-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitscrape-0.0.6.tar", last modified: Tue Apr 11 08:41:44 2023, max compression
+gzip compressed data, was "twitscrape-0.0.7.tar", last modified: Tue Apr 11 18:32:03 2023, max compression
```

## Comparing `twitscrape-0.0.6.tar` & `twitscrape-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 christianharrison   (501) staff       (20)        0 2023-04-11 08:41:44.629407 twitscrape-0.0.6/
--rw-r--r--   0 christianharrison   (501) staff       (20)     1072 2023-04-03 16:06:06.000000 twitscrape-0.0.6/LICENSE
--rw-r--r--   0 christianharrison   (501) staff       (20)     1049 2023-04-11 08:41:44.628887 twitscrape-0.0.6/PKG-INFO
--rw-r--r--   0 christianharrison   (501) staff       (20)      451 2023-04-03 16:06:06.000000 twitscrape-0.0.6/README.md
--rw-r--r--   0 christianharrison   (501) staff       (20)      779 2023-04-11 08:41:24.000000 twitscrape-0.0.6/pyproject.toml
--rw-r--r--   0 christianharrison   (501) staff       (20)       38 2023-04-11 08:41:44.629548 twitscrape-0.0.6/setup.cfg
-drwxr-xr-x   0 christianharrison   (501) staff       (20)        0 2023-04-11 08:41:44.624182 twitscrape-0.0.6/tests/
--rw-r--r--   0 christianharrison   (501) staff       (20)      352 2023-04-03 18:49:58.000000 twitscrape-0.0.6/tests/test_twitter_scraper.py
-drwxr-xr-x   0 christianharrison   (501) staff       (20)        0 2023-04-11 08:41:44.625585 twitscrape-0.0.6/twitscrape/
--rw-r--r--   0 christianharrison   (501) staff       (20)        0 2023-04-03 16:06:06.000000 twitscrape-0.0.6/twitscrape/__init__.py
--rw-r--r--   0 christianharrison   (501) staff       (20)    10883 2023-04-11 08:40:34.000000 twitscrape-0.0.6/twitscrape/twitter_scraper.py
-drwxr-xr-x   0 christianharrison   (501) staff       (20)        0 2023-04-11 08:41:44.628234 twitscrape-0.0.6/twitscrape.egg-info/
--rw-r--r--   0 christianharrison   (501) staff       (20)     1049 2023-04-11 08:41:44.000000 twitscrape-0.0.6/twitscrape.egg-info/PKG-INFO
--rw-r--r--   0 christianharrison   (501) staff       (20)      284 2023-04-11 08:41:44.000000 twitscrape-0.0.6/twitscrape.egg-info/SOURCES.txt
--rw-r--r--   0 christianharrison   (501) staff       (20)        1 2023-04-11 08:41:44.000000 twitscrape-0.0.6/twitscrape.egg-info/dependency_links.txt
--rw-r--r--   0 christianharrison   (501) staff       (20)       60 2023-04-11 08:41:44.000000 twitscrape-0.0.6/twitscrape.egg-info/requires.txt
--rw-r--r--   0 christianharrison   (501) staff       (20)       11 2023-04-11 08:41:44.000000 twitscrape-0.0.6/twitscrape.egg-info/top_level.txt
+drwxr-xr-x   0 christianharrison   (501) staff       (20)        0 2023-04-11 18:32:03.684852 twitscrape-0.0.7/
+-rw-r--r--   0 christianharrison   (501) staff       (20)     1072 2023-04-03 16:06:06.000000 twitscrape-0.0.7/LICENSE
+-rw-r--r--   0 christianharrison   (501) staff       (20)     1049 2023-04-11 18:32:03.684487 twitscrape-0.0.7/PKG-INFO
+-rw-r--r--   0 christianharrison   (501) staff       (20)      451 2023-04-03 16:06:06.000000 twitscrape-0.0.7/README.md
+-rw-r--r--   0 christianharrison   (501) staff       (20)      779 2023-04-11 18:31:52.000000 twitscrape-0.0.7/pyproject.toml
+-rw-r--r--   0 christianharrison   (501) staff       (20)       38 2023-04-11 18:32:03.684989 twitscrape-0.0.7/setup.cfg
+drwxr-xr-x   0 christianharrison   (501) staff       (20)        0 2023-04-11 18:32:03.680716 twitscrape-0.0.7/tests/
+-rw-r--r--   0 christianharrison   (501) staff       (20)      353 2023-04-11 13:55:48.000000 twitscrape-0.0.7/tests/test_twitter_scraper.py
+drwxr-xr-x   0 christianharrison   (501) staff       (20)        0 2023-04-11 18:32:03.681631 twitscrape-0.0.7/twitscrape/
+-rw-r--r--   0 christianharrison   (501) staff       (20)        0 2023-04-03 16:06:06.000000 twitscrape-0.0.7/twitscrape/__init__.py
+-rw-r--r--   0 christianharrison   (501) staff       (20)    11101 2023-04-11 18:27:45.000000 twitscrape-0.0.7/twitscrape/twitter_scraper.py
+drwxr-xr-x   0 christianharrison   (501) staff       (20)        0 2023-04-11 18:32:03.683899 twitscrape-0.0.7/twitscrape.egg-info/
+-rw-r--r--   0 christianharrison   (501) staff       (20)     1049 2023-04-11 18:32:03.000000 twitscrape-0.0.7/twitscrape.egg-info/PKG-INFO
+-rw-r--r--   0 christianharrison   (501) staff       (20)      284 2023-04-11 18:32:03.000000 twitscrape-0.0.7/twitscrape.egg-info/SOURCES.txt
+-rw-r--r--   0 christianharrison   (501) staff       (20)        1 2023-04-11 18:32:03.000000 twitscrape-0.0.7/twitscrape.egg-info/dependency_links.txt
+-rw-r--r--   0 christianharrison   (501) staff       (20)       60 2023-04-11 18:32:03.000000 twitscrape-0.0.7/twitscrape.egg-info/requires.txt
+-rw-r--r--   0 christianharrison   (501) staff       (20)       11 2023-04-11 18:32:03.000000 twitscrape-0.0.7/twitscrape.egg-info/top_level.txt
```

### Comparing `twitscrape-0.0.6/LICENSE` & `twitscrape-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `twitscrape-0.0.6/PKG-INFO` & `twitscrape-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitscrape
-Version: 0.0.6
+Version: 0.0.7
 Summary: Simple package using Selenium to scrape tweet data based on geolocation and datetime
 Author-email: Christian Harrison <christywastakenwastaken@gmail.com>
 Project-URL: Homepage, https://github.com/christywastaken/twitscrape
 Project-URL: Bug Tracker, https://github.com/christywastaken/twitscrape/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `twitscrape-0.0.6/pyproject.toml` & `twitscrape-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 67"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "twitscrape"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Christian Harrison", email="christywastakenwastaken@gmail.com" },
 ]
 description = "Simple package using Selenium to scrape tweet data based on geolocation and datetime"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `twitscrape-0.0.6/twitscrape/twitter_scraper.py` & `twitscrape-0.0.7/twitscrape/twitter_scraper.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,25 +33,24 @@
         self.longitude = longitude
         self.radius = radius
         self.filter_replies = filter_replies
         self.filter_links = filter_links
         self.is_headless = is_headless
         # Set options for browser/driver
         options = Options()
-        options.add_argument("--window-size=2160,3840")
         if is_headless:
             options.add_argument("--headless=new")
           
         # Use ChromeDriverManager().install() to update driver for browser.
         print('-- TwitterGeolocationScraper running. This may take a minute to update the webdriver. --')
         self.driver = webdriver.Chrome(service=Service(ChromeDriverManager().install()), options=options)
         # Narrows the scope of to requests containing 'adaptive' (the requests containing tweets)
         self.driver.scopes= ['.*adaptive.*']
         # Tweet_df_model
-        self.tweet_df_schema = pd.DataFrame(columns=['tweet_id', 'user_id', 'created_at', 'tweet_text', 'hashtags', 'media_url', 'retweet_count', 'favourite_count', 'reply_count', 'views'])
+        self.tweet_df = pd.DataFrame(columns=['tweet_id', 'user_id', 'created_at', 'tweet_text', 'hashtags', 'media_url', 'retweet_count', 'favourite_count', 'reply_count', 'views'])
       
 
 
 
     def create_twitter_url(self) -> str:
         # As default it uses Central Newcastle-Upon-Tyne with 10km radius, filters links and replies, sorted by latest. Start_date & end_date: current date.
         today = datetime.utcnow()
@@ -77,27 +76,34 @@
             return f'https://twitter.com/search?f=live&q=geocode%3A{str(latitude)}%2C{str(longitude)}%2C{str(radius)}km%20until%3A{end_date}%20since%3A{start_date}%20-filter%3Areplies&src=typed_query'                
         if filter_replies == False and filter_links == True:
             return f'https://twitter.com/search?f=live&q=geocode%3A{str(latitude)}%2C{str(longitude)}%2C{str(radius)}km%20until%3A{end_date}%20since%3A{start_date}%20-filter%3Alinks&src=typed_query'
         if filter_replies == True and filter_links == True:  
             return f'https://twitter.com/search?f=live&q=geocode%3A{str(latitude)}%2C{str(longitude)}%2C{str(radius)}km%20until%3A{end_date}%20since%3A{start_date}%20-filter%3Alinks%20-filter%3Areplies&src=typed_query'
 
     
-    def get_tweets(self) -> Tuple[pd.DataFrame, int, int]:
+    def get_tweets(self) -> Tuple[int, int]:
         """
         Waits for the request containing the tweet data.
         Returns a tuple of (tweet dataframe, remaning rate limit, rate limit reset time)
         """
-        tweet_df = self.tweet_df_schema
+        
         try:
             # Waits for the response containing 'Adaptive' which contains the tweet data.
             request = self.driver.wait_for_request('adaptive')
             # Decodes the byte data from the response
             body = decode(request.response.body, request.response.headers.get('Content-Encoding', 'identity')) 
             data = json.loads(body)
-            tweets = data['globalObjects']['tweets']
+            try:
+                tweets = data['globalObjects']['tweets']
+            except Exception as err:
+                print(f'Error: {err}')
+                with open('error_logging.csv', 'a') as f:
+                    f.write(f'BODY: {data} \n')
+                    f.write(f'HEADERS: {request.response.headers.as_string()} ------------------------------------------ \n')
+                #TODO: logg errors properly. 
             # Get rate limit info
             try:
                 rate_lim_remaining = int(request.response.headers.get('x-rate-limit-remaining'))
             except:
                 rate_lim_remaining = None
             try:
                 rate_lim_reset_time = int(request.response.headers.get('x-rate-limit-reset'))
@@ -145,73 +151,78 @@
                 except:
                     favorite_count = None
                 try:
                     views = tweet_data['ext_views']['count']
                 except:
                     views = None
 
-                
                 new_row_df = pd.DataFrame({'tweet_id': [tweet_id],
                                         'user_id': [user_id],
                                         'created_at': [created_at],
                                         'tweet_text': [tweet_text],
                                         'hashtags': [hashtags],
                                         'media_url': [media_urls],
                                         'retweet_count': [retweet_count],
                                         'reply_count': [reply_count],
                                         'favourite_count': [favorite_count],
                                         'views': [views]})
-              
-                tweet_df = pd.concat([tweet_df, new_row_df], ignore_index=True)
+                
+                self.tweet_df = pd.concat([self.tweet_df, new_row_df], ignore_index=True)
+                
         except Exception as err:
             print(f'-- Error: {err} --')
-        tweet_df.sort_values(by='created_at', ascending=False, inplace=True)
-        # Deletes driver.requests so get_tweets() waits for the new request response 
-        del self.driver.requests
-        return (tweet_df, rate_lim_remaining, rate_lim_reset_time)
+        print(f'Tweets Scraped: {len(self.tweet_df)}')
+        return (rate_lim_remaining, rate_lim_reset_time)
+
 
 
     def run(self) -> pd.DataFrame:
-        """
-        Runs the scraper, returning a dataframe with all of the tweet data.
-        """
+        """ Runs the scraper, returning a dataframe with all of the tweet data."""
         self.driver.get(self.create_twitter_url())
         # Wait for the readyState = complete so page has loaded in. 
         state = ''
         while state != 'complete':
             print('Page loading not complete')
             time.sleep(1) 
             state = self.driver.execute_script('return document.readyState')
-        all_tweets_df = self.tweet_df_schema #TODO: should this append to the a class property, or just return it from the function as I already am? 
+
+        rate_lim_remaining, rate_lim_reset_time = self.get_tweets()
+        
         last_height = 0
-        # Loop until the document.body.scrollHeight no longer increases - end of page reached. 
+
         while True:
+            # Loop until the document.body.scrollHeight no longer increases - end of page reached. 
             try:
-                # Destructure output of get_tweets()
-                tweet_df, rate_lim_remaining, rate_lim_reset_time = self.get_tweets()
-                all_tweets_df = pd.concat([all_tweets_df, tweet_df], ignore_index=True)
-                print(f'remaining rate limit: {rate_lim_remaining} | tweets scraped: {len(all_tweets_df)}') #TODO: edit this for better readout. Make activity spinner?
-                
-                time.sleep(0.3) #TODO: Work out a better implementation for this timeout. The scrolling should happen when the page is ready, so it doesn't error.
-                self.driver.execute_script("window.scrollTo(0, document.body.scrollHeight)")
-                new_height = self.driver.execute_script("return document.body.scrollHeight")
-
-                if rate_lim_remaining < 5:
+                if rate_lim_remaining < 3:
                     # If we are getting close to the rate limit, sleep the app until the rate-limit has reset. 
                     time_dif = rate_lim_reset_time - time.time()
-                    # Add 60s for good measure to ensure rate-limit resets.
-                    wait_time = time_dif + 60 #TODO: check if this is really requried after new changes made to else statement that stopped driver scrolling
-                    print(f'-- Waiting {wait_time /60} mins for rate limit to reset --')
-                    time.sleep(wait_time)
+                    wait_time = time_dif + 10 #TODO: check if this is really requried after new changes made to else statement that stopped driver scrolling
+                    print(f'-- Waiting {round(wait_time / 60, 2)} mins for rate limit to reset --')
+                    try:
+                        time.sleep(wait_time)
+                    except Exception as err:
+                        print(f'Error: {err}')
+                        
+                # Deletes driver.requests so get_tweets() waits for the new request response 
+                del self.driver.requests
+                self.driver.execute_script("window.scrollTo(0, document.body.scrollHeight)")
+                new_height = self.driver.execute_script("return document.body.scrollHeight")
+                time.sleep(0.3) #TODO: Work out a better implementation for this timeout. The scrolling should happen when the page is ready, so it doesn't error.
+                
+                try:
+                    rate_lim_remaining, rate_lim_reset_time = self.get_tweets()
+                except Exception as err:
+                    print(f'Error getting data - get_tweets(). Error: {err}') 
 
                 if new_height == last_height:
-                    print('-- Finished running scraper --')
-                    return all_tweets_df
+                    print('-- Scraper Finished Running. Success. --')
+                    return self.tweet_df
                 else:
                     last_height = new_height
             except Exception as err:
                 print(f'Error: {err}')
-                continue
+                print('-- Scraper Finished Running Prematurely. Incomplete Data Returned (self.tweet_df) --')
+                return self.tweet_df
```

### Comparing `twitscrape-0.0.6/twitscrape.egg-info/PKG-INFO` & `twitscrape-0.0.7/twitscrape.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitscrape
-Version: 0.0.6
+Version: 0.0.7
 Summary: Simple package using Selenium to scrape tweet data based on geolocation and datetime
 Author-email: Christian Harrison <christywastakenwastaken@gmail.com>
 Project-URL: Homepage, https://github.com/christywastaken/twitscrape
 Project-URL: Bug Tracker, https://github.com/christywastaken/twitscrape/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

