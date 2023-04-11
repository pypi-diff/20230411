# Comparing `tmp/semantic_kernel-0.2.0.dev0.tar.gz` & `tmp/semantic_kernel-0.2.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_kernel-0.2.0.dev0.tar", max compression
+gzip compressed data, was "semantic_kernel-0.2.1.dev0.tar", max compression
```

## Comparing `semantic_kernel-0.2.0.dev0.tar` & `semantic_kernel-0.2.1.dev0.tar`

### file list

```diff
@@ -1,87 +1,90 @@
--rw-r--r--   0        0        0      632 2023-04-10 18:26:09.498820 semantic_kernel-0.2.0.dev0/pyproject.toml
--rw-r--r--   0        0        0     3551 2023-04-10 18:26:09.496820 semantic_kernel-0.2.0.dev0/README.md
--rw-r--r--   0        0        0     1571 2023-04-06 23:28:27.130010 semantic_kernel-0.2.0.dev0/semantic_kernel/__init__.py
--rw-r--r--   0        0        0     1647 2023-04-06 23:28:27.130010 semantic_kernel-0.2.0.dev0/semantic_kernel/ai/ai_exception.py
--rw-r--r--   0        0        0      495 2023-04-06 23:28:27.131011 semantic_kernel-0.2.0.dev0/semantic_kernel/ai/chat_completion_client_base.py
--rw-r--r--   0        0        0     1129 2023-04-06 23:28:27.131011 semantic_kernel-0.2.0.dev0/semantic_kernel/ai/chat_request_settings.py
--rw-r--r--   0        0        0     1332 2023-04-06 23:28:27.131011 semantic_kernel-0.2.0.dev0/semantic_kernel/ai/complete_request_settings.py
--rw-r--r--   0        0        0      282 2023-04-06 23:28:27.132012 semantic_kernel-0.2.0.dev0/semantic_kernel/ai/embeddings/embedding_generator_base.py
--rw-r--r--   0        0        0      479 2023-04-06 23:28:27.132012 semantic_kernel-0.2.0.dev0/semantic_kernel/ai/embeddings/embedding_index_base.py
--rw-r--r--   0        0        0      817 2023-04-06 23:28:27.133010 semantic_kernel-0.2.0.dev0/semantic_kernel/ai/open_ai/__init__.py
--rw-r--r--   0        0        0     2771 2023-04-07 20:20:53.481793 semantic_kernel-0.2.0.dev0/semantic_kernel/ai/open_ai/services/azure_chat_completion.py
--rw-r--r--   0        0        0     2763 2023-04-07 20:20:53.481793 semantic_kernel-0.2.0.dev0/semantic_kernel/ai/open_ai/services/azure_text_completion.py
--rw-r--r--   0        0        0     2758 2023-04-07 20:20:53.481793 semantic_kernel-0.2.0.dev0/semantic_kernel/ai/open_ai/services/azure_text_embedding.py
--rw-r--r--   0        0        0     4007 2023-04-07 20:20:53.483403 semantic_kernel-0.2.0.dev0/semantic_kernel/ai/open_ai/services/open_ai_chat_completion.py
--rw-r--r--   0        0        0     4441 2023-04-07 20:20:53.484320 semantic_kernel-0.2.0.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_completion.py
--rw-r--r--   0        0        0     2427 2023-04-07 20:20:53.485320 semantic_kernel-0.2.0.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_embedding.py
--rw-r--r--   0        0        0      476 2023-04-06 23:28:27.135522 semantic_kernel-0.2.0.dev0/semantic_kernel/ai/text_completion_client_base.py
--rw-r--r--   0        0        0      383 2023-04-06 23:28:27.136521 semantic_kernel-0.2.0.dev0/semantic_kernel/core_skills/__init__.py
--rw-r--r--   0        0        0     2072 2023-04-07 23:02:47.633613 semantic_kernel-0.2.0.dev0/semantic_kernel/core_skills/file_io_skill.py
--rw-r--r--   0        0        0     4641 2023-04-06 23:28:27.137521 semantic_kernel-0.2.0.dev0/semantic_kernel/core_skills/text_memory_skill.py
--rw-r--r--   0        0        0     2403 2023-04-06 23:28:27.137521 semantic_kernel-0.2.0.dev0/semantic_kernel/core_skills/text_skill.py
--rw-r--r--   0        0        0     5613 2023-04-06 23:28:27.138525 semantic_kernel-0.2.0.dev0/semantic_kernel/core_skills/time_skill.py
--rw-r--r--   0        0        0    10609 2023-04-06 23:28:27.138525 semantic_kernel-0.2.0.dev0/semantic_kernel/kernel.py
--rw-r--r--   0        0        0     2342 2023-04-06 23:28:27.139523 semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_base.py
--rw-r--r--   0        0        0     3097 2023-04-06 23:28:27.139523 semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_builder.py
--rw-r--r--   0        0        0     9134 2023-04-10 18:26:09.500824 semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_config.py
--rw-r--r--   0        0        0     1626 2023-04-06 23:28:27.140524 semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_exception.py
--rw-r--r--   0        0        0      710 2023-04-06 23:28:27.141523 semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_extensions/__init__.py
--rw-r--r--   0        0        0      210 2023-04-06 23:28:27.141523 semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_extensions/extends_kernel.py
--rw-r--r--   0        0        0     2374 2023-04-06 23:28:27.141523 semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_extensions/import_skills.py
--rw-r--r--   0        0        0     2323 2023-04-06 23:28:27.142522 semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_extensions/inline_definition.py
--rw-r--r--   0        0        0     1531 2023-04-06 23:28:27.142522 semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_extensions/memory_configuration.py
--rw-r--r--   0        0        0      160 2023-04-06 23:28:27.143521 semantic_kernel-0.2.0.dev0/semantic_kernel/memory/__init__.py
--rw-r--r--   0        0        0     1174 2023-04-06 23:28:27.143521 semantic_kernel-0.2.0.dev0/semantic_kernel/memory/memory_query_result.py
--rw-r--r--   0        0        0     1598 2023-04-06 23:28:27.143521 semantic_kernel-0.2.0.dev0/semantic_kernel/memory/memory_record.py
--rw-r--r--   0        0        0      299 2023-04-06 23:28:27.144521 semantic_kernel-0.2.0.dev0/semantic_kernel/memory/memory_store_base.py
--rw-r--r--   0        0        0     1137 2023-04-06 23:28:27.144521 semantic_kernel-0.2.0.dev0/semantic_kernel/memory/null_memory.py
--rw-r--r--   0        0        0     2499 2023-04-06 23:28:27.144521 semantic_kernel-0.2.0.dev0/semantic_kernel/memory/semantic_text_memory.py
--rw-r--r--   0        0        0     1237 2023-04-06 23:28:27.145522 semantic_kernel-0.2.0.dev0/semantic_kernel/memory/semantic_text_memory_base.py
--rw-r--r--   0        0        0      836 2023-04-06 23:28:27.145522 semantic_kernel-0.2.0.dev0/semantic_kernel/memory/storage/data_entry.py
--rw-r--r--   0        0        0      953 2023-04-06 23:28:27.145522 semantic_kernel-0.2.0.dev0/semantic_kernel/memory/storage/data_store_base.py
--rw-r--r--   0        0        0     1989 2023-04-06 23:28:27.145522 semantic_kernel-0.2.0.dev0/semantic_kernel/memory/storage/volatile_data_store.py
--rw-r--r--   0        0        0     4050 2023-04-06 23:28:27.146521 semantic_kernel-0.2.0.dev0/semantic_kernel/memory/volatile_memory_store.py
--rw-r--r--   0        0        0     2328 2023-04-06 23:28:27.146521 semantic_kernel-0.2.0.dev0/semantic_kernel/orchestration/context_variables.py
--rw-r--r--   0        0        0     5079 2023-04-06 23:28:27.146521 semantic_kernel-0.2.0.dev0/semantic_kernel/orchestration/delegate_handlers.py
--rw-r--r--   0        0        0     8966 2023-04-06 23:28:27.147521 semantic_kernel-0.2.0.dev0/semantic_kernel/orchestration/delegate_inference.py
--rw-r--r--   0        0        0      638 2023-04-06 23:28:27.147521 semantic_kernel-0.2.0.dev0/semantic_kernel/orchestration/delegate_types.py
--rw-r--r--   0        0        0     7322 2023-04-06 23:28:27.147521 semantic_kernel-0.2.0.dev0/semantic_kernel/orchestration/sk_context.py
--rw-r--r--   0        0        0    16307 2023-04-10 18:26:09.500824 semantic_kernel-0.2.0.dev0/semantic_kernel/orchestration/sk_function.py
--rw-r--r--   0        0        0     6960 2023-04-10 18:26:09.501831 semantic_kernel-0.2.0.dev0/semantic_kernel/orchestration/sk_function_base.py
--rw-r--r--   0        0        0      919 2023-04-06 23:28:27.149523 semantic_kernel-0.2.0.dev0/semantic_kernel/reliability/pass_through_without_retry.py
--rw-r--r--   0        0        0      673 2023-04-06 23:28:27.149523 semantic_kernel-0.2.0.dev0/semantic_kernel/reliability/retry_mechanism.py
--rw-r--r--   0        0        0     2101 2023-04-06 23:28:27.150523 semantic_kernel-0.2.0.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
--rw-r--r--   0        0        0     2332 2023-04-06 23:28:27.150523 semantic_kernel-0.2.0.dev0/semantic_kernel/semantic_functions/prompt_template.py
--rw-r--r--   0        0        0      506 2023-04-06 23:28:27.151524 semantic_kernel-0.2.0.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
--rw-r--r--   0        0        0     3437 2023-04-06 23:28:27.151524 semantic_kernel-0.2.0.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
--rw-r--r--   0        0        0      671 2023-04-06 23:28:27.152522 semantic_kernel-0.2.0.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
--rw-r--r--   0        0        0      322 2023-04-06 23:28:27.152522 semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/__init__.py
--rw-r--r--   0        0        0     2053 2023-04-06 23:28:27.153521 semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/function_view.py
--rw-r--r--   0        0        0     1717 2023-04-06 23:28:27.154523 semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/functions_view.py
--rw-r--r--   0        0        0     1026 2023-04-06 23:28:27.154523 semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/parameter_view.py
--rw-r--r--   0        0        0     2104 2023-04-06 23:28:27.155525 semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
--rw-r--r--   0        0        0     1345 2023-04-06 23:28:27.155525 semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
--rw-r--r--   0        0        0      858 2023-04-06 23:28:27.156525 semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
--rw-r--r--   0        0        0      837 2023-04-06 23:28:27.156525 semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
--rw-r--r--   0        0        0     6056 2023-04-06 23:28:27.156525 semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/skill_collection.py
--rw-r--r--   0        0        0      803 2023-04-06 23:28:27.157522 semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/skill_collection_base.py
--rw-r--r--   0        0        0      830 2023-04-06 23:28:27.158522 semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/blocks/block.py
--rw-r--r--   0        0        0      228 2023-04-06 23:28:27.158522 semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/blocks/block_types.py
--rw-r--r--   0        0        0     4566 2023-04-10 18:26:09.501831 semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/blocks/code_block.py
--rw-r--r--   0        0        0     2653 2023-04-06 23:28:27.159522 semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
--rw-r--r--   0        0        0      276 2023-04-06 23:28:27.160524 semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/blocks/symbols.py
--rw-r--r--   0        0        0     1534 2023-04-06 23:28:27.160524 semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/blocks/text_block.py
--rw-r--r--   0        0        0     2274 2023-04-06 23:28:27.160524 semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/blocks/val_block.py
--rw-r--r--   0        0        0     2517 2023-04-06 23:28:27.161522 semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/blocks/var_block.py
--rw-r--r--   0        0        0     6535 2023-04-06 23:28:27.161522 semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/code_tokenizer.py
--rw-r--r--   0        0        0     6051 2023-04-06 23:28:27.162539 semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/prompt_template_engine.py
--rw-r--r--   0        0        0      532 2023-04-06 23:28:27.162539 semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
--rw-r--r--   0        0        0     3043 2023-04-06 23:28:27.163522 semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
--rw-r--r--   0        0        0      596 2023-04-06 23:28:27.163522 semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
--rw-r--r--   0        0        0     1115 2023-04-06 23:28:27.157522 semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/README.md
--rw-r--r--   0        0        0     7637 2023-04-06 23:28:27.164523 semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/template_tokenizer.py
--rw-r--r--   0        0        0      403 2023-04-06 23:28:27.164523 semantic_kernel-0.2.0.dev0/semantic_kernel/utils/null_logger.py
--rw-r--r--   0        0        0     2436 2023-04-06 23:28:27.165522 semantic_kernel-0.2.0.dev0/semantic_kernel/utils/settings.py
--rw-r--r--   0        0        0      221 2023-04-06 23:28:27.165522 semantic_kernel-0.2.0.dev0/semantic_kernel/utils/static_property.py
--rw-r--r--   0        0        0     2198 2023-04-06 23:28:27.165522 semantic_kernel-0.2.0.dev0/semantic_kernel/utils/validation.py
--rw-r--r--   0        0        0     4165 1970-01-01 00:00:00.000000 semantic_kernel-0.2.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1141 2023-04-10 22:00:30.797159 semantic_kernel-0.2.1.dev0/LICENSE
+-rw-r--r--   0        0        0      648 2023-04-11 19:26:46.128090 semantic_kernel-0.2.1.dev0/pyproject.toml
+-rw-r--r--   0        0        0     3551 2023-04-11 02:19:27.283435 semantic_kernel-0.2.1.dev0/README.md
+-rw-r--r--   0        0        0     1571 2023-04-06 23:28:27.130010 semantic_kernel-0.2.1.dev0/semantic_kernel/__init__.py
+-rw-r--r--   0        0        0     1647 2023-04-06 23:28:27.130010 semantic_kernel-0.2.1.dev0/semantic_kernel/ai/ai_exception.py
+-rw-r--r--   0        0        0      495 2023-04-06 23:28:27.131011 semantic_kernel-0.2.1.dev0/semantic_kernel/ai/chat_completion_client_base.py
+-rw-r--r--   0        0        0     1129 2023-04-06 23:28:27.131011 semantic_kernel-0.2.1.dev0/semantic_kernel/ai/chat_request_settings.py
+-rw-r--r--   0        0        0     1332 2023-04-06 23:28:27.131011 semantic_kernel-0.2.1.dev0/semantic_kernel/ai/complete_request_settings.py
+-rw-r--r--   0        0        0      282 2023-04-06 23:28:27.132012 semantic_kernel-0.2.1.dev0/semantic_kernel/ai/embeddings/embedding_generator_base.py
+-rw-r--r--   0        0        0      479 2023-04-06 23:28:27.132012 semantic_kernel-0.2.1.dev0/semantic_kernel/ai/embeddings/embedding_index_base.py
+-rw-r--r--   0        0        0      817 2023-04-06 23:28:27.133010 semantic_kernel-0.2.1.dev0/semantic_kernel/ai/open_ai/__init__.py
+-rw-r--r--   0        0        0     2771 2023-04-07 20:20:53.481793 semantic_kernel-0.2.1.dev0/semantic_kernel/ai/open_ai/services/azure_chat_completion.py
+-rw-r--r--   0        0        0     2763 2023-04-07 20:20:53.481793 semantic_kernel-0.2.1.dev0/semantic_kernel/ai/open_ai/services/azure_text_completion.py
+-rw-r--r--   0        0        0     2758 2023-04-07 20:20:53.481793 semantic_kernel-0.2.1.dev0/semantic_kernel/ai/open_ai/services/azure_text_embedding.py
+-rw-r--r--   0        0        0     4007 2023-04-07 20:20:53.483403 semantic_kernel-0.2.1.dev0/semantic_kernel/ai/open_ai/services/open_ai_chat_completion.py
+-rw-r--r--   0        0        0     4441 2023-04-07 20:20:53.484320 semantic_kernel-0.2.1.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_completion.py
+-rw-r--r--   0        0        0     2427 2023-04-07 20:20:53.485320 semantic_kernel-0.2.1.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_embedding.py
+-rw-r--r--   0        0        0      476 2023-04-06 23:28:27.135522 semantic_kernel-0.2.1.dev0/semantic_kernel/ai/text_completion_client_base.py
+-rw-r--r--   0        0        0      383 2023-04-06 23:28:27.136521 semantic_kernel-0.2.1.dev0/semantic_kernel/core_skills/__init__.py
+-rw-r--r--   0        0        0     2436 2023-04-10 22:52:46.084150 semantic_kernel-0.2.1.dev0/semantic_kernel/core_skills/constants.py
+-rw-r--r--   0        0        0     5134 2023-04-11 02:19:27.284441 semantic_kernel-0.2.1.dev0/semantic_kernel/core_skills/conversation_summary_skill.py
+-rw-r--r--   0        0        0     2072 2023-04-07 23:02:47.633613 semantic_kernel-0.2.1.dev0/semantic_kernel/core_skills/file_io_skill.py
+-rw-r--r--   0        0        0     4641 2023-04-06 23:28:27.137521 semantic_kernel-0.2.1.dev0/semantic_kernel/core_skills/text_memory_skill.py
+-rw-r--r--   0        0        0     2403 2023-04-06 23:28:27.137521 semantic_kernel-0.2.1.dev0/semantic_kernel/core_skills/text_skill.py
+-rw-r--r--   0        0        0     5613 2023-04-06 23:28:27.138525 semantic_kernel-0.2.1.dev0/semantic_kernel/core_skills/time_skill.py
+-rw-r--r--   0        0        0    10609 2023-04-06 23:28:27.138525 semantic_kernel-0.2.1.dev0/semantic_kernel/kernel.py
+-rw-r--r--   0        0        0     2342 2023-04-06 23:28:27.139523 semantic_kernel-0.2.1.dev0/semantic_kernel/kernel_base.py
+-rw-r--r--   0        0        0     3097 2023-04-06 23:28:27.139523 semantic_kernel-0.2.1.dev0/semantic_kernel/kernel_builder.py
+-rw-r--r--   0        0        0     9134 2023-04-10 18:26:09.500824 semantic_kernel-0.2.1.dev0/semantic_kernel/kernel_config.py
+-rw-r--r--   0        0        0     1626 2023-04-06 23:28:27.140524 semantic_kernel-0.2.1.dev0/semantic_kernel/kernel_exception.py
+-rw-r--r--   0        0        0      710 2023-04-06 23:28:27.141523 semantic_kernel-0.2.1.dev0/semantic_kernel/kernel_extensions/__init__.py
+-rw-r--r--   0        0        0      210 2023-04-06 23:28:27.141523 semantic_kernel-0.2.1.dev0/semantic_kernel/kernel_extensions/extends_kernel.py
+-rw-r--r--   0        0        0     2374 2023-04-06 23:28:27.141523 semantic_kernel-0.2.1.dev0/semantic_kernel/kernel_extensions/import_skills.py
+-rw-r--r--   0        0        0     2323 2023-04-06 23:28:27.142522 semantic_kernel-0.2.1.dev0/semantic_kernel/kernel_extensions/inline_definition.py
+-rw-r--r--   0        0        0     1531 2023-04-06 23:28:27.142522 semantic_kernel-0.2.1.dev0/semantic_kernel/kernel_extensions/memory_configuration.py
+-rw-r--r--   0        0        0      160 2023-04-06 23:28:27.143521 semantic_kernel-0.2.1.dev0/semantic_kernel/memory/__init__.py
+-rw-r--r--   0        0        0     1174 2023-04-06 23:28:27.143521 semantic_kernel-0.2.1.dev0/semantic_kernel/memory/memory_query_result.py
+-rw-r--r--   0        0        0     1598 2023-04-06 23:28:27.143521 semantic_kernel-0.2.1.dev0/semantic_kernel/memory/memory_record.py
+-rw-r--r--   0        0        0      299 2023-04-06 23:28:27.144521 semantic_kernel-0.2.1.dev0/semantic_kernel/memory/memory_store_base.py
+-rw-r--r--   0        0        0     1137 2023-04-06 23:28:27.144521 semantic_kernel-0.2.1.dev0/semantic_kernel/memory/null_memory.py
+-rw-r--r--   0        0        0     2499 2023-04-06 23:28:27.144521 semantic_kernel-0.2.1.dev0/semantic_kernel/memory/semantic_text_memory.py
+-rw-r--r--   0        0        0     1237 2023-04-06 23:28:27.145522 semantic_kernel-0.2.1.dev0/semantic_kernel/memory/semantic_text_memory_base.py
+-rw-r--r--   0        0        0      836 2023-04-06 23:28:27.145522 semantic_kernel-0.2.1.dev0/semantic_kernel/memory/storage/data_entry.py
+-rw-r--r--   0        0        0      953 2023-04-06 23:28:27.145522 semantic_kernel-0.2.1.dev0/semantic_kernel/memory/storage/data_store_base.py
+-rw-r--r--   0        0        0     1989 2023-04-06 23:28:27.145522 semantic_kernel-0.2.1.dev0/semantic_kernel/memory/storage/volatile_data_store.py
+-rw-r--r--   0        0        0     4050 2023-04-06 23:28:27.146521 semantic_kernel-0.2.1.dev0/semantic_kernel/memory/volatile_memory_store.py
+-rw-r--r--   0        0        0     2328 2023-04-06 23:28:27.146521 semantic_kernel-0.2.1.dev0/semantic_kernel/orchestration/context_variables.py
+-rw-r--r--   0        0        0     5079 2023-04-06 23:28:27.146521 semantic_kernel-0.2.1.dev0/semantic_kernel/orchestration/delegate_handlers.py
+-rw-r--r--   0        0        0     8966 2023-04-06 23:28:27.147521 semantic_kernel-0.2.1.dev0/semantic_kernel/orchestration/delegate_inference.py
+-rw-r--r--   0        0        0      638 2023-04-06 23:28:27.147521 semantic_kernel-0.2.1.dev0/semantic_kernel/orchestration/delegate_types.py
+-rw-r--r--   0        0        0     7519 2023-04-11 21:50:16.599845 semantic_kernel-0.2.1.dev0/semantic_kernel/orchestration/sk_context.py
+-rw-r--r--   0        0        0    16307 2023-04-11 02:19:27.285436 semantic_kernel-0.2.1.dev0/semantic_kernel/orchestration/sk_function.py
+-rw-r--r--   0        0        0     6960 2023-04-10 18:26:09.501831 semantic_kernel-0.2.1.dev0/semantic_kernel/orchestration/sk_function_base.py
+-rw-r--r--   0        0        0      919 2023-04-06 23:28:27.149523 semantic_kernel-0.2.1.dev0/semantic_kernel/reliability/pass_through_without_retry.py
+-rw-r--r--   0        0        0      673 2023-04-06 23:28:27.149523 semantic_kernel-0.2.1.dev0/semantic_kernel/reliability/retry_mechanism.py
+-rw-r--r--   0        0        0     2101 2023-04-06 23:28:27.150523 semantic_kernel-0.2.1.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
+-rw-r--r--   0        0        0     2332 2023-04-06 23:28:27.150523 semantic_kernel-0.2.1.dev0/semantic_kernel/semantic_functions/prompt_template.py
+-rw-r--r--   0        0        0      506 2023-04-06 23:28:27.151524 semantic_kernel-0.2.1.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
+-rw-r--r--   0        0        0     3437 2023-04-06 23:28:27.151524 semantic_kernel-0.2.1.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
+-rw-r--r--   0        0        0      671 2023-04-06 23:28:27.152522 semantic_kernel-0.2.1.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
+-rw-r--r--   0        0        0      322 2023-04-06 23:28:27.152522 semantic_kernel-0.2.1.dev0/semantic_kernel/skill_definition/__init__.py
+-rw-r--r--   0        0        0     2053 2023-04-06 23:28:27.153521 semantic_kernel-0.2.1.dev0/semantic_kernel/skill_definition/function_view.py
+-rw-r--r--   0        0        0     1717 2023-04-06 23:28:27.154523 semantic_kernel-0.2.1.dev0/semantic_kernel/skill_definition/functions_view.py
+-rw-r--r--   0        0        0     1026 2023-04-06 23:28:27.154523 semantic_kernel-0.2.1.dev0/semantic_kernel/skill_definition/parameter_view.py
+-rw-r--r--   0        0        0     2104 2023-04-06 23:28:27.155525 semantic_kernel-0.2.1.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
+-rw-r--r--   0        0        0     1345 2023-04-06 23:28:27.155525 semantic_kernel-0.2.1.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
+-rw-r--r--   0        0        0      858 2023-04-06 23:28:27.156525 semantic_kernel-0.2.1.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
+-rw-r--r--   0        0        0      837 2023-04-06 23:28:27.156525 semantic_kernel-0.2.1.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
+-rw-r--r--   0        0        0     6056 2023-04-06 23:28:27.156525 semantic_kernel-0.2.1.dev0/semantic_kernel/skill_definition/skill_collection.py
+-rw-r--r--   0        0        0      803 2023-04-06 23:28:27.157522 semantic_kernel-0.2.1.dev0/semantic_kernel/skill_definition/skill_collection_base.py
+-rw-r--r--   0        0        0      830 2023-04-06 23:28:27.158522 semantic_kernel-0.2.1.dev0/semantic_kernel/template_engine/blocks/block.py
+-rw-r--r--   0        0        0      228 2023-04-06 23:28:27.158522 semantic_kernel-0.2.1.dev0/semantic_kernel/template_engine/blocks/block_types.py
+-rw-r--r--   0        0        0     4566 2023-04-10 18:26:09.501831 semantic_kernel-0.2.1.dev0/semantic_kernel/template_engine/blocks/code_block.py
+-rw-r--r--   0        0        0     2653 2023-04-06 23:28:27.159522 semantic_kernel-0.2.1.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
+-rw-r--r--   0        0        0      276 2023-04-06 23:28:27.160524 semantic_kernel-0.2.1.dev0/semantic_kernel/template_engine/blocks/symbols.py
+-rw-r--r--   0        0        0     1534 2023-04-06 23:28:27.160524 semantic_kernel-0.2.1.dev0/semantic_kernel/template_engine/blocks/text_block.py
+-rw-r--r--   0        0        0     2274 2023-04-06 23:28:27.160524 semantic_kernel-0.2.1.dev0/semantic_kernel/template_engine/blocks/val_block.py
+-rw-r--r--   0        0        0     2517 2023-04-06 23:28:27.161522 semantic_kernel-0.2.1.dev0/semantic_kernel/template_engine/blocks/var_block.py
+-rw-r--r--   0        0        0     6535 2023-04-06 23:28:27.161522 semantic_kernel-0.2.1.dev0/semantic_kernel/template_engine/code_tokenizer.py
+-rw-r--r--   0        0        0     6051 2023-04-06 23:28:27.162539 semantic_kernel-0.2.1.dev0/semantic_kernel/template_engine/prompt_template_engine.py
+-rw-r--r--   0        0        0      532 2023-04-06 23:28:27.162539 semantic_kernel-0.2.1.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
+-rw-r--r--   0        0        0     3043 2023-04-06 23:28:27.163522 semantic_kernel-0.2.1.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
+-rw-r--r--   0        0        0      596 2023-04-06 23:28:27.163522 semantic_kernel-0.2.1.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
+-rw-r--r--   0        0        0     1115 2023-04-06 23:28:27.157522 semantic_kernel-0.2.1.dev0/semantic_kernel/template_engine/README.md
+-rw-r--r--   0        0        0     7637 2023-04-06 23:28:27.164523 semantic_kernel-0.2.1.dev0/semantic_kernel/template_engine/template_tokenizer.py
+-rw-r--r--   0        0        0      403 2023-04-06 23:28:27.164523 semantic_kernel-0.2.1.dev0/semantic_kernel/utils/null_logger.py
+-rw-r--r--   0        0        0     2436 2023-04-06 23:28:27.165522 semantic_kernel-0.2.1.dev0/semantic_kernel/utils/settings.py
+-rw-r--r--   0        0        0      221 2023-04-06 23:28:27.165522 semantic_kernel-0.2.1.dev0/semantic_kernel/utils/static_property.py
+-rw-r--r--   0        0        0     2198 2023-04-06 23:28:27.165522 semantic_kernel-0.2.1.dev0/semantic_kernel/utils/validation.py
+-rw-r--r--   0        0        0     4229 1970-01-01 00:00:00.000000 semantic_kernel-0.2.1.dev0/PKG-INFO
```

### Comparing `semantic_kernel-0.2.0.dev0/pyproject.toml` & `semantic_kernel-0.2.1.dev0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "semantic-kernel"
-version = "0.2.0.dev"
+version = "0.2.1.dev"
 description = ""
 authors = ["Microsoft <SK-Support@microsoft.com>"]
 readme = "README.md"
 packages = [{include = "semantic_kernel"}]
+license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "^1.24.2"
 openai = "^0.27.0"
 aiofiles = "^23.1.0"
 asyncio = "^3.4.3"
```

### Comparing `semantic_kernel-0.2.0.dev0/README.md` & `semantic_kernel-0.2.1.dev0/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/__init__.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/ai/ai_exception.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/ai/ai_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/ai/chat_request_settings.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/ai/chat_request_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/ai/complete_request_settings.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/ai/complete_request_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/ai/open_ai/__init__.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/ai/open_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/ai/open_ai/services/azure_chat_completion.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/ai/open_ai/services/azure_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/ai/open_ai/services/azure_text_completion.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/ai/open_ai/services/azure_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/ai/open_ai/services/azure_text_embedding.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/ai/open_ai/services/azure_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/ai/open_ai/services/open_ai_chat_completion.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/ai/open_ai/services/open_ai_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_completion.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_embedding.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/ai/open_ai/services/open_ai_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/core_skills/file_io_skill.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/core_skills/file_io_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/core_skills/text_memory_skill.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/core_skills/text_memory_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/core_skills/text_skill.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/core_skills/text_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/core_skills/time_skill.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/core_skills/time_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/kernel.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/kernel.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_base.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/kernel_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_builder.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/kernel_builder.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_config.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/kernel_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_exception.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/kernel_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_extensions/__init__.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/kernel_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_extensions/import_skills.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/kernel_extensions/import_skills.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_extensions/inline_definition.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/kernel_extensions/inline_definition.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/kernel_extensions/memory_configuration.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/kernel_extensions/memory_configuration.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/memory/memory_query_result.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/memory/memory_query_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/memory/memory_record.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/memory/memory_record.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/memory/null_memory.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/memory/null_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/memory/semantic_text_memory.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/memory/semantic_text_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/memory/semantic_text_memory_base.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/memory/semantic_text_memory_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/memory/storage/data_entry.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/memory/storage/data_entry.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/memory/storage/data_store_base.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/memory/storage/data_store_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/memory/storage/volatile_data_store.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/memory/storage/volatile_data_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/memory/volatile_memory_store.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/memory/volatile_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/orchestration/context_variables.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/orchestration/context_variables.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/orchestration/delegate_handlers.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/orchestration/delegate_handlers.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/orchestration/delegate_inference.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/orchestration/delegate_inference.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/orchestration/delegate_types.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/orchestration/delegate_types.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/orchestration/sk_context.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/orchestration/sk_context.py`

 * *Files 3% similar despite different names*

```diff
@@ -127,14 +127,21 @@
         Read only skills collection.
 
         Returns:
             ReadOnlySkillCollectionBase -- The skills collection.
         """
         return self._skill_collection
 
+    @skills.setter
+    def skills(self, value: ReadOnlySkillCollectionBase) -> None:
+        """
+        Set the value of skills collection
+        """
+        self._skill_collection = value
+    
     @property
     def log(self) -> Logger:
         """
         The logger.
 
         Returns:
             Logger -- The logger.
@@ -231,7 +238,8 @@
         if self._skill_collection.has_semantic_function(skill_name, function_name):
             the_func = self._skill_collection.get_semantic_function(
                 skill_name, function_name
             )
             return True, the_func
 
         return False, None
+
```

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/orchestration/sk_function.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/orchestration/sk_function.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/orchestration/sk_function_base.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/orchestration/sk_function_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/reliability/pass_through_without_retry.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/reliability/pass_through_without_retry.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/reliability/retry_mechanism.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/reliability/retry_mechanism.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/semantic_functions/prompt_template.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/semantic_functions/prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/semantic_functions/prompt_template_config.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/semantic_functions/prompt_template_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/semantic_functions/semantic_function_config.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/semantic_functions/semantic_function_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/function_view.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/skill_definition/function_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/functions_view.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/skill_definition/functions_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/parameter_view.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/skill_definition/parameter_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/sk_function_decorator.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/skill_definition/sk_function_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/skill_collection.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/skill_definition/skill_collection.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/skill_definition/skill_collection_base.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/skill_definition/skill_collection_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/blocks/block.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/template_engine/blocks/block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/blocks/code_block.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/template_engine/blocks/code_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/blocks/function_id_block.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/template_engine/blocks/function_id_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/blocks/text_block.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/template_engine/blocks/text_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/blocks/val_block.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/template_engine/blocks/val_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/blocks/var_block.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/template_engine/blocks/var_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/code_tokenizer.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/template_engine/code_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/prompt_template_engine.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/template_engine/prompt_template_engine.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/protocols/code_renderer.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/template_engine/protocols/code_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/protocols/text_renderer.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/template_engine/protocols/text_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/README.md` & `semantic_kernel-0.2.1.dev0/semantic_kernel/template_engine/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/template_engine/template_tokenizer.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/template_engine/template_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/utils/settings.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/utils/settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/semantic_kernel/utils/validation.py` & `semantic_kernel-0.2.1.dev0/semantic_kernel/utils/validation.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.0.dev0/PKG-INFO` & `semantic_kernel-0.2.1.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: semantic-kernel
-Version: 0.2.0.dev0
+Version: 0.2.1.dev0
 Summary: 
+License: MIT
 Author: Microsoft
 Author-email: SK-Support@microsoft.com
 Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
```

