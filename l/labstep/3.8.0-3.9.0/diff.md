# Comparing `tmp/labstep-3.8.0.tar.gz` & `tmp/labstep-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labstep-3.8.0.tar", last modified: Fri Nov 19 13:46:57 2021, max compression
+gzip compressed data, was "labstep-3.9.0.tar", last modified: Wed Dec  8 17:42:14 2021, max compression
```

## Comparing `labstep-3.8.0.tar` & `labstep-3.9.0.tar`

### file list

```diff
@@ -1,170 +1,176 @@
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.522356 labstep-3.8.0/
--rw-r--r--   0 barneywalker   (501) staff       (20)      921 2021-11-19 13:46:57.522072 labstep-3.8.0/PKG-INFO
--rw-r--r--   0 barneywalker   (501) staff       (20)      681 2020-11-17 16:28:10.000000 labstep-3.8.0/README.rst
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.462044 labstep-3.8.0/labstep/
--rwxr-xr-x   0 barneywalker   (501) staff       (20)      268 2021-10-18 11:49:26.000000 labstep-3.8.0/labstep/__init__.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.465754 labstep-3.8.0/labstep/config/
--rw-r--r--   0 barneywalker   (501) staff       (20)       30 2021-04-15 16:09:10.000000 labstep-3.8.0/labstep/config/export.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.466575 labstep-3.8.0/labstep/constants/
--rw-r--r--   0 barneywalker   (501) staff       (20)      111 2021-11-19 13:46:21.000000 labstep-3.8.0/labstep/constants/version.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.467731 labstep-3.8.0/labstep/converter/
--rw-r--r--   0 barneywalker   (501) staff       (20)       40 2021-01-12 09:57:43.000000 labstep-3.8.0/labstep/converter/__init__.py
--rw-r--r--   0 barneywalker   (501) staff       (20)      614 2021-01-15 18:28:50.000000 labstep-3.8.0/labstep/converter/htmlToProseMirror.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.458572 labstep-3.8.0/labstep/entities/
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.469369 labstep-3.8.0/labstep/entities/autoshare/
--rw-r--r--   0 barneywalker   (501) staff       (20)     1854 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/autoshare/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)        0 2021-01-28 17:00:26.000000 labstep-3.8.0/labstep/entities/autoshare/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.470507 labstep-3.8.0/labstep/entities/collection/
--rw-r--r--   0 barneywalker   (501) staff       (20)     1778 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/collection/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)     2311 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/collection/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.471963 labstep-3.8.0/labstep/entities/comment/
--rw-r--r--   0 barneywalker   (501) staff       (20)     1384 2021-11-05 12:24:47.000000 labstep-3.8.0/labstep/entities/comment/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)     2003 2021-11-19 13:46:21.000000 labstep-3.8.0/labstep/entities/comment/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.473644 labstep-3.8.0/labstep/entities/device/
--rw-r--r--   0 barneywalker   (501) staff       (20)     7495 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/device/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)      843 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/device/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.475136 labstep-3.8.0/labstep/entities/deviceData/
--rw-r--r--   0 barneywalker   (501) staff       (20)      554 2021-10-18 11:49:26.000000 labstep-3.8.0/labstep/entities/deviceData/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)        0 2021-01-12 09:57:43.000000 labstep-3.8.0/labstep/entities/deviceData/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.476579 labstep-3.8.0/labstep/entities/experiment/
--rw-r--r--   0 barneywalker   (501) staff       (20)    16175 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/experiment/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)     2805 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/experiment/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.478200 labstep-3.8.0/labstep/entities/experimentDataField/
--rw-r--r--   0 barneywalker   (501) staff       (20)     5072 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/experimentDataField/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)     4414 2021-11-19 13:46:21.000000 labstep-3.8.0/labstep/entities/experimentDataField/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.479681 labstep-3.8.0/labstep/entities/experimentMaterial/
--rw-r--r--   0 barneywalker   (501) staff       (20)     2106 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/experimentMaterial/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)     1574 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/experimentMaterial/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.480872 labstep-3.8.0/labstep/entities/experimentProtocol/
--rw-r--r--   0 barneywalker   (501) staff       (20)    15091 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/experimentProtocol/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)      708 2021-10-18 11:49:26.000000 labstep-3.8.0/labstep/entities/experimentProtocol/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.482020 labstep-3.8.0/labstep/entities/experimentSignature/
--rw-r--r--   0 barneywalker   (501) staff       (20)      675 2021-10-18 11:49:26.000000 labstep-3.8.0/labstep/entities/experimentSignature/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)        0 2021-01-12 09:57:43.000000 labstep-3.8.0/labstep/entities/experimentSignature/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.482811 labstep-3.8.0/labstep/entities/experimentSignatureRequest/
--rw-r--r--   0 barneywalker   (501) staff       (20)      712 2021-10-18 11:49:26.000000 labstep-3.8.0/labstep/entities/experimentSignatureRequest/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)      703 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/experimentSignatureRequest/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.484151 labstep-3.8.0/labstep/entities/experimentStep/
--rw-r--r--   0 barneywalker   (501) staff       (20)     2956 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/experimentStep/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)        0 2021-01-12 09:57:43.000000 labstep-3.8.0/labstep/entities/experimentStep/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.485038 labstep-3.8.0/labstep/entities/experimentTable/
--rw-r--r--   0 barneywalker   (501) staff       (20)     3123 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/experimentTable/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)        0 2021-01-12 09:57:43.000000 labstep-3.8.0/labstep/entities/experimentTable/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.486018 labstep-3.8.0/labstep/entities/experimentTimer/
--rw-r--r--   0 barneywalker   (501) staff       (20)     1872 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/experimentTimer/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)        0 2021-01-12 09:57:43.000000 labstep-3.8.0/labstep/entities/experimentTimer/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.487046 labstep-3.8.0/labstep/entities/file/
--rw-r--r--   0 barneywalker   (501) staff       (20)     2065 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/file/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)     1988 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/file/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.488661 labstep-3.8.0/labstep/entities/invitation/
--rw-r--r--   0 barneywalker   (501) staff       (20)      214 2021-04-15 16:09:10.000000 labstep-3.8.0/labstep/entities/invitation/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)     1010 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/invitation/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.489604 labstep-3.8.0/labstep/entities/jupyterInstance/
--rw-r--r--   0 barneywalker   (501) staff       (20)     1782 2021-11-05 12:24:47.000000 labstep-3.8.0/labstep/entities/jupyterInstance/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)      566 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/jupyterInstance/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.490656 labstep-3.8.0/labstep/entities/jupyterNotebook/
--rw-r--r--   0 barneywalker   (501) staff       (20)     1270 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/jupyterNotebook/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)      772 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/jupyterNotebook/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.491703 labstep-3.8.0/labstep/entities/metadata/
--rw-r--r--   0 barneywalker   (501) staff       (20)     4296 2021-11-19 13:46:21.000000 labstep-3.8.0/labstep/entities/metadata/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)     2462 2021-11-19 11:52:41.000000 labstep-3.8.0/labstep/entities/metadata/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.492725 labstep-3.8.0/labstep/entities/orderRequest/
--rw-r--r--   0 barneywalker   (501) staff       (20)     3197 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/orderRequest/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)     1484 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/orderRequest/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.494186 labstep-3.8.0/labstep/entities/organization/
--rw-r--r--   0 barneywalker   (501) staff       (20)     4229 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/organization/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)      868 2021-10-18 11:49:26.000000 labstep-3.8.0/labstep/entities/organization/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.495035 labstep-3.8.0/labstep/entities/organizationUser/
--rw-r--r--   0 barneywalker   (501) staff       (20)     1332 2021-10-18 11:49:26.000000 labstep-3.8.0/labstep/entities/organizationUser/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)     1150 2021-10-18 11:49:26.000000 labstep-3.8.0/labstep/entities/organizationUser/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.495815 labstep-3.8.0/labstep/entities/permission/
--rw-r--r--   0 barneywalker   (501) staff       (20)     1090 2021-10-18 11:49:26.000000 labstep-3.8.0/labstep/entities/permission/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)     2590 2021-10-29 09:14:15.000000 labstep-3.8.0/labstep/entities/permission/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.496973 labstep-3.8.0/labstep/entities/protocol/
--rw-r--r--   0 barneywalker   (501) staff       (20)    16761 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/protocol/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)     2409 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/protocol/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.497872 labstep-3.8.0/labstep/entities/protocolDataField/
--rw-r--r--   0 barneywalker   (501) staff       (20)     3172 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/protocolDataField/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)     1816 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/protocolDataField/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.498793 labstep-3.8.0/labstep/entities/protocolMaterial/
--rw-r--r--   0 barneywalker   (501) staff       (20)     1823 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/protocolMaterial/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)     1398 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/protocolMaterial/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.499978 labstep-3.8.0/labstep/entities/protocolStep/
--rw-r--r--   0 barneywalker   (501) staff       (20)      208 2021-01-12 09:57:43.000000 labstep-3.8.0/labstep/entities/protocolStep/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)        0 2021-01-12 09:57:43.000000 labstep-3.8.0/labstep/entities/protocolStep/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.500621 labstep-3.8.0/labstep/entities/protocolTable/
--rw-r--r--   0 barneywalker   (501) staff       (20)     3095 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/protocolTable/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)        0 2021-01-12 09:57:43.000000 labstep-3.8.0/labstep/entities/protocolTable/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.501219 labstep-3.8.0/labstep/entities/protocolTimer/
--rw-r--r--   0 barneywalker   (501) staff       (20)     1443 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/protocolTimer/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)        0 2021-01-12 09:57:43.000000 labstep-3.8.0/labstep/entities/protocolTimer/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.502041 labstep-3.8.0/labstep/entities/protocolVersion/
--rw-r--r--   0 barneywalker   (501) staff       (20)      206 2021-01-12 09:57:43.000000 labstep-3.8.0/labstep/entities/protocolVersion/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)        0 2021-01-12 09:57:43.000000 labstep-3.8.0/labstep/entities/protocolVersion/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.502687 labstep-3.8.0/labstep/entities/resource/
--rw-r--r--   0 barneywalker   (501) staff       (20)     9127 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/resource/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)     1136 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/resource/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.503512 labstep-3.8.0/labstep/entities/resourceCategory/
--rw-r--r--   0 barneywalker   (501) staff       (20)     4194 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/resourceCategory/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)     2396 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/resourceCategory/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.504358 labstep-3.8.0/labstep/entities/resourceItem/
--rw-r--r--   0 barneywalker   (501) staff       (20)     6941 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/resourceItem/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)     1832 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/resourceItem/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.505036 labstep-3.8.0/labstep/entities/resourceLocation/
--rw-r--r--   0 barneywalker   (501) staff       (20)     2665 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/resourceLocation/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)     1115 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/resourceLocation/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.505794 labstep-3.8.0/labstep/entities/resourceTemplate/
--rw-r--r--   0 barneywalker   (501) staff       (20)     2482 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/resourceTemplate/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)        0 2021-01-12 09:57:43.000000 labstep-3.8.0/labstep/entities/resourceTemplate/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.506438 labstep-3.8.0/labstep/entities/sharelink/
--rw-r--r--   0 barneywalker   (501) staff       (20)     2157 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/sharelink/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)      386 2021-10-18 11:49:26.000000 labstep-3.8.0/labstep/entities/sharelink/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.507494 labstep-3.8.0/labstep/entities/tag/
--rw-r--r--   0 barneywalker   (501) staff       (20)     1588 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/tag/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)     4661 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/tag/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.509254 labstep-3.8.0/labstep/entities/user/
--rw-r--r--   0 barneywalker   (501) staff       (20)     1755 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/user/facade.py
--rw-r--r--   0 barneywalker   (501) staff       (20)    30816 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/user/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)     2038 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/user/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.510741 labstep-3.8.0/labstep/entities/workspace/
--rw-r--r--   0 barneywalker   (501) staff       (20)    20582 2021-11-19 13:46:21.000000 labstep-3.8.0/labstep/entities/workspace/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)      874 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/workspace/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.511927 labstep-3.8.0/labstep/entities/workspaceMember/
--rw-r--r--   0 barneywalker   (501) staff       (20)      722 2021-10-18 11:49:26.000000 labstep-3.8.0/labstep/entities/workspaceMember/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)     1221 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/entities/workspaceMember/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.460374 labstep-3.8.0/labstep/generic/
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.512993 labstep-3.8.0/labstep/generic/entity/
--rw-r--r--   0 barneywalker   (501) staff       (20)     1556 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/generic/entity/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)     5441 2021-11-19 11:56:00.000000 labstep-3.8.0/labstep/generic/entity/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.513647 labstep-3.8.0/labstep/generic/entityList/
--rw-r--r--   0 barneywalker   (501) staff       (20)      560 2021-11-11 19:24:14.000000 labstep-3.8.0/labstep/generic/entityList/model.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.514304 labstep-3.8.0/labstep/generic/entityPrimary/
--rw-r--r--   0 barneywalker   (501) staff       (20)      386 2021-11-05 12:24:47.000000 labstep-3.8.0/labstep/generic/entityPrimary/model.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.515012 labstep-3.8.0/labstep/generic/entityWithComments/
--rw-r--r--   0 barneywalker   (501) staff       (20)     1665 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/generic/entityWithComments/model.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.515883 labstep-3.8.0/labstep/generic/entityWithMetadata/
--rw-r--r--   0 barneywalker   (501) staff       (20)     2408 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/generic/entityWithMetadata/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)        0 2021-11-05 12:24:47.000000 labstep-3.8.0/labstep/generic/entityWithMetadata/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.516148 labstep-3.8.0/labstep/generic/entityWithSharing/
--rw-r--r--   0 barneywalker   (501) staff       (20)     1880 2021-11-05 12:24:47.000000 labstep-3.8.0/labstep/generic/entityWithSharing/model.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.517252 labstep-3.8.0/labstep/generic/entityWithTags/
--rw-r--r--   0 barneywalker   (501) staff       (20)     1325 2021-11-05 12:24:47.000000 labstep-3.8.0/labstep/generic/entityWithTags/model.py
--rw-r--r--   0 barneywalker   (501) staff       (20)        0 2021-11-05 12:24:47.000000 labstep-3.8.0/labstep/generic/entityWithTags/repository.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.521350 labstep-3.8.0/labstep/service/
--rw-r--r--   0 barneywalker   (501) staff       (20)        0 2021-01-12 09:57:43.000000 labstep-3.8.0/labstep/service/__init__.py
--rwxr-xr-x   0 barneywalker   (501) staff       (20)      607 2021-09-07 14:21:12.000000 labstep-3.8.0/labstep/service/config.py
--rwxr-xr-x   0 barneywalker   (501) staff       (20)     3497 2021-11-19 13:46:21.000000 labstep-3.8.0/labstep/service/helpers.py
--rwxr-xr-x   0 barneywalker   (501) staff       (20)     1786 2021-11-08 17:07:55.000000 labstep-3.8.0/labstep/service/htmlExport.py
--rwxr-xr-x   0 barneywalker   (501) staff       (20)      949 2021-01-15 18:28:50.000000 labstep-3.8.0/labstep/service/htmlToProseMirror.py
--rwxr-xr-x   0 barneywalker   (501) staff       (20)      698 2021-10-18 11:49:26.000000 labstep-3.8.0/labstep/service/jupyter.py
--rwxr-xr-x   0 barneywalker   (501) staff       (20)      503 2021-09-01 17:37:18.000000 labstep-3.8.0/labstep/service/ping.py
--rwxr-xr-x   0 barneywalker   (501) staff       (20)     2335 2021-11-19 11:19:25.000000 labstep-3.8.0/labstep/service/request.py
-drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-11-19 13:46:57.465388 labstep-3.8.0/labstep.egg-info/
--rw-r--r--   0 barneywalker   (501) staff       (20)      921 2021-11-19 13:46:57.000000 labstep-3.8.0/labstep.egg-info/PKG-INFO
--rw-r--r--   0 barneywalker   (501) staff       (20)     4373 2021-11-19 13:46:57.000000 labstep-3.8.0/labstep.egg-info/SOURCES.txt
--rw-r--r--   0 barneywalker   (501) staff       (20)        1 2021-11-19 13:46:57.000000 labstep-3.8.0/labstep.egg-info/dependency_links.txt
--rw-r--r--   0 barneywalker   (501) staff       (20)        1 2020-11-18 11:42:18.000000 labstep-3.8.0/labstep.egg-info/not-zip-safe
--rw-r--r--   0 barneywalker   (501) staff       (20)       69 2021-11-19 13:46:57.000000 labstep-3.8.0/labstep.egg-info/requires.txt
--rw-r--r--   0 barneywalker   (501) staff       (20)        8 2021-11-19 13:46:57.000000 labstep-3.8.0/labstep.egg-info/top_level.txt
--rw-r--r--   0 barneywalker   (501) staff       (20)       38 2021-11-19 13:46:57.522451 labstep-3.8.0/setup.cfg
--rw-r--r--   0 barneywalker   (501) staff       (20)      793 2021-11-15 16:16:36.000000 labstep-3.8.0/setup.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.763681 labstep-3.9.0/
+-rw-r--r--   0 barneywalker   (501) staff       (20)      921 2021-12-08 17:42:14.763438 labstep-3.9.0/PKG-INFO
+-rw-r--r--   0 barneywalker   (501) staff       (20)      681 2020-11-17 16:28:10.000000 labstep-3.9.0/README.rst
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.720754 labstep-3.9.0/labstep/
+-rwxr-xr-x   0 barneywalker   (501) staff       (20)      268 2021-10-18 11:49:26.000000 labstep-3.9.0/labstep/__init__.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.723384 labstep-3.9.0/labstep/config/
+-rw-r--r--   0 barneywalker   (501) staff       (20)       30 2021-11-26 11:57:06.000000 labstep-3.9.0/labstep/config/export.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.724758 labstep-3.9.0/labstep/constants/
+-rw-r--r--   0 barneywalker   (501) staff       (20)       66 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/constants/__init__.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)      101 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/constants/unspecified.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)       18 2021-12-08 17:35:36.000000 labstep-3.9.0/labstep/constants/version.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.725697 labstep-3.9.0/labstep/converter/
+-rw-r--r--   0 barneywalker   (501) staff       (20)       40 2021-01-12 09:57:43.000000 labstep-3.9.0/labstep/converter/__init__.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)      614 2021-01-15 18:28:50.000000 labstep-3.9.0/labstep/converter/htmlToProseMirror.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.718814 labstep-3.9.0/labstep/entities/
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.726789 labstep-3.9.0/labstep/entities/autoshare/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     1931 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/autoshare/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)        0 2021-01-28 17:00:26.000000 labstep-3.9.0/labstep/entities/autoshare/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.727422 labstep-3.9.0/labstep/entities/collection/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     1827 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/collection/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)     2367 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/collection/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.728129 labstep-3.9.0/labstep/entities/comment/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     1384 2021-11-05 12:24:47.000000 labstep-3.9.0/labstep/entities/comment/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)     2087 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/comment/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.728722 labstep-3.9.0/labstep/entities/device/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     7647 2021-12-07 13:37:45.000000 labstep-3.9.0/labstep/entities/device/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)      906 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/device/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.729409 labstep-3.9.0/labstep/entities/deviceData/
+-rw-r--r--   0 barneywalker   (501) staff       (20)      554 2021-10-18 11:49:26.000000 labstep-3.9.0/labstep/entities/deviceData/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)        0 2021-01-12 09:57:43.000000 labstep-3.9.0/labstep/entities/deviceData/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.730501 labstep-3.9.0/labstep/entities/experiment/
+-rw-r--r--   0 barneywalker   (501) staff       (20)    19656 2021-12-08 17:09:00.000000 labstep-3.9.0/labstep/entities/experiment/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)     2931 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/experiment/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.731598 labstep-3.9.0/labstep/entities/experimentDataField/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     5128 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/experimentDataField/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)     4519 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/experimentDataField/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.732434 labstep-3.9.0/labstep/entities/experimentLink/
+-rw-r--r--   0 barneywalker   (501) staff       (20)      766 2021-12-08 11:59:18.000000 labstep-3.9.0/labstep/entities/experimentLink/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)      702 2021-12-08 11:59:18.000000 labstep-3.9.0/labstep/entities/experimentLink/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.733092 labstep-3.9.0/labstep/entities/experimentMaterial/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     2183 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/experimentMaterial/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)     1686 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/experimentMaterial/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.734211 labstep-3.9.0/labstep/entities/experimentProtocol/
+-rw-r--r--   0 barneywalker   (501) staff       (20)    15294 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/experimentProtocol/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)      708 2021-10-18 11:49:26.000000 labstep-3.9.0/labstep/entities/experimentProtocol/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.734820 labstep-3.9.0/labstep/entities/experimentSignature/
+-rw-r--r--   0 barneywalker   (501) staff       (20)      675 2021-10-18 11:49:26.000000 labstep-3.9.0/labstep/entities/experimentSignature/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)        0 2021-01-12 09:57:43.000000 labstep-3.9.0/labstep/entities/experimentSignature/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.735534 labstep-3.9.0/labstep/entities/experimentSignatureRequest/
+-rw-r--r--   0 barneywalker   (501) staff       (20)      712 2021-10-18 11:49:26.000000 labstep-3.9.0/labstep/entities/experimentSignatureRequest/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)      752 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/experimentSignatureRequest/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.736522 labstep-3.9.0/labstep/entities/experimentStep/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     1418 2021-12-08 17:09:00.000000 labstep-3.9.0/labstep/entities/experimentStep/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)        0 2021-01-12 09:57:43.000000 labstep-3.9.0/labstep/entities/experimentStep/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.737070 labstep-3.9.0/labstep/entities/experimentTable/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     3179 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/experimentTable/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)        0 2021-01-12 09:57:43.000000 labstep-3.9.0/labstep/entities/experimentTable/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.737860 labstep-3.9.0/labstep/entities/experimentTimer/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     1979 2021-12-07 13:37:45.000000 labstep-3.9.0/labstep/entities/experimentTimer/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)        0 2021-01-12 09:57:43.000000 labstep-3.9.0/labstep/entities/experimentTimer/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.738598 labstep-3.9.0/labstep/entities/file/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     2135 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/file/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)     2190 2021-12-07 13:37:45.000000 labstep-3.9.0/labstep/entities/file/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.739839 labstep-3.9.0/labstep/entities/invitation/
+-rw-r--r--   0 barneywalker   (501) staff       (20)      214 2021-04-15 16:09:10.000000 labstep-3.9.0/labstep/entities/invitation/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)     1066 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/invitation/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.740599 labstep-3.9.0/labstep/entities/jupyterInstance/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     2553 2021-12-07 13:37:45.000000 labstep-3.9.0/labstep/entities/jupyterInstance/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)      666 2021-12-07 13:37:45.000000 labstep-3.9.0/labstep/entities/jupyterInstance/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.741203 labstep-3.9.0/labstep/entities/jupyterNotebook/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     1333 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/jupyterNotebook/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)      849 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/jupyterNotebook/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.741812 labstep-3.9.0/labstep/entities/metadata/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     4351 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/metadata/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)     2586 2021-12-07 13:37:45.000000 labstep-3.9.0/labstep/entities/metadata/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.742489 labstep-3.9.0/labstep/entities/orderRequest/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     3274 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/orderRequest/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)     1596 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/orderRequest/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.743193 labstep-3.9.0/labstep/entities/organization/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     4285 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/organization/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)      868 2021-10-18 11:49:26.000000 labstep-3.9.0/labstep/entities/organization/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.744032 labstep-3.9.0/labstep/entities/organizationUser/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     1332 2021-10-18 11:49:26.000000 labstep-3.9.0/labstep/entities/organizationUser/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)     1150 2021-10-18 11:49:26.000000 labstep-3.9.0/labstep/entities/organizationUser/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.744790 labstep-3.9.0/labstep/entities/permission/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     1090 2021-10-18 11:49:26.000000 labstep-3.9.0/labstep/entities/permission/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)     2590 2021-10-29 09:14:15.000000 labstep-3.9.0/labstep/entities/permission/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.745331 labstep-3.9.0/labstep/entities/protocol/
+-rw-r--r--   0 barneywalker   (501) staff       (20)    16936 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/protocol/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)     2514 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/protocol/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.745827 labstep-3.9.0/labstep/entities/protocolDataField/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     3228 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/protocolDataField/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)     1921 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/protocolDataField/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.746307 labstep-3.9.0/labstep/entities/protocolMaterial/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     1893 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/protocolMaterial/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)     1496 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/protocolMaterial/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.747494 labstep-3.9.0/labstep/entities/protocolStep/
+-rw-r--r--   0 barneywalker   (501) staff       (20)      208 2021-01-12 09:57:43.000000 labstep-3.9.0/labstep/entities/protocolStep/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)        0 2021-01-12 09:57:43.000000 labstep-3.9.0/labstep/entities/protocolStep/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.748489 labstep-3.9.0/labstep/entities/protocolTable/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     3151 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/protocolTable/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)        0 2021-01-12 09:57:43.000000 labstep-3.9.0/labstep/entities/protocolTable/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.749204 labstep-3.9.0/labstep/entities/protocolTimer/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     1557 2021-12-07 13:37:45.000000 labstep-3.9.0/labstep/entities/protocolTimer/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)        0 2021-01-12 09:57:43.000000 labstep-3.9.0/labstep/entities/protocolTimer/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.749667 labstep-3.9.0/labstep/entities/protocolVersion/
+-rw-r--r--   0 barneywalker   (501) staff       (20)      206 2021-01-12 09:57:43.000000 labstep-3.9.0/labstep/entities/protocolVersion/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)        0 2021-01-12 09:57:43.000000 labstep-3.9.0/labstep/entities/protocolVersion/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.750137 labstep-3.9.0/labstep/entities/resource/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     9211 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/resource/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)     1220 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/resource/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.750832 labstep-3.9.0/labstep/entities/resourceCategory/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     4243 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/resourceCategory/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)     2466 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/resourceCategory/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.751815 labstep-3.9.0/labstep/entities/resourceItem/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     7060 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/resourceItem/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)     1972 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/resourceItem/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.752485 labstep-3.9.0/labstep/entities/resourceLocation/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     2714 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/resourceLocation/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)     1132 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/resourceLocation/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.753142 labstep-3.9.0/labstep/entities/resourceTemplate/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     2559 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/resourceTemplate/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)        0 2021-01-12 09:57:43.000000 labstep-3.9.0/labstep/entities/resourceTemplate/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.753633 labstep-3.9.0/labstep/entities/sharelink/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     2213 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/sharelink/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)      386 2021-10-18 11:49:26.000000 labstep-3.9.0/labstep/entities/sharelink/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.754185 labstep-3.9.0/labstep/entities/tag/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     1637 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/tag/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)     4717 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/tag/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.755038 labstep-3.9.0/labstep/entities/user/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     1825 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/user/facade.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)    31082 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/user/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)     2074 2021-12-07 13:37:45.000000 labstep-3.9.0/labstep/entities/user/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.756118 labstep-3.9.0/labstep/entities/workspace/
+-rw-r--r--   0 barneywalker   (501) staff       (20)    20834 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/workspace/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)      937 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/workspace/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.756713 labstep-3.9.0/labstep/entities/workspaceMember/
+-rw-r--r--   0 barneywalker   (501) staff       (20)      722 2021-10-18 11:49:26.000000 labstep-3.9.0/labstep/entities/workspaceMember/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)     1270 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/entities/workspaceMember/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.719857 labstep-3.9.0/labstep/generic/
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.757256 labstep-3.9.0/labstep/generic/entity/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     1666 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/generic/entity/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)     5286 2021-12-08 17:09:00.000000 labstep-3.9.0/labstep/generic/entity/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.757526 labstep-3.9.0/labstep/generic/entityList/
+-rw-r--r--   0 barneywalker   (501) staff       (20)      573 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/generic/entityList/model.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.757775 labstep-3.9.0/labstep/generic/entityPrimary/
+-rw-r--r--   0 barneywalker   (501) staff       (20)      386 2021-11-05 12:24:47.000000 labstep-3.9.0/labstep/generic/entityPrimary/model.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.758015 labstep-3.9.0/labstep/generic/entityWithComments/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     1714 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/generic/entityWithComments/model.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.758505 labstep-3.9.0/labstep/generic/entityWithMetadata/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     2485 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/generic/entityWithMetadata/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)        0 2021-11-05 12:24:47.000000 labstep-3.9.0/labstep/generic/entityWithMetadata/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.758691 labstep-3.9.0/labstep/generic/entityWithSharing/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     1880 2021-11-05 12:24:47.000000 labstep-3.9.0/labstep/generic/entityWithSharing/model.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.759175 labstep-3.9.0/labstep/generic/entityWithTags/
+-rw-r--r--   0 barneywalker   (501) staff       (20)     1325 2021-11-05 12:24:47.000000 labstep-3.9.0/labstep/generic/entityWithTags/model.py
+-rw-r--r--   0 barneywalker   (501) staff       (20)        0 2021-11-05 12:24:47.000000 labstep-3.9.0/labstep/generic/entityWithTags/repository.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.762806 labstep-3.9.0/labstep/service/
+-rw-r--r--   0 barneywalker   (501) staff       (20)        0 2021-01-12 09:57:43.000000 labstep-3.9.0/labstep/service/__init__.py
+-rwxr-xr-x   0 barneywalker   (501) staff       (20)      607 2021-09-07 14:21:12.000000 labstep-3.9.0/labstep/service/config.py
+-rwxr-xr-x   0 barneywalker   (501) staff       (20)     4255 2021-12-07 13:37:45.000000 labstep-3.9.0/labstep/service/helpers.py
+-rwxr-xr-x   0 barneywalker   (501) staff       (20)     1835 2021-12-08 11:59:18.000000 labstep-3.9.0/labstep/service/htmlExport.py
+-rwxr-xr-x   0 barneywalker   (501) staff       (20)      763 2021-12-08 11:59:18.000000 labstep-3.9.0/labstep/service/htmlToPDF.py
+-rwxr-xr-x   0 barneywalker   (501) staff       (20)      949 2021-01-15 18:28:50.000000 labstep-3.9.0/labstep/service/htmlToProseMirror.py
+-rwxr-xr-x   0 barneywalker   (501) staff       (20)      698 2021-10-18 11:49:26.000000 labstep-3.9.0/labstep/service/jupyter.py
+-rwxr-xr-x   0 barneywalker   (501) staff       (20)      503 2021-09-01 17:37:18.000000 labstep-3.9.0/labstep/service/ping.py
+-rwxr-xr-x   0 barneywalker   (501) staff       (20)     2181 2021-11-26 11:58:12.000000 labstep-3.9.0/labstep/service/request.py
+drwxr-xr-x   0 barneywalker   (501) staff       (20)        0 2021-12-08 17:42:14.723110 labstep-3.9.0/labstep.egg-info/
+-rw-r--r--   0 barneywalker   (501) staff       (20)      921 2021-12-08 17:42:14.000000 labstep-3.9.0/labstep.egg-info/PKG-INFO
+-rw-r--r--   0 barneywalker   (501) staff       (20)     4552 2021-12-08 17:42:14.000000 labstep-3.9.0/labstep.egg-info/SOURCES.txt
+-rw-r--r--   0 barneywalker   (501) staff       (20)        1 2021-12-08 17:42:14.000000 labstep-3.9.0/labstep.egg-info/dependency_links.txt
+-rw-r--r--   0 barneywalker   (501) staff       (20)        1 2020-11-18 11:42:18.000000 labstep-3.9.0/labstep.egg-info/not-zip-safe
+-rw-r--r--   0 barneywalker   (501) staff       (20)       69 2021-12-08 17:42:14.000000 labstep-3.9.0/labstep.egg-info/requires.txt
+-rw-r--r--   0 barneywalker   (501) staff       (20)        8 2021-12-08 17:42:14.000000 labstep-3.9.0/labstep.egg-info/top_level.txt
+-rw-r--r--   0 barneywalker   (501) staff       (20)       38 2021-12-08 17:42:14.763756 labstep-3.9.0/setup.cfg
+-rw-r--r--   0 barneywalker   (501) staff       (20)      793 2021-11-26 11:57:06.000000 labstep-3.9.0/setup.py
```

### Comparing `labstep-3.8.0/PKG-INFO` & `labstep-3.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labstep
-Version: 3.8.0
+Version: 3.9.0
 Summary: Python SDK for working with the Labstep API
 Home-page: http://github.com/Labstep/labstepPy
 Author: Barney Walker
 Author-email: barney@labstep.com
 License: MIT
 Platform: UNKNOWN
```

### Comparing `labstep-3.8.0/README.rst` & `labstep-3.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `labstep-3.8.0/labstep/converter/htmlToProseMirror.py` & `labstep-3.9.0/labstep/converter/htmlToProseMirror.py`

 * *Files identical despite different names*

### Comparing `labstep-3.8.0/labstep/entities/autoshare/model.py` & `labstep-3.9.0/labstep/entities/autoshare/model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
 
 from labstep.generic.entity.model import Entity
+from labstep.constants import UNSPECIFIED
 
 
 class Autoshare(Entity):
     """
     Represents an Autosharing rule on Labstep.
     """
 
     __entityName__ = "security-policy"
     __isLegacy__ = True
 
     def edit(
         self,
-        experiment_sharing=None,
-        protocol_sharing=None,
-        resource_sharing=None,
+        experiment_sharing=UNSPECIFIED,
+        protocol_sharing=UNSPECIFIED,
+        resource_sharing=UNSPECIFIED,
         extraParams={},
     ):
         """
         Edit an autosharing policy.
 
         Parameters
         ----------
@@ -54,15 +55,15 @@
             sharelink = experiment.getSharelink()
 
             # Edit the sharelink
             sharelink.edit(type='view')
         """
         from labstep.generic.entity.repository import editEntity
 
-        options = {True: "edit", False: "none", None: None}
+        options = {True: "edit", False: "none", UNSPECIFIED: UNSPECIFIED}
 
         fields = {
             "experiment_workflow": options[experiment_sharing],
             "protocol_collection": options[protocol_sharing],
             "resource": options[resource_sharing],
             **extraParams,
         }
```

### Comparing `labstep-3.8.0/labstep/entities/collection/model.py` & `labstep-3.9.0/labstep/entities/collection/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
 
 from labstep.generic.entity.model import Entity
 from labstep.service.helpers import getTime
+from labstep.constants import UNSPECIFIED
 
 
 class Collection(Entity):
     """
     Represents a Collection on Labstep.
 
     To see all attributes of a collection run
@@ -19,15 +20,15 @@
         print(my_collection.name)
         print(my_collection.id)
     """
 
     __entityName__ = "folder"
     __hasParentGroup__ = True
 
-    def edit(self, name=None, extraParams={}):
+    def edit(self, name=UNSPECIFIED, extraParams={}):
         """
         Edit the name of an existing Collection.
 
         Parameters
         ----------
         name (str)
             The new name of the Collection.
```

### Comparing `labstep-3.8.0/labstep/entities/collection/repository.py` & `labstep-3.9.0/labstep/entities/collection/repository.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 
 import json
 from labstep.entities.collection.model import Collection
 from labstep.service.request import requestService
 from labstep.service.helpers import url_join, getHeaders
 from labstep.service.config import configService
 from labstep.generic.entity.repository import getEntities, editEntity, newEntity
+from labstep.constants import UNSPECIFIED
 
 
 def getCollections(
-    user, count=1000, type=None, search_query=None, extraParams={}
+    user, count=1000, type=UNSPECIFIED, search_query=UNSPECIFIED, extraParams={}
 ):
     types = {
         "experiment": "experiment_workflow",
         "protocol": "protocol_collection",
         None: None,
     }
     params = {"search_query": search_query, "type": types[type], **extraParams}
```

### Comparing `labstep-3.8.0/labstep/entities/comment/model.py` & `labstep-3.9.0/labstep/entities/comment/model.py`

 * *Files identical despite different names*

### Comparing `labstep-3.8.0/labstep/entities/comment/repository.py` & `labstep-3.9.0/labstep/entities/comment/repository.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
 
 from labstep.entities.comment.model import Comment
 from labstep.generic.entity.repository import getEntities, newEntity, editEntity, exportEntity
 import labstep.entities.file.repository as fileRepository
 from labstep.service.helpers import handleString
+from labstep.constants import UNSPECIFIED
 
 
 def getComments(entity, count=100, extraParams={}):
 
     if hasattr(entity, 'thread') is False:
         entity.update()
 
@@ -23,41 +24,41 @@
         "parent_thread_id": entity.thread["id"],
         "search": None,
         **extraParams,
     }
     return getEntities(entity.__user__, Comment, count, params)
 
 
-def addComment(entity, body, fileId=None, extraParams={}):
+def addComment(entity, body, fileId=UNSPECIFIED, extraParams={}):
     if hasattr(entity, 'thread') is False:
         raise Exception('You cannot add a comment to this entity')
 
     threadId = entity.thread["id"]
 
     params = {
         "body": handleString(body),
         "parent_thread_id": threadId,
-        "file_id": [[fileId]] if fileId is not None else None,
+        "file_id": [[fileId]] if fileId is not UNSPECIFIED else UNSPECIFIED,
         **extraParams,
     }
 
     entity.thread["comment_count"] += 1
 
     return newEntity(entity.__user__, Comment, params)
 
 
 def addCommentWithFile(entity, body, filepath, extraParams={}):
-    if filepath is not None:
+    if filepath is not UNSPECIFIED:
         fileId = fileRepository.newFile(entity.__user__, filepath).id
     else:
-        fileId = None
+        fileId = UNSPECIFIED
     return addComment(entity, body, fileId=fileId, extraParams=extraParams)
 
 
-def editComment(comment, body=None, extraParams={}):
+def editComment(comment, body=UNSPECIFIED, extraParams={}):
     params = {"body": body, **extraParams}
     return editEntity(comment, params)
 
 
 def exportComment(comment, rootPath):
     commentDir = exportEntity(
         comment, rootPath)
```

### Comparing `labstep-3.8.0/labstep/entities/device/model.py` & `labstep-3.9.0/labstep/entities/device/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Author: Barney Walker <barney@labstep.com>
 
 from labstep.entities.deviceData.model import DeviceData
 from labstep.generic.entityWithMetadata.model import EntityWithMetadata
 from labstep.generic.entityWithSharing.model import EntityWithSharing
 from labstep.generic.entityWithComments.model import EntityWithComments
 from labstep.service.helpers import getTime
+from labstep.constants import UNSPECIFIED
 
 
 TYPE_DEFAULT = "default"
 TYPE_NUMERIC = "numeric"
 TYPE_FILE = "file"
 
 FIELD_TYPES = {
@@ -45,15 +46,15 @@
     ::
         print(my_device.name)
         print(my_device.id)
     """
 
     __entityName__ = "device"
 
-    def edit(self, name=None, extraParams={}):
+    def edit(self, name=UNSPECIFIED, extraParams={}):
         """
         Edit an existing Device.
 
         Parameters
         ----------
         name (str)
             The new name of the Device.
@@ -89,19 +90,19 @@
 
         return deviceRepository.editDevice(self, deleted_at=getTime())
 
     def addMetadata(
         self,
         fieldName,
         fieldType="default",
-        value=None,
-        date=None,
-        number=None,
-        unit=None,
-        filepath=None,
+        value=UNSPECIFIED,
+        date=UNSPECIFIED,
+        number=UNSPECIFIED,
+        unit=UNSPECIFIED,
+        filepath=UNSPECIFIED,
         extraParams={},
     ):
         """
         Add Metadata to a Device.
 
         Parameters
         ----------
@@ -166,15 +167,15 @@
             metadatas = my_device.getMetadata()
             metadatas[0].attributes()
         """
         import labstep.entities.metadata.repository as metadataRepository
 
         return metadataRepository.getMetadata(self)
 
-    def getData(self, count=100, search_query=None, extraParams={}):
+    def getData(self, count=100, search_query=UNSPECIFIED, extraParams={}):
         """
         Retrieve a list of the data sent by an device.
 
         Parameters
         ----------
         count (int)
             The total count of data points to return.
@@ -194,18 +195,18 @@
                   "device_id": self.id, **extraParams}
         return getEntities(self.__user__, DeviceData, count, params)
 
     def addData(
         self,
         fieldName,
         fieldType="text",
-        text=None,
-        number=None,
-        unit=None,
-        filepath=None,
+        text=UNSPECIFIED,
+        number=UNSPECIFIED,
+        unit=UNSPECIFIED,
+        filepath=UNSPECIFIED,
         extraParams={},
     ):
         """
         Send new data from the Device.
 
         Parameters
         ----------
@@ -239,23 +240,23 @@
         from labstep.generic.entity.repository import newEntity
         from labstep.entities.file.repository import newFile
 
         if fieldType not in FIELD_TYPES:
             msg = "Not a supported data type '{}'".format(fieldType)
             raise ValueError(msg)
 
-        if filepath is not None:
+        if filepath is not UNSPECIFIED:
             file_id = newFile(self.__user__, filepath).id
         else:
-            file_id = None
+            file_id = UNSPECIFIED
 
         allowedFieldsForType = set(ALLOWED_FIELDS[FIELD_TYPES[fieldType]])
         fields = {"value": text, "number": number,
                   "unit": unit, "file_id": file_id}
-        fields = {k: v for k, v in fields.items() if v}
+        fields = {k: v for k, v in fields.items() if v is not UNSPECIFIED}
         fields = set(fields.keys())
         violations = fields - allowedFieldsForType
         if violations:
             msg = "Unallowed fields [{}] for type {}".format(
                 ",".join(violations), fieldType
             )
             raise ValueError(msg)
```

### Comparing `labstep-3.8.0/labstep/entities/device/repository.py` & `labstep-3.9.0/labstep/entities/workspace/repository.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
 
-from labstep.entities.device.model import Device
+from labstep.entities.workspace.model import Workspace
 import labstep.generic.entity.repository as entityRepository
+from labstep.constants import UNSPECIFIED
 
 
-def getDevice(user, device_id):
-    return entityRepository.getEntity(user, Device, id=device_id)
+def getWorkspace(user, workspace_id):
+    return entityRepository.getEntity(user, Workspace, id=workspace_id)
 
 
-def getDevices(user, count=100, search_query=None, extraParams={}):
-    params = {"search_query": search_query, **extraParams}
-    return entityRepository.getEntities(user, Device, count, params)
+def getWorkspaces(user, count=100, search_query=UNSPECIFIED, extraParams={}):
+    params = {"name": search_query, **extraParams}
+    return entityRepository.getEntities(user, Workspace, count, params)
 
 
-def newDevice(user, name, extraParams={}):
+def newWorkspace(user, name, extraParams={}):
     params = {"name": name, **extraParams}
-    return entityRepository.newEntity(user, Device, params)
+    return entityRepository.newEntity(user, Workspace, params)
 
 
-def editDevice(device, name=None, deleted_at=None, extraParams={}):
+def editWorkspace(workspace, name=UNSPECIFIED, deleted_at=UNSPECIFIED, extraParams={}):
     params = {"name": name, "deleted_at": deleted_at, **extraParams}
-    return entityRepository.editEntity(device, params)
+    return entityRepository.editEntity(workspace, params)
```

### Comparing `labstep-3.8.0/labstep/entities/deviceData/model.py` & `labstep-3.9.0/labstep/entities/deviceData/model.py`

 * *Files identical despite different names*

### Comparing `labstep-3.8.0/labstep/entities/experiment/model.py` & `labstep-3.9.0/labstep/entities/experimentProtocol/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,539 +1,476 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
 from deprecated import deprecated
-from labstep.generic.entityPrimary.model import EntityPrimary
+from labstep.entities.file.model import File
+from labstep.generic.entity.model import Entity
 from labstep.generic.entityList.model import EntityList
-from labstep.entities.experimentProtocol.model import ExperimentProtocol
-from labstep.entities.experimentMaterial.model import ExperimentMaterial
+from labstep.entities.experimentStep.model import ExperimentStep
 from labstep.entities.experimentTable.model import ExperimentTable
-from labstep.entities.experimentSignature.model import ExperimentSignature
-from labstep.service.helpers import getTime
+from labstep.entities.experimentTimer.model import ExperimentTimer
+import labstep.entities.file.repository as fileRepository
+import labstep.entities.experimentMaterial.repository as experimentMaterialRepository
+from labstep.constants import UNSPECIFIED
 
 
-class Experiment(EntityPrimary):
-    """
-    Represents an Experiment on Labstep.
+class ExperimentProtocol(Entity):
+    __entityName__ = "experiment"
 
-    To see all attributes of an experiment run
-    ::
-        print(my_experiment)
-
-    Specific attributes can be inspected via dot notation like so...
-    ::
-        print(my_experiment.name)
-        print(my_experiment.id)
-    """
-
-    __entityName__ = "experiment-workflow"
-
-    def __init__(self, data, user):
-        super().__init__(data, user)
-        if "root_experiment" in data:
-            self.root_experiment = ExperimentProtocol(
-                data['root_experiment'], user)
-
-    def edit(self, name=None, entry=None, started_at=None, extraParams={}):
+    def edit(
+        self, name=UNSPECIFIED, body=UNSPECIFIED, started_at=UNSPECIFIED, ended_at=UNSPECIFIED, extraParams={}
+    ):
         """
-        Edit an existing Experiment.
+        Edit an existing ExperimentProtocol.
 
         Parameters
         ----------
         name (str)
-            The new name of the Experiment.
-        entry (obj)
-            A JSON object representing the state of the Experiment Entry.
+            The new name of the ExperimentProtocol.
+        body (dict)
+            A JSON object representing the new body of the ExperimentProtocol.
         started_at (str)
-            The start date of the Experiment
+            The date the ExperimentProtocol was started
+            in the format of "YYYY-MM-DD HH:MM".
+        ended_at (str)
+            The date the ExperimentProtocol was finished
             in the format of "YYYY-MM-DD HH:MM".
 
         Returns
         -------
-        :class:`~labstep.entities.experiment.model.Experiment`
-            An object representing the edited Experiment.
+        :class:`~labstep.entities.experimentProtocol.model.ExperimentProtocol`
+            An object representing the edited ExperimentProtocol.
 
         Example
         -------
         ::
 
             my_experiment = user.getExperiment(17000)
-            my_experiment.edit(name='A New Experiment Name',
+            protocols = my_experiment.getProtocols()
+            protocols[0].edit(name='A New Experiment Name',
                                started_at='2018-06-06 12:05')
         """
-        import labstep.entities.experiment.repository as experimentRepository
-
-        return experimentRepository.editExperiment(
-            self, name=name, entry=entry, started_at=started_at, extraParams=extraParams
-        )
-
-    def delete(self):
-        """
-        Delete an existing Experiment.
-
-        Example
-        -------
-        ::
-
-            my_experiment = user.getExperiment(17000)
-            my_experiment.delete()
-        """
-        import labstep.entities.experiment.repository as experimentRepository
+        import labstep.generic.entity.repository as entityRepository
 
-        return experimentRepository.editExperiment(self, deleted_at=getTime())
+        fields = {
+            "name": name,
+            "state": body,
+            "started_at": started_at,
+            "ended_at": ended_at,
+            **extraParams,
+        }
+        return entityRepository.editEntity(self, fields)
 
-    def getEntry(self):
-        """
-        Returns a JSON document representing the entry for the experiment.
+    def getExperiment(self):
 
-        Example
-        -------
-        ::
+        from labstep.entities.experiment.repository import getExperiment
 
-            my_experiment = user.getExperiment(17000)
-            print(my_experiment.getEntry())
-        """
-        import labstep.generic.entity.repository as entityRepository
+        if hasattr(self, 'experiment_workflow') is False:
+            self.update()
 
-        return entityRepository.getEntity(
-            self.__user__, ExperimentProtocol, self.root_experiment.id
-        ).state
+        return getExperiment(self.__user__, self.experiment_workflow['id'])
 
-    def addProtocol(self, protocol):
+    def getBody(self):
         """
-        Add a Labstep Protocol to a Labstep Experiment.
-
-        Parameters
-        ----------
-        protocol (Protocol)
-            The :class:`~labstep.entities.protocol.model.Protocol` to attach.
-
-        Returns
-        -------
-        :class:`~labstep.entities.protocol.model.Protocol`
-            An object representing the Protocol attached to the Experiment.
+        Returns the body of the protocol as a JSON document
 
         Example
         -------
         ::
 
-            # Get an Experiment
             my_experiment = user.getExperiment(17000)
-
-            # Get a Protocol
-            my_protocol = user.getProtocol(10000)
-
-            # Attach the Protocol to the Experiment
-            my_experiment.addProtocol(my_protocol)
+            protocols = my_experiment.getProtocols()
+            protocols[0].getBody()
         """
-        import labstep.entities.experiment.repository as experimentRepository
+        self.update()
+        return getattr(self, "state", None)
 
-        return experimentRepository.addProtocolToExperiment(self, protocol)
-
-    def getProtocols(self, count=100):
+    def getMaterials(self, count=100, extraParams={}):
         """
-        Retrieve the Protocols attached to this Labstep Experiment.
+        Returns a list of the materials in a Protocol within an Experiment.
 
         Returns
         -------
-        List[:class:`~labstep.entities.experimentProtocol.model.ExperimentProtocol`]
-            List of the Protocols attached to the Experiment.
+        List[:class:`~labstep.entities.experimentMaterial.model.ExperimentMaterial`]
+            List of the materials in an Experiment's Protocol.
 
         Example
         -------
         ::
 
-            entity = user.getExperiment(17000)
-            protocols = entity.getProtocols()
-            protocols[0].attributes()
+            experiment = user.getExperiment(17000)
+            exp_protocol = experiment.getProtocols()[0]
+            exp_protocol_materials = exp_protocol.getMaterials()
+            exp_protocol_materials[0].attributes()
         """
-        import labstep.generic.entity.repository as entityRepository
 
-        return entityRepository.getEntities(
-            self.__user__,
-            ExperimentProtocol,
-            count,
-            {"is_root": 0, "experiment_workflow_id": self.id},
-        )
+        return experimentMaterialRepository.getExperimentMaterials(self.__user__,
+                                                                   experiment_id=self.id, count=count, extraParams=extraParams)
 
-    def addDataField(
+    def addMaterial(
         self,
-        fieldName,
-        fieldType="default",
-        value=None,
-        date=None,
-        number=None,
-        unit=None,
-        filepath=None,
+        name=UNSPECIFIED,
+        amount=UNSPECIFIED,
+        units=UNSPECIFIED,
+        resource_id=UNSPECIFIED,
+        resource_item_id=UNSPECIFIED,
         extraParams={},
     ):
         """
-        Add Data Fields to a Labstep Experiment.
+        Add a new material to the ExperimentProtocol.
 
         Parameters
         ----------
-        fieldName (str)
-            The name of the field.
-        fieldType (str)
-            The Metadata field type. Options are: "default", "date",
-            "numeric", or "file". The "default" type is "Text".
-        value (str)
-            The value accompanying the fieldName entry.
-        date (str)
-            The date and time accompanying the fieldName entry. Must be
-            in the format of "YYYY-MM-DD HH:MM".
-        number (float)
-            The quantity.
-        unit (str)
-            The unit accompanying the number entry.
-        filepath (str)
-            Local path to the file to upload for type 'file'
+        name (str)
+            The name of the material to add.
+        amount (str)
+            The amount used.
+        units (str)
+            The units for the amount.
+        resource_id (int)
+            The id of the :class:`~labstep.entities.resource.model.Resource` used.
+        resource_item_id (ResourceItem)
+            The id of the specific
+            :class:`~labstep.entities.resource.model.ResourceItem` used.
 
         Returns
         -------
-        :class:`~labstep.entities.experimentDataField.model.ExperimentDataField`
-            An object representing the new Labstep Data Field.
+        :class:`~labstep.entities.experimentMaterial.model.ExperimentMaterial`
+            The newly added material entity.
 
         Example
         -------
         ::
 
             experiment = user.getExperiment(17000)
-            dataField = experiment.addDataField("Refractive Index",
-                                               value="1.73")
+            resource = user.getResources(search_query='Sample A')[0]
+            experiment.addMaterial(name='Sample A', amount='2', units='ml',
+                                 resource_id=resource.id)
         """
-        return self.root_experiment.addDataField(
-            fieldName=fieldName,
-            fieldType=fieldType,
-            value=value,
-            date=date,
-            number=number,
-            unit=unit,
-            filepath=filepath,
-            extraParams=extraParams,
-        )
+        return experimentMaterialRepository.newExperimentMaterial(self.__user__,
+                                                                  experiment_id=self.id,
+                                                                  name=name,
+                                                                  amount=amount,
+                                                                  units=units,
+                                                                  resource_id=resource_id,
+                                                                  resource_item_id=resource_item_id,
+                                                                  extraParams=extraParams)
 
-    def getDataFields(self):
+    def addSteps(self, N):
         """
-        Retrieve the Data Fields of a Protocol within an Experiment.
+        Add steps to a Protocol within an Experiment
 
-        Returns
-        -------
-        :class:`~labstep.entities.experimentDataField.model.ExperimentDataField`
-            An array of objects representing Data Fields
-            on a Protocol within an Experiment.
+        Parameters
+        ----------
+        N (int)
+            The number of steps to add.
 
         Example
         -------
         ::
 
             experiment = user.getExperiment(17000)
             exp_protocol = experiment.getProtocols()[0]
-            dataFields = exp_protocol.getDataFields()
-        """
-        return self.root_experiment.getDataFields()
-
-    def getSignatures(self):
+            exp_protocol_steps = exp_protocol.addSteps(5)
         """
-        Retrieve a list of signatures added to the experiment
+        import labstep.generic.entity.repository as entityRepository
 
-        Returns
-        -------
-        List[:class:`~labstep.entities.experimentSignature.model.ExperimentSignature`]
-            List of the signatures added to the Experiment
-        """
-        exp = self.__user__.getExperiment(self.id)
-        return EntityList(exp.signatures, ExperimentSignature, self.__user__)
+        steps = [{"experiment_id": self.id}] * N
+        return entityRepository.newEntities(self.__user__, ExperimentStep, steps)
 
-    def addSignature(self, statement=None, lock=False):
+    def addTable(self, name=UNSPECIFIED, data=UNSPECIFIED):
         """
-        Add a signature to experiment
+        Add a new table to a Protocol within an Experiment.
 
         Parameters
         ----------
-        statement (str)
-            Statement describing the signature.
-        lock (boolean)
-            Whether to lock the experiment against further edits.
+        name (str)
+            The name of the table.
+        data (json)
+            The data of the table in json format.
 
         Returns
         -------
-        :class:`~labstep.entities.experimentSignature.model.ExperimentSignature`
-            The signature that has been added
-        """
-        import labstep.generic.entity.repository as entityRepository
-
-        params = {
-            "statement": statement,
-            "is_lock": int(lock),
-            "experiment_workflow_id": self.id,
-        }
-        return entityRepository.newEntity(self.__user__, ExperimentSignature, params)
-
-    def getSignatureRequests(self):
-        """
-        Returns a list of pending signature requests for the experiment.
+        :class:`~labstep.entities.experimentTable.model.ExperimentTable`
+            The newly added table entity.
 
-        Returns
+        Example
         -------
-        List[:class:`~labstep.entities.experimentSignatureRequest.model.ExperimentSignatureRequest`]
-        """
-        import labstep.entities.experimentSignatureRequest.repository as experimentSignatureRequestRepository
-
-        return experimentSignatureRequestRepository.getExperimentSignatureRequests(self.__user__, self.id)
-
-    def requestSignature(self, user_id, message=None):
-        """
-        Request a signature from another user in the workspace
-
-        Parameters
-        ----------
-
-        user_id (int)
-            Id of the user you are requesting a signature from
+        ::
 
-        message (str)
-            Optional message to include in signature request email
+            data = {
+                "rowCount": 12,
+                "columnCount": 12,
+                "colHeaderData": {},
+                "data": {
+                    "dataTable": {
+                        0: {
+                            0: {
+                                "value": 'Cell A1'
+                            },
+                            1: {
+                                "value": 'Cell B1'
+                            }
+                        }
+                    }
+                }
+            }
 
+            experiment = user.getExperiment(17000)
+            exp_protocol = experiment.getProtocols()[0]
+            exp_protocol.addTable(name='Calibration', data=data)
         """
-        import labstep.entities.experimentSignatureRequest.repository as experimentSignatureRequestRepository
+        import labstep.generic.entity.repository as entityRepository
 
-        return experimentSignatureRequestRepository.newExperimentSignatureRequest(self.__user__, self.id, user_id=user_id, message=message)
+        params = {"experiment_id": self.id, "name": name, "data": data}
+        return entityRepository.newEntity(self.__user__, ExperimentTable, params)
 
-    def getMaterials(self):
+    def getSteps(self):
         """
-        Returns a list of the materials in the Experiment.
+        Returns a list of the steps in a Protocol within an Experiment.
 
         Returns
         -------
-        List[:class:`~labstep.entities.experimentMaterial.model.ExperimentMaterial`]
-            List of the materials in an Experiment.
+        List[:class:`~labstep.entities.experimentStep.model.ExperimentStep`]
+            List of the steps in an Experiment's Protocol.
 
         Example
         -------
         ::
 
             experiment = user.getExperiment(17000)
-            exp_materials = experiment.getMaterials()
-            print(exp_materials[0])
+            exp_protocol = experiment.getProtocols()[0]
+            exp_protocol_steps = exp_protocol.getSteps()
+            exp_protocol_steps[0].attributes()
         """
-        return self.root_experiment.getMaterials()
+        self.update()
+        steps = self.experiment_steps
+        return EntityList(steps, ExperimentStep, self.__user__)
 
-    def addMaterial(
-        self,
-        name=None,
-        amount=None,
-        units=None,
-        resource_id=None,
-        resource_item_id=None,
-        extraParams={},
-    ):
+    def addTimer(self, name=UNSPECIFIED, hours=UNSPECIFIED, minutes=UNSPECIFIED, seconds=UNSPECIFIED):
         """
-        Add a new material to the Experiment.
+        Add a new timer to a Protocol within an Experiment.
 
         Parameters
         ----------
         name (str)
-            The name of the material to add.
-        amount (str)
-            The amount used.
-        units (str)
-            The units for the amount.
-        resource_id (int)
-            The id of the :class:`~labstep.entities.resource.model.Resource` used.
-        resource_item_id (ResourceItem)
-            The id of the specific
-            :class:`~labstep.entities.resource.model.ResourceItem` used.
+            The name of the timer.
+        hours (int)
+            The hours of the timer.
+        minutes (int)
+            The minutes of the timer.
+        seconds (int)
+            The seconds of the timer.
 
         Returns
         -------
-        :class:`~labstep.entities.experimentMaterial.model.ExperimentMaterial`
-            The newly added material entity.
+        :class:`~labstep.entities.ExperimentTimer.model.ExperimentTimer`
+            The newly added timer entity.
 
         Example
         -------
         ::
 
             experiment = user.getExperiment(17000)
-            resource = user.getResources(search_query='Sample A')[0]
-            experiment.addMaterial(name='Sample A', amount='2', units='ml',
-                                 resource_id=resource.id)
+            exp_protocol = experiment.getProtocols()[0]
+            exp_protocol.addTimer(name='Refluxing', hours='4', minutes='30')
         """
-        return self.root_experiment.addMaterial(name=name,
-                                                resource_id=resource_id,
-                                                resource_item_id=resource_item_id,
-                                                amount=amount,
-                                                units=units,
-                                                extraParams=extraParams)
+        import labstep.generic.entity.repository as entityRepository
 
-    def addToCollection(self, collection_id):
-        """
-        Add the experiment to a collection.
+        params = {
+            "experiment_id": self.id,
+            "name": name,
+            "hours": hours,
+            "minutes": minutes,
+            "seconds": seconds,
+        }
+        return entityRepository.newEntity(self.__user__, ExperimentTimer, params)
 
-        Parameters
-        ----------
-        collection_id (int)
-            The id of the collection to add to
+    def getTables(self):
+        """
+        Returns a list of the tables in a Protocol within an Experiment.
 
         Returns
         -------
-        None
-        """
-        import labstep.entities.collection.repository as collectionRepository
+        List[:class:`~labstep.entities.experimentTable.model.ExperimentTable`]
+            List of the tables in an Experiment's Protocol.
 
-        return collectionRepository.addToCollection(self, collection_id=collection_id)
+        Example
+        -------
+        ::
 
-    def getCollections(self):
-        """
-        Returns the list of collections the protocol is in.
+            experiment = user.getExperiment(17000)
+            exp_protocol = experiment.getProtocols()[0]
+            exp_protocol_tables = exp_protocol.getTables()
+            exp_protocol_tables[0].attributes()
         """
-        import labstep.entities.collection.repository as collectionRepository
+        self.update()
+        tables = self.experiment_tables
+        return EntityList(tables, ExperimentTable, self.__user__)
 
-        return collectionRepository.getAttachedCollections(self)
-
-    def removeFromCollection(self, collection_id):
+    def getTimers(self):
         """
-        Remove the experiment from a collection.
+        Returns a list of the timers in a Protocol within an Experiment.
 
-        Parameters
-        ----------
-        collection_id (int)
-            The id of the collection to remove from
+        Returns
+        -------
+        List[:class:`~labstep.entities.experimentTimer.model.ExperimentTimer`]
+            List of the timers in an Experiment's Protocol.
 
-        """
-        import labstep.entities.collection.repository as collectionRepository
+        Example
+        -------
+        ::
 
-        return collectionRepository.removeFromCollection(self, collection_id)
+            experiment = user.getExperiment(17000)
+            exp_protocol = experiment.getProtocols()[0]
+            exp_protocol_timers = exp_protocol.getTimers()
+            exp_protocol_timers[0].attributes()
+        """
+        self.update()
+        timers = self.experiment_timers
+        return EntityList(timers, ExperimentTimer, self.__user__)
 
-    def getTables(self):
+    def getDataFields(self):
         """
-        Returns a list of the tables in the entry of an Experiment.
+        Retrieve the Data Fields of a Protocol within an Experiment.
 
         Returns
         -------
-        List[:class:`~labstep.entities.experimentTable.model.ExperimentTable`]
-            List of the tables in an Experiment entry
+        :class:`~labstep.entities.experimentDataField.model.ExperimentDataField`
+            An array of objects representing the Labstep
+            Data Fields on a Protocol within an Experiment.
 
         Example
         -------
         ::
 
             experiment = user.getExperiment(17000)
-            tables = experiment.getTables()
+            exp_protocol = experiment.getProtocols()[0]
+            metadata = exp_protocol.getDataFields()
         """
-        return self.root_experiment.getTables()
+        import labstep.entities.experimentDataField.repository as experimentDataFieldRepository
 
-    def addTable(self, name=None, data=None):
+        return experimentDataFieldRepository.getDataFields(self)
+
+    def addDataField(
+        self,
+        fieldName,
+        fieldType="default",
+        value=UNSPECIFIED,
+        date=UNSPECIFIED,
+        number=UNSPECIFIED,
+        unit=UNSPECIFIED,
+        filepath=UNSPECIFIED,
+        extraParams={},
+    ):
         """
-        Add a new table to an Experiment.
+        Add a Data Field to a Protocol within an Experiment.
 
         Parameters
         ----------
-        name (str)
-            The name of the table.
-        data (json)
-            The data of the table in json format.
+        fieldName (str)
+            The name of the field.
+        fieldType (str)
+            The field type. Options are: "default", "date",
+            "quantity", or "number". The "default" type is "Text".
+        value (str)
+            The value accompanying the fieldName entry.
+        date (str)
+            The date and time accompanying the fieldName entry. Must be
+            in the format of "YYYY-MM-DD HH:MM".
+        number (float)
+            The quantity.
+        unit (str)
+            The unit accompanying the number entry.
+        filepath (str)
+            Local path to the file to upload for type 'file'
 
         Returns
         -------
-        :class:`~labstep.entities.experimentTable.model.ExperimentTable`
-            The newly added table entity.
+        :class:`~labstep.entities.metadata.model.Metadata`
+            An object representing the new Labstep Data Field.
 
         Example
         -------
         ::
 
-            data = {
-                "rowCount": 12,
-                "columnCount": 12,
-                "colHeaderData": {},
-                "data": {
-                    "dataTable": {
-                        0: {
-                            0: {
-                                "value": 'Cell A1'
-                            },
-                            1: {
-                                "value": 'Cell B1'
-                            }
-                        }
-                    }
-                }
-            }
-
             experiment = user.getExperiment(17000)
-            experiment.addTable(name='Calibration', data=data)
+            experiment_protocol = experiment.getProtocols()[0]
+            dataField = experiment_protocol.addDataField(
+                "Refractive Index", value="1.73"
+            )
         """
-        return self.root_experiment.addTable(name=name, data=data)
+        import labstep.entities.experimentDataField.repository as experimentDataFieldRepository
 
-    def addFile(self, filepath=None, rawData=None):
+        return experimentDataFieldRepository.addDataFieldTo(
+            self,
+            fieldName=fieldName,
+            fieldType=fieldType,
+            value=value,
+            date=date,
+            number=number,
+            unit=unit,
+            filepath=filepath,
+            extraParams=extraParams,
+        )
+
+    def addFile(self, filepath=UNSPECIFIED, rawData=UNSPECIFIED):
         """
-        Add a file to an experiment entry.
-        (Only use for files to be embedded in the body of the entry)
+        Add a file to an Experiment Protocol.
 
         Parameters
         ----------
         filepath (str)
             The path to the file to upload.
         rawData (bytes)
-            Raw bytes data to upload as file
+            Raw data to upload as a file.
 
         Returns
         -------
         :class:`~labstep.file.File`
             The newly added file entity.
 
         Example
         -------
         ::
 
             experiment = user.getExperiment(17000)
-            experiment.addFile(filepath='./my_file.csv')
+            experiment_protocol = experiment.getProtocols()[0]
+            file = experiment_protocol.addFile(filepath='./my_file.csv')
         """
-        return self.root_experiment.addFile(filepath, rawData)
+        params = {'experiment_id': self.id}
+        return fileRepository.newFile(self.__user__, filepath=filepath, rawData=rawData, extraParams=params)
 
     def getFiles(self):
         """
-        Returns a list of the files in a experiment entry.
-        (Only includes the files embedded in the body of the entry)
+        Returns a list of the files in a Protocol.
 
         Returns
         -------
         List[:class:`~labstep.file.File`]
-            List of the files in a experiment.
-
-        Example
-        -------
-        ::
-
-            experiment = user.getExperiment(17000)
-            experiment_files = experiment.getFiles()
-        """
-        return self.root_experiment.getFiles()
-
-    def export(self, path):
-        """
-        Export the experiment to the directory specified. 
-
-        Parameters
-        -------
-        path (str)
-            The path to the directory to save the experiment.
+            List of the files in a Protocol.
 
         Example
         -------
         ::
 
             experiment = user.getExperiment(17000)
-            experiment.export('/my_folder')
+            experiment_protocol = experiment.getProtocols()[0]
+            filess = experiment_protocol.getFiles()
         """
-        import labstep.entities.experiment.repository as experimentRepository
-
-        return experimentRepository.exportExperiment(self, path)
+        self.update()
+        files = self.files
+        return EntityList(files, File, self.__user__)
+
+    def export(self, rootPath, folderName=UNSPECIFIED):
+        import labstep.entities.experimentProtocol.repository as experimentProtocolRepository
+        return experimentProtocolRepository.exportExperimentProtocol(self, rootPath, folderName=folderName)
 
-    @deprecated(version='3.3.2', reason="You should use experiment.addDataField instead")
+    @deprecated(version='3.3.2', reason="You should use experimentProtocol.addDataField instead")
     def addDataElement(self, *args, **kwargs):
+
         return self.addDataField(*args, **kwargs)
 
-    @deprecated(version='3.3.2', reason="You should use experiment.getDataFields instead")
+    @deprecated(version='3.3.2', reason="You should use experimentProtocol.getDataFields instead")
     def getDataElements(self):
+
         return self.getDataFields()
```

### Comparing `labstep-3.8.0/labstep/entities/experiment/repository.py` & `labstep-3.9.0/labstep/entities/experiment/repository.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,48 +4,49 @@
 
 from labstep.service.helpers import (
     handleDate,
 )
 from labstep.entities.experiment.model import Experiment, ExperimentProtocol
 import labstep.generic.entity.repository as entityRepository
 from labstep.service.htmlExport import htmlExportService
+from labstep.constants import UNSPECIFIED
 
 
 def getExperiment(user, experiment_id):
     return entityRepository.getEntity(user, Experiment, id=experiment_id)
 
 
 def getExperiments(
 
     user,
     count=100,
-    search_query=None,
-    created_at_from=None,
-    created_at_to=None,
-    tag_id=None,
-    collection_id=None,
+    search_query=UNSPECIFIED,
+    created_at_from=UNSPECIFIED,
+    created_at_to=UNSPECIFIED,
+    tag_id=UNSPECIFIED,
+    collection_id=UNSPECIFIED,
     extraParams={},
 ):
     params = {
         "search_query": search_query,
         "created_at_from": handleDate(created_at_from),
         "created_at_to": handleDate(created_at_to),
         "tag_id": tag_id,
         "folder_id": collection_id,
         **extraParams,
     }
     return entityRepository.getEntities(user, Experiment, count, params)
 
 
-def newExperiment(user, name, entry=None, extraParams={}):
+def newExperiment(user, name, entry=UNSPECIFIED, extraParams={}):
     params = {"name": name, **extraParams}
 
     experiment = entityRepository.newEntity(user, Experiment, params)
 
-    if entry is not None:
+    if entry is not UNSPECIFIED:
         experiment = experiment.edit(entry=entry)
 
     return experiment
 
 
 def addProtocolToExperiment(experiment, protocol):
     params = {
@@ -56,28 +57,28 @@
         experiment.__user__, ExperimentProtocol, params
     )
 
 
 def editExperiment(
 
     experiment,
-    name=None,
-    entry=None,
-    started_at=None,
-    deleted_at=None,
+    name=UNSPECIFIED,
+    entry=UNSPECIFIED,
+    started_at=UNSPECIFIED,
+    deleted_at=UNSPECIFIED,
     extraParams={},
 ):
     params = {
         "name": name,
         "started_at": handleDate(started_at),
         "deleted_at": deleted_at,
         **extraParams,
     }
 
-    if entry is not None:
+    if entry is not UNSPECIFIED:
         experiment.root_experiment.edit(body=entry)
         experiment.update()
 
     return entityRepository.editEntity(experiment, params)
 
 
 def exportExperiment(experiment, root_path):
```

### Comparing `labstep-3.8.0/labstep/entities/experimentDataField/model.py` & `labstep-3.9.0/labstep/entities/experimentDataField/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
 
 from labstep.generic.entityWithComments.model import EntityWithComments
 import labstep.generic.entity.repository as entityRepository
 from labstep.service.helpers import getTime
+from labstep.constants import UNSPECIFIED
 
 
 class ExperimentDataField(EntityWithComments):
     """
     Represents a single data field attached to a Labstep Experiment.
 
     To see the attributes of the data field run
@@ -20,15 +21,15 @@
         print(my_data_field.value)
         print(my_data_field.id)
     """
 
     __entityName__ = "metadata"
     __searchKey__ = 'label'
 
-    def edit(self, fieldName=None, value=None, extraParams={}):
+    def edit(self, fieldName=UNSPECIFIED, value=UNSPECIFIED, extraParams={}):
         """
         Edit the value of an existing data field.
 
         Parameters
         ----------
         fieldName (str)
             The new name of the field.
```

### Comparing `labstep-3.8.0/labstep/entities/experimentDataField/repository.py` & `labstep-3.9.0/labstep/entities/experimentDataField/repository.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from labstep.generic.entityList.model import EntityList
 from labstep.service.helpers import formatDate, handleDate, handleString
 from labstep.entities.experimentDataField.model import ExperimentDataField
 from labstep.entities.experimentProtocol.model import ExperimentProtocol
 from labstep.entities.resource.model import Resource
 from labstep.entities.resourceItem.model import ResourceItem
 from labstep.entities.file.model import File
+from labstep.constants import UNSPECIFIED
 
 
 def getDataFields(entity, count=1000, extraParams={}):
 
     params = {}
 
     if isinstance(entity, ExperimentProtocol):
@@ -39,25 +40,25 @@
 
 
 def addDataFieldTo(
 
     entity,
     fieldName,
     fieldType="default",
-    value=None,
-    date=None,
-    number=None,
-    unit=None,
-    filepath=None,
+    value=UNSPECIFIED,
+    date=UNSPECIFIED,
+    number=UNSPECIFIED,
+    unit=UNSPECIFIED,
+    filepath=UNSPECIFIED,
     extraParams={},
 ):
-    if filepath is not None:
+    if filepath is not UNSPECIFIED:
         fileId = fileRepository.newFile(entity.__user__, filepath).id
     else:
-        fileId = None
+        fileId = UNSPECIFIED
 
     params = {
         "metadata_thread_id": entity.metadata_thread["id"],
         "type": fieldType,
         "label": handleString(fieldName),
         "value": handleString(value),
         "date": handleDate(date),
@@ -66,15 +67,15 @@
         "file_id": fileId,
         **extraParams,
     }
 
     return entityRepository.newEntity(entity.__user__, ExperimentDataField, params)
 
 
-def editDataField(dataField, fieldName=None, value=None, extraParams={}):
+def editDataField(dataField, fieldName=UNSPECIFIED, value=UNSPECIFIED, extraParams={}):
     params = {
         "label": handleString(fieldName),
         "value": handleString(value),
         **extraParams
     }
     return entityRepository.editEntity(dataField, params)
```

### Comparing `labstep-3.8.0/labstep/entities/experimentMaterial/model.py` & `labstep-3.9.0/labstep/entities/experimentMaterial/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
 
 from labstep.generic.entity.model import Entity
+from labstep.constants import UNSPECIFIED
 
 
 class ExperimentMaterial(Entity):
     __entityName__ = "experiment-value"
 
     def __init__(self, data, user):
         super().__init__(data, user)
         self.amount = self.value
 
-    def edit(self, name=None, amount=None, units=None, resource_id=None, resource_item_id=None, extraParams={}):
+    def edit(self, name=UNSPECIFIED, amount=UNSPECIFIED, units=UNSPECIFIED, resource_id=UNSPECIFIED, resource_item_id=UNSPECIFIED, extraParams={}):
         """
         Edit an existing Experiment Material.
 
         Parameters
         ----------
         amount (str)
             The amount of the Experiment Material.
```

### Comparing `labstep-3.8.0/labstep/entities/experimentProtocol/model.py` & `labstep-3.9.0/labstep/entities/experiment/model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,125 +1,391 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
 from deprecated import deprecated
-from labstep.entities.file.model import File
-from labstep.generic.entity.model import Entity
+from labstep.entities.experimentLink.repository import newExperimentLink
+from labstep.generic.entityPrimary.model import EntityPrimary
 from labstep.generic.entityList.model import EntityList
-from labstep.entities.experimentStep.model import ExperimentStep
-from labstep.entities.experimentTable.model import ExperimentTable
-from labstep.entities.experimentTimer.model import ExperimentTimer
-import labstep.entities.file.repository as fileRepository
-import labstep.entities.experimentMaterial.repository as experimentMaterialRepository
+from labstep.entities.experimentProtocol.model import ExperimentProtocol
+from labstep.entities.experimentSignature.model import ExperimentSignature
+from labstep.service.helpers import getTime, handleDate
+from labstep.constants import UNSPECIFIED
 
 
-class ExperimentProtocol(Entity):
-    __entityName__ = "experiment"
+class Experiment(EntityPrimary):
+    """
+    Represents an Experiment on Labstep.
 
-    def edit(
-        self, name=None, body=None, started_at=None, ended_at=None, extraParams={}
-    ):
+    To see all attributes of an experiment run
+    ::
+        print(my_experiment)
+
+    Specific attributes can be inspected via dot notation like so...
+    ::
+        print(my_experiment.name)
+        print(my_experiment.id)
+    """
+
+    __entityName__ = "experiment-workflow"
+
+    def __init__(self, data, user):
+        super().__init__(data, user)
+        if "root_experiment" in data:
+            self.root_experiment = ExperimentProtocol(
+                data['root_experiment'], user)
+
+    def edit(self, name=UNSPECIFIED, entry=UNSPECIFIED, started_at=UNSPECIFIED, extraParams={}):
         """
-        Edit an existing ExperimentProtocol.
+        Edit an existing Experiment.
 
         Parameters
         ----------
         name (str)
-            The new name of the ExperimentProtocol.
-        body (dict)
-            A JSON object representing the new body of the ExperimentProtocol.
+            The new name of the Experiment.
+        entry (obj)
+            A JSON object representing the state of the Experiment Entry.
         started_at (str)
-            The date the ExperimentProtocol was started
-            in the format of "YYYY-MM-DD HH:MM".
-        ended_at (str)
-            The date the ExperimentProtocol was finished
+            The start date of the Experiment
             in the format of "YYYY-MM-DD HH:MM".
 
         Returns
         -------
-        :class:`~labstep.entities.experimentProtocol.model.ExperimentProtocol`
-            An object representing the edited ExperimentProtocol.
+        :class:`~labstep.entities.experiment.model.Experiment`
+            An object representing the edited Experiment.
 
         Example
         -------
         ::
 
             my_experiment = user.getExperiment(17000)
-            protocols = my_experiment.getProtocols()
-            protocols[0].edit(name='A New Experiment Name',
+            my_experiment.edit(name='A New Experiment Name',
                                started_at='2018-06-06 12:05')
         """
-        import labstep.generic.entity.repository as entityRepository
+        import labstep.entities.experiment.repository as experimentRepository
 
-        fields = {
-            "name": name,
-            "state": body,
-            "started_at": started_at,
-            "ended_at": ended_at,
-            **extraParams,
-        }
-        return entityRepository.editEntity(self, fields)
+        return experimentRepository.editExperiment(
+            self, name=name, entry=entry, started_at=started_at, extraParams=extraParams
+        )
+
+    def delete(self):
+        """
+        Delete an existing Experiment.
+
+        Example
+        -------
+        ::
+
+            my_experiment = user.getExperiment(17000)
+            my_experiment.delete()
+        """
+        import labstep.entities.experiment.repository as experimentRepository
+
+        return experimentRepository.editExperiment(self, deleted_at=getTime())
+
+    def lock(self):
+        """
+        Lock an Experiment. Once locked, only owners can unlock.
+
+        Example
+        -------
+        ::
+
+            my_experiment = user.getExperiment(17000)
+            my_experiment.lock()
+        """
+        import labstep.entities.experiment.repository as experimentRepository
+        return experimentRepository.editExperiment(self, extraParams={'locked_at': getTime()})
+
+    def unlock(self):
+        """
+        Unlock a locked Experiment. Can only be done with owner permission.
 
-    def getExperiment(self):
+        Example
+        -------
+        ::
+
+            my_experiment = user.getExperiment(17000)
+            my_experiment.lock()
+            my_experiment.unlock()
+        """
+        import labstep.entities.experiment.repository as experimentRepository
+        return experimentRepository.editExperiment(self, extraParams={'locked_at': None})
 
-        from labstep.entities.experiment.repository import getExperiment
+    def complete(self, date=UNSPECIFIED):
+        """
+        Marks an experiment as complete.
 
-        if hasattr(self, 'experiment_workflow') is False:
+        Parameters
+        ----------
+        date (str)
+            Optionally specify a particular datetime it was completed.
+            Date format 'YYYY-MM-DD HH:MM:SS'
+
+        Example
+        -------
+        ::
+
+            my_experiment = user.getExperiment(17000)
+            my_experiment.complete()
+        """
+        import labstep.entities.experiment.repository as experimentRepository
+        return experimentRepository.editExperiment(self,
+                                                   extraParams={'ended_at': handleDate(date) if date is not UNSPECIFIED else getTime()})
+
+    def getEntry(self):
+        """
+        Returns a JSON document representing the entry for the experiment.
+
+        Example
+        -------
+        ::
+
+            my_experiment = user.getExperiment(17000)
+            print(my_experiment.getEntry())
+        """
+        import labstep.generic.entity.repository as entityRepository
+
+        if hasattr(self, 'root_experiment') is False:
             self.update()
 
-        return getExperiment(self.__user__, self.experiment_workflow['id'])
+        return entityRepository.getEntity(
+            self.__user__, ExperimentProtocol, self.root_experiment.id
+        ).state
 
-    def getBody(self):
+    def addProtocol(self, protocol):
         """
-        Returns the body of the protocol as a JSON document
+        Add a Labstep Protocol to a Labstep Experiment.
+
+        Parameters
+        ----------
+        protocol (Protocol)
+            The :class:`~labstep.entities.protocol.model.Protocol` to attach.
+
+        Returns
+        -------
+        :class:`~labstep.entities.protocol.model.Protocol`
+            An object representing the Protocol attached to the Experiment.
 
         Example
         -------
         ::
 
+            # Get an Experiment
             my_experiment = user.getExperiment(17000)
-            protocols = my_experiment.getProtocols()
-            protocols[0].getBody()
+
+            # Get a Protocol
+            my_protocol = user.getProtocol(10000)
+
+            # Attach the Protocol to the Experiment
+            my_experiment.addProtocol(my_protocol)
         """
-        self.update()
-        return getattr(self, "state", None)
+        import labstep.entities.experiment.repository as experimentRepository
+
+        return experimentRepository.addProtocolToExperiment(self, protocol)
 
-    def getMaterials(self, count=100, extraParams={}):
+    def getProtocols(self, count=100):
         """
-        Returns a list of the materials in a Protocol within an Experiment.
+        Retrieve the Protocols attached to this Labstep Experiment.
 
         Returns
         -------
-        List[:class:`~labstep.entities.experimentMaterial.model.ExperimentMaterial`]
-            List of the materials in an Experiment's Protocol.
+        List[:class:`~labstep.entities.experimentProtocol.model.ExperimentProtocol`]
+            List of the Protocols attached to the Experiment.
+
+        Example
+        -------
+        ::
+
+            entity = user.getExperiment(17000)
+            protocols = entity.getProtocols()
+            protocols[0].attributes()
+        """
+        import labstep.generic.entity.repository as entityRepository
+
+        return entityRepository.getEntities(
+            self.__user__,
+            ExperimentProtocol,
+            count,
+            {"is_root": 0, "experiment_workflow_id": self.id},
+        )
+
+    def addDataField(
+        self,
+        fieldName,
+        fieldType="default",
+        value=UNSPECIFIED,
+        date=UNSPECIFIED,
+        number=UNSPECIFIED,
+        unit=UNSPECIFIED,
+        filepath=UNSPECIFIED,
+        extraParams={},
+    ):
+        """
+        Add Data Fields to a Labstep Experiment.
+
+        Parameters
+        ----------
+        fieldName (str)
+            The name of the field.
+        fieldType (str)
+            The Metadata field type. Options are: "default", "date",
+            "numeric", or "file". The "default" type is "Text".
+        value (str)
+            The value accompanying the fieldName entry.
+        date (str)
+            The date and time accompanying the fieldName entry. Must be
+            in the format of "YYYY-MM-DD HH:MM".
+        number (float)
+            The quantity.
+        unit (str)
+            The unit accompanying the number entry.
+        filepath (str)
+            Local path to the file to upload for type 'file'
+
+        Returns
+        -------
+        :class:`~labstep.entities.experimentDataField.model.ExperimentDataField`
+            An object representing the new Labstep Data Field.
+
+        Example
+        -------
+        ::
+
+            experiment = user.getExperiment(17000)
+            dataField = experiment.addDataField("Refractive Index",
+                                               value="1.73")
+        """
+        return self.root_experiment.addDataField(
+            fieldName=fieldName,
+            fieldType=fieldType,
+            value=value,
+            date=date,
+            number=number,
+            unit=unit,
+            filepath=filepath,
+            extraParams=extraParams,
+        )
+
+    def getDataFields(self):
+        """
+        Retrieve the Data Fields of a Protocol within an Experiment.
+
+        Returns
+        -------
+        :class:`~labstep.entities.experimentDataField.model.ExperimentDataField`
+            An array of objects representing Data Fields
+            on a Protocol within an Experiment.
 
         Example
         -------
         ::
 
             experiment = user.getExperiment(17000)
             exp_protocol = experiment.getProtocols()[0]
-            exp_protocol_materials = exp_protocol.getMaterials()
-            exp_protocol_materials[0].attributes()
+            dataFields = exp_protocol.getDataFields()
+        """
+        return self.root_experiment.getDataFields()
+
+    def getSignatures(self):
         """
+        Retrieve a list of signatures added to the experiment
 
-        return experimentMaterialRepository.getExperimentMaterials(self.__user__,
-                                                                   experiment_id=self.id, count=count, extraParams=extraParams)
+        Returns
+        -------
+        List[:class:`~labstep.entities.experimentSignature.model.ExperimentSignature`]
+            List of the signatures added to the Experiment
+        """
+        exp = self.__user__.getExperiment(self.id)
+        return EntityList(exp.signatures, ExperimentSignature, self.__user__)
+
+    def addSignature(self, statement=UNSPECIFIED, lock=False):
+        """
+        Add a signature to experiment
+
+        Parameters
+        ----------
+        statement (str)
+            Statement describing the signature.
+        lock (boolean)
+            Whether to lock the experiment against further edits.
+
+        Returns
+        -------
+        :class:`~labstep.entities.experimentSignature.model.ExperimentSignature`
+            The signature that has been added
+        """
+        import labstep.generic.entity.repository as entityRepository
+
+        params = {
+            "statement": statement,
+            "is_lock": int(lock),
+            "experiment_workflow_id": self.id,
+        }
+        return entityRepository.newEntity(self.__user__, ExperimentSignature, params)
+
+    def getSignatureRequests(self):
+        """
+        Returns a list of pending signature requests for the experiment.
+
+        Returns
+        -------
+        List[:class:`~labstep.entities.experimentSignatureRequest.model.ExperimentSignatureRequest`]
+        """
+        import labstep.entities.experimentSignatureRequest.repository as experimentSignatureRequestRepository
+
+        return experimentSignatureRequestRepository.getExperimentSignatureRequests(self.__user__, self.id)
+
+    def requestSignature(self, user_id, message=UNSPECIFIED):
+        """
+        Request a signature from another user in the workspace
+
+        Parameters
+        ----------
+
+        user_id (int)
+            Id of the user you are requesting a signature from
+
+        message (str)
+            Optional message to include in signature request email
+
+        """
+        import labstep.entities.experimentSignatureRequest.repository as experimentSignatureRequestRepository
+
+        return experimentSignatureRequestRepository.newExperimentSignatureRequest(self.__user__, self.id, user_id=user_id, message=message)
+
+    def getMaterials(self):
+        """
+        Returns a list of the materials in the Experiment.
+
+        Returns
+        -------
+        List[:class:`~labstep.entities.experimentMaterial.model.ExperimentMaterial`]
+            List of the materials in an Experiment.
+
+        Example
+        -------
+        ::
+
+            experiment = user.getExperiment(17000)
+            exp_materials = experiment.getMaterials()
+            print(exp_materials[0])
+        """
+        return self.root_experiment.getMaterials()
 
     def addMaterial(
         self,
-        name=None,
-        amount=None,
-        units=None,
-        resource_id=None,
-        resource_item_id=None,
+        name=UNSPECIFIED,
+        amount=UNSPECIFIED,
+        units=UNSPECIFIED,
+        resource_id=UNSPECIFIED,
+        resource_item_id=UNSPECIFIED,
         extraParams={},
     ):
         """
-        Add a new material to the ExperimentProtocol.
+        Add a new material to the Experiment.
 
         Parameters
         ----------
         name (str)
             The name of the material to add.
         amount (str)
             The amount used.
@@ -141,48 +407,81 @@
         ::
 
             experiment = user.getExperiment(17000)
             resource = user.getResources(search_query='Sample A')[0]
             experiment.addMaterial(name='Sample A', amount='2', units='ml',
                                  resource_id=resource.id)
         """
-        return experimentMaterialRepository.newExperimentMaterial(self.__user__,
-                                                                  experiment_id=self.id,
-                                                                  name=name,
-                                                                  amount=amount,
-                                                                  units=units,
-                                                                  resource_id=resource_id,
-                                                                  resource_item_id=resource_item_id,
-                                                                  extraParams=extraParams)
+        return self.root_experiment.addMaterial(name=name,
+                                                resource_id=resource_id,
+                                                resource_item_id=resource_item_id,
+                                                amount=amount,
+                                                units=units,
+                                                extraParams=extraParams)
 
-    def addSteps(self, N):
+    def addToCollection(self, collection_id):
         """
-        Add steps to a Protocol within an Experiment
+        Add the experiment to a collection.
 
         Parameters
         ----------
-        N (int)
-            The number of steps to add.
+        collection_id (int)
+            The id of the collection to add to
+
+        Returns
+        -------
+        None
+        """
+        import labstep.entities.collection.repository as collectionRepository
+
+        return collectionRepository.addToCollection(self, collection_id=collection_id)
+
+    def getCollections(self):
+        """
+        Returns the list of collections the protocol is in.
+        """
+        import labstep.entities.collection.repository as collectionRepository
+
+        return collectionRepository.getAttachedCollections(self)
+
+    def removeFromCollection(self, collection_id):
+        """
+        Remove the experiment from a collection.
+
+        Parameters
+        ----------
+        collection_id (int)
+            The id of the collection to remove from
+
+        """
+        import labstep.entities.collection.repository as collectionRepository
+
+        return collectionRepository.removeFromCollection(self, collection_id)
+
+    def getTables(self):
+        """
+        Returns a list of the tables in the entry of an Experiment.
+
+        Returns
+        -------
+        List[:class:`~labstep.entities.experimentTable.model.ExperimentTable`]
+            List of the tables in an Experiment entry
 
         Example
         -------
         ::
 
             experiment = user.getExperiment(17000)
-            exp_protocol = experiment.getProtocols()[0]
-            exp_protocol_steps = exp_protocol.addSteps(5)
+            tables = experiment.getTables()
         """
-        import labstep.generic.entity.repository as entityRepository
-
-        steps = [{"experiment_id": self.id}] * N
-        return entityRepository.newEntities(self.__user__, ExperimentStep, steps)
+        return self.root_experiment.getTables()
 
-    def addTable(self, name=None, data=None):
+    def addTable(self, name=UNSPECIFIED, data=UNSPECIFIED):
         """
-        Add a new table to a Protocol within an Experiment.
+        Add a new table to an Experiment.
 
         Parameters
         ----------
         name (str)
             The name of the table.
         data (json)
             The data of the table in json format.
@@ -211,265 +510,134 @@
                             }
                         }
                     }
                 }
             }
 
             experiment = user.getExperiment(17000)
-            exp_protocol = experiment.getProtocols()[0]
-            exp_protocol.addTable(name='Calibration', data=data)
+            experiment.addTable(name='Calibration', data=data)
         """
-        import labstep.generic.entity.repository as entityRepository
-
-        params = {"experiment_id": self.id, "name": name, "data": data}
-        return entityRepository.newEntity(self.__user__, ExperimentTable, params)
+        return self.root_experiment.addTable(name=name, data=data)
 
-    def getSteps(self):
+    def addFile(self, filepath=UNSPECIFIED, rawData=UNSPECIFIED):
         """
-        Returns a list of the steps in a Protocol within an Experiment.
-
-        Returns
-        -------
-        List[:class:`~labstep.entities.experimentStep.model.ExperimentStep`]
-            List of the steps in an Experiment's Protocol.
-
-        Example
-        -------
-        ::
-
-            experiment = user.getExperiment(17000)
-            exp_protocol = experiment.getProtocols()[0]
-            exp_protocol_steps = exp_protocol.getSteps()
-            exp_protocol_steps[0].attributes()
-        """
-        self.update()
-        steps = self.experiment_steps
-        return EntityList(steps, ExperimentStep, self.__user__)
-
-    def addTimer(self, name=None, hours=None, minutes=None, seconds=None):
-        """
-        Add a new timer to a Protocol within an Experiment.
+        Add a file to an experiment entry.
+        (Only use for files to be embedded in the body of the entry)
 
         Parameters
         ----------
-        name (str)
-            The name of the timer.
-        hours (int)
-            The hours of the timer.
-        minutes (int)
-            The minutes of the timer.
-        seconds (int)
-            The seconds of the timer.
+        filepath (str)
+            The path to the file to upload.
+        rawData (bytes)
+            Raw bytes data to upload as file
 
         Returns
         -------
-        :class:`~labstep.entities.ExperimentTimer.model.ExperimentTimer`
-            The newly added timer entity.
+        :class:`~labstep.file.File`
+            The newly added file entity.
 
         Example
         -------
         ::
 
             experiment = user.getExperiment(17000)
-            exp_protocol = experiment.getProtocols()[0]
-            exp_protocol.addTimer(name='Refluxing', hours='4', minutes='30')
+            experiment.addFile(filepath='./my_file.csv')
         """
-        import labstep.generic.entity.repository as entityRepository
+        return self.root_experiment.addFile(filepath, rawData)
 
-        params = {
-            "experiment_id": self.id,
-            "name": name,
-            "hours": hours,
-            "minutes": minutes,
-            "seconds": seconds,
-        }
-        return entityRepository.newEntity(self.__user__, ExperimentTimer, params)
-
-    def getTables(self):
+    def getComments(self, count=100):
         """
-        Returns a list of the tables in a Protocol within an Experiment.
+        Retrieve the Comments attached to this Labstep Entity.
 
         Returns
         -------
-        List[:class:`~labstep.entities.experimentTable.model.ExperimentTable`]
-            List of the tables in an Experiment's Protocol.
+        List[:class:`~labstep.entities.comment.model.Comment`]
+            List of the comments attached.
 
         Example
         -------
         ::
 
-            experiment = user.getExperiment(17000)
-            exp_protocol = experiment.getProtocols()[0]
-            exp_protocol_tables = exp_protocol.getTables()
-            exp_protocol_tables[0].attributes()
+            entity = user.getExperiment(17000)
+            comments = entity.getComments()
+            comments[0].attributes()
         """
-        self.update()
-        tables = self.experiment_tables
-        return EntityList(tables, ExperimentTable, self.__user__)
-
-    def getTimers(self):
-        """
-        Returns a list of the timers in a Protocol within an Experiment.
-
-        Returns
-        -------
-        List[:class:`~labstep.entities.experimentTimer.model.ExperimentTimer`]
-            List of the timers in an Experiment's Protocol.
+        import labstep.entities.comment.repository as commentRepository
 
-        Example
-        -------
-        ::
+        if hasattr(self, 'thread_ids') is False:
+            self.update()
 
-            experiment = user.getExperiment(17000)
-            exp_protocol = experiment.getProtocols()[0]
-            exp_protocol_timers = exp_protocol.getTimers()
-            exp_protocol_timers[0].attributes()
-        """
-        self.update()
-        timers = self.experiment_timers
-        return EntityList(timers, ExperimentTimer, self.__user__)
+        return commentRepository.getComments(self, count, extraParams={'parent_thread_id': self.thread_ids})
 
-    def getDataFields(self):
+    def getFiles(self):
         """
-        Retrieve the Data Fields of a Protocol within an Experiment.
+        Returns a list of the files in a experiment entry.
+        (Only includes the files embedded in the body of the entry)
 
         Returns
         -------
-        :class:`~labstep.entities.experimentDataField.model.ExperimentDataField`
-            An array of objects representing the Labstep
-            Data Fields on a Protocol within an Experiment.
+        List[:class:`~labstep.file.File`]
+            List of the files in a experiment.
 
         Example
         -------
         ::
 
             experiment = user.getExperiment(17000)
-            exp_protocol = experiment.getProtocols()[0]
-            metadata = exp_protocol.getDataFields()
+            experiment_files = experiment.getFiles()
         """
-        import labstep.entities.experimentDataField.repository as experimentDataFieldRepository
+        return self.root_experiment.getFiles()
 
-        return experimentDataFieldRepository.getDataFields(self)
-
-    def addDataField(
-        self,
-        fieldName,
-        fieldType="default",
-        value=None,
-        date=None,
-        number=None,
-        unit=None,
-        filepath=None,
-        extraParams={},
-    ):
+    def addExperimentLink(self, experiment_id):
+        """
+        Link this experiment to a previous experiment.
         """
-        Add a Data Field to a Protocol within an Experiment.
+        return newExperimentLink(self.__user__, src_experiment_id=self.id, dest_experiment_id=experiment_id)
 
-        Parameters
-        ----------
-        fieldName (str)
-            The name of the field.
-        fieldType (str)
-            The field type. Options are: "default", "date",
-            "quantity", or "number". The "default" type is "Text".
-        value (str)
-            The value accompanying the fieldName entry.
-        date (str)
-            The date and time accompanying the fieldName entry. Must be
-            in the format of "YYYY-MM-DD HH:MM".
-        number (float)
-            The quantity.
-        unit (str)
-            The unit accompanying the number entry.
-        filepath (str)
-            Local path to the file to upload for type 'file'
+    def getExperimentLinks(self, direction='forward'):
+        """
+        Returns a list of experiments that the current experiment references (direction = "forward")
+        or a list of experiments that reference the current experiment (direction = "backwards")
 
         Returns
         -------
-        :class:`~labstep.entities.metadata.model.Metadata`
-            An object representing the new Labstep Data Field.
+        List[:class:`~labstep.experimentLink.ExperimentLink`]
+            List of linked experiments.
 
         Example
         -------
         ::
 
             experiment = user.getExperiment(17000)
-            experiment_protocol = experiment.getProtocols()[0]
-            dataField = experiment_protocol.addDataField(
-                "Refractive Index", value="1.73"
-            )
+            experimentLinks = experiment.getExperimentLinks(direction="backwards")
         """
-        import labstep.entities.experimentDataField.repository as experimentDataFieldRepository
+        import labstep.entities.experimentLink.repository as experimentLinkRepository
 
-        return experimentDataFieldRepository.addDataFieldTo(
-            self,
-            fieldName=fieldName,
-            fieldType=fieldType,
-            value=value,
-            date=date,
-            number=number,
-            unit=unit,
-            filepath=filepath,
-            extraParams=extraParams,
-        )
+        return experimentLinkRepository.getExperimentLinks(self.__user__, self.id, direction=direction)
 
-    def addFile(self, filepath=None, rawData=None):
+    def export(self, path):
         """
-        Add a file to an Experiment Protocol.
+        Export the experiment to the directory specified. 
 
         Parameters
-        ----------
-        filepath (str)
-            The path to the file to upload.
-        rawData (bytes)
-            Raw data to upload as a file.
-
-        Returns
         -------
-        :class:`~labstep.file.File`
-            The newly added file entity.
+        path (str)
+            The path to the directory to save the experiment.
 
         Example
         -------
         ::
 
             experiment = user.getExperiment(17000)
-            experiment_protocol = experiment.getProtocols()[0]
-            file = experiment_protocol.addFile(filepath='./my_file.csv')
-        """
-        params = {'experiment_id': self.id}
-        return fileRepository.newFile(self.__user__, filepath=filepath, rawData=rawData, extraParams=params)
-
-    def getFiles(self):
+            experiment.export('/my_folder')
         """
-        Returns a list of the files in a Protocol.
+        import labstep.entities.experiment.repository as experimentRepository
 
-        Returns
-        -------
-        List[:class:`~labstep.file.File`]
-            List of the files in a Protocol.
+        return experimentRepository.exportExperiment(self, path)
 
-        Example
-        -------
-        ::
-
-            experiment = user.getExperiment(17000)
-            experiment_protocol = experiment.getProtocols()[0]
-            filess = experiment_protocol.getFiles()
-        """
-        self.update()
-        files = self.files
-        return EntityList(files, File, self.__user__)
-
-    def export(self, rootPath, folderName=None):
-        import labstep.entities.experimentProtocol.repository as experimentProtocolRepository
-        return experimentProtocolRepository.exportExperimentProtocol(self, rootPath, folderName=folderName)
-
-    @deprecated(version='3.3.2', reason="You should use experimentProtocol.addDataField instead")
+    @deprecated(version='3.3.2', reason="You should use experiment.addDataField instead")
     def addDataElement(self, *args, **kwargs):
-
         return self.addDataField(*args, **kwargs)
 
-    @deprecated(version='3.3.2', reason="You should use experimentProtocol.getDataFields instead")
+    @deprecated(version='3.3.2', reason="You should use experiment.getDataFields instead")
     def getDataElements(self):
-
         return self.getDataFields()
```

### Comparing `labstep-3.8.0/labstep/entities/experimentProtocol/repository.py` & `labstep-3.9.0/labstep/entities/experimentProtocol/repository.py`

 * *Files identical despite different names*

### Comparing `labstep-3.8.0/labstep/entities/experimentSignature/model.py` & `labstep-3.9.0/labstep/entities/experimentSignature/model.py`

 * *Files identical despite different names*

### Comparing `labstep-3.8.0/labstep/entities/experimentSignatureRequest/model.py` & `labstep-3.9.0/labstep/entities/experimentSignatureRequest/model.py`

 * *Files identical despite different names*

### Comparing `labstep-3.8.0/labstep/entities/experimentSignatureRequest/repository.py` & `labstep-3.9.0/labstep/entities/experimentSignatureRequest/repository.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 
 from labstep.entities.experimentSignatureRequest.model import ExperimentSignatureRequest
 import labstep.generic.entity.repository as entityRepository
+from labstep.constants import UNSPECIFIED
 
 
-def newExperimentSignatureRequest(user, experiment_id, user_id, message=None):
+def newExperimentSignatureRequest(user, experiment_id, user_id, message=UNSPECIFIED):
     fields = {
         "experiment_workflow_id": experiment_id,
         "message": message,
         "user_id": user_id
     }
     return entityRepository.newEntity(user, ExperimentSignatureRequest, fields=fields)
```

### Comparing `labstep-3.8.0/labstep/entities/experimentStep/model.py` & `labstep-3.9.0/labstep/entities/experimentStep/model.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
 
-from labstep.generic.entity.model import Entity
+from labstep.generic.entityWithComments.model import EntityWithComments
 from labstep.service.helpers import getTime
+from labstep.constants import UNSPECIFIED
 
 
-class ExperimentStep(Entity):
+class ExperimentStep(EntityWithComments):
     __entityName__ = "experiment-step"
 
-    def edit(self, completed_at=None):
+    def edit(self, completed_at=UNSPECIFIED):
         """
         Edit an existing Experiment Step.
 
         Parameters
         ----------
         completed_at (str)
             The datetime at which the Experiment Step was completed.
@@ -40,65 +41,7 @@
             exp_protocol = experiment.getProtocols()[0]
             exp_protocol_steps = exp_protocol.getSteps()
             exp_protocol_steps[0].complete()
             exp_protocol_steps[1].complete()
             exp_protocol_steps[2].complete()
         """
         return self.edit(completed_at=getTime())
-
-    def addComment(self, body, filepath=None):
-        """
-        Add a comment and/or file to this step.
-
-        Parameters
-        ----------
-        body (str)
-            The body of the comment.
-        filepath (str)
-            A Labstep File entity to attach to the comment,
-            including the filepath.
-
-        Returns
-        -------
-        :class:`~labstep.entities.comment.model.Comment`
-            The comment added.
-
-        Example
-        -------
-        ::
-
-            experiment = user.getExperiment(17000)
-            exp_protocol = experiment.getProtocols()[0]
-            exp_protocol_steps = exp_protocol.getSteps()
-            exp_protocol_steps[0].addComment('This step failed')
-        """
-        import labstep.entities.comment.repository as commentRepository
-
-        return commentRepository.addCommentWithFile(self, body, filepath)
-
-    def getComments(self, count=100):
-        """
-        Retrieve the Comments attached to this step.
-
-        Parameters
-        ----------
-
-        count (int)
-            The number of comments to return
-
-        Returns
-        -------
-        List[:class:`~labstep.entities.comment.model.Comment`]
-            List of the comments attached.
-
-        Example
-        -------
-        ::
-
-           experiment = user.getExperiment(17000)
-            exp_protocol = experiment.getProtocols()[0]
-            exp_protocol_steps = exp_protocol.getSteps()
-            exp_protocol_steps[0].getComments()
-        """
-        import labstep.entities.comment.repository as commentRepository
-
-        return commentRepository.getComments(self, count)
```

### Comparing `labstep-3.8.0/labstep/entities/experimentTable/model.py` & `labstep-3.9.0/labstep/entities/experimentTable/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
 
 from labstep.generic.entity.model import Entity
 from labstep.service.helpers import dataTableToDataFrame
+from labstep.constants import UNSPECIFIED
 
 
 class ExperimentTable(Entity):
     __entityName__ = "experiment-table"
 
-    def edit(self, name=None, data=None):
+    def edit(self, name=UNSPECIFIED, data=UNSPECIFIED):
         """
         Edit an existing Experiment Table.
 
         Parameters
         ----------
         name (str)
             The name of the Experiment Table.
```

### Comparing `labstep-3.8.0/labstep/entities/experimentTimer/model.py` & `labstep-3.9.0/labstep/entities/experimentTimer/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
 
 from labstep.generic.entity.model import Entity
+from labstep.constants import UNSPECIFIED
 
 
 class ExperimentTimer(Entity):
     __entityName__ = "experiment-timer"
+    __hasGuid__ = True
 
-    def edit(self, hours=None, minutes=None, seconds=None):
+    def edit(self, hours=UNSPECIFIED, minutes=UNSPECIFIED, seconds=UNSPECIFIED):
         """
         Edit an existing Experiment Timer.
 
         Parameters
         ----------
         hours (int)
             The hours of the timer.
@@ -35,19 +37,19 @@
             exp_protocol_timers = exp_protocol.getTimers()
             exp_protocol_timers[0].edit(minutes=1, seconds=7)
         """
         import labstep.generic.entity.repository as entityRepository
 
         fields = {}
 
-        if hours is not None:
+        if hours is not UNSPECIFIED:
             fields["hours"] = hours
-        if minutes is not None:
+        if minutes is not UNSPECIFIED:
             fields["minutes"] = minutes
-        if seconds is not None:
+        if seconds is not UNSPECIFIED:
             fields["seconds"] = seconds
 
         return entityRepository.editEntity(self, fields)
 
     """ def start(self):
         time = getTime() + self.hours + self.minutes + self.seconds
         fields = {'ended_at': time}
```

### Comparing `labstep-3.8.0/labstep/entities/file/model.py` & `labstep-3.9.0/labstep/entities/file/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
 
 import os
 from labstep.generic.entity.model import Entity
+from labstep.constants import UNSPECIFIED
 
 
 class File(Entity):
     __entityName__ = "file"
 
     def getData(self):
         """
@@ -21,15 +22,15 @@
             file = entities[0]
             data = file.getData()
         """
         import labstep.entities.file.repository as fileRepository
 
         return fileRepository.downloadFile(self.__user__, self.id)
 
-    def save(self, folder=None, name=None):
+    def save(self, folder=UNSPECIFIED, name=UNSPECIFIED):
         """
         Save a Labstep file to the local filesystem.
 
         Parameters
         ----------
         folder (str)
             The path to the folder where the file should be saved
@@ -49,18 +50,18 @@
             file = entities[0]
             file.save()
         """
         if self.link_source is not None:
             print('Warning: Files from External Cloud Providers cannot be downloaded')
             return
 
-        if name is None:
+        if name is UNSPECIFIED:
             name = self.name
 
-        if folder is not None:
+        if folder is not UNSPECIFIED:
             filepath = os.path.join(folder, name)
         else:
             filepath = name
 
         data = self.getData()
         open(filepath, "wb").write(data)
```

### Comparing `labstep-3.8.0/labstep/entities/file/repository.py` & `labstep-3.9.0/labstep/entities/file/repository.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,48 +4,53 @@
 
 import json
 from labstep.service.config import configService
 from labstep.service.helpers import url_join, getHeaders
 from labstep.entities.file.model import File
 from labstep.service.request import requestService
 import labstep.generic.entity.repository as entityRepository
+from labstep.constants import UNSPECIFIED
 
 
-def newFile(user, filepath=None, rawData=None, extraParams={}):
-    if filepath is not None:
+def newFile(user, filepath=UNSPECIFIED, rawData=UNSPECIFIED, extraParams={}):
+    if filepath is not UNSPECIFIED:
         rawData = open(filepath, 'rb')
-    if rawData is None:
+    if rawData is UNSPECIFIED:
         raise Exception('Please specify filepath or raw data')
 
     files = {'file': rawData}
     params = {"group_id": user.activeWorkspace, **extraParams}
     headers = getHeaders(user=user)
     url = url_join(configService.getHost(), "/api/generic/file/upload")
     response = requestService.post(
         url, headers=headers, files=files, data=params)
     data = json.loads(response.content)
     return File(list(data.values())[0], user)
 
 
 def getFile(user, fileId):
-    return entityRepository.getEntity(user, File, fileId, isDeleted=None)
+    return entityRepository.getEntity(user, File, fileId, isDeleted=UNSPECIFIED)
 
 
-def downloadFile(user, fileId):
+def getFileDownloadLink(user, fileId):
     headers = getHeaders(user=user)
     url = url_join(configService.getHost(),
                    "/api/generic/file/download", str(fileId))
     response = requestService.post(url, headers=headers)
-    rawData = requestService.get(json.loads(response.content)[
-        "signed_url"], headers=None).content
-    return rawData
+    return json.loads(response.content)["signed_url"]
+
+
+def downloadFile(user, fileId):
+    downloadLink = getFileDownloadLink(user, fileId)
+    response = requestService.get(downloadLink, headers=None)
+    return response.content
 
 
 def getFiles(
-    user, count=100, search_query=None, file_type=None, extraParams={}
+    user, count=100, search_query=UNSPECIFIED, file_type=UNSPECIFIED, extraParams={}
 ):
     params = {"search_query": search_query,
               "filetype": file_type, **extraParams}
     return entityRepository.getEntities(user, File, count, params)
 
 
 def exportFile(file, root_path):
```

### Comparing `labstep-3.8.0/labstep/entities/invitation/repository.py` & `labstep-3.9.0/labstep/entities/invitation/repository.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 # Author: Barney Walker <barney@labstep.com>
 
 from labstep.service.helpers import url_join, getHeaders
 from labstep.service.config import configService
 from labstep.service.request import requestService
 from labstep.entities.invitation.model import Invitation
 import labstep.generic.entity.repository as entityRepository
+from labstep.constants import UNSPECIFIED
 
 
-def newInvitations(user, invitationType, emails, organization_id, workspace_id=None):
+def newInvitations(user, invitationType, emails, organization_id, workspace_id=UNSPECIFIED):
     url = url_join(configService.getHost(), 'api/generic',
                    'share-link-invitation', invitationType)
     headers = getHeaders(user=user)
     json = {
         'emails': emails,
         'organization_id': organization_id,
         'organization_group_id': workspace_id
     }
     requestService.post(url=url, headers=headers, json=json)
 
 
 def getInvitations(user, organization_id, extraParams):
-    return entityRepository.getEntities(user, Invitation, count=None, filterParams={
+    return entityRepository.getEntities(user, Invitation, count=UNSPECIFIED, filterParams={
         'organization_id': organization_id, **extraParams})
```

### Comparing `labstep-3.8.0/labstep/entities/jupyterInstance/model.py` & `labstep-3.9.0/labstep/entities/jupyterInstance/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -59,7 +59,34 @@
             my_jupyterInstance.end()
         """
         import labstep.entities.jupyterInstance.repository as jupyterInstanceRepository
 
         return jupyterInstanceRepository.editJupyterInstance(
             self, endedAt=getTime()
         )
+
+    def edit(self, data=None, extraParams={}):
+        """
+        Edit an existing JupyterInstance.
+
+        Parameters
+        ----------
+        data (str)
+            JupyterNotebook ipyb JSON data.
+
+        Returns
+        -------
+        :class:`~labstep.entities.jupyterInstance.model.JupyterInstance`
+            An object representing the edited JupyterInstance.
+
+        Example
+        -------
+        ::
+
+            my_jupyterInstance = user.getJupyterInstance("872b3e7e-e21f-4403-9ef3-3650fe0d86ba")
+            my_jupyterInstance.edit(data='{test: 42}')
+        """
+        import labstep.entities.jupyterInstance.repository as jupyterInstanceRepository
+
+        return jupyterInstanceRepository.editJupyterInstance(
+            self, data=data
+        )
```

### Comparing `labstep-3.8.0/labstep/entities/jupyterInstance/repository.py` & `labstep-3.9.0/labstep/entities/jupyterInstance/repository.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Author: Thomas Bullier <thomas@labstep.com>
 
 from labstep.entities.jupyterInstance.model import JupyterInstance
 import labstep.generic.entity.repository as entityRepository
+from labstep.constants import UNSPECIFIED
 
 
 def getJupyterInstance(user, guid):
     return entityRepository.getEntity(user, JupyterInstance, id=guid)
 
 
 def editJupyterInstance(
     jupyterInstance,
-    startedAt=None,
-    endedAt=None
+    data=UNSPECIFIED,
+    startedAt=UNSPECIFIED,
+    endedAt=UNSPECIFIED
 ):
     params = {
+        "data": data,
         "started_at": startedAt,
         "ended_at": endedAt,
     }
 
     return entityRepository.editEntity(jupyterInstance, params)
```

### Comparing `labstep-3.8.0/labstep/entities/jupyterNotebook/model.py` & `labstep-3.9.0/labstep/entities/jupyterNotebook/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Author: Thomas Bullier <thomas@labstep.com>
 
 from labstep.generic.entity.model import Entity
+from labstep.constants import UNSPECIFIED
 
 
 class JupyterNotebook(Entity):
     """
     Represents an JupyterNotebook on Labstep.
     """
 
     __entityName__ = "jupyter-notebook"
     __hasGuid__ = True
 
-    def edit(self, name=None, status=None, data=None, extraParams={}):
+    def edit(self, name=UNSPECIFIED, status=UNSPECIFIED, data=UNSPECIFIED, extraParams={}):
         """
         Edit an existing JupyterNotebook.
 
         Parameters
         ----------
         name (str)
             A display name.
```

### Comparing `labstep-3.8.0/labstep/entities/jupyterNotebook/repository.py` & `labstep-3.9.0/labstep/entities/jupyterNotebook/repository.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Author: Thomas Bullier <thomas@labstep.com>
 
 from labstep.entities.jupyterNotebook.model import JupyterNotebook
 import labstep.generic.entity.repository as entityRepository
+from labstep.constants import UNSPECIFIED
 
 
-def newJupyterNotebook(user, name=None, data=None):
+def newJupyterNotebook(user, name=UNSPECIFIED, data=UNSPECIFIED):
     return entityRepository.newEntity(user, JupyterNotebook, {"name": name, "data": data})
 
 
 def getJupyterNotebook(user, guid):
     return entityRepository.getEntity(user, JupyterNotebook, id=guid)
 
 
 def editJupyterNotebook(
     jupyterNotebook,
-    name=None,
-    status=None,
-    data=None,
+    name=UNSPECIFIED,
+    status=UNSPECIFIED,
+    data=UNSPECIFIED,
     extraParams={},
 ):
     params = {
         "name": name,
         "status": status,
         "data": data,
         **extraParams,
```

### Comparing `labstep-3.8.0/labstep/entities/metadata/model.py` & `labstep-3.9.0/labstep/entities/metadata/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
 
 from labstep.generic.entity.model import Entity
 from labstep.service.helpers import handleDate, getTime
-
+from labstep.constants import UNSPECIFIED
 
 TYPE_DEFAULT = "default"
 TYPE_NUMERIC = "numeric"
 TYPE_DATE = "date"
 TYPE_FILE = "file"
 TYPE_MOLECULE = "molecule"
 TYPE_SEQUENCE = "sequence"
@@ -67,15 +67,15 @@
         print(my_metadata_field.value)
         print(my_metadata_field.id)
     """
 
     __entityName__ = "metadata"
     __searchKey__ = "label"
 
-    def edit(self, fieldName=None, value=None, extraParams={}):
+    def edit(self, fieldName=UNSPECIFIED, value=UNSPECIFIED, extraParams={}):
         """
         Edit the value of an existing Metadata.
 
         Parameters
         ----------
         fieldName (str)
             The new name of the field.
```

### Comparing `labstep-3.8.0/labstep/entities/metadata/repository.py` & `labstep-3.9.0/labstep/entities/metadata/repository.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Author: Barney Walker <barney@labstep.com>
 
 import labstep.entities.file.repository as fileRepository
 import labstep.generic.entity.repository as entityRepository
 from labstep.generic.entityList.model import EntityList
 from labstep.service.helpers import handleDate, handleString
 from labstep.entities.metadata.model import Metadata, FIELDS, ALLOWED_FIELDS
+from labstep.constants import UNSPECIFIED
 
 
 def getMetadata(entity, count=1000, extraParams={}):
     if hasattr(entity, 'metadata_thread') is False:
         entity.update()
     if 'metadatas' in entity.metadata_thread:
         return EntityList(entity.metadata_thread['metadatas'], Metadata, entity.__user__)
@@ -22,39 +23,39 @@
 
 
 def addMetadataTo(
 
     entity,
     fieldName,
     fieldType="default",
-    value=None,
-    date=None,
-    number=None,
-    unit=None,
-    filepath=None,
+    value=UNSPECIFIED,
+    date=UNSPECIFIED,
+    number=UNSPECIFIED,
+    unit=UNSPECIFIED,
+    filepath=UNSPECIFIED,
     extraParams={},
 ):
-    if filepath is not None:
+    if filepath is not UNSPECIFIED:
         fileId = fileRepository.newFile(entity.__user__, filepath).id
     else:
-        fileId = None
+        fileId = UNSPECIFIED
 
     if fieldType not in FIELDS:
         msg = "Not a supported metadata type '{}'".format(fieldType)
         raise ValueError(msg)
 
     allowedFieldsForType = set(ALLOWED_FIELDS[fieldType])
     fields = {
         "value": value,
         "date": date,
         "number": number,
         "unit": unit,
         "file_id": fileId,
     }
-    fields = {k: v for k, v in fields.items() if v}
+    fields = {k: v for k, v in fields.items() if v is not UNSPECIFIED}
     fields = set(fields.keys())
     violations = fields - allowedFieldsForType
     if violations:
         msg = "Unallowed fields [{}] for type {}".format(
             ",".join(violations), fieldType
         )
         raise ValueError(msg)
@@ -70,14 +71,14 @@
         "file_id": fileId,
         **extraParams,
     }
 
     return entityRepository.newEntity(entity.__user__, Metadata, params)
 
 
-def editMetadata(metadata, fieldName=None, value=None, extraParams={}):
+def editMetadata(metadata, fieldName=UNSPECIFIED, value=UNSPECIFIED, extraParams={}):
     params = {
         "label": handleString(fieldName),
         "value": handleString(value),
         **extraParams
     }
     return entityRepository.editEntity(metadata, params)
```

### Comparing `labstep-3.8.0/labstep/entities/orderRequest/model.py` & `labstep-3.9.0/labstep/entities/orderRequest/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
 
 from labstep.generic.entityPrimary.model import EntityPrimary
 from labstep.generic.entityWithMetadata.model import EntityWithMetadata
 from labstep.service.helpers import getTime
+from labstep.constants import UNSPECIFIED
 
 
 class OrderRequest(EntityPrimary, EntityWithMetadata):
     """
     Represents an Order Request on Labstep.
 
     To see all attributes of the order request run
@@ -21,19 +22,19 @@
         print(my_order_request.id)
     """
 
     __entityName__ = "order-request"
 
     def edit(
         self,
-        status=None,
-        resource_id=None,
-        quantity=None,
-        price=None,
-        currency=None,
+        status=UNSPECIFIED,
+        resource_id=UNSPECIFIED,
+        quantity=UNSPECIFIED,
+        price=UNSPECIFIED,
+        currency=UNSPECIFIED,
         extraParams={},
     ):
         """
         Edit an existing OrderRequest.
 
         Parameters
         ----------
```

### Comparing `labstep-3.8.0/labstep/entities/orderRequest/repository.py` & `labstep-3.9.0/labstep/entities/orderRequest/repository.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
 
 from labstep.service.helpers import handleKeyword
 from labstep.entities.orderRequest.model import OrderRequest
 import labstep.generic.entity.repository as entityRepository
+from labstep.constants import UNSPECIFIED
 
 
 def getOrderRequest(user, orderRequest_id):
     return entityRepository.getEntity(user, OrderRequest, id=orderRequest_id)
 
 
 def getOrderRequests(
     user,
     count=100,
-    search_query=None,
-    tag_id=None,
-    status=None,
+    search_query=UNSPECIFIED,
+    tag_id=UNSPECIFIED,
+    status=UNSPECIFIED,
     extraParams={},
 ):
     params = {
         "group_id": user.activeWorkspace,
         "search_query": search_query,
         "tag_id": tag_id,
         "status": handleKeyword(status),
         **extraParams,
     }
     return entityRepository.getEntities(user, OrderRequest, count, params)
 
 
-def newOrderRequest(user, resource_id=None, quantity=1, extraParams={}):
+def newOrderRequest(user, resource_id=UNSPECIFIED, quantity=1, extraParams={}):
     params = {"resource_id": resource_id, "quantity": quantity, **extraParams}
     return entityRepository.newEntity(user, OrderRequest, params)
 
 
 def editOrderRequest(
     orderRequest,
-    status=None,
-    resource_id=None,
-    quantity=None,
-    price=None,
-    currency=None,
-    deleted_at=None,
+    status=UNSPECIFIED,
+    resource_id=UNSPECIFIED,
+    quantity=UNSPECIFIED,
+    price=UNSPECIFIED,
+    currency=UNSPECIFIED,
+    deleted_at=UNSPECIFIED,
     extraParams={},
 ):
     params = {
         "status": handleKeyword(status),
         "resource_id": resource_id,
         "quantity": quantity,
         "price": price,
```

### Comparing `labstep-3.8.0/labstep/entities/organization/model.py` & `labstep-3.9.0/labstep/entities/organization/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Author: Barney Walker <barney@labstep.com>
 
 import labstep.entities.organizationUser.repository as organizationUserRepository
 from labstep.generic.entity.model import Entity
 import labstep.generic.entity.repository as entityRepository
 import labstep.entities.workspace.repository as workspaceRepository
 import labstep.entities.invitation.repository as invitationRepository
+from labstep.constants import UNSPECIFIED
 
 
 class Organization(Entity):
     __entityName__ = "organization"
 
     def edit(self, name, extraParams={}):
         """
@@ -32,15 +33,15 @@
 
             my_organization.edit(name='My new organization.')
         """
         import labstep.entities.organization.repository as organizationRepository
 
         return organizationRepository.editOrganization(self.__user__, name, extraParams=extraParams)
 
-    def inviteUsers(self, emails, workspace_id=None):
+    def inviteUsers(self, emails, workspace_id=UNSPECIFIED):
         """
         Invite users to your organization.
 
         Parameters
         ----------
         emails (list)
             A list of email address to send invitations to.
@@ -57,15 +58,15 @@
         """
         return invitationRepository.newInvitations(self.__user__,
                                                    invitationType='organization',
                                                    emails=emails,
                                                    organization_id=self.id,
                                                    workspace_id=workspace_id)
 
-    def getWorkspaces(self, count=100, search_query=None):
+    def getWorkspaces(self, count=100, search_query=UNSPECIFIED):
         """
         Get the workspaces in your Organization
 
         Parameters
         ----------
         count (int)
             Number of workspaces to return.
```

### Comparing `labstep-3.8.0/labstep/entities/organization/repository.py` & `labstep-3.9.0/labstep/entities/organization/repository.py`

 * *Files identical despite different names*

### Comparing `labstep-3.8.0/labstep/entities/organizationUser/model.py` & `labstep-3.9.0/labstep/entities/organizationUser/model.py`

 * *Files identical despite different names*

### Comparing `labstep-3.8.0/labstep/entities/organizationUser/repository.py` & `labstep-3.9.0/labstep/entities/organizationUser/repository.py`

 * *Files identical despite different names*

### Comparing `labstep-3.8.0/labstep/entities/permission/model.py` & `labstep-3.9.0/labstep/entities/permission/model.py`

 * *Files identical despite different names*

### Comparing `labstep-3.8.0/labstep/entities/permission/repository.py` & `labstep-3.9.0/labstep/entities/permission/repository.py`

 * *Files identical despite different names*

### Comparing `labstep-3.8.0/labstep/entities/protocol/model.py` & `labstep-3.9.0/labstep/entities/protocol/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from labstep.entities.protocolVersion.model import ProtocolVersion
 from labstep.entities.protocolMaterial.model import ProtocolMaterial
 import labstep.entities.protocolMaterial.repository as protocolMaterialRepository
 from labstep.generic.entityList.model import EntityList
 from labstep.entities.file.model import File
 import labstep.entities.file.repository as fileRepository
 from labstep.service.helpers import getTime
+from labstep.constants import UNSPECIFIED
 
 
 class Protocol(EntityPrimary):
     """
     Represents a Protocol on Labstep.
 
     To see all attributes of a protocol run
@@ -29,15 +30,15 @@
         print(my_protocol.name)
         print(my_protocol.id)
     """
 
     __entityName__ = "protocol-collection"
     __searchKey__ = 'label'
 
-    def edit(self, name=None, body=None, extraParams={}):
+    def edit(self, name=UNSPECIFIED, body=UNSPECIFIED, extraParams={}):
         """
         Edit an existing Protocol.
 
         Parameters
         ----------
         name (str)
             The name of the Protocol.
@@ -203,19 +204,19 @@
 
         return EntityList(map(addId, self.last_version["metadata_thread"]["metadatas"]), ProtocolDataField, self.__user__)
 
     def addDataField(
         self,
         fieldName,
         fieldType="default",
-        value=None,
-        date=None,
-        number=None,
-        unit=None,
-        filepath=None,
+        value=UNSPECIFIED,
+        date=UNSPECIFIED,
+        number=UNSPECIFIED,
+        unit=UNSPECIFIED,
+        filepath=UNSPECIFIED,
         extraParams={},
     ):
         """
         Add a Data Field to a Protocol.
 
         Parameters
         ----------
@@ -258,15 +259,15 @@
             number=number,
             unit=unit,
             filepath=filepath,
             extraParams=extraParams,
         )
 
     def addMaterial(
-        self, name=None, amount=None, units=None, resource_id=None, extraParams={}
+        self, name=UNSPECIFIED, amount=UNSPECIFIED, units=UNSPECIFIED, resource_id=UNSPECIFIED, extraParams={}
     ):
         """
         Add a new material to the Protocol.
 
         Parameters
         ----------
         name (str)
@@ -319,15 +320,15 @@
         """
         self.update()
         if "protocol_values" not in self.last_version:
             return []
         materials = self.last_version["protocol_values"]
         return EntityList(materials, ProtocolMaterial, self.__user__)
 
-    def addTimer(self, name=None, hours=None, minutes=None, seconds=None):
+    def addTimer(self, name=UNSPECIFIED, hours=UNSPECIFIED, minutes=UNSPECIFIED, seconds=UNSPECIFIED):
         """
         Add a new timer to the Protocol.
 
         Parameters
         ----------
         name (str)
             The name of the timer.
@@ -381,15 +382,15 @@
         self.update()
         if "protocol_timers" not in self.last_version:
             return []
 
         timers = self.last_version["protocol_timers"]
         return EntityList(timers, ProtocolTimer, self.__user__)
 
-    def addTable(self, name=None, data=None):
+    def addTable(self, name=UNSPECIFIED, data=UNSPECIFIED):
         """
         Add a new table to the Protocol.
 
         Parameters
         ----------
         name (str)
             The name of the table.
@@ -491,15 +492,15 @@
             The id of the collection to remove from
 
         """
         import labstep.entities.collection.repository as collectionRepository
 
         return collectionRepository.removeFromCollection(self, collection_id)
 
-    def addFile(self, filepath=None, rawData=None):
+    def addFile(self, filepath=UNSPECIFIED, rawData=UNSPECIFIED):
         """
         Add a file to a Protocol.
 
         Parameters
         ----------
         filepath (str)
             The path to the file to upload.
```

### Comparing `labstep-3.8.0/labstep/entities/protocol/repository.py` & `labstep-3.9.0/labstep/entities/protocol/repository.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,30 @@
 from labstep.service.helpers import (
     handleDate,
 )
 from labstep.entities.protocol.model import Protocol
 from labstep.entities.protocolVersion.model import ProtocolVersion
 import labstep.generic.entity.repository as entityRepository
 from labstep.service.htmlExport import htmlExportService
+from labstep.constants import UNSPECIFIED
 
 
 def getProtocol(user, protocol_id):
     return entityRepository.getEntity(user, Protocol, id=protocol_id)
 
 
 def getProtocols(
 
     user,
     count=100,
-    search_query=None,
-    created_at_from=None,
-    created_at_to=None,
-    tag_id=None,
-    collection_id=None,
+    search_query=UNSPECIFIED,
+    created_at_from=UNSPECIFIED,
+    created_at_to=UNSPECIFIED,
+    tag_id=UNSPECIFIED,
+    collection_id=UNSPECIFIED,
     extraParams={},
 ):
     params = {
         "search_query": search_query,
         "created_at_from": handleDate(created_at_from),
         "created_at_to": handleDate(created_at_to),
         "tag_id": tag_id,
@@ -39,19 +40,19 @@
 
 def newProtocol(user, name, extraParams={}):
     params = {"name": name, **extraParams}
     return entityRepository.newEntity(user, Protocol, params)
 
 
 def editProtocol(
-    protocol, name=None, body=None, deleted_at=None, extraParams={}
+    protocol, name=UNSPECIFIED, body=UNSPECIFIED, deleted_at=UNSPECIFIED, extraParams={}
 ):
     params = {"name": name, "deleted_at": deleted_at, **extraParams}
 
-    if body is not None:
+    if body is not UNSPECIFIED:
         entityRepository.editEntity(
             ProtocolVersion(protocol.last_version, protocol.__user__),
             {"state": body},
         )
         protocol.update()
 
     return entityRepository.editEntity(protocol, params)
```

### Comparing `labstep-3.8.0/labstep/entities/protocolDataField/model.py` & `labstep-3.9.0/labstep/entities/protocolDataField/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
 
 from labstep.generic.entity.model import Entity
 import labstep.generic.entity.repository as entityRepository
 from labstep.service.helpers import getTime
+from labstep.constants import UNSPECIFIED
 
 
 class ProtocolDataField(Entity):
     """
     Represents a data field on a Labstep Protocol.
 
     To see the attributes of the data field run
@@ -20,15 +21,15 @@
         print(my_data_field.value)
         print(my_data_field.id)
     """
 
     __entityName__ = "metadata"
     __searchKey__ = "label"
 
-    def edit(self, fieldName=None, value=None, extraParams={}):
+    def edit(self, fieldName=UNSPECIFIED, value=UNSPECIFIED, extraParams={}):
         """
         Edit the value of an existing data field.
 
         Parameters
         ----------
         fieldName (str)
             The new name of the field.
```

### Comparing `labstep-3.8.0/labstep/entities/protocolDataField/repository.py` & `labstep-3.9.0/labstep/entities/protocolDataField/repository.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Author: Barney Walker <barney@labstep.com>
 
 import labstep.entities.file.repository as fileRepository
 import labstep.generic.entity.repository as entityRepository
 from labstep.service.helpers import handleDate, handleString
 from labstep.entities.protocolDataField.model import ProtocolDataField
 from labstep.entities.protocolVersion.model import ProtocolVersion
+from labstep.constants import UNSPECIFIED
 
 
 def getDataFields(entity, count=1000, extraParams={}):
 
     if isinstance(entity, ProtocolVersion):
         params = {
             "metadata_thread_id": entity.metadata_thread["id"]}
@@ -22,25 +23,25 @@
 
 
 def addDataFieldTo(
 
     entity,
     fieldName,
     fieldType="default",
-    value=None,
-    date=None,
-    number=None,
-    unit=None,
-    filepath=None,
+    value=UNSPECIFIED,
+    date=UNSPECIFIED,
+    number=UNSPECIFIED,
+    unit=UNSPECIFIED,
+    filepath=UNSPECIFIED,
     extraParams={},
 ):
-    if filepath is not None:
+    if filepath is not UNSPECIFIED:
         fileId = fileRepository.newFile(entity.__user__, filepath).id
     else:
-        fileId = None
+        fileId = UNSPECIFIED
 
     params = {
         "metadata_thread_id": entity.metadata_thread["id"],
         "type": fieldType,
         "label": handleString(fieldName),
         "value": handleString(value),
         "date": handleDate(date),
@@ -54,14 +55,14 @@
         entity.__user__, ProtocolDataField, params)
 
     dataField.protocol_id = entity.id
 
     return dataField
 
 
-def editDataField(dataField, fieldName=None, value=None, extraParams={}):
+def editDataField(dataField, fieldName=UNSPECIFIED, value=UNSPECIFIED, extraParams={}):
     params = {
         "label": handleString(fieldName),
         "value": handleString(value),
         **extraParams
     }
     return entityRepository.editEntity(dataField, params)
```

### Comparing `labstep-3.8.0/labstep/entities/protocolMaterial/model.py` & `labstep-3.9.0/labstep/entities/protocolMaterial/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
 
 from labstep.generic.entity.model import Entity
+from labstep.constants import UNSPECIFIED
 
 
 class ProtocolMaterial(Entity):
     __entityName__ = "protocol-value"
 
     def __init__(self, data, user):
         super().__init__(data, user)
         self.amount = self.value
 
     def edit(
-        self, name=None, amount=None, units=None, resource_id=None, extraParams={}
+        self, name=UNSPECIFIED, amount=UNSPECIFIED, units=UNSPECIFIED, resource_id=UNSPECIFIED, extraParams={}
     ):
         """
         Edit an existing Protocol Material.
 
         Parameters
         ----------
         name (str)
```

### Comparing `labstep-3.8.0/labstep/entities/protocolMaterial/repository.py` & `labstep-3.9.0/labstep/entities/protocolMaterial/repository.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
 
 from labstep.entities.protocolMaterial.model import ProtocolMaterial
 import labstep.generic.entity.repository as entityRepository
+from labstep.constants import UNSPECIFIED
 
 
 def getProtocolMaterial(user, protocol_material_id):
     return entityRepository.getEntity(
         user, ProtocolMaterial, id=protocol_material_id
     )
 
@@ -16,31 +17,31 @@
     params = {
         'protocol_id': protocol_id,
         **extraParams
     }
     return entityRepository.getEntities(user, ProtocolMaterial, count, params)
 
 
-def newProtocolMaterial(user, protocol_id, name, resource_id=None, amount=None, units=None, extraParams={}):
+def newProtocolMaterial(user, protocol_id, name, resource_id=UNSPECIFIED, amount=UNSPECIFIED, units=UNSPECIFIED, extraParams={}):
     params = {
         "protocol_id": protocol_id,
         "name": name,
         "resource_id": resource_id,
         "value": amount,
         "units": units,
         **extraParams,
     }
 
-    if params["value"] is not None:
+    if params["value"] is not UNSPECIFIED:
         params["value"] = str(params["value"])
 
     return entityRepository.newEntity(user, ProtocolMaterial, params)
 
 
-def editProtocolMaterial(protocol_material, name=None, amount=None, units=None, resource_id=None, extraParams={}):
+def editProtocolMaterial(protocol_material, name=UNSPECIFIED, amount=UNSPECIFIED, units=UNSPECIFIED, resource_id=UNSPECIFIED, extraParams={}):
     params = {
         "name": name,
         "value": amount,
         "units": units,
         "resource_id": resource_id,
         **extraParams
     }
```

### Comparing `labstep-3.8.0/labstep/entities/protocolTable/model.py` & `labstep-3.9.0/labstep/entities/protocolTable/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
 
 from labstep.generic.entity.model import Entity
 from labstep.service.helpers import dataTableToDataFrame
+from labstep.constants import UNSPECIFIED
 
 
 class ProtocolTable(Entity):
     __entityName__ = "protocol-table"
 
-    def edit(self, name=None, data=None, extraParams={}):
+    def edit(self, name=UNSPECIFIED, data=UNSPECIFIED, extraParams={}):
         """
         Edit an existing Protocol Table.
 
         Parameters
         ----------
         name (str)
             The name of the Protocol Table.
```

### Comparing `labstep-3.8.0/labstep/entities/protocolTimer/model.py` & `labstep-3.9.0/labstep/entities/protocolTimer/model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
 
 from labstep.generic.entity.model import Entity
+from labstep.constants import UNSPECIFIED
 
 
 class ProtocolTimer(Entity):
     __entityName__ = "protocol-timer"
+    __hasGuid__ = True
 
-    def edit(self, name=None, hours=None, minutes=None, seconds=None, extraParams={}):
+    def edit(self, name=UNSPECIFIED, hours=UNSPECIFIED, minutes=UNSPECIFIED, seconds=UNSPECIFIED, extraParams={}):
         """
         Edit an existing Protocol Timer.
 
         Parameters
         ----------
         name (str)
             The name of the timer.
@@ -37,15 +39,15 @@
             protocol_timers[0].edit(name='New Timer Name',
                                     minutes=1, seconds=17)
         """
         import labstep.generic.entity.repository as entityRepository
 
         params = {"name": name, **extraParams}
 
-        if hours is not None:
+        if hours is not UNSPECIFIED:
             params["hours"] = hours
-        if minutes is not None:
+        if minutes is not UNSPECIFIED:
             params["minutes"] = minutes
-        if seconds is not None:
+        if seconds is not UNSPECIFIED:
             params["seconds"] = seconds
 
         return entityRepository.editEntity(self, params)
```

### Comparing `labstep-3.8.0/labstep/entities/resource/model.py` & `labstep-3.9.0/labstep/entities/resource/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
 
 from labstep.service.helpers import getTime
 from labstep.generic.entityPrimary.model import EntityPrimary
 from labstep.generic.entityWithMetadata.model import EntityWithMetadata
 from labstep.entities.resourceItem.model import ResourceItem
+from labstep.constants import UNSPECIFIED
 
 
 class Resource(EntityPrimary, EntityWithMetadata):
     """
     Represents a Resource on Labstep.
 
     To see all attributes of the resource run
@@ -20,15 +21,15 @@
     ::
         print(my_resource.name)
         print(my_resource.id)
     """
 
     __entityName__ = "resource"
 
-    def edit(self, name=None, extraParams={}):
+    def edit(self, name=UNSPECIFIED, extraParams={}):
         """
         Edit an existing Resource.
 
         Parameters
         ----------
         name (str)
             The new name of the Resource.
@@ -147,15 +148,15 @@
         return orderRequestRepository.newOrderRequest(
             self.__user__,
             resource_id=self.id,
             quantity=quantity,
             extraParams=extraParams,
         )
 
-    def getItems(self, count=100, search_query=None, extraParams={}):
+    def getItems(self, count=100, search_query=UNSPECIFIED, extraParams={}):
         """
         Returns the items of this Resource.
 
         Parameters
         ----------
         count (int)
             The number of ResourceItems to retrieve.
@@ -184,19 +185,19 @@
             count=count,
             search_query=search_query,
             extraParams=extraParams,
         )
 
     def newItem(
         self,
-        name=None,
+        name=UNSPECIFIED,
         availability="available",
-        quantity_amount=None,
-        quantity_unit=None,
-        resource_location_id=None,
+        quantity_amount=UNSPECIFIED,
+        quantity_unit=UNSPECIFIED,
+        resource_location_id=UNSPECIFIED,
         extraParams={},
     ):
         """
         Create a new Labstep ResourceItem.
 
         Parameters
         ----------
```

### Comparing `labstep-3.8.0/labstep/entities/resourceCategory/model.py` & `labstep-3.9.0/labstep/entities/resourceCategory/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
 
 from labstep.generic.entityWithSharing.model import EntityWithSharing
 from labstep.service.helpers import getTime
 from labstep.entities.resourceTemplate.model import ResourceTemplate
 from labstep.entities.resourceItem.model import ResourceItem
+from labstep.constants import UNSPECIFIED
 
 
 class ResourceCategory(EntityWithSharing):
     """
     Represents a Resource Category on Labstep.
 
     To see all attributes of the resource category run
@@ -20,15 +21,15 @@
     ::
         print(my_resource_category.name)
         print(my_resource_category.id)
     """
 
     __entityName__ = "resource"
 
-    def edit(self, name=None, extraParams={}):
+    def edit(self, name=UNSPECIFIED, extraParams={}):
         """
         Edit an existing ResourceCategory.
 
         Parameters
         ----------
         name (str)
             The new name of the ResourceCategory.
```

### Comparing `labstep-3.8.0/labstep/entities/resourceCategory/repository.py` & `labstep-3.9.0/labstep/entities/resourceCategory/repository.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
 
 from labstep.entities.resourceCategory.model import ResourceCategory
 import labstep.generic.entity.repository as entityRepository
+from labstep.constants import UNSPECIFIED
 
 
 def getResourceCategory(user, resourceCategory_id):
     """
     Retrieve a specific Labstep ResourceCategory.
 
     Parameters
@@ -23,15 +24,15 @@
     ResourceCategory
         An object representing a Labstep ResourceCategory.
     """
     return entityRepository.getEntity(user, ResourceCategory, id=resourceCategory_id)
 
 
 def getResourceCategorys(
-        user, count=100, search_query=None, tag_id=None, extraParams={}
+        user, count=100, search_query=UNSPECIFIED, tag_id=UNSPECIFIED, extraParams={}
 ):
     """
     Retrieve a list of a user's ResourceCategorys on Labstep,
     which can be filtered using the parameters:
 
     Parameters
     ----------
@@ -73,11 +74,11 @@
         An object representing the new Labstep ResourceCategory.
     """
     params = {"name": name, **extraParams, "is_template": 1}
     return entityRepository.newEntity(user, ResourceCategory, params)
 
 
 def editResourceCategory(
-        resourceCategory, name=None, deleted_at=None, extraParams={}
+        resourceCategory, name=UNSPECIFIED, deleted_at=UNSPECIFIED, extraParams={}
 ):
     params = {"name": name, "deleted_at": deleted_at, **extraParams}
     return entityRepository.editEntity(resourceCategory, params)
```

### Comparing `labstep-3.8.0/labstep/entities/resourceItem/model.py` & `labstep-3.9.0/labstep/entities/resourceItem/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
 
 from labstep.generic.entity.model import Entity
 from labstep.service.helpers import getTime
+from labstep.constants import UNSPECIFIED
 
 
 class ResourceItem(Entity):
     """
     Represents a Resource Item on Labstep.
 
     To see all attributes of the resource item run
@@ -20,19 +21,19 @@
         print(my_resource_item.id)
     """
 
     __entityName__ = "resource-item"
 
     def edit(
         self,
-        name=None,
-        availability=None,
-        quantity_amount=None,
-        quantity_unit=None,
-        resource_location_id=None,
+        name=UNSPECIFIED,
+        availability=UNSPECIFIED,
+        quantity_amount=UNSPECIFIED,
+        quantity_unit=UNSPECIFIED,
+        resource_location_id=UNSPECIFIED,
         extraParams={},
     ):
         """
         Edit an existing ResourceItem.
 
         Parameters
         ----------
@@ -83,15 +84,15 @@
             my_resource_item = user.getResourceItem(17000)
             my_resource_item.delete()
         """
         import labstep.entities.resourceItem.repository as resourceItemRepository
 
         return resourceItemRepository.editResourceItem(self, deleted_at=getTime())
 
-    def addComment(self, body, filepath=None, extraParams={}):
+    def addComment(self, body, filepath=UNSPECIFIED, extraParams={}):
         """
         Add a comment and/or file to a Labstep ResourceItem.
 
         Parameters
         ----------
         body (str)
             The body of the comment.
@@ -140,19 +141,19 @@
 
         return commentRepository.getComments(self, count, extraParams=extraParams)
 
     def addMetadata(
         self,
         fieldName,
         fieldType="default",
-        value=None,
-        date=None,
-        number=None,
-        unit=None,
-        filepath=None,
+        value=UNSPECIFIED,
+        date=UNSPECIFIED,
+        number=UNSPECIFIED,
+        unit=UNSPECIFIED,
+        filepath=UNSPECIFIED,
         extraParams={},
     ):
         """
         Add Metadata to a ResourceItem.
 
         Parameters
         ----------
```

### Comparing `labstep-3.8.0/labstep/entities/resourceLocation/model.py` & `labstep-3.9.0/labstep/entities/resourceLocation/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
 
 from labstep.generic.entityWithMetadata.model import EntityWithMetadata
 from labstep.generic.entityWithComments.model import EntityWithComments
 from labstep.service.helpers import getTime
+from labstep.constants import UNSPECIFIED
 
 
 class ResourceLocation(EntityWithMetadata, EntityWithComments):
     """
     Represents a Resource Location on Labstep.
 
     To see all attributes of the resource location run
@@ -20,15 +21,15 @@
         print(my_resource_location.name)
         print(my_resource_location.id)
     """
 
     __entityName__ = "resource-location"
     __hasParentGroup__ = True
 
-    def edit(self, name=None, extraParams={}):
+    def edit(self, name=UNSPECIFIED, extraParams={}):
         """
         Edit an existing ResourceLocation.
 
         Parameters
         ----------
         name (str)
             The new name of the ResourceLocation.
```

### Comparing `labstep-3.8.0/labstep/entities/resourceLocation/repository.py` & `labstep-3.9.0/labstep/entities/resourceLocation/repository.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
 
 from labstep.entities.resourceLocation.model import ResourceLocation
 import labstep.generic.entity.repository as entityRepository
+from labstep.constants import UNSPECIFIED
 
 
 def getResourceLocation(user, resource_location_id):
     return entityRepository.getEntity(
         user, ResourceLocation, id=resource_location_id
     )
 
 
 def getResourceLocations(
-    user, count=100, search_query=None, tag_id=None, extraParams={}
+    user, count=100, search_query=UNSPECIFIED, extraParams={}
 ):
     params = {
         "group_id": user.activeWorkspace,
         "search_query": search_query,
-        "tag_id": tag_id,
         **extraParams,
     }
     return entityRepository.getEntities(user, ResourceLocation, count, params)
 
 
-def newResourceLocation(user, name, outer_location_id=None, extraParams={}):
+def newResourceLocation(user, name, outer_location_id=UNSPECIFIED, extraParams={}):
     params = {"name": name, "outer_location_id": outer_location_id, **extraParams}
     return entityRepository.newEntity(user, ResourceLocation, params)
 
 
 def editResourceLocation(resourceLocation, name, extraParams={}):
     params = {"name": name, **extraParams}
     return entityRepository.editEntity(resourceLocation, params)
```

### Comparing `labstep-3.8.0/labstep/entities/resourceTemplate/model.py` & `labstep-3.9.0/labstep/generic/entityWithMetadata/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
 
 from labstep.generic.entity.model import Entity
+from labstep.constants import UNSPECIFIED
 
 
-class ResourceTemplate(Entity):
-    __entityName__ = "resource"
-
+class EntityWithMetadata(Entity):
     def addMetadata(
         self,
         fieldName,
         fieldType="default",
-        value=None,
-        date=None,
-        number=None,
-        unit=None,
-        filepath=None,
+        value=UNSPECIFIED,
+        date=UNSPECIFIED,
+        number=UNSPECIFIED,
+        unit=UNSPECIFIED,
+        filepath=UNSPECIFIED,
         extraParams={},
     ):
         """
-        Add Metadata to the Resource Template.
+        Add Metadata to a Labstep Entity.
 
         Parameters
         ----------
         fieldName (str)
             The name of the field.
         fieldType (str)
             The Metadata field type. Options are: "default", "date",
@@ -46,45 +45,44 @@
         :class:`~labstep.entities.metadata.model.Metadata`
             An object representing the new Labstep Metadata.
 
         Example
         -------
         ::
 
-            resource_category = user.getResourceCategory(17000)
-            metadata = my_resource_category.addMetadata("Refractive Index",
-                                                        value="1.73")
+            resource = user.getResource(17000)
+            metadata = resource.addMetadata("Refractive Index",
+                                               value="1.73")
         """
         import labstep.entities.metadata.repository as metadataRepository
 
         return metadataRepository.addMetadataTo(
             self,
-            fieldName,
-            fieldType,
-            value,
-            date,
-            number,
-            unit,
+            fieldName=fieldName,
+            fieldType=fieldType,
+            value=value,
+            date=date,
+            number=number,
+            unit=unit,
             filepath=filepath,
             extraParams=extraParams,
         )
 
     def getMetadata(self):
         """
-        Retrieve the Metadata of the Resource Template.
+        Retrieve the Metadata of a Labstep Entity.
 
         Returns
         -------
         :class:`~labstep.entities.metadata.model.Metadata`
-            An array of Metadata objects for the Resource.
+            An array of Metadata objects for the Entity.
 
         Example
         -------
         ::
 
-            entity = user.getResourceCategory(17000)
-            metadatas = entity.getMetadata()
-            metadatas[0].attributes()
+            my_resource = user.getResource(17000)
+            metadatas = my_resource.getMetadata()
         """
         import labstep.entities.metadata.repository as metadataRepository
 
         return metadataRepository.getMetadata(self)
```

### Comparing `labstep-3.8.0/labstep/entities/sharelink/model.py` & `labstep-3.9.0/labstep/entities/sharelink/model.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
 
 import requests
 from labstep.generic.entity.model import Entity
 from labstep.service.config import configService
 from labstep.service.helpers import url_join, handleError, getHeaders
+from labstep.constants import UNSPECIFIED
 
 
 class Sharelink(Entity):
     """
     Represents a Sharelink on Labstep.
     """
 
     __entityName__ = "share-link"
     __isLegacy__ = True
 
-    def edit(self, permission=None, extraParams={}):
+    def edit(self, permission=UNSPECIFIED, extraParams={}):
         """
         Edit a sharelink.
 
         Parameters
         ----------
         permission (str)
             Set the permission granted by the sharelink
@@ -48,15 +49,15 @@
 
         fields = {
             "type": permission,
             **extraParams,
         }
         return entityRepository.editEntity(self, fields=fields)
 
-    def sendEmails(self, emails, message=None):
+    def sendEmails(self, emails, message=UNSPECIFIED):
         """
         Send sharelinks to collaborators via email.
 
         Parameters
         ----------
         emails (list)
             A list of the emails to send the invite to.
```

### Comparing `labstep-3.8.0/labstep/entities/tag/model.py` & `labstep-3.9.0/labstep/entities/tag/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
 
 from labstep.generic.entity.model import Entity
+from labstep.constants import UNSPECIFIED
 
 
 class Tag(Entity):
     """
     Represents a Tag on Labstep.
 
     To see all attributes of a tag run
@@ -18,15 +19,15 @@
         print(my_tag.name)
         print(my_tag.id)
     """
 
     __entityName__ = "tag"
     __hasParentGroup__ = True
 
-    def edit(self, name=None, extraParams={}):
+    def edit(self, name=UNSPECIFIED, extraParams={}):
         """
         Edit the name of an existing Tag.
 
         Parameters
         ----------
         name (str)
             The new name of the Tag.
```

### Comparing `labstep-3.8.0/labstep/entities/tag/repository.py` & `labstep-3.9.0/labstep/entities/tag/repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 
 import json
 from labstep.service.config import configService
 from labstep.service.helpers import url_join, handleKeyword, getHeaders
 from labstep.entities.tag.model import Tag
 from labstep.service.request import requestService
 import labstep.generic.entity.repository as entityRepository
+from labstep.constants import UNSPECIFIED
 
 
-def getTags(user, count=1000, type=None, search_query=None, extraParams={}):
+def getTags(user, count=1000, type=UNSPECIFIED, search_query=UNSPECIFIED, extraParams={}):
     """
     Retrieve a list of the user's tags.
 
     Parameters
     ----------
     user (obj)
         The Labstep user.
```

### Comparing `labstep-3.8.0/labstep/entities/user/facade.py` & `labstep-3.9.0/labstep/entities/user/facade.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
 
 import os
 import labstep.entities.user.repository as userRepository
+from labstep.constants import UNSPECIFIED
 
 
 def newUser(
-    first_name, last_name, email, password, share_link_token=None, extraParams={}
+    first_name, last_name, email, password, share_link_token=UNSPECIFIED, extraParams={}
 ):
     """
     TODO
     """
     return userRepository.newUser(
         first_name, last_name, email, password, share_link_token, extraParams
     )
 
 
-def authenticate(username=None, apikey=None):
+def authenticate(username=UNSPECIFIED, apikey=UNSPECIFIED):
     """
     Returns an authenticated Labstep User object to allow
     you to interact with the Labstep API.
 
     Parameters
     ----------
     username (str)
@@ -38,15 +39,15 @@
     -------
     ::
 
         import labstep
 
         user = labstep.authenticate('myaccount@labstep.com', 'MY_API_KEY')
     """
-    if (apikey is None):
+    if (apikey is UNSPECIFIED):
         apikey = os.environ['LABSTEP_API_KEY']
 
     return userRepository.authenticate(username, apikey)
 
 
 def login(username, password):
     """
```

### Comparing `labstep-3.8.0/labstep/entities/user/model.py` & `labstep-3.9.0/labstep/entities/user/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Author: Barney Walker <barney@labstep.com>
 
 from deprecated import deprecated
 from labstep.generic.entity.model import Entity
 from labstep.service.config import configService
 from labstep.service.helpers import url_join, getHeaders
 from labstep.service.request import requestService
+from labstep.constants import UNSPECIFIED
 
 
 class User(Entity):
     """
     Represents a Labstep User.
 
     To see all attributes of the user run
@@ -20,16 +21,16 @@
     Specific attributes can be accessed via dot notation like so...
     ::
         print(user.name)
         print(user.id)
     """
     __entityName__ = "user"
 
-    def __init__(self, user, adminUser=None):
-        self.__user__ = adminUser if adminUser is not None else self
+    def __init__(self, user, adminUser=UNSPECIFIED):
+        self.__user__ = adminUser if adminUser is not UNSPECIFIED else self
         if 'group' not in user or user["group"] is None:
             print(
                 """Warning: No default workspace.
             Please set a workspace to continue."""
             )
             self.activeWorkspace = None
         else:
@@ -332,19 +333,19 @@
         return deviceRepository.getDevice(self, device_id)
 
     # getMany()
 
     def getExperiments(
         self,
         count=100,
-        search_query=None,
-        created_at_from=None,
-        created_at_to=None,
-        tag_id=None,
-        collection_id=None,
+        search_query=UNSPECIFIED,
+        created_at_from=UNSPECIFIED,
+        created_at_to=UNSPECIFIED,
+        tag_id=UNSPECIFIED,
+        collection_id=UNSPECIFIED,
         extraParams={},
     ):
         """
         Retrieve a list of a User's Experiments
         across all Workspaces on Labstep,
         which can be filtered using the parameters:
 
@@ -391,19 +392,19 @@
             collection_id=collection_id,
             extraParams=extraParams,
         )
 
     def getProtocols(
         self,
         count=100,
-        search_query=None,
-        created_at_from=None,
-        created_at_to=None,
-        tag_id=None,
-        collection_id=None,
+        search_query=UNSPECIFIED,
+        created_at_from=UNSPECIFIED,
+        created_at_to=UNSPECIFIED,
+        tag_id=UNSPECIFIED,
+        collection_id=UNSPECIFIED,
         extraParams={},
     ):
         """
         Retrieve a list of a User's Protocols
         across all Workspaces on Labstep,
         which can be filtered using the parameters:
 
@@ -447,15 +448,15 @@
             created_at_from=created_at_from,
             created_at_to=created_at_to,
             tag_id=tag_id,
             collection_id=collection_id,
             extraParams=extraParams,
         )
 
-    def getResources(self, count=100, search_query=None, tag_id=None, extraParams={}):
+    def getResources(self, count=100, search_query=UNSPECIFIED, tag_id=UNSPECIFIED, extraParams={}):
         """
         Retrieve a list of a User's Resources
         across all Workspaces on Labstep,
         which can be filtered using the parameters:
 
         Parameters
         ----------
@@ -485,15 +486,15 @@
             count=count,
             search_query=search_query,
             tag_id=tag_id,
             extraParams=extraParams,
         )
 
     def getResourceCategorys(
-        self, count=100, search_query=None, tag_id=None, extraParams={}
+        self, count=100, search_query=UNSPECIFIED, tag_id=UNSPECIFIED, extraParams={}
     ):
         """
         Retrieve a list of a User's Resource Categorys
         across all Workspaces on Labstep,
         which can be filtered using the parameters:
 
         Parameters
@@ -523,15 +524,15 @@
             self,
             count=count,
             search_query=search_query,
             tag_id=tag_id,
             extraParams=extraParams,
         )
 
-    def getResourceLocations(self, count=100, search_query=None, extraParams={}):
+    def getResourceLocations(self, count=100, search_query=UNSPECIFIED, extraParams={}):
         """
         Retrieve a list of a user's ResourceLocations on Labstep,
         which can be filtered using the parameters:
 
         Parameters
         ----------
         count (int)
@@ -552,15 +553,15 @@
         """
         import labstep.entities.resourceLocation.repository as resourceLocationRepository
 
         return resourceLocationRepository.getResourceLocations(
             self, count=count, search_query=search_query, extraParams=extraParams
         )
 
-    def getResourceItems(self, count=100, search_query=None, extraParams={}):
+    def getResourceItems(self, count=100, search_query=UNSPECIFIED, extraParams={}):
         """
         Retrieve a list of a user's ResourceItems on Labstep,
         which can be filtered using the parameters:
 
         Parameters
         ----------
         count (int)
@@ -582,15 +583,15 @@
         import labstep.entities.resourceItem.repository as resourceItemRepository
 
         return resourceItemRepository.getResourceItems(
             self, count=count, search_query=search_query, extraParams=extraParams
         )
 
     def getOrderRequests(
-        self, count=100, search_query=None, status=None, tag_id=None, extraParams={}
+        self, count=100, search_query=UNSPECIFIED, status=UNSPECIFIED, tag_id=UNSPECIFIED, extraParams={}
     ):
         """
         Retrieve a list of a user's OrderRequests on Labstep,
         which can be filtered using the parameters:
 
         Parameters
         ----------
@@ -623,15 +624,15 @@
             count=count,
             search_query=search_query,
             status=status,
             tag_id=tag_id,
             extraParams=extraParams,
         )
 
-    def getTags(self, count=1000, search_query=None, type=None, extraParams={}):
+    def getTags(self, count=1000, search_query=UNSPECIFIED, type=UNSPECIFIED, extraParams={}):
         """
         Retrieve a list of a User's Tags
         across all Workspaces on Labstep,
         which can be filtered using the parameters:
 
         Parameters
         ----------
@@ -661,15 +662,15 @@
             self,
             count=count,
             type=type,
             search_query=search_query,
             extraParams=extraParams,
         )
 
-    def getWorkspaces(self, count=100, search_query=None, extraParams={}):
+    def getWorkspaces(self, count=100, search_query=UNSPECIFIED, extraParams={}):
         """
         Retrieve a list of a user's Workspaces on Labstep,
         which can be filtered using the parameters:
 
         Parameters
         ----------
         count (int)
@@ -692,18 +693,18 @@
         import labstep.entities.workspace.repository as workspaceRepository
 
         return workspaceRepository.getWorkspaces(
             self, count=count, search_query=search_query, extraParams=extraParams
         )
 
     @deprecated(version='3.0.3', reason="You should use workspace.getFiles instead")
-    def getFiles(self, count=100, search_query=None, file_type=None, extraParams={}):
+    def getFiles(self, count=100, search_query=UNSPECIFIED, file_type=UNSPECIFIED, extraParams={}):
         return []
 
-    def getDevices(self, count=100, search_query=None, extraParams={}):
+    def getDevices(self, count=100, search_query=UNSPECIFIED, extraParams={}):
         """
         Retrieve a list of a User's Devices
         across all Workspaces on Labstep,
         which can be filtered using the parameters:
 
         Parameters
         ----------
@@ -727,15 +728,15 @@
 
         return deviceRepository.getDevices(
             self, count=count, search_query=search_query, extraParams=extraParams
         )
 
     # newEntity()
 
-    def newExperiment(self, name, entry=None, extraParams={}):
+    def newExperiment(self, name, entry=UNSPECIFIED, extraParams={}):
         """
         Create a new Labstep Experiment.
 
         Parameters
         ----------
         name (str)
             Give your Experiment a name.
@@ -779,15 +780,15 @@
 
             entity = user.newProtocol(name='Synthesising Aspirin')
         """
         import labstep.entities.protocol.repository as protocolRepository
 
         return protocolRepository.newProtocol(self, name, extraParams=extraParams)
 
-    def newResource(self, name, resource_category_id=None, extraParams={}):
+    def newResource(self, name, resource_category_id=UNSPECIFIED, extraParams={}):
         """
         Create a new Labstep Resource.
 
         Parameters
         ----------
         name (str)
             Give your Resource a name.
@@ -832,15 +833,15 @@
         """
         import labstep.entities.resourceCategory.repository as resourceCategoryRepository
 
         return resourceCategoryRepository.newResourceCategory(
             self, name, extraParams=extraParams
         )
 
-    def newResourceLocation(self, name, outer_location_id=None, extraParams={}):
+    def newResourceLocation(self, name, outer_location_id=UNSPECIFIED, extraParams={}):
         """
         Create a new Labstep ResourceLocation.
 
         Parameters
         ----------
         name (str)
             Give your ResourceLocation a name.
@@ -947,15 +948,15 @@
 
             entity = user.newWorkspace(name='Aspirin Project')
         """
         import labstep.entities.workspace.repository as workspaceRepository
 
         return workspaceRepository.newWorkspace(self, name, extraParams=extraParams)
 
-    def newFile(self, filepath=None, rawData=None, extraParams={}):
+    def newFile(self, filepath=UNSPECIFIED, rawData=UNSPECIFIED, extraParams={}):
         """
         Upload a file to the Labstep entity Data.
 
         Parameters
         ----------
         filepath (str)
             The filepath to the file to attach.
```

### Comparing `labstep-3.8.0/labstep/entities/user/repository.py` & `labstep-3.9.0/labstep/entities/user/repository.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
 
 import json
-import urllib.parse
+from labstep.constants import UNSPECIFIED
 from labstep.entities.user.model import User
 from labstep.service.config import configService
 from labstep.service.helpers import url_join
 from labstep.service.request import requestService
 
 
 def getUser(username, apikey):
@@ -18,29 +18,29 @@
 
 
 def newUser(
     first_name,
     last_name,
     email,
     password,
-    share_link_token=None,
+    share_link_token=UNSPECIFIED,
     extraParams={},
 ):
     url = url_join(configService.getHost(), "public-api/user")
     params = {
         "first_name": first_name,
         "last_name": last_name,
         "email": email,
         "password": password,
         "share_link_token": share_link_token,
         **extraParams,
     }
 
     params = dict(
-        filter(lambda field: field[1] is not None, params.items()))
+        filter(lambda field: field[1] is not UNSPECIFIED, params.items()))
 
     response = requestService.post(url=url, json=params, headers=None)
     return User(json.loads(response.content))
 
 
 def authenticate(username, apikey):
     url = url_join(configService.getHost(), "api/generic/user/info")
```

### Comparing `labstep-3.8.0/labstep/entities/workspace/model.py` & `labstep-3.9.0/labstep/entities/workspace/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Author: Barney Walker <barney@labstep.com>
 
 from labstep.entities.autoshare.model import Autoshare
 from labstep.generic.entity.model import Entity
 from labstep.entities.workspaceMember.model import WorkspaceMember
 from labstep.entities.sharelink.model import Sharelink
 from labstep.service.helpers import getTime
+from labstep.constants import UNSPECIFIED
 
 
 class Workspace(Entity):
     """
     Represents a Labstep Workspace.
 
     To see all attributes of the workspace run
@@ -21,15 +22,15 @@
     ::
         print(my_workspace.name)
         print(my_workspace.id)
     """
 
     __entityName__ = "group"
 
-    def edit(self, name=None, extraParams={}):
+    def edit(self, name=UNSPECIFIED, extraParams={}):
         """
         Edit an existing Workspace.
 
         Parameters
         ----------
         name (str)
             The new name of the Workspace.
@@ -65,19 +66,19 @@
 
         return workspaceRepository.editWorkspace(self, deleted_at=getTime())
 
     # getMany()
     def getExperiments(
         self,
         count=100,
-        search_query=None,
-        created_at_from=None,
-        created_at_to=None,
-        tag_id=None,
-        collection_id=None,
+        search_query=UNSPECIFIED,
+        created_at_from=UNSPECIFIED,
+        created_at_to=UNSPECIFIED,
+        tag_id=UNSPECIFIED,
+        collection_id=UNSPECIFIED,
         extraParams={},
     ):
         """
         Retrieve a list of Experiments within this specific Workspace,
         which can be filtered using the parameters:
 
         Parameters
@@ -125,19 +126,19 @@
             collection_id=collection_id,
             extraParams=extraParams,
         )
 
     def getProtocols(
         self,
         count=100,
-        search_query=None,
-        created_at_from=None,
-        created_at_to=None,
-        tag_id=None,
-        collection_id=None,
+        search_query=UNSPECIFIED,
+        created_at_from=UNSPECIFIED,
+        created_at_to=UNSPECIFIED,
+        tag_id=UNSPECIFIED,
+        collection_id=UNSPECIFIED,
         extraParams={},
     ):
         """
         Retrieve a list of Protocols within this specific Workspace,
         which can be filtered using the parameters:
 
         Parameters
@@ -182,15 +183,15 @@
             created_at_from=created_at_from,
             created_at_to=created_at_to,
             tag_id=tag_id,
             collection_id=collection_id,
             extraParams=extraParams,
         )
 
-    def getResources(self, count=100, search_query=None, tag_id=None, extraParams={}):
+    def getResources(self, count=100, search_query=UNSPECIFIED, tag_id=UNSPECIFIED, extraParams={}):
         """
         Retrieve a list of Resources within this specific Workspace,
         which can be filtered using the parameters:
 
         Parameters
         ----------
         count (int)
@@ -217,15 +218,15 @@
         extraParams = {"group_id": self.id, **extraParams}
 
         return resourceRepository.getResources(
             self.__user__, count, search_query, tag_id, extraParams=extraParams
         )
 
     def getResourceCategorys(
-        self, count=100, search_query=None, tag_id=None, extraParams={}
+        self, count=100, search_query=UNSPECIFIED, tag_id=UNSPECIFIED, extraParams={}
     ):
         """
         Retrieve a list of Resource Categories within this specific Workspace,
         which can be filtered using the parameters:
 
         Parameters
         ----------
@@ -252,15 +253,15 @@
 
         extraParams = {"group_id": self.id, **extraParams}
 
         return resourceCategoryRepository.getResourceCategorys(
             self.__user__, count, search_query, tag_id, extraParams=extraParams
         )
 
-    def getResourceLocations(self, count=100, search_query=None, extraParams={}):
+    def getResourceLocations(self, count=100, search_query=UNSPECIFIED, extraParams={}):
         """
         Retrieve a list of Resource Locations within this specific Workspace,
         which can be filtered using the parameters:
 
         Parameters
         ----------
         count (int)
@@ -284,15 +285,15 @@
 
         extraParams = {"group_id": self.id, **extraParams}
 
         return resourceLocationRepository.getResourceLocations(
             self.__user__, count, search_query, extraParams=extraParams
         )
 
-    def getResourceItems(self, count=100, search_query=None, extraParams={}):
+    def getResourceItems(self, count=100, search_query=UNSPECIFIED, extraParams={}):
         """
         Retrieve a list of ResourceItems in a workspace on Labstep.
 
         Parameters
         ----------
         count (int)
             The number of ResourceItems to retrieve.
@@ -314,15 +315,15 @@
         extraParams = {"group_id": self.id, **extraParams}
 
         return resourceItemRepository.getResourceItems(
             self.__user__, count=count, search_query=search_query, extraParams=extraParams
         )
 
     def getOrderRequests(
-        self, count=100, name=None, status=None, tag_id=None, extraParams={}
+        self, count=100, name=UNSPECIFIED, status=UNSPECIFIED, tag_id=UNSPECIFIED, extraParams={}
     ):
         """
         Retrieve a list of Order Requests within this specific Workspace,
         which can be filtered using the parameters:
 
         Parameters
         ----------
@@ -352,15 +353,15 @@
             count=count,
             search_query=name,
             status=status,
             tag_id=tag_id,
             extraParams=extraParams,
         )
 
-    def getTags(self, count=1000, search_query=None, type=None, extraParams={}):
+    def getTags(self, count=1000, search_query=UNSPECIFIED, type=UNSPECIFIED, extraParams={}):
         """
         Retrieve a list of Tags within this specific Workspace,
         which can be filtered using the parameters:
 
         Parameters
         ----------
         count (int)
@@ -412,15 +413,15 @@
         ::
 
             newMember = workspace.addMember(user_id=123)
         """
         import labstep.entities.workspaceMember.repository as workspaceMemberRepository
         return workspaceMemberRepository.addMember(self.__user__, workspace_id=self.id, user_id=user_id)
 
-    def getMembers(self, count=100, search_query=None, extraParams={}):
+    def getMembers(self, count=100, search_query=UNSPECIFIED, extraParams={}):
         """
         Retrieve a list of the members of the workspace.
 
         Parameters
         ----------
         count (int)
             The number of members to retrieve.
@@ -438,15 +439,15 @@
         ::
 
             members = workspace.getMembers(search_query='john')
         """
         import labstep.entities.workspaceMember.repository as workspaceMemberRepository
         return workspaceMemberRepository.getMembers(self.__user__, workspace_id=self.id, search_query=search_query, extraParams=extraParams)
 
-    def getFiles(self, count=100, search_query=None, file_type=None, extraParams={}):
+    def getFiles(self, count=100, search_query=UNSPECIFIED, file_type=UNSPECIFIED, extraParams={}):
         """
         Retrieve a list of Files in the Workspace on Labstep,
         which can be filtered using the parameters:
 
         Parameters
         ----------
         count (int)
@@ -473,15 +474,15 @@
 
         extraParams = {"group_id": self.id, **extraParams}
 
         return fileRepository.getFiles(
             self.__user__, count, search_query, file_type, extraParams=extraParams
         )
 
-    def getDevices(self, count=100, search_query=None, extraParams={}):
+    def getDevices(self, count=100, search_query=UNSPECIFIED, extraParams={}):
         """
         Retrieve a list of Devices within this specific Workspace,
         which can be filtered using the parameters:
 
         Parameters
         ----------
         count (int)
@@ -544,15 +545,15 @@
 
         """
 
         import labstep.entities.sharelink.repository as shareLinkRepository
         return shareLinkRepository.getSharelink(self)
 
     def getCollections(
-        self, count=1000, search_query=None, type="experiment", extraParams={}
+        self, count=1000, search_query=UNSPECIFIED, type="experiment", extraParams={}
     ):
         """
         Retrieve a list of Collections within this specific Workspace,
         which can be filtered using the parameters:
 
         Parameters
         ----------
@@ -615,15 +616,15 @@
         """
         member = WorkspaceMember(self.logged_user_user_group, self.__user__)
         import labstep.generic.entity.repository as entityRepository
 
         return entityRepository.editEntity(member, {"is_home": True})
 
     def setAutosharing(
-        self, experiment_sharing=None, protocol_sharing=None, resource_sharing=None
+        self, experiment_sharing=UNSPECIFIED, protocol_sharing=UNSPECIFIED, resource_sharing=UNSPECIFIED
     ):
         """
         Parameters
         ----------
         experiment_sharing (str)
             Automatically share experiments
             you create and own with this workspace. Set to True or False
```

### Comparing `labstep-3.8.0/labstep/entities/workspaceMember/model.py` & `labstep-3.9.0/labstep/entities/workspaceMember/model.py`

 * *Files identical despite different names*

### Comparing `labstep-3.8.0/labstep/entities/workspaceMember/repository.py` & `labstep-3.9.0/labstep/entities/workspaceMember/repository.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 # Author: Barney Walker <barney@labstep.com>
 
 from labstep.entities.workspaceMember.model import WorkspaceMember
 import labstep.generic.entity.repository as entityRepository
 from labstep.service.helpers import url_join, getHeaders
 from labstep.service.config import configService
 from labstep.service.request import requestService
+from labstep.constants import UNSPECIFIED
 
 
-def getMembers(user, workspace_id, count=100, search_query=None, extraParams={}):
+def getMembers(user, workspace_id, count=100, search_query=UNSPECIFIED, extraParams={}):
 
     params = {"group_id": workspace_id,
               "search_query_user": search_query, **extraParams}
 
     return entityRepository.getEntities(user, WorkspaceMember, count, params)
```

### Comparing `labstep-3.8.0/labstep/generic/entity/model.py` & `labstep-3.9.0/labstep/generic/entity/model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
 
 import inspect
-import json
 import pprint
 from labstep.service.helpers import update
+from labstep.constants import UNSPECIFIED
 
 
 class Entity:
 
     def __init__(self, data, user):
         self.__user__ = user
         self.__data__ = data
@@ -21,26 +21,29 @@
             self, lambda a: not (inspect.isroutine(a)))
         entity_attributes = {
             k: v for k, v in all_attributes if not (k.startswith("__"))
         }
         pp = pprint.PrettyPrinter(indent=1)
         return pp.pformat(entity_attributes)
 
+    def __getitem__(self, key):
+        return getattr(self, key, None)
+
     def update(self):
         """
         Fetches the most up-to-date version of the entity from Labstep.
         """
         import labstep.generic.entity.repository as entityRepository
 
         data = entityRepository.getEntity(
             self.__user__, type(self), self.id).__data__
         self.__init__(data, self.__user__)
         return self
 
-    def export(self, rootPath, folderName=None):
+    def export(self, rootPath, folderName=UNSPECIFIED):
         """
         Export the entity to the directory specified. 
 
         Parameters
         -------
         path (str)
             The path to the directory to save the experiment.
```

### Comparing `labstep-3.8.0/labstep/generic/entity/repository.py` & `labstep-3.9.0/labstep/generic/entity/repository.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 
 import json
 from pathlib import Path
 from pathvalidate import sanitize_filepath
 from labstep.generic.entityList.model import EntityList
 from labstep.service.config import configService
 from labstep.service.helpers import (
+    filterUnspecified,
     url_join,
     getHeaders,
 )
 from labstep.service.request import requestService
 from labstep.config.export import entityNameInFolderName
+from labstep.constants import UNSPECIFIED
 
 
 def getLegacyEntity(user, entityClass, id):
     headers = getHeaders(user=user)
     url = url_join(configService.getHost(), "/api/generic/",
                    entityClass.__entityName__, str(id))
     response = requestService.get(url, headers=headers)
@@ -36,41 +38,46 @@
     url = url_join(configService.getHost(), "/api/generic/",
                    entityClass.__entityName__)
     response = requestService.get(url, headers=headers, params=params)
     return entityClass(json.loads(response.content), user)
 
 
 def getEntities(user, entityClass, count, filterParams={}):
-    countParameter = min(count, 50) if count is not None else None
+    countParameter = min(
+        count, 50) if count is not UNSPECIFIED else UNSPECIFIED
     searchParams = {"search": 1, "cursor": -1, "count": countParameter}
 
     params = {**searchParams, **filterParams}
 
     headers = getHeaders(user=user)
     url = url_join(configService.getHost(), "/api/generic/",
                    entityClass.__entityName__)
     response = requestService.get(url, params=params, headers=headers)
     resp = json.loads(response.content)
     items = resp["items"]
-    expectedResults = min(
-        resp["total"], count) if count is not None else resp["total"]
-    while len(items) < expectedResults:
+
+    while resp["next_cursor"] != '-1':
+        if count is not UNSPECIFIED:
+            remainingItems = count - len(items)
+            params["count"] = min(remainingItems, 50)
+            if remainingItems <= 0:
+                break
+
         params["cursor"] = resp["next_cursor"]
         response = requestService.get(url, headers=headers, params=params)
         resp = json.loads(response.content)
         items.extend(resp["items"])
+
     return EntityList(items, entityClass, user)
 
 
 def newEntity(user, entityClass, fields):
     headers = getHeaders(user=user)
     url = url_join(configService.getHost(), "/api/generic/",
                    entityClass.__entityName__)
-    fields = dict(
-        filter(lambda field: field[1] is not None, fields.items()))
 
     if "group_id" not in fields and getattr(
         entityClass, "__hasParentGroup__", False
     ):
         fields["group_id"] = user.activeWorkspace
 
     response = requestService.post(url, headers=headers, json=fields)
@@ -98,35 +105,30 @@
     response = requestService.post(
         url, headers=headers, json={"items": items, "group_id": user.activeWorkspace})
     entities = json.loads(response.content)
     return EntityList(entities, entityClass, user)
 
 
 def editEntity(entity, fields):
-    # Filter the 'fields' dictionary by removing {'fields': None}
-    # to preserve the existing data in the 'fields', otherwise
-    # the 'fields' will be overwritten to 'None'.
     identifier = entity.guid if getattr(
         entity, "__hasGuid__", None) and hasattr(entity, 'guid') else entity.id
 
-    newFields = dict(
-        filter(lambda field: field[1] is not None, fields.items()))
     headers = getHeaders(entity.__user__)
     url = url_join(configService.getHost(), "/api/generic/",
                    entity.__entityName__, str(identifier))
-    response = requestService.put(url, json=newFields, headers=headers)
+    response = requestService.put(url, json=fields, headers=headers)
     entity.__init__(json.loads(response.content), entity.__user__)
     return entity
 
 
-def exportEntity(entity, rootPath, folderName=None):
+def exportEntity(entity, rootPath, folderName=UNSPECIFIED):
 
     from labstep.entities.file.model import File
 
-    if folderName is None:
+    if folderName is UNSPECIFIED:
         if entityNameInFolderName:
             folderName = f'{entity.id} - {entity.name}' if hasattr(
                 entity, 'name') else f'{entity.id}'
         else:
             folderName = str(entity.id)
 
     entityDir = Path(rootPath).joinpath(sanitize_filepath(folderName))
```

### Comparing `labstep-3.8.0/labstep/generic/entityList/model.py` & `labstep-3.9.0/labstep/generic/entityList/model.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,10 +10,10 @@
         if len(hits) == 0:
             return None
 
         if len(hits) == 1:
             return hits[0]
 
         if len(hits) > 1:
-            print('Warning: multiple matches found')
+            print(f'Warning: multiple matches found for "{key}"')
 
             return hits[0]
```

### Comparing `labstep-3.8.0/labstep/generic/entityWithComments/model.py` & `labstep-3.9.0/labstep/generic/entityWithComments/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
 
 from labstep.generic.entity.model import Entity
+from labstep.constants import UNSPECIFIED
 
 
 class EntityWithComments(Entity):
 
-    def addComment(self, body, filepath=None, extraParams={}):
+    def addComment(self, body, filepath=UNSPECIFIED, extraParams={}):
         """
         Add a comment and/or file to a Labstep Entity.
 
         Parameters
         ----------
         body (str)
             The body of the comment.
```

### Comparing `labstep-3.8.0/labstep/generic/entityWithSharing/model.py` & `labstep-3.9.0/labstep/generic/entityWithSharing/model.py`

 * *Files identical despite different names*

### Comparing `labstep-3.8.0/labstep/generic/entityWithTags/model.py` & `labstep-3.9.0/labstep/generic/entityWithTags/model.py`

 * *Files identical despite different names*

### Comparing `labstep-3.8.0/labstep/service/config.py` & `labstep-3.9.0/labstep/service/config.py`

 * *Files identical despite different names*

### Comparing `labstep-3.8.0/labstep/service/helpers.py` & `labstep-3.9.0/labstep/service/helpers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Author: Barney Walker <barney@labstep.com>
-
+import pandas
 from datetime import datetime
 from time import gmtime, strftime
-from labstep.constants.version import VERSION
-import pandas
+from labstep.constants import VERSION, UNSPECIFIED
 
 
 def url_join(*args):
     """
     Join a set of args with a slash (/) between them. Instead of
     checking for the presence of a slash, the slashes from both sides
     of each arg will be .strip() and then args .join() together.
@@ -58,53 +57,67 @@
     return timestamp
 
 
 def formatDate(date, time=True):
     if date is None:
         return None
 
+    if date is UNSPECIFIED:
+        return UNSPECIFIED
+
     format = '%Y-%m-%d %H:%M:%S' if time else '%Y-%m-%d'
 
     return datetime.strptime(date, '%Y-%m-%dT%H:%M:%S+00:00').strftime(format)
 
 
 def handleDate(date):
     """
     Returns
     -------
         The datetime for in json serializable format.
     """
     if date is None:
         return None
 
+    if date is UNSPECIFIED:
+        return UNSPECIFIED
+
     for fmt in ('%Y-%m-%d', '%Y-%m-%d %H:%M', '%Y-%m-%d %H:%M:%S'):
         try:
             return datetime.strptime(date, fmt).strftime('%Y-%m-%dT%H:%M:%S+00:00')
         except ValueError:
             pass
     raise ValueError(
         'Please Specify date in format: YY-MM-DD or YY-MM-DD HH:MM:SS')
 
 
 def handleString(string):
     """
     Casts to string or returns None
     """
-    return str(string) if string else None
+    if string is None:
+        return None
+    if string is UNSPECIFIED:
+        return UNSPECIFIED
+
+    return str(string)
 
 
 def handleKeyword(string):
     """
     Returns
     -------
     string
         The string in lowercase, and any whitespace replaced with '_'.
     """
     if string is None:
         return None
+    if string is UNSPECIFIED:
+        return UNSPECIFIED
+
     else:
         return string.lower().replace(" ", "_")
 
 
 def update(entity, newData):
     """
     Returns
@@ -125,23 +138,44 @@
     else:
         return {
             "apikey": user.api_key,
             "User-Agent": f"Python SDK {VERSION}"
         }
 
 
+def boolToString(kv):
+    """ convert bool values to 'true'/'false' strings for json compat """
+    def enc(x): return x if not isinstance(
+        x, bool) else 'true' if x else 'false'
+
+    return None if kv is None else {k: enc(v) for k, v in kv.items()}
+
+
+def filterUnspecified(obj):
+    return None if obj is None else {k: v for (k, v) in obj.items() if v is not UNSPECIFIED}
+
+
 def getKeyValues(obj):
     return obj.items() if isinstance(obj, dict) else enumerate(obj)
 
 
+def getCellValue(cell):
+    if 'value' not in cell:
+        return None
+    if isinstance(cell['value'], str):
+        return str(cell['value']).strip()
+
+    return cell['value']
+
+
 def dataTableToDataFrame(dataTable):
 
     values = {
         str(rowKey): {
-            str(columnKey): str(cell['value']).strip() if isinstance(cell['value'], str) else cell['value']
+            str(columnKey): getCellValue(cell)
             for (columnKey, cell) in getKeyValues(row)
         } for (rowKey, row) in getKeyValues(dataTable)
     }
 
     header = values.pop('0')
 
     df = pandas.DataFrame(values).T.rename(columns=header)
```

### Comparing `labstep-3.8.0/labstep/service/htmlExport.py` & `labstep-3.9.0/labstep/service/htmlExport.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 from labstep.service.helpers import (
     url_join,
     getHeaders,
 )
 
 
 class HTMLExportService:
-    def getHTML(self, entity):
+    def getHTML(self, entity, withImages=False):
         """
         Gets HTML summary of experiments / protocols.
 
         """
         headers = getHeaders(entity.__user__)
 
         body = {
             "group_id": entity.__user__.activeWorkspace,
             "query_entity_name": entity.__entityName__.replace("-", "_"),
             "query_parameters": {
                 "id": entity.id
             },
-            "type": "html"
+            "type": "html_file" if withImages else "html"
         }
 
         url = url_join(configService.getHost(), 'api/generic', 'entity-export')
         response = requestService.post(url, json=body, headers=headers)
 
         return json.loads(response.content)['html']
```

### Comparing `labstep-3.8.0/labstep/service/htmlToProseMirror.py` & `labstep-3.9.0/labstep/service/htmlToProseMirror.py`

 * *Files identical despite different names*

### Comparing `labstep-3.8.0/labstep/service/jupyter.py` & `labstep-3.9.0/labstep/service/jupyter.py`

 * *Files identical despite different names*

### Comparing `labstep-3.8.0/labstep/service/request.py` & `labstep-3.9.0/labstep/service/request.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # TODO Implement routing name
 # Example: url = url_join(configService.getHost(), "api/generic/share-link/email")
 
 import os
 import requests
 from requests.adapters import HTTPAdapter
 from urllib3.util.retry import Retry
-from labstep.service.helpers import handleError
+from labstep.service.helpers import boolToString, filterUnspecified, handleError
 
 DEFAULT_TIMEOUT = 60  # seconds
 
 
 class TimeoutHTTPAdapter(HTTPAdapter):
     def __init__(self, *args, **kwargs):
         self.timeout = DEFAULT_TIMEOUT
@@ -40,36 +40,30 @@
 # Mount it for both http and https usage
 adapter = TimeoutHTTPAdapter(timeout=60, max_retries=retry_strategy)
 http.hooks["response"] = [handleError]
 http.mount("https://", adapter)
 http.mount("http://", adapter)
 
 
-def encode_boolean_values(kv):
-    """ convert bool values to 'true'/'false' strings for json compat """
-    def enc(x): return x if not isinstance(
-        x, bool) else 'true' if x else 'false'
-
-    return None if kv is None else {k: enc(v) for k, v in kv.items()}
-
-
 class RequestService:
     def get(self, url, headers, params=None):
+
         response = http.get(url, headers=headers,
-                            params=encode_boolean_values(params))
+                            params=boolToString(
+                                filterUnspecified(params)))
         return response
 
     def post(self, url, headers, json=None, files=None, data=None):
         response = http.post(
-            url, headers=headers, json=json, files=files, data=data
+            url, headers=headers, json=filterUnspecified(json), files=files, data=data
         )
         return response
 
     def put(self, url, headers, json=None):
-        response = http.put(url, headers=headers, json=json)
+        response = http.put(url, headers=headers, json=filterUnspecified(json))
         return response
 
     def delete(self, url, headers, json=None):
         response = http.delete(url, headers=headers, json=json)
         return response
```

### Comparing `labstep-3.8.0/labstep.egg-info/PKG-INFO` & `labstep-3.9.0/labstep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labstep
-Version: 3.8.0
+Version: 3.9.0
 Summary: Python SDK for working with the Labstep API
 Home-page: http://github.com/Labstep/labstepPy
 Author: Barney Walker
 Author-email: barney@labstep.com
 License: MIT
 Platform: UNKNOWN
```

### Comparing `labstep-3.8.0/labstep.egg-info/SOURCES.txt` & `labstep-3.9.0/labstep.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 labstep.egg-info/PKG-INFO
 labstep.egg-info/SOURCES.txt
 labstep.egg-info/dependency_links.txt
 labstep.egg-info/not-zip-safe
 labstep.egg-info/requires.txt
 labstep.egg-info/top_level.txt
 labstep/config/export.py
+labstep/constants/__init__.py
+labstep/constants/unspecified.py
 labstep/constants/version.py
 labstep/converter/__init__.py
 labstep/converter/htmlToProseMirror.py
 labstep/entities/autoshare/model.py
 labstep/entities/autoshare/repository.py
 labstep/entities/collection/model.py
 labstep/entities/collection/repository.py
@@ -21,14 +23,16 @@
 labstep/entities/device/repository.py
 labstep/entities/deviceData/model.py
 labstep/entities/deviceData/repository.py
 labstep/entities/experiment/model.py
 labstep/entities/experiment/repository.py
 labstep/entities/experimentDataField/model.py
 labstep/entities/experimentDataField/repository.py
+labstep/entities/experimentLink/model.py
+labstep/entities/experimentLink/repository.py
 labstep/entities/experimentMaterial/model.py
 labstep/entities/experimentMaterial/repository.py
 labstep/entities/experimentProtocol/model.py
 labstep/entities/experimentProtocol/repository.py
 labstep/entities/experimentSignature/model.py
 labstep/entities/experimentSignature/repository.py
 labstep/entities/experimentSignatureRequest/model.py
@@ -102,11 +106,12 @@
 labstep/generic/entityWithSharing/model.py
 labstep/generic/entityWithTags/model.py
 labstep/generic/entityWithTags/repository.py
 labstep/service/__init__.py
 labstep/service/config.py
 labstep/service/helpers.py
 labstep/service/htmlExport.py
+labstep/service/htmlToPDF.py
 labstep/service/htmlToProseMirror.py
 labstep/service/jupyter.py
 labstep/service/ping.py
 labstep/service/request.py
```

### Comparing `labstep-3.8.0/setup.py` & `labstep-3.9.0/setup.py`

 * *Files identical despite different names*

