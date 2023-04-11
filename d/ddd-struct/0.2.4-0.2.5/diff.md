# Comparing `tmp/ddd-struct-0.2.4.tar.gz` & `tmp/ddd-struct-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddd-struct-0.2.4.tar", last modified: Tue Apr 11 11:51:21 2023, max compression
+gzip compressed data, was "ddd-struct-0.2.5.tar", last modified: Tue Apr 11 16:27:15 2023, max compression
```

## Comparing `ddd-struct-0.2.4.tar` & `ddd-struct-0.2.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:51:21.266086 ddd-struct-0.2.4/
--rw-rw-rw-   0 root         (0) root         (0)     1091 2023-04-11 11:51:13.000000 ddd-struct-0.2.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      258 2023-04-11 11:51:21.266086 ddd-struct-0.2.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      299 2023-04-11 11:51:13.000000 ddd-struct-0.2.4/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 11:51:21.266086 ddd-struct-0.2.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      646 2023-04-11 11:51:13.000000 ddd-struct-0.2.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:51:21.258086 ddd-struct-0.2.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:51:21.262086 ddd-struct-0.2.4/src/ddd_struct/
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-04-11 11:51:13.000000 ddd-struct-0.2.4/src/ddd_struct/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:51:21.262086 ddd-struct-0.2.4/src/ddd_struct/application/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 11:51:13.000000 ddd-struct-0.2.4/src/ddd_struct/application/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8716 2023-04-11 11:51:13.000000 ddd-struct-0.2.4/src/ddd_struct/application/action.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:51:21.262086 ddd-struct-0.2.4/src/ddd_struct/domain/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 11:51:13.000000 ddd-struct-0.2.4/src/ddd_struct/domain/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-04-11 11:51:13.000000 ddd-struct-0.2.4/src/ddd_struct/domain/repository.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:51:21.262086 ddd-struct-0.2.4/src/ddd_struct/infrastructure/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 11:51:13.000000 ddd-struct-0.2.4/src/ddd_struct/infrastructure/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3870 2023-04-11 11:51:13.000000 ddd-struct-0.2.4/src/ddd_struct/infrastructure/repository_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:51:21.266086 ddd-struct-0.2.4/src/ddd_struct/lib/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-04-11 11:51:13.000000 ddd-struct-0.2.4/src/ddd_struct/lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1890 2023-04-11 11:51:13.000000 ddd-struct-0.2.4/src/ddd_struct/lib/common.py
--rw-rw-rw-   0 root         (0) root         (0)     5078 2023-04-11 11:51:13.000000 ddd-struct-0.2.4/src/ddd_struct/lib/thread.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-04-11 11:51:13.000000 ddd-struct-0.2.4/src/ddd_struct/lib/warning.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-11 11:51:13.000000 ddd-struct-0.2.4/src/ddd_struct/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:51:21.262086 ddd-struct-0.2.4/src/ddd_struct.egg-info/
--rw-r--r--   0 root         (0) root         (0)      258 2023-04-11 11:51:21.000000 ddd-struct-0.2.4/src/ddd_struct.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      624 2023-04-11 11:51:21.000000 ddd-struct-0.2.4/src/ddd_struct.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 11:51:21.000000 ddd-struct-0.2.4/src/ddd_struct.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-11 11:51:21.000000 ddd-struct-0.2.4/src/ddd_struct.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-11 11:51:21.000000 ddd-struct-0.2.4/src/ddd_struct.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:27:15.826456 ddd-struct-0.2.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2023-04-11 16:27:07.000000 ddd-struct-0.2.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      258 2023-04-11 16:27:15.822456 ddd-struct-0.2.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      299 2023-04-11 16:27:07.000000 ddd-struct-0.2.5/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 16:27:15.826456 ddd-struct-0.2.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      646 2023-04-11 16:27:07.000000 ddd-struct-0.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:27:15.802455 ddd-struct-0.2.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:27:15.822456 ddd-struct-0.2.5/src/ddd_struct/
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-04-11 16:27:07.000000 ddd-struct-0.2.5/src/ddd_struct/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:27:15.822456 ddd-struct-0.2.5/src/ddd_struct/application/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 16:27:07.000000 ddd-struct-0.2.5/src/ddd_struct/application/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8716 2023-04-11 16:27:07.000000 ddd-struct-0.2.5/src/ddd_struct/application/action.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:27:15.822456 ddd-struct-0.2.5/src/ddd_struct/domain/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 16:27:07.000000 ddd-struct-0.2.5/src/ddd_struct/domain/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-04-11 16:27:07.000000 ddd-struct-0.2.5/src/ddd_struct/domain/repository.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:27:15.822456 ddd-struct-0.2.5/src/ddd_struct/infrastructure/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 16:27:07.000000 ddd-struct-0.2.5/src/ddd_struct/infrastructure/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3870 2023-04-11 16:27:07.000000 ddd-struct-0.2.5/src/ddd_struct/infrastructure/repository_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:27:15.822456 ddd-struct-0.2.5/src/ddd_struct/lib/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-04-11 16:27:07.000000 ddd-struct-0.2.5/src/ddd_struct/lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1715 2023-04-11 16:27:07.000000 ddd-struct-0.2.5/src/ddd_struct/lib/common.py
+-rw-rw-rw-   0 root         (0) root         (0)     4696 2023-04-11 16:27:07.000000 ddd-struct-0.2.5/src/ddd_struct/lib/thread.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-04-11 16:27:07.000000 ddd-struct-0.2.5/src/ddd_struct/lib/warning.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-11 16:27:07.000000 ddd-struct-0.2.5/src/ddd_struct/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 16:27:15.822456 ddd-struct-0.2.5/src/ddd_struct.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-04-11 16:27:15.000000 ddd-struct-0.2.5/src/ddd_struct.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      624 2023-04-11 16:27:15.000000 ddd-struct-0.2.5/src/ddd_struct.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 16:27:15.000000 ddd-struct-0.2.5/src/ddd_struct.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-11 16:27:15.000000 ddd-struct-0.2.5/src/ddd_struct.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-11 16:27:15.000000 ddd-struct-0.2.5/src/ddd_struct.egg-info/top_level.txt
```

### Comparing `ddd-struct-0.2.4/LICENSE` & `ddd-struct-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ddd-struct-0.2.4/setup.py` & `ddd-struct-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `ddd-struct-0.2.4/src/ddd_struct/application/action.py` & `ddd-struct-0.2.5/src/ddd_struct/application/action.py`

 * *Files identical despite different names*

### Comparing `ddd-struct-0.2.4/src/ddd_struct/domain/repository.py` & `ddd-struct-0.2.5/src/ddd_struct/domain/repository.py`

 * *Files identical despite different names*

### Comparing `ddd-struct-0.2.4/src/ddd_struct/infrastructure/repository_impl.py` & `ddd-struct-0.2.5/src/ddd_struct/infrastructure/repository_impl.py`

 * *Files identical despite different names*

### Comparing `ddd-struct-0.2.4/src/ddd_struct/lib/common.py` & `ddd-struct-0.2.5/src/ddd_struct/lib/common.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,46 +11,41 @@
 
 
 def get_md5(txt):
     md5hash = hashlib.md5(str(txt).encode('utf-8'))
     return md5hash.hexdigest()
 
 def monitor_usage(sample_interval, func, *args, **kwargs):
-    def sample_func(sample_interval, stop_event, queue):
+    def sample_func(process, sample_interval, stop_event, queue):
         while not stop_event.is_set():
             time.sleep(sample_interval)
-            pid = os.getpid()
-            p = psutil.Process(pid)
-            cpu_percent = p.cpu_percent()
-            mem_info = p.memory_info()
+            cpu_percent = process.cpu_percent()
+            mem_info = process.memory_info()
             mem_usage = mem_info.rss / 1024 / 1024
             if queue.full():
                 queue.get()
             queue.put((cpu_percent, mem_usage))
 
     pid = os.getpid()
     p = psutil.Process(pid)
     init_cpu_percent = p.cpu_percent()
     mem_info = p.memory_info()
     init_mem_usage = mem_info.rss / 1024 / 1024
 
     stop_event = Event()
     queue = Queue(maxsize=1000)
-    proc = Process(target=sample_func, args=(sample_interval, stop_event, queue))
+    proc = Process(target=sample_func, args=(p, sample_interval, stop_event, queue))
     proc.start()
     ret = func(*args, **kwargs)
     stop_event.set()
     proc.join()
     cpus = []
     memories = []
-    cpu_count = psutil.cpu_count(logical=False)
     for i in range(queue.qsize()):
         cpu_percent, mem_usage = queue.get()
-        cpu_percent -= init_cpu_percent
         mem_usage -= init_mem_usage
-        cpu_usage = cpu_percent*cpu_count
-        cpus.append(cpu_usage)
+        cpus.append(cpu_percent)
         memories.append(mem_usage)
     stat = {'max_cpu_usage': max(cpus), 'max_mem_usage': max(memories), 
             'avg_cpu_usage': sum(cpus)/len(cpus), 'avg_mem_usage': sum(memories)/len(memories)}
     return ret, stat
```

### Comparing `ddd-struct-0.2.4/src/ddd_struct/lib/thread.py` & `ddd-struct-0.2.5/src/ddd_struct/lib/thread.py`

 * *Files 7% similar despite different names*

```diff
@@ -75,65 +75,56 @@
         for _ in range(1000000000):
             if (time.time()-start_time)>timeout:
                 self.ret_list_when_timeout = ret_list
                 raise ValueError(f'Fail to finish task in {timeout}s')
 
             # create task
             if len(runner)<self.n_workers and wait_list:
-                print('create task')
                 task_item:TaskItem = wait_list.pop()
                 task = self.create_task(task_item)
                 runner.append((task_item.index, task, task_item))
             else:
-                print('check task')
                 # check tasks
                 for i, (idx, task, item) in enumerate(runner):
                     if not task.done():
                         continue
                     succeed, result = self._get_task_result(task)
                     if succeed:
-                        print('succeed', result)
                         ret_list[idx] = result
                         runner[i] = None
                         if idx in self.failed: del self.failed[idx]
                     elif idx not in self.failed and item.retry>0:
-                        print('failed1', result)
                         assert idx==item.index
                         self.failed[idx] = 1
                         task = self.create_task(item)
                         runner[i] = (item.index, task, item)
                     elif idx in self.failed and self.failed[idx]<item.retry:
-                        print('failed2', result)
                         self.failed[idx] += 1
                         task = self.create_task(item)
                         runner[i] = (item.index, task, item)
                     else:
-                        print('failed3', result)
                         ret_list[idx] = result
                         runner[i] = None
                         if idx in self.failed: del self.failed[idx]
                 runner = [r for r in runner if r is not None]
 
                 #exit
                 if not runner and not wait_list:
-                    print(runner, wait_list)
-                    print('break')
                     break
                 await asyncio.sleep(delay)
         return ret_list
 
 
     def execute(self, delay=0, timeout=100, n_workers=None):
         if n_workers is not None:
             self.n_workers = n_workers
         wait_list = copy(self.wait_list)
 
         event_loop = asyncio.get_event_loop()
         ret_list = event_loop.run_until_complete(self.run(wait_list, delay, timeout))
-        print('finish')
         # ret_list = asyncio.run(run())
         self.wait_list = []
         return ret_list
     
 
     async def gather(self, delay=0, timeout=100, n_workers=None):
         if n_workers is not None:
```

### Comparing `ddd-struct-0.2.4/src/ddd_struct/lib/warning.py` & `ddd-struct-0.2.5/src/ddd_struct/lib/warning.py`

 * *Files identical despite different names*

### Comparing `ddd-struct-0.2.4/src/ddd_struct.egg-info/SOURCES.txt` & `ddd-struct-0.2.5/src/ddd_struct.egg-info/SOURCES.txt`

 * *Files identical despite different names*

