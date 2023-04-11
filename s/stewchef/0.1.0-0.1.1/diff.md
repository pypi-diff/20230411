# Comparing `tmp/stewchef-0.1.0.tar.gz` & `tmp/stewchef-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stewchef-0.1.0.tar", max compression
+gzip compressed data, was "stewchef-0.1.1.tar", max compression
```

## Comparing `stewchef-0.1.0.tar` & `stewchef-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       26 2023-04-06 13:22:20.521585 stewchef-0.1.0/README.md
--rw-r--r--   0        0        0      489 2023-04-06 13:27:14.872484 stewchef-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-06 13:20:00.114249 stewchef-0.1.0/stewchef/__init__.py
--rw-r--r--   0        0        0     9935 2023-04-06 13:35:54.058495 stewchef-0.1.0/stewchef/main.py
--rw-r--r--   0        0        0      762 1970-01-01 00:00:00.000000 stewchef-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     5654 2023-04-11 15:37:45.191398 stewchef-0.1.1/README.md
+-rw-r--r--   0        0        0      489 2023-04-11 15:39:30.183809 stewchef-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-06 13:20:00.114249 stewchef-0.1.1/stewchef/__init__.py
+-rw-r--r--   0        0        0    13090 2023-04-11 14:30:19.267721 stewchef-0.1.1/stewchef/main.py
+-rw-r--r--   0        0        0     6390 1970-01-01 00:00:00.000000 stewchef-0.1.1/PKG-INFO
```

### Comparing `stewchef-0.1.0/stewchef/main.py` & `stewchef-0.1.1/stewchef/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,14 +9,31 @@
 import time
 from difflib import Differ
 
 MAX_ITER = 10000
 app = typer.Typer()
 
 def login(URL, USER, PASSWORD):
+    """Logs bot into the Wiki's API.
+
+    This function sends a GET request for a login token and further on
+    a POST request with the bots Username and Password to the URL set in config.toml.
+    All arguments for this function are set in the config.toml file by default.
+    It gets back the active session and CSRF_TOKEN which is required for page
+    modification.
+
+    Args:
+        URL: URL of the Wiki's API endpoint.
+        USER: Username of the bot.
+        PASSWORD: Password of the bot.
+
+    Returns:
+        S: Active session object to send GET/POST requests to.
+        CSRF_TOKEN: A token needed to be given when modifying pages.
+    """
     S = requests.Session()
 
     PARAMS_0 = {
         "action": "query",
         "meta": "tokens",
         "type": "login",
         "format": "json"
@@ -50,15 +67,33 @@
         print(f"[bold red]ERROR![/bold red] Could not log in.. Check credentials for [bold yellow]{URL} [/bold yellow]")
         raise typer.Exit()
 
     return S, CSRF_TOKEN
 
 
 def retrievePagePacket(prev_continue, URL, S, verbose:bool = False):
-    # Get all pages with their matching titles
+    """Get a packet of pages with their matching titles.
+
+    Will query the Wiki API endpoint for all pages via the 'allpages' generator.
+    This generator only returns packets of about 10 pages or so, so multiple queries
+    are needed to get all pages. This function is called multiple times in a while True
+    loop from inside feast() which is where that is done so. This function does not
+    however get their contents, only their titles.
+
+    Args:
+        prev_continue: A token returned by the previous call of the generator. 
+            Is an empty dictionary for first iteration.
+        URL: URL of the Wiki's API endpoint.
+        S: Active session object to send GET/POST requests to.
+        verbose: If True be more verbose.
+    
+    Returns:
+        ALL_PAGE_DATA: Direct data given from GET request 
+        prev_continue: A token returned by the previous call of the generator.
+    """
     PARAMS = {
         "action": "query",
         "generator": "allpages",
         "gapcontinue": prev_continue,
         "format": "json"
     }
 
@@ -77,14 +112,40 @@
     if verbose:
         print(prev_continue)
 
     return ALL_PAGE_DATA, prev_continue
 
 
 def modifyPagePacket(ALL_PAGE_DATA, CSRF_TOKEN, URL, S, regisoup_out: bool = False, commit: bool= False, diff: bool = False):
+    """Take a packet of pages and run them through RegiSoup.
+
+    This function gets the contents of a packet of pages by each
+    individual pages title. It then parses the page contents through 
+    RegiSoup via a temporary file and returns the edited contents. If the
+    commit flag is set, then changes are pushed to the API endpoint via a
+    POST request. A CSRF_TOKEN is needed to commit the changes. It can be
+    the same token for all the changes.
+
+    Args:
+        ALL_PAGE_DATA: Direct data (JSON object) given from GET request to 
+            to the API endpoint called in retrievePagePacket().
+        CSRF_TOKEN: Token gotten from login. Needed to commit changes to Wiki.
+        URL: URL of the Wiki's API endpoint.
+        S: Active session object to send GET/POST requests to.
+        regisoup_out: If true, log the output of RegiSoup to stdout.
+        commit: If true, commit changes to the Wiki.
+        diff: If true, create a directory diff/ and fill it with diff files for
+            each page to be modified. Each title corresponds to one page and a
+            delta difference between the modified and unmodified version is given.
+        
+    Returns:
+        pages_edited: Number of pages that were edited and had those edits
+            committed to the Wiki.
+    
+    """
     # Statistics counters
     pages_edited = 0
 
     # For every page title
     for page in ALL_PAGE_DATA["query"]["pages"]:
         page_data = ALL_PAGE_DATA["query"]["pages"][page]
         page_title = page_data["title"]
@@ -112,15 +173,15 @@
             input = str(soup)
             f.write(input)
 
         print(f"[bold yellow]RegiSoup[/bold yellow] :innocent: is cooking {page_title}")
 
         # Send page contents to RegiSoup
         bashCommand = f"regisoup tmp/tmp_storage.txt  tmp/tmp_out.txt \"{page_title}\""
-        
+
         bash_output = subprocess.run(bashCommand, shell=True, capture_output=True)
         if bash_output.stderr:
             print(f"[bold red]CRITICAL![/bold red] Encountered exception on page {page_title}!")
 
         if regisoup_out:
             print(bash_output.stdout.decode())
 
@@ -145,15 +206,15 @@
 
 
         if diff:
             d = Differ()
             delta = ''.join(list(d.compare(input.splitlines(keepends=True), output.splitlines(keepends=True))))
 
             delta_file = f"diff/{page_title.replace(' ', '')}.diff"
-            
+
             # Create the file path if it does not yet exist
             if not os.path.exists("diff"):
                 os.makedirs("diff")
 
             try:
                 # Write the diff to a file
                 with open(delta_file, "w+") as f:
@@ -172,21 +233,27 @@
 @app.command()
 def feast(config_path: str = typer.Argument("config.toml", help="Filename of config file, relative to RegiSoup's main.py"),
          verbose: bool = typer.Option(False, help = "Be more verbose"),
          commit: bool = typer.Option(False, help = "Commit changes to the live wikipedia API endpoint"),
          diff: bool = typer.Option(False, help = "Get diff after conversion. Output in diff/"),
          regisoup_out: bool = typer.Option(False, help = "Print out RegiSoup responses"),
          dry_run: bool = typer.Option(False, help = "Only retrieve pages but don't send them to RegiSoup")):
+    """
+    StewChef: Feast-size serving
+
+    MASS retrieve all the pages on the Wiki and state modifications by RegiSoup. If specified, changes
+    will be committed to the Wiki given at the API endpoint
+    """
     # Statistics counters
     total_pages_edited = 0
 
     # Read config.toml
     with open(config_path, "rb") as f:
         config = tomllib.load(f)
-    
+
     URL = config["server"]["url"]
 
     USER = config["bot"]["user"]
     PASSWORD = config["bot"]["password"]
 
     with Progress(SpinnerColumn(), TextColumn("[progress.description]{task.description}"), transient=True) as progress:
         task1 = progress.add_task("Logging in..", total=1)
@@ -208,37 +275,42 @@
             # Sleep so we don't spam the server with requests
             time.sleep(0.2)
             iter_counter += 1
 
             # Exit condition from retrievePagePacket() handled here
             if "continue" not in ALL_PAGE_DATA or iter_counter >= MAX_ITER:
                 break
-        
+
         progress.update(task2, advance=1)
 
         if commit:
             print(f"[bold green]Success![/bold green] Retrieved and modified {total_pages_edited} pages :blush:")
         elif dry_run:
             print(f"[bold green]Done recieving pages :blush:[/bold green]")
         elif diff:
             print(f"[bold green]Success![/bold green] Generated diff files :blush:")
         else:
             print(f"[bold green]Success![/bold green] I have done nothing, because you haven't specified any flags :upside__down_face:")
-        
+
 
 @app.command()
 def single(page_title: str = typer.Argument(...,help="Filename of output file, relative to RegiSoup's main.py"),
            config_path: str = typer.Argument("config.toml", help="Filename of config file, relative to RegiSoup's main.py"),
            verbose: bool = typer.Option(False, help = "Be more verbose"),
            save: bool = typer.Option(False, help = "Save requested file"),
            save_path: str = typer.Argument(None, help="Path of file to save requested page"),
            as_html: bool = typer.Option(False, help = "Save file as HTML document")):
+    """
+    StewChef: Single Serving
+
+    Retrieve, modify and, if specified, save a single page of the Wiki
+    given at the API endpoint by the Wiki page's title.
+    """
     print("[bold blue]Cooking up a single serving![/bold blue]")
     # Read config.toml
-
     try:
         with open(config_path, "rb") as f:
             config = tomllib.load(f)
     except FileNotFoundError:
         print(f"[bold red]ERROR![/bold red] Config file not found.. Read the documentation for more information.")
         raise typer.Exit()
 
@@ -263,15 +335,15 @@
         R = S.get(URL, params=PARAMS)
         DATA = R.json()
         try:
             page_contents = DATA["parse"]["wikitext"]["*"]
         except KeyError:
             print(f"[bold red]ERROR![/bold red] Page titled [purple]{page_title}[/purple] not found!")
             raise typer.Exit()  # Exit the program
-        
+
         progress.update(task2, advance=1)
 
         if verbose:
             print(DATA)
         else:
             pprint(page_contents)
 
@@ -283,12 +355,12 @@
 
             if as_html:
                 with open(save_path, "w+") as f:
                     f.write(str(BeautifulSoup(page_contents, features="lxml")))
             else:
                 with open(save_path, "w+") as f:
                     f.write(page_contents)
-    
+
 
 
 # if __name__ == "__main__":
 #     app()
```

