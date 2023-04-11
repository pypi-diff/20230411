# Comparing `tmp/ckanext-comments-0.2.0.tar.gz` & `tmp/ckanext-comments-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-comments-0.2.0.tar", last modified: Mon Apr  3 15:47:51 2023, max compression
+gzip compressed data, was "ckanext-comments-0.3.0.tar", last modified: Tue Apr 11 14:42:11 2023, max compression
```

## Comparing `ckanext-comments-0.2.0.tar` & `ckanext-comments-0.3.0.tar`

### file list

```diff
@@ -1,100 +1,82 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 15:47:51.489851 ckanext-comments-0.2.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       67 2022-11-08 21:05:03.000000 ckanext-comments-0.2.0/.coveragerc
--rw-r--r--   0 sergey    (1000) sergey    (1000)      267 2022-11-08 21:05:03.000000 ckanext-comments-0.2.0/.editorconfig
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 15:47:51.429852 ckanext-comments-0.2.0/.github/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 15:47:51.469851 ckanext-comments-0.2.0/.github/workflows/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1950 2023-03-01 00:26:28.000000 ckanext-comments-0.2.0/.github/workflows/test.yml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      620 2023-03-03 00:16:07.000000 ckanext-comments-0.2.0/.gitignore
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1307 2023-04-03 15:47:33.000000 ckanext-comments-0.2.0/CHANGELOG.md
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2022-11-08 21:05:03.000000 ckanext-comments-0.2.0/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      208 2023-03-03 00:10:04.000000 ckanext-comments-0.2.0/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4762 2023-04-03 15:47:51.489851 ckanext-comments-0.2.0/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4115 2023-03-01 17:33:07.000000 ckanext-comments-0.2.0/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 15:47:51.469851 ckanext-comments-0.2.0/ckanext/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2022-11-28 18:43:47.000000 ckanext-comments-0.2.0/ckanext/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 15:47:51.479851 ckanext-comments-0.2.0/ckanext/comments/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-11-08 21:05:03.000000 ckanext-comments-0.2.0/ckanext/comments/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 15:47:51.479851 ckanext-comments-0.2.0/ckanext/comments/assets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-11-08 21:05:03.000000 ckanext-comments-0.2.0/ckanext/comments/assets/.gitignore
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 15:47:51.479851 ckanext-comments-0.2.0/ckanext/comments/assets/css/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1675 2022-11-08 21:05:03.000000 ckanext-comments-0.2.0/ckanext/comments/assets/css/comments-thread.css
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 15:47:51.479851 ckanext-comments-0.2.0/ckanext/comments/assets/js/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5608 2023-03-01 11:53:33.000000 ckanext-comments-0.2.0/ckanext/comments/assets/js/comments-thread.js
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 15:47:51.479851 ckanext-comments-0.2.0/ckanext/comments/assets/less/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2129 2022-11-08 21:05:03.000000 ckanext-comments-0.2.0/ckanext/comments/assets/less/comments-thread.less
--rw-r--r--   0 sergey    (1000) sergey    (1000)      326 2022-11-08 21:05:03.000000 ckanext-comments-0.2.0/ckanext/comments/assets/webassets.yml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2294 2023-03-28 11:57:40.000000 ckanext-comments-0.2.0/ckanext/comments/config.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      110 2023-03-01 20:44:22.000000 ckanext-comments-0.2.0/ckanext/comments/config_declaration.yaml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      158 2022-11-08 21:05:03.000000 ckanext-comments-0.2.0/ckanext/comments/exceptions.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1540 2023-03-28 11:57:40.000000 ckanext-comments-0.2.0/ckanext/comments/helpers.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 15:47:51.479851 ckanext-comments-0.2.0/ckanext/comments/i18n/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-11-08 21:05:03.000000 ckanext-comments-0.2.0/ckanext/comments/i18n/.gitignore
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 15:47:51.479851 ckanext-comments-0.2.0/ckanext/comments/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-11-08 21:05:03.000000 ckanext-comments-0.2.0/ckanext/comments/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8285 2023-03-28 11:57:40.000000 ckanext-comments-0.2.0/ckanext/comments/logic/action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2595 2023-03-28 11:57:40.000000 ckanext-comments-0.2.0/ckanext/comments/logic/auth.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1942 2023-03-28 11:57:40.000000 ckanext-comments-0.2.0/ckanext/comments/logic/schema.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      460 2023-03-28 11:57:40.000000 ckanext-comments-0.2.0/ckanext/comments/logic/validators.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 15:47:51.439851 ckanext-comments-0.2.0/ckanext/comments/migration/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 15:47:51.479851 ckanext-comments-0.2.0/ckanext/comments/migration/comments/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2022-11-08 21:05:03.000000 ckanext-comments-0.2.0/ckanext/comments/migration/comments/README
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1800 2022-11-08 21:05:03.000000 ckanext-comments-0.2.0/ckanext/comments/migration/comments/alembic.ini
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2228 2023-03-28 11:57:40.000000 ckanext-comments-0.2.0/ckanext/comments/migration/comments/env.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      494 2022-11-08 21:05:03.000000 ckanext-comments-0.2.0/ckanext/comments/migration/comments/script.py.mako
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 15:47:51.479851 ckanext-comments-0.2.0/ckanext/comments/migration/comments/versions/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1803 2023-03-28 11:57:37.000000 ckanext-comments-0.2.0/ckanext/comments/migration/comments/versions/275515c51af1_init_tables.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 15:47:51.479851 ckanext-comments-0.2.0/ckanext/comments/model/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       89 2023-04-03 15:46:05.000000 ckanext-comments-0.2.0/ckanext/comments/model/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)       83 2022-11-08 21:05:03.000000 ckanext-comments-0.2.0/ckanext/comments/model/base.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2885 2023-03-28 11:57:40.000000 ckanext-comments-0.2.0/ckanext/comments/model/comment.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3272 2023-03-28 11:57:40.000000 ckanext-comments-0.2.0/ckanext/comments/model/dictize.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2108 2023-03-28 11:57:40.000000 ckanext-comments-0.2.0/ckanext/comments/model/thread.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1248 2023-03-28 11:57:40.000000 ckanext-comments-0.2.0/ckanext/comments/plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 15:47:51.479851 ckanext-comments-0.2.0/ckanext/comments/public/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-11-08 21:05:03.000000 ckanext-comments-0.2.0/ckanext/comments/public/.gitignore
--rw-r--r--   0 sergey    (1000) sergey    (1000)      773 2023-03-28 11:57:40.000000 ckanext-comments-0.2.0/ckanext/comments/signals.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 15:47:51.479851 ckanext-comments-0.2.0/ckanext/comments/templates/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-11-08 21:05:03.000000 ckanext-comments-0.2.0/ckanext/comments/templates/.gitignore
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 15:47:51.439851 ckanext-comments-0.2.0/ckanext/comments/templates/comments/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 15:47:51.489851 ckanext-comments-0.2.0/ckanext/comments/templates/comments/snippets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2989 2023-03-01 11:49:29.000000 ckanext-comments-0.2.0/ckanext/comments/templates/comments/snippets/comment.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)      403 2023-03-01 07:36:07.000000 ckanext-comments-0.2.0/ckanext/comments/templates/comments/snippets/comment_form.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)      738 2022-11-08 21:05:03.000000 ckanext-comments-0.2.0/ckanext/comments/templates/comments/snippets/comments_list.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1088 2023-03-01 11:54:44.000000 ckanext-comments-0.2.0/ckanext/comments/templates/comments/snippets/confirmation.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)      863 2022-11-08 21:05:03.000000 ckanext-comments-0.2.0/ckanext/comments/templates/comments/snippets/thread.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 15:47:51.489851 ckanext-comments-0.2.0/ckanext/comments/templates/package/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      270 2023-03-01 04:08:30.000000 ckanext-comments-0.2.0/ckanext/comments/templates/package/read.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 15:47:51.489851 ckanext-comments-0.2.0/ckanext/comments/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-11-08 21:05:03.000000 ckanext-comments-0.2.0/ckanext/comments/tests/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      453 2023-03-28 11:57:40.000000 ckanext-comments-0.2.0/ckanext/comments/tests/conftest.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1358 2023-03-28 11:57:37.000000 ckanext-comments-0.2.0/ckanext/comments/tests/factories.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 15:47:51.489851 ckanext-comments-0.2.0/ckanext/comments/tests/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-11-08 21:05:03.000000 ckanext-comments-0.2.0/ckanext/comments/tests/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     9191 2023-03-28 11:57:40.000000 ckanext-comments-0.2.0/ckanext/comments/tests/logic/test_action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3608 2023-03-28 11:57:40.000000 ckanext-comments-0.2.0/ckanext/comments/tests/logic/test_auth.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-11-08 21:05:03.000000 ckanext-comments-0.2.0/ckanext/comments/tests/logic/test_validators.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 15:47:51.489851 ckanext-comments-0.2.0/ckanext/comments/tests/model/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-11-08 21:05:03.000000 ckanext-comments-0.2.0/ckanext/comments/tests/model/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1741 2023-03-28 11:57:40.000000 ckanext-comments-0.2.0/ckanext/comments/tests/model/test_comment.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4978 2023-03-28 11:57:40.000000 ckanext-comments-0.2.0/ckanext/comments/tests/model/test_dictize.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1389 2023-03-28 11:57:40.000000 ckanext-comments-0.2.0/ckanext/comments/tests/model/test_thread.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)       87 2022-11-08 21:05:03.000000 ckanext-comments-0.2.0/ckanext/comments/tests/test_helpers.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1259 2022-11-08 21:05:03.000000 ckanext-comments-0.2.0/ckanext/comments/tests/test_plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      347 2023-03-28 11:57:37.000000 ckanext-comments-0.2.0/ckanext/comments/utils.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 15:47:51.489851 ckanext-comments-0.2.0/ckanext_comments.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4762 2023-04-03 15:47:51.000000 ckanext-comments-0.2.0/ckanext_comments.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2578 2023-04-03 15:47:51.000000 ckanext-comments-0.2.0/ckanext_comments.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-04-03 15:47:51.000000 ckanext-comments-0.2.0/ckanext_comments.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      122 2023-04-03 15:47:51.000000 ckanext-comments-0.2.0/ckanext_comments.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-04-03 15:47:51.000000 ckanext-comments-0.2.0/ckanext_comments.egg-info/namespace_packages.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       26 2023-04-03 15:47:51.000000 ckanext-comments-0.2.0/ckanext_comments.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-04-03 15:47:51.000000 ckanext-comments-0.2.0/ckanext_comments.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       12 2022-11-08 21:05:03.000000 ckanext-comments-0.2.0/dev-requirements.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      762 2022-11-08 21:05:03.000000 ckanext-comments-0.2.0/gulpfile.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)   297177 2023-04-03 15:47:33.000000 ckanext-comments-0.2.0/package-lock.json
--rw-r--r--   0 sergey    (1000) sergey    (1000)      838 2023-04-03 15:47:33.000000 ckanext-comments-0.2.0/package.json
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2822 2023-03-28 11:57:07.000000 ckanext-comments-0.2.0/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-11-08 21:05:03.000000 ckanext-comments-0.2.0/requirements.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1638 2023-04-03 15:47:51.489851 ckanext-comments-0.2.0/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)      528 2022-11-08 21:05:03.000000 ckanext-comments-0.2.0/setup.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      787 2022-11-08 21:05:03.000000 ckanext-comments-0.2.0/test.ini
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-11 14:42:11.814863 ckanext-comments-0.3.0/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)    34500 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/LICENSE
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      208 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/MANIFEST.in
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     5048 2023-04-11 14:42:11.814863 ckanext-comments-0.3.0/PKG-INFO
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     4401 2023-04-07 13:14:24.000000 ckanext-comments-0.3.0/README.md
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-11 14:42:11.806863 ckanext-comments-0.3.0/ckanext/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      221 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/__init__.py
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-11 14:42:11.810863 ckanext-comments-0.3.0/ckanext/comments/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)        0 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/__init__.py
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-11 14:42:11.810863 ckanext-comments-0.3.0/ckanext/comments/assets/
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-11 14:42:11.810863 ckanext-comments-0.3.0/ckanext/comments/assets/css/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     1675 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/assets/css/comments-thread.css
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-11 14:42:11.810863 ckanext-comments-0.3.0/ckanext/comments/assets/js/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     6450 2023-04-11 13:08:05.000000 ckanext-comments-0.3.0/ckanext/comments/assets/js/comments-thread.js
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-11 14:42:11.810863 ckanext-comments-0.3.0/ckanext/comments/assets/less/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     2129 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/assets/less/comments-thread.less
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      326 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/assets/webassets.yml
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     2294 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/config.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      110 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/config_declaration.yaml
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      158 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/exceptions.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     1540 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/helpers.py
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-11 14:42:11.810863 ckanext-comments-0.3.0/ckanext/comments/logic/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)        0 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/logic/__init__.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     8285 2023-04-10 14:01:46.000000 ckanext-comments-0.3.0/ckanext/comments/logic/action.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     2595 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/logic/auth.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     1890 2023-04-07 10:59:00.000000 ckanext-comments-0.3.0/ckanext/comments/logic/schema.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      460 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/logic/validators.py
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-11 14:42:11.806863 ckanext-comments-0.3.0/ckanext/comments/migration/
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-11 14:42:11.810863 ckanext-comments-0.3.0/ckanext/comments/migration/comments/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     1800 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/migration/comments/alembic.ini
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     2228 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/migration/comments/env.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      494 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/migration/comments/script.py.mako
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-11 14:42:11.810863 ckanext-comments-0.3.0/ckanext/comments/migration/comments/versions/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     1803 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/migration/comments/versions/275515c51af1_init_tables.py
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-11 14:42:11.810863 ckanext-comments-0.3.0/ckanext/comments/model/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)       89 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/model/__init__.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)       83 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/model/base.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     2885 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/model/comment.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     3272 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/model/dictize.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     2331 2023-04-07 13:10:03.000000 ckanext-comments-0.3.0/ckanext/comments/model/thread.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     1248 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/plugin.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      773 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/signals.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      275 2023-04-07 13:11:20.000000 ckanext-comments-0.3.0/ckanext/comments/subject.py
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-11 14:42:11.806863 ckanext-comments-0.3.0/ckanext/comments/templates/
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-11 14:42:11.806863 ckanext-comments-0.3.0/ckanext/comments/templates/comments/
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-11 14:42:11.814863 ckanext-comments-0.3.0/ckanext/comments/templates/comments/snippets/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     2989 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/templates/comments/snippets/comment.html
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      403 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/templates/comments/snippets/comment_form.html
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      738 2023-04-10 08:48:43.000000 ckanext-comments-0.3.0/ckanext/comments/templates/comments/snippets/comments_list.html
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     1088 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/templates/comments/snippets/confirmation.html
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      863 2023-04-11 14:39:59.000000 ckanext-comments-0.3.0/ckanext/comments/templates/comments/snippets/thread.html
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-11 14:42:11.814863 ckanext-comments-0.3.0/ckanext/comments/templates/package/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      270 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/templates/package/read.html
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-11 14:42:11.814863 ckanext-comments-0.3.0/ckanext/comments/tests/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)        0 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/tests/__init__.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      453 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/tests/conftest.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     1358 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/tests/factories.py
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-11 14:42:11.814863 ckanext-comments-0.3.0/ckanext/comments/tests/logic/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)        0 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/tests/logic/__init__.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     9191 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/tests/logic/test_action.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     3608 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/tests/logic/test_auth.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)        0 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/tests/logic/test_validators.py
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-11 14:42:11.814863 ckanext-comments-0.3.0/ckanext/comments/tests/model/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)        0 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/tests/model/__init__.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     1741 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/tests/model/test_comment.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     4978 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/tests/model/test_dictize.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     1389 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/tests/model/test_thread.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)       87 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/tests/test_helpers.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     1259 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/tests/test_plugin.py
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      347 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/ckanext/comments/utils.py
+drwxrwxr-x   0 cherry    (1000) cherry    (1000)        0 2023-04-11 14:42:11.814863 ckanext-comments-0.3.0/ckanext_comments.egg-info/
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     5048 2023-04-11 14:42:11.000000 ckanext-comments-0.3.0/ckanext_comments.egg-info/PKG-INFO
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     2272 2023-04-11 14:42:11.000000 ckanext-comments-0.3.0/ckanext_comments.egg-info/SOURCES.txt
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)        1 2023-04-11 14:42:11.000000 ckanext-comments-0.3.0/ckanext_comments.egg-info/dependency_links.txt
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      122 2023-04-11 14:42:11.000000 ckanext-comments-0.3.0/ckanext_comments.egg-info/entry_points.txt
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)        8 2023-04-11 14:42:11.000000 ckanext-comments-0.3.0/ckanext_comments.egg-info/namespace_packages.txt
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)       26 2023-04-11 14:42:11.000000 ckanext-comments-0.3.0/ckanext_comments.egg-info/requires.txt
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)        8 2023-04-11 14:42:11.000000 ckanext-comments-0.3.0/ckanext_comments.egg-info/top_level.txt
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     2822 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/pyproject.toml
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)        0 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/requirements.txt
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)     1638 2023-04-11 14:42:11.818863 ckanext-comments-0.3.0/setup.cfg
+-rw-rw-r--   0 cherry    (1000) cherry    (1000)      528 2023-04-06 18:18:55.000000 ckanext-comments-0.3.0/setup.py
```

### Comparing `ckanext-comments-0.2.0/LICENSE` & `ckanext-comments-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-comments-0.2.0/PKG-INFO` & `ckanext-comments-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: ckanext-comments
-Version: 0.2.0
-Home-page: https://github.com/DataShades/ckanext-comments
-Author: Sergey Motornyuk
-Author-email: sergey.motornyuk@linkdigital.com.au
-License: AGPL
-Keywords: CKAN
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Tests](https://github.com/DataShades/ckanext-comments/actions/workflows/test.yml/badge.svg)](https://github.com/DataShades/ckanext-comments/actions/workflows/test.yml)
 
 # ckanext-comments
 
 Add comment-trees to CKAN pages.
 
 This plugins provides comment threads linked to any of the main CKAN entities:
@@ -100,16 +82,23 @@
 # Number of reply levels that are shown on mobile layout
 # (optional, default: 3).
 ckanext.comments.mobile_depth_threshold = 3
 
 # Include default thread implementation on the dataset page
 # (optional, default: false).
 ckanext.comments.enable_default_dataset_comments = true
+
+# Register custom getter for a subject by providing a path to a function
+# ckanext.comments.subject.{self.subject_type}_getter = path
+# The function must accept an ID and return a model object
+ckanext.comments.subject.question_getter = ckanext.msf_ask_question.model.question_getter
 ```
 
+
+
 ## API
 
 ### `comments_thread_create`
 Create a thread for the subject.
 
 Args:
 * subject_id(str): unique ID of the commented entity
```

### Comparing `ckanext-comments-0.2.0/README.md` & `ckanext-comments-0.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: ckanext-comments
+Version: 0.3.0
+Home-page: https://github.com/DataShades/ckanext-comments
+Author: Sergey Motornyuk
+Author-email: sergey.motornyuk@linkdigital.com.au
+License: AGPL
+Keywords: CKAN
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![Tests](https://github.com/DataShades/ckanext-comments/actions/workflows/test.yml/badge.svg)](https://github.com/DataShades/ckanext-comments/actions/workflows/test.yml)
 
 # ckanext-comments
 
 Add comment-trees to CKAN pages.
 
 This plugins provides comment threads linked to any of the main CKAN entities:
@@ -82,16 +100,23 @@
 # Number of reply levels that are shown on mobile layout
 # (optional, default: 3).
 ckanext.comments.mobile_depth_threshold = 3
 
 # Include default thread implementation on the dataset page
 # (optional, default: false).
 ckanext.comments.enable_default_dataset_comments = true
+
+# Register custom getter for a subject by providing a path to a function
+# ckanext.comments.subject.{self.subject_type}_getter = path
+# The function must accept an ID and return a model object
+ckanext.comments.subject.question_getter = ckanext.msf_ask_question.model.question_getter
 ```
 
+
+
 ## API
 
 ### `comments_thread_create`
 Create a thread for the subject.
 
 Args:
 * subject_id(str): unique ID of the commented entity
```

### Comparing `ckanext-comments-0.2.0/ckanext/comments/assets/css/comments-thread.css` & `ckanext-comments-0.3.0/ckanext/comments/assets/css/comments-thread.css`

 * *Files identical despite different names*

### Comparing `ckanext-comments-0.2.0/ckanext/comments/assets/js/comments-thread.js` & `ckanext-comments-0.3.0/ckanext/comments/assets/js/comments-thread.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,15 @@
 ckan.module("comments-thread", function($) {
     "use strict";
 
     return {
         options: {
             subjectId: null,
             subjectType: null,
+            ajaxReload: null,
         },
         initialize: function() {
             $.proxyAll(this, /_on/);
             this.$(".comment-actions .remove-comment").on(
                 "click",
                 this._onRemoveComment
             );
@@ -19,27 +20,27 @@
             this.$(".comment-actions .reply-to-comment").on(
                 "click",
                 this._onReplyToComment
             );
             this.$(".comment-actions .edit-comment").on("click", this._onEditComment);
             this.$(".comment-actions .save-comment").on("click", this._onSaveComment);
             this.$(".comment-footer").on("click", this._onFooterClick);
-            this.$(".comment-form").on("submit", this._onSubmit);
+            this.$(".comment-form").off("submit").on("submit", this._onSubmit);
         },
         teardown: function() {
             this.$(".comment-action.remove-comment").off(
                 "click",
                 this._onRemoveComment
             );
             this.$(".comment-actions .approve-comment").off(
                 "click",
                 this._onApproveComment
             );
 
-            this.$("comment-form").off("sumbit", this._onSubmit);
+            this.$(".comment-form").off("submit", this._onSubmit);
         },
         _onFooterClick: function(e) {
             if (e.target.classList.contains("cancel-reply")) {
                 this._disableActiveReply();
             } else if (e.target.classList.contains("save-reply")) {
                 var content = e.currentTarget.querySelector(
                     ".reply-textarea-wrapper textarea"
@@ -48,38 +49,50 @@
                     content: content,
                     reply_to_id: e.target.dataset.id,
                 });
             }
         },
         _onRemoveComment: function(e) {
             var id = e.currentTarget.dataset.id;
+            var ajaxReload = this.options.ajaxReload;
 
             this.sandbox.client.call(
                 "POST",
                 "comments_comment_delete", {
                     id: id,
                 },
-                function() {
-                    window.location.reload();
+                function(e) {
+                    if (ajaxReload) {
+                        $(".modal").modal("hide");
+
+                        $(document).trigger("comments:changed");
+                    } else {
+                        window.location.reload();
+                    }
                 }
             );
         },
         _onApproveComment: function(e) {
             var id = e.currentTarget.dataset.id;
+            var ajaxReload = this.options.ajaxReload;
+
             this.sandbox.client.call(
                 "POST",
                 "comments_comment_approve", {
                     id: id,
                 },
                 function() {
-                    window.location.reload();
+                    if (ajaxReload) {
+                        $(document).trigger("comments:changed");
+                    } else {
+                        window.location.reload();
+                    }
                 }
             );
         },
-
         _disableActiveReply: function() {
             $(".comment .reply-textarea-wrapper").remove();
         },
         _onReplyToComment: function(e) {
             this._disableActiveReply();
             this._disableActiveEdit();
             var id = e.currentTarget.dataset.id;
@@ -139,22 +152,28 @@
         _onSaveComment: function(e) {
             var self = this;
             var id = e.currentTarget.dataset.id;
             var target = $(e.currentTarget);
             var notify = this.sandbox.notify;
             var _ = this.sandbox.translate;
             var content = target.closest(".comment").find(".comment-body textarea");
+            var ajaxReload = this.options.ajaxReload;
+
             this.sandbox.client.call(
                 "POST",
                 "comments_comment_update", {
                     id: id,
                     content: content.val(),
                 },
                 function() {
-                    window.location.reload();
+                    if (ajaxReload) {
+                        $(document).trigger("comments:changed");
+                    } else {
+                        window.location.reload();
+                    }
                 },
                 function(err) {
                     console.log(err);
                     var oldEl = notify.el;
                     notify.el = target.closest(".comment");
                     notify(
                         self._("An Error Occurred").fetch(),
@@ -171,20 +190,30 @@
             var data = new FormData(e.target);
             this._saveComment({
                 content: data.get("content"),
                 create_thread: true
             });
         },
         _saveComment: function(data) {
+            if (!data.content) {
+                return;
+            }
+
             data.subject_id = this.options.subjectId;
             data.subject_type = this.options.subjectType;
+            var ajaxReload = this.options.ajaxReload;
+
             this.sandbox.client.call(
                 "POST",
                 "comments_comment_create",
                 data,
                 function() {
-                    window.location.reload();
+                    if (ajaxReload) {
+                        $(document).trigger("comments:changed");
+                    } else {
+                        window.location.reload();
+                    }
                 }
             );
         },
     };
 });
```

### Comparing `ckanext-comments-0.2.0/ckanext/comments/assets/less/comments-thread.less` & `ckanext-comments-0.3.0/ckanext/comments/assets/less/comments-thread.less`

 * *Files identical despite different names*

### Comparing `ckanext-comments-0.2.0/ckanext/comments/config.py` & `ckanext-comments-0.3.0/ckanext/comments/config.py`

 * *Files identical despite different names*

### Comparing `ckanext-comments-0.2.0/ckanext/comments/helpers.py` & `ckanext-comments-0.3.0/ckanext/comments/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-comments-0.2.0/ckanext/comments/logic/action.py` & `ckanext-comments-0.3.0/ckanext/comments/logic/action.py`

 * *Files identical despite different names*

### Comparing `ckanext-comments-0.2.0/ckanext/comments/logic/auth.py` & `ckanext-comments-0.3.0/ckanext/comments/logic/auth.py`

 * *Files identical despite different names*

### Comparing `ckanext-comments-0.2.0/ckanext/comments/migration/comments/alembic.ini` & `ckanext-comments-0.3.0/ckanext/comments/migration/comments/alembic.ini`

 * *Files identical despite different names*

### Comparing `ckanext-comments-0.2.0/ckanext/comments/migration/comments/env.py` & `ckanext-comments-0.3.0/ckanext/comments/migration/comments/env.py`

 * *Files identical despite different names*

### Comparing `ckanext-comments-0.2.0/ckanext/comments/migration/comments/versions/275515c51af1_init_tables.py` & `ckanext-comments-0.3.0/ckanext/comments/migration/comments/versions/275515c51af1_init_tables.py`

 * *Files identical despite different names*

### Comparing `ckanext-comments-0.2.0/ckanext/comments/model/comment.py` & `ckanext-comments-0.3.0/ckanext/comments/model/comment.py`

 * *Files identical despite different names*

### Comparing `ckanext-comments-0.2.0/ckanext/comments/model/dictize.py` & `ckanext-comments-0.3.0/ckanext/comments/model/dictize.py`

 * *Files identical despite different names*

### Comparing `ckanext-comments-0.2.0/ckanext/comments/model/thread.py` & `ckanext-comments-0.3.0/ckanext/comments/model/thread.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
 import logging
 from datetime import datetime
 from typing import TYPE_CHECKING, Callable, Optional, Union, cast
+from werkzeug.utils import import_string
 
 from sqlalchemy import Column, DateTime, Text
 from sqlalchemy.orm import Query
 
 import ckan.model as model
+import ckan.plugins.toolkit as tk
 from ckan.model.types import make_uuid
 
 from ckanext.comments.exceptions import UnsupportedSubjectType
 
 from .base import Base
 
 if TYPE_CHECKING:
@@ -43,20 +45,26 @@
 
     def comments(self) -> Query:
         from .comment import Comment
 
         return Comment.by_thread(self.id)
 
     def get_subject(self) -> Optional[Subject]:
-        try:
+        getter = import_string(
+            tk.config.get(f"ckanext.comments.subject.{self.subject_type}_getter"),
+            True,
+        )
+
+        if not getter and self.subject_type in self._subject_getters:
             getter = self._subject_getters[self.subject_type]
-        except KeyError:
-            log.error("Unknown subject type: %s", self.subject_type)
+
+        if not getter:
             raise UnsupportedSubjectType(self.subject_type)
-        return getter(self.subject_id)
+
+        return getter(self.subject_id)  # type: ignore
 
     @classmethod
     def for_subject(
         cls, type_: str, id_: str, init_missing: bool = False
     ) -> Optional[Thread]:
         thread = cast(
             Optional[Thread],
```

### Comparing `ckanext-comments-0.2.0/ckanext/comments/plugin.py` & `ckanext-comments-0.3.0/ckanext/comments/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-comments-0.2.0/ckanext/comments/signals.py` & `ckanext-comments-0.3.0/ckanext/comments/signals.py`

 * *Files identical despite different names*

### Comparing `ckanext-comments-0.2.0/ckanext/comments/templates/comments/snippets/comment.html` & `ckanext-comments-0.3.0/ckanext/comments/templates/comments/snippets/comment.html`

 * *Files identical despite different names*

### Comparing `ckanext-comments-0.2.0/ckanext/comments/templates/comments/snippets/comments_list.html` & `ckanext-comments-0.3.0/ckanext/comments/templates/comments/snippets/comments_list.html`

 * *Files identical despite different names*

### Comparing `ckanext-comments-0.2.0/ckanext/comments/templates/comments/snippets/confirmation.html` & `ckanext-comments-0.3.0/ckanext/comments/templates/comments/snippets/confirmation.html`

 * *Files identical despite different names*

### Comparing `ckanext-comments-0.2.0/ckanext/comments/templates/comments/snippets/thread.html` & `ckanext-comments-0.3.0/ckanext/comments/templates/comments/snippets/thread.html`

 * *Files identical despite different names*

### Comparing `ckanext-comments-0.2.0/ckanext/comments/tests/factories.py` & `ckanext-comments-0.3.0/ckanext/comments/tests/factories.py`

 * *Files identical despite different names*

### Comparing `ckanext-comments-0.2.0/ckanext/comments/tests/logic/test_action.py` & `ckanext-comments-0.3.0/ckanext/comments/tests/logic/test_action.py`

 * *Files identical despite different names*

### Comparing `ckanext-comments-0.2.0/ckanext/comments/tests/logic/test_auth.py` & `ckanext-comments-0.3.0/ckanext/comments/tests/logic/test_auth.py`

 * *Files identical despite different names*

### Comparing `ckanext-comments-0.2.0/ckanext/comments/tests/model/test_comment.py` & `ckanext-comments-0.3.0/ckanext/comments/tests/model/test_comment.py`

 * *Files identical despite different names*

### Comparing `ckanext-comments-0.2.0/ckanext/comments/tests/model/test_dictize.py` & `ckanext-comments-0.3.0/ckanext/comments/tests/model/test_dictize.py`

 * *Files identical despite different names*

### Comparing `ckanext-comments-0.2.0/ckanext/comments/tests/model/test_thread.py` & `ckanext-comments-0.3.0/ckanext/comments/tests/model/test_thread.py`

 * *Files identical despite different names*

### Comparing `ckanext-comments-0.2.0/ckanext/comments/tests/test_plugin.py` & `ckanext-comments-0.3.0/ckanext/comments/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-comments-0.2.0/ckanext_comments.egg-info/PKG-INFO` & `ckanext-comments-0.3.0/ckanext_comments.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-comments
-Version: 0.2.0
+Version: 0.3.0
 Home-page: https://github.com/DataShades/ckanext-comments
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
@@ -100,16 +100,23 @@
 # Number of reply levels that are shown on mobile layout
 # (optional, default: 3).
 ckanext.comments.mobile_depth_threshold = 3
 
 # Include default thread implementation on the dataset page
 # (optional, default: false).
 ckanext.comments.enable_default_dataset_comments = true
+
+# Register custom getter for a subject by providing a path to a function
+# ckanext.comments.subject.{self.subject_type}_getter = path
+# The function must accept an ID and return a model object
+ckanext.comments.subject.question_getter = ckanext.msf_ask_question.model.question_getter
 ```
 
+
+
 ## API
 
 ### `comments_thread_create`
 Create a thread for the subject.
 
 Args:
 * subject_id(str): unique ID of the commented entity
```

### Comparing `ckanext-comments-0.2.0/ckanext_comments.egg-info/SOURCES.txt` & `ckanext-comments-0.3.0/ckanext_comments.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,56 +1,42 @@
-.coveragerc
-.editorconfig
-.gitignore
-CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
-dev-requirements.txt
-gulpfile.js
-package-lock.json
-package.json
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
-test.ini
-.github/workflows/test.yml
 ckanext/__init__.py
 ckanext/comments/__init__.py
 ckanext/comments/config.py
 ckanext/comments/config_declaration.yaml
 ckanext/comments/exceptions.py
 ckanext/comments/helpers.py
 ckanext/comments/plugin.py
 ckanext/comments/signals.py
+ckanext/comments/subject.py
 ckanext/comments/utils.py
-ckanext/comments/assets/.gitignore
 ckanext/comments/assets/webassets.yml
 ckanext/comments/assets/css/comments-thread.css
 ckanext/comments/assets/js/comments-thread.js
 ckanext/comments/assets/less/comments-thread.less
-ckanext/comments/i18n/.gitignore
 ckanext/comments/logic/__init__.py
 ckanext/comments/logic/action.py
 ckanext/comments/logic/auth.py
 ckanext/comments/logic/schema.py
 ckanext/comments/logic/validators.py
-ckanext/comments/migration/comments/README
 ckanext/comments/migration/comments/alembic.ini
 ckanext/comments/migration/comments/env.py
 ckanext/comments/migration/comments/script.py.mako
 ckanext/comments/migration/comments/versions/275515c51af1_init_tables.py
 ckanext/comments/model/__init__.py
 ckanext/comments/model/base.py
 ckanext/comments/model/comment.py
 ckanext/comments/model/dictize.py
 ckanext/comments/model/thread.py
-ckanext/comments/public/.gitignore
-ckanext/comments/templates/.gitignore
 ckanext/comments/templates/comments/snippets/comment.html
 ckanext/comments/templates/comments/snippets/comment_form.html
 ckanext/comments/templates/comments/snippets/comments_list.html
 ckanext/comments/templates/comments/snippets/confirmation.html
 ckanext/comments/templates/comments/snippets/thread.html
 ckanext/comments/templates/package/read.html
 ckanext/comments/tests/__init__.py
```

### Comparing `ckanext-comments-0.2.0/pyproject.toml` & `ckanext-comments-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ckanext-comments-0.2.0/setup.cfg` & `ckanext-comments-0.3.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ckanext-comments
-version = 0.2.0
+version = 0.3.0
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/DataShades/ckanext-comments
 author = Sergey Motornyuk
 author_email = sergey.motornyuk@linkdigital.com.au
 license = AGPL
```

### Comparing `ckanext-comments-0.2.0/setup.py` & `ckanext-comments-0.3.0/setup.py`

 * *Files identical despite different names*

