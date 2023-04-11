# Comparing `tmp/dicebear-2.5.2.tar.gz` & `tmp/dicebear-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicebear-2.5.2.tar", last modified: Tue Mar 21 14:45:50 2023, max compression
+gzip compressed data, was "dicebear-2.6.1.tar", last modified: Tue Apr 11 14:58:11 2023, max compression
```

## Comparing `dicebear-2.5.2.tar` & `dicebear-2.6.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-03-21 14:45:50.596019 dicebear-2.5.2/
--rw-rw-rw-   0        0        0     1095 2023-01-24 16:05:16.000000 dicebear-2.5.2/LICENSE
--rw-rw-rw-   0        0        0    10312 2023-03-21 14:45:50.595021 dicebear-2.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     8331 2023-03-16 11:25:17.000000 dicebear-2.5.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-21 14:45:50.483662 dicebear-2.5.2/dicebear/
--rw-rw-rw-   0        0        0     1255 2023-03-21 14:42:37.000000 dicebear-2.5.2/dicebear/__init__.py
--rw-rw-rw-   0        0        0    17380 2023-03-21 14:15:09.000000 dicebear-2.5.2/dicebear/avatar.py
--rw-rw-rw-   0        0        0     3957 2023-02-28 14:02:30.000000 dicebear-2.5.2/dicebear/errors.py
--rw-rw-rw-   0        0        0     9064 2023-03-21 14:12:54.000000 dicebear-2.5.2/dicebear/models.py
--rw-rw-rw-   0        0        0     3776 2023-03-21 14:16:20.000000 dicebear-2.5.2/dicebear/utility.py
-drwxrwxrwx   0        0        0        0 2023-03-21 14:45:50.496821 dicebear-2.5.2/dicebear.egg-info/
--rw-rw-rw-   0        0        0    10312 2023-03-21 14:45:50.000000 dicebear-2.5.2/dicebear.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2023-03-21 14:45:50.000000 dicebear-2.5.2/dicebear.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-21 14:45:50.000000 dicebear-2.5.2/dicebear.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-03-21 14:45:50.000000 dicebear-2.5.2/dicebear.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-03-21 14:45:50.000000 dicebear-2.5.2/dicebear.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      414 2023-02-22 11:00:24.000000 dicebear-2.5.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-21 14:45:50.596019 dicebear-2.5.2/setup.cfg
--rw-rw-rw-   0        0        0     3670 2023-03-13 12:15:13.000000 dicebear-2.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-21 14:45:50.542734 dicebear-2.5.2/tests/
--rw-rw-rw-   0        0        0       23 2023-03-13 12:13:43.000000 dicebear-2.5.2/tests/__init__.py
--rw-rw-rw-   0        0        0     4423 2023-03-13 12:06:39.000000 dicebear-2.5.2/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2023-04-11 14:58:11.904641 dicebear-2.6.1/
+-rw-rw-rw-   0        0        0     1095 2023-01-24 16:05:16.000000 dicebear-2.6.1/LICENSE
+-rw-rw-rw-   0        0        0    10530 2023-04-11 14:58:11.904641 dicebear-2.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8519 2023-04-11 14:09:21.000000 dicebear-2.6.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 14:58:11.811595 dicebear-2.6.1/dicebear/
+-rw-rw-rw-   0        0        0     1255 2023-04-11 14:12:19.000000 dicebear-2.6.1/dicebear/__init__.py
+-rw-rw-rw-   0        0        0    17380 2023-04-11 14:14:36.000000 dicebear-2.6.1/dicebear/avatar.py
+-rw-rw-rw-   0        0        0     3957 2023-02-28 14:02:30.000000 dicebear-2.6.1/dicebear/errors.py
+-rw-rw-rw-   0        0        0     9066 2023-04-11 14:30:32.000000 dicebear-2.6.1/dicebear/models.py
+-rw-rw-rw-   0        0        0     4912 2023-04-11 14:53:52.000000 dicebear-2.6.1/dicebear/utility.py
+drwxrwxrwx   0        0        0        0 2023-04-11 14:58:11.834752 dicebear-2.6.1/dicebear.egg-info/
+-rw-rw-rw-   0        0        0    10530 2023-04-11 14:58:11.000000 dicebear-2.6.1/dicebear.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2023-04-11 14:58:11.000000 dicebear-2.6.1/dicebear.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 14:58:11.000000 dicebear-2.6.1/dicebear.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-11 14:58:11.000000 dicebear-2.6.1/dicebear.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-11 14:58:11.000000 dicebear-2.6.1/dicebear.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      414 2023-02-22 11:00:24.000000 dicebear-2.6.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-11 14:58:11.905637 dicebear-2.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     3706 2023-04-11 14:53:38.000000 dicebear-2.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 14:58:11.896106 dicebear-2.6.1/tests/
+-rw-rw-rw-   0        0        0       23 2023-03-13 12:13:43.000000 dicebear-2.6.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     4573 2023-04-11 14:41:58.000000 dicebear-2.6.1/tests/test_main.py
```

### Comparing `dicebear-2.5.2/LICENSE` & `dicebear-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dicebear-2.5.2/PKG-INFO` & `dicebear-2.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: dicebear
-Version: 2.5.2
+Version: 2.6.1
 Summary: A python wrapper for DiceBear's avatar generating API.
 Home-page: https://dicebear.janvh.tk
 Author: jvherck
 Author-email: contact@janvh.be
 Maintainer: jvherck
 Maintainer-email: contact@janvh.be
 License: MIT License
 Project-URL: Documentation, https://jvherck.github.io/dicebear
 Project-URL: Source, https://github.com/jvherck/dicebear
 Project-URL: Tracker, https://github.com/jvherck/dicebear/issues
-Keywords: python,dicebear,avatar,avatars,generating,generation,generator,API,wrapper,image,images,picture,pictures,png,jpg,svg,json,cli,pillow,pil,requests,adventurer,adventurer-neutral,avataaars,avataaars-neutral,big-ears,big-ears-neutral,big-smile,bottts,bottts-neutral,croodles,croodles-neutral,fun-emoji,icons,identicon,initials,lorelei,lorelei-neutral,micah,miniavs,open-peeps,personas,pixel-art,pixel-art-neutral,shapes,thumbs
+Keywords: python,dicebear,avatar,avatars,generating,generation,generator,API,wrapper,image,images,picture,pictures,png,jpg,svg,json,cli,pillow,pil,requests,adventurer,adventurer-neutral,avataaars,avataaars-neutral,big-ears,big-ears-neutral,big-smile,bottts,bottts-neutral,croodles,croodles-neutral,fun-emoji,icons,identicon,initials,lorelei,lorelei-neutral,micah,miniavs,notionists,notionists-neutral,open-peeps,personas,pixel-art,pixel-art-neutral,shapes,thumbs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
@@ -185,14 +185,16 @@
 * `icons`  
 * `identicon`  
 * `initials`  
 * `lorelei`  
 * `lorelei-neutral`  
 * `micah`  
 * `miniavs`  
+* `notionists`
+* `notionists-neutral`
 * `open-peeps`  
 * `personas`  
 * `pixel-art`  
 * `pixel-art-neutral`
 * `shapes`
 * `thumbs`
 
@@ -235,14 +237,16 @@
 * [icons](https://dicebear.com/styles/icons#options)  
 * [identicon](https://dicebear.com/styles/identicon#options)  
 * [initials](https://dicebear.com/styles/initials#options)  
 * [lorelei](https://dicebear.com/styles/lorelei#options)  
 * [lorelei-neutral](https://dicebear.com/styles/lorelei-neutral#options)  
 * [micah](https://dicebear.com/styles/micah#options)  
 * [miniavs](https://dicebear.com/styles/miniavs#options)  
+* [notionists](https://dicebear.com/styles/notionists#options)  
+* [notionists-neutral](https://dicebear.com/styles/notionists-neutral#options)  
 * [open-peeps](https://dicebear.com/styles/open-peeps#options)  
 * [personas](https://dicebear.com/styles/personas#options)  
 * [pixel-art](https://dicebear.com/styles/pixel-art#options)  
 * [pixel-art-neutral](https://dicebear.com/styles/pixel-art-neutral#options)  
 * [shapes](https://dicebear.com/styles/shapes#options)  
 * [thumbs](https://dicebear.com/styles/thumbs#options)
```

### Comparing `dicebear-2.5.2/README.md` & `dicebear-2.6.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -147,14 +147,16 @@
 * `icons`  
 * `identicon`  
 * `initials`  
 * `lorelei`  
 * `lorelei-neutral`  
 * `micah`  
 * `miniavs`  
+* `notionists`
+* `notionists-neutral`
 * `open-peeps`  
 * `personas`  
 * `pixel-art`  
 * `pixel-art-neutral`
 * `shapes`
 * `thumbs`
 
@@ -197,14 +199,16 @@
 * [icons](https://dicebear.com/styles/icons#options)  
 * [identicon](https://dicebear.com/styles/identicon#options)  
 * [initials](https://dicebear.com/styles/initials#options)  
 * [lorelei](https://dicebear.com/styles/lorelei#options)  
 * [lorelei-neutral](https://dicebear.com/styles/lorelei-neutral#options)  
 * [micah](https://dicebear.com/styles/micah#options)  
 * [miniavs](https://dicebear.com/styles/miniavs#options)  
+* [notionists](https://dicebear.com/styles/notionists#options)  
+* [notionists-neutral](https://dicebear.com/styles/notionists-neutral#options)  
 * [open-peeps](https://dicebear.com/styles/open-peeps#options)  
 * [personas](https://dicebear.com/styles/personas#options)  
 * [pixel-art](https://dicebear.com/styles/pixel-art#options)  
 * [pixel-art-neutral](https://dicebear.com/styles/pixel-art-neutral#options)  
 * [shapes](https://dicebear.com/styles/shapes#options)  
 * [thumbs](https://dicebear.com/styles/thumbs#options)
```

### Comparing `dicebear-2.5.2/dicebear/__init__.py` & `dicebear-2.6.1/dicebear/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 # SOFTWARE.
 
 from .avatar import *
 from .errors import *
 from .models import *
 from .utility import *
 
-__version__ = "2.5.2"
+__version__ = "2.6.1"
```

### Comparing `dicebear-2.5.2/dicebear/avatar.py` & `dicebear-2.6.1/dicebear/avatar.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     class i:
         class Image:
             def show(self): pass
 
 
     _FindPil.found = False
 
-_x = "https://api.dicebear.com/5.3/{}/svg?seed={}&"  # style, format, seed
+_x = "https://api.dicebear.com/6.x/{}/svg?seed={}&"  # style, format, seed
 
 
 class DAvatar:
     """
     Base class for the avatar generator.
     """
     default_options: dict = default_options
```

### Comparing `dicebear-2.5.2/dicebear/errors.py` & `dicebear-2.6.1/dicebear/errors.py`

 * *Files identical despite different names*

### Comparing `dicebear-2.5.2/dicebear/models.py` & `dicebear-2.6.1/dicebear/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+
 import signal
 from typing import Union, List
 from random import choice, choices
 from requests import post
 from contextlib import contextmanager
 
 from .errors import *
```

### Comparing `dicebear-2.5.2/dicebear/utility.py` & `dicebear-2.6.1/dicebear/utility.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,34 +17,35 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from string import ascii_lowercase, digits
-from random import choices
+from random import choices, choice, randint
 from typing import Union, List, Annotated
 
 from .avatar import DAvatar
-from .models import DStyle, DOptions, _statsIncrease
+from .models import DStyle, DOptions, DColor, _statsIncrease
 
 __all__ = (
     'create_avatar',
+    'create_random',
     'bulk_create',
 )
 __filename__ = "utility.py"
 
 
 def create_avatar(
-    style: DStyle,
-    seed: str,
-    options: Union[DOptions, None] = None,
-    customisations: Union[dict, None] = None,
-    *,
-    test: bool = False
+        style: DStyle,
+        seed: str,
+        options: Union[DOptions, None] = None,
+        customisations: Union[dict, None] = None,
+        *,
+        test: bool = False
 ) -> DAvatar:
     """
     Creates a DAvatar object and returns it.
 
     :param style: class `DStyle` :: the style of your avatar
     :param seed: class `str` :: the seed for the avatar; the avatar will be edited according to the seed
     :param options: class `DOptions` :: the options for the avatar
@@ -53,21 +54,47 @@
     :type test: bool
     :return: DAvatar object
     """
     _statsIncrease(__filename__, "/", ".create_avatar()", test)
     return DAvatar(style, seed, options=options, custom=customisations)
 
 
+def create_random(
+        randomOptions: bool = False,
+        *,
+        test: bool = False
+) -> DAvatar:
+    """
+    Creates a random DAvatar object and returns it.
+
+    :param randomOptions: class `bool` :: whether to use random (background) options for this avatar or not
+    :type randomOptions: bool
+    :param test: class `bool` :: to indicate if you are currently testing or not
+    :type test: bool
+    :return: DAvatar object
+    """
+    _statsIncrease(__filename__, "/", ".create_random()", test)
+    if randomOptions:
+        _type = choice(["solid", "gradientLinear"])
+        _color = [DColor.random()]
+        if _type == "gradientLinear": _color.append(DColor.random())
+        options = DOptions(flip=choice([True, False]), backgroundColor=DColor([str(x) for x in _color]),
+                           backgroundType=_type, backgroundRotation=randint(0, 360))
+    else:
+        options = None
+    return DAvatar(DStyle.random(), "".join(choices(ascii_lowercase + digits, k=20)), options=options)
+
+
 def bulk_create(
-    style: DStyle = DStyle.random(),
-    amount: Annotated[int, "Min: 1, Max: 50"] = 2,
-    *,
-    options: DOptions = None,
-    custom: dict = None,
-    test: bool = False
+        style: DStyle = DStyle.random(),
+        amount: Annotated[int, "Min: 1, Max: 50"] = 2,
+        *,
+        options: DOptions = None,
+        custom: dict = None,
+        test: bool = False
 ) -> List[DAvatar]:
     """
     Creates a list of :py:class:`DAvatar` objects. Easy way to make multiple of the same style (but different randomly generated seeds) at once.
 
     :param style: class `DStyle` :: the style to apply to all avatars
     :type style: dicebear.models.DStyle
     :param amount: class `int` :: the amount of DAvatars to create. Default: 2, Min: 1, Max: 50
```

### Comparing `dicebear-2.5.2/dicebear.egg-info/PKG-INFO` & `dicebear-2.6.1/dicebear.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: dicebear
-Version: 2.5.2
+Version: 2.6.1
 Summary: A python wrapper for DiceBear's avatar generating API.
 Home-page: https://dicebear.janvh.tk
 Author: jvherck
 Author-email: contact@janvh.be
 Maintainer: jvherck
 Maintainer-email: contact@janvh.be
 License: MIT License
 Project-URL: Documentation, https://jvherck.github.io/dicebear
 Project-URL: Source, https://github.com/jvherck/dicebear
 Project-URL: Tracker, https://github.com/jvherck/dicebear/issues
-Keywords: python,dicebear,avatar,avatars,generating,generation,generator,API,wrapper,image,images,picture,pictures,png,jpg,svg,json,cli,pillow,pil,requests,adventurer,adventurer-neutral,avataaars,avataaars-neutral,big-ears,big-ears-neutral,big-smile,bottts,bottts-neutral,croodles,croodles-neutral,fun-emoji,icons,identicon,initials,lorelei,lorelei-neutral,micah,miniavs,open-peeps,personas,pixel-art,pixel-art-neutral,shapes,thumbs
+Keywords: python,dicebear,avatar,avatars,generating,generation,generator,API,wrapper,image,images,picture,pictures,png,jpg,svg,json,cli,pillow,pil,requests,adventurer,adventurer-neutral,avataaars,avataaars-neutral,big-ears,big-ears-neutral,big-smile,bottts,bottts-neutral,croodles,croodles-neutral,fun-emoji,icons,identicon,initials,lorelei,lorelei-neutral,micah,miniavs,notionists,notionists-neutral,open-peeps,personas,pixel-art,pixel-art-neutral,shapes,thumbs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
@@ -185,14 +185,16 @@
 * `icons`  
 * `identicon`  
 * `initials`  
 * `lorelei`  
 * `lorelei-neutral`  
 * `micah`  
 * `miniavs`  
+* `notionists`
+* `notionists-neutral`
 * `open-peeps`  
 * `personas`  
 * `pixel-art`  
 * `pixel-art-neutral`
 * `shapes`
 * `thumbs`
 
@@ -235,14 +237,16 @@
 * [icons](https://dicebear.com/styles/icons#options)  
 * [identicon](https://dicebear.com/styles/identicon#options)  
 * [initials](https://dicebear.com/styles/initials#options)  
 * [lorelei](https://dicebear.com/styles/lorelei#options)  
 * [lorelei-neutral](https://dicebear.com/styles/lorelei-neutral#options)  
 * [micah](https://dicebear.com/styles/micah#options)  
 * [miniavs](https://dicebear.com/styles/miniavs#options)  
+* [notionists](https://dicebear.com/styles/notionists#options)  
+* [notionists-neutral](https://dicebear.com/styles/notionists-neutral#options)  
 * [open-peeps](https://dicebear.com/styles/open-peeps#options)  
 * [personas](https://dicebear.com/styles/personas#options)  
 * [pixel-art](https://dicebear.com/styles/pixel-art#options)  
 * [pixel-art-neutral](https://dicebear.com/styles/pixel-art-neutral#options)  
 * [shapes](https://dicebear.com/styles/shapes#options)  
 * [thumbs](https://dicebear.com/styles/thumbs#options)
```

### Comparing `dicebear-2.5.2/setup.py` & `dicebear-2.6.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,16 +41,16 @@
     packages=find_packages(),
     install_requires=['requests', 'urllib3'],
     python_requires='>=3.7',
     keywords=['python', 'dicebear', 'avatar', 'avatars', 'generating', 'generation', 'generator', 'API', 'wrapper',
               'image', 'images', 'picture', 'pictures', 'png', 'jpg', 'svg', 'json', 'cli', 'pillow', 'pil', 'requests',
               'adventurer', 'adventurer-neutral', 'avataaars', 'avataaars-neutral', 'big-ears', 'big-ears-neutral',
               'big-smile', 'bottts', 'bottts-neutral', 'croodles', 'croodles-neutral', 'fun-emoji', 'icons',
-              'identicon', 'initials', 'lorelei', 'lorelei-neutral', 'micah', 'miniavs', 'open-peeps', 'personas',
-              'pixel-art', 'pixel-art-neutral', 'shapes', 'thumbs'],
+              'identicon', 'initials', 'lorelei', 'lorelei-neutral', 'micah', 'miniavs', 'notionists',
+              'notionists-neutral', 'open-peeps', 'personas', 'pixel-art', 'pixel-art-neutral', 'shapes', 'thumbs'],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Other Audience",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
```

### Comparing `dicebear-2.5.2/tests/test_main.py` & `dicebear-2.6.1/tests/test_main.py`

 * *Files 8% similar despite different names*

```diff
@@ -101,14 +101,19 @@
         custom = {"face": "face04"}
         av = utility.create_avatar(style, seed, options, custom)
         self.assertEqual(
             av,
             avatar._x.format(quote(style), quote(seed)) + "rotate=90&face=face04"
         )
 
+    def testRandom(self):
+        av = utility.create_random(True)
+        _url_svg = av.url_svg
+        self.assertEqual(av.url_svg, _url_svg)
+
     def testMulti(self):
         style = models.DStyle.thumbs
         options = models.DOptions(rotate=90)
         custom = {"faceOffsetX": 15}
         avs = utility.bulk_create(style, 3, options=options, custom=custom)
         self.assertEqual(len(avs), 3)
         for item in avs:
```

