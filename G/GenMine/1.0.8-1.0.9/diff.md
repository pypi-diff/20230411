# Comparing `tmp/GenMine-1.0.8.tar.gz` & `tmp/GenMine-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GenMine-1.0.8.tar", last modified: Fri Mar 24 01:19:54 2023, max compression
+gzip compressed data, was "GenMine-1.0.9.tar", last modified: Tue Apr 11 01:37:57 2023, max compression
```

## Comparing `GenMine-1.0.8.tar` & `GenMine-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-03-24 01:19:54.809968 GenMine-1.0.8/
-drwxrwxrwx   0        0        0        0 2023-03-24 01:19:54.785968 GenMine-1.0.8/GenMine/
--rw-rw-rw-   0        0        0    43657 2023-03-24 01:17:41.000000 GenMine-1.0.8/GenMine/GenMine.py
--rw-rw-rw-   0        0        0        0 2022-10-27 01:45:14.000000 GenMine-1.0.8/GenMine/__init__.py
--rw-rw-rw-   0        0        0     1726 2022-11-01 23:36:51.000000 GenMine-1.0.8/GenMine/command.py
--rw-rw-rw-   0        0        0     5293 2022-11-04 00:39:34.000000 GenMine-1.0.8/GenMine/main.py
-drwxrwxrwx   0        0        0        0 2023-03-24 01:19:54.806968 GenMine-1.0.8/GenMine.egg-info/
--rw-rw-rw-   0        0        0      277 2023-03-24 01:19:54.000000 GenMine-1.0.8/GenMine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-03-24 01:19:54.000000 GenMine-1.0.8/GenMine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-24 01:19:54.000000 GenMine-1.0.8/GenMine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-03-24 01:19:54.000000 GenMine-1.0.8/GenMine.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-10-25 05:12:45.000000 GenMine-1.0.8/GenMine.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       68 2023-03-24 01:19:54.000000 GenMine-1.0.8/GenMine.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-24 01:19:54.000000 GenMine-1.0.8/GenMine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2022-02-07 04:16:54.000000 GenMine-1.0.8/LICENSE
--rw-rw-rw-   0        0        0      277 2023-03-24 01:19:54.808968 GenMine-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3278 2023-02-01 06:40:14.000000 GenMine-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-03-24 01:19:54.809968 GenMine-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      741 2023-03-24 00:32:24.000000 GenMine-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 01:37:57.790885 GenMine-1.0.9/
+drwxrwxrwx   0        0        0        0 2023-04-11 01:37:57.764882 GenMine-1.0.9/GenMine/
+-rw-rw-rw-   0        0        0    43616 2023-04-11 01:28:45.000000 GenMine-1.0.9/GenMine/GenMine.py
+-rw-rw-rw-   0        0        0        0 2022-10-27 01:45:14.000000 GenMine-1.0.9/GenMine/__init__.py
+-rw-rw-rw-   0        0        0     1726 2022-11-01 23:36:51.000000 GenMine-1.0.9/GenMine/command.py
+-rw-rw-rw-   0        0        0     5293 2022-11-04 00:39:34.000000 GenMine-1.0.9/GenMine/main.py
+drwxrwxrwx   0        0        0        0 2023-04-11 01:37:57.786883 GenMine-1.0.9/GenMine.egg-info/
+-rw-rw-rw-   0        0        0      277 2023-04-11 01:37:57.000000 GenMine-1.0.9/GenMine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2023-04-11 01:37:57.000000 GenMine-1.0.9/GenMine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 01:37:57.000000 GenMine-1.0.9/GenMine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-11 01:37:57.000000 GenMine-1.0.9/GenMine.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2022-10-25 05:12:45.000000 GenMine-1.0.9/GenMine.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       68 2023-04-11 01:37:57.000000 GenMine-1.0.9/GenMine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-11 01:37:57.000000 GenMine-1.0.9/GenMine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2022-02-07 04:16:54.000000 GenMine-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0      277 2023-04-11 01:37:57.788885 GenMine-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3278 2023-02-01 06:40:14.000000 GenMine-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-11 01:37:57.790885 GenMine-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      741 2023-04-11 01:35:31.000000 GenMine-1.0.9/setup.py
```

### Comparing `GenMine-1.0.8/GenMine/GenMine.py` & `GenMine-1.0.9/GenMine/GenMine.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import re
 import pickle
 import pandas as pd
 import shutil
 
 log_file = open("log.txt", "w")
 
+
 # Logging Functions
 def Time_now():
     now = datetime.now()
     Date_time = "%s-%s-%s %s:%s:%s " % (
         now.year,
         now.month,
         now.day,
@@ -69,30 +70,28 @@
         return string[:-1]
     else:
         return string
 
 
 # Main GenBank file downloadig function
 def downloader(list_acc, path_tmp, out, cut=50):
-
     # Parse
     cnt = 0  # counter by 50
     cnt_all = len(list_acc)  # total number of records
 
     start_time = time.time()
 
     record_list = []
 
     if cnt_all == 0:
         Mes("No accessions available in GenBank. Please check your input")
         return -1
 
     # Iterating with 50 items
     for i in range(int((len(list_acc) - 1) / cut) + 1):
-
         # Try to parse saved files
         if str(i) in [file for file in os.listdir(f"{path_tmp}")]:
             Mes("Found saved")
             cnt += cut
             with open(f"{path_tmp}/{i}", "rb") as fp:
                 data = pickle.load(fp)
                 for record in data:
@@ -230,15 +229,14 @@
         os.remove(f"{path_tmp}/{file}")
 
     return 1
 
 
 # Get accession list from GenBank
 def ncbi_getacc(email, term, out):
-
     Entrez.email = email
 
     # Get all ID
     handle = Entrez.esearch(db="Nucleotide", term=term)
     record = Entrez.read(handle)
 
     sleep(5)
@@ -249,39 +247,42 @@
 
     list_acc = record["IdList"]
 
     Mes(f"Number of IDs: {len(list_acc)}")
 
     return list_acc
 
+
 # To manage shotgun contig accessions
 def entrez_query_generator(acc_list):
     acc_tmp_list = []
     for acc in acc_list:
         # for normal genbank accession
         if re.fullmatch(
             r"(([A-Z]{1}[0-9]{5})(\.[0-9]{1}){0,1})|(([A-Z]{2}[\_]{0,1}[0-9]{6}){1}([\.][0-9]){0,1})",
             acc.strip(),
         ):
-            acc_tmp_list.append(f"{acc.strip().split('.')[0]}") 
+            acc_tmp_list.append(f"{acc.strip().split('.')[0]}")
         # For shotgun sequences
-        elif re.fullmatch(r"(([A-Z]{4}[0-9]{8})(\.[0-9]{1}){0,1})|(([A-Z]{6}[0-9]{9,})(\.[0-9]{1}){0,1})", acc.strip()):
-            acc_tmp_list.append(
-                acc.strip().split(".")[0]
-            )
+        elif re.fullmatch(
+            r"(([A-Z]{4}[0-9]{8})(\.[0-9]{1}){0,1})|(([A-Z]{6}[0-9]{9,})(\.[0-9]{1}){0,1})",
+            acc.strip(),
+        ):
+            acc_tmp_list.append(acc.strip().split(".")[0])
         else:
             Mes(
                 f"[Error] Developmental error, bad accession {acc} entered entrez_query_generator please ask to developer"
             )
             raise Exception
 
     acc_string = " ".join(acc_tmp_list)
 
     return acc_string
 
+
 # filter accessions by regex
 def filter_acc(acc_list, email) -> list:
     # We can do this with pythonic expressions, but using iterative way for reporting
     return_acc_list = []
     for acc in acc_list:
         if acc.strip() == "":
             pass
@@ -290,18 +291,19 @@
             r"(([A-Z]{1}[0-9]{5})(\.[0-9]{1}){0,1})|(([A-Z]{2}[\_]{0,1}[0-9]{6}){1}([\.][0-9]){0,1})",
             acc.strip(),
         ):
             return_acc_list.append(
                 acc.strip().split(".")[0]
             )  # Use most recent version of sequence
         # For shotgun sequences
-        elif re.fullmatch(r"(([A-Z]{4}[0-9]{8})(\.[0-9]{1}){0,1})|(([A-Z]{6}[0-9]{9,})(\.[0-9]{1}){0,1})", acc.strip()):
-            return_acc_list.append(
-                acc.strip().split(".")[0]
-            )
+        elif re.fullmatch(
+            r"(([A-Z]{4}[0-9]{8})(\.[0-9]{1}){0,1})|(([A-Z]{6}[0-9]{9,})(\.[0-9]{1}){0,1})",
+            acc.strip(),
+        ):
+            return_acc_list.append(acc.strip().split(".")[0])
         else:
             Mes(
                 f"[Warning] Accession {acc} does not seems to be valid accession. Passing"
             )
 
     # Check if acc are valid by asking to GenBank
     # to get number of result
@@ -381,23 +383,21 @@
 
         elif type(input_dict[key]) is list:
             for o in input_dict[key]:
                 if type(o) is dict:
                     obj_list += retrieve_parallel(o, label, label_value, obj)
 
         elif type(input_dict[key]) is dict:
-
             obj_list += retrieve_parallel(input_dict[key], label, label_value, obj)
 
     return obj_list
 
 
 # change list output as string form
 def format_list(input_list, filter_list=[], add=", ", default=""):
-
     out_list = []
     for o in input_list:
         if not (o in filter_list):
             out_list.append(o)
 
     if len(out_list) == 0:
         return default
@@ -536,15 +536,14 @@
         if department == []:
             pass
 
         return journal, department
 
     # Get paper title from given record json
     def Get_title(record):
-
         state = 0
         title = []
         if "GBSeq_references" in record:
             for reference in record["GBSeq_references"]["GBReference"]:
                 if type(reference) == type({"dict": "dict"}):
                     try:
                         # print(len(reference))
@@ -590,98 +589,90 @@
         else:
             title = []
 
         return title
 
     # Get voucher from given record json
     def Get_voucher(record):
-
         obj_list = retrieve_parallel(
             input_dict=record,
             label="GBQualifier_name",
             label_value="specimen_voucher",
             obj="GBQualifier_value",
         )
 
         return format_list(input_list=obj_list, filter_list=[], add=" = ", default="")
 
     # Get type_material from given record json
     def Get_type_material(record):
-
         obj_list = retrieve_parallel(
             input_dict=record,
             label="GBQualifier_name",
             label_value="type_material",
             obj="GBQualifier_value",
         )
 
         return format_list(input_list=obj_list, filter_list=[], add=" = ", default="")
 
     # Get strain from given record json
     def Get_strain(record):
-
         obj_list = retrieve_parallel(
             input_dict=record,
             label="GBQualifier_name",
             label_value="strain",
             obj="GBQualifier_value",
         )
 
         return format_list(input_list=obj_list, filter_list=[], add=" = ", default="")
 
     # Get culture_collection from given record json
     def Get_culture_collection(record):
-
         obj_list = retrieve_parallel(
             input_dict=record,
             label="GBQualifier_name",
             label_value="culture_collection",
             obj="GBQualifier_value",
         )
 
         return format_list(input_list=obj_list, filter_list=[], add=" = ", default="")
 
     # Get note from given record json
     def Get_note(record):
-
         obj_list = retrieve_parallel(
             input_dict=record,
             label="GBQualifier_name",
             label_value="note",
             obj="GBQualifier_value",
         )
 
         return format_list(input_list=obj_list, filter_list=[], add=" = ", default="")
 
     # Get isolate from given record json
     def Get_isolate(record):
-
         obj_list = retrieve_parallel(
             input_dict=record,
             label="GBQualifier_name",
             label_value="isolate",
             obj="GBQualifier_value",
         )
 
         return format_list(input_list=obj_list, filter_list=[], add=" = ", default="")
 
     # Get clone from given record json
     def Get_clone(record):
-
         obj_list = retrieve_parallel(
             input_dict=record,
             label="GBQualifier_name",
             label_value="clone",
             obj="GBQualifier_value",
         )
 
         return format_list(input_list=obj_list, filter_list=[], add=" = ", default="")
 
     def Get_author(record):
-
         author_list = []
 
         if "GBSeq_references" in record.keys():
             if "GBReference" in record["GBSeq_references"].keys():
                 if isinstance(record["GBSeq_references"]["GBReference"], dict):
                     if (
                         "GBReference_authors"
@@ -803,15 +794,14 @@
     with open(json_in) as json_file:
         json_data = json.load(json_file)
 
     json_temp = []
 
     # Transform to output format
     for record in json_data:
-
         """
         dict_temp = {
             "acc": "",
             "length": "",
             "seqname": "",
             "spname": "",
             "uploader": [],
@@ -828,15 +818,14 @@
         }
         """
         dict_temp = {}
 
         if (
             "GBSeq_sequence" in record or "GBSeq_feature-table" in record
         ):  # remove data without sequence
-
             dict_temp["acc"] = record["GBSeq_locus"]
             dict_temp["length"] = record["GBSeq_length"]
             dict_temp["seqname"] = record["GBSeq_definition"]
             dict_temp["spname"] = record["GBSeq_organism"]
             dict_temp["uploader"] = Get_author(record)
             dict_temp["journal"], dict_temp["department"] = Get_journal(record)
             dict_temp["title"] = Get_title(record)
@@ -863,15 +852,14 @@
             raise Exception
 
     with open(out, "w") as fp:
         json_term = json.dump(json_temp, fp, indent=4)
 
 
 def getseq(DB, out, additional_terms=[]):
-
     # terms are chosen in definition
     # additional terms are chosen in all parts
 
     temp_list = []
     with open(DB) as json_file:
         json_data = json.load(json_file)
 
@@ -905,15 +893,14 @@
     outjson = out + ".json"
 
     with open(outjson, "w") as fp:
         json_term = json.dump(temp_list, fp, indent=4)
 
 
 def getseq_without(DB, out, additional_terms=[], exceptional_terms=[]):
-
     # terms are chosen in definition
     # additional terms are chosen in all parts
 
     temp_list = []
     with open(DB) as json_file:
         json_data = json.load(json_file)
 
@@ -951,15 +938,14 @@
     outjson = out + ".json"
 
     with open(outjson, "w") as fp:
         json_term = json.dump(temp_list, fp, indent=4)
 
 
 def seqrecordtodict(Seqrecord):
-
     dict_record = {
         "acc": "",
         "len": 0,
         "seqname": "",
         "spname": "",
         "uploader": [],
         "journal_things": [],
@@ -970,15 +956,14 @@
     dict_record["acc"] = Seqrecord.id
     dict_record["len"] = len(Seqrecord)
     dict_record["seqname"] = Seqrecord.description
 
     dict_record["spname"] = Seqrecord.annotations["organism"]
 
     for Reference in Seqrecord.annotations["references"]:
-
         dict_record["journal_things"].append(Reference.title)
         dict_record["journal_things"].append(Reference.journal)
 
         for author in list(map(delcomma, Reference.authors.split(" "))):
             if not (author in dict_record["uploader"]):
                 if author != "and":
                     dict_record["uploader"].append(author)
@@ -1013,15 +998,14 @@
         "DEC": "12",
     }
     spl = string.split("-")
     return f"{spl[2]}-{dict_mon[spl[1]]}-{spl[0]}"
 
 
 def classification(description):
-
     if (
         "internal transcribed spacer 1" in description
         and "internal transcribed spacer 2" in description
     ):
         return "ITS1, ITS2"
         print("ITS1, ITS2")
     elif "internal transcribed spacer 1" in description:
@@ -1097,43 +1081,40 @@
         print("mt_others")
     else:
         print(description)
         return "others"
 
 
 def BLAST_downloader(fasta_in, blast_out):
-
     records = SeqIO.parse(fasta_in, "fasta")
     for i, record in enumerate(list(records)):
         print(i)
         query = SeqIO.write(record, "temp.fasta", "fasta")
         os.system(
             f"blastn -out {blast_out}_{i}.xml -outfmt 5 -query temp.fasta -db /data/cwseo/BLAST_DB/public/nt -evalue 0.1 -num_threads 2"
         )
         # blastn_cline = ncbiblastnCommandline(query="temp.fasta",db="nr",evalue=0.1,outfmt=7,out=f"{blast_out}_{i}.xml")
         # print(blastn_cline)
         # blastn_cline()
 
 
 def Build_DB(DB_fasta, out):
-
     cmd = "makeblastdb -in " + DB_fasta + " -out " + out + " -dbtype nucl"
     os.system(cmd)
 
 
 def BLASTn(query, db, evalue, out):
     blastn_cline = ncbiblastnCommandline(
         query=query, db=db, evalue=evalue, outfmt=7, out=out
     )
     Mes("BLAST: " + str(blastn_cline))
     blastn_cline()
 
 
 def classifier(json_in, out):
-
     with open(json_in) as json_file:
         json_data = json.load(json_file)
 
     dict_fasta = {}
 
     for record in json_data:
         if not (record["primer"] in dict_fasta):
@@ -1155,29 +1136,27 @@
         file.close()
 
     return new_keys
 
 
 # get list of acc in transformed json
 def get_acc(json_file):
-
     file = open(json_file, encoding="UTF-8")
     json_list = json.loads(file.read())
 
     list_acc = []
 
     for read in json_list:
         list_acc.append(read["acc"])
 
     return list_acc
 
 
 # from json file, pick data with given acc and save as json
 def json_pick(json_file, acc_list, out):
-
     file = open(json_file, encoding="UTF-8")
     json_list = json.loads(file.read())
 
     list_json = []
 
     for read in json_list:
         print(read["acc"])
@@ -1192,15 +1171,14 @@
         with open(out, "w") as fp:
             json.dump(list_json, fp, indent=4)
 
         return True
 
 
 def json_merge(json_list, out):
-
     all_records = []
     for json_file in json_list:
         file = open(json_file, encoding="UTF-8")
         tmp_list = json.loads(file.read())
         all_records += tmp_list
 
     with open(out, "w") as fp:
@@ -1249,15 +1227,14 @@
 
 
 # GenBank, download all by given term
 # genus term is space seperated string of genus (eg. Penicillium Apiospora Alternaria )
 def ncbi_download(
     email, genus_term, additional_term, name_out, path_work, path_tmp, max_len
 ):
-
     # select outgroup location
     path_localgb = f"{path_work}/{name_out}.json"
     path_localgb_xlsx = f"{path_work}/{name_out}.xlsx"
 
     # Setup email
     Entrez.email = email
 
@@ -1287,15 +1264,14 @@
             max_len=max_len,
             additional_term=additional_term,
         )
 
 
 # Download by given list of accession
 def ncbi_downloadbyacclist(email, list_acc, name_out, path_work, path_tmp, max_len):
-
     Entrez.email = email
 
     Mes(f"Number of IDs: {len(list_acc)}")
     # Download GenBank records
     status = downloader(
         list_acc=list_acc, path_tmp=path_tmp, out=f"{path_work}/{name_out}.json"
     )
```

### Comparing `GenMine-1.0.8/GenMine/command.py` & `GenMine-1.0.9/GenMine/command.py`

 * *Files identical despite different names*

### Comparing `GenMine-1.0.8/GenMine/main.py` & `GenMine-1.0.9/GenMine/main.py`

 * *Files identical despite different names*

### Comparing `GenMine-1.0.8/LICENSE` & `GenMine-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `GenMine-1.0.8/README.md` & `GenMine-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `GenMine-1.0.8/setup.py` & `GenMine-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # GenMine/setup.py
 from setuptools import setup, find_packages
 
 setup(
     name="GenMine",
-    version="1.0.8",
+    version="1.0.9",
     description="GenBank data miner for fungal taxonomists",
     author="Changwan Seo",
     author_email="wan101010@snu.ac.kr",
     url="https://github.com/Changwanseo/GenMine",
     python_requires=">= 3.8",
     packages=find_packages(include=["GenMine"]),
     install_requires=[
```

