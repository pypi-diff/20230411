# Comparing `tmp/ezcode-1.0.8.tar.gz` & `tmp/ezcode-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezcode-1.0.8.tar", last modified: Thu Jan 26 10:21:57 2023, max compression
+gzip compressed data, was "ezcode-1.0.9.tar", last modified: Thu Jan 26 11:08:56 2023, max compression
```

## Comparing `ezcode-1.0.8.tar` & `ezcode-1.0.9.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 10:21:57.893376 ezcode-1.0.8/
--rw-r--r--   0 zgao     (21923) staff       (20)     1066 2023-01-14 06:12:57.000000 ezcode-1.0.8/LICENSE.md
--rw-r--r--   0 zgao     (21923) staff       (20)     1361 2023-01-26 10:21:57.892679 ezcode-1.0.8/PKG-INFO
--rw-r--r--   0 zgao     (21923) staff       (20)      769 2023-01-14 06:12:57.000000 ezcode-1.0.8/README.md
--rw-r--r--   0 zgao     (21923) staff       (20)      132 2023-01-14 06:12:57.000000 ezcode-1.0.8/pyproject.toml
--rw-r--r--   0 zgao     (21923) staff       (20)       38 2023-01-26 10:21:57.893669 ezcode-1.0.8/setup.cfg
--rw-r--r--   0 zgao     (21923) staff       (20)     2160 2023-01-26 10:17:20.000000 ezcode-1.0.8/setup.py
-drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 10:21:57.834272 ezcode-1.0.8/src/
-drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 10:21:57.840894 ezcode-1.0.8/src/ezcode/
-drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 10:21:57.847966 ezcode-1.0.8/src/ezcode/Array/
--rw-r--r--   0 zgao     (21923) staff       (20)    10900 2023-01-20 20:57:08.000000 ezcode-1.0.8/src/ezcode/Array/Interval.py
--rw-r--r--   0 zgao     (21923) staff       (20)     4406 2023-01-14 06:12:57.000000 ezcode-1.0.8/src/ezcode/Array/Search.py
--rw-r--r--   0 zgao     (21923) staff       (20)     1542 2023-01-14 06:12:57.000000 ezcode-1.0.8/src/ezcode/Array/Sort.py
--rw-r--r--   0 zgao     (21923) staff       (20)     2149 2023-01-21 00:07:01.000000 ezcode-1.0.8/src/ezcode/Array/Sub.py
--rw-r--r--   0 zgao     (21923) staff       (20)     7725 2023-01-21 07:52:27.000000 ezcode-1.0.8/src/ezcode/Array/Utils.py
--rw-r--r--   0 zgao     (21923) staff       (20)        0 2023-01-14 06:12:57.000000 ezcode-1.0.8/src/ezcode/Array/__init__.py
-drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 10:21:57.849204 ezcode-1.0.8/src/ezcode/Cache/
--rw-r--r--   0 zgao     (21923) staff       (20)     1250 2023-01-20 20:45:54.000000 ezcode-1.0.8/src/ezcode/Cache/LRUCache.py
--rw-r--r--   0 zgao     (21923) staff       (20)        0 2023-01-23 00:24:04.000000 ezcode-1.0.8/src/ezcode/Cache/__init__.py
-drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 10:21:57.851019 ezcode-1.0.8/src/ezcode/Dynamic/
--rw-r--r--   0 zgao     (21923) staff       (20)    28816 2023-01-14 06:12:57.000000 ezcode-1.0.8/src/ezcode/Dynamic/Knapsack.py
--rw-r--r--   0 zgao     (21923) staff       (20)     5607 2023-01-21 10:28:16.000000 ezcode-1.0.8/src/ezcode/Dynamic/SparseTable.py
--rw-r--r--   0 zgao     (21923) staff       (20)        2 2023-01-21 06:46:19.000000 ezcode-1.0.8/src/ezcode/Dynamic/__init__.py
-drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 10:21:57.853192 ezcode-1.0.8/src/ezcode/Graph/
--rw-r--r--   0 zgao     (21923) staff       (20)     7075 2023-01-14 06:12:57.000000 ezcode-1.0.8/src/ezcode/Graph/DirectedGraph.py
--rw-r--r--   0 zgao     (21923) staff       (20)    10645 2023-01-20 20:56:32.000000 ezcode-1.0.8/src/ezcode/Graph/GraphPathFinder.py
--rw-r--r--   0 zgao     (21923) staff       (20)     4627 2023-01-14 06:12:57.000000 ezcode-1.0.8/src/ezcode/Graph/UndirectedGraph.py
--rw-r--r--   0 zgao     (21923) staff       (20)     2689 2023-01-14 06:12:57.000000 ezcode-1.0.8/src/ezcode/Graph/__init__.py
-drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 10:21:57.854927 ezcode-1.0.8/src/ezcode/Grid/
--rw-r--r--   0 zgao     (21923) staff       (20)    10287 2023-01-14 06:12:57.000000 ezcode-1.0.8/src/ezcode/Grid/GridIterator.py
--rw-r--r--   0 zgao     (21923) staff       (20)    12024 2023-01-20 20:46:30.000000 ezcode-1.0.8/src/ezcode/Grid/GridPathFinder.py
--rw-r--r--   0 zgao     (21923) staff       (20)     1877 2023-01-20 05:19:59.000000 ezcode-1.0.8/src/ezcode/Grid/__init__.py
-drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 10:21:57.858420 ezcode-1.0.8/src/ezcode/Heap/
--rw-r--r--   0 zgao     (21923) staff       (20)     6148 2023-01-20 20:46:19.000000 ezcode-1.0.8/src/ezcode/Heap/PriorityMap.py
--rw-r--r--   0 zgao     (21923) staff       (20)     5620 2023-01-19 08:03:02.000000 ezcode-1.0.8/src/ezcode/Heap/PriorityQueue.py
--rw-r--r--   0 zgao     (21923) staff       (20)     5132 2023-01-19 08:03:38.000000 ezcode-1.0.8/src/ezcode/Heap/PriorityQueueOnPartialArray.py
--rw-r--r--   0 zgao     (21923) staff       (20)        0 2023-01-14 06:12:57.000000 ezcode-1.0.8/src/ezcode/Heap/__init__.py
-drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 10:21:57.861844 ezcode-1.0.8/src/ezcode/List/
--rw-r--r--   0 zgao     (21923) staff       (20)     4613 2023-01-20 20:46:12.000000 ezcode-1.0.8/src/ezcode/List/DoublyLinkedList.py
--rw-r--r--   0 zgao     (21923) staff       (20)     3501 2023-01-20 20:46:08.000000 ezcode-1.0.8/src/ezcode/List/LinkedListAlgorithm.py
--rw-r--r--   0 zgao     (21923) staff       (20)     2672 2023-01-20 20:46:04.000000 ezcode-1.0.8/src/ezcode/List/LinkedListPrinter.py
--rw-r--r--   0 zgao     (21923) staff       (20)    11512 2023-01-21 07:57:10.000000 ezcode-1.0.8/src/ezcode/List/SinglyLinkedList.py
--rw-r--r--   0 zgao     (21923) staff       (20)      158 2023-01-14 06:12:57.000000 ezcode-1.0.8/src/ezcode/List/__init__.py
-drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 10:21:57.863455 ezcode-1.0.8/src/ezcode/Map/
--rw-r--r--   0 zgao     (21923) staff       (20)     2998 2023-01-26 10:14:10.000000 ezcode-1.0.8/src/ezcode/Map/TreeMap.py
--rw-r--r--   0 zgao     (21923) staff       (20)       44 2023-01-26 10:16:21.000000 ezcode-1.0.8/src/ezcode/Map/__init__.py
-drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 10:21:57.867897 ezcode-1.0.8/src/ezcode/Math/
--rw-r--r--   0 zgao     (21923) staff       (20)     4496 2023-01-19 07:59:19.000000 ezcode-1.0.8/src/ezcode/Math/Calculator.py
--rw-r--r--   0 zgao     (21923) staff       (20)     3129 2023-01-19 07:51:48.000000 ezcode-1.0.8/src/ezcode/Math/Combination.py
--rw-r--r--   0 zgao     (21923) staff       (20)     1508 2023-01-19 07:41:35.000000 ezcode-1.0.8/src/ezcode/Math/Enumeration.py
--rw-r--r--   0 zgao     (21923) staff       (20)      584 2023-01-19 07:41:30.000000 ezcode-1.0.8/src/ezcode/Math/Partition.py
--rw-r--r--   0 zgao     (21923) staff       (20)     3436 2023-01-20 23:27:14.000000 ezcode-1.0.8/src/ezcode/Math/Permutation.py
--rw-r--r--   0 zgao     (21923) staff       (20)      250 2023-01-19 07:31:50.000000 ezcode-1.0.8/src/ezcode/Math/__init__.py
-drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 10:21:57.870447 ezcode-1.0.8/src/ezcode/Queue/
--rw-r--r--   0 zgao     (21923) staff       (20)      682 2023-01-20 20:45:28.000000 ezcode-1.0.8/src/ezcode/Queue/MonotonicQueue.py
--rw-r--r--   0 zgao     (21923) staff       (20)     1410 2023-01-20 20:45:32.000000 ezcode-1.0.8/src/ezcode/Queue/Queue.py
--rw-r--r--   0 zgao     (21923) staff       (20)        0 2023-01-21 00:03:24.000000 ezcode-1.0.8/src/ezcode/Queue/QueueOnPartialArray.py
--rw-r--r--   0 zgao     (21923) staff       (20)       82 2023-01-18 04:47:07.000000 ezcode-1.0.8/src/ezcode/Queue/__init__.py
-drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 10:21:57.873931 ezcode-1.0.8/src/ezcode/Random/
--rw-r--r--   0 zgao     (21923) staff       (20)     3628 2023-01-20 19:06:20.000000 ezcode-1.0.8/src/ezcode/Random/RandomDict.py
--rw-r--r--   0 zgao     (21923) staff       (20)     1984 2023-01-20 20:55:16.000000 ezcode-1.0.8/src/ezcode/Random/RandomIndex.py
--rw-r--r--   0 zgao     (21923) staff       (20)     1323 2023-01-20 19:03:49.000000 ezcode-1.0.8/src/ezcode/Random/RandomSet.py
--rw-r--r--   0 zgao     (21923) staff       (20)      289 2023-01-24 11:08:34.000000 ezcode-1.0.8/src/ezcode/Random/Shuffle.py
--rw-r--r--   0 zgao     (21923) staff       (20)        0 2023-01-20 19:07:03.000000 ezcode-1.0.8/src/ezcode/Random/__init__.py
-drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 10:21:57.875133 ezcode-1.0.8/src/ezcode/Set/
--rw-r--r--   0 zgao     (21923) staff       (20)     1046 2023-01-26 10:14:06.000000 ezcode-1.0.8/src/ezcode/Set/TreeSet.py
--rw-r--r--   0 zgao     (21923) staff       (20)       45 2023-01-26 10:16:32.000000 ezcode-1.0.8/src/ezcode/Set/__init__.py
-drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 10:21:57.878289 ezcode-1.0.8/src/ezcode/Stack/
--rw-r--r--   0 zgao     (21923) staff       (20)      920 2023-01-20 20:45:20.000000 ezcode-1.0.8/src/ezcode/Stack/MinMaxStack.py
--rw-r--r--   0 zgao     (21923) staff       (20)     1693 2023-01-18 02:52:55.000000 ezcode-1.0.8/src/ezcode/Stack/PersistentStack.py
--rw-r--r--   0 zgao     (21923) staff       (20)     1260 2023-01-20 20:45:23.000000 ezcode-1.0.8/src/ezcode/Stack/Stack.py
--rw-r--r--   0 zgao     (21923) staff       (20)        0 2023-01-21 00:04:16.000000 ezcode-1.0.8/src/ezcode/Stack/StackOnPartialArray.py
--rw-r--r--   0 zgao     (21923) staff       (20)      122 2023-01-18 04:47:17.000000 ezcode-1.0.8/src/ezcode/Stack/__init__.py
-drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 10:21:57.888810 ezcode-1.0.8/src/ezcode/Tree/
--rw-r--r--   0 zgao     (21923) staff       (20)    12411 2023-01-26 09:58:36.000000 ezcode-1.0.8/src/ezcode/Tree/AVLTree.py
--rw-r--r--   0 zgao     (21923) staff       (20)     8280 2023-01-26 09:58:43.000000 ezcode-1.0.8/src/ezcode/Tree/BinarySearchTree.py
--rw-r--r--   0 zgao     (21923) staff       (20)    16040 2023-01-26 10:20:22.000000 ezcode-1.0.8/src/ezcode/Tree/BinaryTree.py
--rw-r--r--   0 zgao     (21923) staff       (20)     5133 2023-01-26 10:20:40.000000 ezcode-1.0.8/src/ezcode/Tree/BinaryTreeAlgorithm.py
--rw-r--r--   0 zgao     (21923) staff       (20)      209 2023-01-26 10:20:10.000000 ezcode-1.0.8/src/ezcode/Tree/BinaryTreeConstant.py
--rw-r--r--   0 zgao     (21923) staff       (20)     2760 2023-01-26 10:20:46.000000 ezcode-1.0.8/src/ezcode/Tree/BinaryTreeIterator.py
--rw-r--r--   0 zgao     (21923) staff       (20)     8046 2023-01-26 10:20:50.000000 ezcode-1.0.8/src/ezcode/Tree/BinaryTreePrinter.py
--rw-r--r--   0 zgao     (21923) staff       (20)     1409 2023-01-20 20:44:51.000000 ezcode-1.0.8/src/ezcode/Tree/DecisionTree.py
--rw-r--r--   0 zgao     (21923) staff       (20)     5343 2023-01-14 06:12:57.000000 ezcode-1.0.8/src/ezcode/Tree/FileSystem.py
--rw-r--r--   0 zgao     (21923) staff       (20)    13653 2023-01-26 09:58:30.000000 ezcode-1.0.8/src/ezcode/Tree/RedBlackTree.py
--rw-r--r--   0 zgao     (21923) staff       (20)    17298 2023-01-26 08:02:55.000000 ezcode-1.0.8/src/ezcode/Tree/RedBlackTreeWithParent.py
--rw-r--r--   0 zgao     (21923) staff       (20)     3464 2023-01-25 18:47:53.000000 ezcode-1.0.8/src/ezcode/Tree/SegmentTree.py
--rw-r--r--   0 zgao     (21923) staff       (20)     4013 2023-01-14 06:12:57.000000 ezcode-1.0.8/src/ezcode/Tree/Trie.py
--rw-r--r--   0 zgao     (21923) staff       (20)      241 2023-01-26 10:21:42.000000 ezcode-1.0.8/src/ezcode/Tree/__init__.py
--rw-r--r--   0 zgao     (21923) staff       (20)      781 2023-01-19 08:17:26.000000 ezcode-1.0.8/src/ezcode/Tree/dependency_trees.py
--rw-r--r--   0 zgao     (21923) staff       (20)     2106 2023-01-14 06:12:57.000000 ezcode-1.0.8/src/ezcode/Tree/disjoint_sets.py
-drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 10:21:57.891921 ezcode-1.0.8/src/ezcode/Utils/
--rw-r--r--   0 zgao     (21923) staff       (20)      287 2023-01-14 12:49:26.000000 ezcode-1.0.8/src/ezcode/Utils/Bit.py
--rw-r--r--   0 zgao     (21923) staff       (20)      249 2023-01-14 11:36:53.000000 ezcode-1.0.8/src/ezcode/Utils/Color.py
--rw-r--r--   0 zgao     (21923) staff       (20)     2488 2023-01-14 06:12:57.000000 ezcode-1.0.8/src/ezcode/Utils/Hash.py
--rw-r--r--   0 zgao     (21923) staff       (20)     1733 2023-01-14 06:12:57.000000 ezcode-1.0.8/src/ezcode/Utils/String.py
--rw-r--r--   0 zgao     (21923) staff       (20)     1130 2023-01-21 07:45:05.000000 ezcode-1.0.8/src/ezcode/Utils/__init__.py
--rw-r--r--   0 zgao     (21923) staff       (20)      407 2023-01-26 10:21:51.000000 ezcode-1.0.8/src/ezcode/__init__.py
-drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 10:21:57.843951 ezcode-1.0.8/src/ezcode.egg-info/
--rw-r--r--   0 zgao     (21923) staff       (20)     1361 2023-01-26 10:21:57.000000 ezcode-1.0.8/src/ezcode.egg-info/PKG-INFO
--rw-r--r--   0 zgao     (21923) staff       (20)     2459 2023-01-26 10:21:57.000000 ezcode-1.0.8/src/ezcode.egg-info/SOURCES.txt
--rw-r--r--   0 zgao     (21923) staff       (20)        1 2023-01-26 10:21:57.000000 ezcode-1.0.8/src/ezcode.egg-info/dependency_links.txt
--rw-r--r--   0 zgao     (21923) staff       (20)        7 2023-01-26 10:21:57.000000 ezcode-1.0.8/src/ezcode.egg-info/top_level.txt
+drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 11:08:56.414882 ezcode-1.0.9/
+-rw-r--r--   0 zgao     (21923) staff       (20)     1066 2023-01-14 06:12:57.000000 ezcode-1.0.9/LICENSE.md
+-rw-r--r--   0 zgao     (21923) staff       (20)     1361 2023-01-26 11:08:56.414205 ezcode-1.0.9/PKG-INFO
+-rw-r--r--   0 zgao     (21923) staff       (20)      769 2023-01-14 06:12:57.000000 ezcode-1.0.9/README.md
+-rw-r--r--   0 zgao     (21923) staff       (20)      132 2023-01-14 06:12:57.000000 ezcode-1.0.9/pyproject.toml
+-rw-r--r--   0 zgao     (21923) staff       (20)       38 2023-01-26 11:08:56.415057 ezcode-1.0.9/setup.cfg
+-rw-r--r--   0 zgao     (21923) staff       (20)     2160 2023-01-26 11:01:52.000000 ezcode-1.0.9/setup.py
+drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 11:08:56.349459 ezcode-1.0.9/src/
+drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 11:08:56.355502 ezcode-1.0.9/src/ezcode/
+drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 11:08:56.362928 ezcode-1.0.9/src/ezcode/Array/
+-rw-r--r--   0 zgao     (21923) staff       (20)    10900 2023-01-20 20:57:08.000000 ezcode-1.0.9/src/ezcode/Array/Interval.py
+-rw-r--r--   0 zgao     (21923) staff       (20)     4406 2023-01-14 06:12:57.000000 ezcode-1.0.9/src/ezcode/Array/Search.py
+-rw-r--r--   0 zgao     (21923) staff       (20)     1542 2023-01-14 06:12:57.000000 ezcode-1.0.9/src/ezcode/Array/Sort.py
+-rw-r--r--   0 zgao     (21923) staff       (20)     2149 2023-01-21 00:07:01.000000 ezcode-1.0.9/src/ezcode/Array/Sub.py
+-rw-r--r--   0 zgao     (21923) staff       (20)     7725 2023-01-21 07:52:27.000000 ezcode-1.0.9/src/ezcode/Array/Utils.py
+-rw-r--r--   0 zgao     (21923) staff       (20)        0 2023-01-14 06:12:57.000000 ezcode-1.0.9/src/ezcode/Array/__init__.py
+drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 11:08:56.364040 ezcode-1.0.9/src/ezcode/Cache/
+-rw-r--r--   0 zgao     (21923) staff       (20)     1250 2023-01-20 20:45:54.000000 ezcode-1.0.9/src/ezcode/Cache/LRUCache.py
+-rw-r--r--   0 zgao     (21923) staff       (20)        0 2023-01-23 00:24:04.000000 ezcode-1.0.9/src/ezcode/Cache/__init__.py
+drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 11:08:56.366227 ezcode-1.0.9/src/ezcode/Dynamic/
+-rw-r--r--   0 zgao     (21923) staff       (20)    28816 2023-01-14 06:12:57.000000 ezcode-1.0.9/src/ezcode/Dynamic/Knapsack.py
+-rw-r--r--   0 zgao     (21923) staff       (20)     5607 2023-01-21 10:28:16.000000 ezcode-1.0.9/src/ezcode/Dynamic/SparseTable.py
+-rw-r--r--   0 zgao     (21923) staff       (20)        2 2023-01-21 06:46:19.000000 ezcode-1.0.9/src/ezcode/Dynamic/__init__.py
+drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 11:08:56.368947 ezcode-1.0.9/src/ezcode/Graph/
+-rw-r--r--   0 zgao     (21923) staff       (20)     7075 2023-01-14 06:12:57.000000 ezcode-1.0.9/src/ezcode/Graph/DirectedGraph.py
+-rw-r--r--   0 zgao     (21923) staff       (20)    10645 2023-01-20 20:56:32.000000 ezcode-1.0.9/src/ezcode/Graph/GraphPathFinder.py
+-rw-r--r--   0 zgao     (21923) staff       (20)     4627 2023-01-14 06:12:57.000000 ezcode-1.0.9/src/ezcode/Graph/UndirectedGraph.py
+-rw-r--r--   0 zgao     (21923) staff       (20)     2689 2023-01-14 06:12:57.000000 ezcode-1.0.9/src/ezcode/Graph/__init__.py
+drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 11:08:56.371009 ezcode-1.0.9/src/ezcode/Grid/
+-rw-r--r--   0 zgao     (21923) staff       (20)    10287 2023-01-14 06:12:57.000000 ezcode-1.0.9/src/ezcode/Grid/GridIterator.py
+-rw-r--r--   0 zgao     (21923) staff       (20)    12024 2023-01-20 20:46:30.000000 ezcode-1.0.9/src/ezcode/Grid/GridPathFinder.py
+-rw-r--r--   0 zgao     (21923) staff       (20)     1877 2023-01-20 05:19:59.000000 ezcode-1.0.9/src/ezcode/Grid/__init__.py
+drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 11:08:56.373555 ezcode-1.0.9/src/ezcode/Heap/
+-rw-r--r--   0 zgao     (21923) staff       (20)     6148 2023-01-20 20:46:19.000000 ezcode-1.0.9/src/ezcode/Heap/PriorityMap.py
+-rw-r--r--   0 zgao     (21923) staff       (20)     5620 2023-01-19 08:03:02.000000 ezcode-1.0.9/src/ezcode/Heap/PriorityQueue.py
+-rw-r--r--   0 zgao     (21923) staff       (20)     5132 2023-01-19 08:03:38.000000 ezcode-1.0.9/src/ezcode/Heap/PriorityQueueOnPartialArray.py
+-rw-r--r--   0 zgao     (21923) staff       (20)        0 2023-01-14 06:12:57.000000 ezcode-1.0.9/src/ezcode/Heap/__init__.py
+drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 11:08:56.377153 ezcode-1.0.9/src/ezcode/List/
+-rw-r--r--   0 zgao     (21923) staff       (20)     4613 2023-01-20 20:46:12.000000 ezcode-1.0.9/src/ezcode/List/DoublyLinkedList.py
+-rw-r--r--   0 zgao     (21923) staff       (20)     3501 2023-01-20 20:46:08.000000 ezcode-1.0.9/src/ezcode/List/LinkedListAlgorithm.py
+-rw-r--r--   0 zgao     (21923) staff       (20)     2672 2023-01-20 20:46:04.000000 ezcode-1.0.9/src/ezcode/List/LinkedListPrinter.py
+-rw-r--r--   0 zgao     (21923) staff       (20)    11512 2023-01-21 07:57:10.000000 ezcode-1.0.9/src/ezcode/List/SinglyLinkedList.py
+-rw-r--r--   0 zgao     (21923) staff       (20)      158 2023-01-14 06:12:57.000000 ezcode-1.0.9/src/ezcode/List/__init__.py
+drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 11:08:56.378478 ezcode-1.0.9/src/ezcode/Map/
+-rw-r--r--   0 zgao     (21923) staff       (20)     2963 2023-01-26 11:02:51.000000 ezcode-1.0.9/src/ezcode/Map/TreeMap.py
+-rw-r--r--   0 zgao     (21923) staff       (20)       44 2023-01-26 10:16:21.000000 ezcode-1.0.9/src/ezcode/Map/__init__.py
+drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 11:08:56.383541 ezcode-1.0.9/src/ezcode/Math/
+-rw-r--r--   0 zgao     (21923) staff       (20)     4496 2023-01-19 07:59:19.000000 ezcode-1.0.9/src/ezcode/Math/Calculator.py
+-rw-r--r--   0 zgao     (21923) staff       (20)     3129 2023-01-19 07:51:48.000000 ezcode-1.0.9/src/ezcode/Math/Combination.py
+-rw-r--r--   0 zgao     (21923) staff       (20)     1508 2023-01-19 07:41:35.000000 ezcode-1.0.9/src/ezcode/Math/Enumeration.py
+-rw-r--r--   0 zgao     (21923) staff       (20)      584 2023-01-19 07:41:30.000000 ezcode-1.0.9/src/ezcode/Math/Partition.py
+-rw-r--r--   0 zgao     (21923) staff       (20)     3436 2023-01-20 23:27:14.000000 ezcode-1.0.9/src/ezcode/Math/Permutation.py
+-rw-r--r--   0 zgao     (21923) staff       (20)      250 2023-01-19 07:31:50.000000 ezcode-1.0.9/src/ezcode/Math/__init__.py
+drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 11:08:56.386881 ezcode-1.0.9/src/ezcode/Queue/
+-rw-r--r--   0 zgao     (21923) staff       (20)      682 2023-01-20 20:45:28.000000 ezcode-1.0.9/src/ezcode/Queue/MonotonicQueue.py
+-rw-r--r--   0 zgao     (21923) staff       (20)     1410 2023-01-20 20:45:32.000000 ezcode-1.0.9/src/ezcode/Queue/Queue.py
+-rw-r--r--   0 zgao     (21923) staff       (20)        0 2023-01-21 00:03:24.000000 ezcode-1.0.9/src/ezcode/Queue/QueueOnPartialArray.py
+-rw-r--r--   0 zgao     (21923) staff       (20)       82 2023-01-18 04:47:07.000000 ezcode-1.0.9/src/ezcode/Queue/__init__.py
+drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 11:08:56.390475 ezcode-1.0.9/src/ezcode/Random/
+-rw-r--r--   0 zgao     (21923) staff       (20)     3628 2023-01-20 19:06:20.000000 ezcode-1.0.9/src/ezcode/Random/RandomDict.py
+-rw-r--r--   0 zgao     (21923) staff       (20)     1984 2023-01-20 20:55:16.000000 ezcode-1.0.9/src/ezcode/Random/RandomIndex.py
+-rw-r--r--   0 zgao     (21923) staff       (20)     1323 2023-01-20 19:03:49.000000 ezcode-1.0.9/src/ezcode/Random/RandomSet.py
+-rw-r--r--   0 zgao     (21923) staff       (20)      289 2023-01-24 11:08:34.000000 ezcode-1.0.9/src/ezcode/Random/Shuffle.py
+-rw-r--r--   0 zgao     (21923) staff       (20)        0 2023-01-20 19:07:03.000000 ezcode-1.0.9/src/ezcode/Random/__init__.py
+drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 11:08:56.392033 ezcode-1.0.9/src/ezcode/Set/
+-rw-r--r--   0 zgao     (21923) staff       (20)     1046 2023-01-26 10:14:06.000000 ezcode-1.0.9/src/ezcode/Set/TreeSet.py
+-rw-r--r--   0 zgao     (21923) staff       (20)       45 2023-01-26 10:16:32.000000 ezcode-1.0.9/src/ezcode/Set/__init__.py
+drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 11:08:56.396145 ezcode-1.0.9/src/ezcode/Stack/
+-rw-r--r--   0 zgao     (21923) staff       (20)      920 2023-01-20 20:45:20.000000 ezcode-1.0.9/src/ezcode/Stack/MinMaxStack.py
+-rw-r--r--   0 zgao     (21923) staff       (20)     1693 2023-01-18 02:52:55.000000 ezcode-1.0.9/src/ezcode/Stack/PersistentStack.py
+-rw-r--r--   0 zgao     (21923) staff       (20)     1260 2023-01-20 20:45:23.000000 ezcode-1.0.9/src/ezcode/Stack/Stack.py
+-rw-r--r--   0 zgao     (21923) staff       (20)        0 2023-01-21 00:04:16.000000 ezcode-1.0.9/src/ezcode/Stack/StackOnPartialArray.py
+-rw-r--r--   0 zgao     (21923) staff       (20)      122 2023-01-18 04:47:17.000000 ezcode-1.0.9/src/ezcode/Stack/__init__.py
+drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 11:08:56.409806 ezcode-1.0.9/src/ezcode/Tree/
+-rw-r--r--   0 zgao     (21923) staff       (20)    12411 2023-01-26 09:58:36.000000 ezcode-1.0.9/src/ezcode/Tree/AVLTree.py
+-rw-r--r--   0 zgao     (21923) staff       (20)     8280 2023-01-26 09:58:43.000000 ezcode-1.0.9/src/ezcode/Tree/BinarySearchTree.py
+-rw-r--r--   0 zgao     (21923) staff       (20)    16040 2023-01-26 10:20:22.000000 ezcode-1.0.9/src/ezcode/Tree/BinaryTree.py
+-rw-r--r--   0 zgao     (21923) staff       (20)     5133 2023-01-26 10:20:40.000000 ezcode-1.0.9/src/ezcode/Tree/BinaryTreeAlgorithm.py
+-rw-r--r--   0 zgao     (21923) staff       (20)      209 2023-01-26 10:20:10.000000 ezcode-1.0.9/src/ezcode/Tree/BinaryTreeConstant.py
+-rw-r--r--   0 zgao     (21923) staff       (20)     2760 2023-01-26 10:20:46.000000 ezcode-1.0.9/src/ezcode/Tree/BinaryTreeIterator.py
+-rw-r--r--   0 zgao     (21923) staff       (20)     8046 2023-01-26 10:20:50.000000 ezcode-1.0.9/src/ezcode/Tree/BinaryTreePrinter.py
+-rw-r--r--   0 zgao     (21923) staff       (20)     1409 2023-01-20 20:44:51.000000 ezcode-1.0.9/src/ezcode/Tree/DecisionTree.py
+-rw-r--r--   0 zgao     (21923) staff       (20)     5343 2023-01-14 06:12:57.000000 ezcode-1.0.9/src/ezcode/Tree/FileSystem.py
+-rw-r--r--   0 zgao     (21923) staff       (20)    14136 2023-01-26 10:46:09.000000 ezcode-1.0.9/src/ezcode/Tree/RedBlackTree.py
+-rw-r--r--   0 zgao     (21923) staff       (20)    17298 2023-01-26 08:02:55.000000 ezcode-1.0.9/src/ezcode/Tree/RedBlackTreeWithParent.py
+-rw-r--r--   0 zgao     (21923) staff       (20)     3464 2023-01-25 18:47:53.000000 ezcode-1.0.9/src/ezcode/Tree/SegmentTree.py
+-rw-r--r--   0 zgao     (21923) staff       (20)     4013 2023-01-14 06:12:57.000000 ezcode-1.0.9/src/ezcode/Tree/Trie.py
+-rw-r--r--   0 zgao     (21923) staff       (20)      241 2023-01-26 10:21:42.000000 ezcode-1.0.9/src/ezcode/Tree/__init__.py
+-rw-r--r--   0 zgao     (21923) staff       (20)      781 2023-01-19 08:17:26.000000 ezcode-1.0.9/src/ezcode/Tree/dependency_trees.py
+-rw-r--r--   0 zgao     (21923) staff       (20)     2106 2023-01-14 06:12:57.000000 ezcode-1.0.9/src/ezcode/Tree/disjoint_sets.py
+drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 11:08:56.413242 ezcode-1.0.9/src/ezcode/Utils/
+-rw-r--r--   0 zgao     (21923) staff       (20)      287 2023-01-14 12:49:26.000000 ezcode-1.0.9/src/ezcode/Utils/Bit.py
+-rw-r--r--   0 zgao     (21923) staff       (20)      249 2023-01-14 11:36:53.000000 ezcode-1.0.9/src/ezcode/Utils/Color.py
+-rw-r--r--   0 zgao     (21923) staff       (20)     2488 2023-01-14 06:12:57.000000 ezcode-1.0.9/src/ezcode/Utils/Hash.py
+-rw-r--r--   0 zgao     (21923) staff       (20)     1733 2023-01-14 06:12:57.000000 ezcode-1.0.9/src/ezcode/Utils/String.py
+-rw-r--r--   0 zgao     (21923) staff       (20)     1130 2023-01-21 07:45:05.000000 ezcode-1.0.9/src/ezcode/Utils/__init__.py
+-rw-r--r--   0 zgao     (21923) staff       (20)      407 2023-01-26 10:21:51.000000 ezcode-1.0.9/src/ezcode/__init__.py
+drwxr-xr-x   0 zgao     (21923) staff       (20)        0 2023-01-26 11:08:56.358506 ezcode-1.0.9/src/ezcode.egg-info/
+-rw-r--r--   0 zgao     (21923) staff       (20)     1361 2023-01-26 11:08:56.000000 ezcode-1.0.9/src/ezcode.egg-info/PKG-INFO
+-rw-r--r--   0 zgao     (21923) staff       (20)     2459 2023-01-26 11:08:56.000000 ezcode-1.0.9/src/ezcode.egg-info/SOURCES.txt
+-rw-r--r--   0 zgao     (21923) staff       (20)        1 2023-01-26 11:08:56.000000 ezcode-1.0.9/src/ezcode.egg-info/dependency_links.txt
+-rw-r--r--   0 zgao     (21923) staff       (20)        7 2023-01-26 11:08:56.000000 ezcode-1.0.9/src/ezcode.egg-info/top_level.txt
```

### Comparing `ezcode-1.0.8/LICENSE.md` & `ezcode-1.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/PKG-INFO` & `ezcode-1.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezcode
-Version: 1.0.8
+Version: 1.0.9
 Summary: Easy Algorithm & Data Structure
 Home-page: https://github.com/zheng-gao/ez_code
 Author: Zheng Gao
 Author-email: mail.zheng.gao@gmail.com
 Project-URL: Documentation, https://github.com/zheng-gao/ez_code/blob/main/docs/readme.md
 Project-URL: Bug Tracker, https://github.com/zheng-gao/ez_code/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ezcode-1.0.8/README.md` & `ezcode-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/setup.py` & `ezcode-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 ez_code/ez.sh -o/--operations test -a/--arguments test_array.py::test_binary_search
 ```
 """
 
 
 setup(
     name="ezcode",
-    version="1.0.8",
+    version="1.0.9",
     author="Zheng Gao",
     author_email="mail.zheng.gao@gmail.com",
     description="Easy Algorithm & Data Structure",
     url="https://github.com/zheng-gao/ez_code",
     project_urls={
         "Documentation": "https://github.com/zheng-gao/ez_code/blob/main/docs/readme.md",
         "Bug Tracker": "https://github.com/zheng-gao/ez_code/issues",
```

### Comparing `ezcode-1.0.8/src/ezcode/Array/Interval.py` & `ezcode-1.0.9/src/ezcode/Array/Interval.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Array/Search.py` & `ezcode-1.0.9/src/ezcode/Array/Search.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Array/Sort.py` & `ezcode-1.0.9/src/ezcode/Array/Sort.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Array/Sub.py` & `ezcode-1.0.9/src/ezcode/Array/Sub.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Array/Utils.py` & `ezcode-1.0.9/src/ezcode/Array/Utils.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Cache/LRUCache.py` & `ezcode-1.0.9/src/ezcode/Cache/LRUCache.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Dynamic/Knapsack.py` & `ezcode-1.0.9/src/ezcode/Dynamic/Knapsack.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Dynamic/SparseTable.py` & `ezcode-1.0.9/src/ezcode/Dynamic/SparseTable.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Graph/DirectedGraph.py` & `ezcode-1.0.9/src/ezcode/Graph/DirectedGraph.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Graph/GraphPathFinder.py` & `ezcode-1.0.9/src/ezcode/Graph/GraphPathFinder.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Graph/UndirectedGraph.py` & `ezcode-1.0.9/src/ezcode/Graph/UndirectedGraph.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Graph/__init__.py` & `ezcode-1.0.9/src/ezcode/Graph/__init__.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Grid/GridIterator.py` & `ezcode-1.0.9/src/ezcode/Grid/GridIterator.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Grid/GridPathFinder.py` & `ezcode-1.0.9/src/ezcode/Grid/GridPathFinder.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Grid/__init__.py` & `ezcode-1.0.9/src/ezcode/Grid/__init__.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Heap/PriorityMap.py` & `ezcode-1.0.9/src/ezcode/Heap/PriorityMap.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Heap/PriorityQueue.py` & `ezcode-1.0.9/src/ezcode/Heap/PriorityQueue.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Heap/PriorityQueueOnPartialArray.py` & `ezcode-1.0.9/src/ezcode/Heap/PriorityQueueOnPartialArray.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/List/DoublyLinkedList.py` & `ezcode-1.0.9/src/ezcode/List/DoublyLinkedList.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/List/LinkedListAlgorithm.py` & `ezcode-1.0.9/src/ezcode/List/LinkedListAlgorithm.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/List/LinkedListPrinter.py` & `ezcode-1.0.9/src/ezcode/List/LinkedListPrinter.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/List/SinglyLinkedList.py` & `ezcode-1.0.9/src/ezcode/List/SinglyLinkedList.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Map/TreeMap.py` & `ezcode-1.0.9/src/ezcode/Map/TreeMap.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from typing import Iterable
 from ezcode.Tree.RedBlackTree import RedBlackTree
 from ezcode.Tree.BinarySearchTree import BinarySearchTree
 
 
 class TreeMap:
     class Entry:
         def __init__(self, key, value=None):
@@ -20,18 +19,18 @@
 
         def __str__(self):
             return f"{repr(self.key)},{repr(self.value)}"  # for tree printer
 
         def __repr__(self):
             return f"({repr(self.key)}, {repr(self.value)})"
 
-    def __init__(self, init_data: Iterable = None, tree: BinarySearchTree = RedBlackTree()):
+    def __init__(self, init_map=None, tree: BinarySearchTree = RedBlackTree()):
         self.tree = tree
-        if init_data is not None:
-            for key, value in init_data:
+        if init_map is not None:
+            for key, value in init_map.items():
                 self[key] = value
 
     def __len__(self):
         return len(self.tree)
 
     def __contains__(self, key):
         return TreeMap.Entry(key, None) in self.tree
```

### Comparing `ezcode-1.0.8/src/ezcode/Math/Calculator.py` & `ezcode-1.0.9/src/ezcode/Math/Calculator.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Math/Combination.py` & `ezcode-1.0.9/src/ezcode/Math/Combination.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Math/Enumeration.py` & `ezcode-1.0.9/src/ezcode/Math/Enumeration.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Math/Partition.py` & `ezcode-1.0.9/src/ezcode/Math/Partition.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Math/Permutation.py` & `ezcode-1.0.9/src/ezcode/Math/Permutation.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Queue/MonotonicQueue.py` & `ezcode-1.0.9/src/ezcode/Queue/MonotonicQueue.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Queue/Queue.py` & `ezcode-1.0.9/src/ezcode/Queue/Queue.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Random/RandomDict.py` & `ezcode-1.0.9/src/ezcode/Random/RandomDict.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Random/RandomIndex.py` & `ezcode-1.0.9/src/ezcode/Random/RandomIndex.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Random/RandomSet.py` & `ezcode-1.0.9/src/ezcode/Random/RandomSet.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Set/TreeSet.py` & `ezcode-1.0.9/src/ezcode/Set/TreeSet.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Stack/MinMaxStack.py` & `ezcode-1.0.9/src/ezcode/Stack/MinMaxStack.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Stack/PersistentStack.py` & `ezcode-1.0.9/src/ezcode/Stack/PersistentStack.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Stack/Stack.py` & `ezcode-1.0.9/src/ezcode/Stack/Stack.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Tree/AVLTree.py` & `ezcode-1.0.9/src/ezcode/Tree/AVLTree.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Tree/BinarySearchTree.py` & `ezcode-1.0.9/src/ezcode/Tree/BinarySearchTree.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Tree/BinaryTree.py` & `ezcode-1.0.9/src/ezcode/Tree/BinaryTree.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Tree/BinaryTreeAlgorithm.py` & `ezcode-1.0.9/src/ezcode/Tree/BinaryTreeAlgorithm.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Tree/BinaryTreeIterator.py` & `ezcode-1.0.9/src/ezcode/Tree/BinaryTreeIterator.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Tree/BinaryTreePrinter.py` & `ezcode-1.0.9/src/ezcode/Tree/BinaryTreePrinter.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Tree/DecisionTree.py` & `ezcode-1.0.9/src/ezcode/Tree/DecisionTree.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Tree/FileSystem.py` & `ezcode-1.0.9/src/ezcode/Tree/FileSystem.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Tree/RedBlackTree.py` & `ezcode-1.0.9/src/ezcode/Tree/RedBlackTree.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 from __future__ import annotations
 from typing import Iterable
 from ezcode.Tree.BinarySearchTree import BinarySearchTree
 
 
 class RedBlackTree(BinarySearchTree):
+    """
+                    RedBlackTree                          AVLTree
+     Storage        1 extra bit for color                 1 extra int for height
+    Balanced        Not Strictly Balanced                 Strictly Balanced
+      Search        O(logN)                               O(logN) faster
+      Insert        O(logN)                               O(logN) slightly faster
+    * Remove        O(logN) faster, rotations <= 3        O(logN) logN rotations, slower
+    """
     def __init__(self, init_data: Iterable = None, root=None, root_copy=None):
         super().__init__(
             init_data=init_data, root=root, root_copy=root_copy,
             data_name="data", left_name="left", right_name="right"
         )
 
     def new_node(self, is_red: bool = True, data=None, left=None, right=None):
```

### Comparing `ezcode-1.0.8/src/ezcode/Tree/RedBlackTreeWithParent.py` & `ezcode-1.0.9/src/ezcode/Tree/RedBlackTreeWithParent.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Tree/SegmentTree.py` & `ezcode-1.0.9/src/ezcode/Tree/SegmentTree.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Tree/Trie.py` & `ezcode-1.0.9/src/ezcode/Tree/Trie.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Tree/dependency_trees.py` & `ezcode-1.0.9/src/ezcode/Tree/dependency_trees.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Tree/disjoint_sets.py` & `ezcode-1.0.9/src/ezcode/Tree/disjoint_sets.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Utils/Hash.py` & `ezcode-1.0.9/src/ezcode/Utils/Hash.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Utils/String.py` & `ezcode-1.0.9/src/ezcode/Utils/String.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode/Utils/__init__.py` & `ezcode-1.0.9/src/ezcode/Utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ezcode-1.0.8/src/ezcode.egg-info/PKG-INFO` & `ezcode-1.0.9/src/ezcode.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezcode
-Version: 1.0.8
+Version: 1.0.9
 Summary: Easy Algorithm & Data Structure
 Home-page: https://github.com/zheng-gao/ez_code
 Author: Zheng Gao
 Author-email: mail.zheng.gao@gmail.com
 Project-URL: Documentation, https://github.com/zheng-gao/ez_code/blob/main/docs/readme.md
 Project-URL: Bug Tracker, https://github.com/zheng-gao/ez_code/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ezcode-1.0.8/src/ezcode.egg-info/SOURCES.txt` & `ezcode-1.0.9/src/ezcode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

