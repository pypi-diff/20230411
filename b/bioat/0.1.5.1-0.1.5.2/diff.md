# Comparing `tmp/bioat-0.1.5.1.tar.gz` & `tmp/bioat-0.1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioat-0.1.5.1.tar", max compression
+gzip compressed data, was "bioat-0.1.5.2.tar", max compression
```

## Comparing `bioat-0.1.5.1.tar` & `bioat-0.1.5.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     1080 2022-10-12 10:28:48.000000 bioat-0.1.5.1/LICENSE
--rw-r--r--   0        0        0     1215 2023-03-31 15:29:35.600902 bioat-0.1.5.1/README.md
--rw-r--r--   0        0        0     1044 2023-04-07 08:13:22.521088 bioat-0.1.5.1/pyproject.toml
--rw-r--r--   0        0        0      471 2023-04-01 11:15:49.201131 bioat-0.1.5.1/src/bioat/__init__.py
--rw-r--r--   0        0        0      508 2023-04-02 12:41:49.000000 bioat-0.1.5.1/src/bioat/about.py
--rw-r--r--   0        0        0    13130 2023-03-31 17:13:33.632897 bioat-0.1.5.1/src/bioat/bam.py
--rw-r--r--   0        0        0     1413 2023-04-06 11:55:25.000000 bioat-0.1.5.1/src/bioat/cli.py
--rw-r--r--   0        0        0       63 2022-10-12 10:34:44.000000 bioat-0.1.5.1/src/bioat/exceptions.py
--rw-r--r--   0        0        0    11016 2023-03-13 04:00:08.114588 bioat-0.1.5.1/src/bioat/fastx.py
--rw-r--r--   0        0        0      818 2023-03-13 04:16:15.365909 bioat-0.1.5.1/src/bioat/genome.py
--rw-r--r--   0        0        0     5529 2023-04-06 10:53:27.000000 bioat-0.1.5.1/src/bioat/hic.py
--rw-r--r--   0        0        0        0 2023-04-01 12:21:31.028419 bioat-0.1.5.1/src/bioat/lib/__init__.py
--rw-r--r--   0        0        0      854 2023-04-01 13:16:24.000000 bioat-0.1.5.1/src/bioat/lib/_dev_tools.py
--rw-r--r--   0        0        0     2285 2023-04-06 10:50:24.000000 bioat-0.1.5.1/src/bioat/lib/libcolor.py
--rw-r--r--   0        0        0     7917 2023-04-06 10:50:04.000000 bioat-0.1.5.1/src/bioat/lib/libcrispr.py
--rw-r--r--   0        0        0     1128 2023-03-26 11:49:26.175731 bioat-0.1.5.1/src/bioat/logger.py
--rw-r--r--   0        0        0      685 2023-03-13 15:37:04.537990 bioat-0.1.5.1/src/bioat/mgi.py
--rw-r--r--   0        0        0     5629 2023-03-12 14:27:33.279607 bioat-0.1.5.1/src/bioat/system.py
--rw-r--r--   0        0        0     3245 2023-04-07 08:00:16.234706 bioat-0.1.5.1/src/bioat/table.py
--rw-r--r--   0        0        0    23903 2023-04-06 13:09:33.000000 bioat-0.1.5.1/src/bioat/targeted_deep_sequencing.py
--rw-r--r--   0        0        0      384 2023-04-07 08:13:27.906137 bioat-0.1.5.1/src/bioat/version.py
--rw-r--r--   0        0        0     2207 1970-01-01 00:00:00.000000 bioat-0.1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2022-10-12 10:28:48.000000 bioat-0.1.5.2/LICENSE
+-rw-r--r--   0        0        0      689 2023-04-10 17:11:40.000000 bioat-0.1.5.2/README.md
+-rw-r--r--   0        0        0     1064 2023-04-08 13:49:15.966541 bioat-0.1.5.2/pyproject.toml
+-rw-r--r--   0        0        0      471 2023-04-01 11:15:49.201131 bioat-0.1.5.2/src/bioat/__init__.py
+-rw-r--r--   0        0        0      508 2023-04-02 12:41:49.000000 bioat-0.1.5.2/src/bioat/about.py
+-rw-r--r--   0        0        0    13631 2023-04-10 17:00:33.000000 bioat-0.1.5.2/src/bioat/bam.py
+-rw-r--r--   0        0        0     1413 2023-04-06 11:55:25.000000 bioat-0.1.5.2/src/bioat/cli.py
+-rw-r--r--   0        0        0       63 2022-10-12 10:34:44.000000 bioat-0.1.5.2/src/bioat/exceptions.py
+-rw-r--r--   0        0        0    11016 2023-03-13 04:00:08.114588 bioat-0.1.5.2/src/bioat/fastx.py
+-rw-r--r--   0        0        0      818 2023-03-13 04:16:15.365909 bioat-0.1.5.2/src/bioat/genome.py
+-rw-r--r--   0        0        0     5895 2023-04-10 17:00:56.000000 bioat-0.1.5.2/src/bioat/hic.py
+-rw-r--r--   0        0        0        0 2023-04-01 12:21:31.028419 bioat-0.1.5.2/src/bioat/lib/__init__.py
+-rw-r--r--   0        0        0      854 2023-04-08 13:49:32.058220 bioat-0.1.5.2/src/bioat/lib/_dev_tools.py
+-rw-r--r--   0        0        0     5550 2023-04-11 16:07:38.982348 bioat-0.1.5.2/src/bioat/lib/libalignment.py
+-rw-r--r--   0        0        0     2719 2023-04-11 14:34:02.889267 bioat-0.1.5.2/src/bioat/lib/libcolor.py
+-rw-r--r--   0        0        0     7042 2023-04-11 11:27:23.563291 bioat-0.1.5.2/src/bioat/lib/libcrispr.py
+-rw-r--r--   0        0        0     1442 2023-04-10 17:17:40.000000 bioat-0.1.5.2/src/bioat/logger.py
+-rw-r--r--   0        0        0      668 2023-04-07 16:11:22.000000 bioat-0.1.5.2/src/bioat/mgi.py
+-rw-r--r--   0        0        0     5629 2023-03-12 14:27:33.279607 bioat-0.1.5.2/src/bioat/system.py
+-rw-r--r--   0        0        0     3245 2023-04-07 08:00:16.234706 bioat-0.1.5.2/src/bioat/table.py
+-rw-r--r--   0        0        0    27616 2023-04-11 16:22:40.513555 bioat-0.1.5.2/src/bioat/targeted_deep_sequencing.py
+-rw-r--r--   0        0        0      384 2023-04-10 17:03:51.000000 bioat-0.1.5.2/src/bioat/version.py
+-rw-r--r--   0        0        0     1723 1970-01-01 00:00:00.000000 bioat-0.1.5.2/PKG-INFO
```

### Comparing `bioat-0.1.5.1/LICENSE` & `bioat-0.1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bioat-0.1.5.1/pyproject.toml` & `bioat-0.1.5.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bioat"
-version = "0.1.5.1"
+version = "0.1.5.2"
 description = "Bioinformatic toolkit with python (It's still under development!)"
 license = "MIT"
 authors = ["Herman Zhao <hermanzhaozzzz@gmail.com>"]
 repository = "https://github.com/hermanzhaozzzz/BioinformaticAnalysisTools"
 homepage = "https://github.com/hermanzhaozzzz/BioinformaticAnalysisTools"
 # README file(s) are used as the package description
 readme = "README.md"
@@ -18,14 +18,15 @@
 tqdm = "^4.64.1"
 fire = "^0.5.0"
 cython = "^0.29.33"
 pysam = "^0.20.0"
 biopython = "^1.81"
 pandarallel = "^1.6.4"
 matplotlib = "^3.7.1"
+tabulate = "^0.9.0"
 
 [tool.poetry.scripts]
 bioat = "bioat.cli:main"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 pytest-cov = "^3.0"
```

### Comparing `bioat-0.1.5.1/src/bioat/bam.py` & `bioat-0.1.5.2/src/bioat/bam.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,18 +32,21 @@
         :param threads: Multiple threads number
         :param mutation_number_threshold: Only contain mutation info go to the output, set 0 mean output all site
         :param temp_dir: Where to keep temp files, default is /tmp
         :param remove_temp: Where to keep temp files, default is /tmp
         :param log_level: 'CRITICAL', 'ERROR', 'WARNING', 'INFO', 'DEBUG', 'NOTSET'
         """
         set_logging_level(level=log_level)
-
+        # set logger
+        lib_name = __name__
+        function_name = sys._getframe().f_code.co_name
+        logger = logging.getLogger(f'{lib_name}.{function_name} ==> ')
         def _temp_split_bam(mpileup, threads, temp_dir):
             # creat temp file name and open file
-            logging.debug("Making temp files...")
+            logger.debug("Making temp files...")
 
             input_file_basename = os.path.basename(mpileup)
 
             temp_filename_list = []
             temp_file_list = []
 
             os.makedirs(temp_dir, exist_ok=True)
@@ -56,43 +59,43 @@
                 temp_filename_list.append(temp_file_name)
 
                 # open file
                 temp_file = gzip.open(temp_file_name, "wt")
                 temp_file_list.append(temp_file)
 
             # counting input file line number
-            logging.debug("Counting input file...")
+            logger.debug("Counting input file...")
 
             total_input_line_num = 0
             input_file = gzip.open(mpileup, "rt") if mpileup.endswith('.gz') else open(mpileup, "rt")
 
             # count total_input_line_num
             for _ in input_file:
                 total_input_line_num += 1
 
             if total_input_line_num % threads == 0:
                 each_file_line_num = (total_input_line_num // threads)
             else:
                 each_file_line_num = (total_input_line_num // threads) + 1
 
             input_file.close()
-            logging.debug("Done!")
+            logger.debug("Done!")
 
             # split temp files
             # write into output filename
             input_file = gzip.open(mpileup, "rt") if mpileup.endswith('.gz') else open(mpileup, "rt")
 
             for index, line in enumerate(input_file):
                 file_index = index // each_file_line_num
                 temp_file_list[file_index].write(line)
 
             # close output filename
             input_file.close()
             [temp_file.close() for temp_file in temp_file_list]
-            logging.debug("Make temp files done!")
+            logger.debug("Make temp files done!")
 
             return temp_filename_list
 
         def _merge_out_bmat(temp_filename_list, output, remove_temp=True):
             if type(output) is str:
                 output = gzip.open(output, "wt") if output.endswith('.gz') else open(output, "wt")
             # write header
@@ -127,57 +130,65 @@
                     os.remove(temp_filename)
                     os.remove(temp_filename + ".bmat.gz")
                 os.rmdir(temp_dir)
 
         # make temp files
         temp_filename_list = _temp_split_bam(mpileup=mpileup, threads=threads, temp_dir=temp_dir)
         # multiple processing part
-        logging.debug("Parsing files...")
+        logger.debug("Parsing files...")
 
         procs_list = []
 
         for index, temp_mpileup in enumerate(temp_filename_list):
             temp_output = temp_mpileup + ".bmat.gz"
             # add multiprocess
             sub_proc = Process(target=_run_mpileup_to_table,
                                args=(temp_mpileup, temp_output, mutation_number_threshold,))
             procs_list.append(sub_proc)
             sub_proc.start()
 
         for sub_proc in procs_list:
             sub_proc.join()
-        logging.debug("Done!")
+        logger.debug("Done!")
         # merge output files
-        logging.debug("Merging files...")
+        logger.debug("Merging files...")
         _merge_out_bmat(temp_filename_list=temp_filename_list, output=output, remove_temp=remove_temp)
-        logging.debug("Done!...")
+        logger.debug("Done!...")
 
     def remove_clip(
             self,
             input: str = 'stdin',
             output: str = 'stdout',
             threads: int = 1,
             output_fmt: str = 'SAM',
             remove_as_paired: bool = True,
-            max_clip: int = 0
+            max_clip: int = 0,
+            log_level: str = 'INFO'
     ):
         """Remove softclip reads in BAM file.
 
         :param input: BAM file sorted by coordinate with soft/hard clip reads, pipe stdin is supported
 
                         [samtools view -h foo_sort_name.bam | bioat bam remove_clip <flags>]
         :param output: BAM file sorted by coordinate without soft/hard clip reads, pipe stdout is supported
 
                         [bioat bam remove_clip <flags> | wc -l]
                         [bioat bam remove_clip <flags> | samtools view ....]
         :param threads: threads used by pysam and samtools core
         :param output_format: BAM, SAM
         :param remove_as_paired: True, False. remove single clip(False) / clip and its pair read(True)
         :param max_clip: the maximum clips allowed per read
+        :param log_level: 'CRITICAL', 'ERROR', 'WARNING', 'INFO', 'DEBUG', 'NOTSET'
         """
+        set_logging_level(level=log_level)
+        # set logger
+        lib_name = __name__
+        function_name = sys._getframe().f_code.co_name
+        logger = logging.getLogger(f'{lib_name}.{function_name} ==> ')
+
         if sys.stdin.isatty():  # not stdin
             bam_in = pysam.AlignmentFile(input, "r", threads=threads, check_sq=False)
         else:  # stdin
             bam_in = pysam.AlignmentFile("-", "r", threads=threads, check_sq=False)
 
         # fix output
         if output == 'stdout':
@@ -186,19 +197,19 @@
         try:
             so = bam_in.header['HD']['SO']
         except KeyError:
             so = None
 
         if so:
             if so != "queryname":
-                logging.fatal(f"the input BAM|SAM must be sorted by name and has header [SO:queryname]!\n"
+                logger.fatal(f"the input BAM|SAM must be sorted by name and has header [SO:queryname]!\n"
                               f"your header: [SO:{so}]\n")
                 exit(1)
         else:
-            logging.warning(f"the input BAM|SAM must be sorted by name and has header [SO:queryname]!\n"
+            logger.warning(f"the input BAM|SAM must be sorted by name and has header [SO:queryname]!\n"
                             "your bam file does not have a header\n")
 
         write_mode = 'wb' if output_fmt.upper() == "BAM" else 'w'
         bam_out = pysam.AlignmentFile(output, write_mode, template=bam_in)
 
         # Iterate through reads.
         read1, read2 = None, None
@@ -238,18 +249,18 @@
                     if softclip2 <= max_clip:
                         bam_out.write(read2)
                 else:
                     if softclip1 <= max_clip and softclip2 <= max_clip:
                         bam_out.write(read1)
                         bam_out.write(read2)
             else:
-                logging.fatal(
+                logger.fatal(
                     'something wrong with read1/2 pairs, they may have different read id or there is None in them')
-                logging.fatal(f'read1={read1}, read2={read2}')
-                logging.fatal(f'read1_id={read1.query_name}, read2_id={read2.query_name}')
+                logger.fatal(f'read1={read1}, read2={read2}')
+                logger.fatal(f'read1_id={read1.query_name}, read2_id={read2.query_name}')
                 exit(1)
 
         bam_in.close()
         bam_out.close()
 
 
 def _run_mpileup_to_table(temp_mpileup, temp_output, mutation_number_threshold):
```

### Comparing `bioat-0.1.5.1/src/bioat/cli.py` & `bioat-0.1.5.2/src/bioat/cli.py`

 * *Files identical despite different names*

### Comparing `bioat-0.1.5.1/src/bioat/fastx.py` & `bioat-0.1.5.2/src/bioat/fastx.py`

 * *Files identical despite different names*

### Comparing `bioat-0.1.5.1/src/bioat/genome.py` & `bioat-0.1.5.2/src/bioat/genome.py`

 * *Files identical despite different names*

### Comparing `bioat-0.1.5.1/src/bioat/hic.py` & `bioat-0.1.5.2/src/bioat/hic.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from __future__ import absolute_import
-
+import sys
 import time
 import pandas as pd
 from bioat.logger import set_logging_level
 from pandarallel import pandarallel
 import logging
 from bioat.lib._dev_tools import profile
 import gc
 
-
 try:
     pandarallel.initialize(
         progress_bar=False,
         use_memory_fs=True,
         verbose=1
     )
 except SystemError:
@@ -24,24 +23,36 @@
 
 
 class HiC:
     def __init__(self):
         pass
 
     @profile
-    def get_effective_resolutions(self, genome_index, valid_pairs, output):
+    def get_effective_resolutions(
+            self,
+            genome_index,
+            valid_pairs,
+            output,
+            log_level: str = 'INFO'
+    ):
         """Get deepest resolution of cis-interation.
 
         输入为result文件，输出为matrix的大致resolution.
 
         :param genome_index: genome.fa.fai
         :param valid_pairs: rm_dup_pairs.allValidPairs by HiC-Pro
         :param output: table_output, TSV file
+        :param log_level: 'CRITICAL', 'ERROR', 'WARNING', 'INFO', 'DEBUG', 'NOTSET'
         """
-        logging.debug('Develop mode is on')
+        set_logging_level(level=log_level)
+        # set logger
+        lib_name = __name__
+        function_name = sys._getframe().f_code.co_name
+        logger = logging.getLogger(f'{lib_name}.{function_name} ==> ')
+        logger.debug('Develop mode is on')
         # load ref genome lengths
         df_chromosome = pd.read_csv(
             genome_index,
             sep='\t',
             usecols=[0, 1],
             names=['chromosome', 'length'],
             index_col='chromosome',
@@ -67,19 +78,19 @@
         chunks = []
 
         while True:
             try:
                 chunk = reader.get_chunk(10_000_000)
                 chunks.append(chunk)
             except StopIteration:
-                logging.debug("pandas reader iteration is done.")
+                logger.debug("pandas reader iteration is done.")
                 break
 
         df_valid_pairs = pd.concat(chunks, ignore_index=True)
-        logging.debug(df_valid_pairs.info(memory_usage='deep'))
+        logger.debug(df_valid_pairs.info(memory_usage='deep'))
         # 思路：二分法确认new_bin下线
         output = open(output, 'wt')
         write_lines = 0
         output.write('test_bin(kb)\ttotal_bins\tthreshold(%)\tis_effective\n')
         write_lines += 1
         # 思路：二分法确认new_bin下线
         circle = 1
@@ -101,15 +112,15 @@
             # calculate total bins
             df_chromosome['bins'] = df_chromosome['length'].map(lambda x: int(x / new_bin) + 1)
             df_chromosome['bins_cumsum'] = df_chromosome['bins'].cumsum()
             total_bins = df_chromosome.iloc[-1, 2]
 
             # calculate mapped bin index
             df_valid_pairs[['bin_index_A', 'bin_index_B']] = df_valid_pairs.parallel_apply(
-            # df_valid_pairs[['bin_index_A', 'bin_index_B']] = df_valid_pairs.apply(
+                # df_valid_pairs[['bin_index_A', 'bin_index_B']] = df_valid_pairs.apply(
                 get_bin_index,
                 axis=1,
                 result_type='expand'
             )
 
             # print(df_valid_pairs)
             # threshold calculation
@@ -136,15 +147,14 @@
                 break
             del s_bin_idx_count1, s_bin_idx_count2, df_bin_interaction_count
             gc.collect()
         output.close()
 
 
 if __name__ == '__main__':
-    set_logging_level(level='DEBUG')
     a = time.time()
     hic = HiC()
     hic.get_effective_resolutions(
         genome_index="/Volumes/zhaohn_HD/Bio/1.database/db_genomes/genome_fa/genome_ucsc_hg38/genome_ucsc_hg38.fa.fai",
         valid_pairs="../../data/hic/test.rm_dup_pairs.allValidPairs",
         output="/Users/zhaohuanan/Downloads/testout"
     )
```

### Comparing `bioat-0.1.5.1/src/bioat/lib/_dev_tools.py` & `bioat-0.1.5.2/src/bioat/lib/_dev_tools.py`

 * *Files identical despite different names*

### Comparing `bioat-0.1.5.1/src/bioat/lib/libcolor.py` & `bioat-0.1.5.2/src/bioat/lib/libcolor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
-
+import sys
+import logging
 
 def convert_hex_to_rgb(hex_color: str) -> tuple:
     """Convert HEX color to RGB color.
 
     :param hex_color: str, like '#FFFFAA'
     :return: tuple, like (255, 255, 170)
     """
@@ -51,31 +52,43 @@
 
         if not match_state:
             value_idx_list.append(index + 1)
 
     return tuple(color_list[col_idx] for col_idx in value_idx_list)
 
 
-def make_color_list(low_color_RGB, high_color_RGB, length_out=20, back_format="Hex"):
+def make_color_list(low_color_RGB, high_color_RGB, length_out=20, return_fmt="HEX"):
     """
     INPUT
         <low_color_RGB> <high_color_RGB>
             Format like (210, 179, 150), tuple, list, or np.array
 
         <back_format>
             Hex OR RGB
 
     RETURN
         <color_list>
     """
+    # set logger
+    lib_name = __name__
+    function_name = sys._getframe().f_code.co_name
+    logger = logging.getLogger(f'{lib_name}.{function_name} ==> ')
+
+    supported_fmt = ('HEX', 'RGB')
+    return_fmt = return_fmt.upper()
+    if return_fmt not in supported_fmt:
+        logger.critical(
+            f'not supported color format: {return_fmt}\n'
+            f'supported_fmt = {supported_fmt}'
+        )
     low_color = np.array(low_color_RGB)
     high_color = np.array(high_color_RGB)
 
     color_list = []
     for index in range(0, length_out + 1):
         rgb_color = low_color + (high_color - low_color) // length_out * index
-        if back_format == "Hex":
+        if return_fmt == "HEX":
             color_list.append(convert_rgb_to_hex(tuple(rgb_color)))
         else:
             color_list.append(tuple(rgb_color))
 
     return color_list
```

### Comparing `bioat-0.1.5.1/src/bioat/lib/libcrispr.py` & `bioat-0.1.5.2/src/bioat/lib/libcrispr.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,146 +1,57 @@
-TARGET_REGIONS_LIB = {
-    "EMX1": "GAGTCCGAGCAGAAGAAGAA$GGG$",
-    "HEK3": "GGCCCAGACTGAGCACGTGA$TGG$",
-    "HEK4": "GGCACTGCGGCTGGAGGTGG$GGG$",
-    "RNF2": "GTCATCTTAGTCATTACCTG$AGG$",
-    "VEGFA": "GACCCCCTCCACCCCGCCTC$CGG$",
-    "CDKN2A": "$TTTA$GCCCCAATAATCCCCACATGTCA",
-    "DYRK1A": "$TTTA$GAAGCACATCAAGGACATTCTAA",
+from __future__ import absolute_import
+import logging
+import sys
+from Bio.Seq import Seq
+from Bio.Align import PairwiseAligner
+from bioat.lib.libalignment import get_alignment_info
+
+"""TARGET_REGIONS_LIB.
+
+bioat targeted_deep_sequencing region_heatmap test_sorted.mpileup.info.tsv test.pdf --get_built_in_target_region
+
+INFO:root:You can use <key> in built-in <target_regions> to represent your target_region:
+        <key>   <target_region>
+        EMX1    GAGTCCGAGCAGAAGAAGAA^GGG^
+        HEK3    GGCCCAGACTGAGCACGTGA^TGG^
+        HEK4    GGCACTGCGGCTGGAGGTGG^GGG^
+        ...
+"""
+TARGET_SEQ_LIB = {
+    "EMX1": "GAGTCCGAGCAGAAGAAGAA^GGG^",
+    "HEK3": "GGCCCAGACTGAGCACGTGA^TGG^",
+    "HEK4": "GGCACTGCGGCTGGAGGTGG^GGG^",
+    "RNF2": "GTCATCTTAGTCATTACCTG^AGG^",
+    "VEGFA": "GACCCCCTCCACCCCGCCTC^CGG^",
+    "CDKN2A": "^TTTA^GCCCCAATAATCCCCACATGTCA",
+    "DYRK1A": "^TTTA^GAAGCACATCAAGGACATTCTAA",
     "ND4": "TGCTAGTAACCACGTTCTCCTGATCAAATATCACTCTCCTACTTACAGGA",
     "ND5.1": "TAGCATTAGCAGGAATACCTTTCCTCACAGGTTTCTACTCCAAAGA",
     "ND6": "TGACCCCCATGCCTCAGGATACTCCTCAATAGCCATCG",
 }
 
 
 def find_seq_PAM_index(query_seq):
-    """
-    <INPUT>
-        query_seq
+    """Find seq PAM index.
 
-    <HELP>
-        e.g. query_seq = "AAAGAGAG"
-        return index list = [1,3,5], which means search NAG, NGG at the same time
+    :param query_seq: e.g. query_seq = "AAAGAGAG"
+    :return: index list = [1,3,5], which means search NAG, NGG at the same time
     """
     pam_index_list = []
 
     for index, base in enumerate(query_seq[:-2]):
         if query_seq[index + 1:index + 3] == "AG":
             pam_index_list.append((index, "NAG"))
 
         elif query_seq[index + 1:index + 3] == "GG":
             pam_index_list.append((index, "NGG"))
 
     return (pam_index_list)
 
 
-def analysis_align_obj(alignment, reverse_state=False):
-    """
-    INPUT:
-        <alignment obj>
-
-    OUTPUT:
-        <info>
-            1. match count
-            2. mismatch count
-            3. gap count
-            4. alignment.score
-
-    HELP:
-        2019-11-15 fix-1
-            The gap count should be the num of gap contain in sgRNA alignment region.
-
-            e.g.
-
-            AGTGGTAAGAAGAAGACGAGACATAATGAG
-            ------||||||||||||||X|----||||
-            ------AAGAAGAAGACGAGCC----TGAG
-
-            gap count should be 4, rather than 10.
-
-        2019-11-15 fix-2
-            add return info, start_index, end_index, now the retrun list will be
-
-            return_list = [
-                match_count,
-                mismatch_count,
-                gap_count,
-                alignment.score,
-                start_index,
-                end_index
-            ]
-
-            The <start_index> and <end_index> are index related to sgRNA alignment string
-
-    """
-
-    # define params
-    match_count = 0
-    mismatch_count = 0
-    gap_count = 0
-
-    alignment_list = str(alignment).split("\n")
-    query_length = len(alignment.query)
-
-    if reverse_state:
-        target_list = alignment_list[0][::-1]
-        info_list = alignment_list[1][::-1]
-        query_list = alignment_list[2][::-1]
-
-    else:
-        target_list = alignment_list[0]
-        info_list = alignment_list[1]
-        query_list = alignment_list[2]
-
-    count_state = False
-    count_query_base = 0
-
-    ref_align_start_index = 0
-    ref_align_end_index = len(alignment.target) - 1
-
-    # counting
-    for index, info_base in enumerate(info_list):
-        if not count_state:
-            if query_list[index] != "-":
-                count_state = True
-                ref_align_start_index = index
-
-        if not count_state:
-            continue
-
-        else:
-            if info_base == "|":
-                match_count += 1
-                count_query_base += 1
-
-            elif info_base == "X":
-                mismatch_count += 1
-                count_query_base += 1
-
-            elif info_base == "-":
-                gap_count += 1
-                if query_list[index] != "-":
-                    count_query_base += 1
-
-        if count_query_base >= query_length:
-            ref_align_end_index = index
-            break
-
-    return_list = [
-        match_count,
-        mismatch_count,
-        gap_count,
-        alignment.score,
-        ref_align_start_index,
-        ref_align_end_index
-    ]
-
-    return (return_list)
-
-
 def sign_value(x):
     """
     HELP
         sign function
     """
     if x < 0:
         return (-1)
@@ -163,35 +74,39 @@
     sort_rev_state_list = [True, False, False, True]
 
     for order_index, align_index in enumerate(sort_index_list):
         if (align_a[align_index] - align_b[align_index]) == 0:
             continue
         else:
             if sort_rev_state_list[order_index]:
-                return (-1 * sign_value(align_a[align_index] - align_b[align_index]))
+                return (-1 *
+                        sign_value(align_a[align_index] - align_b[align_index]))
             else:
-                return (sign_value(align_a[align_index] - align_b[align_index]))
+                return (
+                    sign_value(
+                        align_a[align_index] -
+                        align_b[align_index]))
 
     for index, char_a in enumerate(align_a[7]):
         if index <= (len(align_b[7]) - 1):
             value_a = align_alphabet[char_a]
             value_b = align_alphabet[align_b[7][index]]
 
             if value_a > value_b:
                 return 1
             elif value_a < value_b:
                 return -1
 
     return 0
 
 
-def run_sgRNA_alignment(align_ref_seq, align_sgRNA, sgRNA_aligner, extend_len=3):
+def run_sgRNA_alignment(align_ref_seq, align_sgRNA, aligner, extend_len=3):
     """
     INPUT
-        <align_ref_seq>
+        <ref_seq>
 
         <align_sgRNA>
             sgRNA seq without PAM
 
         <possible_sgRNA_region>
 
     RETURN
@@ -215,23 +130,23 @@
 
         # select PAM and sgRNA in the possible region
         region_seq_start = PAM_start_idx - len(align_sgRNA) - extend_len
         region_seq_end = PAM_start_idx + 3
 
         # alignment part
         region_seq = align_ref_seq[region_seq_start: PAM_start_idx]
-        align_res = sgRNA_aligner.align(region_seq[::-1], align_sgRNA_rev)
+        alignments = aligner.align(region_seq[::-1], align_sgRNA_rev)
 
         # parse alignment
-        ## if contain multiple alignment result with the same score, keep the best one;
-        ## sort reason score -> gap -> mismatch -> match
+        # if contain multiple alignment result with the same score, keep the best one;
+        # sort reason score -> gap -> mismatch -> match
         align_res_list = []
-        for align in align_res:
-            align_analysis_res = analysis_align_obj(align, reverse_state=True)
-            align_info_list = [x[::-1] for x in str(align).strip().split("\n")]
+        for alignment in alignments:
+            align_analysis_res = get_alignment_info(alignment, reverse=True)
+            align_info_list = [x[::-1] for x in str(alignment).strip().split("\n")]
             align_analysis_res += align_info_list
             align_analysis_res += [PAM_start_idx, PAM_type]
             align_res_list.append(align_analysis_res)
 
         if len(align_res_list) == 1:
             final_align_res_list.append(align_res_list[0])
 
@@ -241,46 +156,65 @@
 
     # sort final alignment
     final_align_res_list.sort(cmp=cmp_align_list)
 
     return (final_align_res_list)
 
 
-def run_no_PAM_sgRNA_alignment_no_chop(align_ref_seq, align_sgRNA_full, no_PAM_sgRNA_aligner):
-    """
-    INPUT
-        <align_ref_seq>
-
-        <align_sgRNA>
-            sgRNA seq without PAM
-
-        <no_PAM_sgRNA_aligner>
-            An obj from BioPython pairwise alignment
+def run_no_PAM_sgRNA_alignment_no_chop(
+        ref_seq: Seq,
+        target_seq: Seq,
+        aligner: PairwiseAligner
+) -> list:
+    """global alignment for target_seq
+
+    :param ref_seq: a Seq object from BioPython, reference sequence for the targeted deep sequencing
+    :param target_seq: a Seq object from BioPython, target region sequence for the editing window, usually the sgRNA
+        sequencing without PAM
+    :param aligner: an obj from BioPython pairwise alignment
+    :return: a list: list contains some dict, each one is an alignment result.
+    [
+        {
+            'match_count': 26,
+            'mismatch_count': 3,
+            'gap_count': 4,
+            'alignment_score': 96.0,
+            'ref_align_start_index': 0,
+            'ref_align_end_index': 32,
+            'alignment': {
+                'aligned_reference_seq': 'GGCACTGCGGCTGGAAAAAAAAAAAAAAA--GT',
+                'aligned_seq_info':      '--..|.|||||||||||||||||||||||--||',
+                'aligned_target_seq':    '--GGCAGCGGCTGGAAAAAAAAAAAAAAAAGGT'
+            },
+            'PAM_start_index': None,
+            'PAM_type': None
+        },
+        ...
+    ]
 
-    RETURN
-        <final_align_res_list>
     """
+    # set logger
+    lib_name = __name__
+    function_name = sys._getframe().f_code.co_name
+    logger = logging.getLogger(f'{lib_name}.{function_name} ==> ')
 
     # alignment part
-    align_res = no_PAM_sgRNA_aligner.align(align_ref_seq, align_sgRNA_full)
-
+    alignments = aligner.align(ref_seq, target_seq)
     # parse alignment
-    ## if contain multiple alignment result with the same score, keep the best one;
-    ## sort reason score -> gap -> mismatch -> match
-    align_res_list = []
-    for align in align_res:
-        align_analysis_res_temp = analysis_align_obj(align, reverse_state=False)
-        align_analysis_res = align_analysis_res_temp[:]
-        align_analysis_res += str(align).strip().split("\n")
-
-        PAM_start_index = align_analysis_res[5] - 2
-        PAM_type = ref_seq[PAM_start_index: PAM_start_index + 3]
-
-        align_analysis_res += [PAM_start_index, PAM_type]
-        align_res_list.append(align_analysis_res)
-
-    if len(align_res_list) == 1:
-        return (align_res_list)
+    # if contain multiple alignment result with the same score, keep the best one;
+    # sort reason score -> gap -> mismatch -> match
+    alignment_results = []
+
+    for alignment in alignments:
+        # logging.debug(type(align))  # Bio.Align.Alignment object
+        alignment_analysis_result = get_alignment_info(alignment, reverse=False)
+        logger.debug(f'alignment_analysis_result:\n{alignment_analysis_result}')
+        alignment_results.append(alignment_analysis_result)
+
+        if len(alignment_results) == 1:
+            logger.debug(f'find 1 alignment result:\n{alignment_results}')
+        return alignment_results
 
     else:
-        align_res_list.sort(cmp=cmp_align_list)
-        return (align_res_list)
+        alignment_results.sort(cmp=cmp_align_list)
+        logger.debug(f'find more than 1 alignment results:\n{alignment_results}')
+        return alignment_results
```

### Comparing `bioat-0.1.5.1/src/bioat/logger.py` & `bioat-0.1.5.2/src/bioat/logger.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,41 @@
+import sys
 import logging
 from logging import (CRITICAL, ERROR, WARNING, INFO, DEBUG, NOTSET)
 
 
 def set_logging_level(level='ERROR'):
-
     level = level.upper()
 
     dt_level = {
         k: v
         for k, v in zip(
             ['CRITICAL', 'ERROR', 'WARNING', 'INFO', 'DEBUG', 'NOTSET'],
             [CRITICAL, ERROR, WARNING, INFO, DEBUG, NOTSET]
         )
     }
     logging.basicConfig(level=dt_level[level])
+    # set logger
+    lib_name = __name__
+    function_name = sys._getframe().f_code.co_name
+    logger = logging.getLogger(f'{lib_name}.{function_name} ==> ')
 
     if level not in ('NOTSET', 'INFO'):
-        logging.info(f'set logging level = {level}')
+        logger.info(f'set logging level = {level}')
 
 
 if __name__ == '__main__':
     #  ['CRITICAL', 'ERROR', 'WARNING', 'INFO', 'DEBUG', 'NOTSET'],
     # 一个比一个轻
     set_logging_level('CRITICAL')  # 只打印 CRITICAL
     # set_logging_level('ERROR')  # DEBUG、INFO、WARNING 没打印
     # set_logging_level('WARNING')  # DEBUG、INFO 没打印
     # set_logging_level('INFO')  # DEBUG 没打印
     # set_logging_level('DEBUG')  # 全打印
     # set_logging_level('NOTSET')  # 全打印
-
+    # CRITICAL > ERROR > WARNING > INFO > DEBUG = NOTSET
+    # 也就是说,如果设置为WARNING,就只打印WARNING及左边,的CRITICAL和ERROR
     logging.debug('Python debug')
     logging.info('Python info')
     logging.warning('Python warning')
     logging.error('Python Error')
     logging.critical('Python critical')
-
```

### Comparing `bioat-0.1.5.1/src/bioat/system.py` & `bioat-0.1.5.2/src/bioat/system.py`

 * *Files identical despite different names*

### Comparing `bioat-0.1.5.1/src/bioat/table.py` & `bioat-0.1.5.2/src/bioat/table.py`

 * *Files identical despite different names*

### Comparing `bioat-0.1.5.1/PKG-INFO` & `bioat-0.1.5.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioat
-Version: 0.1.5.1
+Version: 0.1.5.2
 Summary: Bioinformatic toolkit with python (It's still under development!)
 Home-page: https://github.com/hermanzhaozzzz/BioinformaticAnalysisTools
 License: MIT
 Author: Herman Zhao
 Author-email: hermanzhaozzzz@gmail.com
 Requires-Python: >=3.9.6,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -15,14 +15,15 @@
 Requires-Dist: cython (>=0.29.33,<0.30.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (>=1.24.1,<2.0.0)
 Requires-Dist: pandarallel (>=1.6.4,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pysam (>=0.20.0,<0.21.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Project-URL: Repository, https://github.com/hermanzhaozzzz/BioinformaticAnalysisTools
 Description-Content-Type: text/markdown
 
 # BioinformaticAnalysisTools
 
 ## Introduction
@@ -31,14 +32,15 @@
 \<under development\>
 
 - Author: Hua-nan ZHAO @Tsinghua University
 - E-Mail: hermanzhaozzzz@gmail.com
 
 ## Installation
 ```shell
+# supported platform: Linux / MacOS (intel & arm64) / WSL on Windows
 pip install --upgrade bioat
 ```
 
 
 ## usage
 ```shell
 # list commands
@@ -50,24 +52,9 @@
 
 # example usage
 bioat bam remove_clip --help
 samtools view -h test_sorted_n.bam | bioat bam remove_clip | tail
 ```
 
 ## known trouble
-- You should run bioat in a rosetta env while using Apple M Silicon-Arm64 (M1/M2) 
-    because that one dependent package [`pysam`](https://github.com/pysam-developers/pysam)
-    do not support this platform now. See below to use a rosetta env created by conda.
-```shell
-# create rosetta env
-CONDA_SUBDIR=osx-64 conda create -n rosetta python
-conda activate rosetta
-# in rosetta env
-python -c "import platform;print(platform.machine())"  # should print “x86_64”
-conda env config vars set CONDA_SUBDIR=osx-64
-conda deactivate      # need reactivate rosetta env to enable this var
-conda activate rosetta
-# now you can do this in this env
-pip install --upgrade bioat
-bioat version
-```
+- sometimes, pysam dependent foo.lib can be absent, just `brew install foo.lib` to fix it.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

