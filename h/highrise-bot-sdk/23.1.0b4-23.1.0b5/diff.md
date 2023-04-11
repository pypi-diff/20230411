# Comparing `tmp/highrise_bot_sdk-23.1.0b4.tar.gz` & `tmp/highrise_bot_sdk-23.1.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "highrise_bot_sdk-23.1.0b4.tar", max compression
+gzip compressed data, was "highrise_bot_sdk-23.1.0b5.tar", max compression
```

## Comparing `highrise_bot_sdk-23.1.0b4.tar` & `highrise_bot_sdk-23.1.0b5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1847 2023-04-05 10:12:30.293263 highrise_bot_sdk-23.1.0b4/README.md
--rw-r--r--   0        0        0      941 2023-04-03 21:41:50.607834 highrise_bot_sdk-23.1.0b4/pyproject.toml
--rw-r--r--   0        0        0     6682 2023-04-04 18:50:56.161394 highrise_bot_sdk-23.1.0b4/src/highrise/__init__.py
--rw-r--r--   0        0        0     6727 2023-04-03 21:41:54.240229 highrise_bot_sdk-23.1.0b4/src/highrise/__main__.py
--rw-r--r--   0        0        0     3064 2023-04-03 21:20:12.923631 highrise_bot_sdk-23.1.0b4/src/highrise/_unions.py
--rw-r--r--   0        0        0     5596 2023-04-03 21:41:50.609614 highrise_bot_sdk-23.1.0b4/src/highrise/models.py
--rw-r--r--   0        0        0        0 2023-03-06 18:33:21.284537 highrise_bot_sdk-23.1.0b4/src/highrise/py.typed
--rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 highrise_bot_sdk-23.1.0b4/setup.py
--rw-r--r--   0        0        0     2386 1970-01-01 00:00:00.000000 highrise_bot_sdk-23.1.0b4/PKG-INFO
+-rw-r--r--   0        0        0     2227 2023-04-11 15:28:48.858654 highrise_bot_sdk-23.1.0b5/README.md
+-rw-r--r--   0        0        0      941 2023-04-05 10:55:11.593090 highrise_bot_sdk-23.1.0b5/pyproject.toml
+-rw-r--r--   0        0        0     7970 2023-04-11 15:27:49.521691 highrise_bot_sdk-23.1.0b5/src/highrise/__init__.py
+-rw-r--r--   0        0        0     6923 2023-04-11 15:27:49.521577 highrise_bot_sdk-23.1.0b5/src/highrise/__main__.py
+-rw-r--r--   0        0        0     3064 2023-03-31 11:07:05.693250 highrise_bot_sdk-23.1.0b5/src/highrise/_unions.py
+-rw-r--r--   0        0        0     7386 2023-04-11 15:27:49.521650 highrise_bot_sdk-23.1.0b5/src/highrise/models.py
+-rw-r--r--   0        0        0        0 2023-03-30 13:16:17.585454 highrise_bot_sdk-23.1.0b5/src/highrise/py.typed
+-rw-r--r--   0        0        0     3169 1970-01-01 00:00:00.000000 highrise_bot_sdk-23.1.0b5/setup.py
+-rw-r--r--   0        0        0     2766 1970-01-01 00:00:00.000000 highrise_bot_sdk-23.1.0b5/PKG-INFO
```

### Comparing `highrise_bot_sdk-23.1.0b4/README.md` & `highrise_bot_sdk-23.1.0b5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ---
 
 The Highrise Python Bot SDK is a python library for writing and running Highrise bots.
 
 First, install the library (preferably in a virtual environment):
 
 ```shell
-$ pip install highrise-bot-sdk==23.1.0b4
+$ pip install highrise-bot-sdk==23.1.0b5
 ```
 
 In the [`Settings` section of the Highrise website](https://highrise.game/account/settings), create a bot and generate the API token. You'll need the token to start your bot later.
 You will also need a room ID for your bot to connect to; the room needs to be owned by you or your bot user needs to have designer rights to enter it.
 
 Open a new file, and paste the following to get started (into `mybot.py` for example):
 
@@ -28,14 +28,21 @@
 
 ```
 $ highrise mybot:Bot <room ID> <API token>
 ```
 
 ## Changelog
 
+### 23.1.0b5 (2023-04-11)
+
+- Add support for getting room permissions for users (`self.highrise.get_room_privilege(user_id)`).
+- Add support changing room permissions for users (`self.highrise.set_room_privilege(user_id, privilege)`).
+- Add support for moderating rooms (`self.highrise.moderate_room(user_id, moderate_action, action_length)`). 
+- Rework how keepalive is handled
+
 ### 23.1.0b4 (2023-04-05)
 
 - Methods mapping to requests with empty responses (`chat`, `send_whisper`, `send_emote`, `react`, `set_indicator`, `send_channel`, `walk_to`, `teleport`) now return `None`, and raise a `highrise.ResponseError` on an error response.
 - Fix the emote API.
 - Internally rework request handling to improve robustness.
 
 ### 23.1.0b3 (2023-04-03)
```

### Comparing `highrise_bot_sdk-23.1.0b4/pyproject.toml` & `highrise_bot_sdk-23.1.0b5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "highrise-bot-sdk"
-version = "23.1.0.b4"
+version = "23.1.0.b5"
 description = "The Highrise Bot SDK, for running Highrise bots written in Python."
 authors = ["Pocket Worlds Inc <server@high.rs>"]
 license = "proprietary"
 readme = "README.md"
 packages = [{include = "highrise", from = "src"}]
```

### Comparing `highrise_bot_sdk-23.1.0b4/src/highrise/__init__.py` & `highrise_bot_sdk-23.1.0b5/src/highrise/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 """The Highrise bot SDK."""
 from __future__ import annotations
 
 from asyncio import Queue, TaskGroup, sleep
 from itertools import count
-from typing import TYPE_CHECKING, Any, Callable, Protocol, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Callable, Literal, Protocol, TypeVar, Union
 
 from aiohttp import ClientWebSocketResponse
 from cattrs.preconf.json import make_converter
 
 from ._unions import configure_tagged_union
 from .models import (
     AnchorPosition,
+    ChangeRoomPrivilegeRequest,
     ChannelEvent,
     ChannelRequest,
     ChatEvent,
     ChatRequest,
     CurrencyItem,
     EmoteEvent,
     EmoteRequest,
     Error,
     FloorHitRequest,
+    GetRoomPrivilegeRequest,
     GetRoomUsersRequest,
     GetWalletRequest,
     IndicatorRequest,
     Item,
+    KeepaliveRequest,
+    ModerateRoomRequest,
     Position,
     Reaction,
     ReactionEvent,
     ReactionRequest,
+    RoomPermissions,
     SessionMetadata,
     TeleportRequest,
     TipReactionEvent,
     User,
     UserJoinedEvent,
     UserLeftEvent,
 )
@@ -40,15 +45,23 @@
     from attrs import AttrsInstance
 else:
 
     class AttrsInstance(Protocol):
         pass
 
 
-__all__ = ["BaseBot", "Highrise", "User", "Position", "Reaction", "AnchorPosition"]
+__all__ = [
+    "BaseBot",
+    "Highrise",
+    "User",
+    "Position",
+    "Reaction",
+    "AnchorPosition",
+    "RoomPermissions",
+]
 A = TypeVar("A", bound=AttrsInstance)
 T = TypeVar("T")
 
 
 class BaseBot:
     """A base class for Highrise bots.
     Bots join a room and interact with everything in it.
@@ -158,14 +171,42 @@
         )
         return await q.get()
 
     async def get_wallet(self) -> GetWalletRequest.GetWalletResponse | Error:
         """Fetch the bot wallet."""
         return await do_req_resp(self, GetWalletRequest())
 
+    async def moderate_room(
+        self,
+        user_id: str,
+        action: Literal["kick", "ban", "unban", "mute"],
+        action_length: int | None = None,
+    ) -> None:
+        """Moderate a user in the room."""
+        await _do_req_no_resp(self, ModerateRoomRequest(user_id, action, action_length))
+
+    async def get_room_privilege(
+        self, user_id: str
+    ) -> RoomPermissions | Error:
+        """Fetch the room privilege for given user_id."""
+        resp = await do_req_resp(self, GetRoomPrivilegeRequest(user_id))
+        if isinstance(resp, Error):
+            return resp
+        return resp.content
+
+    async def change_room_privilege(
+        self, user_id: str, permissions: RoomPermissions
+    ) -> None:
+        """Change the room privilege for given user_id.
+
+        example: self.highrise.change_room_privilege(user_id, RoomPermissions(moderator=True))
+
+        """
+        await _do_req_no_resp(self, ChangeRoomPrivilegeRequest(user_id, permissions))
+
     def call_in(self, callback: Callable, delay: float) -> None:
         self.tg.create_task(_delayed_callback(callback, delay))
 
 
 class ResponseError(Exception):
     """An API response error."""
 
@@ -216,14 +257,18 @@
     | ReactionRequest
     | EmoteRequest
     | ChannelRequest
     | FloorHitRequest
     | TeleportRequest
     | GetRoomUsersRequest
     | GetWalletRequest
+    | GetRoomPrivilegeRequest
+    | ChangeRoomPrivilegeRequest
+    | ModerateRoomRequest
+    | KeepaliveRequest
 )
 IncomingEvents = (
     Error
     | ChatEvent
     | EmoteEvent
     | ReactionEvent
     | UserJoinedEvent
```

### Comparing `highrise_bot_sdk-23.1.0b4/src/highrise/__main__.py` & `highrise_bot_sdk-23.1.0b5/src/highrise/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 
 from asyncio import TaskGroup
 from asyncio import run as arun
 from asyncio import sleep
+from asyncio.exceptions import TimeoutError
 from importlib import import_module
 from math import ceil
 from os import environ, getcwd
 from sys import path
 from time import monotonic
-from typing import Any, AsyncGenerator
+from typing import Any, AsyncGenerator, Final
 
 from aiohttp import ClientSession, WebSocketError, WSServerHandshakeError
 from click import argument, command
 
 from . import BaseBot, Highrise, Incoming, IncomingEvents, converter
 from .models import (
     ChannelEvent,
@@ -22,14 +23,17 @@
     ReactionEvent,
     SessionMetadata,
     TipReactionEvent,
     UserJoinedEvent,
     UserLeftEvent,
 )
 
+KEEPALIVE_RATE: Final[int] = 15
+READ_TIMEOUT: Final[int] = 20
+
 
 @command()
 @argument("bot_path")
 @argument("room_id")
 @argument("api_token")
 def run(bot_path: str, room_id: str, api_token: str) -> None:
     """Run a Highrise bot.
@@ -53,15 +57,15 @@
                     async with session.ws_connect(
                         environ.get("HR_WEBAPI_URL", "wss://highrise.game/web/webapi"),
                         headers={"room-id": room_id, "api-token": api_key},
                     ) as ws:
 
                         async def send_keepalive() -> None:
                             while True:
-                                await sleep(15)
+                                await sleep(KEEPALIVE_RATE)
                                 try:
                                     await ws.send_json({"_type": "KeepaliveRequest"})
                                 except ConnectionResetError:
                                     # We don't want to close the entire TaskGroup.
                                     return
 
                         ka_task = tg.create_task(send_keepalive())
@@ -75,15 +79,16 @@
                         bot_id = str(session_metadata.user_id)
                         chat = Highrise()
                         chat.ws = ws
                         chat.tg = tg
 
                         bot.highrise = chat
                         tg.create_task(bot.on_start(session_metadata))
-                        async for frame in ws:
+                        while True:
+                            frame = await ws.receive(READ_TIMEOUT)
                             if isinstance(frame.data, WebSocketError):
                                 print("Websocket error, exiting.")
                                 return
                             msg: IncomingEvents = converter.loads(frame.data, Incoming)  # type: ignore
                             match msg:
                                 case object(rid=rid) if hasattr(msg, "rid"):  # type: ignore
                                     if rid not in chat._req_id_registry:
@@ -122,15 +127,15 @@
                                     tg.create_task(bot.on_user_join(user))
                                 case UserLeftEvent(user=user):
                                     tg.create_task(bot.on_user_leave(user))
                                 case TipReactionEvent(
                                     sender=sender, receiver=receiver, item=tip
                                 ):
                                     tg.create_task(bot.on_tip(sender, receiver, tip))
-            except (ConnectionResetError, WSServerHandshakeError):
+            except (ConnectionResetError, WSServerHandshakeError, TimeoutError):
                 # The throttler should kick in up-code.
                 print("ERROR")
                 pass
 
 
 async def throttler(
     drops: int = 10, drop_recharge: float = 1.0
```

### Comparing `highrise_bot_sdk-23.1.0b4/src/highrise/_unions.py` & `highrise_bot_sdk-23.1.0b5/src/highrise/_unions.py`

 * *Files identical despite different names*

### Comparing `highrise_bot_sdk-23.1.0b4/src/highrise/models.py` & `highrise_bot_sdk-23.1.0b5/src/highrise/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 
 
 Reaction: TypeAlias = Literal["clap", "heart", "thumbs", "wave", "wink"]
 Facing: TypeAlias = Literal["FrontRight", "FrontLeft", "BackRight", "BackLeft"]
 
 
 @define
+class RoomPermissions:
+    moderator: bool | None = None
+    designer: bool | None = None
+
+
+@define
 class Position:
     x: float
     y: float
     z: float
     facing: Facing = "FrontRight"
 
 
@@ -163,14 +169,26 @@
 class KeepaliveRequest:
     """
     Send a keepalive request.
 
     This must be sent every 15 seconds or the server will terminate the connection.
     """
 
+    rid: str | None = None
+
+    @define
+    class KeepaliveResponse:
+        """
+        A response to a successful reaction.
+        """
+
+        rid: str | None = None
+
+    Response: ClassVar = KeepaliveResponse
+
 
 @define
 class TeleportRequest:
     """
     Teleport the provided `user_id` to the provided `destination`.
 
     """
@@ -248,14 +266,84 @@
         content: list[CurrencyItem]
         rid: str
 
     Response: ClassVar = GetWalletResponse
 
 
 @define
+class ModerateRoomRequest:
+    """
+    Moderate the room.
+
+    This can be used to kick, ban, unban, or mute a user.
+    """
+
+    user_id: str
+    moderation_action: Literal["kick", "ban", "unban", "mute"]
+    action_length: int | None = None
+    rid: str | None = None
+
+    @define
+    class ModerateRoomResponse:
+        """
+        The successful response to a `ModerateRoomRequest`.
+        """
+
+        rid: str | None = None
+
+    Response: ClassVar = ModerateRoomResponse
+
+
+@define
+class GetRoomPrivilegeRequest:
+    """
+    Fetch the room privileges for provided `user_id`.
+    """
+
+    user_id: str
+    rid: str | None = None
+
+    @define
+    class GetRoomPrivilegeResponse:
+        """
+        The room privileges for provided `user_id`.
+        """
+
+        content: RoomPermissions
+        rid: str
+
+    Response: ClassVar = GetRoomPrivilegeResponse
+
+
+@define
+class ChangeRoomPrivilegeRequest:
+    """
+    Change the room privileges for provided `user_id`.
+    This can be used to both give and take moderation and designer privileges for current room.
+
+    Bots have to be in the room to change privileges.
+    Bots are using their owner's privileges.
+    """
+
+    user_id: str
+    permissions: RoomPermissions
+    rid: str | None = None
+
+    @define
+    class ChangeRoomPrivilegeResponse:
+        """
+        The successful response to a `ChangeRoomPrivilegeRequest`.
+        """
+
+        rid: str
+
+    Response: ClassVar = ChangeRoomPrivilegeResponse
+
+
+@define
 class SessionMetadata:
     """
     Initial session data.
 
     This will be sent once, as the first message when a connection is established.
     """
```

### Comparing `highrise_bot_sdk-23.1.0b4/setup.py` & `highrise_bot_sdk-23.1.0b5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 ['aiohttp>=3.8.4', 'cattrs>=22.2.0,<23.0.0', 'click>=8.1.3']
 
 entry_points = \
 {'console_scripts': ['highrise = highrise.__main__:run']}
 
 setup_kwargs = {
     'name': 'highrise-bot-sdk',
-    'version': '23.1.0b4',
+    'version': '23.1.0b5',
     'description': 'The Highrise Bot SDK, for running Highrise bots written in Python.',
-    'long_description': "# The Highrise Python Bot SDK\n\n---\n\nThe Highrise Python Bot SDK is a python library for writing and running Highrise bots.\n\nFirst, install the library (preferably in a virtual environment):\n\n```shell\n$ pip install highrise-bot-sdk==23.1.0b4\n```\n\nIn the [`Settings` section of the Highrise website](https://highrise.game/account/settings), create a bot and generate the API token. You'll need the token to start your bot later.\nYou will also need a room ID for your bot to connect to; the room needs to be owned by you or your bot user needs to have designer rights to enter it.\n\nOpen a new file, and paste the following to get started (into `mybot.py` for example):\n\n```python\nfrom highrise import BaseBot\n\nclass Bot(BaseBot):\n    pass\n```\n\nOverride methods from `BaseBot` as needed.\n\nWhen you're ready, run the bot from the terminal using the SDK, giving it the Python path to the Bot class:\n\n```\n$ highrise mybot:Bot <room ID> <API token>\n```\n\n## Changelog\n\n### 23.1.0b4 (2023-04-05)\n\n- Methods mapping to requests with empty responses (`chat`, `send_whisper`, `send_emote`, `react`, `set_indicator`, `send_channel`, `walk_to`, `teleport`) now return `None`, and raise a `highrise.ResponseError` on an error response.\n- Fix the emote API.\n- Internally rework request handling to improve robustness.\n\n### 23.1.0b3 (2023-04-03)\n\n- Fix the chatting API.\n\n### 23.1.0b2 (2023-04-03)\n\n- Add support for receiving and sending reactions.\n- Fix support for hidden channels.\n- Migrate to the new message for avatars leaving.\n- Improve concurrency when awaiting bot methods.\n- Fix issues with teleporting users.\n- Fix issues with user coordinates.\n- Add support for fetching the bot wallet (`self.highrise.get_wallet()`).\n\n### 23.1.0b1 (2023-03-28)\n\n- Add support for emotes and hidden channel messages.\n\n### 23.1.0b0 (2023-03-10)\n\n- Initial beta release.\n",
+    'long_description': "# The Highrise Python Bot SDK\n\n---\n\nThe Highrise Python Bot SDK is a python library for writing and running Highrise bots.\n\nFirst, install the library (preferably in a virtual environment):\n\n```shell\n$ pip install highrise-bot-sdk==23.1.0b5\n```\n\nIn the [`Settings` section of the Highrise website](https://highrise.game/account/settings), create a bot and generate the API token. You'll need the token to start your bot later.\nYou will also need a room ID for your bot to connect to; the room needs to be owned by you or your bot user needs to have designer rights to enter it.\n\nOpen a new file, and paste the following to get started (into `mybot.py` for example):\n\n```python\nfrom highrise import BaseBot\n\nclass Bot(BaseBot):\n    pass\n```\n\nOverride methods from `BaseBot` as needed.\n\nWhen you're ready, run the bot from the terminal using the SDK, giving it the Python path to the Bot class:\n\n```\n$ highrise mybot:Bot <room ID> <API token>\n```\n\n## Changelog\n\n### 23.1.0b5 (2023-04-11)\n\n- Add support for getting room permissions for users (`self.highrise.get_room_privilege(user_id)`).\n- Add support changing room permissions for users (`self.highrise.set_room_privilege(user_id, privilege)`).\n- Add support for moderating rooms (`self.highrise.moderate_room(user_id, moderate_action, action_length)`). \n- Rework how keepalive is handled\n\n### 23.1.0b4 (2023-04-05)\n\n- Methods mapping to requests with empty responses (`chat`, `send_whisper`, `send_emote`, `react`, `set_indicator`, `send_channel`, `walk_to`, `teleport`) now return `None`, and raise a `highrise.ResponseError` on an error response.\n- Fix the emote API.\n- Internally rework request handling to improve robustness.\n\n### 23.1.0b3 (2023-04-03)\n\n- Fix the chatting API.\n\n### 23.1.0b2 (2023-04-03)\n\n- Add support for receiving and sending reactions.\n- Fix support for hidden channels.\n- Migrate to the new message for avatars leaving.\n- Improve concurrency when awaiting bot methods.\n- Fix issues with teleporting users.\n- Fix issues with user coordinates.\n- Add support for fetching the bot wallet (`self.highrise.get_wallet()`).\n\n### 23.1.0b1 (2023-03-28)\n\n- Add support for emotes and hidden channel messages.\n\n### 23.1.0b0 (2023-03-10)\n\n- Initial beta release.\n",
     'author': 'Pocket Worlds Inc',
     'author_email': 'server@high.rs',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `highrise_bot_sdk-23.1.0b4/PKG-INFO` & `highrise_bot_sdk-23.1.0b5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: highrise-bot-sdk
-Version: 23.1.0b4
+Version: 23.1.0b5
 Summary: The Highrise Bot SDK, for running Highrise bots written in Python.
 License: Proprietary
 Author: Pocket Worlds Inc
 Author-email: server@high.rs
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 ---
 
 The Highrise Python Bot SDK is a python library for writing and running Highrise bots.
 
 First, install the library (preferably in a virtual environment):
 
 ```shell
-$ pip install highrise-bot-sdk==23.1.0b4
+$ pip install highrise-bot-sdk==23.1.0b5
 ```
 
 In the [`Settings` section of the Highrise website](https://highrise.game/account/settings), create a bot and generate the API token. You'll need the token to start your bot later.
 You will also need a room ID for your bot to connect to; the room needs to be owned by you or your bot user needs to have designer rights to enter it.
 
 Open a new file, and paste the following to get started (into `mybot.py` for example):
 
@@ -44,14 +44,21 @@
 
 ```
 $ highrise mybot:Bot <room ID> <API token>
 ```
 
 ## Changelog
 
+### 23.1.0b5 (2023-04-11)
+
+- Add support for getting room permissions for users (`self.highrise.get_room_privilege(user_id)`).
+- Add support changing room permissions for users (`self.highrise.set_room_privilege(user_id, privilege)`).
+- Add support for moderating rooms (`self.highrise.moderate_room(user_id, moderate_action, action_length)`). 
+- Rework how keepalive is handled
+
 ### 23.1.0b4 (2023-04-05)
 
 - Methods mapping to requests with empty responses (`chat`, `send_whisper`, `send_emote`, `react`, `set_indicator`, `send_channel`, `walk_to`, `teleport`) now return `None`, and raise a `highrise.ResponseError` on an error response.
 - Fix the emote API.
 - Internally rework request handling to improve robustness.
 
 ### 23.1.0b3 (2023-04-03)
```

