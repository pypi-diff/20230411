# Comparing `tmp/ddd-struct-0.2.2.tar.gz` & `tmp/ddd-struct-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddd-struct-0.2.2.tar", last modified: Fri Apr  7 06:19:56 2023, max compression
+gzip compressed data, was "ddd-struct-0.2.3.tar", last modified: Tue Apr 11 10:11:02 2023, max compression
```

## Comparing `ddd-struct-0.2.2.tar` & `ddd-struct-0.2.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 06:19:56.928193 ddd-struct-0.2.2/
--rw-rw-rw-   0 root         (0) root         (0)     1091 2023-04-07 06:19:47.000000 ddd-struct-0.2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      258 2023-04-07 06:19:56.928193 ddd-struct-0.2.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      299 2023-04-07 06:19:47.000000 ddd-struct-0.2.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-07 06:19:56.928193 ddd-struct-0.2.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-04-07 06:19:47.000000 ddd-struct-0.2.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 06:19:56.924193 ddd-struct-0.2.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 06:19:56.924193 ddd-struct-0.2.2/src/ddd_struct/
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-04-07 06:19:47.000000 ddd-struct-0.2.2/src/ddd_struct/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 06:19:56.928193 ddd-struct-0.2.2/src/ddd_struct/application/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-07 06:19:47.000000 ddd-struct-0.2.2/src/ddd_struct/application/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8716 2023-04-07 06:19:47.000000 ddd-struct-0.2.2/src/ddd_struct/application/action.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 06:19:56.928193 ddd-struct-0.2.2/src/ddd_struct/domain/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-07 06:19:47.000000 ddd-struct-0.2.2/src/ddd_struct/domain/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-04-07 06:19:47.000000 ddd-struct-0.2.2/src/ddd_struct/domain/repository.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 06:19:56.928193 ddd-struct-0.2.2/src/ddd_struct/infrastructure/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-07 06:19:47.000000 ddd-struct-0.2.2/src/ddd_struct/infrastructure/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3870 2023-04-07 06:19:47.000000 ddd-struct-0.2.2/src/ddd_struct/infrastructure/repository_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 06:19:56.928193 ddd-struct-0.2.2/src/ddd_struct/lib/
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-04-07 06:19:47.000000 ddd-struct-0.2.2/src/ddd_struct/lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-04-07 06:19:47.000000 ddd-struct-0.2.2/src/ddd_struct/lib/common.py
--rw-rw-rw-   0 root         (0) root         (0)     4542 2023-04-07 06:19:47.000000 ddd-struct-0.2.2/src/ddd_struct/lib/thread.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-04-07 06:19:47.000000 ddd-struct-0.2.2/src/ddd_struct/lib/warning.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-07 06:19:47.000000 ddd-struct-0.2.2/src/ddd_struct/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 06:19:56.924193 ddd-struct-0.2.2/src/ddd_struct.egg-info/
--rw-r--r--   0 root         (0) root         (0)      258 2023-04-07 06:19:56.000000 ddd-struct-0.2.2/src/ddd_struct.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      624 2023-04-07 06:19:56.000000 ddd-struct-0.2.2/src/ddd_struct.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 06:19:56.000000 ddd-struct-0.2.2/src/ddd_struct.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-07 06:19:56.000000 ddd-struct-0.2.2/src/ddd_struct.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-07 06:19:56.000000 ddd-struct-0.2.2/src/ddd_struct.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:11:02.548491 ddd-struct-0.2.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2023-04-11 10:10:55.000000 ddd-struct-0.2.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      258 2023-04-11 10:11:02.548491 ddd-struct-0.2.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      299 2023-04-11 10:10:55.000000 ddd-struct-0.2.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 10:11:02.552492 ddd-struct-0.2.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      646 2023-04-11 10:10:55.000000 ddd-struct-0.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:11:02.544491 ddd-struct-0.2.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:11:02.544491 ddd-struct-0.2.3/src/ddd_struct/
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-04-11 10:10:55.000000 ddd-struct-0.2.3/src/ddd_struct/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:11:02.548491 ddd-struct-0.2.3/src/ddd_struct/application/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 10:10:55.000000 ddd-struct-0.2.3/src/ddd_struct/application/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8716 2023-04-11 10:10:55.000000 ddd-struct-0.2.3/src/ddd_struct/application/action.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:11:02.548491 ddd-struct-0.2.3/src/ddd_struct/domain/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 10:10:55.000000 ddd-struct-0.2.3/src/ddd_struct/domain/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-04-11 10:10:55.000000 ddd-struct-0.2.3/src/ddd_struct/domain/repository.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:11:02.548491 ddd-struct-0.2.3/src/ddd_struct/infrastructure/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 10:10:55.000000 ddd-struct-0.2.3/src/ddd_struct/infrastructure/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3870 2023-04-11 10:10:55.000000 ddd-struct-0.2.3/src/ddd_struct/infrastructure/repository_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:11:02.548491 ddd-struct-0.2.3/src/ddd_struct/lib/
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-04-11 10:10:55.000000 ddd-struct-0.2.3/src/ddd_struct/lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1873 2023-04-11 10:10:55.000000 ddd-struct-0.2.3/src/ddd_struct/lib/common.py
+-rw-rw-rw-   0 root         (0) root         (0)     5051 2023-04-11 10:10:55.000000 ddd-struct-0.2.3/src/ddd_struct/lib/thread.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-04-11 10:10:55.000000 ddd-struct-0.2.3/src/ddd_struct/lib/warning.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-11 10:10:55.000000 ddd-struct-0.2.3/src/ddd_struct/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 10:11:02.548491 ddd-struct-0.2.3/src/ddd_struct.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-04-11 10:11:02.000000 ddd-struct-0.2.3/src/ddd_struct.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      624 2023-04-11 10:11:02.000000 ddd-struct-0.2.3/src/ddd_struct.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 10:11:02.000000 ddd-struct-0.2.3/src/ddd_struct.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-11 10:11:02.000000 ddd-struct-0.2.3/src/ddd_struct.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-11 10:11:02.000000 ddd-struct-0.2.3/src/ddd_struct.egg-info/top_level.txt
```

### Comparing `ddd-struct-0.2.2/LICENSE` & `ddd-struct-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ddd-struct-0.2.2/setup.py` & `ddd-struct-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,9 +14,9 @@
     description="Data structures",
     package_dir={"": "src"},
     packages=find_packages(where='src'),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
     ],
-    install_requires=['retry2', 'ddd-interface'],
+    install_requires=['retry2', 'ddd-interface', 'psutil'],
 )
```

### Comparing `ddd-struct-0.2.2/src/ddd_struct/application/action.py` & `ddd-struct-0.2.3/src/ddd_struct/application/action.py`

 * *Files identical despite different names*

### Comparing `ddd-struct-0.2.2/src/ddd_struct/domain/repository.py` & `ddd-struct-0.2.3/src/ddd_struct/domain/repository.py`

 * *Files identical despite different names*

### Comparing `ddd-struct-0.2.2/src/ddd_struct/infrastructure/repository_impl.py` & `ddd-struct-0.2.3/src/ddd_struct/infrastructure/repository_impl.py`

 * *Files identical despite different names*

### Comparing `ddd-struct-0.2.2/src/ddd_struct/lib/thread.py` & `ddd-struct-0.2.3/src/ddd_struct/lib/thread.py`

 * *Files 26% similar despite different names*

```diff
@@ -60,68 +60,82 @@
 
 
     def create_task(self, task_item:TaskItem):
         func, args, kwargs = task_item.func, task_item.args, task_item.kwargs
         func = async_wrap(func)
         task = asyncio.create_task(func(*args, **kwargs))
         return task
+    
+
+    async def run(self, wait_list, delay=0, timeout=100):
+        start_time = time.time()
+        ret_list = [None]*len(wait_list)
+        runner = []
+        
+        for _ in range(1000000000):
+            if (time.time()-start_time)>timeout:
+                self.ret_list_when_timeout = ret_list
+                raise ValueError(f'Fail to finish task in {timeout}s')
+
+            # create task
+            if len(runner)<self.n_workers and wait_list:
+                print('create task')
+                task_item:TaskItem = wait_list.pop()
+                task = self.create_task(task_item)
+                runner.append((task_item.index, task, task_item))
+            else:
+                print('check task')
+                # check tasks
+                for i, (idx, task, item) in enumerate(runner):
+                    if not task.done():
+                        continue
+                    succeed, result = self._get_task_result(task)
+                    if succeed:
+                        print('succeed', result)
+                        ret_list[idx] = result
+                        runner[i] = None
+                        if idx in self.failed: del self.failed[idx]
+                    elif idx not in self.failed and item.retry>0:
+                        print('failed1', result)
+                        assert idx==item.index
+                        self.failed[idx] = 1
+                        task = self.create_task(item)
+                        runner[i] = (item.index, task, item)
+                    elif idx in self.failed and self.failed[idx]<item.retry:
+                        print('failed2', result)
+                        self.failed[idx] += 1
+                        task = self.create_task(item)
+                        runner[i] = (item.index, task, item)
+                    else:
+                        print('failed3', result)
+                        ret_list[idx] = result
+                        runner[i] = None
+                        if idx in self.failed: del self.failed[idx]
+                runner = [r for r in runner if r is not None]
+
+                #exit
+                if not runner and not wait_list:
+                    print(runner, wait_list)
+                    print('break')
+                    break
+                await asyncio.sleep(delay)
+        return ret_list
 
 
     def execute(self, delay=0, timeout=100, n_workers=None):
         if n_workers is not None:
             self.n_workers = n_workers
         wait_list = copy(self.wait_list)
 
-        async def run():
-            start_time = time.time()
-            ret_list = [None]*len(wait_list)
-            runner = []
-            
-            for _ in range(1000000000):
-                if (time.time()-start_time)>timeout:
-                    self.ret_list_when_timeout = ret_list
-                    raise ValueError(f'Fail to finish task in {timeout}s')
-
-                # create task
-                if len(runner)<self.n_workers and wait_list:
-                    task_item:TaskItem = wait_list.pop()
-                    task = self.create_task(task_item)
-                    runner.append((task_item.index, task, task_item))
-                else:
-                    # check tasks
-                    for i, (idx, task, item) in enumerate(runner):
-                        if not task.done():
-                            continue
-                        succeed, result = self._get_task_result(task)
-                        if succeed:
-                            ret_list[idx] = result
-                            runner[i] = None
-                            if idx in self.failed: del self.failed[idx]
-                        elif idx not in self.failed and item.retry>0:
-                            assert idx==item.index
-                            self.failed[idx] = 1
-                            task = self.create_task(item)
-                            runner[i] = (item.index, task, item)
-                        elif idx in self.failed and self.failed[idx]<item.retry:
-                            self.failed[idx] += 1
-                            task = self.create_task(item)
-                            runner[i] = (item.index, task, item)
-                        else:
-                            ret_list[idx] = result
-                            runner[i] = None
-                            if idx in self.failed: del self.failed[idx]
-                    runner = [r for r in runner if r is not None]
-
-                    #exit
-                    if not runner and not wait_list:
-                        break
-                    await asyncio.sleep(delay)
-            return ret_list
-
         event_loop = asyncio.get_event_loop()
-        ret_list = event_loop.run_until_complete(run())
+        ret_list = event_loop.run_until_complete(self.run(wait_list, delay, timeout))
+        print('finish')
         # ret_list = asyncio.run(run())
         self.wait_list = []
         return ret_list
-                
-
+    
 
+    async def gather(self, delay=0, timeout=100, n_workers=None):
+        if n_workers is not None:
+            self.n_workers = n_workers
+        wait_list = copy(self.wait_list)
+        return await self.run(wait_list, delay, timeout)
```

### Comparing `ddd-struct-0.2.2/src/ddd_struct/lib/warning.py` & `ddd-struct-0.2.3/src/ddd_struct/lib/warning.py`

 * *Files identical despite different names*

### Comparing `ddd-struct-0.2.2/src/ddd_struct.egg-info/SOURCES.txt` & `ddd-struct-0.2.3/src/ddd_struct.egg-info/SOURCES.txt`

 * *Files identical despite different names*

