# Comparing `tmp/regisoup-0.1.7.tar.gz` & `tmp/regisoup-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regisoup-0.1.7.tar", max compression
+gzip compressed data, was "regisoup-0.1.8.tar", max compression
```

## Comparing `regisoup-0.1.7.tar` & `regisoup-0.1.8.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      276 2023-03-31 15:45:19.984515 regisoup-0.1.7/README.md
--rw-r--r--   0        0        0      504 2023-04-03 15:53:48.986670 regisoup-0.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-31 15:36:16.680509 regisoup-0.1.7/regisoup/__init__.py
--rw-r--r--   0        0        0     8734 2023-04-03 15:52:32.074541 regisoup-0.1.7/regisoup/main.py
--rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 regisoup-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      276 2023-03-31 15:45:19.984515 regisoup-0.1.8/README.md
+-rw-r--r--   0        0        0      504 2023-04-11 09:18:28.469575 regisoup-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-31 15:36:16.680509 regisoup-0.1.8/regisoup/__init__.py
+-rw-r--r--   0        0        0       47 2023-04-11 09:16:28.020368 regisoup-0.1.8/regisoup/__main__.py
+-rw-r--r--   0        0        0    12079 2023-04-07 15:33:11.175948 regisoup-0.1.8/regisoup/main.py
+-rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 regisoup-0.1.8/PKG-INFO
```

### Comparing `regisoup-0.1.7/regisoup/main.py` & `regisoup-0.1.8/regisoup/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,33 +8,76 @@
 import time
 import os
 
 MAX_ITER = 100
 warnings.simplefilter(action='ignore', category=FutureWarning)
 
 
-def cookSoup(filename: str):  # Alias open a file
+def cookSoup(filename: str) -> BeautifulSoup:
+    """Open a file as BeautifulSoup object.
+
+    Will eventually have to be merged with prepareIngredients().
+
+    Args:
+        filename: Filename of file to open.
+    
+    Returns:
+        A BeautifulSoup object containing all the contents of that
+        file.
+    """
     with open(filename) as f:
         soup = BeautifulSoup(f, "xml")
     
     return soup
 
 
-def prepareIngredients(filename: str):  # Alias convert &lt; and &gt: to < and >
+def prepareIngredients(filename: str) -> str:  # Alias convert &lt; and &gt: to < and >
+    """Unescape HTML characters.
+
+    This function unescapes HTML characters by saving the file as a decoded file.
+    The saved file is made temporary as it is later cleaned up by cleanUpKitchen().
+    This function should be deprecated in the future once I get around to merging it
+    with cookSoup() as it starts off almost identically as eatSoup().
+
+    Args:
+        filename: Filename of file to open.
+    
+    Returns:
+        output_filename: Filename of the temporary unescaped file.
+    """
+
     with open(filename) as f:
         ingredients = f.read()
     
     output_filename = filename.removesuffix(".xml") + str(time.time()) + ".xml"
     with open(output_filename, "w+") as f_out:
         f_out.write(html.unescape(ingredients))
 
     # Return temp file name, so we can recall it later
     return output_filename
 
-def modifyOpenSoupFigure(soup, caption: bool = True, verbose: bool = False, title: str = None):
+def modifyOpenSoupFigure(soup, caption: bool = True, verbose: bool = False, title: str = None)->int:
+    """Finds and replaces <figure> tags.
+
+    This function finds <figure> tags by their child <caption> tags and gets
+    things like id, page title and figure file from the tag. The tag is then replaced with the
+    new format as described in https://www.mediawiki.org/wiki/Extension:Figures. A quick
+    fix for replacing tags that then cease to exist (replace_with did not seem to cooperate) is
+    wrap them in dummy tags <p> which are later filtered out and removed by modifyOpenPTags().
+
+    Args:
+        soup: BeautifulSoup object that contains the page contents.
+        caption: If False will use ID for new figure label.
+        verbose: If True will be more verbose.
+        title: If given will use given title instead of found page title. Useful in situations, where tags
+            don't supply the page's title.
+    
+    Returns:
+        figure_counter: Returns number of modified <figure> tags.
+    """
     # Statistics counter
     figure_counter = 0
 
     for caption_tag in soup.find_all("caption"):
         figure_tag = caption_tag.parent
         
         if verbose:
@@ -80,14 +123,31 @@
         figure_tag.replace_with(clear_text_tag)
         figure_counter += 1
     
     return figure_counter
 
 
 def modifyOpenSoupCrossReference(soup, verbose: bool = False, title: str = None):
+    """Finds and replaces <xr> tags.
+
+    This function finds <xr> tags by their and gets
+    things like id and page title from the tag. The tag is then replaced with the
+    new format as described in https://www.mediawiki.org/wiki/Extension:Figures. A quick
+    fix for replacing tags that then cease to exist (replace_with did not seem to cooperate) is
+    wrap them in dummy tags <p> which are later filtered out and removed by modifyOpenPTags().
+
+    Args:
+        soup: BeautifulSoup object that contains the page contents.
+        verbose: If True will be more verbose.
+        title: If given will use given title instead of found page title. Useful in situations, where tags
+            don't supply the page's title.
+    
+    Returns:
+        xr_counter: Returns number of modified <figure> tags.
+    """
     # Statistics counter
     xr_counter = 0
     for xr_tag in soup.find_all("xr"):
         try:
             id = xr_tag["id"]
             # Find page name up the XML tree
             page = xr_tag.find_previous("title").string
@@ -106,28 +166,54 @@
         xr_tag.replace_with(clear_text_tag)
         xr_counter += 1
 
     return xr_counter
 
 
 def modifyOpenPTags(soup, verbose: bool = False):
-    # Might seem counter intuative to do so many passes of the document but it was 
+    """Finds and replaces dummy <p> tags.
+
+    This function finds dummy <p> tags that are added by modifyOpenSoupFigure() and 
+    modifyOpenSoupCrossReference().
+
+    Args:
+        soup: BeautifulSoup object that contains the page contents.
+        verbose: If True will be more verbose.
+    """
+    # Might seem counter intuitive to do so many passes of the document but it was 
     # the simplest method I could find.
     for p_tag in soup.find_all("p"):
         if verbose:
             print(f"[bold blue]Currently replacing:[/bold blue] {p_tag}")
         p_tag.replace_with(p_tag.string)
 
 
 
 def cleanUpKitchen(filename: str):  # Alias remove temp file
+    """Remove temporary converted file.
+
+    This function is used just as a fun alias for os.remove().
+
+    Args:
+        filename: Filename of file to remove.
+    """
     os.remove(filename)
 
 
 def eatSoup(output:str, soup, verbose: bool = False, magic: bool = True):  # Alias save file as string
+    """Save edited file as encoded file.
+
+    Currently the magic flag is not in use..
+
+    Args:
+        output: Filename of file to write output to.
+        soup: BeautifulSoup object that contains the page contents.
+        verbose: If True will be more verbose.
+        magic: If False will not do magic conversion of escaping HTML characters.
+    """
     # Save <text> contents as html, the rest as UTF-8 otherwise importDump.php complains.
     if magic:
         for text_tag in soup.find_all("text"):
             # Check through all content. If content is string, escape the HTML 
             # and put it back into the contents. Has to be contents otherwise <ref> tags go away.
             strings = [s for s in text_tag.strings]
             contents = [c for c in text_tag.contents]
```

### Comparing `regisoup-0.1.7/PKG-INFO` & `regisoup-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regisoup
-Version: 0.1.7
+Version: 0.1.8
 Summary: Convert <figure> and <xr> tags from deprecated MediaWiki extension to a new supported format.
 Author: pengu5055
 Author-email: urbancmarko1@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

