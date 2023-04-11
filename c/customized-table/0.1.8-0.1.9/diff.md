# Comparing `tmp/customized_table-0.1.8.tar.gz` & `tmp/customized_table-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/customized_table-0.1.8.tar", last modified: Wed Mar  1 10:32:23 2023, max compression
+gzip compressed data, was "dist/customized_table-0.1.9.tar", last modified: Wed Mar  1 11:07:09 2023, max compression
```

## Comparing `customized_table-0.1.8.tar` & `customized_table-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-03-01 10:32:23.754855 customized_table-0.1.8/
--rw-r--r--   0 johanhagelback   (503) staff       (20)       91 2022-09-28 03:55:26.000000 customized_table-0.1.8/.gitignore
--rw-r--r--   0 johanhagelback   (503) staff       (20)    29327 2023-03-01 10:30:50.000000 customized_table-0.1.8/Docs.ipynb
--rw-r--r--   0 johanhagelback   (503) staff       (20)   110548 2023-03-01 10:27:47.000000 customized_table-0.1.8/Examples.ipynb
--rw-r--r--   0 johanhagelback   (503) staff       (20)     1073 2022-09-28 03:53:57.000000 customized_table-0.1.8/LICENSE
--rw-r--r--   0 johanhagelback   (503) staff       (20)      568 2023-03-01 10:32:23.753828 customized_table-0.1.8/PKG-INFO
--rw-r--r--   0 johanhagelback   (503) staff       (20)      544 2023-02-15 12:19:33.000000 customized_table-0.1.8/README.md
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-03-01 10:32:23.742952 customized_table-0.1.8/customized_table/
--rwxr-xr-x   0 johanhagelback   (503) staff       (20)      208 2023-03-01 10:26:16.000000 customized_table-0.1.8/customized_table/__init__.py
--rwxr-xr-x   0 johanhagelback   (503) staff       (20)    29501 2023-03-01 10:26:10.000000 customized_table-0.1.8/customized_table/customized_table.py
--rwxr-xr-x   0 johanhagelback   (503) staff       (20)    14342 2023-03-01 10:30:00.000000 customized_table-0.1.8/customized_table/docs.py
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-03-01 10:32:23.750613 customized_table-0.1.8/customized_table.egg-info/
--rw-r--r--   0 johanhagelback   (503) staff       (20)      568 2023-03-01 10:32:23.000000 customized_table-0.1.8/customized_table.egg-info/PKG-INFO
--rw-r--r--   0 johanhagelback   (503) staff       (20)      353 2023-03-01 10:32:23.000000 customized_table-0.1.8/customized_table.egg-info/SOURCES.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)        1 2023-03-01 10:32:23.000000 customized_table-0.1.8/customized_table.egg-info/dependency_links.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)       10 2023-03-01 10:32:23.000000 customized_table-0.1.8/customized_table.egg-info/requires.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)       17 2023-03-01 10:32:23.000000 customized_table-0.1.8/customized_table.egg-info/top_level.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)       38 2023-03-01 10:32:23.755082 customized_table-0.1.8/setup.cfg
--rw-r--r--   0 johanhagelback   (503) staff       (20)      675 2023-03-01 10:26:25.000000 customized_table-0.1.8/setup.py
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-03-01 11:07:09.385410 customized_table-0.1.9/
+-rw-r--r--   0 johanhagelback   (503) staff       (20)       91 2022-09-28 03:55:26.000000 customized_table-0.1.9/.gitignore
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    29366 2023-03-01 11:05:12.000000 customized_table-0.1.9/Docs.ipynb
+-rw-r--r--   0 johanhagelback   (503) staff       (20)   103035 2023-03-01 11:03:44.000000 customized_table-0.1.9/Examples.ipynb
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     1073 2022-09-28 03:53:57.000000 customized_table-0.1.9/LICENSE
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      568 2023-03-01 11:07:09.384507 customized_table-0.1.9/PKG-INFO
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      544 2023-02-15 12:19:33.000000 customized_table-0.1.9/README.md
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-03-01 11:07:09.376265 customized_table-0.1.9/customized_table/
+-rwxr-xr-x   0 johanhagelback   (503) staff       (20)      208 2023-03-01 10:50:31.000000 customized_table-0.1.9/customized_table/__init__.py
+-rwxr-xr-x   0 johanhagelback   (503) staff       (20)    30051 2023-03-01 10:58:22.000000 customized_table-0.1.9/customized_table/customized_table.py
+-rwxr-xr-x   0 johanhagelback   (503) staff       (20)    14381 2023-03-01 11:04:37.000000 customized_table-0.1.9/customized_table/docs.py
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-03-01 11:07:09.382921 customized_table-0.1.9/customized_table.egg-info/
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      568 2023-03-01 11:07:08.000000 customized_table-0.1.9/customized_table.egg-info/PKG-INFO
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      353 2023-03-01 11:07:09.000000 customized_table-0.1.9/customized_table.egg-info/SOURCES.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)        1 2023-03-01 11:07:08.000000 customized_table-0.1.9/customized_table.egg-info/dependency_links.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)       10 2023-03-01 11:07:09.000000 customized_table-0.1.9/customized_table.egg-info/requires.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)       17 2023-03-01 11:07:09.000000 customized_table-0.1.9/customized_table.egg-info/top_level.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)       38 2023-03-01 11:07:09.385634 customized_table-0.1.9/setup.cfg
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      675 2023-03-01 10:50:23.000000 customized_table-0.1.9/setup.py
```

### Comparing `customized_table-0.1.8/Docs.ipynb` & `customized_table-0.1.9/Docs.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997612847222221%*

 * *Differences: {"'cells'": "{0: {'outputs': {0: {'text': ['Version 0.1.9\\n']}}}, 6: {'outputs': {0: {'data': "*

 * *            "{'text/html': {insert: [(3, "*

 * *            '";font-family:Courier;font-size:12px;filter:brightness(100%);border-bottom:1px solid '*

 * *            "#aaa;font:Courier 12px;'>Generates a counts table (number of occurences for each "*

 * *            'item) from a list or dict.<br>Params:<br>&nbsp;<span '*

 * *            "style='color:#a44;font-style:italic;'>data</span> Data to generate counts from. <span "*

 * *        […]*

```diff
@@ -6,15 +6,15 @@
             "id": "532f5660-db16-400e-874f-77400e2f124d",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Version 0.1.8\n"
+                        "Version 0.1.9\n"
                     ]
                 }
             ],
             "source": [
                 "import customized_table\n",
                 "print(\"Version\", customized_table.__version__)\n",
                 "from customized_table import *\n",
@@ -118,15 +118,15 @@
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<table style='width=1110px; max-width:1110px; min-width:1110px; table-layout: fixed; word-wrap: break-word;'><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Courier;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Courier 12px;text-align:left;' width=220>Functions (general)</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Courier;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Courier 12px;text-align:left;'>Description</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#272;font-family:Courier;font-size:12px;font-weight:bold;filter:brightness(100%);font:Courier 12px;'>tag_text</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;cell-format:list:\n",
                             ";font-family:Courier;font-size:12px;filter:brightness(100%);font:Courier 12px;'>Handles tagged text strings. Tagged text strings can contain tags for text color and style.<br>Params:<br>&nbsp;<span style='color:#a44;font-style:italic;'>txt</span> Tagged text string. <span style='color:#888;'>(string)</span><br>Examples:<br>&nbsp;<span style='color:#a44;'>&lt;bold&gt;bold&lt;/&gt;</span> shows a <span style='font-weight:bold;'>bold</span> text.<br>&nbsp;<span style='color:#a44;'>&lt;italic&gt;titalic&lt;/&gt;</span> shows an <span style='font-style:italic;'>italic</span> text.<br>&nbsp;<span style='color:#a44;'>&lt;blue&gt;blue&lt;/&gt;</span> shows a <span style='color:blue;'>blue</span> text.<br>&nbsp;<span style='color:#a44;'>&lt;blue bold&gt;blue and bold&lt;/&gt;</span> shows a <span style='color:blue;font-weight:bold;'>blue and bold</span> text.<br>&nbsp;<span style='color:#a44;'>&lt;red italic&gt;red and italic&lt;/&gt;</span> shows a <span style='color:red;font-style:italic;'>red and italic</span> text.<br>&nbsp;<span style='color:#a44;'>&lt;#f708b1&gt;pink&lt;/&gt;</span> shows a <span style='color:#f708b1;'>pink</span> text.</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#272;font-family:Courier;font-size:12px;font-weight:bold;filter:brightness(96%);font:Courier 12px;'>from_csv</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;cell-format:list:\n",
                             ";font-family:Courier;font-size:12px;filter:brightness(96%);font:Courier 12px;'>Creates a table from a <span style='font-style:italic;'>csv</span> file.<br>Params:<br>&nbsp;<span style='color:#a44;font-style:italic;'>file</span> File name and path for the file. <span style='color:#888;'>(string)</span></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#272;font-family:Courier;font-size:12px;font-weight:bold;filter:brightness(100%);border-bottom:1px solid #aaa;font:Courier 12px;'>generate_counts</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;cell-format:list:\n",
-                            ";font-family:Courier;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Courier 12px;'>Generates a counts table (number of occurences for each item) from a list or dict.<br>Params:<br>&nbsp;<span style='color:#a44;font-style:italic;'>data</span> Data to generate counts from. <span style='color:#888;'>(list or dict)</span><br>&nbsp;<span style='color:#a44;font-style:italic;'>cidx</span> Column to generate counts from, if data is list of lists. <span style='color:#888;'>(column index, optional)</span><br>&nbsp;<span style='color:#a44;font-style:italic;'>title</span> Title of the table. <span style='color:#888;'>(string, optional)</span><br>&nbsp;<span style='color:#a44;font-style:italic;'>sort</span> How to sort the counts table. <span style='color:#888;'>(None for no sorting, or 'key', 'asc', 'desc')</span><br>&nbsp;<span style='color:#a44;font-style:italic;'>footer</span> What to show in the footer. <span style='color:#888;'>(list ('total','mean') or None)</span><br>&nbsp;<span style='color:#a44;font-style:italic;'>group</span> Group all entries after the specified row to make the table more compact. <span style='color:#888;'>(row index, optional)</span><br>&nbsp;<span style='color:#a44;font-style:italic;'>style</span> Changes default formatting. <span style='color:#888;'>(dict, optional)</span></td></tr></table>"
+                            ";font-family:Courier;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Courier 12px;'>Generates a counts table (number of occurences for each item) from a list or dict.<br>Params:<br>&nbsp;<span style='color:#a44;font-style:italic;'>data</span> Data to generate counts from. <span style='color:#888;'>(list or dict)</span><br>&nbsp;<span style='color:#a44;font-style:italic;'>cidx</span> Column to generate counts from, if data is list of lists. <span style='color:#888;'>(column index, optional)</span><br>&nbsp;<span style='color:#a44;font-style:italic;'>labels</span> Set labels for the counts table (title,no,part,total,mean). <span style='color:#888;'>(dict, optional)</span><br>&nbsp;<span style='color:#a44;font-style:italic;'>sort</span> How to sort the counts table. <span style='color:#888;'>(None for no sorting, or 'key', 'asc', 'desc')</span><br>&nbsp;<span style='color:#a44;font-style:italic;'>footer</span> What to show in the footer. <span style='color:#888;'>(list ('total','mean') or None)</span><br>&nbsp;<span style='color:#a44;font-style:italic;'>group</span> Group all entries after the specified row to make the table more compact. <span style='color:#888;'>(row index, optional)</span><br>&nbsp;<span style='color:#a44;font-style:italic;'>style</span> Changes default formatting. <span style='color:#888;'>(dict, optional)</span></td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
```

### Comparing `customized_table-0.1.8/Examples.ipynb` & `customized_table-0.1.9/Examples.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991355988882481%*

 * *Differences: {"'cells'": "{1: {'outputs': {0: {'text': ['0.1.9\\n']}}}, 6: {'source': {insert: [(0, 't = "*

 * *            'CustomizedTable(\\n\'), (1, \'    ["Title", "Year", "Rating"], \\n\'), (2, \'    '*

 * *            'subheader_style={"background": "#eef"}, \\n\'), (3, \'    header_style={"background": '*

 * *            '"#eef"}\\n\'), (4, \')\\n\')], delete: [0]}}, 22: {\'source\': {insert: [(4, '*

 * *            '\'t.add_colspan_row(\\n\'), (5, \'    [["IMDB ratings", 3]], \\n\'), (6, \'    '*

 * *            'style={"color": "green […]*

```diff
@@ -14,15 +14,15 @@
             "id": "532f5660-db16-400e-874f-77400e2f124d",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "0.1.8\n"
+                        "0.1.9\n"
                     ]
                 }
             ],
             "source": [
                 "import customized_table\n",
                 "print(customized_table.__version__)\n",
                 "from customized_table import *\n",
@@ -85,15 +85,19 @@
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "t = CustomizedTable([\"Title\", \"Year\", \"Rating\"], subheader_style={\"background\": \"#eef\"}, header_style={\"background\": \"#eef\"})\n",
+                "t = CustomizedTable(\n",
+                "    [\"Title\", \"Year\", \"Rating\"], \n",
+                "    subheader_style={\"background\": \"#eef\"}, \n",
+                "    header_style={\"background\": \"#eef\"}\n",
+                ")\n",
                 "for r in data:\n",
                 "    t.add_row(r)\n",
                 "t.add_subheader([\"Mean:\", \"\", np.mean([x[2] for x in data])])\n",
                 "t.display()"
             ]
         },
         {
@@ -390,15 +394,17 @@
                 }
             ],
             "source": [
                 "t = CustomizedTable([\"Title\", \"Year\", \"Rating\"], width=500)\n",
                 "for r in data:\n",
                 "    t.add_row(r.copy())\n",
                 "t.update_cell(0, 2, tag_text(\"<name bold>Batman</> Begins\"))\n",
-                "t.add_colspan_row([[\"IMDB ratings\", 3]], style={\"color\": \"green\", \"font\": \"bold\", \"background\": \"#7e7\", \"row-toggle-background\": 0, \"border\": \"top\", \"text-align\": \"center\", \"padding\": \"10px 15px\"})\n",
+                "t.add_colspan_row(\n",
+                "    [[\"IMDB ratings\", 3]], \n",
+                "    style={\"color\": \"green\", \"font\": \"bold\", \"background\": \"#7e7\", \"row-toggle-background\": 0, \"border\": \"top\", \"text-align\": \"center\", \"padding\": \"10px 15px\"})\n",
                 "t.display()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "2c85ab4c-e9ce-446c-8acb-34cdbd82c472",
             "metadata": {},
@@ -521,15 +527,16 @@
                 "t = CustomizedTable([\"\"], header=False)\n",
                 "t.add_row([titles], style={\"cell-format\": \"list\", \"color\": \"#272\"})\n",
                 "t.add_row([numbers], style={\"cell-format\": \"list\"})\n",
                 "t.add_row([numbers], style={\"cell-format\": \"list\", \"num-format\": \"dec-4\"})\n",
                 "t.add_row([numbers], style={\"cell-format\": \"list\", \"num-format\": \"dec-2\"})\n",
                 "t.add_row([numbers], style={\"cell-format\": \"list: \", \"num-format\": \"pct-2\"})\n",
                 "t.add_row([numbers], style={\"cell-format\": \"list:\\n\", \"num-format\": \"pct-0\", \"color\": \"blue\"})\n",
-                "t.add_row([\"This is <orange>a</> <red italic>tagged</> <bold green>text</> with\\nline break\"], style={\"cell-format\": \"tag-text\"})\n",
+                "t.add_row([\"This is <orange>a</> <red italic>tagged</> <bold green>text</> with\\nline break\"], \n",
+                "          style={\"cell-format\": \"tag-text\"})\n",
                 "t.display()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "f68aa5f2-e9a3-4604-a912-128c30538c6d",
             "metadata": {},
@@ -561,56 +568,41 @@
                     "text": [
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
-                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Courier;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Courier 12px;text-align:left;'>Genres</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Courier;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Courier 12px;text-align:left;'>No</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Courier;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Courier 12px;text-align:left;'>Part</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Courier;font-size:12px;filter:brightness(100%);font:Courier 12px;'>Drama</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Courier;font-size:12px;filter:brightness(100%);font:Courier 12px;'>12</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Courier;font-size:12px;filter:brightness(100%);font:Courier 12px;'>27.91%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Courier;font-size:12px;filter:brightness(96%);font:Courier 12px;'>Fantasy</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Courier;font-size:12px;filter:brightness(96%);font:Courier 12px;'>8</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Courier;font-size:12px;filter:brightness(96%);font:Courier 12px;'>18.60%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Courier;font-size:12px;filter:brightness(100%);font:Courier 12px;'>Thriller</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Courier;font-size:12px;filter:brightness(100%);font:Courier 12px;'>7</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Courier;font-size:12px;filter:brightness(100%);font:Courier 12px;'>16.28%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Courier;font-size:12px;filter:brightness(96%);font:Courier 12px;'>Sci-Fi</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Courier;font-size:12px;filter:brightness(96%);font:Courier 12px;'>6</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Courier;font-size:12px;filter:brightness(96%);font:Courier 12px;'>13.95%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Courier;font-size:12px;filter:brightness(100%);font:Courier 12px;'>Crime</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Courier;font-size:12px;filter:brightness(100%);font:Courier 12px;'>4</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Courier;font-size:12px;filter:brightness(100%);font:Courier 12px;'>9.30%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Courier;font-size:12px;filter:brightness(96%);font:Courier 12px;'>Action</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Courier;font-size:12px;filter:brightness(96%);font:Courier 12px;'>3</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Courier;font-size:12px;filter:brightness(96%);font:Courier 12px;'>6.98%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Courier;font-size:12px;filter:brightness(100%);font:Courier 12px;'>History</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Courier;font-size:12px;filter:brightness(100%);font:Courier 12px;'>2</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Courier;font-size:12px;filter:brightness(100%);font:Courier 12px;'>4.65%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Courier;font-size:12px;border-bottom:1px solid #aaa;filter:brightness(96%);font:Courier 12px;'>Comedy</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Courier;font-size:12px;border-bottom:1px solid #aaa;filter:brightness(96%);font:Courier 12px;'>1</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Courier;font-size:12px;border-bottom:1px solid #aaa;filter:brightness(96%);font:Courier 12px;'>2.33%</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;font-family:Courier;font-size:12px;font:Courier 12px;'>Total:</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;row-toggle-background:0;font-family:Courier;font-size:12px;font:Courier 12px;'>43</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;row-toggle-background:0;font-family:Courier;font-size:12px;font:Courier 12px;'></td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;font-family:Courier;font-size:12px;border-bottom:1px solid #aaa;font:Courier 12px;'>Mean:</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;row-toggle-background:0;num-format:dec-2;font-family:Courier;font-size:12px;border-bottom:1px solid #aaa;font:Courier 12px;'>5.38</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;row-toggle-background:0;font-family:Courier;font-size:12px;border-bottom:1px solid #aaa;font:Courier 12px;'></td></tr></table>"
-                        ],
-                        "text/plain": [
-                            "<IPython.core.display.HTML object>"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "text/html": [
-                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Arial;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Arial 12px;text-align:left;'>Genres</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Arial;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Arial 12px;text-align:left;'>No</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Arial;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Arial 12px;text-align:left;'>Part</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Arial;font-size:12px;filter:brightness(100%);font:Arial 12px;'>Drama</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Arial;font-size:12px;filter:brightness(100%);font:Arial 12px;'>12</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Arial;font-size:12px;filter:brightness(100%);font:Arial 12px;'>27.91%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Arial;font-size:12px;filter:brightness(96%);font:Arial 12px;'>Fantasy</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Arial;font-size:12px;filter:brightness(96%);font:Arial 12px;'>8</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Arial;font-size:12px;filter:brightness(96%);font:Arial 12px;'>18.60%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Arial;font-size:12px;filter:brightness(100%);font:Arial 12px;'>Thriller</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Arial;font-size:12px;filter:brightness(100%);font:Arial 12px;'>7</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Arial;font-size:12px;filter:brightness(100%);font:Arial 12px;'>16.28%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Arial;font-size:12px;filter:brightness(96%);font:Arial 12px;'>Sci-Fi</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Arial;font-size:12px;filter:brightness(96%);font:Arial 12px;'>6</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Arial;font-size:12px;filter:brightness(96%);font:Arial 12px;'>13.95%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Arial;font-size:12px;filter:brightness(100%);font:Arial 12px;'>Crime</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Arial;font-size:12px;filter:brightness(100%);font:Arial 12px;'>4</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Arial;font-size:12px;filter:brightness(100%);font:Arial 12px;'>9.30%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#811;font-family:Arial;font-size:12px;border-bottom:1px solid #aaa;filter:brightness(96%);font:Arial 12px;'>Other:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#933;font-family:Arial;font-size:12px;border-bottom:1px solid #aaa;filter:brightness(96%);font:Arial 12px;'>6</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#944;num-format:pct-2;font-family:Arial;font-size:12px;border-bottom:1px solid #aaa;filter:brightness(96%);font:Arial 12px;'>13.95%</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;font-family:Arial;font-size:12px;font:Arial 12px;'>Total:</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;row-toggle-background:0;font-family:Arial;font-size:12px;font:Arial 12px;'>43</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;row-toggle-background:0;font-family:Arial;font-size:12px;font:Arial 12px;'></td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;font-family:Arial;font-size:12px;border-bottom:1px solid #aaa;font:Arial 12px;'>Mean:</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;row-toggle-background:0;num-format:dec-2;font-family:Arial;font-size:12px;border-bottom:1px solid #aaa;font:Arial 12px;'>5.38</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;row-toggle-background:0;font-family:Arial;font-size:12px;border-bottom:1px solid #aaa;font:Arial 12px;'></td></tr></table>"
+                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Arial;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Arial 12px;text-align:left;'>Genre</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Arial;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Arial 12px;text-align:left;'>Antal</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Arial;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Arial 12px;text-align:left;'>Andel</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Arial;font-size:12px;filter:brightness(100%);font:Arial 12px;'>Drama</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Arial;font-size:12px;filter:brightness(100%);font:Arial 12px;'>12</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Arial;font-size:12px;filter:brightness(100%);font:Arial 12px;'>27.91%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Arial;font-size:12px;filter:brightness(96%);font:Arial 12px;'>Fantasy</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Arial;font-size:12px;filter:brightness(96%);font:Arial 12px;'>8</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Arial;font-size:12px;filter:brightness(96%);font:Arial 12px;'>18.60%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Arial;font-size:12px;filter:brightness(100%);font:Arial 12px;'>Thriller</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Arial;font-size:12px;filter:brightness(100%);font:Arial 12px;'>7</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Arial;font-size:12px;filter:brightness(100%);font:Arial 12px;'>16.28%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Arial;font-size:12px;filter:brightness(96%);font:Arial 12px;'>Sci-Fi</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Arial;font-size:12px;filter:brightness(96%);font:Arial 12px;'>6</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Arial;font-size:12px;filter:brightness(96%);font:Arial 12px;'>13.95%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Arial;font-size:12px;filter:brightness(100%);font:Arial 12px;'>Crime</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Arial;font-size:12px;filter:brightness(100%);font:Arial 12px;'>4</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Arial;font-size:12px;filter:brightness(100%);font:Arial 12px;'>9.30%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#811;font-family:Arial;font-size:12px;border-bottom:1px solid #aaa;filter:brightness(96%);font:Arial 12px;'>Other:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#933;font-family:Arial;font-size:12px;border-bottom:1px solid #aaa;filter:brightness(96%);font:Arial 12px;'>6</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#944;num-format:pct-2;font-family:Arial;font-size:12px;border-bottom:1px solid #aaa;filter:brightness(96%);font:Arial 12px;'>13.95%</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;font-family:Arial;font-size:12px;font:Arial 12px;'>Total:</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;row-toggle-background:0;font-family:Arial;font-size:12px;font:Arial 12px;'>43</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;row-toggle-background:0;font-family:Arial;font-size:12px;font:Arial 12px;'></td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;font-family:Arial;font-size:12px;border-bottom:1px solid #aaa;font:Arial 12px;'>Medel:</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;row-toggle-background:0;num-format:dec-2;font-family:Arial;font-size:12px;border-bottom:1px solid #aaa;font:Arial 12px;'>5.38</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;row-toggle-background:0;font-family:Arial;font-size:12px;border-bottom:1px solid #aaa;font:Arial 12px;'></td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "t = generate_counts(genres, sort=\"key\")\n",
                 "t.display()\n",
-                "\n",
                 "print()\n",
-                "\n",
                 "gnrs = {\"Action\": 3, \"Drama\": 12, \"Thriller\": 7, \"Crime\": 4, \"Fantasy\": 8, \"Comedy\": 1, \"Sci-Fi\": 6, \"History\": 2}\n",
-                "t = generate_counts(gnrs, title=\"Genres\", sort=\"desc\", footer=[\"total\",\"mean\"])\n",
-                "t.display()\n",
-                "\n",
-                "print()\n",
-                "\n",
-                "t = generate_counts(gnrs, title=\"Genres\", sort=\"desc\", footer=[\"total\",\"mean\"], group=5, style={\"font\": \"Arial 12px\"})\n",
+                "t = generate_counts(gnrs, \n",
+                "                    labels={\n",
+                "                        \"title\": \"Genre\",\n",
+                "                        \"no\": \"Antal\",\n",
+                "                        \"part\": \"Andel\",\n",
+                "                        \"mean\": \"Medel:\",\n",
+                "                    }, \n",
+                "                    sort=\"desc\", \n",
+                "                    footer=[\"total\",\"mean\"],\n",
+                "                    group=5,\n",
+                "                    style={\"font\": \"Arial 12px\"}\n",
+                "                   )\n",
                 "t.display()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "7e3ca1c1-7f8c-4455-b5b5-5f03303c0eca",
             "metadata": {},
@@ -653,15 +645,17 @@
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "t = CustomizedTable([\"Title\", \"Year\", \"Rating\"], subheader_style={\"background\": \"#eef\"}, header_style={\"background\": \"#eef\"})\n",
+                "t = CustomizedTable([\"Title\", \"Year\", \"Rating\"], \n",
+                "                    subheader_style={\"background\": \"#eef\"}, \n",
+                "                    header_style={\"background\": \"#eef\"})\n",
                 "for r in data:\n",
                 "    t.add_row(r)\n",
                 "# If value in column 2 >= 9 then set style to column 0\n",
                 "t.style_rule(2,\">=\",9,{\"color\": \"green\"},0)\n",
                 "# If value in column 2 < 8 then set style to column 0\n",
                 "t.style_rule(2,\"<\",8,{\"color\": \"red\"},0)\n",
                 "# If value in column 0 equals 'Batman Begins' then set style to whole row\n",
```

### Comparing `customized_table-0.1.8/LICENSE` & `customized_table-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `customized_table-0.1.8/PKG-INFO` & `customized_table-0.1.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: customized_table
-Version: 0.1.8
+Version: 0.1.9
 Summary: Creates flexible tables in Jupyter Notebooks with lots of formatting options
 Home-page: https://github.com/jhagelback/customized_table
 Author: Johan Hagelbäck
 Author-email: johan.hagelback@gmail.com
 License: MIT
 Platform: UNKNOWN
 License-File: LICENSE
```

### Comparing `customized_table-0.1.8/README.md` & `customized_table-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `customized_table-0.1.8/customized_table/customized_table.py` & `customized_table-0.1.9/customized_table/customized_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -861,15 +861,15 @@
         print(colored("Error: ", "red", attrs=["bold"]) + "unable to create table from csv file")
         return CustomizedTable([""])
 
 
 #
 # Generates a counts table from a list or dict.
 #
-def generate_counts(data, cidx=0, title="", sort=None, footer=["total"], group=None, style=None):
+def generate_counts(data, cidx=0, labels=None, sort=None, footer=["total"], group=None, style=None):
     if type(data) not in [dict, list]:
         print(colored("Warning", "red", attrs=["bold"]) + ": data must dict or list")
         return
     
     # Convert from list to dict
     if type(data) == list:
         cnt = {}
@@ -880,25 +880,32 @@
             if v not in cnt:
                 cnt.update({v: 0})
             cnt[v] += 1
     if type(data) == dict:
         cnt = data
     
     # Generate table from dict
+    title = ""
+    if labels is not None and "title" in labels:
+        title = labels["title"]
+    cnlbl = "No"
+    if labels is not None and "no" in labels:
+        cnlbl = labels["no"]
+    cplbl = "Part"
+    if labels is not None and "part" in labels:
+        cplbl = labels["part"]
+        
     if style is None:
-        t = CustomizedTable([title, "No", "Part"])
+        t = CustomizedTable([title, cnlbl, cplbl])
     else:
-        t = CustomizedTable([title, "No", "Part"], style=style)
+        t = CustomizedTable([title, cnlbl, cplbl], style=style)
     t.column_style(1, {"color": "value"})
     t.column_style(2, {"color": "percent", "num-format": "pct-2"})
     tot = sum(list(cnt.values()))
     for key,n in cnt.items():
-        #if group is not None and t.no_rows() >= group:
-        #    ngrp += 1
-        #else:
         t.add_row([key,n,n/tot])
     
     # Sort table
     if sort in ["key", 0]:
         t.sort(0)
     if sort in ["asc", "ascending", 1]:
         t.sort(1)
@@ -909,25 +916,34 @@
     ngrp = 0
     if group is not None:
         ngrp = sum([x[1] for x in t.rows[group:]])
         t.rows = t.rows[:group]
     
     # Grouped row
     if ngrp > 0:
-        t.add_row(["Other:",ngrp,ngrp/tot])
+        olbl = "Other:"
+        if labels is not None and "other" in labels:
+            olbl = labels["other"]
+        t.add_row([olbl,ngrp,ngrp/tot])
         t.cell_style(0,-1,{"color": "#811"})
         t.cell_style(1,-1,{"color": "#933"})
         t.cell_style(2,-1,{"color": "#944"})
 
     # Bottom border
     t.row_style(-1, {"border": "bottom"})
     
     # Add total and/or mean row
     if footer is not None:
         if "total" in footer:
-            t.add_row(["Total:", tot, ""], style={"background": "#eee", "row-toggle-background": 0})
+            tlbl = "Total:"
+            if labels is not None and "total" in labels:
+                tlbl = labels["total"]
+            t.add_row([tlbl, tot, ""], style={"background": "#eee", "row-toggle-background": 0})
         if "mean" in footer:
-            t.add_row(["Mean:", tot/len(cnt), ""], style={"background": "#eee", "row-toggle-background": 0})
+            mlbl = "Mean:"
+            if labels is not None and "mean" in labels:
+                mlbl = labels["mean"]
+            t.add_row([mlbl, tot/len(cnt), ""], style={"background": "#eee", "row-toggle-background": 0})
             t.cell_style(1,-1,{"num-format": "dec-2"})
     
     return t
```

### Comparing `customized_table-0.1.8/customized_table/docs.py` & `customized_table-0.1.9/customized_table/docs.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,15 @@
                         ]])
     t.cell_style(1, -1, {"cell-format": "list:\n"})
     
     t.add_row(["generate_counts", [tag_text("Generates a counts table (number of occurences for each item) from a list or dict."),
                         "Params:", 
                         tag_text("&nbsp;<#a44 italic>data</> Data to generate counts from. <#888>(list or dict)</>"),
                         tag_text("&nbsp;<#a44 italic>cidx</> Column to generate counts from, if data is list of lists. <#888>(column index, optional)</>"),
-                        tag_text("&nbsp;<#a44 italic>title</> Title of the table. <#888>(string, optional)</>"),
+                        tag_text("&nbsp;<#a44 italic>labels</> Set labels for the counts table (title,no,part,total,mean). <#888>(dict, optional)</>"),
                         tag_text("&nbsp;<#a44 italic>sort</> How to sort the counts table. <#888>(None for no sorting, or 'key', 'asc', 'desc')</>"),
                         tag_text("&nbsp;<#a44 italic>footer</> What to show in the footer. <#888>(list ('total','mean') or None)</>"),
                         tag_text("&nbsp;<#a44 italic>group</> Group all entries after the specified row to make the table more compact. <#888>(row index, optional)</>"),
                         tag_text("&nbsp;<#a44 italic>style</> Changes default formatting. <#888>(dict, optional)</>"),
                         
                         ]])
     t.cell_style(1, -1, {"cell-format": "list:\n"})
```

### Comparing `customized_table-0.1.8/customized_table.egg-info/PKG-INFO` & `customized_table-0.1.9/customized_table.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: customized-table
-Version: 0.1.8
+Version: 0.1.9
 Summary: Creates flexible tables in Jupyter Notebooks with lots of formatting options
 Home-page: https://github.com/jhagelback/customized_table
 Author: Johan Hagelbäck
 Author-email: johan.hagelback@gmail.com
 License: MIT
 Platform: UNKNOWN
 License-File: LICENSE
```

### Comparing `customized_table-0.1.8/setup.py` & `customized_table-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 setup(name="customized_table",
-    version="0.1.8",
+    version="0.1.9",
     author="Johan Hagelbäck",
     author_email="johan.hagelback@gmail.com",
     description="Creates flexible tables in Jupyter Notebooks with lots of formatting options",
     long_description="Creates flexible tables in Jupyter Notebooks with lots of formatting options such as changing font, font color, cell background, number formatting and much more. Tables can also be saved to csv or Excel files, or generated from csv data files.",
     license="MIT",
     packages=["customized_table"],
     url="https://github.com/jhagelback/customized_table",
```

