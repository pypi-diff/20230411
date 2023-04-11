# Comparing `tmp/kfsdutils-0.0.8.tar.gz` & `tmp/kfsdutils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfsdutils-0.0.8.tar", last modified: Fri Jan 14 05:58:02 2022, max compression
+gzip compressed data, was "kfsdutils-0.0.9.tar", last modified: Sat Feb 12 00:07:52 2022, max compression
```

## Comparing `kfsdutils-0.0.8.tar` & `kfsdutils-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 05:58:02.921148 kfsdutils-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)    34378 2022-01-14 05:57:50.000000 kfsdutils-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-01-14 05:58:02.921148 kfsdutils-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-01-14 05:57:50.000000 kfsdutils-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 05:58:02.917148 kfsdutils-0.0.8/kfsdutils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-14 05:57:50.000000 kfsdutils-0.0.8/kfsdutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3297 2022-01-14 05:57:50.000000 kfsdutils-0.0.8/kfsdutils/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1719 2022-01-14 05:57:50.000000 kfsdutils-0.0.8/kfsdutils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 05:58:02.921148 kfsdutils-0.0.8/kfsdutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-01-14 05:58:02.000000 kfsdutils-0.0.8/kfsdutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-01-14 05:58:02.000000 kfsdutils-0.0.8/kfsdutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-14 05:58:02.000000 kfsdutils-0.0.8/kfsdutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-14 05:58:02.000000 kfsdutils-0.0.8/kfsdutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-01-14 05:58:02.000000 kfsdutils-0.0.8/kfsdutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-01-14 05:58:02.000000 kfsdutils-0.0.8/kfsdutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-01-14 05:57:50.000000 kfsdutils-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-14 05:58:02.921148 kfsdutils-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-01-14 05:57:50.000000 kfsdutils-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-12 00:07:52.511787 kfsdutils-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    34378 2022-02-12 00:07:39.000000 kfsdutils-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      242 2022-02-12 00:07:52.511787 kfsdutils-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2022-02-12 00:07:39.000000 kfsdutils-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-12 00:07:52.511787 kfsdutils-0.0.9/kfsdutils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-12 00:07:39.000000 kfsdutils-0.0.9/kfsdutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3589 2022-02-12 00:07:39.000000 kfsdutils-0.0.9/kfsdutils/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1719 2022-02-12 00:07:39.000000 kfsdutils-0.0.9/kfsdutils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-12 00:07:52.511787 kfsdutils-0.0.9/kfsdutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      242 2022-02-12 00:07:52.000000 kfsdutils-0.0.9/kfsdutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      296 2022-02-12 00:07:52.000000 kfsdutils-0.0.9/kfsdutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-12 00:07:52.000000 kfsdutils-0.0.9/kfsdutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-12 00:07:52.000000 kfsdutils-0.0.9/kfsdutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-02-12 00:07:52.000000 kfsdutils-0.0.9/kfsdutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-02-12 00:07:52.000000 kfsdutils-0.0.9/kfsdutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2022-02-12 00:07:39.000000 kfsdutils-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-12 00:07:52.511787 kfsdutils-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      424 2022-02-12 00:07:39.000000 kfsdutils-0.0.9/setup.py
```

### Comparing `kfsdutils-0.0.8/LICENSE` & `kfsdutils-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.8/kfsdutils/base.py` & `kfsdutils-0.0.9/kfsdutils/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -105,15 +105,21 @@
 		if not os.path.exists(destPath):
 			return False
 		return True
 
 	def runCmd(self, cmd):
 		return subprocess.getoutput(cmd)
 
-	def cmdsExec(self, cmds):
-		return [self.cmdExec(cmd) if not type(cmd) == list else self.cmdsExec(cmd) for cmd in cmds]
+	def cmdsExec(self, cmds, returnOutput=True):
+		return [self.cmdExec(cmd, returnOutput) if not type(cmd) == list else self.cmdsExec(cmd, returnOutput) for cmd in cmds]
 
-	def cmdExec(self, cmd):
-		cmdOutput = subprocess.getstatusoutput(cmd)
-		returnVal = cmdOutput[1] if cmdOutput[0]==0 else None
-		self.log("INFO", "CMD: {}, Output: {}".format(cmd, returnVal))
-		return returnVal
+	def cmdExec(self, cmd, returnOutput=True):
+		if returnOutput:
+			cmdOutput = subprocess.getstatusoutput(cmd)
+			returnVal = cmdOutput[1] if cmdOutput[0]==0 else None
+			self.log("INFO", "CMD: {}, Output: {}".format(cmd, returnVal))
+			return returnVal
+		else:
+			args = shlex.split(cmd)
+			proc = subprocess.Popen(args, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+			for line in proc.stdout:
+				self.log("INFO", "{}".format(line.decode().strip()))
```

### Comparing `kfsdutils-0.0.8/kfsdutils/utils.py` & `kfsdutils-0.0.9/kfsdutils/utils.py`

 * *Files identical despite different names*

