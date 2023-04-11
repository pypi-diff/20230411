# Comparing `tmp/stpyvista-0.0.7.tar.gz` & `tmp/stpyvista-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stpyvista-0.0.7.tar", last modified: Wed Mar 29 11:38:38 2023, max compression
+gzip compressed data, was "stpyvista-0.0.8.tar", last modified: Tue Apr 11 16:18:51 2023, max compression
```

## Comparing `stpyvista-0.0.7.tar` & `stpyvista-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 edwin     (1000) edwin     (1000)        0 2023-03-29 11:38:38.919206 stpyvista-0.0.7/
--rw-rw-r--   0 edwin     (1000) edwin     (1000)    35129 2022-10-10 23:59:26.000000 stpyvista-0.0.7/LICENSE
--rw-rw-r--   0 edwin     (1000) edwin     (1000)       78 2022-10-10 23:59:26.000000 stpyvista-0.0.7/MANIFEST.in
--rw-rw-r--   0 edwin     (1000) edwin     (1000)     2293 2023-03-29 11:38:38.919206 stpyvista-0.0.7/PKG-INFO
--rw-rw-r--   0 edwin     (1000) edwin     (1000)     1700 2023-03-29 11:28:06.000000 stpyvista-0.0.7/README.md
--rw-rw-r--   0 edwin     (1000) edwin     (1000)      741 2023-03-29 11:36:56.000000 stpyvista-0.0.7/pyproject.toml
--rw-rw-r--   0 edwin     (1000) edwin     (1000)       38 2023-03-29 11:38:38.923206 stpyvista-0.0.7/setup.cfg
--rw-rw-r--   0 edwin     (1000) edwin     (1000)      735 2023-03-29 11:36:42.000000 stpyvista-0.0.7/setup.py
-drwxrwxr-x   0 edwin     (1000) edwin     (1000)        0 2023-03-29 11:38:38.919206 stpyvista-0.0.7/src/
-drwxrwxr-x   0 edwin     (1000) edwin     (1000)        0 2023-03-29 11:38:38.919206 stpyvista-0.0.7/src/stpyvista/
--rw-rw-r--   0 edwin     (1000) edwin     (1000)     3310 2023-03-29 11:36:26.000000 stpyvista-0.0.7/src/stpyvista/__init__.py
--rw-rw-r--   0 edwin     (1000) edwin     (1000)       74 2022-10-11 00:08:17.000000 stpyvista-0.0.7/src/stpyvista/__main__.py
-drwxrwxr-x   0 edwin     (1000) edwin     (1000)        0 2023-03-29 11:38:38.919206 stpyvista-0.0.7/src/stpyvista/frontend/
--rw-rw-r--   0 edwin     (1000) edwin     (1000)      631 2022-11-06 19:43:06.000000 stpyvista-0.0.7/src/stpyvista/frontend/index.html
--rw-rw-r--   0 edwin     (1000) edwin     (1000)     1989 2023-03-26 22:01:18.000000 stpyvista-0.0.7/src/stpyvista/frontend/main.js
--rw-rw-r--   0 edwin     (1000) edwin     (1000)     1198 2023-03-10 15:57:04.000000 stpyvista-0.0.7/src/stpyvista/frontend/streamlit-component-lib.js
--rw-rw-r--   0 edwin     (1000) edwin     (1000)      166 2023-03-09 01:49:59.000000 stpyvista-0.0.7/src/stpyvista/frontend/style.css
-drwxrwxr-x   0 edwin     (1000) edwin     (1000)        0 2023-03-29 11:38:38.919206 stpyvista-0.0.7/src/stpyvista.egg-info/
--rw-rw-r--   0 edwin     (1000) edwin     (1000)     2293 2023-03-29 11:38:38.000000 stpyvista-0.0.7/src/stpyvista.egg-info/PKG-INFO
--rw-rw-r--   0 edwin     (1000) edwin     (1000)      437 2023-03-29 11:38:38.000000 stpyvista-0.0.7/src/stpyvista.egg-info/SOURCES.txt
--rw-rw-r--   0 edwin     (1000) edwin     (1000)        1 2023-03-29 11:38:38.000000 stpyvista-0.0.7/src/stpyvista.egg-info/dependency_links.txt
--rw-rw-r--   0 edwin     (1000) edwin     (1000)       38 2023-03-29 11:38:38.000000 stpyvista-0.0.7/src/stpyvista.egg-info/requires.txt
--rw-rw-r--   0 edwin     (1000) edwin     (1000)       10 2023-03-29 11:38:38.000000 stpyvista-0.0.7/src/stpyvista.egg-info/top_level.txt
+drwxrwxr-x   0 edwin     (1000) edwin     (1000)        0 2023-04-11 16:18:51.246677 stpyvista-0.0.8/
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)    35129 2022-10-10 23:59:26.000000 stpyvista-0.0.8/LICENSE
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)       78 2022-10-10 23:59:26.000000 stpyvista-0.0.8/MANIFEST.in
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)     2548 2023-04-11 16:18:51.246677 stpyvista-0.0.8/PKG-INFO
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)     1955 2023-04-11 16:18:15.000000 stpyvista-0.0.8/README.md
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)      741 2023-04-11 16:18:34.000000 stpyvista-0.0.8/pyproject.toml
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)       38 2023-04-11 16:18:51.246677 stpyvista-0.0.8/setup.cfg
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)      735 2023-04-11 16:17:19.000000 stpyvista-0.0.8/setup.py
+drwxrwxr-x   0 edwin     (1000) edwin     (1000)        0 2023-04-11 16:18:51.242676 stpyvista-0.0.8/src/
+drwxrwxr-x   0 edwin     (1000) edwin     (1000)        0 2023-04-11 16:18:51.242676 stpyvista-0.0.8/src/stpyvista/
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)     3760 2023-03-30 13:25:16.000000 stpyvista-0.0.8/src/stpyvista/__init__.py
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)       74 2022-10-11 00:08:17.000000 stpyvista-0.0.8/src/stpyvista/__main__.py
+drwxrwxr-x   0 edwin     (1000) edwin     (1000)        0 2023-04-11 16:18:51.246677 stpyvista-0.0.8/src/stpyvista/frontend/
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)      631 2022-11-06 19:43:06.000000 stpyvista-0.0.8/src/stpyvista/frontend/index.html
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)     2021 2023-03-30 13:18:38.000000 stpyvista-0.0.8/src/stpyvista/frontend/main.js
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)     1198 2023-03-10 15:57:04.000000 stpyvista-0.0.8/src/stpyvista/frontend/streamlit-component-lib.js
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)      166 2023-03-09 01:49:59.000000 stpyvista-0.0.8/src/stpyvista/frontend/style.css
+drwxrwxr-x   0 edwin     (1000) edwin     (1000)        0 2023-04-11 16:18:51.242676 stpyvista-0.0.8/src/stpyvista.egg-info/
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)     2548 2023-04-11 16:18:51.000000 stpyvista-0.0.8/src/stpyvista.egg-info/PKG-INFO
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)      437 2023-04-11 16:18:51.000000 stpyvista-0.0.8/src/stpyvista.egg-info/SOURCES.txt
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)        1 2023-04-11 16:18:51.000000 stpyvista-0.0.8/src/stpyvista.egg-info/dependency_links.txt
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)       38 2023-04-11 16:18:51.000000 stpyvista-0.0.8/src/stpyvista.egg-info/requires.txt
+-rw-rw-r--   0 edwin     (1000) edwin     (1000)       10 2023-04-11 16:18:51.000000 stpyvista-0.0.8/src/stpyvista.egg-info/top_level.txt
```

### Comparing `stpyvista-0.0.7/LICENSE` & `stpyvista-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `stpyvista-0.0.7/PKG-INFO` & `stpyvista-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stpyvista
-Version: 0.0.7
+Version: 0.0.8
 Summary: Streamlit component that allows you to show PyVista 3d visualizations
 Author: Edwin S
 Author-email: Edwin S <esaavedrac@u.northwestern.edu>
 Project-URL: Homepage, https://github.com/edsaac/streamlit-PyVista-viewer
 Project-URL: Bug Tracker, https://github.com/edsaac/streamlit-PyVista-viewer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -42,27 +42,35 @@
 mesh = pv.Cube(center=(0,0,0))
 
 ## Add some scalar field associated to the mesh
 mesh['myscalar'] = mesh.points[:, 2]*mesh.points[:, 0]
 
 ## Add mesh to the plotter
 plotter.add_mesh(mesh, scalars='myscalar', cmap='bwr', line_width=1)
+plotter.add_scalar_bar()
 
 ## Final touches
 plotter.view_isometric()
 plotter.background_color = 'white'
 
 ## Pass a key to avoid re-rendering at each time something changes in the page
 stpyvista(plotter, key="pv_cube")
 ```
 
 ## Log changes
 
 <details>
 <summary>
+v 0.0.8
+</summary>
+- Remove excessive whitespace below the rendered component.
+- Can pass additional kwargs to panel.pane.vtk, e.g. setting an orientation_widget. Check panel-vtk for details on valid kwargs.
+</details>
+
+<summary>
 v 0.0.6
 </summary>
 - Replaced pythreejs backend for panel backend. This is a temporary solution as pyvista will remove panel support in favor of trame.
 </details>
 
 <details>
 <summary>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: stpyvista Version: 0.0.7 Summary: Streamlit
+Metadata-Version: 2.1 Name: stpyvista Version: 0.0.8 Summary: Streamlit
 component that allows you to show PyVista 3d visualizations Author: Edwin S
 Author-email: Edwin S
 u.northwestern.edu> Project-URL: Homepage, https://github.com/edsaac/streamlit-
 PyVista-viewer Project-URL: Bug Tracker, https://github.com/edsaac/streamlit-
 PyVista-viewer/issues Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.8 Description-Content-Type: text/
@@ -11,18 +11,21 @@
 stpyvista ``` ## Usage instructions [Streamlit_Cloud] ```python import
 streamlit as st import pyvista as pv from stpyvista import stpyvista #
 pythreejs does not support scalar bars :( pv.global_theme.show_scalar_bar =
 False ## Initialize a plotter object plotter = pv.Plotter(window_size=
 [400,400]) ## Create a mesh with a cube mesh = pv.Cube(center=(0,0,0)) ## Add
 some scalar field associated to the mesh mesh['myscalar'] = mesh.points[:,
 2]*mesh.points[:, 0] ## Add mesh to the plotter plotter.add_mesh(mesh,
-scalars='myscalar', cmap='bwr', line_width=1) ## Final touches
-plotter.view_isometric() plotter.background_color = 'white' ## Pass a key to
-avoid re-rendering at each time something changes in the page stpyvista
-(plotter, key="pv_cube") ``` ## Log changes   v 0.0.6  - Replaced pythreejs
-backend for panel backend. This is a temporary solution as pyvista will remove
-panel support in favor of trame.    v 0.0.5  - Support transparent backgrounds
-to blend with streamlit's web app theme. - Add a control to spin along a
-certain axis the first mesh passed to the plotter.    v 0.0.4  - Pass a key to
-the stpyvista component to avoid re-rendering at every streamlit interaction -
-Using ipywidgets `embed_minimal_html` directly instead of pyvista
-`export_html`. - Update examples as a multipage streamlit app
+scalars='myscalar', cmap='bwr', line_width=1) plotter.add_scalar_bar() ## Final
+touches plotter.view_isometric() plotter.background_color = 'white' ## Pass a
+key to avoid re-rendering at each time something changes in the page stpyvista
+(plotter, key="pv_cube") ``` ## Log changes   v 0.0.8  - Remove excessive
+whitespace below the rendered component. - Can pass additional kwargs to
+panel.pane.vtk, e.g. setting an orientation_widget. Check panel-vtk for details
+on valid kwargs.   v 0.0.6  - Replaced pythreejs backend for panel backend.
+This is a temporary solution as pyvista will remove panel support in favor of
+trame.    v 0.0.5  - Support transparent backgrounds to blend with streamlit's
+web app theme. - Add a control to spin along a certain axis the first mesh
+passed to the plotter.    v 0.0.4  - Pass a key to the stpyvista component to
+avoid re-rendering at every streamlit interaction - Using ipywidgets
+`embed_minimal_html` directly instead of pyvista `export_html`. - Update
+examples as a multipage streamlit app
```

### Comparing `stpyvista-0.0.7/README.md` & `stpyvista-0.0.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -27,27 +27,35 @@
 mesh = pv.Cube(center=(0,0,0))
 
 ## Add some scalar field associated to the mesh
 mesh['myscalar'] = mesh.points[:, 2]*mesh.points[:, 0]
 
 ## Add mesh to the plotter
 plotter.add_mesh(mesh, scalars='myscalar', cmap='bwr', line_width=1)
+plotter.add_scalar_bar()
 
 ## Final touches
 plotter.view_isometric()
 plotter.background_color = 'white'
 
 ## Pass a key to avoid re-rendering at each time something changes in the page
 stpyvista(plotter, key="pv_cube")
 ```
 
 ## Log changes
 
 <details>
 <summary>
+v 0.0.8
+</summary>
+- Remove excessive whitespace below the rendered component.
+- Can pass additional kwargs to panel.pane.vtk, e.g. setting an orientation_widget. Check panel-vtk for details on valid kwargs.
+</details>
+
+<summary>
 v 0.0.6
 </summary>
 - Replaced pythreejs backend for panel backend. This is a temporary solution as pyvista will remove panel support in favor of trame.
 </details>
 
 <details>
 <summary>
```

#### html2text {}

```diff
@@ -2,18 +2,21 @@
 Installation instructions ```sh pip install stpyvista ``` ## Usage instructions
 [Streamlit_Cloud] ```python import streamlit as st import pyvista as pv from
 stpyvista import stpyvista # pythreejs does not support scalar bars :
 ( pv.global_theme.show_scalar_bar = False ## Initialize a plotter object
 plotter = pv.Plotter(window_size=[400,400]) ## Create a mesh with a cube mesh =
 pv.Cube(center=(0,0,0)) ## Add some scalar field associated to the mesh mesh
 ['myscalar'] = mesh.points[:, 2]*mesh.points[:, 0] ## Add mesh to the plotter
-plotter.add_mesh(mesh, scalars='myscalar', cmap='bwr', line_width=1) ## Final
-touches plotter.view_isometric() plotter.background_color = 'white' ## Pass a
-key to avoid re-rendering at each time something changes in the page stpyvista
-(plotter, key="pv_cube") ``` ## Log changes   v 0.0.6  - Replaced pythreejs
-backend for panel backend. This is a temporary solution as pyvista will remove
-panel support in favor of trame.    v 0.0.5  - Support transparent backgrounds
-to blend with streamlit's web app theme. - Add a control to spin along a
-certain axis the first mesh passed to the plotter.    v 0.0.4  - Pass a key to
-the stpyvista component to avoid re-rendering at every streamlit interaction -
-Using ipywidgets `embed_minimal_html` directly instead of pyvista
-`export_html`. - Update examples as a multipage streamlit app
+plotter.add_mesh(mesh, scalars='myscalar', cmap='bwr', line_width=1)
+plotter.add_scalar_bar() ## Final touches plotter.view_isometric()
+plotter.background_color = 'white' ## Pass a key to avoid re-rendering at each
+time something changes in the page stpyvista(plotter, key="pv_cube") ``` ## Log
+changes   v 0.0.8  - Remove excessive whitespace below the rendered component.
+- Can pass additional kwargs to panel.pane.vtk, e.g. setting an
+orientation_widget. Check panel-vtk for details on valid kwargs.   v 0.0.6  -
+Replaced pythreejs backend for panel backend. This is a temporary solution as
+pyvista will remove panel support in favor of trame.    v 0.0.5  - Support
+transparent backgrounds to blend with streamlit's web app theme. - Add a
+control to spin along a certain axis the first mesh passed to the plotter.    v
+0.0.4  - Pass a key to the stpyvista component to avoid re-rendering at every
+streamlit interaction - Using ipywidgets `embed_minimal_html` directly instead
+of pyvista `export_html`. - Update examples as a multipage streamlit app
```

### Comparing `stpyvista-0.0.7/pyproject.toml` & `stpyvista-0.0.8/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stpyvista"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Edwin S", email="esaavedrac@u.northwestern.edu" },
 ]
 description = "Streamlit component that allows you to show PyVista 3d visualizations"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `stpyvista-0.0.7/setup.py` & `stpyvista-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="stpyvista",
-    version="0.0.7",
+    version="0.0.8",
     author="Edwin S",
     author_email="esaavedrac@u.northwestern.edu",
     description="Streamlit component that allows you to visualize pyvista 3D visualizations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     package_dir={"": "src"},
```

### Comparing `stpyvista-0.0.7/src/stpyvista/__init__.py` & `stpyvista-0.0.8/src/stpyvista/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,52 +49,70 @@
     """ Unsupported format for input? """
     pass
 
 # Create the python function that will be called from the front end
 def stpyvista(
     plotter : pv.Plotter,
     horizontal_align : str = "center",
+    panel_kwargs = None,
     key: Optional[str] = None
     ) -> None:
 
     """
     Renders a HTML_stpyvista as a threejs model.
     
     Parameters
     ----------
     input: Union[pv.Plotter, HTML_stpyvista]
         Plotter to render
     
     horizontal_align: str = "center"
         Either "center", "left" or "right"
 
+    panel_kwargs: dict | None
+        Optional keyword parameters to pass to pn.panel() Check: 
+        https://panel.holoviz.org/api/panel.pane.vtk.html for details. Here is
+        a useful one:
+        
+        orientation_widget: bool
+            Show the xyz axis indicator
+
+
     key: str|None
         An optional key that uniquely identifies this component. If this is
         None, and the component's arguments are changed, the component will
         be re-mounted in the Streamlit frontend and lose its current state.
     
     Returns
     -------
     None
     """
 
     if isinstance(plotter, pv.Plotter): 
+
+        if panel_kwargs is None:
+            panel_kwargs = dict()
+        
         width, height = plotter.window_size
-        geo_pan_pv = pn.panel(plotter.ren_win, width=width, height=height) 
+        geo_pan_pv = pn.panel(
+            plotter.ren_win, 
+            width = width, 
+            height = height,
+            **panel_kwargs) 
         
         # Create HTML file
         model_bytes = BytesIO()
         geo_pan_pv.save(model_bytes, resources=INLINE)
         panel_html = model_bytes.getvalue().decode('utf-8')
         model_bytes.close()
 
         component_value = _component_func(
             panel_html = panel_html,
             width = width,
-            height = height+100,
+            height = height,
             horizontal_align = horizontal_align,
             key = key,
             default = 0)
 
         return component_value
 
     else:
```

### Comparing `stpyvista-0.0.7/src/stpyvista/frontend/index.html` & `stpyvista-0.0.8/src/stpyvista/frontend/index.html`

 * *Files identical despite different names*

### Comparing `stpyvista-0.0.7/src/stpyvista/frontend/main.js` & `stpyvista-0.0.8/src/stpyvista/frontend/main.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -24,28 +24,29 @@
             height,
             horizontal_align,
             key
         } = event.detail.args;
         const stpyvistadiv = document.getElementById("stpyvistadiv");
         const stpyvistaframe = document.getElementById("stpyvistaframe");
 
-        // Style the wrapping div for the iframe
-        stpyvistadiv.style.width = width + 15;
-        stpyvistadiv.style.textAlign = horizontal_align;
 
         // Overwrite default iframe dimensions and put model in the iframe
         // just CSS styling does not apply to the iframe
         stpyvistaframe.srcdoc = panel_html;
-        stpyvistaframe.width = width + 15;
-        console.log("WIDTH", width)
+        stpyvistaframe.width = width + 24;
+        stpyvistaframe.height = height + 20;
+        stpyvistaframe.scrolling = "yes";
+        // console.log("WIDTH", width)
+
+        // Style the wrapping div for the iframe
+        // stpyvistadiv.style.width = stpyvistaframe.width + 10;
+        stpyvistadiv.style.textAlign = horizontal_align;
 
-        stpyvistaframe.height = height + 15;
-        Streamlit.setFrameHeight(height + 40)
-        console.log("HEIGHT", width)
-        stpyvistaframe.scrolling = "no";
+        // console.log("HEIGHT", height)
+        Streamlit.setFrameHeight(height + 50);
         stpyvistaframe.style.border = "2px red";
 
         // Send some value to python 
         // Not very useful at the moment but keep it for later
         // stpyvistadiv.addEventListener('click', event => sendValue(50), false);
 
         window.rendered = true;
```

### Comparing `stpyvista-0.0.7/src/stpyvista/frontend/streamlit-component-lib.js` & `stpyvista-0.0.8/src/stpyvista/frontend/streamlit-component-lib.js`

 * *Files identical despite different names*

### Comparing `stpyvista-0.0.7/src/stpyvista.egg-info/PKG-INFO` & `stpyvista-0.0.8/src/stpyvista.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stpyvista
-Version: 0.0.7
+Version: 0.0.8
 Summary: Streamlit component that allows you to show PyVista 3d visualizations
 Author: Edwin S
 Author-email: Edwin S <esaavedrac@u.northwestern.edu>
 Project-URL: Homepage, https://github.com/edsaac/streamlit-PyVista-viewer
 Project-URL: Bug Tracker, https://github.com/edsaac/streamlit-PyVista-viewer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -42,27 +42,35 @@
 mesh = pv.Cube(center=(0,0,0))
 
 ## Add some scalar field associated to the mesh
 mesh['myscalar'] = mesh.points[:, 2]*mesh.points[:, 0]
 
 ## Add mesh to the plotter
 plotter.add_mesh(mesh, scalars='myscalar', cmap='bwr', line_width=1)
+plotter.add_scalar_bar()
 
 ## Final touches
 plotter.view_isometric()
 plotter.background_color = 'white'
 
 ## Pass a key to avoid re-rendering at each time something changes in the page
 stpyvista(plotter, key="pv_cube")
 ```
 
 ## Log changes
 
 <details>
 <summary>
+v 0.0.8
+</summary>
+- Remove excessive whitespace below the rendered component.
+- Can pass additional kwargs to panel.pane.vtk, e.g. setting an orientation_widget. Check panel-vtk for details on valid kwargs.
+</details>
+
+<summary>
 v 0.0.6
 </summary>
 - Replaced pythreejs backend for panel backend. This is a temporary solution as pyvista will remove panel support in favor of trame.
 </details>
 
 <details>
 <summary>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: stpyvista Version: 0.0.7 Summary: Streamlit
+Metadata-Version: 2.1 Name: stpyvista Version: 0.0.8 Summary: Streamlit
 component that allows you to show PyVista 3d visualizations Author: Edwin S
 Author-email: Edwin S
 u.northwestern.edu> Project-URL: Homepage, https://github.com/edsaac/streamlit-
 PyVista-viewer Project-URL: Bug Tracker, https://github.com/edsaac/streamlit-
 PyVista-viewer/issues Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.8 Description-Content-Type: text/
@@ -11,18 +11,21 @@
 stpyvista ``` ## Usage instructions [Streamlit_Cloud] ```python import
 streamlit as st import pyvista as pv from stpyvista import stpyvista #
 pythreejs does not support scalar bars :( pv.global_theme.show_scalar_bar =
 False ## Initialize a plotter object plotter = pv.Plotter(window_size=
 [400,400]) ## Create a mesh with a cube mesh = pv.Cube(center=(0,0,0)) ## Add
 some scalar field associated to the mesh mesh['myscalar'] = mesh.points[:,
 2]*mesh.points[:, 0] ## Add mesh to the plotter plotter.add_mesh(mesh,
-scalars='myscalar', cmap='bwr', line_width=1) ## Final touches
-plotter.view_isometric() plotter.background_color = 'white' ## Pass a key to
-avoid re-rendering at each time something changes in the page stpyvista
-(plotter, key="pv_cube") ``` ## Log changes   v 0.0.6  - Replaced pythreejs
-backend for panel backend. This is a temporary solution as pyvista will remove
-panel support in favor of trame.    v 0.0.5  - Support transparent backgrounds
-to blend with streamlit's web app theme. - Add a control to spin along a
-certain axis the first mesh passed to the plotter.    v 0.0.4  - Pass a key to
-the stpyvista component to avoid re-rendering at every streamlit interaction -
-Using ipywidgets `embed_minimal_html` directly instead of pyvista
-`export_html`. - Update examples as a multipage streamlit app
+scalars='myscalar', cmap='bwr', line_width=1) plotter.add_scalar_bar() ## Final
+touches plotter.view_isometric() plotter.background_color = 'white' ## Pass a
+key to avoid re-rendering at each time something changes in the page stpyvista
+(plotter, key="pv_cube") ``` ## Log changes   v 0.0.8  - Remove excessive
+whitespace below the rendered component. - Can pass additional kwargs to
+panel.pane.vtk, e.g. setting an orientation_widget. Check panel-vtk for details
+on valid kwargs.   v 0.0.6  - Replaced pythreejs backend for panel backend.
+This is a temporary solution as pyvista will remove panel support in favor of
+trame.    v 0.0.5  - Support transparent backgrounds to blend with streamlit's
+web app theme. - Add a control to spin along a certain axis the first mesh
+passed to the plotter.    v 0.0.4  - Pass a key to the stpyvista component to
+avoid re-rendering at every streamlit interaction - Using ipywidgets
+`embed_minimal_html` directly instead of pyvista `export_html`. - Update
+examples as a multipage streamlit app
```

