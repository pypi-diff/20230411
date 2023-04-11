# Comparing `tmp/genbank-0.69.tar.gz` & `tmp/genbank-0.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genbank-0.69.tar", last modified: Wed Feb  8 22:14:12 2023, max compression
+gzip compressed data, was "genbank-0.75.tar", last modified: Tue Apr 11 20:59:56 2023, max compression
```

## Comparing `genbank-0.69.tar` & `genbank-0.75.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 katelyn    (501) staff       (20)        0 2023-02-08 22:14:12.625660 genbank-0.69/
--rw-r--r--   0 katelyn    (501) staff       (20)    35149 2022-02-15 23:16:16.000000 genbank-0.69/LICENSE
--rw-r--r--   0 katelyn    (501) staff       (20)       51 2022-12-13 21:12:02.000000 genbank-0.69/MANIFEST.in
--rw-r--r--   0 katelyn    (501) staff       (20)     3209 2023-02-08 22:14:12.625352 genbank-0.69/PKG-INFO
--rw-r--r--   0 katelyn    (501) staff       (20)     2744 2022-12-13 21:12:02.000000 genbank-0.69/README.md
--rw-r--r--   0 katelyn    (501) staff       (20)        5 2023-02-07 21:34:05.000000 genbank-0.69/VERSION
-drwxr-xr-x   0 katelyn    (501) staff       (20)        0 2023-02-08 22:14:12.622935 genbank-0.69/genbank/
--rw-r--r--   0 katelyn    (501) staff       (20)        0 2022-02-15 23:20:41.000000 genbank-0.69/genbank/__init__.py
--rw-r--r--   0 katelyn    (501) staff       (20)     3235 2022-03-01 21:08:53.000000 genbank-0.69/genbank/codons.py
--rw-r--r--   0 katelyn    (501) staff       (20)     6129 2023-02-06 22:58:10.000000 genbank-0.69/genbank/feature.py
--rw-r--r--   0 katelyn    (501) staff       (20)     2918 2023-02-07 21:33:49.000000 genbank-0.69/genbank/file.py
--rw-r--r--   0 katelyn    (501) staff       (20)    11416 2023-02-07 21:24:21.000000 genbank-0.69/genbank/locus.py
--rw-r--r--   0 katelyn    (501) staff       (20)     2726 2022-03-08 22:07:42.000000 genbank-0.69/genbank/translate.py
-drwxr-xr-x   0 katelyn    (501) staff       (20)        0 2023-02-08 22:14:12.624258 genbank-0.69/genbank.egg-info/
--rw-r--r--   0 katelyn    (501) staff       (20)     3209 2023-02-08 22:14:12.000000 genbank-0.69/genbank.egg-info/PKG-INFO
--rw-r--r--   0 katelyn    (501) staff       (20)      310 2023-02-08 22:14:12.000000 genbank-0.69/genbank.egg-info/SOURCES.txt
--rw-r--r--   0 katelyn    (501) staff       (20)        1 2023-02-08 22:14:12.000000 genbank-0.69/genbank.egg-info/dependency_links.txt
--rw-r--r--   0 katelyn    (501) staff       (20)        8 2023-02-08 22:14:12.000000 genbank-0.69/genbank.egg-info/top_level.txt
--rw-r--r--   0 katelyn    (501) staff       (20)     5971 2023-02-03 01:57:14.000000 genbank-0.69/genbank.py
--rw-r--r--   0 katelyn    (501) staff       (20)       38 2023-02-08 22:14:12.625731 genbank-0.69/setup.cfg
--rw-r--r--   0 katelyn    (501) staff       (20)     1397 2022-03-30 22:21:48.000000 genbank-0.69/setup.py
-drwxr-xr-x   0 katelyn    (501) staff       (20)        0 2023-02-08 22:14:12.624635 genbank-0.69/tests/
--rw-r--r--   0 katelyn    (501) staff       (20)      126 2022-04-07 22:19:14.000000 genbank-0.69/tests/small.fasta
+drwxr-xr-x   0 katelyn    (501) staff       (20)        0 2023-04-11 20:59:56.130232 genbank-0.75/
+-rw-r--r--   0 katelyn    (501) staff       (20)    35149 2022-02-15 23:16:16.000000 genbank-0.75/LICENSE
+-rw-r--r--   0 katelyn    (501) staff       (20)       51 2022-12-13 21:12:02.000000 genbank-0.75/MANIFEST.in
+-rw-r--r--   0 katelyn    (501) staff       (20)     3209 2023-04-11 20:59:56.130005 genbank-0.75/PKG-INFO
+-rw-r--r--   0 katelyn    (501) staff       (20)     2744 2022-12-13 21:12:02.000000 genbank-0.75/README.md
+-rw-r--r--   0 katelyn    (501) staff       (20)        5 2023-04-11 20:58:36.000000 genbank-0.75/VERSION
+drwxr-xr-x   0 katelyn    (501) staff       (20)        0 2023-04-11 20:59:56.128481 genbank-0.75/genbank/
+-rw-r--r--   0 katelyn    (501) staff       (20)        0 2022-02-15 23:20:41.000000 genbank-0.75/genbank/__init__.py
+-rw-r--r--   0 katelyn    (501) staff       (20)     3235 2022-03-01 21:08:53.000000 genbank-0.75/genbank/codons.py
+-rw-r--r--   0 katelyn    (501) staff       (20)     6602 2023-02-15 02:40:07.000000 genbank-0.75/genbank/feature.py
+-rw-r--r--   0 katelyn    (501) staff       (20)     2918 2023-02-07 21:33:49.000000 genbank-0.75/genbank/file.py
+-rw-r--r--   0 katelyn    (501) staff       (20)    11229 2023-03-20 20:20:53.000000 genbank-0.75/genbank/locus.py
+-rw-r--r--   0 katelyn    (501) staff       (20)      371 2023-04-11 20:58:21.000000 genbank-0.75/genbank/sequence.py
+-rw-r--r--   0 katelyn    (501) staff       (20)     2726 2022-03-08 22:07:42.000000 genbank-0.75/genbank/translate.py
+drwxr-xr-x   0 katelyn    (501) staff       (20)        0 2023-04-11 20:59:56.129486 genbank-0.75/genbank.egg-info/
+-rw-r--r--   0 katelyn    (501) staff       (20)     3209 2023-04-11 20:59:56.000000 genbank-0.75/genbank.egg-info/PKG-INFO
+-rw-r--r--   0 katelyn    (501) staff       (20)      330 2023-04-11 20:59:56.000000 genbank-0.75/genbank.egg-info/SOURCES.txt
+-rw-r--r--   0 katelyn    (501) staff       (20)        1 2023-04-11 20:59:56.000000 genbank-0.75/genbank.egg-info/dependency_links.txt
+-rw-r--r--   0 katelyn    (501) staff       (20)        8 2023-04-11 20:59:56.000000 genbank-0.75/genbank.egg-info/top_level.txt
+-rw-r--r--   0 katelyn    (501) staff       (20)     5972 2023-02-27 22:07:26.000000 genbank-0.75/genbank.py
+-rw-r--r--   0 katelyn    (501) staff       (20)       38 2023-04-11 20:59:56.130301 genbank-0.75/setup.cfg
+-rw-r--r--   0 katelyn    (501) staff       (20)     1397 2022-03-30 22:21:48.000000 genbank-0.75/setup.py
+drwxr-xr-x   0 katelyn    (501) staff       (20)        0 2023-04-11 20:59:56.129729 genbank-0.75/tests/
+-rw-r--r--   0 katelyn    (501) staff       (20)      126 2022-04-07 22:19:14.000000 genbank-0.75/tests/small.fasta
```

### Comparing `genbank-0.69/LICENSE` & `genbank-0.75/LICENSE`

 * *Files identical despite different names*

### Comparing `genbank-0.69/PKG-INFO` & `genbank-0.75/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genbank
-Version: 0.69
+Version: 0.75
 Summary: Code to work with Genbank files
 Home-page: https://github.com/deprekate/genbank
 Author: Katelyn McNair
 Author-email: deprekate@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `genbank-0.69/README.md` & `genbank-0.75/README.md`

 * *Files identical despite different names*

### Comparing `genbank-0.69/genbank/codons.py` & `genbank-0.75/genbank/codons.py`

 * *Files identical despite different names*

### Comparing `genbank-0.69/genbank/feature.py` & `genbank-0.75/genbank/feature.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from itertools import zip_longest, chain
 import textwrap
 import copy
 
+from genbank.sequence import Seq
 
 def rev_comp(dna):
 	a = 'acgtrykmbvdh'
 	b = 'tgcayrmkvbhd'
 	tab = str.maketrans(a,b)
 	return dna.translate(tab)[::-1]
 
@@ -24,27 +25,72 @@
 		self.strand = strand
 		# tuplize the pairs
 		self.pairs = tuple([tuple(pair) for pair in pairs])
 		self.locus = locus
 		self.tags = tags if tags else dict()
 		#self.dna = ''
 		#self.partial = False
+
+	def frame(self, end='left'):
+		if self.type != 'CDS':
+			return 0
+		elif end == 'right' or self.partial() == 'left':
+			return (self.right()%3+1) * self.strand
+		elif end == 'left' or self.partial() == 'right':
+			return (self.left()%3+1) * self.strand
+
+	def left(self):
+		# convert genbank 1-based indexing to standard 0-based
+		# this is probably not right for <1 that should -2
+		return nint(self.pairs[0][0]) - 1
+	
+	def right(self):
+		# convert genbank 1-based indexing to standard 0-based
+		return nint(self.pairs[-1][-1]) - 3
 	
 	def length(self):
 		return len(self.seq())
 
 	def seq(self):
 		seq = ''
 		for n in self.base_locations():
 			seq += self.locus.seq(n,n+1, self.strand)
 		if self.strand > 0:
 			return seq
 		else:
 			return seq[::-1]
 
+	def base_locations(self, full=True):
+		#if full and self.partial() == 'left': 
+		if self.partial() == 'left': 
+			for i in range(-(self.frame()%3),0,1): #range(-((3 - self.frame() % 3) % 3), 0, 1):
+				yield i
+		for left,right in self:
+			#left,right = map(int, [ item.replace('<','').replace('>','') for item in self.pair ] )
+			for i in range(left,right+1):
+				if i < self.locus.length():
+					yield i
+
+	def codon_locations(self, full=True):
+		assert self.type == 'CDS'
+		for triplet in grouper(self.base_locations(full=True), 3):
+			#if triplet[0] >= 0:
+			yield triplet
+
+	def codons(self):
+		assert self.type == 'CDS'
+		if self.strand > 0:
+			for locations in self.codon_locations():
+				#yield ''.join([self.locus.dna[loc] if loc else '' for loc in locations])
+				yield self.locus.seq()[locations[0]:locations[2]+1]
+		else:
+			for locations in self.codon_locations():
+				#yield rev_comp(''.join([self.locus.dna[loc] if loc else '' for loc in locations]))
+				yield rev_comp(self.locus.seq()[ locations[0] : locations[2]+1 ])
+
 	def fna(self):
 		return self.header() + self.seq() + "\n"
 
 	def faa(self):
 		return self.header() + self.translation() + "\n"
 	
 	def header(self):
@@ -54,22 +100,14 @@
 				for value in values:
 					if value:
 						header += " [" + tag + "=" + value +"]"
 					else:
 						header += " [" + tag +"]"
 		return header + "\n"
 
-	def frame(self, end):
-		if self.type != 'CDS':
-			return 0
-		elif end == 'right':
-			return (self.right()%3+1) * self.strand
-		elif end == 'left':
-			return (self.left()%3+1) * self.strand
-
 	def hypothetical(self):
 		function = self.tags['product'] if 'product' in self.tags else ''
 		if 'hypot'  in function or \
 		   'etical' in function or \
 		   'unchar' in function or \
 		   ('orf' in function and 'orfb' not in function):
 			return True
@@ -91,22 +129,14 @@
 
 	def is_type(self, _type):
 		if self.type == _type:
 			return True
 		else:
 			return False
 
-	def left(self):
-		# convert genbank 1-based indexing to standard 0-based
-		return nint(self.pairs[0][0]) - 1
-	
-	def right(self):
-		# convert genbank 1-based indexing to standard 0-based
-		return nint(self.pairs[-1][-1]) - 3
-
 	def is_joined(self):
 		if len(self.pairs) > 1:
 			return True
 		return False
 
 	def __iter__(self):
 		for left,*right in self.pairs:
@@ -152,47 +182,23 @@
 		if len(pairs) > 1:
 			location = 'join(' + location + ')'
 		if self.strand < 0:
 			location = 'complement(' + location + ')'
 		return location
 
 
-	def base_locations(self, full=False):
-		if full and self.partial() == 'left': 
-			for i in range(-((3 - self.length() % 3) % 3), 0, 1):
-				yield i
-		for left,right in self:
-			#left,right = map(int, [ item.replace('<','').replace('>','') for item in self.pair ] )
-			for i in range(left,right+1):
-				if i < self.locus.length():
-					yield i
-
-	def codon_locations(self):
-		assert self.type == 'CDS'
-		for triplet in grouper(self.base_locations(full=True), 3):
-			if triplet[0] >= 0:
-				yield triplet
-
-	def codons(self):
-		assert self.type == 'CDS'
-		for locations in self.codon_locations():
-			if self.strand > 0:
-				yield ''.join([self.locus.dna[loc] if loc else '' for loc in locations])
-			else:
-				yield rev_comp(''.join([self.locus.dna[loc] if loc else '' for loc in locations]))
-
 	def split(self):
 		a = copy.copy(self)
 		b = copy.copy(self)
 		return a,b
 
 	def translation(self):
 		aa = []
 		codon = ''
-		first = 0 if not self.partial() else self.length() % 3
+		first = self.length() % 3 if (self.partial() == 'left' and self.strand > 0) or (self.partial() == 'right' and self.strand < 0) else 0
 		dna = self.seq()
 		for i in range(first, self.length(), 3):
 			codon = dna[ i : i+3 ]
 			aa.append(self.locus.translate.codon(codon))
 		#if self.strand < 0:
 		#	aa = aa[::-1]
 		# keeping the stop codon character adds 'information' as does which of
```

### Comparing `genbank-0.69/genbank/file.py` & `genbank-0.75/genbank/file.py`

 * *Files identical despite different names*

### Comparing `genbank-0.69/genbank/locus.py` & `genbank-0.75/genbank/locus.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from collections.abc import Sequence
 from itertools import chain
 
 from genbank.codons import Last
 from genbank.codons import Next
 from genbank.codons import Codons
 from genbank.feature import Feature
+from genbank.sequence import Seq
 from genbank.translate import Translate
 
 def rev_comp(dna):
 	a = 'acgtrykmbvdh'
 	b = 'tgcayrmkvbhd'
 	tab = str.maketrans(a,b)
 	return dna.translate(tab)[::-1]
@@ -28,23 +29,14 @@
 			out.append(func(item))
 	return type(items)(out)
 
 def recursive_map(func, items):
     return (recursive_map(func, x) if isinstance(x, tuple) else func(x) for x in items)
 
 
-class Seq(str):
-	# this is just to capture negative string indices as zero
-	def __getitem__(self, key):
-		if isinstance(key, slice) and key.start < 0:
-			key = slice(0, key.stop, key.step)
-		elif isinstance(key, int) and key >= len(self):
-			return ''
-		return super().__getitem__(key)
-
 class Locus(dict):
 	def __init__(self, name='', dna=''):
 		if not hasattr(self, 'feature'):
 			self.feature = Feature
 		#self.name = name
 		self.dna = dna.lower()
 		#self.codons = dict()
@@ -57,15 +49,16 @@
 
 	def __init_subclass__(cls, feature=Feature, **kwargs):
 		'''this method allows for a Feature class to be modified through inheritance in other code '''
 		super().__init_subclass__(**kwargs)
 		cls.feature = feature
 
 	def name(self):
-		return self.groups['LOCUS'][0].split()[0]
+		#return self.groups['LOCUS'][0].split()[0]
+		return self.groups['LOCUS'][0].split(' ')[0]
 
 	def molecule(self):
 		if len(locus) > 2:
 			return locus[3]
 		else:
 			return 'DNA'
 
@@ -76,16 +69,16 @@
 
 	def seq(self, left=0, right=None, strand=None):
 		# this should always refer to zero based indexing
 		#if strand is None:
 		#	strand = self.strand
 		if left < 0:
 			left = None
-		#if right is None:
-		#	right = self.length() - 1
+		if right and right < 0:
+			right = 0
 		if strand and strand < 0:
 			return Seq(rev_comp(self.dna[left : right]))
 		else:
 			return Seq(         self.dna[left : right] )
 
 	def length(self):
 		return len(self.dna)
@@ -175,33 +168,33 @@
 			self.write_gbk(outfile)
 		elif args.format == 'gff':
 			self.write_gff(outfile)
 		elif args.format == 'gff3':
 			self.write_gff3(outfile)
 
 	def write_gbk(self, outfile=sys.stdout):
-		for group,values in chain(self.groups.items(), [[None,[None]]] ):
+		for group,values in chain(self.groups.items(), [[None,[True, False]]] ):
 			for value in values:
 				if group == 'LOCUS':
 					outfile.write('LOCUS       ')
 					cols = self.groups['LOCUS'][0].split(' ')
 					# I eventually need to properly format the locus line
 					outfile.write(self.name().ljust(9))
 					outfile.write(str(len(self.dna)).rjust(19))
 					outfile.write(' bp ')
 					if 'bp' in cols:
 						outfile.write(' '.join(cols[cols.index('bp')+1:]))
 					else:
 						outfile.write('\n')
 					continue
-				elif group == 'FEATURES' or (not group and 'FEATURES' not in self.groups):
+				elif group == 'FEATURES' or (not group and value and 'FEATURES' not in self.groups):
 					outfile.write('FEATURES             Location/Qualifiers\n')
 					for feature in self:
 						feature.write(outfile)
-				elif group == 'ORIGIN' or (not group and 'ORIGIN' not in self.groups):
+				elif group == 'ORIGIN' or (not group and not value and 'ORIGIN' not in self.groups):
 					# should there be spaces after ORIGIN?
 					outfile.write('ORIGIN      ')
 					i = 0
 					dna = textwrap.wrap(self.dna, 10)
 					for block in dna:
 						if(i%60 == 0):
 							outfile.write('\n')
```

### Comparing `genbank-0.69/genbank/translate.py` & `genbank-0.75/genbank/translate.py`

 * *Files identical despite different names*

### Comparing `genbank-0.69/genbank.egg-info/PKG-INFO` & `genbank-0.75/genbank.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genbank
-Version: 0.69
+Version: 0.75
 Summary: Code to work with Genbank files
 Home-page: https://github.com/deprekate/genbank
 Author: Katelyn McNair
 Author-email: deprekate@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `genbank-0.69/genbank.py` & `genbank-0.75/genbank.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 	parser.add_argument('-e', '--edit', help='This edits the given feature key with the value from the shell input via < new_keys.txt', type=str, default=None)
 	parser.add_argument('-k', '--key', help='Print the given keys [and qualifiers]', type=str, default=None)
 	args = parser.parse_args()
 
 	if not args.get:
 		genbank = File(args.infile)
 	else:
-		raise Exception("not implemented yet")
+		#raise Exception("not implemented yet")
 		# not ready yet
 		accession,rettype = args.infile.split('.')
 		with urllib.request.urlopen('http://eutils.ncbi.nlm.nih.gov/entrez/eutils/efetch.fcgi?db=nuccore&id=' + accession + '&rettype=' + rettype + '&retmode=text') as response:
 			with tempfile.NamedTemporaryFile() as tmp:
 				shutil.copyfileobj(response, tmp)
 				genbank = File(tmp.name)
```

### Comparing `genbank-0.69/setup.py` & `genbank-0.75/setup.py`

 * *Files identical despite different names*

