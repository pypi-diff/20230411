# Comparing `tmp/property-lister-1.6.tar.gz` & `tmp/property-lister-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "property-lister-1.6.tar", last modified: Sun Apr  9 10:22:10 2023, max compression
+gzip compressed data, was "property-lister-1.7.tar", last modified: Tue Apr 11 15:32:45 2023, max compression
```

## Comparing `property-lister-1.6.tar` & `property-lister-1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 10:22:10.452973 property-lister-1.6/
--rwxrwx---   0 root         (0) root         (0)     1090 2023-04-08 16:38:41.000000 property-lister-1.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2614 2023-04-09 10:22:10.448971 property-lister-1.6/PKG-INFO
--rwxrwx---   0 root         (0) root         (0)     2229 2023-04-08 16:40:20.000000 property-lister-1.6/README.md
--rwxrwx---   0 root         (0) root         (0)      728 2023-04-08 16:40:03.000000 property-lister-1.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-09 10:22:10.452973 property-lister-1.6/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 10:22:10.448971 property-lister-1.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 10:22:10.448971 property-lister-1.6/src/property_lister/
--rwxrwx---   0 root         (0) root         (0)        0 2023-04-08 16:38:41.000000 property-lister-1.6/src/property_lister/__init__.py
--rwxrwx---   0 root         (0) root         (0)     9038 2023-04-09 10:21:14.000000 property-lister-1.6/src/property_lister/property_lister.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 10:22:10.448971 property-lister-1.6/src/property_lister.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2614 2023-04-09 10:22:10.000000 property-lister-1.6/src/property_lister.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      363 2023-04-09 10:22:10.000000 property-lister-1.6/src/property_lister.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 10:22:10.000000 property-lister-1.6/src/property_lister.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-09 10:22:10.000000 property-lister-1.6/src/property_lister.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-09 10:22:10.000000 property-lister-1.6/src/property_lister.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-09 10:22:10.000000 property-lister-1.6/src/property_lister.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 15:32:45.582714 property-lister-1.7/
+-rwxrwx---   0 root         (0) root         (0)     1090 2023-04-09 10:26:05.000000 property-lister-1.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2852 2023-04-11 15:32:45.582714 property-lister-1.7/PKG-INFO
+-rwxrwx---   0 root         (0) root         (0)     2479 2023-04-11 15:29:00.000000 property-lister-1.7/README.md
+-rwxrwx---   0 root         (0) root         (0)      728 2023-04-11 14:51:09.000000 property-lister-1.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 15:32:45.582714 property-lister-1.7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 15:32:45.582714 property-lister-1.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 15:32:45.582714 property-lister-1.7/src/property_lister/
+-rwxrwx---   0 root         (0) root         (0)        0 2023-04-09 10:26:05.000000 property-lister-1.7/src/property_lister/__init__.py
+-rwxrwx---   0 root         (0) root         (0)     9299 2023-04-11 15:32:02.000000 property-lister-1.7/src/property_lister/property_lister.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 15:32:45.582714 property-lister-1.7/src/property_lister.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2852 2023-04-11 15:32:45.000000 property-lister-1.7/src/property_lister.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      363 2023-04-11 15:32:45.000000 property-lister-1.7/src/property_lister.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 15:32:45.000000 property-lister-1.7/src/property_lister.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-11 15:32:45.000000 property-lister-1.7/src/property_lister.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-11 15:32:45.000000 property-lister-1.7/src/property_lister.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-11 15:32:45.000000 property-lister-1.7/src/property_lister.egg-info/top_level.txt
```

### Comparing `property-lister-1.6/LICENSE` & `property-lister-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `property-lister-1.6/PKG-INFO` & `property-lister-1.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,86 +1,85 @@
-Metadata-Version: 2.1
-Name: property-lister
-Version: 1.6
-Summary: Extract property list files from an SQLite unencrypted database file.
-Author: Ivan Sincek
-Project-URL: Homepage, https://github.com/ivan-sincek/property-lister
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Property Lister
-
-Extract and convert property list files from SQLite unencrypted database files and from other property list files.
-
-Tested on Kali Linux v2023.1 (64-bit).
-
-Made for educational purposes. I hope it will help!
-
-## Table of Contents
-
-* [How to Install](#how-to-install)
-* [How to Build and Install Manually](#how-to-build-and-install-manually)
-* [Extract Property List Files](#extract-property-list-files)
-* [Usage](#usage)
-
-## How to Install
-
-```bash
-pip3 install property-lister
-
-pip3 install --upgrade property-lister
-```
-
-## How to Build and Install Manually
-
-Run the following commands:
-
-```bash
-git clone https://github.com/ivan-sincek/property-lister && cd property-lister
-
-python3 -m pip install --upgrade build
-
-python3 -m build
-
-python3 -m pip install dist/property_lister-1.6-py3-none-any.whl
-```
-
-## Extract Property List Files
-
-```fundamental
-scp root@192.168.1.10:/var/mobile/Containers/Data/Application/YYY...YYY/Library/Caches/com.someapp.dev/Cache.db ./
-
-property-lister -db Cache.db -o results
-```
-
-Check my other project on how to [find files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#3-search-for-files-and-directories) and on how to [extract sensitive data from files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#4-inspect-files).
-
-## Usage
-
-```fundamental
-Property Lister v1.6 ( github.com/ivan-sincek/property-lister )
-
---- Extract from an SQLite unencrypted database file ---
-Usage:   property-lister -db database -o out
-Example: property-lister -db Cache.db -o results
-
---- Extract from a property list file ---
-Usage:   property-lister -pl property-list -o out
-Example: property-lister -pl Info.plist    -o results
-
-DESCRIPTION
-    Extract and convert property list files
-DATABASE
-    SQLite unencrypted database file, or directory containing multiple files
-    -db <database> - Cache.db | databases | etc.
-PROPERTY LIST
-    Property list file, or directory containing multiple files
-    -pl <property-list> - Info.plist | plists | etc.
-OUT
-    Output directory
-    All extracted propery list files will be saved in this directory
-    -o <out> - results | etc.
-```
+# Property Lister
+
+Extract and convert property list files from SQLite database files and from other property list files.
+
+Tested on Kali Linux v2023.1 (64-bit).
+
+Made for educational purposes. I hope it will help!
+
+## Table of Contents
+
+* [How to Install](#how-to-install)
+* [How to Build and Install Manually](#how-to-build-and-install-manually)
+* [Extracting and Converting](#extracting-and-converting)
+* [Usage](#usage)
+
+## How to Install
+
+```bash
+pip3 install property-lister
+
+pip3 install --upgrade property-lister
+```
+
+## How to Build and Install Manually
+
+Run the following commands:
+
+```bash
+git clone https://github.com/ivan-sincek/property-lister && cd property-lister
+
+python3 -m pip install --upgrade build
+
+python3 -m build
+
+python3 -m pip install dist/property_lister-1.7-py3-none-any.whl
+```
+
+## Extracting and Converting
+
+Extract and convert property list files inside Cache.db unencrypted SQLite database file:
+
+```fundamental
+scp root@192.168.1.10:/var/mobile/Containers/Data/Application/YYY...YYY/Library/Caches/com.someapp.dev/Cache.db ./
+
+property-lister -db Cache.db -o results
+```
+
+Extract and convert property list files inside an IPA file:
+
+```fundamental
+unzip someapp.ipa
+
+property-lister -db Payload -o results_db
+
+property-lister -pl Payload -o results_pl
+```
+
+Check my other project on how to [find files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#3-search-for-files-and-directories) and on how to [extract sensitive data from the files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#4-inspect-files).
+
+## Usage
+
+```fundamental
+Property Lister v1.7 ( github.com/ivan-sincek/property-lister )
+
+--- Extract from an SQLite database file ---
+Usage:   property-lister -db database -o out
+Example: property-lister -db Cache.db -o results
+
+--- Extract from a property list file ---
+Usage:   property-lister -pl property-list -o out
+Example: property-lister -pl Info.plist    -o results
+
+DESCRIPTION
+    Extract and convert property list files
+DATABASE
+    SQLite database file, or directory containing multiple files
+    -db <database> - Cache.db | databases | etc.
+PROPERTY LIST
+    Property list file, or directory containing multiple files
+    -pl <property-list> - Info.plist | plists | etc.
+OUT
+    Output directory
+    All extracted propery list files will be saved in this directory
+    -o <out> - results | etc.
+```
```

### Comparing `property-lister-1.6/README.md` & `property-lister-1.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,73 +1,98 @@
-# Property Lister
-
-Extract and convert property list files from SQLite unencrypted database files and from other property list files.
-
-Tested on Kali Linux v2023.1 (64-bit).
-
-Made for educational purposes. I hope it will help!
-
-## Table of Contents
-
-* [How to Install](#how-to-install)
-* [How to Build and Install Manually](#how-to-build-and-install-manually)
-* [Extract Property List Files](#extract-property-list-files)
-* [Usage](#usage)
-
-## How to Install
-
-```bash
-pip3 install property-lister
-
-pip3 install --upgrade property-lister
-```
-
-## How to Build and Install Manually
-
-Run the following commands:
-
-```bash
-git clone https://github.com/ivan-sincek/property-lister && cd property-lister
-
-python3 -m pip install --upgrade build
-
-python3 -m build
-
-python3 -m pip install dist/property_lister-1.6-py3-none-any.whl
-```
-
-## Extract Property List Files
-
-```fundamental
-scp root@192.168.1.10:/var/mobile/Containers/Data/Application/YYY...YYY/Library/Caches/com.someapp.dev/Cache.db ./
-
-property-lister -db Cache.db -o results
-```
-
-Check my other project on how to [find files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#3-search-for-files-and-directories) and on how to [extract sensitive data from files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#4-inspect-files).
-
-## Usage
-
-```fundamental
-Property Lister v1.6 ( github.com/ivan-sincek/property-lister )
-
---- Extract from an SQLite unencrypted database file ---
-Usage:   property-lister -db database -o out
-Example: property-lister -db Cache.db -o results
-
---- Extract from a property list file ---
-Usage:   property-lister -pl property-list -o out
-Example: property-lister -pl Info.plist    -o results
-
-DESCRIPTION
-    Extract and convert property list files
-DATABASE
-    SQLite unencrypted database file, or directory containing multiple files
-    -db <database> - Cache.db | databases | etc.
-PROPERTY LIST
-    Property list file, or directory containing multiple files
-    -pl <property-list> - Info.plist | plists | etc.
-OUT
-    Output directory
-    All extracted propery list files will be saved in this directory
-    -o <out> - results | etc.
-```
+Metadata-Version: 2.1
+Name: property-lister
+Version: 1.7
+Summary: Extract property list files from an SQLite unencrypted database file.
+Author: Ivan Sincek
+Project-URL: Homepage, https://github.com/ivan-sincek/property-lister
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Property Lister
+
+Extract and convert property list files from SQLite database files and from other property list files.
+
+Tested on Kali Linux v2023.1 (64-bit).
+
+Made for educational purposes. I hope it will help!
+
+## Table of Contents
+
+* [How to Install](#how-to-install)
+* [How to Build and Install Manually](#how-to-build-and-install-manually)
+* [Extracting and Converting](#extracting-and-converting)
+* [Usage](#usage)
+
+## How to Install
+
+```bash
+pip3 install property-lister
+
+pip3 install --upgrade property-lister
+```
+
+## How to Build and Install Manually
+
+Run the following commands:
+
+```bash
+git clone https://github.com/ivan-sincek/property-lister && cd property-lister
+
+python3 -m pip install --upgrade build
+
+python3 -m build
+
+python3 -m pip install dist/property_lister-1.7-py3-none-any.whl
+```
+
+## Extracting and Converting
+
+Extract and convert property list files inside Cache.db unencrypted SQLite database file:
+
+```fundamental
+scp root@192.168.1.10:/var/mobile/Containers/Data/Application/YYY...YYY/Library/Caches/com.someapp.dev/Cache.db ./
+
+property-lister -db Cache.db -o results
+```
+
+Extract and convert property list files inside an IPA file:
+
+```fundamental
+unzip someapp.ipa
+
+property-lister -db Payload -o results_db
+
+property-lister -pl Payload -o results_pl
+```
+
+Check my other project on how to [find files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#3-search-for-files-and-directories) and on how to [extract sensitive data from the files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#4-inspect-files).
+
+## Usage
+
+```fundamental
+Property Lister v1.7 ( github.com/ivan-sincek/property-lister )
+
+--- Extract from an SQLite database file ---
+Usage:   property-lister -db database -o out
+Example: property-lister -db Cache.db -o results
+
+--- Extract from a property list file ---
+Usage:   property-lister -pl property-list -o out
+Example: property-lister -pl Info.plist    -o results
+
+DESCRIPTION
+    Extract and convert property list files
+DATABASE
+    SQLite database file, or directory containing multiple files
+    -db <database> - Cache.db | databases | etc.
+PROPERTY LIST
+    Property list file, or directory containing multiple files
+    -pl <property-list> - Info.plist | plists | etc.
+OUT
+    Output directory
+    All extracted propery list files will be saved in this directory
+    -o <out> - results | etc.
+```
```

### Comparing `property-lister-1.6/pyproject.toml` & `property-lister-1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "property-lister"
-version = "1.6"
+version = "1.7"
 authors = [{ name = "Ivan Sincek" }]
 description = "Extract property list files from an SQLite unencrypted database file."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
```

### Comparing `property-lister-1.6/src/property_lister/property_lister.py` & `property-lister-1.7/src/property_lister/property_lister.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,31 +13,31 @@
 start = datetime.datetime.now()
 
 # -------------------------- INFO --------------------------
 
 def basic():
 	global proceed
 	proceed = False
-	print("Property Lister v1.6 ( github.com/ivan-sincek/property-lister )")
+	print("Property Lister v1.7 ( github.com/ivan-sincek/property-lister )")
 	print("")
-	print("--- Extract from an SQLite unencrypted database file ---")
+	print("--- Extract from an SQLite database file ---")
 	print("Usage:   property-lister -db database -o out")
 	print("Example: property-lister -db Cache.db -o results")
 	print("")
 	print("--- Extract from a property list file ---")
 	print("Usage:   property-lister -pl property-list -o out")
 	print("Example: property-lister -pl Info.plist    -o results")
 
 def advanced():
 	basic()
 	print("")
 	print("DESCRIPTION")
 	print("    Extract and convert property list files")
 	print("DATABASE")
-	print("    SQLite unencrypted database file, or directory containing multiple files")
+	print("    SQLite database file, or directory containing multiple files")
 	print("    -db <database> - Cache.db | databases | etc.")
 	print("PROPERTY LIST")
 	print("    Property list file, or directory containing multiple files")
 	print("    -pl <property-list> - Info.plist | plists | etc.")
 	print("OUT")
 	print("    Output directory")
 	print("    All extracted propery list files will be saved in this directory")
@@ -73,18 +73,19 @@
 		overwrite = input("Overwrite the output directory (yes): ").lower()
 	if overwrite == "yes" and remove_directory(directory):
 		success = create_directory(directory)
 	return success
 
 def check_directory_files(directory):
 	tmp = []
-	for file in os.listdir(directory):
-		file = os.path.join(directory, file)
-		if os.path.isfile(file) and os.access(file, os.R_OK) and os.stat(file).st_size > 0:
-			tmp.append(file)
+	for path, dirs, files in os.walk(directory):
+		for file in files:
+			file = os.path.join(path, file)
+			if os.path.isfile(file) and os.access(file, os.R_OK) and os.stat(file).st_size > 0:
+				tmp.append(file)
 	return tmp
 
 # -------------------- MISCELENIOUS END --------------------
 
 # -------------------- VALIDATION BEGIN --------------------
 
 # my own validation algorithm
@@ -148,39 +149,40 @@
 			count += 1
 	return argc - count == argc / 2
 
 # --------------------- VALIDATION END ---------------------
 
 # ----------------- GLOBAL VARIABLES BEGIN -----------------
 
-ext = {"blob": ".blob", "plist": ".plist", "xml": ".plist.xml"}
+ext = {"blob": ".blob", "txt": ".txt", "plist": ".plist", "xml": ".plist.xml"}
 
 # ------------------ GLOBAL VARIABLES END ------------------
 
 # ----------------------- TASK BEGIN -----------------------
 
 def read_database(file):
 	tmp = ""
 	db = None
 	try:
 		db = sqlite3.connect(file)
-		tmp = ("").join(db.iterdump())
+		tmp = ("\n").join(db.iterdump())
 	except sqlite3.DatabaseError:
 		pass
 	finally:
 		if db:
 			db.close()
 	return tmp
 
 # database --> full path (external)
 def dump(database, out):
 	for db in database:
 		count = 0
 		data = read_database(db)
 		if data:
+			open(os.path.join(out, os.path.basename(db) + ext["txt"]), "w").write(data)
 			blobs = re.findall(r"(?<=,x')[\w\d]+", data, re.IGNORECASE)
 			if blobs:
 				for blob in blobs:
 					count += 1
 					open(os.path.join(out, os.path.basename(db) + "." + str(count) + ext["blob"]), "wb").write(binascii.unhexlify(blob))
 
 # file --> full path (external/internal)
@@ -202,24 +204,26 @@
 						biplist.writePlist(string, file)
 						extract(file, out)
 	except (biplist.InvalidPlistException, biplist.NotBinaryPlistException):
 		pass
 
 # file --> full path (internal)
 def convert(file, out):
+	stream = None
 	try:
-		data = None
-		with open(file, "rb") as stream:
-			data = plistlib.load(stream)
-		stream.close()
+		stream = open(file, "rb")
+		data = plistlib.load(stream)
 		if data:
 			open(file, "wb").write(plistlib.dumps(data, fmt = plistlib.FMT_XML))
 			os.rename(file, file.rsplit(".", 1)[0] + ext["xml"])
-	except plistlib.InvalidFileException:
+	except (biplist.InvalidPlistException, biplist.NotBinaryPlistException, TypeError):
 		pass
+	finally:
+		if stream:
+			stream.close()
 
 def main():
 	argc = len(sys.argv) - 1
 
 	if argc == 0:
 		advanced()
 	elif argc == 1:
@@ -237,15 +241,15 @@
 			error("Missing a mandatory option (-pl, -o)", True)
 	else:
 		error("Incorrect usage", True)
 
 	if proceed and check_directory(args["out"]):
 		print("######################################################################")
 		print("#                                                                    #")
-		print("#                        Property Lister v1.6                        #")
+		print("#                        Property Lister v1.7                        #")
 		print("#                                   by Ivan Sincek                   #")
 		print("#                                                                    #")
 		print("# Extract and convert property list files.                           #")
 		print("# GitHub repository at github.com/ivan-sincek/property-lister.       #")
 		print("# Feel free to donate bitcoin at 1BrZM6T7G9RN8vbabnfXu4M6Lpgztq6Y14. #")
 		print("#                                                                    #")
 		print("######################################################################")
@@ -258,13 +262,16 @@
 					convert(os.path.join(args["out"], file), args["out"])
 		elif args["plist"]:
 			for file in args["plist"]:
 				extract(file, args["out"])
 			for file in os.listdir(args["out"]):
 				if file.lower().endswith(ext["plist"]):
 					convert(os.path.join(args["out"], file), args["out"])
+		if not os.listdir(args["out"]):
+			print("No results")
+			remove_directory(args["out"])
 		print(("Script has finished in {0}").format(datetime.datetime.now() - start))
 
 if __name__ == "__main__":
 	main()
 
 # ------------------------ TASK END ------------------------
```

### Comparing `property-lister-1.6/src/property_lister.egg-info/PKG-INFO` & `property-lister-1.7/src/property_lister.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: property-lister
-Version: 1.6
+Version: 1.7
 Summary: Extract property list files from an SQLite unencrypted database file.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/property-lister
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Property Lister
 
-Extract and convert property list files from SQLite unencrypted database files and from other property list files.
+Extract and convert property list files from SQLite database files and from other property list files.
 
 Tested on Kali Linux v2023.1 (64-bit).
 
 Made for educational purposes. I hope it will help!
 
 ## Table of Contents
 
 * [How to Install](#how-to-install)
 * [How to Build and Install Manually](#how-to-build-and-install-manually)
-* [Extract Property List Files](#extract-property-list-files)
+* [Extracting and Converting](#extracting-and-converting)
 * [Usage](#usage)
 
 ## How to Install
 
 ```bash
 pip3 install property-lister
 
@@ -41,44 +41,56 @@
 ```bash
 git clone https://github.com/ivan-sincek/property-lister && cd property-lister
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/property_lister-1.6-py3-none-any.whl
+python3 -m pip install dist/property_lister-1.7-py3-none-any.whl
 ```
 
-## Extract Property List Files
+## Extracting and Converting
+
+Extract and convert property list files inside Cache.db unencrypted SQLite database file:
 
 ```fundamental
 scp root@192.168.1.10:/var/mobile/Containers/Data/Application/YYY...YYY/Library/Caches/com.someapp.dev/Cache.db ./
 
 property-lister -db Cache.db -o results
 ```
 
-Check my other project on how to [find files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#3-search-for-files-and-directories) and on how to [extract sensitive data from files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#4-inspect-files).
+Extract and convert property list files inside an IPA file:
+
+```fundamental
+unzip someapp.ipa
+
+property-lister -db Payload -o results_db
+
+property-lister -pl Payload -o results_pl
+```
+
+Check my other project on how to [find files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#3-search-for-files-and-directories) and on how to [extract sensitive data from the files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#4-inspect-files).
 
 ## Usage
 
 ```fundamental
-Property Lister v1.6 ( github.com/ivan-sincek/property-lister )
+Property Lister v1.7 ( github.com/ivan-sincek/property-lister )
 
---- Extract from an SQLite unencrypted database file ---
+--- Extract from an SQLite database file ---
 Usage:   property-lister -db database -o out
 Example: property-lister -db Cache.db -o results
 
 --- Extract from a property list file ---
 Usage:   property-lister -pl property-list -o out
 Example: property-lister -pl Info.plist    -o results
 
 DESCRIPTION
     Extract and convert property list files
 DATABASE
-    SQLite unencrypted database file, or directory containing multiple files
+    SQLite database file, or directory containing multiple files
     -db <database> - Cache.db | databases | etc.
 PROPERTY LIST
     Property list file, or directory containing multiple files
     -pl <property-list> - Info.plist | plists | etc.
 OUT
     Output directory
     All extracted propery list files will be saved in this directory
```

