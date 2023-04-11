# Comparing `tmp/doc2tei-CERTIC-0.0.8.tar.gz` & `tmp/doc2tei-CERTIC-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doc2tei-CERTIC-0.0.8.tar", last modified: Fri May 21 15:00:37 2021, max compression
+gzip compressed data, was "doc2tei-CERTIC-0.0.9.tar", last modified: Thu Jul  1 08:42:03 2021, max compression
```

## Comparing `doc2tei-CERTIC-0.0.8.tar` & `doc2tei-CERTIC-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,40 @@
-drwxr-xr-x   0 mickael    (501) staff       (20)        0 2021-05-21 15:00:37.537492 doc2tei-CERTIC-0.0.8/
--rw-r--r--   0 mickael    (501) staff       (20)       64 2021-05-21 14:46:27.000000 doc2tei-CERTIC-0.0.8/MANIFEST.in
--rw-r--r--   0 mickael    (501) staff       (20)      523 2021-05-21 15:00:37.537375 doc2tei-CERTIC-0.0.8/PKG-INFO
-drwxr-xr-x   0 mickael    (501) staff       (20)        0 2021-05-21 15:00:37.532943 doc2tei-CERTIC-0.0.8/doc2tei/
--rw-r--r--   0 mickael    (501) staff       (20)     4803 2021-05-21 14:54:52.000000 doc2tei-CERTIC-0.0.8/doc2tei/__init__.py
-drwxr-xr-x   0 mickael    (501) staff       (20)        0 2021-05-21 15:00:37.533243 doc2tei-CERTIC-0.0.8/doc2tei/resources/
--rw-r--r--   0 mickael    (501) staff       (20)    14095 2021-05-21 14:46:27.000000 doc2tei-CERTIC-0.0.8/doc2tei/resources/cleanup.xsl
--rw-r--r--   0 mickael    (501) staff       (20)     4012 2021-05-21 14:46:27.000000 doc2tei-CERTIC-0.0.8/doc2tei/resources/hierarchize.xsl
--rw-r--r--   0 mickael    (501) staff       (20)  5046534 2021-05-21 14:46:27.000000 doc2tei-CERTIC-0.0.8/doc2tei/resources/saxon9.jar
-drwxr-xr-x   0 mickael    (501) staff       (20)        0 2021-05-21 15:00:37.537225 doc2tei-CERTIC-0.0.8/doc2tei_CERTIC.egg-info/
--rw-r--r--   0 mickael    (501) staff       (20)      523 2021-05-21 15:00:37.000000 doc2tei-CERTIC-0.0.8/doc2tei_CERTIC.egg-info/PKG-INFO
--rw-r--r--   0 mickael    (501) staff       (20)      322 2021-05-21 15:00:37.000000 doc2tei-CERTIC-0.0.8/doc2tei_CERTIC.egg-info/SOURCES.txt
--rw-r--r--   0 mickael    (501) staff       (20)        1 2021-05-21 15:00:37.000000 doc2tei-CERTIC-0.0.8/doc2tei_CERTIC.egg-info/dependency_links.txt
--rw-r--r--   0 mickael    (501) staff       (20)       13 2021-05-21 15:00:37.000000 doc2tei-CERTIC-0.0.8/doc2tei_CERTIC.egg-info/requires.txt
--rw-r--r--   0 mickael    (501) staff       (20)        8 2021-05-21 15:00:37.000000 doc2tei-CERTIC-0.0.8/doc2tei_CERTIC.egg-info/top_level.txt
--rw-r--r--   0 mickael    (501) staff       (20)       38 2021-05-21 15:00:37.537528 doc2tei-CERTIC-0.0.8/setup.cfg
--rw-r--r--   0 mickael    (501) staff       (20)      721 2021-05-21 14:55:15.000000 doc2tei-CERTIC-0.0.8/setup.py
+drwxr-xr-x   0 mickael    (501) staff       (20)        0 2021-07-01 08:42:03.940081 doc2tei-CERTIC-0.0.9/
+-rw-r--r--   0 mickael    (501) staff       (20)       64 2021-06-10 06:27:08.000000 doc2tei-CERTIC-0.0.9/MANIFEST.in
+-rw-r--r--   0 mickael    (501) staff       (20)      523 2021-07-01 08:42:03.939950 doc2tei-CERTIC-0.0.9/PKG-INFO
+-rw-r--r--   0 mickael    (501) staff       (20)     1710 2021-06-24 15:26:57.000000 doc2tei-CERTIC-0.0.9/README.md
+drwxr-xr-x   0 mickael    (501) staff       (20)        0 2021-07-01 08:42:03.928903 doc2tei-CERTIC-0.0.9/doc2tei/
+-rw-r--r--   0 mickael    (501) staff       (20)     8432 2021-06-29 14:10:57.000000 doc2tei-CERTIC-0.0.9/doc2tei/__init__.py
+drwxr-xr-x   0 mickael    (501) staff       (20)        0 2021-07-01 08:42:03.928999 doc2tei-CERTIC-0.0.9/doc2tei/resources/
+drwxr-xr-x   0 mickael    (501) staff       (20)        0 2021-07-01 08:42:03.932511 doc2tei-CERTIC-0.0.9/doc2tei/resources/cleanup/
+-rw-r--r--   0 mickael    (501) staff       (20)    16502 2021-06-29 12:33:42.000000 doc2tei-CERTIC-0.0.9/doc2tei/resources/cleanup/cleanup.xsl
+drwxr-xr-x   0 mickael    (501) staff       (20)        0 2021-07-01 08:42:03.936394 doc2tei-CERTIC-0.0.9/doc2tei/resources/control/
+-rw-r--r--   0 mickael    (501) staff       (20)     3812 2021-06-29 13:07:08.000000 doc2tei-CERTIC-0.0.9/doc2tei/resources/control/control.xsl
+drwxr-xr-x   0 mickael    (501) staff       (20)        0 2021-07-01 08:42:03.936636 doc2tei-CERTIC-0.0.9/doc2tei/resources/hierarchize/
+-rw-r--r--   0 mickael    (501) staff       (20)     4349 2021-06-29 12:33:42.000000 doc2tei-CERTIC-0.0.9/doc2tei/resources/hierarchize/hierarchize.xsl
+drwxr-xr-x   0 mickael    (501) staff       (20)        0 2021-07-01 08:42:03.937995 doc2tei-CERTIC-0.0.9/doc2tei/resources/normalisation/
+-rw-r--r--   0 mickael    (501) staff       (20)     2963 2021-06-29 12:33:42.000000 doc2tei-CERTIC-0.0.9/doc2tei/resources/normalisation/bookmark.xsl
+-rw-r--r--   0 mickael    (501) staff       (20)     2821 2021-06-29 12:33:42.000000 doc2tei-CERTIC-0.0.9/doc2tei/resources/normalisation/img.xsl
+-rw-r--r--   0 mickael    (501) staff       (20)     7722 2021-06-29 12:33:42.000000 doc2tei-CERTIC-0.0.9/doc2tei/resources/normalisation/index.xsl
+-rw-r--r--   0 mickael    (501) staff       (20)     2448 2021-06-29 12:33:42.000000 doc2tei-CERTIC-0.0.9/doc2tei/resources/normalisation/list.xsl
+-rw-r--r--   0 mickael    (501) staff       (20)     2064 2021-06-29 12:33:42.000000 doc2tei-CERTIC-0.0.9/doc2tei/resources/normalisation/math.xsl
+-rw-r--r--   0 mickael    (501) staff       (20)     2748 2021-06-29 12:33:42.000000 doc2tei-CERTIC-0.0.9/doc2tei/resources/normalisation/normalize.xsl
+-rw-r--r--   0 mickael    (501) staff       (20)     2863 2021-06-29 12:33:42.000000 doc2tei-CERTIC-0.0.9/doc2tei/resources/normalisation/notes.xsl
+-rw-r--r--   0 mickael    (501) staff       (20)     2571 2021-06-29 12:33:42.000000 doc2tei-CERTIC-0.0.9/doc2tei/resources/normalisation/table.xsl
+-rw-r--r--   0 mickael    (501) staff       (20)  5046534 2021-06-10 06:27:08.000000 doc2tei-CERTIC-0.0.9/doc2tei/resources/saxon9.jar
+drwxr-xr-x   0 mickael    (501) staff       (20)        0 2021-07-01 08:42:03.939200 doc2tei-CERTIC-0.0.9/doc2tei/resources/totei-modules/
+-rw-r--r--   0 mickael    (501) staff       (20)     2975 2021-06-29 12:33:42.000000 doc2tei-CERTIC-0.0.9/doc2tei/resources/totei-modules/back_biblio.xsl
+-rw-r--r--   0 mickael    (501) staff       (20)     3329 2021-06-29 12:33:42.000000 doc2tei-CERTIC-0.0.9/doc2tei/resources/totei-modules/core_div-para.xsl
+-rw-r--r--   0 mickael    (501) staff       (20)     3606 2021-06-29 12:33:42.000000 doc2tei-CERTIC-0.0.9/doc2tei/resources/totei-modules/core_linking.xsl
+-rw-r--r--   0 mickael    (501) staff       (20)     3240 2021-06-29 12:33:42.000000 doc2tei-CERTIC-0.0.9/doc2tei/resources/totei-modules/core_note.xsl
+-rw-r--r--   0 mickael    (501) staff       (20)     3242 2021-06-29 12:33:42.000000 doc2tei-CERTIC-0.0.9/doc2tei/resources/totei-modules/core_quote.xsl
+-rw-r--r--   0 mickael    (501) staff       (20)     4734 2021-06-29 12:33:42.000000 doc2tei-CERTIC-0.0.9/doc2tei/resources/totei-modules/core_table.xsl
+-rw-r--r--   0 mickael    (501) staff       (20)     3024 2021-06-29 12:33:42.000000 doc2tei-CERTIC-0.0.9/doc2tei/resources/totei-modules/core_typo.xsl
+-rw-r--r--   0 mickael    (501) staff       (20)     4667 2021-06-29 12:33:42.000000 doc2tei-CERTIC-0.0.9/doc2tei/resources/totei-modules/totei.xsl
+drwxr-xr-x   0 mickael    (501) staff       (20)        0 2021-07-01 08:42:03.939770 doc2tei-CERTIC-0.0.9/doc2tei_CERTIC.egg-info/
+-rw-r--r--   0 mickael    (501) staff       (20)      523 2021-07-01 08:42:03.000000 doc2tei-CERTIC-0.0.9/doc2tei_CERTIC.egg-info/PKG-INFO
+-rw-r--r--   0 mickael    (501) staff       (20)     1104 2021-07-01 08:42:03.000000 doc2tei-CERTIC-0.0.9/doc2tei_CERTIC.egg-info/SOURCES.txt
+-rw-r--r--   0 mickael    (501) staff       (20)        1 2021-07-01 08:42:03.000000 doc2tei-CERTIC-0.0.9/doc2tei_CERTIC.egg-info/dependency_links.txt
+-rw-r--r--   0 mickael    (501) staff       (20)       13 2021-07-01 08:42:03.000000 doc2tei-CERTIC-0.0.9/doc2tei_CERTIC.egg-info/requires.txt
+-rw-r--r--   0 mickael    (501) staff       (20)        8 2021-07-01 08:42:03.000000 doc2tei-CERTIC-0.0.9/doc2tei_CERTIC.egg-info/top_level.txt
+-rw-r--r--   0 mickael    (501) staff       (20)       38 2021-07-01 08:42:03.940120 doc2tei-CERTIC-0.0.9/setup.cfg
+-rw-r--r--   0 mickael    (501) staff       (20)      721 2021-07-01 08:41:39.000000 doc2tei-CERTIC-0.0.9/setup.py
```

### Comparing `doc2tei-CERTIC-0.0.8/PKG-INFO` & `doc2tei-CERTIC-0.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doc2tei-CERTIC
-Version: 0.0.8
+Version: 0.0.9
 Summary: Convert ODT and DOCX files to TEI
 Home-page: https://git.unicaen.fr/fnso/i-fair-ir/xsl-tei-circe
 Author: Mickaël Desfrênes
 Author-email: mickael.desfrenes@unicaen.fr
 License: UNKNOWN
 Description: Convert ODT and DOCX files to TEI
 Platform: UNKNOWN
```

### Comparing `doc2tei-CERTIC-0.0.8/doc2tei/resources/cleanup.xsl` & `doc2tei-CERTIC-0.0.9/doc2tei/resources/cleanup/cleanup.xsl`

 * *Files 16% similar despite different names*

```diff
@@ -107,14 +107,15 @@
 <xsl:template match="office:forms"/>
 <!-- caractères de saut, tabulations -->
 <xsl:template match="text:soft-page-break"/>
 <xsl:template match="text:tab"/>
 <xsl:template match="text:s"/> <!-- This element shall be used to represent the second and all following “ “ (U+0020, SPACE) characters in a sequence of “ “ (U+0020, SPACE) characters. -->
 <!-- ancres par défaut -->
 <xsl:template match="text:bookmark[starts-with(@text:name,'_')]"/>
+<xsl:template match="text:bookmark[starts-with(@text:name,'RANGE!')]"/>
 <!-- images en binaire -->
 <xsl:template match="office:binary-data"/>
 <!-- élément engloblant office:text (à conserver pour génération de la mainDiv) -->
 <!-- A priori office:body est toujours présents dans les fichiers. office:text n'est plus à conserver pour génération de la mainDiv-->
 <xsl:template match="office:text">
   <xsl:apply-templates/>
 </xsl:template>
@@ -139,14 +140,17 @@
 <xsl:choose>
     <!-- Suppression des éléments vides -->
     <xsl:when test=".[not(*|comment()|processing-instruction()) and normalize-space()='']"/>
     <!-- Gestion des enrichissements typographiques text:span -->
     <xsl:when test="$currentElementName='text:span'">
         <xsl:choose>
         <!-- enrichissements typo traitement de texte (l'application de styles de caractères ne génère pas de raccourcis de styles)-->
+            <xsl:when test="child::text:note">
+                <xsl:apply-templates/>
+            </xsl:when>
             <xsl:when test="matches(@text:style-name,'[T]\d{1,2}')">
                 <xsl:choose>
                     <!-- premier test pour une liste des propriétés retenus -->
                     <xsl:when test="//style:style[@style:name=$currentStyle]/style:text-properties/(@fo:font-style|@fo:font-variant|@fo:font-weight|@style:text-position|@style:text-underline-style)">
                     <xsl:element name="text:span">
                         <xsl:attribute name="rendition">
                         <!-- ajouter le rtl -->
@@ -223,15 +227,15 @@
                 <xsl:otherwise>
                     <xsl:copy-of select="@text:outline-level"/>
                 </xsl:otherwise>
             </xsl:choose>
             <xsl:apply-templates/>
         </xsl:element>
     </xsl:when>
-    <!-- Gestion du titre principale si source Libre Office : conversion de text:p à text:h  (à voir si besoin d'être conservé, car on peut affecter un niveau de plan via la stylage dans Libre Office) -->
+    <!-- Gestion du titre principal si source Libre Office : conversion de text:p à text:h  (à voir si besoin d'être conservé, car on peut affecter un niveau de plan via la stylage dans Libre Office) -->
     <xsl:when test="$currentElementName='text:p' and (@text:style-name='Title' or //style:style[@style:name=$currentStyle]/@style:parent-style-name='Title')">
         <xsl:element name="text:h">
             <xsl:copy-of select="@*"/>
             <xsl:attribute name="text:outline-level">0</xsl:attribute>
             <xsl:attribute name="text:style-name">
                 <xsl:choose>
                     <xsl:when test="matches($currentStyle,'[P]\d{1,2}')">
@@ -241,14 +245,59 @@
                         <xsl:value-of select="$currentStyle"/>
                     </xsl:otherwise>
                 </xsl:choose>
             </xsl:attribute>
             <xsl:apply-templates/>
         </xsl:element>
     </xsl:when>
+<!-- ajout d'un @outline-level sur le titre de section biblio-->
+	<xsl:when test="$currentElementName='text:p' and (@text:style-name='Titre-section-biblio' or //style:style[@style:name=$currentStyle]/@style:parent-style-name='Titre-section-biblio')">
+		<xsl:element name="text:h">
+            <xsl:copy-of select="@*"/>
+            <xsl:attribute name="text:outline-level">1</xsl:attribute>
+            <xsl:attribute name="subtype">biblio</xsl:attribute>
+            <xsl:attribute name="text:style-name">
+                <xsl:choose>
+                    <xsl:when test="matches($currentStyle,'[P]\d{1,2}')">
+                        <xsl:value-of select="//style:style[@style:name=$currentStyle]/@style:parent-style-name"/>
+                    </xsl:when>
+                    <xsl:otherwise>
+                        <xsl:value-of select="$currentStyle"/>
+                    </xsl:otherwise>
+                </xsl:choose>
+            </xsl:attribute>
+            <xsl:apply-templates/>
+        </xsl:element>
+	</xsl:when>
+    <xsl:when test="$currentElementName='text:list'">
+        <xsl:choose>
+            <xsl:when test="descendant::text:h">
+                <xsl:apply-templates select="descendant::text:h"/>
+            </xsl:when>
+        <xsl:otherwise>
+            <xsl:comment>Que fait-on ?</xsl:comment>
+            <xsl:variable name="firstChild">
+                <xsl:copy-of select="//text:list-style[@style:name=$currentStyle]/*[1]/local-name()"/>
+            </xsl:variable>
+            <xsl:element name="{$currentElementName}">
+                <xsl:copy-of select="@*"/>
+                <xsl:choose>
+                    <xsl:when test="$firstChild='list-level-style-number'">
+                        <xsl:attribute name="type">ordered</xsl:attribute>
+                        <xsl:copy-of select="//text:list-style[@style:name=$currentStyle]/*[1]/@style:num-format"/>
+                    </xsl:when>
+                    <xsl:otherwise>
+                        <xsl:attribute name="type">unordered</xsl:attribute>
+                    </xsl:otherwise>
+                </xsl:choose>
+                <xsl:apply-templates/>
+            </xsl:element>
+        </xsl:otherwise>
+        </xsl:choose>
+    </xsl:when>
     <!-- Gestion des autres éléments -->
     <xsl:otherwise>
         <xsl:element name="{$currentElementName}">
             <xsl:copy-of select="@*"/>
             <xsl:attribute name="text:style-name">
                 <xsl:choose>
                     <!-- est-ce qu'on estime que le système de nommage des raccourcis de styles est normalisé ? -->
```

### Comparing `doc2tei-CERTIC-0.0.8/doc2tei/resources/hierarchize.xsl` & `doc2tei-CERTIC-0.0.9/doc2tei/resources/hierarchize/hierarchize.xsl`

 * *Files 10% similar despite different names*

#### Comparing `doc2tei-CERTIC-0.0.8/doc2tei/resources/hierarchize.xsl` & `doc2tei-CERTIC-0.0.9/doc2tei/resources/hierarchize/hierarchize.xsl`

```diff
@@ -4,31 +4,41 @@
   <xsl:template match="@*|node()">
     <xsl:copy>
       <xsl:apply-templates select="@*|node()"/>
     </xsl:copy>
   </xsl:template>
   <!-- Match sur le corps du document, on ne touche pas au reste. On active le traitement sur le niveau de titre le plus haut (0) -->
   <xsl:template match="office:body">
-    <div type="article">
+    <text>
       <xsl:for-each-group select="*" group-starting-with="text:h[@text:outline-level=0]">
         <xsl:call-template name="addDiv">
           <xsl:with-param name="level" select="1"/>
           <xsl:with-param name="currentGroup" select="current-group()"/>
         </xsl:call-template>
       </xsl:for-each-group>
-    </div>
+    </text>
   </xsl:template>
   <!-- Pour chaque groupe commençant par un text:h, on relance le traitement en passant le niveau en paramètre. Si le groupe courant contient un text:h du niveau souhaité, le traitement se poursuit, sinon il s'arrête -->
   <xsl:template name="addDiv">
     <xsl:param name="level"/>
     <xsl:param name="currentGroup"/>
     <xsl:for-each-group select="$currentGroup" group-starting-with="text:h[@text:outline-level=$level]">
       <xsl:choose>
         <xsl:when test="self::text:h[@text:outline-level=$level]">
-          <div type="section{$level}">
+          <div>
+            <xsl:attribute name="type">
+              <xsl:choose>
+                <xsl:when test="@subtype='biblio'">
+                  <xsl:text>bibliography</xsl:text>
+                </xsl:when>
+                <xsl:otherwise>
+                  <xsl:value-of select="concat('section',$level)"/>
+                </xsl:otherwise>
+              </xsl:choose>
+            </xsl:attribute>
             <xsl:call-template name="addDiv">
               <xsl:with-param name="level" select="$level+1"/>
               <xsl:with-param name="currentGroup" select="current-group()"/>
             </xsl:call-template>
           </div>
         </xsl:when>
         <xsl:otherwise>
```

### Comparing `doc2tei-CERTIC-0.0.8/doc2tei/resources/saxon9.jar` & `doc2tei-CERTIC-0.0.9/doc2tei/resources/saxon9.jar`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.8/doc2tei_CERTIC.egg-info/PKG-INFO` & `doc2tei-CERTIC-0.0.9/doc2tei_CERTIC.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doc2tei-CERTIC
-Version: 0.0.8
+Version: 0.0.9
 Summary: Convert ODT and DOCX files to TEI
 Home-page: https://git.unicaen.fr/fnso/i-fair-ir/xsl-tei-circe
 Author: Mickaël Desfrênes
 Author-email: mickael.desfrenes@unicaen.fr
 License: UNKNOWN
 Description: Convert ODT and DOCX files to TEI
 Platform: UNKNOWN
```

### Comparing `doc2tei-CERTIC-0.0.8/setup.py` & `doc2tei-CERTIC-0.0.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="doc2tei-CERTIC",
-    version="0.0.8",
+    version="0.0.9",
     author="Mickaël Desfrênes",
     author_email="mickael.desfrenes@unicaen.fr",
     description="Convert ODT and DOCX files to TEI",
     long_description="Convert ODT and DOCX files to TEI",
     long_description_content_type="text/plain",
     url="https://git.unicaen.fr/fnso/i-fair-ir/xsl-tei-circe",
     packages=setuptools.find_packages(),
```

