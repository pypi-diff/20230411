# Comparing `tmp/bcrpy-1.1.4.tar.gz` & `tmp/bcrpy-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcrpy-1.1.4.tar", max compression
+gzip compressed data, was "bcrpy-1.1.5.tar", max compression
```

## Comparing `bcrpy-1.1.4.tar` & `bcrpy-1.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1080 2023-03-13 04:47:05.859626 bcrpy-1.1.4/LICENSE
--rw-r--r--   0        0        0     1422 2023-03-29 02:42:38.498886 bcrpy-1.1.4/README.md
--rw-r--r--   0        0        0       50 2023-03-14 02:59:53.153055 bcrpy-1.1.4/bcrpy/__init__.py
--rw-r--r--   0        0        0     3502 2023-03-29 03:07:57.005455 bcrpy-1.1.4/bcrpy/anexo.py
--rw-r--r--   0        0        0    12281 2023-03-29 02:38:23.187507 bcrpy-1.1.4/bcrpy/main.py
--rw-r--r--   0        0        0      576 2023-03-29 04:13:52.110218 bcrpy-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     2369 1970-01-01 00:00:00.000000 bcrpy-1.1.4/setup.py
--rw-r--r--   0        0        0     2386 1970-01-01 00:00:00.000000 bcrpy-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-03-13 04:47:05.859626 bcrpy-1.1.5/LICENSE
+-rw-r--r--   0        0        0     1422 2023-03-29 02:42:38.498886 bcrpy-1.1.5/README.md
+-rw-r--r--   0        0        0       50 2023-03-14 02:59:53.153055 bcrpy-1.1.5/bcrpy/__init__.py
+-rw-r--r--   0        0        0     3502 2023-03-29 03:07:57.005455 bcrpy-1.1.5/bcrpy/anexo.py
+-rw-r--r--   0        0        0    12277 2023-04-11 17:27:50.917119 bcrpy-1.1.5/bcrpy/main.py
+-rw-r--r--   0        0        0      576 2023-04-11 17:28:07.340240 bcrpy-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2369 1970-01-01 00:00:00.000000 bcrpy-1.1.5/setup.py
+-rw-r--r--   0        0        0     2386 1970-01-01 00:00:00.000000 bcrpy-1.1.5/PKG-INFO
```

### Comparing `bcrpy-1.1.4/LICENSE` & `bcrpy-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bcrpy-1.1.4/README.md` & `bcrpy-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `bcrpy-1.1.4/bcrpy/anexo.py` & `bcrpy-1.1.5/bcrpy/anexo.py`

 * *Files identical despite different names*

### Comparing `bcrpy-1.1.4/bcrpy/main.py` & `bcrpy-1.1.5/bcrpy/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         '''Este es el marco principal para almacenar variables y ejecutar metodos para extraer, buscar y manejar datos. 
 
         Parametros
         ----------
         metadata: pandas.DataFrame
             Los metadatos de las series estadísticas del BRCPData, los cuales pueden ser reducidos con el metodo ref_metadata de esta `class`. 
         data: pandas.DataFrame
-            Los datos extraidos del BRCPData de acuerdo a la informacion declarada en las variables constructoras (vea metodo `state_inputs()`) con el metodo `GET()` de esta clase.  
+            Los datos extraidos del BRCPData de acuerdo a la informacion declarada en las variables constructoras (vea metodo `parametros()`) con el metodo `GET()` de esta clase.  
         codigos : list(str)
             lista de codigos de series en interes para usar con los metodos de esta `class`. 
         formato : str
             formato para extraer / procesar datos (predeterminado: json)
         fechaini : str
             fecha de inicio para la(s) serie(s) seleccionada(s) en mes año (A) y mes (M) (formato AAAA-M)
         fechafin : str
@@ -39,15 +39,15 @@
         self.data = pandas.DataFrame([])
         self.codigos = ['PN01288PM','PN01289PM']
         self.formato = 'json'
         self.fechaini = '2010-1'
         self.fechafin = '2016-9'
         self.idioma = 'ing'
 
-    def state_inputs(self):
+    def parametros(self):
         '''Declara el estado actual de todas las variables constructoras de la clase Marco. 
         '''
 
         print('''corriendo estado actual de todas las variables constructoras...\n
 objeto.metadata = {}
 objeto.codigos = {}
 objeto.formato = {}
```

### Comparing `bcrpy-1.1.4/pyproject.toml` & `bcrpy-1.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bcrpy"
-version = "1.1.4"
+version = "1.1.5"
 description = "Un cliente API para la extraccion, consulta y analisis de la base de datos BCRPData del Banco Central de Reserva del Peru (BCRP)"
 authors = ["andrewrgarcia <garcia.gtr@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `bcrpy-1.1.4/setup.py` & `bcrpy-1.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'requests>=2.28.2,<3.0.0',
  'sphinx>=6.1.3,<7.0.0',
  'tabulate>=0.9.0,<0.10.0',
  'tqdm>=4.65.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'bcrpy',
-    'version': '1.1.4',
+    'version': '1.1.5',
     'description': 'Un cliente API para la extraccion, consulta y analisis de la base de datos BCRPData del Banco Central de Reserva del Peru (BCRP)',
     'long_description': '# bcrpy\n\n[![](docs/img/icon_bcrpy.png)](https://bcrpy.readthedocs.io/en/latest/)\n\n\nUn cliente API para la extraccion, consulta y analisis de la base de datos [BCRPData](https://estadisticas.bcrp.gob.pe/estadisticas/series/) del [Banco Central de Reserva del Peru (BCRP)](https://www.bcrp.gob.pe/) escrito para Python. Este cliente es un _wrapper_ de la [API para Desarrolladores](https://estadisticas.bcrp.gob.pe/estadisticas/series/ayuda/api) del BCRP.\n\n![](docs/img/icon_bcrp.png)\n\n## Vinculos \n\n[Documentación en linea (readthedocs)](https://bcrpy.readthedocs.io/en/latest/) \n\n[Manual bcrpy (pdf)](https://raw.githubusercontent.com/andrewrgarcia/bcrpy/main/bcrpy.pdf)\n\n[pip package index](https://pypi.org/project/bcrpy/) \n\n# Instalacion\n\nEn su sistema local (laptop o computadora) bcrpy puede ser instalada con el comando pip install bcrpy. Aun asi, se\nrecomienda instalar bcrpy dentro de un ambiente virtual virtualenv. El protocolo para aquel seria el siguiente:\n\n\n```ruby\nvirtualenv venv\nsource venv/bin/activate\npip install bcrpy\n```\n\nbcrpy ha sido desarrollado con un protocolo de programación orientada a objetos (tambien conocido como *Object\nOriented Programming (OOP)*) lo cual se reduce a que objetos pueden ser usados a almacenar metodos (funciones),\ndatos, y su manejo de aquellos.\n\n\n[![](docs/img/colaboratory.svg)](https://colab.research.google.com/drive/1YdyCYeU0S98428WgBg4n9Ad9auKrurQZ?usp=sharing)\n',
     'author': 'andrewrgarcia',
     'author_email': 'garcia.gtr@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `bcrpy-1.1.4/PKG-INFO` & `bcrpy-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcrpy
-Version: 1.1.4
+Version: 1.1.5
 Summary: Un cliente API para la extraccion, consulta y analisis de la base de datos BCRPData del Banco Central de Reserva del Peru (BCRP)
 License: MIT
 Author: andrewrgarcia
 Author-email: garcia.gtr@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

