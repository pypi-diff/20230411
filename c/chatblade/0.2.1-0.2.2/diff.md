# Comparing `tmp/chatblade-0.2.1.tar.gz` & `tmp/chatblade-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatblade-0.2.1.tar", last modified: Sun Apr  2 13:41:40 2023, max compression
+gzip compressed data, was "chatblade-0.2.2.tar", last modified: Tue Apr 11 09:31:41 2023, max compression
```

## Comparing `chatblade-0.2.1.tar` & `chatblade-0.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 npiv       (501) staff       (20)        0 2023-04-02 13:41:40.336670 chatblade-0.2.1/
--rw-r--r--   0 npiv       (501) staff       (20)    34600 2023-03-19 21:07:18.000000 chatblade-0.2.1/LICENSE
--rw-r--r--   0 npiv       (501) staff       (20)    10709 2023-04-02 13:41:40.336738 chatblade-0.2.1/PKG-INFO
--rw-r--r--   0 npiv       (501) staff       (20)    10405 2023-04-02 08:27:40.000000 chatblade-0.2.1/README.md
-drwxr-xr-x   0 npiv       (501) staff       (20)        0 2023-04-02 13:41:40.335925 chatblade-0.2.1/chatblade/
--rw-r--r--   0 npiv       (501) staff       (20)        0 2023-03-21 01:08:04.000000 chatblade-0.2.1/chatblade/__init__.py
--rw-r--r--   0 npiv       (501) staff       (20)       86 2023-03-18 14:05:20.000000 chatblade-0.2.1/chatblade/__main__.py
--rw-r--r--   0 npiv       (501) staff       (20)     4466 2023-04-02 07:58:37.000000 chatblade-0.2.1/chatblade/chat.py
--rw-r--r--   0 npiv       (501) staff       (20)     4584 2023-04-02 13:23:08.000000 chatblade-0.2.1/chatblade/cli.py
--rw-r--r--   0 npiv       (501) staff       (20)       42 2023-03-21 01:25:46.000000 chatblade-0.2.1/chatblade/errors.py
--rw-r--r--   0 npiv       (501) staff       (20)     5590 2023-04-02 08:04:15.000000 chatblade-0.2.1/chatblade/parser.py
--rw-r--r--   0 npiv       (501) staff       (20)     4543 2023-04-02 07:58:37.000000 chatblade-0.2.1/chatblade/printer.py
--rw-r--r--   0 npiv       (501) staff       (20)     1106 2023-04-02 07:58:37.000000 chatblade-0.2.1/chatblade/session.py
--rw-r--r--   0 npiv       (501) staff       (20)     4077 2023-04-02 08:18:36.000000 chatblade-0.2.1/chatblade/storage.py
--rw-r--r--   0 npiv       (501) staff       (20)      683 2023-04-02 07:58:37.000000 chatblade-0.2.1/chatblade/utils.py
-drwxr-xr-x   0 npiv       (501) staff       (20)        0 2023-04-02 13:41:40.336578 chatblade-0.2.1/chatblade.egg-info/
--rw-r--r--   0 npiv       (501) staff       (20)    10709 2023-04-02 13:41:40.000000 chatblade-0.2.1/chatblade.egg-info/PKG-INFO
--rw-r--r--   0 npiv       (501) staff       (20)      452 2023-04-02 13:41:40.000000 chatblade-0.2.1/chatblade.egg-info/SOURCES.txt
--rw-r--r--   0 npiv       (501) staff       (20)        1 2023-04-02 13:41:40.000000 chatblade-0.2.1/chatblade.egg-info/dependency_links.txt
--rw-r--r--   0 npiv       (501) staff       (20)       54 2023-04-02 13:41:40.000000 chatblade-0.2.1/chatblade.egg-info/entry_points.txt
--rw-r--r--   0 npiv       (501) staff       (20)       49 2023-04-02 13:41:40.000000 chatblade-0.2.1/chatblade.egg-info/requires.txt
--rw-r--r--   0 npiv       (501) staff       (20)       10 2023-04-02 13:41:40.000000 chatblade-0.2.1/chatblade.egg-info/top_level.txt
--rw-r--r--   0 npiv       (501) staff       (20)       90 2023-03-22 17:02:55.000000 chatblade-0.2.1/pyproject.toml
--rw-r--r--   0 npiv       (501) staff       (20)      567 2023-04-02 13:41:40.337084 chatblade-0.2.1/setup.cfg
--rw-r--r--   0 npiv       (501) staff       (20)       38 2023-03-18 13:34:51.000000 chatblade-0.2.1/setup.py
+drwxr-xr-x   0 npiv       (501) staff       (20)        0 2023-04-11 09:31:41.489752 chatblade-0.2.2/
+-rw-r--r--   0 npiv       (501) staff       (20)    34600 2023-03-19 21:07:18.000000 chatblade-0.2.2/LICENSE
+-rw-r--r--   0 npiv       (501) staff       (20)    10709 2023-04-11 09:31:41.489806 chatblade-0.2.2/PKG-INFO
+-rw-r--r--   0 npiv       (501) staff       (20)    10405 2023-04-11 09:29:23.000000 chatblade-0.2.2/README.md
+drwxr-xr-x   0 npiv       (501) staff       (20)        0 2023-04-11 09:31:41.489031 chatblade-0.2.2/chatblade/
+-rw-r--r--   0 npiv       (501) staff       (20)        0 2023-03-21 01:08:04.000000 chatblade-0.2.2/chatblade/__init__.py
+-rw-r--r--   0 npiv       (501) staff       (20)       86 2023-03-18 14:05:20.000000 chatblade-0.2.2/chatblade/__main__.py
+-rw-r--r--   0 npiv       (501) staff       (20)     4466 2023-04-02 07:58:37.000000 chatblade-0.2.2/chatblade/chat.py
+-rw-r--r--   0 npiv       (501) staff       (20)     4584 2023-04-09 08:15:38.000000 chatblade-0.2.2/chatblade/cli.py
+-rw-r--r--   0 npiv       (501) staff       (20)       42 2023-03-21 01:25:46.000000 chatblade-0.2.2/chatblade/errors.py
+-rw-r--r--   0 npiv       (501) staff       (20)     5590 2023-04-09 08:15:38.000000 chatblade-0.2.2/chatblade/parser.py
+-rw-r--r--   0 npiv       (501) staff       (20)     4543 2023-04-02 07:58:37.000000 chatblade-0.2.2/chatblade/printer.py
+-rw-r--r--   0 npiv       (501) staff       (20)     1106 2023-04-02 07:58:37.000000 chatblade-0.2.2/chatblade/session.py
+-rw-r--r--   0 npiv       (501) staff       (20)     4079 2023-04-11 09:29:23.000000 chatblade-0.2.2/chatblade/storage.py
+-rw-r--r--   0 npiv       (501) staff       (20)      683 2023-04-02 07:58:37.000000 chatblade-0.2.2/chatblade/utils.py
+drwxr-xr-x   0 npiv       (501) staff       (20)        0 2023-04-11 09:31:41.489658 chatblade-0.2.2/chatblade.egg-info/
+-rw-r--r--   0 npiv       (501) staff       (20)    10709 2023-04-11 09:31:41.000000 chatblade-0.2.2/chatblade.egg-info/PKG-INFO
+-rw-r--r--   0 npiv       (501) staff       (20)      452 2023-04-11 09:31:41.000000 chatblade-0.2.2/chatblade.egg-info/SOURCES.txt
+-rw-r--r--   0 npiv       (501) staff       (20)        1 2023-04-11 09:31:41.000000 chatblade-0.2.2/chatblade.egg-info/dependency_links.txt
+-rw-r--r--   0 npiv       (501) staff       (20)       54 2023-04-11 09:31:41.000000 chatblade-0.2.2/chatblade.egg-info/entry_points.txt
+-rw-r--r--   0 npiv       (501) staff       (20)       49 2023-04-11 09:31:41.000000 chatblade-0.2.2/chatblade.egg-info/requires.txt
+-rw-r--r--   0 npiv       (501) staff       (20)       10 2023-04-11 09:31:41.000000 chatblade-0.2.2/chatblade.egg-info/top_level.txt
+-rw-r--r--   0 npiv       (501) staff       (20)       90 2023-03-22 17:02:55.000000 chatblade-0.2.2/pyproject.toml
+-rw-r--r--   0 npiv       (501) staff       (20)      567 2023-04-11 09:31:41.490054 chatblade-0.2.2/setup.cfg
+-rw-r--r--   0 npiv       (501) staff       (20)       38 2023-03-18 13:34:51.000000 chatblade-0.2.2/setup.py
```

### Comparing `chatblade-0.2.1/LICENSE` & `chatblade-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chatblade-0.2.1/PKG-INFO` & `chatblade-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatblade
-Version: 0.2.1
+Version: 0.2.2
 Summary: CLI Swiss Army Knife for ChatGPT
 Home-page: https://github.com/npiv/chatblade
 Project-URL: Documentation, https://github.com/npiv/chatblade
 Keywords: chatblade chatgpt cli python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -48,15 +48,15 @@
 ```bash
 chatblade how can I extract a still frame from a video at 22:01 with ffmpeg
 ```
 <img width="650" alt="image" src="https://user-images.githubusercontent.com/452020/226869260-1dcd4faf-521c-466b-998a-fd5cfdc5b3c7.png">
 
 #### recall the last conversation
 
-if you would like to revall the last conversation just call it back with `-l`
+if you would like to recall the last conversation just call it back with `-l`
 
 ```bash
 chatblade -l
 ```
 
 #### Continue the last conversation
```

### Comparing `chatblade-0.2.1/README.md` & `chatblade-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 ```bash
 chatblade how can I extract a still frame from a video at 22:01 with ffmpeg
 ```
 <img width="650" alt="image" src="https://user-images.githubusercontent.com/452020/226869260-1dcd4faf-521c-466b-998a-fd5cfdc5b3c7.png">
 
 #### recall the last conversation
 
-if you would like to revall the last conversation just call it back with `-l`
+if you would like to recall the last conversation just call it back with `-l`
 
 ```bash
 chatblade -l
 ```
 
 #### Continue the last conversation
```

### Comparing `chatblade-0.2.1/chatblade/chat.py` & `chatblade-0.2.2/chatblade/chat.py`

 * *Files identical despite different names*

### Comparing `chatblade-0.2.1/chatblade/cli.py` & `chatblade-0.2.2/chatblade/cli.py`

 * *Files identical despite different names*

### Comparing `chatblade-0.2.1/chatblade/parser.py` & `chatblade-0.2.2/chatblade/parser.py`

 * *Files identical despite different names*

### Comparing `chatblade-0.2.1/chatblade/printer.py` & `chatblade-0.2.2/chatblade/printer.py`

 * *Files identical despite different names*

### Comparing `chatblade-0.2.1/chatblade/session.py` & `chatblade-0.2.2/chatblade/session.py`

 * *Files identical despite different names*

### Comparing `chatblade-0.2.1/chatblade/storage.py` & `chatblade-0.2.2/chatblade/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 def to_cache(messages, session):
     """cache the current messages state"""
     file_path = get_session_path(session)
     file_path_tmp = file_path + make_postfix()
     with open(file_path_tmp, "w") as f:
         yaml.dump(messages, f)
-    os.rename(file_path_tmp, file_path)
+    os.replace(file_path_tmp, file_path)
 
 
 def messages_from_cache(session):
     """load messages from session
     Return empty list if not exists"""
     file_path = get_session_path(session)
     if not os.path.exists(file_path):
@@ -80,15 +80,15 @@
 def migrate_to_session(session):
     """save pre-session last messages to session"""
     file_path = get_cache_path(False)
     messages = messages_from_cache_legacy()
     file_path_tmp = file_path + make_postfix()
     # resolve name conflict, but keep old cache file
     # until all has gone through fine
-    os.rename(file_path, file_path_tmp)
+    os.replace(file_path, file_path_tmp)
     to_cache(messages, session)
     os.unlink(file_path_tmp)
 
 
 def load_prompt_file(prompt_name):
     """
     load a prompt configuration by its name
```

### Comparing `chatblade-0.2.1/chatblade/utils.py` & `chatblade-0.2.2/chatblade/utils.py`

 * *Files identical despite different names*

### Comparing `chatblade-0.2.1/chatblade.egg-info/PKG-INFO` & `chatblade-0.2.2/chatblade.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatblade
-Version: 0.2.1
+Version: 0.2.2
 Summary: CLI Swiss Army Knife for ChatGPT
 Home-page: https://github.com/npiv/chatblade
 Project-URL: Documentation, https://github.com/npiv/chatblade
 Keywords: chatblade chatgpt cli python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -48,15 +48,15 @@
 ```bash
 chatblade how can I extract a still frame from a video at 22:01 with ffmpeg
 ```
 <img width="650" alt="image" src="https://user-images.githubusercontent.com/452020/226869260-1dcd4faf-521c-466b-998a-fd5cfdc5b3c7.png">
 
 #### recall the last conversation
 
-if you would like to revall the last conversation just call it back with `-l`
+if you would like to recall the last conversation just call it back with `-l`
 
 ```bash
 chatblade -l
 ```
 
 #### Continue the last conversation
```

### Comparing `chatblade-0.2.1/setup.cfg` & `chatblade-0.2.2/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chatblade
-version = 0.2.1
+version = 0.2.2
 description = CLI Swiss Army Knife for ChatGPT
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_file = LICENSE
 url = https://github.com/npiv/chatblade
 keywords = chatblade chatgpt cli python
 project_urls =
```

