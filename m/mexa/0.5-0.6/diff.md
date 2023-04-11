# Comparing `tmp/mexa-0.5.tar.gz` & `tmp/mexa-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mexa-0.5.tar", last modified: Mon Apr 10 13:01:15 2023, max compression
+gzip compressed data, was "mexa-0.6.tar", last modified: Tue Apr 11 14:43:04 2023, max compression
```

## Comparing `mexa-0.5.tar` & `mexa-0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 fitorec   (1002) fitorec   (1002)        0 2023-04-10 13:01:15.350175 mexa-0.5/
--rw-rw-r--   0 fitorec   (1002) fitorec   (1002)     2650 2023-04-10 13:01:15.350175 mexa-0.5/PKG-INFO
--rw-rw-r--   0 fitorec   (1002) fitorec   (1002)     2255 2023-04-10 12:32:27.000000 mexa-0.5/README.md
-drwxrwxr-x   0 fitorec   (1002) fitorec   (1002)        0 2023-04-10 13:01:15.350175 mexa-0.5/mexa/
--rw-rw-r--   0 fitorec   (1002) fitorec   (1002)     6339 2023-04-10 12:05:44.000000 mexa-0.5/mexa/CurpField.py
--rw-rw-r--   0 fitorec   (1002) fitorec   (1002)     5088 2023-04-09 06:32:38.000000 mexa-0.5/mexa/CurpUtils.py
--rw-rw-r--   0 fitorec   (1002) fitorec   (1002)      455 2023-04-09 07:02:37.000000 mexa-0.5/mexa/ErrorMsgs.py
--rw-rw-r--   0 fitorec   (1002) fitorec   (1002)      801 2023-04-05 05:08:01.000000 mexa-0.5/mexa/Estados.py
--rw-rw-r--   0 fitorec   (1002) fitorec   (1002)     4026 2023-04-10 12:28:08.000000 mexa-0.5/mexa/NssField.py
--rw-rw-r--   0 fitorec   (1002) fitorec   (1002)      731 2023-04-06 08:12:32.000000 mexa-0.5/mexa/__init__.py
--rw-rw-r--   0 fitorec   (1002) fitorec   (1002)     1647 2023-04-09 06:59:20.000000 mexa-0.5/mexa/core.py
--rw-rw-r--   0 fitorec   (1002) fitorec   (1002)     2231 2023-04-04 05:39:25.000000 mexa-0.5/mexa/data_ladas.py
-drwxrwxr-x   0 fitorec   (1002) fitorec   (1002)        0 2023-04-10 13:01:15.350175 mexa-0.5/mexa.egg-info/
--rw-rw-r--   0 fitorec   (1002) fitorec   (1002)     2650 2023-04-10 13:01:15.000000 mexa-0.5/mexa.egg-info/PKG-INFO
--rw-rw-r--   0 fitorec   (1002) fitorec   (1002)      266 2023-04-10 13:01:15.000000 mexa-0.5/mexa.egg-info/SOURCES.txt
--rw-rw-r--   0 fitorec   (1002) fitorec   (1002)        1 2023-04-10 13:01:15.000000 mexa-0.5/mexa.egg-info/dependency_links.txt
--rw-rw-r--   0 fitorec   (1002) fitorec   (1002)        5 2023-04-10 13:01:15.000000 mexa-0.5/mexa.egg-info/top_level.txt
--rw-rw-r--   0 fitorec   (1002) fitorec   (1002)       38 2023-04-10 13:01:15.350175 mexa-0.5/setup.cfg
--rw-rw-r--   0 fitorec   (1002) fitorec   (1002)      641 2023-04-10 12:49:34.000000 mexa-0.5/setup.py
+drwxrwxr-x   0 fitorec   (1002) fitorec   (1002)        0 2023-04-11 14:43:04.702286 mexa-0.6/
+-rw-rw-r--   0 fitorec   (1002) fitorec   (1002)     4364 2023-04-11 14:43:04.702286 mexa-0.6/PKG-INFO
+-rw-rw-r--   0 fitorec   (1002) fitorec   (1002)     3969 2023-04-11 14:07:28.000000 mexa-0.6/README.md
+drwxrwxr-x   0 fitorec   (1002) fitorec   (1002)        0 2023-04-11 14:43:04.698285 mexa-0.6/mexa/
+-rw-rw-r--   0 fitorec   (1002) fitorec   (1002)     6666 2023-04-11 14:34:40.000000 mexa-0.6/mexa/CurpField.py
+-rw-rw-r--   0 fitorec   (1002) fitorec   (1002)     5595 2023-04-10 21:58:45.000000 mexa-0.6/mexa/CurpUtils.py
+-rw-rw-r--   0 fitorec   (1002) fitorec   (1002)      694 2023-04-10 21:14:42.000000 mexa-0.6/mexa/ErrorMsgs.py
+-rw-rw-r--   0 fitorec   (1002) fitorec   (1002)      801 2023-04-05 05:08:01.000000 mexa-0.6/mexa/Estados.py
+-rw-rw-r--   0 fitorec   (1002) fitorec   (1002)     4302 2023-04-11 14:12:40.000000 mexa-0.6/mexa/NssField.py
+-rw-rw-r--   0 fitorec   (1002) fitorec   (1002)      823 2023-04-10 23:47:57.000000 mexa-0.6/mexa/__init__.py
+-rw-rw-r--   0 fitorec   (1002) fitorec   (1002)     2525 2023-04-11 14:42:16.000000 mexa-0.6/mexa/core.py
+-rw-rw-r--   0 fitorec   (1002) fitorec   (1002)     2231 2023-04-04 05:39:25.000000 mexa-0.6/mexa/data_ladas.py
+drwxrwxr-x   0 fitorec   (1002) fitorec   (1002)        0 2023-04-11 14:43:04.698285 mexa-0.6/mexa.egg-info/
+-rw-rw-r--   0 fitorec   (1002) fitorec   (1002)     4364 2023-04-11 14:43:04.000000 mexa-0.6/mexa.egg-info/PKG-INFO
+-rw-rw-r--   0 fitorec   (1002) fitorec   (1002)      266 2023-04-11 14:43:04.000000 mexa-0.6/mexa.egg-info/SOURCES.txt
+-rw-rw-r--   0 fitorec   (1002) fitorec   (1002)        1 2023-04-11 14:43:04.000000 mexa-0.6/mexa.egg-info/dependency_links.txt
+-rw-rw-r--   0 fitorec   (1002) fitorec   (1002)        5 2023-04-11 14:43:04.000000 mexa-0.6/mexa.egg-info/top_level.txt
+-rw-rw-r--   0 fitorec   (1002) fitorec   (1002)       38 2023-04-11 14:43:04.702286 mexa-0.6/setup.cfg
+-rw-rw-r--   0 fitorec   (1002) fitorec   (1002)      641 2023-04-10 21:53:09.000000 mexa-0.6/setup.py
```

### Comparing `mexa-0.5/PKG-INFO` & `mexa-0.6/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,71 +1,104 @@
-Metadata-Version: 2.1
-Name: mexa
-Version: 0.5
-Summary: Validador y Generador de campos para tramites mexicanos
-Home-page: https://github.com/fitorec/mexa-py
-Author: @Fitorec - Miguel Angel Marcial Martinez
-Author-email: fitorec@mundosica.com
-License: MIT
-Keywords: RFC,CURP,NSS,Clabe
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
+<h1>
+<span style="color:green">M</span>ex<span style="color:red">a</span> -
+<small>Mexican Power</small>
+</h1>
 
-# Mexa 
 
-#### Generador y Verificador de campos __Mexican Power__.
+#### Generador y Verificador de campos.
 
 __Mexa__ es un validador y generador de diferentes campos, utiles para la tramitología mexicana:
 
 ### Listado de campos:
 
  - **CURP**: Clave Única de Registro de Población.
  - **Nss**: Número de Seguro Social.
  - **RFC**: Registro Federal de Contribuyentes(física y moral).
- - **Tel**: Telefonos con lada MX.
+ - **Tel**: Télefonos con lada de México.
 
+### Instalación.
+
+
+El paquete esta disponible en **pypi** (__<https://pypi.org/project/mexa/>__), para puedes instalarlo desde `pip`:
+
+```
+# Instalación de Mexa.
+pip install mexa
+```
 
 
 ### Uso:
 
 
 
 ```python
-from mexa import fake, validate, Nss, Curp
+from mexa import fake, validate, Nss, Curp, generate
+
 
-# Usando el comando fake para genearar un Nss completamente aleatorio.
+# ------------------------- fake --------------------------------------------
+## Fake generando campos aleatorios.
+#
 nss = fake('nss') # Valor valido por ejemplo `48979152914`
+curp = fake('curp') # Valor valido por ejemplo `AAMR740524HOCBRN08`
+
+# ------------------------- validate ------------------------------------------
+## Validación de datos
 if validate('nss', nss): # Esto debe valer True por lo tanto mostrará el nss generado
     print(nss)
-#
-curp = fake('curp') # Valor valido por ejemplo `AAMR740524HOCBRN08`
+
 if validate('curp', curp): # Esto debe valer True
     print(curp)
 
+## EXPERIMENTAL. #####
+# Devuelve true si:
+#  - El curp es valido
+#  - Con el  valor del campo nombre, es viable formar el CURP recibido.
+data = {"nombre" : "MIGUEL ANGEL"}
+if validate('curp', value = "BAUM690216HMSLRG18", match = data):
+    print(curp)
+
+# ------------------------- generate ------------------------------------------
+#
+# Puede generar un curp tomando en consideración los datos que ingrese.
+curp_str = generate('curp', data)
+print('curp generada a partir del nombre', curp_str) # por ejemplo: ZUVM471127HOCTJG03
+# Los datos restantes los genera de forma aleatoria, en este sentido es parecida a fake.
+# Pero... en la medida que agregue datos el CURP generado es predictivo, ejemplo:
+data = {
+    "nombre" : "Juan Manuel",
+    "primer_ap": "Lopéz",
+    "segundo_ap": "Lopéz",
+    "f_nacimiento": "780609", # 9 de junio del 1978
+    "sexo": "H", # H: hombre, M: Mujer,
+    "entidad_federativa": "SP" # San Luis Potosí
+}
+curp_str = generate('curp', data) # resultado: LOLJ780609HSPPPN09
+print('curp generado con todos los datos recibidos', curp_str)
+
+nss_data = {
+    "region_imss" : "72",
+    "folio_imss" : "0804",
+    "f_nacimiento": "56",
+    "f_afiliacion": "79",
+}
+nss_str = generate('nss', nss_data) # resultado: 72795608040
+print('NSS generado con todos los datos recibidos', nss_str)
 
+# ------------------------- Manejo de errores ---------------------------------
 
 # Un caso de error en donde el año de afiliación/nacimiento
 if not validate('nss', '12345678901'):
-    print(Nss.errors)
+    print('NSS Errores: ', Nss.errors)
 
 # De forma similar probamos con un valor invalido para el curp
 if not validate('curp', '--invalido--'):
-    print(Curp.errors)
+    print('CURP Errores: ', Curp.errors)
 #
-```
 
-### Instalación.
-
-
-El paquete esta disponible en **pypi** (__<https://pypi.org/project/mexa/>__), para puedes instalarlo desde `pip`:
-
-```
-# Instalación de Mexa.
-pip install mexa
+#
 ```
 
 
 # Número de seguro social Nss
 
 El numero de seguro social de México se conforma de 11 dígitos:
 
@@ -79,19 +112,17 @@
 ### Diez digitos de información.
 
  - 2 Dígitos Región IMSS.
  - 2 Dígitos Año afiliación al Seguro Social.
  - 2 Dígitos Año de nacimiento.
  - 4 Folio IMSS.
 
-### El verificador es el último dígito (el onceavo).
+### Un digito verificador (el último)
 
-Este dígito permite validar los primeros diez dígitos previos, previniendo errores de captura pues la simple alteración de un digito en la cadena de diez digitos genera un cambio en el dígito verificador.
+En la onceava posición y ultima posición se encuentra el dígito permite validar los diez dígitos previos, previniendo errores de captura pues la simple alteración de un digito en la cadena de diez digitos genera un cambio en el dígito verificador.
 
 Este digito es creado por medio de una implementación del **algoritmo Luhn**.
 
 
 > Nota: para mayores informes consultar la definición del algoritmo en wikipedia:
 > :point_right:  <https://es.wikipedia.org/wiki/Algoritmo_de_Luhn>
 
-
-
```

### Comparing `mexa-0.5/mexa/CurpField.py` & `mexa-0.6/mexa/CurpField.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 # encoding: utf-8
 '''Clase encargada del CURP'''
-import re
 from random import randint
 from calendar import monthrange
-from mexa.core import FieldInterface, year_by_last2digit
+from mexa.core import FieldInterface, Partes
 from mexa.Estados import estados
 from mexa.CurpUtils import Rand, CurpTools, CONSONANTS
-from mexa.ErrorMsgs import CURP_ERRORS
+from mexa.ErrorMsgs import CURP_ERRORS as ERRORS
+
+
+# Expresión regular para validar y las partes(groups) que conforman el CURP
+partes = Partes(r'^([A-Z]{4})(\d{6})([H|M])([A-Z]{2})([A-Z]{3})(\S)(\d)$')
+ID_NOMBRE = 1
+FECHA_NACIMIENTO = 2
+SEXO = 3
+ENTIDAD_FEDERATIVA = 4
+ID2_NOMBRE = 5
+HOMOCLAVE = 6
+CHECKSUM = 7
 
 class CurpField(FieldInterface):
     '''CurpField'''
-    errorMsgs = CURP_ERRORS
+    errorMsgs = ERRORS
 
     @staticmethod
     def gen_id_nombre(data):
         '''Genera la parte del nombre, los primeros 4 dígitos'''
         out = ['X','X','X','X']
         # Tomando la parte del primer apellido (paterno)
         if 'primer_ap' in data:
@@ -61,27 +71,27 @@
             out[2] = CurpTools.primer_consonante_interna(nombre)
         else:
             out[2] = Rand.consonante()
         return CurpTools.sanitizar(''.join(out))
 
 
     @staticmethod
-    def error_parte_nombre1(s):
+    def check_part_nombre1(s):
         '''Recibe la primer parte del nombre y valida esta'''
         print('parametro recibido:' + s)
         return False
 
     @staticmethod
-    def error_parte_fecha(fecha_str):
+    def check_fecha(fecha_str, homo_serial):
         '''Revisa si existe algún error en el en formato fecha AAMMDD
 
             devuelve el código de error o
             None en caso de no existir error.
         '''
-        y = year_by_last2digit(fecha_str[0:2])
+        y = CurpTools.anio(fecha_str[0:2], homo_serial)
         m = int(fecha_str[2:4])
         if m > 12:
             return 102
         dias_mes = monthrange(y, m)[1]
         d = int(fecha_str[4:6])
         if d > dias_mes:
             return 103
@@ -93,48 +103,51 @@
         Calculate the checksum for the mexican CURP.
         """
         chars = "0123456789ABCDEFGHIJKLMNNOPQRSTUVWXYZ"
         suma = sum([(18 - i) * chars.index(curp[i]) for i in range(17)])
         return (10 - (suma % 10)) % 10
 
     @staticmethod
-    def is_valid(value):
+    def is_valid(value, match = None):
         '''Regresa True si y solo si value es un CURP valido'''
-        # formato: id_nombre, f_nac, sexo, ent fed, id2_nombre, homoclave
         CurpField.clear_errors()
-        # rex = r'^([A-Z]{4})(\d{6})([H|M])([A-Z]{2})([A-Z]{3})([A-Z0-9]{2})$'
-        rex = r'^([A-Z]{4})(\d{6})([H|M])([A-Z]{2})([A-Z]{3})(\S)(\d)$'
-        s = re.search(rex, CurpTools.sanitizar(value))
-        if not s:
+        #
+        partes.load(CurpTools.sanitizar(value))
+        if partes.error:
             CurpField.add_error(code = 100)
             return False
         # Fecha de nacimiento.
-        error_code = CurpField.error_parte_fecha(s.group(2))
+        error_code = CurpField.check_fecha(
+            partes.get(FECHA_NACIMIENTO),
+            partes.get(HOMOCLAVE)
+        )
         if error_code is not None:
             CurpField.add_error(error_code)
         # Sexo
-        if s.group(3) not in ('H', 'M'):
-            CurpField.add_error(code = 101, value = s.group(3))
-        # Entidad Federativa, NE es no especificado el caso mas común es para extrangeros
+        if partes.get(SEXO) not in ('H', 'M'):
+            CurpField.add_error(code = 101, value = partes.get(SEXO))
+        # Entidad Federativa, NE es no especificado el caso común es para extrangeros
         # Ya que no nació en ninguna entidad federativa.
-        if s.group(4) not in estados:
-            CurpField.add_error(code = 104, value = s.group(4))
+        if partes.get(ENTIDAD_FEDERATIVA) not in estados:
+            CurpField.add_error(code = 104, value = partes.get(ENTIDAD_FEDERATIVA))
         # La parte del nombre esta conformada por la 1er consonante interna del:
         # primer apellido, 2d apellido, nombre pila
-        par_nombre = s.group(5)
+        par_nombre = partes.get(ID2_NOMBRE)
         for c in par_nombre:
             if c not in CONSONANTS:
                 CurpField.add_error(code = 105, value = c)
-        curp_val = s.group(0)
+        curp_val = partes.value()
         cs = CurpField.checksum(curp_val)
-        if cs != int(s.group(7)):
+        if cs != int(partes.get(7)):
             CurpField.add_error(code = 106, value = curp_val)
+        if  match is not None:
+            # Falta agregar la implementación del match
+            CurpField.add_error(code = 100)
         return not CurpField.has_errors()
 
-
     @staticmethod
     def gen_fecha_nacimiento(data):
         '''Genera la fecha de nacimiento'''
         if 'f_nacimiento' in data and len(data['f_nacimiento']) == 6:
             return data['f_nacimiento']
         return Rand.fecha()
```

### Comparing `mexa-0.5/mexa/CurpUtils.py` & `mexa-0.6/mexa/CurpUtils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # encoding: utf-8
-'''Módulo que contiene un conjunto de utilerías diseñadas para darle soporte a la Clae CurpField'''
+'''
+Módulo que contiene un conjunto de utilerías diseñadas
+para darle soporte a la Clase: CurpField
+'''
+import math
 import datetime
 import string
 from random import randint
 from calendar import monthrange
 from mexa.Estados import estados
 
 ALPHABET = string.ascii_uppercase
@@ -60,15 +64,15 @@
             'I': ['Ì', 'Í', 'Ï', 'Î'],
             'O': ['Ò', 'Ó', 'Ö', 'Ô'],
             'U': ['Ù', 'Ú', 'Ü', 'Û'],
             'a': ['ã', 'à', 'á', 'ä', 'â'],
             'e': ['è', 'é', 'ë', 'ê'],
             'i': ['ì', 'í', 'ï', 'î'],
             'o': ['ò', 'ó', 'ö', 'ô'],
-            'u': [ 'ù','ú', 'ü', 'û'],
+            'u': ['ù', 'ú', 'ü', 'û'],
             'C': ['Ç', 'ç'],
             'X': ['ñ', 'Ñ'],
         }
         out = ''
         keys = remplazos.keys()
         for char in value:
             insertado = False
@@ -153,7 +157,20 @@
         if len(parts) <= 1:
             return parts[0]
         especiales = ('JOSE', 'J.', 'MARIA', 'MA.')
         for p in parts:
             if p not in especiales:
                 return p
         return parts[0] if len(parts) else 'X'
+
+    @staticmethod
+    def anio(last2_digits, homo_serial):
+        '''
+            Devuelve al año, agregando los primeros digitos, esto si la parte de la
+            homoclave que genera la serialización para evitar curps repetidos Si es
+            mayor a A entonces nacio despues del año 2000
+        '''
+        y = int(last2_digits)
+        if math.isnan(y):
+            return None
+        centenas = 19 if homo_serial in '12345667890' else 20
+        return (centenas * 100) + y
```

### Comparing `mexa-0.5/mexa/Estados.py` & `mexa-0.6/mexa/Estados.py`

 * *Files identical despite different names*

### Comparing `mexa-0.5/mexa/NssField.py` & `mexa-0.6/mexa/NssField.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,64 @@
 # encoding: utf-8
 '''Clase encargada del Nss'''
-import re
 import random
-from mexa.core import FieldInterface, year_by_last2digit
+from mexa.core import FieldInterface, year_by_last2digit, Partes
+from mexa.ErrorMsgs import NSS_ERRORS as ERRORS
+
+partes = Partes(r'^(\d{2})(\d{2})(\d{2})(\d{4})(\d)$')
+REGION_IMSS = 1
+ANIO_ALTA = 2
+ANIO_NACIMIENTO = 3
+FOLIO_IMSS = 4
+CHECKSUM = 5
 
 class NssField(FieldInterface):
     '''Clase que modela el Nss'''
+    errorMsgs = ERRORS
+    # region_imss, anio_alta, anio_nacimiento, folio_imss, checksum
 
     @staticmethod
     def nss_checksum(nss):
         '''Recibe un string que representa el nss, regresa el checksum'''
         if len(nss) < 10:
             NssField.error_msg = None
             return -1
         suma = 0
         for i in range(10):
-            # factor = 2 if (i % 2 == 1) else 1
             factor = 1 + (i % 2)
             v = int(nss[i]) * factor
             suma += (1 + v % 10) if (v > 9) else v
         cs = (suma * 9) % 10
         return cs
 
 
     @staticmethod
-    def is_valid(value):
+    def is_valid(value, match = None):
         '''Devuelve true si value es valido'''
         NssField.clear_errors()
         if len(value) != 11:
-            NssField.error_msg = 'El valor debe tener una longitud de 11'
+            NssField.add_error(code = 100)
             return False
-        s = re.search(r'^(\d{2})(\d{2})(\d{2})(\d{4})(\d)$', value)
-        if not s:
-            NssField.error_msg = 'Formato invalido de entrada'
+        partes.load(value)
+        if partes.error:
+            NssField.add_error(code = 100)
             return False
-        # reg_imss = s.group(1)
-        f_afi = year_by_last2digit(s.group(2))
-        f_nac = year_by_last2digit(s.group(3))
+        # revisando los años de afiliación/nacimiento
+        f_afi = year_by_last2digit(partes.get(ANIO_ALTA))
+        f_nac = year_by_last2digit(partes.get(ANIO_NACIMIENTO))
         if int(f_afi) < int(f_nac):
-            msg = f"No se pudo afiliar({f_afi}) antes de haber nacido({f_nac})"
-            NssField.error_msg = msg
+            NssField.add_error(code = 101)
             return False
-        if NssField.nss_checksum(value) == int(s.group(5)):
-            return True
-        NssField.error_msg = 'Input invalido'
-        return False
-
+        # revisando el checksum
+        cs = NssField.nss_checksum(value)
+        if cs != int(partes.get(CHECKSUM)):
+            NssField.add_error(code = 102, value = partes.get(CHECKSUM))
+            return False
+        # Falta agregar la implementación del match
+        return match is None
 
     @staticmethod
     def autocomplete(value):
         '''Devuelve true si value es valido'''
         if len(value) != 10:
             return value
         cs = NssField.nss_checksum(value)
```

### Comparing `mexa-0.5/mexa/__init__.py` & `mexa-0.6/mexa/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,16 @@
         return Curp.generate(data)
     raise TypeError(f"Tipo invalido: {type_field}")
 
 def fake(type_field):
     '''faker'''
     return generate(type_field, {})
 
-def validate(type_field, value):
+def validate(type_field, value, match = None):
     '''Valida el type_field el valor'''
     if type_field == 'nss':
-        return Nss.is_valid(value)
+        return Nss.is_valid(value, match)
     if type_field == 'curp':
-        return Curp.is_valid(value)
+        return Curp.is_valid(value, match)
     raise TypeError(f"Tipo invalido: {type_field}")
+
+__all__ = ['generate', 'validate', 'Curp', 'Nss', 'CurpTools']
```

### Comparing `mexa-0.5/mexa/data_ladas.py` & `mexa-0.6/mexa/data_ladas.py`

 * *Files identical despite different names*

### Comparing `mexa-0.5/setup.py` & `mexa-0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 readme = open('./README.md', 'r')
 
 setup(
     name = 'mexa',
-    version = '0.5',
+    version = '0.6',
     packages=['mexa'],
     description = 'Validador y Generador de campos para tramites mexicanos',
     author='@Fitorec - Miguel Angel Marcial Martinez',
     author_email = 'fitorec@mundosica.com',
     url = 'https://github.com/fitorec/mexa-py',
     long_description = readme.read(),
     long_description_content_type = 'text/markdown',
```

