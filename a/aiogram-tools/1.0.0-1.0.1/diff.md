# Comparing `tmp/aiogram-tools-1.0.0.tar.gz` & `tmp/aiogram-tools-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram-tools-1.0.0.tar", last modified: Tue Apr 11 11:45:15 2023, max compression
+gzip compressed data, was "aiogram-tools-1.0.1.tar", last modified: Tue Apr 11 12:11:30 2023, max compression
```

## Comparing `aiogram-tools-1.0.0.tar` & `aiogram-tools-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0      190 2023-04-11 11:42:09.781868 aiogram-tools-1.0.0/aiogram_tools/__init__.py
--rw-r--r--   0        0        0     3041 2023-04-11 10:54:36.147201 aiogram-tools-1.0.0/aiogram_tools/_bot.py
--rw-r--r--   0        0        0     6412 2023-04-11 10:54:36.147201 aiogram-tools-1.0.0/aiogram_tools/_currents.py
--rw-r--r--   0        0        0     1475 2023-04-11 10:54:36.147201 aiogram-tools-1.0.0/aiogram_tools/_inline_keyboard.py
--rw-r--r--   0        0        0     2101 2023-04-11 10:54:36.148209 aiogram-tools-1.0.0/aiogram_tools/_models.py
--rw-r--r--   0        0        0     2289 2023-04-11 10:54:36.148209 aiogram-tools-1.0.0/aiogram_tools/_questions.py
--rw-r--r--   0        0        0     5410 2023-04-11 10:54:36.148209 aiogram-tools-1.0.0/aiogram_tools/_states.py
--rw-r--r--   0        0        0     1586 2023-04-11 10:54:36.148209 aiogram-tools-1.0.0/aiogram_tools/context.py
--rw-r--r--   0        0        0     5245 2023-04-11 11:36:47.149746 aiogram-tools-1.0.0/aiogram_tools/dispatcher.py
--rw-r--r--   0        0        0     3748 2023-04-11 11:36:47.165780 aiogram-tools-1.0.0/aiogram_tools/filters.py
--rw-r--r--   0        0        0     2026 2023-04-11 11:42:09.798989 aiogram-tools-1.0.0/aiogram_tools/keyboards.py
--rw-r--r--   0        0        0      158 2023-04-11 10:54:36.149502 aiogram-tools-1.0.0/aiogram_tools/middlewares/__init__.py
--rw-r--r--   0        0        0     6923 2023-04-11 10:54:36.149502 aiogram-tools-1.0.0/aiogram_tools/middlewares/_conversation.py
--rw-r--r--   0        0        0     1534 2023-04-11 10:54:36.150546 aiogram-tools-1.0.0/aiogram_tools/middlewares/_membership.py
--rw-r--r--   0        0        0     1487 2023-04-11 10:54:36.150546 aiogram-tools-1.0.0/aiogram_tools/middlewares/misc.py
--rw-r--r--   0        0        0     2079 2023-04-11 10:54:36.150546 aiogram-tools-1.0.0/aiogram_tools/middlewares/throttling.py
--rw-r--r--   0        0        0      302 2023-04-11 11:31:53.786647 aiogram-tools-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       21 2023-04-11 11:28:20.640417 aiogram-tools-1.0.0/README.md
--rw-r--r--   0        0        0      154 1970-01-01 00:00:00.000000 aiogram-tools-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      232 2023-04-11 11:58:04.206246 aiogram-tools-1.0.1/aiogram_tools/__init__.py
+-rw-r--r--   0        0        0     3007 2023-04-11 11:53:07.691383 aiogram-tools-1.0.1/aiogram_tools/_bot.py
+-rw-r--r--   0        0        0     6470 2023-04-11 11:53:07.739292 aiogram-tools-1.0.1/aiogram_tools/_currents.py
+-rw-r--r--   0        0        0     1573 2023-04-11 11:53:07.617772 aiogram-tools-1.0.1/aiogram_tools/_inline_keyboard.py
+-rw-r--r--   0        0        0     2099 2023-04-11 11:53:07.649026 aiogram-tools-1.0.1/aiogram_tools/_models.py
+-rw-r--r--   0        0        0     2293 2023-04-11 11:53:07.649026 aiogram-tools-1.0.1/aiogram_tools/_questions.py
+-rw-r--r--   0        0        0     5406 2023-04-11 11:53:07.707408 aiogram-tools-1.0.1/aiogram_tools/_states.py
+-rw-r--r--   0        0        0     1665 2023-04-11 12:03:57.675683 aiogram-tools-1.0.1/aiogram_tools/context.py
+-rw-r--r--   0        0        0      965 2023-04-11 12:07:22.049542 aiogram-tools-1.0.1/aiogram_tools/deps.py
+-rw-r--r--   0        0        0     5382 2023-04-11 12:09:03.428321 aiogram-tools-1.0.1/aiogram_tools/dispatcher.py
+-rw-r--r--   0        0        0     3800 2023-04-11 11:53:07.707408 aiogram-tools-1.0.1/aiogram_tools/filters.py
+-rw-r--r--   0        0        0     2353 2023-04-11 12:03:57.691475 aiogram-tools-1.0.1/aiogram_tools/keyboards.py
+-rw-r--r--   0        0        0      158 2023-04-11 10:54:36.149502 aiogram-tools-1.0.1/aiogram_tools/middlewares/__init__.py
+-rw-r--r--   0        0        0     6987 2023-04-11 11:53:07.723527 aiogram-tools-1.0.1/aiogram_tools/middlewares/_conversation.py
+-rw-r--r--   0        0        0     1534 2023-04-11 11:53:07.675758 aiogram-tools-1.0.1/aiogram_tools/middlewares/_membership.py
+-rw-r--r--   0        0        0     1503 2023-04-11 11:53:07.675758 aiogram-tools-1.0.1/aiogram_tools/middlewares/misc.py
+-rw-r--r--   0        0        0     2178 2023-04-11 11:53:07.691383 aiogram-tools-1.0.1/aiogram_tools/middlewares/throttling.py
+-rw-r--r--   0        0        0      302 2023-04-11 12:11:20.490057 aiogram-tools-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-04-11 11:28:20.640417 aiogram-tools-1.0.1/README.md
+-rw-r--r--   0        0        0      154 1970-01-01 00:00:00.000000 aiogram-tools-1.0.1/PKG-INFO
```

### Comparing `aiogram-tools-1.0.0/aiogram_tools/_bot.py` & `aiogram-tools-1.0.1/aiogram_tools/_bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 from aiogram import Bot as _Bot
 from aiogram.bot.base import TelegramAPIServer, aiohttp, TELEGRAM_PRODUCTION
 from aiogram.types import base
 from pyrogram import Client, raw
 
 
 class Userbot:
-
-    def __init__(self, api_id: int, api_hash: str, session_name='aiogram_data/bound_userbot'):
-        for folder in ['aiogram_data']:
+    def __init__(
+        self, api_id: int, api_hash: str, session_name="aiogram_data/bound_userbot"
+    ):
+        for folder in ["aiogram_data"]:
             if not os.path.exists(folder):
                 os.mkdir(folder)
 
         self._client = Client(session_name, api_id, api_hash)
 
     @property
     async def client(self) -> Client:
@@ -26,18 +27,18 @@
         return self._client
 
     async def stop_client(self):
         if self._client.is_connected:
             await self._client.stop()
 
     async def create_group(
-            self,
-            title: str,
-            bound_bot: Union[int, str],
-            other_users: Union[Union[int, str], list[Union[int, str]]]
+        self,
+        title: str,
+        bound_bot: Union[int, str],
+        other_users: Union[Union[int, str], list[Union[int, str]]],
     ):
         client = await self.client
 
         if not isinstance(other_users, list):
             other_users = [other_users]
 
         other_users.append(bound_bot)
@@ -45,34 +46,33 @@
 
         peer = await client.resolve_peer(new_group.id)
 
         await client.send(
             raw.functions.messages.EditChatAdmin(
                 chat_id=peer.chat_id,
                 user_id=await client.resolve_peer(bound_bot),
-                is_admin=True
+                is_admin=True,
             )
         )
 
 
 class Bot(_Bot):
-
     def __init__(
-            self,
-            token: base.String,
-            loop: Union[asyncio.BaseEventLoop, asyncio.AbstractEventLoop, None] = None,
-            connections_limit: Optional[base.Integer] = None,
-            proxy: Optional[base.String] = None,
-            proxy_auth: Optional[aiohttp.BasicAuth] = None,
-            validate_token: Optional[base.Boolean] = True,
-            parse_mode: Optional[base.String] = None,
-            timeout: Union[base.Integer, base.Float, aiohttp.ClientTimeout, None] = None,
-            server: TelegramAPIServer = TELEGRAM_PRODUCTION,
-            bound_userbot_api_id: Optional[int] = None,
-            bound_userbot_api_hash: Optional[str] = None,
+        self,
+        token: base.String,
+        loop: Union[asyncio.BaseEventLoop, asyncio.AbstractEventLoop, None] = None,
+        connections_limit: Optional[base.Integer] = None,
+        proxy: Optional[base.String] = None,
+        proxy_auth: Optional[aiohttp.BasicAuth] = None,
+        validate_token: Optional[base.Boolean] = True,
+        parse_mode: Optional[base.String] = None,
+        timeout: Union[base.Integer, base.Float, aiohttp.ClientTimeout, None] = None,
+        server: TelegramAPIServer = TELEGRAM_PRODUCTION,
+        bound_userbot_api_id: Optional[int] = None,
+        bound_userbot_api_hash: Optional[str] = None,
     ):
         super().__init__(
             token=token,
             loop=loop,
             connections_limit=connections_limit,
             proxy=proxy,
             proxy_auth=proxy_auth,
@@ -80,11 +80,13 @@
             parse_mode=parse_mode,
             timeout=timeout,
             server=server,
         )
 
         self.bound_userbot = Userbot(bound_userbot_api_id, bound_userbot_api_hash)
 
-    async def create_group(self, title: str, users: Union[Union[int, str], list[Union[int, str]]] = None):
+    async def create_group(
+        self, title: str, users: Union[Union[int, str], list[Union[int, str]]] = None
+    ):
         users = users or []
         bound_bot_username = (await self.me).username
         await self.bound_userbot.create_group(title, bound_bot_username, users)
```

### Comparing `aiogram-tools-1.0.0/aiogram_tools/_currents.py` & `aiogram-tools-1.0.1/aiogram_tools/_currents.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Optional, Any, Awaitable, Callable
 
 from aiogram import types, Dispatcher as Dispatcher, Bot as Bot
 from aiogram.utils.mixins import ContextInstanceMixin
 
 from aiogram_tools._states import State, StatesGroup2
 
-__all__ = ['CurrentObjects']
+__all__ = ["CurrentObjects"]
 
 
 async def get_udata(obj: Dispatcher) -> dict:
     try:
         return await obj.current_state().get_data()
     except AttributeError:
         return {}
@@ -26,16 +26,17 @@
 
 
 async def get_state(obj: Dispatcher) -> Optional[State]:
     return await StatesGroup2.get_current_state()
 
 
 class ContextObj:
-
-    def __init__(self, ctx_type: type[ContextInstanceMixin], get_target: callable = lambda x: x):
+    def __init__(
+        self, ctx_type: type[ContextInstanceMixin], get_target: callable = lambda x: x
+    ):
         self.ctx_type = ctx_type
         self.get_target = get_target
 
     async def get_current(self) -> Optional[Any]:
         try:
             obj = self.ctx_type.get_current()
 
@@ -44,21 +45,22 @@
                 target = await target
 
             return target
         except AttributeError:
             return None
 
     def __repr__(self):
-        return f'{type(self).__name__}(type={self.ctx_type.__name__}, target={self.get_target.__name__})'
+        return f"{type(self).__name__}(type={self.ctx_type.__name__}, target={self.get_target.__name__})"
 
 
 class CurrentObjects:
     """Context telegram objects and derivatives.
     You can specify own objects and aliases at runtime.
     """
+
     bot = ContextObj(Bot)
     dp = ContextObj(Dispatcher)
     update = ContextObj(types.Update)
     msg = ContextObj(types.Message)
     user = ContextObj(types.User)
     chat = ContextObj(types.Chat)
     query = ContextObj(types.CallbackQuery)
@@ -121,15 +123,20 @@
         return await obj.get_current()
 
     @classmethod
     def set_alias(cls, ctx_obj: str, alias: str):
         setattr(cls, alias, getattr(cls, ctx_obj))
 
     @classmethod
-    def set_ctx_obj(cls, name: str, ctx_obj: type[ContextInstanceMixin], get_target: callable = lambda x: x):
+    def set_ctx_obj(
+        cls,
+        name: str,
+        ctx_obj: type[ContextInstanceMixin],
+        get_target: callable = lambda x: x,
+    ):
         setattr(cls, name, ContextObj(ctx_obj, get_target))
 
     @classmethod
     def decorate_handler(cls, handler) -> callable:
         """Now handler will receive current objects only according it's signature."""
 
         @functools.wraps(handler)
@@ -152,15 +159,14 @@
 
     @classmethod
     def decorate(cls, func) -> Callable[..., Awaitable]:
         """Now func will receive current objects for missing args (kwargs only)."""
 
         @functools.wraps(func)
         async def wrapper(*args, **kwargs):
-
             spec_kwargs = inspect.getfullargspec(func).kwonlyargs
 
             for arg in spec_kwargs:
                 if arg not in kwargs:
                     if arg in cls.keywords:
                         kwargs[arg] = await cls.get(arg)
```

### Comparing `aiogram-tools-1.0.0/aiogram_tools/_inline_keyboard.py` & `aiogram-tools-1.0.1/aiogram_tools/_inline_keyboard.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,28 +8,36 @@
     DATA_ROWS: list[Item, tuple[Item]] = []
 
     def __init__(self, cdata_and_text: dict[str, str] = None, row_width=2):
         """Buttons in format: {callback_data:text} for DATA_ROWS."""
         super().__init__(row_width)
 
         if cdata_and_text:
-            buttons = {cdata.upper(): text for cdata, text in cdata_and_text.items() if text}
+            buttons = {
+                cdata.upper(): text for cdata, text in cdata_and_text.items() if text
+            }
         else:
             buttons = {}
 
         for data_row in self.data_rows:
             btn_row = self.make_buttons_row(data_row, buttons)
             self.row(*btn_row)
 
     @property
     def data_rows(self) -> list[list[str]]:
         return [self._to_values_list(row) for row in self.DATA_ROWS]
 
-    def make_buttons_row(self, data_row: list[str], buttons: dict) -> list[InlineKeyboardButton]:
-        return [self._make_data_button(cdata, buttons) for cdata in data_row if cdata in buttons]
+    def make_buttons_row(
+        self, data_row: list[str], buttons: dict
+    ) -> list[InlineKeyboardButton]:
+        return [
+            self._make_data_button(cdata, buttons)
+            for cdata in data_row
+            if cdata in buttons
+        ]
 
     @staticmethod
     def _to_values_list(data_row: str or tuple[str]) -> list[str]:
         if not isinstance(data_row, tuple):
             data_row = (data_row,)
         return [button.value for button in data_row]
```

### Comparing `aiogram-tools-1.0.0/aiogram_tools/_models.py` & `aiogram-tools-1.0.1/aiogram_tools/_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,24 +2,23 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field, fields, asdict, Field
 from typing import Union, TypeVar
 
 from bson import ObjectId
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 # TODO: warning
 EmptyList = field(default_factory=list)
 EmptyDict = field(default_factory=dict)
 
 
 @dataclass
 class DataModel:
-
     def to_dict(self):
         return asdict(self)
 
     @classmethod
     @property
     def field_names(cls) -> list[str]:
         return [f.name for f in fields(cls)]
@@ -42,27 +41,27 @@
         if not obj_data:
             return None
 
         resolved_data = cls._resolve_fields(obj_data)
 
         for _field, value in resolved_data.items():
             field_type = cls.__annotations__.get(_field)
-            factory = getattr(field_type, 'from_dict', None)
+            factory = getattr(field_type, "from_dict", None)
             if factory:
                 resolved_data[_field] = factory(value)
 
         # noinspection PyArgumentList
         return cls(**resolved_data)
 
 
 class MongoModelMeta(type):
     def __new__(mcs, name, bases, namespace):
-        if '_id' not in namespace:
-            namespace['_id'] = field(default=None)
-            namespace.setdefault('__annotations__', {})['_id'] = None
+        if "_id" not in namespace:
+            namespace["_id"] = field(default=None)
+            namespace.setdefault("__annotations__", {})["_id"] = None
 
         cls = super().__new__(mcs, name, bases, namespace)
         return cls
 
 
 class MongoModel(DataModel, metaclass=MongoModelMeta):
     _id: Union[str, int, ObjectId] = None
@@ -71,8 +70,8 @@
     def id(self) -> Union[str, int, None]:
         if isinstance(self._id, ObjectId):
             return str(self._id)
         return self._id
 
     @id.setter
     def id(self, value: Union[str, int, None]):
-        setattr(self, '_id', value)
+        setattr(self, "_id", value)
```

### Comparing `aiogram-tools-1.0.0/aiogram_tools/_questions.py` & `aiogram-tools-1.0.1/aiogram_tools/_questions.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,21 +14,23 @@
 
 AsyncFunction = Callable[[], Awaitable]
 
 
 @dataclass
 class QuestText:
     """Text and keyboard for an ordinary question."""
+
     text: str
     keyboard: KeyboardMarkup
 
 
 @dataclass
 class QuestFunc:
     """Async function for an extraordinary question. Will be called without args."""
+
     async_func: AsyncFunction
 
 
 Quest = Union[str, QuestText, QuestFunc, None]
 Quests = Union[Quest, list[Quest]]
 
 
@@ -42,15 +44,15 @@
 
 class ConvStatesGroupMeta(StatesGroupMeta2):
     """Check if StatesGroup have only ConvState attributes (not State)."""
 
     def __new__(mcs, class_name, bases, namespace, **kwargs):
         for prop in namespace:
             if isinstance(prop, State) and not isinstance(prop, ConvState):
-                err_text = f'{class_name} attrs must be instance of {ConvState.__name__}, not {State.__name__}'
+                err_text = f"{class_name} attrs must be instance of {ConvState.__name__}, not {State.__name__}"
                 raise TypeError(err_text)
 
         return super().__new__(mcs, class_name, bases, namespace, **kwargs)
 
 
 class ConvStatesGroup(StatesGroup2, metaclass=ConvStatesGroupMeta):
     """StatesGroup with only ConvState attributes (not State)."""
```

### Comparing `aiogram-tools-1.0.0/aiogram_tools/_states.py` & `aiogram-tools-1.0.1/aiogram_tools/_states.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,23 @@
 
 from aiogram import Dispatcher
 from aiogram.dispatcher import FSMContext
 from aiogram.dispatcher.filters.state import State, StatesGroup, StatesGroupMeta
 
 
 class StatesGroupMeta2(StatesGroupMeta):
-
     def __new__(mcs, name, bases, namespace, **kwargs):
         cls = super(StatesGroupMeta, mcs).__new__(mcs, name, bases, namespace)
 
         states = []
         childs = []
 
         cls._group_name = name
 
         for name, prop in namespace.items():
-
             if isinstance(prop, State):
                 states.append(prop)
                 StatesGroup2.all_states_groups_states.add(prop)
             elif inspect.isclass(prop) and issubclass(prop, StatesGroup):
                 childs.append(prop)
                 prop._parent = cls
```

### Comparing `aiogram-tools-1.0.0/aiogram_tools/filters.py` & `aiogram-tools-1.0.1/aiogram_tools/filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 from aiogram.dispatcher.filters import BoundFilter
 from aiogram.types import InlineKeyboardButton, KeyboardButton
 
 
 class StorageDataFilter(BoundFilter):
     """Check if all items matches the relevant items in the storage (for current User+Chat)."""
 
-    key = 'storage'
+    key = "storage"
 
     def __init__(self, dispatcher, storage: dict):
         self.dispatcher = dispatcher
         self.storage = storage
 
     def is_matching(self, storage_data: dict) -> bool:
         for key, value in self.storage.items():
             if key not in storage_data:
                 return False
 
-            if value == '*':
+            if value == "*":
                 continue
 
             if isinstance(value, (list, tuple, set)) and storage_data[key] in value:
                 continue
 
             if storage_data[key] == value:
                 continue
@@ -39,15 +39,15 @@
     async def check(self, *args) -> bool:
         state_ctx = self.dispatcher.current_state()
         storage_data = await state_ctx.get_data()
         return self.is_matching(storage_data)
 
 
 class _ButtonFilter(BoundFilter):
-    key = 'button'
+    key = "button"
 
     @abstractmethod
     def cast_button(self, button):
         """Cast button to string for matching"""
 
     @abstractmethod
     def cast_update(self, obj):
@@ -64,60 +64,61 @@
 
         for item in button:
             if isinstance(item, str):
                 button_data = item
             else:
                 button_data = self.cast_button(item)
 
-            assert isinstance(button_data, str), f'Invalid data for {self.__class__.__name__} filter'
+            assert isinstance(
+                button_data, str
+            ), f"Invalid data for {self.__class__.__name__} filter"
             buttons_regexps.append(self.make_regexp(button_data))
 
         self.buttons_regexps = buttons_regexps
 
     def check_one(self, obj, button_regexp: str) -> Optional[dict]:
         obj_data = self.cast_update(obj)
         with suppress(TypeError):
             match = re.fullmatch(button_regexp, obj_data)
             if match:
-                return {'button': match.groupdict()}
+                return {"button": match.groupdict()}
 
     async def check(self, obj) -> Union[dict, bool]:
         for regexp in self.buttons_regexps:
             result = self.check_one(obj, regexp)
             if result:
                 return result
         return False
 
 
 class CallbackQueryButton(_ButtonFilter):
-
     def cast_button(self, button: InlineKeyboardButton):
         return button.callback_data
 
     def cast_update(self, obj: types.CallbackQuery):
         return obj.data
 
 
 class InlineQueryButton(_ButtonFilter):
-
     def cast_button(self, button: InlineKeyboardButton):
         if button.switch_inline_query is None:
             return button.switch_inline_query_current_chat
         return button.switch_inline_query
 
     def cast_update(self, obj: types.InlineQuery):
         return obj.query
 
 
 class MessageButton(_ButtonFilter):
-
     def cast_button(self, button: Union[KeyboardButton, InlineKeyboardButton]):
         if isinstance(button, KeyboardButton):
             return button.text
 
-        assert 'start=' in button.url, f'Invalid data for {self.__class__.__name__} filter'
+        assert (
+            "start=" in button.url
+        ), f"Invalid data for {self.__class__.__name__} filter"
 
         start_param = button.url.split("start=")[-1]
-        return f'/start {start_param}'
+        return f"/start {start_param}"
 
     def cast_update(self, obj: types.Message):
         return obj.text
```

### Comparing `aiogram-tools-1.0.0/aiogram_tools/keyboards.py` & `aiogram-tools-1.0.1/aiogram_tools/keyboards.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 from __future__ import annotations
 
 from copy import deepcopy
-from typing import Optional, Union
 
-from aiogram import Bot
-from aiogram.types import InlineKeyboardButton, KeyboardButton
+from .deps import (
+    InlineKeyboardButton,
+    ReplyKeyboardMarkup,
+    InlineKeyboardMarkup,
+    Bot,
+)
 
-DEEPLINK_BASE = 'https://t.me/{bot_username}?start={start_param}'
+DEEPLINK_BASE = "https://t.me/{bot_username}?start={start_param}"
 
 
-def _get_bot_username() -> Optional[str]:
+def _get_bot_username() -> str | None:
     bot = Bot.get_current()
     try:
-        return getattr(getattr(bot, '_me'), 'username')
+        return getattr(getattr(bot, "_me"), "username")
     except AttributeError:
         raise RuntimeError("Can't get bot username for deeplink")
 
 
-Button = KeyboardButton
-
-
 class InlineButton(InlineKeyboardButton):
     def __init__(
-            self, text: str,
-            callback: Union[str, bool] = None,
-            url: Union[str, bool] = None,
-            start_param: Union[str, bool] = None,
-            switch_iquery: Union[str, bool] = None,
-            switch_iquery_current: Union[str, bool] = None,
+        self,
+        text: str,
+        callback: str | bool = None,
+        url: str | bool = None,
+        start_param: str | bool = None,
+        switch_iquery: str | bool = None,
+        switch_iquery_current: str | bool = None,
     ):
         # update args
         if url is True:
             url = text
         elif start_param is True:
             start_param = text
         elif callback is True:
@@ -40,15 +41,17 @@
             switch_iquery = text
         elif switch_iquery_current is True:
             switch_iquery_current = text
 
         # cast start_param to url
         if start_param:
             bot_username = _get_bot_username()
-            url = DEEPLINK_BASE.format(bot_username=bot_username, start_param=start_param)
+            url = DEEPLINK_BASE.format(
+                bot_username=bot_username, start_param=start_param
+            )
 
         super().__init__(
             text,
             url=url,
             callback_data=callback,
             switch_inline_query=switch_iquery,
             switch_inline_query_current_chat=switch_iquery_current,
@@ -59,7 +62,19 @@
         new_button = deepcopy(self)
 
         for item, value in new_button.values.items():
             if isinstance(value, str):
                 new_button[item] = value.format(*args, **kwargs)
 
         return new_button
+
+
+class ReplyKeyboard(ReplyKeyboardMarkup):
+    def __init__(self, *buttons: str, row_width=1):
+        super().__init__(row_width=row_width, resize_keyboard=True)
+        self.add(*buttons)
+
+
+class InlineKeyboard(InlineKeyboardMarkup):
+    def __init__(self, *buttons: InlineButton, row_width=1):
+        super().__init__(row_width=row_width)
+        self.add(*buttons)
```

### Comparing `aiogram-tools-1.0.0/aiogram_tools/middlewares/_conversation.py` & `aiogram-tools-1.0.1/aiogram_tools/middlewares/_conversation.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,33 +8,37 @@
 from aiogram.dispatcher import FSMContext
 from aiogram.dispatcher.middlewares import BaseMiddleware
 from aiogram.dispatcher.storage import FSMContextProxy
 
 from aiogram_tools._questions import ConvState, ConvStatesGroup, ConvStatesGroupMeta
 from aiogram_tools._questions import Quest, Quests, QuestText, QuestFunc
 
-__all__ = ['UpdateData', 'UpdateUserState', 'AnswerOnReturn']
+__all__ = ["UpdateData", "UpdateUserState", "AnswerOnReturn"]
 
-T = TypeVar('T')
+T = TypeVar("T")
 _StorageData = Union[str, int, tuple, dict, None]
 StorageData = Union[_StorageData, list[_StorageData]]
-NewState = Union[Literal['next', 'previous', 'exit'], ConvState, type[ConvStatesGroup], None]
+NewState = Union[
+    Literal["next", "previous", "exit"], ConvState, type[ConvStatesGroup], None
+]
 
 
 def to_list(obj) -> list:
     """Cast obj to list if it's not yet."""
     if not isinstance(obj, list):
         obj = [obj]
     return obj
 
 
 TypeT = type[T]
 
 
-def search_in_results(obj_type: Union[TypeT, tuple[TypeT]], container: list) -> Optional[T]:
+def search_in_results(
+    obj_type: Union[TypeT, tuple[TypeT]], container: list
+) -> Optional[T]:
     """Recursive search for instance of obj_type in lists/tuples."""
     if isinstance(container, (list, tuple)):
         for item in container:
             obj = search_in_results(obj_type, item)
             if obj is not None:  # object found
                 return obj
     elif isinstance(container, obj_type):
@@ -60,15 +64,15 @@
 
 @dataclass
 class UpdateData:
     set_data: dict[str, StorageData] = field(default_factory=dict)
     extend_data: dict[str, StorageData] = field(default_factory=dict)
     remove_data: dict[str, StorageData] = field(default_factory=dict)
     delete_keys: Union[str, list[str]] = field(default_factory=list)
-    new_state: NewState = 'next'
+    new_state: NewState = "next"
     on_conv_exit: Quests = None
 
     @property
     def state_ctx(self) -> FSMContext:
         return Dispatcher.get_current().current_state()
 
     def _extend_data(self, proxy: FSMContextProxy, no_error=True):
@@ -106,29 +110,29 @@
 
         if isinstance(self.new_state, ConvState):
             return self.new_state
 
         if isinstance(self.new_state, ConvStatesGroupMeta):
             return self.new_state.states[0]
 
-        if self.new_state == 'previous':
+        if self.new_state == "previous":
             state = await ConvStatesGroup.get_current_state()
             if state and state.group:
                 group: ConvStatesGroup = state.group
                 new_state = await group.get_previous_state()
                 return new_state
 
-        if self.new_state == 'next':
+        if self.new_state == "next":
             state = await ConvStatesGroup.get_current_state()
             if state:
                 group: ConvStatesGroup = state.group
                 new_state = await group.get_next_state()
                 return new_state
 
-        if self.new_state == 'exit':
+        if self.new_state == "exit":
             return None
 
         if self.new_state is None:
             return False
 
     async def switch_state(self, new_state: Union[ConvState, bool, None]):
         """
@@ -145,19 +149,23 @@
 
 
 class PostMiddleware(BaseMiddleware, ABC):
     """Abstract Middleware for post processing Message and CallbackQuery."""
 
     @staticmethod
     @abstractmethod
-    async def on_post_process_message(msg: types.Message, results: list, state_dict: dict):
+    async def on_post_process_message(
+        msg: types.Message, results: list, state_dict: dict
+    ):
         """Works after processing any message by handler."""
 
     @classmethod
-    async def on_post_process_callback_query(cls, query: types.CallbackQuery, results: list, state_dict: dict):
+    async def on_post_process_callback_query(
+        cls, query: types.CallbackQuery, results: list, state_dict: dict
+    ):
         """Answer query [empty text] and call on_post_process_message(query.message)."""
         await query.answer()
         await cls.on_post_process_message(query.message, results, state_dict)
 
 
 class UpdateUserState(PostMiddleware):
     """Handle returned from handler UpdateData instance.
@@ -179,11 +187,13 @@
             await new_data.switch_state(new_state)
 
 
 class AnswerOnReturn(PostMiddleware):
     """Ask question from returned string, QuestText or QuestFunc."""
 
     @staticmethod
-    async def on_post_process_message(msg: types.Message, results: list, state_dict: dict):
+    async def on_post_process_message(
+        msg: types.Message, results: list, state_dict: dict
+    ):
         question = search_in_results((str, QuestText, QuestFunc), results)
         if question:
             await ask_question(question)
```

### Comparing `aiogram-tools-1.0.0/aiogram_tools/middlewares/_membership.py` & `aiogram-tools-1.0.1/aiogram_tools/middlewares/_membership.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import annotations
 
 from aiogram import types, Bot
 from aiogram.dispatcher.handler import CancelHandler
 from aiogram.dispatcher.middlewares import BaseMiddleware
 from aiogram.utils.exceptions import BadRequest
 
-__all__ = ['CheckMembership']
+__all__ = ["CheckMembership"]
 
 
 class CheckMembership(BaseMiddleware):
     """Check if user is member of group or subscribed on channel."""
 
     def __init__(self, chat_username: str, error_text: str = None):
         if not error_text:
-            error_text = f'Error, you are not member of {chat_username}'
+            error_text = f"Error, you are not member of {chat_username}"
         self.chat = chat_username
         self.error_text = error_text
         super().__init__()
 
     async def is_chat_member(self, user_id: int) -> bool:
         """Check if user is currently member of chat."""
         bot = Bot.get_current()
```

### Comparing `aiogram-tools-1.0.0/aiogram_tools/middlewares/misc.py` & `aiogram-tools-1.0.1/aiogram_tools/middlewares/misc.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,13 +28,15 @@
     async def on_post_process_message(self, msg: types.Message, results: list, *_):
         for item in self.unfold_results(results):
             if isinstance(item, str):
                 await msg.answer(item)
             elif inspect.iscoroutine(item):
                 await item
 
-    async def on_post_process_callback_query(self, query: types.CallbackQuery, results: list, *_):
+    async def on_post_process_callback_query(
+        self, query: types.CallbackQuery, results: list, *_
+    ):
         for item in self.unfold_results(results):
             if isinstance(item, str):
                 await query.message.answer(item)
             elif inspect.iscoroutine(item):
                 await item
```

### Comparing `aiogram-tools-1.0.0/aiogram_tools/middlewares/throttling.py` & `aiogram-tools-1.0.1/aiogram_tools/middlewares/throttling.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,42 +8,51 @@
 from aiogram.dispatcher.middlewares import BaseMiddleware
 from aiogram.utils.exceptions import Throttled
 
 
 class ThrottlingMiddleware(BaseMiddleware):
     """Simple middleware"""
 
-    def __init__(self, on_throttled_text: str, on_unblocked_text: str,
-                 limit=DEFAULT_RATE_LIMIT, key_prefix='antiflood_'):
+    def __init__(
+        self,
+        on_throttled_text: str,
+        on_unblocked_text: str,
+        limit=DEFAULT_RATE_LIMIT,
+        key_prefix="antiflood_",
+    ):
         self.on_throttled_text = on_throttled_text
         self.on_unblocked_text = on_unblocked_text
         self.rate_limit = limit
         self.prefix = key_prefix
         super().__init__()
 
     async def on_process_message(self, message: types.Message, _):
         handler = current_handler.get()
         dispatcher = Dispatcher.get_current()
         if handler:
-            limit = getattr(handler, 'throttling_rate_limit', self.rate_limit)
-            key = getattr(handler, 'throttling_key', f"{self.prefix}_{handler.__name__}")
+            limit = getattr(handler, "throttling_rate_limit", self.rate_limit)
+            key = getattr(
+                handler, "throttling_key", f"{self.prefix}_{handler.__name__}"
+            )
         else:
             limit = self.rate_limit
             key = f"{self.prefix}_message"
         try:
             await dispatcher.throttle(key, rate=limit)
         except Throttled as t:
             await self.message_throttled(message, t)
             raise CancelHandler()
 
     async def message_throttled(self, message: types.Message, throttled: Throttled):
         handler = current_handler.get()
         dispatcher = Dispatcher.get_current()
         if handler:
-            key = getattr(handler, 'throttling_key', f"{self.prefix}_{handler.__name__}")
+            key = getattr(
+                handler, "throttling_key", f"{self.prefix}_{handler.__name__}"
+            )
         else:
             key = f"{self.prefix}_message"
         delta = throttled.rate - throttled.delta
         if throttled.exceeded_count <= 2:
             await message.reply(self.on_throttled_text)
         await asyncio.sleep(delta)
         thr = await dispatcher.check_key(key)
```

