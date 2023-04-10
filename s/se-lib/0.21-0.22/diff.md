# Comparing `tmp/se_lib-0.21.tar.gz` & `tmp/se_lib-0.22.tar.gz`

## Comparing `se_lib-0.21.tar` & `se_lib-0.22.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 se_lib-0.21/.DS_Store
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 se_lib-0.21/.gitattributes
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 se_lib-0.21/selib/.DS_Store
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 se_lib-0.21/selib/__init__.py
--rw-r--r--   0        0        0    57249 2020-02-02 00:00:00.000000 se_lib-0.21/selib/selib.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 se_lib-0.21/LICENSE
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 se_lib-0.21/README.md
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 se_lib-0.21/pyproject.toml
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 se_lib-0.21/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 se_lib-0.22/.DS_Store
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 se_lib-0.22/.gitattributes
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 se_lib-0.22/selib/.DS_Store
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 se_lib-0.22/selib/__init__.py
+-rw-r--r--   0        0        0    62356 2020-02-02 00:00:00.000000 se_lib-0.22/selib/selib.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 se_lib-0.22/LICENSE
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 se_lib-0.22/README.md
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 se_lib-0.22/pyproject.toml
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 se_lib-0.22/PKG-INFO
```

### Comparing `se_lib-0.21/.DS_Store` & `se_lib-0.22/.DS_Store`

 * *Files 6% similar despite different names*

```diff
@@ -276,21 +276,21 @@
 00001130: 0908 095f 101d 7b7b 2d31 3430 362c 202d  ..._..{{-1406, -
 00001140: 3330 327d 2c20 7b31 3430 342c 2031 3931  302}, {1404, 191
 00001150: 367d 7d09 0815 232f 3b52 5f6b 6c6d 6e6f  6}}...#/;R_klmno
 00001160: 8f00 0000 0000 0001 0100 0000 0000 0000  ................
 00001170: 0d00 0000 0000 0000 0000 0000 0000 0000  ................
 00001180: 9000 0000 0400 6400 6900 7300 7464 7363  ......d.i.s.tdsc
 00001190: 6c62 6f6f 6c01 0000 0004 0064 0069 0073  lbool......d.i.s
-000011a0: 0074 6c67 3153 636f 6d70 0000 0000 0001  .tlg1Scomp......
-000011b0: 0b5f 0000 0004 0064 0069 0073 0074 6d6f  ._.....d.i.s.tmo
-000011c0: 4444 626c 6f62 0000 0008 7e87 06c8 64f0  DDblob....~...d.
+000011a0: 0074 6c67 3153 636f 6d70 0000 0000 0000  .tlg1Scomp......
+000011b0: a5e7 0000 0004 0064 0069 0073 0074 6d6f  .......d.i.s.tmo
+000011c0: 4444 626c 6f62 0000 0008 213b e5ed 61f2  DDblob....!;..a.
 000011d0: c441 0000 0004 0064 0069 0073 0074 6d6f  .A.....d.i.s.tmo
-000011e0: 6444 626c 6f62 0000 0008 7e87 06c8 64f0  dDblob....~...d.
+000011e0: 6444 626c 6f62 0000 0008 213b e5ed 61f2  dDblob....!;..a.
 000011f0: c441 0000 0004 0064 0069 0073 0074 7068  .A.....d.i.s.tph
-00001200: 3153 636f 6d70 0000 0000 0001 4000 0000  1Scomp......@...
+00001200: 3153 636f 6d70 0000 0000 0000 c000 0000  1Scomp..........
 00001210: 0004 0064 0069 0073 0074 7653 726e 6c6f  ...d.i.s.tvSrnlo
 00001220: 6e67 0000 0001 0000 0007 004c 0049 0043  ng.........L.I.C
 00001230: 0045 004e 0053 0045 496c 6f63 626c 6f62  .E.N.S.EIlocblob
 00001240: 0000 0010 0000 00af 0000 002e ffff ffff  ................
 00001250: ffff 0000 0000 000e 0070 0079 0070 0072  .........p.y.p.r
 00001260: 006f 006a 0065 0063 0074 002e 0074 006f  .o.j.e.c.t...t.o
 00001270: 006d 006c 496c 6f63 626c 6f62 0000 0010  .m.lIlocblob....
```

### Comparing `se_lib-0.21/selib/.DS_Store` & `se_lib-0.22/selib/.DS_Store`

 * *Files identical despite different names*

### Comparing `se_lib-0.21/selib/selib.py` & `se_lib-0.22/selib/selib.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-se-lib Version .196
+se-lib Version .22
 
 Copyright (c) 2022-2023 Ray Madachy
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
@@ -1366,45 +1366,203 @@
             except BaseException:
                 continue
     if verbose: print(f'***{css=}') # rm
     ft = copy
     return(css)
 
 # system dynamics simulation functions
+
+def init_model(start, stop, dt):
+  """
+  Instantiates a system dynamics model for simulation
+  """
+  global xmile_header, model, model_specs
+  xmile_header = f"""<?xml version="1.0" encoding="UTF-8" standalone="yes"?>
+    <xmile version="1.0" xmlns="http://docs.oasis-open.org/xmile/ns/XMILE/v1.0">
+        <header>
+            <vendor>Ray Madachy</vendor>
+            <name>Battle Simulator</name>
+            <options>
+                <uses_outputs/>
+            </options>
+            <product version="1.0">PyML .20 dev</product>
+        </header>"""
+
+  model_specs = f"""
+        <sim_specs>
+                <stop>{stop}</stop>
+                <start>{start}</start>
+                <dt>{dt}</dt>
+        </sim_specs>"""
+  model = ""
+  build_model()
+
+def build_model():
+  global xmile_string
+  xmile_closing = """
+    </xmile>
+    """
+  model_string = """
+        <model>
+            <variables>""" + f"{model}" + """
+            </variables>
+        </model>"""
+  xmile_string = xmile_header + model_specs + model_string + xmile_closing
+  with open('test.xmile', 'w') as f:
+    f.write(xmile_string)
+    
+def add_stock(name, initial, inflows=[], outflows=[]):
+  """
+  Adds a stock to the model
+    
+  Parameters
+  ----------
+  name: str
+    The name of the stock 
+  initial: float
+    Initial value of stock at start of simulation
+  inflows: list of float
+    The names of the inflows to the stock
+  outflows: list of float
+    The names of the outflows to the stock
+  """
+  global model
+  inflow_string, outflow_string = "", ""
+  for flow in inflows:
+    inflow_string += f"""<inflow>"{flow}"</inflow>"""
+  for flow in outflows:
+    outflow_string += f"""<outflow>"{flow}"</outflow>"""
+  model += f"""
+                <stock name="{name}">
+                    <doc>{name}</doc>
+                    {inflow_string}
+                    {outflow_string}
+                    <eqn>{initial}</eqn>
+                </stock>"""
+  build_model()
+  
+def add_auxiliary(name, equation):
+  """
+  Adds auxiliary equation or constant to the model
+
+  Parameters
+  ----------
+  name: str
+    The name of the auxiliary 
+  equation: str
+    Equation for the auxiliary using other named model variables
+  """
+  if "random()" in str(equation): equation = convert_random_to_xmile(equation) 
+  if "random.uniform(" in str(equation): equation = convert_random_to_xmile(equation)
+  if "RANDOM" in str(equation): equation = equation.replace("RANDOM", '(GET_TIME_VALUE(0,0,0) + .00001) / (GET_TIME_VALUE(0,0,0) + .00001) * RANDOM')
+  global model
+  model += f"""
+                <aux name="{name}">
+                    <doc>{name}</doc>
+                    <eqn>{equation}</eqn>
+                </aux>"""
+  build_model()
+    
 def add_flow(name, equation):
     """
     Adds a flow to the model
 
     Parameters
     ----------
     name: str
       The name of the flow 
     equation: str
       Equation for the flow using other named model variables
     """
+    if "random()" in str(equation): equation = convert_random_to_xmile(equation) 
+    if "random.uniform(" in str(equation): equation = convert_random_to_xmile(equation)
+    if "RANDOM" in str(equation): equation = equation.replace("RANDOM", '(GET_TIME_VALUE(0,0,0) + .00001) / (GET_TIME_VALUE(0,0,0) + .00001) * RANDOM')
     global model
     model += f"""
                 <flow name="{name}">
                     <doc>{name}</doc>
                     <eqn>{equation}</eqn>
                 </flow>"""
     build_model()
 
+def convert_random_to_xmile(equation):
+  equation = equation.replace("random(", "RANDOM_0_1(")
+  equation = equation.replace("random.uniform(", "RANDOM_UNIFORM(")
+  return(equation)
+
+
 def plot_graph(*outputs):
     """
     displays matplotlib graph for each model variable
 
     Parameters
     ----------
-    variables: variable name or list of variable names to plot on graph
+    variables: str or list
+    	comma separated variable name(s) or lists of variable names to plot on single graphs
 
-    Returns:
+    Returns
     ----------
     matplotlib graph
     """
     #print (outputs, len(outputs))
     for var in outputs:
         fig, axis = plot.subplots(figsize=(4, 3))
         axis.set(xlabel='Time', ylabel=var)
         axis.plot(output.index, output[var].values, label=var)
         if len(outputs) > 1: axis.legend(loc="best", )
-        plot.show()
+        plot.show()
+  
+def save_graph(*outputs, filename="graph.png"):
+  """
+  save graph to file
+
+  Parameters
+  ----------
+  variables: variable name or list of variable names to plot on graph
+  filename: file name with format extension
+  """
+  for var in outputs:
+    #print(var)
+    fig, axis = plot.subplots()
+    axis.set(xlabel='Time', ylabel=var)
+    axis.plot(output.index, output[var].values, label=var)
+    axis.legend(loc="best", )
+    #plot.show()
+    plot.savefig(filename)
+            
+def run_model():
+    """
+    Executes the model
+    
+    Returns
+    ----------
+    Pandas dataframe containing run outputs for each variable each timestep
+    """
+    import pysd
+    global output
+    global model
+    model = pysd.read_xmile('./test.xmile')
+    output = model.run(progress=False)
+    return (output)
+    
+def set_logical_run_time(condition):
+    """
+    Enables a run time to be measured based on a logical condition for when the simulation should be run (like a while statement).  The logical end time will be available from the 'get_logical_end_time()' function in lieu of the fixed end time for a simulation. 
+    """
+    add_flow("time_flow", 'if_then_else('+str(condition)+', 1, 0)')
+    #add_flow("time_flow", 'if_then_else(not '+str(condition)+', 1, 0)')
+    #add_flow("time_flow", 'if_then_else('+condition+', 0, 1)')
+    add_stock("logical_end_time", 0, inflows=["time_flow"])
+    
+def get_logical_end_time():
+    """
+    Returns the logical end time as specified in a previous 'set_logical_run_time()' function call, in lieu of the fixed end time for a simulation. 
+    
+    Returns
+    ----------
+    logical_end_time: float
+        end time when the 'set_logical_run_time()'' condition expires
+    """
+    return (get_final_value("logical_end_time"))  
+    
+def get_final_value(variable):
+    return (output[variable][model['FINAL TIME']])
```

### Comparing `se_lib-0.21/LICENSE` & `se_lib-0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `se_lib-0.21/README.md` & `se_lib-0.22/README.md`

 * *Files identical despite different names*

### Comparing `se_lib-0.21/PKG-INFO` & `se_lib-0.22/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: se-lib
-Version: 0.21
+Version: 0.22
 Summary: Systems Engineering Library (se-lib)
 Project-URL: Homepage, http://se-lib.org
 Author-email: se-lib Development Team <info@se-lib.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

