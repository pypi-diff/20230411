# Comparing `tmp/tulp-0.4.0.tar.gz` & `tmp/tulp-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tulp-0.4.0.tar", last modified: Mon Apr 10 14:07:30 2023, max compression
+gzip compressed data, was "tulp-0.4.1.tar", last modified: Mon Apr 10 21:27:41 2023, max compression
```

## Comparing `tulp-0.4.0.tar` & `tulp-0.4.1.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2023-04-10 14:07:30.321810 tulp-0.4.0/
--rw-rw-r--   0 fede      (1000) fede      (1000)      684 2023-04-10 13:46:44.000000 tulp-0.4.0/LICENSE
--rw-rw-r--   0 fede      (1000) fede      (1000)     5605 2023-04-10 14:07:30.321810 tulp-0.4.0/PKG-INFO
--rw-rw-r--   0 fede      (1000) fede      (1000)     5010 2023-04-09 15:35:50.000000 tulp-0.4.0/README.md
--rw-rw-r--   0 fede      (1000) fede      (1000)      900 2023-04-10 14:07:30.321810 tulp-0.4.0/setup.cfg
--rw-rw-r--   0 fede      (1000) fede      (1000)       39 2023-04-10 13:18:19.000000 tulp-0.4.0/setup.py
-drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2023-04-10 14:07:30.321810 tulp-0.4.0/tulp/
--rw-rw-r--   0 fede      (1000) fede      (1000)       74 2023-04-10 13:37:14.000000 tulp-0.4.0/tulp/__init__.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     3977 2023-04-09 15:21:27.000000 tulp-0.4.0/tulp/filteringPrompt.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     2230 2023-04-09 15:21:27.000000 tulp-0.4.0/tulp/requestPrompt.py
--rwxrwxr-x   0 fede      (1000) fede      (1000)     5231 2023-04-10 14:05:27.000000 tulp-0.4.0/tulp/tulp.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     1008 2023-04-10 14:01:41.000000 tulp-0.4.0/tulp/tulpconfig.py
--rw-rw-r--   0 fede      (1000) fede      (1000)      991 2023-04-10 14:01:12.000000 tulp-0.4.0/tulp/tulplogger.py
--rw-rw-r--   0 fede      (1000) fede      (1000)       18 2023-04-10 13:49:07.000000 tulp-0.4.0/tulp/version.py
-drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2023-04-10 14:07:30.321810 tulp-0.4.0/tulp.egg-info/
--rw-rw-r--   0 fede      (1000) fede      (1000)     5605 2023-04-10 14:07:30.000000 tulp-0.4.0/tulp.egg-info/PKG-INFO
--rw-rw-r--   0 fede      (1000) fede      (1000)      359 2023-04-10 14:07:30.000000 tulp-0.4.0/tulp.egg-info/SOURCES.txt
--rw-rw-r--   0 fede      (1000) fede      (1000)        1 2023-04-10 14:07:30.000000 tulp-0.4.0/tulp.egg-info/dependency_links.txt
--rw-rw-r--   0 fede      (1000) fede      (1000)       39 2023-04-10 14:07:30.000000 tulp-0.4.0/tulp.egg-info/entry_points.txt
--rw-rw-r--   0 fede      (1000) fede      (1000)       15 2023-04-10 14:07:30.000000 tulp-0.4.0/tulp.egg-info/requires.txt
--rw-rw-r--   0 fede      (1000) fede      (1000)        5 2023-04-10 14:07:30.000000 tulp-0.4.0/tulp.egg-info/top_level.txt
--rw-rw-r--   0 fede      (1000) fede      (1000)        1 2023-04-10 13:32:42.000000 tulp-0.4.0/tulp.egg-info/zip-safe
+drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2023-04-10 21:27:41.748621 tulp-0.4.1/
+-rw-rw-r--   0 fede      (1000) fede      (1000)      684 2023-04-10 13:46:44.000000 tulp-0.4.1/LICENSE
+-rw-rw-r--   0 fede      (1000) fede      (1000)     5603 2023-04-10 21:27:41.748621 tulp-0.4.1/PKG-INFO
+-rw-rw-r--   0 fede      (1000) fede      (1000)     5008 2023-04-10 16:47:53.000000 tulp-0.4.1/README.md
+-rw-rw-r--   0 fede      (1000) fede      (1000)      900 2023-04-10 21:27:41.748621 tulp-0.4.1/setup.cfg
+-rw-rw-r--   0 fede      (1000) fede      (1000)       39 2023-04-10 13:18:19.000000 tulp-0.4.1/setup.py
+drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2023-04-10 21:27:41.744621 tulp-0.4.1/tulp/
+-rw-rw-r--   0 fede      (1000) fede      (1000)       74 2023-04-10 13:37:14.000000 tulp-0.4.1/tulp/__init__.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     3996 2023-04-10 14:39:02.000000 tulp-0.4.1/tulp/filteringPrompt.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     3977 2023-04-10 14:12:07.000000 tulp-0.4.1/tulp/filteringPrompt.v1.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     3887 2023-04-10 14:20:00.000000 tulp-0.4.1/tulp/filteringPrompt.v2.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     2230 2023-04-09 15:21:27.000000 tulp-0.4.1/tulp/requestPrompt.py
+-rwxrwxr-x   0 fede      (1000) fede      (1000)     5331 2023-04-10 16:53:12.000000 tulp-0.4.1/tulp/tulp.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     1008 2023-04-10 14:01:41.000000 tulp-0.4.1/tulp/tulpconfig.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)      991 2023-04-10 14:01:12.000000 tulp-0.4.1/tulp/tulplogger.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)       18 2023-04-10 21:27:24.000000 tulp-0.4.1/tulp/version.py
+drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2023-04-10 21:27:41.748621 tulp-0.4.1/tulp.egg-info/
+-rw-rw-r--   0 fede      (1000) fede      (1000)     5603 2023-04-10 21:27:41.000000 tulp-0.4.1/tulp.egg-info/PKG-INFO
+-rw-rw-r--   0 fede      (1000) fede      (1000)      413 2023-04-10 21:27:41.000000 tulp-0.4.1/tulp.egg-info/SOURCES.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)        1 2023-04-10 21:27:41.000000 tulp-0.4.1/tulp.egg-info/dependency_links.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)       39 2023-04-10 21:27:41.000000 tulp-0.4.1/tulp.egg-info/entry_points.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)       15 2023-04-10 21:27:41.000000 tulp-0.4.1/tulp.egg-info/requires.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)        5 2023-04-10 21:27:41.000000 tulp-0.4.1/tulp.egg-info/top_level.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)        1 2023-04-10 13:32:42.000000 tulp-0.4.1/tulp.egg-info/zip-safe
```

### Comparing `tulp-0.4.0/LICENSE` & `tulp-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tulp-0.4.0/PKG-INFO` & `tulp-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulp
-Version: 0.4.0
+Version: 0.4.1
 Summary: TULP: A command line tool, in the best essence of POSIX tooling, that will help you to **process**, **filter**, and **create** data in this new Artificial Intelligence world.
 Home-page: https://github.com/fedenunez/tulp
 Author: Federico Nuñez
 Author-email: fedenunez@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
@@ -42,25 +42,25 @@
 
 ## Configuration 
 The configuration file is located at ~/.tulp.conf. Define your own ~/.tulp.conf file or define the same environment variable but using prefix TULP. 
 
 The following are the parameters that can be configured:
 - LOG_LEVEL: The log level of Tulip. Valid options are DEBUG, INFO, WARNING, ERROR, and CRITICAL. The default value is INFO.
 - OPENAI_API_KEY: The API key for OpenAI. The default value is an empty string.
-- CHAR_LIMIT: The maximum number of characters processed in one chunk. The default value is 5000.
+- MAX_CHARS: The maximum number of characters processed in one chunk. The default value is 5000.
 - MODEL: The openai model used by Tulip. The default value is gpt-3.5-turbo, but gpt-4 is also available
 
-As environment variables they will become: TULP_LOG_LEVEL, TULP_OPENAI_API_KEY, TULP_CHAR_LIMIT or TULP_MODEL
+As environment variables they will become: TULP_LOG_LEVEL, TULP_OPENAI_API_KEY, TULP_MAX_CHARS or TULP_MODEL
 
 Here is an example configuration file with the default values:
 ```
 [DEFAULT]
 LOG_LEVEL = INFO
 OPENAI_API_KEY = <<<YOUR API KEY >>>>
-CHAR_LIMIT = 5000
+MAX_CHARS = 10000
 MODEL = gpt-3.5-turbo
 ```
 ## Examples:
 The usage is endless, but anyway, here you have some ideas as inspirations:
 ### Typical Unix tooling replacement:
 #### Sed
 ```
```

### Comparing `tulp-0.4.0/README.md` & `tulp-0.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -28,25 +28,25 @@
 
 ## Configuration 
 The configuration file is located at ~/.tulp.conf. Define your own ~/.tulp.conf file or define the same environment variable but using prefix TULP. 
 
 The following are the parameters that can be configured:
 - LOG_LEVEL: The log level of Tulip. Valid options are DEBUG, INFO, WARNING, ERROR, and CRITICAL. The default value is INFO.
 - OPENAI_API_KEY: The API key for OpenAI. The default value is an empty string.
-- CHAR_LIMIT: The maximum number of characters processed in one chunk. The default value is 5000.
+- MAX_CHARS: The maximum number of characters processed in one chunk. The default value is 5000.
 - MODEL: The openai model used by Tulip. The default value is gpt-3.5-turbo, but gpt-4 is also available
 
-As environment variables they will become: TULP_LOG_LEVEL, TULP_OPENAI_API_KEY, TULP_CHAR_LIMIT or TULP_MODEL
+As environment variables they will become: TULP_LOG_LEVEL, TULP_OPENAI_API_KEY, TULP_MAX_CHARS or TULP_MODEL
 
 Here is an example configuration file with the default values:
 ```
 [DEFAULT]
 LOG_LEVEL = INFO
 OPENAI_API_KEY = <<<YOUR API KEY >>>>
-CHAR_LIMIT = 5000
+MAX_CHARS = 10000
 MODEL = gpt-3.5-turbo
 ```
 ## Examples:
 The usage is endless, but anyway, here you have some ideas as inspirations:
 ### Typical Unix tooling replacement:
 #### Sed
 ```
```

### Comparing `tulp-0.4.0/setup.cfg` & `tulp-0.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `tulp-0.4.0/tulp/filteringPrompt.py` & `tulp-0.4.1/tulp/filteringPrompt.v1.py`

 * *Files identical despite different names*

### Comparing `tulp-0.4.0/tulp/requestPrompt.py` & `tulp-0.4.1/tulp/requestPrompt.py`

 * *Files identical despite different names*

### Comparing `tulp-0.4.0/tulp/tulp.py` & `tulp-0.4.1/tulp/tulp.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,30 +65,30 @@
         import tulp.requestPrompt
         instructionFunction=tulp.requestPrompt.getBaseMessages
 
     user_messages=[]
     # Split input text into chunks to fit within max token window
     max_chars = config.max_chars  # Maximum number of chars that we will send to GPT
     if len(input_text) > max_chars:
-        log.warning(f"Warning: input is to big, we will split processing in chunks of less than {max_chars}")
+        log.warning(f"Warning: input is to big, we will split processing in chunks of less than {max_chars}. You may use the TULP_MAX_CHARS env variable to control the size of the processing chunk size.")
     input_lines = input_text.splitlines()
     # try to split it in lines or max_size
     compressed_lines = [""]
 
     for iline in input_lines:
         compresed_index = len(compressed_lines) - 1
         clen = len(compressed_lines[compresed_index]) 
         if clen + len(iline) < max_chars:
             compressed_lines[compresed_index] += iline + "\n"
         else:
             if clen != 0:
                 if (len(iline) < max_chars):
                     compressed_lines.append(iline + "\n")
                 else:
-                    for i in range(0,math.floor(iline)/max_chars+1):
+                    for i in range(0,math.floor(len(iline)/max_chars)+1):
                         input_chunk = iline[i*max_chars:(i+1)*max_chars] 
                         compressed_lines.append(input_chunk)
                     compressed_lines[compresed_index] += "\n"
 
     for line in compressed_lines:
          user_messages.append( {"role": "user", "content": line})
```

### Comparing `tulp-0.4.0/tulp/tulpconfig.py` & `tulp-0.4.1/tulp/tulpconfig.py`

 * *Files identical despite different names*

### Comparing `tulp-0.4.0/tulp/tulplogger.py` & `tulp-0.4.1/tulp/tulplogger.py`

 * *Files identical despite different names*

### Comparing `tulp-0.4.0/tulp.egg-info/PKG-INFO` & `tulp-0.4.1/tulp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulp
-Version: 0.4.0
+Version: 0.4.1
 Summary: TULP: A command line tool, in the best essence of POSIX tooling, that will help you to **process**, **filter**, and **create** data in this new Artificial Intelligence world.
 Home-page: https://github.com/fedenunez/tulp
 Author: Federico Nuñez
 Author-email: fedenunez@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
@@ -42,25 +42,25 @@
 
 ## Configuration 
 The configuration file is located at ~/.tulp.conf. Define your own ~/.tulp.conf file or define the same environment variable but using prefix TULP. 
 
 The following are the parameters that can be configured:
 - LOG_LEVEL: The log level of Tulip. Valid options are DEBUG, INFO, WARNING, ERROR, and CRITICAL. The default value is INFO.
 - OPENAI_API_KEY: The API key for OpenAI. The default value is an empty string.
-- CHAR_LIMIT: The maximum number of characters processed in one chunk. The default value is 5000.
+- MAX_CHARS: The maximum number of characters processed in one chunk. The default value is 5000.
 - MODEL: The openai model used by Tulip. The default value is gpt-3.5-turbo, but gpt-4 is also available
 
-As environment variables they will become: TULP_LOG_LEVEL, TULP_OPENAI_API_KEY, TULP_CHAR_LIMIT or TULP_MODEL
+As environment variables they will become: TULP_LOG_LEVEL, TULP_OPENAI_API_KEY, TULP_MAX_CHARS or TULP_MODEL
 
 Here is an example configuration file with the default values:
 ```
 [DEFAULT]
 LOG_LEVEL = INFO
 OPENAI_API_KEY = <<<YOUR API KEY >>>>
-CHAR_LIMIT = 5000
+MAX_CHARS = 10000
 MODEL = gpt-3.5-turbo
 ```
 ## Examples:
 The usage is endless, but anyway, here you have some ideas as inspirations:
 ### Typical Unix tooling replacement:
 #### Sed
 ```
```

