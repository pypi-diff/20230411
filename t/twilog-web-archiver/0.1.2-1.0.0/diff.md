# Comparing `tmp/twilog-web-archiver-0.1.2.tar.gz` & `tmp/twilog-web-archiver-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twilog-web-archiver-0.1.2.tar", last modified: Sun Sep 20 10:10:38 2020, max compression
+gzip compressed data, was "twilog-web-archiver-1.0.0.tar", max compression
```

## Comparing `twilog-web-archiver-0.1.2.tar` & `twilog-web-archiver-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2020-09-20 09:37:45.033601 twilog-web-archiver-0.1.2/LICENSE
--rw-r--r--   0        0        0      805 2020-09-20 09:37:45.033601 twilog-web-archiver-0.1.2/README.rst
--rw-r--r--   0        0        0      789 2020-09-20 10:10:34.359731 twilog-web-archiver-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       22 2020-09-20 09:37:45.033601 twilog-web-archiver-0.1.2/twilog_web_archiver/__init__.py
--rw-r--r--   0        0        0     1308 2020-09-20 09:37:45.033601 twilog-web-archiver-0.1.2/twilog_web_archiver/main.py
--rw-r--r--   0        0        0     1798 2020-09-20 10:10:38.026667 twilog-web-archiver-0.1.2/setup.py
--rw-r--r--   0        0        0     1760 2020-09-20 10:10:38.027320 twilog-web-archiver-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-11 04:02:39.080251 twilog-web-archiver-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1193 2023-04-11 05:23:00.570375 twilog-web-archiver-1.0.0/README.rst
+-rw-r--r--   0        0        0      855 2023-04-11 05:28:46.479003 twilog-web-archiver-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-11 05:32:42.966969 twilog-web-archiver-1.0.0/twilog_web_archiver/__init__.py
+-rw-r--r--   0        0        0     1644 2023-04-11 05:21:18.916522 twilog-web-archiver-1.0.0/twilog_web_archiver/main.py
+-rw-r--r--   0        0        0     2212 2023-04-11 13:46:39.894416 twilog-web-archiver-1.0.0/setup.py
+-rw-r--r--   0        0        0     2098 2023-04-11 13:46:39.894624 twilog-web-archiver-1.0.0/PKG-INFO
```

### Comparing `twilog-web-archiver-0.1.2/LICENSE` & `twilog-web-archiver-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twilog-web-archiver-0.1.2/pyproject.toml` & `twilog-web-archiver-1.0.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 [tool.poetry]
 name = "twilog-web-archiver"
-version = "0.1.2"
-description = "Save month list pages of twilog.org by using archive.org."
+version = "1.0.0"
+description = "Archive twilog website month list pages into Internet Archive Wayback Machine"
 authors = ["TAKAHASHI Shuuji <shuuji3@gmail.com>"]
 
 license = 'GPL-3.0-or-later'
 
 readme = 'README.rst'
 
 repository = 'https://github.com/shuuji3/twilog-web-archiver'
 homepage = 'https://github.com/shuuji3/twilog-web-archiver'
 
-keywords = ['twilog', 'twitter', 'archive']
+keywords = ['twilog', 'twitter', 'archive', 'Wayback Machine', 'Internet Archive']
 
 [tool.poetry.scripts]
 twilog-web-archiver = "twilog_web_archiver.main:main"
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.9"
 bs4 = "^0.0.1"
-click = "^7.0"
+click = "^8.0"
 requests = "^2.21"
-savepagenow = ">=0.0.12,<1.1.1"
 lxml = "^4.3"
 pluggy = "^0.13.1"
+waybackpy = "^3.0.6"
 
 [tool.poetry.dev-dependencies]
-pytest = "^6.0"
+pytest = "^6.1"
 coverage = "^5.3"
+black = "^23.3.0"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `twilog-web-archiver-0.1.2/twilog_web_archiver/main.py` & `twilog-web-archiver-1.0.0/twilog_web_archiver/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,60 @@
 from typing import List
 
 from bs4 import BeautifulSoup
 import click
 import requests
-import savepagenow
+from waybackpy import WaybackMachineSaveAPI
 
 
 def get_month_links(screen_name: str) -> List[str]:
     """Get month link for the screen_name."""
     url = f'https://twilog.org/{screen_name}/archives'
     s = get_soup(url)
     return list(
-        filter(lambda x: 'month-' in x, map(lambda x: x['href'], s.select('section.main-list-box1 .side-list li a'))))
+        filter(
+            lambda x: 'month-' in x,
+            map(
+                lambda x: x['href'], s.select('section.main-list-box1 .side-list li a')
+            ),
+        )
+    )
 
 
 def get_soup(url: str) -> BeautifulSoup:
     """Get BeautifulSoup object for the url."""
     r = requests.get(url)
     return BeautifulSoup(r.text, 'lxml')
 
 
-def parse_month(month_link: str) -> None:
+def archive_month_pages(month_link: str) -> None:
     """Archive all the pages of the month list."""
-    archive_url, _ = savepagenow.capture_or_cache(month_link)
-    print('archived:', archive_url)
+    try:
+        save_api = WaybackMachineSaveAPI(month_link)
+        archive_url = save_api.archive_url
+        cached = save_api.cached_save
+        print(f'archived (cached: {cached}): {archive_url}')
+    except MaximumSaveRetriesExceeded as e:
+        print('⚠ failed to archive the page:')
+        print(e)
+
     s = get_soup(month_link)
     next_links = s.select('.nav-next a')
     if len(next_links) != 0:
         next_link = next_links[0]['href']
-        parse_month(next_link)
+        archive_month_pages(next_link)
 
 
 @click.command()
 @click.argument('screen_name')
 def archive_user_page(screen_name):
     """Archvie all month list pages for the specified screen_name into Wayback Machine."""
     month_links = get_month_links(screen_name)
     for month_link in month_links:
-        parse_month(month_link)
+        archive_month_pages(month_link)
 
 
 def main():
     archive_user_page()
 
 
 if __name__ == '__main__':
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `twilog-web-archiver-0.1.2/setup.py` & `twilog-web-archiver-1.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,35 +5,35 @@
 ['twilog_web_archiver']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['bs4>=0.0.1,<0.0.2',
- 'click>=7.0,<8.0',
+ 'click>=8.0,<9.0',
  'lxml>=4.3,<5.0',
  'pluggy>=0.13.1,<0.14.0',
  'requests>=2.21,<3.0',
- 'savepagenow>=0.0.12,<1.1.1']
+ 'waybackpy>=3.0.6,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['twilog-web-archiver = twilog_web_archiver.main:main']}
 
 setup_kwargs = {
     'name': 'twilog-web-archiver',
-    'version': '0.1.2',
-    'description': 'Save month list pages of twilog.org by using archive.org.',
-    'long_description': 'twilog-web-archiver\n===================\n\n.. image:: https://circleci.com/gh/shuuji3/twilog-web-archiver.svg?style=svg\n    :target: https://circleci.com/gh/shuuji3/twilog-web-archiver\n\nSave month list pages of twilog.org using archive.org.\n\nRequirement\n-----------\n\n- :code:`Python >= 3.6`\n\nInstall\n-------\n\n.. code-block:: bash\n\n    $ pip install twilog-web-archiver\n\nUsage\n-----\n\n.. code-block:: bash\n\n    $ twilog-web-archiver SCREEN_NAME\n\nDescription\n-----------\n\nWhen a user has registered twilog.org, you will see the month list page in the user archive page, i.e. `https://twilog.org/NHK_PR/archives <https://twilog.org/NHK_PR/archives>`_.\n\nThis program saves every pages in this month list into Wayback Machine on `archive.org <archive.org>`_.\n\nLicense\n-------\n\n- `GNU GPL 3.0 or later <LICENSE>`_\n',
+    'version': '1.0.0',
+    'description': 'Archive twilog website month list pages into Internet Archive Wayback Machine',
+    'long_description': 'twilog-web-archiver\n===================\n\nSave month list pages of twilog.org using archive.org.\n\nRequirement\n-----------\n\n- :code:`Python >= 3.9`\n\nInstall\n-------\n\n.. code-block:: bash\n\n    pip install twilog-web-archiver\n\nUsage\n-----\n\n.. code-block:: bash\n\n    twilog-web-archiver SCREEN_NAME\n\nExample output\n--------------\n\n.. code-block:: bash\n\n    twilog-web-archiver nhk_pr\n    archived (cached: True): https://web.archive.org/web/20230411042930/https://twilog.org/NHK_PR/month-2304\n    archived (cached: True): https://web.archive.org/web/20230411051906/https://twilog.org/NHK_PR/month-2303\n    archived (cached: False): https://web.archive.org/web/20230411051956/https://twilog.org/NHK_PR/month-2303/2\n    archived (cached: False): https://web.archive.org/web/20230411052032/https://twilog.org/NHK_PR/month-2303/3\n    ...\n\nDescription\n-----------\n\nWhen a user has registered twilog.org, you will see the month list page in the user archive page, i.e. `https://twilog.org/NHK_PR/archives <https://twilog.org/NHK_PR/archives>`_.\n\nThis program saves every pages in this month list into Wayback Machine on `archive.org <archive.org>`_.\n\nLicense\n-------\n\n- `GNU GPL 3.0 or later <LICENSE>`_\n',
     'author': 'TAKAHASHI Shuuji',
     'author_email': 'shuuji3@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/shuuji3/twilog-web-archiver',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.6,<4.0',
+    'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `twilog-web-archiver-0.1.2/PKG-INFO` & `twilog-web-archiver-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,64 @@
 Metadata-Version: 2.1
 Name: twilog-web-archiver
-Version: 0.1.2
-Summary: Save month list pages of twilog.org by using archive.org.
+Version: 1.0.0
+Summary: Archive twilog website month list pages into Internet Archive Wayback Machine
 Home-page: https://github.com/shuuji3/twilog-web-archiver
 License: GPL-3.0-or-later
-Keywords: twilog,twitter,archive
+Keywords: twilog,twitter,archive,Wayback Machine,Internet Archive
 Author: TAKAHASHI Shuuji
 Author-email: shuuji3@gmail.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
-Requires-Dist: click (>=7.0,<8.0)
+Requires-Dist: click (>=8.0,<9.0)
 Requires-Dist: lxml (>=4.3,<5.0)
 Requires-Dist: pluggy (>=0.13.1,<0.14.0)
 Requires-Dist: requests (>=2.21,<3.0)
-Requires-Dist: savepagenow (>=0.0.12,<1.1.1)
+Requires-Dist: waybackpy (>=3.0.6,<4.0.0)
 Project-URL: Repository, https://github.com/shuuji3/twilog-web-archiver
 Description-Content-Type: text/x-rst
 
 twilog-web-archiver
 ===================
 
-.. image:: https://circleci.com/gh/shuuji3/twilog-web-archiver.svg?style=svg
-    :target: https://circleci.com/gh/shuuji3/twilog-web-archiver
-
 Save month list pages of twilog.org using archive.org.
 
 Requirement
 -----------
 
-- :code:`Python >= 3.6`
+- :code:`Python >= 3.9`
 
 Install
 -------
 
 .. code-block:: bash
 
-    $ pip install twilog-web-archiver
+    pip install twilog-web-archiver
 
 Usage
 -----
 
 .. code-block:: bash
 
-    $ twilog-web-archiver SCREEN_NAME
+    twilog-web-archiver SCREEN_NAME
+
+Example output
+--------------
+
+.. code-block:: bash
+
+    twilog-web-archiver nhk_pr
+    archived (cached: True): https://web.archive.org/web/20230411042930/https://twilog.org/NHK_PR/month-2304
+    archived (cached: True): https://web.archive.org/web/20230411051906/https://twilog.org/NHK_PR/month-2303
+    archived (cached: False): https://web.archive.org/web/20230411051956/https://twilog.org/NHK_PR/month-2303/2
+    archived (cached: False): https://web.archive.org/web/20230411052032/https://twilog.org/NHK_PR/month-2303/3
+    ...
 
 Description
 -----------
 
 When a user has registered twilog.org, you will see the month list page in the user archive page, i.e. `https://twilog.org/NHK_PR/archives <https://twilog.org/NHK_PR/archives>`_.
 
 This program saves every pages in this month list into Wayback Machine on `archive.org <archive.org>`_.
```

