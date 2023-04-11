# Comparing `tmp/fastapi_all_out-0.2.0.tar.gz` & `tmp/fastapi_all_out-0.2.1.tar.gz`

## Comparing `fastapi_all_out-0.2.0.tar` & `fastapi_all_out-0.2.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/__init__.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/app.py
--rw-r--r--   0        0        0     5065 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/code_responses.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/enums.py
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/lazy.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/mailing.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/models.py
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/responses.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/schemas.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/auth/__init__.py
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/auth/base.py
--rw-r--r--   0        0        0     5394 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/auth/router.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/auth/schemas.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/auth/user_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/auth/jwt/__init__.py
--rw-r--r--   0        0        0     6544 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/auth/jwt/backend.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/auth/jwt/schemas.py
--rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/auth/jwt/strategy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/auth/roles/__init__.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/auth/roles/router.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/auth/roles/schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/contrib/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/contrib/tortoise/__init__.py
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/contrib/tortoise/conntection.py
--rw-r--r--   0        0        0    33364 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/contrib/tortoise/repository.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/contrib/tortoise/repository_meta.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/contrib/tortoise/user_repository.py
--rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/contrib/tortoise/user_service.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/contrib/tortoise/fields/__init__.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/contrib/tortoise/fields/name_enum_field.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/contrib/tortoise/filters/__init__.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/contrib/tortoise/filters/fk.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/contrib/tortoise/filters/int.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/contrib/tortoise/filters/simple.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/contrib/tortoise/filters/str.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/contrib/tortoise/models/__init__.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/contrib/tortoise/models/base.py
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/contrib/tortoise/models/base_user.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/contrib/tortoise/models/content_type.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/contrib/tortoise/models/permissions.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/management/__init__.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/management/command.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/pydantic/__init__.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/pydantic/camel_model.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/pydantic/comma_separated.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/pydantic/fields/__init__.py
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/pydantic/fields/field_in_related_model.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/pydantic/fields/password.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/pydantic/fields/phonenumber.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/pydantic/fields/related_list.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/pydantic/fields/username.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/routers/__init__.py
--rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/routers/base_repository.py
--rw-r--r--   0        0        0    20297 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/routers/crud_router.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/routers/exceptions.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/routers/utils.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/routers/filters/__init__.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/routers/filters/base.py
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/routers/filters/bool.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/routers/filters/fk.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/routers/filters/int.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/routers/filters/int_btw.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/routers/filters/str.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/templates/activation.html
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/fastapi_all_out/templates/password_reset.html
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/LICENSE.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/README.md
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/__init__.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/app.py
+-rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/code_responses.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/enums.py
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/lazy.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/mailing.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/models.py
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/responses.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/schemas.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/auth/__init__.py
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/auth/base.py
+-rw-r--r--   0        0        0     5512 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/auth/router.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/auth/schemas.py
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/auth/user_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/auth/jwt/__init__.py
+-rw-r--r--   0        0        0     6716 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/auth/jwt/backend.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/auth/jwt/schemas.py
+-rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/auth/jwt/strategy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/auth/roles/__init__.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/auth/roles/router.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/auth/roles/schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/__init__.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/conntection.py
+-rw-r--r--   0        0        0    32984 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/repository.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/repository_meta.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/user_repository.py
+-rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/user_service.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/fields/__init__.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/fields/name_enum_field.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/filters/__init__.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/filters/fk.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/filters/int.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/filters/simple.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/filters/str.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/models/__init__.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/models/base.py
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/models/base_user.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/models/content_type.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/models/permissions.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/management/__init__.py
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/management/command.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/pydantic/__init__.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/pydantic/camel_model.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/pydantic/comma_separated.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/pydantic/fields/__init__.py
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/pydantic/fields/field_in_related_model.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/pydantic/fields/password.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/pydantic/fields/phonenumber.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/pydantic/fields/related_list.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/pydantic/fields/username.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/routers/__init__.py
+-rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/routers/base_repository.py
+-rw-r--r--   0        0        0    20297 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/routers/crud_router.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/routers/exceptions.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/routers/utils.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/routers/filters/__init__.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/routers/filters/base.py
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/routers/filters/bool.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/routers/filters/fk.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/routers/filters/int.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/routers/filters/int_btw.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/routers/filters/str.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/templates/activation.html
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/templates/password_reset.html
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/LICENSE.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/README.md
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/PKG-INFO
```

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/app.py` & `fastapi_all_out-0.2.1/fastapi_all_out/app.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/code_responses.py` & `fastapi_all_out-0.2.1/fastapi_all_out/code_responses.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from __future__ import annotations
 from enum import Enum
 from itertools import groupby
 from types import DynamicClassAttribute
-from typing import Any, Type
+from typing import Any, Type , Union
 
 from fastapi import BackgroundTasks
 
 from fastapi_all_out.pydantic import CamelModel, lower_camel
 from fastapi_all_out.responses import BgHTTPException
 
 
@@ -68,15 +67,15 @@
 
     def resp_detail(self, **kwargs) -> dict[str, Any]:
         return {**self.resp, **kwargs}
 
     @classmethod
     def responses(
             cls,
-            *codes: BaseCodes | tuple[BaseCodes, dict[str, Any]],
+            *codes: Union["BaseCodes", tuple["BaseCodes", dict[str, Any]]],
     ) -> dict[int, dict[str, Any]]:
 
         def key(x: BaseCodes | tuple[BaseCodes, dict[str, Any]]):
             if isinstance(x, tuple):
                 x = x[0]
             return x.status
```

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/lazy.py` & `fastapi_all_out-0.2.1/fastapi_all_out/lazy.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/mailing.py` & `fastapi_all_out-0.2.1/fastapi_all_out/mailing.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/models.py` & `fastapi_all_out-0.2.1/fastapi_all_out/models.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/responses.py` & `fastapi_all_out-0.2.1/fastapi_all_out/responses.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/settings.py` & `fastapi_all_out-0.2.1/fastapi_all_out/settings.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/auth/base.py` & `fastapi_all_out-0.2.1/fastapi_all_out/auth/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from abc import ABC, abstractmethod
 from datetime import datetime
 from typing import Callable, Coroutine, Any, Optional
 from uuid import UUID
 
 from fastapi import APIRouter
+from fastapi_all_out.lazy import get_codes
+
+
+Codes = get_codes()
 
 
 class AuthStrategy(ABC):
     authorize_response_model: Any
 
     def authorize(self, user) -> Any: ...
 
@@ -24,15 +28,34 @@
 
     @abstractmethod
     def auth_required(self) -> Callable[[], Coroutine[Any, Any, None]]: ...
 
     @abstractmethod
     def with_permissions(self, *permissions: tuple[str, str]) -> Callable[[], Coroutine[Any, Any, None]]: ...
 
-    def create_router(self, **kwargs) -> APIRouter: ...
+    def create_router(
+            self,
+            add_login_route: bool = True,
+            add_logout_route: bool = True,
+            **kwargs
+    ) -> APIRouter:
+        kwargs.setdefault('prefix', '/auth/jwt')
+        kwargs.setdefault('tags', ['auth'])
+        router = APIRouter(**kwargs)
+        if add_login_route:
+            self.add_login_route(router)
+        if add_logout_route:
+            self.add_logout_route(router)
+        return router
+
+    @abstractmethod
+    def add_login_route(self, router: APIRouter) -> None: ...
+
+    @abstractmethod
+    def add_logout_route(self, router: APIRouter) -> None: ...
 
 
 class BaseUser:
     id: int
     uuid: UUID
     username: Optional[str]
     email: Optional[str]
```

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/auth/router.py` & `fastapi_all_out-0.2.1/fastapi_all_out/auth/router.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 
 
 auth_backend = get_auth_backend()
 UserRepository = get_user_repository()
 UserService = get_user_service()
 Codes = get_codes()
 UserRead = get_schema(UserRead)
+UserMeRead = get_schema(UserMeRead)
 UserEdit = get_schema(UserEdit)
+UserMeEdit = get_schema(UserMeEdit)
 UserCreate = get_schema(UserCreate)
 UserRegistration = get_schema(UserRegistration)
 
 
 def create_users_router(
         add_get_me_route: bool = True,
         add_edit_me_route: bool = True,
@@ -83,15 +85,16 @@
                 raise router.field_errors(e)
             user_service = UserService(user)
             await user_service.post_registration(request=request, background_tasks=background_tasks)
             return Codes.activation_email.resp_detail(uuid=user_service.user.uuid)
 
     if add_account_activation_route:
         @router.get(
-            '/activation', response_model=auth_backend.strategy.authorize_response_model, responses=Codes.responses(
+            '/activation', response_model=auth_backend.strategy.authorize_response_model, response_model_by_alias=False,
+            responses=Codes.responses(
                 router.not_found_error_instance(),
                 Codes.activation_email_resend,
                 Codes.activation_email_code_incorrect,
                 Codes.already_active,
             )
         )
         async def activate_account(
```

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/auth/schemas.py` & `fastapi_all_out-0.2.1/fastapi_all_out/auth/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/auth/user_service.py` & `fastapi_all_out-0.2.1/fastapi_all_out/auth/user_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import TypeVar, Any, Generic, Literal
 from abc import ABC, abstractmethod
 
 from passlib.context import CryptContext
-from fastapi import Request, BackgroundTasks
+from fastapi import Request, BackgroundTasks, Response
 
 from fastapi_all_out.enums import TempCodeTriggers
 from .base import BaseUser
 
 
 USER_MODEL = TypeVar("USER_MODEL", bound=BaseUser)
 UNUSED_PASSWORD_PREFIX = '!'
@@ -19,14 +19,17 @@
 
     def __init__(self, user: USER_MODEL):
         self.user = user
 
     def can_login(self) -> bool:
         return self.user.is_active
 
+    async def if_cant_login(self, request: Request, background_tasks: BackgroundTasks, response: Response) -> None:
+        pass
+
     def token_expired(self, iat: int) -> bool:
         return self.user.password_change_dt.timestamp() > iat
 
     @abstractmethod
     def set_password(self, password: str) -> None: ...
 
     def get_fake_password(self, password: str) -> str:
```

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/auth/jwt/backend.py` & `fastapi_all_out-0.2.1/fastapi_all_out/auth/jwt/backend.py`

 * *Files 9% similar despite different names*

```diff
@@ -91,31 +91,29 @@
                     raise Codes.not_authenticated.err()
 
             if not (user.is_superuser or user.has_permissions(*permissions)):
                 raise Codes.permission_denied.err()
 
         return wrapper
 
-    def create_router(self, **kwargs) -> APIRouter:
-        kwargs.setdefault('prefix', '/auth/jwt')
-        kwargs.setdefault('tags', ['auth'])
-        router = APIRouter(**kwargs)
-
-        self.add_login_route(router)
-        self.add_logout_route(router)
-        self.add_refresh_route(router)
-
+    def create_router(self, add_refresh_route: bool = True, **kwargs) -> APIRouter:
+        router = super().create_router(**kwargs)
+        if add_refresh_route:
+            self.add_refresh_route(router)
         return router
 
+    def login_responses(self):
+        return Codes.responses(Codes.not_authenticated)
+
     def add_login_route(self, router: APIRouter) -> None:
         @router.post(
             '/login', response_model=self.strategy.authorize_response_model, response_model_by_alias=False,
-            responses=Codes.responses(Codes.not_authenticated)
+            responses=self.login_responses()
         )
-        async def wrapper(
+        async def login(
                 request: Request,
                 background_tasks: BackgroundTasks,
                 response: Response,
                 form: OAuth2PasswordRequestForm = Depends(),
         ):
             login_password = LoginPasswordSchema(login=form.username, password=form.password)
             field, value = login_password.get_auth_field_and_value()
@@ -126,26 +124,30 @@
                 raise Codes.not_authenticated.err()
 
             user_service = UserService(user)
             if not user_service.verify_password(password=login_password.password):
                 raise Codes.not_authenticated.err()
 
             if not user_service.can_login():
+                await user_service.if_cant_login(request=request, background_tasks=background_tasks, response=response)
                 raise Codes.not_authenticated.err()
             return self.strategy.authorize(user)
 
     def add_logout_route(self, router: APIRouter) -> None:
         pass
 
+    def refresh_responses(self):
+        return Codes.responses(Codes.not_authenticated)
+
     def add_refresh_route(self, router: APIRouter) -> None:
         @router.post(
             '/refresh', response_model=self.strategy.authorize_response_model, response_model_by_alias=False,
-            responses=Codes.responses(Codes.not_authenticated)
+            responses=self.refresh_responses()
         )
-        async def wrapper(
+        async def refresh(
                 request: Request,
                 background_tasks: BackgroundTasks,
                 response: Response,
                 token: str = Body(..., alias='refreshToken')
         ):
             token = self.strategy.get_refresh_token(token)
             try:
```

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/auth/jwt/schemas.py` & `fastapi_all_out-0.2.1/fastapi_all_out/auth/jwt/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/auth/jwt/strategy.py` & `fastapi_all_out-0.2.1/fastapi_all_out/auth/jwt/strategy.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/auth/roles/router.py` & `fastapi_all_out-0.2.1/fastapi_all_out/auth/roles/router.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/auth/roles/schemas.py` & `fastapi_all_out-0.2.1/fastapi_all_out/auth/roles/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/contrib/tortoise/conntection.py` & `fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/conntection.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/contrib/tortoise/repository.py` & `fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,44 +34,35 @@
     def __init__(self, *args, select_related: tuple[str] = (), prefetch_related: tuple[str] = (), **kwargs):
         super().__init__(*args, **kwargs)
         self.select_related = select_related
         self.prefetch_related = prefetch_related
         self.root_instance = None
 
     def get_queryset(self):
-        if self.request is None:
-            path, method = '', ''
-        else:
-            path, method = self.request.scope['route'].path, self.request.method
-
         query = self.model.all()
-        if default_filters := self.qs_default_filters(path, method):
+        if default_filters := self.qs_default_filters():
             query = query.filter(**default_filters)
-        if annotate_fields := self.qs_annotate_fields(path, method):
+        if annotate_fields := self.qs_annotate_fields():
             query = query.annotate(**annotate_fields)
-        if final_select_related := {*self.qs_select_related(path, method), *self.select_related}:
+        if final_select_related := {*self.qs_select_related(), *self.select_related}:
             query = query.select_related(*final_select_related)
-        if final_prefetch_related := {*self.qs_prefetch_related(path, method), *self.prefetch_related}:
+        if final_prefetch_related := {*self.qs_prefetch_related(), *self.prefetch_related}:
             query = query.prefetch_related(*final_prefetch_related)
         return query
 
-    @classmethod
-    def qs_default_filters(cls, path: str, method: str) -> dict[str, Any]:
+    def qs_default_filters(self) -> dict[str, Any]:
         return {}
 
-    @classmethod
-    def qs_annotate_fields(cls, path: str, method: str) -> dict[str, Any]:
+    def qs_annotate_fields(self) -> dict[str, Any]:
         return {}
 
-    @classmethod
-    def qs_select_related(cls, path: str, method: str) -> set[str]:
+    def qs_select_related(self) -> set[str]:
         return set()
 
-    @classmethod
-    def qs_prefetch_related(cls, path: str, method: str) -> set[str]:
+    def qs_prefetch_related(self) -> set[str]:
         return set()
 
     async def get_all(
             self,
             skip: Optional[int],
             limit: Optional[int],
             sort: set[str],
```

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/contrib/tortoise/user_repository.py` & `fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/user_repository.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/contrib/tortoise/user_service.py` & `fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/user_service.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/contrib/tortoise/fields/name_enum_field.py` & `fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/fields/name_enum_field.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/contrib/tortoise/filters/simple.py` & `fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/filters/simple.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/contrib/tortoise/filters/str.py` & `fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/filters/str.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/contrib/tortoise/models/base.py` & `fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/models/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/contrib/tortoise/models/base_user.py` & `fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/models/base_user.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/contrib/tortoise/models/content_type.py` & `fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/models/content_type.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/contrib/tortoise/models/permissions.py` & `fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/models/permissions.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/management/command.py` & `fastapi_all_out-0.2.1/fastapi_all_out/management/command.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/pydantic/camel_model.py` & `fastapi_all_out-0.2.1/fastapi_all_out/pydantic/camel_model.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/pydantic/comma_separated.py` & `fastapi_all_out-0.2.1/fastapi_all_out/pydantic/comma_separated.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/pydantic/fields/field_in_related_model.py` & `fastapi_all_out-0.2.1/fastapi_all_out/pydantic/fields/field_in_related_model.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/pydantic/fields/password.py` & `fastapi_all_out-0.2.1/fastapi_all_out/pydantic/fields/password.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/pydantic/fields/phonenumber.py` & `fastapi_all_out-0.2.1/fastapi_all_out/pydantic/fields/phonenumber.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/pydantic/fields/related_list.py` & `fastapi_all_out-0.2.1/fastapi_all_out/pydantic/fields/related_list.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/pydantic/fields/username.py` & `fastapi_all_out-0.2.1/fastapi_all_out/pydantic/fields/username.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/routers/base_repository.py` & `fastapi_all_out-0.2.1/fastapi_all_out/routers/base_repository.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,14 +48,24 @@
             background_tasks: Optional[BackgroundTasks] = None,
             response: Optional[Response] = None
     ):
         self.request = request
         self.background_tasks = background_tasks
         self.response = response
 
+    @property
+    def request_path(self) -> Optional[str]:
+        if self.request:
+            return self.request.scope['route'].path
+
+    @property
+    def request_method(self) -> Optional[str]:
+        if self.request:
+            return self.request.method.upper()
+
     @abstractmethod
     def get_queryset(self): ...
 
     @abstractmethod
     async def get_all(
             self,
             skip: Optional[int],
```

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/routers/crud_router.py` & `fastapi_all_out-0.2.1/fastapi_all_out/routers/crud_router.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/routers/exceptions.py` & `fastapi_all_out-0.2.1/fastapi_all_out/routers/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/routers/utils.py` & `fastapi_all_out-0.2.1/fastapi_all_out/routers/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/routers/filters/base.py` & `fastapi_all_out-0.2.1/fastapi_all_out/routers/filters/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/routers/filters/bool.py` & `fastapi_all_out-0.2.1/fastapi_all_out/routers/filters/bool.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/routers/filters/int.py` & `fastapi_all_out-0.2.1/fastapi_all_out/routers/filters/int.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/routers/filters/int_btw.py` & `fastapi_all_out-0.2.1/fastapi_all_out/routers/filters/int_btw.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/routers/filters/str.py` & `fastapi_all_out-0.2.1/fastapi_all_out/routers/filters/str.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/templates/activation.html` & `fastapi_all_out-0.2.1/fastapi_all_out/templates/activation.html`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/fastapi_all_out/templates/password_reset.html` & `fastapi_all_out-0.2.1/fastapi_all_out/templates/password_reset.html`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/LICENSE.md` & `fastapi_all_out-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.0/pyproject.toml` & `fastapi_all_out-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.hatch.build]
 ignore-vcs = true
 include = ["fastapi_all_out"]
 
 [project]
 name = "fastapi-all-out"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Alexandr Tamrazov", email="alta77@mail.ru" },
 ]
 maintainers = [
   { name="Alexandr Tamrazov", email="alta77@mail.ru" },
 ]
 keywords = ["DDD", "Domain-driven design", "Database", "WEB", "Architecture", "Backend"]
```

### Comparing `fastapi_all_out-0.2.0/PKG-INFO` & `fastapi_all_out-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-all-out
-Version: 0.2.0
+Version: 0.2.1
 Summary: Makes fastapi much easier and stronger, then Django
 Project-URL: Github, https://github.com/alta7700/fastapi_all_out/
 Author-email: Alexandr Tamrazov <alta77@mail.ru>
 Maintainer-email: Alexandr Tamrazov <alta77@mail.ru>
 License: Copyright © 2023 Alexandr Tamrazov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

