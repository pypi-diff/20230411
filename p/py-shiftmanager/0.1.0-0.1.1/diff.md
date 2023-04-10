# Comparing `tmp/py_shiftmanager-0.1.0.tar.gz` & `tmp/py_shiftmanager-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_shiftmanager-0.1.0.tar", last modified: Sun Apr  9 14:34:38 2023, max compression
+gzip compressed data, was "py_shiftmanager-0.1.1.tar", last modified: Mon Apr 10 23:50:06 2023, max compression
```

## Comparing `py_shiftmanager-0.1.0.tar` & `py_shiftmanager-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-09 14:34:38.305058 py_shiftmanager-0.1.0/
--rw-r--r--   0 amitnakash   (501) staff       (20)      318 2023-04-09 14:34:38.304863 py_shiftmanager-0.1.0/PKG-INFO
-drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-09 14:34:38.303695 py_shiftmanager-0.1.0/py_shiftmanager/
--rw-r--r--   0 amitnakash   (501) staff       (20)      312 2023-04-09 14:15:13.000000 py_shiftmanager-0.1.0/py_shiftmanager/__init__.py
--rw-r--r--   0 amitnakash   (501) staff       (20)       42 2023-04-09 13:34:58.000000 py_shiftmanager-0.1.0/py_shiftmanager/exceptions.py
--rw-r--r--   0 amitnakash   (501) staff       (20)      428 2023-04-09 13:34:58.000000 py_shiftmanager-0.1.0/py_shiftmanager/logger.py
--rw-r--r--   0 amitnakash   (501) staff       (20)     4274 2023-04-09 14:34:19.000000 py_shiftmanager-0.1.0/py_shiftmanager/shiftmanager_compute.py
--rw-r--r--   0 amitnakash   (501) staff       (20)     4538 2023-04-09 14:21:30.000000 py_shiftmanager-0.1.0/py_shiftmanager/shiftmanager_io.py
--rw-r--r--   0 amitnakash   (501) staff       (20)     2607 2023-04-09 13:43:25.000000 py_shiftmanager-0.1.0/py_shiftmanager/worker.py
-drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-09 14:34:38.304628 py_shiftmanager-0.1.0/py_shiftmanager.egg-info/
--rw-r--r--   0 amitnakash   (501) staff       (20)      318 2023-04-09 14:34:38.000000 py_shiftmanager-0.1.0/py_shiftmanager.egg-info/PKG-INFO
--rw-r--r--   0 amitnakash   (501) staff       (20)      387 2023-04-09 14:34:38.000000 py_shiftmanager-0.1.0/py_shiftmanager.egg-info/SOURCES.txt
--rw-r--r--   0 amitnakash   (501) staff       (20)        1 2023-04-09 14:34:38.000000 py_shiftmanager-0.1.0/py_shiftmanager.egg-info/dependency_links.txt
--rw-r--r--   0 amitnakash   (501) staff       (20)       12 2023-04-09 14:34:38.000000 py_shiftmanager-0.1.0/py_shiftmanager.egg-info/requires.txt
--rw-r--r--   0 amitnakash   (501) staff       (20)       16 2023-04-09 14:34:38.000000 py_shiftmanager-0.1.0/py_shiftmanager.egg-info/top_level.txt
--rw-r--r--   0 amitnakash   (501) staff       (20)       38 2023-04-09 14:34:38.305119 py_shiftmanager-0.1.0/setup.cfg
--rw-r--r--   0 amitnakash   (501) staff       (20)      477 2023-04-09 14:34:19.000000 py_shiftmanager-0.1.0/setup.py
+drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-10 23:50:06.357824 py_shiftmanager-0.1.1/
+-rw-r--r--   0 amitnakash   (501) staff       (20)       17 2023-04-10 17:56:51.000000 py_shiftmanager-0.1.1/MANIFEST.in
+-rw-r--r--   0 amitnakash   (501) staff       (20)     6483 2023-04-10 23:50:06.357723 py_shiftmanager-0.1.1/PKG-INFO
+-rw-r--r--   0 amitnakash   (501) staff       (20)     6164 2023-04-10 23:46:28.000000 py_shiftmanager-0.1.1/Readme.md
+drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-10 23:50:06.356930 py_shiftmanager-0.1.1/py_shiftmanager/
+-rw-r--r--   0 amitnakash   (501) staff       (20)      370 2023-04-10 21:43:31.000000 py_shiftmanager-0.1.1/py_shiftmanager/__init__.py
+-rw-r--r--   0 amitnakash   (501) staff       (20)       42 2023-04-09 13:34:58.000000 py_shiftmanager-0.1.1/py_shiftmanager/exceptions.py
+-rw-r--r--   0 amitnakash   (501) staff       (20)      428 2023-04-09 13:34:58.000000 py_shiftmanager-0.1.1/py_shiftmanager/logger.py
+-rw-r--r--   0 amitnakash   (501) staff       (20)     4300 2023-04-10 23:44:55.000000 py_shiftmanager-0.1.1/py_shiftmanager/shiftmanager_compute.py
+-rw-r--r--   0 amitnakash   (501) staff       (20)     4637 2023-04-10 20:29:30.000000 py_shiftmanager-0.1.1/py_shiftmanager/shiftmanager_io.py
+-rw-r--r--   0 amitnakash   (501) staff       (20)      820 2023-04-10 23:44:58.000000 py_shiftmanager-0.1.1/py_shiftmanager/timeout.py
+-rw-r--r--   0 amitnakash   (501) staff       (20)     3273 2023-04-10 23:44:53.000000 py_shiftmanager-0.1.1/py_shiftmanager/worker.py
+drwxr-xr-x   0 amitnakash   (501) staff       (20)        0 2023-04-10 23:50:06.357553 py_shiftmanager-0.1.1/py_shiftmanager.egg-info/
+-rw-r--r--   0 amitnakash   (501) staff       (20)     6483 2023-04-10 23:50:06.000000 py_shiftmanager-0.1.1/py_shiftmanager.egg-info/PKG-INFO
+-rw-r--r--   0 amitnakash   (501) staff       (20)      436 2023-04-10 23:50:06.000000 py_shiftmanager-0.1.1/py_shiftmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 amitnakash   (501) staff       (20)        1 2023-04-10 23:50:06.000000 py_shiftmanager-0.1.1/py_shiftmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 amitnakash   (501) staff       (20)       12 2023-04-10 23:50:06.000000 py_shiftmanager-0.1.1/py_shiftmanager.egg-info/requires.txt
+-rw-r--r--   0 amitnakash   (501) staff       (20)       16 2023-04-10 23:50:06.000000 py_shiftmanager-0.1.1/py_shiftmanager.egg-info/top_level.txt
+-rw-r--r--   0 amitnakash   (501) staff       (20)       38 2023-04-10 23:50:06.357857 py_shiftmanager-0.1.1/setup.cfg
+-rw-r--r--   0 amitnakash   (501) staff       (20)      591 2023-04-10 23:50:02.000000 py_shiftmanager-0.1.1/setup.py
```

### Comparing `py_shiftmanager-0.1.0/py_shiftmanager/shiftmanager_compute.py` & `py_shiftmanager-0.1.1/py_shiftmanager/shiftmanager_compute.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 logger = Logger()
 
 
 class ShiftManager_Compute(ShiftManager_IO):
     pool: multiprocessing.Pool
 
-    def __init__(self, num_of_workers: int = 1, daemon: bool = False, queue_size: int = 10) -> NoReturn:
+    def __init__(self, num_of_workers: int = multiprocessing.cpu_count(), daemon: bool = False, queue_size: int = 10) -> NoReturn:
         super().__init__(num_of_workers, daemon)
         self._q_in = multiprocessing.JoinableQueue(maxsize=queue_size)
         self._q_out = multiprocessing.Queue(maxsize=int(queue_size * 1.5))
         self.worker = Worker_COM()
         self.workers = []
         self._lock = multiprocessing.Lock()
```

### Comparing `py_shiftmanager-0.1.0/py_shiftmanager/shiftmanager_io.py` & `py_shiftmanager-0.1.1/py_shiftmanager/shiftmanager_io.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 class ShiftManager_IO:
     _num_of_workers: int
     _q_in: queue.Queue
     _q_out: multiprocessing.Queue
 
-    def __init__(self, num_of_workers: int = 1, daemon: bool = False, queue_size: int = 10) -> NoReturn:
+    def __init__(self, num_of_workers: int = 2, daemon: bool = False, queue_size: int = 10) -> NoReturn:
         self._num_of_workers = num_of_workers
         self.daemon = daemon
         self.queue_size = queue_size
         self._q_in = queue.Queue(maxsize=self.queue_size)
         self._q_out = multiprocessing.Queue(maxsize=int(self.queue_size * 1.5))
         self.worker = Worker_IO()
         self.workers = []
@@ -54,15 +54,16 @@
     def __divmod__(self, x: int) -> NoReturn:
         self._num_of_workers /= x
 
     """ Task and queue management """
     def new_task(self, func: Callable, *args) -> NoReturn:
         new_task = {"arrival_time": int(datetime.datetime.now().timestamp()), "func": dill.dumps(func), "args": args}
         try:
-            self._q_in.put(new_task)
+            with self._lock:
+                self._q_in.put(new_task)
         except QueueFullError:
             logger.logger.warn("INPUT-QUEUE IS FULL.")
 
     def new_batch(self, tasks: List[tuple]) -> NoReturn:
         for task in tasks:
             self.new_task(*task)
 
@@ -87,27 +88,28 @@
 
         if self._q_in.qsize() > 0:
             self._q_in.join()
 
     def get_results(self) -> List:
         # self._q_in.join()
         results = []
-        while not self._q_out.empty():
-            results.append(self._q_out.get())
+        with self._lock:
+            while not self._q_out.empty():
+                results.append(self._q_out.get())
         return results
 
     def join_all_workers(self) -> NoReturn:
         for worker in self.workers:
             worker.join()
 
     def end_shift(self) -> NoReturn:
         self._q_in.join()
-        # self.flush_queue()
-        for _ in range(self._num_of_workers):
-            self._q_in.put(None)
+        with self._lock:
+            for _ in range(self._num_of_workers):
+                self._q_in.put(None)
         self.join_all_workers()
         self.workers.clear()
         self.flush_queue()
 
     # def del_task(self, task: Any) -> NoReturn:
     #     temp_queue = queue.Queue()
     #     with self._lock:
@@ -118,15 +120,16 @@
     #                 continue
     #             temp_queue.put(current_item)
     #
     #         while not temp_queue.empty():
     #             self._q_in.put(temp_queue.get())
 
     def flush_queue(self) -> NoReturn:
-        self._q_in.queue.clear()
+        with self._lock:
+            self._q_in.queue.clear()
 
     def autoscale(self, arrival_rate: float, avg_queue_time: float, avg_service_time: float) -> NoReturn:
         """
         [!] Currently unavailable.
 
         This method auto-calculates the number of workers/processes needed for the kind of tasks provided -
         and auto-scales them each time it's called.
```

