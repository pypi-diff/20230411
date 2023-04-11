# Comparing `tmp/aiogram-tools-0.5.tar.gz` & `tmp/aiogram-tools-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram-tools-0.5.tar", last modified: Tue Jun 15 12:50:56 2021, max compression
+gzip compressed data, was "aiogram-tools-1.0.0.tar", last modified: Tue Apr 11 11:45:15 2023, max compression
```

## Comparing `aiogram-tools-0.5.tar` & `aiogram-tools-1.0.0.tar`

### file list

```diff
@@ -1,34 +1,19 @@
-drwxrwxrwx   0        0        0        0 2021-06-15 12:50:56.364813 aiogram-tools-0.5/
--rw-rw-rw-   0        0        0     1070 2021-03-02 21:45:20.000000 aiogram-tools-0.5/LICENSE
--rw-rw-rw-   0        0        0      588 2021-06-15 12:50:56.364813 aiogram-tools-0.5/PKG-INFO
--rw-rw-rw-   0        0        0        8 2021-03-02 21:21:05.000000 aiogram-tools-0.5/README.md
-drwxrwxrwx   0        0        0        0 2021-06-15 12:50:56.294077 aiogram-tools-0.5/aiogram_tools/
--rw-rw-rw-   0        0        0      227 2021-04-08 14:31:46.000000 aiogram-tools-0.5/aiogram_tools/__init__.py
--rw-rw-rw-   0        0        0     3041 2021-04-17 12:34:00.000000 aiogram-tools-0.5/aiogram_tools/_bot.py
--rw-rw-rw-   0        0        0     6412 2021-06-15 12:50:19.000000 aiogram-tools-0.5/aiogram_tools/_currents.py
--rw-rw-rw-   0        0        0     1437 2021-06-15 12:50:19.000000 aiogram-tools-0.5/aiogram_tools/_inline_keyboard.py
--rw-rw-rw-   0        0        0     2101 2021-06-15 12:50:19.000000 aiogram-tools-0.5/aiogram_tools/_models.py
--rw-rw-rw-   0        0        0     2289 2021-04-08 13:20:26.000000 aiogram-tools-0.5/aiogram_tools/_questions.py
--rw-rw-rw-   0        0        0     5410 2021-06-15 12:50:19.000000 aiogram-tools-0.5/aiogram_tools/_states.py
--rw-rw-rw-   0        0        0     1586 2021-06-15 12:50:19.000000 aiogram-tools-0.5/aiogram_tools/context.py
--rw-rw-rw-   0        0        0     9486 2021-06-15 12:50:19.000000 aiogram-tools-0.5/aiogram_tools/dispatcher.py
--rw-rw-rw-   0        0        0     3733 2021-06-15 12:50:19.000000 aiogram-tools-0.5/aiogram_tools/filters.py
--rw-rw-rw-   0        0        0     2122 2021-04-08 14:31:46.000000 aiogram-tools-0.5/aiogram_tools/keyboards.py
-drwxrwxrwx   0        0        0        0 2021-06-15 12:50:56.353820 aiogram-tools-0.5/aiogram_tools/middlewares/
--rw-rw-rw-   0        0        0      158 2021-04-08 14:03:42.000000 aiogram-tools-0.5/aiogram_tools/middlewares/__init__.py
--rw-rw-rw-   0        0        0     6923 2021-04-08 13:20:26.000000 aiogram-tools-0.5/aiogram_tools/middlewares/_conversation.py
--rw-rw-rw-   0        0        0     1534 2021-06-15 12:50:19.000000 aiogram-tools-0.5/aiogram_tools/middlewares/_membership.py
--rw-rw-rw-   0        0        0     1487 2021-06-15 12:50:19.000000 aiogram-tools-0.5/aiogram_tools/middlewares/misc.py
--rw-rw-rw-   0        0        0     2079 2021-06-15 12:50:19.000000 aiogram-tools-0.5/aiogram_tools/middlewares/throttling.py
-drwxrwxrwx   0        0        0        0 2021-06-15 12:50:56.339729 aiogram-tools-0.5/aiogram_tools.egg-info/
--rw-rw-rw-   0        0        0      588 2021-06-15 12:50:56.000000 aiogram-tools-0.5/aiogram_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      758 2021-06-15 12:50:56.000000 aiogram-tools-0.5/aiogram_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-06-15 12:50:56.000000 aiogram-tools-0.5/aiogram_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2021-06-15 12:50:56.000000 aiogram-tools-0.5/aiogram_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2021-06-15 12:50:56.000000 aiogram-tools-0.5/aiogram_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      597 2021-06-15 12:50:56.367812 aiogram-tools-0.5/setup.cfg
--rw-rw-rw-   0        0        0      117 2021-04-18 15:40:33.000000 aiogram-tools-0.5/setup.py
-drwxrwxrwx   0        0        0        0 2021-06-15 12:50:56.361815 aiogram-tools-0.5/tests/
--rw-rw-rw-   0        0        0        0 2021-04-16 10:12:43.000000 aiogram-tools-0.5/tests/__init__.py
--rw-rw-rw-   0        0        0      143 2021-04-17 04:34:52.000000 aiogram-tools-0.5/tests/config.py
--rw-rw-rw-   0        0        0      314 2021-04-29 21:18:08.000000 aiogram-tools-0.5/tests/loader.py
+-rw-r--r--   0        0        0      190 2023-04-11 11:42:09.781868 aiogram-tools-1.0.0/aiogram_tools/__init__.py
+-rw-r--r--   0        0        0     3041 2023-04-11 10:54:36.147201 aiogram-tools-1.0.0/aiogram_tools/_bot.py
+-rw-r--r--   0        0        0     6412 2023-04-11 10:54:36.147201 aiogram-tools-1.0.0/aiogram_tools/_currents.py
+-rw-r--r--   0        0        0     1475 2023-04-11 10:54:36.147201 aiogram-tools-1.0.0/aiogram_tools/_inline_keyboard.py
+-rw-r--r--   0        0        0     2101 2023-04-11 10:54:36.148209 aiogram-tools-1.0.0/aiogram_tools/_models.py
+-rw-r--r--   0        0        0     2289 2023-04-11 10:54:36.148209 aiogram-tools-1.0.0/aiogram_tools/_questions.py
+-rw-r--r--   0        0        0     5410 2023-04-11 10:54:36.148209 aiogram-tools-1.0.0/aiogram_tools/_states.py
+-rw-r--r--   0        0        0     1586 2023-04-11 10:54:36.148209 aiogram-tools-1.0.0/aiogram_tools/context.py
+-rw-r--r--   0        0        0     5245 2023-04-11 11:36:47.149746 aiogram-tools-1.0.0/aiogram_tools/dispatcher.py
+-rw-r--r--   0        0        0     3748 2023-04-11 11:36:47.165780 aiogram-tools-1.0.0/aiogram_tools/filters.py
+-rw-r--r--   0        0        0     2026 2023-04-11 11:42:09.798989 aiogram-tools-1.0.0/aiogram_tools/keyboards.py
+-rw-r--r--   0        0        0      158 2023-04-11 10:54:36.149502 aiogram-tools-1.0.0/aiogram_tools/middlewares/__init__.py
+-rw-r--r--   0        0        0     6923 2023-04-11 10:54:36.149502 aiogram-tools-1.0.0/aiogram_tools/middlewares/_conversation.py
+-rw-r--r--   0        0        0     1534 2023-04-11 10:54:36.150546 aiogram-tools-1.0.0/aiogram_tools/middlewares/_membership.py
+-rw-r--r--   0        0        0     1487 2023-04-11 10:54:36.150546 aiogram-tools-1.0.0/aiogram_tools/middlewares/misc.py
+-rw-r--r--   0        0        0     2079 2023-04-11 10:54:36.150546 aiogram-tools-1.0.0/aiogram_tools/middlewares/throttling.py
+-rw-r--r--   0        0        0      302 2023-04-11 11:31:53.786647 aiogram-tools-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-04-11 11:28:20.640417 aiogram-tools-1.0.0/README.md
+-rw-r--r--   0        0        0      154 1970-01-01 00:00:00.000000 aiogram-tools-1.0.0/PKG-INFO
```

### Comparing `aiogram-tools-0.5/aiogram_tools/_bot.py` & `aiogram-tools-1.0.0/aiogram_tools/_bot.py`

 * *Files identical despite different names*

### Comparing `aiogram-tools-0.5/aiogram_tools/_currents.py` & `aiogram-tools-1.0.0/aiogram_tools/_currents.py`

 * *Files identical despite different names*

### Comparing `aiogram-tools-0.5/aiogram_tools/_inline_keyboard.py` & `aiogram-tools-1.0.0/aiogram_tools/_inline_keyboard.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from __future__ import annotations
-
-from aiogram.types import InlineKeyboardMarkup, InlineKeyboardButton
-from aiogram.utils.helper import Item, Helper
-
-
-class InlineKeyboard(InlineKeyboardMarkup, Helper):
-    DATA_ROWS: list[Item, tuple[Item]] = []
-
-    def __init__(self, cdata_and_text: dict[str, str] = None, row_width=2):
-        """Buttons in format: {callback_data:text} for DATA_ROWS."""
-        super().__init__(row_width)
-
-        if cdata_and_text:
-            buttons = {cdata.upper(): text for cdata, text in cdata_and_text.items() if text}
-        else:
-            buttons = {}
-
-        for data_row in self.data_rows:
-            btn_row = self.make_buttons_row(data_row, buttons)
-            self.row(*btn_row)
-
-    @property
-    def data_rows(self) -> list[list[str]]:
-        return [self._to_values_list(row) for row in self.DATA_ROWS]
-
-    def make_buttons_row(self, data_row: list[str], buttons: dict) -> list[InlineKeyboardButton]:
-        return [self._make_data_button(cdata, buttons) for cdata in data_row if cdata in buttons]
-
-    @staticmethod
-    def _to_values_list(data_row: str or tuple[str]) -> list[str]:
-        if not isinstance(data_row, tuple):
-            data_row = (data_row,)
-        return [button.value for button in data_row]
-
-    @staticmethod
-    def _make_data_button(data: str, _locals: dict) -> InlineKeyboardButton:
-        return InlineKeyboardButton(_locals[data], callback_data=data)
+from __future__ import annotations
+
+from aiogram.types import InlineKeyboardMarkup, InlineKeyboardButton
+from aiogram.utils.helper import Item, Helper
+
+
+class InlineKeyboard(InlineKeyboardMarkup, Helper):
+    DATA_ROWS: list[Item, tuple[Item]] = []
+
+    def __init__(self, cdata_and_text: dict[str, str] = None, row_width=2):
+        """Buttons in format: {callback_data:text} for DATA_ROWS."""
+        super().__init__(row_width)
+
+        if cdata_and_text:
+            buttons = {cdata.upper(): text for cdata, text in cdata_and_text.items() if text}
+        else:
+            buttons = {}
+
+        for data_row in self.data_rows:
+            btn_row = self.make_buttons_row(data_row, buttons)
+            self.row(*btn_row)
+
+    @property
+    def data_rows(self) -> list[list[str]]:
+        return [self._to_values_list(row) for row in self.DATA_ROWS]
+
+    def make_buttons_row(self, data_row: list[str], buttons: dict) -> list[InlineKeyboardButton]:
+        return [self._make_data_button(cdata, buttons) for cdata in data_row if cdata in buttons]
+
+    @staticmethod
+    def _to_values_list(data_row: str or tuple[str]) -> list[str]:
+        if not isinstance(data_row, tuple):
+            data_row = (data_row,)
+        return [button.value for button in data_row]
+
+    @staticmethod
+    def _make_data_button(data: str, _locals: dict) -> InlineKeyboardButton:
+        return InlineKeyboardButton(_locals[data], callback_data=data)
```

### Comparing `aiogram-tools-0.5/aiogram_tools/_models.py` & `aiogram-tools-1.0.0/aiogram_tools/_models.py`

 * *Files identical despite different names*

### Comparing `aiogram-tools-0.5/aiogram_tools/_questions.py` & `aiogram-tools-1.0.0/aiogram_tools/_questions.py`

 * *Files identical despite different names*

### Comparing `aiogram-tools-0.5/aiogram_tools/_states.py` & `aiogram-tools-1.0.0/aiogram_tools/_states.py`

 * *Files identical despite different names*

### Comparing `aiogram-tools-0.5/aiogram_tools/context.py` & `aiogram-tools-1.0.0/aiogram_tools/context.py`

 * *Files identical despite different names*

### Comparing `aiogram-tools-0.5/aiogram_tools/filters.py` & `aiogram-tools-1.0.0/aiogram_tools/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     @abstractmethod
     def cast_update(self, obj):
         """Cast update-obj to string for matching"""
 
     @staticmethod
     def make_regexp(text: str):
-        return re.sub(r'{(.+?)}', r'(?P<\1>.+)', text)
+        return re.sub(r"\\{(.+?)\\}", r"(?P<\1>.+)", re.escape(text))
 
     def __init__(self, button):
         buttons_regexps = []
         if not isinstance(button, (list, tuple, set)):
             button = [button]
 
         for item in button:
```

### Comparing `aiogram-tools-0.5/aiogram_tools/keyboards.py` & `aiogram-tools-1.0.0/aiogram_tools/keyboards.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,32 +9,30 @@
 DEEPLINK_BASE = 'https://t.me/{bot_username}?start={start_param}'
 
 
 def _get_bot_username() -> Optional[str]:
     bot = Bot.get_current()
     try:
         return getattr(getattr(bot, '_me'), 'username')
-    except:
+    except AttributeError:
         raise RuntimeError("Can't get bot username for deeplink")
 
 
 Button = KeyboardButton
 
 
 class InlineButton(InlineKeyboardButton):
-    def __init__(self, text: str,
-                 callback: Union[str, bool] = None,
-                 url: Union[str, bool] = None,
-                 start_param: Union[str, bool] = None,
-                 switch_iquery: Union[str, bool] = None,
-                 switch_iquery_current: Union[str, bool] = None,
-                 ):
-
-        # TODO: validation
-
+    def __init__(
+            self, text: str,
+            callback: Union[str, bool] = None,
+            url: Union[str, bool] = None,
+            start_param: Union[str, bool] = None,
+            switch_iquery: Union[str, bool] = None,
+            switch_iquery_current: Union[str, bool] = None,
+    ):
         # update args
         if url is True:
             url = text
         elif start_param is True:
             start_param = text
         elif callback is True:
             callback = text
@@ -44,20 +42,21 @@
             switch_iquery_current = text
 
         # cast start_param to url
         if start_param:
             bot_username = _get_bot_username()
             url = DEEPLINK_BASE.format(bot_username=bot_username, start_param=start_param)
 
-        super().__init__(text,
-                         url=url,
-                         callback_data=callback,
-                         switch_inline_query=switch_iquery,
-                         switch_inline_query_current_chat=switch_iquery_current,
-                         )
+        super().__init__(
+            text,
+            url=url,
+            callback_data=callback,
+            switch_inline_query=switch_iquery,
+            switch_inline_query_current_chat=switch_iquery_current,
+        )
 
     def format(self, *args, **kwargs) -> InlineButton:
         """Return new button with formatted values."""
         new_button = deepcopy(self)
 
         for item, value in new_button.values.items():
             if isinstance(value, str):
```

### Comparing `aiogram-tools-0.5/aiogram_tools/middlewares/_conversation.py` & `aiogram-tools-1.0.0/aiogram_tools/middlewares/_conversation.py`

 * *Files identical despite different names*

### Comparing `aiogram-tools-0.5/aiogram_tools/middlewares/_membership.py` & `aiogram-tools-1.0.0/aiogram_tools/middlewares/_membership.py`

 * *Files identical despite different names*

### Comparing `aiogram-tools-0.5/aiogram_tools/middlewares/misc.py` & `aiogram-tools-1.0.0/aiogram_tools/middlewares/misc.py`

 * *Files identical despite different names*

### Comparing `aiogram-tools-0.5/aiogram_tools/middlewares/throttling.py` & `aiogram-tools-1.0.0/aiogram_tools/middlewares/throttling.py`

 * *Files identical despite different names*

