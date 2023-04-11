# Comparing `tmp/chat_research-0.1.8.tar.gz` & `tmp/chat_research-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat_research-0.1.8.tar", max compression
+gzip compressed data, was "chat_research-0.1.9.tar", max compression
```

## Comparing `chat_research-0.1.8.tar` & `chat_research-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0     1067 2023-04-05 17:01:07.146466 chat_research-0.1.8/LICENSE
--rw-r--r--   0        0        0     4849 2023-04-05 17:01:07.146466 chat_research-0.1.8/README.md
--rw-r--r--   0        0        0     1429 2023-04-05 17:01:24.190704 chat_research-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      221 2023-04-05 17:01:07.150466 chat_research-0.1.8/src/chat_research/__init__.py
--rw-r--r--   0        0        0     3485 2023-04-05 17:01:07.150466 chat_research-0.1.8/src/chat_research/__main__.py
--rw-r--r--   0        0        0     1936 2023-04-05 17:01:07.150466 chat_research-0.1.8/src/chat_research/aexport.py
--rw-r--r--   0        0        0     6407 2023-04-05 17:01:07.150466 chat_research-0.1.8/src/chat_research/app.py
--rw-r--r--   0        0        0    18737 2023-04-05 17:01:07.150466 chat_research-0.1.8/src/chat_research/areader.py
--rw-r--r--   0        0        0    24489 2023-04-05 17:01:07.150466 chat_research-0.1.8/src/chat_research/commands/chat_arxiv.py
--rw-r--r--   0        0        0    24663 2023-04-05 17:01:07.150466 chat_research-0.1.8/src/chat_research/commands/chat_async_arxiv.py
--rw-r--r--   0        0        0     9062 2023-04-05 17:01:07.150466 chat_research-0.1.8/src/chat_research/commands/chat_async_biorxiv.py
--rw-r--r--   0        0        0     9346 2023-04-05 17:01:07.150466 chat_research-0.1.8/src/chat_research/commands/chat_async_paper.py
--rw-r--r--   0        0        0     2160 2023-04-05 17:01:07.150466 chat_research-0.1.8/src/chat_research/commands/chat_config.py
--rw-r--r--   0        0        0     5459 2023-04-05 17:01:07.150466 chat_research-0.1.8/src/chat_research/commands/chat_response.py
--rw-r--r--   0        0        0    11627 2023-04-05 17:01:07.154466 chat_research-0.1.8/src/chat_research/commands/chat_reviewer.py
--rw-r--r--   0        0        0     1900 2023-04-05 17:01:07.154466 chat_research-0.1.8/src/chat_research/export.py
--rw-r--r--   0        0        0    10143 2023-04-05 17:01:07.154466 chat_research-0.1.8/src/chat_research/paper.py
--rw-r--r--   0        0        0    14333 2023-04-05 17:01:07.154466 chat_research-0.1.8/src/chat_research/paper_with_image.py
--rw-r--r--   0        0        0    26432 2023-04-05 17:01:07.154466 chat_research-0.1.8/src/chat_research/provider/arxiv.py
--rw-r--r--   0        0        0    26506 2023-04-05 17:01:07.154466 chat_research-0.1.8/src/chat_research/provider/async_arxiv.py
--rw-r--r--   0        0        0    18669 2023-04-05 17:01:07.154466 chat_research-0.1.8/src/chat_research/provider/async_biorxiv.py
--rw-r--r--   0        0        0    18657 2023-04-05 17:01:07.154466 chat_research-0.1.8/src/chat_research/reader.py
--rw-r--r--   0        0        0        0 2023-04-05 17:01:07.154466 chat_research-0.1.8/src/chat_research/summary.py
--rw-r--r--   0        0        0     1314 2023-04-05 17:01:07.154466 chat_research-0.1.8/src/chat_research/utils.py
--rw-r--r--   0        0        0     6440 1970-01-01 00:00:00.000000 chat_research-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-05 21:01:16.991423 chat_research-0.1.9/LICENSE
+-rw-r--r--   0        0        0     4959 2023-04-05 21:01:16.991423 chat_research-0.1.9/README.md
+-rw-r--r--   0        0        0     1429 2023-04-05 21:01:31.875817 chat_research-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      199 2023-04-05 21:01:17.051425 chat_research-0.1.9/src/chat_research/__init__.py
+-rw-r--r--   0        0        0     3485 2023-04-05 21:01:17.051425 chat_research-0.1.9/src/chat_research/__main__.py
+-rw-r--r--   0        0        0     3526 2023-04-05 21:01:17.051425 chat_research-0.1.9/src/chat_research/aexport.py
+-rw-r--r--   0        0        0     6407 2023-04-05 21:01:17.051425 chat_research-0.1.9/src/chat_research/app.py
+-rw-r--r--   0        0        0    18994 2023-04-05 21:01:17.051425 chat_research-0.1.9/src/chat_research/areader.py
+-rw-r--r--   0        0        0    24489 2023-04-05 21:01:17.051425 chat_research-0.1.9/src/chat_research/commands/chat_arxiv.py
+-rw-r--r--   0        0        0    24663 2023-04-05 21:01:17.051425 chat_research-0.1.9/src/chat_research/commands/chat_async_arxiv.py
+-rw-r--r--   0        0        0     9179 2023-04-05 21:01:17.051425 chat_research-0.1.9/src/chat_research/commands/chat_async_biorxiv.py
+-rw-r--r--   0        0        0     9273 2023-04-05 21:01:17.051425 chat_research-0.1.9/src/chat_research/commands/chat_async_paper.py
+-rw-r--r--   0        0        0     2160 2023-04-05 21:01:17.051425 chat_research-0.1.9/src/chat_research/commands/chat_config.py
+-rw-r--r--   0        0        0     5459 2023-04-05 21:01:17.051425 chat_research-0.1.9/src/chat_research/commands/chat_response.py
+-rw-r--r--   0        0        0    11627 2023-04-05 21:01:17.051425 chat_research-0.1.9/src/chat_research/commands/chat_reviewer.py
+-rw-r--r--   0        0        0     1900 2023-04-05 21:01:17.051425 chat_research-0.1.9/src/chat_research/export.py
+-rw-r--r--   0        0        0    10143 2023-04-05 21:01:17.051425 chat_research-0.1.9/src/chat_research/paper.py
+-rw-r--r--   0        0        0    14486 2023-04-05 21:01:17.051425 chat_research-0.1.9/src/chat_research/paper_with_image.py
+-rw-r--r--   0        0        0    26432 2023-04-05 21:01:17.051425 chat_research-0.1.9/src/chat_research/provider/arxiv.py
+-rw-r--r--   0        0        0    26504 2023-04-05 21:01:17.051425 chat_research-0.1.9/src/chat_research/provider/async_arxiv.py
+-rw-r--r--   0        0        0    18657 2023-04-05 21:01:17.051425 chat_research-0.1.9/src/chat_research/provider/async_biorxiv.py
+-rw-r--r--   0        0        0    18657 2023-04-05 21:01:17.051425 chat_research-0.1.9/src/chat_research/reader.py
+-rw-r--r--   0        0        0        0 2023-04-05 21:01:17.051425 chat_research-0.1.9/src/chat_research/summary.py
+-rw-r--r--   0        0        0      390 2023-04-05 21:01:17.051425 chat_research-0.1.9/src/chat_research/template/__init__.py
+-rw-r--r--   0        0        0    30474 2023-04-05 21:01:17.051425 chat_research-0.1.9/src/chat_research/template/eisvogel.tex
+-rw-r--r--   0        0        0     1314 2023-04-05 21:01:17.051425 chat_research-0.1.9/src/chat_research/utils.py
+-rw-r--r--   0        0        0     6550 1970-01-01 00:00:00.000000 chat_research-0.1.9/PKG-INFO
```

### Comparing `chat_research-0.1.8/LICENSE` & `chat_research-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chat_research-0.1.8/README.md` & `chat_research-0.1.9/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -25,46 +25,45 @@
 I welcome any suggestions, proposals, and pull requests.
 
 ## TODO
 
 - [x] Multi thread and Asynchronous support
 - [x] Add GIF for document
 - [x] Use config to set key
-- [ ] Format PDF output
-- [ ] Tune prompt to support latex
-- [ ] Support output latex
+- [x] Support output for Latex and PDF
 - [ ] Fine-tune prompt
 - [ ] Generate Image
 - [ ] Add RSS support for multiple journal
 - [ ] Revise help message
+- [ ] add classic paper as examples
 
 ## Features
 
 - [Chat Config](#chat-config): Generate `chatre.toml` in current working directory or set environment variable `OPENAI_API_KEY`.
 - [Chat Paper](#chat-paper): Fetch or summary paper from local or arxiv with specified query, research fields, and language.
 - [Chat Biorxiv](#chat-biorxiv): Fetch and summary paper from bioarxiv with specified category, filter keys, and language.
 - [Chat Reviewer](#chat-reviewer): Generate summary paper with specified research fields and language.
 - [Chat Response](#chat-response): Generate response for review comment with specified language.
-- [Markdown](https://github.com/cauliyang/ChatResearch/blob/main/images/example2.md) and [PDF report](https://github.com/cauliyang/ChatResearch/blob/main/images/example1.pdf)
+- [Markdown](https://github.com/cauliyang/ChatResearch/blob/main/docs/images/example2.md), [PDF](https://github.com/cauliyang/ChatResearch/blob/main/docs/images/example1.pdf), and [Latex](https://github.com/cauliyang/ChatResearch/blob/main/docs/images/example5.tex)
 
-<img src="https://github.com/cauliyang/ChatResearch/blob/main//tutorial/project.gif" width="800" height="400">
+<img src="https://github.com/cauliyang/ChatResearch/blob/main//docs/tutorial/project.gif" width="800" height="400">
 
 ## Installation
 
 ```console
 $pip install chat-research
 ```
 
 ## Usage
 
-<img src="https://github.com/cauliyang/ChatResearch/blob/main//tutorial/help.gif" width="800" height="400">
+<img src="https://github.com/cauliyang/ChatResearch/blob/main//docs/tutorial/help.gif" width="800" height="400">
 
 ### Chat Config
 
-<img src="https://github.com/cauliyang/ChatResearch/blob/main//tutorial/config.gif" width="800" height="400">
+<img src="https://github.com/cauliyang/ChatResearch/blob/main//docs/tutorial/config.gif" width="800" height="400">
 
 ```console
 ❯ chatre config
 ```
 
 It will generate `chatre.toml` in current working directory. Otherwise,
 setting environment variable `OPENAI_API_KEY` is another way to config API KEY.
@@ -80,23 +79,23 @@
 owner = "your_gitee_name"
 repo = "your_repo_name"
 path = "files_name_in_your_repo"
 ```
 
 ### Chat Paper
 
-<img src="https://github.com/cauliyang/ChatResearch/blob/main//tutorial/paper.gif" width="800" height="400">
+<img src="https://github.com/cauliyang/ChatResearch/blob/main//docs/tutorial/paper.gif" width="800" height="400">
 
 ### Chat Biorxiv
 
-<img src="https://github.com/cauliyang/ChatResearch/blob/main//tutorial/biorxiv.gif" width="800" height="400">
+<img src="https://github.com/cauliyang/ChatResearch/blob/main//docs/tutorial/biorxiv.gif" width="800" height="400">
 
 ### Chat Response
 
-<img src="https://github.com/cauliyang/ChatResearch/blob/main//tutorial/response.gif" width="800" height="400">
+<img src="https://github.com/cauliyang/ChatResearch/blob/main//docs/tutorial/response.gif" width="800" height="400">
 
 ### Chat Reviewer
 
 ```console
 > chatre reviewer -h
 usage: chatre reviewer [-h] --paper-path  [--file-format] [--review-format] [--research-fields] [--language]
```

### Comparing `chat_research-0.1.8/pyproject.toml` & `chat_research-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chat-research"
-version = "0.1.8"
+version = "0.1.9"
 description = "Use ChatGPT to accelerator your research."
 authors = ["Yangyang Li <yangyang.li@northwestern.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/cauliyang/ChatResearch"
 repository = "https://github.com/cauliyang/ChatResearch"
 documentation = "https://github.com/cauliyang/ChatResearch"
```

### Comparing `chat_research-0.1.8/src/chat_research/__main__.py` & `chat_research-0.1.9/src/chat_research/__main__.py`

 * *Files identical despite different names*

### Comparing `chat_research-0.1.8/src/chat_research/app.py` & `chat_research-0.1.9/src/chat_research/app.py`

 * *Files identical despite different names*

### Comparing `chat_research-0.1.8/src/chat_research/areader.py` & `chat_research-0.1.9/src/chat_research/areader.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,19 @@
                 for index, paper in enumerate(paper_list)
             ]
         )
 
     def summary_with_chat(self, paper_list: list[Paper], key_words):
         asyncio.run(self._summary_with_chat(paper_list, key_words))
 
+    def find_title(self, text):
+        for line in text.split("\n"):
+            if "Title:" in line:
+                return line.split("Title:")[1].strip()
+
     async def summary_with_chat_for_one_paper(
         self, paper: Paper, paper_index: int, key_words
     ):
         htmls = []
         # 第一步先用title，abs，和introduction进行总结。
         text = ""
         text += "Title:" + paper.title
@@ -75,14 +80,17 @@
                     text=text,
                     key_words=key_words,
                     summary_prompt_token=summary_prompt_token,
                 )
             else:
                 raise e
 
+        if (title := self.find_title(chat_summary_text)) is not None:
+            paper.title = title
+
         htmls.append("## Paper:" + str(paper_index + 1))
         htmls.append("\n\n\n")
         htmls.append(chat_summary_text)
 
         # 第二步总结方法：
         # WARNING，由于有些文章的方法章节名是算法名，
         # 所以简单的通过关键词来筛选，很难获取，后面需要用其他的方案去优化。
@@ -403,15 +411,15 @@
         # 将论文的乱七八糟的路径格式修正
         rstr = r"[\/\\\:\*\?\"\<\>\|]"  # '/ \ : * ? " < > |'
         new_title = re.sub(rstr, "_", title)  # 替换为下划线
         return new_title
 
     def show_token_usage(self):
         money = self.token_usage / 1000 * 0.002
-        logger.info(f"total_token_used: {self.token_usage} ({money:.4f} USD)")
+        logger.info(f"TOKENS: {self.token_usage} / PRICES: ${money:.6f}")
 
     def report_token_usage(self, response):
         logger.trace(f"prompt_token_used: {response.usage.prompt_tokens}")
         logger.trace(f"completion_token_used: {response.usage.completion_tokens}")
         logger.trace(f"total_token_used: {response.usage.total_tokens}")
         logger.trace(f"response_time: { response.response_ms / 1000.0}s")
         self.token_usage += response.usage.total_tokens
```

### Comparing `chat_research-0.1.8/src/chat_research/commands/chat_arxiv.py` & `chat_research-0.1.9/src/chat_research/commands/chat_arxiv.py`

 * *Files identical despite different names*

### Comparing `chat_research-0.1.8/src/chat_research/commands/chat_async_arxiv.py` & `chat_research-0.1.9/src/chat_research/commands/chat_async_arxiv.py`

 * *Files identical despite different names*

### Comparing `chat_research-0.1.8/src/chat_research/commands/chat_async_biorxiv.py` & `chat_research-0.1.9/src/chat_research/commands/chat_async_biorxiv.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,17 +73,19 @@
                 max_results=max_results,
             )
 
     def filter_arxiv(self, max_results=30) -> list[biorxiv.Result]:
         search = self.get_biorxiv(max_results=max_results)
         results = list(search.results())
 
-        logger.info("all search:")
+        logger.info("All search:")
         for index, result in enumerate(results):
-            logger.info(f"{index=}, {result.title=}, {result.date}")
+            logger.info(
+                f"{index=}, title={result.title} {result.date.strftime('%Y-%m-%d')}"
+            )
 
         # if self.filter_keys is empty then do not filter out
         if not self.filter_keys:
             return results
 
         filter_results = []
 
@@ -99,15 +101,17 @@
 
             if meet_num == len(self.filter_keys):
                 filter_results.append(result)
 
         logger.info(f"filter_results: {len(filter_results)}")
         logger.info("filter_papers:")
         for index, result in enumerate(filter_results):
-            logger.info(f"{index=}, {result.title=}, {result.date}")
+            logger.info(
+                f"{index=}, title={result.title} {result.date.strftime('%Y-%m-%d')}"
+            )
 
         return filter_results
 
     def download_pdf(self, filter_results):
         return asyncio.run(self._download_pdf(filter_results))
 
     @staticmethod
@@ -265,15 +269,15 @@
         help="save image? It takes a minute or two to save a picture! But pretty (default: %(default)s)",
     )
 
     subparser.add_argument(
         "--file-format",
         type=str,
         default="md",
-        choices=["md", "txt", "pdf"],
+        choices=["md", "txt", "pdf", "tex"],
         metavar="",
         help="the format of the exported file, if you save the picture, it is best to be md, if not, the txt will not be messy (default: %(default)s)",
     )
 
     subparser.add_argument(
         "--language",
         type=str,
```

### Comparing `chat_research-0.1.8/src/chat_research/commands/chat_async_paper.py` & `chat_research-0.1.9/src/chat_research/commands/chat_async_paper.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 
 from ..areader import AsyncBaseReader
 from ..paper_with_image import Paper
 from ..provider import async_arxiv as arxiv
 
 
 class PaperParams(BaseModel):
-    pdf_path: str
+    pdf: str
     query: str
     key_word: str
     filter_keys: Optional[list[str]] = None
     max_results: int
     sort: str
     save_image: bool
     file_format: str
     language: str
 
-    @validator("pdf_path")
+    @validator("pdf")
     def pdf_path_must_exist(cls, v):
         if not Path(v).exists():
             raise ValueError("pdf_path must exist")
         return v
 
 
 # 定义Reader类
@@ -76,17 +76,19 @@
         )
         return search
 
     def filter_arxiv(self, max_results=30):
         search = self.get_arxiv(max_results=max_results)
         results = list(search.results())
 
-        logger.info("all search:")
+        logger.info("All search:")
         for index, result in enumerate(results):
-            logger.info(f"{index=}, {result.title=}, {result.updated}")
+            logger.info(
+                f"{index=}, title={result.title} {result.updated.strftime('%Y-%m-%d')}"
+            )
 
         # if self.filter_keys is empty then do not filter out
         if not self.filter_keys:
             return results
 
         filter_results = []
 
@@ -100,15 +102,18 @@
                     meet_num += 1
             if meet_num == len(self.filter_keys):
                 filter_results.append(result)
 
         logger.info(f"filter_results: {len(filter_results)}")
         logger.info("filter_papers:")
         for index, result in enumerate(filter_results):
-            logger.info(f"{index=}, {result.title=}, {result.updated}")
+            logger.info(
+                f"{index=}, title={result.title} {result.updated.strftime('%Y-%m-%d')}"
+            )
+
         return filter_results
 
     def download_pdf(self, filter_results):
         return asyncio.run(self._download_pdf(filter_results))
 
     @staticmethod
     def create_paper(results_mapping, paper_path):
@@ -165,15 +170,15 @@
 
 def add_subcommand(parser):
     name = "paper"
     subparser = parser.add_parser(
         name, help="Fetch or Summary paper from local or arxiv"
     )
     subparser.add_argument(
-        "--pdf-path",
+        "--pdf",
         type=str,
         default="",
         metavar="",
         help="if none, the bot will download from arxiv with query",
     )
 
     subparser.add_argument(
@@ -224,15 +229,15 @@
         help="save image? It takes a minute or two to save a picture! But pretty (default: %(default)s)",
     )
 
     subparser.add_argument(
         "--file-format",
         type=str,
         default="md",
-        choices=["md", "txt", "pdf"],
+        choices=["md", "txt", "pdf", "tex"],
         metavar="",
         help="the format of the exported file, if you save the picture, it is best to be md, if not, the txt will not be messy (default: %(default)s)",
     )
 
     subparser.add_argument(
         "--language",
         type=str,
@@ -249,42 +254,39 @@
     if args.sort == "Relevance":
         sort = arxiv.SortCriterion.Relevance
     elif args.sort == "LastUpdatedDate":
         sort = arxiv.SortCriterion.LastUpdatedDate
     else:
         sort = arxiv.SortCriterion.Relevance
 
-    if args.pdf_path:
+    if args.pdf:
         reader = Reader(
             key_word=args.key_word,
             query=args.query,
             filter_keys=args.filter_keys,
             sort=sort,
             args=args,
         )
         reader.show_info()
-        # 开始判断是路径还是文件：
         paper_list = []
-        if args.pdf_path.endswith(".pdf"):
-            paper_list.append(Paper(path=args.pdf_path))
-            logger.info(f"read pdf file {args.pdf_path}")
+        if args.pdf.endswith(".pdf"):
+            paper_list.append(Paper(path=args.pdf))
+            logger.info(f"read pdf file {args.pdf}")
         else:
-            logger.info(f"read pdf files from path {args.pdf_path}")
-            for root, dirs, files in os.walk(args.pdf_path):
+            logger.info(f"read pdf files from path {args.pdf}")
+            for root, dirs, files in os.walk(args.pdf):
                 logger.trace(f"root: {root}, dirs: {dirs}, files: {files}")
                 for filename in files:
-                    # 如果找到PDF文件，则将其复制到目标文件夹中
                     if filename.endswith(".pdf"):
                         paper_list.append(Paper(path=os.path.join(root, filename)))
 
         logger.info("paper_num: {}".format(len(paper_list)))
-        for paper_index, paper_name in enumerate(paper_list):
-            name = paper_name.path.split("\\")[-1]
+        for paper_index, paper in enumerate(paper_list):
+            name = Path(paper.path).name
             logger.info(f"{paper_index=}, {name=}")
-
         reader.summary_with_chat(paper_list=paper_list, key_words=reader.key_word)
     else:
         reader = Reader(
             key_word=args.key_word,
             query=args.query,
             filter_keys=args.filter_keys,
             sort=sort,
```

### Comparing `chat_research-0.1.8/src/chat_research/commands/chat_config.py` & `chat_research-0.1.9/src/chat_research/commands/chat_config.py`

 * *Files identical despite different names*

### Comparing `chat_research-0.1.8/src/chat_research/commands/chat_response.py` & `chat_research-0.1.9/src/chat_research/commands/chat_response.py`

 * *Files identical despite different names*

### Comparing `chat_research-0.1.8/src/chat_research/commands/chat_reviewer.py` & `chat_research-0.1.9/src/chat_research/commands/chat_reviewer.py`

 * *Files identical despite different names*

### Comparing `chat_research-0.1.8/src/chat_research/export.py` & `chat_research-0.1.9/src/chat_research/export.py`

 * *Files identical despite different names*

### Comparing `chat_research-0.1.8/src/chat_research/paper.py` & `chat_research-0.1.9/src/chat_research/paper.py`

 * *Files identical despite different names*

### Comparing `chat_research-0.1.8/src/chat_research/paper_with_image.py` & `chat_research-0.1.9/src/chat_research/paper_with_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,19 @@
             "IIX",
             "IX",
             "X",
         ]
         self.digit_num = [str(d + 1) for d in range(10)]
         self.first_image = ""
 
+    def __repr__(self):
+        return f"""Papers(title={self.title}, url={self.url}, authers={self.authers} abs={self.abs})"""
+
+    __str__ = __repr__
+
     def parse_pdf(self):
         self.pdf = fitz.open(self.path)  # pdf文档
         self.text_list = [page.get_text() for page in self.pdf]
         self.all_text = " ".join(self.text_list)
         self.section_page_dict = self._get_all_page_index()  # 段落与页码的对应字典
         logger.trace(f"section_page_dict {self.section_page_dict}")
         self.section_text_dict = self._get_all_page()  # 段落与内容的对应字典
```

### Comparing `chat_research-0.1.8/src/chat_research/provider/arxiv.py` & `chat_research-0.1.9/src/chat_research/provider/arxiv.py`

 * *Files identical despite different names*

### Comparing `chat_research-0.1.8/src/chat_research/provider/async_arxiv.py` & `chat_research-0.1.9/src/chat_research/provider/async_arxiv.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,15 @@
         if not filename:
             filename = self._get_default_filename()
 
         if isinstance(dirpath, str):
             dirpath = Path(dirpath)
 
         path = dirpath / filename
-        logger.info(f"Downloading PDF to {path}")
+        logger.info(f"Downloading: {filename}")
 
         async with session.get(
             self.pdf_url, headers=self.headers, raise_for_status=True
         ) as response:
             async with aiofiles.open(path, "wb") as f:
                 async for chunk in response.content.iter_chunked(1024):
                     await asyncio.sleep(0.001)
```

### Comparing `chat_research-0.1.8/src/chat_research/provider/async_biorxiv.py` & `chat_research-0.1.9/src/chat_research/provider/async_biorxiv.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,15 +274,15 @@
 
         if not filename:
             filename = self._get_default_filename()
 
         path = dirpath / filename
 
         self.pdf_url = await self.get_pdf_url(session)
-        logger.info(f"Downloading PDF from {self.pdf_url}")
+        logger.info(f"Downloading: {filename}")
         async with session.get(
             self.pdf_url, headers=self.headers, raise_for_status=True
         ) as response:
             async with aiofiles.open(path, "wb") as f:
                 async for chunk in response.content.iter_chunked(1024):
                     await asyncio.sleep(0.001)
                     await f.write(chunk)
```

### Comparing `chat_research-0.1.8/src/chat_research/reader.py` & `chat_research-0.1.9/src/chat_research/reader.py`

 * *Files identical despite different names*

### Comparing `chat_research-0.1.8/src/chat_research/utils.py` & `chat_research-0.1.9/src/chat_research/utils.py`

 * *Files identical despite different names*

### Comparing `chat_research-0.1.8/PKG-INFO` & `chat_research-0.1.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-research
-Version: 0.1.8
+Version: 0.1.9
 Summary: Use ChatGPT to accelerator your research.
 Home-page: https://github.com/cauliyang/ChatResearch
 License: MIT
 Author: Yangyang Li
 Author-email: yangyang.li@northwestern.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -64,46 +64,45 @@
 I welcome any suggestions, proposals, and pull requests.
 
 ## TODO
 
 - [x] Multi thread and Asynchronous support
 - [x] Add GIF for document
 - [x] Use config to set key
-- [ ] Format PDF output
-- [ ] Tune prompt to support latex
-- [ ] Support output latex
+- [x] Support output for Latex and PDF
 - [ ] Fine-tune prompt
 - [ ] Generate Image
 - [ ] Add RSS support for multiple journal
 - [ ] Revise help message
+- [ ] add classic paper as examples
 
 ## Features
 
 - [Chat Config](#chat-config): Generate `chatre.toml` in current working directory or set environment variable `OPENAI_API_KEY`.
 - [Chat Paper](#chat-paper): Fetch or summary paper from local or arxiv with specified query, research fields, and language.
 - [Chat Biorxiv](#chat-biorxiv): Fetch and summary paper from bioarxiv with specified category, filter keys, and language.
 - [Chat Reviewer](#chat-reviewer): Generate summary paper with specified research fields and language.
 - [Chat Response](#chat-response): Generate response for review comment with specified language.
-- [Markdown](https://github.com/cauliyang/ChatResearch/blob/main/images/example2.md) and [PDF report](https://github.com/cauliyang/ChatResearch/blob/main/images/example1.pdf)
+- [Markdown](https://github.com/cauliyang/ChatResearch/blob/main/docs/images/example2.md), [PDF](https://github.com/cauliyang/ChatResearch/blob/main/docs/images/example1.pdf), and [Latex](https://github.com/cauliyang/ChatResearch/blob/main/docs/images/example5.tex)
 
-<img src="https://github.com/cauliyang/ChatResearch/blob/main//tutorial/project.gif" width="800" height="400">
+<img src="https://github.com/cauliyang/ChatResearch/blob/main//docs/tutorial/project.gif" width="800" height="400">
 
 ## Installation
 
 ```console
 $pip install chat-research
 ```
 
 ## Usage
 
-<img src="https://github.com/cauliyang/ChatResearch/blob/main//tutorial/help.gif" width="800" height="400">
+<img src="https://github.com/cauliyang/ChatResearch/blob/main//docs/tutorial/help.gif" width="800" height="400">
 
 ### Chat Config
 
-<img src="https://github.com/cauliyang/ChatResearch/blob/main//tutorial/config.gif" width="800" height="400">
+<img src="https://github.com/cauliyang/ChatResearch/blob/main//docs/tutorial/config.gif" width="800" height="400">
 
 ```console
 ❯ chatre config
 ```
 
 It will generate `chatre.toml` in current working directory. Otherwise,
 setting environment variable `OPENAI_API_KEY` is another way to config API KEY.
@@ -119,23 +118,23 @@
 owner = "your_gitee_name"
 repo = "your_repo_name"
 path = "files_name_in_your_repo"
 ```
 
 ### Chat Paper
 
-<img src="https://github.com/cauliyang/ChatResearch/blob/main//tutorial/paper.gif" width="800" height="400">
+<img src="https://github.com/cauliyang/ChatResearch/blob/main//docs/tutorial/paper.gif" width="800" height="400">
 
 ### Chat Biorxiv
 
-<img src="https://github.com/cauliyang/ChatResearch/blob/main//tutorial/biorxiv.gif" width="800" height="400">
+<img src="https://github.com/cauliyang/ChatResearch/blob/main//docs/tutorial/biorxiv.gif" width="800" height="400">
 
 ### Chat Response
 
-<img src="https://github.com/cauliyang/ChatResearch/blob/main//tutorial/response.gif" width="800" height="400">
+<img src="https://github.com/cauliyang/ChatResearch/blob/main//docs/tutorial/response.gif" width="800" height="400">
 
 ### Chat Reviewer
 
 ```console
 > chatre reviewer -h
 usage: chatre reviewer [-h] --paper-path  [--file-format] [--review-format] [--research-fields] [--language]
```

