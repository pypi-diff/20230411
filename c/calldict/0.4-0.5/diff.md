# Comparing `tmp/calldict-0.4.tar.gz` & `tmp/calldict-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\calldict-0.4.tar", last modified: Tue Apr 11 17:13:51 2023, max compression
+gzip compressed data, was "dist\calldict-0.5.tar", last modified: Tue Apr 11 18:23:13 2023, max compression
```

## Comparing `calldict-0.4.tar` & `calldict-0.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 17:13:51.403276 calldict-0.4/
--rw-rw-rw-   0        0        0      400 2023-04-11 17:13:51.404275 calldict-0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-11 17:13:51.399276 calldict-0.4/calldict/
--rw-rw-rw-   0        0        0     6771 2023-04-11 17:12:17.052421 calldict-0.4/calldict/__init__.py
--rw-rw-rw-   0        0        0      535 2023-04-11 11:53:12.349672 calldict-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 18:23:13.316107 calldict-0.5/
+-rw-rw-rw-   0        0        0      400 2023-04-11 18:23:13.316107 calldict-0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-11 18:23:13.315107 calldict-0.5/calldict/
+-rw-rw-rw-   0        0        0     7128 2023-04-11 17:55:45.236743 calldict-0.5/calldict/__init__.py
+-rw-rw-rw-   0        0        0      535 2023-04-11 18:23:02.461336 calldict-0.5/setup.py
```

### Comparing `calldict-0.4/calldict/__init__.py` & `calldict-0.5/calldict/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,21 @@
     def __getattr__(self, name):
         if name in {'__setstate__'}:
             raise AttributeError
         if self.name is not None:
             name = self.name + '.' + name
         return self.__class__(name)
 
+    def __getitem__(self, key):
+        key = '[' + key + ']'
+        if self.name is not None:
+            key = self.name + key
+        return self.__class__(key)
+
+
     def __repr__(self):
         v = super(SharedValue, self).__repr__()
         return v[:v.find(' object')] + ('.' +
                                         self.name if self.name else '') + '>'
 
     def __deepcopy__(self, memo):
         return self
@@ -52,15 +59,16 @@
         return False
 
     def resolve(self, data):
         if not self.name:
             return data
         # use PEP-3101 field names specification to support attributes and
         # indexes
-        return string.Formatter().get_field(self.name, [], data)[0]
+        name = '0.' + self.name if self.name[0] != '[' else '0' + self.name
+        return string.Formatter().get_field(name, [data], {})[0]
 
 
 class SafeSharedValue(SharedValue):
     """
     Useful for multistage evaluation, when some values depends on other shared
     values and have to be resolved in several evaluations.
     """
@@ -173,11 +181,13 @@
     # Call itself
     result = data['func'](*data['args'], **data['kwargs'])
 
     if isinstance(result, SharedValue):
         result = result.resolve(shared_data)
 
     if 'returns' in data:
-        for v in data['returns'] if isinstance(data['returns'], list) else [data['returns']]:
+        for v in data['returns'] if isinstance(data['returns'],
+                                               list) else [data['returns']]:
             # support both, str and SharedValue instances
-            shared_data[v.name if isinstance(v, SharedValue) else v] = result
+            shared_data[v.name.strip('[]') if isinstance(v, SharedValue
+                                                         ) else v] = result
     return result
```

### Comparing `calldict-0.4/setup.py` & `calldict-0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='calldict',
     packages=['calldict'],
-    version='0.4',
+    version='0.5',
     description='Protocol to markup and evaluate functions in data structures',
     author='Konstantin Maslyuk',
     author_email='kostyamaslyuk@gmail.com',
     url='https://github.com/kalemas/calldict',
     download_url='https://github.com/kalemas/calldict/archive/master.zip',
     keywords=['dict', 'evaluation', 'yaml'],
     classifiers=[],
```

