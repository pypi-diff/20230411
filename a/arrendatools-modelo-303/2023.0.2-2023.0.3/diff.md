# Comparing `tmp/arrendatools_modelo_303-2023.0.2.tar.gz` & `tmp/arrendatools_modelo_303-2023.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrendatools_modelo_303-2023.0.2.tar", last modified: Fri Apr  7 16:05:26 2023, max compression
+gzip compressed data, was "arrendatools_modelo_303-2023.0.3.tar", last modified: Tue Apr 11 19:55:36 2023, max compression
```

## Comparing `arrendatools_modelo_303-2023.0.2.tar` & `arrendatools_modelo_303-2023.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 16:05:26.632214 arrendatools_modelo_303-2023.0.2/
--rw-r--r--   0 root         (0) root         (0)     1062 2023-04-07 16:05:23.000000 arrendatools_modelo_303-2023.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      772 2023-04-07 16:05:26.632214 arrendatools_modelo_303-2023.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6177 2023-04-07 16:05:23.000000 arrendatools_modelo_303-2023.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 16:05:26.628214 arrendatools_modelo_303-2023.0.2/arrendatools_modelo_303/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 16:05:23.000000 arrendatools_modelo_303-2023.0.2/arrendatools_modelo_303/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42511 2023-04-07 16:05:23.000000 arrendatools_modelo_303-2023.0.2/arrendatools_modelo_303/modelo_303.py
--rw-r--r--   0 root         (0) root         (0)      105 2023-04-07 16:05:23.000000 arrendatools_modelo_303-2023.0.2/arrendatools_modelo_303/periodos.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 16:05:26.632214 arrendatools_modelo_303-2023.0.2/arrendatools_modelo_303.egg-info/
--rw-r--r--   0 root         (0) root         (0)      772 2023-04-07 16:05:26.000000 arrendatools_modelo_303-2023.0.2/arrendatools_modelo_303.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      358 2023-04-07 16:05:26.000000 arrendatools_modelo_303-2023.0.2/arrendatools_modelo_303.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 16:05:26.000000 arrendatools_modelo_303-2023.0.2/arrendatools_modelo_303.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-04-07 16:05:26.000000 arrendatools_modelo_303-2023.0.2/arrendatools_modelo_303.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       98 2023-04-07 16:05:26.632214 arrendatools_modelo_303-2023.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      893 2023-04-07 16:05:24.000000 arrendatools_modelo_303-2023.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 16:05:26.632214 arrendatools_modelo_303-2023.0.2/test/
--rw-r--r--   0 root         (0) root         (0)    29537 2023-04-07 16:05:23.000000 arrendatools_modelo_303-2023.0.2/test/test_modelo_303.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 19:55:36.053286 arrendatools_modelo_303-2023.0.3/
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-04-11 19:55:33.000000 arrendatools_modelo_303-2023.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      772 2023-04-11 19:55:36.053286 arrendatools_modelo_303-2023.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6179 2023-04-11 19:55:33.000000 arrendatools_modelo_303-2023.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 19:55:36.053286 arrendatools_modelo_303-2023.0.3/arrendatools_modelo_303/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 19:55:33.000000 arrendatools_modelo_303-2023.0.3/arrendatools_modelo_303/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43093 2023-04-11 19:55:33.000000 arrendatools_modelo_303-2023.0.3/arrendatools_modelo_303/modelo_303.py
+-rw-r--r--   0 root         (0) root         (0)      105 2023-04-11 19:55:33.000000 arrendatools_modelo_303-2023.0.3/arrendatools_modelo_303/periodos.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 19:55:36.053286 arrendatools_modelo_303-2023.0.3/arrendatools_modelo_303.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      772 2023-04-11 19:55:36.000000 arrendatools_modelo_303-2023.0.3/arrendatools_modelo_303.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      358 2023-04-11 19:55:36.000000 arrendatools_modelo_303-2023.0.3/arrendatools_modelo_303.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 19:55:36.000000 arrendatools_modelo_303-2023.0.3/arrendatools_modelo_303.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-11 19:55:36.000000 arrendatools_modelo_303-2023.0.3/arrendatools_modelo_303.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2023-04-11 19:55:36.053286 arrendatools_modelo_303-2023.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      893 2023-04-11 19:55:33.000000 arrendatools_modelo_303-2023.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 19:55:36.053286 arrendatools_modelo_303-2023.0.3/test/
+-rw-r--r--   0 root         (0) root         (0)    34609 2023-04-11 19:55:33.000000 arrendatools_modelo_303-2023.0.3/test/test_modelo_303.py
```

### Comparing `arrendatools_modelo_303-2023.0.2/LICENSE` & `arrendatools_modelo_303-2023.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `arrendatools_modelo_303-2023.0.2/PKG-INFO` & `arrendatools_modelo_303-2023.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrendatools_modelo_303
-Version: 2023.0.2
+Version: 2023.0.3
 Summary: Módulo de Python que genera un string para la importación de datos en el modelo 303 de la Agencia Tributaria de España (PRE 303 - Servicio ayuda modelo 303)
 Home-page: https://github.com/hokus15/ArrendaToolsModelo303
 Author: hokus15
 Author-email: hokus@hotmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `arrendatools_modelo_303-2023.0.2/README.md` & `arrendatools_modelo_303-2023.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 - Si el % atribuible a la Administración del Estado es distinto de 100%.
 - En el IVA a la importación liquidado por la Aduana pendiente de ingreso.
 - En autoliquidaciones complementarias (opción y número de justificante).
 - En casos en los que el volumen de operaciones anual sea igual a 0.
 - Cuando existan cuotas pendientes de compensar de periodos anteriores.
 - En la cuenta corriente tributaria - ingreso.
 - En la cuenta corriente tributaria - devolución.
-- En devoluciones por transferencia al extranjero.
+- En la devolución por transferencia al extranjero.
 
 Por lo tanto, se recomienda al usuario verificar que se cumplen todas las condiciones necesarias antes de utilizar este módulo para la presentación del IVA trimestral.
 
 ## Descargo de responsabilidad
 
 Este módulo proporciona una opción para generar un archivo con la información necesaria para el modelo 303 de la Agencia Tributaria española en un formato legible por su servicio de ayuda. Sin embargo, es importante tener en cuenta que la correcta generación, presentación e introducción de los datos, así como la veracidad del contenido, son responsabilidad exclusiva del usuario. **El usuario es siempre el último responsable de verificar que los datos introducidos son correctos y cumplen con los requisitos de la Agencia Tributaria.**
```

### Comparing `arrendatools_modelo_303-2023.0.2/arrendatools_modelo_303/modelo_303.py` & `arrendatools_modelo_303-2023.0.3/arrendatools_modelo_303/modelo_303.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
     Attributes:
         periodo (string): Periodo de la declaración Datos validos: (1T, 2T, 3T o 4T)
         nif_empresa_desarrollo (string): NIF de la empresa de desarrollo. A cumplimentar por las entidades desarrolladoras (EEDD). Máximo 9 caracteres.
         version (string): Versión del programa. Debe consignarse el identificador de la versión del SW desarrollado por la ED. Máximo 4 caracteres.
         nombre_fiscal (string): Apellidos y nombre o Razón social del contribuyente. Máximo 80 caracteres.
         nif_contribuyente: (string): NIF contribuyente. Máximo 9 caracteres.
-        iban (string): IBAN donde domiciliar el pago/devolucion.
-        base_impobible (float): Importe trimestral del alquiler sin computar el IVA. Tenga en cuenta que la base imponible del IVA en el arrendamiento de un local de negocio está constituida por el importe total de la contraprestación, incluyendo no solo el importe de la renta, sino también las cantidades asimiladas que el arrendador pueda exigir al arrendatario o inquilino. Por ejemplo, los gastos de comunidad, el IBI, los gastos de suministros (calefacción, agua, luz), las reparaciones y otros conceptos análogos. En ocasiones, estos gastos son facturados al arrendador y posteriormente el arrendador los repercute al arrendatario. No se solicitan las cuotas de IVA puesto que se calculan aplicando sobre la base consignada el 21 por 100. Tenga en cuenta que deberá declarar las cuotas de arrendamiento exigibles, hayan sido cobradas o no. En caso de impago podrá recuperar el IVA ingresado cuando se cumplan los requisitos previstos en el artículo 80.Tres o Cuatro, consignando las casillas "Modificación bases y cuotas" (casillas 14 y 15).
+        base_imponible (float): Importe trimestral del alquiler sin computar el IVA. Tenga en cuenta que la base imponible del IVA en el arrendamiento de un local de negocio está constituida por el importe total de la contraprestación, incluyendo no solo el importe de la renta, sino también las cantidades asimiladas que el arrendador pueda exigir al arrendatario o inquilino. Por ejemplo, los gastos de comunidad, el IBI, los gastos de suministros (calefacción, agua, luz), las reparaciones y otros conceptos análogos. En ocasiones, estos gastos son facturados al arrendador y posteriormente el arrendador los repercute al arrendatario. No se solicitan las cuotas de IVA puesto que se calculan aplicando sobre la base consignada el 21 por 100. Tenga en cuenta que deberá declarar las cuotas de arrendamiento exigibles, hayan sido cobradas o no. En caso de impago podrá recuperar el IVA ingresado cuando se cumplan los requisitos previstos en el artículo 80.Tres o Cuatro, consignando las casillas "Modificación bases y cuotas" (casillas 14 y 15).
+        iban (string): IBAN donde domiciliar el pago/devolucion. Sólo se permiten IBAN españoles (que empiecen por ES).
         gastos_bienes_servicios (float): Base imponible trimestral de los gastos en bienes y servicios corrientes.
         iva_gastos_bienes_servicios (float): IVA trimestral soportado deducible de los gastos en bienes y servicios corrientes. Para ser deducible el IVA soportado debe disponer de factura completa emitida a nombre del arrendador. Podrá incluir, entre otras, las cuotas soportadas por suministros, reparaciones y obras de mejora, servicios profesionales independientes (abogados, asesoría, notaría, API) y servicios exteriores (publicidad, limpieza, vigilancia). No son deducibles, ni siquiera parcialmente, las cuotas soportadas en bienes y servicios que se utilicen simultáneamente para esta actividad y para necesidades privadas cuando el precio de adquisición sea inferior a 3.005,06 euros (ordenadores, móviles...). Tampoco son deducibles los gastos en los que no se soporte el impuesto (intereses de préstamo, seguros, IBI o la amortización del inmueble).
         adquisiciones_bienes_inversion (float): Base imponible trimestral de las adquisiciones de bienes de inversión.
         iva_adquisiciones_bienes_inversion (float): IVA trimestral soportado deducible de las adquisiciones de bienes de inversión. Podrá deducir el importe de las cuotas soportadas por la adquisición de bienes de inversión (cuantía superior a 3.005,06 euros) que se utilicen en la actividad de arrendamiento, como el mobiliario. Asimismo, el IVA soportado en la construcción o adquisición del inmueble, las obras de reforma o mejoras. En el caso de que la afectación a la actividad sea parcial, deberá calcularse la parte afecta.
         volumen_anual_operaciones (float): Volumen anual de operaciones. Sólo necesario para 4T.
     """
     _LONGITUD_NIF = 9
+    _EJERCICIO = "2023"
 
-    _MAX_LONGITUD_IBAN = 34
+    # _MAX_LONGITUD_IBAN = 34 -> Los 34 son para cuentas en el extranjero que no está soportado por el módulo
+    _MAX_LONGITUD_IBAN = 24
     _MAX_LONGITUD_VERSION = 4
     _MAX_LONGITUD_NOMBRE_FISCAL_CONTRIBUYENTE = 80
-    _EJERCICIO = "2023"
 
     _INICIO_APERTURA = "<T"
     _INICIO_CIERRE = "</T"
     _MODELO = "303"
     _DISCRIMINANTE = "0"
     _CIERRE = ">"
     _TIPO_Y_CIERRE = "0000" + _CIERRE
@@ -71,59 +72,68 @@
     def __init__(
         self,
         periodo,                                 # Periodo de la declaración Datos validos: (1T, 2T, 3T o 4T)
         nif_empresa_desarrollo,                  # NIF de la empresa de desarrollo. A cumplimentar por las entidades desarrolladoras (EEDD). Máximo 9 caracteres.
         version,                                 # Versión del programa: Debe consignarse el identificador de la versión del SW desarrollado por la ED. Máximo 4 caracteres.
         nombre_fiscal_contribuyente,             # Apellidos y nombre o Razón social del contribuyente. Máximo 80 caracteres.
         nif_contribuyente,                       # NIF contribuyente. Máximo 9 caracteres.
-        iban,                                    # IBAN donde domiciliar el pago/devolucion.
         base_imponible,                          # Importe trimestral del alquiler sin computar el IVA. Tenga en cuenta que la base imponible del IVA en el arrendamiento de un local de negocio está constituida por el importe total de la contraprestación, incluyendo no solo el importe de la renta, sino también las cantidades asimiladas que el arrendador pueda exigir al arrendatario o inquilino. Por ejemplo, los gastos de comunidad, el IBI, los gastos de suministros (calefacción, agua, luz), las reparaciones y otros conceptos análogos. En ocasiones, estos gastos son facturados al arrendador y posteriormente el arrendador los repercute al arrendatario. No se solicitan las cuotas de IVA puesto que se calculan aplicando sobre la base consignada el 21 por 100. Tenga en cuenta que deberá declarar las cuotas de arrendamiento exigibles, hayan sido cobradas o no. En caso de impago podrá recuperar el IVA ingresado cuando se cumplan los requisitos previstos en el artículo 80.Tres o Cuatro, consignando las casillas "Modificación bases y cuotas" (casillas 14 y 15).
+        iban="",                                 # IBAN donde domiciliar el pago/devolucion.
         gastos_bienes_servicios=0.0,             # Base imponible trimestral de los gastos en bienes y servicios corrientes.
         iva_gastos_bienes_servicios=0.0,         # IVA trimestral soportado deducible de los gastos en bienes y servicios corrientes. Para ser deducible el IVA soportado debe disponer de factura completa emitida a nombre del arrendador. Podrá incluir, entre otras, las cuotas soportadas por suministros, reparaciones y obras de mejora, servicios profesionales independientes (abogados, asesoría, notaría, API) y servicios exteriores (publicidad, limpieza, vigilancia). No son deducibles, ni siquiera parcialmente, las cuotas soportadas en bienes y servicios que se utilicen simultáneamente para esta actividad y para necesidades privadas cuando el precio de adquisición sea inferior a 3.005,06 euros (ordenadores, móviles...). Tampoco son deducibles los gastos en los que no se soporte el impuesto (intereses de préstamo, seguros, IBI o la amortización del inmueble).
         adquisiciones_bienes_inversion=0.0,      # Base imponible trimestral de las adquisiciones de bienes de inversión.
         iva_adquisiciones_bienes_inversion=0.0,  # IVA trimestral soportado deducible de las adquisiciones de bienes de inversión. Podrá deducir el importe de las cuotas soportadas por la adquisición de bienes de inversión (cuantía superior a 3.005,06 euros) que se utilicen en la actividad de arrendamiento, como el mobiliario. Asimismo, el IVA soportado en la construcción o adquisición del inmueble, las obras de reforma o mejoras. En el caso de que la afectación a la actividad sea parcial, deberá calcularse la parte afecta.
-        volumen_anual_operaciones=0.0            # Volumen anual de operaciones. Sólo necesario para 4T.
+        volumen_anual_operaciones=None           # Volumen anual de operaciones. Sólo necesario para 4T.
     ):
+        # Validación de los datos
+        if not [periodo, nif_empresa_desarrollo, version, nombre_fiscal_contribuyente, nif_contribuyente, base_imponible]:
+            raise ValueError("periodo, nif_empresa_desarrollo, version, nombre_fiscal_contribuyente, nif_contribuyente, base_imponible son campos obligatorios")
         if len(nif_empresa_desarrollo) != Modelo303._LONGITUD_NIF:
             raise ValueError(f"El NIF de la empresa de desarrollo debe ser de {Modelo303._LONGITUD_NIF} caracteres")
         if len(version) > Modelo303._MAX_LONGITUD_VERSION:
             raise ValueError(f"La versión no puede tener más de {Modelo303._MAX_LONGITUD_VERSION} caracteres")
         if len(nombre_fiscal_contribuyente) > Modelo303._MAX_LONGITUD_NOMBRE_FISCAL_CONTRIBUYENTE:
             raise ValueError(f"El nombre o razón social del contribuyente no puede tener más de {Modelo303._MAX_LONGITUD_NOMBRE_FISCAL_CONTRIBUYENTE} caracteres")
         if len(nif_contribuyente) != Modelo303._LONGITUD_NIF:
             raise ValueError(f"El NIF del contribuyente debe ser de {Modelo303._LONGITUD_NIF} caracteres")
-        if len(iban) > Modelo303._MAX_LONGITUD_IBAN:
-            raise ValueError(f"El IBAN no puede tener más de {Modelo303._MAX_LONGITUD_IBAN} caracteres")
         if (periodo == Periodo.P4T and volumen_anual_operaciones is None):
             raise ValueError("El volumen anual de operaciones es obligatorio en el 4º trimestre (4T)")
 
+        # Campos obligatorios
         self.ejercicio = self._EJERCICIO
         self.periodo = periodo.value
         self.nif_empresa_desarrollo = nif_empresa_desarrollo.upper()
         self.version = version
         self.nombre_fiscal = nombre_fiscal_contribuyente.upper()
         self.nif_contribuyente = nif_contribuyente.upper()
-        self.iban = iban.upper()
         self.base_imponible = base_imponible
-        if not gastos_bienes_servicios:
-            self.gastos_bienes_servicios = 0.0
-        else:
-            self.gastos_bienes_servicios = gastos_bienes_servicios
-        if not iva_gastos_bienes_servicios:
-            self.iva_gastos_bienes_servicios = 0.0
-        else:
-            self.iva_gastos_bienes_servicios = iva_gastos_bienes_servicios
-        if not adquisiciones_bienes_inversion:
-            self.adquisiciones_bienes_inversion = 0.0
-        else:
-            self.adquisiciones_bienes_inversion = adquisiciones_bienes_inversion
-        if not iva_adquisiciones_bienes_inversion:
-            self.iva_adquisiciones_bienes_inversion = 0.0
-        else:
-            self.iva_adquisiciones_bienes_inversion = iva_adquisiciones_bienes_inversion
+        # Validación campos opcionales
+        if iban is None:
+            iban = ""
+
+        if gastos_bienes_servicios is None:
+            gastos_bienes_servicios = 0.0
+
+        if iva_gastos_bienes_servicios is None:
+            iva_gastos_bienes_servicios = 0.0
+
+        if adquisiciones_bienes_inversion is None:
+            adquisiciones_bienes_inversion = 0.0
+
+        if iva_adquisiciones_bienes_inversion is None:
+            iva_adquisiciones_bienes_inversion = 0.0
+
+        # Asignamos los campos opcionales
+        self.iban = iban.upper()
+        if len(iban) > Modelo303._MAX_LONGITUD_IBAN:
+            raise ValueError(f"El IBAN no puede tener más de {Modelo303._MAX_LONGITUD_IBAN} caracteres")
+        self.gastos_bienes_servicios = gastos_bienes_servicios
+        self.iva_gastos_bienes_servicios = iva_gastos_bienes_servicios
+        self.adquisiciones_bienes_inversion = adquisiciones_bienes_inversion
+        self.iva_adquisiciones_bienes_inversion = iva_adquisiciones_bienes_inversion
         self.volumen_anual_operaciones = volumen_anual_operaciones
 
     def generar(self):
         """
         Genera el string para la importación de datos en el modelo 303 de la Agencia Tributaria de España (PRE 303 - Servicio ayuda modelo 303).
         El string generado se puede guardar en un fichero y es compatible con el modelo 303 para la presentación trimestral del IVA.
         """
@@ -412,15 +422,15 @@
         iva_devengado = round(self.base_imponible * 0.21, 2)
         total_iva_deducible = round(self.iva_gastos_bienes_servicios + self.iva_adquisiciones_bienes_inversion, 2)
         return round(iva_devengado - total_iva_deducible, 2)
 
     def _tipo_declaracion(self):
         """
         Obtiene el tipo de declaración en base al IVA devengado y el IBAN.
-        Sólo tiene en cuenta los tipos N, U e I. El resto de tipos no están soportados.
+        Sólo tiene en cuenta los tipos N, C, D, U e I. El resto de tipos no están soportados.
         El tipo de declaración puede ser:
         C (solicitud de compensación)
         D (devolución)
         G (cuenta corriente tributaria-ingreso)
         I (ingreso)
         N (sin actividad/resultado cero)
         V (cuenta corriente tributaria -devolución)
```

### Comparing `arrendatools_modelo_303-2023.0.2/arrendatools_modelo_303.egg-info/PKG-INFO` & `arrendatools_modelo_303-2023.0.3/arrendatools_modelo_303.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrendatools-modelo-303
-Version: 2023.0.2
+Version: 2023.0.3
 Summary: Módulo de Python que genera un string para la importación de datos en el modelo 303 de la Agencia Tributaria de España (PRE 303 - Servicio ayuda modelo 303)
 Home-page: https://github.com/hokus15/ArrendaToolsModelo303
 Author: hokus15
 Author-email: hokus@hotmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `arrendatools_modelo_303-2023.0.2/setup.py` & `arrendatools_modelo_303-2023.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-__version__ = "2023.0.2"
+__version__ = "2023.0.3"
 
 setup(
     name='arrendatools_modelo_303',
     version=__version__,
     description='Módulo de Python que genera un string para la importación de datos en el modelo 303 de la Agencia Tributaria de España (PRE 303 - Servicio ayuda modelo 303)',
     url='https://github.com/hokus15/ArrendaToolsModelo303',
     author='hokus15',
```

### Comparing `arrendatools_modelo_303-2023.0.2/test/test_modelo_303.py` & `arrendatools_modelo_303-2023.0.3/test/test_modelo_303.py`

 * *Files 7% similar despite different names*

```diff
@@ -343,10 +343,41 @@
                 gastos_bienes_servicios=gastos_bienes_servicios,
                 iva_gastos_bienes_servicios=iva_gastos_bienes_servicios,
                 adquisiciones_bienes_inversion=adquisiciones_bienes_inversion,
                 iva_adquisiciones_bienes_inversion=iva_adquisiciones_bienes_inversion,
                 volumen_anual_operaciones=volumen_anual_operaciones
             )
 
+    def test_generar_modelo_sin_iban(self):
+        expected_result = "<T303020231T0000><AUX>                                                                      v1.0    12345678X                                                                                                                                                                                                                     </AUX><T30301000> I12345678EDE LOS PALOTES PERICO                                                           20231T22322222200000000 20000000000000000000000000000000000000000000000000000000000004000000000000000000000000000000000000005000000000000000000000000000000000000010000000000000000000000000000000200000021000000000000004200000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001750000000000000000000000000000000000000000000000000000000000000000000000000001400000000000000000000000000000000000005200000000000000000000000000000000000000000000000000000000000000004200000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000042000                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     </T30301000><T30303000>0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000420001000000000000000042000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000042000000000000000000000000000000000000000000000000042000                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       </T30303000><T303DID00>                                                                                                                                                                                      0                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         </T303DID00></T303020231T0000>"
+        periodo = Periodo.P1T
+        nif_empresa_desarrollo = "12345678X"
+        version = "v1.0"
+        nombre_fiscal_contribuyente = "DE LOS PALOTES PERICO"
+        nif_contribuyente = "12345678E"
+        base_imponible = 2000.00
+        gastos_bienes_servicios = 0.0
+        iva_gastos_bienes_servicios = 0.0
+        adquisiciones_bienes_inversion = 0.0
+        iva_adquisiciones_bienes_inversion = 0.0
+        volumen_anual_operaciones = None
+
+        datos_modelo = Modelo303(
+            periodo=periodo,
+            nif_empresa_desarrollo=nif_empresa_desarrollo,
+            version=version,
+            nombre_fiscal_contribuyente=nombre_fiscal_contribuyente,
+            nif_contribuyente=nif_contribuyente,
+            base_imponible=base_imponible,
+            gastos_bienes_servicios=gastos_bienes_servicios,
+            iva_gastos_bienes_servicios=iva_gastos_bienes_servicios,
+            adquisiciones_bienes_inversion=adquisiciones_bienes_inversion,
+            iva_adquisiciones_bienes_inversion=iva_adquisiciones_bienes_inversion,
+            volumen_anual_operaciones=volumen_anual_operaciones
+        )
+
+        datos_fichero = datos_modelo.generar()
+        self.assertEquals(datos_fichero, expected_result)
+
 
 if __name__ == '__main__':
     unittest.main()
```

