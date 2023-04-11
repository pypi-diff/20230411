# Comparing `tmp/frascii-2.2.tar.gz` & `tmp/frascii-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frascii-2.2.tar", last modified: Tue Mar  7 12:26:31 2023, max compression
+gzip compressed data, was "frascii-2.3.tar", last modified: Tue Apr 11 13:54:48 2023, max compression
```

## Comparing `frascii-2.2.tar` & `frascii-2.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-03-07 12:26:31.934619 frascii-2.2/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      233 2023-03-07 12:26:31.934619 frascii-2.2/PKG-INFO
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     8674 2023-03-03 18:20:18.000000 frascii-2.2/README.md
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-03-07 12:26:31.934619 frascii-2.2/frascii/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1533 2023-03-07 12:26:27.000000 frascii-2.2/frascii/__init__.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     6323 2023-03-07 12:25:21.000000 frascii-2.2/frascii/commands.py
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-03-07 12:26:31.934619 frascii-2.2/frascii/fractals/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        0 2023-02-24 11:27:22.000000 frascii-2.2/frascii/fractals/__init__.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      306 2023-03-03 18:15:44.000000 frascii-2.2/frascii/fractals/cantor.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2224 2023-02-28 08:13:57.000000 frascii-2.2/frascii/fractals/dragon_curve.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1263 2023-03-03 18:15:51.000000 frascii-2.2/frascii/fractals/fibonacci.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1816 2023-02-28 08:12:17.000000 frascii-2.2/frascii/fractals/hilbert_curve.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      744 2023-02-28 13:56:01.000000 frascii-2.2/frascii/fractals/julia.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2078 2023-03-01 08:32:48.000000 frascii-2.2/frascii/fractals/koch.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2520 2023-03-07 12:05:08.000000 frascii-2.2/frascii/fractals/l_system.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      609 2023-02-24 15:05:19.000000 frascii-2.2/frascii/fractals/mandelbrot.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2072 2023-02-26 23:51:55.000000 frascii-2.2/frascii/fractals/peano_curve.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      553 2023-02-24 11:50:58.000000 frascii-2.2/frascii/fractals/sierpinski_carpet.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      395 2023-02-28 09:01:32.000000 frascii-2.2/frascii/fractals/sierpinski_triangle.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      494 2023-02-28 14:05:15.000000 frascii-2.2/frascii/fractals/vicsek.py
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-03-07 12:26:31.934619 frascii-2.2/frascii.egg-info/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      233 2023-03-07 12:26:31.000000 frascii-2.2/frascii.egg-info/PKG-INFO
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      627 2023-03-07 12:26:31.000000 frascii-2.2/frascii.egg-info/SOURCES.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        1 2023-03-07 12:26:31.000000 frascii-2.2/frascii.egg-info/dependency_links.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       55 2023-03-07 12:26:31.000000 frascii-2.2/frascii.egg-info/entry_points.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        8 2023-03-07 12:26:31.000000 frascii-2.2/frascii.egg-info/top_level.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       79 2023-03-07 12:26:31.934619 frascii-2.2/setup.cfg
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      374 2023-02-24 14:54:57.000000 frascii-2.2/setup.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-11 13:54:48.322233 frascii-2.3/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      233 2023-04-11 13:54:48.322233 frascii-2.3/PKG-INFO
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    12240 2023-04-07 11:54:45.000000 frascii-2.3/README.md
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-11 13:54:48.318233 frascii-2.3/frascii/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1533 2023-04-11 13:54:36.000000 frascii-2.3/frascii/__init__.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     6323 2023-03-07 12:42:34.000000 frascii-2.3/frascii/commands.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-11 13:54:48.322233 frascii-2.3/frascii/fractals/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        0 2023-02-24 11:27:22.000000 frascii-2.3/frascii/fractals/__init__.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      306 2023-03-03 18:15:44.000000 frascii-2.3/frascii/fractals/cantor.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2224 2023-02-28 08:13:57.000000 frascii-2.3/frascii/fractals/dragon_curve.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1263 2023-03-03 18:15:51.000000 frascii-2.3/frascii/fractals/fibonacci.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1816 2023-02-28 08:12:17.000000 frascii-2.3/frascii/fractals/hilbert_curve.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      744 2023-02-28 13:56:01.000000 frascii-2.3/frascii/fractals/julia.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2078 2023-03-01 08:32:48.000000 frascii-2.3/frascii/fractals/koch.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2562 2023-04-11 13:53:30.000000 frascii-2.3/frascii/fractals/l_system.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      609 2023-02-24 15:05:19.000000 frascii-2.3/frascii/fractals/mandelbrot.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2072 2023-02-26 23:51:55.000000 frascii-2.3/frascii/fractals/peano_curve.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      553 2023-02-24 11:50:58.000000 frascii-2.3/frascii/fractals/sierpinski_carpet.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      395 2023-02-28 09:01:32.000000 frascii-2.3/frascii/fractals/sierpinski_triangle.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      494 2023-02-28 14:05:15.000000 frascii-2.3/frascii/fractals/vicsek.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-11 13:54:48.318233 frascii-2.3/frascii.egg-info/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      233 2023-04-11 13:54:48.000000 frascii-2.3/frascii.egg-info/PKG-INFO
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      627 2023-04-11 13:54:48.000000 frascii-2.3/frascii.egg-info/SOURCES.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        1 2023-04-11 13:54:48.000000 frascii-2.3/frascii.egg-info/dependency_links.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       55 2023-04-11 13:54:48.000000 frascii-2.3/frascii.egg-info/entry_points.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        8 2023-04-11 13:54:48.000000 frascii-2.3/frascii.egg-info/top_level.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       79 2023-04-11 13:54:48.322233 frascii-2.3/setup.cfg
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      374 2023-02-24 14:54:57.000000 frascii-2.3/setup.py
```

### Comparing `frascii-2.2/README.md` & `frascii-2.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 # Commands
 
 `frascii sierpinski_carpet <n>`: Displays the n-th iteration of the [Sierpinski Carpet](https://en.wikipedia.org/wiki/Sierpinski_carpet).
 
 `frascii sierpinski_triangle <n>`: Displays the n-th iteration of the [Sierpinski Triangle](https://en.wikipedia.org/wiki/Sierpinski_triangle).
 
+`frascii cantor <n>`: Displays the n-th iteration of the [Cantor Set](https://en.wikipedia.org/wiki/Cantor_set).
+
 `frascii koch <n>`: Displays the n-th iteration of the [Koch Snowflake](https://en.wikipedia.org/wiki/Koch_snowflake).
 
 `frascii vicsek <n>`: Displays the n-th iteration of the [Vicsek Fractal](https://en.wikipedia.org/wiki/Vicsek_fractal).
 
 `frascii hilbert_curve <n>`: Displays the n-th iteration of the [Hilbert Curve](https://en.wikipedia.org/wiki/Hilbert_curve).
 
 `frascii peano_curve <n>`: Displays the n-th iteration of the [Peano Curve](https://en.wikipedia.org/wiki/Peano_curve).
@@ -21,14 +23,16 @@
 
 `frascii fibonacci <n>`: Displays the [Fibonacci Sequence](https://en.wikipedia.org/wiki/Fibonacci_sequence) up to n as squares.
 
 `frascii mandelbrot <x, y, x_radius, y_radius, stepsize, max_iter>`: Displays a specified part of the [Mandelbrot Set](https://en.wikipedia.org/wiki/Mandelbrot_set).
 
 `frascii julia <f, x, y, x_radius, y_radius, stepsize, max_iter>`: Displays a specified part of the [Julia Set](https://en.wikipedia.org/wiki/Julia_set) for a given f(z).
 
+`frascii l_system <start, rules, n>`: Displays a curve generated by a [L-System](https://en.wikipedia.org/wiki/L-system). Angles will be fixed to 90°.
+
 
 more to come ...
 
 # Examples
 
 ## Mandelbrot set
 `frascii mandelbrot -x_radius 400 -y_radius 180 -stepsize 0.0033`
@@ -131,14 +135,77 @@
   └─┘   ┌─┼─┼─┘       ┌─┘                                       
         └─┼─┼─┐ ┌─┐ ┌─┼─┐                                       
         ┌─┼─┘ └─┼─┼─┘ └─┘                                       
         └─┼─┐   └─┼─┐                                           
           └─┘     └─┘                                           
 
 ```
+
+## L-systems
+
+### Rules
+
+**F** will draw a forward line.
+
+**+** will turn right.
+
+**-** will turn left.
+
+Any other character can be used in the rules but will be ignored when drawing.
+
+`frascii l_system -start "F" -rules "(F->F+F-F-F+F)" -n 2 -direction R`
+
+```
+          ┌─┐           
+        ┌─┘ └─┐         
+      ┌─┘     └─┐       
+    ┌─┼─┐     ┌─┼─┐     
+  ╶─┘ └─┘     └─┘ └─╴   
+```
+
+`frascii l_system -start "F+F+F+F" -rules "(F->F+F-F-FF+F+F-F)" -n 2 -direction U` leads to a **Koch Island**.
+
+```
+                      ┌─┐                                 
+                    ┌─┘ │ ┌─┐                             
+                    └─┐ └─┘ └─┐                           
+                  ┌───┘   ┌───┘                           
+              ┌─┐ └─┐     └─┐         ┌─┐                 
+            ┌─┘ │ ┌─┘       │       ┌─┘ │ ┌─┐             
+            └─┐ └─┘         └─┐     └─┐ └─┘ └─┐           
+          ┌───┘           ┌───┘   ┌───┘   ┌───┘           
+          └─┐ ┌─┐         └─┐ ┌─┐ └─┐     └─┐ ┌─┐         
+            └─┘ │ ┌─┐       └─┘ │ ┌─┘       └─┘ │ ┌─┐     
+                └─┘ └─┐         └─┘             └─┘ └─┐   
+                  ┌───┘                           ┌───┘   
+      ┌─┐     ┌─┐ └─┐                 ┌─┐     ┌─┐ └─┐     
+    ┌─┘ │ ┌───┘ │ ┌─┘               ┌─┘ │ ┌───┘ │ ┌─┘     
+    └─┐ └─┘     └─┘                 └─┐ └─┘     └─┘       
+  ┌───┘                           ┌───┘                   
+  └─┐ ┌─┐             ┌─┐         └─┐ ┌─┐                 
+    └─┘ │ ┌─┐       ┌─┘ │ ┌─┐       └─┘ │ ┌─┐             
+        └─┘ └─┐     └─┐ └─┘ └─┐         └─┘ └─┐           
+          ┌───┘   ┌───┘   ┌───┘           ┌───┘           
+          └─┐ ┌─┐ └─┐     └─┐         ┌─┐ └─┐             
+            └─┘ │ ┌─┘       │       ┌─┘ │ ┌─┘             
+                └─┘         └─┐     └─┐ └─┘               
+                          ┌───┘   ┌───┘                   
+                          └─┐ ┌─┐ └─┐                     
+                            └─┘ │ ┌─┘                     
+                                └─┘                       
+```
+
+
+`frascii l_system -start "A" -rules "(A->+BF-AFA-FB+),(B->-AF+BFB+FA-)" -n 4 -direction R` leads to a **Hilbert Curve**.
+
+`frascii l_system -start "FX" -rules "(X->X+YF+),(Y->-FX-Y)" -n 10 -direction U` leads to a **Dragon Curve**.
+
+`frascii l_system -start Y -rules "(Y->YZ-Z-Z-ZA--),(X->XZ),(Z->XF),(A->Z)" -n 6` leads to **Fibonacci Squares**.
+
+
 # Tip for better visualization
 
 Make a new custom terminal profile and set its fontsize to 1 (Menu->Preferences->Profiles).
 Then you can switch between the default profile and the new one to have "more pixels" on one page.
 
 <img src="readme_images/profile.png" width=25% height=25%>
 <img src="readme_images/fontsize.png" width=50% height=50%>
```

### Comparing `frascii-2.2/frascii/__init__.py` & `frascii-2.3/frascii/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from frascii.fractals.vicsek import vicsek_string
 from frascii.fractals.hilbert_curve import hilbert_curve_string
 from frascii.fractals.peano_curve import peano_curve_string
 from frascii.fractals.dragon_curve import dragon_curve_string
 from frascii.fractals.fibonacci import fibonacci_string
 from frascii.fractals.l_system import l_system_string
 
-__version__ = '2.2'
+__version__ = '2.3'
 
 def mandelbrot(x, y, x_radius, y_radius, stepsize, max_iter):
 	return mandelbrot_string(x, y, x_radius, y_radius, stepsize, max_iter)
 
 def julia(f, x, y, x_radius, y_radius, stepsize, max_iter):
 	return julia_string(f, x, y, x_radius, y_radius, stepsize, max_iter)
```

### Comparing `frascii-2.2/frascii/commands.py` & `frascii-2.3/frascii/commands.py`

 * *Files identical despite different names*

### Comparing `frascii-2.2/frascii/fractals/dragon_curve.py` & `frascii-2.3/frascii/fractals/dragon_curve.py`

 * *Files identical despite different names*

### Comparing `frascii-2.2/frascii/fractals/fibonacci.py` & `frascii-2.3/frascii/fractals/fibonacci.py`

 * *Files identical despite different names*

### Comparing `frascii-2.2/frascii/fractals/hilbert_curve.py` & `frascii-2.3/frascii/fractals/hilbert_curve.py`

 * *Files identical despite different names*

### Comparing `frascii-2.2/frascii/fractals/julia.py` & `frascii-2.3/frascii/fractals/julia.py`

 * *Files identical despite different names*

### Comparing `frascii-2.2/frascii/fractals/koch.py` & `frascii-2.3/frascii/fractals/koch.py`

 * *Files identical despite different names*

### Comparing `frascii-2.2/frascii/fractals/l_system.py` & `frascii-2.3/frascii/fractals/l_system.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 def l_system(start, rules, n):
 	letters = start
 	rules = rules.replace("(", "").replace(")", "").replace(" ", "").split(",")
 	rules = dict(rule.split("->") for rule in rules)
 	for i in range(n):
 		letters = "".join(rules[l] if l in rules else l for l in letters)
-	return "".join(l for l in letters if l in "+-F")
+	return "".join(l for l in letters if l in "+-Ff")
 	
 
 def cleanup(arr):
 	if all(seg == "  " for seg in arr[0]):
 		arr = arr[1:]
 	if all(seg == "  " for seg in arr[-1]):
 		arr = arr[:-1]
@@ -47,26 +47,28 @@
 		curr = out[pos[0]][pos[1]]
 		if turn == "-":
 			comp = comp[1:] + comp[0]
 
 		elif turn == "+":
 			comp = comp[-1] + comp[:-1]
 
-		elif turn == "F":
-			out[pos[0]][pos[1]] = curr.replace(comp[0], "")
+		elif turn in "fF":
+			if turn == "F":
+				out[pos[0]][pos[1]] = curr.replace(comp[0], "")
 			prev_comp = comp	
 			if comp[0] == "U":
 				pos[0] -= 1
 			elif comp[0] == "R":
 				pos[1] += 1
 			elif comp[0] == "D":
 				pos[0] += 1
 			elif comp[0] == "L":
 				pos[1] -= 1
-			out[pos[0]][pos[1]] = out[pos[0]][pos[1]].replace(comp[2], "")
+			if turn == "F":
+				out[pos[0]][pos[1]] = out[pos[0]][pos[1]].replace(comp[2], "")
 
 	# Enlarge grid
 	if pos[0] == len(out) - 1:
 		out.append(["URDL" for i in range(len(out[0]))])
 	if pos[1] == len(out[0]) - 1:
 		out = [row + ["URDL"] for row in out]
 	if pos[0] == 0:
@@ -80,8 +82,8 @@
 			 "RDL": "╵ ", "RL": "│ ", "UD": "──", "UR": "┐ ",
 			 "UL": "┌─", "RD": "┘ ", "DL": "└─", "U": "┬─",
 			 "R": "┤ ", "D": "┴─", "L": "├─", "": "┼─"}
 	return "\n".join("".join(trans[c] for c in row) for row in cleanup(out))
 
 
 if __name__ == '__main__':
-	print(l_system_string("A", "(A->+BF-AFA-FB+), (B->-AF+BFB+FA-)", 3, "R"))
+	print(l_system_string("A", "(A->+Bf-AFA-FB+), (B->-AF+BFB+FA-)", 3, "R"))
```

### Comparing `frascii-2.2/frascii/fractals/mandelbrot.py` & `frascii-2.3/frascii/fractals/mandelbrot.py`

 * *Files identical despite different names*

### Comparing `frascii-2.2/frascii/fractals/peano_curve.py` & `frascii-2.3/frascii/fractals/peano_curve.py`

 * *Files identical despite different names*

### Comparing `frascii-2.2/frascii/fractals/sierpinski_carpet.py` & `frascii-2.3/frascii/fractals/sierpinski_carpet.py`

 * *Files identical despite different names*

### Comparing `frascii-2.2/frascii.egg-info/SOURCES.txt` & `frascii-2.3/frascii.egg-info/SOURCES.txt`

 * *Files identical despite different names*

