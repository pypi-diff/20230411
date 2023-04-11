# Comparing `tmp/kz_iin_validator-0.5.0.tar.gz` & `tmp/kz_iin_validator-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kz_iin_validator-0.5.0.tar", last modified: Tue Apr 11 05:03:48 2023, max compression
+gzip compressed data, was "kz_iin_validator-0.6.0.tar", last modified: Tue Apr 11 06:54:52 2023, max compression
```

## Comparing `kz_iin_validator-0.5.0.tar` & `kz_iin_validator-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 05:03:48.324736 kz_iin_validator-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-04-11 05:03:41.000000 kz_iin_validator-0.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4205 2023-04-11 05:03:48.324736 kz_iin_validator-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3890 2023-04-11 05:03:41.000000 kz_iin_validator-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 05:03:48.324736 kz_iin_validator-0.5.0/kz_iin_validator/
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-04-11 05:03:41.000000 kz_iin_validator-0.5.0/kz_iin_validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-04-11 05:03:41.000000 kz_iin_validator-0.5.0/kz_iin_validator/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1809 2023-04-11 05:03:41.000000 kz_iin_validator-0.5.0/kz_iin_validator/iin_generator.py
--rw-r--r--   0 runner    (1001) docker     (122)     4280 2023-04-11 05:03:41.000000 kz_iin_validator-0.5.0/kz_iin_validator/iin_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-04-11 05:03:41.000000 kz_iin_validator-0.5.0/kz_iin_validator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 05:03:48.324736 kz_iin_validator-0.5.0/kz_iin_validator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4205 2023-04-11 05:03:48.000000 kz_iin_validator-0.5.0/kz_iin_validator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-04-11 05:03:48.000000 kz_iin_validator-0.5.0/kz_iin_validator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 05:03:48.000000 kz_iin_validator-0.5.0/kz_iin_validator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-11 05:03:48.000000 kz_iin_validator-0.5.0/kz_iin_validator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 05:03:48.324736 kz_iin_validator-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      848 2023-04-11 05:03:41.000000 kz_iin_validator-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 06:54:52.683955 kz_iin_validator-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-04-11 06:54:44.000000 kz_iin_validator-0.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4769 2023-04-11 06:54:52.683955 kz_iin_validator-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4439 2023-04-11 06:54:44.000000 kz_iin_validator-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 06:54:52.679955 kz_iin_validator-0.6.0/kz_iin_validator/
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-04-11 06:54:44.000000 kz_iin_validator-0.6.0/kz_iin_validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-04-11 06:54:44.000000 kz_iin_validator-0.6.0/kz_iin_validator/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-04-11 06:54:44.000000 kz_iin_validator-0.6.0/kz_iin_validator/iin_generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4133 2023-04-11 06:54:44.000000 kz_iin_validator-0.6.0/kz_iin_validator/iin_validator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-04-11 06:54:44.000000 kz_iin_validator-0.6.0/kz_iin_validator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 06:54:52.679955 kz_iin_validator-0.6.0/kz_iin_validator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4769 2023-04-11 06:54:52.000000 kz_iin_validator-0.6.0/kz_iin_validator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-04-11 06:54:52.000000 kz_iin_validator-0.6.0/kz_iin_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 06:54:52.000000 kz_iin_validator-0.6.0/kz_iin_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-11 06:54:52.000000 kz_iin_validator-0.6.0/kz_iin_validator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 06:54:52.683955 kz_iin_validator-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      869 2023-04-11 06:54:44.000000 kz_iin_validator-0.6.0/setup.py
```

### Comparing `kz_iin_validator-0.5.0/LICENSE.txt` & `kz_iin_validator-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kz_iin_validator-0.5.0/PKG-INFO` & `kz_iin_validator-0.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,35 @@
-Metadata-Version: 2.1
-Name: kz_iin_validator
-Version: 0.5.0
-Summary: Kazakhstan IIN parser and validator
-Home-page: https://github.com/ZhymabekRoman/kz-iin-validator
-Author: Zhymabek Roman
-Author-email: robanokssamit@yandex.ru
-License: LICENSE.txt
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # kz-iin-validator
 
+[![MIT License](https://img.shields.io/pypi/l/kz-iin-validator.svg?style=flat-square)](https://opensource.org/licenses/MIT)
+[![PyPI version](https://img.shields.io/pypi/v/kz-iin-validator.svg?style=flat-square)](https://pypi.org/project/kz-iin-validator/)
+[![PyPI downloads](https://img.shields.io/pypi/dm/kz-iin-validator.svg?style=flat-square)](https://pypi.org/project/kz-iin-validator/)
 [![codecov](https://img.shields.io/codecov/c/github/ZhymabekRoman/kz-iin-validator?style=flat-square)](https://app.codecov.io/github/ZhymabekRoman/kz-iin-validator)
 [![tests](https://img.shields.io/github/actions/workflow/status/ZhymabekRoman/kz-iin-validator/pytest.yml?branch=main&style=flat-square)](https://github.com/ZhymabekRoman/kz-iin-validator/actions)
 
 **kz-iin-validator** - Библиотека для проверки и извлечения данных из ИИН на Python 3. ИИН - это Индивидуальный Идентификационный Номер граждан Республики Казахстан (РК) и юридических лиц РК
 
 ## Возможности:
 - Production-ready библиотека
 - 100% code coverage - Библиотека полностью покрыта тестами
 - Zero-depency - Не требует дополнительных зависимостей
 - Базовая валидация данных ИИН, таких как дата, месяц, год
 - Генератор ИИН
-- Два варианта валидации: стандратное (по умолчанию) и дополнительно с использованием регулярных выражении (включается через аргумент `weak_fast_check=True`, не рекомендуется к использованию) 
+- Два варианта валидации: стандартное (по умолчанию) и дополнительно с использованием регулярных выражении (включается через аргумент `weak_fast_check=True`, не рекомендуется к использованию) 
 - Проверка целостности по хэш сумме ИИН. Алгоритм формирования ИИН регулируется Постановлением правительства РК "Об утверждении Программы перехода на единый номер физического (юридического) лица (индивидуальный идентификационный номер (бизнес-идентификационный номер) в целях создания Национальных реестров идентификационных номеров Республики Казахстан" от 11 июня 2003 года N 565 - [Ссылка на источник приказа](https://adilet.zan.kz/rus/docs/P030000565_)
 
 ## Требования:
 - Python 3.7 и выше * **
 > \* судя по информации утилиты Vermin
 
 > ** я могу адаптировать (забэкпортить) библиотеку для более старых версии Python, но стоит ли оно? Если что дайте мне знать
 
 ## TODO:
 - Реализовать поддержку валидации БИН
-- Улучшеная документация
+- Улучшить документация
 - Static type hint using Mypy
 
 ## Схема формирования ИИН:
 <details>
   <summary>Схема</summary>
     <img src="https://raw.githubusercontent.com/ZhymabekRoman/kz-iin-validator/main/images/iin_schema.webp" alt="Schema IIN" />
 </details>
@@ -51,31 +43,34 @@
 ```bash
 python3 -m pip install git+https://github.com/ZhymabekRoman/kz-iin-validator
 ```
 
 ## Использование:
 ### Валидация ИИН:
 ```python
-from kz_iin_validator import validate_iin
+from kz_iin_validator import safe_validate_iin, validate_iin
 
 iin = "061211600012"
-validated_iin, error = validate_iin(iin)
+# use kz_iin_validator as in Golang (preferred in production)
+validated_iin, error = safe_validate_iin(iin)
+# or directly with exceptions raising:
+# validated_iin = validate_iin(iin)
 
 print(f"ИИН: {iin}")
 
 # Print IIN owner gender:
 print(f"Пол: {validated_iin.gender.name.upper()}")
 
 # Print IIN owner born information:
 print(f"День: {validated_iin.born_date.day}")
 print(f"Месяц: {validated_iin.born_date.month}")
 print(f"Год: {validated_iin.born_date.year}")
 
 # or directly access to datetime object:
-# validated_iin.born_date._datetime
+# validated_iin.born_date.datetime
 ```
 
 ### Генератор ИИН:
 ```python
 from kz_iin_validator import generate_iin
 
 generated_iin = generate_iin()
```

### Comparing `kz_iin_validator-0.5.0/README.md` & `kz_iin_validator-0.6.0/kz_iin_validator.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,47 @@
+Metadata-Version: 2.1
+Name: kz-iin-validator
+Version: 0.6.0
+Summary: Kazakhstan IIN parser and validator
+Home-page: https://github.com/ZhymabekRoman/kz-iin-validator
+Author: Zhymabek Roman
+Author-email: robanokssamit@yandex.ru
+License: MIT
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # kz-iin-validator
 
+[![MIT License](https://img.shields.io/pypi/l/kz-iin-validator.svg?style=flat-square)](https://opensource.org/licenses/MIT)
+[![PyPI version](https://img.shields.io/pypi/v/kz-iin-validator.svg?style=flat-square)](https://pypi.org/project/kz-iin-validator/)
+[![PyPI downloads](https://img.shields.io/pypi/dm/kz-iin-validator.svg?style=flat-square)](https://pypi.org/project/kz-iin-validator/)
 [![codecov](https://img.shields.io/codecov/c/github/ZhymabekRoman/kz-iin-validator?style=flat-square)](https://app.codecov.io/github/ZhymabekRoman/kz-iin-validator)
 [![tests](https://img.shields.io/github/actions/workflow/status/ZhymabekRoman/kz-iin-validator/pytest.yml?branch=main&style=flat-square)](https://github.com/ZhymabekRoman/kz-iin-validator/actions)
 
 **kz-iin-validator** - Библиотека для проверки и извлечения данных из ИИН на Python 3. ИИН - это Индивидуальный Идентификационный Номер граждан Республики Казахстан (РК) и юридических лиц РК
 
 ## Возможности:
 - Production-ready библиотека
 - 100% code coverage - Библиотека полностью покрыта тестами
 - Zero-depency - Не требует дополнительных зависимостей
 - Базовая валидация данных ИИН, таких как дата, месяц, год
 - Генератор ИИН
-- Два варианта валидации: стандратное (по умолчанию) и дополнительно с использованием регулярных выражении (включается через аргумент `weak_fast_check=True`, не рекомендуется к использованию) 
+- Два варианта валидации: стандартное (по умолчанию) и дополнительно с использованием регулярных выражении (включается через аргумент `weak_fast_check=True`, не рекомендуется к использованию) 
 - Проверка целостности по хэш сумме ИИН. Алгоритм формирования ИИН регулируется Постановлением правительства РК "Об утверждении Программы перехода на единый номер физического (юридического) лица (индивидуальный идентификационный номер (бизнес-идентификационный номер) в целях создания Национальных реестров идентификационных номеров Республики Казахстан" от 11 июня 2003 года N 565 - [Ссылка на источник приказа](https://adilet.zan.kz/rus/docs/P030000565_)
 
 ## Требования:
 - Python 3.7 и выше * **
 > \* судя по информации утилиты Vermin
 
 > ** я могу адаптировать (забэкпортить) библиотеку для более старых версии Python, но стоит ли оно? Если что дайте мне знать
 
 ## TODO:
 - Реализовать поддержку валидации БИН
-- Улучшеная документация
+- Улучшить документация
 - Static type hint using Mypy
 
 ## Схема формирования ИИН:
 <details>
   <summary>Схема</summary>
     <img src="https://raw.githubusercontent.com/ZhymabekRoman/kz-iin-validator/main/images/iin_schema.webp" alt="Schema IIN" />
 </details>
@@ -40,31 +55,34 @@
 ```bash
 python3 -m pip install git+https://github.com/ZhymabekRoman/kz-iin-validator
 ```
 
 ## Использование:
 ### Валидация ИИН:
 ```python
-from kz_iin_validator import validate_iin
+from kz_iin_validator import safe_validate_iin, validate_iin
 
 iin = "061211600012"
-validated_iin, error = validate_iin(iin)
+# use kz_iin_validator as in Golang (preferred in production)
+validated_iin, error = safe_validate_iin(iin)
+# or directly with exceptions raising:
+# validated_iin = validate_iin(iin)
 
 print(f"ИИН: {iin}")
 
 # Print IIN owner gender:
 print(f"Пол: {validated_iin.gender.name.upper()}")
 
 # Print IIN owner born information:
 print(f"День: {validated_iin.born_date.day}")
 print(f"Месяц: {validated_iin.born_date.month}")
 print(f"Год: {validated_iin.born_date.year}")
 
 # or directly access to datetime object:
-# validated_iin.born_date._datetime
+# validated_iin.born_date.datetime
 ```
 
 ### Генератор ИИН:
 ```python
 from kz_iin_validator import generate_iin
 
 generated_iin = generate_iin()
```

### Comparing `kz_iin_validator-0.5.0/kz_iin_validator/iin_generator.py` & `kz_iin_validator-0.6.0/kz_iin_validator/iin_generator.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
     if day_bound == 28 and ((year_centry % 4 == 0 and year_centry % 100 != 0) or year_centry % 400 == 0):
         day_bound = 29
 
     day = random.randint(1, day_bound)
 
     # zfill
-    year_str = '{:02d}'.format(year)
-    month_str = '{:02d}'.format(month)
-    day_str = '{:02d}'.format(day)
+    year_str = f'{year:02d}'
+    month_str = f'{month:02d}'
+    day_str = f'{day:02d}'
 
     dob = f"{year_str}{month_str}{day_str}"
 
     individual_number = f"{random.randint(1, 9999):04d}"
 
     iin = f"{dob}{centry_and_gender_code}{individual_number}"
```

### Comparing `kz_iin_validator-0.5.0/kz_iin_validator/iin_validator.py` & `kz_iin_validator-0.6.0/kz_iin_validator/iin_validator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import datetime as dt
 import re
 from dataclasses import dataclass
 from enum import Enum, auto
 from typing import Union
 
-from .utils import is_digit_string
 from .exceptions import IINValidateError
+from .utils import is_digit_string
 
 IIN_REGEX_WEAK_FAST = re.compile(r"^[0-9]{12}$")
 IIN_REGEX_WEAK = re.compile(r"^((0[48]|[2468][048]|[13579][26])0230[1-5]|000230[34]|\d\d((0[13578]|1[02])(0[1-9]|[12]\d|3[01])|(0[469]|11)(0[1-9]|[12]\d|30)|02(0[1-9]|[1-2]\d)))[0-6]\d{5}$")
 
 
 @dataclass
 class BornDate:
     day: int
     month: int
     year: int
-    _datetime: dt.datetime
+    datetime: dt.datetime
 
 
 class IINGender(Enum):
     male = auto()
     female = auto()
 
 
@@ -32,54 +32,52 @@
     born_date: BornDate
 
 
 class ValidatedIIN(IIN):
     is_validated: bool = True
 
 
-def validate_iin(iin: Union[str, IIN], weak_fast_check: bool = False, raise_exception: bool = True, full_error_info: bool = True):
+def safe_validate_iin(iin: Union[str, IIN], weak_fast_check: bool = False):
     # Golang like exception returning logic
     try:
-        result = _validate_iin(iin, weak_fast_check)
+        result = validate_iin(iin, weak_fast_check)
     except Exception as ex:
-        if raise_exception:
-            raise ex
-        if full_error_info:
-            exception_msg = f"During validating IIN exception was caught: {str(ex)}"
-        else:
-            exception_msg = "During validating IIN exception was caught"
+        exception_msg = f"During validating IIN exception was caught: {str(ex)}"
         return None, exception_msg
     else:
         return result, None
 
 
-def _validate_iin(iin: Union[str, IIN], weak_fast_check: bool = False):
+# TODO: refactor into separate functions
+def validate_iin(iin: Union[str, IIN], weak_fast_check: bool = False) -> ValidatedIIN:
     if isinstance(iin, IIN):
         iin = iin.iin
     elif not isinstance(iin, str):
         raise IINValidateError(f"Parametr 'iin' must be string, not {type(iin).__name__}")
 
     if weak_fast_check:
         iin_regex_fast = IIN_REGEX_WEAK_FAST.match(iin)
         if iin_regex_fast is None:
             raise IINValidateError("Not valid IIN!")
 
         iin_regex_weak = IIN_REGEX_WEAK.match(iin)
         if iin_regex_weak is None:
             raise IINValidateError("Not correct integers range")
 
-    if len(iin) != 12:
-        raise IINValidateError("IIN must be 12 lenght")
-
     if not is_digit_string(iin):
         raise IINValidateError("IIN must contains only numbers")
 
+    if len(iin) != 12:
+        raise IINValidateError("IIN must be 12 length")
+
     # iin helper functions
-    iin_int = lambda index: int(iin[index])
-    iin_int_range = lambda x, y: int(iin[x:y])
+    def iin_int(index):
+        return int(iin[index])
+    def iin_int_range(x, y):
+        return int(iin[x:y])
 
     is_person = (iin_int(6) != 0)
     if is_person:
         if iin_int(6) % 2 == 1:
             gender = IINGender.male
         else:
             gender = IINGender.female
```

### Comparing `kz_iin_validator-0.5.0/kz_iin_validator.egg-info/PKG-INFO` & `kz_iin_validator-0.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 Metadata-Version: 2.1
-Name: kz-iin-validator
-Version: 0.5.0
+Name: kz_iin_validator
+Version: 0.6.0
 Summary: Kazakhstan IIN parser and validator
 Home-page: https://github.com/ZhymabekRoman/kz-iin-validator
 Author: Zhymabek Roman
 Author-email: robanokssamit@yandex.ru
-License: LICENSE.txt
+License: MIT
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # kz-iin-validator
 
+[![MIT License](https://img.shields.io/pypi/l/kz-iin-validator.svg?style=flat-square)](https://opensource.org/licenses/MIT)
+[![PyPI version](https://img.shields.io/pypi/v/kz-iin-validator.svg?style=flat-square)](https://pypi.org/project/kz-iin-validator/)
+[![PyPI downloads](https://img.shields.io/pypi/dm/kz-iin-validator.svg?style=flat-square)](https://pypi.org/project/kz-iin-validator/)
 [![codecov](https://img.shields.io/codecov/c/github/ZhymabekRoman/kz-iin-validator?style=flat-square)](https://app.codecov.io/github/ZhymabekRoman/kz-iin-validator)
 [![tests](https://img.shields.io/github/actions/workflow/status/ZhymabekRoman/kz-iin-validator/pytest.yml?branch=main&style=flat-square)](https://github.com/ZhymabekRoman/kz-iin-validator/actions)
 
 **kz-iin-validator** - Библиотека для проверки и извлечения данных из ИИН на Python 3. ИИН - это Индивидуальный Идентификационный Номер граждан Республики Казахстан (РК) и юридических лиц РК
 
 ## Возможности:
 - Production-ready библиотека
 - 100% code coverage - Библиотека полностью покрыта тестами
 - Zero-depency - Не требует дополнительных зависимостей
 - Базовая валидация данных ИИН, таких как дата, месяц, год
 - Генератор ИИН
-- Два варианта валидации: стандратное (по умолчанию) и дополнительно с использованием регулярных выражении (включается через аргумент `weak_fast_check=True`, не рекомендуется к использованию) 
+- Два варианта валидации: стандартное (по умолчанию) и дополнительно с использованием регулярных выражении (включается через аргумент `weak_fast_check=True`, не рекомендуется к использованию) 
 - Проверка целостности по хэш сумме ИИН. Алгоритм формирования ИИН регулируется Постановлением правительства РК "Об утверждении Программы перехода на единый номер физического (юридического) лица (индивидуальный идентификационный номер (бизнес-идентификационный номер) в целях создания Национальных реестров идентификационных номеров Республики Казахстан" от 11 июня 2003 года N 565 - [Ссылка на источник приказа](https://adilet.zan.kz/rus/docs/P030000565_)
 
 ## Требования:
 - Python 3.7 и выше * **
 > \* судя по информации утилиты Vermin
 
 > ** я могу адаптировать (забэкпортить) библиотеку для более старых версии Python, но стоит ли оно? Если что дайте мне знать
 
 ## TODO:
 - Реализовать поддержку валидации БИН
-- Улучшеная документация
+- Улучшить документация
 - Static type hint using Mypy
 
 ## Схема формирования ИИН:
 <details>
   <summary>Схема</summary>
     <img src="https://raw.githubusercontent.com/ZhymabekRoman/kz-iin-validator/main/images/iin_schema.webp" alt="Schema IIN" />
 </details>
@@ -51,31 +55,34 @@
 ```bash
 python3 -m pip install git+https://github.com/ZhymabekRoman/kz-iin-validator
 ```
 
 ## Использование:
 ### Валидация ИИН:
 ```python
-from kz_iin_validator import validate_iin
+from kz_iin_validator import safe_validate_iin, validate_iin
 
 iin = "061211600012"
-validated_iin, error = validate_iin(iin)
+# use kz_iin_validator as in Golang (preferred in production)
+validated_iin, error = safe_validate_iin(iin)
+# or directly with exceptions raising:
+# validated_iin = validate_iin(iin)
 
 print(f"ИИН: {iin}")
 
 # Print IIN owner gender:
 print(f"Пол: {validated_iin.gender.name.upper()}")
 
 # Print IIN owner born information:
 print(f"День: {validated_iin.born_date.day}")
 print(f"Месяц: {validated_iin.born_date.month}")
 print(f"Год: {validated_iin.born_date.year}")
 
 # or directly access to datetime object:
-# validated_iin.born_date._datetime
+# validated_iin.born_date.datetime
 ```
 
 ### Генератор ИИН:
 ```python
 from kz_iin_validator import generate_iin
 
 generated_iin = generate_iin()
```

### Comparing `kz_iin_validator-0.5.0/setup.py` & `kz_iin_validator-0.6.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 def read_requirements(filename):
     with open(filename, "r", encoding="utf-8") as fp:
         return fp.read().strip().splitlines()
 
 
 setup(
     name="kz_iin_validator",
-    version="0.5.0",
+    version="0.6.0",
+    python_requires='>=3.7',
     author="Zhymabek Roman",
     author_email="robanokssamit@yandex.ru",
     long_description=readme_description,
     long_description_content_type="text/markdown",
     include_package_data=True,
     packages=find_packages(exclude=["tests", "images"]),
     url="https://github.com/ZhymabekRoman/kz-iin-validator",
-    license="LICENSE.txt",
+    license="MIT",
     description="Kazakhstan IIN parser and validator",
     install_requires=read_requirements("requirements.txt"),
 )
```

