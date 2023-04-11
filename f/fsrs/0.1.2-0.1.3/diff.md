# Comparing `tmp/fsrs-0.1.2.tar.gz` & `tmp/fsrs-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs-0.1.2.tar", last modified: Mon Mar  6 05:08:20 2023, max compression
+gzip compressed data, was "fsrs-0.1.3.tar", last modified: Tue Apr 11 11:03:03 2023, max compression
```

## Comparing `fsrs-0.1.2.tar` & `fsrs-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jarrettye   (501) staff       (20)        0 2023-03-06 05:08:20.506484 fsrs-0.1.2/
--rw-r--r--   0 jarrettye   (501) staff       (20)     1079 2022-11-28 10:42:22.000000 fsrs-0.1.2/LICENSE
--rw-r--r--   0 jarrettye   (501) staff       (20)     3340 2023-03-06 05:08:20.506349 fsrs-0.1.2/PKG-INFO
--rw-r--r--   0 jarrettye   (501) staff       (20)     1647 2023-02-27 08:38:12.000000 fsrs-0.1.2/README.md
--rw-r--r--   0 jarrettye   (501) staff       (20)      593 2023-03-06 02:03:54.000000 fsrs-0.1.2/pyproject.toml
--rw-r--r--   0 jarrettye   (501) staff       (20)       38 2023-03-06 05:08:20.506526 fsrs-0.1.2/setup.cfg
--rw-r--r--   0 jarrettye   (501) staff       (20)       37 2022-11-28 09:57:57.000000 fsrs-0.1.2/setup.py
-drwxr-xr-x   0 jarrettye   (501) staff       (20)        0 2023-03-06 05:08:20.504024 fsrs-0.1.2/src/
-drwxr-xr-x   0 jarrettye   (501) staff       (20)        0 2023-03-06 05:08:20.505260 fsrs-0.1.2/src/fsrs/
--rw-r--r--   0 jarrettye   (501) staff       (20)       97 2023-03-06 02:04:01.000000 fsrs-0.1.2/src/fsrs/__init__.py
--rw-r--r--   0 jarrettye   (501) staff       (20)     4634 2023-03-06 02:04:37.000000 fsrs-0.1.2/src/fsrs/fsrs.py
--rw-r--r--   0 jarrettye   (501) staff       (20)     4326 2023-02-27 08:45:13.000000 fsrs-0.1.2/src/fsrs/models.py
-drwxr-xr-x   0 jarrettye   (501) staff       (20)        0 2023-03-06 05:08:20.505920 fsrs-0.1.2/src/fsrs.egg-info/
--rw-r--r--   0 jarrettye   (501) staff       (20)     3340 2023-03-06 05:08:20.000000 fsrs-0.1.2/src/fsrs.egg-info/PKG-INFO
--rw-r--r--   0 jarrettye   (501) staff       (20)      245 2023-03-06 05:08:20.000000 fsrs-0.1.2/src/fsrs.egg-info/SOURCES.txt
--rw-r--r--   0 jarrettye   (501) staff       (20)        1 2023-03-06 05:08:20.000000 fsrs-0.1.2/src/fsrs.egg-info/dependency_links.txt
--rw-r--r--   0 jarrettye   (501) staff       (20)        5 2023-03-06 05:08:20.000000 fsrs-0.1.2/src/fsrs.egg-info/top_level.txt
-drwxr-xr-x   0 jarrettye   (501) staff       (20)        0 2023-03-06 05:08:20.506032 fsrs-0.1.2/tests/
--rw-r--r--   0 jarrettye   (501) staff       (20)     1535 2022-11-30 08:56:29.000000 fsrs-0.1.2/tests/test_fsrs.py
+drwxr-xr-x   0 jarrettye   (501) staff       (20)        0 2023-04-11 11:03:03.311644 fsrs-0.1.3/
+-rw-r--r--   0 jarrettye   (501) staff       (20)     1079 2022-11-28 10:42:22.000000 fsrs-0.1.3/LICENSE
+-rw-r--r--   0 jarrettye   (501) staff       (20)     3340 2023-04-11 11:03:03.311195 fsrs-0.1.3/PKG-INFO
+-rw-r--r--   0 jarrettye   (501) staff       (20)     1647 2023-02-27 08:38:12.000000 fsrs-0.1.3/README.md
+-rw-r--r--   0 jarrettye   (501) staff       (20)      593 2023-04-11 10:58:40.000000 fsrs-0.1.3/pyproject.toml
+-rw-r--r--   0 jarrettye   (501) staff       (20)       38 2023-04-11 11:03:03.311714 fsrs-0.1.3/setup.cfg
+-rw-r--r--   0 jarrettye   (501) staff       (20)       37 2022-11-28 09:57:57.000000 fsrs-0.1.3/setup.py
+drwxr-xr-x   0 jarrettye   (501) staff       (20)        0 2023-04-11 11:03:03.307133 fsrs-0.1.3/src/
+drwxr-xr-x   0 jarrettye   (501) staff       (20)        0 2023-04-11 11:03:03.309379 fsrs-0.1.3/src/fsrs/
+-rw-r--r--   0 jarrettye   (501) staff       (20)       97 2023-04-11 10:58:57.000000 fsrs-0.1.3/src/fsrs/__init__.py
+-rw-r--r--   0 jarrettye   (501) staff       (20)     4575 2023-04-11 10:50:58.000000 fsrs-0.1.3/src/fsrs/fsrs.py
+-rw-r--r--   0 jarrettye   (501) staff       (20)     4423 2023-04-11 10:50:58.000000 fsrs-0.1.3/src/fsrs/models.py
+drwxr-xr-x   0 jarrettye   (501) staff       (20)        0 2023-04-11 11:03:03.310618 fsrs-0.1.3/src/fsrs.egg-info/
+-rw-r--r--   0 jarrettye   (501) staff       (20)     3340 2023-04-11 11:03:03.000000 fsrs-0.1.3/src/fsrs.egg-info/PKG-INFO
+-rw-r--r--   0 jarrettye   (501) staff       (20)      245 2023-04-11 11:03:03.000000 fsrs-0.1.3/src/fsrs.egg-info/SOURCES.txt
+-rw-r--r--   0 jarrettye   (501) staff       (20)        1 2023-04-11 11:03:03.000000 fsrs-0.1.3/src/fsrs.egg-info/dependency_links.txt
+-rw-r--r--   0 jarrettye   (501) staff       (20)        5 2023-04-11 11:03:03.000000 fsrs-0.1.3/src/fsrs.egg-info/top_level.txt
+drwxr-xr-x   0 jarrettye   (501) staff       (20)        0 2023-04-11 11:03:03.310808 fsrs-0.1.3/tests/
+-rw-r--r--   0 jarrettye   (501) staff       (20)     1535 2022-11-30 08:56:29.000000 fsrs-0.1.3/tests/test_fsrs.py
```

### Comparing `fsrs-0.1.2/LICENSE` & `fsrs-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fsrs-0.1.2/PKG-INFO` & `fsrs-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsrs
-Version: 0.1.2
+Version: 0.1.3
 Summary: Free Spaced Repetition Scheduler
 Author-email: Jarrett Ye <jarrett.ye@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Open Spaced Repetition
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `fsrs-0.1.2/README.md` & `fsrs-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `fsrs-0.1.2/pyproject.toml` & `fsrs-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fsrs"
-version = "0.1.2"
+version = "0.1.3"
 description = "Free Spaced Repetition Scheduler"
 readme = "README.md"
 authors = [{ name = "Jarrett Ye", email = "jarrett.ye@outlook.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
```

### Comparing `fsrs-0.1.2/src/fsrs/fsrs.py` & `fsrs-0.1.3/src/fsrs/fsrs.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,16 +25,16 @@
             s.again.due = now + timedelta(minutes=1)
             s.hard.due = now + timedelta(minutes=5)
             s.good.due = now + timedelta(minutes=10)
             easy_interval = self.next_interval(s.easy.stability * self.p.easy_bonus)
             s.easy.scheduled_days = easy_interval
             s.easy.due = now + timedelta(days=easy_interval)
         elif card.state == State.Learning or card.state == State.Relearning:
-            hard_interval = self.next_interval(s.hard.stability)
-            good_interval = max(self.next_interval(s.good.stability), hard_interval + 1)
+            hard_interval = 0
+            good_interval = self.next_interval(s.good.stability)
             easy_interval = max(self.next_interval(s.easy.stability * self.p.easy_bonus), good_interval + 1)
 
             s.schedule(now, hard_interval, good_interval, easy_interval)
         elif card.state == State.Review:
             interval = card.elapsed_days
             last_d = card.difficulty
             last_s = card.stability
```

### Comparing `fsrs-0.1.2/src/fsrs/models.py` & `fsrs-0.1.3/src/fsrs/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             self.again.state = State.Learning
             self.hard.state = State.Learning
             self.good.state = State.Learning
             self.easy.state = State.Review
             self.again.lapses += 1
         elif state == State.Learning or state == State.Relearning:
             self.again.state = state
-            self.hard.state = State.Review
+            self.hard.state = state
             self.good.state = State.Review
             self.easy.state = State.Review
         elif state == State.Review:
             self.again.state = State.Relearning
             self.hard.state = State.Review
             self.good.state = State.Review
             self.easy.state = State.Review
@@ -97,15 +97,18 @@
 
     def schedule(self, now: datetime, hard_interval: float, good_interval: float, easy_interval: float):
         self.again.scheduled_days = 0
         self.hard.scheduled_days = hard_interval
         self.good.scheduled_days = good_interval
         self.easy.scheduled_days = easy_interval
         self.again.due = now + timedelta(minutes=5)
-        self.hard.due = now + timedelta(days=hard_interval)
+        if hard_interval > 0:
+            self.hard.due = now + timedelta(days=hard_interval)
+        else:
+            self.hard.due = now + timedelta(minutes=10)
         self.good.due = now + timedelta(days=good_interval)
         self.easy.due = now + timedelta(days=easy_interval)
 
     def record_log(self, card: Card, now: datetime) -> dict[int, SchedulingInfo]:
         return {
             Rating.Again: SchedulingInfo(self.again,
                                          ReviewLog(Rating.Again, self.again.scheduled_days, card.elapsed_days, now,
```

### Comparing `fsrs-0.1.2/src/fsrs.egg-info/PKG-INFO` & `fsrs-0.1.3/src/fsrs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsrs
-Version: 0.1.2
+Version: 0.1.3
 Summary: Free Spaced Repetition Scheduler
 Author-email: Jarrett Ye <jarrett.ye@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Open Spaced Repetition
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `fsrs-0.1.2/tests/test_fsrs.py` & `fsrs-0.1.3/tests/test_fsrs.py`

 * *Files identical despite different names*

