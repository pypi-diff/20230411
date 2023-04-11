# Comparing `tmp/altb-0.4.5.tar.gz` & `tmp/altb-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altb-0.4.5.tar", max compression
+gzip compressed data, was "altb-0.5.1.tar", max compression
```

## Comparing `altb-0.4.5.tar` & `altb-0.5.1.tar`

### file list

```diff
@@ -1,12 +1,20 @@
--rw-r--r--   0        0        0     1535 2023-04-01 21:52:56.911114 altb-0.4.5/README.md
--rw-r--r--   0        0        0        0 2023-04-01 21:52:56.911114 altb-0.4.5/altb/__init__.py
--rw-r--r--   0        0        0      115 2023-04-01 21:52:56.915114 altb-0.4.5/altb/common.py
--rw-r--r--   0        0        0    13877 2023-04-01 21:52:56.915114 altb-0.4.5/altb/config.py
--rw-r--r--   0        0        0      638 2023-04-01 21:52:56.915114 altb-0.4.5/altb/constants.py
--rw-r--r--   0        0        0    14096 2023-04-01 21:52:56.915114 altb-0.4.5/altb/main.py
--rw-r--r--   0        0        0     2545 2023-04-01 21:52:56.915114 altb-0.4.5/altb/options.py
--rw-r--r--   0        0        0     1747 2023-04-01 21:52:56.915114 altb-0.4.5/altb/track.py
--rw-r--r--   0        0        0       18 2023-04-01 21:53:12.347303 altb-0.4.5/altb/version_file.py
--rw-r--r--   0        0        0      751 2023-04-01 21:53:12.307303 altb-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     2456 1970-01-01 00:00:00.000000 altb-0.4.5/setup.py
--rw-r--r--   0        0        0     2393 1970-01-01 00:00:00.000000 altb-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1541 2023-04-11 19:07:53.402512 altb-0.5.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-11 19:07:53.402512 altb-0.5.1/altb/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 19:07:53.402512 altb-0.5.1/altb/common/__init__.py
+-rw-r--r--   0        0        0      109 2023-04-11 19:07:53.402512 altb-0.5.1/altb/common/console.py
+-rw-r--r--   0        0        0      378 2023-04-11 19:07:53.402512 altb-0.5.1/altb/common/constants.py
+-rw-r--r--   0        0        0     1148 2023-04-11 19:07:53.402512 altb-0.5.1/altb/common/rich.py
+-rw-r--r--   0        0        0     3336 2023-04-11 19:07:53.402512 altb-0.5.1/altb/common/selector.py
+-rw-r--r--   0        0        0      275 2023-04-11 19:07:53.402512 altb-0.5.1/altb/common/utils.py
+-rw-r--r--   0        0        0    10799 2023-04-11 19:07:53.402512 altb-0.5.1/altb/main.py
+-rw-r--r--   0        0        0        0 2023-04-11 19:07:53.402512 altb-0.5.1/altb/model/__init__.py
+-rw-r--r--   0        0        0      739 2023-04-11 19:07:53.402512 altb-0.5.1/altb/model/config.py
+-rw-r--r--   0        0        0     1021 2023-04-11 19:07:53.402512 altb-0.5.1/altb/model/settings.py
+-rw-r--r--   0        0        0     1548 2023-04-11 19:07:53.402512 altb-0.5.1/altb/model/tags.py
+-rw-r--r--   0        0        0     2680 2023-04-11 19:07:53.402512 altb-0.5.1/altb/options.py
+-rw-r--r--   0        0        0    10849 2023-04-11 19:07:53.402512 altb-0.5.1/altb/service.py
+-rw-r--r--   0        0        0     1805 2023-04-11 19:07:53.402512 altb-0.5.1/altb/track.py
+-rw-r--r--   0        0        0       18 2023-04-11 19:08:01.882676 altb-0.5.1/altb/version_file.py
+-rw-r--r--   0        0        0      898 2023-04-11 19:08:01.846675 altb-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2490 1970-01-01 00:00:00.000000 altb-0.5.1/setup.py
+-rw-r--r--   0        0        0     2398 1970-01-01 00:00:00.000000 altb-0.5.1/PKG-INFO
```

### Comparing `altb-0.4.5/README.md` & `altb-0.5.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 example:
 ```bash
 altb use python@2.7
 ```
 this will link the tracked path to `~/.local/bin/<app_name>` in this case - `~/.local/bin/python`
 
-Copy specific standalone binary automatically to `~/.local/altb/versions/<app_name>/<app_name>_<tag>`
+Copy specific standalone binary automatically to `~/.local/share/altb/versions/<app_name>/<app_name>_<tag>`
 ```bash
 altb track path helm@3 ~/Downloads/helm --copy
 ```
 
 You can run custom commands using:
 ```bash
 altb track command special_command@latest "echo This is a command"
```

### Comparing `altb-0.4.5/altb/main.py` & `altb-0.5.1/altb/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,197 +1,95 @@
 import sys
-import curses
 import json
-from contextlib import contextmanager
-from typing import ContextManager, Union, List, Dict, TypeVar, TypedDict, Tuple, Optional, cast
+from typing import List, Optional, cast
 
 import typer
 import yaml
-from rich.live import Live
 from rich.tree import Tree
 from rich.text import Text
-from blessed import Terminal
 from natsort import natsorted
 from rich.padding import Padding
 from rich.prompt import Confirm
 from rich.syntax import Syntax
-from rich.console import ConsoleRenderable, Console, ConsoleOptions, RenderResult, Group
+from rich.console import Group
 
 from altb import version_file
+from altb.common.console import error_console, console
+from altb.common.rich import RichText
+from altb.common.selector import Entry, run_selector
+from altb.common.utils import pretty_errors
+from altb.model.config import AppConfig
+from altb.model.settings import Settings
+from altb.model.tags import TagConfig, LinkTag, CommandTag
+from altb.service import AltbService
 from altb.track import track
-from altb.common import console, error_console
-from altb.config import (Settings,
-                         RichText,
-                         TagConfig,
-                         settings_changes,
-                         pretty_errors, CommandTag, LinkTag)
-from altb.constants import TYPE_TO_COLOR, PACKAGE_NAME
+from altb.common.constants import TYPE_TO_COLOR, PACKAGE_NAME
 from altb.options import (app_name_option,
                           is_short_option,
                           is_current_option,
                           all_tags_option,
                           full_app_name_option, should_force_option)
 
-app = typer.Typer(pretty_exceptions_enable=False)
-
-T = TypeVar("T")
-
 
-class Entry(TypedDict):
-    key: Union[str, Text]
-    value: T
-
-
-class Selector(ConsoleRenderable):
-    def __init__(self, options: List[Entry]):
-        self.options = options
-        self.marked = set()
-        self._hovered = 0
-
-    def increment(self):
-        if self._hovered < len(self.options) - 1:
-            self._hovered += 1
-
-        else:
-            self._hovered = 0
-
-    def decrement(self):
-        if self._hovered > 0:
-            self._hovered -= 1
-
-        else:
-            self._hovered = len(self.options) - 1
-
-    def select(self):
-        element = self._hovered
-        if element in self.marked:
-            self.marked.remove(element)
-
-        else:
-            self.marked.add(element)
-
-    @property
-    def selections(self) -> List[T]:
-        return [self.options[i]['value'] for i in self.marked]
-
-    def __rich_console__(
-            self, console: Console, options: ConsoleOptions
-    ) -> RenderResult:
-        for i, row in enumerate(self.options):
-            marked_char = "⬢" if i in self.marked else "⬡"
-            hovered_char = "➤" if i == self._hovered else " "
-            symbol_style_fg = "default"
-            symbol_style_bg = "default"
-            text_style_fg = "default"
-            text_style_bg = "default"
-            hovered_style_fg = "default"
-            hovered_style_bg = "default"
-            if i == self._hovered:
-                hovered_style_bg = symbol_style_bg = text_style_bg = "default"
-                hovered_style_fg = symbol_style_fg = text_style_fg = "default"
-
-            if i in self.marked:
-                text_style_fg = "green4"
-                symbol_style_fg = "green4"
-
-            text_style = f"{text_style_fg} on {text_style_bg}"
-            symbol_style = f"{symbol_style_fg} on {symbol_style_bg}"
-            hovered_style = f"{hovered_style_fg} on {hovered_style_bg}"
-            rendered_row = Text(f"{hovered_char} ", style=hovered_style, end="")
-            yield Group(rendered_row, row['key'])
-
-
-@contextmanager
-def run_selector(options: List[Dict[str, T]], single=True) -> ContextManager[Tuple[Live, Selector]]:
-    term = Terminal()
-    selector = Selector(options)
-    with term.cbreak(), term.hidden_cursor():
-        with Live(selector, auto_refresh=False) as live:  # update 4 times a second to feel fluid
-            try:
-                done = False
-                while not done:
-                    val = term.inkey(timeout=0.5)
-                    if val.is_sequence and val.code == curses.KEY_DOWN or \
-                            (not val.is_sequence and str(val).lower() == "j") or \
-                            (val.code == term.KEY_TAB):
-                        selector.increment()
-
-                    elif (val.is_sequence and val.code == curses.KEY_UP) or \
-                            (not val.is_sequence and str(val).lower() == "k"):
-                        selector.decrement()
-
-                    elif str(val) == " ":
-                        selector.select()
-                        if single:
-                            done = True
-
-                    elif val.is_sequence and val.code == curses.KEY_ENTER:
-                        if single:
-                            selector.select()
-                        done = True
-
-                    live.refresh()
-
-                yield live, selector
+app = typer.Typer(pretty_exceptions_enable=False)
 
-            except KeyboardInterrupt:
-                raise
+app.add_typer(track, name="track")
 
 
 @app.command()
 def config(ctx: typer.Context, is_json: bool = typer.Option(False, '-j', '--json', help='Output in json format')):
     """Get the config specifications."""
     settings = ctx.ensure_object(Settings)
-    to_print = settings.config.json(indent=2)
+    service = AltbService(settings)
+    to_print = service.config.json(indent=2)
     if not is_json:
         to_print = yaml.safe_dump(yaml.safe_load(to_print))
 
     if sys.stdout.isatty():
         console.print(Syntax(to_print, "yaml" if not is_json else "json",
                              background_color="default", word_wrap=True))
 
     else:
         typer.echo(to_print)
 
 
-app.add_typer(track, name="track")
-
-
 @app.command(name="list")
 def list_applications(
         ctx: typer.Context,
         app_name=app_name_option,
         is_short=is_short_option,
         all_tags=all_tags_option,
         current_only=is_current_option,
 ):
     """List all applications tracked."""
     settings = ctx.ensure_object(Settings)
-    if len(settings.config.binaries) == 0:
+    service = AltbService(settings)
+
+    if len(service.config.binaries) == 0:
         error_console.print(f'No binaries currently tracked, please use "{PACKAGE_NAME} track" command to start')
         return
 
-    if app_name is not None and app_name not in settings.config.binaries:
+    if app_name is not None and app_name not in service.config.binaries:
         error_console.print(RichText('app {app_name} doesn\'t exist in config!', app_name=app_name))
         raise typer.Exit(1)
 
     if app_name is not None and current_only:
-        selected_tag = settings.config.binaries[app_name].selected
+        selected_tag = service.config.binaries[app_name].selected
         if not selected_tag:
             error_console.print(RichText("app {app_name} doesn\'t have selected tag!", app_name=app_name))
             raise typer.Exit(1)
 
         console.print(Text(selected_tag, style=TYPE_TO_COLOR['tag']))
         return
 
-    app_names = [app_name] if app_name is not None else settings.config.binaries.keys()
+    app_names = [app_name] if app_name is not None else service.config.binaries.keys()
     for app_name in app_names:
         tree = Tree(Text(app_name, style=TYPE_TO_COLOR['app_name']))
-        selected_tag = settings.config.binaries[app_name].selected
-        for tag, value in natsorted(settings.config.binaries[app_name].tags.items(), key=lambda a: a[0]):
+        selected_tag = service.config.binaries[app_name].selected
+        for tag, value in natsorted(service.config.binaries[app_name].tags.items(), key=lambda a: a[0]):
             tag_struct = cast(TagConfig, value)
             if not all_tags and tag != selected_tag:
                 continue
 
             group = Group()
             line = Text("* " if tag == selected_tag else "  ", style="bold magenta3") + Text(tag,
                                                                                              style=TYPE_TO_COLOR['tag'])
@@ -225,16 +123,16 @@
     """Rename tag."""
     settings = ctx.ensure_object(Settings)
     app_name, tag = app_details
     if not tag:
         error_console.print(RichText('tag not specified for application {app_name}', app_name=app_name))
         raise typer.Exit(1)
 
-    with settings_changes(settings):
-        settings.config.rename_tag(app_name, tag, tag_name)
+    with pretty_errors(), AltbService(settings) as service:
+        service.rename_tag(app_name, tag, tag_name)
 
 
 @app.command()
 def describe(
         ctx: typer.Context,
         app_details=full_app_name_option,
         description: str = typer.Option(None, "-d", "--description", help="Description of the tracked file"),
@@ -247,36 +145,36 @@
         raise typer.Exit(1)
 
     if description is None:
         should_continue = Confirm.ask("Description will be deleted, are you sure?", default=False)
         if not should_continue:
             raise typer.Exit(1)
 
-    with settings_changes(settings):
-        settings.config.describe_tag(app_name, tag, description)
+    with pretty_errors(), AltbService(settings) as service:
+        service.describe_tag(app_name, tag, description)
 
 
-def get_app_dynamic(settings: Settings):
-    apps: List[str] = natsorted(settings.config.binaries.keys())
+def get_app_dynamic(app_config: AppConfig):
+    apps: List[str] = natsorted(app_config.binaries.keys())
     options: List[Entry] = []
     for app_name in apps:
         options.append({
             "key": RichText("{app_name}", app_name=app_name).text,
             "value": app_name,
         })
 
     with run_selector(options) as context:
         live, selector = context
         app_name = selector.selections[0]
         live.update(RichText('select tag for {app_name}:', app_name=app_name))
         return app_name
 
 
-def get_tag_dynamic(settings: Settings, app_name: str):
-    tags = natsorted(settings.config.binaries[app_name].tags.items(), key=lambda a: a[0])
+def get_tag_dynamic(app_config: AppConfig, app_name: str):
+    tags = natsorted(app_config.binaries[app_name].tags.items(), key=lambda a: a[0])
     options: List[Entry] = []
     for tag, details in tags:
         if isinstance(details, LinkTag):
             options.append({
                 "key": RichText("{tag} - {app_path}", tag=tag, app_path=details.spec.path).text,
                 "value": tag,
             })
@@ -301,72 +199,75 @@
 def use(
         ctx: typer.Context,
         app_details=full_app_name_option,
         force=should_force_option,
 ):
     """Select which tag to run of a given app."""
     settings = ctx.ensure_object(Settings)
+    service = AltbService(settings)
     app_name, tag = app_details
     if not tag:
-        tag = get_tag_dynamic(settings, app_name)
+        tag = get_tag_dynamic(service.config, app_name)
 
     console.print(RichText('using tag {tag} for app {app_name}', tag=tag, app_name=app_name))
-    with settings_changes(settings):
-        settings.config.select(app_name, tag, force=force)
+    with pretty_errors(), AltbService(settings) as service:
+        service.select(app_name, tag, force=force)
 
 
 @app.command()
 def run(
         ctx: typer.Context,
         app_name=app_name_option,
         args: Optional[List[str]] = typer.Argument(None)
 ):
     """Run application with propagated args."""
     if args is None:
         args = []
 
     settings = ctx.ensure_object(Settings)
-    with pretty_errors():
-        settings.config.run(app_name, args)
+    with pretty_errors(), AltbService(settings) as service:
+        service.run(app_name, args)
 
 
 @app.command()
 def untrack(
         ctx: typer.Context,
         app_details=full_app_name_option,
 ):
     """Remove tracking of a tag completely."""
     settings = ctx.ensure_object(Settings)
+    service = AltbService(settings)
     app_name, tag = app_details
     if not tag:
-        tag = get_tag_dynamic(settings, app_name)
+        tag = get_tag_dynamic(service.config, app_name)
 
-    with settings_changes(settings):
-        settings.config.remove(app_name, tag)
+    with pretty_errors(), AltbService(settings) as service:
+        service.remove(app_name, tag)
 
 
 @app.command()
 def unlink(
         ctx: typer.Context,
         app_name=app_name_option,
 ):
     """Unset selected tag for a given app."""
     settings = ctx.ensure_object(Settings)
-    with settings_changes(settings):
-        settings.config.select(app_name, tag=None)
+    with pretty_errors(), AltbService(settings) as service:
+        service.select(app_name, tag=None)
 
 
 @app.command()
 def schema(
         ctx: typer.Context,
         model: Optional[str] = typer.Argument(None),
         dump_all: Optional[bool] = typer.Option(False, '-a', '--all', help='Dump all scheme')
 ):
     settings = ctx.ensure_object(Settings)
-    schema = settings.config.schema()
+    service = AltbService(settings)
+    schema = service.config.schema()
 
     if model is not None:
         if model not in schema['definitions']:
             error_console.print(RichText('model `{model}` does not exists', model=model))
             raise typer.Exit(1)
 
         console.print(Syntax(json.dumps(schema['definitions'][model], indent=2), "json",
@@ -390,15 +291,16 @@
         raise typer.Exit()
 
     if ctx.invoked_subcommand is not None:
         return
 
     # if no subcommand is specified, use the default one
     settings = ctx.ensure_object(Settings)
-    app_name = get_app_dynamic(settings)
+    service = AltbService(settings)
+    app_name = get_app_dynamic(service.config)
     ctx.invoke(use, ctx=ctx, app_details=(app_name, None))
 
 
 def main():
     app()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `altb-0.4.5/altb/options.py` & `altb-0.5.1/altb/options.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-import pathlib
 import re
 from typing import Optional
 
 import typer
 
-from altb.common import error_console
-from altb.config import Settings, LinkTag, CommandTag
+from altb.common.console import error_console
+from altb.model.settings import Settings
+from altb.model.tags import LinkTag, CommandTag
+from altb.service import AltbService
 
 app_name_regex = re.compile(r'(?P<app_name>[\w\-_]+)(?:@(?P<tag>.+))?')
 
 
 def complete_app_name(ctx: typer.Context, incomplete: str):
     settings = ctx.ensure_object(Settings)
-    for app_name in settings.config.binaries:
+    service = AltbService(settings)
+    for app_name in service.config.binaries:
         if incomplete in app_name:
             yield app_name
 
 
 def parse_app_name(ctx: typer.Context, full_app_name: str) -> tuple[str, str]:
     match = app_name_regex.match(full_app_name)
     if not match:
@@ -24,20 +26,21 @@
         raise typer.Exit(1)
 
     return match.group('app_name'), match.group('tag')
 
 
 def complete_full_app_name(ctx: typer.Context, incomplete: str):
     settings = ctx.ensure_object(Settings)
+    service = AltbService(settings)
     app_names = list(complete_app_name(ctx, incomplete))
     if "@" not in incomplete and len(app_names) > 1:
         yield from app_names
 
     else:
-        for key, binary_struct in settings.config.binaries.items():
+        for key, binary_struct in service.config.binaries.items():
             yield key
             for tag, tag_struct in binary_struct.tags.items():
                 full_name = f"{key}@{tag}"
                 if incomplete in full_name:
                     if isinstance(tag_struct, LinkTag):
                         yield full_name, str(tag_struct.spec.path)
```

### Comparing `altb-0.4.5/altb/track.py` & `altb-0.5.1/altb/track.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import pathlib
 from typing import Optional
 
 import typer
 
-from altb.config import Settings, settings_changes
+from altb.common.utils import pretty_errors
+from altb.model.settings import Settings
 from altb.options import should_copy_option, should_force_option, full_app_name_option
+from altb.service import AltbService
 
 track = typer.Typer()
 
 
 @track.command()
 def path(
         ctx: typer.Context,
@@ -17,27 +19,26 @@
         description: str = typer.Option(None, "-d", "--description", help="Description of the tracked file"),
         should_copy: bool = should_copy_option,
         force: bool = should_force_option,
 ):
     """Add new tracking of path kind."""
     settings = ctx.ensure_object(Settings)
     app_name, tag = app_details
-    with settings_changes(settings):
-        settings.config.track_path(app_name, app_path, tag=tag, description=description, should_copy=should_copy,
-                                   force=force)
+    with pretty_errors(), AltbService(settings) as service:
+        service.track_path(app_name, app_path, tag=tag, description=description, should_copy=should_copy, force=force)
 
 
 @track.command()
 def command(
         ctx: typer.Context,
         app_details=full_app_name_option,
         command_string: str = typer.Argument(..., help='Command to run'),
         description: str = typer.Option(None, "-d", "--description", help="Description of the tracked file"),
         working_directory: Optional[pathlib.Path] = typer.Option(None, '-w', '--working-directory',
                                                                  help="Working directory of running command"),
 ):
     """Add new tracking of command kind."""
     settings = ctx.ensure_object(Settings)
     app_name, tag = app_details
-    with settings_changes(settings):
-        settings.config.track_command(app_name, command_string, tag=tag, description=description,
-                                      working_directory=working_directory)
+    with pretty_errors(), AltbService(settings) as service:
+        service.track_command(app_name, command_string, tag=tag, description=description,
+                              working_directory=working_directory)
```

### Comparing `altb-0.4.5/pyproject.toml` & `altb-0.5.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 [tool.poetry]
 name = "altb"
-version = "0.4.5"  # this means version is development
+version = "0.5.1"  # this means version is development
 description = "Cli tool for tracking over binaries and easily swapping between them"
 readme = "README.md"
 authors = ["Elran Shefer <elran777@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Utilities",
 ]
 homepage = "https://github.com/IamShobe/altb"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-rich = "^10.15.2"
+rich = "^13.3.3"
 getch = "^1.0"
 blessed = "^1.19.0"
 pydantic = "^1.8.2"
 typer = "^0.7.0"
 PyYAML = "^6.0"
 natsort = "^8.3.1"
 
 [tool.poetry.dev-dependencies]
 ipdb = "^0.13.9"
 
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.3.0"
+ruff = "^0.0.261"
+mypy = "^1.2.0"
+types-pyyaml = "^6.0.12.9"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 altb = 'altb.main:main'
+
+[tool.ruff]
+line-length = 120
```

### Comparing `altb-0.4.5/setup.py` & `altb-0.5.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['altb']
+['altb', 'altb.common', 'altb.model']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['PyYAML>=6.0,<7.0',
  'blessed>=1.19.0,<2.0.0',
  'getch>=1.0,<2.0',
  'natsort>=8.3.1,<9.0.0',
  'pydantic>=1.8.2,<2.0.0',
- 'rich>=10.15.2,<11.0.0',
+ 'rich>=13.3.3,<14.0.0',
  'typer>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['altb = altb.main:main']}
 
 setup_kwargs = {
     'name': 'altb',
-    'version': '0.4.5',
+    'version': '0.5.1',
     'description': 'Cli tool for tracking over binaries and easily swapping between them',
-    'long_description': '# altb\naltb is a cli utility influenced by `update-alternatives` of ubuntu.  \nLinked paths are added to `$HOME/.local/bin` according to [XDG Base Directory Specification](https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html).  \nConfig file is located at `$HOME/.config/altb/config.yaml`.\n\n### How to start?\n\n**Must use Python > 3.9**\nexecute:\n```bash\npipx install altb\n```\n\nto track new binary use:\n```bash\naltb track path <app_name>@<app_tag> /path/to/binary\n```\nfor example:\n```bash\naltb track path python@2.7 /bin/python2.7\naltb track path python@3.8 /bin/python3.8\n# altb track path python ~/Downloads/python # will also work and generate a new hash for it\n```\n\nList all tracked versions:\n```bash\n$ altb list -a\npython\n|----   2.7 - /bin/python2.7\n|----   3.8 - /bin/python3.8\n```\n\nUse specific version:\n```bash\naltb use <app_name>[@<app_tag>]\n```\n\nexample:\n```bash\naltb use python@2.7\n```\nthis will link the tracked path to `~/.local/bin/<app_name>` in this case - `~/.local/bin/python`\n\nCopy specific standalone binary automatically to `~/.local/altb/versions/<app_name>/<app_name>_<tag>`\n```bash\naltb track path helm@3 ~/Downloads/helm --copy\n```\n\nYou can run custom commands using:\n```bash\naltb track command special_command@latest "echo This is a command"\n```\nthis especially useful for latest developments, example:\n```bash\naltb track command special_command@latest "go run ./cmd/special_command" --working-directory "$HOME/special_command"\n```\n',
+    'long_description': '# altb\naltb is a cli utility influenced by `update-alternatives` of ubuntu.  \nLinked paths are added to `$HOME/.local/bin` according to [XDG Base Directory Specification](https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html).  \nConfig file is located at `$HOME/.config/altb/config.yaml`.\n\n### How to start?\n\n**Must use Python > 3.9**\nexecute:\n```bash\npipx install altb\n```\n\nto track new binary use:\n```bash\naltb track path <app_name>@<app_tag> /path/to/binary\n```\nfor example:\n```bash\naltb track path python@2.7 /bin/python2.7\naltb track path python@3.8 /bin/python3.8\n# altb track path python ~/Downloads/python # will also work and generate a new hash for it\n```\n\nList all tracked versions:\n```bash\n$ altb list -a\npython\n|----   2.7 - /bin/python2.7\n|----   3.8 - /bin/python3.8\n```\n\nUse specific version:\n```bash\naltb use <app_name>[@<app_tag>]\n```\n\nexample:\n```bash\naltb use python@2.7\n```\nthis will link the tracked path to `~/.local/bin/<app_name>` in this case - `~/.local/bin/python`\n\nCopy specific standalone binary automatically to `~/.local/share/altb/versions/<app_name>/<app_name>_<tag>`\n```bash\naltb track path helm@3 ~/Downloads/helm --copy\n```\n\nYou can run custom commands using:\n```bash\naltb track command special_command@latest "echo This is a command"\n```\nthis especially useful for latest developments, example:\n```bash\naltb track command special_command@latest "go run ./cmd/special_command" --working-directory "$HOME/special_command"\n```\n',
     'author': 'Elran Shefer',
     'author_email': 'elran777@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/IamShobe/altb',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `altb-0.4.5/PKG-INFO` & `altb-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altb
-Version: 0.4.5
+Version: 0.5.1
 Summary: Cli tool for tracking over binaries and easily swapping between them
 Home-page: https://github.com/IamShobe/altb
 License: MIT
 Author: Elran Shefer
 Author-email: elran777@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Utilities
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: blessed (>=1.19.0,<2.0.0)
 Requires-Dist: getch (>=1.0,<2.0)
 Requires-Dist: natsort (>=8.3.1,<9.0.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
-Requires-Dist: rich (>=10.15.2,<11.0.0)
+Requires-Dist: rich (>=13.3.3,<14.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 # altb
 altb is a cli utility influenced by `update-alternatives` of ubuntu.  
 Linked paths are added to `$HOME/.local/bin` according to [XDG Base Directory Specification](https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html).  
 Config file is located at `$HOME/.config/altb/config.yaml`.
@@ -62,15 +62,15 @@
 
 example:
 ```bash
 altb use python@2.7
 ```
 this will link the tracked path to `~/.local/bin/<app_name>` in this case - `~/.local/bin/python`
 
-Copy specific standalone binary automatically to `~/.local/altb/versions/<app_name>/<app_name>_<tag>`
+Copy specific standalone binary automatically to `~/.local/share/altb/versions/<app_name>/<app_name>_<tag>`
 ```bash
 altb track path helm@3 ~/Downloads/helm --copy
 ```
 
 You can run custom commands using:
 ```bash
 altb track command special_command@latest "echo This is a command"
```

