# Comparing `tmp/ory-hydra-client-2.1.0.tar.gz` & `tmp/ory-hydra-client-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ory-hydra-client-2.1.0.tar", last modified: Fri Apr  7 12:21:17 2023, max compression
+gzip compressed data, was "dist/ory-hydra-client-2.1.1.tar", last modified: Tue Apr 11 11:02:18 2023, max compression
```

## Comparing `ory-hydra-client-2.1.0.tar` & `ory-hydra-client-2.1.1.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 12:21:17.000000 ory-hydra-client-2.1.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      368 2023-04-07 12:21:17.000000 ory-hydra-client-2.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13643 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 12:21:17.000000 ory-hydra-client-2.1.0/ory_hydra_client/
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 12:21:17.000000 ory-hydra-client-2.1.0/ory_hydra_client/api/
--rw-r--r--   0 root         (0) root         (0)      216 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40315 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/api/jwk_api.py
--rw-r--r--   0 root         (0) root         (0)    15923 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/api/metadata_api.py
--rw-r--r--   0 root         (0) root         (0)   161855 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/api/o_auth2_api.py
--rw-r--r--   0 root         (0) root         (0)    39735 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/api/oidc_api.py
--rw-r--r--   0 root         (0) root         (0)     5812 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/api/wellknown_api.py
--rw-r--r--   0 root         (0) root         (0)    39105 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 12:21:17.000000 ory-hydra-client-2.1.0/ory_hydra_client/apis/
--rw-r--r--   0 root         (0) root         (0)      692 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17353 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5065 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 12:21:17.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13862 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/accept_o_auth2_consent_request.py
--rw-r--r--   0 root         (0) root         (0)    13280 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/accept_o_auth2_consent_request_session.py
--rw-r--r--   0 root         (0) root         (0)    18024 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/accept_o_auth2_login_request.py
--rw-r--r--   0 root         (0) root         (0)    12717 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/create_json_web_key_set.py
--rw-r--r--   0 root         (0) root         (0)    12578 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/error_o_auth2.py
--rw-r--r--   0 root         (0) root         (0)    13854 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/generic_error.py
--rw-r--r--   0 root         (0) root         (0)    11491 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/get_version200_response.py
--rw-r--r--   0 root         (0) root         (0)    11595 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/health_not_ready_status.py
--rw-r--r--   0 root         (0) root         (0)    11469 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/health_status.py
--rw-r--r--   0 root         (0) root         (0)    17903 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/introspected_o_auth2_token.py
--rw-r--r--   0 root         (0) root         (0)    11455 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/is_ready200_response.py
--rw-r--r--   0 root         (0) root         (0)    11589 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/is_ready503_response.py
--rw-r--r--   0 root         (0) root         (0)    13268 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/json_patch.py
--rw-r--r--   0 root         (0) root         (0)    11973 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/json_patch_document.py
--rw-r--r--   0 root         (0) root         (0)    17879 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/json_web_key.py
--rw-r--r--   0 root         (0) root         (0)    12231 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/json_web_key_set.py
--rw-r--r--   0 root         (0) root         (0)    11777 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/null_duration.py
--rw-r--r--   0 root         (0) root         (0)    38709 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/o_auth2_client.py
--rw-r--r--   0 root         (0) root         (0)    15319 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/o_auth2_client_token_lifespans.py
--rw-r--r--   0 root         (0) root         (0)    18380 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/o_auth2_consent_request.py
--rw-r--r--   0 root         (0) root         (0)    18408 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/o_auth2_consent_request_open_id_connect_context.py
--rw-r--r--   0 root         (0) root         (0)    14822 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/o_auth2_consent_session.py
--rw-r--r--   0 root         (0) root         (0)    12423 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/o_auth2_consent_session_expires_at.py
--rw-r--r--   0 root         (0) root         (0)    12114 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/o_auth2_consent_sessions.py
--rw-r--r--   0 root         (0) root         (0)    17251 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/o_auth2_login_request.py
--rw-r--r--   0 root         (0) root         (0)    13458 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/o_auth2_logout_request.py
--rw-r--r--   0 root         (0) root         (0)    11760 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/o_auth2_redirect_to.py
--rw-r--r--   0 root         (0) root         (0)    13444 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/o_auth2_token_exchange.py
--rw-r--r--   0 root         (0) root         (0)    32243 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/oidc_configuration.py
--rw-r--r--   0 root         (0) root         (0)    24504 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/oidc_user_info.py
--rw-r--r--   0 root         (0) root         (0)    12744 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/pagination.py
--rw-r--r--   0 root         (0) root         (0)    12101 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/pagination_headers.py
--rw-r--r--   0 root         (0) root         (0)    13152 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/reject_o_auth2_request.py
--rw-r--r--   0 root         (0) root         (0)    11698 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/string_slice_json_format.py
--rw-r--r--   0 root         (0) root         (0)    12759 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/token_pagination.py
--rw-r--r--   0 root         (0) root         (0)    12116 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/token_pagination_headers.py
--rw-r--r--   0 root         (0) root         (0)    12809 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/token_pagination_request_parameters.py
--rw-r--r--   0 root         (0) root         (0)    13024 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/token_pagination_response_headers.py
--rw-r--r--   0 root         (0) root         (0)    13797 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/trust_o_auth2_jwt_grant_issuer.py
--rw-r--r--   0 root         (0) root         (0)    14371 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/trusted_o_auth2_jwt_grant_issuer.py
--rw-r--r--   0 root         (0) root         (0)    12284 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/trusted_o_auth2_jwt_grant_issuers.py
--rw-r--r--   0 root         (0) root         (0)    11968 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/trusted_o_auth2_jwt_grant_json_web_key.py
--rw-r--r--   0 root         (0) root         (0)    11465 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model/version.py
--rw-r--r--   0 root         (0) root         (0)    82577 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 12:21:17.000000 ory-hydra-client-2.1.0/ory_hydra_client/models/
--rw-r--r--   0 root         (0) root         (0)     3793 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14271 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/ory_hydra_client/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 12:21:17.000000 ory-hydra-client-2.1.0/ory_hydra_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      368 2023-04-07 12:21:16.000000 ory-hydra-client-2.1.0/ory_hydra_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4561 2023-04-07 12:21:17.000000 ory-hydra-client-2.1.0/ory_hydra_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 12:21:16.000000 ory-hydra-client-2.1.0/ory_hydra_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-04-07 12:21:16.000000 ory-hydra-client-2.1.0/ory_hydra_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-04-07 12:21:17.000000 ory-hydra-client-2.1.0/ory_hydra_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-04-07 12:21:17.000000 ory-hydra-client-2.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1043 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 12:21:17.000000 ory-hydra-client-2.1.0/test/
--rw-r--r--   0 root         (0) root         (0)     1170 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_accept_o_auth2_consent_request.py
--rw-r--r--   0 root         (0) root         (0)      888 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_accept_o_auth2_consent_request_session.py
--rw-r--r--   0 root         (0) root         (0)      965 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_accept_o_auth2_login_request.py
--rw-r--r--   0 root         (0) root         (0)      789 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_create_json_web_key_set.py
--rw-r--r--   0 root         (0) root         (0)      731 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_error_o_auth2.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_generic_error.py
--rw-r--r--   0 root         (0) root         (0)      801 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_get_version200_response.py
--rw-r--r--   0 root         (0) root         (0)      795 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_health_not_ready_status.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_health_status.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_introspected_o_auth2_token.py
--rw-r--r--   0 root         (0) root         (0)      780 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_is_ready200_response.py
--rw-r--r--   0 root         (0) root         (0)      780 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_is_ready503_response.py
--rw-r--r--   0 root         (0) root         (0)      716 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_json_patch.py
--rw-r--r--   0 root         (0) root         (0)      864 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_json_patch_document.py
--rw-r--r--   0 root         (0) root         (0)      724 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_json_web_key.py
--rw-r--r--   0 root         (0) root         (0)      842 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_json_web_key_set.py
--rw-r--r--   0 root         (0) root         (0)     1636 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_jwk_api.py
--rw-r--r--   0 root         (0) root         (0)     1001 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_null_duration.py
--rw-r--r--   0 root         (0) root         (0)     5738 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_o_auth2_api.py
--rw-r--r--   0 root         (0) root         (0)      982 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_o_auth2_client.py
--rw-r--r--   0 root         (0) root         (0)      941 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_o_auth2_client_token_lifespans.py
--rw-r--r--   0 root         (0) root         (0)     1261 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_o_auth2_consent_request.py
--rw-r--r--   0 root         (0) root         (0)      939 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_o_auth2_consent_request_open_id_connect_context.py
--rw-r--r--   0 root         (0) root         (0)     1439 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_o_auth2_consent_session.py
--rw-r--r--   0 root         (0) root         (0)      860 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_o_auth2_consent_session_expires_at.py
--rw-r--r--   0 root         (0) root         (0)      939 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_o_auth2_consent_sessions.py
--rw-r--r--   0 root         (0) root         (0)     1247 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_o_auth2_login_request.py
--rw-r--r--   0 root         (0) root         (0)      892 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_o_auth2_logout_request.py
--rw-r--r--   0 root         (0) root         (0)      767 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_o_auth2_redirect_to.py
--rw-r--r--   0 root         (0) root         (0)      788 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_o_auth2_token_exchange.py
--rw-r--r--   0 root         (0) root         (0)     1913 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_oidc_api.py
--rw-r--r--   0 root         (0) root         (0)      772 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_oidc_configuration.py
--rw-r--r--   0 root         (0) root         (0)      738 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_oidc_user_info.py
--rw-r--r--   0 root         (0) root         (0)      722 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_pagination.py
--rw-r--r--   0 root         (0) root         (0)      772 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_pagination_headers.py
--rw-r--r--   0 root         (0) root         (0)      788 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_reject_o_auth2_request.py
--rw-r--r--   0 root         (0) root         (0)      802 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_string_slice_json_format.py
--rw-r--r--   0 root         (0) root         (0)      758 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_token_pagination.py
--rw-r--r--   0 root         (0) root         (0)      808 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_token_pagination_headers.py
--rw-r--r--   0 root         (0) root         (0)      879 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_token_pagination_request_parameters.py
--rw-r--r--   0 root         (0) root         (0)      865 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_token_pagination_response_headers.py
--rw-r--r--   0 root         (0) root         (0)      928 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_trust_o_auth2_jwt_grant_issuer.py
--rw-r--r--   0 root         (0) root         (0)     1031 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_trusted_o_auth2_jwt_grant_issuer.py
--rw-r--r--   0 root         (0) root         (0)     1020 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_trusted_o_auth2_jwt_grant_issuers.py
--rw-r--r--   0 root         (0) root         (0)      876 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_trusted_o_auth2_jwt_grant_json_web_key.py
--rw-r--r--   0 root         (0) root         (0)      701 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_version.py
--rw-r--r--   0 root         (0) root         (0)      742 2023-04-07 12:17:19.000000 ory-hydra-client-2.1.0/test/test_wellknown_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:02:18.000000 ory-hydra-client-2.1.1/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-04-11 10:57:25.000000 ory-hydra-client-2.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      368 2023-04-11 11:02:18.000000 ory-hydra-client-2.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13643 2023-04-11 10:57:25.000000 ory-hydra-client-2.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:02:18.000000 ory-hydra-client-2.1.1/ory_hydra_client/
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-11 10:57:25.000000 ory-hydra-client-2.1.1/ory_hydra_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:02:18.000000 ory-hydra-client-2.1.1/ory_hydra_client/api/
+-rw-r--r--   0 root         (0) root         (0)      216 2023-04-11 10:57:25.000000 ory-hydra-client-2.1.1/ory_hydra_client/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40315 2023-04-11 10:57:25.000000 ory-hydra-client-2.1.1/ory_hydra_client/api/jwk_api.py
+-rw-r--r--   0 root         (0) root         (0)    15923 2023-04-11 10:57:25.000000 ory-hydra-client-2.1.1/ory_hydra_client/api/metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)   161855 2023-04-11 10:57:25.000000 ory-hydra-client-2.1.1/ory_hydra_client/api/o_auth2_api.py
+-rw-r--r--   0 root         (0) root         (0)    39735 2023-04-11 10:57:25.000000 ory-hydra-client-2.1.1/ory_hydra_client/api/oidc_api.py
+-rw-r--r--   0 root         (0) root         (0)     5812 2023-04-11 10:57:25.000000 ory-hydra-client-2.1.1/ory_hydra_client/api/wellknown_api.py
+-rw-r--r--   0 root         (0) root         (0)    39105 2023-04-11 10:57:25.000000 ory-hydra-client-2.1.1/ory_hydra_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:02:18.000000 ory-hydra-client-2.1.1/ory_hydra_client/apis/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-04-11 10:57:25.000000 ory-hydra-client-2.1.1/ory_hydra_client/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17353 2023-04-11 10:57:25.000000 ory-hydra-client-2.1.1/ory_hydra_client/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5065 2023-04-11 10:57:25.000000 ory-hydra-client-2.1.1/ory_hydra_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:02:18.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 10:57:25.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13862 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/accept_o_auth2_consent_request.py
+-rw-r--r--   0 root         (0) root         (0)    13280 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/accept_o_auth2_consent_request_session.py
+-rw-r--r--   0 root         (0) root         (0)    18024 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/accept_o_auth2_login_request.py
+-rw-r--r--   0 root         (0) root         (0)    12717 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/create_json_web_key_set.py
+-rw-r--r--   0 root         (0) root         (0)    12578 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/error_o_auth2.py
+-rw-r--r--   0 root         (0) root         (0)    13854 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/generic_error.py
+-rw-r--r--   0 root         (0) root         (0)    11491 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/get_version200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11595 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/health_not_ready_status.py
+-rw-r--r--   0 root         (0) root         (0)    11469 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/health_status.py
+-rw-r--r--   0 root         (0) root         (0)    17903 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/introspected_o_auth2_token.py
+-rw-r--r--   0 root         (0) root         (0)    11455 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/is_ready200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11589 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/is_ready503_response.py
+-rw-r--r--   0 root         (0) root         (0)    13268 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/json_patch.py
+-rw-r--r--   0 root         (0) root         (0)    11973 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/json_patch_document.py
+-rw-r--r--   0 root         (0) root         (0)    17879 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/json_web_key.py
+-rw-r--r--   0 root         (0) root         (0)    12231 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/json_web_key_set.py
+-rw-r--r--   0 root         (0) root         (0)    11777 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/null_duration.py
+-rw-r--r--   0 root         (0) root         (0)    38709 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/o_auth2_client.py
+-rw-r--r--   0 root         (0) root         (0)    15319 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/o_auth2_client_token_lifespans.py
+-rw-r--r--   0 root         (0) root         (0)    18380 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/o_auth2_consent_request.py
+-rw-r--r--   0 root         (0) root         (0)    18408 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/o_auth2_consent_request_open_id_connect_context.py
+-rw-r--r--   0 root         (0) root         (0)    14822 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/o_auth2_consent_session.py
+-rw-r--r--   0 root         (0) root         (0)    12423 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/o_auth2_consent_session_expires_at.py
+-rw-r--r--   0 root         (0) root         (0)    12114 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/o_auth2_consent_sessions.py
+-rw-r--r--   0 root         (0) root         (0)    17251 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/o_auth2_login_request.py
+-rw-r--r--   0 root         (0) root         (0)    13458 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/o_auth2_logout_request.py
+-rw-r--r--   0 root         (0) root         (0)    11760 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/o_auth2_redirect_to.py
+-rw-r--r--   0 root         (0) root         (0)    13444 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/o_auth2_token_exchange.py
+-rw-r--r--   0 root         (0) root         (0)    32243 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/oidc_configuration.py
+-rw-r--r--   0 root         (0) root         (0)    24504 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/oidc_user_info.py
+-rw-r--r--   0 root         (0) root         (0)    12744 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/pagination.py
+-rw-r--r--   0 root         (0) root         (0)    12101 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/pagination_headers.py
+-rw-r--r--   0 root         (0) root         (0)    13152 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/reject_o_auth2_request.py
+-rw-r--r--   0 root         (0) root         (0)    11698 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/string_slice_json_format.py
+-rw-r--r--   0 root         (0) root         (0)    12759 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/token_pagination.py
+-rw-r--r--   0 root         (0) root         (0)    12116 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/token_pagination_headers.py
+-rw-r--r--   0 root         (0) root         (0)    12809 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/token_pagination_request_parameters.py
+-rw-r--r--   0 root         (0) root         (0)    13024 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/token_pagination_response_headers.py
+-rw-r--r--   0 root         (0) root         (0)    13797 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/trust_o_auth2_jwt_grant_issuer.py
+-rw-r--r--   0 root         (0) root         (0)    14371 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/trusted_o_auth2_jwt_grant_issuer.py
+-rw-r--r--   0 root         (0) root         (0)    12284 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/trusted_o_auth2_jwt_grant_issuers.py
+-rw-r--r--   0 root         (0) root         (0)    11968 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/trusted_o_auth2_jwt_grant_json_web_key.py
+-rw-r--r--   0 root         (0) root         (0)    11465 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/ory_hydra_client/model/version.py
+-rw-r--r--   0 root         (0) root         (0)    82577 2023-04-11 10:57:25.000000 ory-hydra-client-2.1.1/ory_hydra_client/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:02:18.000000 ory-hydra-client-2.1.1/ory_hydra_client/models/
+-rw-r--r--   0 root         (0) root         (0)     3793 2023-04-11 10:57:25.000000 ory-hydra-client-2.1.1/ory_hydra_client/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14271 2023-04-11 10:57:25.000000 ory-hydra-client-2.1.1/ory_hydra_client/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:02:18.000000 ory-hydra-client-2.1.1/ory_hydra_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      368 2023-04-11 11:02:18.000000 ory-hydra-client-2.1.1/ory_hydra_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4561 2023-04-11 11:02:18.000000 ory-hydra-client-2.1.1/ory_hydra_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 11:02:18.000000 ory-hydra-client-2.1.1/ory_hydra_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-11 11:02:18.000000 ory-hydra-client-2.1.1/ory_hydra_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-11 11:02:18.000000 ory-hydra-client-2.1.1/ory_hydra_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-04-11 11:02:18.000000 ory-hydra-client-2.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-04-11 10:57:25.000000 ory-hydra-client-2.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:02:18.000000 ory-hydra-client-2.1.1/test/
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_accept_o_auth2_consent_request.py
+-rw-r--r--   0 root         (0) root         (0)      888 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_accept_o_auth2_consent_request_session.py
+-rw-r--r--   0 root         (0) root         (0)      965 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_accept_o_auth2_login_request.py
+-rw-r--r--   0 root         (0) root         (0)      789 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_create_json_web_key_set.py
+-rw-r--r--   0 root         (0) root         (0)      731 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_error_o_auth2.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_generic_error.py
+-rw-r--r--   0 root         (0) root         (0)      801 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_get_version200_response.py
+-rw-r--r--   0 root         (0) root         (0)      795 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_health_not_ready_status.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_health_status.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_introspected_o_auth2_token.py
+-rw-r--r--   0 root         (0) root         (0)      780 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_is_ready200_response.py
+-rw-r--r--   0 root         (0) root         (0)      780 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_is_ready503_response.py
+-rw-r--r--   0 root         (0) root         (0)      716 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_json_patch.py
+-rw-r--r--   0 root         (0) root         (0)      864 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_json_patch_document.py
+-rw-r--r--   0 root         (0) root         (0)      724 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_json_web_key.py
+-rw-r--r--   0 root         (0) root         (0)      842 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_json_web_key_set.py
+-rw-r--r--   0 root         (0) root         (0)     1636 2023-04-11 10:57:25.000000 ory-hydra-client-2.1.1/test/test_jwk_api.py
+-rw-r--r--   0 root         (0) root         (0)     1001 2023-04-11 10:57:25.000000 ory-hydra-client-2.1.1/test/test_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_null_duration.py
+-rw-r--r--   0 root         (0) root         (0)     5738 2023-04-11 10:57:25.000000 ory-hydra-client-2.1.1/test/test_o_auth2_api.py
+-rw-r--r--   0 root         (0) root         (0)      982 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_o_auth2_client.py
+-rw-r--r--   0 root         (0) root         (0)      941 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_o_auth2_client_token_lifespans.py
+-rw-r--r--   0 root         (0) root         (0)     1261 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_o_auth2_consent_request.py
+-rw-r--r--   0 root         (0) root         (0)      939 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_o_auth2_consent_request_open_id_connect_context.py
+-rw-r--r--   0 root         (0) root         (0)     1439 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_o_auth2_consent_session.py
+-rw-r--r--   0 root         (0) root         (0)      860 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_o_auth2_consent_session_expires_at.py
+-rw-r--r--   0 root         (0) root         (0)      939 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_o_auth2_consent_sessions.py
+-rw-r--r--   0 root         (0) root         (0)     1247 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_o_auth2_login_request.py
+-rw-r--r--   0 root         (0) root         (0)      892 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_o_auth2_logout_request.py
+-rw-r--r--   0 root         (0) root         (0)      767 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_o_auth2_redirect_to.py
+-rw-r--r--   0 root         (0) root         (0)      788 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_o_auth2_token_exchange.py
+-rw-r--r--   0 root         (0) root         (0)     1913 2023-04-11 10:57:25.000000 ory-hydra-client-2.1.1/test/test_oidc_api.py
+-rw-r--r--   0 root         (0) root         (0)      772 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_oidc_configuration.py
+-rw-r--r--   0 root         (0) root         (0)      738 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_oidc_user_info.py
+-rw-r--r--   0 root         (0) root         (0)      722 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_pagination.py
+-rw-r--r--   0 root         (0) root         (0)      772 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_pagination_headers.py
+-rw-r--r--   0 root         (0) root         (0)      788 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_reject_o_auth2_request.py
+-rw-r--r--   0 root         (0) root         (0)      802 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_string_slice_json_format.py
+-rw-r--r--   0 root         (0) root         (0)      758 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_token_pagination.py
+-rw-r--r--   0 root         (0) root         (0)      808 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_token_pagination_headers.py
+-rw-r--r--   0 root         (0) root         (0)      879 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_token_pagination_request_parameters.py
+-rw-r--r--   0 root         (0) root         (0)      865 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_token_pagination_response_headers.py
+-rw-r--r--   0 root         (0) root         (0)      928 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_trust_o_auth2_jwt_grant_issuer.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_trusted_o_auth2_jwt_grant_issuer.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_trusted_o_auth2_jwt_grant_issuers.py
+-rw-r--r--   0 root         (0) root         (0)      876 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_trusted_o_auth2_jwt_grant_json_web_key.py
+-rw-r--r--   0 root         (0) root         (0)      701 2023-04-11 10:57:24.000000 ory-hydra-client-2.1.1/test/test_version.py
+-rw-r--r--   0 root         (0) root         (0)      742 2023-04-11 10:57:25.000000 ory-hydra-client-2.1.1/test/test_wellknown_api.py
```

### Comparing `ory-hydra-client-2.1.0/LICENSE` & `ory-hydra-client-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ory-hydra-client-2.1.0/README.md` & `ory-hydra-client-2.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # ory-hydra-client
 Documentation for all of Ory Hydra's APIs.
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: v2.1.0
-- Package version: v2.1.0
+- API version: v2.1.1
+- Package version: v2.1.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python >=3.6
 
 ## Installation & Usage
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/__init__.py` & `ory-hydra-client-2.1.1/ory_hydra_client/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # flake8: noqa
 
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "v2.1.0"
+__version__ = "v2.1.1"
 
 # import ApiClient
 from ory_hydra_client.api_client import ApiClient
 
 # import Configuration
 from ory_hydra_client.configuration import Configuration
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/api/jwk_api.py` & `ory-hydra-client-2.1.1/ory_hydra_client/api/jwk_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/api/metadata_api.py` & `ory-hydra-client-2.1.1/ory_hydra_client/api/metadata_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/api/o_auth2_api.py` & `ory-hydra-client-2.1.1/ory_hydra_client/api/o_auth2_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/api/oidc_api.py` & `ory-hydra-client-2.1.1/ory_hydra_client/api/oidc_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/api/wellknown_api.py` & `ory-hydra-client-2.1.1/ory_hydra_client/api/wellknown_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/api_client.py` & `ory-hydra-client-2.1.1/ory_hydra_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/v2.1.0/python'
+        self.user_agent = 'OpenAPI-Generator/v2.1.1/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/apis/__init__.py` & `ory-hydra-client-2.1.1/ory_hydra_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/configuration.py` & `ory-hydra-client-2.1.1/ory_hydra_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import copy
 import logging
@@ -414,16 +414,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: v2.1.0\n"\
-               "SDK Package Version: v2.1.0".\
+               "Version of the API: v2.1.1\n"\
+               "SDK Package Version: v2.1.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/exceptions.py` & `ory-hydra-client-2.1.1/ory_hydra_client/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/accept_o_auth2_consent_request.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/accept_o_auth2_consent_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/accept_o_auth2_consent_request_session.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/accept_o_auth2_consent_request_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/accept_o_auth2_login_request.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/accept_o_auth2_login_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/create_json_web_key_set.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/create_json_web_key_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/error_o_auth2.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/error_o_auth2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/generic_error.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/generic_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/get_version200_response.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/get_version200_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/health_not_ready_status.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/health_not_ready_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/health_status.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/health_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/introspected_o_auth2_token.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/introspected_o_auth2_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/is_ready200_response.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/is_ready200_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/is_ready503_response.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/is_ready503_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/json_patch.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/json_patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/json_patch_document.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/json_patch_document.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/json_web_key.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/json_web_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/json_web_key_set.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/json_web_key_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/null_duration.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/null_duration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/o_auth2_client.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/o_auth2_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/o_auth2_client_token_lifespans.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/o_auth2_client_token_lifespans.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/o_auth2_consent_request.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/o_auth2_consent_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/o_auth2_consent_request_open_id_connect_context.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/o_auth2_consent_request_open_id_connect_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/o_auth2_consent_session.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/o_auth2_consent_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/o_auth2_consent_session_expires_at.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/o_auth2_consent_session_expires_at.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/o_auth2_consent_sessions.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/o_auth2_consent_sessions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/o_auth2_login_request.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/o_auth2_login_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/o_auth2_logout_request.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/o_auth2_logout_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/o_auth2_redirect_to.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/o_auth2_redirect_to.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/o_auth2_token_exchange.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/o_auth2_token_exchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/oidc_configuration.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/oidc_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/oidc_user_info.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/oidc_user_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/pagination.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/pagination.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/pagination_headers.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/pagination_headers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/reject_o_auth2_request.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/reject_o_auth2_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/string_slice_json_format.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/string_slice_json_format.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/token_pagination.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/token_pagination.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/token_pagination_headers.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/token_pagination_headers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/token_pagination_request_parameters.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/token_pagination_request_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/token_pagination_response_headers.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/token_pagination_response_headers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/trust_o_auth2_jwt_grant_issuer.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/trust_o_auth2_jwt_grant_issuer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/trusted_o_auth2_jwt_grant_issuer.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/trusted_o_auth2_jwt_grant_issuer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/trusted_o_auth2_jwt_grant_issuers.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/trusted_o_auth2_jwt_grant_issuers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/trusted_o_auth2_jwt_grant_json_web_key.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/trusted_o_auth2_jwt_grant_json_web_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model/version.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/model_utils.py` & `ory-hydra-client-2.1.1/ory_hydra_client/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/models/__init__.py` & `ory-hydra-client-2.1.1/ory_hydra_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client/rest.py` & `ory-hydra-client-2.1.1/ory_hydra_client/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
```

### Comparing `ory-hydra-client-2.1.0/ory_hydra_client.egg-info/SOURCES.txt` & `ory-hydra-client-2.1.1/ory_hydra_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ory-hydra-client-2.1.0/setup.py` & `ory-hydra-client-2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "ory-hydra-client"
-VERSION = "v2.1.0"
+VERSION = "v2.1.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `ory-hydra-client-2.1.0/test/test_accept_o_auth2_consent_request.py` & `ory-hydra-client-2.1.1/test/test_accept_o_auth2_consent_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_accept_o_auth2_consent_request_session.py` & `ory-hydra-client-2.1.1/test/test_accept_o_auth2_consent_request_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_accept_o_auth2_login_request.py` & `ory-hydra-client-2.1.1/test/test_accept_o_auth2_login_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_create_json_web_key_set.py` & `ory-hydra-client-2.1.1/test/test_create_json_web_key_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_error_o_auth2.py` & `ory-hydra-client-2.1.1/test/test_error_o_auth2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_generic_error.py` & `ory-hydra-client-2.1.1/test/test_generic_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_get_version200_response.py` & `ory-hydra-client-2.1.1/test/test_get_version200_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_health_not_ready_status.py` & `ory-hydra-client-2.1.1/test/test_health_not_ready_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_health_status.py` & `ory-hydra-client-2.1.1/test/test_oidc_user_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_hydra_client
-from ory_hydra_client.model.health_status import HealthStatus
+from ory_hydra_client.model.oidc_user_info import OidcUserInfo
 
 
-class TestHealthStatus(unittest.TestCase):
-    """HealthStatus unit test stubs"""
+class TestOidcUserInfo(unittest.TestCase):
+    """OidcUserInfo unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testHealthStatus(self):
-        """Test HealthStatus"""
+    def testOidcUserInfo(self):
+        """Test OidcUserInfo"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = HealthStatus()  # noqa: E501
+        # model = OidcUserInfo()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-hydra-client-2.1.0/test/test_introspected_o_auth2_token.py` & `ory-hydra-client-2.1.1/test/test_introspected_o_auth2_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_is_ready200_response.py` & `ory-hydra-client-2.1.1/test/test_is_ready200_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_is_ready503_response.py` & `ory-hydra-client-2.1.1/test/test_is_ready503_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_json_patch.py` & `ory-hydra-client-2.1.1/test/test_json_patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_json_patch_document.py` & `ory-hydra-client-2.1.1/test/test_json_patch_document.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_json_web_key.py` & `ory-hydra-client-2.1.1/test/test_json_web_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_json_web_key_set.py` & `ory-hydra-client-2.1.1/test/test_json_web_key_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_jwk_api.py` & `ory-hydra-client-2.1.1/test/test_jwk_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_metadata_api.py` & `ory-hydra-client-2.1.1/test/test_metadata_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_null_duration.py` & `ory-hydra-client-2.1.1/test/test_null_duration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_o_auth2_api.py` & `ory-hydra-client-2.1.1/test/test_o_auth2_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_o_auth2_client.py` & `ory-hydra-client-2.1.1/test/test_o_auth2_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_o_auth2_client_token_lifespans.py` & `ory-hydra-client-2.1.1/test/test_o_auth2_client_token_lifespans.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_o_auth2_consent_request.py` & `ory-hydra-client-2.1.1/test/test_o_auth2_consent_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_o_auth2_consent_request_open_id_connect_context.py` & `ory-hydra-client-2.1.1/test/test_o_auth2_consent_request_open_id_connect_context.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_o_auth2_consent_session.py` & `ory-hydra-client-2.1.1/test/test_o_auth2_consent_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_o_auth2_consent_session_expires_at.py` & `ory-hydra-client-2.1.1/test/test_o_auth2_consent_session_expires_at.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_o_auth2_consent_sessions.py` & `ory-hydra-client-2.1.1/test/test_o_auth2_consent_sessions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_o_auth2_login_request.py` & `ory-hydra-client-2.1.1/test/test_o_auth2_login_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_o_auth2_logout_request.py` & `ory-hydra-client-2.1.1/test/test_o_auth2_logout_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_o_auth2_redirect_to.py` & `ory-hydra-client-2.1.1/test/test_o_auth2_redirect_to.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_o_auth2_token_exchange.py` & `ory-hydra-client-2.1.1/test/test_o_auth2_token_exchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_oidc_api.py` & `ory-hydra-client-2.1.1/test/test_oidc_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_oidc_configuration.py` & `ory-hydra-client-2.1.1/test/test_oidc_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_oidc_user_info.py` & `ory-hydra-client-2.1.1/test/test_version.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_hydra_client
-from ory_hydra_client.model.oidc_user_info import OidcUserInfo
+from ory_hydra_client.model.version import Version
 
 
-class TestOidcUserInfo(unittest.TestCase):
-    """OidcUserInfo unit test stubs"""
+class TestVersion(unittest.TestCase):
+    """Version unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testOidcUserInfo(self):
-        """Test OidcUserInfo"""
+    def testVersion(self):
+        """Test Version"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = OidcUserInfo()  # noqa: E501
+        # model = Version()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-hydra-client-2.1.0/test/test_pagination.py` & `ory-hydra-client-2.1.1/test/test_pagination.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_pagination_headers.py` & `ory-hydra-client-2.1.1/test/test_pagination_headers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_reject_o_auth2_request.py` & `ory-hydra-client-2.1.1/test/test_reject_o_auth2_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_string_slice_json_format.py` & `ory-hydra-client-2.1.1/test/test_string_slice_json_format.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_token_pagination.py` & `ory-hydra-client-2.1.1/test/test_token_pagination.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_token_pagination_headers.py` & `ory-hydra-client-2.1.1/test/test_token_pagination_headers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_token_pagination_request_parameters.py` & `ory-hydra-client-2.1.1/test/test_token_pagination_request_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_token_pagination_response_headers.py` & `ory-hydra-client-2.1.1/test/test_token_pagination_response_headers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_trust_o_auth2_jwt_grant_issuer.py` & `ory-hydra-client-2.1.1/test/test_trust_o_auth2_jwt_grant_issuer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_trusted_o_auth2_jwt_grant_issuer.py` & `ory-hydra-client-2.1.1/test/test_trusted_o_auth2_jwt_grant_issuer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_trusted_o_auth2_jwt_grant_issuers.py` & `ory-hydra-client-2.1.1/test/test_trusted_o_auth2_jwt_grant_issuers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_trusted_o_auth2_jwt_grant_json_web_key.py` & `ory-hydra-client-2.1.1/test/test_trusted_o_auth2_jwt_grant_json_web_key.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-hydra-client-2.1.0/test/test_version.py` & `ory-hydra-client-2.1.1/test/test_health_status.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_hydra_client
-from ory_hydra_client.model.version import Version
+from ory_hydra_client.model.health_status import HealthStatus
 
 
-class TestVersion(unittest.TestCase):
-    """Version unit test stubs"""
+class TestHealthStatus(unittest.TestCase):
+    """HealthStatus unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testVersion(self):
-        """Test Version"""
+    def testHealthStatus(self):
+        """Test HealthStatus"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = Version()  # noqa: E501
+        # model = HealthStatus()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-hydra-client-2.1.0/test/test_wellknown_api.py` & `ory-hydra-client-2.1.1/test/test_wellknown_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory Hydra API
 
     Documentation for all of Ory Hydra's APIs.   # noqa: E501
 
-    The version of the OpenAPI document: v2.1.0
+    The version of the OpenAPI document: v2.1.1
     Contact: hi@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

