# Comparing `tmp/poe-web-client-0.0.5.tar.gz` & `tmp/poe-web-client-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poe-web-client-0.0.5.tar", last modified: Mon Apr 10 22:15:34 2023, max compression
+gzip compressed data, was "poe-web-client-0.0.6.tar", last modified: Tue Apr 11 01:11:21 2023, max compression
```

## Comparing `poe-web-client-0.0.5.tar` & `poe-web-client-0.0.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 zhaoyandong   (501) staff       (20)        0 2023-04-10 22:15:34.349174 poe-web-client-0.0.5/
--rw-r--r--   0 zhaoyandong   (501) staff       (20)    35149 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/LICENSE
--rw-r--r--   0 zhaoyandong   (501) staff       (20)     8957 2023-04-10 22:15:34.348460 poe-web-client-0.0.5/PKG-INFO
--rw-r--r--   0 zhaoyandong   (501) staff       (20)     8459 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/README.md
-drwxr-xr-x   0 zhaoyandong   (501) staff       (20)        0 2023-04-10 22:15:34.307434 poe-web-client-0.0.5/poe-api/
-drwxr-xr-x   0 zhaoyandong   (501) staff       (20)        0 2023-04-10 22:15:34.309593 poe-web-client-0.0.5/poe-api/src/
--rw-r--r--   0 zhaoyandong   (501) staff       (20)    12055 2023-04-10 22:14:16.000000 poe-web-client-0.0.5/poe-api/src/poe.py
-drwxr-xr-x   0 zhaoyandong   (501) staff       (20)        0 2023-04-10 22:15:34.341771 poe-web-client-0.0.5/poe-api/src/poe_graphql/
--rw-r--r--   0 zhaoyandong   (501) staff       (20)     1093 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/poe-api/src/poe_graphql/AddHumanMessageMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      373 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/poe-api/src/poe_graphql/AddMessageBreakMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      180 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/poe-api/src/poe_graphql/AutoSubscriptionMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)       97 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/poe-api/src/poe_graphql/BioFragment.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)       73 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/poe-api/src/poe_graphql/ChatAddedSubscription.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      100 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/poe-api/src/poe_graphql/ChatFragment.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)     6971 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/poe-api/src/poe_graphql/ChatListPaginationQuery.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      686 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/poe-api/src/poe_graphql/ChatPaginationQuery.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      154 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/poe-api/src/poe_graphql/ChatViewQuery.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      160 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/poe-api/src/poe_graphql/DeleteHumanMessagesMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      123 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/poe-api/src/poe_graphql/DeleteMessageMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      103 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/poe-api/src/poe_graphql/HandleFragment.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      306 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/poe-api/src/poe_graphql/LoginWithVerificationCodeMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)     1885 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/poe-api/src/poe_graphql/MessageAddedSubscription.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      135 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/poe-api/src/poe_graphql/MessageDeletedSubscription.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      194 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/poe-api/src/poe_graphql/MessageFragment.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      145 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/poe-api/src/poe_graphql/MessageRemoveVoteMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      216 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/poe-api/src/poe_graphql/MessageSetVoteMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      710 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/poe-api/src/poe_graphql/SendMessageMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      263 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/poe-api/src/poe_graphql/SendVerificationCodeForLoginMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      213 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/poe-api/src/poe_graphql/ShareMessagesMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      308 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/poe-api/src/poe_graphql/SignupWithVerificationCodeMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      159 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/poe-api/src/poe_graphql/StaleChatUpdateMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      162 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/poe-api/src/poe_graphql/SubscriptionsMutation.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)       95 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/poe-api/src/poe_graphql/SummarizePlainPostQuery.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      147 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/poe-api/src/poe_graphql/SummarizeQuotePostQuery.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      180 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/poe-api/src/poe_graphql/SummarizeSharePostQuery.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      368 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/poe-api/src/poe_graphql/UserSnippetFragment.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      400 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/poe-api/src/poe_graphql/ViewerInfoQuery.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)     1038 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/poe-api/src/poe_graphql/ViewerStateFragment.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)      657 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/poe-api/src/poe_graphql/ViewerStateUpdatedSubscription.graphql
--rw-r--r--   0 zhaoyandong   (501) staff       (20)        0 2023-04-09 00:01:12.000000 poe-web-client-0.0.5/poe-api/src/poe_graphql/__init__.py
-drwxr-xr-x   0 zhaoyandong   (501) staff       (20)        0 2023-04-10 22:15:34.347277 poe-web-client-0.0.5/poe-api/src/poe_web_client.egg-info/
--rw-r--r--   0 zhaoyandong   (501) staff       (20)     8957 2023-04-10 22:15:34.000000 poe-web-client-0.0.5/poe-api/src/poe_web_client.egg-info/PKG-INFO
--rw-r--r--   0 zhaoyandong   (501) staff       (20)     2035 2023-04-10 22:15:34.000000 poe-web-client-0.0.5/poe-api/src/poe_web_client.egg-info/SOURCES.txt
--rw-r--r--   0 zhaoyandong   (501) staff       (20)        1 2023-04-10 22:15:34.000000 poe-web-client-0.0.5/poe-api/src/poe_web_client.egg-info/dependency_links.txt
--rw-r--r--   0 zhaoyandong   (501) staff       (20)       46 2023-04-10 22:15:34.000000 poe-web-client-0.0.5/poe-api/src/poe_web_client.egg-info/requires.txt
--rw-r--r--   0 zhaoyandong   (501) staff       (20)       16 2023-04-10 22:15:34.000000 poe-web-client-0.0.5/poe-api/src/poe_web_client.egg-info/top_level.txt
--rw-r--r--   0 zhaoyandong   (501) staff       (20)       38 2023-04-10 22:15:34.349327 poe-web-client-0.0.5/setup.cfg
--rw-r--r--   0 zhaoyandong   (501) staff       (20)     1044 2023-04-10 22:15:08.000000 poe-web-client-0.0.5/setup.py
+drwxr-xr-x   0 zhaoyandong   (501) staff       (20)        0 2023-04-11 01:11:21.945840 poe-web-client-0.0.6/
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)    35149 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/LICENSE
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)     8957 2023-04-11 01:11:21.945340 poe-web-client-0.0.6/PKG-INFO
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)     8459 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/README.md
+drwxr-xr-x   0 zhaoyandong   (501) staff       (20)        0 2023-04-11 01:11:21.879882 poe-web-client-0.0.6/poe-api/
+drwxr-xr-x   0 zhaoyandong   (501) staff       (20)        0 2023-04-11 01:11:21.883332 poe-web-client-0.0.6/poe-api/src/
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)    12092 2023-04-11 01:10:38.000000 poe-web-client-0.0.6/poe-api/src/poe.py
+drwxr-xr-x   0 zhaoyandong   (501) staff       (20)        0 2023-04-11 01:11:21.940478 poe-web-client-0.0.6/poe-api/src/poe_graphql/
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)     1093 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/AddHumanMessageMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      373 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/AddMessageBreakMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      180 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/AutoSubscriptionMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)       97 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/BioFragment.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)       73 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/ChatAddedSubscription.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      100 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/ChatFragment.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)     6971 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/ChatListPaginationQuery.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      686 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/ChatPaginationQuery.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      154 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/ChatViewQuery.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      160 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/DeleteHumanMessagesMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      123 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/DeleteMessageMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      103 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/HandleFragment.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      306 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/LoginWithVerificationCodeMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)     1885 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/MessageAddedSubscription.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      135 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/MessageDeletedSubscription.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      194 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/MessageFragment.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      145 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/MessageRemoveVoteMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      216 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/MessageSetVoteMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      710 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/SendMessageMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      263 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/SendVerificationCodeForLoginMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      213 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/ShareMessagesMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      308 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/SignupWithVerificationCodeMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      159 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/StaleChatUpdateMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      162 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/SubscriptionsMutation.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)       95 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/SummarizePlainPostQuery.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      147 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/SummarizeQuotePostQuery.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      180 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/SummarizeSharePostQuery.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      368 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/UserSnippetFragment.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      400 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/ViewerInfoQuery.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)     1038 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/ViewerStateFragment.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)      657 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/ViewerStateUpdatedSubscription.graphql
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)        0 2023-04-09 00:01:12.000000 poe-web-client-0.0.6/poe-api/src/poe_graphql/__init__.py
+drwxr-xr-x   0 zhaoyandong   (501) staff       (20)        0 2023-04-11 01:11:21.944593 poe-web-client-0.0.6/poe-api/src/poe_web_client.egg-info/
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)     8957 2023-04-11 01:11:21.000000 poe-web-client-0.0.6/poe-api/src/poe_web_client.egg-info/PKG-INFO
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)     2035 2023-04-11 01:11:21.000000 poe-web-client-0.0.6/poe-api/src/poe_web_client.egg-info/SOURCES.txt
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)        1 2023-04-11 01:11:21.000000 poe-web-client-0.0.6/poe-api/src/poe_web_client.egg-info/dependency_links.txt
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)       46 2023-04-11 01:11:21.000000 poe-web-client-0.0.6/poe-api/src/poe_web_client.egg-info/requires.txt
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)       16 2023-04-11 01:11:21.000000 poe-web-client-0.0.6/poe-api/src/poe_web_client.egg-info/top_level.txt
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)       38 2023-04-11 01:11:21.945955 poe-web-client-0.0.6/setup.cfg
+-rw-r--r--   0 zhaoyandong   (501) staff       (20)     1044 2023-04-11 01:10:03.000000 poe-web-client-0.0.6/setup.py
```

### Comparing `poe-web-client-0.0.5/LICENSE` & `poe-web-client-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `poe-web-client-0.0.5/PKG-INFO` & `poe-web-client-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poe-web-client
-Version: 0.0.5
+Version: 0.0.6
 Summary: A reverse engineered API wrapper for Quora's Poe,fork from https://github.com/ading2210/poe-api
 Home-page: https://github.com/libaiabcd/poe-api
 Author: libaiabcd
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `poe-web-client-0.0.5/README.md` & `poe-web-client-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `poe-web-client-0.0.5/poe-api/src/poe.py` & `poe-web-client-0.0.6/poe-api/src/poe.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,17 +45,20 @@
   formkey = ""
   next_data = {}
   bots = {}
   active_messages = {}
   message_queues = {}
   ws = None
   ws_connected = False
+
+  token = ""
   
   def __init__(self, token, proxy=None):
     self.proxy = proxy
+    self.token = token
     self.session = requests.Session()
         
     if proxy:
       self.session.proxies = {
         "http": self.proxy,
         "https": self.proxy
       }
```

### Comparing `poe-web-client-0.0.5/poe-api/src/poe_graphql/AddHumanMessageMutation.graphql` & `poe-web-client-0.0.6/poe-api/src/poe_graphql/AddHumanMessageMutation.graphql`

 * *Files identical despite different names*

### Comparing `poe-web-client-0.0.5/poe-api/src/poe_graphql/ChatListPaginationQuery.graphql` & `poe-web-client-0.0.6/poe-api/src/poe_graphql/ChatListPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `poe-web-client-0.0.5/poe-api/src/poe_graphql/ChatPaginationQuery.graphql` & `poe-web-client-0.0.6/poe-api/src/poe_graphql/ChatPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `poe-web-client-0.0.5/poe-api/src/poe_graphql/MessageAddedSubscription.graphql` & `poe-web-client-0.0.6/poe-api/src/poe_graphql/MessageAddedSubscription.graphql`

 * *Files identical despite different names*

### Comparing `poe-web-client-0.0.5/poe-api/src/poe_graphql/SendMessageMutation.graphql` & `poe-web-client-0.0.6/poe-api/src/poe_graphql/SendMessageMutation.graphql`

 * *Files identical despite different names*

### Comparing `poe-web-client-0.0.5/poe-api/src/poe_graphql/ViewerStateFragment.graphql` & `poe-web-client-0.0.6/poe-api/src/poe_graphql/ViewerStateFragment.graphql`

 * *Files identical despite different names*

### Comparing `poe-web-client-0.0.5/poe-api/src/poe_graphql/ViewerStateUpdatedSubscription.graphql` & `poe-web-client-0.0.6/poe-api/src/poe_graphql/ViewerStateUpdatedSubscription.graphql`

 * *Files identical despite different names*

### Comparing `poe-web-client-0.0.5/poe-api/src/poe_web_client.egg-info/PKG-INFO` & `poe-web-client-0.0.6/poe-api/src/poe_web_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poe-web-client
-Version: 0.0.5
+Version: 0.0.6
 Summary: A reverse engineered API wrapper for Quora's Poe,fork from https://github.com/ading2210/poe-api
 Home-page: https://github.com/libaiabcd/poe-api
 Author: libaiabcd
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `poe-web-client-0.0.5/poe-api/src/poe_web_client.egg-info/SOURCES.txt` & `poe-web-client-0.0.6/poe-api/src/poe_web_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `poe-web-client-0.0.5/setup.py` & `poe-web-client-0.0.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #pip wheel --no-deps -w dist .
 
 base_path = Path(__file__).parent
 long_description = (base_path / "README.md").read_text()
 
 setuptools.setup(
   name="poe-web-client",
-  version="0.0.5",
+  version="0.0.6",
   author="libaiabcd",
   license="GPLv3",
   description="A reverse engineered API wrapper for Quora's Poe,fork from https://github.com/ading2210/poe-api",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=["poe_graphql"],
   classifiers=[
```

