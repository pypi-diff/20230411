# Comparing `tmp/litestar-2.0.0a3.tar.gz` & `tmp/litestar-2.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litestar-2.0.0a3.tar", max compression
+gzip compressed data, was "litestar-2.0.0a4.tar", max compression
```

## Comparing `litestar-2.0.0a3.tar` & `litestar-2.0.0a4.tar`

### file list

```diff
@@ -1,273 +1,273 @@
--rw-r--r--   0        0        0     1092 2023-04-07 17:38:15.152994 litestar-2.0.0a3/LICENSE
--rw-r--r--   0        0        0    47243 2023-04-07 17:38:15.152994 litestar-2.0.0a3/README.md
--rw-r--r--   0        0        0      744 2023-04-07 17:38:15.168995 litestar-2.0.0a3/litestar/__init__.py
--rw-r--r--   0        0        0      103 2023-04-07 17:38:15.168995 litestar-2.0.0a3/litestar/__main__.py
--rw-r--r--   0        0        0       77 2023-04-07 17:38:15.168995 litestar-2.0.0a3/litestar/_asgi/__init__.py
--rw-r--r--   0        0        0     8644 2023-04-07 17:38:15.168995 litestar-2.0.0a3/litestar/_asgi/asgi_router.py
--rw-r--r--   0        0        0      349 2023-04-07 17:38:15.168995 litestar-2.0.0a3/litestar/_asgi/routing_trie/__init__.py
--rw-r--r--   0        0        0     7823 2023-04-07 17:38:15.168995 litestar-2.0.0a3/litestar/_asgi/routing_trie/mapping.py
--rw-r--r--   0        0        0     5938 2023-04-07 17:38:15.168995 litestar-2.0.0a3/litestar/_asgi/routing_trie/traversal.py
--rw-r--r--   0        0        0     2598 2023-04-07 17:38:15.168995 litestar-2.0.0a3/litestar/_asgi/routing_trie/types.py
--rw-r--r--   0        0        0     1267 2023-04-07 17:38:15.168995 litestar-2.0.0a3/litestar/_asgi/routing_trie/validate.py
--rw-r--r--   0        0        0     1528 2023-04-07 17:38:15.168995 litestar-2.0.0a3/litestar/_asgi/utils.py
--rw-r--r--   0        0        0       66 2023-04-07 17:38:15.168995 litestar-2.0.0a3/litestar/_kwargs/__init__.py
--rw-r--r--   0        0        0     3868 2023-04-07 17:38:15.168995 litestar-2.0.0a3/litestar/_kwargs/cleanup.py
--rw-r--r--   0        0        0     4245 2023-04-07 17:38:15.168995 litestar-2.0.0a3/litestar/_kwargs/dependencies.py
--rw-r--r--   0        0        0    14496 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/_kwargs/extractors.py
--rw-r--r--   0        0        0    20822 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/_kwargs/kwargs_model.py
--rw-r--r--   0        0        0     2759 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/_kwargs/parameter_definition.py
--rw-r--r--   0        0        0        0 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/_layers/__init__.py
--rw-r--r--   0        0        0     1288 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/_layers/utils.py
--rw-r--r--   0        0        0     5935 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/_multipart.py
--rw-r--r--   0        0        0        0 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/_openapi/__init__.py
--rw-r--r--   0        0        0    10155 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/_openapi/parameters.py
--rw-r--r--   0        0        0     5490 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/_openapi/path_item.py
--rw-r--r--   0        0        0     1237 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/_openapi/request_body.py
--rw-r--r--   0        0        0    10005 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/_openapi/responses.py
--rw-r--r--   0        0        0       64 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/_openapi/schema_generation/__init__.py
--rw-r--r--   0        0        0     7009 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/_openapi/schema_generation/constrained_fields.py
--rw-r--r--   0        0        0     2093 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/_openapi/schema_generation/examples.py
--rw-r--r--   0        0        0    28143 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/_openapi/schema_generation/schema.py
--rw-r--r--   0        0        0        0 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/_openapi/typescript_converter/__init__.py
--rw-r--r--   0        0        0    10970 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/_openapi/typescript_converter/converter.py
--rw-r--r--   0        0        0     5242 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/_openapi/typescript_converter/schema_parsing.py
--rw-r--r--   0        0        0     7685 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/_openapi/typescript_converter/types.py
--rw-r--r--   0        0        0     1483 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/_openapi/utils.py
--rw-r--r--   0        0        0     2465 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/_parsers.py
--rw-r--r--   0        0        0      182 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/_signature/__init__.py
--rw-r--r--   0        0        0     5955 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/_signature/field.py
--rw-r--r--   0        0        0       64 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/_signature/models/__init__.py
--rw-r--r--   0        0        0    12437 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/_signature/models/attrs_signature_model.py
--rw-r--r--   0        0        0     3989 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/_signature/models/base.py
--rw-r--r--   0        0        0     7268 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/_signature/models/pydantic_signature_model.py
--rw-r--r--   0        0        0     8721 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/_signature/utils.py
--rw-r--r--   0        0        0    38451 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/app.py
--rw-r--r--   0        0        0     2200 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/background_tasks.py
--rw-r--r--   0        0        0        0 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/cli/__init__.py
--rw-r--r--   0        0        0    11820 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/cli/_utils.py
--rw-r--r--   0        0        0        0 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/cli/commands/__init__.py
--rw-r--r--   0        0        0     4553 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/cli/commands/core.py
--rw-r--r--   0        0        0     2365 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/cli/commands/schema.py
--rw-r--r--   0        0        0     2224 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/cli/commands/sessions.py
--rw-r--r--   0        0        0      807 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/cli/main.py
--rw-r--r--   0        0        0        0 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/config/__init__.py
--rw-r--r--   0        0        0     1747 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/config/allowed_hosts.py
--rw-r--r--   0        0        0    12358 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/config/app.py
--rw-r--r--   0        0        0     2742 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/config/compression.py
--rw-r--r--   0        0        0     5177 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/config/cors.py
--rw-r--r--   0        0        0     1771 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/config/csrf.py
--rw-r--r--   0        0        0     1991 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/config/response_cache.py
--rw-r--r--   0        0        0     1922 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/connection/__init__.py
--rw-r--r--   0        0        0    10838 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/connection/base.py
--rw-r--r--   0        0        0     7698 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/connection/request.py
--rw-r--r--   0        0        0     9005 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/connection/websocket.py
--rw-r--r--   0        0        0      997 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/constants.py
--rw-r--r--   0        0        0        0 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/contrib/htmx/__init__.py
--rw-r--r--   0        0        0     4917 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/contrib/htmx/_utils.py
--rw-r--r--   0        0        0     4051 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/contrib/htmx/request.py
--rw-r--r--   0        0        0     8349 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/contrib/htmx/response.py
--rw-r--r--   0        0        0     1261 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/contrib/htmx/types.py
--rw-r--r--   0        0        0     2557 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/contrib/jinja.py
--rw-r--r--   0        0        0      521 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/contrib/jwt/__init__.py
--rw-r--r--   0        0        0    28720 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/contrib/jwt/jwt_auth.py
--rw-r--r--   0        0        0     3978 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/contrib/jwt/jwt_token.py
--rw-r--r--   0        0        0     6970 2023-04-07 17:38:15.172995 litestar-2.0.0a3/litestar/contrib/jwt/middleware.py
--rw-r--r--   0        0        0     3916 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/contrib/mako.py
--rw-r--r--   0        0        0        0 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/contrib/msgspec/__init__.py
--rw-r--r--   0        0        0      180 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/contrib/opentelemetry/__init__.py
--rw-r--r--   0        0        0      845 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/contrib/opentelemetry/_utils.py
--rw-r--r--   0        0        0     4206 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/contrib/opentelemetry/config.py
--rw-r--r--   0        0        0     2212 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/contrib/opentelemetry/middleware.py
--rw-r--r--   0        0        0     4044 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/contrib/piccolo_orm.py
--rw-r--r--   0        0        0        0 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/contrib/pydantic/__init__.py
--rw-r--r--   0        0        0      280 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/contrib/repository/__init__.py
--rw-r--r--   0        0        0     9079 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/contrib/repository/abc.py
--rw-r--r--   0        0        0      328 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/contrib/repository/exceptions.py
--rw-r--r--   0        0        0     1162 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/contrib/repository/filters.py
--rw-r--r--   0        0        0        0 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/contrib/repository/testing/__init__.py
--rw-r--r--   0        0        0    12484 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/contrib/repository/testing/generic_mock_repository.py
--rw-r--r--   0        0        0        0 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     3460 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/contrib/sqlalchemy/base.py
--rw-r--r--   0        0        0        0 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/contrib/sqlalchemy/dto.py
--rw-r--r--   0        0        0      390 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/contrib/sqlalchemy/init_plugin/__init__.py
--rw-r--r--   0        0        0      458 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/contrib/sqlalchemy/init_plugin/config/__init__.py
--rw-r--r--   0        0        0     3602 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/contrib/sqlalchemy/init_plugin/config/asyncio.py
--rw-r--r--   0        0        0    11308 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/contrib/sqlalchemy/init_plugin/config/common.py
--rw-r--r--   0        0        0    11499 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/contrib/sqlalchemy/init_plugin/config/engine.py
--rw-r--r--   0        0        0     2849 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/contrib/sqlalchemy/init_plugin/config/sync.py
--rw-r--r--   0        0        0     1527 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/contrib/sqlalchemy/init_plugin/plugin.py
--rw-r--r--   0        0        0    19731 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/contrib/sqlalchemy/repository.py
--rw-r--r--   0        0        0        0 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/contrib/sqlalchemy_1/__init__.py
--rw-r--r--   0        0        0    13770 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/contrib/sqlalchemy_1/config.py
--rw-r--r--   0        0        0    19447 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/contrib/sqlalchemy_1/plugin.py
--rw-r--r--   0        0        0     1319 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/contrib/sqlalchemy_1/types.py
--rw-r--r--   0        0        0     6071 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/contrib/tortoise_orm.py
--rw-r--r--   0        0        0     9559 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/controller.py
--rw-r--r--   0        0        0    16462 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/data_extractors.py
--rw-r--r--   0        0        0      883 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/datastructures/__init__.py
--rw-r--r--   0        0        0     3757 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/datastructures/cookie.py
--rw-r--r--   0        0        0    17316 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/datastructures/headers.py
--rw-r--r--   0        0        0     2977 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/datastructures/multi_dicts.py
--rw-r--r--   0        0        0     5027 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/datastructures/response_header.py
--rw-r--r--   0        0        0     9302 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/datastructures/state.py
--rw-r--r--   0        0        0     3360 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/datastructures/upload_file.py
--rw-r--r--   0        0        0     7273 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/datastructures/url.py
--rw-r--r--   0        0        0     2386 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/di.py
--rw-r--r--   0        0        0        0 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/dto/__init__.py
--rw-r--r--   0        0        0      337 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/dto/exceptions.py
--rw-r--r--   0        0        0     2537 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/dto/interface.py
--rw-r--r--   0        0        0     1728 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/enums.py
--rw-r--r--   0        0        0      201 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/events/__init__.py
--rw-r--r--   0        0        0     4597 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/events/emitter.py
--rw-r--r--   0        0        0     1305 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/events/listener.py
--rw-r--r--   0        0        0     1142 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/exceptions/__init__.py
--rw-r--r--   0        0        0     1608 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/exceptions/base_exceptions.py
--rw-r--r--   0        0        0     4629 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/exceptions/http_exceptions.py
--rw-r--r--   0        0        0     1351 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/exceptions/websocket_exceptions.py
--rw-r--r--   0        0        0     5350 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/file_system.py
--rw-r--r--   0        0        0      559 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/handlers/__init__.py
--rw-r--r--   0        0        0     3877 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/handlers/asgi_handlers.py
--rw-r--r--   0        0        0    16408 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/handlers/base.py
--rw-r--r--   0        0        0      263 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/handlers/http_handlers/__init__.py
--rw-r--r--   0        0        0     9280 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/handlers/http_handlers/_utils.py
--rw-r--r--   0        0        0    25419 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/handlers/http_handlers/base.py
--rw-r--r--   0        0        0    60867 2023-04-07 17:38:15.176996 litestar-2.0.0a3/litestar/handlers/http_handlers/decorators.py
--rw-r--r--   0        0        0    16609 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/handlers/websocket_handlers.py
--rw-r--r--   0        0        0      147 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/logging/__init__.py
--rw-r--r--   0        0        0      569 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/logging/_utils.py
--rw-r--r--   0        0        0    12050 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/logging/config.py
--rw-r--r--   0        0        0     1129 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/logging/picologging.py
--rw-r--r--   0        0        0      860 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/logging/standard.py
--rw-r--r--   0        0        0      385 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/middleware/__init__.py
--rw-r--r--   0        0        0     2081 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/middleware/_utils.py
--rw-r--r--   0        0        0     2973 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/middleware/allowed_hosts.py
--rw-r--r--   0        0        0     3436 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/middleware/authentication.py
--rw-r--r--   0        0        0     5302 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/middleware/base.py
--rw-r--r--   0        0        0     8367 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/middleware/compression.py
--rw-r--r--   0        0        0     2573 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/middleware/cors.py
--rw-r--r--   0        0        0     6474 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/middleware/csrf.py
--rw-r--r--   0        0        0      124 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/middleware/exceptions/__init__.py
--rw-r--r--   0        0        0     7191 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/middleware/exceptions/_debug_response.py
--rw-r--r--   0        0        0     9006 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/middleware/exceptions/middleware.py
--rw-r--r--   0        0        0      398 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/middleware/exceptions/templates/body.html
--rw-r--r--   0        0        0      344 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/middleware/exceptions/templates/frame.html
--rw-r--r--   0        0        0      920 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/middleware/exceptions/templates/scripts.js
--rw-r--r--   0        0        0     1830 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/middleware/exceptions/templates/styles.css
--rw-r--r--   0        0        0    13393 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/middleware/logging.py
--rw-r--r--   0        0        0    10821 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/middleware/rate_limit.py
--rw-r--r--   0        0        0       70 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/middleware/session/__init__.py
--rw-r--r--   0        0        0     7961 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/middleware/session/base.py
--rw-r--r--   0        0        0    10387 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/middleware/session/client_side.py
--rw-r--r--   0        0        0     8580 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/middleware/session/server_side.py
--rw-r--r--   0        0        0      231 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/__init__.py
--rw-r--r--   0        0        0     5226 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/config.py
--rw-r--r--   0        0        0    16449 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/controller.py
--rw-r--r--   0        0        0      898 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/datastructures.py
--rw-r--r--   0        0        0     1691 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/spec/__init__.py
--rw-r--r--   0        0        0     1648 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/spec/base.py
--rw-r--r--   0        0        0      961 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/spec/callback.py
--rw-r--r--   0        0        0     2936 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/spec/components.py
--rw-r--r--   0        0        0      592 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/spec/contact.py
--rw-r--r--   0        0        0      950 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/spec/discriminator.py
--rw-r--r--   0        0        0     3290 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/spec/encoding.py
--rw-r--r--   0        0        0      974 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/spec/enums.py
--rw-r--r--   0        0        0     1168 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/spec/example.py
--rw-r--r--   0        0        0      614 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/spec/external_documentation.py
--rw-r--r--   0        0        0     5669 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/spec/header.py
--rw-r--r--   0        0        0     1413 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/spec/info.py
--rw-r--r--   0        0        0      752 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/spec/license.py
--rw-r--r--   0        0        0     2876 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/spec/link.py
--rw-r--r--   0        0        0     1882 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/spec/media_type.py
--rw-r--r--   0        0        0     1195 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/spec/oauth_flow.py
--rw-r--r--   0        0        0      897 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/spec/oauth_flows.py
--rw-r--r--   0        0        0     4218 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/spec/open_api.py
--rw-r--r--   0        0        0     4842 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/spec/operation.py
--rw-r--r--   0        0        0     6242 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/spec/parameter.py
--rw-r--r--   0        0        0     3245 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/spec/path_item.py
--rw-r--r--   0        0        0     1255 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/spec/paths.py
--rw-r--r--   0        0        0     1351 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/spec/reference.py
--rw-r--r--   0        0        0     1095 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/spec/request_body.py
--rw-r--r--   0        0        0     1854 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/spec/response.py
--rw-r--r--   0        0        0     2367 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/spec/responses.py
--rw-r--r--   0        0        0    34574 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/spec/schema.py
--rw-r--r--   0        0        0     1686 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/spec/security_requirement.py
--rw-r--r--   0        0        0     2690 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/spec/security_scheme.py
--rw-r--r--   0        0        0     1077 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/spec/server.py
--rw-r--r--   0        0        0     1171 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/spec/server_variable.py
--rw-r--r--   0        0        0      923 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/spec/tag.py
--rw-r--r--   0        0        0     1702 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/openapi/spec/xml.py
--rw-r--r--   0        0        0    10984 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/pagination.py
--rw-r--r--   0        0        0    16805 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/params.py
--rw-r--r--   0        0        0     6337 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/partial.py
--rw-r--r--   0        0        0     7209 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/plugins.py
--rw-r--r--   0        0        0        0 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/py.typed
--rw-r--r--   0        0        0      278 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/response/__init__.py
--rw-r--r--   0        0        0    12185 2023-04-07 17:38:15.180996 litestar-2.0.0a3/litestar/response/base.py
--rw-r--r--   0        0        0     8954 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/response/file.py
--rw-r--r--   0        0        0     2422 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/response/redirect.py
--rw-r--r--   0        0        0     4893 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/response/streaming.py
--rw-r--r--   0        0        0     2994 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/response/template.py
--rw-r--r--   0        0        0    14975 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/response_containers.py
--rw-r--r--   0        0        0    15028 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/router.py
--rw-r--r--   0        0        0      191 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/routes/__init__.py
--rw-r--r--   0        0        0     1763 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/routes/asgi.py
--rw-r--r--   0        0        0     6443 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/routes/base.py
--rw-r--r--   0        0        0    13384 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/routes/http.py
--rw-r--r--   0        0        0     3058 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/routes/websocket.py
--rw-r--r--   0        0        0       97 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/security/__init__.py
--rw-r--r--   0        0        0     7165 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/security/base.py
--rw-r--r--   0        0        0      188 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/security/session_auth/__init__.py
--rw-r--r--   0        0        0     5602 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/security/session_auth/auth.py
--rw-r--r--   0        0        0     4941 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/security/session_auth/middleware.py
--rw-r--r--   0        0        0     6606 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/serialization.py
--rw-r--r--   0        0        0      158 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/static_files/__init__.py
--rw-r--r--   0        0        0     5019 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/static_files/base.py
--rw-r--r--   0        0        0     3582 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/static_files/config.py
--rw-r--r--   0        0        0     9536 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/status_codes.py
--rw-r--r--   0        0        0        0 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/stores/__init__.py
--rw-r--r--   0        0        0     4377 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/stores/base.py
--rw-r--r--   0        0        0     5425 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/stores/file.py
--rw-r--r--   0        0        0     3625 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/stores/memory.py
--rw-r--r--   0        0        0     6231 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/stores/redis.py
--rw-r--r--   0        0        0     2233 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/stores/registry.py
--rw-r--r--   0        0        0      204 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/template/__init__.py
--rw-r--r--   0        0        0     4113 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/template/base.py
--rw-r--r--   0        0        0     1894 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/template/config.py
--rw-r--r--   0        0        0      581 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/testing/__init__.py
--rw-r--r--   0        0        0     1816 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/testing/client/__init__.py
--rw-r--r--   0        0        0    17450 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/testing/client/async_client.py
--rw-r--r--   0        0        0     5132 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/testing/client/base.py
--rw-r--r--   0        0        0    19556 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/testing/client/sync_client.py
--rw-r--r--   0        0        0    31465 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/testing/helpers.py
--rw-r--r--   0        0        0     2534 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/testing/life_span_handler.py
--rw-r--r--   0        0        0    21905 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/testing/request_factory.py
--rw-r--r--   0        0        0     8094 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/testing/transport.py
--rw-r--r--   0        0        0     6943 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/testing/websocket_test_session.py
--rw-r--r--   0        0        0     4105 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/types/__init__.py
--rw-r--r--   0        0        0     8697 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/types/asgi_types.py
--rw-r--r--   0        0        0      453 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/types/builtin_types.py
--rw-r--r--   0        0        0     2291 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/types/callable_types.py
--rw-r--r--   0        0        0     1645 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/types/composite_types.py
--rw-r--r--   0        0        0      183 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/types/empty.py
--rw-r--r--   0        0        0     2662 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/types/file_types.py
--rw-r--r--   0        0        0      344 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/types/helper_types.py
--rw-r--r--   0        0        0     1487 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/types/internal_types.py
--rw-r--r--   0        0        0     8707 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/types/parsed_signature.py
--rw-r--r--   0        0        0     2407 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/types/protocols.py
--rw-r--r--   0        0        0     1820 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/types/serialization.py
--rw-r--r--   0        0        0     1718 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/utils/__init__.py
--rw-r--r--   0        0        0      729 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/utils/compat.py
--rw-r--r--   0        0        0     3449 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/utils/dataclass.py
--rw-r--r--   0        0        0     3520 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/utils/deprecation.py
--rw-r--r--   0        0        0     1483 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/utils/helpers.py
--rw-r--r--   0        0        0      723 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/utils/path.py
--rw-r--r--   0        0        0     9389 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/utils/predicates.py
--rw-r--r--   0        0        0     2720 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/utils/scope.py
--rw-r--r--   0        0        0      992 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/utils/sequence.py
--rw-r--r--   0        0        0     1970 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/utils/signature_parsing.py
--rw-r--r--   0        0        0     5351 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/utils/sync.py
--rw-r--r--   0        0        0     6156 2023-04-07 17:38:15.184996 litestar-2.0.0a3/litestar/utils/typing.py
--rw-r--r--   0        0        0     1921 2023-04-07 17:38:15.188996 litestar-2.0.0a3/litestar/utils/version.py
--rw-r--r--   0        0        0     9225 2023-04-07 17:38:15.188996 litestar-2.0.0a3/pyproject.toml
--rw-r--r--   0        0        0    50598 1970-01-01 00:00:00.000000 litestar-2.0.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-04-11 16:09:54.380440 litestar-2.0.0a4/LICENSE
+-rw-r--r--   0        0        0    48376 2023-04-11 16:09:54.380440 litestar-2.0.0a4/README.md
+-rw-r--r--   0        0        0      744 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/__init__.py
+-rw-r--r--   0        0        0      103 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/__main__.py
+-rw-r--r--   0        0        0       77 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_asgi/__init__.py
+-rw-r--r--   0        0        0     8644 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_asgi/asgi_router.py
+-rw-r--r--   0        0        0      349 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_asgi/routing_trie/__init__.py
+-rw-r--r--   0        0        0     7823 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_asgi/routing_trie/mapping.py
+-rw-r--r--   0        0        0     5938 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_asgi/routing_trie/traversal.py
+-rw-r--r--   0        0        0     2598 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_asgi/routing_trie/types.py
+-rw-r--r--   0        0        0     1267 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_asgi/routing_trie/validate.py
+-rw-r--r--   0        0        0     1528 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_asgi/utils.py
+-rw-r--r--   0        0        0       66 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_kwargs/__init__.py
+-rw-r--r--   0        0        0     3868 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_kwargs/cleanup.py
+-rw-r--r--   0        0        0     4245 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_kwargs/dependencies.py
+-rw-r--r--   0        0        0    14489 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_kwargs/extractors.py
+-rw-r--r--   0        0        0    20815 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_kwargs/kwargs_model.py
+-rw-r--r--   0        0        0     2759 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_kwargs/parameter_definition.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_layers/__init__.py
+-rw-r--r--   0        0        0     1288 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_layers/utils.py
+-rw-r--r--   0        0        0     5935 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_multipart.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_openapi/__init__.py
+-rw-r--r--   0        0        0    10155 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_openapi/parameters.py
+-rw-r--r--   0        0        0     5490 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_openapi/path_item.py
+-rw-r--r--   0        0        0     1237 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_openapi/request_body.py
+-rw-r--r--   0        0        0    10005 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_openapi/responses.py
+-rw-r--r--   0        0        0       64 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_openapi/schema_generation/__init__.py
+-rw-r--r--   0        0        0     7120 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_openapi/schema_generation/constrained_fields.py
+-rw-r--r--   0        0        0     2093 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_openapi/schema_generation/examples.py
+-rw-r--r--   0        0        0    28352 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_openapi/schema_generation/schema.py
+-rw-r--r--   0        0        0      524 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_openapi/schema_generation/utils.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_openapi/typescript_converter/__init__.py
+-rw-r--r--   0        0        0    10970 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_openapi/typescript_converter/converter.py
+-rw-r--r--   0        0        0     5242 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_openapi/typescript_converter/schema_parsing.py
+-rw-r--r--   0        0        0     7685 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_openapi/typescript_converter/types.py
+-rw-r--r--   0        0        0     1483 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_openapi/utils.py
+-rw-r--r--   0        0        0     2465 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_parsers.py
+-rw-r--r--   0        0        0      182 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_signature/__init__.py
+-rw-r--r--   0        0        0     5995 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_signature/field.py
+-rw-r--r--   0        0        0       64 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_signature/models/__init__.py
+-rw-r--r--   0        0        0    12635 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_signature/models/attrs_signature_model.py
+-rw-r--r--   0        0        0     3982 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_signature/models/base.py
+-rw-r--r--   0        0        0     7456 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_signature/models/pydantic_signature_model.py
+-rw-r--r--   0        0        0     8714 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_signature/utils.py
+-rw-r--r--   0        0        0    38796 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/app.py
+-rw-r--r--   0        0        0     2200 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/background_tasks.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/cli/__init__.py
+-rw-r--r--   0        0        0    11820 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/cli/_utils.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/cli/commands/__init__.py
+-rw-r--r--   0        0        0     4553 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/cli/commands/core.py
+-rw-r--r--   0        0        0     2365 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/cli/commands/schema.py
+-rw-r--r--   0        0        0     2224 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/cli/commands/sessions.py
+-rw-r--r--   0        0        0      807 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/cli/main.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/config/__init__.py
+-rw-r--r--   0        0        0     1747 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/config/allowed_hosts.py
+-rw-r--r--   0        0        0    12358 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/config/app.py
+-rw-r--r--   0        0        0     2742 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/config/compression.py
+-rw-r--r--   0        0        0     5177 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/config/cors.py
+-rw-r--r--   0        0        0     1771 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/config/csrf.py
+-rw-r--r--   0        0        0     1991 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/config/response_cache.py
+-rw-r--r--   0        0        0     1922 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/connection/__init__.py
+-rw-r--r--   0        0        0    10838 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/connection/base.py
+-rw-r--r--   0        0        0     7698 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/connection/request.py
+-rw-r--r--   0        0        0     9005 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/connection/websocket.py
+-rw-r--r--   0        0        0     1098 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/constants.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/htmx/__init__.py
+-rw-r--r--   0        0        0     4917 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/htmx/_utils.py
+-rw-r--r--   0        0        0     4051 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/htmx/request.py
+-rw-r--r--   0        0        0     8349 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/htmx/response.py
+-rw-r--r--   0        0        0     1261 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/htmx/types.py
+-rw-r--r--   0        0        0     2557 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/jinja.py
+-rw-r--r--   0        0        0      521 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/jwt/__init__.py
+-rw-r--r--   0        0        0    28720 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/jwt/jwt_auth.py
+-rw-r--r--   0        0        0     3978 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/jwt/jwt_token.py
+-rw-r--r--   0        0        0     6970 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/jwt/middleware.py
+-rw-r--r--   0        0        0     3916 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/mako.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/msgspec/__init__.py
+-rw-r--r--   0        0        0      180 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/opentelemetry/__init__.py
+-rw-r--r--   0        0        0      845 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/opentelemetry/_utils.py
+-rw-r--r--   0        0        0     4206 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/opentelemetry/config.py
+-rw-r--r--   0        0        0     2212 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/opentelemetry/middleware.py
+-rw-r--r--   0        0        0     4044 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/piccolo_orm.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/pydantic/__init__.py
+-rw-r--r--   0        0        0      280 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/repository/__init__.py
+-rw-r--r--   0        0        0     9079 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/repository/abc.py
+-rw-r--r--   0        0        0      328 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/repository/exceptions.py
+-rw-r--r--   0        0        0     1162 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/repository/filters.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/repository/testing/__init__.py
+-rw-r--r--   0        0        0    12484 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/repository/testing/generic_mock_repository.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     3460 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/sqlalchemy/base.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/sqlalchemy/dto.py
+-rw-r--r--   0        0        0      390 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/sqlalchemy/init_plugin/__init__.py
+-rw-r--r--   0        0        0      458 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/sqlalchemy/init_plugin/config/__init__.py
+-rw-r--r--   0        0        0     3602 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/sqlalchemy/init_plugin/config/asyncio.py
+-rw-r--r--   0        0        0    11308 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/sqlalchemy/init_plugin/config/common.py
+-rw-r--r--   0        0        0    11499 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/sqlalchemy/init_plugin/config/engine.py
+-rw-r--r--   0        0        0     2849 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/sqlalchemy/init_plugin/config/sync.py
+-rw-r--r--   0        0        0     1527 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/sqlalchemy/init_plugin/plugin.py
+-rw-r--r--   0        0        0    19731 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/sqlalchemy/repository.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/sqlalchemy_1/__init__.py
+-rw-r--r--   0        0        0    13770 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/sqlalchemy_1/config.py
+-rw-r--r--   0        0        0    19447 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/sqlalchemy_1/plugin.py
+-rw-r--r--   0        0        0     1319 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/sqlalchemy_1/types.py
+-rw-r--r--   0        0        0     6071 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/tortoise_orm.py
+-rw-r--r--   0        0        0     9559 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/controller.py
+-rw-r--r--   0        0        0    16462 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/data_extractors.py
+-rw-r--r--   0        0        0      883 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/datastructures/__init__.py
+-rw-r--r--   0        0        0     3757 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/datastructures/cookie.py
+-rw-r--r--   0        0        0    17316 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/datastructures/headers.py
+-rw-r--r--   0        0        0     2977 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/datastructures/multi_dicts.py
+-rw-r--r--   0        0        0     5027 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/datastructures/response_header.py
+-rw-r--r--   0        0        0     9302 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/datastructures/state.py
+-rw-r--r--   0        0        0     3360 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/datastructures/upload_file.py
+-rw-r--r--   0        0        0     7273 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/datastructures/url.py
+-rw-r--r--   0        0        0     2386 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/di.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/dto/__init__.py
+-rw-r--r--   0        0        0      337 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/dto/exceptions.py
+-rw-r--r--   0        0        0     2484 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/dto/interface.py
+-rw-r--r--   0        0        0     1728 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/enums.py
+-rw-r--r--   0        0        0      201 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/events/__init__.py
+-rw-r--r--   0        0        0     4597 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/events/emitter.py
+-rw-r--r--   0        0        0     1305 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/events/listener.py
+-rw-r--r--   0        0        0     1142 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/exceptions/__init__.py
+-rw-r--r--   0        0        0     1608 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/exceptions/base_exceptions.py
+-rw-r--r--   0        0        0     4629 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/exceptions/http_exceptions.py
+-rw-r--r--   0        0        0     1351 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/exceptions/websocket_exceptions.py
+-rw-r--r--   0        0        0     5350 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/file_system.py
+-rw-r--r--   0        0        0      559 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/handlers/__init__.py
+-rw-r--r--   0        0        0     3877 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/handlers/asgi_handlers.py
+-rw-r--r--   0        0        0    16350 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/handlers/base.py
+-rw-r--r--   0        0        0      263 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/handlers/http_handlers/__init__.py
+-rw-r--r--   0        0        0     9280 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/handlers/http_handlers/_utils.py
+-rw-r--r--   0        0        0    25419 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/handlers/http_handlers/base.py
+-rw-r--r--   0        0        0    60867 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/handlers/http_handlers/decorators.py
+-rw-r--r--   0        0        0    16602 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/handlers/websocket_handlers.py
+-rw-r--r--   0        0        0      147 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/logging/__init__.py
+-rw-r--r--   0        0        0      569 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/logging/_utils.py
+-rw-r--r--   0        0        0    12050 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/logging/config.py
+-rw-r--r--   0        0        0     1129 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/logging/picologging.py
+-rw-r--r--   0        0        0      860 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/logging/standard.py
+-rw-r--r--   0        0        0      385 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/__init__.py
+-rw-r--r--   0        0        0     2081 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/_utils.py
+-rw-r--r--   0        0        0     2973 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/allowed_hosts.py
+-rw-r--r--   0        0        0     3436 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/authentication.py
+-rw-r--r--   0        0        0     5302 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/base.py
+-rw-r--r--   0        0        0     8367 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/compression.py
+-rw-r--r--   0        0        0     2573 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/cors.py
+-rw-r--r--   0        0        0     6474 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/csrf.py
+-rw-r--r--   0        0        0      124 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/exceptions/__init__.py
+-rw-r--r--   0        0        0     7191 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/exceptions/_debug_response.py
+-rw-r--r--   0        0        0     9006 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/exceptions/middleware.py
+-rw-r--r--   0        0        0      398 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/exceptions/templates/body.html
+-rw-r--r--   0        0        0      344 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/exceptions/templates/frame.html
+-rw-r--r--   0        0        0      920 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/exceptions/templates/scripts.js
+-rw-r--r--   0        0        0     1830 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/exceptions/templates/styles.css
+-rw-r--r--   0        0        0    13393 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/logging.py
+-rw-r--r--   0        0        0    10821 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/rate_limit.py
+-rw-r--r--   0        0        0       70 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/session/__init__.py
+-rw-r--r--   0        0        0     7961 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/session/base.py
+-rw-r--r--   0        0        0    10387 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/session/client_side.py
+-rw-r--r--   0        0        0     8580 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/session/server_side.py
+-rw-r--r--   0        0        0      231 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/openapi/__init__.py
+-rw-r--r--   0        0        0     5226 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/openapi/config.py
+-rw-r--r--   0        0        0    16449 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/openapi/controller.py
+-rw-r--r--   0        0        0      898 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/openapi/datastructures.py
+-rw-r--r--   0        0        0     1691 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/openapi/spec/__init__.py
+-rw-r--r--   0        0        0     1648 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/openapi/spec/base.py
+-rw-r--r--   0        0        0      961 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/openapi/spec/callback.py
+-rw-r--r--   0        0        0     2936 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/openapi/spec/components.py
+-rw-r--r--   0        0        0      592 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/openapi/spec/contact.py
+-rw-r--r--   0        0        0      950 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/discriminator.py
+-rw-r--r--   0        0        0     3290 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/encoding.py
+-rw-r--r--   0        0        0      974 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/enums.py
+-rw-r--r--   0        0        0     1168 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/example.py
+-rw-r--r--   0        0        0      614 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/external_documentation.py
+-rw-r--r--   0        0        0     5669 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/header.py
+-rw-r--r--   0        0        0     1413 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/info.py
+-rw-r--r--   0        0        0      752 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/license.py
+-rw-r--r--   0        0        0     2876 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/link.py
+-rw-r--r--   0        0        0     1882 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/media_type.py
+-rw-r--r--   0        0        0     1195 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/oauth_flow.py
+-rw-r--r--   0        0        0      897 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/oauth_flows.py
+-rw-r--r--   0        0        0     4218 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/open_api.py
+-rw-r--r--   0        0        0     4842 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/operation.py
+-rw-r--r--   0        0        0     6242 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/parameter.py
+-rw-r--r--   0        0        0     3245 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/path_item.py
+-rw-r--r--   0        0        0     1255 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/paths.py
+-rw-r--r--   0        0        0     1351 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/reference.py
+-rw-r--r--   0        0        0     1095 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/request_body.py
+-rw-r--r--   0        0        0     1854 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/response.py
+-rw-r--r--   0        0        0     2367 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/responses.py
+-rw-r--r--   0        0        0    34574 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/schema.py
+-rw-r--r--   0        0        0     1686 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/security_requirement.py
+-rw-r--r--   0        0        0     2690 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/security_scheme.py
+-rw-r--r--   0        0        0     1077 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/server.py
+-rw-r--r--   0        0        0     1171 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/server_variable.py
+-rw-r--r--   0        0        0      923 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/tag.py
+-rw-r--r--   0        0        0     1702 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/xml.py
+-rw-r--r--   0        0        0    10984 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/pagination.py
+-rw-r--r--   0        0        0    16805 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/params.py
+-rw-r--r--   0        0        0     7102 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/partial.py
+-rw-r--r--   0        0        0     7209 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/plugins.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/py.typed
+-rw-r--r--   0        0        0      278 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/response/__init__.py
+-rw-r--r--   0        0        0    12185 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/response/base.py
+-rw-r--r--   0        0        0     8954 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/response/file.py
+-rw-r--r--   0        0        0     2952 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/response/redirect.py
+-rw-r--r--   0        0        0     4893 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/response/streaming.py
+-rw-r--r--   0        0        0     2994 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/response/template.py
+-rw-r--r--   0        0        0    14975 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/response_containers.py
+-rw-r--r--   0        0        0    15028 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/router.py
+-rw-r--r--   0        0        0      191 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/routes/__init__.py
+-rw-r--r--   0        0        0     1763 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/routes/asgi.py
+-rw-r--r--   0        0        0     6443 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/routes/base.py
+-rw-r--r--   0        0        0    13384 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/routes/http.py
+-rw-r--r--   0        0        0     3058 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/routes/websocket.py
+-rw-r--r--   0        0        0       97 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/security/__init__.py
+-rw-r--r--   0        0        0     7165 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/security/base.py
+-rw-r--r--   0        0        0      188 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/security/session_auth/__init__.py
+-rw-r--r--   0        0        0     5602 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/security/session_auth/auth.py
+-rw-r--r--   0        0        0     4941 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/security/session_auth/middleware.py
+-rw-r--r--   0        0        0     6606 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/serialization.py
+-rw-r--r--   0        0        0      158 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/static_files/__init__.py
+-rw-r--r--   0        0        0     5019 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/static_files/base.py
+-rw-r--r--   0        0        0     3582 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/static_files/config.py
+-rw-r--r--   0        0        0     9536 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/status_codes.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/stores/__init__.py
+-rw-r--r--   0        0        0     4377 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/stores/base.py
+-rw-r--r--   0        0        0     5425 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/stores/file.py
+-rw-r--r--   0        0        0     3625 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/stores/memory.py
+-rw-r--r--   0        0        0     6231 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/stores/redis.py
+-rw-r--r--   0        0        0     2233 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/stores/registry.py
+-rw-r--r--   0        0        0      204 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/template/__init__.py
+-rw-r--r--   0        0        0     4113 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/template/base.py
+-rw-r--r--   0        0        0     1894 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/template/config.py
+-rw-r--r--   0        0        0      581 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/testing/__init__.py
+-rw-r--r--   0        0        0     1816 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/testing/client/__init__.py
+-rw-r--r--   0        0        0    17450 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/testing/client/async_client.py
+-rw-r--r--   0        0        0     5132 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/testing/client/base.py
+-rw-r--r--   0        0        0    19556 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/testing/client/sync_client.py
+-rw-r--r--   0        0        0    31465 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/testing/helpers.py
+-rw-r--r--   0        0        0     2534 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/testing/life_span_handler.py
+-rw-r--r--   0        0        0    21905 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/testing/request_factory.py
+-rw-r--r--   0        0        0     8094 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/testing/transport.py
+-rw-r--r--   0        0        0     6943 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/testing/websocket_test_session.py
+-rw-r--r--   0        0        0     4105 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/types/__init__.py
+-rw-r--r--   0        0        0     8697 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/types/asgi_types.py
+-rw-r--r--   0        0        0      453 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/types/builtin_types.py
+-rw-r--r--   0        0        0     2291 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/types/callable_types.py
+-rw-r--r--   0        0        0     1645 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/types/composite_types.py
+-rw-r--r--   0        0        0      183 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/types/empty.py
+-rw-r--r--   0        0        0     2662 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/types/file_types.py
+-rw-r--r--   0        0        0      344 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/types/helper_types.py
+-rw-r--r--   0        0        0     1487 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/types/internal_types.py
+-rw-r--r--   0        0        0     2607 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/types/protocols.py
+-rw-r--r--   0        0        0     1820 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/types/serialization.py
+-rw-r--r--   0        0        0     1906 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/utils/__init__.py
+-rw-r--r--   0        0        0      729 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/utils/compat.py
+-rw-r--r--   0        0        0     3449 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/utils/dataclass.py
+-rw-r--r--   0        0        0     3520 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/utils/deprecation.py
+-rw-r--r--   0        0        0     1483 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/utils/helpers.py
+-rw-r--r--   0        0        0      723 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/utils/path.py
+-rw-r--r--   0        0        0    10438 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/utils/predicates.py
+-rw-r--r--   0        0        0     2720 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/utils/scope.py
+-rw-r--r--   0        0        0     1003 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/utils/sequence.py
+-rw-r--r--   0        0        0    10889 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/utils/signature.py
+-rw-r--r--   0        0        0     5337 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/utils/sync.py
+-rw-r--r--   0        0        0     6405 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/utils/typing.py
+-rw-r--r--   0        0        0     1921 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/utils/version.py
+-rw-r--r--   0        0        0     9282 2023-04-11 16:09:54.416435 litestar-2.0.0a4/pyproject.toml
+-rw-r--r--   0        0        0    51743 1970-01-01 00:00:00.000000 litestar-2.0.0a4/PKG-INFO
```

### Comparing `litestar-2.0.0a3/LICENSE` & `litestar-2.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/README.md` & `litestar-2.0.0a4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 
 <!-- prettier-ignore-start -->
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-92-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-95-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 <!-- prettier-ignore-end -->
 
 [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestar?label=r%2FLitestar&logo=reddit)](https://reddit.com/r/litestar-api)
 [![Discord](https://img.shields.io/discord/919193495116337154?color=blue&label=chat%20on%20discord&logo=discord)](https://discord.gg/X3FJqy8d2j)
 [![Matrix](https://img.shields.io/badge/%5Bm%5D%20chat%20on%20Matrix-bridged-blue)](https://matrix.to/#/#litestar:matrix.org)
 [![Medium](https://img.shields.io/badge/Medium-12100E?style=flat&logo=medium&logoColor=white)](https://blog.litestar.dev)
@@ -34,15 +34,15 @@
 # Starlite → Litestar
 
 **[Starlite has been renamed to Litestar](https://litestar.dev/about/organization.html#litestar-and-starlite)**
 
 <hr>
 
 Litestar is a powerful, performant, flexible and opinionated ASGI framework,
-offering first class typing support and a full [Pydantic](https://github.com/samuelcolvin/pydantic)
+offering first class typing support and a full [Pydantic](https://github.com/pydantic/pydantic)
 integration.
 
 Check out the [documentation 📚](https://docs.litestar.dev/).
 
 ## Installation
 
 ```shell
@@ -71,15 +71,15 @@
 app = Litestar(route_handlers=[hello_world])
 ```
 
 ## Core Features
 
 - [Class based controllers](#class-based-controllers)
 - [Dependency Injection](#dependency-injection)
-- [Validation and Parsing](#data-parsing-type-hints-and-pydantic) using [Pydantic](https://github.com/samuelcolvin/pydantic)
+- [Validation and Parsing](#data-parsing-type-hints-and-pydantic) using [Pydantic](https://github.com/pydantic/pydantic)
 - [Layered Middleware](#middleware)
 - [Plugin System](#plugin-system-orm-support-and-dtos)
 - [OpenAPI 3.1 schema generation](#openapi)
 - [Life Cycle Hooks](#request-life-cycle-hooks)
 - [Route Guards based Authorization](#route-guards)
 - Layered Parameter declaration
 - SQLAlchemy Support (via plugin)
@@ -399,14 +399,17 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Galdanwing"><img src="https://avatars.githubusercontent.com/u/29492757?v=4?s=100" width="100px;" alt="Antoine van der Horst"/><br /><sub><b>Antoine van der Horst</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=Galdanwing" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://nick.groenen.me"><img src="https://avatars.githubusercontent.com/u/145285?v=4?s=100" width="100px;" alt="Nick Groenen"/><br /><sub><b>Nick Groenen</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=zoni" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/giorgiovilardo"><img src="https://avatars.githubusercontent.com/u/56472600?v=4?s=100" width="100px;" alt="Giorgio Vilardo"/><br /><sub><b>Giorgio Vilardo</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=giorgiovilardo" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/bollwyvl"><img src="https://avatars.githubusercontent.com/u/45380?v=4?s=100" width="100px;" alt="Nicholas Bollweg"/><br /><sub><b>Nicholas Bollweg</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=bollwyvl" title="Code">💻</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/tompin82"><img src="https://avatars.githubusercontent.com/u/47041409?v=4?s=100" width="100px;" alt="Tomas Jonsson"/><br /><sub><b>Tomas Jonsson</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=tompin82" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://www.linkedin.com/in/khiem-doan/"><img src="https://avatars.githubusercontent.com/u/15646249?v=4?s=100" width="100px;" alt="Khiem Doan"/><br /><sub><b>Khiem Doan</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=khiemdoan" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/kedod"><img src="https://avatars.githubusercontent.com/u/35638715?v=4?s=100" width="100px;" alt="kedod"/><br /><sub><b>kedod</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=kedod" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/sonpro1296"><img src="https://avatars.githubusercontent.com/u/17319142?v=4?s=100" width="100px;" alt="sonpro1296"/><br /><sub><b>sonpro1296</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=sonpro1296" title="Code">💻</a> <a href="https://github.com/litestar-org/litestar/commits?author=sonpro1296" title="Tests">⚠️</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `litestar-2.0.0a3/litestar/__init__.py` & `litestar-2.0.0a4/litestar/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/_asgi/asgi_router.py` & `litestar-2.0.0a4/litestar/_asgi/asgi_router.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/_asgi/routing_trie/mapping.py` & `litestar-2.0.0a4/litestar/_asgi/routing_trie/mapping.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/_asgi/routing_trie/traversal.py` & `litestar-2.0.0a4/litestar/_asgi/routing_trie/traversal.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/_asgi/routing_trie/types.py` & `litestar-2.0.0a4/litestar/_asgi/routing_trie/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/_asgi/routing_trie/validate.py` & `litestar-2.0.0a4/litestar/_asgi/routing_trie/validate.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/_asgi/utils.py` & `litestar-2.0.0a4/litestar/_asgi/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/_kwargs/cleanup.py` & `litestar-2.0.0a4/litestar/_kwargs/cleanup.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/_kwargs/dependencies.py` & `litestar-2.0.0a4/litestar/_kwargs/dependencies.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/_kwargs/extractors.py` & `litestar-2.0.0a4/litestar/_kwargs/extractors.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from litestar.types import Empty
 
 if TYPE_CHECKING:
     from litestar._kwargs import KwargsModel
     from litestar._kwargs.parameter_definition import ParameterDefinition
     from litestar._signature.field import SignatureField
     from litestar.connection import ASGIConnection, Request
-    from litestar.types.parsed_signature import ParsedParameter
+    from litestar.utils.signature import ParsedParameter
 
 __all__ = (
     "body_extractor",
     "cookies_extractor",
     "create_connection_value_extractor",
     "create_data_extractor",
     "create_multipart_extractor",
```

### Comparing `litestar-2.0.0a3/litestar/_kwargs/kwargs_model.py` & `litestar-2.0.0a4/litestar/_kwargs/kwargs_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 __all__ = ("KwargsModel",)
 
 
 if TYPE_CHECKING:
     from litestar.connection import ASGIConnection
     from litestar.di import Provide
-    from litestar.types.parsed_signature import ParsedParameter, ParsedSignature
+    from litestar.utils.signature import ParsedParameter, ParsedSignature
 
 
 class KwargsModel:
     """Model required kwargs for a given RouteHandler and its dependencies.
 
     This is done once and is memoized during application bootstrap, ensuring minimal runtime overhead.
     """
```

### Comparing `litestar-2.0.0a3/litestar/_kwargs/parameter_definition.py` & `litestar-2.0.0a4/litestar/_kwargs/parameter_definition.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/_layers/utils.py` & `litestar-2.0.0a4/litestar/_layers/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/_multipart.py` & `litestar-2.0.0a4/litestar/_multipart.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/_openapi/parameters.py` & `litestar-2.0.0a4/litestar/_openapi/parameters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/_openapi/path_item.py` & `litestar-2.0.0a4/litestar/_openapi/path_item.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/_openapi/request_body.py` & `litestar-2.0.0a4/litestar/_openapi/request_body.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/_openapi/responses.py` & `litestar-2.0.0a4/litestar/_openapi/responses.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/_openapi/schema_generation/constrained_fields.py` & `litestar-2.0.0a4/litestar/_openapi/schema_generation/constrained_fields.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from datetime import datetime
 from re import Pattern
 from typing import TYPE_CHECKING, Any
 
+from litestar._openapi.schema_generation.utils import sort_schemas_and_references
 from litestar.exceptions import MissingDependencyException
 from litestar.openapi.spec.enums import OpenAPIFormat, OpenAPIType
 from litestar.openapi.spec.schema import Schema
 
 if TYPE_CHECKING:
     from litestar.plugins import OpenAPISchemaPluginProtocol
 
@@ -123,15 +124,15 @@
         schema.unique_items = True
     if children:
         items = [
             create_schema(field=sub_field, generate_examples=False, plugins=plugins, schemas=schemas)
             for sub_field in children
         ]
         if len(items) > 1:
-            schema.items = Schema(one_of=items)
+            schema.items = Schema(one_of=sort_schemas_and_references(items))
         else:
             schema.items = items[0]
     else:
         from litestar._signature.field import SignatureField
 
         schema.items = create_schema(
             field=SignatureField.create(field_type=field_type.item_type, name=f"{field_type.__name__}Field"),
```

### Comparing `litestar-2.0.0a3/litestar/_openapi/schema_generation/examples.py` & `litestar-2.0.0a4/litestar/_openapi/schema_generation/examples.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/_openapi/schema_generation/schema.py` & `litestar-2.0.0a4/litestar/_openapi/schema_generation/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from _decimal import Decimal
 from typing_extensions import get_args, get_type_hints
 
 from litestar._openapi.schema_generation.constrained_fields import (
     create_constrained_field_schema,
 )
 from litestar._openapi.schema_generation.examples import create_examples_for_field
+from litestar._openapi.schema_generation.utils import sort_schemas_and_references
 from litestar._signature.field import SignatureField
 from litestar.constants import UNDEFINED_SENTINELS
 from litestar.datastructures import UploadFile
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.openapi.spec import Reference
 from litestar.openapi.spec.enums import OpenAPIFormat, OpenAPIType
 from litestar.openapi.spec.schema import Schema, SchemaDataContainer
@@ -382,18 +383,20 @@
         plugins: A list of plugins.
         schemas: A mapping of namespaces to schemas - this mapping is used in the OA components section.
 
     Returns:
         A schema instance.
     """
     return Schema(
-        one_of=[
-            create_schema(field=sub_field, generate_examples=generate_examples, plugins=plugins, schemas=schemas)
-            for sub_field in field.children or []
-        ]
+        one_of=sort_schemas_and_references(
+            [
+                create_schema(field=sub_field, generate_examples=generate_examples, plugins=plugins, schemas=schemas)
+                for sub_field in field.children or []
+            ]
+        )
     )
 
 
 def create_schema_for_object_type(
     field: "SignatureField",
     generate_examples: bool,
     plugins: list["OpenAPISchemaPluginProtocol"],
@@ -415,15 +418,18 @@
 
     if field.is_non_string_sequence or field.is_non_string_iterable:
         items = [
             create_schema(field=sub_field, generate_examples=generate_examples, plugins=plugins, schemas=schemas)
             for sub_field in (field.children or ())
         ]
 
-        return Schema(type=OpenAPIType.ARRAY, items=Schema(one_of=items) if len(items) > 1 else items[0])
+        return Schema(
+            type=OpenAPIType.ARRAY,
+            items=Schema(one_of=sort_schemas_and_references(items)) if len(items) > 1 else items[0],
+        )
 
     if field.is_literal:
         return create_literal_schema(field.field_type)
 
     raise ImproperlyConfiguredException(
         f"Parameter '{field.name}' with type '{field.field_type}' could not be mapped to an Open API type. "
         f"This can occur if a user-defined generic type is resolved as a parameter. If '{field.name}' should "
```

### Comparing `litestar-2.0.0a3/litestar/_openapi/typescript_converter/converter.py` & `litestar-2.0.0a4/litestar/_openapi/typescript_converter/converter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/_openapi/typescript_converter/schema_parsing.py` & `litestar-2.0.0a4/litestar/_openapi/typescript_converter/schema_parsing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/_openapi/typescript_converter/types.py` & `litestar-2.0.0a4/litestar/_openapi/typescript_converter/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/_openapi/utils.py` & `litestar-2.0.0a4/litestar/_openapi/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/_parsers.py` & `litestar-2.0.0a4/litestar/_parsers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/_signature/field.py` & `litestar-2.0.0a4/litestar/_signature/field.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,24 @@
 from typing import Any, Literal
 
 from typing_extensions import get_args, get_origin
 
 from litestar.constants import UNDEFINED_SENTINELS
 from litestar.params import BodyKwarg, DependencyKwarg, ParameterKwarg
 from litestar.types import Empty
-from litestar.utils import is_any, is_optional_union, is_union, make_non_optional_union
-from litestar.utils.predicates import is_generic, is_mapping, is_non_string_iterable, is_non_string_sequence
+from litestar.utils.predicates import (
+    is_any,
+    is_generic,
+    is_mapping,
+    is_non_string_iterable,
+    is_non_string_sequence,
+    is_optional_union,
+    is_union,
+)
+from litestar.utils.typing import make_non_optional_union
 
 __all__ = ("SignatureField",)
 
 
 @dataclass(unsafe_hash=True, frozen=True)
 class SignatureField:
     """Abstraction representing a model field. This class is meant to replace equivalent datastructures from other
```

### Comparing `litestar-2.0.0a3/litestar/_signature/models/attrs_signature_model.py` & `litestar-2.0.0a4/litestar/_signature/models/attrs_signature_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import re
 import traceback
 from dataclasses import asdict
-from datetime import date, datetime, time, timedelta
+from datetime import date, datetime, time, timedelta, timezone
 from functools import lru_cache, partial
 from pathlib import PurePath
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     cast,
@@ -35,15 +35,15 @@
     import attrs
     import cattrs
 except ImportError as e:
     raise MissingDependencyException("attrs is not installed") from e
 
 if TYPE_CHECKING:
     from litestar.plugins import PluginMapping
-    from litestar.types.parsed_signature import ParsedSignature
+    from litestar.utils.signature import ParsedSignature
 
 key_re = re.compile("@ attribute (.*)|'(.*)'")
 
 __all__ = ("AttrsSignatureModel",)
 
 try:
     import pydantic
@@ -69,15 +69,15 @@
 
 
 def _structure_datetime(value: Any, cls: type[datetime]) -> datetime:
     if isinstance(value, datetime):
         return value
 
     try:
-        return cls.fromtimestamp(float(value))
+        return cls.fromtimestamp(float(value), tz=timezone.utc)
     except (ValueError, TypeError):
         pass
 
     return parse(value)
 
 
 def _structure_date(value: Any, cls: type[date]) -> date:
@@ -299,33 +299,35 @@
         type_overrides: dict[str, Any],
     ) -> type[SignatureModel]:
         attributes: dict[str, Any] = {}
 
         for parameter in parsed_signature.parameters.values():
             annotation = type_overrides.get(parameter.name, parameter.parsed_type.annotation)
 
-            if isinstance(parameter.default, (ParameterKwarg, BodyKwarg)):
-                attribute = attr.attrib(
-                    type=annotation,
-                    metadata={
-                        **asdict(parameter.default),
-                        "kwargs_model": parameter.default,
-                        "parsed_parameter": parameter,
-                    },
-                    default=parameter.default.default if parameter.default.default is not Empty else attr.NOTHING,
-                    validator=_create_validators(annotation=annotation, kwargs_model=parameter.default),
-                )
-            elif isinstance(parameter.default, DependencyKwarg):
-                attribute = attr.attrib(
-                    type=annotation,
-                    default=parameter.default.default if parameter.default.default is not Empty else None,
-                    metadata={
-                        "kwargs_model": parameter.default,
-                    },
-                )
+            if kwargs_container := parameter.kwarg_container:
+                if isinstance(kwargs_container, DependencyKwarg):
+                    attribute = attr.attrib(
+                        type=annotation if not kwargs_container.skip_validation else Any,
+                        default=kwargs_container.default if kwargs_container.default is not Empty else None,
+                        metadata={
+                            "kwargs_model": kwargs_container,
+                            "parsed_parameter": parameter,
+                        },
+                    )
+                else:
+                    attribute = attr.attrib(
+                        type=annotation,
+                        metadata={
+                            **asdict(kwargs_container),
+                            "kwargs_model": kwargs_container,
+                            "parsed_parameter": parameter,
+                        },
+                        default=kwargs_container.default if kwargs_container.default is not Empty else attr.NOTHING,
+                        validator=_create_validators(annotation=annotation, kwargs_model=kwargs_container),
+                    )
             elif parameter.has_default:
                 attribute = attr.attrib(type=annotation, default=parameter.default)
             else:
                 attribute = attr.attrib(
                     type=annotation, default=None if parameter.parsed_type.is_optional else attr.NOTHING
                 )
```

### Comparing `litestar-2.0.0a3/litestar/_signature/models/base.py` & `litestar-2.0.0a4/litestar/_signature/models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from litestar.enums import ScopeType
 from litestar.exceptions import InternalServerException, ValidationException
 
 if TYPE_CHECKING:
     from litestar._signature.field import SignatureField
     from litestar.connection import ASGIConnection
     from litestar.plugins import PluginMapping
-    from litestar.types.parsed_signature import ParsedSignature
+    from litestar.utils.signature import ParsedSignature
 
 __all__ = ("SignatureModel",)
 
 
 class ErrorMessage(TypedDict):
     key: str
     message: str
```

### Comparing `litestar-2.0.0a3/litestar/_signature/models/pydantic_signature_model.py` & `litestar-2.0.0a4/litestar/_signature/models/pydantic_signature_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from __future__ import annotations
 
 from dataclasses import asdict
 from typing import TYPE_CHECKING, Any
 
 from pydantic import BaseConfig, BaseModel, ValidationError, create_model
-from pydantic.fields import FieldInfo, ModelField, Undefined
+from pydantic.fields import FieldInfo, ModelField
 
 from litestar._signature.field import SignatureField
 from litestar._signature.models.base import SignatureModel
 from litestar.constants import UNDEFINED_SENTINELS
 from litestar.params import BodyKwarg, DependencyKwarg, ParameterKwarg
 from litestar.types import Empty
 from litestar.utils.predicates import is_pydantic_constrained_field
 
 if TYPE_CHECKING:
     from litestar.connection import ASGIConnection
     from litestar.plugins import PluginMapping
-    from litestar.types.parsed_signature import ParsedSignature
+    from litestar.utils.signature import ParsedSignature
 
 __all__ = ("PydanticSignatureModel",)
 
 
 class PydanticSignatureModel(SignatureModel, BaseModel):
     """Model that represents a function signature that uses a pydantic specific type or types."""
 
@@ -147,31 +147,38 @@
             The created PydanticSignatureModel.
         """
         field_definitions: dict[str, tuple[Any, Any]] = {}
 
         for parameter in parsed_signature.parameters.values():
             field_type = type_overrides.get(parameter.name, parameter.parsed_type.annotation)
 
-            if isinstance(parameter.default, (ParameterKwarg, BodyKwarg)):
-                field_info = FieldInfo(
-                    **asdict(parameter.default), kwargs_model=parameter.default, parsed_parameter=parameter
-                )
+            if kwargs_container := parameter.kwarg_container:
+                if isinstance(kwargs_container, DependencyKwarg):
+                    field_info = FieldInfo(
+                        default=kwargs_container.default if kwargs_container.default is not Empty else None,
+                        kwargs_model=kwargs_container,
+                        parsed_parameter=parameter,
+                    )
+                    if kwargs_container.skip_validation:
+                        field_type = Any
+                else:
+                    field_info = FieldInfo(
+                        **{k: v for k, v in asdict(kwargs_container).items() if v is not Empty},
+                        kwargs_model=kwargs_container,
+                        parsed_parameter=parameter,
+                    )
             else:
                 field_info = FieldInfo(default=..., parsed_parameter=parameter)
 
-            if isinstance(parameter.default, DependencyKwarg):
-                field_info.default = parameter.default.default if parameter.default.default is not Empty else None
-            elif isinstance(parameter.default, (ParameterKwarg, BodyKwarg)):
-                field_info.default = parameter.default.default if parameter.default.default is not Empty else Undefined
-            elif is_pydantic_constrained_field(parameter.default):
-                field_type = parameter.default
-            elif parameter.has_default:
-                field_info.default = parameter.default
-            elif parameter.parsed_type.is_optional:
-                field_info.default = None
+                if is_pydantic_constrained_field(parameter.default):
+                    field_type = parameter.default
+                elif parameter.has_default:
+                    field_info.default = parameter.default
+                elif parameter.parsed_type.is_optional:
+                    field_info.default = None
 
             field_definitions[parameter.name] = (field_type, field_info)
 
         model: type[PydanticSignatureModel] = create_model(  # type: ignore
             f"{fn_name}_signature_model",
             __base__=PydanticSignatureModel,
             __module__=fn_module or "pydantic.main",
```

### Comparing `litestar-2.0.0a3/litestar/_signature/utils.py` & `litestar-2.0.0a4/litestar/_signature/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     AttrsSignatureModel = Empty  # type: ignore
 
 if TYPE_CHECKING:
     from typing_extensions import TypeAlias
 
     from litestar._signature.models.base import SignatureModel
     from litestar.plugins import SerializationPluginProtocol
-    from litestar.types.parsed_signature import ParsedParameter, ParsedSignature
+    from litestar.utils.signature import ParsedParameter, ParsedSignature
 
 __all__ = (
     "create_signature_model",
     "get_signature_model",
 )
```

### Comparing `litestar-2.0.0a3/litestar/app.py` & `litestar-2.0.0a4/litestar/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import logging
 from datetime import date, datetime, time, timedelta
 from functools import partial
 from itertools import chain
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Literal, Mapping, Sequence, cast
 
 from typing_extensions import Self, TypedDict
@@ -35,24 +36,24 @@
 )
 from litestar.router import Router
 from litestar.routes import ASGIRoute, HTTPRoute, WebSocketRoute
 from litestar.static_files.base import StaticFiles
 from litestar.stores.registry import StoreRegistry
 from litestar.types import Empty
 from litestar.types.internal_types import PathParameterDefinition
-from litestar.types.parsed_signature import ParsedSignature
 from litestar.utils import (
     as_async_callable_list,
     async_partial,
     is_async_callable,
     join_paths,
     unique,
 )
 from litestar.utils.dataclass import extract_dataclass_items
 from litestar.utils.helpers import unwrap_partial
+from litestar.utils.signature import ParsedSignature
 
 if TYPE_CHECKING:
     from litestar.config.compression import CompressionConfig
     from litestar.config.cors import CORSConfig
     from litestar.config.csrf import CSRFConfig
     from litestar.datastructures import CacheControlHeader, ETag, ResponseHeader
     from litestar.dto.interface import DTOInterface
@@ -128,28 +129,28 @@
     """The Litestar application.
 
     ``Litestar`` is the root level of the app - it has the base path of ``/`` and all root level Controllers, Routers
     and Route Handlers should be registered on it.
     """
 
     __slots__ = (
+        "_debug",
         "_openapi_schema",
         "after_exception",
         "after_shutdown",
         "after_startup",
         "allowed_hosts",
         "asgi_handler",
         "asgi_router",
         "before_send",
         "before_shutdown",
         "before_startup",
         "compression_config",
         "cors_config",
         "csrf_config",
-        "debug",
         "event_emitter",
         "get_logger",
         "logger",
         "logging_config",
         "multipart_form_part_limit",
         "signature_namespace",
         "on_shutdown",
@@ -369,14 +370,15 @@
         for handler in chain(
             on_app_init or [],
             (p.on_app_init for p in config.plugins if isinstance(p, InitPluginProtocol)),
         ):
             config = handler(config)
 
         self._openapi_schema: OpenAPI | None = None
+        self._debug: bool = True
         self.get_logger: GetLogger = get_logger_placeholder
         self.logger: Logger | None = None
         self.routes: list[HTTPRoute | ASGIRoute | WebSocketRoute] = []
         self.asgi_router = ASGIRouter(app=self)
 
         self.allowed_hosts = cast("AllowedHostsConfig | None", config.allowed_hosts)
         self.after_exception = as_async_callable_list(config.after_exception)
@@ -385,15 +387,14 @@
         self.allowed_hosts = cast("AllowedHostsConfig | None", config.allowed_hosts)
         self.before_send = as_async_callable_list(config.before_send)
         self.before_shutdown = as_async_callable_list(config.before_shutdown)
         self.before_startup = as_async_callable_list(config.before_startup)
         self.compression_config = config.compression_config
         self.cors_config = config.cors_config
         self.csrf_config = config.csrf_config
-        self.debug = config.debug
         self.event_emitter = config.event_emitter_backend(listeners=config.listeners)
         self.logging_config = config.logging_config
         self.multipart_form_part_limit = config.multipart_form_part_limit
         self.on_shutdown = config.on_shutdown
         self.on_startup = config.on_startup
         self.openapi_config = config.openapi_config
         self.openapi_schema_plugins = [p for p in config.plugins if isinstance(p, OpenAPISchemaPluginProtocol)]
@@ -401,14 +402,15 @@
         self.request_class = config.request_class or Request
         self.response_cache_config = config.response_cache_config
         self.serialization_plugins = [p for p in config.plugins if isinstance(p, SerializationPluginProtocol)]
         self.state = config.state
         self.static_files_config = config.static_files_config
         self.template_engine = config.template_config.engine_instance if config.template_config else None
         self.websocket_class = config.websocket_class or WebSocket
+        self.debug = config.debug
 
         super().__init__(
             after_request=config.after_request,
             after_response=config.after_response,
             before_request=config.before_request,
             cache_control=config.cache_control,
             dependencies=config.dependencies,
@@ -431,30 +433,41 @@
             tags=config.tags,
             type_encoders=config.type_encoders,
         )
 
         for route_handler in config.route_handlers:
             self.register(route_handler)
 
-        if self.debug and isinstance(self.logging_config, LoggingConfig):
-            self.logging_config.loggers["litestar"]["level"] = "DEBUG"
-
         if self.logging_config:
             self.get_logger = self.logging_config.configure()
             self.logger = self.get_logger("litestar")
 
         if self.openapi_config:
             self.register(self.openapi_config.openapi_controller)
 
         for static_config in self.static_files_config:
             self.register(static_config.to_static_files_app())
 
         self.asgi_handler = self._create_asgi_handler()
 
-        self.stores = config.stores if isinstance(config.stores, StoreRegistry) else StoreRegistry(config.stores)
+        self.stores: StoreRegistry = (
+            config.stores if isinstance(config.stores, StoreRegistry) else StoreRegistry(config.stores)
+        )
+
+    @property
+    def debug(self) -> bool:
+        return self._debug
+
+    @debug.setter
+    def debug(self, value: bool) -> None:
+        if self.logger:
+            self.logger.setLevel(logging.DEBUG if value else logging.INFO)
+        if isinstance(self.logging_config, LoggingConfig):
+            self.logging_config.loggers["litestar"]["level"] = "DEBUG" if value else "INFO"
+        self._debug = value
 
     async def __call__(
         self,
         scope: Scope | LifeSpanScope,
         receive: Receive | LifeSpanReceive,
         send: Send | LifeSpanSend,
     ) -> None:
```

### Comparing `litestar-2.0.0a3/litestar/background_tasks.py` & `litestar-2.0.0a4/litestar/background_tasks.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/cli/_utils.py` & `litestar-2.0.0a4/litestar/cli/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/cli/commands/core.py` & `litestar-2.0.0a4/litestar/cli/commands/core.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/cli/commands/schema.py` & `litestar-2.0.0a4/litestar/cli/commands/schema.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/cli/commands/sessions.py` & `litestar-2.0.0a4/litestar/cli/commands/sessions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/cli/main.py` & `litestar-2.0.0a4/litestar/cli/main.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/config/allowed_hosts.py` & `litestar-2.0.0a4/litestar/config/allowed_hosts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/config/app.py` & `litestar-2.0.0a4/litestar/config/app.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/config/compression.py` & `litestar-2.0.0a4/litestar/config/compression.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/config/cors.py` & `litestar-2.0.0a4/litestar/config/cors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/config/csrf.py` & `litestar-2.0.0a4/litestar/config/csrf.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/config/response_cache.py` & `litestar-2.0.0a4/litestar/config/response_cache.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/connection/__init__.py` & `litestar-2.0.0a4/litestar/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/connection/base.py` & `litestar-2.0.0a4/litestar/connection/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/connection/request.py` & `litestar-2.0.0a4/litestar/connection/request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/connection/websocket.py` & `litestar-2.0.0a4/litestar/connection/websocket.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/constants.py` & `litestar-2.0.0a4/litestar/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from inspect import Signature
 
 from pydantic.fields import Undefined
 
+from litestar.enums import MediaType
 from litestar.types import Empty
 
 DEFAULT_ALLOWED_CORS_HEADERS = {"Accept", "Accept-Language", "Content-Language", "Content-Type"}
 DEFAULT_CHUNK_SIZE = 1024 * 128  # 128KB
 HTTP_DISCONNECT = "http.disconnect"
 HTTP_RESPONSE_BODY = "http.response.body"
 HTTP_RESPONSE_START = "http.response.start"
 ONE_MEGABYTE = 1024 * 1024
 OPENAPI_NOT_INITIALIZED = "Litestar has not been instantiated with OpenAPIConfig"
 REDIRECT_STATUS_CODES = {301, 302, 303, 307, 308}
+REDIRECT_ALLOWED_MEDIA_TYPES = {MediaType.TEXT, MediaType.HTML}
 RESERVED_KWARGS = {"state", "headers", "cookies", "request", "socket", "data", "query", "scope", "body"}
 SCOPE_STATE_DEPENDENCY_CACHE = "dependency_cache"
 SCOPE_STATE_NAMESPACE = "__litestar__"
 SCOPE_STATE_RESPONSE_COMPRESSED = "response_compressed"
 SKIP_VALIDATION_NAMES = {"request", "socket", "scope", "receive", "send"}
 UNDEFINED_SENTINELS = {Undefined, Signature.empty, Empty, Ellipsis}
 WEBSOCKET_CLOSE = "websocket.close"
```

### Comparing `litestar-2.0.0a3/litestar/contrib/htmx/_utils.py` & `litestar-2.0.0a4/litestar/contrib/htmx/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/contrib/htmx/request.py` & `litestar-2.0.0a4/litestar/contrib/htmx/request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/contrib/htmx/response.py` & `litestar-2.0.0a4/litestar/contrib/htmx/response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/contrib/htmx/types.py` & `litestar-2.0.0a4/litestar/contrib/htmx/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/contrib/jinja.py` & `litestar-2.0.0a4/litestar/contrib/jinja.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/contrib/jwt/__init__.py` & `litestar-2.0.0a4/litestar/contrib/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/contrib/jwt/jwt_auth.py` & `litestar-2.0.0a4/litestar/contrib/jwt/jwt_auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/contrib/jwt/jwt_token.py` & `litestar-2.0.0a4/litestar/contrib/jwt/jwt_token.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/contrib/jwt/middleware.py` & `litestar-2.0.0a4/litestar/contrib/jwt/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/contrib/mako.py` & `litestar-2.0.0a4/litestar/contrib/mako.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/contrib/opentelemetry/_utils.py` & `litestar-2.0.0a4/litestar/contrib/opentelemetry/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/contrib/opentelemetry/config.py` & `litestar-2.0.0a4/litestar/contrib/opentelemetry/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/contrib/opentelemetry/middleware.py` & `litestar-2.0.0a4/litestar/contrib/opentelemetry/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/contrib/piccolo_orm.py` & `litestar-2.0.0a4/litestar/contrib/piccolo_orm.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/contrib/repository/abc.py` & `litestar-2.0.0a4/litestar/contrib/repository/abc.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/contrib/repository/filters.py` & `litestar-2.0.0a4/litestar/contrib/repository/filters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/contrib/repository/testing/generic_mock_repository.py` & `litestar-2.0.0a4/litestar/contrib/repository/testing/generic_mock_repository.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/contrib/sqlalchemy/base.py` & `litestar-2.0.0a4/litestar/contrib/sqlalchemy/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/contrib/sqlalchemy/init_plugin/config/asyncio.py` & `litestar-2.0.0a4/litestar/contrib/sqlalchemy/init_plugin/config/asyncio.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/contrib/sqlalchemy/init_plugin/config/common.py` & `litestar-2.0.0a4/litestar/contrib/sqlalchemy/init_plugin/config/common.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/contrib/sqlalchemy/init_plugin/config/engine.py` & `litestar-2.0.0a4/litestar/contrib/sqlalchemy/init_plugin/config/engine.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/contrib/sqlalchemy/init_plugin/config/sync.py` & `litestar-2.0.0a4/litestar/contrib/sqlalchemy/init_plugin/config/sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/contrib/sqlalchemy/init_plugin/plugin.py` & `litestar-2.0.0a4/litestar/contrib/sqlalchemy/init_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/contrib/sqlalchemy/repository.py` & `litestar-2.0.0a4/litestar/contrib/sqlalchemy/repository.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/contrib/sqlalchemy_1/config.py` & `litestar-2.0.0a4/litestar/contrib/sqlalchemy_1/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/contrib/sqlalchemy_1/plugin.py` & `litestar-2.0.0a4/litestar/contrib/sqlalchemy_1/plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/contrib/sqlalchemy_1/types.py` & `litestar-2.0.0a4/litestar/contrib/sqlalchemy_1/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/contrib/tortoise_orm.py` & `litestar-2.0.0a4/litestar/contrib/tortoise_orm.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/controller.py` & `litestar-2.0.0a4/litestar/controller.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/data_extractors.py` & `litestar-2.0.0a4/litestar/data_extractors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/datastructures/__init__.py` & `litestar-2.0.0a4/litestar/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/datastructures/cookie.py` & `litestar-2.0.0a4/litestar/datastructures/cookie.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/datastructures/headers.py` & `litestar-2.0.0a4/litestar/datastructures/headers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/datastructures/multi_dicts.py` & `litestar-2.0.0a4/litestar/datastructures/multi_dicts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/datastructures/response_header.py` & `litestar-2.0.0a4/litestar/datastructures/response_header.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/datastructures/state.py` & `litestar-2.0.0a4/litestar/datastructures/state.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/datastructures/upload_file.py` & `litestar-2.0.0a4/litestar/datastructures/upload_file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/datastructures/url.py` & `litestar-2.0.0a4/litestar/datastructures/url.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/di.py` & `litestar-2.0.0a4/litestar/di.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/dto/interface.py` & `litestar-2.0.0a4/litestar/dto/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
     from litestar.connection import Request
     from litestar.handlers import BaseRouteHandler
     from litestar.types import LitestarEncodableType
-    from litestar.types.parsed_signature import ParsedType
+    from litestar.utils.signature import ParsedType
 
 __all__ = ("DTOInterface",)
 
 
 @runtime_checkable
 class DTOInterface(Protocol):
     __slots__ = ()
@@ -63,14 +63,14 @@
     def on_registration(cls, parsed_type: ParsedType, route_handler: BaseRouteHandler) -> None:
         """Receive the ``parsed_type`` and ``route_handler`` that this DTO is configured to represent.
 
         At this point, if the DTO type does not support the annotated type of ``parsed_type``, it should raise an
         ``UnsupportedType`` exception.
 
         Args:
-            parsed_type: :class:`ParsedType <.types.parsed_signature.ParsedType>` instance, will be either the parsed
+            parsed_type: ParsedType instance, will be either the parsed
                 annotation of a ``"data"`` kwarg, or the parsed return type annotation of a route handler.
             route_handler: :class:`HTTPRouteHandler <.handlers.HTTPRouteHandler>` DTO type is declared upon.
 
         Raises:
             UnsupportedType: If the DTO type does not support the annotated type of ``parsed_type``.
         """
```

### Comparing `litestar-2.0.0a3/litestar/enums.py` & `litestar-2.0.0a4/litestar/enums.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/events/emitter.py` & `litestar-2.0.0a4/litestar/events/emitter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/events/listener.py` & `litestar-2.0.0a4/litestar/events/listener.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/exceptions/__init__.py` & `litestar-2.0.0a4/litestar/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/exceptions/base_exceptions.py` & `litestar-2.0.0a4/litestar/exceptions/base_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/exceptions/http_exceptions.py` & `litestar-2.0.0a4/litestar/exceptions/http_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/exceptions/websocket_exceptions.py` & `litestar-2.0.0a4/litestar/exceptions/websocket_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/file_system.py` & `litestar-2.0.0a4/litestar/file_system.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/handlers/__init__.py` & `litestar-2.0.0a4/litestar/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/handlers/asgi_handlers.py` & `litestar-2.0.0a4/litestar/handlers/asgi_handlers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/handlers/base.py` & `litestar-2.0.0a4/litestar/handlers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from copy import copy
 from typing import TYPE_CHECKING, Any, Generic, Mapping, Sequence, TypeVar, cast
 
 from litestar._signature.field import SignatureField
 from litestar.dto.interface import DTOInterface
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.types import Dependencies, Empty, ExceptionHandlersMap, Guard, Middleware, TypeEncodersMap
-from litestar.types.parsed_signature import ParsedSignature
 from litestar.utils import AsyncCallable, Ref, get_name, normalize_path
 from litestar.utils.helpers import unwrap_partial
+from litestar.utils.signature import ParsedSignature
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
     from litestar._signature.models import SignatureModel
     from litestar.connection import ASGIConnection
     from litestar.controller import Controller
@@ -148,15 +148,15 @@
     @property
     def parsed_fn_signature(self) -> ParsedSignature:
         """Return the parsed signature of the handler function.
 
         This method is memoized so the computation occurs only once.
 
         Returns:
-            A :class:`ParsedSignature <.types.parsed_signature.ParsedSignature>` instance
+            A ParsedSignature instance
         """
         if self._parsed_fn_signature is Empty:
             self._parsed_fn_signature = ParsedSignature.from_fn(
                 unwrap_partial(self.fn.value), self.resolve_signature_namespace()
             )
 
         return cast("ParsedSignature", self._parsed_fn_signature)
```

### Comparing `litestar-2.0.0a3/litestar/handlers/http_handlers/_utils.py` & `litestar-2.0.0a4/litestar/handlers/http_handlers/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/handlers/http_handlers/base.py` & `litestar-2.0.0a4/litestar/handlers/http_handlers/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/handlers/http_handlers/decorators.py` & `litestar-2.0.0a4/litestar/handlers/http_handlers/decorators.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/handlers/websocket_handlers.py` & `litestar-2.0.0a4/litestar/handlers/websocket_handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from msgspec.json import Encoder as JsonEncoder
 
 from litestar.exceptions import ImproperlyConfiguredException, WebSocketDisconnect
 from litestar.handlers.base import BaseRouteHandler
 from litestar.serialization import decode_json, default_serializer
 from litestar.types.builtin_types import NoneType
 from litestar.types.empty import Empty
-from litestar.types.parsed_signature import ParsedSignature
 from litestar.utils import AsyncCallable, is_async_callable
+from litestar.utils.signature import ParsedSignature
 
 __all__ = ("WebsocketRouteHandler", "websocket", "websocket_listener", "WebsocketListener")
 
 if TYPE_CHECKING:
     from typing import Any, Mapping
 
     from litestar.connection import WebSocket
```

### Comparing `litestar-2.0.0a3/litestar/logging/_utils.py` & `litestar-2.0.0a4/litestar/logging/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/logging/config.py` & `litestar-2.0.0a4/litestar/logging/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/logging/picologging.py` & `litestar-2.0.0a4/litestar/logging/picologging.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/logging/standard.py` & `litestar-2.0.0a4/litestar/logging/standard.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/middleware/_utils.py` & `litestar-2.0.0a4/litestar/middleware/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/middleware/allowed_hosts.py` & `litestar-2.0.0a4/litestar/middleware/allowed_hosts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/middleware/authentication.py` & `litestar-2.0.0a4/litestar/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/middleware/base.py` & `litestar-2.0.0a4/litestar/middleware/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/middleware/compression.py` & `litestar-2.0.0a4/litestar/middleware/compression.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/middleware/cors.py` & `litestar-2.0.0a4/litestar/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/middleware/csrf.py` & `litestar-2.0.0a4/litestar/middleware/csrf.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/middleware/exceptions/_debug_response.py` & `litestar-2.0.0a4/litestar/middleware/exceptions/_debug_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/middleware/exceptions/middleware.py` & `litestar-2.0.0a4/litestar/middleware/exceptions/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/middleware/exceptions/templates/scripts.js` & `litestar-2.0.0a4/litestar/middleware/exceptions/templates/scripts.js`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/middleware/exceptions/templates/styles.css` & `litestar-2.0.0a4/litestar/middleware/exceptions/templates/styles.css`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/middleware/logging.py` & `litestar-2.0.0a4/litestar/middleware/logging.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/middleware/rate_limit.py` & `litestar-2.0.0a4/litestar/middleware/rate_limit.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/middleware/session/base.py` & `litestar-2.0.0a4/litestar/middleware/session/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/middleware/session/client_side.py` & `litestar-2.0.0a4/litestar/middleware/session/client_side.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/middleware/session/server_side.py` & `litestar-2.0.0a4/litestar/middleware/session/server_side.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/config.py` & `litestar-2.0.0a4/litestar/openapi/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/controller.py` & `litestar-2.0.0a4/litestar/openapi/controller.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/datastructures.py` & `litestar-2.0.0a4/litestar/openapi/datastructures.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/spec/__init__.py` & `litestar-2.0.0a4/litestar/openapi/spec/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/spec/base.py` & `litestar-2.0.0a4/litestar/openapi/spec/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/spec/callback.py` & `litestar-2.0.0a4/litestar/openapi/spec/callback.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/spec/components.py` & `litestar-2.0.0a4/litestar/openapi/spec/components.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/spec/contact.py` & `litestar-2.0.0a4/litestar/openapi/spec/contact.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/spec/discriminator.py` & `litestar-2.0.0a4/litestar/openapi/spec/discriminator.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/spec/encoding.py` & `litestar-2.0.0a4/litestar/openapi/spec/encoding.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/spec/enums.py` & `litestar-2.0.0a4/litestar/openapi/spec/enums.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/spec/example.py` & `litestar-2.0.0a4/litestar/openapi/spec/example.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/spec/external_documentation.py` & `litestar-2.0.0a4/litestar/openapi/spec/external_documentation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/spec/header.py` & `litestar-2.0.0a4/litestar/openapi/spec/header.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/spec/info.py` & `litestar-2.0.0a4/litestar/openapi/spec/info.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/spec/license.py` & `litestar-2.0.0a4/litestar/openapi/spec/license.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/spec/link.py` & `litestar-2.0.0a4/litestar/openapi/spec/link.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/spec/media_type.py` & `litestar-2.0.0a4/litestar/openapi/spec/media_type.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/spec/oauth_flow.py` & `litestar-2.0.0a4/litestar/openapi/spec/oauth_flow.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/spec/oauth_flows.py` & `litestar-2.0.0a4/litestar/openapi/spec/oauth_flows.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/spec/open_api.py` & `litestar-2.0.0a4/litestar/openapi/spec/open_api.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/spec/operation.py` & `litestar-2.0.0a4/litestar/openapi/spec/operation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/spec/parameter.py` & `litestar-2.0.0a4/litestar/openapi/spec/parameter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/spec/path_item.py` & `litestar-2.0.0a4/litestar/openapi/spec/path_item.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/spec/paths.py` & `litestar-2.0.0a4/litestar/openapi/spec/paths.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/spec/reference.py` & `litestar-2.0.0a4/litestar/openapi/spec/reference.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/spec/request_body.py` & `litestar-2.0.0a4/litestar/openapi/spec/request_body.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/spec/response.py` & `litestar-2.0.0a4/litestar/openapi/spec/response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/spec/responses.py` & `litestar-2.0.0a4/litestar/openapi/spec/responses.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/spec/schema.py` & `litestar-2.0.0a4/litestar/openapi/spec/schema.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/spec/security_requirement.py` & `litestar-2.0.0a4/litestar/openapi/spec/security_requirement.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/spec/security_scheme.py` & `litestar-2.0.0a4/litestar/openapi/spec/security_scheme.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/spec/server.py` & `litestar-2.0.0a4/litestar/openapi/spec/server.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/spec/server_variable.py` & `litestar-2.0.0a4/litestar/openapi/spec/server_variable.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/spec/tag.py` & `litestar-2.0.0a4/litestar/openapi/spec/tag.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/openapi/spec/xml.py` & `litestar-2.0.0a4/litestar/openapi/spec/xml.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/pagination.py` & `litestar-2.0.0a4/litestar/pagination.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/params.py` & `litestar-2.0.0a4/litestar/params.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/plugins.py` & `litestar-2.0.0a4/litestar/plugins.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/response/base.py` & `litestar-2.0.0a4/litestar/response/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/response/file.py` & `litestar-2.0.0a4/litestar/response/file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/response/streaming.py` & `litestar-2.0.0a4/litestar/response/streaming.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/response/template.py` & `litestar-2.0.0a4/litestar/response/template.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/response_containers.py` & `litestar-2.0.0a4/litestar/response_containers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/router.py` & `litestar-2.0.0a4/litestar/router.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/routes/asgi.py` & `litestar-2.0.0a4/litestar/routes/asgi.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/routes/base.py` & `litestar-2.0.0a4/litestar/routes/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/routes/http.py` & `litestar-2.0.0a4/litestar/routes/http.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/routes/websocket.py` & `litestar-2.0.0a4/litestar/routes/websocket.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/security/base.py` & `litestar-2.0.0a4/litestar/security/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/security/session_auth/auth.py` & `litestar-2.0.0a4/litestar/security/session_auth/auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/security/session_auth/middleware.py` & `litestar-2.0.0a4/litestar/security/session_auth/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/serialization.py` & `litestar-2.0.0a4/litestar/serialization.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/static_files/base.py` & `litestar-2.0.0a4/litestar/static_files/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/static_files/config.py` & `litestar-2.0.0a4/litestar/static_files/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/status_codes.py` & `litestar-2.0.0a4/litestar/status_codes.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/stores/base.py` & `litestar-2.0.0a4/litestar/stores/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/stores/file.py` & `litestar-2.0.0a4/litestar/stores/file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/stores/memory.py` & `litestar-2.0.0a4/litestar/stores/memory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/stores/redis.py` & `litestar-2.0.0a4/litestar/stores/redis.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/stores/registry.py` & `litestar-2.0.0a4/litestar/stores/registry.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/template/base.py` & `litestar-2.0.0a4/litestar/template/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/template/config.py` & `litestar-2.0.0a4/litestar/template/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/testing/__init__.py` & `litestar-2.0.0a4/litestar/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/testing/client/__init__.py` & `litestar-2.0.0a4/litestar/testing/client/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/testing/client/async_client.py` & `litestar-2.0.0a4/litestar/testing/client/async_client.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/testing/client/base.py` & `litestar-2.0.0a4/litestar/testing/client/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/testing/client/sync_client.py` & `litestar-2.0.0a4/litestar/testing/client/sync_client.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/testing/helpers.py` & `litestar-2.0.0a4/litestar/testing/helpers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/testing/life_span_handler.py` & `litestar-2.0.0a4/litestar/testing/life_span_handler.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/testing/request_factory.py` & `litestar-2.0.0a4/litestar/testing/request_factory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/testing/transport.py` & `litestar-2.0.0a4/litestar/testing/transport.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/testing/websocket_test_session.py` & `litestar-2.0.0a4/litestar/testing/websocket_test_session.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/types/__init__.py` & `litestar-2.0.0a4/litestar/types/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/types/asgi_types.py` & `litestar-2.0.0a4/litestar/types/asgi_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/types/callable_types.py` & `litestar-2.0.0a4/litestar/types/callable_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/types/composite_types.py` & `litestar-2.0.0a4/litestar/types/composite_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/types/file_types.py` & `litestar-2.0.0a4/litestar/types/file_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/types/internal_types.py` & `litestar-2.0.0a4/litestar/types/internal_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/types/parsed_signature.py` & `litestar-2.0.0a4/litestar/utils/signature.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,74 @@
 from __future__ import annotations
 
-from collections.abc import Collection
+import sys
+import typing
 from dataclasses import dataclass
-from inspect import Parameter, Signature
-from typing import TYPE_CHECKING, Any, AnyStr, Union
+from inspect import Parameter, Signature, getmembers, isclass, ismethod
+from itertools import chain
+from typing import Any, AnyStr, Collection, Union
 
-from typing_extensions import Annotated, NotRequired, Required, get_args, get_origin
+from typing_extensions import Annotated, NotRequired, Required, get_args, get_origin, get_type_hints
 
-from litestar.datastructures.state import ImmutableState
+from litestar import connection, datastructures, types
+from litestar.datastructures import ImmutableState
 from litestar.exceptions import ImproperlyConfiguredException
+from litestar.params import BodyKwarg, DependencyKwarg, ParameterKwarg
+from litestar.types import AnyCallable, Empty
 from litestar.types.builtin_types import UNION_TYPES, NoneType
-from litestar.types.empty import Empty
-from litestar.utils.signature_parsing import get_fn_type_hints
 from litestar.utils.typing import get_safe_generic_origin, unwrap_annotation
 
-if TYPE_CHECKING:
-    from litestar.types import AnyCallable
+_GLOBAL_NAMES = {
+    namespace: export
+    for namespace, export in chain(
+        tuple(getmembers(types)), tuple(getmembers(connection)), tuple(getmembers(datastructures))
+    )
+    if namespace[0].isupper()
+    and namespace in chain(types.__all__, connection.__all__, datastructures.__all__)  # pyright: ignore
+}
+"""A mapping of names used for handler signature forward-ref resolution.
+
+This allows users to include these names within an `if TYPE_CHECKING:` block in their handler module.
+"""
+
+__all__ = ("get_fn_type_hints", "ParsedType", "ParsedParameter", "ParsedSignature")
+
 
-__all__ = (
-    "ParsedType",
-    "ParsedParameter",
-    "ParsedSignature",
-)
+def get_fn_type_hints(fn: Any, namespace: dict[str, Any] | None = None) -> dict[str, Any]:
+    """Resolve type hints for ``fn``.
+
+    Args:
+        fn: Callable that is being inspected
+        namespace: Extra names for resolution of forward references.
+
+    Returns:
+        Mapping of names to types.
+    """
+    fn_to_inspect: Any = fn
+
+    if isclass(fn_to_inspect):
+        fn_to_inspect = fn_to_inspect.__init__
+
+    # detect objects that are not functions and that have a `__call__` method
+    if callable(fn_to_inspect) and ismethod(fn_to_inspect.__call__):
+        fn_to_inspect = fn_to_inspect.__call__
+
+    # inspect the underlying function for methods
+    if hasattr(fn_to_inspect, "__func__"):
+        fn_to_inspect = fn_to_inspect.__func__
+
+    # Order important. If a litestar name has been overridden in the function module, we want
+    # to use that instead of the litestar one.
+    namespace = {
+        **_GLOBAL_NAMES,
+        **vars(typing),
+        **vars(sys.modules[fn_to_inspect.__module__]),
+        **(namespace or {}),
+    }
+    return get_type_hints(fn_to_inspect, globalns=namespace, include_extras=True)
 
 
 @dataclass(frozen=True)
 class ParsedType:
     """Represents a type annotation."""
 
     __slots__ = (
@@ -148,14 +191,27 @@
     """The name of the parameter."""
     default: Any | Empty
     """The default value of the parameter."""
     parsed_type: ParsedType
     """The annotation of the parameter."""
 
     @property
+    def kwarg_container(self) -> ParameterKwarg | BodyKwarg | DependencyKwarg | None:
+        """A kwarg container, if any"""
+        for value in (*self.metadata, self.default):
+            if isinstance(value, (ParameterKwarg, BodyKwarg, DependencyKwarg)):
+                return value
+        return None
+
+    @property
+    def metadata(self) -> tuple[Any, ...]:
+        """The metadata of the parameter's annotation."""
+        return self.parsed_type.metadata
+
+    @property
     def annotation(self) -> Any:
         """The annotation of the parameter."""
         return self.parsed_type.annotation
 
     @property
     def has_default(self) -> bool:
         """Whether the parameter has a default value or not."""
```

### Comparing `litestar-2.0.0a3/litestar/types/protocols.py` & `litestar-2.0.0a4/litestar/types/protocols.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,13 +75,23 @@
 
         Args:
              event: Log message.
              *args: Any args.
              **kwargs: Any kwargs.
         """
 
+    def setLevel(self, level: int) -> None:  # noqa: N802
+        """Set the log level
+
+        Args:
+            level: Log level to set as an integer
+
+        Returns:
+            None
+        """
+
 
 @runtime_checkable
 class DataclassProtocol(Protocol):
     """Protocol for instance checking dataclasses"""
 
     __dataclass_fields__: ClassVar[Dict[str, Any]]
```

### Comparing `litestar-2.0.0a3/litestar/types/serialization.py` & `litestar-2.0.0a4/litestar/types/serialization.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/utils/__init__.py` & `litestar-2.0.0a4/litestar/utils/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,16 +2,20 @@
 
 from .helpers import Ref, get_enum_string_value, get_name
 from .path import join_paths, normalize_path
 from .predicates import (
     is_any,
     is_attrs_class,
     is_class_and_subclass,
+    is_class_var,
     is_dataclass_class,
+    is_generic,
     is_mapping,
+    is_non_string_iterable,
+    is_non_string_sequence,
     is_optional_union,
     is_pydantic_constrained_field,
     is_pydantic_model_class,
     is_pydantic_model_instance,
     is_typed_dict,
     is_union,
 )
@@ -39,24 +43,28 @@
     "as_async_callable_list",
     "async_partial",
     "compact",
     "delete_litestar_scope_state",
     "deprecated",
     "find_index",
     "get_enum_string_value",
+    "get_litestar_scope_state",
     "get_name",
     "get_origin_or_inner_type",
     "get_serializer_from_scope",
-    "get_litestar_scope_state",
     "is_any",
     "is_async_callable",
     "is_attrs_class",
     "is_class_and_subclass",
+    "is_class_var",
     "is_dataclass_class",
+    "is_generic",
     "is_mapping",
+    "is_non_string_iterable",
+    "is_non_string_sequence",
     "is_optional_union",
     "is_pydantic_constrained_field",
     "is_pydantic_model_class",
     "is_pydantic_model_instance",
     "is_typed_dict",
     "is_union",
     "join_paths",
```

### Comparing `litestar-2.0.0a3/litestar/utils/compat.py` & `litestar-2.0.0a4/litestar/utils/compat.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/utils/dataclass.py` & `litestar-2.0.0a4/litestar/utils/dataclass.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/utils/deprecation.py` & `litestar-2.0.0a4/litestar/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/utils/helpers.py` & `litestar-2.0.0a4/litestar/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/utils/path.py` & `litestar-2.0.0a4/litestar/utils/path.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/utils/predicates.py` & `litestar-2.0.0a4/litestar/utils/predicates.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from collections import defaultdict, deque
 from collections.abc import Iterable as CollectionsIterable
 from dataclasses import is_dataclass
 from inspect import isclass
 from typing import (
     TYPE_CHECKING,
     Any,
+    ClassVar,
     DefaultDict,
     Deque,
     Dict,
     FrozenSet,
     Generic,
     Iterable,
     List,
@@ -18,14 +19,15 @@
     Optional,
     Sequence,
     Set,
     Tuple,
     TypeVar,
 )
 
+from msgspec import Struct
 from typing_extensions import (
     ParamSpec,
     TypeGuard,
     get_args,
     is_typeddict,
 )
 
@@ -44,14 +46,31 @@
     pydantic = Empty  # type: ignore
 
 try:
     import attrs
 except ImportError:  # pragma: no cover
     attrs = Empty  # type: ignore
 
+__all__ = (
+    "is_any",
+    "is_attrs_class",
+    "is_class_and_subclass",
+    "is_class_var",
+    "is_dataclass_class",
+    "is_generic",
+    "is_mapping",
+    "is_non_string_iterable",
+    "is_non_string_sequence",
+    "is_optional_union",
+    "is_pydantic_constrained_field",
+    "is_pydantic_model_class",
+    "is_pydantic_model_instance",
+    "is_typed_dict",
+    "is_union",
+)
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
 
 def is_class_and_subclass(annotation: Any, t_type: type[T]) -> TypeGuard[type[T]]:
     """Return ``True`` if ``value`` is a ``class`` and is a subtype of ``t_type``.
@@ -248,15 +267,15 @@
         A typeguard determining whether the type is :data:`BaseModel pydantic.BaseModel>`.
     """
     if pydantic is not Empty:  # type: ignore[comparison-overlap]
         return isinstance(annotation, pydantic.BaseModel)  # pyright: ignore
     return False  # pragma: no cover
 
 
-def is_attrs_class(annotation: Any) -> TypeGuard["attrs.AttrsInstance"]:  # pyright: ignore
+def is_attrs_class(annotation: Any) -> TypeGuard[type[attrs.AttrsInstance]]:  # pyright: ignore
     """Given a type annotation determine if the annotation is a class that includes an attrs attribute.
 
     Args:
         annotation: A type.
 
     Returns:
         A typeguard determining whether the type is an attrs class.
@@ -302,7 +321,32 @@
                 pydantic.ConstrainedList,
                 pydantic.ConstrainedSet,
                 pydantic.ConstrainedStr,
             )
         )
     except ImportError:
         return False
+
+
+def is_struct_class(annotation: Any) -> TypeGuard[type[Struct]]:
+    """Check if the given annotation is a :class:`Struct <msgspec.Struct>` type.
+
+    Args:
+        annotation: A type annotation
+
+    Returns:
+        A typeguard for :class:`Struct <msgspec.Struct>`.
+    """
+    return is_class_and_subclass(annotation, Struct)
+
+
+def is_class_var(annotation: Any) -> bool:
+    """Check if the given annotation is a ClassVar.
+
+    Args:
+        annotation: A type annotation
+
+    Returns:
+        A boolean.
+    """
+    annotation = get_origin_or_inner_type(annotation) or annotation
+    return annotation is ClassVar
```

### Comparing `litestar-2.0.0a3/litestar/utils/scope.py` & `litestar-2.0.0a4/litestar/utils/scope.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/litestar/utils/sequence.py` & `litestar-2.0.0a4/litestar/utils/sequence.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from typing import Any, Callable, Sequence, TypeVar
 
-__all__ = ("find_index", "unique")
+__all__ = ("find_index", "unique", "compact")
 
 
 T = TypeVar("T")
 
 
 def find_index(target_list: list[T], predicate: Callable[[T], bool]) -> int:
     """Find element in list given a key and value.
```

### Comparing `litestar-2.0.0a3/litestar/utils/sync.py` & `litestar-2.0.0a4/litestar/utils/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.types import Empty
 from litestar.utils.helpers import Ref
 
 if TYPE_CHECKING:
     from litestar.types.empty import EmptyType
-    from litestar.types.parsed_signature import ParsedSignature
+    from litestar.utils.signature import ParsedSignature
 
 __all__ = ("AsyncCallable", "AsyncIteratorWrapper", "as_async_callable_list", "async_partial", "is_async_callable")
 
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
@@ -91,15 +91,15 @@
 
     def set_parsed_signature(self, namespace: dict[str, Any]) -> None:
         """Set the parsed signature of the wrapped function.
 
         Args:
             namespace: Namespace for forward ref resolution.
         """
-        from litestar.types.parsed_signature import ParsedSignature
+        from litestar.utils.signature import ParsedSignature
 
         self._parsed_signature = ParsedSignature.from_fn(self.ref.value, namespace)
 
 
 def as_async_callable_list(value: Callable | list[Callable]) -> list[AsyncCallable]:
     """Wrap callables in ``AsyncCallable`` s.
```

### Comparing `litestar-2.0.0a3/litestar/utils/typing.py` & `litestar-2.0.0a4/litestar/utils/typing.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
 from typing_extensions import Annotated, NotRequired, Required, TypeGuard, get_args, get_origin
 
 from litestar.types.builtin_types import UNION_TYPES, NoneType
 
 __all__ = (
     "annotation_is_iterable_of_type",
+    "get_origin_or_inner_type",
     "get_safe_generic_origin",
     "make_non_optional_union",
     "unwrap_annotation",
 )
 
 
 T = TypeVar("T")
@@ -192,18 +193,20 @@
 
     Args:
         annotation: A type annotation.
 
     Returns:
         Any type.
     """
-
     origin = get_origin(annotation)
     if origin in wrapper_type_set:
-        origin, _, _ = unwrap_annotation(annotation)
+        inner, _, _ = unwrap_annotation(annotation)
+        # we need to recursively call here 'get_origin_or_inner_type' because we might be dealing with a generic type alias
+        # e.g. Annotated[dict[str, list[int]]
+        origin = get_origin_or_inner_type(inner)
     return types_mapping.get(origin, origin)
 
 
 def get_safe_generic_origin(origin_type: Any) -> Any:
     """Get a type that is safe to use as a generic type across all supported Python versions.
 
     Args:
```

### Comparing `litestar-2.0.0a3/litestar/utils/version.py` & `litestar-2.0.0a4/litestar/utils/version.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a3/pyproject.toml` & `litestar-2.0.0a4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "litestar"
-version = "2.0.0alpha3"
+version = "2.0.0alpha4"
 description = "Performant, light and flexible ASGI API Framework"
 authors = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
     "Peter Schutt <peter.github@proton.me>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
 ]
@@ -65,15 +65,15 @@
 jinja2 = { version = ">=3.1.2", optional = true }
 jsbeautifier = { version = "*", optional = true }
 mako = { version = ">=1.2.4", optional = true }
 msgspec = "*"
 multidict = ">=6.0.2"
 opentelemetry-instrumentation-asgi = { version = "*", optional = true }
 picologging = { version = "*", optional = true }
-polyfactory = "*"
+polyfactory = {version = ">=2.0.0a1", allow-prereleases = true}
 pydantic = "<2"
 python-dateutil = { version = "*", optional = true }
 python-jose = { version = "*", optional = true }
 pytimeparse = { version = "*", optional = true }
 pyyaml = "*"
 redis = { version = ">=4.4.4,!=4.5.0,!=4.5.1,!=4.5.2,!=4.5.3", optional = true, extras = ["hiredis"] }
 rich = { version = ">=13.0.0", optional = true }
@@ -137,15 +137,15 @@
 sphinxcontrib-mermaid = ">=0.8.1,<1"
 litestar-sphinx-theme = { git = "https://github.com/litestar-org/litestar-sphinx-theme.git" }
 uvicorn = "*"
 
 [tool.poetry.extras]
 attrs = ["attrs", "cattrs", "python-dateutil", "pytimeparse"]
 brotli = ["brotli"]
-cli = ["click", "rich", "jsbeautifier"]
+cli = ["click", "rich", "jsbeautifier", "uvicorn"]
 cryptography = ["cryptography"]
 jinja = ["jinja2"]
 jwt = ["python-jose", "cryptography"]
 opentelemetry = ["opentelemetry-instrumentation-asgi"]
 picologging = ["picologging"]
 redis = ["redis"]
 sqlalchemy = ["sqlalchemy", "alembic"]
```

### Comparing `litestar-2.0.0a3/PKG-INFO` & `litestar-2.0.0a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litestar
-Version: 2.0.0a3
+Version: 2.0.0a4
 Summary: Performant, light and flexible ASGI API Framework
 Home-page: https://litestar.dev/
 License: MIT
 Keywords: api,rest,http,asgi,pydantic,litestar,starlite,framework,websocket,litestar
 Author: Na'aman Hirschfeld
 Author-email: nhirschfeld@gmail.com
 Maintainer: Na'aman Hirschfeld
@@ -56,15 +56,15 @@
 Requires-Dist: jinja2 (>=3.1.2) ; extra == "jinja" or extra == "standard" or extra == "full"
 Requires-Dist: jsbeautifier ; extra == "cli" or extra == "standard" or extra == "full"
 Requires-Dist: mako (>=1.2.4)
 Requires-Dist: msgspec
 Requires-Dist: multidict (>=6.0.2)
 Requires-Dist: opentelemetry-instrumentation-asgi ; extra == "opentelemetry" or extra == "full"
 Requires-Dist: picologging ; extra == "picologging" or extra == "full"
-Requires-Dist: polyfactory
+Requires-Dist: polyfactory (>=2.0.0a1)
 Requires-Dist: pydantic (<2)
 Requires-Dist: python-dateutil ; extra == "attrs"
 Requires-Dist: python-jose ; extra == "jwt" or extra == "full"
 Requires-Dist: pytimeparse ; extra == "attrs"
 Requires-Dist: pyyaml
 Requires-Dist: redis[hiredis] (>=4.4.4,!=4.5.0,!=4.5.1,!=4.5.2,!=4.5.3) ; extra == "redis" or extra == "full"
 Requires-Dist: rich (>=13.0.0) ; extra == "cli" or extra == "standard" or extra == "full"
@@ -93,15 +93,15 @@
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 
 <!-- prettier-ignore-start -->
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-92-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-95-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 <!-- prettier-ignore-end -->
 
 [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestar?label=r%2FLitestar&logo=reddit)](https://reddit.com/r/litestar-api)
 [![Discord](https://img.shields.io/discord/919193495116337154?color=blue&label=chat%20on%20discord&logo=discord)](https://discord.gg/X3FJqy8d2j)
 [![Matrix](https://img.shields.io/badge/%5Bm%5D%20chat%20on%20Matrix-bridged-blue)](https://matrix.to/#/#litestar:matrix.org)
 [![Medium](https://img.shields.io/badge/Medium-12100E?style=flat&logo=medium&logoColor=white)](https://blog.litestar.dev)
@@ -111,15 +111,15 @@
 # Starlite → Litestar
 
 **[Starlite has been renamed to Litestar](https://litestar.dev/about/organization.html#litestar-and-starlite)**
 
 <hr>
 
 Litestar is a powerful, performant, flexible and opinionated ASGI framework,
-offering first class typing support and a full [Pydantic](https://github.com/samuelcolvin/pydantic)
+offering first class typing support and a full [Pydantic](https://github.com/pydantic/pydantic)
 integration.
 
 Check out the [documentation 📚](https://docs.litestar.dev/).
 
 ## Installation
 
 ```shell
@@ -148,15 +148,15 @@
 app = Litestar(route_handlers=[hello_world])
 ```
 
 ## Core Features
 
 - [Class based controllers](#class-based-controllers)
 - [Dependency Injection](#dependency-injection)
-- [Validation and Parsing](#data-parsing-type-hints-and-pydantic) using [Pydantic](https://github.com/samuelcolvin/pydantic)
+- [Validation and Parsing](#data-parsing-type-hints-and-pydantic) using [Pydantic](https://github.com/pydantic/pydantic)
 - [Layered Middleware](#middleware)
 - [Plugin System](#plugin-system-orm-support-and-dtos)
 - [OpenAPI 3.1 schema generation](#openapi)
 - [Life Cycle Hooks](#request-life-cycle-hooks)
 - [Route Guards based Authorization](#route-guards)
 - Layered Parameter declaration
 - SQLAlchemy Support (via plugin)
@@ -476,14 +476,17 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Galdanwing"><img src="https://avatars.githubusercontent.com/u/29492757?v=4?s=100" width="100px;" alt="Antoine van der Horst"/><br /><sub><b>Antoine van der Horst</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=Galdanwing" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://nick.groenen.me"><img src="https://avatars.githubusercontent.com/u/145285?v=4?s=100" width="100px;" alt="Nick Groenen"/><br /><sub><b>Nick Groenen</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=zoni" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/giorgiovilardo"><img src="https://avatars.githubusercontent.com/u/56472600?v=4?s=100" width="100px;" alt="Giorgio Vilardo"/><br /><sub><b>Giorgio Vilardo</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=giorgiovilardo" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/bollwyvl"><img src="https://avatars.githubusercontent.com/u/45380?v=4?s=100" width="100px;" alt="Nicholas Bollweg"/><br /><sub><b>Nicholas Bollweg</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=bollwyvl" title="Code">💻</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/tompin82"><img src="https://avatars.githubusercontent.com/u/47041409?v=4?s=100" width="100px;" alt="Tomas Jonsson"/><br /><sub><b>Tomas Jonsson</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=tompin82" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://www.linkedin.com/in/khiem-doan/"><img src="https://avatars.githubusercontent.com/u/15646249?v=4?s=100" width="100px;" alt="Khiem Doan"/><br /><sub><b>Khiem Doan</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=khiemdoan" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/kedod"><img src="https://avatars.githubusercontent.com/u/35638715?v=4?s=100" width="100px;" alt="kedod"/><br /><sub><b>kedod</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=kedod" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/sonpro1296"><img src="https://avatars.githubusercontent.com/u/17319142?v=4?s=100" width="100px;" alt="sonpro1296"/><br /><sub><b>sonpro1296</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=sonpro1296" title="Code">💻</a> <a href="https://github.com/litestar-org/litestar/commits?author=sonpro1296" title="Tests">⚠️</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

