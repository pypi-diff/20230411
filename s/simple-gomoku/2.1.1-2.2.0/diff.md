# Comparing `tmp/simple_gomoku-2.1.1-py3-none-any.whl.zip` & `tmp/simple_gomoku-2.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3770 bytes, number of entries: 8
--rw-r--r--  2.0 unx      161 b- defN 23-Mar-11 06:42 simple_gomoku/__init__.py
--rw-r--r--  2.0 unx     3468 b- defN 23-Mar-11 06:42 simple_gomoku/env/Gomoku.py
--rw-r--r--  2.0 unx     1711 b- defN 23-Mar-11 06:42 simple_gomoku/env/TicTacToe.py
--rw-r--r--  2.0 unx       87 b- defN 23-Mar-11 06:42 simple_gomoku/env/__init__.py
--rw-r--r--  2.0 unx      456 b- defN 23-Mar-11 06:43 simple_gomoku-2.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-11 06:43 simple_gomoku-2.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Mar-11 06:43 simple_gomoku-2.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      657 b- defN 23-Mar-11 06:43 simple_gomoku-2.1.1.dist-info/RECORD
-8 files, 6646 bytes uncompressed, 2614 bytes compressed:  60.7%
+Zip file size: 3880 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      161 b- defN 23-Apr-11 15:31 simple_gomoku/__init__.py
+-rw-r--r--  2.0 unx     3973 b- defN 23-Apr-11 15:31 simple_gomoku/env/Gomoku.py
+-rw-r--r--  2.0 unx     1711 b- defN 23-Apr-11 15:31 simple_gomoku/env/TicTacToe.py
+-rw-r--r--  2.0 unx       87 b- defN 23-Apr-11 15:31 simple_gomoku/env/__init__.py
+-rw-r--r--  2.0 unx      435 b- defN 23-Apr-11 15:31 simple_gomoku-2.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 15:31 simple_gomoku-2.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Apr-11 15:31 simple_gomoku-2.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      657 b- defN 23-Apr-11 15:31 simple_gomoku-2.2.0.dist-info/RECORD
+8 files, 7130 bytes uncompressed, 2724 bytes compressed:  61.8%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: simple_gomoku/env/TicTacToe.py
 Comment: 
 
 Filename: simple_gomoku/env/__init__.py
 Comment: 
 
-Filename: simple_gomoku-2.1.1.dist-info/METADATA
+Filename: simple_gomoku-2.2.0.dist-info/METADATA
 Comment: 
 
-Filename: simple_gomoku-2.1.1.dist-info/WHEEL
+Filename: simple_gomoku-2.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: simple_gomoku-2.1.1.dist-info/top_level.txt
+Filename: simple_gomoku-2.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: simple_gomoku-2.1.1.dist-info/RECORD
+Filename: simple_gomoku-2.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## simple_gomoku/env/Gomoku.py

```diff
@@ -45,14 +45,34 @@
     def get_legal_actions(self):
         state = np.array(self.state).reshape(-1)
         return np.where(state==0)[0]
 
     def show(self, state):
         print(state)
 
+    def render(self):
+        state = self.state
+        print("  ", end="")
+
+        for i in range(len(state)):
+            print(i, end=" ")
+        print()
+
+        for i, row in enumerate(state):
+            print(i, end=" ")
+            for piece in row:
+                if piece == -1:
+                    print("X", end=" ")
+                elif piece == 1:
+                    print("O", end=" ")
+                else:
+                    print("-", end=" ")
+            print()
+        print()
+
     def _pass(self):
         self.player = -self.player
         pass
 
     def _is_done(self, a):
         """ a: action """
```

