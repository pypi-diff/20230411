# Comparing `tmp/py_shiftmanager-0.1.1.tar.gz` & `tmp/py_shiftmanager-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_shiftmanager-0.1.1.tar", last modified: Mon Apr 10 23:50:06 2023, max compression
+gzip compressed data, was "py_shiftmanager-0.1.2.tar", last modified: Tue Apr 11 13:06:53 2023, max compression
```

## Comparing `py_shiftmanager-0.1.1.tar` & `py_shiftmanager-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-10 23:50:06.357824 py_shiftmanager-0.1.1/
--rw-r--r--   0 amitnakash   (501) staff       (20)       17 2023-04-10 17:56:51.000000 py_shiftmanager-0.1.1/MANIFEST.in
--rw-r--r--   0 amitnakash   (501) staff       (20)     6483 2023-04-10 23:50:06.357723 py_shiftmanager-0.1.1/PKG-INFO
--rw-r--r--   0 amitnakash   (501) staff       (20)     6164 2023-04-10 23:46:28.000000 py_shiftmanager-0.1.1/Readme.md
-drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-10 23:50:06.356930 py_shiftmanager-0.1.1/py_shiftmanager/
--rw-r--r--   0 amitnakash   (501) staff       (20)      370 2023-04-10 21:43:31.000000 py_shiftmanager-0.1.1/py_shiftmanager/__init__.py
--rw-r--r--   0 amitnakash   (501) staff       (20)       42 2023-04-09 13:34:58.000000 py_shiftmanager-0.1.1/py_shiftmanager/exceptions.py
--rw-r--r--   0 amitnakash   (501) staff       (20)      428 2023-04-09 13:34:58.000000 py_shiftmanager-0.1.1/py_shiftmanager/logger.py
--rw-r--r--   0 amitnakash   (501) staff       (20)     4300 2023-04-10 23:44:55.000000 py_shiftmanager-0.1.1/py_shiftmanager/shiftmanager_compute.py
--rw-r--r--   0 amitnakash   (501) staff       (20)     4637 2023-04-10 20:29:30.000000 py_shiftmanager-0.1.1/py_shiftmanager/shiftmanager_io.py
--rw-r--r--   0 amitnakash   (501) staff       (20)      820 2023-04-10 23:44:58.000000 py_shiftmanager-0.1.1/py_shiftmanager/timeout.py
--rw-r--r--   0 amitnakash   (501) staff       (20)     3273 2023-04-10 23:44:53.000000 py_shiftmanager-0.1.1/py_shiftmanager/worker.py
-drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-10 23:50:06.357553 py_shiftmanager-0.1.1/py_shiftmanager.egg-info/
--rw-r--r--   0 amitnakash   (501) staff       (20)     6483 2023-04-10 23:50:06.000000 py_shiftmanager-0.1.1/py_shiftmanager.egg-info/PKG-INFO
--rw-r--r--   0 amitnakash   (501) staff       (20)      436 2023-04-10 23:50:06.000000 py_shiftmanager-0.1.1/py_shiftmanager.egg-info/SOURCES.txt
--rw-r--r--   0 amitnakash   (501) staff       (20)        1 2023-04-10 23:50:06.000000 py_shiftmanager-0.1.1/py_shiftmanager.egg-info/dependency_links.txt
--rw-r--r--   0 amitnakash   (501) staff       (20)       12 2023-04-10 23:50:06.000000 py_shiftmanager-0.1.1/py_shiftmanager.egg-info/requires.txt
--rw-r--r--   0 amitnakash   (501) staff       (20)       16 2023-04-10 23:50:06.000000 py_shiftmanager-0.1.1/py_shiftmanager.egg-info/top_level.txt
--rw-r--r--   0 amitnakash   (501) staff       (20)       38 2023-04-10 23:50:06.357857 py_shiftmanager-0.1.1/setup.cfg
--rw-r--r--   0 amitnakash   (501) staff       (20)      591 2023-04-10 23:50:02.000000 py_shiftmanager-0.1.1/setup.py
+drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-11 13:06:53.229206 py_shiftmanager-0.1.2/
+-rw-r--r--   0 amitnakash   (501) staff       (20)       17 2023-04-11 08:18:28.000000 py_shiftmanager-0.1.2/MANIFEST.in
+-rw-r--r--   0 amitnakash   (501) staff       (20)     6976 2023-04-11 13:06:53.229054 py_shiftmanager-0.1.2/PKG-INFO
+-rw-r--r--   0 amitnakash   (501) staff       (20)     6657 2023-04-11 12:49:14.000000 py_shiftmanager-0.1.2/Readme.md
+drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-11 13:06:53.227995 py_shiftmanager-0.1.2/py_shiftmanager/
+-rw-r--r--   0 amitnakash   (501) staff       (20)      370 2023-04-11 08:18:28.000000 py_shiftmanager-0.1.2/py_shiftmanager/__init__.py
+-rw-r--r--   0 amitnakash   (501) staff       (20)       42 2023-04-09 13:34:58.000000 py_shiftmanager-0.1.2/py_shiftmanager/exceptions.py
+-rw-r--r--   0 amitnakash   (501) staff       (20)      428 2023-04-09 13:34:58.000000 py_shiftmanager-0.1.2/py_shiftmanager/logger.py
+-rw-r--r--   0 amitnakash   (501) staff       (20)     4794 2023-04-11 13:05:25.000000 py_shiftmanager-0.1.2/py_shiftmanager/shiftmanager_compute.py
+-rw-r--r--   0 amitnakash   (501) staff       (20)     5100 2023-04-11 13:05:35.000000 py_shiftmanager-0.1.2/py_shiftmanager/shiftmanager_io.py
+-rw-r--r--   0 amitnakash   (501) staff       (20)      820 2023-04-11 08:18:28.000000 py_shiftmanager-0.1.2/py_shiftmanager/timeout.py
+-rw-r--r--   0 amitnakash   (501) staff       (20)     3273 2023-04-11 08:18:28.000000 py_shiftmanager-0.1.2/py_shiftmanager/worker.py
+drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-11 13:06:53.228842 py_shiftmanager-0.1.2/py_shiftmanager.egg-info/
+-rw-r--r--   0 amitnakash   (501) staff       (20)     6976 2023-04-11 13:06:53.000000 py_shiftmanager-0.1.2/py_shiftmanager.egg-info/PKG-INFO
+-rw-r--r--   0 amitnakash   (501) staff       (20)      436 2023-04-11 13:06:53.000000 py_shiftmanager-0.1.2/py_shiftmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 amitnakash   (501) staff       (20)        1 2023-04-11 13:06:53.000000 py_shiftmanager-0.1.2/py_shiftmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 amitnakash   (501) staff       (20)       12 2023-04-11 13:06:53.000000 py_shiftmanager-0.1.2/py_shiftmanager.egg-info/requires.txt
+-rw-r--r--   0 amitnakash   (501) staff       (20)       16 2023-04-11 13:06:53.000000 py_shiftmanager-0.1.2/py_shiftmanager.egg-info/top_level.txt
+-rw-r--r--   0 amitnakash   (501) staff       (20)       38 2023-04-11 13:06:53.229251 py_shiftmanager-0.1.2/setup.cfg
+-rw-r--r--   0 amitnakash   (501) staff       (20)      591 2023-04-11 12:49:38.000000 py_shiftmanager-0.1.2/setup.py
```

### Comparing `py_shiftmanager-0.1.1/PKG-INFO` & `py_shiftmanager-0.1.2/py_shiftmanager.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 Metadata-Version: 2.1
-Name: py_shiftmanager
-Version: 0.1.1
+Name: py-shiftmanager
+Version: 0.1.2
 Summary: A simplified, all-in-one shop for handling multithreading/multiprocessing using a managed queue system.
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 
 # Py-ShiftManager
-#### v0.1.1
+#### v0.1.2
 
 Py-ShiftManager is a Python module that provides a managed queue environment for handling IO and computational tasks, allowing you to easily manage concurrency and multiprocessing without worrying about the details.
 
 ## Installation
 You can install Py-ShiftManager using pip:
 `pip install py-shiftmanager`
 
 ## What's new in v0.1.1
-This small update is dedicaded to my friend Ram :).
+This small update is dedicated to my friend Ram Manor :).
 * Introducing new timeout wrapper: *timeout_timer* - import it, decorate your functions, set amount of seconds, get a result for a task that has timed out without blocking your flow. 
 * Better thread locking system to ensure even smaller chances of getting in a deadlock situation.  
 * *ShiftManager_Compute* now initializes the number of workers with the number of CPU's available in the system, by default.  
 * *ShiftManager_IO* now initializes the number of workers to 2, instead of 1, by default.  
+### New for v0.1.2
+* New context manager for *ShiftManager* - use the `with` keyword and get all the benefits of *ShiftManager* for a specific set of tasks, for even less lines of code!    
+`with ShiftManager_Compute() as manager:`  
+`   manager.new_task(lambda x: x**2, 4)`  
+`   manager.new_task(lambda x: x**4, 13)`  
+then get the results:  
+`results = manager.get_results()`  
+It's that simple.  
 
 ## Usage
 Here's an example of how to use Py-ShiftManager to handle IO tasks:  
 `from py-shiftmanager import ShiftManager_IO`.  
 Now, lets also import *timeout_timer* wrapper:  
 `from py-shiftmanager.timeout import timeout_timer`
 
@@ -32,29 +40,31 @@
 `manager = ShiftManager_IO(num_of_workers=4)`  
 
 **Note**: by default *ShiftManager* objects init with these values for its attributes:
 * num_of_workers = `2`
 * daemon = `False`
 * queue size = `10`    
 
-Also, by default the output queue is sent to 1.5 times the input queue size.
+Also, by default the output queue is set to 1.5 times the input queue size.
   
 # Add some tasks to the input queue
-Assume we have created a function and applied the *timeout_timer* decorator, incase a task takes longer than 3 seconds to complete, like so:  
+Assume we have created a function and applied the *timeout_timer* decorator, with a 3 seconds timeout counter, in case a task takes longer than 3 seconds to complete, like so:  
 `import requests`  
 `@timeout_timer(seconds=3)`  
 `def get_status(url):`  
 `   return requests.get(url).status_code`  
 We can assign single tasks to the queue:  
 `manager.new_task(get_status, "http://www.google.com")`  
 `manager.new_task(get_status, "http://www.facebook.com")`  
 `manager.new_task(get_status, "http://www.twitter.com")`   
 Or we can submit a batch by passing a list of tuples:  
 `tasks = [(get_status, "http://www.google.com"),(get_status, "http://www.facebook.com")]`  
-`manager.new_batch(tasks)`
+`manager.new_batch(tasks)`  
+  
+**Note**: you can also pass *lambda* functions.
 
 # Handle the tasks
 `manager.handle_work()`  
 *ShiftManager* spins up the workers and starts consuming tasks from the input queue.  
 Since we applied the *timeout_timer* decorator, if a task takes longer than 3 seconds - it will be terminated, but you'll still recieve a result with the task details, and that it has ran out of time.  
 
 # Wait for the tasks to complete
@@ -152,10 +162,9 @@
 `get_results() -> List`  
 Returns the results of the completed tasks from the output queue.
 
 `end_shift() -> None`  
 Ends the shift and waits for all tasks to complete.  
 
 **timeout_timer**  
-
 `@timeout_timer(seconds: int = 5)`  
 A decorator that attaches a timeout counter to your methods, use it to set a time limit to tasks in seconds; 5 seconds by default.
```

### Comparing `py_shiftmanager-0.1.1/Readme.md` & `py_shiftmanager-0.1.2/Readme.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 # Py-ShiftManager
-#### v0.1.1
+#### v0.1.2
 
 Py-ShiftManager is a Python module that provides a managed queue environment for handling IO and computational tasks, allowing you to easily manage concurrency and multiprocessing without worrying about the details.
 
 ## Installation
 You can install Py-ShiftManager using pip:
 `pip install py-shiftmanager`
 
 ## What's new in v0.1.1
-This small update is dedicaded to my friend Ram :).
+This small update is dedicated to my friend Ram Manor :).
 * Introducing new timeout wrapper: *timeout_timer* - import it, decorate your functions, set amount of seconds, get a result for a task that has timed out without blocking your flow. 
 * Better thread locking system to ensure even smaller chances of getting in a deadlock situation.  
 * *ShiftManager_Compute* now initializes the number of workers with the number of CPU's available in the system, by default.  
 * *ShiftManager_IO* now initializes the number of workers to 2, instead of 1, by default.  
+### New for v0.1.2
+* New context manager for *ShiftManager* - use the `with` keyword and get all the benefits of *ShiftManager* for a specific set of tasks, for even less lines of code!    
+`with ShiftManager_Compute() as manager:`  
+`   manager.new_task(lambda x: x**2, 4)`  
+`   manager.new_task(lambda x: x**4, 13)`  
+then get the results:  
+`results = manager.get_results()`  
+It's that simple.  
 
 ## Usage
 Here's an example of how to use Py-ShiftManager to handle IO tasks:  
 `from py-shiftmanager import ShiftManager_IO`.  
 Now, lets also import *timeout_timer* wrapper:  
 `from py-shiftmanager.timeout import timeout_timer`
 
@@ -24,29 +32,31 @@
 `manager = ShiftManager_IO(num_of_workers=4)`  
 
 **Note**: by default *ShiftManager* objects init with these values for its attributes:
 * num_of_workers = `2`
 * daemon = `False`
 * queue size = `10`    
 
-Also, by default the output queue is sent to 1.5 times the input queue size.
+Also, by default the output queue is set to 1.5 times the input queue size.
   
 # Add some tasks to the input queue
-Assume we have created a function and applied the *timeout_timer* decorator, incase a task takes longer than 3 seconds to complete, like so:  
+Assume we have created a function and applied the *timeout_timer* decorator, with a 3 seconds timeout counter, in case a task takes longer than 3 seconds to complete, like so:  
 `import requests`  
 `@timeout_timer(seconds=3)`  
 `def get_status(url):`  
 `   return requests.get(url).status_code`  
 We can assign single tasks to the queue:  
 `manager.new_task(get_status, "http://www.google.com")`  
 `manager.new_task(get_status, "http://www.facebook.com")`  
 `manager.new_task(get_status, "http://www.twitter.com")`   
 Or we can submit a batch by passing a list of tuples:  
 `tasks = [(get_status, "http://www.google.com"),(get_status, "http://www.facebook.com")]`  
-`manager.new_batch(tasks)`
+`manager.new_batch(tasks)`  
+  
+**Note**: you can also pass *lambda* functions.
 
 # Handle the tasks
 `manager.handle_work()`  
 *ShiftManager* spins up the workers and starts consuming tasks from the input queue.  
 Since we applied the *timeout_timer* decorator, if a task takes longer than 3 seconds - it will be terminated, but you'll still recieve a result with the task details, and that it has ran out of time.  
 
 # Wait for the tasks to complete
@@ -144,10 +154,9 @@
 `get_results() -> List`  
 Returns the results of the completed tasks from the output queue.
 
 `end_shift() -> None`  
 Ends the shift and waits for all tasks to complete.  
 
 **timeout_timer**  
-
 `@timeout_timer(seconds: int = 5)`  
 A decorator that attaches a timeout counter to your methods, use it to set a time limit to tasks in seconds; 5 seconds by default.
```

### Comparing `py_shiftmanager-0.1.1/py_shiftmanager/shiftmanager_compute.py` & `py_shiftmanager-0.1.2/py_shiftmanager/shiftmanager_compute.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,24 @@
     def __init__(self, num_of_workers: int = multiprocessing.cpu_count(), daemon: bool = False, queue_size: int = 10) -> NoReturn:
         super().__init__(num_of_workers, daemon)
         self._q_in = multiprocessing.JoinableQueue(maxsize=queue_size)
         self._q_out = multiprocessing.Queue(maxsize=int(queue_size * 1.5))
         self.worker = Worker_COM()
         self.workers = []
         self._lock = multiprocessing.Lock()
+        
+    def __enter__(self, num_of_workers: int = multiprocessing.cpu_count(), daemon: bool = False, queue_size: int = 10):
+        self.manager = ShiftManager_Compute(num_of_workers, daemon, queue_size)
+        return self.manager
+    
+    def __exit__(self, exc_type, exc_val, exc_tb) -> NoReturn:
+        if exc_type is not None:
+            logger.logger.error(f"An exception of type {exc_type} occurred: {exc_val}")
+        self.manager.handle_work()
+        self.manager.end_shift()
 
     def __repr__(self):
         return f"""ShiftManagerCOM;daemonized={self.daemon};workers={self._num_of_workers}"""
 
     """ Manual scaling of workers """
     def __add__(self, x: int) -> NoReturn:
         super().__add__(x)
```

### Comparing `py_shiftmanager-0.1.1/py_shiftmanager/shiftmanager_io.py` & `py_shiftmanager-0.1.2/py_shiftmanager/shiftmanager_io.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,24 @@
         self.daemon = daemon
         self.queue_size = queue_size
         self._q_in = queue.Queue(maxsize=self.queue_size)
         self._q_out = multiprocessing.Queue(maxsize=int(self.queue_size * 1.5))
         self.worker = Worker_IO()
         self.workers = []
         self._lock = threading.Lock()
+        
+    def __enter__(self, num_of_workers: int = 2, daemon: bool = False, queue_size: int = 10):
+        self.manager = ShiftManager_IO(num_of_workers, daemon, queue_size)
+        return self.manager
+    
+    def __exit__(self, exc_type, exc_val, exc_tb) -> NoReturn:
+        if exc_type is not None:
+            logger.logger.error(f"An exception of type {exc_type} occurred: {exc_val}")
+        self.manager.handle_work()
+        self.manager.end_shift()
 
     def __repr__(self):
         return f"""ShiftManagerIO;daemonized={self.daemon};workers={self._num_of_workers}"""
 
     """ Manual scaling of workers """
     def __add__(self, x: int) -> NoReturn:
         self._num_of_workers += x
```

### Comparing `py_shiftmanager-0.1.1/py_shiftmanager/timeout.py` & `py_shiftmanager-0.1.2/py_shiftmanager/timeout.py`

 * *Files identical despite different names*

### Comparing `py_shiftmanager-0.1.1/py_shiftmanager/worker.py` & `py_shiftmanager-0.1.2/py_shiftmanager/worker.py`

 * *Files identical despite different names*

### Comparing `py_shiftmanager-0.1.1/py_shiftmanager.egg-info/PKG-INFO` & `py_shiftmanager-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 Metadata-Version: 2.1
-Name: py-shiftmanager
-Version: 0.1.1
+Name: py_shiftmanager
+Version: 0.1.2
 Summary: A simplified, all-in-one shop for handling multithreading/multiprocessing using a managed queue system.
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 
 # Py-ShiftManager
-#### v0.1.1
+#### v0.1.2
 
 Py-ShiftManager is a Python module that provides a managed queue environment for handling IO and computational tasks, allowing you to easily manage concurrency and multiprocessing without worrying about the details.
 
 ## Installation
 You can install Py-ShiftManager using pip:
 `pip install py-shiftmanager`
 
 ## What's new in v0.1.1
-This small update is dedicaded to my friend Ram :).
+This small update is dedicated to my friend Ram Manor :).
 * Introducing new timeout wrapper: *timeout_timer* - import it, decorate your functions, set amount of seconds, get a result for a task that has timed out without blocking your flow. 
 * Better thread locking system to ensure even smaller chances of getting in a deadlock situation.  
 * *ShiftManager_Compute* now initializes the number of workers with the number of CPU's available in the system, by default.  
 * *ShiftManager_IO* now initializes the number of workers to 2, instead of 1, by default.  
+### New for v0.1.2
+* New context manager for *ShiftManager* - use the `with` keyword and get all the benefits of *ShiftManager* for a specific set of tasks, for even less lines of code!    
+`with ShiftManager_Compute() as manager:`  
+`   manager.new_task(lambda x: x**2, 4)`  
+`   manager.new_task(lambda x: x**4, 13)`  
+then get the results:  
+`results = manager.get_results()`  
+It's that simple.  
 
 ## Usage
 Here's an example of how to use Py-ShiftManager to handle IO tasks:  
 `from py-shiftmanager import ShiftManager_IO`.  
 Now, lets also import *timeout_timer* wrapper:  
 `from py-shiftmanager.timeout import timeout_timer`
 
@@ -32,29 +40,31 @@
 `manager = ShiftManager_IO(num_of_workers=4)`  
 
 **Note**: by default *ShiftManager* objects init with these values for its attributes:
 * num_of_workers = `2`
 * daemon = `False`
 * queue size = `10`    
 
-Also, by default the output queue is sent to 1.5 times the input queue size.
+Also, by default the output queue is set to 1.5 times the input queue size.
   
 # Add some tasks to the input queue
-Assume we have created a function and applied the *timeout_timer* decorator, incase a task takes longer than 3 seconds to complete, like so:  
+Assume we have created a function and applied the *timeout_timer* decorator, with a 3 seconds timeout counter, in case a task takes longer than 3 seconds to complete, like so:  
 `import requests`  
 `@timeout_timer(seconds=3)`  
 `def get_status(url):`  
 `   return requests.get(url).status_code`  
 We can assign single tasks to the queue:  
 `manager.new_task(get_status, "http://www.google.com")`  
 `manager.new_task(get_status, "http://www.facebook.com")`  
 `manager.new_task(get_status, "http://www.twitter.com")`   
 Or we can submit a batch by passing a list of tuples:  
 `tasks = [(get_status, "http://www.google.com"),(get_status, "http://www.facebook.com")]`  
-`manager.new_batch(tasks)`
+`manager.new_batch(tasks)`  
+  
+**Note**: you can also pass *lambda* functions.
 
 # Handle the tasks
 `manager.handle_work()`  
 *ShiftManager* spins up the workers and starts consuming tasks from the input queue.  
 Since we applied the *timeout_timer* decorator, if a task takes longer than 3 seconds - it will be terminated, but you'll still recieve a result with the task details, and that it has ran out of time.  
 
 # Wait for the tasks to complete
@@ -152,10 +162,9 @@
 `get_results() -> List`  
 Returns the results of the completed tasks from the output queue.
 
 `end_shift() -> None`  
 Ends the shift and waits for all tasks to complete.  
 
 **timeout_timer**  
-
 `@timeout_timer(seconds: int = 5)`  
 A decorator that attaches a timeout counter to your methods, use it to set a time limit to tasks in seconds; 5 seconds by default.
```

### Comparing `py_shiftmanager-0.1.1/setup.py` & `py_shiftmanager-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 long_description = Path('Readme.md').read_text()
 
 setup(
     name='py_shiftmanager',
-    version='0.1.1',
+    version='0.1.2',
     description='A simplified, all-in-one shop for handling multithreading/multiprocessing using a managed queue system.',
     long_description=long_description,
     packages=find_packages(),
     install_requires=[
         'dill==0.3.6',
     ],
     classifiers=[
```

