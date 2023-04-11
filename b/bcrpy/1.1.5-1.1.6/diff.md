# Comparing `tmp/bcrpy-1.1.5.tar.gz` & `tmp/bcrpy-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcrpy-1.1.5.tar", max compression
+gzip compressed data, was "bcrpy-1.1.6.tar", max compression
```

## Comparing `bcrpy-1.1.5.tar` & `bcrpy-1.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1080 2023-03-13 04:47:05.859626 bcrpy-1.1.5/LICENSE
--rw-r--r--   0        0        0     1422 2023-03-29 02:42:38.498886 bcrpy-1.1.5/README.md
--rw-r--r--   0        0        0       50 2023-03-14 02:59:53.153055 bcrpy-1.1.5/bcrpy/__init__.py
--rw-r--r--   0        0        0     3502 2023-03-29 03:07:57.005455 bcrpy-1.1.5/bcrpy/anexo.py
--rw-r--r--   0        0        0    12277 2023-04-11 17:27:50.917119 bcrpy-1.1.5/bcrpy/main.py
--rw-r--r--   0        0        0      576 2023-04-11 17:28:07.340240 bcrpy-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     2369 1970-01-01 00:00:00.000000 bcrpy-1.1.5/setup.py
--rw-r--r--   0        0        0     2386 1970-01-01 00:00:00.000000 bcrpy-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-03-13 04:47:05.859626 bcrpy-1.1.6/LICENSE
+-rw-r--r--   0        0        0     1422 2023-03-29 02:42:38.498886 bcrpy-1.1.6/README.md
+-rw-r--r--   0        0        0       50 2023-03-14 02:59:53.153055 bcrpy-1.1.6/bcrpy/__init__.py
+-rw-r--r--   0        0        0     3502 2023-03-29 03:07:57.005455 bcrpy-1.1.6/bcrpy/anexo.py
+-rw-r--r--   0        0        0    12981 2023-04-11 21:11:59.125812 bcrpy-1.1.6/bcrpy/main.py
+-rw-r--r--   0        0        0      617 2023-04-11 21:14:06.613541 bcrpy-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2424 1970-01-01 00:00:00.000000 bcrpy-1.1.6/setup.py
+-rw-r--r--   0        0        0     2469 1970-01-01 00:00:00.000000 bcrpy-1.1.6/PKG-INFO
```

### Comparing `bcrpy-1.1.5/LICENSE` & `bcrpy-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bcrpy-1.1.5/README.md` & `bcrpy-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `bcrpy-1.1.5/bcrpy/anexo.py` & `bcrpy-1.1.6/bcrpy/anexo.py`

 * *Files identical despite different names*

### Comparing `bcrpy-1.1.5/bcrpy/main.py` & `bcrpy-1.1.6/bcrpy/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 
 from tqdm import tqdm
 from time import sleep
 
 import matplotlib.pyplot as plt 
 from bcrpy.anexo import Levenshtein
 
+from termcolor import colored, cprint
+from colorama import just_fix_windows_console
+just_fix_windows_console()
 
 class Marco:
     def __init__(self):
         '''Este es el marco principal para almacenar variables y ejecutar metodos para extraer, buscar y manejar datos. 
 
         Parametros
         ----------
@@ -42,28 +45,34 @@
         self.fechaini = '2010-1'
         self.fechafin = '2016-9'
         self.idioma = 'ing'
 
     def parametros(self):
         '''Declara el estado actual de todas las variables constructoras de la clase Marco. 
         '''
+        
+        decoration = colored("Estado actual de parametros constructores del objeto:", "green")
+
 
-        print('''corriendo estado actual de todas las variables constructoras...\n
+        text = '''
 objeto.metadata = {}
 objeto.codigos = {}
 objeto.formato = {}
 objeto.fechaini = {}
 objeto.fechafin = {}
 objeto.idioma = {}
 '''.format('<vacio>' if len(self.metadata)==0 else str(type(self.metadata))+' size: '+str(self.metadata.shape),
         self.codigos,
         self.formato,
         self.fechaini, 
         self.fechafin,
-        self.idioma))
+        self.idioma)
+
+        print(decoration)
+        print(text)
 
 
     def get_metadata(self, filename='metadata.csv'): 
         '''Extrae todos los metadatos de BCRPData. 
         
         Parametros
         ----------
@@ -108,19 +117,23 @@
         ----------
         codigo : str
             Nombre de codigo de series a consultar
         '''
         self.get_metadata() if len(self.metadata) == 0 else None
         df = self.metadata
 
-
-        print('corriendo query para {}...\n'.format(codigo))
+        # print('corriendo query para {}...\n'.format(codigo))
+        print(colored('corriendo query para {}...\n'.format(codigo), "green"))
 
         index = df.index[df.iloc[:,0] == codigo].tolist()
-        print('{} es indice {} en metadatos'.format(codigo, index[0]))
+        # print('{} es indice {} en metadatos'.format(codigo, index[0]))
+        # print(colored(codigo, "blue",attrs=["bold"]),end=" ")
+        cprint(codigo, "white", "on_green",end=" ")
+
+        print('es indice {} en metadatos'.format(index[0]))
 
         dict = self.metadata.loc[index].to_dict()
         for i in dict.keys():
             dict[i] = dict[i][index[0]]
         dict.pop("Unnamed: 13" ) if "Unnamed: 13" in dict.keys() else None
 
         jsondata = json.dumps(dict,indent = 8,ensure_ascii=False)
@@ -128,15 +141,14 @@
         return jsondata
     
     def querydict(self,codigo='PD39793AM'):
 
         self.get_metadata() if len(self.metadata) == 0 else None
         df = self.metadata
 
-
         # print('corriendo query para {}...\n'.format(codigo))
 
         index = df.index[df.iloc[:,0] == codigo].tolist()
         # print('{} es indice {} en metadatos'.format(codigo, index[0]))
 
         dict = self.metadata.loc[index].to_dict()
         for i in dict.keys():
@@ -152,22 +164,22 @@
         Parametros
         ----------
         keyword : str
             Palabra clave para reducir los metadatos
         cutoff : float
             Este es el Levenshtein similarity ratio (predeterminado=0.65). Un cutoff de 1.00 solo regresara metadatos que contienen palabras que coinciden con la palabra clave al 100%.
         columnas : str
-            Indices de columnas de los metadatos seleccionados para correr el metodo. Predeterminado='all' corre el metodo en todas las columnas. 
+            Indices de columnas de los metadatos seleccionados para correr el metodo. Predeterminado='all' corre el metodo en todas las columnas. Seleccion por indice: e.g. [0,2,4] busca en la primera, tercera, y quinta columna. 
         '''
 
-        print('corriendo wordsearch: `{}`'.format(keyword))
-        print('cutoff =',cutoff, end='')
+        print('\nBusqueda difusa de palabra: `{}`'.format(keyword))
+        print('cutoff (tolerancia) =',cutoff, end='')
         print('; columnas =',"`"+columnas+"`(todas)" if columnas=='all' else columnas)
         # print('*medido con Levenshtein similarity ratio')
-        print('por favor esperar...\n')
+        print(colored('corriendo wordsearch...', "green", attrs=["blink"]))
 
         INDICES = []
         self.get_metadata() if len(self.metadata) == 0 else None
         df= self.metadata
 
         'placeholder dataframes (so that nothing gets overwritten)'
         new_df = df.copy()
@@ -258,15 +270,18 @@
         format = self.formato 
         code_series = '-'.join(self.codigos)
         period = '{}/{}'.format(self.fechaini,self.fechafin) 
         language = self.idioma
 
         url = "{}/{}/{}/{}/{}".format(root,code_series,format,period,language)
 
-        'https://www.geeksforgeeks.org/response-json-python-requests/'
+        print('URL:')
+        print(url)
+
+        print(colored('Obteniendo información con la URL de arriba usando requests.get. Por favor espere...',"green", attrs=["blink"]))
         response = requests.get(url)
 
         dict  = response.json()
 
         header = [k['name'] for k in dict['config']['series'] ]
         df = pandas.DataFrame(columns=header) # aqui todavia no se han insertado los datos en las filas
```

### Comparing `bcrpy-1.1.5/pyproject.toml` & `bcrpy-1.1.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bcrpy"
-version = "1.1.5"
+version = "1.1.6"
 description = "Un cliente API para la extraccion, consulta y analisis de la base de datos BCRPData del Banco Central de Reserva del Peru (BCRP)"
 authors = ["andrewrgarcia <garcia.gtr@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -12,12 +12,14 @@
 numpy = "^1.24.2"
 pandas = "^1.5.3"
 tqdm = "^4.65.0"
 matplotlib = "^3.7.1"
 sphinx = "^6.1.3"
 iteration-utilities = "^0.11.0"
 tabulate = "^0.9.0"
+termcolor = "^2.2.0"
+colorama = "^0.4.6"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `bcrpy-1.1.5/setup.py` & `bcrpy-1.1.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 packages = \
 ['bcrpy']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['iteration-utilities>=0.11.0,<0.12.0',
+['colorama>=0.4.6,<0.5.0',
+ 'iteration-utilities>=0.11.0,<0.12.0',
  'matplotlib>=3.7.1,<4.0.0',
  'numpy>=1.24.2,<2.0.0',
  'pandas>=1.5.3,<2.0.0',
  'requests>=2.28.2,<3.0.0',
  'sphinx>=6.1.3,<7.0.0',
  'tabulate>=0.9.0,<0.10.0',
+ 'termcolor>=2.2.0,<3.0.0',
  'tqdm>=4.65.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'bcrpy',
-    'version': '1.1.5',
+    'version': '1.1.6',
     'description': 'Un cliente API para la extraccion, consulta y analisis de la base de datos BCRPData del Banco Central de Reserva del Peru (BCRP)',
     'long_description': '# bcrpy\n\n[![](docs/img/icon_bcrpy.png)](https://bcrpy.readthedocs.io/en/latest/)\n\n\nUn cliente API para la extraccion, consulta y analisis de la base de datos [BCRPData](https://estadisticas.bcrp.gob.pe/estadisticas/series/) del [Banco Central de Reserva del Peru (BCRP)](https://www.bcrp.gob.pe/) escrito para Python. Este cliente es un _wrapper_ de la [API para Desarrolladores](https://estadisticas.bcrp.gob.pe/estadisticas/series/ayuda/api) del BCRP.\n\n![](docs/img/icon_bcrp.png)\n\n## Vinculos \n\n[Documentación en linea (readthedocs)](https://bcrpy.readthedocs.io/en/latest/) \n\n[Manual bcrpy (pdf)](https://raw.githubusercontent.com/andrewrgarcia/bcrpy/main/bcrpy.pdf)\n\n[pip package index](https://pypi.org/project/bcrpy/) \n\n# Instalacion\n\nEn su sistema local (laptop o computadora) bcrpy puede ser instalada con el comando pip install bcrpy. Aun asi, se\nrecomienda instalar bcrpy dentro de un ambiente virtual virtualenv. El protocolo para aquel seria el siguiente:\n\n\n```ruby\nvirtualenv venv\nsource venv/bin/activate\npip install bcrpy\n```\n\nbcrpy ha sido desarrollado con un protocolo de programación orientada a objetos (tambien conocido como *Object\nOriented Programming (OOP)*) lo cual se reduce a que objetos pueden ser usados a almacenar metodos (funciones),\ndatos, y su manejo de aquellos.\n\n\n[![](docs/img/colaboratory.svg)](https://colab.research.google.com/drive/1YdyCYeU0S98428WgBg4n9Ad9auKrurQZ?usp=sharing)\n',
     'author': 'andrewrgarcia',
     'author_email': 'garcia.gtr@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `bcrpy-1.1.5/PKG-INFO` & `bcrpy-1.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: bcrpy
-Version: 1.1.5
+Version: 1.1.6
 Summary: Un cliente API para la extraccion, consulta y analisis de la base de datos BCRPData del Banco Central de Reserva del Peru (BCRP)
 License: MIT
 Author: andrewrgarcia
 Author-email: garcia.gtr@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: iteration-utilities (>=0.11.0,<0.12.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: sphinx (>=6.1.3,<7.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
+Requires-Dist: termcolor (>=2.2.0,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # bcrpy
 
 [![](docs/img/icon_bcrpy.png)](https://bcrpy.readthedocs.io/en/latest/)
```

