# Comparing `tmp/psg_reskinner-2.3.7.tar.gz` & `tmp/psg_reskinner-2.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psg_reskinner-2.3.7.tar", last modified: Sat Apr  8 02:13:03 2023, max compression
+gzip compressed data, was "N:\Code\Python\psg_reskinner\dist\.tmp-t9rkq8yy\psg_reskinner-2.3.8.tar", last modified: Tue Apr 11 02:25:37 2023, max compression
```

## Comparing `psg_reskinner-2.3.7.tar` & `psg_reskinner-2.3.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 02:13:03.340000 psg_reskinner-2.3.7/
--rw-rw-rw-   0        0        0     1097 2022-08-17 20:33:30.000000 psg_reskinner-2.3.7/LICENSE
--rw-rw-rw-   0        0        0     3351 2023-04-08 02:13:04.000000 psg_reskinner-2.3.7/PKG-INFO
--rw-rw-rw-   0        0        0     3533 2022-11-09 13:37:28.000000 psg_reskinner-2.3.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 02:13:03.510000 psg_reskinner-2.3.7/psg_reskinner/
--rw-rw-rw-   0        0        0      169 2022-11-08 22:43:38.000000 psg_reskinner-2.3.7/psg_reskinner/__init__.py
--rw-rw-rw-   0        0        0    37099 2023-04-08 01:10:44.000000 psg_reskinner-2.3.7/psg_reskinner/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-08 02:13:03.570000 psg_reskinner-2.3.7/psg_reskinner.egg-info/
--rw-rw-rw-   0        0        0     3351 2023-04-08 02:13:04.000000 psg_reskinner-2.3.7/psg_reskinner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2023-04-08 02:13:04.000000 psg_reskinner-2.3.7/psg_reskinner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 02:13:04.000000 psg_reskinner-2.3.7/psg_reskinner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-08 02:13:04.000000 psg_reskinner-2.3.7/psg_reskinner.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-08 02:13:04.000000 psg_reskinner-2.3.7/psg_reskinner.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1011 2023-04-08 02:12:00.000000 psg_reskinner-2.3.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-08 02:13:04.000000 psg_reskinner-2.3.7/setup.cfg
--rw-rw-rw-   0        0        0     1022 2022-11-05 19:22:34.000000 psg_reskinner-2.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 02:25:37.000000 psg_reskinner-2.3.8/
+-rw-rw-rw-   0        0        0     1316 2022-11-09 13:35:42.000000 psg_reskinner-2.3.8/DESCRIPTION.md
+-rw-rw-rw-   0        0        0     1097 2022-08-17 20:33:30.000000 psg_reskinner-2.3.8/LICENSE
+-rw-rw-rw-   0        0        0     3260 2023-04-11 02:25:38.000000 psg_reskinner-2.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3592 2023-04-11 02:00:46.000000 psg_reskinner-2.3.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 02:25:37.000000 psg_reskinner-2.3.8/psg_reskinner/
+-rw-rw-rw-   0        0        0      169 2022-11-08 22:43:38.000000 psg_reskinner-2.3.8/psg_reskinner/__init__.py
+-rw-rw-rw-   0        0        0    36667 2023-04-11 02:00:48.000000 psg_reskinner-2.3.8/psg_reskinner/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 02:25:37.000000 psg_reskinner-2.3.8/psg_reskinner.egg-info/
+-rw-rw-rw-   0        0        0     3260 2023-04-11 02:25:38.000000 psg_reskinner-2.3.8/psg_reskinner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-04-11 02:25:38.000000 psg_reskinner-2.3.8/psg_reskinner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 02:25:38.000000 psg_reskinner-2.3.8/psg_reskinner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-04-11 02:25:38.000000 psg_reskinner-2.3.8/psg_reskinner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-11 02:25:38.000000 psg_reskinner-2.3.8/psg_reskinner.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1379 2023-04-11 02:23:48.000000 psg_reskinner-2.3.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-11 02:25:38.000000 psg_reskinner-2.3.8/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `psg_reskinner-2.3.7/LICENSE` & `psg_reskinner-2.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `psg_reskinner-2.3.7/PKG-INFO` & `psg_reskinner-2.3.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: psg_reskinner
-Version: 2.3.7
+Version: 2.3.8
 Summary: Instantaneous theme changing for PySimpleGUI windows.
-Home-page: https://github.com/definite-d/psg_reskinner/
-Author: Divine U. Afam-Ifediogor
 Author-email: "Divine U. Afam-Ifediogor" <divineafam@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Divine Afam-Ifediogor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `psg_reskinner-2.3.7/README.md` & `psg_reskinner-2.3.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -20,21 +20,21 @@
 Reskinner is a Python 3 plugin for PySimpleGUI's Tkinter port which enables changing the theme of a PySimpleGUI window on the fly without the need for re-instantiating the window.
 
 Please consider starring the project if you find it useful.
 
 ## Example Usage (Demo)
 
 ```python
-# Reskinner Version 2
+# Reskinner Version 2.3.8
 
 from psg_reskinner import reskin, animated_reskin, __version__
-from PySimpleGUI import Window, Text, Button, Push, Titlebar, theme_list, theme, LOOK_AND_FEEL_TABLE, TIMEOUT_KEY
+from PySimpleGUI import Window, Text, Button, Push, Titlebar, theme, LOOK_AND_FEEL_TABLE, TIMEOUT_KEY
 from random import choice as rc
 
-rmenu = ['', ['Hi', 'There']]
+rmenu = ['', [['Hi', ['Next Level', ['Deeper Level', ['a', 'b', 'c']], 'Hoho']], 'There']]
 
 window_layout = [
     [Titlebar('Reskinner Demo')],
     [Text('Hello!', font=('Helvetica', 20))],
     [Text('You are currently running Reskinner instead of importing it.')],
     [Text('The theme of this window changes every 3 seconds.')],
     [Text('Changing to:')],
@@ -50,20 +50,23 @@
 
     if e in (None, 'Exit'):
         window.Close()
         break
 
     elif e == TIMEOUT_KEY:
         '''reskin(window, rc(theme_list()), theme, LOOK_AND_FEEL_TABLE)'''
-        new = rc(safethemes)
+        new = rc(LOOK_AND_FEEL_TABLE.keys())
         window['ctheme'].update(new)
-        animated_reskin(window=window,
-                        new_theme=new,
-                        theme_function=theme,
-                        lf_table=LOOK_AND_FEEL_TABLE,)
+        animated_reskin(
+            window=window,
+            new_theme=new,
+            theme_function=theme,
+            lf_table=LOOK_AND_FEEL_TABLE,
+        )
+
 ``` 
 
 ## How does it work?
 
 Reskinner runs through each element in a window, then by relying on the `element.widget` interface to access the underlying Tkinter object, it applies style changes to the window.
 
 ## What's the story behind psg_reskinner?
```

### Comparing `psg_reskinner-2.3.7/psg_reskinner/__main__.py` & `psg_reskinner-2.3.8/psg_reskinner/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 PySimpleGUI Reskinner Plugin
 
 https://github.com/definite_d/psg_reskinner/
+
 Enables changing the theme of a PySimpleGUI window on the fly without the need for re-instantiating the window
 
-Copyright (c) 2022 Divine Afam-Ifediogor
+Copyright (c) 2023 Divine Afam-Ifediogor
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -20,32 +21,32 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
-
 # IMPORTS
-from _tkinter import TclError
-from colour import COLOR_NAME_TO_RGB, Color
 from datetime import datetime as dt, timedelta
-from PySimpleGUI.PySimpleGUI import COLOR_SYSTEM_DEFAULT, LOOK_AND_FEEL_TABLE, TITLEBAR_METADATA_MARKER,\
-    Window, _hex_to_hsl, _hsl_to_rgb, rgb, theme, theme_add_new, theme_background_color, theme_button_color, \
-    theme_input_background_color, theme_input_text_color, theme_progress_bar_color, theme_slider_color, \
-    theme_text_color, theme_text_element_background_color, ttk_part_mapping_dict
 from random import choice as rc
+from tkinter import Menu as TKMenu, Widget
 from tkinter.ttk import Style
 from typing import Callable, Dict, Union
 from warnings import warn
 
+from PySimpleGUI.PySimpleGUI import COLOR_SYSTEM_DEFAULT, LOOK_AND_FEEL_TABLE, TITLEBAR_METADATA_MARKER, \
+    Window, _hex_to_hsl, _hsl_to_rgb, rgb, theme, ttk_part_mapping_dict
+from _tkinter import TclError
+
+from colour import COLOR_NAME_TO_RGB, Color
+
 # VERSIONING
-__version__: str = '2.3.7'
+__version__: str = '2.3.8'
 
-# DEPRECATIION TRIGGER
+# DEPRECATION TRIGGER
 if __version__.startswith('2.4'):
     m = 'Hello! Annoying little reminder to remove the deprecated functions, and this message.'
     raise Exception(m)
 
 # CONSTANTS
 NON_GENERIC_ELEMENTS = [
     'progressbar',
@@ -264,27 +265,28 @@
     Internal use only.
 
     Performs an interpolation calculation between two colors (start and end) and returns a Color object as the result.
     Inspired by https://www.alanzucconi.com/2016/01/06/colour-interpolation/ .
 
     - RGB interpolation is simple lerping through RGB color space.
     - Hue interpolation is lerping through HSL color space but moving only forward on the hue scale until it reaches the end color.
-    - HSV interpolation also lerps across HSL color space but it takes the shortest route to get to the end color.
+    - HSV interpolation also lerps across HSL color space, but it takes the shortest route to get to the end color.
 
     Note: "lerp" means "linear-interpolation", in case you didn't know.
 
     Each interpolation mode has a different visual effect which may look better than the others in certain scenarios.
 
     First available from v2.3.4.
 
+
     :param start: The starting color.
     :param end: The end color.
     :param progress: A float representing the current point in the interpolation where 0 marks the beginning and 1 marks
     the end.
-    :param mode: The method to use for the interpolation calculation. Defaults to RGB interpolation.
+    :param interpolation_mode: The method to use for the interpolation calculation. Defaults to RGB interpolation.
     :return: A web-format color string representing the result of the calculation.
     """
     result = Color()
     start = Color(start)
     end = Color(end)
     if interpolation_mode == RGB_INTERPOLATION:
         result.set_red((start.get_red() + ((end.get_red() - start.get_red()) * progress)))
@@ -309,14 +311,41 @@
         result.set_hue(hue)
         result.set_saturation((start.get_saturation() + ((end.get_saturation() - start.get_saturation()) * progress)))
         result.set_luminance((start.get_luminance() + ((end.get_luminance() - start.get_luminance()) * progress)))
 
     return result.get_web()
 
 
+def _recurse_menu(tkmenu: Union[TKMenu, Widget], fg: Union[Color, str], bg: Union[Color, str]):
+    """
+    Internal use only.
+
+    New and improved logic to change the theme of menus; we no longer take the lazy route of
+    re-declaring new menu elements with each theme change - a method which Tkinter has an upper limit
+    on. Rather, we recursively find and reconfigure the individual Menu objects that make up menus and
+    submenus.
+
+    First available from v2.3.7.
+
+    :param tkmenu: The Tkinter menu object.
+    :return: None
+    """
+    for index in range(0, tkmenu.index('end') + 1):
+        tkmenu.entryconfigure(
+            index,
+            background=bg,
+            foreground=fg,
+            activeforeground=bg,
+            activebackground=fg,
+        )
+    for child in tkmenu.children.values():
+        if issubclass(type(child), TKMenu):
+            _recurse_menu(child, fg, bg)
+
+
 # RESKIN AND UTILITY FUNCTIONS
 def reskin(
         window: Window,
         new_theme: str,
         theme_function: Callable,
         lf_table: dict,
         set_future: bool = False,
@@ -359,15 +388,15 @@
     old_theme, old_theme_dict = WINDOW_THEME_MAP[window]
 
     # New theme stuff
     new_theme_dict = lf_table[new_theme].copy()
 
     # Window level changes
     if reskin_background:
-        window.TKroot.config(background=new_theme_dict['BACKGROUND'])
+        window.TKroot.configure(background=new_theme_dict['BACKGROUND'])
 
     titlebar_row_frame = 'Not Set'
 
     # Per-element changes happen henceforth
     for element in window.element_list():
         if element.key in whitelist:
 
@@ -380,28 +409,15 @@
                 element.widget.configure(background=new_theme_dict['BACKGROUND'])
 
             # Declare a styler object.
             styler = Style()
 
             # Right Click Menus (thanks for pointing this out @dwelden!)
             if element.TKRightClickMenu:
-                element.ParentForm.right_click_menu_background_color = new_theme_dict['INPUT']
-                element.ParentForm.right_click_menu_text_color = new_theme_dict['TEXT_INPUT']
-                element.ParentForm.right_click_menu_disabled_color = DISABLED_COLOR
-                element.ParentForm.right_click_menu_selected_colors = (
-                    new_theme_dict['INPUT'], new_theme_dict['TEXT_INPUT']
-                )
-                element.set_right_click_menu(element.RightClickMenu)
-                # We were never here...
-                element.ParentForm.right_click_menu_background_color = old_theme_dict['INPUT']
-                element.ParentForm.right_click_menu_text_color = old_theme_dict['TEXT_INPUT']
-                element.ParentForm.right_click_menu_disabled_color = DISABLED_COLOR
-                element.ParentForm.right_click_menu_selected_colors = (
-                    old_theme_dict['INPUT'], old_theme_dict['TEXT_INPUT']
-                )
+                _recurse_menu(element.TKRightClickMenu, new_theme_dict['TEXT_INPUT'], new_theme_dict['INPUT'])
 
             # Handling ttk scrollbars
             if hasattr(element, 'ttk_style_name'):
                 _configure_ttk_scrollbar_style(element.ttk_style_name, styler, new_theme_dict)
 
             # Elements _________________________________________________________________________________________________
             # Custom Titlebar
@@ -412,15 +428,15 @@
                 titlebar_row_frame = str(element.ParentRowFrame)
                 continue
 
             # Titlebar elements
             if str(element.widget).startswith(titlebar_row_frame+'.'):
                 element.ParentRowFrame.configure(background=new_theme_dict['BUTTON'][1])
                 element.widget.configure(background=new_theme_dict['BUTTON'][1])
-                if el in ('image', 'text'):
+                if 'foreground' in element.widget.keys():
                     element.widget.configure(foreground=new_theme_dict['BUTTON'][0])
                 continue
 
             if el in ('text', 'statusbar'):
                 text_fg = element.widget.cget('foreground')
                 text_bg = element.widget.cget('background')
                 if _check_for_honors(text_fg, old_theme_dict['TEXT'], honor_previous):
@@ -436,18 +452,17 @@
                 continue
 
             elif el == 'frame':
                 element.widget.configure(foreground=new_theme_dict['TEXT'])
                 continue
 
             elif el == 'menu':
-                element.BackgroundColor = new_theme_dict['INPUT']
-                element.TextColor = new_theme_dict['TEXT_INPUT']
-                menudef = getattr(element, 'MenuDefinition')
-                element.update(menu_definition=menudef)
+                _recurse_menu(element.widget, new_theme_dict['TEXT_INPUT'], new_theme_dict['INPUT'])
+                # menudef = getattr(element, 'MenuDefinition')
+                # element.update(menu_definition=menudef)
                 continue
 
             elif el == 'sizegrip':
                 sizegrip_style = element.widget.cget('style')
                 styler.configure(sizegrip_style, background=new_theme_dict['BACKGROUND'])
                 continue
 
@@ -486,15 +501,14 @@
                 continue
 
             elif el == 'slider':
                 element.widget.configure(foreground=new_theme_dict['TEXT'], troughcolor=new_theme_dict['SCROLL'])
                 continue
 
             elif el == 'button':
-                element.ButtonColor = new_theme_dict['BUTTON']
                 # For regular Tk buttons
                 if 'ttk' not in str(type(getattr(element, 'TKButton'))).lower():
                     element.widget.configure(
                         background=new_theme_dict['BUTTON'][1],
                         foreground=new_theme_dict['BUTTON'][0],
                         activebackground=new_theme_dict['BUTTON'][0],
                         activeforeground=new_theme_dict['BUTTON'][1]
@@ -524,25 +538,19 @@
                 style_name = getattr(element, 'TKProgressBar').style_name
                 styler.configure(
                     style_name, background=new_theme_dict['PROGRESS'][1],
                     troughcolor=new_theme_dict['PROGRESS'][0])
                 continue
 
             elif el == 'buttonmenu':
-                menudef = getattr(element, 'MenuDefinition')
-                element.BackgroundColor = new_theme_dict['INPUT']
-                element.TextColor = new_theme_dict['TEXT_INPUT']
                 element.widget.configure(
                     background=new_theme_dict['BUTTON'][1],
                     foreground=new_theme_dict['BUTTON'][0]
                 )
-                element.update(menu_definition=menudef)
-                # We were never here.
-                element.BackgroundColor = old_theme_dict['INPUT']
-                element.TextColor = old_theme_dict['TEXT_INPUT']
+                _recurse_menu(element.TKMenu, fg=new_theme_dict['TEXT_INPUT'], bg=new_theme_dict['INPUT'])
                 continue
 
             elif el in 'spin':
                 element.widget.configure(
                     background=new_theme_dict['INPUT'],
                     foreground=new_theme_dict['TEXT_INPUT'],
                     buttonbackground=new_theme_dict['INPUT']
@@ -741,16 +749,16 @@
                        exempt_element_keys, target_element_keys, honor_previous, reskin_background)
             except TclError:  # The window has been closed.
                 pass
         """
         End of animation reached.
 
         Due to smaller, more precise time-based delta (duration progress per frame) increments, and the condition for 
-        checking if the animation should end being based on (ultimately imprecise) time comparisons, delta never actually 
-        reaches 1, hence the interpolation will not end exactly at the new theme's colors (the destination). 
+        checking if the animation should end being based on (ultimately imprecise) time comparisons, delta never 
+        actually reaches 1, hence the interpolation will not end exactly at the new theme's colors (the destination). 
 
         Rather, it will end at a value as close as the time comparison permits (which is extremely close to the actual 
         destination), then skip to the destination itself.
 
         The effect of the skip is almost unnoticeable, and the end user probably wouldn't even know, but it's there ;).
 
         Hope that explains the animation process.
@@ -761,15 +769,17 @@
                    target_element_keys, honor_previous, reskin_background)
         except TclError:  # The window has been closed.
             pass
 
     except Exception as e:
         # Basically provide more context to whatever error occurs.
         print(
-            f'While trying to perform an animated reskin from {WINDOW_THEME_MAP[window][0]} to {new_theme}, an exception occurred:')
+            f'While trying to perform an animated reskin from {WINDOW_THEME_MAP[window][0]} to {new_theme}, an '
+            f'exception occurred:'
+        )
         raise e
 
 
 def toggle_transparency(window: Window) -> None:
     """
     Use this function to toggle background transparency on or off. Works with reskinned and non-reskinned windows.
 
@@ -794,19 +804,19 @@
     """
     Main Function.
 
     Gets called when the module is run instead of imported.
 
     First available from v1.0.0.
     """
-    # from psg_reskinner import reskin, animated_reskin, __version__
-    from PySimpleGUI import Window, Text, Button, Push, Titlebar, theme_list, theme, LOOK_AND_FEEL_TABLE, TIMEOUT_KEY
-    # from random import choice as rc
+    from psg_reskinner import reskin, animated_reskin, __version__
+    from PySimpleGUI import Window, Text, Button, Push, Titlebar, theme, LOOK_AND_FEEL_TABLE, TIMEOUT_KEY
+    from random import choice as rc
 
-    rmenu = ['', ['Hi', 'There']]
+    rmenu = ['', [['Hi', ['Next Level', ['Deeper Level', ['a', 'b', 'c']], 'Hoho']], 'There']]
 
     window_layout = [
         [Titlebar('Reskinner Demo')],
         [Text('Hello!', font=('Helvetica', 20))],
         [Text('You are currently running Reskinner instead of importing it.')],
         [Text('The theme of this window changes every 3 seconds.')],
         [Text('Changing to:')],
```

### Comparing `psg_reskinner-2.3.7/psg_reskinner.egg-info/PKG-INFO` & `psg_reskinner-2.3.8/psg_reskinner.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: psg-reskinner
-Version: 2.3.7
+Version: 2.3.8
 Summary: Instantaneous theme changing for PySimpleGUI windows.
-Home-page: https://github.com/definite-d/psg_reskinner/
-Author: Divine U. Afam-Ifediogor
 Author-email: "Divine U. Afam-Ifediogor" <divineafam@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Divine Afam-Ifediogor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `psg_reskinner-2.3.7/pyproject.toml` & `psg_reskinner-2.3.8/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,51 @@
 [build-system]
-requires = ["setuptools>=61.0.0", "wheel"]
+requires = ["setuptools>=61.0.0", "wheel", "bumpver"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "psg_reskinner"
-dynamic = ["version"]
 description = "Instantaneous theme changing for PySimpleGUI windows."
+version = "2.3.8"
 readme = "DESCRIPTION.md"
 authors = [{ name = "Divine U. Afam-Ifediogor", email = "divineafam@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers=[
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
 ]
 keywords = ["PySimpleGUI", "reskin", "realtime", "theme", "color"]
 dependencies = [
-    "PySimpleGUI >= 4.60.3.96",
-    "colour"
+    "colour>=0.1.5",
+    "PySimpleGUI>=4.60.3.96"
 ]
 requires-python = ">=3.6"
 
 [project.urls]
 "Homepage" = "https://github.com/definite-d/psg_reskinner/"
 "Bug Tracker" = "https://github.com/definite-d/psg_reskinner/issues/"
 
-[tool.setuptools.dynamic]
-version = {attr = "psg_reskinner.__version__"}
-
 [tool.setuptools]
 packages = ["psg_reskinner"]
 
+[tool.bumpver]
+current_version = "2.3.8"
+version_pattern = "MAJOR.MINOR.PATCH"
+commit_message = "New {new_version} update from {old_version}"
+commit = true
+tag = true
+push = true
+
+[tool.bumpver.file_patterns]
+"pyproject.toml" = [
+    'current_version = "{version}"',
+    'version = "{version}"',
+]
+"README.md" = [
+    "Version {version}",
+]
+"psg_reskinner/__main__.py" = [
+    "__version__: str = '{version}'"
+]
+
```

