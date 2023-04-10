# Comparing `tmp/llamabot-0.0.4.tar.gz` & `tmp/llamabot-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llamabot-0.0.4.tar", last modified: Mon Apr  3 20:31:05 2023, max compression
+gzip compressed data, was "llamabot-0.0.5.tar", last modified: Mon Apr 10 22:48:22 2023, max compression
```

## Comparing `llamabot-0.0.4.tar` & `llamabot-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-03 20:31:05.364391 llamabot-0.0.4/
--rw-r--r--   0 ericmjl    (501) staff       (20)      124 2023-04-03 18:38:54.000000 llamabot-0.0.4/MANIFEST.in
--rw-r--r--   0 ericmjl    (501) staff       (20)       95 2023-04-03 20:31:05.364247 llamabot-0.0.4/PKG-INFO
--rw-r--r--   0 ericmjl    (501) staff       (20)     5549 2023-04-03 19:37:38.000000 llamabot-0.0.4/README.md
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-03 20:31:05.362910 llamabot-0.0.4/llamabot/
--rw-r--r--   0 ericmjl    (501) staff       (20)      262 2023-04-03 18:42:06.000000 llamabot-0.0.4/llamabot/__init__.py
--rw-r--r--   0 ericmjl    (501) staff       (20)     2724 2023-04-03 18:39:42.000000 llamabot-0.0.4/llamabot/bot.py
--rw-r--r--   0 ericmjl    (501) staff       (20)      652 2023-04-03 18:38:54.000000 llamabot-0.0.4/llamabot/cli.py
--rw-r--r--   0 ericmjl    (501) staff       (20)       35 2023-04-03 18:38:54.000000 llamabot-0.0.4/llamabot/preprocessing.py
--rw-r--r--   0 ericmjl    (501) staff       (20)      182 2023-04-03 18:38:54.000000 llamabot-0.0.4/llamabot/schemas.py
--rw-r--r--   0 ericmjl    (501) staff       (20)       30 2023-04-03 18:38:54.000000 llamabot-0.0.4/llamabot/utils.py
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-03 20:31:05.363680 llamabot-0.0.4/llamabot.egg-info/
--rw-r--r--   0 ericmjl    (501) staff       (20)       95 2023-04-03 20:31:05.000000 llamabot-0.0.4/llamabot.egg-info/PKG-INFO
--rw-r--r--   0 ericmjl    (501) staff       (20)      409 2023-04-03 20:31:05.000000 llamabot-0.0.4/llamabot.egg-info/SOURCES.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)        1 2023-04-03 20:31:05.000000 llamabot-0.0.4/llamabot.egg-info/dependency_links.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)       46 2023-04-03 20:31:05.000000 llamabot-0.0.4/llamabot.egg-info/entry_points.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)       64 2023-04-03 20:31:05.000000 llamabot-0.0.4/llamabot.egg-info/requires.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)        9 2023-04-03 20:31:05.000000 llamabot-0.0.4/llamabot.egg-info/top_level.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)     1482 2023-04-03 20:31:01.000000 llamabot-0.0.4/pyproject.toml
--rw-r--r--   0 ericmjl    (501) staff       (20)       38 2023-04-03 20:31:05.364427 llamabot-0.0.4/setup.cfg
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-03 20:31:05.364060 llamabot-0.0.4/tests/
--rw-r--r--   0 ericmjl    (501) staff       (20)       26 2023-04-03 18:38:54.000000 llamabot-0.0.4/tests/test___init__.py
--rw-r--r--   0 ericmjl    (501) staff       (20)       30 2023-04-03 18:38:54.000000 llamabot-0.0.4/tests/test_cli.py
--rw-r--r--   0 ericmjl    (501) staff       (20)       52 2023-04-03 18:38:54.000000 llamabot-0.0.4/tests/test_models.py
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-10 22:48:22.371590 llamabot-0.0.5/
+-rw-r--r--   0 ericmjl    (501) staff       (20)      124 2023-04-03 18:38:54.000000 llamabot-0.0.5/MANIFEST.in
+-rw-r--r--   0 ericmjl    (501) staff       (20)       95 2023-04-10 22:48:22.371441 llamabot-0.0.5/PKG-INFO
+-rw-r--r--   0 ericmjl    (501) staff       (20)     5647 2023-04-04 15:17:20.000000 llamabot-0.0.5/README.md
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-10 22:48:22.369794 llamabot-0.0.5/llamabot/
+-rw-r--r--   0 ericmjl    (501) staff       (20)      284 2023-04-10 22:45:50.000000 llamabot-0.0.5/llamabot/__init__.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)     5720 2023-04-10 22:47:57.000000 llamabot-0.0.5/llamabot/bot.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)      652 2023-04-03 18:38:54.000000 llamabot-0.0.5/llamabot/cli.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)       35 2023-04-03 18:38:54.000000 llamabot-0.0.5/llamabot/preprocessing.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)      182 2023-04-03 18:38:54.000000 llamabot-0.0.5/llamabot/schemas.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)       30 2023-04-03 18:38:54.000000 llamabot-0.0.5/llamabot/utils.py
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-10 22:48:22.370635 llamabot-0.0.5/llamabot.egg-info/
+-rw-r--r--   0 ericmjl    (501) staff       (20)       95 2023-04-10 22:48:22.000000 llamabot-0.0.5/llamabot.egg-info/PKG-INFO
+-rw-r--r--   0 ericmjl    (501) staff       (20)      409 2023-04-10 22:48:22.000000 llamabot-0.0.5/llamabot.egg-info/SOURCES.txt
+-rw-r--r--   0 ericmjl    (501) staff       (20)        1 2023-04-10 22:48:22.000000 llamabot-0.0.5/llamabot.egg-info/dependency_links.txt
+-rw-r--r--   0 ericmjl    (501) staff       (20)       46 2023-04-10 22:48:22.000000 llamabot-0.0.5/llamabot.egg-info/entry_points.txt
+-rw-r--r--   0 ericmjl    (501) staff       (20)       90 2023-04-10 22:48:22.000000 llamabot-0.0.5/llamabot.egg-info/requires.txt
+-rw-r--r--   0 ericmjl    (501) staff       (20)        9 2023-04-10 22:48:22.000000 llamabot-0.0.5/llamabot.egg-info/top_level.txt
+-rw-r--r--   0 ericmjl    (501) staff       (20)     1529 2023-04-10 22:48:19.000000 llamabot-0.0.5/pyproject.toml
+-rw-r--r--   0 ericmjl    (501) staff       (20)       38 2023-04-10 22:48:22.371632 llamabot-0.0.5/setup.cfg
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-10 22:48:22.371231 llamabot-0.0.5/tests/
+-rw-r--r--   0 ericmjl    (501) staff       (20)       26 2023-04-03 18:38:54.000000 llamabot-0.0.5/tests/test___init__.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)       30 2023-04-03 18:38:54.000000 llamabot-0.0.5/tests/test_cli.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)       52 2023-04-03 18:38:54.000000 llamabot-0.0.5/tests/test_models.py
```

### Comparing `llamabot-0.0.4/README.md` & `llamabot-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # LLaMaBot: A Pythonic bot interface to LLMs
 
 LLaMaBot implements a Pythonic interface to LLMs,
-making it much easier to experiment with LLMs in a Jupyter notebook.
+making it much easier to experiment with LLMs in a Jupyter notebook
+and build simple utility apps that utilize LLMs.
 The model that we default to using is OpenAI's largest GPT-4 model.
 
 ## Install LLaMaBot
 
 To install LLaMaBot:
 
 ```python
@@ -23,18 +24,21 @@
 
 We recommend setting the environment variable in a `.env` file
 in the root of your project repository.
 From there, `llamabot` will automagically load the environment variable for you.
 
 ### Simple Bot
 
-The simplest use case of LLaMaBot is to create a simple bot that keeps no record of chat history.
+The simplest use case of LLaMaBot
+is to create a simple bot that keeps no record of chat history.
 This is useful for prompt experimentation,
-or for creating simple bots that can be called upon repeatedly with different messages.
-For example, to create a Bot that explains a given chunk of text like Richard Feynman would:
+or for creating simple bots that are preconditioned on an instruction to handle texts
+and are then called upon repeatedly with different texts.
+For example, to create a Bot that explains a given chunk of text
+like Richard Feynman would:
 
 ```python
 from llamabot import SimpleBot
 
 feynman = SimpleBot("You are Richard Feynman. You will be given a difficult concept, and your task is to explain it back.")
 ```
 
@@ -43,16 +47,18 @@
 
 ```python
 feynman("Enzyme function annotation is a fundamental challenge, and numerous computational tools have been developed. However, most of these tools cannot accurately predict functional annotations, such as enzyme commission (EC) number, for less-studied proteins or those with previously uncharacterized functions or multiple activities. We present a machine learning algorithm named CLEAN (contrastive learning–enabled enzyme annotation) to assign EC numbers to enzymes with better accuracy, reliability, and sensitivity compared with the state-of-the-art tool BLASTp. The contrastive learning framework empowers CLEAN to confidently (i) annotate understudied enzymes, (ii) correct mislabeled enzymes, and (iii) identify promiscuous enzymes with two or more EC numbers—functions that we demonstrate by systematic in silico and in vitro experiments. We anticipate that this tool will be widely used for predicting the functions of uncharacterized enzymes, thereby advancing many fields, such as genomics, synthetic biology, and biocatalysis.")
 ```
 
 ### Chat Bot
 
-To experiment with a Chat Bot in the Jupyter notebook, we also provide the ChatBot interface.
-This interface automagically keeps track of chat history for as long as your Jupyter session is alive.
+To experiment with a Chat Bot in the Jupyter notebook,
+we also provide the ChatBot interface.
+This interface automagically keeps track of chat history
+for as long as your Jupyter session is alive.
 Doing so allows you to use your own local Jupyter notebook as a chat interface.
 
 For example:
 
 ```python
 from llamabot import ChatBot
 
@@ -81,15 +87,15 @@
 
 ### Bug reports
 
 Please submit a bug report using the issue tracker.
 
 ### Questions/Discussions
 
-Please use the Discussions feature on GitHub.
+Please use the issue tracker on GitHub.
 
 ## Contributors
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
```

### Comparing `llamabot-0.0.4/llamabot/cli.py` & `llamabot-0.0.5/llamabot/cli.py`

 * *Files identical despite different names*

