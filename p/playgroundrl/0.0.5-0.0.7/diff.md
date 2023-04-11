# Comparing `tmp/playgroundrl-0.0.5.tar.gz` & `tmp/playgroundrl-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playgroundrl-0.0.5.tar", last modified: Fri Mar  3 09:59:22 2023, max compression
+gzip compressed data, was "playgroundrl-0.0.7.tar", last modified: Tue Apr 11 19:38:39 2023, max compression
```

## Comparing `playgroundrl-0.0.5.tar` & `playgroundrl-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-03-03 09:59:22.849591 playgroundrl-0.0.5/
--rw-r--r--   0 rayan      (501) staff       (20)      188 2023-03-03 09:59:22.849652 playgroundrl-0.0.5/PKG-INFO
--rw-r--r--   0 rayan      (501) staff       (20)      162 2023-02-23 11:25:13.000000 playgroundrl-0.0.5/README.md
--rw-r--r--   0 rayan      (501) staff       (20)       38 2023-03-03 09:59:22.849840 playgroundrl-0.0.5/setup.cfg
--rw-r--r--   0 rayan      (501) staff       (20)      462 2023-03-03 09:59:10.000000 playgroundrl-0.0.5/setup.py
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-03-03 09:59:22.847401 playgroundrl-0.0.5/src/
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-03-03 09:59:22.848676 playgroundrl-0.0.5/src/playgroundrl/
--rw-r--r--   0 rayan      (501) staff       (20)        0 2023-02-27 07:47:18.000000 playgroundrl-0.0.5/src/playgroundrl/__init__.py
--rw-r--r--   0 rayan      (501) staff       (20)     8292 2023-03-02 22:54:39.000000 playgroundrl-0.0.5/src/playgroundrl/client.py
--rw-r--r--   0 rayan      (501) staff       (20)     2307 2023-03-02 22:47:13.000000 playgroundrl-0.0.5/src/playgroundrl/state.py
-drwxr-xr-x   0 rayan      (501) staff       (20)        0 2023-03-03 09:59:22.849480 playgroundrl-0.0.5/src/playgroundrl.egg-info/
--rw-r--r--   0 rayan      (501) staff       (20)      188 2023-03-03 09:59:22.000000 playgroundrl-0.0.5/src/playgroundrl.egg-info/PKG-INFO
--rw-r--r--   0 rayan      (501) staff       (20)      309 2023-03-03 09:59:22.000000 playgroundrl-0.0.5/src/playgroundrl.egg-info/SOURCES.txt
--rw-r--r--   0 rayan      (501) staff       (20)        1 2023-03-03 09:59:22.000000 playgroundrl-0.0.5/src/playgroundrl.egg-info/dependency_links.txt
--rw-r--r--   0 rayan      (501) staff       (20)       52 2023-03-03 09:59:22.000000 playgroundrl-0.0.5/src/playgroundrl.egg-info/requires.txt
--rw-r--r--   0 rayan      (501) staff       (20)       13 2023-03-03 09:59:22.000000 playgroundrl-0.0.5/src/playgroundrl.egg-info/top_level.txt
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-04-11 19:38:39.720244 playgroundrl-0.0.7/
+-rw-r--r--   0 langston   (501) staff       (20)      170 2023-04-11 19:38:39.720313 playgroundrl-0.0.7/PKG-INFO
+-rw-r--r--   0 langston   (501) staff       (20)      162 2023-04-08 20:30:44.000000 playgroundrl-0.0.7/README.md
+-rw-r--r--   0 langston   (501) staff       (20)       38 2023-04-11 19:38:39.720487 playgroundrl-0.0.7/setup.cfg
+-rw-r--r--   0 langston   (501) staff       (20)      443 2023-04-11 19:38:32.000000 playgroundrl-0.0.7/setup.py
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-04-11 19:38:39.717758 playgroundrl-0.0.7/src/
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-04-11 19:38:39.719127 playgroundrl-0.0.7/src/playgroundrl/
+-rw-r--r--   0 langston   (501) staff       (20)        0 2023-04-08 20:30:44.000000 playgroundrl-0.0.7/src/playgroundrl/__init__.py
+-rw-r--r--   0 langston   (501) staff       (20)     8937 2023-04-08 21:07:04.000000 playgroundrl-0.0.7/src/playgroundrl/client.py
+-rw-r--r--   0 langston   (501) staff       (20)     5104 2023-04-08 21:07:04.000000 playgroundrl-0.0.7/src/playgroundrl/state.py
+drwxr-xr-x   0 langston   (501) staff       (20)        0 2023-04-11 19:38:39.720115 playgroundrl-0.0.7/src/playgroundrl.egg-info/
+-rw-r--r--   0 langston   (501) staff       (20)      170 2023-04-11 19:38:39.000000 playgroundrl-0.0.7/src/playgroundrl.egg-info/PKG-INFO
+-rw-r--r--   0 langston   (501) staff       (20)      309 2023-04-11 19:38:39.000000 playgroundrl-0.0.7/src/playgroundrl.egg-info/SOURCES.txt
+-rw-r--r--   0 langston   (501) staff       (20)        1 2023-04-11 19:38:39.000000 playgroundrl-0.0.7/src/playgroundrl.egg-info/dependency_links.txt
+-rw-r--r--   0 langston   (501) staff       (20)       52 2023-04-11 19:38:39.000000 playgroundrl-0.0.7/src/playgroundrl.egg-info/requires.txt
+-rw-r--r--   0 langston   (501) staff       (20)       13 2023-04-11 19:38:39.000000 playgroundrl-0.0.7/src/playgroundrl.egg-info/top_level.txt
```

### Comparing `playgroundrl-0.0.5/src/playgroundrl/client.py` & `playgroundrl-0.0.7/src/playgroundrl/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,19 +15,28 @@
 
     TICTACTOE = 'tic_tac_toe'
 
     CHESS = 'chess'
 
     CATAN = 'catan'
 
+    POKER = 'poker'
+
+    GO = 'go'
+
+    CODENAMES = 'codenames'
+
 TYPE_MAPPING = {
     GameType.SNAKE : SnakeState,
     GameType.TICTACTOE: TicTacToeState,
     GameType.CHESS: ChessState,
-    GameType.CATAN: CatanState
+    GameType.CATAN: CatanState,
+    GameType.POKER: PokerState,
+    GameType.GO: GoState,
+    GameType.CODENAMES: CodenamesState,
 }
 
 # Hack to get cattrs to parse catan actions correctl 
 def hook(d, t):
     return d
 
 cattrs.register_structure_hook(Union[str, List[str]],  hook )
@@ -65,28 +74,31 @@
         model_name: str,
         auth: Dict,
         pool: Pool = Pool(1),  # must be 1 or 2
         endpoint: str = "https://cdn.playgroundrl.com:8083",
         num_games: int = 1,
         render_gameplay: bool = False,
         maximum_messages: int = 5000,
+        self_training: bool = False,
     ):
         """
         Initializes a client Object and connects to the server. 
 
         :param game: String representing game name. 'tictactoe', 'chess', or 'snake'. 
         :param model_name: Name of your RL model. Should be distinct in your user. 
         :param auth: Dictionary containing auth data. In simple case, should contain 
                 'email' and 'api_key' fields. 
         :param pool: Which game pool to play in, must be MODEL_ONLY or OPEN. 
         :param endpoint: URL of backend endpoint to connect to. Mainly used for 
                 connecting to development server. 
         :param num_games: Number of games to play before disconnecting
         :param render_gameplay: Whether to visualize game-play server-side
         :param maximum_messages: A timeout to prevent games from going on forever. 
+        :param self_training: Perform self-training. Instead of being matched with another
+            player, this class will be responsible for all players in the game
         """
         assert(pool.value in [1, 2])
         assert(num_games >= 1)
 
         # Retrieve user id
         # urljoin has weird behavior when it's not terminated right
         if not endpoint.endswith('/'):
@@ -112,14 +124,15 @@
         self.game_type = game
         self.model_name = model_name
         self.pool = pool
         self.num_games = num_games
         self.render_gameplay = render_gameplay
         self.game_id = None
         self.endpoint = endpoint
+        self.self_training = self_training
 
         # Temporary variable to limit number of messages received
         # Todo: Find a more elegant solution to prevent infinite loops
         self.maximum_messages = maximum_messages
         self.exchanged = 0
 
     @abstractmethod
@@ -155,14 +168,15 @@
         self.num_games -= 1
         self.sio.emit(
             "start_game",
             {
                 "game": self.game_type.value,
                 "game_type": self.pool.value,
                 "model_name": self.model_name,
+                "self_training": self.self_training,
             },
         )
         self.sio.wait()
 
     def _register_handlers(self):
         self.sio.on("return_server_side_sid", lambda msg: self._on_get_server_side_sid(msg))
         self.sio.on("state_msg", lambda msg: self._on_state_msg(msg))
@@ -204,15 +218,15 @@
 
     def _on_action_ack_msg(self, msg):
         print(" --ack message received", msg)
         # self.sio.emit('get_state', {'game_id': self.game_id})
 
     # TODO: handle this gracefully
     def _on_game_over_msg(self, msg):
-        print("  --Game ended. Outcome:", msg["outcome"])
+        print(f"  --Game ended. Outcome for player {msg['player_id']}:  {msg['outcome']}")
         if self.num_games <= 0:
             self.sio.disconnect()
             exit()
         self.run()
 
     def _on_send_game_id_msg(self, msg):
         print("  --send_game_id message received", msg)
@@ -225,15 +239,19 @@
             webbrowser.open(url
                             + self.game_type.value.replace("_", "")
                             + "/?listen_to_sid="
                             + self.server_side_sid)
 
         self.game_id = msg["game_id"]
         assert self.game_id is not None
-        self.sio.emit("get_state", {"game_id": self.game_id})
+
+        # Server sends player_ids this client has ownership over 
+        self.player_ids = msg['player_ids']
+
+        self.sio.emit("get_state", {"game_id": self.game_id, "player_id": self.player_ids[0]})
 
 
     def _default_callback(self, msg_type, msg):
         raise Exception("Received unexpected data from server: " + msg_type + msg)
 
     def _on_error_msg(self, msg):
         raise Exception(msg)
```

