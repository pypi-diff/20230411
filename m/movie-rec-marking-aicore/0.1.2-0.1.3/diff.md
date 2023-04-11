# Comparing `tmp/movie-rec-marking-aicore-0.1.2.tar.gz` & `tmp/movie-rec-marking-aicore-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movie-rec-marking-aicore-0.1.2.tar", last modified: Mon Dec 12 18:45:22 2022, max compression
+gzip compressed data, was "movie-rec-marking-aicore-0.1.3.tar", last modified: Tue Apr 11 08:31:43 2023, max compression
```

## Comparing `movie-rec-marking-aicore-0.1.2.tar` & `movie-rec-marking-aicore-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ivanyingx  (1000) ivanyingx  (1000)        0 2022-12-12 18:45:22.902717 movie-rec-marking-aicore-0.1.2/
--rw-rw-r--   0 ivanyingx  (1000) ivanyingx  (1000)      216 2022-12-12 18:45:22.902717 movie-rec-marking-aicore-0.1.2/PKG-INFO
-drwxrwxr-x   0 ivanyingx  (1000) ivanyingx  (1000)        0 2022-12-12 18:45:22.902717 movie-rec-marking-aicore-0.1.2/movie_rec_marking/
--rw-rw-r--   0 ivanyingx  (1000) ivanyingx  (1000)        0 2022-12-12 17:43:54.000000 movie-rec-marking-aicore-0.1.2/movie_rec_marking/__init__.py
--rw-rw-r--   0 ivanyingx  (1000) ivanyingx  (1000)     2099 2022-12-12 17:43:54.000000 movie-rec-marking-aicore-0.1.2/movie_rec_marking/test_milestone_1.py
--rw-rw-r--   0 ivanyingx  (1000) ivanyingx  (1000)     6817 2022-12-12 17:43:54.000000 movie-rec-marking-aicore-0.1.2/movie_rec_marking/test_milestone_2.py
--rw-rw-r--   0 ivanyingx  (1000) ivanyingx  (1000)     5200 2022-12-12 17:43:54.000000 movie-rec-marking-aicore-0.1.2/movie_rec_marking/test_milestone_3.py
--rw-rw-r--   0 ivanyingx  (1000) ivanyingx  (1000)     6243 2022-12-12 17:43:54.000000 movie-rec-marking-aicore-0.1.2/movie_rec_marking/test_milestone_4.py
--rw-rw-r--   0 ivanyingx  (1000) ivanyingx  (1000)     9059 2022-12-12 18:45:01.000000 movie-rec-marking-aicore-0.1.2/movie_rec_marking/test_milestone_5.py
-drwxrwxr-x   0 ivanyingx  (1000) ivanyingx  (1000)        0 2022-12-12 18:45:22.902717 movie-rec-marking-aicore-0.1.2/movie_rec_marking_aicore.egg-info/
--rw-rw-r--   0 ivanyingx  (1000) ivanyingx  (1000)      216 2022-12-12 18:45:21.000000 movie-rec-marking-aicore-0.1.2/movie_rec_marking_aicore.egg-info/PKG-INFO
--rw-rw-r--   0 ivanyingx  (1000) ivanyingx  (1000)      467 2022-12-12 18:45:22.000000 movie-rec-marking-aicore-0.1.2/movie_rec_marking_aicore.egg-info/SOURCES.txt
--rw-rw-r--   0 ivanyingx  (1000) ivanyingx  (1000)        1 2022-12-12 18:45:21.000000 movie-rec-marking-aicore-0.1.2/movie_rec_marking_aicore.egg-info/dependency_links.txt
--rw-rw-r--   0 ivanyingx  (1000) ivanyingx  (1000)       26 2022-12-12 18:45:21.000000 movie-rec-marking-aicore-0.1.2/movie_rec_marking_aicore.egg-info/requires.txt
--rw-rw-r--   0 ivanyingx  (1000) ivanyingx  (1000)       18 2022-12-12 18:45:21.000000 movie-rec-marking-aicore-0.1.2/movie_rec_marking_aicore.egg-info/top_level.txt
--rw-rw-r--   0 ivanyingx  (1000) ivanyingx  (1000)       38 2022-12-12 18:45:22.902717 movie-rec-marking-aicore-0.1.2/setup.cfg
--rw-rw-r--   0 ivanyingx  (1000) ivanyingx  (1000)      390 2022-12-12 18:45:05.000000 movie-rec-marking-aicore-0.1.2/setup.py
+drwxr-xr-x   0 tianwenwangye   (501) staff       (20)        0 2023-04-11 08:31:43.546223 movie-rec-marking-aicore-0.1.3/
+-rw-r--r--   0 tianwenwangye   (501) staff       (20)      216 2023-04-11 08:31:43.544014 movie-rec-marking-aicore-0.1.3/PKG-INFO
+drwxr-xr-x   0 tianwenwangye   (501) staff       (20)        0 2023-04-11 08:31:43.535237 movie-rec-marking-aicore-0.1.3/movie_rec_marking/
+-rw-r--r--   0 tianwenwangye   (501) staff       (20)        0 2023-03-17 16:01:21.000000 movie-rec-marking-aicore-0.1.3/movie_rec_marking/__init__.py
+-rw-r--r--   0 tianwenwangye   (501) staff       (20)     2099 2023-03-17 16:01:21.000000 movie-rec-marking-aicore-0.1.3/movie_rec_marking/test_milestone_1.py
+-rw-r--r--   0 tianwenwangye   (501) staff       (20)     7331 2023-04-11 08:18:46.000000 movie-rec-marking-aicore-0.1.3/movie_rec_marking/test_milestone_2.py
+-rw-r--r--   0 tianwenwangye   (501) staff       (20)     5308 2023-04-11 08:31:37.000000 movie-rec-marking-aicore-0.1.3/movie_rec_marking/test_milestone_3.py
+-rw-r--r--   0 tianwenwangye   (501) staff       (20)     6242 2023-03-17 16:01:21.000000 movie-rec-marking-aicore-0.1.3/movie_rec_marking/test_milestone_4.py
+-rw-r--r--   0 tianwenwangye   (501) staff       (20)     9059 2023-03-17 16:01:21.000000 movie-rec-marking-aicore-0.1.3/movie_rec_marking/test_milestone_5.py
+drwxr-xr-x   0 tianwenwangye   (501) staff       (20)        0 2023-04-11 08:31:43.542802 movie-rec-marking-aicore-0.1.3/movie_rec_marking_aicore.egg-info/
+-rw-r--r--   0 tianwenwangye   (501) staff       (20)      216 2023-04-11 08:31:43.000000 movie-rec-marking-aicore-0.1.3/movie_rec_marking_aicore.egg-info/PKG-INFO
+-rw-r--r--   0 tianwenwangye   (501) staff       (20)      467 2023-04-11 08:31:43.000000 movie-rec-marking-aicore-0.1.3/movie_rec_marking_aicore.egg-info/SOURCES.txt
+-rw-r--r--   0 tianwenwangye   (501) staff       (20)        1 2023-04-11 08:31:43.000000 movie-rec-marking-aicore-0.1.3/movie_rec_marking_aicore.egg-info/dependency_links.txt
+-rw-r--r--   0 tianwenwangye   (501) staff       (20)       26 2023-04-11 08:31:43.000000 movie-rec-marking-aicore-0.1.3/movie_rec_marking_aicore.egg-info/requires.txt
+-rw-r--r--   0 tianwenwangye   (501) staff       (20)       18 2023-04-11 08:31:43.000000 movie-rec-marking-aicore-0.1.3/movie_rec_marking_aicore.egg-info/top_level.txt
+-rw-r--r--   0 tianwenwangye   (501) staff       (20)       38 2023-04-11 08:31:43.546377 movie-rec-marking-aicore-0.1.3/setup.cfg
+-rw-r--r--   0 tianwenwangye   (501) staff       (20)      390 2023-04-11 08:20:09.000000 movie-rec-marking-aicore-0.1.3/setup.py
```

### Comparing `movie-rec-marking-aicore-0.1.2/movie_rec_marking/test_milestone_1.py` & `movie-rec-marking-aicore-0.1.3/movie_rec_marking/test_milestone_1.py`

 * *Files identical despite different names*

### Comparing `movie-rec-marking-aicore-0.1.2/movie_rec_marking/test_milestone_2.py` & `movie-rec-marking-aicore-0.1.3/movie_rec_marking/test_milestone_2.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,17 +25,27 @@
         if len(title) > length_of_longest_movie_title:
             length_of_longest_movie_title = len(title)
             title_of_movie_with_longest_title = title
     return length_of_longest_movie_title, title_of_movie_with_longest_title
 
 def check_print_every_movie_title(func):
     # Check that the function prints every movie name
-    with patch('sys.stdout', new=StringIO()) as fake_out:
-        func()
-        output = fake_out.getvalue()
+    try:
+        with patch('sys.stdout', new=StringIO()) as fake_out:
+            func()
+            output = fake_out.getvalue()
+    except TypeError:
+        with patch('sys.stdout', new=StringIO()) as fake_out:
+            func(movies)
+            output = fake_out.getvalue()
+    except Exception as e:
+        print("Running the function results in an error")
+        print('Check the error here: ', e)
+        print('Please, try again, and don\'t continue until you get the correct output')
+        return False
     
     if not output:
         print("The function doesn't print anything")
         print('Please, try again, and don\'t continue until you get the correct output')
         return False
 
     movie_list = ['The Shawshank Redemption',
@@ -85,14 +95,16 @@
 
 def check_get_avg_movie_description_length(func, task_2):
     if not task_2:
         print("You haven't completed the previous task correctly")
         return False
     try:
         actual = func()
+    except TypeError:
+        actual = func(movies)
     except Exception as e:
         print('Running the "get_avg_movie_description_length" function results in an error')
         print('Check the error here: ', e)
         print('Please, try again, and don\'t continue until you get the correct output')
         return False
     if not actual:
         print("The function doesn't return anything")
@@ -115,14 +127,16 @@
 
 def check_get_max_movie_name_length(func, task_3):
     if not task_3:
         print("You haven't completed the previous task correctly")
         return False
     try:
         actual = func()
+    except TypeError:
+        actual = func(movies)
     except Exception as e:
         print('Running the "get_max_movie_name_length" function results in an error')
         print('Check the error here: ', e)
         print('Please, try again, and don\'t continue until you get the correct output')
         return False
     if not actual:
         print("The function doesn't return anything")
@@ -147,8 +161,8 @@
         return False
     elif actual[1] != expected[1]:
         print('The "get_max_movie_name_length" function doesn\'t return the correct movie name')
         print('Please, try again, and don\'t continue until you get the correct output')
         return False
     else:
         print('Great! The "get_max_movie_name_length" function returns the correct maximum length of the movie name: ', actual)
-        print('Nice job! You have complete the second milestone of the project!')
+        print('Nice job! You have complete the second milestone of the project!')
```

### Comparing `movie-rec-marking-aicore-0.1.2/movie_rec_marking/test_milestone_3.py` & `movie-rec-marking-aicore-0.1.3/movie_rec_marking/test_milestone_3.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 
 def get_movies_in_genre(genre):
     return [movie for movie in movies if movie["genre"] == genre]
 
 def check_load_movies_data(func):
     try:
         movies_in = func()
+    except TypeError:
+        movies_in = func(movies)
     except:
         print('The "load_movies_data" function is not defined correctly')
         print('Make sure you can run it without any errors, and that the function doesn\'t take any arguments')
         print('Please, try again, and don\'t continue until you get the correct output')
         return False
 
     if not movies_in:
@@ -51,14 +53,16 @@
 def check_get_unique_genres(func, task_1):
     if not task_1:
         print('Please, complete the previous task before continuing')
         return False
     # The function should return a set of unique genres
     try:
         genres = func()
+    except TypeError:
+        genres = func(movies)
     except:
         print('The "get_unique_genres" function is not defined correctly')
         print('Make sure you can run it without any errors, and that the function doesn\'t take any arguments')
         print('Please, try again, and don\'t continue until you get the correct output')
         return False
 
     if not genres:
@@ -115,8 +119,8 @@
             print('The "get_movies_in_genre" function doesn\'t return the correct number of movies')
             print(f'There should be {len(movies_genre)} movies in the "{genre}" genre, but your function returns {len(movies_in)}')
             print('Please, try again, and don\'t continue until you get the correct output')
             return False
 
     else:
         print('Great! The "get_movies_in_genre" function returns the correct number of movies')
-        print('Amazing! You have complete the third milestone of the project! Two more to go!')
+        print('Amazing! You have complete the third milestone of the project! Two more to go!')
```

### Comparing `movie-rec-marking-aicore-0.1.2/movie_rec_marking/test_milestone_4.py` & `movie-rec-marking-aicore-0.1.3/movie_rec_marking/test_milestone_4.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,14 @@
     except:
         print('The "get_movie_by_index" function is not defined correctly')
         print('Make sure you call the "get_unique_genres" and "get_unique_genres" functions inside the "get_movie_by_index" function')
         print('Make sure you can run it without any errors, and that the function doesn\'t take any arguments')
         print('Please, try again, and don\'t continue until you get the correct output')
         return False
 
-
     if movie:
         print('The "get_movie_by_index" should not return anything, but just print the movie')
         print('Please, try again, and don\'t continue until you get the correct output')
         return False
 
     output = f.getvalue()
     if 'description' not in output:
```

### Comparing `movie-rec-marking-aicore-0.1.2/movie_rec_marking/test_milestone_5.py` & `movie-rec-marking-aicore-0.1.3/movie_rec_marking/test_milestone_5.py`

 * *Files identical despite different names*

