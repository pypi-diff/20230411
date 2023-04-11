# Comparing `tmp/Products.MeetingPROVHainaut-4.2b5.tar.gz` & `tmp/Products.MeetingPROVHainaut-4.2b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Products.MeetingPROVHainaut-4.2b5.tar", last modified: Fri Jan  7 08:40:12 2022, max compression
+gzip compressed data, was "dist/Products.MeetingPROVHainaut-4.2b6.tar", last modified: Thu Apr 28 08:29:57 2022, max compression
```

## Comparing `Products.MeetingPROVHainaut-4.2b5.tar` & `Products.MeetingPROVHainaut-4.2b6.tar`

### file list

```diff
@@ -1,167 +1,167 @@
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products.MeetingPROVHainaut.egg-info/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products.MeetingPROVHainaut.egg-info/dependency_links.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        9 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products.MeetingPROVHainaut.egg-info/namespace_packages.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        9 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products.MeetingPROVHainaut.egg-info/top_level.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5930 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products.MeetingPROVHainaut.egg-info/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8471 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products.MeetingPROVHainaut.egg-info/SOURCES.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products.MeetingPROVHainaut.egg-info/not-zip-safe
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       61 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products.MeetingPROVHainaut.egg-info/requires.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      489 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/events.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    14061 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/setuphandlers.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/skins/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/skins/meetingprovhainaut_styles/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2911 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/skins/meetingprovhainaut_styles/meetingprovincehainaut.css.dtml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1560 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/skins/meetingprovhainaut_styles/imioapps_properties.props
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/skins/meetingprovhainaut_templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/skins/meetingprovhainaut_templates/.gitkeep
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/skins/meetingprovhainaut_images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      329 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/skins/meetingprovhainaut_images/new_meetingadvicefinancescec.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2725 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/skins/meetingprovhainaut_images/logo.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    47364 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/skins/meetingprovhainaut_images/spinner.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      329 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/skins/meetingprovhainaut_images/new_meetingadvicefinancesnocec.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1150 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/skins/meetingprovhainaut_images/favicon.ico
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1593 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10862 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/adapters.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/locales/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2268 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/locales/PloneMeeting.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/locales/en/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/locales/en/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      545 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/locales/en/LC_MESSAGES/plone.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2406 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/locales/en/LC_MESSAGES/PloneMeeting.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      406 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/locales/plone.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/locales/fr/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      719 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/locales/fr/LC_MESSAGES/plone.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3336 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/locales/fr/LC_MESSAGES/PloneMeeting.po
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      267 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/locales/sync_pos.sh
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/testing/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/testing/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/testing/MeetingPROVHainaut_testing_marker.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/testing/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      880 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/testing/images/overheadAnalysis.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1147 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/testing/images/positive.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/testing/images/attach.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      731 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/testing/images/cahier.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/testing/images/budget.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      742 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/testing/images/financialAnalysis.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      355 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/testing/images/remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      411 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/testing/images/negative.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      216 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/testing/images/decisionAnnex.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      492 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/testing/images/budgetAnalysis.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      216 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/testing/images/itemAnnex.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      332 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/testing/images/legalAnalysis.png
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/testing/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/testing/templates/.gitkeep
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/testing/__init__.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/testing/toolset.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      748 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/testing/import_data.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/default/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      183 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/default/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/default/MeetingPROVHainaut_marker.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      355 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/default/propertiestool.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      960 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/default/skins.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/default/types/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3353 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/default/types/meetingadvicefinancescec.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3344 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/default/types/meetingadvicefinances.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2701 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/default/types/meetingadvicefinancesnocec.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      766 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/default/cssregistry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      304 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/default/types.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      419 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/default/repositorytool.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      411 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/default/import_steps.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/default/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       96 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/default/workflows.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      153 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    44108 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/organizations.csv
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/positive.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/attach.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      731 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/cahier.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/budget.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/legalAdvice.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/negative.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      574 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/deliberation_signed.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      328 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/deliberation_to_sign.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/nil.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        9 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/MeetingPROVHainaut_zprovhainaut_marker.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7816 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/note.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    17869 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/document-travail-conseil.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    17900 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/convocation.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18306 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/document-travail-college.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    79168 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/presences.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    30661 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/deliberation.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11780 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/bordereaux.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    21899 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/arrete.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    80966 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/pv.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    30497 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/rapport.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    78731 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/role.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    14447 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/resolution.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      168 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/toolset.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    17437 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/import_data.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1834 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/testing.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      579 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/interfaces.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1163 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/utils.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/model/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       23 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/model/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       24 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/model/pm_updates.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1866 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/config.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2386 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/events.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      669 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/testing.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      730 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/vocabularies.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/Extensions/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3826 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/Extensions/utils.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/Extensions/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/faceted_conf/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      218 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/faceted_conf/meetingprovhainaut_dashboard_items_widgets.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1271 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testFaceted.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      449 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testVotes.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1380 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testAdvices.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1327 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testMeetingCategory.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1350 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testChangeItemOrderView.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1231 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testUtils.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1160 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testColumns.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1275 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testSetup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1332 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testToolPloneMeeting.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      472 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testWorkflows.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3378 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/helpers.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      567 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/MeetingPROVHainautTestCase.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      761 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testMeetingItem.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2304 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testWFAdaptations.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1287 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testValidators.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1287 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testPortlets.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1312 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testAnnexes.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7564 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testCustomWorkflows.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1292 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      544 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testMeeting.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1261 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testSearches.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1233 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testViews.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      489 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testMeetingConfig.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      868 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/overrides.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      414 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2053 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/migrations/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1307 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/migrations/migrate_to_4202.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      956 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/migrations/migrate_to_4200.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2080 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/migrations/migrate_to_4203.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1844 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/migrations/migrate_to_4201.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/migrations/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       56 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/src/Products/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/docs/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      737 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/docs/LICENSE.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/docs/LICENSE.GPL
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      865 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5930 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      546 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/MANIFEST.in
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4620 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/CHANGES.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      129 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/README.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2022-01-07 08:40:12.000000 Products.MeetingPROVHainaut-4.2b5/setup.cfg
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products.MeetingPROVHainaut.egg-info/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products.MeetingPROVHainaut.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        9 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products.MeetingPROVHainaut.egg-info/namespace_packages.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        9 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products.MeetingPROVHainaut.egg-info/top_level.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6352 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products.MeetingPROVHainaut.egg-info/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8471 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products.MeetingPROVHainaut.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products.MeetingPROVHainaut.egg-info/not-zip-safe
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       61 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products.MeetingPROVHainaut.egg-info/requires.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      489 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/events.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    14414 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/setuphandlers.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/skins/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/skins/meetingprovhainaut_styles/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2911 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/skins/meetingprovhainaut_styles/meetingprovincehainaut.css.dtml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1560 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/skins/meetingprovhainaut_styles/imioapps_properties.props
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/skins/meetingprovhainaut_templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/skins/meetingprovhainaut_templates/.gitkeep
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/skins/meetingprovhainaut_images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      329 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/skins/meetingprovhainaut_images/new_meetingadvicefinancescec.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2725 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/skins/meetingprovhainaut_images/logo.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    47364 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/skins/meetingprovhainaut_images/spinner.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      329 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/skins/meetingprovhainaut_images/new_meetingadvicefinancesnocec.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1150 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/skins/meetingprovhainaut_images/favicon.ico
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1593 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10861 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/adapters.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/locales/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2268 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/locales/PloneMeeting.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/locales/en/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      545 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/locales/en/LC_MESSAGES/plone.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2406 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/locales/en/LC_MESSAGES/PloneMeeting.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      406 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/locales/plone.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/locales/fr/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      719 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/locales/fr/LC_MESSAGES/plone.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3336 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/locales/fr/LC_MESSAGES/PloneMeeting.po
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      267 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/locales/sync_pos.sh
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/testing/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/testing/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/testing/MeetingPROVHainaut_testing_marker.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/testing/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      880 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/testing/images/overheadAnalysis.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1147 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/testing/images/positive.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/testing/images/attach.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      731 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/testing/images/cahier.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/testing/images/budget.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      742 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/testing/images/financialAnalysis.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      355 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/testing/images/remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      411 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/testing/images/negative.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      216 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/testing/images/decisionAnnex.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      492 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/testing/images/budgetAnalysis.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      216 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/testing/images/itemAnnex.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      332 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/testing/images/legalAnalysis.png
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/testing/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/testing/templates/.gitkeep
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/testing/__init__.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/testing/toolset.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      748 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/testing/import_data.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/default/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      183 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/default/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/default/MeetingPROVHainaut_marker.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      355 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/default/propertiestool.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      960 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/default/skins.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/default/types/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3353 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/default/types/meetingadvicefinancescec.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3344 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/default/types/meetingadvicefinances.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2701 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/default/types/meetingadvicefinancesnocec.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      766 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/default/cssregistry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      304 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/default/types.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      419 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/default/repositorytool.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      411 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/default/import_steps.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/default/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       96 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/default/workflows.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      153 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    44108 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/organizations.csv
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/positive.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/attach.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      731 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/cahier.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/budget.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/legalAdvice.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/negative.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      574 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/deliberation_signed.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      328 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/deliberation_to_sign.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/nil.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        9 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/MeetingPROVHainaut_zprovhainaut_marker.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7816 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/note.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    17869 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/document-travail-conseil.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    17900 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/convocation.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18306 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/document-travail-college.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    79168 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/presences.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    30661 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/deliberation.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11780 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/bordereaux.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    21899 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/arrete.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    80966 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/pv.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    30497 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/rapport.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    78731 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/role.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    14447 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/resolution.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      168 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/toolset.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18824 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/import_data.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1834 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/testing.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      579 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/interfaces.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1163 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/utils.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/model/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       23 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/model/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       24 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/model/pm_updates.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3317 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/config.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1802 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/events.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      669 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/testing.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      730 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/vocabularies.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/Extensions/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3826 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/Extensions/utils.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/Extensions/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/faceted_conf/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      218 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/faceted_conf/meetingprovhainaut_dashboard_items_widgets.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1271 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testFaceted.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      449 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testVotes.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1380 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testAdvices.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1327 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testMeetingCategory.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1350 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testChangeItemOrderView.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1231 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testUtils.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1160 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testColumns.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1275 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testSetup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1332 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testToolPloneMeeting.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      472 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testWorkflows.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3378 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/helpers.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      567 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/MeetingPROVHainautTestCase.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      761 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testMeetingItem.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2452 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testWFAdaptations.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1287 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testValidators.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1287 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testPortlets.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1312 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testAnnexes.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11484 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testCustomWorkflows.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1292 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      544 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testMeeting.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1261 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testSearches.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1233 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testViews.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      489 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testMeetingConfig.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      868 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/overrides.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      414 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2053 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/migrations/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1307 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/migrations/migrate_to_4202.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      956 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/migrations/migrate_to_4200.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2080 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/migrations/migrate_to_4203.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1844 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/migrations/migrate_to_4201.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/migrations/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       56 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/src/Products/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/docs/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      737 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/docs/LICENSE.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/docs/LICENSE.GPL
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      865 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6352 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      546 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/MANIFEST.in
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4962 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/CHANGES.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      129 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/README.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2022-04-28 08:29:57.000000 Products.MeetingPROVHainaut-4.2b6/setup.cfg
```

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products.MeetingPROVHainaut.egg-info/PKG-INFO` & `Products.MeetingPROVHainaut-4.2b6/src/Products.MeetingPROVHainaut.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 Metadata-Version: 2.1
 Name: Products.MeetingPROVHainaut
-Version: 4.2b5
+Version: 4.2b6
 Summary: PloneMeeting profile for Province de Hainaut
 Home-page: http://www.imio.be/produits/gestion-des-deliberations
 Author: 
 Author-email: 
 License: GPL
 Description: Products.PloneMeeting profile for Province de Hainaut (Belgium)
         ===============================================================
         
         
         
         Products.MeetingPROVHainaut Changelog
         =====================================
         
+        4.2b6 (2022-04-28)
+        ------------------
+        
+        - Adapted `events.onAdviceAfterTransition`, do no more call
+          `MeetingItem.update_local_roles` as it is done in PloneMeeting in
+          `events.onAdviceTransition` now, just after call to `AdviceAfterTransitionEvent`.
+          [gbastien]
+        - Fixed `zprovhainaut import_data`, was failing with demo data.
+          [gbastien]
+        
         4.2b5 (2022-01-07)
         ------------------
         
         - Fixed call to `ToolPloneMeeting.isManager`, pass no context when `realManagers=True`.
           [gbastien]
         
         4.2b4 (2021-07-19)
```

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products.MeetingPROVHainaut.egg-info/SOURCES.txt` & `Products.MeetingPROVHainaut-4.2b6/src/Products.MeetingPROVHainaut.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/setuphandlers.py` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/setuphandlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,19 @@
 from dexterity.localroles.utils import add_fti_configuration
 from plone import api
 from Products.CMFPlone.utils import _createObjectByType
 from Products.MeetingCommunes.config import SAMPLE_TEXT
 from Products.MeetingCommunes.setuphandlers import _showHomeTab
 from Products.MeetingCommunes.setuphandlers import logStep
 from Products.MeetingPROVHainaut.config import PROJECTNAME
+from Products.MeetingPROVHainaut.utils import finance_group_cec_uid
+from Products.MeetingPROVHainaut.utils import finance_group_no_cec_uid
 from Products.PloneMeeting.exportimport.content import ToolInitializer
 from Products.PloneMeeting.utils import org_id_to_uid
+from Products.PloneMeeting.indexes import REAL_ORG_UID_PATTERN
 
 import logging
 import os
 
 
 logger = logging.getLogger('MeetingPROVHainaut: setuphandlers')
 
@@ -46,17 +49,17 @@
     logStep("_configureDexterityLocalRolesField", context)
     _configureDexterityLocalRolesField()
     finalizePROVHainautInstance(context)
     # configure the FINANCE_ADVICES_COLLECTION_ID collection
     site = context.getSite()
     cfg = site.portal_plonemeeting.objectValues('MeetingConfig')[0]
     cfg.adapted()._setUsedFinanceGroupIds(
-        ['delay_row_id__unique_id_002',
-         'delay_row_id__unique_id_003',
-         'delay_row_id__unique_id_004'])
+        [u'delay_row_id__unique_id_003',
+         REAL_ORG_UID_PATTERN.format(finance_group_cec_uid()),
+         REAL_ORG_UID_PATTERN.format(finance_group_no_cec_uid())])
 
 
 def post_handler_testing(context):
     """ """
     if not hasattr(context, '_profile_path'):
         profile_id = 'profile-Products.MeetingPROVHainaut:testing'
         context = context._getImportContext(profile_id)
@@ -294,14 +297,16 @@
     mTool.createMemberArea(userId)
     # in tests, the MeetingConfig id is generated
     cfg1 = tool.objectValues('MeetingConfig')[0]
     cfg1_id = cfg1.getId()
     userFolder = tool.getPloneMeetingFolder(cfg1_id, userId)
     date = datetime.now() - timedelta(days=1)
     with api.env.adopt_user(userId):
+        # avoid problems with cached methods when using adopt_user
+        tool.invalidateAllCache()
         meeting = api.content.create(container=userFolder,
                                      type='MeetingZCollege',
                                      id=date.strftime('%Y%m%d'),
                                      date=date)
         i = 1
         cfg = tool.getMeetingConfig(meeting)
         site.REQUEST['PUBLISHED'] = meeting
```

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/skins/meetingprovhainaut_styles/meetingprovincehainaut.css.dtml` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/skins/meetingprovhainaut_styles/meetingprovincehainaut.css.dtml`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/skins/meetingprovhainaut_styles/imioapps_properties.props` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/skins/meetingprovhainaut_styles/imioapps_properties.props`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/skins/meetingprovhainaut_images/logo.png` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/skins/meetingprovhainaut_images/logo.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/skins/meetingprovhainaut_images/spinner.gif` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/skins/meetingprovhainaut_images/spinner.gif`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/skins/meetingprovhainaut_images/favicon.ico` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/skins/meetingprovhainaut_images/favicon.ico`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/configure.zcml` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/adapters.py` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/adapters.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,14 @@
     ''' '''
 
     def __init__(self, item):
         self.context = item
 
     def mayEvaluateCompleteness(self):
         '''Completeness can be evaluated by the finance precontroller.'''
-
         item = self.getSelf()
         if item.isDefinedInTool():
             return False
 
         # finances advice asked?
         finance_org_uid = finance_group_uid()
         finance_org_cec_uid = finance_group_cec_uid()
```

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/locales/PloneMeeting.pot` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/locales/PloneMeeting.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/locales/en/LC_MESSAGES/plone.po` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/locales/en/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/locales/en/LC_MESSAGES/PloneMeeting.po` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/locales/en/LC_MESSAGES/PloneMeeting.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/locales/fr/LC_MESSAGES/plone.po` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/locales/fr/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/locales/fr/LC_MESSAGES/PloneMeeting.po` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/locales/fr/LC_MESSAGES/PloneMeeting.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/testing/images/overheadAnalysis.png` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/testing/images/overheadAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/testing/images/positive.png` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/testing/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/testing/images/attach.png` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/testing/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/testing/images/cahier.png` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/testing/images/cahier.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/testing/images/budget.png` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/testing/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/testing/images/financialAnalysis.png` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/testing/images/financialAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/testing/import_data.py` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/testing/import_data.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/default/skins.xml` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/default/skins.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/default/types/meetingadvicefinancescec.xml` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/default/types/meetingadvicefinancescec.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/default/types/meetingadvicefinances.xml` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/default/types/meetingadvicefinances.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/default/types/meetingadvicefinancesnocec.xml` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/default/types/meetingadvicefinancesnocec.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/default/cssregistry.xml` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/default/cssregistry.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/organizations.csv` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/organizations.csv`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/positive.png` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/attach.png` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/cahier.png` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/cahier.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/budget.png` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/remarks.png` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/legalAdvice.png` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/negative.png` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/deliberation_signed.png` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/images/deliberation_signed.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/note.odt` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/note.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/document-travail-conseil.odt` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/document-travail-conseil.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/convocation.odt` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/convocation.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/document-travail-college.odt` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/document-travail-college.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/presences.odt` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/presences.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/deliberation.odt` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/deliberation.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/bordereaux.odt` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/bordereaux.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/arrete.odt` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/arrete.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/pv.odt` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/pv.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/rapport.odt` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/rapport.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/role.odt` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/role.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/resolution.odt` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/templates/resolution.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/import_data.py` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles/zprovhainaut/import_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -221,22 +221,22 @@
     u'getCategory', u'proposing_group_acronym', u'associated_groups_acronym',
     u'groups_in_charge_acronym', u'advices', u'toDiscuss', u'actions')
 collegeMeeting.itemActionsInterface = \
     'Products.MeetingPROVHainaut.interfaces.IMeetingItemPROVHainautWorkflowActions'
 collegeMeeting.itemConditionsInterface = \
     'Products.MeetingPROVHainaut.interfaces.IMeetingItemPROVHainautWorkflowConditions'
 collegeMeeting.itemWFValidationLevels = (
-    {'leading_transition': '',
+    {'leading_transition': '-',
      'state_title': 'itemcreated',
      'suffix': 'creators',
      'enabled': '1',
      'state': 'itemcreated',
      'back_transition_title': 'backToItemCreated',
      'back_transition': 'backToItemCreated',
-     'leading_transition_title': '',
+     'leading_transition_title': '-',
      'extra_suffixes': []},
     {'leading_transition': 'propose',
      'state_title': 'proposed',
      'suffix': 'reviewers',
      'enabled': '0',
      'state': 'proposed',
      'back_transition_title': 'backToProposed',
@@ -352,12 +352,30 @@
                                       'no_publication',
                                       'refused',
                                       'delayed',
                                       'accepted_but_modified',)
 councilMeeting.transitionsToConfirm = []
 councilMeeting.itemBudgetInfosStates = []
 councilMeeting.orderedContacts = []
-
 data = PloneMeetingConfiguration(
     meetingFolderTitle='Mes séances',
     meetingConfigs=[collegeMeeting, councilMeeting],
     orgs=orgs)
+data.directory_position_types = [
+    {'name': u'D\xe9faut', 'token': u'default'},
+    {'name': u'Pr\xe9sident|Pr\xe9sidents|Pr\xe9sidente|Pr\xe9sidentes',
+     'token': u'president'},
+    {'name': u'D\xe9put\xe9 provincial|D\xe9put\xe9s provinciaux|D\xe9put\xe9e provinciale|D\xe9put\xe9es provinciales',
+     'token': u'depute'},
+    {'name': u'Directeur G\xe9n\xe9ral provincial|Directeurs G\xe9n\xe9raux provinciaux|Directrice G\xe9n\xe9rale provinciale|Directrices G\xe9n\xe9rales provinciales',
+     'token': u'dgp'},
+    {'name': u'D\xe9put\xe9 provincial f.f.|D\xe9put\xe9s provinciaux f.f.|D\xe9put\xe9e provinciale f.f.|D\xe9put\xe9es provinciales f.f.',
+     'token': u'deputeff'},
+    {'name': u'Secr\xe9taire|Secr\xe9taires|Secr\xe9taire|Secr\xe9taires',
+     'token': u'secretaire'},
+    {'name': u'Commissaire du Gouvernement wallon|Commissaires du Gouvernement wallon|Commissaire du Gouvernement wallon|Commissaires du Gouvernement wallon',
+     'token': u'comgovw'},
+    {'name': u'Commissaire du Gouvernement wallon f.f.|Commissaires du Gouvernement wallon f.f.|Commissaire du Gouvernement wallon f.f.|Commissaires du Gouvernement wallon f.f.',
+     'token': u'comgovwff'},
+    {'name': u'Pr\xe9sident du Conseil provincial|Pr\xe9sidents du Conseil provincial|Pr\xe9sidente du Conseil provincial|Pr\xe9sidentes du Conseil provincial',
+     'token': u'president-cp'}
+]
```

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/testing.py` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/testing.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/interfaces.py` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/interfaces.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/utils.py` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/utils.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/testing.zcml` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/testing.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/vocabularies.py` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/vocabularies.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/Extensions/utils.py` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/Extensions/utils.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testFaceted.py` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testFaceted.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testAdvices.py` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testAdvices.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testMeetingCategory.py` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testMeetingCategory.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testChangeItemOrderView.py` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testChangeItemOrderView.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testUtils.py` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testUtils.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testColumns.py` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testColumns.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testSetup.py` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testSetup.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testToolPloneMeeting.py` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testToolPloneMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/helpers.py` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/MeetingPROVHainautTestCase.py` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/MeetingPROVHainautTestCase.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testMeetingItem.py` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testMeetingItem.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testWFAdaptations.py` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testWFAdaptations.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,18 +15,22 @@
              'accepted_out_of_meeting',
              'accepted_out_of_meeting_and_duplicated',
              'accepted_out_of_meeting_emergency',
              'accepted_out_of_meeting_emergency_and_duplicated',
              'decide_item_when_back_to_meeting_from_returned_to_proposing_group',
              'delayed',
              'hide_decisions_when_under_writing',
+             'item_validation_no_validate_shortcuts',
+             'item_validation_shortcuts',
              'mark_not_applicable',
              'meetingadvicefinances_add_advicecreated_state',
              'meetingadvicefinances_controller_propose_to_manager',
              'meetingmanager_correct_closed_meeting',
+             'no_decide',
+             'no_freeze',
              'no_publication',
              'only_creator_may_delete',
              'postpone_next_meeting',
              'pre_accepted',
              'presented_item_back_to_itemcreated',
              'presented_item_back_to_proposed',
              'refused',
```

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testValidators.py` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testValidators.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testPortlets.py` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testPortlets.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testAnnexes.py` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testAnnexes.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/__init__.py` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testMeeting.py` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testSearches.py` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testSearches.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/tests/testViews.py` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/tests/testViews.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/overrides.zcml` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/overrides.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/profiles.zcml` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/profiles.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/migrations/migrate_to_4202.py` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/migrations/migrate_to_4202.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/migrations/migrate_to_4200.py` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/migrations/migrate_to_4200.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/migrations/migrate_to_4203.py` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/migrations/migrate_to_4203.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/src/Products/MeetingPROVHainaut/migrations/migrate_to_4201.py` & `Products.MeetingPROVHainaut-4.2b6/src/Products/MeetingPROVHainaut/migrations/migrate_to_4201.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/docs/LICENSE.txt` & `Products.MeetingPROVHainaut-4.2b6/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/docs/LICENSE.GPL` & `Products.MeetingPROVHainaut-4.2b6/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/setup.py` & `Products.MeetingPROVHainaut-4.2b6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = '4.2b5'
+version = '4.2b6'
 
 setup(name='Products.MeetingPROVHainaut',
       version=version,
       description="PloneMeeting profile for Province de Hainaut",
       long_description=open("README.rst").read() + "\n\n" + open("CHANGES.rst").read(),
       classifiers=["Programming Language :: Python"],
       keywords='',
```

### Comparing `Products.MeetingPROVHainaut-4.2b5/PKG-INFO` & `Products.MeetingPROVHainaut-4.2b6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 Metadata-Version: 2.1
 Name: Products.MeetingPROVHainaut
-Version: 4.2b5
+Version: 4.2b6
 Summary: PloneMeeting profile for Province de Hainaut
 Home-page: http://www.imio.be/produits/gestion-des-deliberations
 Author: 
 Author-email: 
 License: GPL
 Description: Products.PloneMeeting profile for Province de Hainaut (Belgium)
         ===============================================================
         
         
         
         Products.MeetingPROVHainaut Changelog
         =====================================
         
+        4.2b6 (2022-04-28)
+        ------------------
+        
+        - Adapted `events.onAdviceAfterTransition`, do no more call
+          `MeetingItem.update_local_roles` as it is done in PloneMeeting in
+          `events.onAdviceTransition` now, just after call to `AdviceAfterTransitionEvent`.
+          [gbastien]
+        - Fixed `zprovhainaut import_data`, was failing with demo data.
+          [gbastien]
+        
         4.2b5 (2022-01-07)
         ------------------
         
         - Fixed call to `ToolPloneMeeting.isManager`, pass no context when `realManagers=True`.
           [gbastien]
         
         4.2b4 (2021-07-19)
```

### Comparing `Products.MeetingPROVHainaut-4.2b5/MANIFEST.in` & `Products.MeetingPROVHainaut-4.2b6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Products.MeetingPROVHainaut-4.2b5/CHANGES.rst` & `Products.MeetingPROVHainaut-4.2b6/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Products.MeetingPROVHainaut Changelog
 =====================================
 
+4.2b6 (2022-04-28)
+------------------
+
+- Adapted `events.onAdviceAfterTransition`, do no more call
+  `MeetingItem.update_local_roles` as it is done in PloneMeeting in
+  `events.onAdviceTransition` now, just after call to `AdviceAfterTransitionEvent`.
+  [gbastien]
+- Fixed `zprovhainaut import_data`, was failing with demo data.
+  [gbastien]
+
 4.2b5 (2022-01-07)
 ------------------
 
 - Fixed call to `ToolPloneMeeting.isManager`, pass no context when `realManagers=True`.
   [gbastien]
 
 4.2b4 (2021-07-19)
```

