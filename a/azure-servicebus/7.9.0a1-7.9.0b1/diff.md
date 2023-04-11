# Comparing `tmp/azure-servicebus-7.9.0a1.zip` & `tmp/azure-servicebus-7.9.0b1.zip`

## zipinfo {}

```diff
@@ -1,245 +1,243 @@
-Zip file size: 571133 bytes, number of entries: 243
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-11 18:36 azure-servicebus-7.9.0a1/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-11 18:36 azure-servicebus-7.9.0a1/azure_servicebus.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-11 18:36 azure-servicebus-7.9.0a1/tests/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-11 18:36 azure-servicebus-7.9.0a1/samples/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-11 18:36 azure-servicebus-7.9.0a1/azure/
--rw-rw-r--  2.0 unx      149 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/MANIFEST.in
--rw-rw-r--  2.0 unx    41984 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/CHANGELOG.md
--rw-rw-r--  2.0 unx    78920 b- defN 22-Oct-11 18:36 azure-servicebus-7.9.0a1/PKG-INFO
--rw-rw-r--  2.0 unx     2440 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/setup.py
--rw-rw-r--  2.0 unx    21799 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/migration_guide.md
--rw-rw-r--  2.0 unx     1073 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/LICENSE
--rw-rw-r--  2.0 unx    36180 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/README.md
--rw-rw-r--  2.0 unx       38 b- defN 22-Oct-11 18:36 azure-servicebus-7.9.0a1/setup.cfg
--rw-rw-r--  2.0 unx     9934 b- defN 22-Oct-11 18:36 azure-servicebus-7.9.0a1/azure_servicebus.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx        1 b- defN 22-Oct-11 18:36 azure-servicebus-7.9.0a1/azure_servicebus.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx        1 b- defN 22-Oct-11 18:36 azure-servicebus-7.9.0a1/azure_servicebus.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx    78920 b- defN 22-Oct-11 18:36 azure-servicebus-7.9.0a1/azure_servicebus.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx      120 b- defN 22-Oct-11 18:36 azure-servicebus-7.9.0a1/azure_servicebus.egg-info/requires.txt
--rw-rw-r--  2.0 unx        6 b- defN 22-Oct-11 18:36 azure-servicebus-7.9.0a1/azure_servicebus.egg-info/top_level.txt
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-11 18:36 azure-servicebus-7.9.0a1/tests/livetest/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-11 18:36 azure-servicebus-7.9.0a1/tests/async_tests/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-11 18:36 azure-servicebus-7.9.0a1/tests/perf_tests/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-11 18:36 azure-servicebus-7.9.0a1/tests/mgmt_tests/
--rw-rw-r--  2.0 unx     7017 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/test_connection_string_parser.py
--rw-rw-r--  2.0 unx     2027 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/utilities.py
--rw-rw-r--  2.0 unx    25718 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/servicebus_preparer.py
--rw-rw-r--  2.0 unx    64416 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/test_sessions.py
--rw-rw-r--  2.0 unx    36354 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/test_message.py
--rw-rw-r--  2.0 unx    30056 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/test_sb_client.py
--rw-rw-r--  2.0 unx     3653 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/test_topic.py
--rw-rw-r--  2.0 unx   147762 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/test_queues.py
--rw-rw-r--  2.0 unx     1494 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/mocks.py
--rw-rw-r--  2.0 unx      921 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/sb_env_loader.py
--rw-rw-r--  2.0 unx     8986 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/test_subscriptions.py
--rw-rw-r--  2.0 unx     1799 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/livetest/test_errors.py
--rw-rw-r--  2.0 unx     8112 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/async_tests/test_subscriptions_async.py
--rw-rw-r--  2.0 unx    29127 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/async_tests/test_sb_client_async.py
--rw-rw-r--  2.0 unx    58688 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/async_tests/test_sessions_async.py
--rw-rw-r--  2.0 unx     2895 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/async_tests/test_topic_async.py
--rw-rw-r--  2.0 unx     1423 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/async_tests/mocks_async.py
--rw-rw-r--  2.0 unx   131305 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/async_tests/test_queues_async.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-11 18:36 azure-servicebus-7.9.0a1/tests/perf_tests/T1_legacy_tests/
--rw-rw-r--  2.0 unx     5900 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/perf_tests/_test_base.py
--rw-rw-r--  2.0 unx     1340 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/perf_tests/receive_message_stream.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/perf_tests/__init__.py
--rw-rw-r--  2.0 unx      906 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/perf_tests/send_message.py
--rw-rw-r--  2.0 unx     1674 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/perf_tests/send_message_batch.py
--rw-rw-r--  2.0 unx     1324 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/perf_tests/receive_message_batch.py
--rw-rw-r--  2.0 unx     6664 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/perf_tests/T1_legacy_tests/_test_base.py
--rw-rw-r--  2.0 unx     1299 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/perf_tests/T1_legacy_tests/receive_message_stream.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/perf_tests/T1_legacy_tests/__init__.py
--rw-rw-r--  2.0 unx      927 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/perf_tests/T1_legacy_tests/send_message.py
--rw-rw-r--  2.0 unx     1015 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/perf_tests/T1_legacy_tests/send_message_batch.py
--rw-rw-r--  2.0 unx     1104 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/perf_tests/T1_legacy_tests/receive_message_batch.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-11 18:36 azure-servicebus-7.9.0a1/tests/mgmt_tests/async/
--rw-rw-r--  2.0 unx     4585 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/mgmt_tests/mgmt_test_utilities.py
--rw-rw-r--  2.0 unx    16871 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/mgmt_tests/test_mgmt_rules.py
--rw-rw-r--  2.0 unx    42948 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/mgmt_tests/test_mgmt_queues.py
--rw-rw-r--  2.0 unx    28339 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/mgmt_tests/test_mgmt_subscriptions.py
--rw-rw-r--  2.0 unx    25789 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/mgmt_tests/test_mgmt_topics.py
--rw-rw-r--  2.0 unx     1349 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/mgmt_tests/test_mgmt_namespaces.py
--rw-rw-r--  2.0 unx    26493 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/mgmt_tests/async/test_mgmt_topics_async.py
--rw-rw-r--  2.0 unx    43461 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/mgmt_tests/async/test_mgmt_queues_async.py
--rw-rw-r--  2.0 unx    17182 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/mgmt_tests/async/test_mgmt_rules_async.py
--rw-rw-r--  2.0 unx     5115 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/mgmt_tests/async/mgmt_test_utilities_async.py
--rw-rw-r--  2.0 unx     1394 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/mgmt_tests/async/test_mgmt_namespaces_async.py
--rw-rw-r--  2.0 unx    29536 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/tests/mgmt_tests/async/test_mgmt_subscriptions_async.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-11 18:36 azure-servicebus-7.9.0a1/samples/async_samples/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-11 18:36 azure-servicebus-7.9.0a1/samples/sync_samples/
--rw-rw-r--  2.0 unx     3912 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/async_samples/mgmt_rule_async.py
--rw-rw-r--  2.0 unx     2045 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/async_samples/receive_deferred_message_queue_async.py
--rw-rw-r--  2.0 unx     5456 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/async_samples/deadletter_messages_and_correct_async.py
--rw-rw-r--  2.0 unx     1491 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/async_samples/proxy_async.py
--rw-rw-r--  2.0 unx     1889 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/async_samples/send_queue_async.py
--rw-rw-r--  2.0 unx     1063 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/async_samples/receive_peek_async.py
--rw-rw-r--  2.0 unx     3263 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/async_samples/session_pool_receive_async.py
--rw-rw-r--  2.0 unx     2112 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/async_samples/authenticate_using_azure_sas_credential_async.py
--rw-rw-r--  2.0 unx     3266 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/async_samples/client_identity_authentication_async.py
--rw-rw-r--  2.0 unx     1064 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/async_samples/receive_iterator_queue_async.py
--rw-rw-r--  2.0 unx     3478 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/async_samples/mgmt_subscription_async.py
--rw-rw-r--  2.0 unx     1307 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/async_samples/receive_subscription_async.py
--rw-rw-r--  2.0 unx     1298 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/async_samples/authenticate_client_connstr_async.py
--rw-rw-r--  2.0 unx     1929 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/async_samples/connection_to_custom_endpoint_address_async.py
--rw-rw-r--  2.0 unx     3600 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/async_samples/send_and_receive_amqp_annotated_message_async.py
--rw-rw-r--  2.0 unx     1860 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/async_samples/send_topic_async.py
--rw-rw-r--  2.0 unx     2413 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/async_samples/schedule_topic_messages_and_cancellation_async.py
--rw-rw-r--  2.0 unx     2259 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/async_samples/schedule_messages_and_cancellation_async.py
--rw-rw-r--  2.0 unx     3077 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/async_samples/mgmt_topic_async.py
--rw-rw-r--  2.0 unx     3838 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/async_samples/mgmt_queue_async.py
--rw-rw-r--  2.0 unx     1200 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/async_samples/authenticate_using_azure_named_key_credential_async.py
--rw-rw-r--  2.0 unx    16236 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/async_samples/sample_code_servicebus_async.py
--rw-rw-r--  2.0 unx     1138 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/async_samples/receive_queue_async.py
--rw-rw-r--  2.0 unx     2076 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/async_samples/receive_deadlettered_messages_async.py
--rw-rw-r--  2.0 unx     8793 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/async_samples/topic_subscription_with_rule_operations_async.py
--rw-rw-r--  2.0 unx     6298 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/async_samples/auto_lock_renew_async.py
--rw-rw-r--  2.0 unx     2818 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/async_samples/session_send_receive_async.py
--rw-rw-r--  2.0 unx     3724 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/sync_samples/mgmt_rule.py
--rw-rw-r--  2.0 unx     1725 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/sync_samples/receive_deadlettered_messages.py
--rw-rw-r--  2.0 unx     2431 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/sync_samples/generate_sas_token_and_authenticate_client.py
--rw-rw-r--  2.0 unx     1228 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/sync_samples/authenticate_client_connstr.py
--rw-rw-r--  2.0 unx     2631 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/sync_samples/session_send_receive.py
--rw-rw-r--  2.0 unx     1782 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/sync_samples/connection_to_custom_endpoint_address.py
--rw-rw-r--  2.0 unx     7463 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/sync_samples/failure_and_recovery.py
--rw-rw-r--  2.0 unx    16632 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/sync_samples/sample_code_servicebus.py
--rw-rw-r--  2.0 unx     3378 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/sync_samples/client_identity_authentication.py
--rw-rw-r--  2.0 unx     5142 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/sync_samples/deadletter_messages_and_correct.py
--rw-rw-r--  2.0 unx     1191 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/sync_samples/receive_subscription.py
--rw-rw-r--  2.0 unx     3628 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/sync_samples/mgmt_queue.py
--rw-rw-r--  2.0 unx     1069 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/sync_samples/authenticate_using_azure_named_key_credential.py
--rw-rw-r--  2.0 unx     6097 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/sync_samples/auto_lock_renew.py
--rw-rw-r--  2.0 unx     1950 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/sync_samples/authenticate_using_azure_sas_credential.py
--rw-rw-r--  2.0 unx     1701 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/sync_samples/send_topic.py
--rw-rw-r--  2.0 unx     3400 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/sync_samples/send_and_receive_amqp_annotated_message.py
--rw-rw-r--  2.0 unx     8389 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/sync_samples/topic_subscription_with_rule_operations.py
--rw-rw-r--  2.0 unx     1323 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/sync_samples/proxy.py
--rw-rw-r--  2.0 unx     1802 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/sync_samples/receive_deferred_message_queue.py
--rw-rw-r--  2.0 unx      969 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/sync_samples/receive_peek.py
--rw-rw-r--  2.0 unx     1034 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/sync_samples/receive_queue.py
--rw-rw-r--  2.0 unx     3284 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/sync_samples/mgmt_subscription.py
--rw-rw-r--  2.0 unx     2303 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/sync_samples/schedule_topic_messages_and_cancellation.py
--rw-rw-r--  2.0 unx      934 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/sync_samples/receive_iterator_queue.py
--rw-rw-r--  2.0 unx     3440 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/sync_samples/session_pool_receive.py
--rw-rw-r--  2.0 unx     1704 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/sync_samples/send_queue.py
--rw-rw-r--  2.0 unx     2881 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/sync_samples/mgmt_topic.py
--rw-rw-r--  2.0 unx     2043 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/samples/sync_samples/schedule_messages_and_cancellation.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-11 18:36 azure-servicebus-7.9.0a1/azure/servicebus/
--rw-rw-r--  2.0 unx       84 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-11 18:36 azure-servicebus-7.9.0a1/azure/servicebus/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-11 18:36 azure-servicebus-7.9.0a1/azure/servicebus/amqp/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-11 18:36 azure-servicebus-7.9.0a1/azure/servicebus/management/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-11 18:36 azure-servicebus-7.9.0a1/azure/servicebus/_common/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-11 18:36 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/
--rw-rw-r--  2.0 unx     8185 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_servicebus_session.py
--rw-rw-r--  2.0 unx    22605 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_base_handler.py
--rw-rw-r--  2.0 unx    30774 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_servicebus_client.py
--rw-rw-r--  2.0 unx      172 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_version.py
--rw-rw-r--  2.0 unx    16566 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/exceptions.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/py.typed
--rw-rw-r--  2.0 unx    22858 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_servicebus_sender.py
--rw-rw-r--  2.0 unx     1567 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/__init__.py
--rw-rw-r--  2.0 unx    48932 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_servicebus_receiver.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-11 18:36 azure-servicebus-7.9.0a1/azure/servicebus/aio/management/
--rw-rw-r--  2.0 unx    30969 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/aio/_servicebus_client_async.py
--rw-rw-r--  2.0 unx    16044 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/aio/_base_handler_async.py
--rw-rw-r--  2.0 unx     6735 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/aio/_servicebus_session_async.py
--rw-rw-r--  2.0 unx      725 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/aio/__init__.py
--rw-rw-r--  2.0 unx     2607 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/aio/_async_utils.py
--rw-rw-r--  2.0 unx    10538 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/aio/_async_auto_lock_renewer.py
--rw-rw-r--  2.0 unx    48797 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/aio/_servicebus_receiver_async.py
--rw-rw-r--  2.0 unx    20528 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/aio/_servicebus_sender_async.py
--rw-rw-r--  2.0 unx    57740 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/aio/management/_management_client_async.py
--rw-rw-r--  2.0 unx      468 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/aio/management/__init__.py
--rw-rw-r--  2.0 unx     1674 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/aio/management/_shared_key_policy_async.py
--rw-rw-r--  2.0 unx     6609 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/aio/management/_utils.py
--rw-rw-r--  2.0 unx      516 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/amqp/_constants.py
--rw-rw-r--  2.0 unx      567 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/amqp/__init__.py
--rw-rw-r--  2.0 unx    28997 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/amqp/_amqp_message.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-11 18:36 azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/
--rw-rw-r--  2.0 unx      570 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/management/_api_version.py
--rw-rw-r--  2.0 unx      893 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/management/_handle_response_error.py
--rw-rw-r--  2.0 unx    56838 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/management/_models.py
--rw-rw-r--  2.0 unx     1819 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/management/_xml_workaround_policy.py
--rw-rw-r--  2.0 unx     2056 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/management/_constants.py
--rw-rw-r--  2.0 unx     1543 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/management/__init__.py
--rw-rw-r--  2.0 unx     2050 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/management/_shared_key_policy.py
--rw-rw-r--  2.0 unx    57663 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/management/_management_client.py
--rw-rw-r--  2.0 unx     9516 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/management/_model_workaround.py
--rw-rw-r--  2.0 unx    14441 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/management/_utils.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-11 18:36 azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-11 18:36 azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-11 18:36 azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/models/
--rw-rw-r--  2.0 unx     2379 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/_configuration.py
--rw-rw-r--  2.0 unx     3312 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/_service_bus_management_client.py
--rw-rw-r--  2.0 unx      488 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/_version.py
--rw-rw-r--  2.0 unx      718 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-11 18:36 azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/aio/operations_async/
--rw-rw-r--  2.0 unx      586 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/aio/__init__.py
--rw-rw-r--  2.0 unx     3233 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/aio/_service_bus_management_client_async.py
--rw-rw-r--  2.0 unx     2212 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/aio/_configuration_async.py
--rw-rw-r--  2.0 unx     9771 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/aio/operations_async/_service_bus_management_client_operations_async.py
--rw-rw-r--  2.0 unx    11284 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/aio/operations_async/_subscription_operations_async.py
--rw-rw-r--  2.0 unx      972 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/aio/operations_async/__init__.py
--rw-rw-r--  2.0 unx     4092 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/aio/operations_async/_namespace_operations_async.py
--rw-rw-r--  2.0 unx    10652 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/aio/operations_async/_entity_operations_async.py
--rw-rw-r--  2.0 unx    11874 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/aio/operations_async/_rule_operations_async.py
--rw-rw-r--  2.0 unx      942 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/operations/__init__.py
--rw-rw-r--  2.0 unx     4222 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/operations/_namespace_operations.py
--rw-rw-r--  2.0 unx    10884 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/operations/_entity_operations.py
--rw-rw-r--  2.0 unx    12154 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/operations/_rule_operations.py
--rw-rw-r--  2.0 unx    10041 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/operations/_service_bus_management_client_operations.py
--rw-rw-r--  2.0 unx    11540 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/operations/_subscription_operations.py
--rw-rw-r--  2.0 unx    85085 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/models/_models.py
--rw-rw-r--  2.0 unx    92759 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/models/_models_py3.py
--rw-rw-r--  2.0 unx     6438 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/models/__init__.py
--rw-rw-r--  2.0 unx     1578 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/models/_service_bus_management_client_enums.py
--rw-rw-r--  2.0 unx     3053 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_common/_configuration.py
--rw-rw-r--  2.0 unx    11469 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_common/utils.py
--rw-rw-r--  2.0 unx    15178 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_common/auto_lock_renewer.py
--rw-rw-r--  2.0 unx      308 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_common/__init__.py
--rw-rw-r--  2.0 unx     5757 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_common/receiver_mixins.py
--rw-rw-r--  2.0 unx     7868 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_common/constants.py
--rw-rw-r--  2.0 unx    44212 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_common/message.py
--rw-rw-r--  2.0 unx     3049 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_common/_connection_string_parser.py
--rw-rw-r--  2.0 unx     4372 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_common/mgmt_handlers.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Oct-11 18:36 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/
--rw-rw-r--  2.0 unx     2119 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/types.py
--rw-rw-r--  2.0 unx    27361 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/_transport.py
--rw-rw-r--  2.0 unx     4671 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/management_operation.py
--rw-rw-r--  2.0 unx     3045 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/_platform.py
--rw-rw-r--  2.0 unx    16870 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/endpoints.py
--rw-rw-r--  2.0 unx    37291 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/_connection.py
--rw-rw-r--  2.0 unx     3836 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/utils.py
--rw-rw-r--  2.0 unx    19766 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/session.py
--rw-rw-r--  2.0 unx     8480 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/_message_backcompat.py
--rw-rw-r--  2.0 unx     8261 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/sender.py
--rw-rw-r--  2.0 unx      578 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/__init__.py
--rw-rw-r--  2.0 unx    44924 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/client.py
--rw-rw-r--  2.0 unx     5150 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/receiver.py
--rw-rw-r--  2.0 unx    11746 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/management_link.py
--rw-rw-r--  2.0 unx    11706 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/constants.py
--rw-rw-r--  2.0 unx    11453 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/link.py
--rw-rw-r--  2.0 unx    14807 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/error.py
--rw-rw-r--  2.0 unx     5851 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/authentication.py
--rw-rw-r--  2.0 unx    10685 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/cbs.py
--rw-rw-r--  2.0 unx    35488 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/_encode.py
--rw-rw-r--  2.0 unx    17497 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/message.py
--rw-rw-r--  2.0 unx    40120 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/performatives.py
--rw-rw-r--  2.0 unx    10461 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/outcomes.py
--rw-rw-r--  2.0 unx     4293 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/sasl.py
--rw-rw-r--  2.0 unx    11523 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/_decode.py
--rw-rw-r--  2.0 unx     2395 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_authentication_async.py
--rw-rw-r--  2.0 unx     8566 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_sender_async.py
--rw-rw-r--  2.0 unx     1185 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/__init__.py
--rw-rw-r--  2.0 unx    37799 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_connection_async.py
--rw-rw-r--  2.0 unx    20564 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_session_async.py
--rw-rw-r--  2.0 unx    42626 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_client_async.py
--rw-rw-r--  2.0 unx    11652 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_management_link_async.py
--rw-rw-r--  2.0 unx     4607 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_sasl_async.py
--rw-rw-r--  2.0 unx    11704 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_link_async.py
--rw-rw-r--  2.0 unx     9868 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_cbs_async.py
--rw-rw-r--  2.0 unx    20859 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_transport_async.py
--rw-rw-r--  2.0 unx     5288 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_receiver_async.py
--rw-rw-r--  2.0 unx     4748 b- defN 22-Oct-11 18:35 azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_management_operation_async.py
-243 files, 2757961 bytes uncompressed, 519721 bytes compressed:  81.2%
+Zip file size: 573982 bytes, number of entries: 241
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-10 01:31 azure-servicebus-7.9.0b1/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-10 01:31 azure-servicebus-7.9.0b1/azure_servicebus.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-10 01:31 azure-servicebus-7.9.0b1/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-10 01:31 azure-servicebus-7.9.0b1/samples/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-10 01:31 azure-servicebus-7.9.0b1/tests/
+-rw-rw-r--  2.0 unx     2489 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/setup.py
+-rw-rw-r--  2.0 unx    36189 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/README.md
+-rw-rw-r--  2.0 unx       38 b- defN 23-Mar-10 01:31 azure-servicebus-7.9.0b1/setup.cfg
+-rw-rw-r--  2.0 unx    21799 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/migration_guide.md
+-rw-rw-r--  2.0 unx       86 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/pyproject.toml
+-rw-rw-r--  2.0 unx      149 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/MANIFEST.in
+-rw-rw-r--  2.0 unx     1073 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/LICENSE
+-rw-rw-r--  2.0 unx    79514 b- defN 23-Mar-10 01:31 azure-servicebus-7.9.0b1/PKG-INFO
+-rw-rw-r--  2.0 unx    42519 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/CHANGELOG.md
+-rw-rw-r--  2.0 unx        1 b- defN 23-Mar-10 01:31 azure-servicebus-7.9.0b1/azure_servicebus.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx        6 b- defN 23-Mar-10 01:31 azure-servicebus-7.9.0b1/azure_servicebus.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Mar-10 01:31 azure-servicebus-7.9.0b1/azure_servicebus.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx     9855 b- defN 23-Mar-10 01:31 azure-servicebus-7.9.0b1/azure_servicebus.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx    79514 b- defN 23-Mar-10 01:31 azure-servicebus-7.9.0b1/azure_servicebus.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx      120 b- defN 23-Mar-10 01:31 azure-servicebus-7.9.0b1/azure_servicebus.egg-info/requires.txt
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-10 01:31 azure-servicebus-7.9.0b1/azure/servicebus/
+-rw-rw-r--  2.0 unx       84 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-10 01:31 azure-servicebus-7.9.0b1/azure/servicebus/_common/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-10 01:31 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-10 01:31 azure-servicebus-7.9.0b1/azure/servicebus/amqp/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-10 01:31 azure-servicebus-7.9.0b1/azure/servicebus/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-10 01:31 azure-servicebus-7.9.0b1/azure/servicebus/management/
+-rw-rw-r--  2.0 unx    22634 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_base_handler.py
+-rw-rw-r--  2.0 unx     1567 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/__init__.py
+-rw-rw-r--  2.0 unx    30774 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_servicebus_client.py
+-rw-rw-r--  2.0 unx    48272 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_servicebus_receiver.py
+-rw-rw-r--  2.0 unx     8257 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_servicebus_session.py
+-rw-rw-r--  2.0 unx    16566 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/exceptions.py
+-rw-rw-r--  2.0 unx      172 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_version.py
+-rw-rw-r--  2.0 unx    23115 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_servicebus_sender.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/py.typed
+-rw-rw-r--  2.0 unx      308 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_common/__init__.py
+-rw-rw-r--  2.0 unx     3053 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_common/_configuration.py
+-rw-rw-r--  2.0 unx     7868 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_common/constants.py
+-rw-rw-r--  2.0 unx     3049 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_common/_connection_string_parser.py
+-rw-rw-r--  2.0 unx     4372 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_common/mgmt_handlers.py
+-rw-rw-r--  2.0 unx    11486 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_common/utils.py
+-rw-rw-r--  2.0 unx    44186 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_common/message.py
+-rw-rw-r--  2.0 unx    15178 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_common/auto_lock_renewer.py
+-rw-rw-r--  2.0 unx     6153 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_common/receiver_mixins.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-10 01:31 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/
+-rw-rw-r--  2.0 unx    35509 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/_encode.py
+-rw-rw-r--  2.0 unx    11560 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/link.py
+-rw-rw-r--  2.0 unx     5855 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/authentication.py
+-rw-rw-r--  2.0 unx      578 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/__init__.py
+-rw-rw-r--  2.0 unx    14807 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/error.py
+-rw-rw-r--  2.0 unx    11170 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/cbs.py
+-rw-rw-r--  2.0 unx     3045 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/_platform.py
+-rw-rw-r--  2.0 unx    48794 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/client.py
+-rw-rw-r--  2.0 unx     5126 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/receiver.py
+-rw-rw-r--  2.0 unx    12126 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/management_link.py
+-rw-rw-r--  2.0 unx     2119 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/types.py
+-rw-rw-r--  2.0 unx    21793 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/session.py
+-rw-rw-r--  2.0 unx    11821 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/constants.py
+-rw-rw-r--  2.0 unx     4833 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/management_operation.py
+-rw-rw-r--  2.0 unx     8480 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/_message_backcompat.py
+-rw-rw-r--  2.0 unx     8369 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/sender.py
+-rw-rw-r--  2.0 unx    11523 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/_decode.py
+-rw-rw-r--  2.0 unx    38701 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/_connection.py
+-rw-rw-r--  2.0 unx    40120 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/performatives.py
+-rw-rw-r--  2.0 unx     4293 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/sasl.py
+-rw-rw-r--  2.0 unx    30989 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/_transport.py
+-rw-rw-r--  2.0 unx     3815 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/utils.py
+-rw-rw-r--  2.0 unx    10461 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/outcomes.py
+-rw-rw-r--  2.0 unx    17497 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/message.py
+-rw-rw-r--  2.0 unx    16870 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/endpoints.py
+-rw-rw-r--  2.0 unx    24604 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_transport_async.py
+-rw-rw-r--  2.0 unx    38885 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_connection_async.py
+-rw-rw-r--  2.0 unx    11811 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_link_async.py
+-rw-rw-r--  2.0 unx     1185 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/__init__.py
+-rw-rw-r--  2.0 unx    45083 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_client_async.py
+-rw-rw-r--  2.0 unx     4607 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_sasl_async.py
+-rw-rw-r--  2.0 unx    21551 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_session_async.py
+-rw-rw-r--  2.0 unx     8671 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_sender_async.py
+-rw-rw-r--  2.0 unx     2395 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_authentication_async.py
+-rw-rw-r--  2.0 unx     5264 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_receiver_async.py
+-rw-rw-r--  2.0 unx    12030 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_management_link_async.py
+-rw-rw-r--  2.0 unx     4910 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_management_operation_async.py
+-rw-rw-r--  2.0 unx    10649 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_cbs_async.py
+-rw-rw-r--  2.0 unx    28997 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/amqp/_amqp_message.py
+-rw-rw-r--  2.0 unx      567 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/amqp/__init__.py
+-rw-rw-r--  2.0 unx      516 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/amqp/_constants.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-10 01:31 azure-servicebus-7.9.0b1/azure/servicebus/aio/management/
+-rw-rw-r--  2.0 unx      725 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/aio/__init__.py
+-rw-rw-r--  2.0 unx    47811 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/aio/_servicebus_receiver_async.py
+-rw-rw-r--  2.0 unx    16038 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/aio/_base_handler_async.py
+-rw-rw-r--  2.0 unx    10538 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/aio/_async_auto_lock_renewer.py
+-rw-rw-r--  2.0 unx    20522 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/aio/_servicebus_sender_async.py
+-rw-rw-r--  2.0 unx    30969 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/aio/_servicebus_client_async.py
+-rw-rw-r--  2.0 unx     2607 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/aio/_async_utils.py
+-rw-rw-r--  2.0 unx     6735 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/aio/_servicebus_session_async.py
+-rw-rw-r--  2.0 unx      468 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/aio/management/__init__.py
+-rw-rw-r--  2.0 unx     6609 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/aio/management/_utils.py
+-rw-rw-r--  2.0 unx    57740 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/aio/management/_management_client_async.py
+-rw-rw-r--  2.0 unx     1674 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/aio/management/_shared_key_policy_async.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-10 01:31 azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/
+-rw-rw-r--  2.0 unx     1543 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/management/__init__.py
+-rw-rw-r--  2.0 unx    56838 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/management/_models.py
+-rw-rw-r--  2.0 unx     9516 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/management/_model_workaround.py
+-rw-rw-r--  2.0 unx    14441 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/management/_utils.py
+-rw-rw-r--  2.0 unx      893 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/management/_handle_response_error.py
+-rw-rw-r--  2.0 unx    57663 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/management/_management_client.py
+-rw-rw-r--  2.0 unx     1819 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/management/_xml_workaround_policy.py
+-rw-rw-r--  2.0 unx      570 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/management/_api_version.py
+-rw-rw-r--  2.0 unx     2050 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/management/_shared_key_policy.py
+-rw-rw-r--  2.0 unx     2056 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/management/_constants.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-10 01:31 azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-10 01:31 azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-10 01:31 azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/aio/
+-rw-rw-r--  2.0 unx      718 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/__init__.py
+-rw-rw-r--  2.0 unx     2379 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/_configuration.py
+-rw-rw-r--  2.0 unx      488 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/_version.py
+-rw-rw-r--  2.0 unx     3312 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/_service_bus_management_client.py
+-rw-rw-r--  2.0 unx     1578 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/models/_service_bus_management_client_enums.py
+-rw-rw-r--  2.0 unx     6438 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/models/__init__.py
+-rw-rw-r--  2.0 unx    85085 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/models/_models.py
+-rw-rw-r--  2.0 unx    92759 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/models/_models_py3.py
+-rw-rw-r--  2.0 unx    10884 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/operations/_entity_operations.py
+-rw-rw-r--  2.0 unx      942 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/operations/__init__.py
+-rw-rw-r--  2.0 unx    10041 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/operations/_service_bus_management_client_operations.py
+-rw-rw-r--  2.0 unx    12154 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/operations/_rule_operations.py
+-rw-rw-r--  2.0 unx     4222 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/operations/_namespace_operations.py
+-rw-rw-r--  2.0 unx    11540 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/operations/_subscription_operations.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-10 01:31 azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/aio/operations_async/
+-rw-rw-r--  2.0 unx      586 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/aio/__init__.py
+-rw-rw-r--  2.0 unx     3233 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/aio/_service_bus_management_client_async.py
+-rw-rw-r--  2.0 unx     2212 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/aio/_configuration_async.py
+-rw-rw-r--  2.0 unx      972 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/aio/operations_async/__init__.py
+-rw-rw-r--  2.0 unx    11874 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/aio/operations_async/_rule_operations_async.py
+-rw-rw-r--  2.0 unx    10652 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/aio/operations_async/_entity_operations_async.py
+-rw-rw-r--  2.0 unx     9771 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/aio/operations_async/_service_bus_management_client_operations_async.py
+-rw-rw-r--  2.0 unx     4092 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/aio/operations_async/_namespace_operations_async.py
+-rw-rw-r--  2.0 unx    11284 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/aio/operations_async/_subscription_operations_async.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-10 01:31 azure-servicebus-7.9.0b1/samples/sync_samples/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-10 01:31 azure-servicebus-7.9.0b1/samples/async_samples/
+-rw-rw-r--  2.0 unx     1802 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/sync_samples/receive_deferred_message_queue.py
+-rw-rw-r--  2.0 unx     1701 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/sync_samples/send_topic.py
+-rw-rw-r--  2.0 unx     3440 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/sync_samples/session_pool_receive.py
+-rw-rw-r--  2.0 unx     2303 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/sync_samples/schedule_topic_messages_and_cancellation.py
+-rw-rw-r--  2.0 unx     1191 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/sync_samples/receive_subscription.py
+-rw-rw-r--  2.0 unx     3400 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/sync_samples/send_and_receive_amqp_annotated_message.py
+-rw-rw-r--  2.0 unx     3284 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/sync_samples/mgmt_subscription.py
+-rw-rw-r--  2.0 unx     1034 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/sync_samples/receive_queue.py
+-rw-rw-r--  2.0 unx     5142 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/sync_samples/deadletter_messages_and_correct.py
+-rw-rw-r--  2.0 unx     1323 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/sync_samples/proxy.py
+-rw-rw-r--  2.0 unx     1782 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/sync_samples/connection_to_custom_endpoint_address.py
+-rw-rw-r--  2.0 unx     3378 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/sync_samples/client_identity_authentication.py
+-rw-rw-r--  2.0 unx     1725 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/sync_samples/receive_deadlettered_messages.py
+-rw-rw-r--  2.0 unx     1950 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/sync_samples/authenticate_using_azure_sas_credential.py
+-rw-rw-r--  2.0 unx      934 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/sync_samples/receive_iterator_queue.py
+-rw-rw-r--  2.0 unx     2631 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/sync_samples/session_send_receive.py
+-rw-rw-r--  2.0 unx     1069 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/sync_samples/authenticate_using_azure_named_key_credential.py
+-rw-rw-r--  2.0 unx     1704 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/sync_samples/send_queue.py
+-rw-rw-r--  2.0 unx     6097 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/sync_samples/auto_lock_renew.py
+-rw-rw-r--  2.0 unx      969 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/sync_samples/receive_peek.py
+-rw-rw-r--  2.0 unx     2881 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/sync_samples/mgmt_topic.py
+-rw-rw-r--  2.0 unx     7463 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/sync_samples/failure_and_recovery.py
+-rw-rw-r--  2.0 unx     8389 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/sync_samples/topic_subscription_with_rule_operations.py
+-rw-rw-r--  2.0 unx     3628 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/sync_samples/mgmt_queue.py
+-rw-rw-r--  2.0 unx     1228 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/sync_samples/authenticate_client_connstr.py
+-rw-rw-r--  2.0 unx     2431 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/sync_samples/generate_sas_token_and_authenticate_client.py
+-rw-rw-r--  2.0 unx     2043 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/sync_samples/schedule_messages_and_cancellation.py
+-rw-rw-r--  2.0 unx     3724 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/sync_samples/mgmt_rule.py
+-rw-rw-r--  2.0 unx    16632 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/sync_samples/sample_code_servicebus.py
+-rw-rw-r--  2.0 unx     3263 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/async_samples/session_pool_receive_async.py
+-rw-rw-r--  2.0 unx     8793 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/async_samples/topic_subscription_with_rule_operations_async.py
+-rw-rw-r--  2.0 unx     3478 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/async_samples/mgmt_subscription_async.py
+-rw-rw-r--  2.0 unx     6298 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/async_samples/auto_lock_renew_async.py
+-rw-rw-r--  2.0 unx     1491 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/async_samples/proxy_async.py
+-rw-rw-r--  2.0 unx    16236 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/async_samples/sample_code_servicebus_async.py
+-rw-rw-r--  2.0 unx     1063 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/async_samples/receive_peek_async.py
+-rw-rw-r--  2.0 unx     2045 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/async_samples/receive_deferred_message_queue_async.py
+-rw-rw-r--  2.0 unx     1929 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/async_samples/connection_to_custom_endpoint_address_async.py
+-rw-rw-r--  2.0 unx     1307 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/async_samples/receive_subscription_async.py
+-rw-rw-r--  2.0 unx     1064 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/async_samples/receive_iterator_queue_async.py
+-rw-rw-r--  2.0 unx     1138 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/async_samples/receive_queue_async.py
+-rw-rw-r--  2.0 unx     5456 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/async_samples/deadletter_messages_and_correct_async.py
+-rw-rw-r--  2.0 unx     1860 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/async_samples/send_topic_async.py
+-rw-rw-r--  2.0 unx     2413 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/async_samples/schedule_topic_messages_and_cancellation_async.py
+-rw-rw-r--  2.0 unx     1298 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/async_samples/authenticate_client_connstr_async.py
+-rw-rw-r--  2.0 unx     1200 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/async_samples/authenticate_using_azure_named_key_credential_async.py
+-rw-rw-r--  2.0 unx     3266 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/async_samples/client_identity_authentication_async.py
+-rw-rw-r--  2.0 unx     2076 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/async_samples/receive_deadlettered_messages_async.py
+-rw-rw-r--  2.0 unx     3077 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/async_samples/mgmt_topic_async.py
+-rw-rw-r--  2.0 unx     2259 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/async_samples/schedule_messages_and_cancellation_async.py
+-rw-rw-r--  2.0 unx     3912 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/async_samples/mgmt_rule_async.py
+-rw-rw-r--  2.0 unx     2112 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/async_samples/authenticate_using_azure_sas_credential_async.py
+-rw-rw-r--  2.0 unx     1889 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/async_samples/send_queue_async.py
+-rw-rw-r--  2.0 unx     2818 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/async_samples/session_send_receive_async.py
+-rw-rw-r--  2.0 unx     3838 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/async_samples/mgmt_queue_async.py
+-rw-rw-r--  2.0 unx     3600 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/samples/async_samples/send_and_receive_amqp_annotated_message_async.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-10 01:31 azure-servicebus-7.9.0b1/tests/livetest/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-10 01:31 azure-servicebus-7.9.0b1/tests/async_tests/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-10 01:31 azure-servicebus-7.9.0b1/tests/perf_tests/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-10 01:31 azure-servicebus-7.9.0b1/tests/mgmt_tests/
+-rw-rw-r--  2.0 unx      921 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/sb_env_loader.py
+-rw-rw-r--  2.0 unx     3653 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/test_topic.py
+-rw-rw-r--  2.0 unx     7017 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/test_connection_string_parser.py
+-rw-rw-r--  2.0 unx     8836 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/test_subscriptions.py
+-rw-rw-r--  2.0 unx   146195 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/test_queues.py
+-rw-rw-r--  2.0 unx    36363 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/test_message.py
+-rw-rw-r--  2.0 unx     2048 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/utilities.py
+-rw-rw-r--  2.0 unx    63784 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/test_sessions.py
+-rw-rw-r--  2.0 unx     1494 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/mocks.py
+-rw-rw-r--  2.0 unx    25718 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/servicebus_preparer.py
+-rw-rw-r--  2.0 unx    30056 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/test_sb_client.py
+-rw-rw-r--  2.0 unx     1799 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/livetest/test_errors.py
+-rw-rw-r--  2.0 unx    58696 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/async_tests/test_sessions_async.py
+-rw-rw-r--  2.0 unx   131161 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/async_tests/test_queues_async.py
+-rw-rw-r--  2.0 unx     8037 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/async_tests/test_subscriptions_async.py
+-rw-rw-r--  2.0 unx     2945 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/async_tests/test_topic_async.py
+-rw-rw-r--  2.0 unx     1423 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/async_tests/mocks_async.py
+-rw-rw-r--  2.0 unx    29427 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/async_tests/test_sb_client_async.py
+-rw-rw-r--  2.0 unx     1368 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/perf_tests/send_topic_message.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/perf_tests/__init__.py
+-rw-rw-r--  2.0 unx     1392 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/perf_tests/receive_subscription_message_stream.py
+-rw-rw-r--  2.0 unx     1371 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/perf_tests/receive_queue_message_stream.py
+-rw-rw-r--  2.0 unx    11815 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/perf_tests/_test_base.py
+-rw-rw-r--  2.0 unx     1268 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/perf_tests/send_topic_message_batch.py
+-rw-rw-r--  2.0 unx     1281 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/perf_tests/send_queue_message_batch.py
+-rw-rw-r--  2.0 unx     1376 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/perf_tests/send_queue_message.py
+-rw-rw-r--  2.0 unx     1194 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/perf_tests/receive_queue_message_batch.py
+-rw-rw-r--  2.0 unx     1197 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/perf_tests/receive_subscription_message_batch.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Mar-10 01:31 azure-servicebus-7.9.0b1/tests/mgmt_tests/async/
+-rw-rw-r--  2.0 unx    25789 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/mgmt_tests/test_mgmt_topics.py
+-rw-rw-r--  2.0 unx    28339 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/mgmt_tests/test_mgmt_subscriptions.py
+-rw-rw-r--  2.0 unx    16871 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/mgmt_tests/test_mgmt_rules.py
+-rw-rw-r--  2.0 unx     4585 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/mgmt_tests/mgmt_test_utilities.py
+-rw-rw-r--  2.0 unx     1349 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/mgmt_tests/test_mgmt_namespaces.py
+-rw-rw-r--  2.0 unx    42948 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/mgmt_tests/test_mgmt_queues.py
+-rw-rw-r--  2.0 unx     5115 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/mgmt_tests/async/mgmt_test_utilities_async.py
+-rw-rw-r--  2.0 unx    29536 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/mgmt_tests/async/test_mgmt_subscriptions_async.py
+-rw-rw-r--  2.0 unx     1394 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/mgmt_tests/async/test_mgmt_namespaces_async.py
+-rw-rw-r--  2.0 unx    26493 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/mgmt_tests/async/test_mgmt_topics_async.py
+-rw-rw-r--  2.0 unx    17182 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/mgmt_tests/async/test_mgmt_rules_async.py
+-rw-rw-r--  2.0 unx    43461 b- defN 23-Mar-10 01:30 azure-servicebus-7.9.0b1/tests/mgmt_tests/async/test_mgmt_queues_async.py
+241 files, 2778821 bytes uncompressed, 523044 bytes compressed:  81.2%
```

## zipnote {}

```diff
@@ -1,730 +1,724 @@
-Filename: azure-servicebus-7.9.0a1/
+Filename: azure-servicebus-7.9.0b1/
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure_servicebus.egg-info/
+Filename: azure-servicebus-7.9.0b1/azure_servicebus.egg-info/
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/
+Filename: azure-servicebus-7.9.0b1/azure/
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/
+Filename: azure-servicebus-7.9.0b1/samples/
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/
+Filename: azure-servicebus-7.9.0b1/tests/
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/MANIFEST.in
+Filename: azure-servicebus-7.9.0b1/setup.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/CHANGELOG.md
+Filename: azure-servicebus-7.9.0b1/README.md
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/PKG-INFO
+Filename: azure-servicebus-7.9.0b1/setup.cfg
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/setup.py
+Filename: azure-servicebus-7.9.0b1/migration_guide.md
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/migration_guide.md
+Filename: azure-servicebus-7.9.0b1/pyproject.toml
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/LICENSE
+Filename: azure-servicebus-7.9.0b1/MANIFEST.in
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/README.md
+Filename: azure-servicebus-7.9.0b1/LICENSE
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/setup.cfg
+Filename: azure-servicebus-7.9.0b1/PKG-INFO
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure_servicebus.egg-info/SOURCES.txt
+Filename: azure-servicebus-7.9.0b1/CHANGELOG.md
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure_servicebus.egg-info/dependency_links.txt
+Filename: azure-servicebus-7.9.0b1/azure_servicebus.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure_servicebus.egg-info/not-zip-safe
+Filename: azure-servicebus-7.9.0b1/azure_servicebus.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure_servicebus.egg-info/PKG-INFO
+Filename: azure-servicebus-7.9.0b1/azure_servicebus.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure_servicebus.egg-info/requires.txt
+Filename: azure-servicebus-7.9.0b1/azure_servicebus.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure_servicebus.egg-info/top_level.txt
+Filename: azure-servicebus-7.9.0b1/azure_servicebus.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/livetest/
+Filename: azure-servicebus-7.9.0b1/azure_servicebus.egg-info/requires.txt
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/async_tests/
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/perf_tests/
+Filename: azure-servicebus-7.9.0b1/azure/__init__.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/mgmt_tests/
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_common/
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/test_connection_string_parser.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/utilities.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/amqp/
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/servicebus_preparer.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/aio/
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/test_sessions.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/test_message.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_base_handler.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/test_sb_client.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/__init__.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/test_topic.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_servicebus_client.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/test_queues.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_servicebus_receiver.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/mocks.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_servicebus_session.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/sb_env_loader.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/exceptions.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/test_subscriptions.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_version.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/livetest/test_errors.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_servicebus_sender.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/async_tests/test_subscriptions_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/py.typed
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/async_tests/test_sb_client_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_common/__init__.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/async_tests/test_sessions_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_common/_configuration.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/async_tests/test_topic_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_common/constants.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/async_tests/mocks_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_common/_connection_string_parser.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/async_tests/test_queues_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_common/mgmt_handlers.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/perf_tests/T1_legacy_tests/
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_common/utils.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/perf_tests/_test_base.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_common/message.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/perf_tests/receive_message_stream.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_common/auto_lock_renewer.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/perf_tests/__init__.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_common/receiver_mixins.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/perf_tests/send_message.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/perf_tests/send_message_batch.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/_encode.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/perf_tests/receive_message_batch.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/link.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/perf_tests/T1_legacy_tests/_test_base.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/authentication.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/perf_tests/T1_legacy_tests/receive_message_stream.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/__init__.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/perf_tests/T1_legacy_tests/__init__.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/error.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/perf_tests/T1_legacy_tests/send_message.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/cbs.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/perf_tests/T1_legacy_tests/send_message_batch.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/_platform.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/perf_tests/T1_legacy_tests/receive_message_batch.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/client.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/mgmt_tests/async/
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/receiver.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/mgmt_tests/mgmt_test_utilities.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/management_link.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/mgmt_tests/test_mgmt_rules.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/types.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/mgmt_tests/test_mgmt_queues.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/session.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/mgmt_tests/test_mgmt_subscriptions.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/constants.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/mgmt_tests/test_mgmt_topics.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/management_operation.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/mgmt_tests/test_mgmt_namespaces.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/_message_backcompat.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/mgmt_tests/async/test_mgmt_topics_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/sender.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/mgmt_tests/async/test_mgmt_queues_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/_decode.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/mgmt_tests/async/test_mgmt_rules_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/_connection.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/mgmt_tests/async/mgmt_test_utilities_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/performatives.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/mgmt_tests/async/test_mgmt_namespaces_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/sasl.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/tests/mgmt_tests/async/test_mgmt_subscriptions_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/_transport.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/async_samples/
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/utils.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/sync_samples/
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/outcomes.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/async_samples/mgmt_rule_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/message.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/async_samples/receive_deferred_message_queue_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/endpoints.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/async_samples/deadletter_messages_and_correct_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_transport_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/async_samples/proxy_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_connection_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/async_samples/send_queue_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_link_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/async_samples/receive_peek_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/__init__.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/async_samples/session_pool_receive_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_client_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/async_samples/authenticate_using_azure_sas_credential_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_sasl_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/async_samples/client_identity_authentication_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_session_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/async_samples/receive_iterator_queue_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_sender_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/async_samples/mgmt_subscription_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_authentication_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/async_samples/receive_subscription_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_receiver_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/async_samples/authenticate_client_connstr_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_management_link_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/async_samples/connection_to_custom_endpoint_address_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_management_operation_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/async_samples/send_and_receive_amqp_annotated_message_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_cbs_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/async_samples/send_topic_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/amqp/_amqp_message.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/async_samples/schedule_topic_messages_and_cancellation_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/amqp/__init__.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/async_samples/schedule_messages_and_cancellation_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/amqp/_constants.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/async_samples/mgmt_topic_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/aio/management/
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/async_samples/mgmt_queue_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/aio/__init__.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/async_samples/authenticate_using_azure_named_key_credential_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/aio/_servicebus_receiver_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/async_samples/sample_code_servicebus_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/aio/_base_handler_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/async_samples/receive_queue_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/aio/_async_auto_lock_renewer.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/async_samples/receive_deadlettered_messages_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/aio/_servicebus_sender_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/async_samples/topic_subscription_with_rule_operations_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/aio/_servicebus_client_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/async_samples/auto_lock_renew_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/aio/_async_utils.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/async_samples/session_send_receive_async.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/aio/_servicebus_session_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/sync_samples/mgmt_rule.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/aio/management/__init__.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/sync_samples/receive_deadlettered_messages.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/aio/management/_utils.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/sync_samples/generate_sas_token_and_authenticate_client.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/aio/management/_management_client_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/sync_samples/authenticate_client_connstr.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/aio/management/_shared_key_policy_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/sync_samples/session_send_receive.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/sync_samples/connection_to_custom_endpoint_address.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/__init__.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/sync_samples/failure_and_recovery.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_models.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/sync_samples/sample_code_servicebus.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_model_workaround.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/sync_samples/client_identity_authentication.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_utils.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/sync_samples/deadletter_messages_and_correct.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_handle_response_error.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/sync_samples/receive_subscription.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_management_client.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/sync_samples/mgmt_queue.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_xml_workaround_policy.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/sync_samples/authenticate_using_azure_named_key_credential.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_api_version.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/sync_samples/auto_lock_renew.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_shared_key_policy.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/sync_samples/authenticate_using_azure_sas_credential.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_constants.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/sync_samples/send_topic.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/models/
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/sync_samples/send_and_receive_amqp_annotated_message.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/operations/
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/sync_samples/topic_subscription_with_rule_operations.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/aio/
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/sync_samples/proxy.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/__init__.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/sync_samples/receive_deferred_message_queue.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/_configuration.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/sync_samples/receive_peek.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/_version.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/sync_samples/receive_queue.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/_service_bus_management_client.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/sync_samples/mgmt_subscription.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/models/_service_bus_management_client_enums.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/sync_samples/schedule_topic_messages_and_cancellation.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/models/__init__.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/sync_samples/receive_iterator_queue.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/models/_models.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/sync_samples/session_pool_receive.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/models/_models_py3.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/sync_samples/send_queue.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/operations/_entity_operations.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/sync_samples/mgmt_topic.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/operations/__init__.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/samples/sync_samples/schedule_messages_and_cancellation.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/operations/_service_bus_management_client_operations.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/operations/_rule_operations.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/__init__.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/operations/_namespace_operations.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/aio/
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/operations/_subscription_operations.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/amqp/
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/aio/operations_async/
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/aio/__init__.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_common/
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/aio/_service_bus_management_client_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/aio/_configuration_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_servicebus_session.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/aio/operations_async/__init__.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_base_handler.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/aio/operations_async/_rule_operations_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_servicebus_client.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/aio/operations_async/_entity_operations_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_version.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/aio/operations_async/_service_bus_management_client_operations_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/exceptions.py
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/aio/operations_async/_namespace_operations_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/py.typed
+Filename: azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/aio/operations_async/_subscription_operations_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_servicebus_sender.py
+Filename: azure-servicebus-7.9.0b1/samples/sync_samples/
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/__init__.py
+Filename: azure-servicebus-7.9.0b1/samples/async_samples/
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_servicebus_receiver.py
+Filename: azure-servicebus-7.9.0b1/samples/sync_samples/receive_deferred_message_queue.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/aio/management/
+Filename: azure-servicebus-7.9.0b1/samples/sync_samples/send_topic.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/aio/_servicebus_client_async.py
+Filename: azure-servicebus-7.9.0b1/samples/sync_samples/session_pool_receive.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/aio/_base_handler_async.py
+Filename: azure-servicebus-7.9.0b1/samples/sync_samples/schedule_topic_messages_and_cancellation.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/aio/_servicebus_session_async.py
+Filename: azure-servicebus-7.9.0b1/samples/sync_samples/receive_subscription.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/aio/__init__.py
+Filename: azure-servicebus-7.9.0b1/samples/sync_samples/send_and_receive_amqp_annotated_message.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/aio/_async_utils.py
+Filename: azure-servicebus-7.9.0b1/samples/sync_samples/mgmt_subscription.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/aio/_async_auto_lock_renewer.py
+Filename: azure-servicebus-7.9.0b1/samples/sync_samples/receive_queue.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/aio/_servicebus_receiver_async.py
+Filename: azure-servicebus-7.9.0b1/samples/sync_samples/deadletter_messages_and_correct.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/aio/_servicebus_sender_async.py
+Filename: azure-servicebus-7.9.0b1/samples/sync_samples/proxy.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/aio/management/_management_client_async.py
+Filename: azure-servicebus-7.9.0b1/samples/sync_samples/connection_to_custom_endpoint_address.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/aio/management/__init__.py
+Filename: azure-servicebus-7.9.0b1/samples/sync_samples/client_identity_authentication.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/aio/management/_shared_key_policy_async.py
+Filename: azure-servicebus-7.9.0b1/samples/sync_samples/receive_deadlettered_messages.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/aio/management/_utils.py
+Filename: azure-servicebus-7.9.0b1/samples/sync_samples/authenticate_using_azure_sas_credential.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/amqp/_constants.py
+Filename: azure-servicebus-7.9.0b1/samples/sync_samples/receive_iterator_queue.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/amqp/__init__.py
+Filename: azure-servicebus-7.9.0b1/samples/sync_samples/session_send_receive.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/amqp/_amqp_message.py
+Filename: azure-servicebus-7.9.0b1/samples/sync_samples/authenticate_using_azure_named_key_credential.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/
+Filename: azure-servicebus-7.9.0b1/samples/sync_samples/send_queue.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_api_version.py
+Filename: azure-servicebus-7.9.0b1/samples/sync_samples/auto_lock_renew.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_handle_response_error.py
+Filename: azure-servicebus-7.9.0b1/samples/sync_samples/receive_peek.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_models.py
+Filename: azure-servicebus-7.9.0b1/samples/sync_samples/mgmt_topic.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_xml_workaround_policy.py
+Filename: azure-servicebus-7.9.0b1/samples/sync_samples/failure_and_recovery.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_constants.py
+Filename: azure-servicebus-7.9.0b1/samples/sync_samples/topic_subscription_with_rule_operations.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/__init__.py
+Filename: azure-servicebus-7.9.0b1/samples/sync_samples/mgmt_queue.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_shared_key_policy.py
+Filename: azure-servicebus-7.9.0b1/samples/sync_samples/authenticate_client_connstr.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_management_client.py
+Filename: azure-servicebus-7.9.0b1/samples/sync_samples/generate_sas_token_and_authenticate_client.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_model_workaround.py
+Filename: azure-servicebus-7.9.0b1/samples/sync_samples/schedule_messages_and_cancellation.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_utils.py
+Filename: azure-servicebus-7.9.0b1/samples/sync_samples/mgmt_rule.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/aio/
+Filename: azure-servicebus-7.9.0b1/samples/sync_samples/sample_code_servicebus.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/operations/
+Filename: azure-servicebus-7.9.0b1/samples/async_samples/session_pool_receive_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/models/
+Filename: azure-servicebus-7.9.0b1/samples/async_samples/topic_subscription_with_rule_operations_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/_configuration.py
+Filename: azure-servicebus-7.9.0b1/samples/async_samples/mgmt_subscription_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/_service_bus_management_client.py
+Filename: azure-servicebus-7.9.0b1/samples/async_samples/auto_lock_renew_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/_version.py
+Filename: azure-servicebus-7.9.0b1/samples/async_samples/proxy_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/__init__.py
+Filename: azure-servicebus-7.9.0b1/samples/async_samples/sample_code_servicebus_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/aio/operations_async/
+Filename: azure-servicebus-7.9.0b1/samples/async_samples/receive_peek_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/aio/__init__.py
+Filename: azure-servicebus-7.9.0b1/samples/async_samples/receive_deferred_message_queue_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/aio/_service_bus_management_client_async.py
+Filename: azure-servicebus-7.9.0b1/samples/async_samples/connection_to_custom_endpoint_address_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/aio/_configuration_async.py
+Filename: azure-servicebus-7.9.0b1/samples/async_samples/receive_subscription_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/aio/operations_async/_service_bus_management_client_operations_async.py
+Filename: azure-servicebus-7.9.0b1/samples/async_samples/receive_iterator_queue_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/aio/operations_async/_subscription_operations_async.py
+Filename: azure-servicebus-7.9.0b1/samples/async_samples/receive_queue_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/aio/operations_async/__init__.py
+Filename: azure-servicebus-7.9.0b1/samples/async_samples/deadletter_messages_and_correct_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/aio/operations_async/_namespace_operations_async.py
+Filename: azure-servicebus-7.9.0b1/samples/async_samples/send_topic_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/aio/operations_async/_entity_operations_async.py
+Filename: azure-servicebus-7.9.0b1/samples/async_samples/schedule_topic_messages_and_cancellation_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/aio/operations_async/_rule_operations_async.py
+Filename: azure-servicebus-7.9.0b1/samples/async_samples/authenticate_client_connstr_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/operations/__init__.py
+Filename: azure-servicebus-7.9.0b1/samples/async_samples/authenticate_using_azure_named_key_credential_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/operations/_namespace_operations.py
+Filename: azure-servicebus-7.9.0b1/samples/async_samples/client_identity_authentication_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/operations/_entity_operations.py
+Filename: azure-servicebus-7.9.0b1/samples/async_samples/receive_deadlettered_messages_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/operations/_rule_operations.py
+Filename: azure-servicebus-7.9.0b1/samples/async_samples/mgmt_topic_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/operations/_service_bus_management_client_operations.py
+Filename: azure-servicebus-7.9.0b1/samples/async_samples/schedule_messages_and_cancellation_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/operations/_subscription_operations.py
+Filename: azure-servicebus-7.9.0b1/samples/async_samples/mgmt_rule_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/models/_models.py
+Filename: azure-servicebus-7.9.0b1/samples/async_samples/authenticate_using_azure_sas_credential_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/models/_models_py3.py
+Filename: azure-servicebus-7.9.0b1/samples/async_samples/send_queue_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/models/__init__.py
+Filename: azure-servicebus-7.9.0b1/samples/async_samples/session_send_receive_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/models/_service_bus_management_client_enums.py
+Filename: azure-servicebus-7.9.0b1/samples/async_samples/mgmt_queue_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_common/_configuration.py
+Filename: azure-servicebus-7.9.0b1/samples/async_samples/send_and_receive_amqp_annotated_message_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_common/utils.py
+Filename: azure-servicebus-7.9.0b1/tests/livetest/
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_common/auto_lock_renewer.py
+Filename: azure-servicebus-7.9.0b1/tests/async_tests/
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_common/__init__.py
+Filename: azure-servicebus-7.9.0b1/tests/perf_tests/
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_common/receiver_mixins.py
+Filename: azure-servicebus-7.9.0b1/tests/mgmt_tests/
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_common/constants.py
+Filename: azure-servicebus-7.9.0b1/tests/sb_env_loader.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_common/message.py
+Filename: azure-servicebus-7.9.0b1/tests/test_topic.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_common/_connection_string_parser.py
+Filename: azure-servicebus-7.9.0b1/tests/test_connection_string_parser.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_common/mgmt_handlers.py
+Filename: azure-servicebus-7.9.0b1/tests/test_subscriptions.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/
+Filename: azure-servicebus-7.9.0b1/tests/test_queues.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/types.py
+Filename: azure-servicebus-7.9.0b1/tests/test_message.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/_transport.py
+Filename: azure-servicebus-7.9.0b1/tests/utilities.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/management_operation.py
+Filename: azure-servicebus-7.9.0b1/tests/test_sessions.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/_platform.py
+Filename: azure-servicebus-7.9.0b1/tests/mocks.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/endpoints.py
+Filename: azure-servicebus-7.9.0b1/tests/servicebus_preparer.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/_connection.py
+Filename: azure-servicebus-7.9.0b1/tests/test_sb_client.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/utils.py
+Filename: azure-servicebus-7.9.0b1/tests/livetest/test_errors.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/session.py
+Filename: azure-servicebus-7.9.0b1/tests/async_tests/test_sessions_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/_message_backcompat.py
+Filename: azure-servicebus-7.9.0b1/tests/async_tests/test_queues_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/sender.py
+Filename: azure-servicebus-7.9.0b1/tests/async_tests/test_subscriptions_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/__init__.py
+Filename: azure-servicebus-7.9.0b1/tests/async_tests/test_topic_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/client.py
+Filename: azure-servicebus-7.9.0b1/tests/async_tests/mocks_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/receiver.py
+Filename: azure-servicebus-7.9.0b1/tests/async_tests/test_sb_client_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/management_link.py
+Filename: azure-servicebus-7.9.0b1/tests/perf_tests/send_topic_message.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/constants.py
+Filename: azure-servicebus-7.9.0b1/tests/perf_tests/__init__.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/link.py
+Filename: azure-servicebus-7.9.0b1/tests/perf_tests/receive_subscription_message_stream.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/error.py
+Filename: azure-servicebus-7.9.0b1/tests/perf_tests/receive_queue_message_stream.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/authentication.py
+Filename: azure-servicebus-7.9.0b1/tests/perf_tests/_test_base.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/cbs.py
+Filename: azure-servicebus-7.9.0b1/tests/perf_tests/send_topic_message_batch.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/_encode.py
+Filename: azure-servicebus-7.9.0b1/tests/perf_tests/send_queue_message_batch.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/message.py
+Filename: azure-servicebus-7.9.0b1/tests/perf_tests/send_queue_message.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/performatives.py
+Filename: azure-servicebus-7.9.0b1/tests/perf_tests/receive_queue_message_batch.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/outcomes.py
+Filename: azure-servicebus-7.9.0b1/tests/perf_tests/receive_subscription_message_batch.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/sasl.py
+Filename: azure-servicebus-7.9.0b1/tests/mgmt_tests/async/
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/_decode.py
+Filename: azure-servicebus-7.9.0b1/tests/mgmt_tests/test_mgmt_topics.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_authentication_async.py
+Filename: azure-servicebus-7.9.0b1/tests/mgmt_tests/test_mgmt_subscriptions.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_sender_async.py
+Filename: azure-servicebus-7.9.0b1/tests/mgmt_tests/test_mgmt_rules.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/__init__.py
+Filename: azure-servicebus-7.9.0b1/tests/mgmt_tests/mgmt_test_utilities.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_connection_async.py
+Filename: azure-servicebus-7.9.0b1/tests/mgmt_tests/test_mgmt_namespaces.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_session_async.py
+Filename: azure-servicebus-7.9.0b1/tests/mgmt_tests/test_mgmt_queues.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_client_async.py
+Filename: azure-servicebus-7.9.0b1/tests/mgmt_tests/async/mgmt_test_utilities_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_management_link_async.py
+Filename: azure-servicebus-7.9.0b1/tests/mgmt_tests/async/test_mgmt_subscriptions_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_sasl_async.py
+Filename: azure-servicebus-7.9.0b1/tests/mgmt_tests/async/test_mgmt_namespaces_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_link_async.py
+Filename: azure-servicebus-7.9.0b1/tests/mgmt_tests/async/test_mgmt_topics_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_cbs_async.py
+Filename: azure-servicebus-7.9.0b1/tests/mgmt_tests/async/test_mgmt_rules_async.py
 Comment: 
 
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_transport_async.py
-Comment: 
-
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_receiver_async.py
-Comment: 
-
-Filename: azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_management_operation_async.py
+Filename: azure-servicebus-7.9.0b1/tests/mgmt_tests/async/test_mgmt_queues_async.py
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-servicebus-7.9.0a1/CHANGELOG.md` & `azure-servicebus-7.9.0b1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,32 @@
 # Release History
 
+## 7.9.0b1 (2023-03-09)
+
+### Features Added
+
+- Iterator receiving from Service Bus entities has been added back in.
+
+## 7.8.3 (2023-03-09)
+
+### Bugs Fixed
+
+- Fixed a bug where asynchronous method to add distributed tracing attributes was not being awaited (Issue #28738).
+
+## 7.8.2 (2023-01-10)
+
+### Bugs Fixed
+
+- Fixed a bug that would cause an exception when `None` was sent to `set_state` instead of clearing session state (Issue #27582).
+
+### Other Changes
+
+- Updated uAMQP dependency to 1.6.3.
+  - Added support for Python 3.11.
+
 ## 7.9.0a1 (2022-10-11)
 
 Version 7.9.0a1 is our first efforts to build an Azure Service Bus client library based on a pure Python implemented AMQP stack.
 
 ### Breaking changes
 
 - The following features have been temporarily pulled out which will be added back in future previews as we work towards a stable release:
```

## Comparing `azure-servicebus-7.9.0a1/PKG-INFO` & `azure-servicebus-7.9.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: azure-servicebus
-Version: 7.9.0a1
+Version: 7.9.0b1
 Summary: Microsoft Azure Service Bus Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Azure Service Bus client library for Python
 
@@ -43,15 +44,15 @@
 ## Getting started
 
 ### Install the package
 
 Install the Azure Service Bus client library for Python with [pip][pip]:
 
 ```Bash
-pip install azure-servicebus
+pip install azure-servicebus==7.9.0b1
 ```
 
 ### Prerequisites:
 To use this package, you must have:
 * Azure subscription - [Create a free account][azure_sub]
 * Azure Service Bus - [Namespace and management credentials][service_bus_namespace]
 * Python 3.7 or later - [Install Python][python]
@@ -127,15 +128,15 @@
 Please find further examples in the [samples](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/servicebus/azure-servicebus/samples) directory demonstrating common Service Bus scenarios such as sending, receiving, session management and message handling.
 
 ### Send messages to a queue
 > **NOTE:** see reference documentation [here][send_reference].
 
 This example sends single message and array of messages to a queue that is assumed to already exist, created via the Azure portal or az commands.
 
-```Python
+```python
 from azure.servicebus import ServiceBusClient, ServiceBusMessage
 
 import os
 connstr = os.environ['SERVICE_BUS_CONNECTION_STR']
 queue_name = os.environ['SERVICE_BUS_QUEUE_NAME']
 
 with ServiceBusClient.from_connection_string(connstr) as client:
@@ -155,15 +156,15 @@
 
 ### Receive messages from a queue
 
 To receive from a queue, you can either perform an ad-hoc receive via `receiver.receive_messages()` or receive persistently through the receiver itself.
 
 #### [Receive messages from a queue through iterating over ServiceBusReceiver][streaming_receive_reference]
 
-```Python
+```python
 from azure.servicebus import ServiceBusClient
 
 import os
 connstr = os.environ['SERVICE_BUS_CONNECTION_STR']
 queue_name = os.environ['SERVICE_BUS_QUEUE_NAME']
 
 with ServiceBusClient.from_connection_string(connstr) as client:
@@ -180,15 +181,15 @@
 > See [AutoLockRenewer](#automatically-renew-message-or-session-locks "Automatically renew Message or Session locks") for a helper to perform this in the background automatically.
 > Lock duration is set in Azure on the queue or topic itself.
 
 #### [Receive messages from a queue through ServiceBusReceiver.receive_messages()][receive_reference]
 
 > **NOTE:** `ServiceBusReceiver.receive_messages()` receives a single or constrained list of messages through an ad-hoc method call, as opposed to receiving perpetually from the generator. It always returns a list.
 
-```Python
+```python
 from azure.servicebus import ServiceBusClient
 
 import os
 connstr = os.environ['SERVICE_BUS_CONNECTION_STR']
 queue_name = os.environ['SERVICE_BUS_QUEUE_NAME']
 
 with ServiceBusClient.from_connection_string(connstr) as client:
@@ -209,15 +210,15 @@
 
 
 ### Send and receive a message from a session enabled queue
 > **NOTE:** see reference documentation for session [send][session_send_reference] and [receive][session_receive_reference].
 
 Sessions provide first-in-first-out and single-receiver semantics on top of a queue or subscription.  While the actual receive syntax is the same, initialization differs slightly.
 
-```Python
+```python
 from azure.servicebus import ServiceBusClient, ServiceBusMessage
 
 import os
 connstr = os.environ['SERVICE_BUS_CONNECTION_STR']
 queue_name = os.environ['SERVICE_BUS_QUEUE_NAME']
 session_id = os.environ['SERVICE_BUS_SESSION_ID']
 
@@ -237,15 +238,15 @@
 
 ### Working with [topics][topic_reference] and [subscriptions][subscription_reference]
 > **NOTE:** see reference documentation for [topics][topic_reference] and [subscriptions][subscription_reference].
 
 Topics and subscriptions give an alternative to queues for sending and receiving messages.  See documents [here][topic_concept] for more overarching detail,
 and of how these differ from queues.
 
-```Python
+```python
 from azure.servicebus import ServiceBusClient, ServiceBusMessage
 
 import os
 connstr = os.environ['SERVICE_BUS_CONNECTION_STR']
 topic_name = os.environ['SERVICE_BUS_TOPIC_NAME']
 subscription_name = os.environ['SERVICE_BUS_SUBSCRIPTION_NAME']
 
@@ -272,15 +273,15 @@
 Lock duration is set in Azure on the queue or topic itself.
 See [AutoLockRenewer](#automatically-renew-message-or-session-locks "Automatically renew Message or Session locks") for a helper to perform this in the background automatically.
 
 #### [Complete][complete_reference]
 
 Declares the message processing to be successfully completed, removing the message from the queue.
 
-```Python
+```python
 from azure.servicebus import ServiceBusClient
 
 import os
 connstr = os.environ['SERVICE_BUS_CONNECTION_STR']
 queue_name = os.environ['SERVICE_BUS_QUEUE_NAME']
 
 with ServiceBusClient.from_connection_string(connstr) as client:
@@ -290,15 +291,15 @@
             receiver.complete_message(msg)
 ```
 
 #### [Abandon][abandon_reference]
 
 Abandon processing of the message for the time being, returning the message immediately back to the queue to be picked up by another (or the same) receiver.
 
-```Python
+```python
 from azure.servicebus import ServiceBusClient
 
 import os
 connstr = os.environ['SERVICE_BUS_CONNECTION_STR']
 queue_name = os.environ['SERVICE_BUS_QUEUE_NAME']
 
 with ServiceBusClient.from_connection_string(connstr) as client:
@@ -308,15 +309,15 @@
             receiver.abandon_message(msg)
 ```
 
 #### [DeadLetter][deadletter_reference]
 
 Transfer the message from the primary queue into a special "dead-letter sub-queue" where it can be accessed using the `ServiceBusClient.get_<queue|subscription>_receiver` function with parameter `sub_queue=ServiceBusSubQueue.DEAD_LETTER` and consumed from like any other receiver. (see sample [here](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/servicebus/azure-servicebus/samples/sync_samples/receive_deadlettered_messages.py))
 
-```Python
+```python
 from azure.servicebus import ServiceBusClient
 
 import os
 connstr = os.environ['SERVICE_BUS_CONNECTION_STR']
 queue_name = os.environ['SERVICE_BUS_QUEUE_NAME']
 
 with ServiceBusClient.from_connection_string(connstr) as client:
@@ -327,15 +328,15 @@
 ```
 
 #### [Defer][defer_reference]
 
 Defer is subtly different from the prior settlement methods.  It prevents the message from being directly received from the queue
 by setting it aside such that it must be received by sequence number in a call to `ServiceBusReceiver.receive_deferred_messages` (see sample [here](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/servicebus/azure-servicebus/samples/sync_samples/receive_deferred_message_queue.py))
 
-```Python
+```python
 from azure.servicebus import ServiceBusClient
 
 import os
 connstr = os.environ['SERVICE_BUS_CONNECTION_STR']
 queue_name = os.environ['SERVICE_BUS_QUEUE_NAME']
 
 with ServiceBusClient.from_connection_string(connstr) as client:
@@ -563,14 +564,37 @@
 [sample_authenticate_client_connstr]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/servicebus/azure-servicebus/samples/sync_samples/authenticate_client_connstr.py
 [sample_authenticate_client_aad]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/servicebus/azure-servicebus/samples/sync_samples/client_identity_authentication.py
 [migration_guide]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/servicebus/azure-servicebus/migration_guide.md
 
 
 # Release History
 
+## 7.9.0b1 (2023-03-09)
+
+### Features Added
+
+- Iterator receiving from Service Bus entities has been added back in.
+
+## 7.8.3 (2023-03-09)
+
+### Bugs Fixed
+
+- Fixed a bug where asynchronous method to add distributed tracing attributes was not being awaited (Issue #28738).
+
+## 7.8.2 (2023-01-10)
+
+### Bugs Fixed
+
+- Fixed a bug that would cause an exception when `None` was sent to `set_state` instead of clearing session state (Issue #27582).
+
+### Other Changes
+
+- Updated uAMQP dependency to 1.6.3.
+  - Added support for Python 3.11.
+
 ## 7.9.0a1 (2022-10-11)
 
 Version 7.9.0a1 is our first efforts to build an Azure Service Bus client library based on a pure Python implemented AMQP stack.
 
 ### Breaking changes
 
 - The following features have been temporarily pulled out which will be added back in future previews as we work towards a stable release:
```

## Comparing `azure-servicebus-7.9.0a1/setup.py` & `azure-servicebus-7.9.0b1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,21 +41,22 @@
     long_description=readme + '\n\n' + changelog,
     long_description_content_type='text/markdown',
     license='MIT License',
     author='Microsoft Corporation',
     author_email='azpysdkhelp@microsoft.com',
     url='https://github.com/Azure/azure-sdk-for-python',
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         'Programming Language :: Python',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: MIT License',
     ],
     python_requires=">=3.7",
     zip_safe=False,
     packages=find_packages(exclude=[
         'tests',
         'samples',
```

## Comparing `azure-servicebus-7.9.0a1/migration_guide.md` & `azure-servicebus-7.9.0b1/migration_guide.md`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 # for subscription
 subscription_client = client.get_subscription(topic_name, subscription_name)
 subscription_receiver = subscription_client.get_receiver()
 subscription_dead_letter_receiver = subscription_client.get_deadletter_receiver()
 ```
 
 In V7:
-```Python
+```python
 with ServiceBusClient.from_connection_string(connstr) as client:
 
     # for queues
     queue_sender = client.get_queue_sender(queue_name)
     queue_receiver = client.get_queue_receiver(queue_name)
     queue_dead_letter_receiver = client.get_queue_receiver(queue_name, sub_queue=ServiceBusSubQueue.DEAD_LETTER)
```

## Comparing `azure-servicebus-7.9.0a1/LICENSE` & `azure-servicebus-7.9.0b1/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/README.md` & `azure-servicebus-7.9.0b1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ## Getting started
 
 ### Install the package
 
 Install the Azure Service Bus client library for Python with [pip][pip]:
 
 ```Bash
-pip install azure-servicebus
+pip install azure-servicebus==7.9.0b1
 ```
 
 ### Prerequisites:
 To use this package, you must have:
 * Azure subscription - [Create a free account][azure_sub]
 * Azure Service Bus - [Namespace and management credentials][service_bus_namespace]
 * Python 3.7 or later - [Install Python][python]
@@ -107,15 +107,15 @@
 Please find further examples in the [samples](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/servicebus/azure-servicebus/samples) directory demonstrating common Service Bus scenarios such as sending, receiving, session management and message handling.
 
 ### Send messages to a queue
 > **NOTE:** see reference documentation [here][send_reference].
 
 This example sends single message and array of messages to a queue that is assumed to already exist, created via the Azure portal or az commands.
 
-```Python
+```python
 from azure.servicebus import ServiceBusClient, ServiceBusMessage
 
 import os
 connstr = os.environ['SERVICE_BUS_CONNECTION_STR']
 queue_name = os.environ['SERVICE_BUS_QUEUE_NAME']
 
 with ServiceBusClient.from_connection_string(connstr) as client:
@@ -135,15 +135,15 @@
 
 ### Receive messages from a queue
 
 To receive from a queue, you can either perform an ad-hoc receive via `receiver.receive_messages()` or receive persistently through the receiver itself.
 
 #### [Receive messages from a queue through iterating over ServiceBusReceiver][streaming_receive_reference]
 
-```Python
+```python
 from azure.servicebus import ServiceBusClient
 
 import os
 connstr = os.environ['SERVICE_BUS_CONNECTION_STR']
 queue_name = os.environ['SERVICE_BUS_QUEUE_NAME']
 
 with ServiceBusClient.from_connection_string(connstr) as client:
@@ -160,15 +160,15 @@
 > See [AutoLockRenewer](#automatically-renew-message-or-session-locks "Automatically renew Message or Session locks") for a helper to perform this in the background automatically.
 > Lock duration is set in Azure on the queue or topic itself.
 
 #### [Receive messages from a queue through ServiceBusReceiver.receive_messages()][receive_reference]
 
 > **NOTE:** `ServiceBusReceiver.receive_messages()` receives a single or constrained list of messages through an ad-hoc method call, as opposed to receiving perpetually from the generator. It always returns a list.
 
-```Python
+```python
 from azure.servicebus import ServiceBusClient
 
 import os
 connstr = os.environ['SERVICE_BUS_CONNECTION_STR']
 queue_name = os.environ['SERVICE_BUS_QUEUE_NAME']
 
 with ServiceBusClient.from_connection_string(connstr) as client:
@@ -189,15 +189,15 @@
 
 
 ### Send and receive a message from a session enabled queue
 > **NOTE:** see reference documentation for session [send][session_send_reference] and [receive][session_receive_reference].
 
 Sessions provide first-in-first-out and single-receiver semantics on top of a queue or subscription.  While the actual receive syntax is the same, initialization differs slightly.
 
-```Python
+```python
 from azure.servicebus import ServiceBusClient, ServiceBusMessage
 
 import os
 connstr = os.environ['SERVICE_BUS_CONNECTION_STR']
 queue_name = os.environ['SERVICE_BUS_QUEUE_NAME']
 session_id = os.environ['SERVICE_BUS_SESSION_ID']
 
@@ -217,15 +217,15 @@
 
 ### Working with [topics][topic_reference] and [subscriptions][subscription_reference]
 > **NOTE:** see reference documentation for [topics][topic_reference] and [subscriptions][subscription_reference].
 
 Topics and subscriptions give an alternative to queues for sending and receiving messages.  See documents [here][topic_concept] for more overarching detail,
 and of how these differ from queues.
 
-```Python
+```python
 from azure.servicebus import ServiceBusClient, ServiceBusMessage
 
 import os
 connstr = os.environ['SERVICE_BUS_CONNECTION_STR']
 topic_name = os.environ['SERVICE_BUS_TOPIC_NAME']
 subscription_name = os.environ['SERVICE_BUS_SUBSCRIPTION_NAME']
 
@@ -252,15 +252,15 @@
 Lock duration is set in Azure on the queue or topic itself.
 See [AutoLockRenewer](#automatically-renew-message-or-session-locks "Automatically renew Message or Session locks") for a helper to perform this in the background automatically.
 
 #### [Complete][complete_reference]
 
 Declares the message processing to be successfully completed, removing the message from the queue.
 
-```Python
+```python
 from azure.servicebus import ServiceBusClient
 
 import os
 connstr = os.environ['SERVICE_BUS_CONNECTION_STR']
 queue_name = os.environ['SERVICE_BUS_QUEUE_NAME']
 
 with ServiceBusClient.from_connection_string(connstr) as client:
@@ -270,15 +270,15 @@
             receiver.complete_message(msg)
 ```
 
 #### [Abandon][abandon_reference]
 
 Abandon processing of the message for the time being, returning the message immediately back to the queue to be picked up by another (or the same) receiver.
 
-```Python
+```python
 from azure.servicebus import ServiceBusClient
 
 import os
 connstr = os.environ['SERVICE_BUS_CONNECTION_STR']
 queue_name = os.environ['SERVICE_BUS_QUEUE_NAME']
 
 with ServiceBusClient.from_connection_string(connstr) as client:
@@ -288,15 +288,15 @@
             receiver.abandon_message(msg)
 ```
 
 #### [DeadLetter][deadletter_reference]
 
 Transfer the message from the primary queue into a special "dead-letter sub-queue" where it can be accessed using the `ServiceBusClient.get_<queue|subscription>_receiver` function with parameter `sub_queue=ServiceBusSubQueue.DEAD_LETTER` and consumed from like any other receiver. (see sample [here](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/servicebus/azure-servicebus/samples/sync_samples/receive_deadlettered_messages.py))
 
-```Python
+```python
 from azure.servicebus import ServiceBusClient
 
 import os
 connstr = os.environ['SERVICE_BUS_CONNECTION_STR']
 queue_name = os.environ['SERVICE_BUS_QUEUE_NAME']
 
 with ServiceBusClient.from_connection_string(connstr) as client:
@@ -307,15 +307,15 @@
 ```
 
 #### [Defer][defer_reference]
 
 Defer is subtly different from the prior settlement methods.  It prevents the message from being directly received from the queue
 by setting it aside such that it must be received by sequence number in a call to `ServiceBusReceiver.receive_deferred_messages` (see sample [here](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/servicebus/azure-servicebus/samples/sync_samples/receive_deferred_message_queue.py))
 
-```Python
+```python
 from azure.servicebus import ServiceBusClient
 
 import os
 connstr = os.environ['SERVICE_BUS_CONNECTION_STR']
 queue_name = os.environ['SERVICE_BUS_QUEUE_NAME']
 
 with ServiceBusClient.from_connection_string(connstr) as client:
```

## Comparing `azure-servicebus-7.9.0a1/azure_servicebus.egg-info/SOURCES.txt` & `azure-servicebus-7.9.0b1/azure_servicebus.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 migration_guide.md
+pyproject.toml
 setup.py
 azure/__init__.py
 azure/servicebus/__init__.py
 azure/servicebus/_base_handler.py
 azure/servicebus/_servicebus_client.py
 azure/servicebus/_servicebus_receiver.py
 azure/servicebus/_servicebus_sender.py
@@ -199,17 +200,15 @@
 tests/mgmt_tests/async/test_mgmt_namespaces_async.py
 tests/mgmt_tests/async/test_mgmt_queues_async.py
 tests/mgmt_tests/async/test_mgmt_rules_async.py
 tests/mgmt_tests/async/test_mgmt_subscriptions_async.py
 tests/mgmt_tests/async/test_mgmt_topics_async.py
 tests/perf_tests/__init__.py
 tests/perf_tests/_test_base.py
-tests/perf_tests/receive_message_batch.py
-tests/perf_tests/receive_message_stream.py
-tests/perf_tests/send_message.py
-tests/perf_tests/send_message_batch.py
-tests/perf_tests/T1_legacy_tests/__init__.py
-tests/perf_tests/T1_legacy_tests/_test_base.py
-tests/perf_tests/T1_legacy_tests/receive_message_batch.py
-tests/perf_tests/T1_legacy_tests/receive_message_stream.py
-tests/perf_tests/T1_legacy_tests/send_message.py
-tests/perf_tests/T1_legacy_tests/send_message_batch.py
+tests/perf_tests/receive_queue_message_batch.py
+tests/perf_tests/receive_queue_message_stream.py
+tests/perf_tests/receive_subscription_message_batch.py
+tests/perf_tests/receive_subscription_message_stream.py
+tests/perf_tests/send_queue_message.py
+tests/perf_tests/send_queue_message_batch.py
+tests/perf_tests/send_topic_message.py
+tests/perf_tests/send_topic_message_batch.py
```

## Comparing `azure-servicebus-7.9.0a1/azure_servicebus.egg-info/PKG-INFO` & `azure-servicebus-7.9.0b1/azure_servicebus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: azure-servicebus
-Version: 7.9.0a1
+Version: 7.9.0b1
 Summary: Microsoft Azure Service Bus Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Azure Service Bus client library for Python
 
@@ -43,15 +44,15 @@
 ## Getting started
 
 ### Install the package
 
 Install the Azure Service Bus client library for Python with [pip][pip]:
 
 ```Bash
-pip install azure-servicebus
+pip install azure-servicebus==7.9.0b1
 ```
 
 ### Prerequisites:
 To use this package, you must have:
 * Azure subscription - [Create a free account][azure_sub]
 * Azure Service Bus - [Namespace and management credentials][service_bus_namespace]
 * Python 3.7 or later - [Install Python][python]
@@ -127,15 +128,15 @@
 Please find further examples in the [samples](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/servicebus/azure-servicebus/samples) directory demonstrating common Service Bus scenarios such as sending, receiving, session management and message handling.
 
 ### Send messages to a queue
 > **NOTE:** see reference documentation [here][send_reference].
 
 This example sends single message and array of messages to a queue that is assumed to already exist, created via the Azure portal or az commands.
 
-```Python
+```python
 from azure.servicebus import ServiceBusClient, ServiceBusMessage
 
 import os
 connstr = os.environ['SERVICE_BUS_CONNECTION_STR']
 queue_name = os.environ['SERVICE_BUS_QUEUE_NAME']
 
 with ServiceBusClient.from_connection_string(connstr) as client:
@@ -155,15 +156,15 @@
 
 ### Receive messages from a queue
 
 To receive from a queue, you can either perform an ad-hoc receive via `receiver.receive_messages()` or receive persistently through the receiver itself.
 
 #### [Receive messages from a queue through iterating over ServiceBusReceiver][streaming_receive_reference]
 
-```Python
+```python
 from azure.servicebus import ServiceBusClient
 
 import os
 connstr = os.environ['SERVICE_BUS_CONNECTION_STR']
 queue_name = os.environ['SERVICE_BUS_QUEUE_NAME']
 
 with ServiceBusClient.from_connection_string(connstr) as client:
@@ -180,15 +181,15 @@
 > See [AutoLockRenewer](#automatically-renew-message-or-session-locks "Automatically renew Message or Session locks") for a helper to perform this in the background automatically.
 > Lock duration is set in Azure on the queue or topic itself.
 
 #### [Receive messages from a queue through ServiceBusReceiver.receive_messages()][receive_reference]
 
 > **NOTE:** `ServiceBusReceiver.receive_messages()` receives a single or constrained list of messages through an ad-hoc method call, as opposed to receiving perpetually from the generator. It always returns a list.
 
-```Python
+```python
 from azure.servicebus import ServiceBusClient
 
 import os
 connstr = os.environ['SERVICE_BUS_CONNECTION_STR']
 queue_name = os.environ['SERVICE_BUS_QUEUE_NAME']
 
 with ServiceBusClient.from_connection_string(connstr) as client:
@@ -209,15 +210,15 @@
 
 
 ### Send and receive a message from a session enabled queue
 > **NOTE:** see reference documentation for session [send][session_send_reference] and [receive][session_receive_reference].
 
 Sessions provide first-in-first-out and single-receiver semantics on top of a queue or subscription.  While the actual receive syntax is the same, initialization differs slightly.
 
-```Python
+```python
 from azure.servicebus import ServiceBusClient, ServiceBusMessage
 
 import os
 connstr = os.environ['SERVICE_BUS_CONNECTION_STR']
 queue_name = os.environ['SERVICE_BUS_QUEUE_NAME']
 session_id = os.environ['SERVICE_BUS_SESSION_ID']
 
@@ -237,15 +238,15 @@
 
 ### Working with [topics][topic_reference] and [subscriptions][subscription_reference]
 > **NOTE:** see reference documentation for [topics][topic_reference] and [subscriptions][subscription_reference].
 
 Topics and subscriptions give an alternative to queues for sending and receiving messages.  See documents [here][topic_concept] for more overarching detail,
 and of how these differ from queues.
 
-```Python
+```python
 from azure.servicebus import ServiceBusClient, ServiceBusMessage
 
 import os
 connstr = os.environ['SERVICE_BUS_CONNECTION_STR']
 topic_name = os.environ['SERVICE_BUS_TOPIC_NAME']
 subscription_name = os.environ['SERVICE_BUS_SUBSCRIPTION_NAME']
 
@@ -272,15 +273,15 @@
 Lock duration is set in Azure on the queue or topic itself.
 See [AutoLockRenewer](#automatically-renew-message-or-session-locks "Automatically renew Message or Session locks") for a helper to perform this in the background automatically.
 
 #### [Complete][complete_reference]
 
 Declares the message processing to be successfully completed, removing the message from the queue.
 
-```Python
+```python
 from azure.servicebus import ServiceBusClient
 
 import os
 connstr = os.environ['SERVICE_BUS_CONNECTION_STR']
 queue_name = os.environ['SERVICE_BUS_QUEUE_NAME']
 
 with ServiceBusClient.from_connection_string(connstr) as client:
@@ -290,15 +291,15 @@
             receiver.complete_message(msg)
 ```
 
 #### [Abandon][abandon_reference]
 
 Abandon processing of the message for the time being, returning the message immediately back to the queue to be picked up by another (or the same) receiver.
 
-```Python
+```python
 from azure.servicebus import ServiceBusClient
 
 import os
 connstr = os.environ['SERVICE_BUS_CONNECTION_STR']
 queue_name = os.environ['SERVICE_BUS_QUEUE_NAME']
 
 with ServiceBusClient.from_connection_string(connstr) as client:
@@ -308,15 +309,15 @@
             receiver.abandon_message(msg)
 ```
 
 #### [DeadLetter][deadletter_reference]
 
 Transfer the message from the primary queue into a special "dead-letter sub-queue" where it can be accessed using the `ServiceBusClient.get_<queue|subscription>_receiver` function with parameter `sub_queue=ServiceBusSubQueue.DEAD_LETTER` and consumed from like any other receiver. (see sample [here](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/servicebus/azure-servicebus/samples/sync_samples/receive_deadlettered_messages.py))
 
-```Python
+```python
 from azure.servicebus import ServiceBusClient
 
 import os
 connstr = os.environ['SERVICE_BUS_CONNECTION_STR']
 queue_name = os.environ['SERVICE_BUS_QUEUE_NAME']
 
 with ServiceBusClient.from_connection_string(connstr) as client:
@@ -327,15 +328,15 @@
 ```
 
 #### [Defer][defer_reference]
 
 Defer is subtly different from the prior settlement methods.  It prevents the message from being directly received from the queue
 by setting it aside such that it must be received by sequence number in a call to `ServiceBusReceiver.receive_deferred_messages` (see sample [here](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/servicebus/azure-servicebus/samples/sync_samples/receive_deferred_message_queue.py))
 
-```Python
+```python
 from azure.servicebus import ServiceBusClient
 
 import os
 connstr = os.environ['SERVICE_BUS_CONNECTION_STR']
 queue_name = os.environ['SERVICE_BUS_QUEUE_NAME']
 
 with ServiceBusClient.from_connection_string(connstr) as client:
@@ -563,14 +564,37 @@
 [sample_authenticate_client_connstr]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/servicebus/azure-servicebus/samples/sync_samples/authenticate_client_connstr.py
 [sample_authenticate_client_aad]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/servicebus/azure-servicebus/samples/sync_samples/client_identity_authentication.py
 [migration_guide]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/servicebus/azure-servicebus/migration_guide.md
 
 
 # Release History
 
+## 7.9.0b1 (2023-03-09)
+
+### Features Added
+
+- Iterator receiving from Service Bus entities has been added back in.
+
+## 7.8.3 (2023-03-09)
+
+### Bugs Fixed
+
+- Fixed a bug where asynchronous method to add distributed tracing attributes was not being awaited (Issue #28738).
+
+## 7.8.2 (2023-01-10)
+
+### Bugs Fixed
+
+- Fixed a bug that would cause an exception when `None` was sent to `set_state` instead of clearing session state (Issue #27582).
+
+### Other Changes
+
+- Updated uAMQP dependency to 1.6.3.
+  - Added support for Python 3.11.
+
 ## 7.9.0a1 (2022-10-11)
 
 Version 7.9.0a1 is our first efforts to build an Azure Service Bus client library based on a pure Python implemented AMQP stack.
 
 ### Breaking changes
 
 - The following features have been temporarily pulled out which will be added back in future previews as we work towards a stable release:
```

## Comparing `azure-servicebus-7.9.0a1/tests/test_connection_string_parser.py` & `azure-servicebus-7.9.0b1/tests/test_connection_string_parser.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/tests/utilities.py` & `azure-servicebus-7.9.0b1/tests/utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,24 +20,24 @@
         logger.setLevel(level)
         handler = _get_default_handler()
         logger.addHandler(handler)
     return logger
 
 # Note: This was the initial generic logger entry point, kept to allow us to
 # move to more fine-grained logging controls incrementally.
-def get_logger(level, uamqp_level=logging.INFO):
-    _build_logger("uamqp", uamqp_level)
+def get_logger(level, pyamqp_level=logging.INFO):
+    _build_logger("azure.servicebus._pyamqp", pyamqp_level)
     return _build_logger("azure", level)
 
 
 def print_message(_logger, message):
     _logger.info("Receiving: {}".format(message))
     _logger.debug("Time to live: {}".format(message.time_to_live))
     _logger.debug("Sequence number: {}".format(message.sequence_number))
-    _logger.debug("Enqueue Sequence numger: {}".format(message.enqueued_sequence_number))
+    _logger.debug("Enqueue Sequence number: {}".format(message.enqueued_sequence_number))
     _logger.debug("Partition Key: {}".format(message.partition_key))
     _logger.debug("Application Properties: {}".format(message.application_properties))
     _logger.debug("Delivery count: {}".format(message.delivery_count))
     try:
         _logger.debug("Locked until: {}".format(message.locked_until_utc))
         _logger.debug("Lock Token: {}".format(message.lock_token))
     except (TypeError, AttributeError):
```

## Comparing `azure-servicebus-7.9.0a1/tests/servicebus_preparer.py` & `azure-servicebus-7.9.0b1/tests/servicebus_preparer.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/tests/test_sessions.py` & `azure-servicebus-7.9.0b1/tests/test_sessions.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 )
 from utilities import get_logger, print_message, sleep_until_expired
 
 _logger = get_logger(logging.DEBUG)
 
 
 class ServiceBusSessionTests(AzureMgmtTestCase):
-    @pytest.mark.skip(reason="TODO: iterator support")
+    @pytest.mark.skip(reason="TODO: Pyamqp Message Serialization Error")
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer()
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     def test_session_by_session_client_conn_str_receive_handler_peeklock(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         with ServiceBusClient.from_connection_string(
@@ -167,15 +167,15 @@
                         sender.send_messages(message)
                     else:
                         received_cnt_dic[message.message_id] += 1
 
                 assert received_cnt_dic['0'] == 2 and received_cnt_dic['1'] == 2 and received_cnt_dic['2'] == 2
                 assert count == 6
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True, lock_duration='PT5S')
     def test_session_by_queue_client_conn_str_receive_handler_receiveanddelete(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         with ServiceBusClient.from_connection_string(
@@ -205,15 +205,15 @@
 
             messages = []
             with sb_client.get_queue_receiver(servicebus_queue.name, session_id=session_id, receive_mode=ServiceBusReceiveMode.RECEIVE_AND_DELETE, max_wait_time=5) as session:
                 for message in session:
                     messages.append(message)
                 assert len(messages) == 0
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer()
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     def test_session_by_session_client_conn_str_receive_handler_with_stop(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         with ServiceBusClient.from_connection_string(
@@ -300,15 +300,15 @@
 
             with sb_client.get_queue_receiver(servicebus_queue.name, session_id=NEXT_AVAILABLE_SESSION, max_wait_time=5) as receiver:
                 messages = []
                 for message in receiver:
                     messages.append(message)
                 assert len(messages) == 1
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     def test_session_by_session_client_conn_str_receive_handler_with_inactive_session(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         with ServiceBusClient.from_connection_string(
@@ -322,15 +322,15 @@
                                               max_wait_time=5) as session:
                 for message in session:
                     messages.append(message)
 
                 assert session._running
                 assert len(messages) == 0
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     def test_session_by_servicebus_client_iter_messages_with_retrieve_deferred_receiver_complete(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         with ServiceBusClient.from_connection_string(
@@ -365,15 +365,15 @@
                     assert message.lock_token
                     assert not message.locked_until_utc
                     assert message._receiver
                     with pytest.raises(TypeError):
                         receiver.renew_message_lock(message)
                     receiver.complete_message(message)
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     def test_session_by_servicebus_client_iter_messages_with_retrieve_deferred_receiver_deadletter(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         with ServiceBusClient.from_connection_string(
@@ -417,15 +417,15 @@
                     assert message.dead_letter_reason == 'Testing reason'
                     assert message.dead_letter_error_description == 'Testing description'
                     assert message.application_properties[b'DeadLetterReason'] == b'Testing reason'
                     assert message.application_properties[b'DeadLetterErrorDescription'] == b'Testing description'
                     receiver.complete_message(message)
             assert count == 10
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     def test_session_by_servicebus_client_iter_messages_with_retrieve_deferred_receiver_deletemode(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         with ServiceBusClient.from_connection_string(
@@ -456,15 +456,15 @@
                 for message in deferred:
                     assert isinstance(message, ServiceBusReceivedMessage)
                     with pytest.raises(ValueError):
                         receiver.complete_message(message)
                 with pytest.raises(ServiceBusError):
                     deferred = receiver.receive_deferred_messages(deferred_messages)
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     def test_session_by_servicebus_client_iter_messages_with_retrieve_deferred_client(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         with ServiceBusClient.from_connection_string(
@@ -488,15 +488,15 @@
                 assert count == 10
 
                 deferred = receiver.receive_deferred_messages(deferred_messages)
 
                 with pytest.raises(MessageAlreadySettled):
                     receiver.complete_message(message)
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     def test_session_by_servicebus_client_receive_with_retrieve_deadletter(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
 
@@ -642,15 +642,15 @@
                     # potentially as a side effect of network delays/sleeps/"typical distributed systems nonsense."  In a perfect world we wouldn't have a magic number/network hop but this allows
                     # a slightly more robust test in absence of that.
                     assert (receiver.session._locked_until_utc - utc_now()) <= timedelta(seconds=60)
                     sleep_until_expired(receiver.session)
                     with pytest.raises(SessionLockLostError):
                         receiver.complete_message(messages[2])
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True, lock_duration='PT10S')
     def test_session_by_conn_str_receive_handler_with_autolockrenew(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
 
@@ -718,15 +718,15 @@
                                  on_lock_renew_failure=lock_lost_callback)
             sleep_until_expired(receiver.session)
             assert not results
 
             renewer.close()
             assert len(messages) == 2
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True, lock_duration='PT10S')
     def test_session_by_conn_str_receive_handler_with_auto_autolockrenew(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
 
@@ -1012,15 +1012,15 @@
                 count = 0
                 while not messages and count < 13:
                     messages = receiver.receive_messages(max_wait_time=20)
                     receiver.session.renew_lock()
                     count += 1
                 assert len(messages) == 0
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     def test_session_get_set_state_with_receiver(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
 
@@ -1147,15 +1147,15 @@
                 for _ in range(concurrent_receivers):
                     futures.append(thread_pool.submit(message_processing, sb_client))
                 concurrent.futures.wait(futures)
     
             assert not errors
             assert len(messages) == 100
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     def test_session_by_session_client_conn_str_receive_handler_peeklock_abandon(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         with ServiceBusClient.from_connection_string(
@@ -1173,15 +1173,15 @@
                 receiver.abandon_message(message)
                 for next_message in receiver: # we can't be sure there won't be a service delay, so we may not get the message back _immediately_, even if in most cases it shows right back up.
                     if not next_message:
                         raise Exception("Did not successfully re-receive abandoned message, sequence_number 1 was not observed.")
                     if next_message.sequence_number == 1:
                         return
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusTopicPreparer(name_prefix='servicebustest')
     @ServiceBusSubscriptionPreparer(name_prefix='servicebustest', requires_session=True)
     def test_session_basic_topic_subscription_send_and_receive(self, servicebus_namespace_connection_string, servicebus_topic, servicebus_subscription, **kwargs):
```

## Comparing `azure-servicebus-7.9.0a1/tests/test_message.py` & `azure-servicebus-7.9.0b1/tests/test_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # from __future__ import annotations
 import os
-import uamqp
 import pytest
 from datetime import datetime, timedelta
 from azure.servicebus import (
     ServiceBusClient,
     ServiceBusMessage,
     ServiceBusReceivedMessage,
     ServiceBusMessageState,
@@ -300,15 +299,15 @@
             outgoing_message.message.accept()
         with pytest.raises(TypeError):
             outgoing_message.message.release()
         with pytest.raises(TypeError):
             outgoing_message.message.reject()
         with pytest.raises(TypeError):
             outgoing_message.message.modify(True, True)
-        assert outgoing_message.message.state == uamqp.constants.MessageState.SendComplete
+        # assert outgoing_message.message.state == uamqp.constants.MessageState.SendComplete
         assert outgoing_message.message.settled
         assert outgoing_message.message.delivery_annotations is None
         assert outgoing_message.message.delivery_no is None
         assert outgoing_message.message.delivery_tag is None
         assert outgoing_message.message.on_send_complete is None
         assert outgoing_message.message.footer is None
         assert outgoing_message.message.retries >= 0
@@ -342,15 +341,15 @@
         # TODO: Test updating message and resending
         with sb_client.get_queue_receiver(queue_name,
                                             receive_mode=ServiceBusReceiveMode.RECEIVE_AND_DELETE,
                                             max_wait_time=10) as receiver:
             batch = receiver.receive_messages()
             incoming_message = batch[0]
             assert incoming_message.message
-            assert incoming_message.message.state == uamqp.constants.MessageState.ReceivedSettled
+            # assert incoming_message.message.state == uamqp.constants.MessageState.ReceivedSettled
             assert incoming_message.message.settled
             assert incoming_message.message.delivery_annotations == {}
             assert incoming_message.message.delivery_no >= 1
             assert incoming_message.message.delivery_tag is None
             assert incoming_message.message.on_send_complete is None
             assert incoming_message.message.footer is None
             assert incoming_message.message.retries >= 0
@@ -428,15 +427,15 @@
             outgoing_message.message.accept()
         with pytest.raises(TypeError):
             outgoing_message.message.release()
         with pytest.raises(TypeError):
             outgoing_message.message.reject()
         with pytest.raises(TypeError):
             outgoing_message.message.modify(True, True)
-        assert outgoing_message.message.state == uamqp.constants.MessageState.SendComplete
+        # assert outgoing_message.message.state == uamqp.constants.MessageState.SendComplete
         assert outgoing_message.message.settled
         assert outgoing_message.message.delivery_annotations is None
         assert outgoing_message.message.delivery_no is None
         assert outgoing_message.message.delivery_tag is None
         assert outgoing_message.message.on_send_complete is None
         assert outgoing_message.message.footer is None
         assert outgoing_message.message.retries >= 0
@@ -469,15 +468,15 @@
     
         with sb_client.get_queue_receiver(queue_name,
                                             receive_mode=ServiceBusReceiveMode.PEEK_LOCK,
                                             max_wait_time=10) as receiver:
             batch = receiver.receive_messages()       
             incoming_message = batch[0]
             assert incoming_message.message
-            assert incoming_message.message.state == uamqp.constants.MessageState.ReceivedUnsettled
+            # assert incoming_message.message.state == uamqp.constants.MessageState.ReceivedUnsettled
             assert not incoming_message.message.settled
             assert incoming_message.message.delivery_annotations[b'x-opt-lock-token']
             assert incoming_message.message.delivery_no >= 1
             assert incoming_message.message.delivery_tag
             assert incoming_message.message.on_send_complete is None
             assert incoming_message.message.footer is None
             assert incoming_message.message.retries >= 0
@@ -511,15 +510,15 @@
             assert incoming_message.message.properties.creation_time
             assert incoming_message.message.properties.group_id == b'id_session'
             assert incoming_message.message.properties.group_sequence is None
             assert incoming_message.message.properties.reply_to_group_id == b'reply to session'
             assert incoming_message.message.properties.get_properties_obj().message_id
             assert incoming_message.message.accept()
             # TODO: State isn't updated if settled correctly via the receiver.
-            assert incoming_message.message.state == uamqp.constants.MessageState.ReceivedSettled
+            # assert incoming_message.message.state == uamqp.constants.MessageState.ReceivedSettled
             assert incoming_message.message.settled
             assert not incoming_message.message.release()
             assert not incoming_message.message.reject()
             assert not incoming_message.message.modify(True, True)
 
     @pytest.mark.skip("unskip after adding PyamqpTransport + pass in _to_outgoing_amqp_message to LegacyMessage")
     @pytest.mark.liveTest
@@ -544,15 +543,15 @@
 
         with sb_client.get_queue_receiver(queue_name,
                                             receive_mode=ServiceBusReceiveMode.RECEIVE_AND_DELETE,
                                             max_wait_time=10) as receiver:
             batch = receiver.receive_messages()
             incoming_message = batch[0]
             assert incoming_message.message
-            assert incoming_message.message.state == uamqp.constants.MessageState.ReceivedSettled
+            # assert incoming_message.message.state == uamqp.constants.MessageState.ReceivedSettled
             assert incoming_message.message.settled
             with pytest.raises(Exception):
                 incoming_message.message.gather()
             assert incoming_message.message.get_data() == {b"key": b"value"}
             assert not incoming_message.message.accept()
             assert not incoming_message.message.release()
             assert not incoming_message.message.reject()
@@ -581,24 +580,24 @@
 
         with sb_client.get_queue_receiver(queue_name,
                                             receive_mode=ServiceBusReceiveMode.PEEK_LOCK,
                                             max_wait_time=10) as receiver:
             batch = receiver.receive_messages()       
             incoming_message = batch[0]
             assert incoming_message.message
-            assert incoming_message.message.state == uamqp.constants.MessageState.ReceivedUnsettled
+            # assert incoming_message.message.state == uamqp.constants.MessageState.ReceivedUnsettled
             assert not incoming_message.message.settled
             assert incoming_message.message.delivery_annotations[b'x-opt-lock-token']
             assert incoming_message.message.delivery_no >= 1
             assert incoming_message.message.delivery_tag
             with pytest.raises(Exception):
                 incoming_message.message.gather()
             assert incoming_message.message.get_data() == {b"key": b"value"}
             assert incoming_message.message.accept()
-            assert incoming_message.message.state == uamqp.constants.MessageState.ReceivedSettled
+            # assert incoming_message.message.state == uamqp.constants.MessageState.ReceivedSettled
             assert incoming_message.message.settled
             assert not incoming_message.message.release()
             assert not incoming_message.message.reject()
             assert not incoming_message.message.modify(True, True)
 
     @pytest.mark.skip("unskip after adding PyamqpTransport + pass in _to_outgoing_amqp_message to LegacyMessage")
     @pytest.mark.liveTest
@@ -623,15 +622,15 @@
 
         with sb_client.get_queue_receiver(queue_name,
                                             receive_mode=ServiceBusReceiveMode.RECEIVE_AND_DELETE,
                                             max_wait_time=10) as receiver:
             batch = receiver.receive_messages()
             incoming_message = batch[0]
             assert incoming_message.message
-            assert incoming_message.message.state == uamqp.constants.MessageState.ReceivedSettled
+            # assert incoming_message.message.state == uamqp.constants.MessageState.ReceivedSettled
             assert incoming_message.message.settled
             with pytest.raises(Exception):
                 incoming_message.message.gather()
             assert list(incoming_message.message.get_data()) == [[1, 2, 3]]
             assert not incoming_message.message.accept()
             assert not incoming_message.message.release()
             assert not incoming_message.message.reject()
@@ -660,23 +659,23 @@
 
         with sb_client.get_queue_receiver(queue_name,
                                             receive_mode=ServiceBusReceiveMode.PEEK_LOCK,
                                             max_wait_time=10) as receiver:
             batch = receiver.receive_messages()       
             incoming_message = batch[0]
             assert incoming_message.message
-            assert incoming_message.message.state == uamqp.constants.MessageState.ReceivedUnsettled
+            # assert incoming_message.message.state == uamqp.constants.MessageState.ReceivedUnsettled
             assert not incoming_message.message.settled
             assert incoming_message.message.delivery_annotations[b'x-opt-lock-token']
             assert incoming_message.message.delivery_no >= 1
             assert incoming_message.message.delivery_tag
             with pytest.raises(Exception):
                 incoming_message.message.gather()
             assert list(incoming_message.message.get_data()) == [[1, 2, 3]]
             assert incoming_message.message.accept()
-            assert incoming_message.message.state == uamqp.constants.MessageState.ReceivedSettled
+            # assert incoming_message.message.state == uamqp.constants.MessageState.ReceivedSettled
             assert incoming_message.message.settled
             assert not incoming_message.message.release()
             assert not incoming_message.message.reject()
             assert not incoming_message.message.modify(True, True)
 
     # TODO: Add batch message backcompat tests
```

## Comparing `azure-servicebus-7.9.0a1/tests/test_sb_client.py` & `azure-servicebus-7.9.0b1/tests/test_sb_client.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/tests/test_topic.py` & `azure-servicebus-7.9.0b1/tests/test_topic.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/tests/test_queues.py` & `azure-servicebus-7.9.0b1/tests/test_queues.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 # A note regarding live_test_only.
 # Old servicebus tests were not written to work on both stubs and live entities.
 # This disables those tests for non-live scenarios, and should be removed as tests
 # are ported to offline-compatible code.
 class ServiceBusQueueTests(AzureMgmtTestCase):
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     def test_receive_and_delete_reconnect_interaction(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         # Note: This test was to guard against github issue 7079
@@ -90,15 +90,15 @@
             count = len(batch)
 
             for message in receiver:
                _logger.debug(message)
                count += 1
             assert count == 5
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer()
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @CachedServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True, lock_duration='PT5S')
     def test_github_issue_6178(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         with ServiceBusClient.from_connection_string(
@@ -113,15 +113,15 @@
                             _logger.debug(message)
                             _logger.debug(message.sequence_number)
                             _logger.debug(message.enqueued_time_utc)
                             _logger.debug(message._lock_expired)
                             receiver.complete_message(message)
                             time.sleep(10)
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True, lock_duration='PT10S')
     def test_queue_by_queue_client_conn_str_receive_handler_peeklock(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         with ServiceBusClient.from_connection_string(
@@ -203,15 +203,15 @@
             with pytest.raises(ValueError):
                 receiver.receive_deferred_messages([1, 2, 3])
             with pytest.raises(ValueError):
                 receiver.peek_messages()
 
             assert count == 10
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    # @pytest.mark.skip(reason="TODO: Pyamqp Message Serialization Error")
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True, lock_duration='PT10S')
     def test_queue_by_queue_client_conn_str_receive_handler_release_messages(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         with ServiceBusClient.from_connection_string(
@@ -311,28 +311,28 @@
                     outter_recv_cnt = 0
                     for msg in receiver:
                         assert msg.delivery_count == 0
                         outter_recv_cnt += 1
                         receiver.complete_message(msg)
                     assert outter_recv_cnt == 4
 
+
+            def _hack_disable_receive_context_message_received(self, frame, message):
+                # pylint: disable=protected-access
+                self._handler._received_messages.put((frame, message))
+
             def sub_test_non_releasing_messages():
                 # test not releasing messages when prefetch is not 1
                 receiver = sb_client.get_queue_receiver(servicebus_queue.name)
                 sender = sb_client.get_queue_sender(servicebus_queue.name)
 
-                def _hack_disable_receive_context_message_received(self, message):
-                    # pylint: disable=protected-access
-                    self._handler._was_message_received = True
-                    self._handler._received_messages.put(message)
-
                 with sender, receiver:
                     # send 5 msgs to queue first
                     sender.send_messages([ServiceBusMessage('test') for _ in range(5)])
-                    receiver._handler.message_handler.on_message_received = types.MethodType(
+                    receiver._handler._link._on_transfer = types.MethodType(
                         _hack_disable_receive_context_message_received, receiver)
                     received_msgs = []
                     while len(received_msgs) < 5:
                         # issue 10 link credits, client should consume 5 msgs from the service
                         # leaving 5 credits on the wire
                         for msg in receiver.receive_messages(max_message_count=10, max_wait_time=5):
                             receiver.complete_message(msg)
@@ -346,14 +346,15 @@
                     # issue 5 link credits, client should consume 5 msgs from the internal buffer which is already lock expired
                     target_msgs_count = 5
                     received_msgs = []
                     while len(received_msgs) < target_msgs_count:
                         received_msgs.extend(receiver.receive_messages(max_message_count=5, max_wait_time=5))
                     assert len(received_msgs) == 5
                     for msg in received_msgs:
+                        # queue ordering I think
                         assert msg.delivery_count == 0
                         with pytest.raises(ServiceBusError):
                             receiver.complete_message(msg)
 
                     # re-received message with delivery count increased
                     target_msgs_count = 5
                     received_msgs = []
@@ -364,15 +365,15 @@
                         assert msg.delivery_count > 0
                         receiver.complete_message(msg)
 
             sub_test_releasing_messages()
             sub_test_releasing_messages_iterator()
             sub_test_non_releasing_messages()
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     def test_queue_by_queue_client_send_multiple_messages(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         with ServiceBusClient.from_connection_string(
@@ -429,15 +430,15 @@
                 with receiver:
                     raise AssertionError("Should raise ValueError")
             with pytest.raises(ValueError):
                 receiver.receive_deferred_messages([1, 2, 3])
             with pytest.raises(ValueError):
                 receiver.peek_messages()
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True, lock_duration='PT10S')
     def test_queue_by_queue_client_conn_str_receive_handler_receiveanddelete(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         
@@ -480,15 +481,15 @@
             with sb_client.get_queue_receiver(servicebus_queue.name, 
                                               receive_mode=ServiceBusReceiveMode.RECEIVE_AND_DELETE, 
                                               max_wait_time=5) as receiver:
                 for message in receiver:
                     messages.append(message)
                 assert len(messages) == 0
     
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     def test_queue_by_queue_client_conn_str_receive_handler_with_stop(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         
@@ -517,15 +518,15 @@
                     receiver.complete_message(message)
                     if len(messages) >= 5:
                         break
 
             assert not receiver._running
             assert len(messages) == 6
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     def test_queue_by_servicebus_client_iter_messages_simple(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         
@@ -551,15 +552,15 @@
                         receiver.renew_message_lock(message)
                     count += 1
 
                 with pytest.raises(StopIteration):
                     next(receiver)
             assert count == 10
     
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     def test_queue_by_servicebus_conn_str_client_iter_messages_with_abandon(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         
@@ -589,15 +590,15 @@
                 count = 0
                 for message in receiver:
                     print_message(_logger, message)
                     receiver.complete_message(message)
                     count += 1
             assert count == 0
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     def test_queue_by_servicebus_client_iter_messages_with_defer(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         
@@ -627,15 +628,15 @@
                 count = 0
                 for message in receiver:
                     print_message(_logger, message)
                     receiver.complete_message(message)
                     count += 1
             assert count == 0
     
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     def test_queue_by_servicebus_client_iter_messages_with_retrieve_deferred_client(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
     
@@ -665,15 +666,15 @@
                 for message in deferred:
                     assert isinstance(message, ServiceBusReceivedMessage)
                     receiver.complete_message(message)
                 
                 with pytest.raises(ServiceBusError):
                     receiver.receive_deferred_messages(deferred_messages)
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     def test_queue_by_servicebus_client_iter_messages_with_retrieve_deferred_receiver_complete(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
     
@@ -707,15 +708,15 @@
                     assert isinstance(message, ServiceBusReceivedMessage)
                     assert message.lock_token
                     assert message.locked_until_utc
                     assert message._receiver
                     receiver.renew_message_lock(message)
                     receiver.complete_message(message)
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     def test_queue_by_servicebus_client_iter_messages_with_retrieve_deferred_receiver_deadletter(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         with ServiceBusClient.from_connection_string(
@@ -756,15 +757,15 @@
                     assert message.dead_letter_reason == 'Testing reason'
                     assert message.dead_letter_error_description == 'Testing description'
                     assert message.application_properties[b'DeadLetterReason'] == b'Testing reason'
                     assert message.application_properties[b'DeadLetterErrorDescription'] == b'Testing description'
                     receiver.complete_message(message)
             assert count == 10
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     def test_queue_by_servicebus_client_iter_messages_with_retrieve_deferred_receiver_deletemode(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         with ServiceBusClient.from_connection_string(
@@ -792,15 +793,15 @@
                 for message in deferred:
                     assert isinstance(message, ServiceBusReceivedMessage)
                     with pytest.raises(ValueError):
                         receiver.complete_message(message)
                 with pytest.raises(ServiceBusError):
                     deferred = receiver.receive_deferred_messages(deferred_messages)
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     def test_queue_by_servicebus_client_iter_messages_with_retrieve_deferred_not_found(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         with ServiceBusClient.from_connection_string(
@@ -827,15 +828,15 @@
     
                 with pytest.raises(ServiceBusError):
                     deferred = receiver.receive_deferred_messages([3, 4])
     
                 with pytest.raises(ServiceBusError):
                     deferred = receiver.receive_deferred_messages([5, 6, 7])
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     def test_queue_by_servicebus_client_receive_batch_with_deadletter(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
 
@@ -885,15 +886,15 @@
                     count += 1
                     assert message.dead_letter_reason == 'Testing reason'
                     assert message.dead_letter_error_description == 'Testing description'
                     assert message.application_properties[b'DeadLetterReason'] == b'Testing reason'
                     assert message.application_properties[b'DeadLetterErrorDescription'] == b'Testing description'
                 assert count == 10
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     def test_queue_by_servicebus_client_receive_batch_with_retrieve_deadletter(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
     
@@ -978,15 +979,15 @@
                 assert len(messages) == 5
                 assert all(isinstance(m, ServiceBusReceivedMessage) for m in messages)
                 for message in messages:
                     print_message(_logger, message)
                     with pytest.raises(ValueError):
                         receiver.complete_message(message)
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    @pytest.mark.skip(reason="TODO: Pyamqp Message Serialization Error")
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     def test_queue_by_servicebus_client_browse_messages_with_receiver(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
     
@@ -1122,15 +1123,15 @@
                     receiver.complete_message(messages[0])
                     receiver.complete_message(messages[1])
                     assert (messages[2].locked_until_utc - utc_now()) <= timedelta(seconds=60)
                     sleep_until_expired(messages[2])
                     with pytest.raises(ServiceBusError):
                         receiver.complete_message(messages[2])
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True, lock_duration='PT10S')
     def test_queue_by_queue_client_conn_str_receive_handler_with_autolockrenew(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         
@@ -1240,15 +1241,15 @@
 
                 for msg in received_msgs:
                     receiver.complete_message(msg)
             assert len(received_msgs) == 3
             assert renewer._is_max_workers_greater_than_one
             renewer.close()
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True, lock_duration='PT10S')
     def test_queue_by_queue_client_conn_str_receive_handler_with_auto_autolockrenew(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         
@@ -1295,15 +1296,15 @@
                             assert message.delivery_count >= 1
                             print("Remaining messages", message.locked_until_utc, utc_now())
                             messages.append(message)
                             receiver.complete_message(message)
             renewer.close()
             assert len(messages) == 11
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     def test_queue_message_time_to_live(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         
@@ -1330,15 +1331,15 @@
                 count = 0
                 for message in dl_receiver:
                     print_message(_logger, message)
                     dl_receiver.complete_message(message)
                     count += 1
             assert count == 1
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_duplicate_detection=True, dead_lettering_on_message_expiration=True)
     def test_queue_message_duplicate_detection(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         
@@ -1580,15 +1581,15 @@
                         assert len(messages) == 1
                     finally:
                         for message in messages:
                             receiver.complete_message(message)
                 else:
                     raise Exception("Failed to receive schdeduled message.")
             
-    @pytest.mark.skip(reason="TODO: iterator support")
+    @pytest.mark.skip(reason="TODO: Pyamqp Message Serialization Error")
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     def test_queue_schedule_multiple_messages(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
 
@@ -1922,36 +1923,36 @@
 
         assert received_message.scheduled_enqueue_time_utc == new_scheduled_time
 
         received_message.scheduled_enqueue_time_utc = None
 
         assert message.scheduled_enqueue_time_utc is None
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    # @pytest.mark.skip(reason="TODO: Pyamqp Message Serialization Error")
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     def test_queue_receive_batch_without_setting_prefetch(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         with ServiceBusClient.from_connection_string(
                 servicebus_namespace_connection_string, logging_enable=False) as sb_client:
 
             def message_content():
                 for i in range(20):
                     yield ServiceBusMessage(
                         body="Test message",
-                        application_properties={'key': 'value'},
+                        # application_properties={'key': 'value'},
                         subject='1st',
-                        content_type='application/text',
-                        correlation_id='cid',
-                        message_id='mid',
-                        to='to',
-                        reply_to='reply_to',
-                        time_to_live=timedelta(seconds=60)
+                        # content_type='application/text',
+                        # correlation_id='cid',
+                        # message_id='mid',
+                        # to='to',
+                        # reply_to='reply_to',
+                        # time_to_live=timedelta(seconds=60)
                     )
 
             sender = sb_client.get_queue_sender(servicebus_queue.name)
             receiver = sb_client.get_queue_receiver(servicebus_queue.name)
 
             with sender, receiver:
                 message = ServiceBusMessageBatch()
@@ -1967,37 +1968,37 @@
                     for message in receiver._get_streaming_message_iter(max_wait_time=10):
                         messages.append(message)
                     if not messages:
                         break
                     receive_counter += 1
                     for message in messages:
                         print_message(_logger, message)
-                        assert b''.join(message.body) == b'Test message'
-                        assert message.application_properties[b'key'] == b'value'
-                        assert message.content_type == 'application/text'
-                        assert message.correlation_id == 'cid'
-                        assert message.message_id == 'mid'
-                        assert message.to == 'to'
-                        assert message.reply_to == 'reply_to'
-                        assert message.time_to_live == timedelta(seconds=60)
+                        # assert b''.join(message.body) == b'Test message'
+                        # assert message.application_properties[b'key'] == b'value'
+                        # assert message.content_type == 'application/text'
+                        # assert message.correlation_id == 'cid'
+                        # assert message.message_id == 'mid'
+                        # assert message.to == 'to'
+                        # assert message.reply_to == 'reply_to'
+                        # assert message.time_to_live == timedelta(seconds=60)
 
                         if message.subject == '1st':
                             message_1st_received_cnt += 1
                             receiver.complete_message(message)
                             message.subject = '2nd'
                             sender.send_messages(message)  # resending received message
                         elif message.subject == '2nd':
                             message_2nd_received_cnt += 1
                             receiver.complete_message(message)
 
                 assert message_1st_received_cnt == 20 and message_2nd_received_cnt == 20
                 # Network/server might be unstable making flow control ineffective in the leading rounds of connection iteration
                 assert receive_counter < 10  # Dynamic link credit issuing come info effect
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest')
     def test_queue_receiver_alive_after_timeout(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         with ServiceBusClient.from_connection_string(
@@ -2041,15 +2042,15 @@
 
                     for message in messages[2:]:
                         receiver.complete_message(message)
 
                     messages = receiver.receive_messages()
                     assert not messages
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True, lock_duration='PT5M')
     def test_queue_receive_keep_conn_alive(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         with ServiceBusClient.from_connection_string(
@@ -2077,15 +2078,15 @@
                 messages = []
                 for message in receiver:
                     messages.append(message)
 
                 assert len(messages) == 0  # make sure messages are removed from the queue
                 assert receiver_handler == receiver._handler  # make sure no reconnection happened
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest')
     def test_queue_receiver_sender_resume_after_link_timeout(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         with ServiceBusClient.from_connection_string(
@@ -2104,15 +2105,15 @@
                 messages = []
                 with sb_client.get_queue_receiver(servicebus_queue.name, max_wait_time=5) as receiver:
                     
                     for message in receiver._get_streaming_message_iter():
                         messages.append(message)
                 assert len(messages) == 2
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    # @pytest.mark.skip(reason="TODO: _counter doesn't exist in pyamqp")
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest')
     def test_queue_receiver_respects_max_wait_time_overrides(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         with ServiceBusClient.from_connection_string(
@@ -2122,45 +2123,45 @@
             with sb_client.get_queue_sender(servicebus_queue.name) as sender:
                 message = ServiceBusMessage("0")
                 sender.send_messages(message)
 
                 messages = []
                 with sb_client.get_queue_receiver(servicebus_queue.name, max_wait_time=5) as receiver:
 
-                    time_1 = receiver._handler._counter.get_current_ms()
+                    time_1 = time.time()
                     time_3 = time_1 # In case inner loop isn't hit, fail sanely.
                     for message in receiver._get_streaming_message_iter(max_wait_time=10):
                         messages.append(message)
                         receiver.complete_message(message)
 
-                        time_2 = receiver._handler._counter.get_current_ms()
+                        time_2 = time.time()
                         for message in receiver._get_streaming_message_iter(max_wait_time=1):
                             messages.append(message)
-                        time_3 = receiver._handler._counter.get_current_ms()
-                        assert timedelta(seconds=.5) < timedelta(milliseconds=(time_3 - time_2)) <= timedelta(seconds=2)
-                    time_4 = receiver._handler._counter.get_current_ms()
-                    assert timedelta(seconds=8) < timedelta(milliseconds=(time_4 - time_3)) <= timedelta(seconds=11)
+                        time_3 = time.time()
+                        assert timedelta(seconds=.5) < timedelta(seconds=(time_3 - time_2)) <= timedelta(seconds=2)
+                    time_4 = time.time()
+                    assert timedelta(seconds=8) < timedelta(seconds=(time_4 - time_3)) <= timedelta(seconds=11)
 
                     for message in receiver._get_streaming_message_iter(max_wait_time=3):
                         messages.append(message)
-                    time_5 = receiver._handler._counter.get_current_ms()
-                    assert timedelta(seconds=1) < timedelta(milliseconds=(time_5 - time_4)) <= timedelta(seconds=4)
+                    time_5 = time.time()
+                    assert timedelta(seconds=1) < timedelta(seconds=(time_5 - time_4)) <= timedelta(seconds=4)
 
                     for message in receiver:
                         messages.append(message)
-                    time_6 = receiver._handler._counter.get_current_ms()
-                    assert timedelta(seconds=3) < timedelta(milliseconds=(time_6 - time_5)) <= timedelta(seconds=6)
+                    time_6 = time.time()
+                    assert timedelta(seconds=3) < timedelta(seconds=(time_6 - time_5)) <= timedelta(seconds=6)
 
                     for message in receiver._get_streaming_message_iter():
                         messages.append(message)
-                    time_7 = receiver._handler._counter.get_current_ms()
-                    assert timedelta(seconds=3) < timedelta(milliseconds=(time_7 - time_6)) <= timedelta(seconds=6)
+                    time_7 = time.time()
+                    assert timedelta(seconds=3) < timedelta(seconds=(time_7 - time_6)) <= timedelta(seconds=6)
                     assert len(messages) == 1
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest')
     def test_queue_send_twice(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         with ServiceBusClient.from_connection_string(
@@ -2372,15 +2373,15 @@
 
                     receiver._settle_message = origin_sb_receiver_settle_message_method
                     message = receiver.receive_messages(max_wait_time=6)[0]
                     receiver.complete_message(message)
             finally:
                 client.ReceiveClient.settle_messages = original_settlement
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     def test_send_message_no_body(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         sb_client = ServiceBusClient.from_connection_string(
@@ -2434,15 +2435,15 @@
                 pass
             with pytest.raises(ValueError):
                 with sb_client.get_queue_receiver(servicebus_queue.name, 
                                                   sub_queue=str.upper(ServiceBusSubQueue.DEAD_LETTER.value),
                                                   max_wait_time=5) as receiver:
                     raise Exception("Should not get here, should be case sensitive.")
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest')
     def test_queue_send_dict_messages(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         with ServiceBusClient.from_connection_string(
@@ -2468,15 +2469,15 @@
 
                 received_messages = []
                 with sb_client.get_queue_receiver(servicebus_queue.name, max_wait_time=5) as receiver:
                     for message in receiver:
                         received_messages.append(message)
                 assert len(received_messages) == 6
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest')
     def test_queue_send_mapping_messages(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         class MappingMessage(DictMixin):
@@ -2628,39 +2629,38 @@
                     message2_dict = {"message_id": message_id2, "bad_key": content}
                     list_message_dicts = [message_dict, message2_dict]
                     with pytest.raises(TypeError):
                         sender.schedule_messages(message_dict, scheduled_enqueue_time)
                     with pytest.raises(TypeError):
                         sender.schedule_messages(list_message_dicts, scheduled_enqueue_time)
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     def test_queue_receive_iterator_resume_after_link_detach(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
 
-        def hack_iter_next_mock_error(self):
+        def hack_iter_next_mock_error(self, wait_time=None):
             try:
                 self._receive_context.set()
                 self._open()
                 # when trying to receive the second message (execution_times is 1), raising LinkDetach error to mock 10 mins idle timeout
                 if self.execution_times == 1:
-                    from uamqp.errors import LinkDetach
-                    from uamqp.constants import ErrorCodes
+                    from azure.servicebus._pyamqp.error import ErrorCondition, AMQPLinkError
                     self.execution_times += 1
                     self.error_raised = True
-                    raise LinkDetach(ErrorCodes.LinkDetachForced)
+                    raise AMQPLinkError(condition=ErrorCondition.LinkDetachForced)
                 else:
                     self.execution_times += 1
                 if not self._message_iter:
-                    self._message_iter = self._handler.receive_messages_iter()
-                uamqp_message = next(self._message_iter)
-                message = self._build_message(uamqp_message)
+                    self._message_iter = self._handler.receive_messages_iter(timeout=wait_time)
+                pyamqp_message = next(self._message_iter)
+                message = self._build_message(pyamqp_message)
                 return message
             finally:
                 self._receive_context.clear()
 
         with ServiceBusClient.from_connection_string(
                 servicebus_namespace_connection_string, logging_enable=False) as sb_client:
             with sb_client.get_queue_sender(servicebus_queue.name) as sender:
@@ -2675,15 +2675,15 @@
                 for msg in receiver:
                     receiver.complete_message(msg)
                     res.append(msg)
                 assert len(res) == 3
                 assert receiver.error_raised
                 assert receiver.execution_times >= 4  # at least 1 failure and 3 successful receiving iterator
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     def test_queue_send_amqp_annotated_message(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
 
@@ -2727,16 +2727,16 @@
             with pytest.raises(ValueError):
                 AmqpAnnotatedMessage()
 
             content = "normalmessage"
             dict_message = {"body": content}
             sb_message = ServiceBusMessage(body=content)
             message_with_ttl = AmqpAnnotatedMessage(data_body=data_body, header=AmqpMessageHeader(time_to_live=60000))
-            uamqp_with_ttl = message_with_ttl._to_outgoing_amqp_message()
-            assert uamqp_with_ttl.properties.absolute_expiry_time == uamqp_with_ttl.properties.creation_time + uamqp_with_ttl.header.ttl
+            pyamqp_with_ttl = message_with_ttl._to_outgoing_amqp_message()
+            assert pyamqp_with_ttl.properties.absolute_expiry_time == pyamqp_with_ttl.properties.creation_time + pyamqp_with_ttl.header.ttl
 
             recv_data_msg = recv_sequence_msg = recv_value_msg = normal_msg = 0
             with sb_client.get_queue_receiver(servicebus_queue.name, max_wait_time=10) as receiver:
                 with sb_client.get_queue_sender(servicebus_queue.name) as sender:
                     batch = sender.create_message_batch()
                     batch.add_message(data_message)
                     batch.add_message(value_message)
```

## Comparing `azure-servicebus-7.9.0a1/tests/mocks.py` & `azure-servicebus-7.9.0b1/tests/mocks.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/tests/sb_env_loader.py` & `azure-servicebus-7.9.0b1/tests/sb_env_loader.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/tests/test_subscriptions.py` & `azure-servicebus-7.9.0b1/tests/test_subscriptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 )
 from utilities import get_logger, print_message
 
 _logger = get_logger(logging.DEBUG)
 
 
 class ServiceBusSubscriptionTests(AzureMgmtTestCase):
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusTopicPreparer(name_prefix='servicebustest')
     @ServiceBusSubscriptionPreparer(name_prefix='servicebustest')
     def test_subscription_by_subscription_client_conn_str_receive_basic(self, servicebus_namespace_connection_string, servicebus_topic, servicebus_subscription, **kwargs):
@@ -68,15 +68,15 @@
 
                 count = 0
                 for message in receiver:
                     count += 1
                     receiver.complete_message(message)
             assert count == 1
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusTopicPreparer(name_prefix='servicebustest')
     @ServiceBusSubscriptionPreparer(name_prefix='servicebustest')
     def test_subscription_by_sas_token_credential_conn_str_send_basic(self, servicebus_namespace, servicebus_namespace_key_name, servicebus_namespace_primary_key, servicebus_topic, servicebus_subscription, **kwargs):
@@ -122,15 +122,15 @@
 
         subs = client.list_subscriptions(servicebus_topic.name)
         assert len(subs) >= 1
         # assert all(isinstance(s, SubscriptionClient) for s in subs)
         assert subs[0].name == servicebus_subscription.name
         assert subs[0].topic_name == servicebus_topic.name
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusTopicPreparer(name_prefix='servicebustest')
     @ServiceBusSubscriptionPreparer(name_prefix='servicebustest')
     def test_subscription_by_servicebus_client_receive_batch_with_deadletter(self, servicebus_namespace_connection_string, servicebus_topic, servicebus_subscription, **kwargs):
```

## Comparing `azure-servicebus-7.9.0a1/tests/livetest/test_errors.py` & `azure-servicebus-7.9.0b1/tests/livetest/test_errors.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/tests/async_tests/test_subscriptions_async.py` & `azure-servicebus-7.9.0b1/tests/async_tests/test_subscriptions_async.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 )
 from utilities import get_logger, print_message
 
 _logger = get_logger(logging.DEBUG)
 
 
 class ServiceBusSubscriptionAsyncTests(AzureMgmtTestCase):
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusTopicPreparer(name_prefix='servicebustest')
     @ServiceBusSubscriptionPreparer(name_prefix='servicebustest')
     async def test_subscription_by_subscription_client_conn_str_receive_basic(self, servicebus_namespace_connection_string, servicebus_topic, servicebus_subscription, **kwargs):
@@ -69,15 +70,16 @@
 
                 count = 0
                 async for message in receiver:
                     count += 1
                     await receiver.complete_message(message)
             assert count == 1
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusTopicPreparer(name_prefix='servicebustest')
     @ServiceBusSubscriptionPreparer(name_prefix='servicebustest')
     async def test_subscription_by_sas_token_credential_conn_str_send_basic(self, servicebus_namespace, servicebus_namespace_key_name, servicebus_namespace_primary_key, servicebus_topic, servicebus_subscription, **kwargs):
@@ -102,15 +104,16 @@
             ) as receiver:
                 count = 0
                 async for message in receiver:
                     count += 1
                     await receiver.complete_message(message)
             assert count == 1
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusTopicPreparer(name_prefix='servicebustest')
     @ServiceBusSubscriptionPreparer(name_prefix='servicebustest')
     async def test_topic_by_servicebus_client_receive_batch_with_deadletter(self, servicebus_namespace_connection_string, servicebus_topic, servicebus_subscription, **kwargs):
```

## Comparing `azure-servicebus-7.9.0a1/tests/async_tests/test_sb_client_async.py` & `azure-servicebus-7.9.0b1/tests/async_tests/test_sb_client_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 )
 from utilities import get_logger
 
 _logger = get_logger(logging.DEBUG)
 
 class ServiceBusClientAsyncTests(AzureMgmtTestCase):
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @CachedServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_sb_client_bad_credentials_async(self, servicebus_namespace, servicebus_queue, **kwargs):
         client = ServiceBusClient(
@@ -47,27 +48,29 @@
             credential=ServiceBusSharedKeyCredential('invalid', 'invalid'),
             logging_enable=False)
         async with client:
             with pytest.raises(ServiceBusAuthenticationError):
                 async with client.get_queue_sender(servicebus_queue.name) as sender:
                     await sender.send_messages(ServiceBusMessage("test"))
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     async def test_sb_client_bad_namespace_async(self, **kwargs):
 
         client = ServiceBusClient(
             fully_qualified_namespace='invalid.servicebus.windows.net',
             credential=ServiceBusSharedKeyCredential('invalid', 'invalid'),
             logging_enable=False)
         async with client:
             with pytest.raises(ServiceBusError):
                 async with client.get_queue_sender('invalidqueue') as sender:
                     await sender.send_messages(ServiceBusMessage("test"))
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     async def test_sb_client_bad_entity_async(self):
         fake_str = "Endpoint=sb://mock.servicebus.windows.net/;" \
                    "SharedAccessKeyName=mock;SharedAccessKey=mock;EntityPath=mockentity"
@@ -94,14 +97,15 @@
                    "SharedAccessKeyName=mock;SharedAccessKey=mock"
         fake_client = ServiceBusClient.from_connection_string(fake_str)
         fake_client.get_queue_sender('queue')
         fake_client.get_queue_receiver('queue')
         fake_client.get_topic_sender('topic')
         fake_client.get_subscription_receiver('topic', 'subscription')
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @CachedServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     @ServiceBusNamespaceAuthorizationRulePreparer(name_prefix='servicebustest', access_rights=[AccessRights.listen])
     async def test_sb_client_readonly_credentials(self, servicebus_authorization_rule_connection_string, servicebus_queue, **kwargs):
@@ -111,14 +115,15 @@
             async with client.get_queue_receiver(servicebus_queue.name) as receiver:
                 messages = await receiver.receive_messages(max_message_count=1, max_wait_time=1)
 
             with pytest.raises(ServiceBusAuthorizationError):
                 async with client.get_queue_sender(servicebus_queue.name) as sender:
                     await sender.send_messages(ServiceBusMessage("test"))
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @CachedServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     @ServiceBusNamespaceAuthorizationRulePreparer(name_prefix='servicebustest', access_rights=[AccessRights.send])
     async def test_sb_client_writeonly_credentials_async(self, servicebus_authorization_rule_connection_string, servicebus_queue, **kwargs):
@@ -131,14 +136,15 @@
 
             async with client.get_queue_sender(servicebus_queue.name) as sender:
                 await sender.send_messages(ServiceBusMessage("test"))
 
                 with pytest.raises(TypeError):
                     await sender.send_messages("cat")
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer()
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @CachedServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     @CachedServiceBusTopicPreparer(name_prefix='servicebustest')
     @CachedServiceBusSubscriptionPreparer(name_prefix='servicebustest')
@@ -220,14 +226,15 @@
             queue_receiver = client.get_queue_receiver(servicebus_queue.name)
             topic_sender = client.get_topic_sender(servicebus_topic.name)
             subscription_receiver = client.get_subscription_receiver(servicebus_topic.name,
                                                                      servicebus_subscription.name)
         assert len(client._handlers) < 15
         await client.close()
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusNamespaceAuthorizationRulePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest_qone', parameter_name='wrong_queue', dead_lettering_on_message_expiration=True)
     @ServiceBusQueuePreparer(name_prefix='servicebustest_qtwo', dead_lettering_on_message_expiration=True)
@@ -275,14 +282,15 @@
 
             async with ServiceBusReceiver._from_connection_string(
                 servicebus_queue_authorization_rule_connection_string,
                 queue_name=servicebus_queue.name,
             ) as receiver:
                 messages = await receiver.receive_messages(max_message_count=1, max_wait_time=1)
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer()
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @CachedServiceBusQueuePreparer(name_prefix='servicebustest')
     async def test_client_sas_credential_async(self,
                                    servicebus_queue,
@@ -302,14 +310,15 @@
 
         client = ServiceBusClient.from_connection_string(token_conn_str)
         async with client:
             assert len(client._handlers) == 0
             async with client.get_queue_sender(servicebus_queue.name) as sender:
                 await sender.send_messages(ServiceBusMessage("foo"))
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer()
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @CachedServiceBusQueuePreparer(name_prefix='servicebustest')
     async def test_client_credential_async(self,
                                    servicebus_queue,
@@ -341,14 +350,15 @@
 
         client = ServiceBusClient(hostname, credential)
         async with client:
             assert len(client._handlers) == 0
             async with client.get_queue_sender(servicebus_queue.name) as sender:
                 await sender.send_messages(ServiceBusMessage("foo"))
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer()
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @CachedServiceBusQueuePreparer(name_prefix='servicebustest')
     async def test_client_azure_sas_credential_async(self,
                                    servicebus_queue,
@@ -367,14 +377,15 @@
 
         client = ServiceBusClient(hostname, credential)
         async with client:
             assert len(client._handlers) == 0
             async with client.get_queue_sender(servicebus_queue.name) as sender:
                 await sender.send_messages(ServiceBusMessage("foo"))
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer()
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @CachedServiceBusQueuePreparer(name_prefix='servicebustest')
     async def test_client_named_key_credential_async(self,
                                    servicebus_queue,
@@ -519,14 +530,15 @@
         servicebus_client = ServiceBusClient.from_connection_string(conn_str=servicebus_connection_str)
         async with servicebus_client:
             subscription_receiver = servicebus_client.get_subscription_receiver(topic_name, sub_name, client_identifier=custom_id)
             assert subscription_receiver.client_identifier is not None
             assert subscription_receiver.client_identifier == custom_id
 
     @pytest.mark.skip('check that connection verify works for pyproto. Issue #26657.')
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @CachedResourceGroupPreparer()
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @CachedServiceBusQueuePreparer(name_prefix='servicebustest')
     async def test_connection_verify_exception_async(self,
                                    servicebus_queue,
                                    servicebus_namespace,
```

## Comparing `azure-servicebus-7.9.0a1/tests/async_tests/test_sessions_async.py` & `azure-servicebus-7.9.0b1/tests/async_tests/test_sessions_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import sys
 import os
 import pytest
 import time
 import uuid
 from datetime import datetime, timedelta
 
-from uamqp.errors import VendorLinkDetach
 from azure.servicebus import (
     ServiceBusMessage,
     ServiceBusReceivedMessage,
     ServiceBusReceiveMode,
     NEXT_AVAILABLE_SESSION,
     ServiceBusSubQueue
 )
@@ -43,15 +42,16 @@
 )
 from utilities import get_logger, print_message
 
 _logger = get_logger(logging.DEBUG)
 
 
 class ServiceBusAsyncSessionTests(AzureMgmtTestCase):
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     async def test_async_session_by_session_client_conn_str_receive_handler_peeklock(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -95,15 +95,16 @@
                 count += 1
                 await receiver.complete_message(message)
 
             await receiver.close()
 
             assert count == 3
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True, lock_duration='PT10S')
     async def test_async_session_by_queue_client_conn_str_receive_handler_receiveanddelete(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -133,15 +134,16 @@
 
             messages = []
             async with sb_client.get_queue_receiver(servicebus_queue.name, session_id=session_id, receive_mode=ServiceBusReceiveMode.RECEIVE_AND_DELETE, max_wait_time=10) as receiver:
                 async for message in receiver:
                     messages.append(message)
             assert len(messages) == 0
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     async def test_async_session_by_session_client_conn_str_receive_handler_with_stop(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -174,29 +176,31 @@
                     await receiver.complete_message(message)
                     if len(messages) >= 5:
                         break
 
             assert not receiver._running
             assert len(messages) == 6
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @pytest.mark.xfail(reason="'Cannot open log' error, potential service bug", raises=ServiceBusError)
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     async def test_async_session_by_session_client_conn_str_receive_handler_with_no_session(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
             servicebus_namespace_connection_string, logging_enable=False) as sb_client:
 
             receiver = sb_client.get_queue_receiver(servicebus_queue.name, session_id=NEXT_AVAILABLE_SESSION, max_wait_time=10)
             with pytest.raises(OperationTimeoutError):
                 await receiver._open_with_retry()
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     async def test_async_session_by_session_client_conn_str_receive_handler_with_inactive_session(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -208,15 +212,16 @@
             async with receiver:
                 async for message in receiver:
                     messages.append(message)
 
             assert not receiver._running
             assert len(messages) == 0
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     async def test_async_session_by_servicebus_client_iter_messages_with_retrieve_deferred_receiver_complete(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -246,15 +251,16 @@
                     assert message.lock_token
                     assert not message.locked_until_utc
                     assert message._receiver
                     with pytest.raises(TypeError):
                         await receiver.renew_message_lock(message)
                     await receiver.complete_message(message)
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     async def test_async_session_by_servicebus_client_iter_messages_with_retrieve_deferred_receiver_deadletter(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -293,15 +299,16 @@
                     assert message.dead_letter_reason == 'Testing reason'
                     assert message.dead_letter_error_description == 'Testing description'
                     assert message.application_properties[b'DeadLetterReason'] == b'Testing reason'
                     assert message.application_properties[b'DeadLetterErrorDescription'] == b'Testing description'
                     await receiver.complete_message(message)
             assert count == 10
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     async def test_async_session_by_servicebus_client_iter_messages_with_retrieve_deferred_receiver_deletemode(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -328,15 +335,16 @@
                 for message in deferred:
                     assert isinstance(message, ServiceBusReceivedMessage)
                     with pytest.raises(ValueError):
                         await receiver.complete_message(message)
                 with pytest.raises(ServiceBusError):
                     deferred = await receiver.receive_deferred_messages(deferred_messages)
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     async def test_async_session_by_servicebus_client_iter_messages_with_retrieve_deferred_client(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -359,15 +367,16 @@
             await receiver.close()
 
             assert count == 10
 
             with pytest.raises(ValueError):
                 await receiver.complete_message(message)
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     async def test_async_session_by_servicebus_client_fetch_next_with_retrieve_deadletter(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -402,14 +411,15 @@
                     assert message.dead_letter_error_description == 'Testing description'
                     assert message.application_properties[b'DeadLetterReason'] == b'Testing reason'
                     assert message.application_properties[b'DeadLetterErrorDescription'] == b'Testing description'
                     await receiver.complete_message(message)
                     count += 1
             assert count == 10
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     async def test_async_session_by_servicebus_client_browse_messages_client(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -435,14 +445,15 @@
                     with pytest.raises(ValueError):
                         await receiver.complete_message(message)
 
             async with sb_client.get_queue_receiver(servicebus_queue.name, session_id=session_id_2) as receiver:
                 messages = await receiver.peek_messages(5)
                 assert len(messages) == 3
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     async def test_async_session_by_servicebus_client_browse_messages_with_receiver(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -459,14 +470,15 @@
                 assert len(messages) > 0
                 assert all(isinstance(m, ServiceBusReceivedMessage) for m in messages)
                 for message in messages:
                     print_message(_logger, message)
                     with pytest.raises(ValueError):
                         await receiver.complete_message(message)
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     async def test_async_session_by_servicebus_client_renew_client_locks(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -500,15 +512,16 @@
                 finally:
                     await receiver.complete_message(messages[0])
                     await receiver.complete_message(messages[1])
                     time.sleep(40)
                     with pytest.raises(SessionLockLostError):
                         await receiver.complete_message(messages[2])
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True, lock_duration='PT5S')
     async def test_async_session_by_conn_str_receive_handler_with_autolockrenew(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -566,15 +579,16 @@
                 renewer.register(receiver, session, max_lock_renewal_duration=5, on_lock_renew_failure=lock_lost_callback)
             await asyncio.sleep(max(0,(session.locked_until_utc - utc_now()).total_seconds()+1)) # If this pattern repeats make sleep_until_expired_async
             assert not results
 
             await renewer.close()
             assert len(messages) == 2
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True, lock_duration='PT10S')
     async def test_async_session_by_conn_str_receive_handler_with_auto_autolockrenew(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -660,15 +674,15 @@
             received_msgs = await receiver.receive_messages(max_wait_time=10)
             for msg in received_msgs:
                 await receiver.complete_message(msg)
 
         await receiver.close()
         assert not renewer._renewable(receiver._session)
 
-
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     async def test_async_session_message_connection_closed(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -684,15 +698,15 @@
             async with sb_client.get_queue_receiver(servicebus_queue.name, session_id=session_id) as receiver:
                 messages = await receiver.receive_messages(max_wait_time=10)
                 assert len(messages) == 1
 
             with pytest.raises(ValueError):
                 await receiver.complete_message(messages[0])
 
-
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     async def test_async_session_message_expiry(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -723,14 +737,15 @@
             async with sb_client.get_queue_receiver(servicebus_queue.name, session_id=session_id) as receiver:
                 messages = await receiver.receive_messages(max_wait_time=30)
                 assert len(messages) == 1
                 print_message(_logger, messages[0])
                 assert messages[0].delivery_count
                 await receiver.complete_message(messages[0])
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     async def test_async_session_schedule_message(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -759,15 +774,15 @@
                     assert messages[0].scheduled_enqueue_time_utc == enqueue_time
                     assert messages[0].scheduled_enqueue_time_utc == messages[0].enqueued_time_utc.replace(microsecond=0)
                     assert len(messages) == 1
                 else:
                     raise Exception("Failed to receive schdeduled message.")
             await renewer.close()
 
-
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     async def test_async_session_schedule_multiple_messages(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -798,15 +813,16 @@
                     assert messages[0].message_id in (message_id_a, message_id_b)
                     assert messages[0].scheduled_enqueue_time_utc == enqueue_time
                     assert messages[0].scheduled_enqueue_time_utc == messages[0].enqueued_time_utc.replace(microsecond=0)
                     assert len(messages) == 2
                 else:
                     raise Exception("Failed to receive schdeduled message.")
             await renewer.close()
-
+   
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     async def test_async_session_cancel_scheduled_messages(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -832,14 +848,15 @@
                 except AssertionError:
                     for message in messages:
                         print(str(message))
                         await receiver.complete_message(message)
                     raise
             await renewer.close()
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @CachedServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     async def test_session_receiver_partially_invalid_autolockrenew_mode(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         session_id = str(uuid.uuid4())
@@ -855,15 +872,16 @@
             async with sb_client.get_queue_receiver(servicebus_queue.name,
                                               session_id=session_id,
                                               receive_mode=ServiceBusReceiveMode.RECEIVE_AND_DELETE,
                                               auto_lock_renewer=AutoLockRenewer()) as receiver:
                 assert receiver.receive_messages()
                 assert not failures
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     async def test_async_session_get_set_state_with_receiver(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -883,14 +901,15 @@
                     assert m.session_id == session_id
                     count += 1
                 state = await receiver.session.get_state()
                 assert state == b'first_state'
             assert count == 3
 
     @pytest.mark.skip(reason='Requires list sessions')
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     async def test_async_session_by_servicebus_client_list_sessions_with_receiver(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -912,14 +931,15 @@
 
             async with sb_client.get_queue_receiver(servicebus_queue.name, session_id=NEXT_AVAILABLE_SESSION, max_wait_time=5, receive_mode=ServiceBusReceiveMode.PEEK_LOCK) as receiver:
                 current_sessions = await receiver.list_sessions(updated_since=start_time)
                 assert len(current_sessions) == 5
                 assert current_sessions == sessions
 
     @pytest.mark.skip(reason="requires list_session")
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     async def test_async_session_by_servicebus_client_list_sessions_with_client(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -939,14 +959,15 @@
                 async with sb_client.get_queue_receiver(servicebus_queue.name, session_id=session) as receiver:
                     await receiver.session.set_state("SESSION {}".format(session))
 
             current_sessions = await sb_client.list_sessions(updated_since=start_time)
             assert len(current_sessions) == 5
             assert current_sessions == sessions
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @pytest.mark.xfail(reason="'Cannot open log' error, potential service bug")
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     async def test_async_session_by_servicebus_client_session_pool(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
@@ -978,15 +999,16 @@
 
             receive_sessions = [message_processing(sb_client) for _ in range(concurrent_receivers)]
             await asyncio.gather(*receive_sessions, return_exceptions=True)
 
             assert not errors
             assert len(messages) == 100
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusTopicPreparer(name_prefix='servicebustest')
     @ServiceBusSubscriptionPreparer(name_prefix='servicebustest', requires_session=True)
     async def test_async_session_basic_topic_subscription_send_and_receive(self, servicebus_namespace_connection_string, servicebus_topic, servicebus_subscription, **kwargs):
@@ -1006,14 +1028,15 @@
             ) as receiver:
                 count = 0
                 async for message in receiver:
                     count += 1
                     await receiver.complete_message(message)
             assert count == 1
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @pytest.mark.xfail(reason="'Cannot open log' error, potential service bug", raises=ServiceBusError)
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     async def test_async_session_connection_failure_is_idempotent(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
@@ -1045,14 +1068,15 @@
 
             async with sb_client.get_queue_receiver(servicebus_queue.name, session_id=NEXT_AVAILABLE_SESSION, max_wait_time=5) as receiver:
                 messages = []
                 async for message in receiver:
                     messages.append(message)
                 assert len(messages) == 1
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @CachedServiceBusQueuePreparer(name_prefix='servicebustest', requires_session=True)
     async def test_async_session_non_session_send_to_session_queue_should_fail(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
```

## Comparing `azure-servicebus-7.9.0a1/tests/async_tests/test_topic_async.py` & `azure-servicebus-7.9.0b1/tests/async_tests/test_topic_async.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 )
 from utilities import get_logger, print_message
 
 _logger = get_logger(logging.DEBUG)
 
 
 class ServiceBusTopicsAsyncTests(AzureMgmtTestCase):
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @CachedServiceBusTopicPreparer(name_prefix='servicebustest')
     async def test_topic_by_servicebus_client_conn_str_send_basic(self, servicebus_namespace_connection_string, servicebus_topic, **kwargs):
 
@@ -40,14 +41,15 @@
             servicebus_namespace_connection_string,
             logging_enable=False
         ) as sb_client:
             async with sb_client.get_topic_sender(servicebus_topic.name) as sender:
                 message = ServiceBusMessage(b"Sample topic message")
                 await sender.send_messages(message)
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @CachedServiceBusTopicPreparer(name_prefix='servicebustest')
     async def test_topic_by_sas_token_credential_conn_str_send_basic(self, servicebus_namespace, servicebus_namespace_key_name, servicebus_namespace_primary_key, servicebus_topic, **kwargs):
         fully_qualified_namespace = servicebus_namespace.name + '.servicebus.windows.net'
```

## Comparing `azure-servicebus-7.9.0a1/tests/async_tests/mocks_async.py` & `azure-servicebus-7.9.0b1/tests/async_tests/mocks_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/tests/async_tests/test_queues_async.py` & `azure-servicebus-7.9.0b1/tests/async_tests/test_queues_async.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,23 +45,24 @@
     MessageLockLostError,
     MessageAlreadySettled,
     AutoLockRenewTimeout,
     MessageSizeExceededError,
     OperationTimeoutError
 )
 from devtools_testutils import AzureMgmtTestCase, CachedResourceGroupPreparer, AzureTestCase
-from servicebus_preparer import CachedServiceBusNamespacePreparer, CachedServiceBusQueuePreparer, ServiceBusQueuePreparer
-from utilities import get_logger, print_message, sleep_until_expired
+from tests.servicebus_preparer import CachedServiceBusNamespacePreparer, CachedServiceBusQueuePreparer, ServiceBusQueuePreparer
+from tests.utilities import get_logger, print_message, sleep_until_expired
 from mocks_async import MockReceivedMessage, MockReceiver
 
 _logger = get_logger(logging.DEBUG)
 
 
 class ServiceBusQueueAsyncTests(AzureMgmtTestCase):
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True, lock_duration='PT10S')
     async def test_async_queue_by_queue_client_conn_str_receive_handler_peeklock(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -119,15 +120,16 @@
                 async with receiver:
                     raise AssertionError("Should raise ValueError")
             with pytest.raises(ValueError):
                 await receiver.receive_deferred_messages([1, 2, 3])
             with pytest.raises(ValueError):
                 await receiver.peek_messages()
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True, lock_duration='PT10S')
     async def test_async_queue_by_queue_client_conn_str_receive_handler_release_messages(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -232,23 +234,22 @@
                     assert outter_recv_cnt == 4
 
             async def sub_test_non_releasing_messages():
                 # test not releasing messages when prefetch is not 1
                 receiver = sb_client.get_queue_receiver(servicebus_queue.name)
                 sender = sb_client.get_queue_sender(servicebus_queue.name)
 
-                def _hack_disable_receive_context_message_received(self, message):
+                async def _hack_disable_receive_context_message_received(self, frame, message):
                     # pylint: disable=protected-access
-                    self._handler._was_message_received = True
-                    self._handler._received_messages.put(message)
+                    self._handler._received_messages.put((frame, message))
 
                 async with sender, receiver:
                     # send 5 msgs to queue first
                     await sender.send_messages([ServiceBusMessage('test') for _ in range(5)])
-                    receiver._handler.message_handler.on_message_received = types.MethodType(
+                    receiver._handler._link._on_transfer = types.MethodType(
                         _hack_disable_receive_context_message_received, receiver)
                     received_msgs = []
                     while len(received_msgs) < 5:
                         # issue 10 link credits, client should consume 5 msgs from the service
                         # leaving 5 credits on the wire
                         for msg in (await receiver.receive_messages(max_message_count=10, max_wait_time=10)):
                             await receiver.complete_message(msg)
@@ -280,15 +281,16 @@
                         assert msg.delivery_count > 0
                         await receiver.complete_message(msg)
 
             await sub_test_releasing_messages()
             await sub_test_releasing_messages_iterator()
             await sub_test_non_releasing_messages()
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_async_queue_by_queue_client_send_multiple_messages(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -328,15 +330,16 @@
                 async with receiver:
                     raise AssertionError("Should raise ValueError")
             with pytest.raises(ValueError):
                 await receiver.receive_deferred_messages([1, 2, 3])
             with pytest.raises(ValueError):
                 await receiver.peek_messages()
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer()
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_github_issue_7079_async(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -349,15 +352,16 @@
                 batch = await messages.receive_messages()
                 count = len(batch)
                 async for message in messages:
                    _logger.debug(message)
                    count += 1
                 assert count == 5
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer()
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @CachedServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_github_issue_6178_async(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -371,15 +375,16 @@
                     _logger.debug(message)
                     _logger.debug(message.sequence_number)
                     _logger.debug(message.enqueued_time_utc)
                     _logger.debug(message._lock_expired)
                     await receiver.complete_message(message)
                     await asyncio.sleep(40)
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True, lock_duration='PT10S')
     async def test_async_queue_by_queue_client_conn_str_receive_handler_receiveanddelete(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -406,15 +411,16 @@
 
             messages = []
             async with sb_client.get_queue_receiver(servicebus_queue.name, receive_mode=ServiceBusReceiveMode.RECEIVE_AND_DELETE, max_wait_time=5) as receiver:
                 async for message in receiver:
                     messages.append(message)
                 assert len(messages) == 0
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_async_queue_by_queue_client_conn_str_receive_handler_with_stop(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -442,15 +448,16 @@
                     await receiver.complete_message(message)
                     if len(messages) >= 5:
                         break
 
             assert not receiver._running
             assert len(messages) == 6
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_async_queue_by_servicebus_client_iter_messages_simple(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -474,15 +481,16 @@
                     count += 1
 
                 with pytest.raises(StopAsyncIteration):
                     await receiver.__anext__()
 
             assert count == 10
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_async_queue_by_servicebus_conn_str_client_iter_messages_with_abandon(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -511,15 +519,16 @@
                 count = 0
                 async for message in receiver:
                     print_message(_logger, message)
                     await receiver.complete_message(message)
                     count += 1
             assert count == 0
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_async_queue_by_servicebus_client_iter_messages_with_defer(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -545,15 +554,16 @@
                 count = 0
                 async for message in receiver:
                     print_message(_logger, message)
                     await receiver.complete_message(message)
                     count += 1
             assert count == 0
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_async_queue_by_servicebus_client_iter_messages_with_retrieve_deferred_client(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -581,15 +591,16 @@
                 for message in deferred:
                     assert isinstance(message, ServiceBusReceivedMessage)
                     await receiver.complete_message(message)
 
                 with pytest.raises(ServiceBusError):
                     await receiver.receive_deferred_messages(deferred_messages)
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_async_queue_by_servicebus_client_iter_messages_with_retrieve_deferred_receiver_complete(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -618,15 +629,16 @@
                     assert isinstance(message, ServiceBusReceivedMessage)
                     assert message.lock_token
                     assert message.locked_until_utc
                     assert message._receiver
                     await receiver.renew_message_lock(message)
                     await receiver.complete_message(message)
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_async_queue_by_servicebus_client_iter_messages_with_retrieve_deferred_receiver_deadletter(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -664,15 +676,16 @@
                     assert message.dead_letter_reason == 'Testing reason'
                     assert message.dead_letter_error_description == 'Testing description'
                     assert message.application_properties[b'DeadLetterReason'] == b'Testing reason'
                     assert message.application_properties[b'DeadLetterErrorDescription'] == b'Testing description'
                     await receiver.complete_message(message)
             assert count == 10
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_async_queue_by_servicebus_client_iter_messages_with_retrieve_deferred_receiver_deletemode(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -698,15 +711,16 @@
                 for message in deferred:
                     assert isinstance(message, ServiceBusReceivedMessage)
                     with pytest.raises(ValueError):
                         await receiver.complete_message(message)
                 with pytest.raises(ServiceBusError):
                     deferred = await receiver.receive_deferred_messages(deferred_messages)
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_async_queue_by_servicebus_client_iter_messages_with_retrieve_deferred_not_found(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -732,15 +746,16 @@
             async with sb_client.get_queue_receiver(servicebus_queue.name, max_wait_time=10, receive_mode=ServiceBusReceiveMode.PEEK_LOCK) as receiver:
                 with pytest.raises(ServiceBusError):
                     deferred = await receiver.receive_deferred_messages([3, 4])
 
                 with pytest.raises(ServiceBusError):
                     deferred = await receiver.receive_deferred_messages([5, 6, 7])
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_async_queue_by_servicebus_client_receive_batch_with_deadletter(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -783,15 +798,16 @@
                     count += 1
                     assert message.dead_letter_reason == 'Testing reason'
                     assert message.dead_letter_error_description == 'Testing description'
                     assert message.application_properties[b'DeadLetterReason'] == b'Testing reason'
                     assert message.application_properties[b'DeadLetterErrorDescription'] == b'Testing description'
                 assert count == 10
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_async_queue_by_servicebus_client_receive_batch_with_retrieve_deadletter(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -828,29 +844,31 @@
                     assert message.dead_letter_error_description == 'Testing description'
                     assert message.application_properties[b'DeadLetterReason'] == b'Testing reason'
                     assert message.application_properties[b'DeadLetterErrorDescription'] == b'Testing description'
                     await receiver.complete_message(message)
                     count += 1
             assert count == 10
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @CachedServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_async_queue_by_servicebus_client_session_fail(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
             servicebus_namespace_connection_string, logging_enable=False) as sb_client:
 
             with pytest.raises(ServiceBusError):
                 await sb_client.get_queue_receiver(servicebus_queue.name, session_id="test")._open_with_retry()
 
             async with sb_client.get_queue_sender(servicebus_queue.name) as sender:
                 await sender.send_messages(ServiceBusMessage("test session sender", session_id="test"))
-
+ 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_async_queue_by_servicebus_client_browse_messages_client(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -866,14 +884,15 @@
                 assert len(messages) == 5
                 assert all(isinstance(m, ServiceBusReceivedMessage) for m in messages)
                 for message in messages:
                     print_message(_logger, message)
                     with pytest.raises(ValueError):
                         await receiver.complete_message(message)
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_async_queue_by_servicebus_client_browse_messages_with_receiver(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -889,27 +908,29 @@
                 assert len(messages) > 0
                 assert all(isinstance(m, ServiceBusReceivedMessage) for m in messages)
                 for message in messages:
                     print_message(_logger, message)
                     with pytest.raises(ValueError):
                         await receiver.complete_message(message)
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_async_queue_by_servicebus_client_browse_empty_messages(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
             servicebus_namespace_connection_string, logging_enable=False) as sb_client:
 
             async with sb_client.get_queue_receiver(servicebus_queue.name, max_wait_time=5, receive_mode=ServiceBusReceiveMode.PEEK_LOCK, prefetch_count=10) as receiver:
                 messages = await receiver.peek_messages(10)
                 assert len(messages) == 0
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_async_queue_by_servicebus_client_renew_message_locks(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -940,15 +961,16 @@
                 finally:
                     await receiver.complete_message(messages[0])
                     await receiver.complete_message(messages[1])
                     sleep_until_expired(messages[2])
                     with pytest.raises(ServiceBusError):
                         await receiver.complete_message(messages[2])
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True, lock_duration='PT5S')
     async def test_async_queue_by_queue_client_conn_str_receive_handler_with_autolockrenew(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -995,15 +1017,16 @@
                             assert message.delivery_count >= 1
                             print("Remaining messages", message.locked_until_utc, utc_now())
                             messages.append(message)
                             await receiver.complete_message(message)
             await renewer.close()
             assert len(messages) == 11
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True, lock_duration='PT5S')
     async def test_async_queue_by_queue_client_conn_str_receive_handler_with_auto_autolockrenew(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -1049,14 +1072,15 @@
                             assert message.delivery_count >= 1
                             print("Remaining messages", message.locked_until_utc, utc_now())
                             messages.append(message)
                             await receiver.complete_message(message)
             await renewer.close()
             assert len(messages) == 11
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_async_queue_by_servicebus_client_fail_send_messages(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -1068,15 +1092,16 @@
                 with pytest.raises(MessageSizeExceededError):
                     await sender.send_messages(ServiceBusMessage(too_large))
                     
                 half_too_large = "A" * int((1024 * 256) / 2)
                 with pytest.raises(MessageSizeExceededError):
                     await sender.send_messages([ServiceBusMessage(half_too_large), ServiceBusMessage(half_too_large)])
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_async_queue_message_time_to_live(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -1101,15 +1126,16 @@
                 count = 0
                 async for message in receiver:
                     print_message(_logger, message)
                     await receiver.complete_message(message)
                     count += 1
                 assert count == 1
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', requires_duplicate_detection=True, dead_lettering_on_message_expiration=True)
     async def test_async_queue_message_duplicate_detection(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -1128,14 +1154,15 @@
                 async for message in receiver:
                     print_message(_logger, message)
                     assert message.message_id == message_id
                     await receiver.complete_message(message)
                     count += 1
                 assert count == 1
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_async_queue_message_connection_closed(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -1149,14 +1176,15 @@
             async with sb_client.get_queue_receiver(servicebus_queue.name) as receiver:
                 messages = await receiver.receive_messages(max_wait_time=10)
                 assert len(messages) == 1
 
             with pytest.raises(ValueError):
                 await receiver.complete_message(messages[0])
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_async_queue_message_expiry(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -1180,14 +1208,15 @@
             async with sb_client.get_queue_receiver(servicebus_queue.name) as receiver:
                 messages = await receiver.receive_messages(max_wait_time=30)
                 assert len(messages) == 1
                 print_message(_logger, messages[0])
                 assert messages[0].delivery_count > 0
                 await receiver.complete_message(messages[0])
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_async_queue_message_lock_renew(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -1209,14 +1238,15 @@
                 assert not messages[0]._lock_expired
                 await receiver.complete_message(messages[0])
             
             async with sb_client.get_queue_receiver(servicebus_queue.name) as receiver:
                 messages = await receiver.receive_messages(max_wait_time=10)
                 assert len(messages) == 0
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True, lock_duration='PT10S')
     async def test_async_queue_message_receive_and_delete(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -1245,14 +1275,15 @@
             time.sleep(10)
             async with sb_client.get_queue_receiver(servicebus_queue.name) as receiver:
                 messages = await receiver.receive_messages(max_wait_time=10)
                 for m in messages:
                     print_message(_logger, m)
                 assert len(messages) == 0
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_async_queue_message_batch(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -1301,14 +1332,15 @@
                     assert message.sequence_number
                     assert message.enqueued_time_utc
                     assert message.expires_at_utc == (message.enqueued_time_utc + timedelta(seconds=60))
                     print_message(_logger, message)
                     await receiver.complete_message(message)
                     count += 1
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_async_queue_schedule_message(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -1335,15 +1367,16 @@
                         assert len(messages) == 1
                     finally:
                         for message in messages:
                             await receiver.complete_message(message)
                 else:
                     raise Exception("Failed to receive scheduled message.")
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_async_queue_schedule_multiple_messages(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -1384,14 +1417,15 @@
                         assert len(messages) == 2
                     finally:
                         for message in messages:
                             await receiver.complete_message(message)
                 else:
                     raise Exception("Failed to receive scheduled message.")
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_async_queue_cancel_scheduled_messages(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -1406,14 +1440,15 @@
                     assert len(tokens) == 2
 
                     await sender.cancel_scheduled_messages(tokens, timeout=None)
 
                 messages = await receiver.receive_messages(max_wait_time=120)
                 assert len(messages) == 0
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_queue_message_amqp_over_websocket(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -1448,14 +1483,15 @@
         assert sender._config.http_proxy == http_proxy
         assert sender._config.transport_type == TransportType.AmqpOverWebsocket
 
         receiver = sb_client.get_queue_receiver(queue_name="mock")
         assert receiver._config.http_proxy == http_proxy
         assert receiver._config.transport_type == TransportType.AmqpOverWebsocket
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_queue_message_settle_through_mgmt_link_due_to_broken_receiver_link(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -1583,14 +1619,15 @@
         with pytest.raises(ServiceBusError):
             async with auto_lock_renew:
                 pass
 
         with pytest.raises(ServiceBusError):
             auto_lock_renew.register(receiver, renewable=MockReceivedMessage())
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @CachedServiceBusQueuePreparer(name_prefix='servicebustest')
     async def test_queue_receiver_invalid_autolockrenew_mode(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         
@@ -1599,14 +1636,15 @@
             with pytest.raises(ValueError):
                 async with sb_client.get_queue_receiver(servicebus_queue.name, 
                                                   receive_mode=ServiceBusReceiveMode.RECEIVE_AND_DELETE,
                                                   auto_lock_renewer=AutoLockRenewer()) as receiver:
                 
                     raise Exception("Should not get here, should fail fast because RECEIVE_AND_DELETE messages cannot be autorenewed.")
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_async_queue_receive_batch_without_setting_prefetch(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -1651,15 +1689,16 @@
                             message_2nd_received_cnt += 1
                             await receiver.complete_message(message)
 
                 assert message_1st_received_cnt == 20 and message_2nd_received_cnt == 20
                 # Network/server might be unstable making flow control ineffective in the leading rounds of connection iteration
                 assert receive_counter < 10  # Dynamic link credit issuing come info effect
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_async_queue_receiver_alive_after_timeout(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -1703,15 +1742,16 @@
 
                     for message in messages[2:]:
                         await receiver.complete_message(message)
 
                     messages = await receiver.receive_messages()
                     assert not messages
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True, lock_duration='PT5M')
     async def test_queue_receive_keep_conn_alive_async(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -1738,15 +1778,16 @@
                 messages = []
                 async for message in receiver:
                     messages.append(message)
 
                 assert len(messages) == 0  # make sure messages are removed from the queue
                 assert receiver_handler == receiver._handler  # make sure no reconnection happened
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    # @pytest.mark.skip(reason="TODO: _counter doesnt exist in pyamqp")
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest')
     async def test_async_queue_receiver_respects_max_wait_time_overrides(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -1756,44 +1797,45 @@
             async with sb_client.get_queue_sender(servicebus_queue.name) as sender:
                 message = ServiceBusMessage("0")
                 await sender.send_messages(message)
 
                 messages = []
                 async with sb_client.get_queue_receiver(servicebus_queue.name, max_wait_time=5) as receiver:
 
-                    time_1 = receiver._handler._counter.get_current_ms()
+                    time_1 = time.time()
                     async for message in receiver._get_streaming_message_iter(max_wait_time=10):
                         messages.append(message)
                         await receiver.complete_message(message)
 
-                        time_2 = receiver._handler._counter.get_current_ms()
+                        time_2 = time.time()
                         async for message in receiver._get_streaming_message_iter(max_wait_time=1):
                             messages.append(message)
-                        time_3 = receiver._handler._counter.get_current_ms()
-                        assert timedelta(seconds=.5) < timedelta(milliseconds=(time_3 - time_2)) <= timedelta(seconds=2)
-                    time_4 = receiver._handler._counter.get_current_ms()
-                    assert timedelta(seconds=8) < timedelta(milliseconds=(time_4 - time_3)) <= timedelta(seconds=11)
+                        time_3 = time.time()
+                        assert timedelta(seconds=.5) < timedelta(seconds=(time_3 - time_2)) <= timedelta(seconds=2)
+                    time_4 = time.time()
+                    assert timedelta(seconds=8) < timedelta(seconds=(time_4 - time_3)) <= timedelta(seconds=11)
 
                     async for message in receiver._get_streaming_message_iter(max_wait_time=3):
                         messages.append(message)
-                    time_5 = receiver._handler._counter.get_current_ms()
-                    assert timedelta(seconds=1) < timedelta(milliseconds=(time_5 - time_4)) <= timedelta(seconds=4)
+                    time_5 = time.time()
+                    assert timedelta(seconds=1) < timedelta(seconds=(time_5 - time_4)) <= timedelta(seconds=4)
 
                     async for message in receiver:
                         messages.append(message)
-                    time_6 = receiver._handler._counter.get_current_ms()
-                    assert timedelta(seconds=3) < timedelta(milliseconds=(time_6 - time_5)) <= timedelta(seconds=6)
+                    time_6 = time.time()
+                    assert timedelta(seconds=3) < timedelta(seconds=(time_6 - time_5)) <= timedelta(seconds=6)
 
                     async for message in receiver._get_streaming_message_iter():
                         messages.append(message)
-                    time_7 = receiver._handler._counter.get_current_ms()
-                    assert timedelta(seconds=3) < timedelta(milliseconds=(time_7 - time_6)) <= timedelta(seconds=6)
+                    time_7 = time.time()
+                    assert timedelta(seconds=3) < timedelta(seconds=(time_7 - time_6)) <= timedelta(seconds=6)
                     assert len(messages) == 1
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest')
     async def test_async_queue_send_twice(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -1819,14 +1861,15 @@
                 messages = []
                 async with sb_client.get_queue_receiver(servicebus_queue.name, max_wait_time=20) as receiver:
                     async for message in receiver:
                         messages.append(message)
                         await receiver.complete_message(message)
                     assert len(messages) == 2
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @CachedServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_async_queue_send_timeout(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async def _hack_amqp_sender_run_async(self, **kwargs):
@@ -1843,14 +1886,15 @@
                 servicebus_namespace_connection_string, logging_enable=False) as sb_client:
             async with sb_client.get_queue_sender(servicebus_queue.name) as sender:
                 # this one doesn't need to reset the method, as it's hacking the method on the instance
                 sender._handler._client_run_async = types.MethodType(_hack_amqp_sender_run_async, sender._handler)
                 with pytest.raises(OperationTimeoutError):
                     await sender.send_messages(ServiceBusMessage("body"), timeout=5)
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @CachedServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_async_queue_mgmt_operation_timeout(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async def hack_mgmt_execute_async(self, message, operation=None, operation_type=None, timeout=0):
@@ -1882,14 +1926,15 @@
                     with pytest.raises(OperationTimeoutError):
                         scheduled_time_utc = utc_now() + timedelta(seconds=30)
                         await sender.schedule_messages(ServiceBusMessage("ServiceBusMessage to be scheduled"), scheduled_time_utc, timeout=5)
         finally:
             # must reset the mgmt execute method, otherwise other test cases would use the hacked execute method, leading to timeout error
             _management_operation_async.ManagementOperation.execute = original_execute_method
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @CachedServiceBusQueuePreparer(name_prefix='servicebustest', lock_duration='PT10S')
     async def test_async_queue_operation_negative(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async def _hack_amqp_message_complete(cls, _, settlement):
@@ -1934,15 +1979,16 @@
 
                     receiver._settle_message = origin_sb_receiver_settle_message_method
                     message = (await receiver.receive_messages(max_wait_time=10))[0]
                     await receiver.complete_message(message)
             finally:
                 ReceiveClientAsync.settle_messages_async = original_settlement
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_async_send_message_no_body(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -1952,15 +1998,16 @@
                 await sender.send_messages(ServiceBusMessage(body=None))
 
             async with sb_client.get_queue_receiver(servicebus_queue.name,  
                                             max_wait_time=10) as receiver:
                 message = await receiver.__anext__()
                 assert message.body is None
                 await receiver.complete_message(message)
-    
+
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @CachedServiceBusQueuePreparer(name_prefix='servicebustest')
     async def test_async_queue_by_servicebus_client_enum_case_sensitivity(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         # Note: This test is currently intended to enforce case-sensitivity.  If we eventually upgrade to the Fancy Enums being used with new autorest,
@@ -1982,15 +2029,16 @@
                 pass
             with pytest.raises(ValueError):
                 async with sb_client.get_queue_receiver(servicebus_queue.name, 
                                                   sub_queue=str.upper(ServiceBusSubQueue.DEAD_LETTER.value),
                                                   max_wait_time=5) as receiver:
                     raise Exception("Should not get here, should be case sensitive.")
 
-    @pytest.mark.skip(reason="TODO: iterator support")            
+      
+    @pytest.mark.asyncio          
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest')
     async def test_queue_async_send_dict_messages(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -2016,15 +2064,16 @@
 
                 received_messages = []
                 async with sb_client.get_queue_receiver(servicebus_queue.name, max_wait_time=5) as receiver:
                     async for message in receiver:
                         received_messages.append(message)
                 assert len(received_messages) == 6
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest')
     async def test_queue_async_send_mapping_messages(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         class MappingMessage(DictMixin):
@@ -2064,14 +2113,15 @@
 
                 received_messages = []
                 async with sb_client.get_queue_receiver(servicebus_queue.name, max_wait_time=5) as receiver:
                     async for message in receiver:
                         received_messages.append(message)
                 assert len(received_messages) == 6
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest')
     async def test_queue_async_send_dict_messages_error_badly_formatted_dicts(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -2092,14 +2142,15 @@
                     await sender.send_messages(list_message_dicts)
 
                 # create and send BatchMessage with dicts
                 batch_message = await sender.create_message_batch()
                 with pytest.raises(TypeError):
                     batch_message._from_list(list_message_dicts)  # pylint: disable=protected-access
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_queue_async_send_dict_messages_scheduled(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         
@@ -2153,14 +2204,15 @@
                         assert len(messages) == 2
                     finally:
                         for m in messages:
                             await receiver.complete_message(m)
                 else:
                     raise Exception("Failed to receive schdeduled message.")
 
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_queue_async_send_dict_messages_scheduled_error_badly_formatted_dicts(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         
@@ -2176,38 +2228,42 @@
                     message2_dict = {"message_id": message_id2, "bad_key": content}
                     list_message_dicts = [message_dict, message2_dict]
                     with pytest.raises(TypeError):
                         await sender.schedule_messages(message_dict, scheduled_enqueue_time)
                     with pytest.raises(TypeError):
                         await sender.schedule_messages(list_message_dicts, scheduled_enqueue_time)
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_queue_async_receive_iterator_resume_after_link_detach(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
 
-        async def hack_iter_next_mock_error(self):
-            await self._open()
-            # when trying to receive the second message (execution_times is 1), raising LinkDetach error to mock 10 mins idle timeout
-            if self.execution_times == 1:
-                from uamqp.errors import LinkDetach
-                from uamqp.constants import ErrorCodes
-                self.execution_times += 1
-                self.error_raised = True
-                raise LinkDetach(ErrorCodes.LinkDetachForced)
-            else:
-                self.execution_times += 1
-            if not self._message_iter:
-                self._message_iter = self._handler.receive_messages_iter_async()
-            uamqp_message = await self._message_iter.__anext__()
-            message = self._build_message(uamqp_message)
-            return message
+        async def hack_iter_next_mock_error(self, wait_time=None):
+            try:
+                self._receive_context.set()
+                await self._open()
+                # when trying to receive the second message (execution_times is 1), raising LinkDetach error to mock 10 mins idle timeout
+                if self.execution_times == 1:
+                    from azure.servicebus._pyamqp.error import ErrorCondition, AMQPLinkError
+                    self.execution_times += 1
+                    self.error_raised = True
+                    raise AMQPLinkError(condition=ErrorCondition.LinkDetachForced)
+                else:
+                    self.execution_times += 1
+                if not self._message_iter:
+                    self._message_iter = await self._handler.receive_messages_iter_async(timeout=wait_time)
+                pyamqp_message = await self._message_iter.__anext__()
+                message = self._build_message(pyamqp_message)
+                return message
+            finally:
+                self._receive_context.clear()
 
         async with ServiceBusClient.from_connection_string(
                 servicebus_namespace_connection_string, logging_enable=False) as sb_client:
             async with sb_client.get_queue_sender(servicebus_queue.name) as sender:
                 await sender.send_messages(
                     [ServiceBusMessage("test1"), ServiceBusMessage("test2"), ServiceBusMessage("test3")]
                 )
@@ -2219,15 +2275,15 @@
                 async for msg in receiver:
                     await receiver.complete_message(msg)
                     res.append(msg)
                 assert len(res) == 3
                 assert receiver.error_raised
                 assert receiver.execution_times >= 4  # at least 1 failure and 3 successful receiving iterator
 
-    @pytest.mark.skip(reason="TODO: iterator support")
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_queue_async_send_amqp_annotated_message(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
 
@@ -2266,16 +2322,16 @@
                 application_properties=data_app_prop
             )
 
             content = "normalmessage"
             dict_message = {"body": content}
             sb_message = ServiceBusMessage(body=content)
             message_with_ttl = AmqpAnnotatedMessage(data_body=data_body, header=AmqpMessageHeader(time_to_live=60000))
-            uamqp_with_ttl = message_with_ttl._to_outgoing_amqp_message()
-            assert uamqp_with_ttl.properties.absolute_expiry_time == uamqp_with_ttl.properties.creation_time + uamqp_with_ttl.header.time_to_live
+            pyamqp_with_ttl = message_with_ttl._to_outgoing_amqp_message()
+            assert pyamqp_with_ttl.properties.absolute_expiry_time == pyamqp_with_ttl.properties.creation_time + pyamqp_with_ttl.header.ttl
 
             recv_data_msg = recv_sequence_msg = recv_value_msg = normal_msg = 0
             async with sb_client.get_queue_receiver(servicebus_queue.name, max_wait_time=10) as receiver:
                 async with sb_client.get_queue_sender(servicebus_queue.name) as sender:
                     batch = await sender.create_message_batch()
                     batch.add_message(data_message)
                     batch.add_message(value_message)
@@ -2317,15 +2373,15 @@
                         receiver.complete_message(message)
 
                     assert recv_data_msg == 3
                     assert recv_sequence_msg == 3
                     assert recv_value_msg == 3
                     assert normal_msg == 4
 
-
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_state_scheduled_async(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
@@ -2340,15 +2396,15 @@
 
             receiver = sb_client.get_queue_receiver(servicebus_queue.name)
             async with receiver:
                 messages = await receiver.peek_messages()
                 for msg in messages:
                     assert msg.state == ServiceBusMessageState.SCHEDULED
 
-
+    @pytest.mark.asyncio
     @pytest.mark.liveTest
     @pytest.mark.live_test_only
     @CachedResourceGroupPreparer(name_prefix='servicebustest')
     @CachedServiceBusNamespacePreparer(name_prefix='servicebustest')
     @ServiceBusQueuePreparer(name_prefix='servicebustest', dead_lettering_on_message_expiration=True)
     async def test_state_deferred_async(self, servicebus_namespace_connection_string, servicebus_queue, **kwargs):
         async with ServiceBusClient.from_connection_string(
```

## Comparing `azure-servicebus-7.9.0a1/tests/perf_tests/_test_base.py` & `azure-servicebus-7.9.0b1/samples/sync_samples/auto_lock_renew.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,128 +1,133 @@
+#!/usr/bin/env python
+
 # --------------------------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # --------------------------------------------------------------------------------------------
 
-import uuid
+"""
+Example to show usage of AutoLockRenewer:
+    1. Automatically renew locks on messages received from non-sessionful entity
+    2. Automatically renew locks on the session of sessionful entity
+"""
+
+import os
+import time
+
+from azure.servicebus import ServiceBusClient, AutoLockRenewer, ServiceBusMessage
+from azure.servicebus.exceptions import ServiceBusError
+
+CONNECTION_STR = os.environ['SERVICEBUS_CONNECTION_STR']
+QUEUE_NAME = os.environ["SERVICEBUS_QUEUE_NAME"]
+SESSION_QUEUE_NAME = os.environ['SERVICEBUS_SESSION_QUEUE_NAME']
+
+
+def renew_lock_on_message_received_from_non_sessionful_entity():
+    servicebus_client = ServiceBusClient.from_connection_string(conn_str=CONNECTION_STR)
+
+    with servicebus_client:
+        with servicebus_client.get_queue_sender(queue_name=QUEUE_NAME) as sender:
+            msgs_to_send = [ServiceBusMessage("message: {}".format(i)) for i in range(10)]
+            sender.send_messages(msgs_to_send)
+            print('Send messages to non-sessionful queue.')
+
+        # Can also be called via "with AutoLockRenewer() as renewer" to automate shutdown.
+        renewer = AutoLockRenewer()
+
+        with servicebus_client.get_queue_receiver(queue_name=QUEUE_NAME, prefetch_count=10) as receiver:
+            received_msgs = receiver.receive_messages(max_message_count=10, max_wait_time=5)
+
+            for msg in received_msgs:
+                # automatically renew the lock on each message for 100 seconds
+                renewer.register(receiver, msg, max_lock_renewal_duration=100)
+            print('Register messages into AutoLockRenewer done.')
+
+            time.sleep(100)  # message handling for long period (E.g. application logic)
+
+            for msg in received_msgs:
+                receiver.complete_message(msg)  # Settling the message deregisters it from the AutoLockRenewer
+            print('Complete messages.')
+
+        renewer.close()
+
+
+def renew_lock_on_session_of_the_sessionful_entity():
+    servicebus_client = ServiceBusClient.from_connection_string(conn_str=CONNECTION_STR)
+
+    with servicebus_client:
+
+        with servicebus_client.get_queue_sender(queue_name=SESSION_QUEUE_NAME) as sender:
+            msgs_to_send = [ServiceBusMessage("session message: {}".format(i), session_id='SESSION') for i in range(10)]
+            sender.send_messages(msgs_to_send)
+            print('Send messages to sessionful queue.')
 
-from azure_devtools.perfstress_tests import PerfStressTest, get_random_bytes
+        renewer = AutoLockRenewer()
+
+        with servicebus_client.get_queue_receiver(
+            queue_name=SESSION_QUEUE_NAME,
+            session_id='SESSION',
+            prefetch_count=10
+        ) as receiver:
+
+            # automatically renew the lock on the session for 100 seconds
+            renewer.register(receiver, receiver.session, max_lock_renewal_duration=100)
+            print('Register session into AutoLockRenewer.')
+
+            received_msgs = receiver.receive_messages(max_message_count=10, max_wait_time=5)
+            time.sleep(100)  # message handling for long period (E.g. application logic)
+
+            for msg in received_msgs:
+                receiver.complete_message(msg)
+
+            print('Complete messages.')
+
+        renewer.close()
+
+
+def renew_lock_with_lock_renewal_failure_callback():
+    servicebus_client = ServiceBusClient.from_connection_string(conn_str=CONNECTION_STR)
+
+    with servicebus_client:
+        with servicebus_client.get_queue_sender(queue_name=QUEUE_NAME) as sender:
+            sender.send_messages(ServiceBusMessage("message"))
+
+        with AutoLockRenewer() as renewer:
+            # For this sample we're going to set the renewal recurrence of the autolockrenewer to greater than the
+            # service side message lock duration, to demonstrate failure.  Normally, this should not be adjusted.
+            renewer._sleep_time = 40
+            with servicebus_client.get_queue_receiver(queue_name=QUEUE_NAME, prefetch_count=10) as receiver:
+
+                def on_lock_renew_failure_callback(renewable, error):
+                    # If auto-lock-renewal fails, this function will be called.
+                    # If failure is due to an error, the second argument will be populated, otherwise
+                    # it will default to `None`.
+                    # This callback can be an ideal location to log the failure, or take action to safely
+                    # handle any processing on the message or session that was in progress.
+                    print("Intentionally failed to renew lock on {} due to {}".format(renewable, error))
+
+                received_msgs = receiver.receive_messages(max_message_count=1, max_wait_time=5)
+
+                for msg in received_msgs:
+                    # automatically renew the lock on each message for 120 seconds
+                    renewer.register(receiver,
+                                     msg,
+                                     max_lock_renewal_duration=90,
+                                     on_lock_renew_failure=on_lock_renew_failure_callback)
+                print('Register messages into AutoLockRenewer done.')
+
+                # Cause the messages and autorenewal to time out.
+                # Other reasons for renew failure could include a network or service outage.
+                time.sleep(80)
 
-from azure.servicebus import ServiceBusClient, ServiceBusReceiveMode, ServiceBusMessage
-from azure.servicebus.aio import ServiceBusClient as AsyncServiceBusClient
-from azure.servicebus.aio.management import ServiceBusAdministrationClient
-
-MAX_QUEUE_SIZE = 40960
-
-
-class _ServiceTest(PerfStressTest):
-    service_client = None
-    async_service_client = None
-
-    def __init__(self, arguments):
-        super().__init__(arguments)
-
-        connection_string = self.get_from_env("AZURE_SERVICEBUS_CONNECTION_STRING")
-        if self.args.no_client_share:
-            self.service_client = ServiceBusClient.from_connection_string(connection_string)
-            self.async_service_client = AsyncServiceBusClient.from_connection_string(connection_string)
-        else:
-            if not _ServiceTest.service_client:
-                _ServiceTest.service_client = ServiceBusClient.from_connection_string(connection_string)
-                _ServiceTest.async_service_client = AsyncServiceBusClient.from_connection_string(connection_string)
-            self.service_client = _ServiceTest.service_client
-            self.async_service_client =_ServiceTest.async_service_client
-
-
-    async def close(self):
-        self.service_client.close()
-        await self.async_service_client.close()
-        await super().close()
-
-    @staticmethod
-    def add_arguments(parser):
-        super(_ServiceTest, _ServiceTest).add_arguments(parser)
-        parser.add_argument('--message-size', nargs='?', type=int, help='Size of a single message. Defaults to 100 bytes', default=100)
-        parser.add_argument('--no-client-share', action='store_true', help='Create one ServiceClient per test instance.  Default is to share a single ServiceClient.', default=False)
-        parser.add_argument('--num-messages', nargs='?', type=int, help='Number of messages to send or receive. Defaults to 100', default=100)
-
-
-class _QueueTest(_ServiceTest):
-    queue_name = "perfstress-" + str(uuid.uuid4())
-
-    def __init__(self, arguments):
-        super().__init__(arguments)
-        connection_string = self.get_from_env("AZURE_SERVICEBUS_CONNECTION_STRING")
-        self.async_mgmt_client = ServiceBusAdministrationClient.from_connection_string(connection_string)
-
-    async def global_setup(self):
-        await super().global_setup()
-        await self.async_mgmt_client.create_queue(self.queue_name, max_size_in_megabytes=MAX_QUEUE_SIZE)
-
-    async def global_cleanup(self):
-        await self.async_mgmt_client.delete_queue(self.queue_name)
-        await super().global_cleanup()
-
-    async def close(self):
-        await self.async_mgmt_client.close()
-        await super().close()
-
-
-class _SendTest(_QueueTest):
-    def __init__(self, arguments):
-        super().__init__(arguments)
-        connection_string = self.get_from_env("AZURE_SERVICEBUS_CONNECTION_STRING")
-        self.async_mgmt_client = ServiceBusAdministrationClient.from_connection_string(connection_string)
-        self.sender = self.service_client.get_queue_sender(self.queue_name)
-        self.async_sender = self.async_service_client.get_queue_sender(self.queue_name)
-    
-    async def close(self):
-        self.sender.close()
-        await self.async_sender.close()
-        await super().close()
-
-
-class _ReceiveTest(_QueueTest):
-    def __init__(self, arguments):
-        super().__init__(arguments)
-        mode = ServiceBusReceiveMode.PEEK_LOCK if self.args.peeklock else ServiceBusReceiveMode.RECEIVE_AND_DELETE
-        self.receiver = self.service_client.get_queue_receiver(
-            queue_name=self.queue_name,
-            receive_mode=mode,
-            prefetch_count=self.args.num_messages,
-            max_wait_time=self.args.max_wait_time or None)
-        self.async_receiver = self.async_service_client.get_queue_receiver(
-            queue_name=self.queue_name,
-            receive_mode=mode,
-            prefetch_count=self.args.num_messages,
-            max_wait_time=self.args.max_wait_time or None)
-
-    async def _preload_queue(self):
-        data = get_random_bytes(self.args.message_size)
-        async with self.async_service_client.get_queue_sender(self.queue_name) as sender:
-            batch = await sender.create_message_batch()
-            for i in range(self.args.preload):
                 try:
-                    batch.add_message(ServiceBusMessage(data))
-                except ValueError:
-                    # Batch full
-                    await sender.send_messages(batch)
-                    print("Loaded {} messages".format(i))
-                    batch = await sender.create_message_batch()
-                    batch.add_message(ServiceBusMessage(data))
-            await sender.send_messages(batch)
-
-    async def global_setup(self):
-        await super().global_setup()
-        await self._preload_queue()
-    
-    async def close(self):
-        self.receiver.close()
-        await self.async_receiver.close()
-        await super().close()
-
-    @staticmethod
-    def add_arguments(parser):
-        super(_ReceiveTest, _ReceiveTest).add_arguments(parser)
-        parser.add_argument('--peeklock', action='store_true', help='Receive using PeekLock mode and message settlement.', default=False)
-        parser.add_argument('--max-wait-time', nargs='?', type=int, help='Max time to wait for messages before closing. Defaults to 0.', default=0)
-        parser.add_argument('--preload', nargs='?', type=int, help='Number of messages to preload. Default is 10000.', default=10000)
+                    for msg in received_msgs:
+                        receiver.complete_message(msg)
+                except ServiceBusError as e:
+                    print('Messages cannot be settled if they have timed out. (This is expected)')
+
+                print('Lock renew failure demonstration complete.')
+
+
+renew_lock_on_message_received_from_non_sessionful_entity()
+renew_lock_on_session_of_the_sessionful_entity()
+renew_lock_with_lock_renewal_failure_callback()
```

## Comparing `azure-servicebus-7.9.0a1/tests/perf_tests/receive_message_stream.py` & `azure-servicebus-7.9.0b1/tests/perf_tests/receive_queue_message_stream.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # --------------------------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # --------------------------------------------------------------------------------------------
 
 import asyncio
 
-from ._test_base import _ReceiveTest
+from ._test_base import _QueueReceiveTest
 
 
-class ReceiveMessageStreamTest(_ReceiveTest):
-    def run_sync(self):
+class ReceiveQueueMessageStreamTest(_QueueReceiveTest):
+    def run_sync(self) -> None:
         count = 0
         if self.args.peeklock:
             for msg in self.receiver:
                 if count >= self.args.num_messages:
                     break
                 count += 1
                 self.receiver.complete_message(msg)
         else:
             for msg in self.receiver:
                 if count >= self.args.num_messages:
                     break
                 count += 1
 
-    async def run_async(self):
+    async def run_async(self) -> None:
         count = 0
         if self.args.peeklock:
             async for msg in self.async_receiver:
                 if count >= self.args.num_messages:
                     break
                 count += 1
                 await self.async_receiver.complete_message(msg)
```

## Comparing `azure-servicebus-7.9.0a1/tests/perf_tests/send_message.py` & `azure-servicebus-7.9.0b1/tests/perf_tests/send_topic_message_batch.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 # --------------------------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # --------------------------------------------------------------------------------------------
 
-from ._test_base import _SendTest
+from ._test_base import _SendTopicTest
 
 from azure_devtools.perfstress_tests import get_random_bytes
 
 from azure.servicebus import ServiceBusMessage
 
-class SendMessageTest(_SendTest):
-    def __init__(self, arguments):
+
+class SendTopicMessageBatchTest(_SendTopicTest):
+    def __init__(self, arguments) -> None:
         super().__init__(arguments)
         self.data = get_random_bytes(self.args.message_size)
 
-    def run_sync(self):
-        message = ServiceBusMessage(self.data)
-        self.sender.send_messages(message)
-
-    async def run_async(self):
-        message = ServiceBusMessage(self.data)
-        await self.async_sender.send_messages(message)
+    def run_batch_sync(self) -> int:
+        batch = self.sender.create_message_batch()
+        for _ in range(self.args.batch_size):
+            batch.add_message(ServiceBusMessage(self.data))
+        self.sender.send_messages(batch)
+        return self.args.batch_size
+
+    async def run_batch_async(self) -> int:
+        batch = await self.async_sender.create_message_batch()
+        for _ in range(self.args.batch_size):
+            batch.add_message(ServiceBusMessage(self.data))        
+        await self.async_sender.send_messages(batch)
+        return self.args.batch_size
```

## Comparing `azure-servicebus-7.9.0a1/tests/perf_tests/receive_message_batch.py` & `azure-servicebus-7.9.0b1/tests/perf_tests/receive_subscription_message_batch.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 # --------------------------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # --------------------------------------------------------------------------------------------
 
 import asyncio
 
-from ._test_base import _ReceiveTest
+from ._test_base import _SubscriptionReceiveBatchTest
 
 
-class ReceiveMessageBatchTest(_ReceiveTest):
-    def run_sync(self):
-        count = 0
-        while count < self.args.num_messages:
-            batch = self.receiver.receive_messages(
-                max_message_count=self.args.num_messages - count,
-                max_wait_time=self.args.max_wait_time or None)
-            if self.args.peeklock:
-                for msg in batch:
-                    self.receiver.complete_message(msg)
-            count += len(batch)
+class ReceiveSubscriptionMessageBatchTest(_SubscriptionReceiveBatchTest):
+    def run_batch_sync(self) -> None:
+        batch = self.receiver.receive_messages(
+            max_message_count=self.args.num_messages,
+            max_wait_time=self.args.max_wait_time or None)
+        if self.args.peeklock:
+            for msg in batch:
+                self.receiver.complete_message(msg)
+        return len(batch)
 
-    async def run_async(self):
-        count = 0
-        while count < self.args.num_messages:
-            batch = await self.async_receiver.receive_messages(
-                max_message_count=self.args.num_messages - count,
-                max_wait_time=self.args.max_wait_time or None)
-            if self.args.peeklock:
-                await asyncio.gather(*[self.async_receiver.complete_message(m) for m in batch])
-            count += len(batch)
+    async def run_batch_async(self) -> None:
+        batch = await self.async_receiver.receive_messages(
+            max_message_count=self.args.num_messages,
+            max_wait_time=self.args.max_wait_time or None)
+        if self.args.peeklock:
+            await asyncio.gather(*[self.async_receiver.complete_message(m) for m in batch])
+        return len(batch)
```

## Comparing `azure-servicebus-7.9.0a1/tests/perf_tests/T1_legacy_tests/_test_base.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_common/receiver_mixins.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,153 +1,144 @@
-# --------------------------------------------------------------------------------------------
+# ------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License. See License.txt in the project root for license information.
-# --------------------------------------------------------------------------------------------
-
+# Licensed under the MIT License. See License.txt in the project root for
+# license information.
+# -------------------------------------------------------------------------
 import uuid
-from urllib.parse import urlparse
+import time
+from .._pyamqp.endpoints import Source
+from .message import ServiceBusReceivedMessage
+from ..exceptions import _ServiceBusErrorPolicy, MessageAlreadySettled
+from .constants import (
+    NEXT_AVAILABLE_SESSION,
+    SESSION_FILTER,
+    MGMT_REQUEST_SESSION_ID,
+    ServiceBusReceiveMode,
+)
+
+
+class ReceiverMixin(object):  # pylint: disable=too-many-instance-attributes
+    def _populate_attributes(self, **kwargs):
+        if kwargs.get("subscription_name"):
+            self._subscription_name = kwargs.get("subscription_name")
+            self._is_subscription = True
+            self.entity_path = (
+                self._entity_name + "/Subscriptions/" + self._subscription_name
+            )
+        else:
+            self.entity_path = self._entity_name
 
-from azure_devtools.perfstress_tests import PerfStressTest, get_random_bytes
+        self._auth_uri = "sb://{}/{}".format(
+            self.fully_qualified_namespace, self.entity_path
+        )
+        self._entity_uri = "amqps://{}/{}".format(
+            self.fully_qualified_namespace, self.entity_path
+        )
+        self._receive_mode = ServiceBusReceiveMode(
+            kwargs.get("receive_mode", ServiceBusReceiveMode.PEEK_LOCK)
+        )
+
+        self._session_id = kwargs.get("session_id")
+
+        # TODO: What's the retry overlap between servicebus and pyamqp?
+        self._error_policy = _ServiceBusErrorPolicy(
+            is_session=bool(self._session_id),
+            retry_total=self._config.retry_total,
+            retry_mode = self._config.retry_mode,
+            retry_backoff_factor = self._config.retry_backoff_factor,
+            retry_backoff_max = self._config.retry_backoff_max
+        )
+
+        self._name = kwargs.get("client_identifier", "SBReceiver-{}".format(uuid.uuid4()))
+        self._last_received_sequenced_number = None
+        self._message_iter = None
+        self._connection = kwargs.get("connection")
+        prefetch_count = kwargs.get("prefetch_count", 0)
+        if int(prefetch_count) < 0 or int(prefetch_count) > 50000:
+            raise ValueError(
+                "prefetch_count must be an integer between 0 and 50000 inclusive."
+            )
+        self._prefetch_count = prefetch_count + 1
+        # The relationship between the amount can be received and the time interval is linear: amount ~= perf * interval
+        # In large max_message_count case, like 5000, the pull receive would always return hundreds of messages limited
+        # by the perf and time.
+        self._further_pull_receive_timeout = 0.2
+        max_wait_time = kwargs.get("max_wait_time", None)
+        if max_wait_time is not None and max_wait_time <= 0:
+            raise ValueError("The max_wait_time must be greater than 0.")
+        self._max_wait_time = max_wait_time
+
+        self._auto_lock_renewer = kwargs.get("auto_lock_renewer", None)
+        if (
+            self._auto_lock_renewer
+            and self._receive_mode == ServiceBusReceiveMode.RECEIVE_AND_DELETE
+            and self._session_id is None
+        ):
+            raise ValueError(
+                "Messages received in RECEIVE_AND_DELETE receive mode cannot have their locks removed "
+                "as they have been deleted, providing an AutoLockRenewer in this mode is invalid."
+            )
+
+    def _build_message(self, received, message_type=ServiceBusReceivedMessage):
+        message = message_type(
+            message=received[1], receive_mode=self._receive_mode, receiver=self, frame=received[0]
+        )
+        self._last_received_sequenced_number = message.sequence_number
+        return message
+
+    def _get_source(self):
+        # pylint: disable=protected-access
+        if self._session:
+            session_filter = None if self._session_id == NEXT_AVAILABLE_SESSION else self._session_id
+            filter_map = {SESSION_FILTER: session_filter}
+            source = Source(
+                address=self._entity_uri,
+                filters=filter_map
+            )
+            return source
+        return self._entity_uri
+
+    def _check_message_alive(self, message, action):
+        # pylint: disable=no-member, protected-access
+        if message._is_peeked_message:
+            raise ValueError(
+                "The operation {} is not supported for peeked messages."
+                "Only messages received using receive methods in PEEK_LOCK mode can be settled.".format(
+                    action
+                )
+            )
+
+        if self._receive_mode == ServiceBusReceiveMode.RECEIVE_AND_DELETE:
+            raise ValueError(
+                "The operation {} is not supported in 'RECEIVE_AND_DELETE' receive mode.".format(
+                    action
+                )
+            )
+
+        if message._settled:
+            raise MessageAlreadySettled(action=action)
+
+        if not self._running:
+            raise ValueError(
+                "Failed to {} the message as the handler has already been shutdown."
+                "Please use ServiceBusClient to create a new instance.".format(action)
+            )
+
+    def _populate_message_properties(self, message):
+        if self._session:
+            message[MGMT_REQUEST_SESSION_ID] = self._session_id
+
+    def _enhanced_message_received(self, frame, message):
+        # pylint: disable=protected-access
+        self._handler._last_activity_timestamp = time.time()
+        if self._receive_context.is_set():
+            self._handler._received_messages.put((frame, message))
+        else:
+            self._handler.settle_messages(frame[1], 'released')
 
-from azure.servicebus import ServiceBusClient, ReceiveSettleMode, Message
-from azure.servicebus.aio import ServiceBusClient as AsyncServiceBusClient
-from azure.servicebus.control_client import ServiceBusService
-from azure.servicebus.control_client.models import Queue
-
-MAX_QUEUE_SIZE = 40960
-
-
-def parse_connection_string(conn_str):
-    conn_settings = [s.split("=", 1) for s in conn_str.split(";")]
-    conn_settings = dict(conn_settings)
-    shared_access_key = conn_settings.get('SharedAccessKey')
-    shared_access_key_name = conn_settings.get('SharedAccessKeyName')
-    endpoint = conn_settings.get('Endpoint')
-    parsed = urlparse(endpoint.rstrip('/'))
-    namespace = parsed.netloc.strip().split('.')[0]
-    return {
-        'namespace': namespace,
-        'endpoint': endpoint,
-        'entity_path': conn_settings.get('EntityPath'),
-        'shared_access_key_name': shared_access_key_name,
-        'shared_access_key': shared_access_key
-    }
-
-
-class _ServiceTest(PerfStressTest):
-    service_client = None
-    async_service_client = None
-
-    def __init__(self, arguments):
-        super().__init__(arguments)
-
-        connection_string = self.get_from_env("AZURE_SERVICEBUS_CONNECTION_STRING")
-        if self.args.no_client_share:
-            self.service_client = ServiceBusClient.from_connection_string(connection_string)
-            self.async_service_client = AsyncServiceBusClient.from_connection_string(connection_string)
+    async def _enhanced_message_received_async(self, frame, message):
+        # pylint: disable=protected-access
+        self._handler._last_activity_timestamp = time.time()
+        if self._receive_context.is_set():
+            self._handler._received_messages.put((frame, message))
         else:
-            if not _ServiceTest.service_client:
-                    _ServiceTest.service_client = ServiceBusClient.from_connection_string(connection_string)
-                    _ServiceTest.async_service_client = AsyncServiceBusClient.from_connection_string(connection_string)
-            self.service_client = _ServiceTest.service_client
-            self.async_service_client =_ServiceTest.async_service_client
-
-    @staticmethod
-    def add_arguments(parser):
-        super(_ServiceTest, _ServiceTest).add_arguments(parser)
-        parser.add_argument('--message-size', nargs='?', type=int, help='Size of a single message. Defaults to 100 bytes', default=100)
-        parser.add_argument('--no-client-share', action='store_true', help='Create one ServiceClient per test instance.  Default is to share a single ServiceClient.', default=False)
-        parser.add_argument('--num-messages', nargs='?', type=int, help='Number of messages to send or receive. Defaults to 100', default=100)
-
-
-class _QueueTest(_ServiceTest):
-    queue_name = "perfstress-" + str(uuid.uuid4())
-    queue_client = None
-    async_queue_client = None
-
-    def __init__(self, arguments):
-        super().__init__(arguments)
-        connection_string = self.get_from_env("AZURE_SERVICEBUS_CONNECTION_STRING")
-        connection_props = parse_connection_string(connection_string)
-        self.mgmt_client = ServiceBusService(
-            service_namespace=connection_props['namespace'],
-            shared_access_key_name=connection_props['shared_access_key_name'],
-            shared_access_key_value=connection_props['shared_access_key'])
-
-    async def global_setup(self):
-        await super().global_setup()
-        queue = Queue(max_size_in_megabytes=MAX_QUEUE_SIZE)
-        self.mgmt_client.create_queue(self.queue_name, queue=queue)
-
-    async def setup(self):
-        await super().setup()
-        # In T1, these operations check for the existance of the queue
-        # so must be created during setup, rather than in the constructor.
-        self.queue_client = self.service_client.get_queue(self.queue_name)
-        self.async_queue_client = self.async_service_client.get_queue(self.queue_name)
-
-    async def global_cleanup(self):
-        self.mgmt_client.delete_queue(self.queue_name)
-        await super().global_cleanup()
-
-
-class _SendTest(_QueueTest):
-    sender = None
-    async_sender = None
-
-    async def setup(self):
-        await super().setup()
-        self.sender = self.queue_client.get_sender()
-        self.async_sender = self.async_queue_client.get_sender()
-        self.sender.open()
-        await self.async_sender.open()
-    
-    async def close(self):
-        self.sender.close()
-        await self.async_sender.close()
-        await super().close()
-
-
-class _ReceiveTest(_QueueTest):
-    receiver = None
-    async_receiver = None
-
-    async def global_setup(self):
-        await super().global_setup()
-        await self._preload_queue()
-
-    async def setup(self):
-        await super().setup()
-        mode = ReceiveSettleMode.PeekLock if self.args.peeklock else ReceiveSettleMode.ReceiveAndDelete
-        self.receiver = self.queue_client.get_receiver(
-            mode=mode,
-            prefetch=self.args.num_messages,
-            idle_timeout=self.args.max_wait_time)
-        self.async_receiver = self.async_queue_client.get_receiver(
-            mode=mode,
-            prefetch=self.args.num_messages,
-            idle_timeout=self.args.max_wait_time)
-        self.receiver.open()
-        await self.async_receiver.open()
-
-    async def _preload_queue(self):
-        data = get_random_bytes(self.args.message_size)
-        async_queue_client = self.async_service_client.get_queue(self.queue_name)
-        async with async_queue_client.get_sender() as sender:
-            for i in range(self.args.preload):
-                sender.queue_message(Message(data))
-                if i % 1000 == 0:
-                    print("Loaded {} messages".format(i))
-                    await sender.send_pending_messages()
-            await sender.send_pending_messages()
-    
-    async def close(self):
-        self.receiver.close()
-        await self.async_receiver.close()
-        await super().close()
-
-    @staticmethod
-    def add_arguments(parser):
-        super(_ReceiveTest, _ReceiveTest).add_arguments(parser)
-        parser.add_argument('--peeklock', action='store_true', help='Receive using PeekLock mode and message settlement.', default=False)
-        parser.add_argument('--max-wait-time', nargs='?', type=int, help='Max time to wait for messages before closing. Defaults to 0.', default=0)
-        parser.add_argument('--preload', nargs='?', type=int, help='Number of messages to preload. Default is 10000.', default=10000)
+            await self._handler.settle_messages_async(frame[1], 'released')
```

## Comparing `azure-servicebus-7.9.0a1/tests/perf_tests/T1_legacy_tests/receive_message_stream.py` & `azure-servicebus-7.9.0b1/tests/perf_tests/receive_subscription_message_stream.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # --------------------------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # --------------------------------------------------------------------------------------------
 
 import asyncio
 
-from ._test_base import _ReceiveTest
+from ._test_base import _SubscriptionReceiveTest
 
 
-class LegacyReceiveMessageStreamTest(_ReceiveTest):
-    def run_sync(self):
+class ReceiveSubscriptionMessageStreamTest(_SubscriptionReceiveTest):
+    def run_sync(self) -> None:
         count = 0
         if self.args.peeklock:
             for msg in self.receiver:
                 if count >= self.args.num_messages:
                     break
                 count += 1
-                msg.complete()
+                self.receiver.complete_message(msg)
         else:
             for msg in self.receiver:
                 if count >= self.args.num_messages:
                     break
                 count += 1
 
-    async def run_async(self):
+    async def run_async(self) -> None:
         count = 0
         if self.args.peeklock:
             async for msg in self.async_receiver:
                 if count >= self.args.num_messages:
                     break
                 count += 1
-                await msg.complete()
+                await self.async_receiver.complete_message(msg)
         else:
             async for msg in self.async_receiver:
                 if count >= self.args.num_messages:
                     break
-                count += 1
+                count += 1
```

## Comparing `azure-servicebus-7.9.0a1/tests/perf_tests/T1_legacy_tests/send_message.py` & `azure-servicebus-7.9.0b1/tests/perf_tests/send_queue_message.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 # --------------------------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # --------------------------------------------------------------------------------------------
 
-from ._test_base import _SendTest
+from ._test_base import _SendQueueTest
 
 from azure_devtools.perfstress_tests import get_random_bytes
 
-from azure.servicebus import Message
-from azure.servicebus.aio import Message as AsyncMessage
+from azure.servicebus import ServiceBusMessage
 
-
-class LegacySendMessageTest(_SendTest):
-    def __init__(self, arguments):
+class SendQueueMessageTest(_SendQueueTest):
+    def __init__(self, arguments) -> None:
         super().__init__(arguments)
         self.data = get_random_bytes(self.args.message_size)
 
-    def run_sync(self):
-        message = Message(self.data)
-        self.sender.send(message)
-
-    async def run_async(self):
-        message = AsyncMessage(self.data)
-        await self.async_sender.send(message)
+    def run_batch_sync(self) -> int:
+        if self.args.batch_size > 1:
+            self.sender.send_messages(
+                [ServiceBusMessage(self.data) for _ in range(self.args.batch_size)]
+            )
+        else:
+            self.sender.send_messages(ServiceBusMessage(self.data))
+        
+        return self.args.batch_size
+
+    async def run_batch_async(self) -> int:
+        if self.args.batch_size > 1:
+            await self.sender.send_messages(
+                [ServiceBusMessage(self.data) for _ in range(self.args.batch_size)]
+            )
+        else:
+            await self.sender.send_messages(ServiceBusMessage(self.data))
+        
+        return self.args.batch_size
```

## Comparing `azure-servicebus-7.9.0a1/tests/mgmt_tests/mgmt_test_utilities.py` & `azure-servicebus-7.9.0b1/tests/mgmt_tests/mgmt_test_utilities.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/tests/mgmt_tests/test_mgmt_rules.py` & `azure-servicebus-7.9.0b1/tests/mgmt_tests/test_mgmt_rules.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/tests/mgmt_tests/test_mgmt_queues.py` & `azure-servicebus-7.9.0b1/tests/mgmt_tests/test_mgmt_queues.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/tests/mgmt_tests/test_mgmt_subscriptions.py` & `azure-servicebus-7.9.0b1/tests/mgmt_tests/test_mgmt_subscriptions.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/tests/mgmt_tests/test_mgmt_topics.py` & `azure-servicebus-7.9.0b1/tests/mgmt_tests/test_mgmt_topics.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/tests/mgmt_tests/test_mgmt_namespaces.py` & `azure-servicebus-7.9.0b1/tests/mgmt_tests/test_mgmt_namespaces.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/tests/mgmt_tests/async/test_mgmt_topics_async.py` & `azure-servicebus-7.9.0b1/tests/mgmt_tests/async/test_mgmt_topics_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/tests/mgmt_tests/async/test_mgmt_queues_async.py` & `azure-servicebus-7.9.0b1/tests/mgmt_tests/async/test_mgmt_queues_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/tests/mgmt_tests/async/test_mgmt_rules_async.py` & `azure-servicebus-7.9.0b1/tests/mgmt_tests/async/test_mgmt_rules_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/tests/mgmt_tests/async/mgmt_test_utilities_async.py` & `azure-servicebus-7.9.0b1/tests/mgmt_tests/async/mgmt_test_utilities_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/tests/mgmt_tests/async/test_mgmt_namespaces_async.py` & `azure-servicebus-7.9.0b1/tests/mgmt_tests/async/test_mgmt_namespaces_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/tests/mgmt_tests/async/test_mgmt_subscriptions_async.py` & `azure-servicebus-7.9.0b1/tests/mgmt_tests/async/test_mgmt_subscriptions_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/async_samples/mgmt_rule_async.py` & `azure-servicebus-7.9.0b1/samples/async_samples/mgmt_rule_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/async_samples/receive_deferred_message_queue_async.py` & `azure-servicebus-7.9.0b1/samples/async_samples/receive_deferred_message_queue_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/async_samples/deadletter_messages_and_correct_async.py` & `azure-servicebus-7.9.0b1/samples/async_samples/deadletter_messages_and_correct_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/async_samples/proxy_async.py` & `azure-servicebus-7.9.0b1/samples/async_samples/proxy_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/async_samples/send_queue_async.py` & `azure-servicebus-7.9.0b1/samples/async_samples/send_queue_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/async_samples/receive_peek_async.py` & `azure-servicebus-7.9.0b1/samples/async_samples/receive_peek_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/async_samples/session_pool_receive_async.py` & `azure-servicebus-7.9.0b1/samples/async_samples/session_pool_receive_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/async_samples/authenticate_using_azure_sas_credential_async.py` & `azure-servicebus-7.9.0b1/samples/async_samples/authenticate_using_azure_sas_credential_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/async_samples/client_identity_authentication_async.py` & `azure-servicebus-7.9.0b1/samples/async_samples/client_identity_authentication_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/async_samples/receive_iterator_queue_async.py` & `azure-servicebus-7.9.0b1/samples/async_samples/receive_iterator_queue_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/async_samples/mgmt_subscription_async.py` & `azure-servicebus-7.9.0b1/samples/async_samples/mgmt_subscription_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/async_samples/receive_subscription_async.py` & `azure-servicebus-7.9.0b1/samples/async_samples/receive_subscription_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/async_samples/authenticate_client_connstr_async.py` & `azure-servicebus-7.9.0b1/samples/async_samples/authenticate_client_connstr_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/async_samples/connection_to_custom_endpoint_address_async.py` & `azure-servicebus-7.9.0b1/samples/async_samples/connection_to_custom_endpoint_address_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/async_samples/send_and_receive_amqp_annotated_message_async.py` & `azure-servicebus-7.9.0b1/samples/async_samples/send_and_receive_amqp_annotated_message_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/async_samples/send_topic_async.py` & `azure-servicebus-7.9.0b1/samples/async_samples/send_topic_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/async_samples/schedule_topic_messages_and_cancellation_async.py` & `azure-servicebus-7.9.0b1/samples/async_samples/schedule_topic_messages_and_cancellation_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/async_samples/schedule_messages_and_cancellation_async.py` & `azure-servicebus-7.9.0b1/samples/async_samples/schedule_messages_and_cancellation_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/async_samples/mgmt_topic_async.py` & `azure-servicebus-7.9.0b1/samples/async_samples/mgmt_topic_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/async_samples/mgmt_queue_async.py` & `azure-servicebus-7.9.0b1/samples/async_samples/mgmt_queue_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/async_samples/authenticate_using_azure_named_key_credential_async.py` & `azure-servicebus-7.9.0b1/samples/async_samples/authenticate_using_azure_named_key_credential_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/async_samples/sample_code_servicebus_async.py` & `azure-servicebus-7.9.0b1/samples/async_samples/sample_code_servicebus_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/async_samples/receive_queue_async.py` & `azure-servicebus-7.9.0b1/samples/async_samples/receive_queue_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/async_samples/receive_deadlettered_messages_async.py` & `azure-servicebus-7.9.0b1/samples/async_samples/receive_deadlettered_messages_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/async_samples/topic_subscription_with_rule_operations_async.py` & `azure-servicebus-7.9.0b1/samples/async_samples/topic_subscription_with_rule_operations_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/async_samples/auto_lock_renew_async.py` & `azure-servicebus-7.9.0b1/samples/async_samples/auto_lock_renew_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/async_samples/session_send_receive_async.py` & `azure-servicebus-7.9.0b1/samples/async_samples/session_send_receive_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/sync_samples/mgmt_rule.py` & `azure-servicebus-7.9.0b1/samples/sync_samples/mgmt_rule.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/sync_samples/receive_deadlettered_messages.py` & `azure-servicebus-7.9.0b1/samples/sync_samples/receive_deadlettered_messages.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/sync_samples/generate_sas_token_and_authenticate_client.py` & `azure-servicebus-7.9.0b1/samples/sync_samples/generate_sas_token_and_authenticate_client.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/sync_samples/authenticate_client_connstr.py` & `azure-servicebus-7.9.0b1/samples/sync_samples/authenticate_client_connstr.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/sync_samples/session_send_receive.py` & `azure-servicebus-7.9.0b1/samples/sync_samples/session_send_receive.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/sync_samples/connection_to_custom_endpoint_address.py` & `azure-servicebus-7.9.0b1/samples/sync_samples/connection_to_custom_endpoint_address.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/sync_samples/failure_and_recovery.py` & `azure-servicebus-7.9.0b1/samples/sync_samples/failure_and_recovery.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/sync_samples/sample_code_servicebus.py` & `azure-servicebus-7.9.0b1/samples/sync_samples/sample_code_servicebus.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/sync_samples/client_identity_authentication.py` & `azure-servicebus-7.9.0b1/samples/sync_samples/client_identity_authentication.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/sync_samples/deadletter_messages_and_correct.py` & `azure-servicebus-7.9.0b1/samples/sync_samples/deadletter_messages_and_correct.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/sync_samples/receive_subscription.py` & `azure-servicebus-7.9.0b1/samples/sync_samples/receive_subscription.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/sync_samples/mgmt_queue.py` & `azure-servicebus-7.9.0b1/samples/sync_samples/mgmt_queue.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/sync_samples/authenticate_using_azure_named_key_credential.py` & `azure-servicebus-7.9.0b1/samples/sync_samples/authenticate_using_azure_named_key_credential.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/sync_samples/authenticate_using_azure_sas_credential.py` & `azure-servicebus-7.9.0b1/samples/sync_samples/authenticate_using_azure_sas_credential.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/sync_samples/send_topic.py` & `azure-servicebus-7.9.0b1/samples/sync_samples/send_topic.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/sync_samples/send_and_receive_amqp_annotated_message.py` & `azure-servicebus-7.9.0b1/samples/sync_samples/send_and_receive_amqp_annotated_message.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/sync_samples/topic_subscription_with_rule_operations.py` & `azure-servicebus-7.9.0b1/samples/sync_samples/topic_subscription_with_rule_operations.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/sync_samples/proxy.py` & `azure-servicebus-7.9.0b1/samples/sync_samples/proxy.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/sync_samples/receive_deferred_message_queue.py` & `azure-servicebus-7.9.0b1/samples/sync_samples/receive_deferred_message_queue.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/sync_samples/receive_peek.py` & `azure-servicebus-7.9.0b1/samples/sync_samples/receive_peek.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/sync_samples/receive_queue.py` & `azure-servicebus-7.9.0b1/samples/sync_samples/receive_queue.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/sync_samples/mgmt_subscription.py` & `azure-servicebus-7.9.0b1/samples/sync_samples/mgmt_subscription.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/sync_samples/schedule_topic_messages_and_cancellation.py` & `azure-servicebus-7.9.0b1/samples/sync_samples/schedule_topic_messages_and_cancellation.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/sync_samples/receive_iterator_queue.py` & `azure-servicebus-7.9.0b1/samples/sync_samples/receive_iterator_queue.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/sync_samples/session_pool_receive.py` & `azure-servicebus-7.9.0b1/samples/sync_samples/session_pool_receive.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/sync_samples/send_queue.py` & `azure-servicebus-7.9.0b1/samples/sync_samples/send_queue.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/sync_samples/mgmt_topic.py` & `azure-servicebus-7.9.0b1/samples/sync_samples/mgmt_topic.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/samples/sync_samples/schedule_messages_and_cancellation.py` & `azure-servicebus-7.9.0b1/samples/sync_samples/schedule_messages_and_cancellation.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_servicebus_session.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_servicebus_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # --------------------------------------------------------------------------------------------
 import logging
 import datetime
 import warnings
 from typing import TYPE_CHECKING, Any, Union, Optional
-import six
 
 from ._common.utils import utc_from_timestamp, utc_now
 from ._common.constants import (
     REQUEST_RESPONSE_GET_SESSION_STATE_OPERATION,
     REQUEST_RESPONSE_SET_SESSION_STATE_OPERATION,
     REQUEST_RESPONSE_RENEW_SESSION_LOCK_OPERATION,
     MGMT_RESPONSE_SESSION_STATE,
@@ -118,20 +117,22 @@
             {MGMT_REQUEST_SESSION_ID: self._session_id},
             mgmt_handlers.default,
             timeout=timeout,
         )
         session_state = response.get(MGMT_RESPONSE_SESSION_STATE)  # type: ignore
         return session_state
 
-    def set_state(self, state: Union[str, bytes, bytearray], *, timeout: Optional[float] = None, **kwargs: Any) -> None:
+    def set_state(
+        self, state: Optional[Union[str, bytes, bytearray]], *, timeout: Optional[float] = None, **kwargs: Any
+    ) -> None:
         # pylint: disable=protected-access
         """Set the session state.
 
-        :param state: The state value.
-        :type state: Union[str, bytes, bytearray]
+        :param state: The state value. Setting state to None will clear the current session.
+        :type state: Union[str, bytes, bytearray, None]
         :keyword float timeout: The total operation timeout in seconds including all the retries. The value must be
          greater than 0 if specified. The default value is None, meaning no timeout.
 
         .. admonition:: Example:
 
             .. literalinclude:: ../samples/sync_samples/sample_code_servicebus.py
                 :start-after: [START set_session_state_sync]
@@ -142,21 +143,21 @@
         """
         if kwargs:
             warnings.warn(f"Unsupported keyword args: {kwargs}")
         self._receiver._check_live()  # pylint: disable=protected-access
         if timeout is not None and timeout <= 0:
             raise ValueError("The timeout must be greater than 0.")
         state = (
-            state.encode(self._encoding) if isinstance(state, six.text_type) else state
+            state.encode(self._encoding) if isinstance(state, str) else state
         )
         return self._receiver._mgmt_request_response_with_retry(  # type: ignore
             REQUEST_RESPONSE_SET_SESSION_STATE_OPERATION,
             {
                 MGMT_REQUEST_SESSION_ID: self._session_id,
-                MGMT_REQUEST_SESSION_STATE: bytearray(state),
+                MGMT_REQUEST_SESSION_STATE: bytearray(state) if state is not None else None,
             },
             mgmt_handlers.default,
             timeout=timeout,
         )
 
     def renew_lock(self, *, timeout: Optional[float] = None, **kwargs: Any) -> datetime.datetime:
         # pylint: disable=protected-access
@@ -192,12 +193,10 @@
         expiry = self._receiver._mgmt_request_response_with_retry(
             REQUEST_RESPONSE_RENEW_SESSION_LOCK_OPERATION,
             {MGMT_REQUEST_SESSION_ID: self._session_id},
             mgmt_handlers.session_lock_renew_op,
             timeout=timeout,
         )
         expiry_timestamp = expiry[MGMT_RESPONSE_RECEIVER_EXPIRATION] / 1000.0  # type: ignore
-        self._locked_until_utc = utc_from_timestamp(
-            expiry_timestamp
-        )  # type: datetime.datetime
+        self._locked_until_utc = utc_from_timestamp(expiry_timestamp)  # type: datetime.datetime
 
         return self._locked_until_utc
```

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_base_handler.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_base_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -411,17 +411,20 @@
                 self._backoff(
                     retried_times=retried_times,
                     last_exception=last_exception,
                     abs_timeout_time=abs_timeout_time,
                 )
 
     def _backoff(
-        self, retried_times, last_exception, abs_timeout_time=None, entity_name=None
-    ):
-        # type: (int, Exception, Optional[float], str) -> None
+        self,
+        retried_times: int,
+        last_exception: Exception,
+        abs_timeout_time: Optional[float] = None,
+        entity_name: Optional[str] = None
+    ) -> None:
         entity_name = entity_name or self._container_id
         backoff = _get_backoff_time(
                     self._config.retry_mode,
                     self._config.retry_backoff_factor,
                     self._config.retry_backoff_max,
                     retried_times,
                 )
```

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_servicebus_client.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_servicebus_client.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/exceptions.py` & `azure-servicebus-7.9.0b1/azure/servicebus/exceptions.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_servicebus_sender.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_servicebus_sender.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,24 +270,28 @@
                 self._handler._link.remote_max_message_size
                 or MAX_MESSAGE_LENGTH_BYTES
             )
         except:
             self._close_handler()
             raise
 
-    def _send(self, message, timeout=None):
-        # type: (Union[ServiceBusMessage, ServiceBusMessageBatch], Optional[float]) -> None
+    def _send(
+        self,
+        message: Union[ServiceBusMessage, ServiceBusMessageBatch],
+        timeout: Optional[float] = None,
+        last_exception: Optional[Exception] = None  # pylint: disable=unused-argument
+    ) -> None:
         self._open()
         try:
             # TODO This is not batch message sending?
             if isinstance(message, ServiceBusMessageBatch):
                 for batch_message in message._messages: # pylint:disable=protected-access
                     self._handler.send_message(batch_message.raw_amqp_message._to_outgoing_amqp_message(), timeout=timeout) # pylint:disable=line-too-long, protected-access
             else:
-                self._handler.send_message(message.raw_amqp_message._to_outgoing_amqp_message(), timeout=timeout) # pylint:disable=protected-access
+                self._handler.send_message(message.raw_amqp_message._to_outgoing_amqp_message(), timeout=timeout) # pylint:disable=protected-access,line-too-long
         except TimeoutError:
             raise OperationTimeoutError(message="Send operation timed out")
         except MessageException as e:
             raise _create_servicebus_exception(_LOGGER, e)
 
     def schedule_messages(
         self,
@@ -455,17 +459,20 @@
                 and len(obj_message) == 0
             ):  # pylint: disable=len-as-condition
                 return  # Short circuit noop if an empty list or batch is provided.
 
             obj_message = cast(Union[ServiceBusMessage, ServiceBusMessageBatch], obj_message)
             if send_span:
                 self._add_span_request_attributes(send_span)
-            self._send(
+            self._do_retryable_operation(
+                self._send,
                 message=obj_message,
-                timeout=timeout
+                timeout=timeout,
+                operation_requires_timeout=True,
+                require_last_exception=True,
             )
 
     def create_message_batch(
         self,
         max_size_in_bytes: Optional[int] = None
     ) -> ServiceBusMessageBatch:
         """Create a ServiceBusMessageBatch object with the max size of all content being constrained by
```

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/__init__.py` & `azure-servicebus-7.9.0b1/azure/servicebus/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_servicebus_receiver.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_servicebus_receiver.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,43 +222,29 @@
 
     def __iter__(self):
         return self._iter_contextual_wrapper()
 
     def _iter_contextual_wrapper(self, max_wait_time=None):
         """The purpose of this wrapper is to allow both state restoration (for multiple concurrent iteration)
         and per-iter argument passing that requires the former."""
-        # pylint: disable=protected-access
-        original_timeout = None
         while True:
-            # This is not threadsafe, but gives us a way to handle if someone passes
-            # different max_wait_times to different iterators and uses them in concert.
-            if max_wait_time:
-                # _timeout to _idle_timeout
-                original_timeout = self._handler._idle_timeout
-                self._handler._idle_timeout = max_wait_time * 1000
             try:
-                message = self._inner_next()
+                message = self._inner_next(wait_time=max_wait_time)
                 links = get_receive_links(message)
                 with receive_trace_context_manager(self, links=links):
                     yield message
             except StopIteration:
                 break
-            finally:
-                if original_timeout:
-                    try:
-                        self._handler._timeout = original_timeout
-                    except AttributeError:  # Handler may be disposed already.
-                        pass
 
-    def _inner_next(self):
+    def _inner_next(self, wait_time=None):
         # We do this weird wrapping such that an imperitive next() call, and a generator-based iter both trace sanely.
         self._check_live()
         while True:
             try:
-                return self._do_retryable_operation(self._iter_next)
+                return self._do_retryable_operation(self._iter_next, wait_time=wait_time)
             except StopIteration:
                 self._message_iter = None
                 raise
 
     def __next__(self):
         # Normally this would wrap the yield of the iter, but for a direct next call we just trace imperitively.
         try:
@@ -268,23 +254,22 @@
             with receive_trace_context_manager(self, links=links):
                 return message
         finally:
             self._receive_context.clear()
 
     next = __next__  # for python2.7
 
-    def _iter_next(self):
+    def _iter_next(self, wait_time=None):
         try:
             self._receive_context.set()
             self._open()
-            # TODO: Add in Recieve Message Iterator
-            # if not self._message_iter:
-            #     self._message_iter = self._handler.receive_messages_iter()
-            uamqp_message = next(self._message_iter)
-            message = self._build_message(uamqp_message)
+            if not self._message_iter or wait_time:
+                self._message_iter = self._handler.receive_messages_iter(timeout=wait_time)
+            pyamqp_message = next(self._message_iter)
+            message = self._build_message(pyamqp_message)
             if (
                 self._auto_lock_renewer
                 and not self._session
                 and self._receive_mode != ServiceBusReceiveMode.RECEIVE_AND_DELETE
             ):
                 self._auto_lock_renewer.register(self, message)
             return message
@@ -371,15 +356,15 @@
             retry_policy=self._error_policy,
             client_name=self._name,
             on_attach=self._on_attach,
             receive_settle_mode=ServiceBusToAMQPReceiveModeMap[self._receive_mode],
             send_settle_mode=SenderSettleMode.Settled
             if self._receive_mode == ServiceBusReceiveMode.RECEIVE_AND_DELETE
             else SenderSettleMode.Unsettled,
-            timeout=self._max_wait_time * 1000 if self._max_wait_time else 0,
+            timeout=self._max_wait_time * 1 if self._max_wait_time else 0,
             link_credit=self._prefetch_count,
             # If prefetch is 1, then keep_alive coroutine serves as keep receiving for releasing messages
             keep_alive_interval=self._config.keep_alive
             if self._prefetch_count != 1
             else 5,
             shutdown_after_timeout=False,
             link_properties={CONSUMER_IDENTIFIER: self._name},
```

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/aio/_servicebus_client_async.py` & `azure-servicebus-7.9.0b1/azure/servicebus/aio/_servicebus_client_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/aio/_base_handler_async.py` & `azure-servicebus-7.9.0b1/azure/servicebus/aio/_base_handler_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -355,15 +355,15 @@
             message=message,
             callback=callback,
             timeout=timeout,
             operation_requires_timeout=True,
             **kwargs
         )
 
-    async def _add_span_request_attributes(self, span):
+    def _add_span_request_attributes(self, span):
         return BaseHandlerSync._add_span_request_attributes(  # pylint: disable=protected-access
             self, span
         )
 
     async def _open(self):  # pylint: disable=no-self-use
         raise ValueError("Subclass should override the method.")
```

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/aio/_servicebus_session_async.py` & `azure-servicebus-7.9.0b1/azure/servicebus/aio/_servicebus_session_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/aio/__init__.py` & `azure-servicebus-7.9.0b1/azure/servicebus/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/aio/_async_utils.py` & `azure-servicebus-7.9.0b1/azure/servicebus/aio/_async_utils.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/aio/_async_auto_lock_renewer.py` & `azure-servicebus-7.9.0b1/azure/servicebus/aio/_async_auto_lock_renewer.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/aio/_servicebus_receiver_async.py` & `azure-servicebus-7.9.0b1/azure/servicebus/aio/_servicebus_receiver_async.py`

 * *Files 5% similar despite different names*

```diff
@@ -210,81 +210,64 @@
         )
         self._session = (
             None if self._session_id is None else ServiceBusSession(cast(str, self._session_id), self)
         )
         self._receive_context = asyncio.Event()
         self._handler: ReceiveClientAsync
 
-    # Python 3.5 does not allow for yielding from a coroutine, so instead of the try-finally functional wrapper
-    # trick to restore the timeout, let's use a wrapper class to maintain the override that may be specified.
-    class _IterContextualWrapper(collections.abc.AsyncIterator):
-        def __init__(self, receiver, max_wait_time=None):
-            self.receiver = receiver
-            self.max_wait_time = max_wait_time
-
-        async def __anext__(self):
-            # pylint: disable=protected-access
-            original_timeout = None
-            # This is not threadsafe, but gives us a way to handle if someone passes
-            # different max_wait_times to different iterators and uses them in concert.
-            if self.max_wait_time and self.receiver and self.receiver._handler:
-                # TODO: What did the previous _handler.timeout represent here?
-                original_timeout = self.receiver._handler._idle_timeout
-                self.receiver._handler._timeout = self.max_wait_time * 1000
+    async def _iter_contextual_wrapper(self, max_wait_time=None):
+        while True:
             try:
-                self.receiver._receive_context.set()
-                message = await self.receiver._inner_anext()
+                message = await self._inner_anext(wait_time=max_wait_time)
                 links = get_receive_links(message)
-                with receive_trace_context_manager(self.receiver, links=links):
-                    return message
-            finally:
-                self.receiver._receive_context.clear()
-                if original_timeout:
-                    try:
-                        self.receiver._handler._timeout = original_timeout
-                    except AttributeError:  # Handler may be disposed already.
-                        pass
+                with receive_trace_context_manager(self, links=links):
+                    yield message
+            except StopAsyncIteration:
+                break
 
     def __aiter__(self):
-        return self._IterContextualWrapper(self)
+        return self._iter_contextual_wrapper()
 
-    async def _inner_anext(self):
+    async def _inner_anext(self, wait_time=None):
         # We do this weird wrapping such that an imperitive next() call, and a generator-based iter both trace sanely.
         self._check_live()
         while True:
             try:
-                return await self._do_retryable_operation(self._iter_next)
+                return await self._do_retryable_operation(self._iter_next, wait_time=wait_time)
             except StopAsyncIteration:
                 self._message_iter = None
                 raise
 
     async def __anext__(self):
         try:
             self._receive_context.set()
             message = await self._inner_anext()
             links = get_receive_links(message)
             with receive_trace_context_manager(self, links=links):
                 return message
         finally:
             self._receive_context.clear()
 
-    async def _iter_next(self):
-        await self._open()
-        # TODO: Add in Recieve Message Iterator
-        # if not self._message_iter:
-        #     self._message_iter = self._handler.receive_messages_iter_async()
-        uamqp_message = await self._message_iter.__anext__()
-        message = self._build_message(uamqp_message)
-        if (
-            self._auto_lock_renewer
-            and not self._session
-            and self._receive_mode != ServiceBusReceiveMode.RECEIVE_AND_DELETE
-        ):
-            self._auto_lock_renewer.register(self, message)
-        return message
+    async def _iter_next(self, wait_time=None): # pylint: disable=protected-access
+        try:
+            self._receive_context.set()
+            await self._open()
+            if not self._message_iter or wait_time:
+                self._message_iter = await self._handler.receive_messages_iter_async(timeout=wait_time)
+            pyamqp_message = await self._message_iter.__anext__()
+            message = self._build_message(pyamqp_message)
+            if (
+                self._auto_lock_renewer
+                and not self._session
+                and self._receive_mode != ServiceBusReceiveMode.RECEIVE_AND_DELETE
+            ):
+                self._auto_lock_renewer.register(self, message)
+            return message
+        finally:
+            self._receive_context.clear()
 
     @classmethod
     def _from_connection_string(
         cls, conn_str: str, **kwargs: Any
     ) -> "ServiceBusReceiver":
         """Create a ServiceBusReceiver from a connection string.
 
@@ -376,23 +359,25 @@
             retry_policy=self._error_policy,
             client_name=self._name,
             on_attach=self._on_attach,
             receive_settle_mode=ServiceBusToAMQPReceiveModeMap[self._receive_mode],
             send_settle_mode=SenderSettleMode.Settled
             if self._receive_mode == ServiceBusReceiveMode.RECEIVE_AND_DELETE
             else SenderSettleMode.Unsettled,
-            #timeout=self._max_wait_time * 1000 if self._max_wait_time else 0, TODO: This is not working
+            timeout=self._max_wait_time * 1 if self._max_wait_time else 0,
             link_credit=self._prefetch_count,
             # If prefetch is 1, then keep_alive coroutine serves as keep receiving for releasing messages
-            keep_alive_interval=self._config.keep_alive if self._prefetch_count != 1 else 5,
+            keep_alive_interval=self._config.keep_alive
+            if self._prefetch_count != 1
+            else 5,
             shutdown_after_timeout=False,
             link_properties = {CONSUMER_IDENTIFIER:self._name}
         )
         if self._prefetch_count == 1:
-            self._handler._message_received = self._enhanced_message_received  # pylint: disable=protected-access
+            self._handler._message_received_async = self._enhanced_message_received_async  # pylint: disable=protected-access
 
     async def _open(self):
         # pylint: disable=protected-access
         if self._running:
             return
         if self._handler and not self._handler._shutdown:
             await self._handler.close_async()
@@ -513,15 +498,15 @@
         message,
         settle_operation,
         dead_letter_reason=None,
         dead_letter_error_description=None,
     ):
         # type: (ServiceBusReceivedMessage, str, Optional[str], Optional[str]) -> None
         if settle_operation == MESSAGE_COMPLETE:
-            return await self._handler.settle_messages_async(message.delivery_id, 'accepted')
+            return await self._handler.settle_messages_async(message.delivery_id, 'accepted') # pylint:disable=line-too-long
         if settle_operation == MESSAGE_ABANDON:
             return await self._handler.settle_messages_async(
                 message.delivery_id,
                 'modified',
                 delivery_failed=True,
                 undeliverable_here=False
             )
@@ -669,15 +654,15 @@
                 :end-before: [END receive_forever_async]
                 :language: python
                 :dedent: 4
                 :caption: Receive indefinitely from an iterator in streaming fashion.
         """
         if max_wait_time is not None and max_wait_time <= 0:
             raise ValueError("The max_wait_time must be greater than 0.")
-        return self._IterContextualWrapper(self, max_wait_time)
+        return self._iter_contextual_wrapper(max_wait_time)
 
     async def receive_messages(
         self,
         max_message_count: Optional[int] = 1,
         max_wait_time: Optional[float] = None,
     ) -> List[ServiceBusReceivedMessage]:
         """Receive a batch of messages at once.
```

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/aio/_servicebus_sender_async.py` & `azure-servicebus-7.9.0b1/azure/servicebus/aio/_servicebus_sender_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,15 +278,15 @@
             else:
                 if len(obj_messages) == 0:
                     return []  # No-op on empty list.
                 request_body = self._build_schedule_request(
                     schedule_time_utc, send_span, *obj_messages
                 )
             if send_span:
-                await self._add_span_request_attributes(send_span)
+                self._add_span_request_attributes(send_span)
             return await self._mgmt_request_response_with_retry(
                 REQUEST_RESPONSE_SCHEDULE_MESSAGE_OPERATION,
                 request_body,
                 mgmt_handlers.schedule_op,
                 timeout=timeout,
             )
```

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/aio/management/_management_client_async.py` & `azure-servicebus-7.9.0b1/azure/servicebus/aio/management/_management_client_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/aio/management/_shared_key_policy_async.py` & `azure-servicebus-7.9.0b1/azure/servicebus/aio/management/_shared_key_policy_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/aio/management/_utils.py` & `azure-servicebus-7.9.0b1/azure/servicebus/aio/management/_utils.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/amqp/_constants.py` & `azure-servicebus-7.9.0b1/azure/servicebus/amqp/_constants.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/amqp/__init__.py` & `azure-servicebus-7.9.0b1/azure/servicebus/amqp/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/amqp/_amqp_message.py` & `azure-servicebus-7.9.0b1/azure/servicebus/amqp/_amqp_message.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/management/_api_version.py` & `azure-servicebus-7.9.0b1/azure/servicebus/management/_api_version.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/management/_handle_response_error.py` & `azure-servicebus-7.9.0b1/azure/servicebus/management/_handle_response_error.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/management/_models.py` & `azure-servicebus-7.9.0b1/azure/servicebus/management/_models.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/management/_xml_workaround_policy.py` & `azure-servicebus-7.9.0b1/azure/servicebus/management/_xml_workaround_policy.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/management/_constants.py` & `azure-servicebus-7.9.0b1/azure/servicebus/management/_constants.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/management/__init__.py` & `azure-servicebus-7.9.0b1/azure/servicebus/management/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/management/_shared_key_policy.py` & `azure-servicebus-7.9.0b1/azure/servicebus/management/_shared_key_policy.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/management/_management_client.py` & `azure-servicebus-7.9.0b1/azure/servicebus/management/_management_client.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/management/_model_workaround.py` & `azure-servicebus-7.9.0b1/azure/servicebus/management/_model_workaround.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/management/_utils.py` & `azure-servicebus-7.9.0b1/azure/servicebus/management/_utils.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/_configuration.py` & `azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/_service_bus_management_client.py` & `azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/_service_bus_management_client.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/__init__.py` & `azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/aio/__init__.py` & `azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/aio/_service_bus_management_client_async.py` & `azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/aio/_service_bus_management_client_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/aio/_configuration_async.py` & `azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/aio/_configuration_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/aio/operations_async/_service_bus_management_client_operations_async.py` & `azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/aio/operations_async/_service_bus_management_client_operations_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/aio/operations_async/_subscription_operations_async.py` & `azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/aio/operations_async/_subscription_operations_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/aio/operations_async/__init__.py` & `azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/aio/operations_async/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/aio/operations_async/_namespace_operations_async.py` & `azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/aio/operations_async/_namespace_operations_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/aio/operations_async/_entity_operations_async.py` & `azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/aio/operations_async/_entity_operations_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/aio/operations_async/_rule_operations_async.py` & `azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/aio/operations_async/_rule_operations_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/operations/__init__.py` & `azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/operations/_namespace_operations.py` & `azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/operations/_namespace_operations.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/operations/_entity_operations.py` & `azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/operations/_entity_operations.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/operations/_rule_operations.py` & `azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/operations/_rule_operations.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/operations/_service_bus_management_client_operations.py` & `azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/operations/_service_bus_management_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/operations/_subscription_operations.py` & `azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/operations/_subscription_operations.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/models/_models.py` & `azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/models/_models.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/models/_models_py3.py` & `azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/models/__init__.py` & `azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/management/_generated/models/_service_bus_management_client_enums.py` & `azure-servicebus-7.9.0b1/azure/servicebus/management/_generated/models/_service_bus_management_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_common/_configuration.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_common/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_common/utils.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_common/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,16 +262,19 @@
         with span_impl_type(name=span_name, kind=SpanKind.CLIENT) as child:
             yield child
     else:
         yield None
 
 
 @contextmanager
-def receive_trace_context_manager(receiver, span_name=SPAN_NAME_RECEIVE, links=None):
-    # type: (ReceiverMixin, str, List[Link]) -> Iterator[None]
+def receive_trace_context_manager(
+    receiver: "ReceiverMixin",
+    span_name: str = SPAN_NAME_RECEIVE,
+    links: Optional[List[Link]] = None
+) -> Iterator[None]:
     """Tracing"""
     span_impl_type = settings.tracing_implementation()  # type: Type[AbstractSpan]
     if span_impl_type is None:
         yield
     else:
         receive_span = span_impl_type(name=span_name, kind=SpanKind.CONSUMER, links=links)
         receiver._add_span_request_attributes(receive_span)  # type: ignore  # pylint: disable=protected-access
```

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_common/auto_lock_renewer.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_common/auto_lock_renewer.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_common/constants.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_common/constants.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_common/message.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_common/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 # pylint: disable=too-many-lines
 
 from __future__ import annotations
 import time
 import datetime
 import uuid
 from typing import Optional, Dict, List, Union, Iterable, Any, Mapping, cast, TYPE_CHECKING
-from azure.core.tracing import AbstractSpan
 
 from .._pyamqp.message import Message, BatchMessage
 from .._pyamqp.performatives import TransferFrame
 from .._pyamqp._message_backcompat import LegacyMessage, LegacyBatchMessage
 from .._pyamqp.utils import add_batch, get_message_encoded_size
 from .._pyamqp._encode import encode_payload
 
@@ -49,14 +48,15 @@
     utc_from_timestamp,
     utc_now,
     trace_message,
     transform_messages_if_needed,
 )
 
 if TYPE_CHECKING:
+    from azure.core.tracing import AbstractSpan
     from ..aio._servicebus_receiver_async import (
         ServiceBusReceiver as AsyncServiceBusReceiver,
     )
     from .._servicebus_receiver import ServiceBusReceiver
 PrimitiveTypes = Union[
     int,
     float,
@@ -640,26 +640,22 @@
             self.max_size_in_bytes, self._count
         )
         return "ServiceBusMessageBatch({})".format(batch_repr)
 
     def __len__(self) -> int:
         return self._count
 
-    def _from_list(
-            self,
-            messages: Iterable[ServiceBusMessage],
-            parent_span: AbstractSpan = None
-    ) -> None:
+    def _from_list(self, messages: Iterable[ServiceBusMessage], parent_span: Optional["AbstractSpan"] = None) -> None:
         for message in messages:
             self._add(message, parent_span)
 
     def _add(
-            self,
-            add_message: Union[ServiceBusMessage, Mapping[str, Any], AmqpAnnotatedMessage],
-            parent_span: AbstractSpan = None
+        self,
+        add_message: Union[ServiceBusMessage, Mapping[str, Any], AmqpAnnotatedMessage],
+        parent_span: Optional["AbstractSpan"] = None
     ) -> None:
         """Actual add implementation.  The shim exists to hide the internal parameters such as parent_span."""
         message = transform_messages_if_needed(add_message, ServiceBusMessage)
         message = cast(ServiceBusMessage, message)
         trace_message(
             message, parent_span
         )  # parent_span is e.g. if built as part of a send operation.
```

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_common/_connection_string_parser.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_common/_connection_string_parser.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_common/mgmt_handlers.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_common/mgmt_handlers.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/types.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/types.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/_transport.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/_transport.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,15 +52,19 @@
 from ._encode import encode_frame
 from ._decode import decode_frame, decode_empty_frame
 from .constants import (
     TLS_HEADER_FRAME,
     WEBSOCKET_PORT,
     TransportType,
     AMQP_WS_SUBPROTOCOL,
+    TIMEOUT_INTERVAL,
+    WS_TIMEOUT_INTERVAL,
+    READ_TIMEOUT_INTERVAL,
 )
+from .error import AuthenticationException, ErrorCondition
 
 
 try:
     import fcntl
 except ImportError:  # pragma: no cover
     fcntl = None    # type: ignore  # noqa
 
@@ -86,17 +90,14 @@
 _UNAVAIL = {errno.EAGAIN, errno.EINTR, errno.ENOENT, errno.EWOULDBLOCK}
 
 AMQP_PORT = 5672
 AMQPS_PORT = 5671
 AMQP_FRAME = memoryview(b"AMQP")
 EMPTY_BUFFER = bytes()
 SIGNED_INT_MAX = 0x7FFFFFFF
-TIMEOUT_INTERVAL = 1
-WS_TIMEOUT_INTERVAL = 1
-READ_TIMEOUT_INTERVAL = 0.2
 
 # Match things like: [fe80::1]:5432, from RFC 2732
 IPV6_LITERAL = re.compile(r"\[([\.0-9a-f:]+)\](?::(\d+))?")
 
 DEFAULT_SOCKET_SETTINGS = {
     "TCP_NODELAY": 1,
     "TCP_USER_TIMEOUT": 1000,
@@ -152,22 +153,23 @@
         host,
         *,
         port=AMQP_PORT,
         connect_timeout=None,
         read_timeout=None,
         socket_settings=None,
         raise_on_initial_eintr=True,
-        **kwargs    # pylint: disable=unused-argument
+        **kwargs
     ):
         self._quick_recv = None
         self.connected = False
         self.sock = None
         self.raise_on_initial_eintr = raise_on_initial_eintr
         self._read_buffer = BytesIO()
         self.host, self.port = to_host_port(host, port)
+        self.network_trace_params = kwargs.get('network_trace_params')
 
         self.connect_timeout = connect_timeout or TIMEOUT_INTERVAL
         self.read_timeout = read_timeout or READ_TIMEOUT_INTERVAL
         self.socket_settings = socket_settings
         self.socket_lock = Lock()
 
     def connect(self):
@@ -180,15 +182,16 @@
                 self.socket_settings,
                 self.read_timeout,
             )
             # we've sent the banner; signal connect
             # EINTR, EAGAIN, EWOULDBLOCK would signal that the banner
             # has _not_ been sent
             self.connected = True
-        except (OSError, IOError, SSLError):
+        except (OSError, IOError, SSLError) as e:
+            _LOGGER.info("Transport connection failed: %r", e, extra=self.network_trace_params)
             # if not fully connected, close socket, and reraise error
             if self.sock and not self.connected:
                 self.sock.close()
                 self.sock = None
             raise
 
     @contextmanager
@@ -382,84 +385,99 @@
         """Do any preliminary work in shutting down the connection."""
 
     def _write(self, s):
         """Completely write a string to the peer."""
         raise NotImplementedError("Must be overriden in subclass")
 
     def close(self):
-        if self.sock is not None:
-            self._shutdown_transport()
-            # Call shutdown first to make sure that pending messages
-            # reach the AMQP broker if the program exits after
-            # calling this method.
-            try:
-                self.sock.shutdown(socket.SHUT_RDWR)
-            except Exception as exc:  # pylint: disable=broad-except
-                # TODO: shutdown could raise OSError, Transport endpoint is not connected if the endpoint is already
-                #  disconnected. can we safely ignore the errors since the close operation is initiated by us.
-                _LOGGER.info("Transport endpoint is already disconnected: %r", exc)
-            self.sock.close()
-            self.sock = None
-        self.connected = False
+        with self.socket_lock:
+            if self.sock is not None:
+                self._shutdown_transport()
+                # Call shutdown first to make sure that pending messages
+                # reach the AMQP broker if the program exits after
+                # calling this method.
+                try:
+                    self.sock.shutdown(socket.SHUT_RDWR)
+                except Exception as exc:  # pylint: disable=broad-except
+                    # TODO: shutdown could raise OSError, Transport endpoint is not connected if the endpoint is already
+                    #  disconnected. can we safely ignore the errors since the close operation is initiated by us.
+                    _LOGGER.debug(
+                        "Transport endpoint is already disconnected: %r",
+                        exc,
+                        extra=self.network_trace_params
+                    )
+                self.sock.close()
+                self.sock = None
+            self.connected = False
 
     def read(self, verify_frame_type=0):
-        read = self._read
-        read_frame_buffer = BytesIO()
-        try:
-            frame_header = memoryview(bytearray(8))
-            read_frame_buffer.write(read(8, buffer=frame_header, initial=True))
+        with self.socket_lock:
+            read = self._read
+            read_frame_buffer = BytesIO()
+            try:
+                frame_header = memoryview(bytearray(8))
+                read_frame_buffer.write(read(8, buffer=frame_header, initial=True))
 
-            channel = struct.unpack(">H", frame_header[6:])[0]
-            size = frame_header[0:4]
-            if size == AMQP_FRAME:  # Empty frame or AMQP header negotiation TODO
-                return frame_header, channel, None
-            size = struct.unpack(">I", size)[0]
-            offset = frame_header[4]
-            frame_type = frame_header[5]
-            if verify_frame_type is not None and frame_type != verify_frame_type:
-                raise ValueError(
-                    f"Received invalid frame type: {frame_type}, expected: {verify_frame_type}"
-                )
+                channel = struct.unpack(">H", frame_header[6:])[0]
+                size = frame_header[0:4]
+                if size == AMQP_FRAME:  # Empty frame or AMQP header negotiation TODO
+                    return frame_header, channel, None
+                size = struct.unpack(">I", size)[0]
+                offset = frame_header[4]
+                frame_type = frame_header[5]
+                if verify_frame_type is not None and frame_type != verify_frame_type:
+                    _LOGGER.debug(
+                        "Received invalid frame type: %r, expected: %r",
+                        frame_type,
+                        verify_frame_type,
+                        extra=self.network_trace_params
+                    )
+                    raise ValueError(
+                            f"Received invalid frame type: {frame_type}, expected: {verify_frame_type}"
+                    )
 
-            # >I is an unsigned int, but the argument to sock.recv is signed,
-            # so we know the size can be at most 2 * SIGNED_INT_MAX
-            payload_size = size - len(frame_header)
-            payload = memoryview(bytearray(payload_size))
-            if size > SIGNED_INT_MAX:
-                read_frame_buffer.write(read(SIGNED_INT_MAX, buffer=payload))
-                read_frame_buffer.write(
-                    read(size - SIGNED_INT_MAX, buffer=payload[SIGNED_INT_MAX:])
-                )
-            else:
-                read_frame_buffer.write(read(payload_size, buffer=payload))
-        except (socket.timeout, TimeoutError):
-            read_frame_buffer.write(self._read_buffer.getvalue())
-            self._read_buffer = read_frame_buffer
-            self._read_buffer.seek(0)
-            raise
-        except (OSError, IOError, SSLError, socket.error) as exc:
-            # Don't disconnect for ssl read time outs
-            # http://bugs.python.org/issue10272
-            if isinstance(exc, SSLError) and "timed out" in str(exc):
-                raise socket.timeout()
-            if get_errno(exc) not in _UNAVAIL:
-                self.connected = False
-            raise
-        offset -= 2
+                # >I is an unsigned int, but the argument to sock.recv is signed,
+                # so we know the size can be at most 2 * SIGNED_INT_MAX
+                payload_size = size - len(frame_header)
+                payload = memoryview(bytearray(payload_size))
+                if size > SIGNED_INT_MAX:
+                    read_frame_buffer.write(read(SIGNED_INT_MAX, buffer=payload))
+                    read_frame_buffer.write(
+                        read(size - SIGNED_INT_MAX, buffer=payload[SIGNED_INT_MAX:])
+                    )
+                else:
+                    read_frame_buffer.write(read(payload_size, buffer=payload))
+            except (socket.timeout, TimeoutError):
+                read_frame_buffer.write(self._read_buffer.getvalue())
+                self._read_buffer = read_frame_buffer
+                self._read_buffer.seek(0)
+                raise
+            except (OSError, IOError, SSLError, socket.error) as exc:
+                # Don't disconnect for ssl read time outs
+                # http://bugs.python.org/issue10272
+                if isinstance(exc, SSLError) and "timed out" in str(exc):
+                    raise socket.timeout()
+                if get_errno(exc) not in _UNAVAIL:
+                    self.connected = False
+                _LOGGER.debug("Transport read failed: %r", exc, extra=self.network_trace_params)
+                raise
+            offset -= 2
         return frame_header, channel, payload[offset:]
 
     def write(self, s):
-        try:
-            self._write(s)
-        except socket.timeout:
-            raise
-        except (OSError, IOError, socket.error) as exc:
-            if get_errno(exc) not in _UNAVAIL:
-                self.connected = False
-            raise
+        with self.socket_lock:
+            try:
+                self._write(s)
+            except socket.timeout:
+                raise
+            except (OSError, IOError, socket.error) as exc:
+                _LOGGER.debug("Transport write failed: %r", exc, extra=self.network_trace_params)
+                if get_errno(exc) not in _UNAVAIL:
+                    self.connected = False
+                raise
 
     def receive_frame(self, **kwargs):
         try:
             header, channel, payload = self.read(**kwargs)
             if not payload:
                 decoded = decode_empty_frame(header)
             else:
@@ -547,15 +565,23 @@
             "do_handshake_on_connect": do_handshake_on_connect,
             "suppress_ragged_eofs": suppress_ragged_eofs,
             "ciphers": ciphers,
             #'ssl_version': ssl_version
         }
 
         # TODO: We need to refactor this.
-        sock = ssl.wrap_socket(**opts)  # pylint: disable=deprecated-method
+        try:
+            sock = ssl.wrap_socket(**opts)  # pylint: disable=deprecated-method
+        except FileNotFoundError as exc:
+            # FileNotFoundError does not have missing filename info, so adding it below.
+            # Assuming that this must be ca_certs, since this is the only file path that
+            # users can pass in (`connection_verify` in the EH/SB clients) through opts above.
+            # For uamqp exception parity. Remove later when resolving issue #27128.
+            exc.filename = {"ca_certs": ca_certs}
+            raise exc
         # Set SNI headers if supported
         if (
             (server_hostname is not None)
             and (hasattr(ssl, "HAS_SNI") and ssl.HAS_SNI)
             and (hasattr(ssl, "SSLContext"))
         ):
             context = ssl.SSLContext(opts["ssl_version"])
@@ -680,60 +706,100 @@
             http_proxy_host = self._http_proxy["proxy_hostname"]
             http_proxy_port = self._http_proxy["proxy_port"]
             username = self._http_proxy.get("username", None)
             password = self._http_proxy.get("password", None)
             if username or password:
                 http_proxy_auth = (username, password)
         try:
-            from websocket import create_connection
-
+            from websocket import (
+                create_connection,
+                WebSocketAddressException,
+                WebSocketTimeoutException,
+                WebSocketConnectionClosedException
+            )
+        except ImportError:
+            raise ImportError(
+                "Please install websocket-client library to use sync websocket transport."
+            )
+        try:
             self.ws = create_connection(
                 url="wss://{}".format(self._custom_endpoint or self._host),
                 subprotocols=[AMQP_WS_SUBPROTOCOL],
                 timeout=self._connect_timeout,
                 skip_utf8_validation=True,
                 sslopt=self.sslopts,
                 http_proxy_host=http_proxy_host,
                 http_proxy_port=http_proxy_port,
                 http_proxy_auth=http_proxy_auth,
             )
-        except ImportError:
-            raise ValueError(
-                "Please install websocket-client library to use websocket transport."
+        except WebSocketAddressException as exc:
+            raise AuthenticationException(
+                ErrorCondition.ClientError,
+                description="Failed to authenticate the connection due to exception: " + str(exc),
+                error=exc,
             )
+        # TODO: resolve pylance error when type: ignore is removed below, issue #22051
+        except (WebSocketTimeoutException, SSLError, WebSocketConnectionClosedException) as exc:    # type: ignore
+            self.close()
+            raise ConnectionError("Websocket failed to establish connection: %r" % exc) from exc
+        except (OSError, IOError, SSLError) as e:
+            _LOGGER.info("Websocket connection failed: %r", e, extra=self.network_trace_params)
+            self.close()
+            raise
 
     def _read(self, n, initial=False, buffer=None, _errnos=None):  # pylint: disable=unused-argument
         """Read exactly n bytes from the peer."""
         from websocket import WebSocketTimeoutException
-
-        length = 0
-        view = buffer or memoryview(bytearray(n))
-        nbytes = self._read_buffer.readinto(view)
-        length += nbytes
-        n -= nbytes
         try:
-            while n:
-                data = self.ws.recv()
+            length = 0
+            view = buffer or memoryview(bytearray(n))
+            nbytes = self._read_buffer.readinto(view)
+            length += nbytes
+            n -= nbytes
+            try:
+                while n:
+                    data = self.ws.recv()
+                    if len(data) <= n:
+                        view[length : length + len(data)] = data
+                        n -= len(data)
+                        length += len(data)
+                    else:
+                        view[length : length + n] = data[0:n]
+                        self._read_buffer = BytesIO(data[n:])
+                        n = 0
+                return view
+            except AttributeError:
+                raise IOError("Websocket connection has already been closed.")
+            except WebSocketTimeoutException as wte:
+                raise TimeoutError('Websocket receive timed out (%s)' % wte)
+        except:
+            self._read_buffer = BytesIO(view[:length])
+            raise
 
-                if len(data) <= n:
-                    view[length : length + len(data)] = data
-                    n -= len(data)
-                else:
-                    view[length : length + n] = data[0:n]
-                    self._read_buffer = BytesIO(data[n:])
-                    n = 0
-            return view
-        except WebSocketTimeoutException:
-            raise TimeoutError()
+    def close(self):
+        with self.socket_lock:
+            if self.ws:
+                self._shutdown_transport()
+                self.ws = None
 
     def _shutdown_transport(self):
         # TODO Sync and Async close functions named differently
         """Do any preliminary work in shutting down the connection."""
-        self.ws.close()
+        if self.ws:
+            self.ws.close()
 
     def _write(self, s):
         """Completely write a string to the peer.
         ABNF, OPCODE_BINARY = 0x2
         See http://tools.ietf.org/html/rfc5234
         http://tools.ietf.org/html/rfc6455#section-5.2
         """
-        self.ws.send_binary(s)
+        from websocket import WebSocketConnectionClosedException, WebSocketTimeoutException
+        try:
+            self.ws.send_binary(s)
+        except AttributeError:
+            raise IOError("Websocket connection has already been closed.")
+        except WebSocketTimeoutException as e:
+            raise socket.timeout('Websocket send timed out (%s)' % e)
+        except (WebSocketConnectionClosedException, SSLError) as e:
+            raise ConnectionError('Websocket disconnected: %r' % e)
+
```

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/management_operation.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/management_operation.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,19 @@
 
 class ManagementOperation(object):
     def __init__(self, session, endpoint='$management', **kwargs):
         self._mgmt_link_open_status = None
 
         self._session = session
         self._connection = self._session._connection
+        self._network_trace_params = {
+            "amqpConnection": self._session._connection._container_id,
+            "amqpSession": self._session.name,
+            "amqpLink": None
+        }
         self._mgmt_link = self._session.create_request_response_link_pair(
             endpoint=endpoint,
             on_amqp_management_open_complete=self._on_amqp_management_open_complete,
             on_amqp_management_error=self._on_amqp_management_error,
             **kwargs
         )  # type: ManagementLink
         self._responses = {}
@@ -57,30 +62,30 @@
         operation_result,
         status_code,
         status_description,
         raw_message,
         error=None
     ):
         _LOGGER.debug(
-            "mgmt operation completed, operation id: %r; operation_result: %r; status_code: %r; "
-            "status_description: %r, raw_message: %r, error: %r",
+            "Management operation completed, id: %r; result: %r; code: %r; description: %r, error: %r",
             operation_id,
             operation_result,
             status_code,
             status_description,
-            raw_message,
-            error
+            error,
+            extra=self._network_trace_params
         )
 
         if operation_result in\
                 (ManagementExecuteOperationResult.ERROR, ManagementExecuteOperationResult.LINK_CLOSED):
             self._mgmt_error = error
             _LOGGER.error(
-                "Failed to complete mgmt operation due to error: %r. The management request message is: %r",
-                error, raw_message
+                "Failed to complete management operation due to error: %r.",
+                error,
+                extra=self._network_trace_params
             )
         else:
             self._responses[operation_id] = (status_code, status_description, raw_message)
 
     def execute(self, message, operation=None, operation_type=None, timeout=0):
         start_time = time.time()
         operation_id = str(uuid.uuid4())
```

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/_platform.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/_platform.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/endpoints.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/endpoints.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/_connection.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/_connection.py`

 * *Files 7% similar despite different names*

```diff
@@ -100,31 +100,40 @@
         # Custom Endpoint
         custom_endpoint_address = kwargs.get("custom_endpoint_address")
         custom_endpoint = None
         if custom_endpoint_address:
             custom_parsed_url = urlparse(custom_endpoint_address)
             custom_port = custom_parsed_url.port or WEBSOCKET_PORT
             custom_endpoint = f"{custom_parsed_url.hostname}:{custom_port}{custom_parsed_url.path}"
+        self._container_id = kwargs.pop("container_id", None) or str(uuid.uuid4())  # type: str
+        self._network_trace = kwargs.get("network_trace", False)
+        self._network_trace_params = {"amqpConnection": self._container_id, "amqpSession": None, "amqpLink": None}
 
         transport = kwargs.get("transport")
         self._transport_type = kwargs.pop("transport_type", TransportType.Amqp)
         if transport:
             self._transport = transport
         elif "sasl_credential" in kwargs:
             sasl_transport = SASLTransport
             if self._transport_type.name == "AmqpOverWebsocket" or kwargs.get("http_proxy"):
                 sasl_transport = SASLWithWebSocket
                 endpoint = parsed_url.hostname + parsed_url.path
             self._transport = sasl_transport(
-                host=endpoint, credential=kwargs["sasl_credential"], custom_endpoint=custom_endpoint, **kwargs
+                host=endpoint,
+                credential=kwargs["sasl_credential"],
+                custom_endpoint=custom_endpoint,
+                network_trace_params=self._network_trace_params,
+                **kwargs
             )
         else:
-            self._transport = Transport(parsed_url.netloc, transport_type=self._transport_type, **kwargs)
-
-        self._container_id = kwargs.pop("container_id", None) or str(uuid.uuid4())  # type: str
+            self._transport = Transport(
+                parsed_url.netloc,
+                transport_type=self._transport_type,
+                network_trace_params=self._network_trace_params,
+                **kwargs)
         self._max_frame_size = kwargs.pop("max_frame_size", MAX_FRAME_SIZE_BYTES)  # type: int
         self._remote_max_frame_size = None  # type: Optional[int]
         self._channel_max = kwargs.pop("channel_max", MAX_CHANNELS)  # type: int
         self._idle_timeout = kwargs.pop("idle_timeout", None)  # type: Optional[int]
         self._outgoing_locales = kwargs.pop("outgoing_locales", None)  # type: Optional[List[str]]
         self._incoming_locales = kwargs.pop("incoming_locales", None)  # type: Optional[List[str]]
         self._offered_capabilities = None  # type: Optional[str]
@@ -134,16 +143,14 @@
         self._allow_pipelined_open = kwargs.pop("allow_pipelined_open", True)  # type: bool
         self._remote_idle_timeout = None  # type: Optional[int]
         self._remote_idle_timeout_send_frame = None  # type: Optional[int]
         self._idle_timeout_empty_frame_send_ratio = kwargs.get("idle_timeout_empty_frame_send_ratio", 0.5)
         self._last_frame_received_time = None  # type: Optional[float]
         self._last_frame_sent_time = None  # type: Optional[float]
         self._idle_wait_time = kwargs.get("idle_wait_time", 0.1)  # type: float
-        self._network_trace = kwargs.get("network_trace", False)
-        self._network_trace_params = {"connection": self._container_id, "session": None, "link": None}
         self._error = None
         self._outgoing_endpoints = {}  # type: Dict[int, Session]
         self._incoming_endpoints = {}  # type: Dict[int, Session]
 
     def __enter__(self):
         self.open()
         return self
@@ -154,15 +161,20 @@
     def _set_state(self, new_state):
         # type: (ConnectionState) -> None
         """Update the connection state."""
         if new_state is None:
             return
         previous_state = self.state
         self.state = new_state
-        _LOGGER.info("Connection '%s' state changed: %r -> %r", self._container_id, previous_state, new_state)
+        _LOGGER.info(
+            "Connection state changed: %r -> %r",
+            previous_state,
+            new_state,
+            extra=self._network_trace_params
+        )
         for session in self._outgoing_endpoints.values():
             session._on_connection_state_change()  # pylint:disable=protected-access
 
     def _connect(self):
         # type: () -> None
         """Initiate the connection.
 
@@ -177,65 +189,66 @@
                 self._transport.connect()
                 self._set_state(ConnectionState.START)
             self._transport.negotiate()
             self._outgoing_header()
             self._set_state(ConnectionState.HDR_SENT)
             if not self._allow_pipelined_open:
                 # TODO: List/tuple expected as variable args
-                self._process_incoming_frame(*self._read_frame(wait=True))  # type: ignore
+                self._read_frame(wait=True)
                 if self.state != ConnectionState.HDR_EXCH:
                     self._disconnect()
                     raise ValueError("Did not receive reciprocal protocol header. Disconnecting.")
             else:
                 self._set_state(ConnectionState.HDR_SENT)
         except (OSError, IOError, SSLError, socket.error) as exc:
+            # FileNotFoundError is being raised for exception parity with uamqp when invalid
+            # `connection_verify` file path is passed in. Remove later when resolving issue #27128.
+            if isinstance(exc, FileNotFoundError) and exc.filename and "ca_certs" in exc.filename:
+                raise
             raise AMQPConnectionError(
                 ErrorCondition.SocketError,
                 description="Failed to initiate the connection due to exception: " + str(exc),
                 error=exc,
             )
-        except Exception:  # pylint:disable=try-except-raise
-            raise
 
     def _disconnect(self):
         # type: () -> None
         """Disconnect the transport and set state to END."""
         if self.state == ConnectionState.END:
             return
         self._set_state(ConnectionState.END)
         self._transport.close()
 
     def _can_read(self):
         # type: () -> bool
         """Whether the connection is in a state where it is legal to read for incoming frames."""
         return self.state not in (ConnectionState.CLOSE_RCVD, ConnectionState.END)
 
-    def _read_frame(  # type: ignore # TODO: missing return
+    def _read_frame(
         self, wait: Union[bool, float] = True, **kwargs: Any
-    ) -> Tuple[int, Optional[Tuple[int, NamedTuple]]]:
+    ) -> bool:
         """Read an incoming frame from the transport.
 
         :param Union[bool, float] wait: Whether to block on the socket while waiting for an incoming frame.
          The default value is `False`, where the frame will block for the configured timeout only (0.1 seconds).
          If set to `True`, socket will block indefinitely. If set to a timeout value in seconds, the socket will
          block for at most that value.
         :rtype: Tuple[int, Optional[Tuple[int, NamedTuple]]]
         :returns: A tuple with the incoming channel number, and the frame in the form or a tuple of performative
          descriptor and field values.
         """
-        if self._can_read():
-            if wait is False:
-                return self._transport.receive_frame(**kwargs)
-            if wait is True:
-                with self._transport.block():
-                    return self._transport.receive_frame(**kwargs)
-            else:
-                with self._transport.block_with_timeout(timeout=wait):
-                    return self._transport.receive_frame(**kwargs)
-        _LOGGER.warning("Cannot read frame in current state: %r", self.state)
+        if wait is False:
+            new_frame = self._transport.receive_frame(**kwargs)
+        elif wait is True:
+            with self._transport.block():
+                new_frame = self._transport.receive_frame(**kwargs)
+        else:
+            with self._transport.block_with_timeout(timeout=wait):
+                new_frame = self._transport.receive_frame(**kwargs)
+        return self._process_incoming_frame(*new_frame)
 
     def _can_write(self):
         # type: () -> bool
         """Whether the connection is in a state where it is legal to write outgoing frames."""
         return self.state not in _CLOSING_STATES
 
     def _send_frame(self, channel, frame, timeout=None, **kwargs):
@@ -265,15 +278,15 @@
                     ErrorCondition.SocketError,
                     description="Can not send frame out due to exception: " + str(exc),
                     error=exc,
                 )
             except Exception:  # pylint:disable=try-except-raise
                 raise
         else:
-            _LOGGER.warning("Cannot write frame in current state: %r", self.state)
+            _LOGGER.info("Cannot write frame in current state: %r", self.state, extra=self._network_trace_params)
 
     def _get_next_outgoing_channel(self):
         # type: () -> int
         """Get the next available outgoing channel number within the max channel limit.
 
         :raises ValueError: If maximum channels has been reached.
         :returns: The next available outgoing channel number.
@@ -284,15 +297,15 @@
         next_channel = next(i for i in range(1, self._channel_max) if i not in self._outgoing_endpoints)
         return next_channel
 
     def _outgoing_empty(self):
         # type: () -> None
         """Send an empty frame to prevent the connection from reaching an idle timeout."""
         if self._network_trace:
-            _LOGGER.info("-> empty()", extra=self._network_trace_params)
+            _LOGGER.debug("-> EmptyFrame()", extra=self._network_trace_params)
         try:
             raise self._error
         except TypeError:
             pass
         try:
             if self._can_write():
                 self._transport.write(EMPTY_FRAME)
@@ -307,22 +320,22 @@
             raise
 
     def _outgoing_header(self):
         # type: () -> None
         """Send the AMQP protocol header to initiate the connection."""
         self._last_frame_sent_time = time.time()
         if self._network_trace:
-            _LOGGER.info("-> header(%r)", HEADER_FRAME, extra=self._network_trace_params)
+            _LOGGER.debug("-> Header(%r)", HEADER_FRAME, extra=self._network_trace_params)
         self._transport.write(HEADER_FRAME)
 
     def _incoming_header(self, _, frame):
         # type: (int, bytes) -> None
         """Process an incoming AMQP protocol header and update the connection state."""
         if self._network_trace:
-            _LOGGER.info("<- header(%r)", frame, extra=self._network_trace_params)
+            _LOGGER.debug("<- Header(%r)", frame, extra=self._network_trace_params)
         if self.state == ConnectionState.START:
             self._set_state(ConnectionState.HDR_RCVD)
         elif self.state == ConnectionState.HDR_SENT:
             self._set_state(ConnectionState.HDR_EXCH)
         elif self.state == ConnectionState.OPEN_PIPE:
             self._set_state(ConnectionState.OPEN_SENT)
 
@@ -338,15 +351,15 @@
             outgoing_locales=self._outgoing_locales,
             incoming_locales=self._incoming_locales,
             offered_capabilities=self._offered_capabilities if self.state == ConnectionState.OPEN_RCVD else None,
             desired_capabilities=self._desired_capabilities if self.state == ConnectionState.HDR_EXCH else None,
             properties=self._properties,
         )
         if self._network_trace:
-            _LOGGER.info("-> %r", open_frame, extra=self._network_trace_params)
+            _LOGGER.debug("-> %r", open_frame, extra=self._network_trace_params)
         self._send_frame(0, open_frame)
 
     def _incoming_open(self, channel, frame):
         # type: (int, Tuple[Any, ...]) -> None
         """Process incoming Open frame to finish the connection negotiation.
 
         The incoming frame format is::
@@ -365,112 +378,112 @@
         :param int channel: The incoming channel number.
         :param frame: The incoming Open frame.
         :type frame: Tuple[Any, ...]
         :rtype: None
         """
         # TODO: Add type hints for full frame tuple contents.
         if self._network_trace:
-            _LOGGER.info("<- %r", OpenFrame(*frame), extra=self._network_trace_params)
+            _LOGGER.debug("<- %r", OpenFrame(*frame), extra=self._network_trace_params)
         if channel != 0:
-            _LOGGER.error("OPEN frame received on a channel that is not 0.")
+            _LOGGER.error("OPEN frame received on a channel that is not 0.", extra=self._network_trace_params)
             self.close(
                 error=AMQPError(
                     condition=ErrorCondition.NotAllowed, description="OPEN frame received on a channel that is not 0."
                 )
             )
             self._set_state(ConnectionState.END)
         if self.state == ConnectionState.OPENED:
-            _LOGGER.error("OPEN frame received in the OPENED state.")
+            _LOGGER.error("OPEN frame received in the OPENED state.", extra=self._network_trace_params)
             self.close()
         if frame[4]:
             self._remote_idle_timeout = frame[4] / 1000  # Convert to seconds
             self._remote_idle_timeout_send_frame = (
                 self._idle_timeout_empty_frame_send_ratio * self._remote_idle_timeout
             )
 
         if frame[2] < 512:
             # Max frame size is less than supported minimum.
             # If any of the values in the received open frame are invalid then the connection shall be closed.
             # The error amqp:invalid-field shall be set in the error.condition field of the CLOSE frame.
             self.close(
-                error=cast(
-                    AMQPError,
-                    AMQPConnectionError(
-                        condition=ErrorCondition.InvalidField,
-                        description="Failed parsing OPEN frame: Max frame size is less than supported minimum.",
-                    ),
+                error=AMQPError(
+                    condition=ErrorCondition.InvalidField,
+                    description="Failed parsing OPEN frame: Max frame size is less than supported minimum.",
                 )
             )
             _LOGGER.error(
-                "Failed parsing OPEN frame: Max frame size is less than supported minimum."
+                "Failed parsing OPEN frame: Max frame size is less than supported minimum.",
+                extra=self._network_trace_params
             )
-        else:
-            self._remote_max_frame_size = frame[2]
+            return
+        self._remote_max_frame_size = frame[2]
         if self.state == ConnectionState.OPEN_SENT:
             self._set_state(ConnectionState.OPENED)
         elif self.state == ConnectionState.HDR_EXCH:
             self._set_state(ConnectionState.OPEN_RCVD)
             self._outgoing_open()
             self._set_state(ConnectionState.OPENED)
         else:
             self.close(
                 error=AMQPError(
                     condition=ErrorCondition.IllegalState,
                     description=f"connection is an illegal state: {self.state}",
                 )
             )
-            _LOGGER.error("connection is an illegal state: %r", self.state)
+            _LOGGER.error("Connection is an illegal state: %r", self.state, extra=self._network_trace_params)
 
     def _outgoing_close(self, error=None):
         # type: (Optional[AMQPError]) -> None
         """Send a Close frame to shutdown connection with optional error information."""
         close_frame = CloseFrame(error=error)
         if self._network_trace:
-            _LOGGER.info("-> %r", close_frame, extra=self._network_trace_params)
+            _LOGGER.debug("-> %r", close_frame, extra=self._network_trace_params)
         self._send_frame(0, close_frame)
 
     def _incoming_close(self, channel, frame):
         # type: (int, Tuple[Any, ...]) -> None
         """Process incoming Open frame to finish the connection negotiation.
 
         The incoming frame format is::
 
             - frame[0]: error (Optional[AMQPError])
 
         """
         if self._network_trace:
-            _LOGGER.info("<- %r", CloseFrame(*frame), extra=self._network_trace_params)
+            _LOGGER.debug("<- %r", CloseFrame(*frame), extra=self._network_trace_params)
         disconnect_states = [
             ConnectionState.HDR_RCVD,
             ConnectionState.HDR_EXCH,
             ConnectionState.OPEN_RCVD,
             ConnectionState.CLOSE_SENT,
             ConnectionState.DISCARDING,
         ]
         if self.state in disconnect_states:
             self._disconnect()
-            self._set_state(ConnectionState.END)
             return
 
         close_error = None
         if channel > self._channel_max:
-            _LOGGER.error("Invalid channel")
+            _LOGGER.error(
+                "CLOSE frame received on a channel greated than support max.",
+                extra=self._network_trace_params
+            )
             close_error = AMQPError(condition=ErrorCondition.InvalidField, description="Invalid channel", info=None)
 
         self._set_state(ConnectionState.CLOSE_RCVD)
         self._outgoing_close(error=close_error)
         self._disconnect()
-        self._set_state(ConnectionState.END)
 
         if frame[0]:
             self._error = AMQPConnectionError(
                 condition=frame[0][0], description=frame[0][1], info=frame[0][2]
             )
             _LOGGER.error(
-                "Connection error: %r", frame[0]
+                "Connection closed with error: %r", frame[0],
+                extra=self._network_trace_params
             )
 
 
     def _incoming_begin(self, channel, frame):
         # type: (int, Tuple[Any, ...]) -> None
         """Process incoming Begin frame to finish negotiating a new session.
 
@@ -521,14 +534,18 @@
         except KeyError:
             #close the connection
             self.close(
                 error=AMQPError(
                     condition=ErrorCondition.ConnectionCloseForced,
                     description="Invalid channel number received"
                 ))
+            _LOGGER.error(
+                "END frame received on invalid channel. Closing connection.",
+                extra=self._network_trace_params
+            )
             return
 
     def _process_incoming_frame(self, channel, frame):  # pylint:disable=too-many-return-statements
         # type: (int, Optional[Union[bytes, Tuple[int, Tuple[Any, ...]]]]) -> bool
         """Process an incoming frame, either directly or by passing to the necessary Session.
 
         :param int channel: The channel the frame arrived on.
@@ -585,15 +602,15 @@
                 self._incoming_close(channel, fields)
                 return True
             if performative == 0:
                 self._incoming_header(channel, cast(bytes, fields))
                 return True
             if performative == 1:
                 return False
-            _LOGGER.error("Unrecognized incoming frame: %s", frame)
+            _LOGGER.error("Unrecognized incoming frame: %r", frame, extra=self._network_trace_params)
             return True
         except KeyError:
             return True  # TODO: channel error
 
     def _process_outgoing_frame(self, channel, frame):
         # type: (int, NamedTuple) -> None
         """Send an outgoing frame if the connection is in a legal state.
@@ -613,14 +630,18 @@
             raise ValueError("Connection not open.")
         now = time.time()
         if get_local_timeout(
             now,
             cast(float, self._idle_timeout),
             cast(float, self._last_frame_received_time),
         ) or self._get_remote_timeout(now):
+            _LOGGER.info(
+                "No frame received for the idle timeout. Closing connection.",
+                extra=self._network_trace_params
+            )
             self.close(
                 error=AMQPError(
                     condition=ErrorCondition.ConnectionCloseForced,
                     description="No frame received for the idle timeout.",
                 ),
                 wait=False,
             )
@@ -693,35 +714,46 @@
                 if get_local_timeout(
                     now,
                     cast(float, self._idle_timeout),
                     cast(float, self._last_frame_received_time),
                 ) or self._get_remote_timeout(
                     now
                 ):
+                    _LOGGER.info(
+                        "No frame received for the idle timeout. Closing connection.",
+                        extra=self._network_trace_params
+                    )
                     self.close(
                         error=AMQPError(
                             condition=ErrorCondition.ConnectionCloseForced,
                             description="No frame received for the idle timeout.",
                         ),
                         wait=False,
                     )
                     return
             if self.state == ConnectionState.END:
                 self._error = AMQPConnectionError(
                     condition=ErrorCondition.ConnectionCloseForced, description="Connection was already closed."
                 )
                 return
             for _ in range(batch):
-                new_frame = self._read_frame(wait=wait, **kwargs)
-                if self._process_incoming_frame(*new_frame):
+                if self._can_read():
+                    if self._read_frame(wait=wait, **kwargs):
+                        break
+                else:
+                    _LOGGER.info(
+                        "Connection cannot read frames in this state: %r",
+                        self.state,
+                        extra=self._network_trace_params
+                    )
                     break
         except (OSError, IOError, SSLError, socket.error) as exc:
             self._error = AMQPConnectionError(
                 ErrorCondition.SocketError,
-                description="Can not send frame out due to exception: " + str(exc),
+                description="Can not read frame due to exception: " + str(exc),
                 error=exc,
             )
         except Exception:  # pylint:disable=try-except-raise
             raise
 
     def create_session(self, **kwargs):
         # type: (Any) -> Session
@@ -787,21 +819,21 @@
 
         Alternatively this method will be called on exiting a Connection context manager.
 
         :param ~uamqp.AMQPError error: Optional error information to include in the close request.
         :param bool wait: Whether to wait for a service Close response. Default is `False`.
         :rtype: None
         """
-        if self.state in [
-            ConnectionState.END,
-            ConnectionState.CLOSE_SENT,
-            ConnectionState.DISCARDING,
-        ]:
-            return
         try:
+            if self.state in [
+                ConnectionState.END,
+                ConnectionState.CLOSE_SENT,
+                ConnectionState.DISCARDING,
+            ]:
+                return
             self._outgoing_close(error=error)
             if error:
                 self._error = AMQPConnectionError(
                     condition=error.condition,
                     description=error.description,
                     info=error.info,
                 )
@@ -812,11 +844,11 @@
             elif error:
                 self._set_state(ConnectionState.DISCARDING)
             else:
                 self._set_state(ConnectionState.CLOSE_SENT)
             self._wait_for_response(wait, ConnectionState.END)
         except Exception as exc:  # pylint:disable=broad-except
             # If error happened during closing, ignore the error and set state to END
-            _LOGGER.info("An error occurred when closing the connection: %r", exc)
+            _LOGGER.info("An error occurred when closing the connection: %r", exc, extra=self._network_trace_params)
             self._set_state(ConnectionState.END)
         finally:
             self._disconnect()
```

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/utils.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 #--------------------------------------------------------------------------
 import datetime
 from base64 import b64encode
 from hashlib import sha256
 from hmac import HMAC
 from urllib.parse import urlencode, quote_plus
 import time
-import six
 
 from .types import TYPE, VALUE, AMQPTypes
 from ._encode import encode_payload
 
 
 class UTC(datetime.tzinfo):
     """Time Zone info for handling UTC"""
@@ -44,15 +43,15 @@
 
 
 def utc_now():
     return datetime.datetime.now(tz=TZ_UTC)
 
 
 def encode(value, encoding='UTF-8'):
-    return value.encode(encoding) if isinstance(value, six.text_type) else value
+    return value.encode(encoding) if isinstance(value, str) else value
 
 
 def generate_sas_token(audience, policy, key, expiry=None):
     """
     Generate a sas token according to the given audience, policy, key and expiry
 
     :param str audience:
```

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/session.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/session.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         self.offered_capabilities = None
         self.desired_capabilities = kwargs.pop("desired_capabilities", None)
 
         self.allow_pipelined_open = kwargs.pop("allow_pipelined_open", True)
         self.idle_wait_time = kwargs.get("idle_wait_time", 0.1)
         self.network_trace = kwargs["network_trace"]
         self.network_trace_params = kwargs["network_trace_params"]
-        self.network_trace_params["session"] = self.name
+        self.network_trace_params["amqpSession"] = self.name
 
         self.links = {}
         self._connection = connection
         self._output_handles = {}
         self._input_handles = {}
 
     def __enter__(self):
@@ -134,22 +134,22 @@
             else None,
             desired_capabilities=self.desired_capabilities
             if self.state == SessionState.UNMAPPED
             else None,
             properties=self.properties,
         )
         if self.network_trace:
-            _LOGGER.info("-> %r", begin_frame, extra=self.network_trace_params)
+            _LOGGER.debug("-> %r", begin_frame, extra=self.network_trace_params)
         self._connection._process_outgoing_frame(  # pylint: disable=protected-access
             self.channel, begin_frame
         )
 
     def _incoming_begin(self, frame):
         if self.network_trace:
-            _LOGGER.info("<- %r", BeginFrame(*frame), extra=self.network_trace_params)
+            _LOGGER.debug("<- %r", BeginFrame(*frame), extra=self.network_trace_params)
         self.handle_max = frame[4]  # handle_max
         self.next_incoming_id = frame[1]  # next_outgoing_id
         self.remote_incoming_window = frame[2]  # incoming_window
         self.remote_outgoing_window = frame[3]  # outgoing_window
         if self.state == SessionState.BEGIN_SENT:
             self.remote_channel = frame[0]  # remote_channel
             self._set_state(SessionState.MAPPED)
@@ -157,22 +157,22 @@
             self._set_state(SessionState.BEGIN_RCVD)
             self._outgoing_begin()
             self._set_state(SessionState.MAPPED)
 
     def _outgoing_end(self, error=None):
         end_frame = EndFrame(error=error)
         if self.network_trace:
-            _LOGGER.info("-> %r", end_frame, extra=self.network_trace_params)
+            _LOGGER.debug("-> %r", end_frame, extra=self.network_trace_params)
         self._connection._process_outgoing_frame(  # pylint: disable=protected-access
             self.channel, end_frame
         )
 
     def _incoming_end(self, frame):
         if self.network_trace:
-            _LOGGER.info("<- %r", EndFrame(*frame), extra=self.network_trace_params)
+            _LOGGER.debug("<- %r", EndFrame(*frame), extra=self.network_trace_params)
         if self.state not in [
             SessionState.END_RCVD,
             SessionState.END_SENT,
             SessionState.DISCARDING,
         ]:
             self._set_state(SessionState.END_RCVD)
             for _, link in self.links.items():
@@ -194,14 +194,18 @@
             self._input_handles[frame[1]]._incoming_attach(  # pylint: disable=protected-access
                 frame
             )
         except KeyError:
             try:
                 outgoing_handle = self._get_next_output_handle()
             except ValueError:
+                _LOGGER.error(
+                    "Unable to attach new link - cannot allocate more handles.",
+                    extra=self.network_trace_params
+                )
                 # detach the link that would have been set.
                 self.links[frame[0].decode("utf-8")].detach(
                     error=AMQPError(
                         condition=ErrorCondition.LinkDetachForced,
                         description="""Cannot allocate more handles, """
                             """the max number of handles is {}. Detaching link""".format(
                             self.handle_max
@@ -216,38 +220,43 @@
                 )
             else:
                 new_link = SenderLink.from_incoming_frame(self, outgoing_handle, frame)
             new_link._incoming_attach(frame)  # pylint: disable=protected-access
             self.links[frame[0]] = new_link
             self._output_handles[outgoing_handle] = new_link
             self._input_handles[frame[1]] = new_link
-        except ValueError:
+        except ValueError as e:
             # Reject Link
+            _LOGGER.error(
+                    "Unable to attach new link: %r",
+                    e,
+                    extra=self.network_trace_params
+            )
             self._input_handles[frame[1]].detach()
 
     def _outgoing_flow(self, frame=None):
         link_flow = frame or {}
         link_flow.update(
             {
                 "next_incoming_id": self.next_incoming_id,
                 "incoming_window": self.incoming_window,
                 "next_outgoing_id": self.next_outgoing_id,
                 "outgoing_window": self.outgoing_window,
             }
         )
         flow_frame = FlowFrame(**link_flow)
         if self.network_trace:
-            _LOGGER.info("-> %r", flow_frame, extra=self.network_trace_params)
+            _LOGGER.debug("-> %r", flow_frame, extra=self.network_trace_params)
         self._connection._process_outgoing_frame(  # pylint: disable=protected-access
             self.channel, flow_frame
         )
 
     def _incoming_flow(self, frame):
         if self.network_trace:
-            _LOGGER.info("<- %r", FlowFrame(*frame), extra=self.network_trace_params)
+            _LOGGER.debug("<- %r", FlowFrame(*frame), extra=self.network_trace_params)
         self.next_incoming_id = frame[2]  # next_outgoing_id
         remote_incoming_id = (
             frame[0] or self.next_outgoing_id
         )  #  next_incoming_id  TODO "initial-outgoing-id"
         self.remote_incoming_window = (
             remote_incoming_id + frame[1] - self.next_outgoing_id
         )  # incoming_window
@@ -259,15 +268,15 @@
         else:
             for link in self._output_handles.values():
                 if (
                     self.remote_incoming_window > 0 and not link._is_closed  # pylint: disable=protected-access
                 ):
                     link._incoming_flow(frame)  # pylint: disable=protected-access
 
-    def _outgoing_transfer(self, delivery):
+    def _outgoing_transfer(self, delivery, network_trace_params):
         if self.state != SessionState.MAPPED:
             delivery.transfer_state = SessionTransferState.ERROR
         if self.remote_incoming_window <= 0:
             delivery.transfer_state = SessionTransferState.BUSY
         else:
             payload = delivery.frame["payload"]
             payload_size = len(payload)
@@ -296,19 +305,32 @@
                     "settled": delivery.frame["settled"],
                     "more": True,
                     "rcv_settle_mode": delivery.frame["rcv_settle_mode"],
                     "state": delivery.frame["state"],
                     "resume": delivery.frame["resume"],
                     "aborted": delivery.frame["aborted"],
                     "batchable": delivery.frame["batchable"],
-                    "payload": payload[start_idx : start_idx + available_frame_size],
                     "delivery_id": self.next_outgoing_id,
                 }
+                if network_trace_params:
+                    # We determine the logging for the outgoing Transfer frames based on the source
+                    # Link configuration rather than the Session, because it's only at the Session
+                    # level that we can determine how many outgoing frames are needed and their
+                    # delivery IDs.
+                    # TODO: Obscuring the payload for now to investigate the potential for leaks.
+                    _LOGGER.debug(
+                        "-> %r", TransferFrame(payload=b"***", **tmp_delivery_frame),
+                        extra=network_trace_params
+                    )
                 self._connection._process_outgoing_frame(  # pylint: disable=protected-access
-                    self.channel, TransferFrame(**tmp_delivery_frame)
+                    self.channel,
+                    TransferFrame(
+                        payload=payload[start_idx : start_idx + available_frame_size],
+                        **tmp_delivery_frame
+                    )
                 )
                 start_idx += available_frame_size
                 remaining_payload_cnt -= available_frame_size
 
             # encode the last frame
             tmp_delivery_frame = {
                 "handle": delivery.frame["handle"],
@@ -317,19 +339,29 @@
                 "settled": delivery.frame["settled"],
                 "more": False,
                 "rcv_settle_mode": delivery.frame["rcv_settle_mode"],
                 "state": delivery.frame["state"],
                 "resume": delivery.frame["resume"],
                 "aborted": delivery.frame["aborted"],
                 "batchable": delivery.frame["batchable"],
-                "payload": payload[start_idx:],
                 "delivery_id": self.next_outgoing_id,
             }
+            if network_trace_params:
+                # We determine the logging for the outgoing Transfer frames based on the source
+                # Link configuration rather than the Session, because it's only at the Session
+                # level that we can determine how many outgoing frames are needed and their
+                # delivery IDs.
+                # TODO: Obscuring the payload for now to investigate the potential for leaks.
+                _LOGGER.debug(
+                    "-> %r", TransferFrame(payload=b"***", **tmp_delivery_frame),
+                    extra=network_trace_params
+                )
             self._connection._process_outgoing_frame(  # pylint: disable=protected-access
-                self.channel, TransferFrame(**tmp_delivery_frame)
+                self.channel,
+                TransferFrame(payload=payload[start_idx:], **tmp_delivery_frame)
             )
             self.next_outgoing_id += 1
             self.remote_incoming_window -= 1
             self.outgoing_window -= 1
             # TODO: We should probably handle an error at the connection and update state accordingly
             delivery.transfer_state = SessionTransferState.OKAY
 
@@ -338,34 +370,39 @@
         self.remote_outgoing_window -= 1
         self.incoming_window -= 1
         try:
             self._input_handles[frame[0]]._incoming_transfer(  # pylint: disable=protected-access
                 frame
             )
         except KeyError:
+            _LOGGER.error(
+                "Received Transfer frame on unattached link. Ending session.",
+                extra=self.network_trace_params
+            )
             self._set_state(SessionState.DISCARDING)
             self.end(
                 error=AMQPError(
                     condition=ErrorCondition.SessionUnattachedHandle,
                     description="""Invalid handle reference in received frame: """
                         """Handle is not currently associated with an attached link""",
                 )
             )
+            return
         if self.incoming_window == 0:
             self.incoming_window = self.target_incoming_window
             self._outgoing_flow()
 
     def _outgoing_disposition(self, frame):
         self._connection._process_outgoing_frame(  # pylint: disable=protected-access
             self.channel, frame
         )
 
     def _incoming_disposition(self, frame):
         if self.network_trace:
-            _LOGGER.info(
+            _LOGGER.debug(
                 "<- %r", DispositionFrame(*frame), extra=self.network_trace_params
             )
         for link in self._input_handles.values():
             link._incoming_disposition(frame)  # pylint: disable=protected-access
 
     def _outgoing_detach(self, frame):
         self._connection._process_outgoing_frame(  # pylint: disable=protected-access
@@ -423,15 +460,15 @@
                 self._outgoing_end(error=error)
             for _, link in self.links.items():
                 link.detach()
             new_state = SessionState.DISCARDING if error else SessionState.END_SENT
             self._set_state(new_state)
             self._wait_for_response(wait, SessionState.UNMAPPED)
         except Exception as exc:  # pylint: disable=broad-except
-            _LOGGER.info("An error occurred when ending the session: %r", exc)
+            _LOGGER.info("An error occurred when ending the session: %r", exc, extra=self.network_trace_params)
             self._set_state(SessionState.UNMAPPED)
 
     def create_receiver_link(self, source_address, **kwargs):
         assigned_handle = self._get_next_output_handle()
         link = ReceiverLink(
             self,
             handle=assigned_handle,
@@ -459,9 +496,10 @@
         return link
 
     def create_request_response_link_pair(self, endpoint, **kwargs):
         return ManagementLink(
             self,
             endpoint,
             network_trace=kwargs.pop("network_trace", self.network_trace),
+            network_trace_params=dict(self.network_trace_params),
             **kwargs,
         )
```

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/_message_backcompat.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/_message_backcompat.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/sender.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/sender.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,14 @@
 import uuid
 import logging
 import time
 
 from ._encode import encode_payload
 from .link import Link
 from .constants import SessionTransferState, LinkDeliverySettleReason, LinkState, Role, SenderSettleMode, SessionState
-from .performatives import (
-    TransferFrame,
-)
 from .error import AMQPLinkError, ErrorCondition, MessageException
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class PendingDelivery(object):
     def __init__(self, **kwargs):
@@ -25,21 +22,26 @@
         self.sent = False
         self.frame = None
         self.on_delivery_settled = kwargs.get("on_delivery_settled")
         self.start = time.time()
         self.transfer_state = None
         self.timeout = kwargs.get("timeout")
         self.settled = kwargs.get("settled", False)
+        self._network_trace_params = kwargs.get('network_trace_params')
 
     def on_settled(self, reason, state):
         if self.on_delivery_settled and not self.settled:
             try:
                 self.on_delivery_settled(reason, state)
             except Exception as e:  # pylint:disable=broad-except
-                _LOGGER.warning("Message 'on_send_complete' callback failed: %r", e)
+                _LOGGER.warning(
+                    "Message 'on_send_complete' callback failed: %r",
+                    e,
+                    extra=self._network_trace_params
+                )
         self.settled = True
 
 
 class SenderLink(Link):
     def __init__(self, session, handle, target_address, **kwargs):
         name = kwargs.pop("name", None) or str(uuid.uuid4())
         role = Role.Sender
@@ -71,15 +73,18 @@
         self._remove_pending_deliveries()
 
     def _incoming_flow(self, frame):
         rcv_link_credit = frame[6]  # link_credit
         rcv_delivery_count = frame[5]  # delivery_count
         if frame[4] is not None:  # handle
             if rcv_link_credit is None or rcv_delivery_count is None:
-                _LOGGER.info("Unable to get link-credit or delivery-count from incoming ATTACH. Detaching link.")
+                _LOGGER.info(
+                    "Unable to get link-credit or delivery-count from incoming ATTACH. Detaching link.",
+                    extra=self.network_trace_params
+                )
                 self._remove_pending_deliveries()
                 self._set_state(LinkState.DETACHED)  # TODO: Send detach now?
             else:
                 self.current_link_credit = rcv_delivery_count + rcv_link_credit - self.delivery_count
         self.update_pending_deliveries()
 
     def _outgoing_transfer(self, delivery):
@@ -95,20 +100,18 @@
             "rcv_settle_mode": None,
             "state": None,
             "resume": None,
             "aborted": None,
             "batchable": None,
             "payload": output,
         }
-        if self.network_trace:
-            _LOGGER.info(
-                "-> %r", TransferFrame(delivery_id="<pending>", **delivery.frame), extra=self.network_trace_params
-            )
-            _LOGGER.info("   %r", delivery.message, extra=self.network_trace_params)
-        self._session._outgoing_transfer(delivery)  # pylint:disable=protected-access
+        self._session._outgoing_transfer(  # pylint:disable=protected-access
+            delivery,
+            self.network_trace_params if self.network_trace else None
+        )
         sent_and_settled = False
         if delivery.transfer_state == SessionTransferState.OKAY:
             self.delivery_count = delivery_count
             self.current_link_credit -= 1
             delivery.sent = True
             if delivery.settled:
                 delivery.on_settled(LinkDeliverySettleReason.SETTLED, None)
@@ -168,14 +171,15 @@
         if self.send_settle_mode == SenderSettleMode.Mixed:
             settled = kwargs.pop("settled", True)
         delivery = PendingDelivery(
             on_delivery_settled=kwargs.get("on_send_complete"),
             timeout=kwargs.get("timeout"),
             message=message,
             settled=settled,
+            network_trace_params = self.network_trace_params
         )
         if self.current_link_credit == 0 or send_async:
             self._pending_deliveries.append(delivery)
         else:
             sent_and_settled = self._outgoing_transfer(delivery)
             if not sent_and_settled:
                 self._pending_deliveries.append(delivery)
```

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/__init__.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/client.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 # pylint: disable=client-accepts-api-version-keyword
 # pylint: disable=missing-client-constructor-parameter-credential
 # pylint: disable=client-method-missing-type-annotations
 # pylint: disable=too-many-lines
 # TODO: Check types of kwargs (issue exists for this)
 import logging
+import threading
 import queue
 import time
 import uuid
 from functools import partial
 from typing import Any, Dict, Optional, Tuple, Union, overload, cast
 import certifi
 from typing_extensions import Literal
@@ -159,27 +160,29 @@
         self._session = None
         self._link = None
         self._socket_timeout = False
         self._external_connection = False
         self._cbs_authenticator = None
         self._auth_timeout = kwargs.pop("auth_timeout", DEFAULT_AUTH_TIMEOUT)
         self._mgmt_links = {}
+        self._mgmt_link_lock = threading.Lock()
         self._retry_policy = kwargs.pop("retry_policy", RetryPolicy())
-        self._keep_alive_interval = int(kwargs.get("keep_alive_interval") or 0)
+        self._keep_alive_interval = int(kwargs.get("keep_alive_interval", 0))
         self._keep_alive_thread = None
 
         # Connection settings
         self._max_frame_size = kwargs.pop("max_frame_size", MAX_FRAME_SIZE_BYTES)
         self._channel_max = kwargs.pop("channel_max", MAX_CHANNELS)
         self._idle_timeout = kwargs.pop("idle_timeout", None)
         self._properties = kwargs.pop("properties", None)
         self._remote_idle_timeout_empty_frame_send_ratio = kwargs.pop(
             "remote_idle_timeout_empty_frame_send_ratio", None
         )
         self._network_trace = kwargs.pop("network_trace", False)
+        self._network_trace_params = {"amqpConnection": None, "amqpSession": None, "amqpLink": None}
 
         # Session settings
         self._outgoing_window = kwargs.pop("outgoing_window", OUTGOING_WINDOW)
         self._incoming_window = kwargs.pop("incoming_window", INCOMING_WINDOW)
         self._handle_max = kwargs.pop("handle_max", None)
 
         # Link settings
@@ -212,14 +215,28 @@
         self.open()
         return self
 
     def __exit__(self, *args):
         """Close and destroy Client on exiting a context manager."""
         self.close()
 
+    def _keep_alive(self):
+        start_time = time.time()
+        try:
+            while self._connection and not self._shutdown:
+                current_time = time.time()
+                elapsed_time = current_time - start_time
+                if elapsed_time >= self._keep_alive_interval:
+                    _logger.debug("Keeping %r connection alive.", self.__class__.__name__)
+                    self._connection.listen(wait=self._socket_timeout, batch=self._link.current_link_credit)
+                    start_time = current_time
+                time.sleep(1)
+        except Exception as e:  # pylint: disable=broad-except
+            _logger.debug("Connection keep-alive for %r failed: %r.", self.__class__.__name__, e)
+
     def _client_ready(self):  # pylint: disable=no-self-use
         """Determine whether the client is ready to start sending and/or
         receiving messages. To be ready, the connection must be open and
         authentication complete.
 
         :rtype: bool
         """
@@ -276,15 +293,14 @@
         :param connection: An existing Connection that may be shared between
          multiple clients.
         :type connection: ~pyamqp.Connection
         """
         # pylint: disable=protected-access
         if self._session:
             return  # already open.
-        _logger.debug("Opening client connection.")
         if connection:
             self._connection = connection
             self._external_connection = True
         elif not self._connection:
             self._connection = Connection(
                 "amqps://" + self._hostname,
                 sasl_credential=self._auth.sasl,
@@ -302,19 +318,25 @@
             self._connection.open()
         if not self._session:
             self._session = self._connection.create_session(
                 incoming_window=self._incoming_window,
                 outgoing_window=self._outgoing_window,
             )
             self._session.begin()
+        if self._keep_alive_interval:
+            self._keep_alive_thread = threading.Thread(target=self._keep_alive)
+            self._keep_alive_thread.daemon = True
+            self._keep_alive_thread.start()
         if self._auth.auth_type == AUTH_TYPE_CBS:
             self._cbs_authenticator = CBSAuthenticator(
                 session=self._session, auth=self._auth, auth_timeout=self._auth_timeout
             )
             self._cbs_authenticator.open()
+        self._network_trace_params["amqpConnection"] = self._connection._container_id
+        self._network_trace_params["amqpSession"] = self._session.name
         self._shutdown = False
 
     def close(self):
         """Close the client. This includes closing the Session
         and CBS authentication layer as well as the Connection.
         If the client was opened using an external Connection,
         this will be left intact.
@@ -333,14 +355,22 @@
             self._cbs_authenticator.close()
             self._cbs_authenticator = None
         self._session.end()
         self._session = None
         if not self._external_connection:
             self._connection.close()
             self._connection = None
+        if self._keep_alive_thread:
+            try:
+                self._keep_alive_thread.join()
+            except RuntimeError:  # Probably thread failed to start in .open()
+                logging.debug("Keep alive thread failed to join.", exc_info=True)
+            self._keep_alive_thread = None
+        self._network_trace_params["amqpConnection"] = None
+        self._network_trace_params["amqpSession"] = None
 
     def auth_complete(self):
         """Whether the authentication handshake is complete during
         connection initialization.
 
         :rtype: bool
         """
@@ -401,24 +431,24 @@
         # The method also takes "status_code_field" and "status_description_field"
         # keyword arguments as alternate names for the status code and description
         # in the response body. Those two keyword arguments are used in Azure services only.
         operation = kwargs.pop("operation", None)
         operation_type = kwargs.pop("operation_type", None)
         node = kwargs.pop("node", "$management")
         timeout = kwargs.pop("timeout", 0)
-        try:
-            mgmt_link = self._mgmt_links[node]
-        except KeyError:
-            mgmt_link = ManagementOperation(self._session, endpoint=node, **kwargs)
-            self._mgmt_links[node] = mgmt_link
-            mgmt_link.open()
-
-            while not mgmt_link.ready():
-                self._connection.listen(wait=False)
+        with self._mgmt_link_lock:
+            try:
+                mgmt_link = self._mgmt_links[node]
+            except KeyError:
+                mgmt_link = ManagementOperation(self._session, endpoint=node, **kwargs)
+                self._mgmt_links[node] = mgmt_link
+                mgmt_link.open()
 
+        while not mgmt_link.ready():
+            self._connection.listen(wait=False)
         operation_type = operation_type or b"empty"
         status, description, response = mgmt_link.execute(
             message, operation=operation, operation_type=operation_type, timeout=timeout
         )
         return status, description, response
 
 
@@ -551,21 +581,16 @@
         """MessageSender Link is now open - perform message send
         on all pending messages.
         Will return True if operation successful and client can remain open for
         further work.
 
         :rtype: bool
         """
-        try:
-            self._link.update_pending_deliveries()
-            self._connection.listen(wait=self._socket_timeout, **kwargs)
-        except ValueError:
-            _logger.info("Timeout reached, closing sender.")
-            self._shutdown = True
-            return False
+        self._link.update_pending_deliveries()
+        self._connection.listen(wait=self._socket_timeout, **kwargs)
         return True
 
     def _transfer_message(self, message_delivery, timeout=0):
         message_delivery.state = MessageDeliveryState.WaitingForSendAck
         on_send_complete = partial(self._on_send_complete, message_delivery)
         delivery = self._link.send_transfer(
             message_delivery.message,
@@ -627,14 +652,20 @@
         while not self.client_ready():
             time.sleep(0.05)
 
         self._transfer_message(message_delivery, timeout)
         running = True
         while running and message_delivery.state not in MESSAGE_DELIVERY_DONE_STATES:
             running = self.do_work()
+        if message_delivery.state not in MESSAGE_DELIVERY_DONE_STATES:
+            raise MessageException(
+                condition=ErrorCondition.ClientError,
+                description="Send failed - connection not running."
+            )
+
         if message_delivery.state in (
             MessageDeliveryState.Error,
             MessageDeliveryState.Cancelled,
             MessageDeliveryState.Timeout,
         ):
             try:
                 raise message_delivery.error  # pylint: disable=raising-bad-type
@@ -650,15 +681,15 @@
         :keyword float timeout: timeout in seconds. If set to
          0, the client will continue to wait until the message is sent or error happens. The
          default is 0.
         """
         self._do_retryable_operation(self._send_message_impl, message=message, **kwargs)
 
 
-class ReceiveClient(AMQPClient):
+class ReceiveClient(AMQPClient): # pylint:disable=too-many-instance-attributes
     """
     An AMQP client for receiving messages.
     :param source: The source AMQP service endpoint. This can either be the URI as
      a string or a ~pyamqp.endpoint.Source object.
     :type source: str, bytes or ~pyamqp.endpoint.Source
     :keyword auth: Authentication for the connection. This should be one of the following:
         - pyamqp.authentication.SASLAnonymous
@@ -753,14 +784,20 @@
         self._received_messages = queue.Queue()
         self._message_received_callback = kwargs.pop("message_received_callback", None)
 
         # Sender and Link settings
         self._max_message_size = kwargs.pop("max_message_size", MAX_FRAME_SIZE_BYTES)
         self._link_properties = kwargs.pop("link_properties", None)
         self._link_credit = kwargs.pop("link_credit", 300)
+
+        # Iterator
+        self._timeout = kwargs.pop("timeout", 0)
+        self._timeout_reached = False
+        self._last_activity_timestamp = time.time()
+
         super(ReceiveClient, self).__init__(hostname, **kwargs)
 
     def _client_ready(self):
         """Determine whether the client is ready to start receiving messages.
         To be ready, the connection must be open and authentication complete,
         The Session, Link and MessageReceiver must be open and in non-errored
         states.
@@ -790,31 +827,33 @@
         """MessageReceiver Link is now open - start receiving messages.
         Will return True if operation successful and client can remain open for
         further work.
 
         :rtype: bool
         """
         try:
-            self._link.flow()
+            if self._link.current_link_credit == 0:
+                self._link.flow()
             self._connection.listen(wait=self._socket_timeout, **kwargs)
         except ValueError:
-            _logger.info("Timeout reached, closing receiver.")
+            _logger.info("Timeout reached, closing receiver.", extra=self._network_trace_params)
             self._shutdown = True
             return False
         return True
 
     def _message_received(self, frame, message):
         """Callback run on receipt of every message. If there is
         a user-defined callback, this will be called.
         Additionally if the client is retrieving messages for a batch
         or iterator, the message will be added to an internal queue.
 
         :param message: Received message.
         :type message: ~pyamqp.message.Message
         """
+        self._last_activity_timestamp = time.time()
         if self._message_received_callback:
             self._message_received_callback(message)
         if not self._streaming_receive:
             self._received_messages.put((frame, message))
 
     def _receive_message_batch_impl(
         self, max_batch_size=None, on_message_received=None, timeout=0
@@ -823,15 +862,15 @@
         max_batch_size = max_batch_size or self._link_credit
         timeout = time.time() + timeout if timeout else 0
         receiving = True
         batch = []
         self.open()
         while len(batch) < max_batch_size:
             try:
-                # TODO: This looses the transfer frame data
+                # TODO: This drops the transfer frame data
                 _, message = self._received_messages.get_nowait()
                 batch.append(message)
                 self._received_messages.task_done()
             except queue.Empty:
                 break
         else:
             return batch
@@ -886,14 +925,56 @@
          If no messages are received in this time, an empty list will be returned. If set to
          0, the client will continue to wait until at least one message is received. The
          default is 0.
         :type timeout: float
         """
         return self._do_retryable_operation(self._receive_message_batch_impl, **kwargs)
 
+    def receive_messages_iter(self, timeout=None, on_message_received=None):
+        """Receive messages by generator. Messages returned in the generator have already been
+        accepted - if you wish to add logic to accept or reject messages based on custom
+        criteria, pass in a callback.
+
+        :param on_message_received: A callback to process messages as they arrive from the
+         service. It takes a single argument, a ~pyamqp.message.Message object.
+        :type on_message_received: callable[~pyamqp.message.Message]
+        """
+        self._message_received_callback = on_message_received
+        return self._message_generator(timeout=timeout)
+
+    def _message_generator(self, timeout=None):
+        """Iterate over processed messages in the receive queue.
+
+        :rtype: generator[~pyamqp.message.Message]
+        """
+        self.open()
+        self._timeout_reached = False
+        receiving = True
+        message = None
+        self._last_activity_timestamp = time.time()
+        self._timeout = timeout if timeout else self._timeout
+        try:
+            while receiving and not self._timeout_reached:
+                if self._timeout > 0:
+                    if time.time() - self._last_activity_timestamp >= self._timeout:
+                        self._timeout_reached = True
+
+                if not self._timeout_reached:
+                    receiving = self.do_work()
+
+                while not self._received_messages.empty():
+                    message = self._received_messages.get()
+                    self._last_activity_timestamp = time.time()
+                    self._received_messages.task_done()
+                    yield message
+
+        finally:
+            if self._shutdown:
+                self.close()
+
     @overload
     def settle_messages(
         self,
         delivery_id: Union[int, Tuple[int, int]],
         outcome: Literal["accepted"],
         *,
         batchable: Optional[bool] = None
```

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/receiver.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_receiver_async.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,19 +4,22 @@
 # license information.
 # --------------------------------------------------------------------------
 
 import uuid
 import logging
 from typing import Optional, Union
 
-from ._decode import decode_payload
-from .link import Link
-from .constants import LinkState, Role
-from .performatives import TransferFrame, DispositionFrame
-from .outcomes import Received, Accepted, Rejected, Released, Modified
+from .._decode import decode_payload
+from ._link_async import Link
+from ..constants import LinkState, Role
+from ..performatives import (
+    TransferFrame,
+    DispositionFrame,
+)
+from ..outcomes import Received, Accepted, Rejected, Released, Modified
 
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class ReceiverLink(Link):
     def __init__(self, session, handle, source_address, **kwargs):
@@ -30,94 +33,92 @@
 
     @classmethod
     def from_incoming_frame(cls, session, handle, frame):
         # TODO: Assuming we establish all links for now...
         # check link_create_from_endpoint in C lib
         raise NotImplementedError("Pending")
 
-    def _process_incoming_message(self, frame, message):
+    async def _process_incoming_message(self, frame, message):
         try:
-            return self._on_transfer(frame, message)
+            return await self._on_transfer(frame, message)
         except Exception as e:  # pylint: disable=broad-except
-            _LOGGER.error("Handler function failed with error: %r", e)
+            _LOGGER.error("Transfer callback function failed with error: %r", e, extra=self.network_trace_params)
         return None
 
-    def _incoming_attach(self, frame):
-        super(ReceiverLink, self)._incoming_attach(frame)
+    async def _incoming_attach(self, frame):
+        await super(ReceiverLink, self)._incoming_attach(frame)
         if frame[9] is None:  # initial_delivery_count
-            _LOGGER.info("Cannot get initial-delivery-count. Detaching link")
-            self._set_state(LinkState.DETACHED)  # TODO: Send detach now?
+            _LOGGER.info("Cannot get initial-delivery-count. Detaching link", extra=self.network_trace_params)
+            await self._set_state(LinkState.DETACHED)  # TODO: Send detach now?
         self.delivery_count = frame[9]
         self.current_link_credit = self.link_credit
-        self._outgoing_flow()
+        await self._outgoing_flow()
 
-    def _incoming_transfer(self, frame):
+    async def _incoming_transfer(self, frame):
         if self.network_trace:
-            _LOGGER.info("<- %r", TransferFrame(*frame), extra=self.network_trace_params)
+            _LOGGER.debug("<- %r", TransferFrame(payload=b"***", *frame[:-1]), extra=self.network_trace_params)
         self.current_link_credit -= 1
         self.delivery_count += 1
         self.received_delivery_id = frame[1]  # delivery_id
         if not self.received_delivery_id and not self._received_payload:
             pass  # TODO: delivery error
         if self._received_payload or frame[5]:  # more
             self._received_payload.extend(frame[11])
         if not frame[5]:
             if self._received_payload:
                 message = decode_payload(memoryview(self._received_payload))
                 self._received_payload = bytearray()
             else:
                 message = decode_payload(frame[11])
-                if self.network_trace:
-                    _LOGGER.info("   %r", message, extra=self.network_trace_params)
-            delivery_state = self._process_incoming_message(frame, message)
+            delivery_state = await self._process_incoming_message(frame, message)
             if not frame[4] and delivery_state:  # settled
-                self._outgoing_disposition(
+                await self._outgoing_disposition(
                     first=frame[1],
                     last=frame[1],
                     settled=True,
                     state=delivery_state,
                     batchable=None
                 )
 
-    def _wait_for_response(self, wait: Union[bool, float]) -> None:
+    async def _wait_for_response(self, wait: Union[bool, float]) -> None:
         if wait is True:
-            self._session._connection.listen(wait=False) # pylint: disable=protected-access
+            await self._session._connection.listen(wait=False) # pylint: disable=protected-access
             if self.state == LinkState.ERROR:
                 raise self._error
         elif wait:
-            self._session._connection.listen(wait=wait) # pylint: disable=protected-access
+            await self._session._connection.listen(wait=wait) # pylint: disable=protected-access
             if self.state == LinkState.ERROR:
                 raise self._error
 
-    def _outgoing_disposition(
+    async def _outgoing_disposition(
         self,
         first: int,
         last: Optional[int],
         settled: Optional[bool],
         state: Optional[Union[Received, Accepted, Rejected, Released, Modified]],
         batchable: Optional[bool],
     ):
         disposition_frame = DispositionFrame(
             role=self.role, first=first, last=last, settled=settled, state=state, batchable=batchable
         )
         if self.network_trace:
-            _LOGGER.info("-> %r", DispositionFrame(*disposition_frame), extra=self.network_trace_params)
-        self._session._outgoing_disposition(disposition_frame) # pylint: disable=protected-access
+            _LOGGER.debug("-> %r", DispositionFrame(*disposition_frame), extra=self.network_trace_params)
+        await self._session._outgoing_disposition(disposition_frame) # pylint: disable=protected-access
 
-    def attach(self):
-        super().attach()
+    async def attach(self):
+        await super().attach()
         self._received_payload = bytearray()
 
-    def send_disposition(
+    async def send_disposition(
         self,
         *,
         wait: Union[bool, float] = False,
         first_delivery_id: int,
         last_delivery_id: Optional[int] = None,
         settled: Optional[bool] = None,
         delivery_state: Optional[Union[Received, Accepted, Rejected, Released, Modified]] = None,
         batchable: Optional[bool] = None
     ):
         if self._is_closed:
             raise ValueError("Link already closed.")
-        self._outgoing_disposition(first_delivery_id, last_delivery_id, settled, delivery_state, batchable)
-        self._wait_for_response(wait)
+        await self._outgoing_disposition(first_delivery_id, last_delivery_id, settled, delivery_state, batchable)
+        await self._wait_for_response(wait)
```

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/management_link.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/management_link.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,28 +35,31 @@
        # TODO: Fill in docstring
     """
     def __init__(self, session, endpoint, **kwargs):
         self.next_message_id = 0
         self.state = ManagementLinkState.IDLE
         self._pending_operations = []
         self._session = session
+        self._network_trace_params = kwargs.get('network_trace_params')
         self._request_link: SenderLink = session.create_sender_link(
             endpoint,
             source_address=endpoint,
             on_link_state_change=self._on_sender_state_change,
             send_settle_mode=SenderSettleMode.Unsettled,
-            rcv_settle_mode=ReceiverSettleMode.First
+            rcv_settle_mode=ReceiverSettleMode.First,
+            network_trace=kwargs.get("network_trace", False)
         )
         self._response_link: ReceiverLink = session.create_receiver_link(
             endpoint,
             target_address=endpoint,
             on_link_state_change=self._on_receiver_state_change,
             on_transfer=self._on_message_received,
             send_settle_mode=SenderSettleMode.Unsettled,
-            rcv_settle_mode=ReceiverSettleMode.First
+            rcv_settle_mode=ReceiverSettleMode.First,
+            network_trace=kwargs.get("network_trace", False)
         )
         self._on_amqp_management_error = kwargs.get('on_amqp_management_error')
         self._on_amqp_management_open_complete = kwargs.get('on_amqp_management_open_complete')
 
         self._status_code_field = kwargs.get('status_code_field', b'statusCode')
         self._status_description_field = kwargs.get('status_description_field', b'statusDescription')
 
@@ -67,15 +70,20 @@
         self.open()
         return self
 
     def __exit__(self, *args):
         self.close()
 
     def _on_sender_state_change(self, previous_state, new_state):
-        _LOGGER.info("Management link sender state changed: %r -> %r", previous_state, new_state)
+        _LOGGER.info(
+            "Management link sender state changed: %r -> %r",
+            previous_state,
+            new_state,
+            extra=self._network_trace_params
+        )
         if new_state == previous_state:
             return
         if self.state == ManagementLinkState.OPENING:
             if new_state == LinkState.ATTACHED:
                 self._sender_connected = True
                 if self._receiver_connected:
                     self.state = ManagementLinkState.OPEN
@@ -92,15 +100,20 @@
                 self.state = ManagementLinkState.ERROR
                 self._on_amqp_management_error()
         elif self.state == ManagementLinkState.ERROR:
             # All state transitions shall be ignored.
             return
 
     def _on_receiver_state_change(self, previous_state, new_state):
-        _LOGGER.info("Management link receiver state changed: %r -> %r", previous_state, new_state)
+        _LOGGER.info(
+            "Management link receiver state changed: %r -> %r",
+            previous_state,
+            new_state,
+            extra=self._network_trace_params
+        )
         if new_state == previous_state:
             return
         if self.state == ManagementLinkState.OPENING:
             if new_state == LinkState.ATTACHED:
                 self._receiver_connected = True
                 if self._sender_connected:
                     self.state = ManagementLinkState.OPEN
```

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/constants.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,19 @@
 
 SEND_DISPOSITION_ACCEPT = "accepted"
 SEND_DISPOSITION_REJECT = "rejected"
 
 AUTH_TYPE_SASL_PLAIN = "AUTH_SASL_PLAIN"
 AUTH_TYPE_CBS = "AUTH_CBS"
 
+DEFAULT_WEBSOCKET_HEARTBEAT_SECONDS = 10
+READ_TIMEOUT_INTERVAL = 0.2
+TIMEOUT_INTERVAL = 1
+WS_TIMEOUT_INTERVAL = 1
+
 
 class ConnectionState(Enum):
     #: In this state a Connection exists, but nothing has been sent or received. This is the state an
     #: implementation would be in immediately after performing a socket connect or socket accept.
     START = 0
     #: In this state the Connection header has been received from our peer, but we have not yet sent anything.
     HDR_RCVD = 1
```

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/link.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/link.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         self.available = kwargs.pop("available", None)
         self.properties = kwargs.pop("properties", None)
         self.offered_capabilities = None
         self.desired_capabilities = kwargs.pop("desired_capabilities", None)
 
         self.network_trace = kwargs["network_trace"]
         self.network_trace_params = kwargs["network_trace_params"]
-        self.network_trace_params["link"] = self.name
+        self.network_trace_params["amqpLink"] = self.name
         self._session = session
         self._is_closed = False
         self._on_link_state_change = kwargs.get("on_link_state_change")
         self._on_attach = kwargs.get("on_attach")
         self._error = None
 
     def __enter__(self):
@@ -153,24 +153,24 @@
             initial_delivery_count=self.initial_delivery_count if self.role == Role.Sender else None,
             max_message_size=self.max_message_size,
             offered_capabilities=self.offered_capabilities if self.state == LinkState.ATTACH_RCVD else None,
             desired_capabilities=self.desired_capabilities if self.state == LinkState.DETACHED else None,
             properties=self.properties,
         )
         if self.network_trace:
-            _LOGGER.info("-> %r", attach_frame, extra=self.network_trace_params)
+            _LOGGER.debug("-> %r", attach_frame, extra=self.network_trace_params)
         self._session._outgoing_attach(attach_frame) # pylint: disable=protected-access
 
     def _incoming_attach(self, frame):
         if self.network_trace:
-            _LOGGER.info("<- %r", AttachFrame(*frame), extra=self.network_trace_params)
+            _LOGGER.debug("<- %r", AttachFrame(*frame), extra=self.network_trace_params)
         if self._is_closed:
             raise ValueError("Invalid link")
         if not frame[5] or not frame[6]:
-            _LOGGER.info("Cannot get source or target. Detaching link")
+            _LOGGER.info("Cannot get source or target. Detaching link", extra=self.network_trace_params)
             self._set_state(LinkState.DETACHED)
             raise ValueError("Invalid link")
         self.remote_handle = frame[1]  # handle
         self.remote_max_message_size = frame[10]  # max_message_size
         self.offered_capabilities = frame[11]  # offered_capabilities
         if self.properties:
             self.properties.update(frame[13])  # properties
@@ -184,15 +184,15 @@
             try:
                 if frame[5]:
                     frame[5] = Source(*frame[5])
                 if frame[6]:
                     frame[6] = Target(*frame[6])
                 self._on_attach(AttachFrame(*frame))
             except Exception as e:  # pylint: disable=broad-except
-                _LOGGER.warning("Callback for link attach raised error: %r", e)
+                _LOGGER.warning("Callback for link attach raised error: %r", e, extra=self.network_trace_params)
 
     def _outgoing_flow(self, **kwargs):
         flow_frame = {
             "handle": self.handle,
             "delivery_count": self.delivery_count,
             "link_credit": self.current_link_credit,
             "available": kwargs.get("available"),
@@ -207,22 +207,22 @@
 
     def _incoming_disposition(self, frame):
         pass
 
     def _outgoing_detach(self, close=False, error=None):
         detach_frame = DetachFrame(handle=self.handle, closed=close, error=error)
         if self.network_trace:
-            _LOGGER.info("-> %r", detach_frame, extra=self.network_trace_params)
+            _LOGGER.debug("-> %r", detach_frame, extra=self.network_trace_params)
         self._session._outgoing_detach(detach_frame) # pylint: disable=protected-access
         if close:
             self._is_closed = True
 
     def _incoming_detach(self, frame):
         if self.network_trace:
-            _LOGGER.info("<- %r", DetachFrame(*frame), extra=self.network_trace_params)
+            _LOGGER.debug("<- %r", DetachFrame(*frame), extra=self.network_trace_params)
         if self.state == LinkState.ATTACHED:
             self._outgoing_detach(close=frame[1])  # closed
         elif frame[1] and not self._is_closed and self.state in [LinkState.ATTACH_SENT, LinkState.ATTACH_RCVD]:
             # Received a closing detach after we sent a non-closing detach.
             # In this case, we MUST signal that we closed by reattaching and then sending a closing detach.
             self._outgoing_attach()
             self._outgoing_detach(close=True)
@@ -249,13 +249,13 @@
             if self.state in [LinkState.ATTACH_SENT, LinkState.ATTACH_RCVD]:
                 self._outgoing_detach(close=close, error=error)
                 self._set_state(LinkState.DETACHED)
             elif self.state == LinkState.ATTACHED:
                 self._outgoing_detach(close=close, error=error)
                 self._set_state(LinkState.DETACH_SENT)
         except Exception as exc:  # pylint: disable=broad-except
-            _LOGGER.info("An error occurred when detaching the link: %r", exc)
+            _LOGGER.info("An error occurred when detaching the link: %r", exc, extra=self.network_trace_params)
             self._set_state(LinkState.DETACHED)
 
     def flow(self, *, link_credit: Optional[int] = None, **kwargs) -> None:
         self.current_link_credit = link_credit if link_credit is not None else self.link_credit
         self._outgoing_flow(**kwargs)
```

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/error.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/error.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/authentication.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
          tokens. It should return a valid jwt token each time it is called.
         :type get_token: callable object
         :param token_type: The type field of the token request.
          Default value is `"jwt"`.
         :type token_type: str
 
         """
-        super(JWTTokenAuth, self).__init__(uri, audience, kwargs.pop("kwargs", TOKEN_TYPE_JWT), get_token)
+        super(JWTTokenAuth, self).__init__(uri, audience, kwargs.pop("token_type", TOKEN_TYPE_JWT), get_token)
         self.get_token = get_token
 
 
 class SASTokenAuth(_CBSAuth):
     # TODO:
     #  1. naming decision, suffix with Auth vs Credential
     def __init__(
```

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/cbs.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/cbs.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # -------------------------------------------------------------------------
 
 import logging
 from datetime import datetime
+from typing import Optional
 
 from .utils import utc_now, utc_from_timestamp
 from .management_link import ManagementLink
 from .message import Message, Properties
 from .error import (
     AuthenticationException,
     ErrorCondition,
@@ -62,23 +63,27 @@
         self._auth = auth
         self._encoding = "UTF-8"
         self._auth_timeout = kwargs.get("auth_timeout")
         self._token_put_time = None
         self._expires_on = None
         self._token = None
         self._refresh_window = None
+        self._network_trace_params = {
+            "amqpConnection": self._session._connection._container_id,
+            "amqpSession": self._session.name,
+            "amqpLink": None
+        }
 
         self._token_status_code = None
         self._token_status_description = None
 
         self.state = CbsState.CLOSED
         self.auth_state = CbsAuthState.IDLE
 
-    def _put_token(self, token, token_type, audience, expires_on=None):
-        # type: (str, str, str, datetime) -> None
+    def _put_token(self, token: str, token_type: str, audience: str, expires_on: Optional[datetime] = None) -> None:
         message = Message(  # type: ignore  # TODO: missing positional args header, etc.
             value=token,
             properties=Properties(message_id=self._mgmt_link.next_message_id),  # type: ignore
             application_properties={
                 CBS_NAME: audience,
                 CBS_OPERATION: CBS_PUT_TOKEN,
                 CBS_TYPE: token_type,
@@ -95,67 +100,71 @@
         self._mgmt_link.next_message_id += 1
 
     def _on_amqp_management_open_complete(self, management_open_result):
         if self.state in (CbsState.CLOSED, CbsState.ERROR):
             _LOGGER.debug(
                 "CSB with status: %r encounters unexpected AMQP management open complete.",
                 self.state,
+                extra=self._network_trace_params
             )
         elif self.state == CbsState.OPEN:
             self.state = CbsState.ERROR
             _LOGGER.info(
-                "Unexpected AMQP management open complete in OPEN, CBS error occurred on connection %r.",
-                self._connection._container_id,  # pylint:disable=protected-access
+                "Unexpected AMQP management open complete in OPEN, CBS error occurred.",
+                extra=self._network_trace_params
             )
         elif self.state == CbsState.OPENING:
             self.state = (
                 CbsState.OPEN
                 if management_open_result == ManagementOpenResult.OK
                 else CbsState.CLOSED
             )
-            _LOGGER.info(
-                "CBS for connection %r completed opening with status: %r",
-                self._connection._container_id,  # pylint: disable=protected-access
+            _LOGGER.debug(
+                "CBS completed opening with status: %r",
                 management_open_result,
-            )  # pylint:disable=protected-access
+                extra=self._network_trace_params
+            )
 
     def _on_amqp_management_error(self):
         if self.state == CbsState.CLOSED:
-            _LOGGER.info("Unexpected AMQP error in CLOSED state.")
+            _LOGGER.info("Unexpected AMQP error in CLOSED state.", extra=self._network_trace_params)
         elif self.state == CbsState.OPENING:
             self.state = CbsState.ERROR
             self._mgmt_link.close()
             _LOGGER.info(
-                "CBS for connection %r failed to open with status: %r",
-                self._connection._container_id,
+                "CBS failed to open with status: %r",
                 ManagementOpenResult.ERROR,
-            )  # pylint:disable=protected-access
+                extra=self._network_trace_params
+            )
         elif self.state == CbsState.OPEN:
             self.state = CbsState.ERROR
-            _LOGGER.info(
-                "CBS error occurred on connection %r.", self._connection._container_id
-            )  # pylint:disable=protected-access
+            _LOGGER.info("CBS error occurred.", extra=self._network_trace_params)
 
     def _on_execute_operation_complete(
         self,
         execute_operation_result,
         status_code,
         status_description,
         _,
         error_condition=None,
     ):
         if error_condition:
-            _LOGGER.info("CBS Put token error: %r", error_condition)
+            _LOGGER.info(
+                "CBS Put token error: %r",
+                error_condition,
+                extra=self._network_trace_params
+            )
             self.auth_state = CbsAuthState.ERROR
             return
-        _LOGGER.info(
+        _LOGGER.debug(
             "CBS Put token result (%r), status code: %s, status_description: %s.",
             execute_operation_result,
             status_code,
             status_description,
+            extra=self._network_trace_params
         )
         self._token_status_code = status_code
         self._token_status_description = status_description
 
         if execute_operation_result == ManagementExecuteOperationResult.OK:
             self.auth_state = CbsAuthState.OK
         elif execute_operation_result == ManagementExecuteOperationResult.ERROR:
@@ -170,75 +179,88 @@
             self.auth_state = CbsAuthState.ERROR
 
     def _update_status(self):
         if (
             self.auth_state == CbsAuthState.OK
             or self.auth_state == CbsAuthState.REFRESH_REQUIRED
         ):
-            _LOGGER.debug("update_status In refresh required or OK.")
             is_expired, is_refresh_required = check_expiration_and_refresh_status(
                 self._expires_on, self._refresh_window
             )
             _LOGGER.debug(
-                "is expired == %r, is refresh required == %r",
+                "CBS status check: state == %r, expired == %r, refresh required == %r",
+                self.auth_state,
                 is_expired,
                 is_refresh_required,
+                extra=self._network_trace_params
             )
             if is_expired:
                 self.auth_state = CbsAuthState.EXPIRED
             elif is_refresh_required:
                 self.auth_state = CbsAuthState.REFRESH_REQUIRED
         elif self.auth_state == CbsAuthState.IN_PROGRESS:
             _LOGGER.debug(
-                "In update status, in progress. token put time: %r",
+                "CBS update in progress. Token put time: %r",
                 self._token_put_time,
+                extra=self._network_trace_params
             )
             put_timeout = check_put_timeout_status(
                 self._auth_timeout, self._token_put_time
             )
             if put_timeout:
                 self.auth_state = CbsAuthState.TIMEOUT
 
     def _cbs_link_ready(self):
         if self.state == CbsState.OPEN:
             return True
         if self.state != CbsState.OPEN:
             return False
         if self.state in (CbsState.CLOSED, CbsState.ERROR):
-            raise TokenAuthFailure( # pylint: disable = no-value-for-parameter
-                condition=ErrorCondition.ClientError,
-                description="CBS authentication link is in broken status, please recreate the cbs link.",
+            raise TokenAuthFailure(
+                status_code=ErrorCondition.ClientError,
+                status_description="CBS authentication link is in broken status, please recreate the cbs link.",
             )
 
     def open(self):
         self.state = CbsState.OPENING
         self._mgmt_link.open()
 
     def close(self):
         self._mgmt_link.close()
         self.state = CbsState.CLOSED
 
     def update_token(self):
         self.auth_state = CbsAuthState.IN_PROGRESS
         access_token = self._auth.get_token()
         if not access_token:
-            _LOGGER.debug("Update_token received an empty token object")
+            _LOGGER.info(
+                "Token refresh function received an empty token object.",
+                extra=self._network_trace_params
+            )
         elif not access_token.token:
-            _LOGGER.debug("Update_token received an empty token")
+            _LOGGER.info(
+                "Token refresh function received an empty token.",
+                extra=self._network_trace_params
+            )
         self._expires_on = access_token.expires_on
         expires_in = self._expires_on - int(utc_now().timestamp())
         self._refresh_window = int(float(expires_in) * 0.1)
         try:
             self._token = access_token.token.decode()
         except AttributeError:
             self._token = access_token.token
+        try:
+            token_type = self._auth.token_type.decode()
+        except AttributeError:
+            token_type = self._auth.token_type
+
         self._token_put_time = int(utc_now().timestamp())
         self._put_token(
             self._token,
-            self._auth.token_type,
+            token_type,
             self._auth.audience,
             utc_from_timestamp(self._expires_on),
         )
 
     def handle_token(self):
         if not self._cbs_link_ready():
             return False
@@ -248,17 +270,17 @@
             return False
         if self.auth_state == CbsAuthState.IN_PROGRESS:
             return False
         if self.auth_state == CbsAuthState.OK:
             return True
         if self.auth_state == CbsAuthState.REFRESH_REQUIRED:
             _LOGGER.info(
-                "Token on connection %r will expire soon - attempting to refresh.",
-                self._connection._container_id,
-            )  # pylint:disable=protected-access
+                "Token will expire soon - attempting to refresh.",
+                extra=self._network_trace_params
+            )
             self.update_token()
             return False
         if self.auth_state == CbsAuthState.FAILURE:
             raise AuthenticationException(
                 condition=ErrorCondition.InternalError,
                 description="Failed to open CBS authentication link.",
             )
```

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/_encode.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/_encode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
+# TODO: fix mypy errors for _code/_definition/__defaults__ (issue #26500)
 import calendar
 import struct
 import uuid
 from datetime import datetime
 from typing import (
     Iterable,
     Union,
@@ -25,15 +26,14 @@
 )
 
 try:
     from typing import TypeAlias  # type: ignore
 except ImportError:
     from typing_extensions import TypeAlias
 
-import six
 
 from .types import (
     TYPE,
     VALUE,
     AMQPTypes,
     FieldDefinition,
     ObjDefinition,
@@ -297,19 +297,19 @@
 def encode_uuid(
     output, value, with_constructor=True, **kwargs  # pylint: disable=unused-argument
 ):
     # type: (bytearray, Union[uuid.UUID, str, bytes], bool, Any) -> None
     """
     <encoding code="0x98" category="fixed" width="16" label="UUID as defined in section 4.1.2 of RFC-4122"/>
     """
-    if isinstance(value, six.text_type):
+    if isinstance(value, str):
         value = uuid.UUID(value).bytes
     elif isinstance(value, uuid.UUID):
         value = value.bytes
-    elif isinstance(value, six.binary_type):
+    elif isinstance(value, bytes):
         value = uuid.UUID(bytes=value).bytes
     else:
         raise TypeError("Invalid UUID type: {}".format(type(value)))
     output.extend(_construct(ConstructorBytes.uuid, with_constructor))
     output.extend(value)
 
 
@@ -337,15 +337,15 @@
     # type: (bytearray, Union[bytes, str], bool, bool) -> None
     """
     <encoding name="str8-utf8" code="0xa1" category="variable" width="1"
         label="up to 2^8 - 1 octets worth of UTF-8 Unicode (with no byte order mark)"/>
     <encoding name="str32-utf8" code="0xb1" category="variable" width="4"
         label="up to 2^32 - 1 octets worth of UTF-8 Unicode (with no byte order mark)"/>
     """
-    if isinstance(value, six.text_type):
+    if isinstance(value, str):
         value = value.encode("utf-8")
     length = len(value)
     if use_smallest and length <= 255:
         output.extend(_construct(ConstructorBytes.string_small, with_constructor))
         output.extend(struct.pack(">B", length))
         output.extend(value)
         return
@@ -361,15 +361,15 @@
     # type: (bytearray, Union[bytes, str], bool, bool) -> None
     """
     <encoding name="sym8" code="0xa3" category="variable" width="1"
         label="up to 2^8 - 1 seven bit ASCII characters representing a symbolic value"/>
     <encoding name="sym32" code="0xb3" category="variable" width="4"
         label="up to 2^32 - 1 seven bit ASCII characters representing a symbolic value"/>
     """
-    if isinstance(value, six.text_type):
+    if isinstance(value, str):
         value = value.encode("utf-8")
     length = len(value)
     if use_smallest and length <= 255:
         output.extend(_construct(ConstructorBytes.symbol_small, with_constructor))
         output.extend(struct.pack(">B", length))
         output.extend(value)
         return
@@ -581,17 +581,17 @@
     <type name="message-id-binary" class="restricted" source="binary" provides="message-id"/>
     <type name="message-id-string" class="restricted" source="string" provides="message-id"/>
     """
     if isinstance(value, int):
         return {TYPE: AMQPTypes.ulong, VALUE: value}
     if isinstance(value, uuid.UUID):
         return {TYPE: AMQPTypes.uuid, VALUE: value}
-    if isinstance(value, six.binary_type):
+    if isinstance(value, bytes):
         return {TYPE: AMQPTypes.binary, VALUE: value}
-    if isinstance(value, six.text_type):
+    if isinstance(value, str):
         return {TYPE: AMQPTypes.string, VALUE: value}
     raise TypeError("Unsupported Message ID type.")
 
 
 def encode_node_properties(value):
     # type: (Optional[Dict[str, Any]]) -> Dict[str, Any]
     """Properties of a node.
@@ -672,23 +672,23 @@
     """
     Dynamic encoding according to the type of `value`.
     """
     if value is None:
         encode_null(output, **kwargs)
     elif isinstance(value, bool):
         encode_boolean(output, value, **kwargs)
-    elif isinstance(value, six.string_types):
+    elif isinstance(value, str):
         encode_string(output, value, **kwargs)
     elif isinstance(value, uuid.UUID):
         encode_uuid(output, value, **kwargs)
-    elif isinstance(value, (bytearray, six.binary_type)):
+    elif isinstance(value, (bytearray, bytes)):
         encode_binary(output, value, **kwargs)
     elif isinstance(value, float):
         encode_double(output, value, **kwargs)
-    elif isinstance(value, six.integer_types):
+    elif isinstance(value, int):
         encode_int(output, value, **kwargs)
     elif isinstance(value, datetime):
         encode_timestamp(output, value, **kwargs)
     elif isinstance(value, list):
         encode_list(output, value, **kwargs)
     elif isinstance(value, tuple):
         encode_described(output, cast(Tuple[Any, Any], value), **kwargs)
@@ -741,15 +741,16 @@
         encode_unknown(output, value, **kwargs)
 
 
 def describe_performative(performative):
     # type: (Performative) -> Dict[str, Sequence[Collection[str]]]
     body: List[Dict[str, Any]] = []
     for index, value in enumerate(performative):
-        field = performative._definition[index]  # pylint: disable=protected-access
+        # TODO: fix mypy
+        field = performative._definition[index] # type: ignore  # pylint: disable=protected-access
         if value is None:
             body.append({TYPE: AMQPTypes.null, VALUE: None})
         elif field is None:
             continue
         elif isinstance(field.type, FieldDefinition):
             if field.multiple:
                 body.append(
@@ -772,15 +773,15 @@
                 )
             else:
                 body.append({TYPE: field.type, VALUE: value})
 
     return {
         TYPE: AMQPTypes.described,
         VALUE: (
-            {TYPE: AMQPTypes.ulong, VALUE: performative._code},  # pylint: disable=protected-access
+            {TYPE: AMQPTypes.ulong, VALUE: performative._code}, # type: ignore  # pylint: disable=protected-access
             {TYPE: AMQPTypes.list, VALUE: body},
         ),
     }
 
 
 def encode_payload(output, payload):
     # type: (bytearray, Message) -> bytes
```

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/message.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/message.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/performatives.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/performatives.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/outcomes.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/outcomes.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/sasl.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/sasl.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/_decode.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/_decode.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_authentication_async.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_authentication_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_sender_async.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_sender_async.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,14 @@
 import logging
 import time
 import asyncio
 
 from .._encode import encode_payload
 from ._link_async import Link
 from ..constants import SessionTransferState, LinkDeliverySettleReason, LinkState, Role, SenderSettleMode, SessionState
-from ..performatives import (
-    TransferFrame,
-)
 from ..error import AMQPLinkError, ErrorCondition, MessageException
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class PendingDelivery(object):
     def __init__(self, **kwargs):
@@ -26,21 +23,26 @@
         self.sent = False
         self.frame = None
         self.on_delivery_settled = kwargs.get("on_delivery_settled")
         self.start = time.time()
         self.transfer_state = None
         self.timeout = kwargs.get("timeout")
         self.settled = kwargs.get("settled", False)
+        self._network_trace_params = kwargs.get('network_trace_params')
 
     async def on_settled(self, reason, state):
         if self.on_delivery_settled and not self.settled:
             try:
                 await self.on_delivery_settled(reason, state)
             except Exception as e:  # pylint:disable=broad-except
-                _LOGGER.warning("Message 'on_send_complete' callback failed: %r", e)
+                _LOGGER.warning(
+                    "Message 'on_send_complete' callback failed: %r",
+                    e,
+                    extra=self._network_trace_params
+                )
         self.settled = True
 
 
 class SenderLink(Link):
     def __init__(self, session, handle, target_address, **kwargs):
         name = kwargs.pop("name", None) or str(uuid.uuid4())
         role = Role.Sender
@@ -72,15 +74,18 @@
         await self._remove_pending_deliveries()
 
     async def _incoming_flow(self, frame):
         rcv_link_credit = frame[6]  # link_credit
         rcv_delivery_count = frame[5]  # delivery_count
         if frame[4] is not None:  # handle
             if rcv_link_credit is None or rcv_delivery_count is None:
-                _LOGGER.info("Unable to get link-credit or delivery-count from incoming ATTACH. Detaching link.")
+                _LOGGER.info(
+                    "Unable to get link-credit or delivery-count from incoming ATTACH. Detaching link.",
+                    extra=self.network_trace_params
+                )
                 await self._remove_pending_deliveries()
                 await self._set_state(LinkState.DETACHED)  # TODO: Send detach now?
             else:
                 self.current_link_credit = rcv_delivery_count + rcv_link_credit - self.delivery_count
         await self.update_pending_deliveries()
 
     async def _outgoing_transfer(self, delivery):
@@ -96,20 +101,18 @@
             "rcv_settle_mode": None,
             "state": None,
             "resume": None,
             "aborted": None,
             "batchable": None,
             "payload": output,
         }
-        if self.network_trace:
-            _LOGGER.info(
-                "-> %r", TransferFrame(delivery_id="<pending>", **delivery.frame), extra=self.network_trace_params
-            )
-            _LOGGER.info("   %r", delivery.message, extra=self.network_trace_params)
-        await self._session._outgoing_transfer(delivery)  # pylint:disable=protected-access
+        await self._session._outgoing_transfer(  # pylint:disable=protected-access
+            delivery,
+            self.network_trace_params if self.network_trace else None
+        )
         sent_and_settled = False
         if delivery.transfer_state == SessionTransferState.OKAY:
             self.delivery_count = delivery_count
             self.current_link_credit -= 1
             delivery.sent = True
             if delivery.settled:
                 await delivery.on_settled(LinkDeliverySettleReason.SETTLED, None)
@@ -171,14 +174,15 @@
         if self.send_settle_mode == SenderSettleMode.Mixed:
             settled = kwargs.pop("settled", True)
         delivery = PendingDelivery(
             on_delivery_settled=kwargs.get("on_send_complete"),
             timeout=kwargs.get("timeout"),
             message=message,
             settled=settled,
+            network_trace_params=self.network_trace_params
         )
         if self.current_link_credit == 0 or send_async:
             self._pending_deliveries.append(delivery)
         else:
             sent_and_settled = await self._outgoing_transfer(delivery)
             if not sent_and_settled:
                 self._pending_deliveries.append(delivery)
```

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/__init__.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_connection_async.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_connection_async.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     WEBSOCKET_PORT,
     MAX_CHANNELS,
     MAX_FRAME_SIZE_BYTES,
     HEADER_FRAME,
     ConnectionState,
     EMPTY_FRAME,
     TransportType,
+    READ_TIMEOUT_INTERVAL
 )
 
 from ..error import ErrorCondition, AMQPConnectionError, AMQPError
 
 _LOGGER = logging.getLogger(__name__)
 
 
@@ -81,14 +82,19 @@
         # Custom Endpoint
         custom_endpoint_address = kwargs.get("custom_endpoint_address")
         custom_endpoint = None
         if custom_endpoint_address:
             custom_parsed_url = urlparse(custom_endpoint_address)
             custom_port = custom_parsed_url.port or WEBSOCKET_PORT
             custom_endpoint = f"{custom_parsed_url.hostname}:{custom_port}{custom_parsed_url.path}"
+        self._container_id = kwargs.pop("container_id", None) or str(
+            uuid.uuid4()
+        )  # type: str
+        self._network_trace = kwargs.get("network_trace", False)
+        self._network_trace_params = {"amqpConnection": self._container_id, "amqpSession": None, "amqpLink": None}
 
         transport = kwargs.get("transport")
         self._transport_type = kwargs.pop("transport_type", TransportType.Amqp)
         if transport:
             self._transport = transport
         elif "sasl_credential" in kwargs:
             sasl_transport = SASLTransport
@@ -97,22 +103,23 @@
             ):
                 sasl_transport = SASLWithWebSocket
                 endpoint = parsed_url.hostname + parsed_url.path
             self._transport = sasl_transport(
                 host=endpoint,
                 credential=kwargs["sasl_credential"],
                 custom_endpoint=custom_endpoint,
+                network_trace_params=self._network_trace_params,
                 **kwargs,
             )
         else:
-            self._transport = AsyncTransport(parsed_url.netloc, **kwargs)
+            self._transport = AsyncTransport(
+                parsed_url.netloc,
+                network_trace_params=self._network_trace_params,
+                **kwargs)
 
-        self._container_id = kwargs.pop("container_id", None) or str(
-            uuid.uuid4()
-        )  # type: str
         self._max_frame_size = kwargs.pop(
             "max_frame_size", MAX_FRAME_SIZE_BYTES
         )  # type: int
         self._remote_max_frame_size = None  # type: Optional[int]
         self._channel_max = kwargs.pop("channel_max", MAX_CHANNELS)  # type: int
         self._idle_timeout = kwargs.pop("idle_timeout", None)  # type: Optional[int]
         self._outgoing_locales = kwargs.pop(
@@ -136,20 +143,14 @@
         self._remote_idle_timeout_send_frame = None  # type: Optional[int]
         self._idle_timeout_empty_frame_send_ratio = kwargs.get(
             "idle_timeout_empty_frame_send_ratio", 0.5
         )
         self._last_frame_received_time = None  # type: Optional[float]
         self._last_frame_sent_time = None  # type: Optional[float]
         self._idle_wait_time = kwargs.get("idle_wait_time", 0.1)  # type: float
-        self._network_trace = kwargs.get("network_trace", False)
-        self._network_trace_params = {
-            "connection": self._container_id,
-            "session": None,
-            "link": None,
-        }
         self._error = None
         self._outgoing_endpoints = {}  # type: Dict[int, Session]
         self._incoming_endpoints = {}  # type: Dict[int, Session]
 
     async def __aenter__(self):
         await self.open()
         return self
@@ -161,18 +162,18 @@
         # type: (ConnectionState) -> None
         """Update the connection state."""
         if new_state is None:
             return
         previous_state = self.state
         self.state = new_state
         _LOGGER.info(
-            "Connection '%s' state changed: %r -> %r",
-            self._container_id,
+            "Connection state changed: %r -> %r",
             previous_state,
             new_state,
+            extra=self._network_trace_params
         )
         for session in self._outgoing_endpoints.values():
             await session._on_connection_state_change()  # pylint:disable=protected-access
 
     async def _connect(self):
         # type: () -> None
         """Initiate the connection.
@@ -187,23 +188,27 @@
             if not self.state:
                 await self._transport.connect()
                 await self._set_state(ConnectionState.START)
             await self._transport.negotiate()
             await self._outgoing_header()
             await self._set_state(ConnectionState.HDR_SENT)
             if not self._allow_pipelined_open:
-                await self._process_incoming_frame(*(await self._read_frame(wait=True)))
+                await self._read_frame(wait=True)
                 if self.state != ConnectionState.HDR_EXCH:
                     await self._disconnect()
                     raise ValueError(
                         "Did not receive reciprocal protocol header. Disconnecting."
                     )
             else:
                 await self._set_state(ConnectionState.HDR_SENT)
         except (OSError, IOError, SSLError, socket.error, asyncio.TimeoutError) as exc:
+            # FileNotFoundError is being raised for exception parity with uamqp when invalid
+            # `connection_verify` file path is passed in. Remove later when resolving issue #27128.
+            if isinstance(exc, FileNotFoundError) and exc.filename and "ca_certs" in exc.filename:
+                raise
             raise AMQPConnectionError(
                 ErrorCondition.SocketError,
                 description="Failed to initiate the connection due to exception: "
                 + str(exc),
                 error=exc,
             )
 
@@ -215,35 +220,34 @@
         await self._transport.close()
 
     def _can_read(self):
         # type: () -> bool
         """Whether the connection is in a state where it is legal to read for incoming frames."""
         return self.state not in (ConnectionState.CLOSE_RCVD, ConnectionState.END)
 
-    async def _read_frame(self, wait=True, **kwargs):  # type: ignore # TODO: missing return
-        # type: (bool, Any) -> Tuple[int, Optional[Tuple[int, NamedTuple]]]
+    async def _read_frame(self, wait: Union[bool, int, float] = True, **kwargs) -> bool:
         """Read an incoming frame from the transport.
 
         :param Union[bool, float] wait: Whether to block on the socket while waiting for an incoming frame.
          The default value is `False`, where the frame will block for the configured timeout only (0.1 seconds).
          If set to `True`, socket will block indefinitely. If set to a timeout value in seconds, the socket will
          block for at most that value.
         :rtype: Tuple[int, Optional[Tuple[int, NamedTuple]]]
         :returns: A tuple with the incoming channel number, and the frame in the form or a tuple of performative
          descriptor and field values.
         """
-        if self._can_read():
-            if wait is False:
-                timeout = 1  # TODO: What should this default be?
-            elif wait is True:
-                timeout = None
-            else:
-                timeout = wait
-            return await self._transport.receive_frame(timeout=timeout, **kwargs)
-        _LOGGER.warning("Cannot read frame in current state: %r", self.state)
+        timeout: Optional[Union[int, float]] = None
+        if wait is False:
+            timeout = READ_TIMEOUT_INTERVAL
+        elif wait is True:
+            timeout = None
+        else:
+            timeout = wait
+        new_frame = await self._transport.receive_frame(timeout=timeout, **kwargs)
+        return await self._process_incoming_frame(*new_frame)
 
     def _can_write(self):
         # type: () -> bool
         """Whether the connection is in a state where it is legal to write outgoing frames."""
         return self.state not in _CLOSING_STATES
 
     async def _send_frame(self, channel, frame, timeout=None, **kwargs):
@@ -276,15 +280,15 @@
             ) as exc:
                 self._error = AMQPConnectionError(
                     ErrorCondition.SocketError,
                     description="Can not send frame out due to exception: " + str(exc),
                     error=exc,
                 )
         else:
-            _LOGGER.warning("Cannot write frame in current state: %r", self.state)
+            _LOGGER.info("Cannot write frame in current state: %r", self.state, extra=self._network_trace_params)
 
     def _get_next_outgoing_channel(self):
         # type: () -> int
         """Get the next available outgoing channel number within the max channel limit.
 
         :raises ValueError: If maximum channels has been reached.
         :returns: The next available outgoing channel number.
@@ -303,15 +307,15 @@
         )
         return next_channel
 
     async def _outgoing_empty(self):
         # type: () -> None
         """Send an empty frame to prevent the connection from reaching an idle timeout."""
         if self._network_trace:
-            _LOGGER.info("-> empty()", extra=self._network_trace_params)
+            _LOGGER.debug("-> EmptyFrame()", extra=self._network_trace_params)
         try:
             raise self._error
         except TypeError:
             pass
         try:
             if self._can_write():
                 await self._transport.write(EMPTY_FRAME)
@@ -324,24 +328,22 @@
             )
 
     async def _outgoing_header(self):
         # type: () -> None
         """Send the AMQP protocol header to initiate the connection."""
         self._last_frame_sent_time = time.time()
         if self._network_trace:
-            _LOGGER.info(
-                "-> header(%r)", HEADER_FRAME, extra=self._network_trace_params
-            )
+            _LOGGER.debug("-> Header(%r)", HEADER_FRAME, extra=self._network_trace_params)
         await self._transport.write(HEADER_FRAME)
 
     async def _incoming_header(self, _, frame):
         # type: (int, bytes) -> None
         """Process an incoming AMQP protocol header and update the connection state."""
         if self._network_trace:
-            _LOGGER.info("<- header(%r)", frame, extra=self._network_trace_params)
+            _LOGGER.debug("<- Header(%r)", frame, extra=self._network_trace_params)
         if self.state == ConnectionState.START:
             await self._set_state(ConnectionState.HDR_RCVD)
         elif self.state == ConnectionState.HDR_SENT:
             await self._set_state(ConnectionState.HDR_EXCH)
         elif self.state == ConnectionState.OPEN_PIPE:
             await self._set_state(ConnectionState.OPEN_SENT)
 
@@ -363,15 +365,15 @@
             else None,
             desired_capabilities=self._desired_capabilities
             if self.state == ConnectionState.HDR_EXCH
             else None,
             properties=self._properties,
         )
         if self._network_trace:
-            _LOGGER.info("-> %r", open_frame, extra=self._network_trace_params)
+            _LOGGER.debug("-> %r", open_frame, extra=self._network_trace_params)
         await self._send_frame(0, open_frame)
 
     async def _incoming_open(self, channel, frame):
         # type: (int, Tuple[Any, ...]) -> None
         """Process incoming Open frame to finish the connection negotiation.
 
         The incoming frame format is::
@@ -390,117 +392,117 @@
         :param int channel: The incoming channel number.
         :param frame: The incoming Open frame.
         :type frame: Tuple[Any, ...]
         :rtype: None
         """
         # TODO: Add type hints for full frame tuple contents.
         if self._network_trace:
-            _LOGGER.info("<- %r", OpenFrame(*frame), extra=self._network_trace_params)
+            _LOGGER.debug("<- %r", OpenFrame(*frame), extra=self._network_trace_params)
         if channel != 0:
-            _LOGGER.error("OPEN frame received on a channel that is not 0.")
+            _LOGGER.error("OPEN frame received on a channel that is not 0.", extra=self._network_trace_params)
             await self.close(
                 error=AMQPError(
                     condition=ErrorCondition.NotAllowed,
                     description="OPEN frame received on a channel that is not 0.",
                 )
             )
             await self._set_state(ConnectionState.END)
         if self.state == ConnectionState.OPENED:
-            _LOGGER.error("OPEN frame received in the OPENED state.")
+            _LOGGER.error("OPEN frame received in the OPENED state.", extra=self._network_trace_params)
             await self.close()
         if frame[4]:
             self._remote_idle_timeout = frame[4] / 1000  # Convert to seconds
             self._remote_idle_timeout_send_frame = (
                 self._idle_timeout_empty_frame_send_ratio * self._remote_idle_timeout
             )
 
         if frame[2] < 512:
             # Max frame size is less than supported minimum
             # If any of the values in the received open frame are invalid then the connection shall be closed.
             # The error amqp:invalid-field shall be set in the error.condition field of the CLOSE frame.
             await self.close(
-                error=cast(
-                    AMQPError,
-                    AMQPConnectionError(
-                        condition=ErrorCondition.InvalidField,
-                        description="Failed parsing OPEN frame: Max frame size is less than supported minimum.",
-                    ),
+                error=AMQPError(
+                    condition=ErrorCondition.InvalidField,
+                    description="Failed parsing OPEN frame: Max frame size is less than supported minimum.",
                 )
             )
             _LOGGER.error(
-                "Failed parsing OPEN frame: Max frame size is less than supported minimum."
+                "Failed parsing OPEN frame: Max frame size is less than supported minimum.",
+                extra=self._network_trace_params
             )
-        else:
-            self._remote_max_frame_size = frame[2]
+            return
+        self._remote_max_frame_size = frame[2]
         if self.state == ConnectionState.OPEN_SENT:
             await self._set_state(ConnectionState.OPENED)
         elif self.state == ConnectionState.HDR_EXCH:
             await self._set_state(ConnectionState.OPEN_RCVD)
             await self._outgoing_open()
             await self._set_state(ConnectionState.OPENED)
         else:
             await self.close(
                 error=AMQPError(
                     condition=ErrorCondition.IllegalState,
-                    description=f"connection is an illegal state: {self.state}",
+                    description=f"Connection is an illegal state: {self.state}",
                 )
             )
-            _LOGGER.error("connection is an illegal state: %r", self.state)
+            _LOGGER.error("Connection is an illegal state: %r", self.state, extra=self._network_trace_params)
 
     async def _outgoing_close(self, error=None):
         # type: (Optional[AMQPError]) -> None
         """Send a Close frame to shutdown connection with optional error information."""
         close_frame = CloseFrame(error=error)
         if self._network_trace:
-            _LOGGER.info("-> %r", close_frame, extra=self._network_trace_params)
+            _LOGGER.debug("-> %r", close_frame, extra=self._network_trace_params)
         await self._send_frame(0, close_frame)
 
     async def _incoming_close(self, channel, frame):
         # type: (int, Tuple[Any, ...]) -> None
         """Process incoming Open frame to finish the connection negotiation.
 
         The incoming frame format is::
 
             - frame[0]: error (Optional[AMQPError])
 
         """
         if self._network_trace:
-            _LOGGER.info("<- %r", CloseFrame(*frame), extra=self._network_trace_params)
+            _LOGGER.debug("<- %r", CloseFrame(*frame), extra=self._network_trace_params)
         disconnect_states = [
             ConnectionState.HDR_RCVD,
             ConnectionState.HDR_EXCH,
             ConnectionState.OPEN_RCVD,
             ConnectionState.CLOSE_SENT,
             ConnectionState.DISCARDING,
         ]
         if self.state in disconnect_states:
             await self._disconnect()
-            await self._set_state(ConnectionState.END)
             return
 
         close_error = None
         if channel > self._channel_max:
-            _LOGGER.error("Invalid channel")
+            _LOGGER.error(
+                "CLOSE frame received on a channel greated than support max.",
+                extra=self._network_trace_params
+            )
             close_error = AMQPError(
                 condition=ErrorCondition.InvalidField,
                 description="Invalid channel",
                 info=None,
             )
 
         await self._set_state(ConnectionState.CLOSE_RCVD)
         await self._outgoing_close(error=close_error)
         await self._disconnect()
-        await self._set_state(ConnectionState.END)
 
         if frame[0]:
             self._error = AMQPConnectionError(
                 condition=frame[0][0], description=frame[0][1], info=frame[0][2]
             )
             _LOGGER.error(
-                "Connection error: %r",frame[0]
+                "Connection closed with error: %r", frame[0],
+                extra=self._network_trace_params
             )
 
     async def _incoming_begin(self, channel, frame):
         # type: (int, Tuple[Any, ...]) -> None
         """Process incoming Begin frame to finish negotiating a new session.
 
         The incoming frame format is::
@@ -550,14 +552,18 @@
         except KeyError:
             #close the connection
             await self.close(
                 error=AMQPError(
                     condition=ErrorCondition.ConnectionCloseForced,
                     description="Invalid channel number received"
                 ))
+            _LOGGER.error(
+                "END frame received on invalid channel. Closing connection.",
+                extra=self._network_trace_params
+            )
             return
 
     async def _process_incoming_frame(
         self, channel, frame
     ):  # pylint:disable=too-many-return-statements
         # type: (int, Optional[Union[bytes, Tuple[int, Tuple[Any, ...]]]]) -> bool
         """Process an incoming frame, either directly or by passing to the necessary Session.
@@ -616,15 +622,15 @@
                 await self._incoming_close(channel, fields)
                 return True
             if performative == 0:
                 await self._incoming_header(channel, cast(bytes, fields))
                 return True
             if performative == 1:
                 return False  # TODO: incoming EMPTY
-            _LOGGER.error("Unrecognized incoming frame: %s", frame)
+            _LOGGER.error("Unrecognized incoming frame: %r", frame, extra=self._network_trace_params)
             return True
         except KeyError:
             return True  # TODO: channel error
 
     async def _process_outgoing_frame(self, channel, frame):
         # type: (int, NamedTuple) -> None
         """Send an outgoing frame if the connection is in a legal state.
@@ -644,14 +650,18 @@
             raise ValueError("Connection not open.")
         now = time.time()
         if get_local_timeout(
             now,
             cast(float, self._idle_timeout),
             cast(float, self._last_frame_received_time),
         ) or (await self._get_remote_timeout(now)):
+            _LOGGER.info(
+                "No frame received for the idle timeout. Closing connection.",
+                extra=self._network_trace_params
+            )
             await self.close(
                 error=AMQPError(
                     condition=ErrorCondition.ConnectionCloseForced,
                     description="No frame received for the idle timeout.",
                 ),
                 wait=False,
             )
@@ -696,18 +706,14 @@
             timeout = time.time() + wait
             while self.state != end_state:
                 if time.time() >= timeout:
                     break
                 await asyncio.sleep(self._idle_wait_time)
                 await self.listen(wait=False)
 
-    async def _listen_one_frame(self, **kwargs):
-        new_frame = await self._read_frame(**kwargs)
-        return await self._process_incoming_frame(*new_frame)
-
     async def listen(self, wait=False, batch=1, **kwargs):
         # type: (Union[float, int, bool], int, Any) -> None
         """Listen on the socket for incoming frames and process them.
 
         :param wait: Whether to block on the socket until a frame arrives. If set to `True`, socket will
          block indefinitely. Alternatively, if set to a time in seconds, the socket will block for at most
          the specified timeout. Default value is `False`, where the socket will block for its configured read
@@ -726,14 +732,18 @@
             if self.state not in _CLOSING_STATES:
                 now = time.time()
                 if get_local_timeout(
                     now,
                     cast(float, self._idle_timeout),
                     cast(float, self._last_frame_received_time),
                 ) or (await self._get_remote_timeout(now)):
+                    _LOGGER.info(
+                        "No frame received for the idle timeout. Closing connection.",
+                        extra=self._network_trace_params
+                    )
                     await self.close(
                         error=AMQPError(
                             condition=ErrorCondition.ConnectionCloseForced,
                             description="No frame received for the idle timeout.",
                         ),
                         wait=False,
                     )
@@ -742,23 +752,28 @@
                 # TODO: check error condition
                 self._error = AMQPConnectionError(
                     condition=ErrorCondition.ConnectionCloseForced,
                     description="Connection was already closed.",
                 )
                 return
             for _ in range(batch):
-                if await asyncio.ensure_future(
-                    self._listen_one_frame(wait=wait, **kwargs)
-                ):
-                    # TODO: compare the perf difference between ensure_future and direct await
+                if self._can_read():
+                    if await self._read_frame(wait=wait, **kwargs):
+                        break
+                else:
+                    _LOGGER.info(
+                        "Connection cannot read frames in this state: %r",
+                        self.state,
+                        extra=self._network_trace_params
+                    )
                     break
         except (OSError, IOError, SSLError, socket.error) as exc:
             self._error = AMQPConnectionError(
                 ErrorCondition.SocketError,
-                description="Can not send frame out due to exception: " + str(exc),
+                description="Can not read frame due to exception: " + str(exc),
                 error=exc,
             )
 
     def create_session(self, **kwargs):
         # type: (Any) -> Session
         """Create a new session within this connection.
 
@@ -821,21 +836,21 @@
 
         Alternatively this method will be called on exiting a Connection context manager.
 
         :param ~uamqp.AMQPError error: Optional error information to include in the close request.
         :param bool wait: Whether to wait for a service Close response. Default is `False`.
         :rtype: None
         """
-        if self.state in [
-            ConnectionState.END,
-            ConnectionState.CLOSE_SENT,
-            ConnectionState.DISCARDING,
-        ]:
-            return
         try:
+            if self.state in [
+                ConnectionState.END,
+                ConnectionState.CLOSE_SENT,
+                ConnectionState.DISCARDING,
+            ]:
+                return
             await self._outgoing_close(error=error)
             if error:
                 self._error = AMQPConnectionError(
                     condition=error.condition,
                     description=error.description,
                     info=error.info,
                 )
@@ -846,11 +861,11 @@
             elif error:
                 await self._set_state(ConnectionState.DISCARDING)
             else:
                 await self._set_state(ConnectionState.CLOSE_SENT)
             await self._wait_for_response(wait, ConnectionState.END)
         except Exception as exc:  # pylint:disable=broad-except
             # If error happened during closing, ignore the error and set state to END
-            _LOGGER.info("An error occurred when closing the connection: %r", exc)
+            _LOGGER.info("An error occurred when closing the connection: %r", exc, extra=self._network_trace_params)
             await self._set_state(ConnectionState.END)
         finally:
             await self._disconnect()
```

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_session_async.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_session_async.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # --------------------------------------------------------------------------
 
 from __future__ import annotations
 import uuid
 import logging
 import time
 import asyncio
-from typing import Optional, Union
+from typing import Optional, Union, List
 
 from ..constants import ConnectionState, SessionState, SessionTransferState, Role
 from ._sender_async import SenderLink
 from ._receiver_async import ReceiverLink
 from ._management_link_async import ManagementLink
 from ..performatives import (
     BeginFrame,
@@ -57,15 +57,15 @@
         self.offered_capabilities = None
         self.desired_capabilities = kwargs.pop("desired_capabilities", None)
 
         self.allow_pipelined_open = kwargs.pop("allow_pipelined_open", True)
         self.idle_wait_time = kwargs.get("idle_wait_time", 0.1)
         self.network_trace = kwargs["network_trace"]
         self.network_trace_params = kwargs["network_trace_params"]
-        self.network_trace_params["session"] = self.name
+        self.network_trace_params["amqpSession"] = self.name
 
         self.links = {}
         self._connection = connection
         self._output_handles = {}
         self._input_handles = {}
 
     async def __aenter__(self):
@@ -90,20 +90,16 @@
         self.state = new_state
         _LOGGER.info(
             "Session state changed: %r -> %r",
             previous_state,
             new_state,
             extra=self.network_trace_params,
         )
-        futures = []
         for link in self.links.values():
-            futures.append(
-                asyncio.ensure_future(link._on_session_state_change())  # pylint: disable=protected-access
-            )
-        await asyncio.gather(*futures)
+            await link._on_session_state_change()  # pylint: disable=protected-access
 
     async def _on_connection_state_change(self):
         if self._connection.state in [ConnectionState.CLOSE_RCVD, ConnectionState.END]:
             if self.state not in [SessionState.DISCARDING, SessionState.UNMAPPED]:
                 await self._set_state(SessionState.DISCARDING)
 
     def _get_next_output_handle(self):
@@ -111,50 +107,36 @@
         """Get the next available outgoing handle number within the max handle limit.
 
         :raises ValueError: If maximum handle has been reached.
         :returns: The next available outgoing handle number.
         :rtype: int
         """
         if len(self._output_handles) >= self.handle_max:
-            raise ValueError(
-                "Maximum number of handles ({}) has been reached.".format(
-                    self.handle_max
-                )
-            )
-        next_handle = next(
-            i for i in range(1, self.handle_max) if i not in self._output_handles
-        )
+            raise ValueError("Maximum number of handles ({}) has been reached.".format(self.handle_max))
+        next_handle = next(i for i in range(1, self.handle_max) if i not in self._output_handles)
         return next_handle
 
     async def _outgoing_begin(self):
         begin_frame = BeginFrame(
-            remote_channel=self.remote_channel
-            if self.state == SessionState.BEGIN_RCVD
-            else None,
+            remote_channel=self.remote_channel if self.state == SessionState.BEGIN_RCVD else None,
             next_outgoing_id=self.next_outgoing_id,
             outgoing_window=self.outgoing_window,
             incoming_window=self.incoming_window,
             handle_max=self.handle_max,
-            offered_capabilities=self.offered_capabilities
-            if self.state == SessionState.BEGIN_RCVD
-            else None,
-            desired_capabilities=self.desired_capabilities
-            if self.state == SessionState.UNMAPPED
-            else None,
+            offered_capabilities=self.offered_capabilities if self.state == SessionState.BEGIN_RCVD else None,
+            desired_capabilities=self.desired_capabilities if self.state == SessionState.UNMAPPED else None,
             properties=self.properties,
         )
         if self.network_trace:
-            _LOGGER.info("-> %r", begin_frame, extra=self.network_trace_params)
-        await self._connection._process_outgoing_frame(  # pylint: disable=protected-access
-            self.channel, begin_frame
-        )
+            _LOGGER.debug("-> %r", begin_frame, extra=self.network_trace_params)
+        await self._connection._process_outgoing_frame(self.channel, begin_frame)  # pylint: disable=protected-access
 
     async def _incoming_begin(self, frame):
         if self.network_trace:
-            _LOGGER.info("<- %r", BeginFrame(*frame), extra=self.network_trace_params)
+            _LOGGER.debug("<- %r", BeginFrame(*frame), extra=self.network_trace_params)
         self.handle_max = frame[4]  # handle_max
         self.next_incoming_id = frame[1]  # next_outgoing_id
         self.remote_incoming_window = frame[2]  # incoming_window
         self.remote_outgoing_window = frame[3]  # outgoing_window
         if self.state == SessionState.BEGIN_SENT:
             self.remote_channel = frame[0]  # remote_channel
             await self._set_state(SessionState.MAPPED)
@@ -162,121 +144,103 @@
             await self._set_state(SessionState.BEGIN_RCVD)
             await self._outgoing_begin()
             await self._set_state(SessionState.MAPPED)
 
     async def _outgoing_end(self, error=None):
         end_frame = EndFrame(error=error)
         if self.network_trace:
-            _LOGGER.info("-> %r", end_frame, extra=self.network_trace_params)
-        await self._connection._process_outgoing_frame(  # pylint: disable=protected-access
-            self.channel, end_frame
-        )
+            _LOGGER.debug("-> %r", end_frame, extra=self.network_trace_params)
+        await self._connection._process_outgoing_frame(self.channel, end_frame)  # pylint: disable=protected-access
 
     async def _incoming_end(self, frame):
         if self.network_trace:
-            _LOGGER.info("<- %r", EndFrame(*frame), extra=self.network_trace_params)
+            _LOGGER.debug("<- %r", EndFrame(*frame), extra=self.network_trace_params)
         if self.state not in [
             SessionState.END_RCVD,
             SessionState.END_SENT,
             SessionState.DISCARDING,
         ]:
             await self._set_state(SessionState.END_RCVD)
             for _, link in self.links.items():
                 await link.detach()
             # TODO: handling error
             await self._outgoing_end()
         await self._set_state(SessionState.UNMAPPED)
 
     async def _outgoing_attach(self, frame):
-        await self._connection._process_outgoing_frame(  # pylint: disable=protected-access
-            self.channel, frame
-        )
+        await self._connection._process_outgoing_frame(self.channel, frame)  # pylint: disable=protected-access
 
     async def _incoming_attach(self, frame):
         try:
-            self._input_handles[frame[1]] = self.links[
-                frame[0].decode("utf-8")
-            ]  # name and handle
-            await self._input_handles[frame[1]]._incoming_attach(  # pylint: disable=protected-access
-                frame
-            )
+            self._input_handles[frame[1]] = self.links[frame[0].decode("utf-8")]  # name and handle
+            await self._input_handles[frame[1]]._incoming_attach(frame)  # pylint: disable=protected-access
         except KeyError:
             try:
                 outgoing_handle = self._get_next_output_handle()
             except ValueError:
+                _LOGGER.error(
+                    "Unable to attach new link - cannot allocate more handles.",
+                    extra=self.network_trace_params
+                )
                 # detach the link that would have been set.
                 await self.links[frame[0].decode("utf-8")].detach(
                     error=AMQPError(
                         condition=ErrorCondition.LinkDetachForced,
-                        description="""Cannot allocate more handles, """
-                        """the max number of handles is {}. Detaching link""".format(
-                            self.handle_max
-                        ),
+                        description=f"Cannot allocate more handles, the max number of handles is {self.handle_max}. Detaching link", # pylint: disable=line-too-long
                         info=None,
                     )
                 )
                 return
             if frame[2] == Role.Sender:
-                new_link = ReceiverLink.from_incoming_frame(
-                    self, outgoing_handle, frame
-                )
+                new_link = ReceiverLink.from_incoming_frame(self, outgoing_handle, frame)
             else:
                 new_link = SenderLink.from_incoming_frame(self, outgoing_handle, frame)
             await new_link._incoming_attach(frame)  # pylint: disable=protected-access
             self.links[frame[0]] = new_link
             self._output_handles[outgoing_handle] = new_link
             self._input_handles[frame[1]] = new_link
-        except ValueError:
+        except ValueError as e:
             # Reject Link
+            _LOGGER.error(
+                    "Unable to attach new link: %r",
+                    e,
+                    extra=self.network_trace_params
+            )
             await self._input_handles[frame[1]].detach()
 
     async def _outgoing_flow(self, frame=None):
         link_flow = frame or {}
         link_flow.update(
             {
                 "next_incoming_id": self.next_incoming_id,
                 "incoming_window": self.incoming_window,
                 "next_outgoing_id": self.next_outgoing_id,
                 "outgoing_window": self.outgoing_window,
             }
         )
         flow_frame = FlowFrame(**link_flow)
         if self.network_trace:
-            _LOGGER.info("-> %r", flow_frame, extra=self.network_trace_params)
-        await self._connection._process_outgoing_frame(  # pylint: disable=protected-access
-            self.channel, flow_frame
-        )
+            _LOGGER.debug("-> %r", flow_frame, extra=self.network_trace_params)
+        await self._connection._process_outgoing_frame(self.channel, flow_frame)  # pylint: disable=protected-access
 
     async def _incoming_flow(self, frame):
         if self.network_trace:
-            _LOGGER.info("<- %r", FlowFrame(*frame), extra=self.network_trace_params)
+            _LOGGER.debug("<- %r", FlowFrame(*frame), extra=self.network_trace_params)
         self.next_incoming_id = frame[2]  # next_outgoing_id
-        remote_incoming_id = (
-            frame[0] or self.next_outgoing_id
-        )  #  next_incoming_id  TODO "initial-outgoing-id"
-        self.remote_incoming_window = (
-            remote_incoming_id + frame[1] - self.next_outgoing_id
-        )  # incoming_window
+        remote_incoming_id = frame[0] or self.next_outgoing_id  #  next_incoming_id  TODO "initial-outgoing-id"
+        self.remote_incoming_window = remote_incoming_id + frame[1] - self.next_outgoing_id  # incoming_window
         self.remote_outgoing_window = frame[3]  # outgoing_window
         if frame[4] is not None:  # handle
-            await self._input_handles[frame[4]]._incoming_flow(  # pylint: disable=protected-access
-                frame
-            )
+            await self._input_handles[frame[4]]._incoming_flow(frame)  # pylint: disable=protected-access
         else:
-            futures = []
             for link in self._output_handles.values():
-                if (
-                    self.remote_incoming_window > 0 and not link._is_closed  # pylint: disable=protected-access
-                ):
-                    futures.append(
-                        link._incoming_flow(frame)  # pylint: disable=protected-access
-                    )
-            await asyncio.gather(*futures)
+                if self.remote_incoming_window > 0 and not link._is_closed:  # pylint: disable=protected-access
+                    await link._incoming_flow(frame)  # pylint: disable=protected-access
 
-    async def _outgoing_transfer(self, delivery):
+    async def _outgoing_transfer(self, delivery, network_trace_params):
         if self.state != SessionState.MAPPED:
             delivery.transfer_state = SessionTransferState.ERROR
         if self.remote_incoming_window <= 0:
             delivery.transfer_state = SessionTransferState.BUSY
         else:
             payload = delivery.frame["payload"]
             payload_size = len(payload)
@@ -305,19 +269,32 @@
                     "settled": delivery.frame["settled"],
                     "more": True,
                     "rcv_settle_mode": delivery.frame["rcv_settle_mode"],
                     "state": delivery.frame["state"],
                     "resume": delivery.frame["resume"],
                     "aborted": delivery.frame["aborted"],
                     "batchable": delivery.frame["batchable"],
-                    "payload": payload[start_idx : start_idx + available_frame_size],
                     "delivery_id": self.next_outgoing_id,
                 }
+                if network_trace_params:
+                    # We determine the logging for the outgoing Transfer frames based on the source
+                    # Link configuration rather than the Session, because it's only at the Session
+                    # level that we can determine how many outgoing frames are needed and their
+                    # delivery IDs.
+                    # TODO: Obscuring the payload for now to investigate the potential for leaks.
+                    _LOGGER.debug(
+                        "-> %r", TransferFrame(payload=b"***", **tmp_delivery_frame),
+                        extra=network_trace_params
+                    )
                 await self._connection._process_outgoing_frame(  # pylint: disable=protected-access
-                    self.channel, TransferFrame(**tmp_delivery_frame)
+                    self.channel,
+                    TransferFrame(
+                        payload=payload[start_idx : start_idx + available_frame_size],
+                        **tmp_delivery_frame
+                    )
                 )
                 start_idx += available_frame_size
                 remaining_payload_cnt -= available_frame_size
 
             # encode the last frame
             tmp_delivery_frame = {
                 "handle": delivery.frame["handle"],
@@ -326,68 +303,70 @@
                 "settled": delivery.frame["settled"],
                 "more": False,
                 "rcv_settle_mode": delivery.frame["rcv_settle_mode"],
                 "state": delivery.frame["state"],
                 "resume": delivery.frame["resume"],
                 "aborted": delivery.frame["aborted"],
                 "batchable": delivery.frame["batchable"],
-                "payload": payload[start_idx:],
                 "delivery_id": self.next_outgoing_id,
             }
+            if network_trace_params:
+                # We determine the logging for the outgoing Transfer frames based on the source
+                # Link configuration rather than the Session, because it's only at the Session
+                # level that we can determine how many outgoing frames are needed and their
+                # delivery IDs.
+                # TODO: Obscuring the payload for now to investigate the potential for leaks.
+                _LOGGER.debug(
+                    "-> %r", TransferFrame(payload=b"***", **tmp_delivery_frame),
+                    extra=network_trace_params
+                )
             await self._connection._process_outgoing_frame(  # pylint: disable=protected-access
-                self.channel, TransferFrame(**tmp_delivery_frame)
+                self.channel,
+                TransferFrame(payload=payload[start_idx:], **tmp_delivery_frame)
             )
             self.next_outgoing_id += 1
             self.remote_incoming_window -= 1
             self.outgoing_window -= 1
             # TODO: We should probably handle an error at the connection and update state accordingly
             delivery.transfer_state = SessionTransferState.OKAY
 
     async def _incoming_transfer(self, frame):
         self.next_incoming_id += 1
         self.remote_outgoing_window -= 1
         self.incoming_window -= 1
         try:
-            await self._input_handles[frame[0]]._incoming_transfer(  # pylint: disable=protected-access
-                frame
-            )
+            await self._input_handles[frame[0]]._incoming_transfer(frame)  # pylint: disable=protected-access
         except KeyError:
+            _LOGGER.error(
+                "Received Transfer frame on unattached link. Ending session.",
+                extra=self.network_trace_params
+            )
             await self._set_state(SessionState.DISCARDING)
             await self.end(
                 error=AMQPError(
                     condition=ErrorCondition.SessionUnattachedHandle,
                     description="""Invalid handle reference in received frame: """
-                        """Handle is not currently associated with an attached link""",
+                    """Handle is not currently associated with an attached link""",
                 )
             )
         if self.incoming_window == 0:
             self.incoming_window = self.target_incoming_window
             await self._outgoing_flow()
 
     async def _outgoing_disposition(self, frame):
-        await self._connection._process_outgoing_frame(  # pylint: disable=protected-access
-            self.channel, frame
-        )
+        await self._connection._process_outgoing_frame(self.channel, frame)  # pylint: disable=protected-access
 
     async def _incoming_disposition(self, frame):
         if self.network_trace:
-            _LOGGER.info(
-                "<- %r", DispositionFrame(*frame), extra=self.network_trace_params
-            )
-        futures = []
+            _LOGGER.debug("<- %r", DispositionFrame(*frame), extra=self.network_trace_params)
         for link in self._input_handles.values():
-            asyncio.ensure_future(
-                link._incoming_disposition(frame)  # pylint: disable=protected-access
-            )
-        await asyncio.gather(*futures)
+            await link._incoming_disposition(frame)  # pylint: disable=protected-access
 
     async def _outgoing_detach(self, frame):
-        await self._connection._process_outgoing_frame(  # pylint: disable=protected-access
-            self.channel, frame
-        )
+        await self._connection._process_outgoing_frame(self.channel, frame)  # pylint: disable=protected-access
 
     async def _incoming_detach(self, frame):
         try:
             link = self._input_handles[frame[0]]  # handle
             await link._incoming_detach(frame)  # pylint: disable=protected-access
             # if link._is_closed:  TODO
             #     self.links.pop(link.name, None)
@@ -395,15 +374,15 @@
             #     self._output_handles.pop(link.handle, None)
         except KeyError:
             await self._set_state(SessionState.DISCARDING)
             await self._connection.close(
                 error=AMQPError(
                     condition=ErrorCondition.SessionUnattachedHandle,
                     description="""Invalid handle reference in received frame: """
-                        """Handle is not currently associated with an attached link""",
+                    """Handle is not currently associated with an attached link""",
                 )
             )
 
     async def _wait_for_response(self, wait, end_state):
         # type: (Union[bool, float], SessionState) -> None
         if wait is True:
             await self._connection.listen(wait=False)
@@ -421,30 +400,28 @@
 
     async def begin(self, wait=False):
         await self._outgoing_begin()
         await self._set_state(SessionState.BEGIN_SENT)
         if wait:
             await self._wait_for_response(wait, SessionState.BEGIN_SENT)
         elif not self.allow_pipelined_open:
-            raise ValueError(
-                "Connection has been configured to not allow piplined-open. Please set 'wait' parameter."
-            )
+            raise ValueError("Connection has been configured to not allow piplined-open. Please set 'wait' parameter.")
 
     async def end(self, error=None, wait=False):
         # type: (Optional[AMQPError], bool) -> None
         try:
             if self.state not in [SessionState.UNMAPPED, SessionState.DISCARDING]:
                 await self._outgoing_end(error=error)
             for _, link in self.links.items():
                 await link.detach()
             new_state = SessionState.DISCARDING if error else SessionState.END_SENT
             await self._set_state(new_state)
             await self._wait_for_response(wait, SessionState.UNMAPPED)
         except Exception as exc:  # pylint: disable=broad-except
-            _LOGGER.info("An error occurred when ending the session: %r", exc)
+            _LOGGER.info("An error occurred when ending the session: %r", exc, extra=self.network_trace_params)
             await self._set_state(SessionState.UNMAPPED)
 
     def create_receiver_link(self, source_address, **kwargs):
         assigned_handle = self._get_next_output_handle()
         link = ReceiverLink(
             self,
             handle=assigned_handle,
@@ -472,9 +449,10 @@
         return link
 
     def create_request_response_link_pair(self, endpoint, **kwargs):
         return ManagementLink(
             self,
             endpoint,
             network_trace=kwargs.pop("network_trace", self.network_trace),
+            network_trace_params=dict(self.network_trace_params),
             **kwargs,
         )
```

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_client_async.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_client_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,29 +131,43 @@
      If port is not specified in the `custom_endpoint_address`, by default port 443 will be used.
     :paramtype custom_endpoint_address: str
     :keyword connection_verify: Path to the custom CA_BUNDLE file of the SSL certificate which is used to
      authenticate the identity of the connection endpoint.
      Default is None in which case `certifi.where()` will be used.
     :paramtype connection_verify: str
     """
+
+    def __init__(self, hostname, **kwargs):
+        self._mgmt_link_lock_async = asyncio.Lock()
+        super().__init__(hostname,**kwargs)
+
+
     async def _keep_alive_async(self):
         start_time = time.time()
         try:
             while self._connection and not self._shutdown:
                 current_time = time.time()
                 elapsed_time = current_time - start_time
                 if elapsed_time >= self._keep_alive_interval:
-                    _logger.info("Keeping %r connection alive. %r",
-                                 self.__class__.__name__,
-                                 self._connection.container_id)
-                    await asyncio.shield(self._connection.work_async())
+                    _logger.debug(
+                        "Keeping %r connection alive.",
+                        self.__class__.__name__,
+                        extra=self._network_trace_params
+                    )
+                    await asyncio.shield(self._connection.listen(wait=self._socket_timeout,
+                        batch=self._link.current_link_credit))
                     start_time = current_time
                 await asyncio.sleep(1)
         except Exception as e:  # pylint: disable=broad-except
-            _logger.info("Connection keep-alive for %r failed: %r.", self.__class__.__name__, e)
+            _logger.info(
+                "Connection keep-alive for %r failed: %r.",
+                self.__class__.__name__,
+                e,
+                extra=self._network_trace_params
+            )
 
     async def __aenter__(self):
         """Run Client in an async context manager."""
         await self.open_async()
         return self
 
     async def __aexit__(self, *args):
@@ -217,15 +231,14 @@
         :param connection: An existing Connection that may be shared between
          multiple clients.
         :type connection: ~pyamqp.aio.Connection
         """
         # pylint: disable=protected-access
         if self._session:
             return  # already open.
-        _logger.debug("Opening client connection.")
         if connection:
             self._connection = connection
             self._external_connection = True
         if not self._connection:
             self._connection = Connection(
                 "amqps://" + self._hostname,
                 sasl_credential=self._auth.sasl,
@@ -250,39 +263,44 @@
         if self._auth.auth_type == AUTH_TYPE_CBS:
             self._cbs_authenticator = CBSAuthenticator(
                 session=self._session,
                 auth=self._auth,
                 auth_timeout=self._auth_timeout
             )
             await self._cbs_authenticator.open()
+        self._network_trace_params["amqpConnection"] = self._connection._container_id
+        self._network_trace_params["amqpSession"] = self._session.name
         self._shutdown = False
+
         if self._keep_alive_interval:
             self._keep_alive_thread = asyncio.ensure_future(self._keep_alive_async())
 
     async def close_async(self):
         """Close the client asynchronously. This includes closing the Session
         and CBS authentication layer as well as the Connection.
         If the client was opened using an external Connection,
         this will be left intact.
         """
         self._shutdown = True
         if not self._session:
             return  # already closed.
-        if self._keep_alive_thread:
-            await self._keep_alive_thread
-            self._keep_alive_thread = None
         await self._close_link_async()
         if self._cbs_authenticator:
             await self._cbs_authenticator.close()
             self._cbs_authenticator = None
         await self._session.end()
         self._session = None
         if not self._external_connection:
             await self._connection.close()
             self._connection = None
+        if self._keep_alive_thread:
+            await self._keep_alive_thread
+            self._keep_alive_thread = None
+        self._network_trace_params["amqpConnection"] = None
+        self._network_trace_params["amqpSession"] = None
 
     async def auth_complete_async(self):
         """Whether the authentication handshake is complete during
         connection initialization.
 
         :rtype: bool
         """
@@ -314,14 +332,15 @@
         This will return `True` if the connection is still open
         and ready to be used for further work, or `False` if it needs
         to be shut down.
 
         :rtype: bool
         :raises: TimeoutError if CBS authentication timeout reached.
         """
+
         if self._shutdown:
             return False
         if not await self.client_ready_async():
             return True
         return await self._client_run_async(**kwargs)
 
     async def mgmt_request_async(self, message, **kwargs):
@@ -343,23 +362,24 @@
         # The method also takes "status_code_field" and "status_description_field"
         # keyword arguments as alternate names for the status code and description
         # in the response body. Those two keyword arguments are used in Azure services only.
         operation = kwargs.pop("operation", None)
         operation_type = kwargs.pop("operation_type", None)
         node = kwargs.pop("node", "$management")
         timeout = kwargs.pop('timeout', 0)
-        try:
-            mgmt_link = self._mgmt_links[node]
-        except KeyError:
-            mgmt_link = ManagementOperation(self._session, endpoint=node, **kwargs)
-            self._mgmt_links[node] = mgmt_link
-            await mgmt_link.open()
+        async with self._mgmt_link_lock_async:
+            try:
+                mgmt_link = self._mgmt_links[node]
+            except KeyError:
+                mgmt_link = ManagementOperation(self._session, endpoint=node, **kwargs)
+                self._mgmt_links[node] = mgmt_link
+                await mgmt_link.open()
 
-            while not await mgmt_link.ready():
-                await self._connection.listen(wait=False)
+        while not await mgmt_link.ready():
+            await self._connection.listen(wait=False)
 
         operation_type = operation_type or b'empty'
         status, description, response = await mgmt_link.execute(
             message,
             operation=operation,
             operation_type=operation_type,
             timeout=timeout
@@ -489,21 +509,16 @@
         """MessageSender Link is now open - perform message send
         on all pending messages.
         Will return True if operation successful and client can remain open for
         further work.
 
         :rtype: bool
         """
-        try:
-            await self._link.update_pending_deliveries()
-            await self._connection.listen(wait=self._socket_timeout, **kwargs)
-        except ValueError:
-            _logger.info("Timeout reached, closing sender.")
-            self._shutdown = True
-            return False
+        await self._link.update_pending_deliveries()
+        await self._connection.listen(wait=self._socket_timeout, **kwargs)
         return True
 
     async def _transfer_message_async(self, message_delivery, timeout=0):
         message_delivery.state = MessageDeliveryState.WaitingForSendAck
         on_send_complete = partial(self._on_send_complete_async, message_delivery)
         delivery = await self._link.send_transfer(
             message_delivery.message,
@@ -558,14 +573,19 @@
             await asyncio.sleep(0.05)
 
         await self._transfer_message_async(message_delivery, timeout)
 
         running = True
         while running and message_delivery.state not in MESSAGE_DELIVERY_DONE_STATES:
             running = await self.do_work_async()
+        if message_delivery.state not in MESSAGE_DELIVERY_DONE_STATES:
+            raise MessageException(
+                condition=ErrorCondition.ClientError,
+                description="Send failed - connection not running."
+            )
 
         if message_delivery.state in (
             MessageDeliveryState.Error,
             MessageDeliveryState.Cancelled,
             MessageDeliveryState.Timeout
         ):
             try:
@@ -707,50 +727,48 @@
         """MessageReceiver Link is now open - start receiving messages.
         Will return True if operation successful and client can remain open for
         further work.
 
         :rtype: bool
         """
         try:
-            await self._link.flow()
+            if self._link.current_link_credit == 0:
+                await self._link.flow()
             await self._connection.listen(wait=self._socket_timeout, **kwargs)
         except ValueError:
-            _logger.info("Timeout reached, closing receiver.")
+            _logger.info("Timeout reached, closing receiver.", extra=self._network_trace_params)
             self._shutdown = True
             return False
         return True
 
     async def _message_received_async(self, frame, message):
         """Callback run on receipt of every message. If there is
         a user-defined callback, this will be called.
         Additionally if the client is retrieving messages for a batch
         or iterator, the message will be added to an internal queue.
 
         :param message: Received message.
         :type message: ~pyamqp.message.Message
         """
+        self._last_activity_timestamp = time.time()
         if self._message_received_callback:
             await self._message_received_callback(message)
         if not self._streaming_receive:
             self._received_messages.put((frame, message))
-        # TODO: do we need settled property for a message?
-        # elif not message.settled:
-        #    # Message was received with callback processing and wasn't settled.
-        #    _logger.info("Message was not settled.")
 
     async def _receive_message_batch_impl_async(self, max_batch_size=None, on_message_received=None, timeout=0):
         self._message_received_callback = on_message_received
         max_batch_size = max_batch_size or self._link_credit
         timeout_time = time.time() + timeout if timeout else 0
         receiving = True
         batch = []
         await self.open_async()
         while len(batch) < max_batch_size:
             try:
-                # TODO: This looses the transfer frame data
+                # TODO: This drops the transfer frame data
                 _, message = self._received_messages.get_nowait()
                 batch.append(message)
                 self._received_messages.task_done()
             except queue.Empty:
                 break
         else:
             return batch
@@ -816,14 +834,56 @@
         :paramtype timeout: float
         """
         return await self._do_retryable_operation_async(
             self._receive_message_batch_impl_async,
             **kwargs
         )
 
+    async def receive_messages_iter_async(self, timeout=None, on_message_received=None):
+        """Receive messages by generator. Messages returned in the generator have already been
+        accepted - if you wish to add logic to accept or reject messages based on custom
+        criteria, pass in a callback.
+
+        :param on_message_received: A callback to process messages as they arrive from the
+         service. It takes a single argument, a ~pyamqp.message.Message object.
+        :type on_message_received: callable[~pyamqp.message.Message]
+        """
+        self._message_received_callback = on_message_received
+        return self._message_generator_async(timeout=timeout)
+
+    async def _message_generator_async(self, timeout=None):
+        """Iterate over processed messages in the receive queue.
+
+        :rtype: generator[~pyamqp.message.Message]
+        """
+        self.open()
+        receiving = True
+        message = None
+        self._last_activity_timestamp = time.time()
+        self._timeout_reached = False
+        self._timeout = timeout if timeout else self._timeout
+        try:
+            while receiving and not self._timeout_reached:
+                if self._timeout > 0:
+                    if time.time() - self._last_activity_timestamp >= self._timeout:
+                        self._timeout_reached = True
+
+                if not self._timeout_reached:
+                    receiving = await self.do_work_async()
+
+                while not self._received_messages.empty():
+                    message = self._received_messages.get()
+                    self._last_activity_timestamp = time.time()
+                    self._received_messages.task_done()
+                    yield message
+
+        finally:
+            if self._shutdown:
+                await self.close_async()
+
     @overload
     async def settle_messages_async(
         self,
         delivery_id: Union[int, Tuple[int, int]],
         outcome: Literal["accepted"],
         *,
         batchable: Optional[bool] = None
```

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_management_link_async.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_management_link_async.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,28 +34,31 @@
     """
 
     def __init__(self, session, endpoint, **kwargs):
         self.next_message_id = 0
         self.state = ManagementLinkState.IDLE
         self._pending_operations = []
         self._session = session
+        self._network_trace_params = kwargs.get('network_trace_params')
         self._request_link: SenderLink = session.create_sender_link(
             endpoint,
             source_address=endpoint,
             on_link_state_change=self._on_sender_state_change,
             send_settle_mode=SenderSettleMode.Unsettled,
             rcv_settle_mode=ReceiverSettleMode.First,
+            network_trace=kwargs.get("network_trace", False)
         )
         self._response_link: ReceiverLink = session.create_receiver_link(
             endpoint,
             target_address=endpoint,
             on_link_state_change=self._on_receiver_state_change,
             on_transfer=self._on_message_received,
             send_settle_mode=SenderSettleMode.Unsettled,
             rcv_settle_mode=ReceiverSettleMode.First,
+            network_trace=kwargs.get("network_trace", False)
         )
         self._on_amqp_management_error = kwargs.get("on_amqp_management_error")
         self._on_amqp_management_open_complete = kwargs.get("on_amqp_management_open_complete")
 
         self._status_code_field = kwargs.get("status_code_field", b"statusCode")
         self._status_description_field = kwargs.get("status_description_field", b"statusDescription")
 
@@ -66,15 +69,20 @@
         await self.open()
         return self
 
     async def __aexit__(self, *args):
         await self.close()
 
     async def _on_sender_state_change(self, previous_state, new_state):
-        _LOGGER.info("Management link sender state changed: %r -> %r", previous_state, new_state)
+        _LOGGER.info(
+            "Management link sender state changed: %r -> %r",
+            previous_state,
+            new_state,
+            extra=self._network_trace_params
+        )
         if new_state == previous_state:
             return
         if self.state == ManagementLinkState.OPENING:
             if new_state == LinkState.ATTACHED:
                 self._sender_connected = True
                 if self._receiver_connected:
                     self.state = ManagementLinkState.OPEN
@@ -91,15 +99,20 @@
                 self.state = ManagementLinkState.ERROR
                 await self._on_amqp_management_error()
         elif self.state == ManagementLinkState.ERROR:
             # All state transitions shall be ignored.
             return
 
     async def _on_receiver_state_change(self, previous_state, new_state):
-        _LOGGER.info("Management link receiver state changed: %r -> %r", previous_state, new_state)
+        _LOGGER.info(
+            "Management link receiver state changed: %r -> %r",
+            previous_state,
+            new_state,
+            extra=self._network_trace_params
+        )
         if new_state == previous_state:
             return
         if self.state == ManagementLinkState.OPENING:
             if new_state == LinkState.ATTACHED:
                 self._receiver_connected = True
                 if self._sender_connected:
                     self.state = ManagementLinkState.OPEN
```

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_sasl_async.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_sasl_async.py`

 * *Files identical despite different names*

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_link_async.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_link_async.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         self.available = kwargs.pop("available", None)
         self.properties = kwargs.pop("properties", None)
         self.offered_capabilities = None
         self.desired_capabilities = kwargs.pop("desired_capabilities", None)
 
         self.network_trace = kwargs["network_trace"]
         self.network_trace_params = kwargs["network_trace_params"]
-        self.network_trace_params["link"] = self.name
+        self.network_trace_params["amqpLink"] = self.name
         self._session = session
         self._is_closed = False
         self._on_link_state_change = kwargs.get("on_link_state_change")
         self._on_attach = kwargs.get("on_attach")
         self._error = None
 
     async def __aenter__(self):
@@ -154,24 +154,24 @@
             initial_delivery_count=self.initial_delivery_count if self.role == Role.Sender else None,
             max_message_size=self.max_message_size,
             offered_capabilities=self.offered_capabilities if self.state == LinkState.ATTACH_RCVD else None,
             desired_capabilities=self.desired_capabilities if self.state == LinkState.DETACHED else None,
             properties=self.properties,
         )
         if self.network_trace:
-            _LOGGER.info("-> %r", attach_frame, extra=self.network_trace_params)
+            _LOGGER.debug("-> %r", attach_frame, extra=self.network_trace_params)
         await self._session._outgoing_attach(attach_frame) # pylint: disable=protected-access
 
     async def _incoming_attach(self, frame):
         if self.network_trace:
-            _LOGGER.info("<- %r", AttachFrame(*frame), extra=self.network_trace_params)
+            _LOGGER.debug("<- %r", AttachFrame(*frame), extra=self.network_trace_params)
         if self._is_closed:
             raise ValueError("Invalid link")
         if not frame[5] or not frame[6]:
-            _LOGGER.info("Cannot get source or target. Detaching link")
+            _LOGGER.info("Cannot get source or target. Detaching link", extra=self.network_trace_params)
             await self._set_state(LinkState.DETACHED)
             raise ValueError("Invalid link")
         self.remote_handle = frame[1]  # handle
         self.remote_max_message_size = frame[10]  # max_message_size
         self.offered_capabilities = frame[11]  # offered_capabilities
         if self.properties:
             self.properties.update(frame[13])  # properties
@@ -185,15 +185,15 @@
             try:
                 if frame[5]:
                     frame[5] = Source(*frame[5])
                 if frame[6]:
                     frame[6] = Target(*frame[6])
                 await self._on_attach(AttachFrame(*frame))
             except Exception as e:  # pylint: disable=broad-except
-                _LOGGER.warning("Callback for link attach raised error: %s", e)
+                _LOGGER.warning("Callback for link attach raised error: %s", e, extra=self.network_trace_params)
 
     async def _outgoing_flow(self, **kwargs):
         flow_frame = {
             "handle": self.handle,
             "delivery_count": self.delivery_count,
             "link_credit": self.current_link_credit,
             "available": kwargs.get("available"),
@@ -208,22 +208,22 @@
 
     async def _incoming_disposition(self, frame):
         pass
 
     async def _outgoing_detach(self, close=False, error=None):
         detach_frame = DetachFrame(handle=self.handle, closed=close, error=error)
         if self.network_trace:
-            _LOGGER.info("-> %r", detach_frame, extra=self.network_trace_params)
+            _LOGGER.debug("-> %r", detach_frame, extra=self.network_trace_params)
         await self._session._outgoing_detach(detach_frame) # pylint: disable=protected-access
         if close:
             self._is_closed = True
 
     async def _incoming_detach(self, frame):
         if self.network_trace:
-            _LOGGER.info("<- %r", DetachFrame(*frame), extra=self.network_trace_params)
+            _LOGGER.debug("<- %r", DetachFrame(*frame), extra=self.network_trace_params)
         if self.state == LinkState.ATTACHED:
             await self._outgoing_detach(close=frame[1])  # closed
         elif frame[1] and not self._is_closed and self.state in [LinkState.ATTACH_SENT, LinkState.ATTACH_RCVD]:
             # Received a closing detach after we sent a non-closing detach.
             # In this case, we MUST signal that we closed by reattaching and then sending a closing detach.
             await self._outgoing_attach()
             await self._outgoing_detach(close=True)
@@ -250,13 +250,13 @@
             if self.state in [LinkState.ATTACH_SENT, LinkState.ATTACH_RCVD]:
                 await self._outgoing_detach(close=close, error=error)
                 await self._set_state(LinkState.DETACHED)
             elif self.state == LinkState.ATTACHED:
                 await self._outgoing_detach(close=close, error=error)
                 await self._set_state(LinkState.DETACH_SENT)
         except Exception as exc:  # pylint: disable=broad-except
-            _LOGGER.info("An error occurred when detaching the link: %r", exc)
+            _LOGGER.info("An error occurred when detaching the link: %r", exc, extra=self.network_trace_params)
             await self._set_state(LinkState.DETACHED)
 
     async def flow(self, *, link_credit: Optional[int] = None, **kwargs) -> None:
         self.current_link_credit = link_credit if link_credit is not None else self.link_credit
         await self._outgoing_flow(**kwargs)
```

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_cbs_async.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_cbs_async.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # -------------------------------------------------------------------------
 
 import logging
 from datetime import datetime
+from typing import Optional
 
 from ..utils import utc_now, utc_from_timestamp
 from ._management_link_async import ManagementLink
 from ..message import Message, Properties
 from ..error import AuthenticationException, ErrorCondition, TokenAuthFailure, TokenExpired
 from ..constants import (
     CbsState,
@@ -45,23 +46,29 @@
         self._auth = auth
         self._encoding = 'UTF-8'
         self._auth_timeout = kwargs.get('auth_timeout')
         self._token_put_time = None
         self._expires_on = None
         self._token = None
         self._refresh_window = None
+        self._network_trace_params = {
+            "amqpConnection": self._session._connection._container_id,
+            "amqpSession": self._session.name,
+            "amqpLink": None
+        }
 
         self._token_status_code = None
         self._token_status_description = None
 
         self.state = CbsState.CLOSED
         self.auth_state = CbsAuthState.IDLE
 
-    async def _put_token(self, token, token_type, audience, expires_on=None):
-        # type: (str, str, str, datetime) -> None
+    async def _put_token(
+            self, token: str, token_type: str, audience: str, expires_on: Optional[datetime] = None
+    ) -> None:
         message = Message(  # type: ignore # TODO: missing positional args header, etc.
             value=token,
             properties=Properties(message_id=self._mgmt_link.next_message_id),  # type: ignore
             application_properties={
                 CBS_NAME: audience,
                 CBS_OPERATION: CBS_PUT_TOKEN,
                 CBS_TYPE: token_type,
@@ -75,58 +82,65 @@
             operation=CBS_PUT_TOKEN,
             type=token_type,
         )
         self._mgmt_link.next_message_id += 1
 
     async def _on_amqp_management_open_complete(self, management_open_result):
         if self.state in (CbsState.CLOSED, CbsState.ERROR):
-            _LOGGER.debug("CSB with status: %r encounters unexpected AMQP management open complete.", self.state)
+            _LOGGER.debug(
+                "CSB with status: %r encounters unexpected AMQP management open complete.",
+                self.state,
+                extra=self._network_trace_params
+            )
         elif self.state == CbsState.OPEN:
             self.state = CbsState.ERROR
             _LOGGER.info(
-                "Unexpected AMQP management open complete in OPEN, CBS error occurred on connection %r.",
-                self._connection._container_id,  # pylint:disable=protected-access
+                "Unexpected AMQP management open complete in OPEN, CBS error occurred.",
+                extra=self._network_trace_params
             )
         elif self.state == CbsState.OPENING:
             self.state = CbsState.OPEN if management_open_result == ManagementOpenResult.OK else CbsState.CLOSED
             _LOGGER.info(
-                "CBS for connection %r completed opening with status: %r",
-                self._connection._container_id, # pylint: disable=protected-access
+                "CBS completed opening with status: %r",
                 management_open_result,
-            )  # pylint:disable=protected-access
+                extra=self._network_trace_params
+            )
 
     async def _on_amqp_management_error(self):
         if self.state == CbsState.CLOSED:
-            _LOGGER.debug("Unexpected AMQP error in CLOSED state.")
+            _LOGGER.debug("Unexpected AMQP error in CLOSED state.", extra=self._network_trace_params)
         elif self.state == CbsState.OPENING:
             self.state = CbsState.ERROR
             await self._mgmt_link.close()
             _LOGGER.info(
-                "CBS for connection %r failed to open with status: %r",
-                self._connection._container_id,
+                "CBS failed to open with status: %r",
                 ManagementOpenResult.ERROR,
-            )  # pylint:disable=protected-access
+                extra=self._network_trace_params
+            )
         elif self.state == CbsState.OPEN:
             self.state = CbsState.ERROR
-            _LOGGER.info(
-                "CBS error occurred on connection %r.", self._connection._container_id
-            )  # pylint:disable=protected-access
+            _LOGGER.info("CBS error occurred.", extra=self._network_trace_params)
 
     async def _on_execute_operation_complete(
         self, execute_operation_result, status_code, status_description, _, error_condition=None
     ):
         if error_condition:
-            _LOGGER.info("CBS Put token error: %r", error_condition)
+            _LOGGER.info(
+                "CBS Put token error: %r",
+                error_condition,
+                extra=self._network_trace_params
+            )
             self.auth_state = CbsAuthState.ERROR
             return
-        _LOGGER.info(
+        _LOGGER.debug(
             "CBS Put token result (%r), status code: %s, status_description: %s.",
             execute_operation_result,
             status_code,
             status_description,
+            extra=self._network_trace_params
         )
         self._token_status_code = status_code
         self._token_status_description = status_description
 
         if execute_operation_result == ManagementExecuteOperationResult.OK:
             self.auth_state = CbsAuthState.OK
         elif execute_operation_result == ManagementExecuteOperationResult.ERROR:
@@ -135,63 +149,85 @@
             self._token_status_code = 0
             self._token_status_description = "Auth message has been rejected."
         elif execute_operation_result == ManagementExecuteOperationResult.FAILED_BAD_STATUS:
             self.auth_state = CbsAuthState.ERROR
 
     async def _update_status(self):
         if self.auth_state == CbsAuthState.OK or self.auth_state == CbsAuthState.REFRESH_REQUIRED:
-            _LOGGER.debug("update_status In refresh required or OK.")
             is_expired, is_refresh_required = check_expiration_and_refresh_status(
                 self._expires_on, self._refresh_window
             )  # pylint:disable=line-too-long
-            _LOGGER.debug("is expired == %r, is refresh required == %r", is_expired, is_refresh_required)
+            _LOGGER.debug(
+                "CBS status check: state == %r, expired == %r, refresh required == %r",
+                self.auth_state,
+                is_expired,
+                is_refresh_required,
+                extra=self._network_trace_params
+            )
             if is_expired:
                 self.auth_state = CbsAuthState.EXPIRED
             elif is_refresh_required:
                 self.auth_state = CbsAuthState.REFRESH_REQUIRED
         elif self.auth_state == CbsAuthState.IN_PROGRESS:
-            _LOGGER.debug("In update status, in progress. token put time: %r", self._token_put_time)
+            _LOGGER.debug(
+                "CBS update in progress. Token put time: %r",
+                self._token_put_time,
+                extra=self._network_trace_params
+            )
             put_timeout = check_put_timeout_status(self._auth_timeout, self._token_put_time)
             if put_timeout:
                 self.auth_state = CbsAuthState.TIMEOUT
 
     async def _cbs_link_ready(self):
         if self.state == CbsState.OPEN:
             return True
         if self.state != CbsState.OPEN:
             return False
         if self.state in (CbsState.CLOSED, CbsState.ERROR):
-            raise TokenAuthFailure( # pylint: disable = no-value-for-parameter
-                condition=ErrorCondition.ClientError,
-                description="CBS authentication link is in broken status, please recreate the cbs link.",
+            raise TokenAuthFailure(
+                status_code=ErrorCondition.ClientError,
+                status_description="CBS authentication link is in broken status, please recreate the cbs link.",
             )
 
     async def open(self):
         self.state = CbsState.OPENING
         await self._mgmt_link.open()
 
     async def close(self):
         await self._mgmt_link.close()
         self.state = CbsState.CLOSED
 
     async def update_token(self):
         self.auth_state = CbsAuthState.IN_PROGRESS
         access_token = await self._auth.get_token()
-        if not access_token.token:
-            _LOGGER.debug("update_token received an empty token")
+        if not access_token:
+            _LOGGER.info(
+                "Token refresh function received an empty token object.",
+                extra=self._network_trace_params
+            )
+        elif not access_token.token:
+            _LOGGER.info(
+                "Token refresh function received an empty token.",
+                extra=self._network_trace_params
+            )
         self._expires_on = access_token.expires_on
         expires_in = self._expires_on - int(utc_now().timestamp())
         self._refresh_window = int(float(expires_in) * 0.1)
         try:
             self._token = access_token.token.decode()
         except AttributeError:
             self._token = access_token.token
+        try:
+            token_type = self._auth.token_type.decode()
+        except AttributeError:
+            token_type = self._auth.token_type
+
         self._token_put_time = int(utc_now().timestamp())
         await self._put_token(
-            self._token, self._auth.token_type, self._auth.audience, utc_from_timestamp(self._expires_on)
+            self._token, token_type, self._auth.audience, utc_from_timestamp(self._expires_on)
         )
 
     async def handle_token(self):
         if not await self._cbs_link_ready():
             return False
         await self._update_status()
         if self.auth_state == CbsAuthState.IDLE:
@@ -199,16 +235,17 @@
             return False
         if self.auth_state == CbsAuthState.IN_PROGRESS:
             return False
         if self.auth_state == CbsAuthState.OK:
             return True
         if self.auth_state == CbsAuthState.REFRESH_REQUIRED:
             _LOGGER.info(
-                "Token on connection %r will expire soon - attempting to refresh.", self._connection._container_id
-            )  # pylint:disable=protected-access
+                "Token will expire soon - attempting to refresh.",
+                extra=self._network_trace_params
+            )
             await self.update_token()
             return False
         if self.auth_state == CbsAuthState.FAILURE:
             raise AuthenticationException(
                 condition=ErrorCondition.InternalError, description="Failed to open CBS authentication link."
             )
         if self.auth_state == CbsAuthState.ERROR:
```

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_transport_async.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_transport_async.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,31 +38,39 @@
 import ssl
 import struct
 from ssl import SSLError
 from io import BytesIO
 import logging
 
 
+
 import certifi
 
 from .._platform import KNOWN_TCP_OPTS, SOL_TCP
 from .._encode import encode_frame
 from .._decode import decode_frame, decode_empty_frame
-from ..constants import TLS_HEADER_FRAME, WEBSOCKET_PORT, AMQP_WS_SUBPROTOCOL
+from ..constants import (
+    DEFAULT_WEBSOCKET_HEARTBEAT_SECONDS,
+    TLS_HEADER_FRAME,
+    WEBSOCKET_PORT,
+    AMQP_WS_SUBPROTOCOL,
+    TIMEOUT_INTERVAL,
+    READ_TIMEOUT_INTERVAL,
+)
 from .._transport import (
     AMQP_FRAME,
     get_errno,
     to_host_port,
     DEFAULT_SOCKET_SETTINGS,
     SIGNED_INT_MAX,
     _UNAVAIL,
     set_cloexec,
     AMQP_PORT,
-    TIMEOUT_INTERVAL,
 )
+from ..error import AuthenticationException, ErrorCondition
 
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class AsyncTransportMixin:
     async def receive_frame(self, timeout=None, **kwargs):
@@ -70,15 +78,14 @@
             header, channel, payload = await asyncio.wait_for(
                 self.read(**kwargs), timeout=timeout
             )
             if not payload:
                 decoded = decode_empty_frame(header)
             else:
                 decoded = decode_frame(payload)
-            _LOGGER.info("ICH%d <- %r", channel, decoded)
             return channel, decoded
         except (
             TimeoutError,
             socket.timeout,
             asyncio.IncompleteReadError,
             asyncio.TimeoutError,
         ):
@@ -97,18 +104,23 @@
                 size = frame_header[0:4]
                 if size == AMQP_FRAME:  # Empty frame or AMQP header negotiation
                     return frame_header, channel, None
                 size = struct.unpack(">I", size)[0]
                 offset = frame_header[4]
                 frame_type = frame_header[5]
                 if verify_frame_type is not None and frame_type != verify_frame_type:
+                    _LOGGER.debug(
+                        "Received invalid frame type: %r, expected: %r",
+                        frame_type,
+                        verify_frame_type,
+                        extra=self.network_trace_params
+                    )
                     raise ValueError(
                         f"Received invalid frame type: {frame_type}, expected: {verify_frame_type}"
                     )
-
                 # >I is an unsigned int, but the argument to sock.recv is signed,
                 # so we know the size can be at most 2 * SIGNED_INT_MAX
                 payload_size = size - len(frame_header)
                 payload = memoryview(bytearray(payload_size))
                 if size > SIGNED_INT_MAX:
                     read_frame_buffer.write(
                         await self._read(SIGNED_INT_MAX, buffer=payload)
@@ -118,40 +130,58 @@
                             size - SIGNED_INT_MAX, buffer=payload[SIGNED_INT_MAX:]
                         )
                     )
                 else:
                     read_frame_buffer.write(
                         await self._read(payload_size, buffer=payload)
                     )
-            except (TimeoutError, socket.timeout, asyncio.IncompleteReadError):
+            except (
+                asyncio.CancelledError,
+                asyncio.TimeoutError,
+                TimeoutError,
+                socket.timeout,
+                asyncio.IncompleteReadError
+            ):
                 read_frame_buffer.write(self._read_buffer.getvalue())
                 self._read_buffer = read_frame_buffer
                 self._read_buffer.seek(0)
                 raise
             except (OSError, IOError, SSLError, socket.error) as exc:
                 # Don't disconnect for ssl read time outs
                 # http://bugs.python.org/issue10272
                 if isinstance(exc, SSLError) and "timed out" in str(exc):
                     raise socket.timeout()
                 if get_errno(exc) not in _UNAVAIL:
                     self.connected = False
+                _LOGGER.debug("Transport read failed: %r", exc, extra=self.network_trace_params)
                 raise
             offset -= 2
         return frame_header, channel, payload[offset:]
 
+    async def write(self, s):
+        async with self.socket_lock:
+            try:
+                await self._write(s)
+            except socket.timeout:
+                raise
+            except (OSError, IOError, socket.error) as exc:
+                _LOGGER.debug("Transport write failed: %r", exc, extra=self.network_trace_params)
+                if get_errno(exc) not in _UNAVAIL:
+                    self.connected = False
+                raise
+
     async def send_frame(self, channel, frame, **kwargs):
         header, performative = encode_frame(frame, **kwargs)
         if performative is None:
             data = header
         else:
             encoded_channel = struct.pack(">H", channel)
             data = header + encoded_channel + performative
 
         await self.write(data)
-        # _LOGGER.info("OCH%d -> %r", channel, frame)
 
     def _build_ssl_opts(self, sslopts):
         if sslopts in [True, False, None, {}]:
             return sslopts
         try:
             if "context" in sslopts:
                 return self._build_ssl_context(**sslopts.pop("context"))
@@ -172,14 +202,19 @@
                 keyfile = sslopts.get("keyfile")
                 context.verify_mode = cert_reqs
                 if cert_reqs != ssl.CERT_NONE:
                     context.check_hostname = True
                 if (certfile is not None) and (keyfile is not None):
                     context.load_cert_chain(certfile, keyfile)
                 return context
+            ca_certs = sslopts.get("ca_certs")
+            if ca_certs:
+                context = ssl.SSLContext(ssl_version)
+                context.load_verify_locations(ca_certs)
+                return context
             return True
         except TypeError:
             raise TypeError(
                 "SSL configuration must be a dictionary, or the value True."
             )
 
     def _build_ssl_context(
@@ -214,17 +249,17 @@
         self.writer = None
         self.raise_on_initial_eintr = raise_on_initial_eintr
         self._read_buffer = BytesIO()
         self.host, self.port = to_host_port(host, port)
 
         self.connect_timeout = connect_timeout
         self.socket_settings = socket_settings
-        self.loop = asyncio.get_running_loop()
         self.socket_lock = asyncio.Lock()
-        self.sslopts = self._build_ssl_opts(ssl_opts)
+        self.sslopts = ssl_opts
+        self.network_trace_params = kwargs.get('network_trace_params')
 
     async def connect(self):
         try:
             # are we already connected?
             if self.connected:
                 return
             await self._connect(self.host, self.port, self.connect_timeout)
@@ -234,15 +269,16 @@
                 ssl=self.sslopts,
                 server_hostname=self.host if self.sslopts else None,
             )
             # we've sent the banner; signal connect
             # EINTR, EAGAIN, EWOULDBLOCK would signal that the banner
             # has _not_ been sent
             self.connected = True
-        except (OSError, IOError, SSLError):
+        except (OSError, IOError, SSLError) as e:
+            _LOGGER.info("Transport connect failed: %r", e, extra=self.network_trace_params)
             # if not fully connected, close socket, and reraise error
             if self.sock and not self.connected:
                 self.sock.close()
                 self.sock = None
             raise
 
     async def _connect(self, host, port, timeout):
@@ -257,15 +293,15 @@
         # _connect call for extended time.
         e = None
         addr_types = (socket.AF_INET, socket.AF_INET6)
         addr_types_num = len(addr_types)
         for n, family in enumerate(addr_types):
             # first, resolve the address for a single address family
             try:
-                entries = await self.loop.getaddrinfo(
+                entries = await asyncio.get_event_loop().getaddrinfo(
                     host, port, family=family, type=socket.SOCK_STREAM, proto=SOL_TCP
                 )
                 entries_num = len(entries)
             except socket.gaierror:
                 # we may have depleted all our options
                 if n + 1 >= addr_types_num:
                     # if getaddrinfo succeeded before for another address
@@ -279,15 +315,15 @@
                 try:
                     self.sock = socket.socket(af, socktype, proto)
                     try:
                         set_cloexec(self.sock, True)
                     except NotImplementedError:
                         pass
                     self.sock.settimeout(timeout)
-                    await self.loop.sock_connect(self.sock, sa)
+                    await asyncio.get_event_loop().sock_connect(self.sock, sa)
                 except socket.error as ex:
                     e = ex
                     if self.sock is not None:
                         self.sock.close()
                         self.sock = None
                     # we may have depleted all our options
                     if i + 1 >= entries_num and n + 1 >= addr_types_num:
@@ -296,15 +332,26 @@
                     # hurray, we established connection
                     return
 
     def _init_socket(self, socket_settings):
         self.sock.settimeout(None)  # set socket back to blocking mode
         self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1)
         self._set_socket_options(socket_settings)
-        self.sock.settimeout(1)  # set socket back to non-blocking mode
+        try:
+            # Building ssl opts here instead of constructor, so that invalid cert error is raised
+            # when client is connecting, rather then during creation. For uamqp exception parity.
+            self.sslopts = self._build_ssl_opts(self.sslopts)
+        except FileNotFoundError as exc:
+            # FileNotFoundError does not have missing filename info, so adding it below.
+            # Assuming that this must be ca_certs, since this is the only file path that
+            # users can pass in (`connection_verify` in the EH/SB clients) through sslopts above.
+            # For uamqp exception parity. Remove later when resolving issue #27128.
+            exc.filename = self.sslopts
+            raise exc
+        self.sock.settimeout(READ_TIMEOUT_INTERVAL)  # set socket back to non-blocking mode
 
     def _get_tcp_socket_defaults(self, sock):  # pylint: disable=no-self-use
         tcp_opts = {}
         for opt in KNOWN_TCP_OPTS:
             enum = None
             if opt == "TCP_USER_TIMEOUT":
                 try:
@@ -347,14 +394,18 @@
         try:
             while toread:
                 try:
                     view[nbytes : nbytes + toread] = await self.reader.readexactly(
                         toread
                     )
                     nbytes = toread
+                except AttributeError:
+                    # This means that close() was called concurrently
+                    # self.reader has been set to None.
+                    raise IOError("Connection has already been closed")
                 except asyncio.IncompleteReadError as exc:
                     pbytes = len(exc.partial)
                     view[nbytes : nbytes + pbytes] = exc.partial
                     nbytes = pbytes
                 except socket.error as exc:
                     # ssl.sock.read may cause a SSLerror without errno
                     # http://bugs.python.org/issue10272
@@ -375,48 +426,38 @@
         except:  # noqa
             self._read_buffer = BytesIO(view[:length])
             raise
         return view
 
     async def _write(self, s):
         """Write a string out to the SSL socket fully."""
-        self.writer.write(s)
+        try:
+            self.writer.write(s)
+            await self.writer.drain()
+        except AttributeError:
+            raise IOError("Connection has already been closed")
 
     async def close(self):
-        if self.writer is not None:
-            if self.sslopts:
-                # see issue: https://github.com/encode/httpx/issues/914
-                self.writer.transport.abort()
-            self.writer.close()
+        async with self.socket_lock:
+            try:
+                if self.writer is not None:
+                    # Closing the writer closes the underlying socket.
+                    self.writer.close()
+                    if self.sslopts:
+                        # see issue: https://github.com/encode/httpx/issues/914
+                        await asyncio.sleep(0)
+                        self.writer.transport.abort()
+                    await self.writer.wait_closed()
+            except Exception as e:  # pylint: disable=broad-except
+                # Sometimes SSL raises APPLICATION_DATA_AFTER_CLOSE_NOTIFY here on close.
+                _LOGGER.debug("Error shutting down socket: %r", e, extra=self.network_trace_params)
             self.writer, self.reader = None, None
         self.sock = None
         self.connected = False
 
-    async def write(self, s):
-        try:
-            await self._write(s)
-        except socket.timeout:
-            raise
-        except (OSError, IOError, socket.error) as exc:
-            if get_errno(exc) not in _UNAVAIL:
-                self.connected = False
-            raise
-
-    async def receive_frame_with_lock(self, **kwargs):
-        try:
-            async with self.socket_lock:
-                header, channel, payload = await self.read(**kwargs)
-            if not payload:
-                decoded = decode_empty_frame(header)
-            else:
-                decoded = decode_frame(payload)
-            return channel, decoded
-        except (socket.timeout, TimeoutError):
-            return None, None
-
     async def negotiate(self):
         if not self.sslopts:
             return
         await self.write(TLS_HEADER_FRAME)
         _, returned_header = await self.receive_frame(verify_frame_type=None)
         if returned_header[1] == TLS_HEADER_FRAME:
             raise ValueError(
@@ -435,98 +476,120 @@
         port=WEBSOCKET_PORT,
         connect_timeout=None,
         ssl_opts=None,
         **kwargs
     ):
         self._read_buffer = BytesIO()
         self.socket_lock = asyncio.Lock()
-        self.sslopts = self._build_ssl_opts(ssl_opts) if isinstance(ssl_opts, dict) else None
+        self.sslopts = ssl_opts if isinstance(ssl_opts, dict) else None
         self._connect_timeout = connect_timeout or TIMEOUT_INTERVAL
         self._custom_endpoint = kwargs.get("custom_endpoint")
         self.host, self.port = to_host_port(host, port)
         self.ws = None
         self.session = None
         self._http_proxy = kwargs.get("http_proxy", None)
         self.connected = False
+        self.network_trace_params = kwargs.get('network_trace_params')
 
     async def connect(self):
+        self.sslopts = self._build_ssl_opts(self.sslopts)
         username, password = None, None
         http_proxy_host, http_proxy_port = None, None
         http_proxy_auth = None
 
         if self._http_proxy:
             http_proxy_host = self._http_proxy["proxy_hostname"]
             http_proxy_port = self._http_proxy["proxy_port"]
             if http_proxy_host and http_proxy_port:
                 http_proxy_host = f"{http_proxy_host}:{http_proxy_port}"
             username = self._http_proxy.get("username", None)
             password = self._http_proxy.get("password", None)
 
         try:
-            from aiohttp import ClientSession
+            from aiohttp import ClientSession, ClientConnectorError
             from urllib.parse import urlsplit
+        except ImportError:
+            raise ImportError(
+                "Please install aiohttp library to use async websocket transport."
+            )
 
-            if username or password:
-                from aiohttp import BasicAuth
+        if username or password:
+            from aiohttp import BasicAuth
 
-                http_proxy_auth = BasicAuth(login=username, password=password)
+            http_proxy_auth = BasicAuth(login=username, password=password)
 
-            self.session = ClientSession()
-            if self._custom_endpoint:
-                url = f"wss://{self._custom_endpoint}"
-            else:
-                url = f"wss://{self.host}"
-                parsed_url = urlsplit(url)
-                url = f"{parsed_url.scheme}://{parsed_url.netloc}:{self.port}{parsed_url.path}"
+        self.session = ClientSession()
+        if self._custom_endpoint:
+            url = f"wss://{self._custom_endpoint}"
+        else:
+            url = f"wss://{self.host}"
+            parsed_url = urlsplit(url)
+            url = f"{parsed_url.scheme}://{parsed_url.netloc}:{self.port}{parsed_url.path}"
+
+        try:
+            # Enabling heartbeat that sends a ping message every n seconds and waits for pong response.
+            # if pong response is not received then close connection. This raises an error when trying
+            # to communicate with the websocket which is no longer active.
+            # We are waiting a bug fix in aiohttp for these 2 bugs where aiohttp ws might hang on network disconnect
+            # and the heartbeat mechanism helps mitigate these two.
+            # https://github.com/aio-libs/aiohttp/pull/5860
+            # https://github.com/aio-libs/aiohttp/issues/2309
 
             self.ws = await self.session.ws_connect(
                 url=url,
                 timeout=self._connect_timeout,
                 protocols=[AMQP_WS_SUBPROTOCOL],
                 autoclose=False,
                 proxy=http_proxy_host,
                 proxy_auth=http_proxy_auth,
                 ssl=self.sslopts,
+                heartbeat=DEFAULT_WEBSOCKET_HEARTBEAT_SECONDS,
             )
-            self.connected = True
-
-        except ImportError:
-            raise ValueError(
-                "Please install aiohttp library to use websocket transport."
-            )
+        except ClientConnectorError as exc:
+            _LOGGER.info("Websocket connect failed: %r", exc, extra=self.network_trace_params)
+            if self._custom_endpoint:
+                raise AuthenticationException(
+                    ErrorCondition.ClientError,
+                    description="Failed to authenticate the connection due to exception: " + str(exc),
+                    error=exc,
+                )
+            raise ConnectionError("Failed to establish websocket connection: " + str(exc))
+        self.connected = True
 
-    async def _read(self, n, buffer=None, **kwargs):  # pylint: disable=unused-argument
+    async def _read(self, toread, buffer=None, **kwargs):  # pylint: disable=unused-argument
         """Read exactly n bytes from the peer."""
-
         length = 0
-        view = buffer or memoryview(bytearray(n))
+        view = buffer or memoryview(bytearray(toread))
         nbytes = self._read_buffer.readinto(view)
         length += nbytes
-        n -= nbytes
-
+        toread -= nbytes
         try:
-            while n:
+            while toread:
                 data = await self.ws.receive_bytes()
-                if len(data) <= n:
-                    view[length : length + len(data)] = data
-                    n -= len(data)
+                read_length = len(data)
+                if read_length <= toread:
+                    view[length : length + read_length] = data
+                    toread -= read_length
+                    length += read_length
                 else:
-                    view[length : length + n] = data[0:n]
-                    self._read_buffer = BytesIO(data[n:])
-                    n = 0
+                    view[length : length + toread] = data[0:toread]
+                    self._read_buffer = BytesIO(data[toread:])
+                    toread = 0
             return view
-        except asyncio.TimeoutError:
-            raise TimeoutError()
+        except:
+            self._read_buffer = BytesIO(view[:length])
+            raise
 
     async def close(self):
         """Do any preliminary work in shutting down the connection."""
-        await self.ws.close()
-        await self.session.close()
-        self.connected = False
+        async with self.socket_lock:
+            await self.ws.close()
+            await self.session.close()
+            self.connected = False
 
-    async def write(self, s):
+    async def _write(self, s):
         """Completely write a string (byte array) to the peer.
         ABNF, OPCODE_BINARY = 0x2
         See http://tools.ietf.org/html/rfc5234
         http://tools.ietf.org/html/rfc6455#section-5.2
         """
         await self.ws.send_bytes(s)
```

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_receiver_async.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/receiver.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,22 +4,19 @@
 # license information.
 # --------------------------------------------------------------------------
 
 import uuid
 import logging
 from typing import Optional, Union
 
-from .._decode import decode_payload
-from ._link_async import Link
-from ..constants import LinkState, Role
-from ..performatives import (
-    TransferFrame,
-    DispositionFrame,
-)
-from ..outcomes import Received, Accepted, Rejected, Released, Modified
+from ._decode import decode_payload
+from .link import Link
+from .constants import LinkState, Role
+from .performatives import TransferFrame, DispositionFrame
+from .outcomes import Received, Accepted, Rejected, Released, Modified
 
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class ReceiverLink(Link):
     def __init__(self, session, handle, source_address, **kwargs):
@@ -33,94 +30,92 @@
 
     @classmethod
     def from_incoming_frame(cls, session, handle, frame):
         # TODO: Assuming we establish all links for now...
         # check link_create_from_endpoint in C lib
         raise NotImplementedError("Pending")
 
-    async def _process_incoming_message(self, frame, message):
+    def _process_incoming_message(self, frame, message):
         try:
-            return await self._on_transfer(frame, message)
+            return self._on_transfer(frame, message)
         except Exception as e:  # pylint: disable=broad-except
-            _LOGGER.error("Handler function failed with error: %r", e)
+            _LOGGER.error("Transfer callback function failed with error: %r", e, extra=self.network_trace_params)
         return None
 
-    async def _incoming_attach(self, frame):
-        await super(ReceiverLink, self)._incoming_attach(frame)
+    def _incoming_attach(self, frame):
+        super(ReceiverLink, self)._incoming_attach(frame)
         if frame[9] is None:  # initial_delivery_count
-            _LOGGER.info("Cannot get initial-delivery-count. Detaching link")
-            await self._set_state(LinkState.DETACHED)  # TODO: Send detach now?
+            _LOGGER.info("Cannot get initial-delivery-count. Detaching link", extra=self.network_trace_params)
+            self._set_state(LinkState.DETACHED)  # TODO: Send detach now?
         self.delivery_count = frame[9]
         self.current_link_credit = self.link_credit
-        await self._outgoing_flow()
+        self._outgoing_flow()
 
-    async def _incoming_transfer(self, frame):
+    def _incoming_transfer(self, frame):
         if self.network_trace:
-            _LOGGER.info("<- %r", TransferFrame(*frame), extra=self.network_trace_params)
+            _LOGGER.debug("<- %r", TransferFrame(payload=b"***", *frame[:-1]), extra=self.network_trace_params)
         self.current_link_credit -= 1
         self.delivery_count += 1
         self.received_delivery_id = frame[1]  # delivery_id
         if not self.received_delivery_id and not self._received_payload:
             pass  # TODO: delivery error
         if self._received_payload or frame[5]:  # more
             self._received_payload.extend(frame[11])
         if not frame[5]:
             if self._received_payload:
                 message = decode_payload(memoryview(self._received_payload))
                 self._received_payload = bytearray()
             else:
                 message = decode_payload(frame[11])
-                if self.network_trace:
-                    _LOGGER.info("   %r", message, extra=self.network_trace_params)
-            delivery_state = await self._process_incoming_message(frame, message)
+            delivery_state = self._process_incoming_message(frame, message)
             if not frame[4] and delivery_state:  # settled
-                await self._outgoing_disposition(
+                self._outgoing_disposition(
                     first=frame[1],
                     last=frame[1],
                     settled=True,
                     state=delivery_state,
                     batchable=None
                 )
 
-    async def _wait_for_response(self, wait: Union[bool, float]) -> None:
+    def _wait_for_response(self, wait: Union[bool, float]) -> None:
         if wait is True:
-            await self._session._connection.listen(wait=False) # pylint: disable=protected-access
+            self._session._connection.listen(wait=False) # pylint: disable=protected-access
             if self.state == LinkState.ERROR:
                 raise self._error
         elif wait:
-            await self._session._connection.listen(wait=wait) # pylint: disable=protected-access
+            self._session._connection.listen(wait=wait) # pylint: disable=protected-access
             if self.state == LinkState.ERROR:
                 raise self._error
 
-    async def _outgoing_disposition(
+    def _outgoing_disposition(
         self,
         first: int,
         last: Optional[int],
         settled: Optional[bool],
         state: Optional[Union[Received, Accepted, Rejected, Released, Modified]],
         batchable: Optional[bool],
     ):
         disposition_frame = DispositionFrame(
             role=self.role, first=first, last=last, settled=settled, state=state, batchable=batchable
         )
         if self.network_trace:
-            _LOGGER.info("-> %r", DispositionFrame(*disposition_frame), extra=self.network_trace_params)
-        await self._session._outgoing_disposition(disposition_frame) # pylint: disable=protected-access
+            _LOGGER.debug("-> %r", DispositionFrame(*disposition_frame), extra=self.network_trace_params)
+        self._session._outgoing_disposition(disposition_frame) # pylint: disable=protected-access
 
-    async def attach(self):
-        await super().attach()
+    def attach(self):
+        super().attach()
         self._received_payload = bytearray()
 
-    async def send_disposition(
+    def send_disposition(
         self,
         *,
         wait: Union[bool, float] = False,
         first_delivery_id: int,
         last_delivery_id: Optional[int] = None,
         settled: Optional[bool] = None,
         delivery_state: Optional[Union[Received, Accepted, Rejected, Released, Modified]] = None,
         batchable: Optional[bool] = None
     ):
         if self._is_closed:
             raise ValueError("Link already closed.")
-        await self._outgoing_disposition(first_delivery_id, last_delivery_id, settled, delivery_state, batchable)
-        await self._wait_for_response(wait)
+        self._outgoing_disposition(first_delivery_id, last_delivery_id, settled, delivery_state, batchable)
+        self._wait_for_response(wait)
```

## Comparing `azure-servicebus-7.9.0a1/azure/servicebus/_pyamqp/aio/_management_operation_async.py` & `azure-servicebus-7.9.0b1/azure/servicebus/_pyamqp/aio/_management_operation_async.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,19 @@
 
 class ManagementOperation(object):
     def __init__(self, session, endpoint='$management', **kwargs):
         self._mgmt_link_open_status = None
 
         self._session = session
         self._connection = self._session._connection
+        self._network_trace_params = {
+            "amqpConnection": self._session._connection._container_id,
+            "amqpSession": self._session.name,
+            "amqpLink": None
+        }
         self._mgmt_link = self._session.create_request_response_link_pair(
             endpoint=endpoint,
             on_amqp_management_open_complete=self._on_amqp_management_open_complete,
             on_amqp_management_error=self._on_amqp_management_error,
             **kwargs
         )  # type: ManagementLink
         self._responses = {}
@@ -57,30 +62,30 @@
         operation_result,
         status_code,
         status_description,
         raw_message,
         error=None
     ):
         _LOGGER.debug(
-            "mgmt operation completed, operation id: %r; operation_result: %r; status_code: %r; "
-            "status_description: %r, raw_message: %r, error: %r",
+            "Management operation completed, id: %r; result: %r; code: %r; description: %r, error: %r",
             operation_id,
             operation_result,
             status_code,
             status_description,
-            raw_message,
-            error
+            error,
+            extra=self._network_trace_params
         )
 
         if operation_result in\
                 (ManagementExecuteOperationResult.ERROR, ManagementExecuteOperationResult.LINK_CLOSED):
             self._mgmt_error = error
             _LOGGER.error(
-                "Failed to complete mgmt operation due to error: %r. The management request message is: %r",
-                error, raw_message
+                "Failed to complete management operation due to error: %r.",
+                error,
+                extra=self._network_trace_params
             )
         else:
             self._responses[operation_id] = (status_code, status_description, raw_message)
 
     async def execute(self, message, operation=None, operation_type=None, timeout=0):
         start_time = time.time()
         operation_id = str(uuid.uuid4())
```

