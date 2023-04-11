# Comparing `tmp/recon_lw-2.0.0.dev4658666204.tar.gz` & `tmp/recon_lw-2.0.0.dev4665720729.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev4658666204.tar", last modified: Mon Apr 10 15:14:54 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev4665720729.tar", last modified: Tue Apr 11 08:58:40 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev4658666204.tar` & `recon_lw-2.0.0.dev4665720729.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:14:54.000000 recon_lw-2.0.0.dev4658666204/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-10 15:14:20.000000 recon_lw-2.0.0.dev4658666204/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-10 15:14:54.000000 recon_lw-2.0.0.dev4658666204/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-10 15:14:20.000000 recon_lw-2.0.0.dev4658666204/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-10 15:14:41.000000 recon_lw-2.0.0.dev4658666204/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:14:54.000000 recon_lw-2.0.0.dev4658666204/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-10 15:14:20.000000 recon_lw-2.0.0.dev4658666204/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12849 2023-04-10 15:14:20.000000 recon_lw-2.0.0.dev4658666204/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    13157 2023-04-10 15:14:20.000000 recon_lw-2.0.0.dev4658666204/recon_lw/recon_ob.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:14:54.000000 recon_lw-2.0.0.dev4658666204/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-10 15:14:54.000000 recon_lw-2.0.0.dev4658666204/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      287 2023-04-10 15:14:54.000000 recon_lw-2.0.0.dev4658666204/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-10 15:14:54.000000 recon_lw-2.0.0.dev4658666204/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-10 15:14:54.000000 recon_lw-2.0.0.dev4658666204/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-10 15:14:54.000000 recon_lw-2.0.0.dev4658666204/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-10 15:14:20.000000 recon_lw-2.0.0.dev4658666204/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-10 15:14:54.000000 recon_lw-2.0.0.dev4658666204/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-10 15:14:20.000000 recon_lw-2.0.0.dev4658666204/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:58:40.000000 recon_lw-2.0.0.dev4665720729/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-11 08:57:57.000000 recon_lw-2.0.0.dev4665720729/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-11 08:58:40.000000 recon_lw-2.0.0.dev4665720729/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-11 08:57:57.000000 recon_lw-2.0.0.dev4665720729/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-11 08:58:23.000000 recon_lw-2.0.0.dev4665720729/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:58:40.000000 recon_lw-2.0.0.dev4665720729/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-11 08:57:57.000000 recon_lw-2.0.0.dev4665720729/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12849 2023-04-11 08:57:57.000000 recon_lw-2.0.0.dev4665720729/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13342 2023-04-11 08:57:57.000000 recon_lw-2.0.0.dev4665720729/recon_lw/recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:58:40.000000 recon_lw-2.0.0.dev4665720729/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-11 08:58:40.000000 recon_lw-2.0.0.dev4665720729/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      287 2023-04-11 08:58:40.000000 recon_lw-2.0.0.dev4665720729/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 08:58:40.000000 recon_lw-2.0.0.dev4665720729/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-11 08:58:40.000000 recon_lw-2.0.0.dev4665720729/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-11 08:58:40.000000 recon_lw-2.0.0.dev4665720729/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-11 08:57:57.000000 recon_lw-2.0.0.dev4665720729/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 08:58:40.000000 recon_lw-2.0.0.dev4665720729/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-11 08:57:57.000000 recon_lw-2.0.0.dev4665720729/setup.py
```

### Comparing `recon_lw-2.0.0.dev4658666204/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev4665720729/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4658666204/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev4665720729/recon_lw/recon_ob.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,44 +76,46 @@
         events.append(book_id_event)
 
     if book_id is not None:
         if book_id not in books_cache:
             books_cache[book_id] = copy.deepcopy(initial_book_params)            
             #books_cache[book_id] = {"ask": {}, "bid": {}, "status": "?"}
         book = books_cache[book_id]
-        initial_book = copy.deepcopy(book)
-        operation, parameters = update_book_rule(book, mess)
-        if operation is None:
-            return 
-        initial_parameters = copy.copy(parameters)
-        parameters["order_book"] = book
-        result = operation(**parameters)
-        if len(result) > 0:
-            result["operation"] = operation.__name__
-            result["operation_params"] = initial_parameters
-            result["initial_book"] = initial_book
-            result["book_id"] = book_id
-            update_event = recon_lw.create_event("UpdateBookError:" + parent_event["eventName"], "UpdateBookError",
-                                                 event_sequence,
-                                                 ok=False,
-                                                 body=result,
-                                                 parentId=parent_event["eventId"])
-            update_event["attachedMessageIds"] = [mess["messageId"]]
-            events.append(update_event)
-        results = check_book_rule(book, event_sequence)
-        if results is not None:
-            for r in results:
-                if not r["successful"]:
-                    r["body"]["operation_params"] = initial_parameters
-                    r["body"]["initial_book"] = initial_book
-                r["body"]["operation"] = operation.__name__
-                r["body"]["book_id"] = book_id
-                r["parentEventId"] = parent_event["eventId"]
-                r["attachedMessageIds"] = [mess["messageId"]]
-                events.append(r)
+        operations = update_book_rule(book, mess)
+        if operations is None:
+            return
+        
+        for operation, parameters in operations:
+            initial_book = copy.deepcopy(book)
+            initial_parameters = copy.copy(parameters)
+            parameters["order_book"] = book
+            result = operation(**parameters)
+            if len(result) > 0:
+                result["operation"] = operation.__name__
+                result["operation_params"] = initial_parameters
+                result["initial_book"] = initial_book
+                result["book_id"] = book_id
+                update_event = recon_lw.create_event("UpdateBookError:" + parent_event["eventName"], "UpdateBookError",
+                                                     event_sequence,
+                                                     ok=False,
+                                                     body=result,
+                                                     parentId=parent_event["eventId"])
+                update_event["attachedMessageIds"] = [mess["messageId"]]
+                events.append(update_event)
+            results = check_book_rule(book, event_sequence)
+            if results is not None:
+                for r in results:
+                    if not r["successful"]:
+                        r["body"]["operation_params"] = initial_parameters
+                        r["body"]["initial_book"] = initial_book
+                    r["body"]["operation"] = operation.__name__
+                    r["body"]["book_id"] = book_id
+                    r["parentEventId"] = parent_event["eventId"]
+                    r["attachedMessageIds"] = [mess["messageId"]]
+                    events.append(r)
 
 
 def process_ob_rules(sequenced_batch, books_cache, get_book_id_func ,update_book_rule,
                      check_book_rule, event_sequence, send_events_func, parent_event, initial_book_params):
     events = []
     n_processed = 0
     for m in sequenced_batch:
@@ -255,24 +257,24 @@
     for side in ["ask","bid"]:
         for pr,orders in order_book[side].items():
             if order_id in orders:
                 return side, pr, orders[order_id]
     return None, None, None
 
 
-def ob_aggr_add_level(side, level, price, qty, num_orders, impl_qty, impl_num_orders, order_book):
+def ob_aggr_add_level(side, level, price, real_qty, real_num_orders, impl_qty, impl_num_orders, order_book):
     result_body = {}
     max_levels = order_book["aggr_max_levels"]
     side_key = side+"_aggr"
     new_index = level - 1
     if not 0 <= new_index <= len(order_book[side_key]):
         result_body["error"] = "Unexpected level {0}, against existing {1}".format(level, len(order_book[side_key]))
         return result_body
 
-    new_level = {"price": price, "qty": qty, "num_orders": num_orders, "impl_qty": impl_qty,
+    new_level = {"price": price, "real_qty": real_qty, "real_num_orders": real_num_orders, "impl_qty": impl_qty,
                  "impl_num_orders": impl_num_orders}
     order_book[side_key].insert(new_index, new_level)
     if len(order_book[side_key]) == max_levels+1:
         order_book[side_key].pop()
 
     return {}
```

### Comparing `recon_lw-2.0.0.dev4658666204/setup.py` & `recon_lw-2.0.0.dev4665720729/setup.py`

 * *Files identical despite different names*

