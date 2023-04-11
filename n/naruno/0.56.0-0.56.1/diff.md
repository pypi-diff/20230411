# Comparing `tmp/naruno-0.56.0.tar.gz` & `tmp/naruno-0.56.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naruno-0.56.0.tar", last modified: Mon Apr 10 18:13:09 2023, max compression
+gzip compressed data, was "naruno-0.56.1.tar", last modified: Tue Apr 11 06:16:11 2023, max compression
```

## Comparing `naruno-0.56.0.tar` & `naruno-0.56.1.tar`

### file list

```diff
@@ -1,301 +1,301 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.956470 naruno-0.56.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-10 18:13:01.000000 naruno-0.56.0/LICENCE-naruno-gui_lib__.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-10 18:13:01.000000 naruno-0.56.0/LICENCE-naruno-lib-mix__.md
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-10 18:13:01.000000 naruno-0.56.0/LICENCE-naruno-wallet-elipticcurve__.md
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-10 18:13:01.000000 naruno-0.56.0/LICENSE-others__.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-10 18:13:01.000000 naruno-0.56.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-04-10 18:13:09.956470 naruno-0.56.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-04-10 18:13:01.000000 naruno-0.56.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.932469 naruno-0.56.0/naruno/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.932469 naruno-0.56.0/naruno/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/accounts/account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.932469 naruno-0.56.0/naruno/accounts/commanders/
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/accounts/commanders/delete_commander.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/accounts/commanders/get_comnder.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/accounts/commanders/save_commander.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/accounts/get_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/accounts/get_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/accounts/get_sequence_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/accounts/save_accounts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.932469 naruno-0.56.0/naruno/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.932469 naruno-0.56.0/naruno/api/buildozer/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/api/buildozer/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    26232 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/api/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.932469 naruno-0.56.0/naruno/apps/
--rw-r--r--   0 runner    (1001) docker     (123)    29545 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/apps/remote_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.924469 naruno-0.56.0/naruno/blockchain/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.936469 naruno-0.56.0/naruno/blockchain/block/
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/blockchain/block/block_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/blockchain/block/blocks_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/blockchain/block/change_transaction_fee.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/blockchain/block/create_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/blockchain/block/get_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/blockchain/block/get_block_from_blockchain_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/blockchain/block/get_minumum_transfer_amount.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.936469 naruno-0.56.0/naruno/blockchain/block/hash/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/blockchain/block/hash/accounts_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/blockchain/block/hash/blocks_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/blockchain/block/hash/calculate_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/blockchain/block/hash/tx_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/blockchain/block/just_one_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/blockchain/block/max_data_size.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/blockchain/block/max_tx_number.py
--rw-r--r--   0 runner    (1001) docker     (123)    13888 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/blockchain/block/save_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/blockchain/block/save_block_to_blockchain_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/blockchain/block/shares.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.936469 naruno-0.56.0/naruno/blockchain/candidate_block/
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/blockchain/candidate_block/candidate_block_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.936469 naruno-0.56.0/naruno/cli/
--rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.936469 naruno-0.56.0/naruno/consensus/
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/consensus/consensus_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.936469 naruno-0.56.0/naruno/consensus/finished/
--rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/consensus/finished/finished_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.936469 naruno-0.56.0/naruno/consensus/finished/transactions/
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/consensus/finished/transactions/transactions_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.936469 naruno-0.56.0/naruno/consensus/finished/true_time/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/consensus/finished/true_time/true_time_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.936469 naruno-0.56.0/naruno/consensus/ongoing/
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/consensus/ongoing/ongoing_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.928469 naruno-0.56.0/naruno/consensus/rounds/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.936469 naruno-0.56.0/naruno/consensus/rounds/round_1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.936469 naruno-0.56.0/naruno/consensus/rounds/round_1/checks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.936469 naruno-0.56.0/naruno/consensus/rounds/round_1/checks/candidate_blocks/
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/consensus/rounds/round_1/checks/candidate_blocks/candidate_blocks_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/consensus/rounds/round_1/checks/checks_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.928469 naruno-0.56.0/naruno/consensus/rounds/round_1/checks/time/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.936469 naruno-0.56.0/naruno/consensus/rounds/round_1/checks/time/time_difference/
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/consensus/rounds/round_1/checks/time/time_difference/time_difference_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.936469 naruno-0.56.0/naruno/consensus/rounds/round_1/process/
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/consensus/rounds/round_1/process/process_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.936469 naruno-0.56.0/naruno/consensus/rounds/round_1/process/transactions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.936469 naruno-0.56.0/naruno/consensus/rounds/round_1/process/transactions/checks/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/consensus/rounds/round_1/process/transactions/checks/duplicated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.936469 naruno-0.56.0/naruno/consensus/rounds/round_1/process/transactions/find_newly/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/consensus/rounds/round_1/process/transactions/find_newly/find_newly_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.936469 naruno-0.56.0/naruno/consensus/rounds/round_1/process/transactions/find_validated/
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/consensus/rounds/round_1/process/transactions/find_validated/find_validated_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/consensus/rounds/round_1/process/transactions/transactions_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/consensus/rounds/round_1/round_1_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.936469 naruno-0.56.0/naruno/consensus/rounds/round_2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.936469 naruno-0.56.0/naruno/consensus/rounds/round_2/checks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.936469 naruno-0.56.0/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/candidate_blocks_hashes_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/consensus/rounds/round_2/checks/checks_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.928469 naruno-0.56.0/naruno/consensus/rounds/round_2/checks/time/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.936469 naruno-0.56.0/naruno/consensus/rounds/round_2/checks/time/time_difference/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/consensus/rounds/round_2/checks/time/time_difference/time_difference_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.936469 naruno-0.56.0/naruno/consensus/rounds/round_2/process/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.936469 naruno-0.56.0/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/candidate_blocks_hashes_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/consensus/rounds/round_2/process/process_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.936469 naruno-0.56.0/naruno/consensus/rounds/round_2/process/rescue/
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/consensus/rounds/round_2/process/rescue/rescue_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.936469 naruno-0.56.0/naruno/consensus/rounds/round_2/process/validate/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/consensus/rounds/round_2/process/validate/validate_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/consensus/rounds/round_2/round_2_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.936469 naruno-0.56.0/naruno/consensus/sync/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/consensus/sync/send_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/consensus/sync/send_block_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/consensus/sync/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.936469 naruno-0.56.0/naruno/db/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/db/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.936469 naruno-0.56.0/naruno/db/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/db/blocks/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.936469 naruno-0.56.0/naruno/db/commanders/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/db/commanders/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.936469 naruno-0.56.0/naruno/db/connected_nodes/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/db/connected_nodes/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.936469 naruno-0.56.0/naruno/db/connected_nodes_test_0/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/db/connected_nodes_test_0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.940469 naruno-0.56.0/naruno/db/connected_nodes_test_1/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/db/connected_nodes_test_1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.940469 naruno-0.56.0/naruno/db/connected_nodes_test_2/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/db/connected_nodes_test_2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.940469 naruno-0.56.0/naruno/db/extracted_proofs/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/db/extracted_proofs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.940469 naruno-0.56.0/naruno/db/my_transactions/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/db/my_transactions/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.940469 naruno-0.56.0/naruno/db/pending_transactions/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/db/pending_transactions/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.940469 naruno-0.56.0/naruno/db/pending_transactions_test_0/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/db/pending_transactions_test_0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.940469 naruno-0.56.0/naruno/db/pending_transactions_test_1/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/db/pending_transactions_test_1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.940469 naruno-0.56.0/naruno/db/pending_transactions_test_2/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/db/pending_transactions_test_2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.940469 naruno-0.56.0/naruno/db/proof/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/db/proof/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.940469 naruno-0.56.0/naruno/db/qrs/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/db/qrs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.940469 naruno-0.56.0/naruno/db/remote_app_cache/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/db/remote_app_cache/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.940469 naruno-0.56.0/naruno/db/signs/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/db/signs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.940469 naruno-0.56.0/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.940469 naruno-0.56.0/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB_not_our_transaction/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB_not_our_transaction/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.940469 naruno-0.56.0/naruno/db/test_consensus_trigger_finished/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/db/test_consensus_trigger_finished/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.940469 naruno-0.56.0/naruno/db/test_finished_main/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/db/test_finished_main/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.940469 naruno-0.56.0/naruno/db/test_finished_main_2/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/db/test_finished_main_2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.940469 naruno-0.56.0/naruno/db/test_finished_main_3/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/db/test_finished_main_3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.940469 naruno-0.56.0/naruno/db/test_finished_main_false_time/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/db/test_finished_main_false_time/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.940469 naruno-0.56.0/naruno/db/test_finished_main_no_reset/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/db/test_finished_main_no_reset/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.940469 naruno-0.56.0/naruno/db/test_proof_extracted/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/db/test_proof_extracted/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.940469 naruno-0.56.0/naruno/gui/
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui/popup.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui/the_naruno_gui_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.928469 naruno-0.56.0/naruno/gui_lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.944469 naruno-0.56.0/naruno/gui_lib/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/fonts/POPPINS_LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)   151396 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/fonts/Poppins-Black.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   171604 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/fonts/Poppins-BlackItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   153944 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/fonts/Poppins-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   176588 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/fonts/Poppins-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   152764 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/fonts/Poppins-ExtraBold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   173916 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/fonts/Poppins-ExtraBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   161456 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/fonts/Poppins-ExtraLight.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   186168 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/fonts/Poppins-ExtraLightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   182012 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/fonts/Poppins-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   159892 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/fonts/Poppins-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   184460 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/fonts/Poppins-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   156520 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/fonts/Poppins-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   180444 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/fonts/Poppins-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   158240 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/fonts/Poppins-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   155232 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/fonts/Poppins-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   178584 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/fonts/Poppins-SemiBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   161652 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/fonts/Poppins-Thin.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   187044 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/fonts/Poppins-ThinItalic.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.948469 naruno-0.56.0/naruno/gui_lib/images/
--rw-r--r--   0 runner    (1001) docker     (123)   254014 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/images/logo.ico
--rw-r--r--   0 runner    (1001) docker     (123)    19780 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    16238 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/images/logo_sm_orb_fw.png
--rw-r--r--   0 runner    (1001) docker     (123)    21468 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/images/logo_w_bc.png
--rw-r--r--   0 runner    (1001) docker     (123)   254014 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/images/logo_win.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.928469 naruno-0.56.0/naruno/gui_lib/libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.948469 naruno-0.56.0/naruno/gui_lib/libs/baseclass/
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/libs/baseclass/node_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/libs/baseclass/operations_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/libs/baseclass/root_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/libs/baseclass/settings_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/libs/baseclass/tabnavigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/libs/baseclass/wallet_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/libs/baseclass/welcome_screen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.948469 naruno-0.56.0/naruno/gui_lib/libs/kv/
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/libs/kv/node_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/libs/kv/operations_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/libs/kv/root_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/libs/kv/settings_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/libs/kv/tabnavigation.kv
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/libs/kv/wallet_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/gui_lib/libs/kv/welcome_screen.kv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.948469 naruno-0.56.0/naruno/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.948469 naruno-0.56.0/naruno/lib/backup/
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/lib/backup/naruno_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/lib/backup/naruno_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/lib/clean_up.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/lib/config_system.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/lib/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/lib/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/lib/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.948469 naruno-0.56.0/naruno/lib/mix/
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/lib/mix/merkle_root.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/lib/mix/mixlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/lib/notification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.952470 naruno-0.56.0/naruno/lib/performance_analyzers/
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/lib/performance_analyzers/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/lib/performance_analyzers/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/lib/performance_analyzers/blockshash.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/lib/performance_analyzers/blockshash_part.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/lib/performance_analyzers/heartbeat_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/lib/performance_analyzers/transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/lib/perpetualtimer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/lib/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/lib/safety.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/lib/settings_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/lib/sign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/lib/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/lib/verify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.952470 naruno-0.56.0/naruno/logs/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/logs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.952470 naruno-0.56.0/naruno/node/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.952470 naruno-0.56.0/naruno/node/client/
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/node/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/node/get_candidate_blocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.952470 naruno-0.56.0/naruno/node/server/
--rw-r--r--   0 runner    (1001) docker     (123)    28423 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/node/server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/node/unl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.952470 naruno-0.56.0/naruno/transactions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.952470 naruno-0.56.0/naruno/transactions/check/
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/transactions/check/check_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.952470 naruno-0.56.0/naruno/transactions/check/datas/
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/transactions/check/datas/check_datas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.952470 naruno-0.56.0/naruno/transactions/check/len/
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/transactions/check/len/check_len.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.952470 naruno-0.56.0/naruno/transactions/check/sign/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/transactions/check/sign/check_sign.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.952470 naruno-0.56.0/naruno/transactions/check/type/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/transactions/check/type/check_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/transactions/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/transactions/get_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.952470 naruno-0.56.0/naruno/transactions/my_transactions/
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/transactions/my_transactions/check_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/transactions/my_transactions/get_my_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/transactions/my_transactions/get_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/transactions/my_transactions/save_my_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/transactions/my_transactions/save_to_my_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/transactions/my_transactions/sended_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/transactions/my_transactions/validate_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.952470 naruno-0.56.0/naruno/transactions/pending/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/transactions/pending/delete_pending.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/transactions/pending/get_pending.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/transactions/pending/save_pending.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/transactions/pending_to_validating.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/transactions/print_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/transactions/process_the_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/transactions/send.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/transactions/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.952470 naruno-0.56.0/naruno/wallet/
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/wallet/delete_current_wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.956470 naruno-0.56.0/naruno/wallet/ellipticcurve/
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/wallet/ellipticcurve/curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/wallet/ellipticcurve/ecdsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/wallet/ellipticcurve/math.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/wallet/ellipticcurve/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/wallet/ellipticcurve/privateKey.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/wallet/ellipticcurve/publicKey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/wallet/ellipticcurve/signature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.956470 naruno-0.56.0/naruno/wallet/ellipticcurve/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/wallet/ellipticcurve/utils/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/wallet/ellipticcurve/utils/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/wallet/ellipticcurve/utils/der.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/wallet/ellipticcurve/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/wallet/ellipticcurve/utils/integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/wallet/ellipticcurve/utils/oid.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/wallet/ellipticcurve/utils/pem.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/wallet/get_saved_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/wallet/print_wallets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/wallet/save_wallet_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/wallet/wallet_create.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/wallet/wallet_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/wallet/wallet_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-10 18:13:01.000000 naruno-0.56.0/naruno/wallet/wallet_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:13:09.932469 naruno-0.56.0/naruno.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-04-10 18:13:09.000000 naruno-0.56.0/naruno.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-04-10 18:13:09.000000 naruno-0.56.0/naruno.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 18:13:09.000000 naruno-0.56.0/naruno.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-10 18:13:09.000000 naruno-0.56.0/naruno.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-10 18:13:09.000000 naruno-0.56.0/naruno.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 18:13:09.956470 naruno-0.56.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-10 18:13:01.000000 naruno-0.56.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.651673 naruno-0.56.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-11 06:16:02.000000 naruno-0.56.1/LICENCE-naruno-gui_lib__.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-11 06:16:02.000000 naruno-0.56.1/LICENCE-naruno-lib-mix__.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-11 06:16:02.000000 naruno-0.56.1/LICENCE-naruno-wallet-elipticcurve__.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-11 06:16:02.000000 naruno-0.56.1/LICENSE-others__.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-11 06:16:02.000000 naruno-0.56.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-04-11 06:16:11.651673 naruno-0.56.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-04-11 06:16:02.000000 naruno-0.56.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.623673 naruno-0.56.1/naruno/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.627673 naruno-0.56.1/naruno/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/accounts/account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.627673 naruno-0.56.1/naruno/accounts/commanders/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/accounts/commanders/delete_commander.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/accounts/commanders/get_comnder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/accounts/commanders/save_commander.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/accounts/get_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/accounts/get_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/accounts/get_sequence_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/accounts/save_accounts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.627673 naruno-0.56.1/naruno/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.627673 naruno-0.56.1/naruno/api/buildozer/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/api/buildozer/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26232 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/api/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.627673 naruno-0.56.1/naruno/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)    29545 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/apps/remote_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.607673 naruno-0.56.1/naruno/blockchain/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.631673 naruno-0.56.1/naruno/blockchain/block/
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/blockchain/block/block_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/blockchain/block/blocks_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/blockchain/block/change_transaction_fee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/blockchain/block/create_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/blockchain/block/get_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/blockchain/block/get_block_from_blockchain_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/blockchain/block/get_minumum_transfer_amount.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.631673 naruno-0.56.1/naruno/blockchain/block/hash/
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/blockchain/block/hash/accounts_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/blockchain/block/hash/blocks_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/blockchain/block/hash/calculate_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/blockchain/block/hash/tx_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/blockchain/block/just_one_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/blockchain/block/max_data_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/blockchain/block/max_tx_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13888 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/blockchain/block/save_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/blockchain/block/save_block_to_blockchain_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/blockchain/block/shares.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.631673 naruno-0.56.1/naruno/blockchain/candidate_block/
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/blockchain/candidate_block/candidate_block_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.631673 naruno-0.56.1/naruno/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.631673 naruno-0.56.1/naruno/consensus/
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/consensus/consensus_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.631673 naruno-0.56.1/naruno/consensus/finished/
+-rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/consensus/finished/finished_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.631673 naruno-0.56.1/naruno/consensus/finished/transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/consensus/finished/transactions/transactions_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.631673 naruno-0.56.1/naruno/consensus/finished/true_time/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/consensus/finished/true_time/true_time_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.631673 naruno-0.56.1/naruno/consensus/ongoing/
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/consensus/ongoing/ongoing_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.611673 naruno-0.56.1/naruno/consensus/rounds/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.631673 naruno-0.56.1/naruno/consensus/rounds/round_1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.631673 naruno-0.56.1/naruno/consensus/rounds/round_1/checks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.631673 naruno-0.56.1/naruno/consensus/rounds/round_1/checks/candidate_blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/consensus/rounds/round_1/checks/candidate_blocks/candidate_blocks_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/consensus/rounds/round_1/checks/checks_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.611673 naruno-0.56.1/naruno/consensus/rounds/round_1/checks/time/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.631673 naruno-0.56.1/naruno/consensus/rounds/round_1/checks/time/time_difference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/consensus/rounds/round_1/checks/time/time_difference/time_difference_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.631673 naruno-0.56.1/naruno/consensus/rounds/round_1/process/
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/consensus/rounds/round_1/process/process_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.631673 naruno-0.56.1/naruno/consensus/rounds/round_1/process/transactions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.631673 naruno-0.56.1/naruno/consensus/rounds/round_1/process/transactions/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/consensus/rounds/round_1/process/transactions/checks/duplicated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.631673 naruno-0.56.1/naruno/consensus/rounds/round_1/process/transactions/find_newly/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/consensus/rounds/round_1/process/transactions/find_newly/find_newly_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.631673 naruno-0.56.1/naruno/consensus/rounds/round_1/process/transactions/find_validated/
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/consensus/rounds/round_1/process/transactions/find_validated/find_validated_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/consensus/rounds/round_1/process/transactions/transactions_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/consensus/rounds/round_1/round_1_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.631673 naruno-0.56.1/naruno/consensus/rounds/round_2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.631673 naruno-0.56.1/naruno/consensus/rounds/round_2/checks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.631673 naruno-0.56.1/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/candidate_blocks_hashes_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/consensus/rounds/round_2/checks/checks_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.611673 naruno-0.56.1/naruno/consensus/rounds/round_2/checks/time/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.631673 naruno-0.56.1/naruno/consensus/rounds/round_2/checks/time/time_difference/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/consensus/rounds/round_2/checks/time/time_difference/time_difference_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.631673 naruno-0.56.1/naruno/consensus/rounds/round_2/process/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.631673 naruno-0.56.1/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/candidate_blocks_hashes_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/consensus/rounds/round_2/process/process_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.631673 naruno-0.56.1/naruno/consensus/rounds/round_2/process/rescue/
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/consensus/rounds/round_2/process/rescue/rescue_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.631673 naruno-0.56.1/naruno/consensus/rounds/round_2/process/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/consensus/rounds/round_2/process/validate/validate_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/consensus/rounds/round_2/round_2_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.631673 naruno-0.56.1/naruno/consensus/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/consensus/sync/send_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/consensus/sync/send_block_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/consensus/sync/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.631673 naruno-0.56.1/naruno/db/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/db/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.631673 naruno-0.56.1/naruno/db/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/db/blocks/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.631673 naruno-0.56.1/naruno/db/commanders/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/db/commanders/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.635673 naruno-0.56.1/naruno/db/connected_nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/db/connected_nodes/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.635673 naruno-0.56.1/naruno/db/connected_nodes_test_0/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/db/connected_nodes_test_0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.635673 naruno-0.56.1/naruno/db/connected_nodes_test_1/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/db/connected_nodes_test_1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.635673 naruno-0.56.1/naruno/db/connected_nodes_test_2/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/db/connected_nodes_test_2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.635673 naruno-0.56.1/naruno/db/extracted_proofs/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/db/extracted_proofs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.635673 naruno-0.56.1/naruno/db/my_transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/db/my_transactions/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.635673 naruno-0.56.1/naruno/db/pending_transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/db/pending_transactions/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.635673 naruno-0.56.1/naruno/db/pending_transactions_test_0/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/db/pending_transactions_test_0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.635673 naruno-0.56.1/naruno/db/pending_transactions_test_1/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/db/pending_transactions_test_1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.635673 naruno-0.56.1/naruno/db/pending_transactions_test_2/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/db/pending_transactions_test_2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.635673 naruno-0.56.1/naruno/db/proof/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/db/proof/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.635673 naruno-0.56.1/naruno/db/qrs/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/db/qrs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.635673 naruno-0.56.1/naruno/db/remote_app_cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/db/remote_app_cache/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.635673 naruno-0.56.1/naruno/db/signs/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/db/signs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.635673 naruno-0.56.1/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.635673 naruno-0.56.1/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB_not_our_transaction/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB_not_our_transaction/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.635673 naruno-0.56.1/naruno/db/test_consensus_trigger_finished/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/db/test_consensus_trigger_finished/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.635673 naruno-0.56.1/naruno/db/test_finished_main/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/db/test_finished_main/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.639673 naruno-0.56.1/naruno/db/test_finished_main_2/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/db/test_finished_main_2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.639673 naruno-0.56.1/naruno/db/test_finished_main_3/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/db/test_finished_main_3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.639673 naruno-0.56.1/naruno/db/test_finished_main_false_time/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/db/test_finished_main_false_time/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.639673 naruno-0.56.1/naruno/db/test_finished_main_no_reset/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/db/test_finished_main_no_reset/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.639673 naruno-0.56.1/naruno/db/test_proof_extracted/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/db/test_proof_extracted/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.639673 naruno-0.56.1/naruno/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui/popup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui/the_naruno_gui_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.619673 naruno-0.56.1/naruno/gui_lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.643673 naruno-0.56.1/naruno/gui_lib/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/fonts/POPPINS_LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)   151396 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/fonts/Poppins-Black.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   171604 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/fonts/Poppins-BlackItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   153944 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/fonts/Poppins-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   176588 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/fonts/Poppins-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   152764 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/fonts/Poppins-ExtraBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   173916 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/fonts/Poppins-ExtraBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161456 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/fonts/Poppins-ExtraLight.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   186168 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/fonts/Poppins-ExtraLightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   182012 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/fonts/Poppins-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   159892 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/fonts/Poppins-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   184460 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/fonts/Poppins-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   156520 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/fonts/Poppins-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   180444 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/fonts/Poppins-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   158240 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/fonts/Poppins-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   155232 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/fonts/Poppins-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   178584 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/fonts/Poppins-SemiBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161652 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/fonts/Poppins-Thin.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   187044 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/fonts/Poppins-ThinItalic.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.643673 naruno-0.56.1/naruno/gui_lib/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   254014 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/images/logo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    19780 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16238 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/images/logo_sm_orb_fw.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21468 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/images/logo_w_bc.png
+-rw-r--r--   0 runner    (1001) docker     (123)   254014 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/images/logo_win.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.619673 naruno-0.56.1/naruno/gui_lib/libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.643673 naruno-0.56.1/naruno/gui_lib/libs/baseclass/
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/libs/baseclass/node_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/libs/baseclass/operations_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/libs/baseclass/root_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/libs/baseclass/settings_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/libs/baseclass/tabnavigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/libs/baseclass/wallet_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/libs/baseclass/welcome_screen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.647673 naruno-0.56.1/naruno/gui_lib/libs/kv/
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/libs/kv/node_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/libs/kv/operations_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/libs/kv/root_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/libs/kv/settings_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/libs/kv/tabnavigation.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/libs/kv/wallet_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/gui_lib/libs/kv/welcome_screen.kv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.647673 naruno-0.56.1/naruno/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.647673 naruno-0.56.1/naruno/lib/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/lib/backup/naruno_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/lib/backup/naruno_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/lib/clean_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/lib/config_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/lib/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/lib/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/lib/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.647673 naruno-0.56.1/naruno/lib/mix/
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/lib/mix/merkle_root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/lib/mix/mixlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/lib/notification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.647673 naruno-0.56.1/naruno/lib/performance_analyzers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/lib/performance_analyzers/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/lib/performance_analyzers/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/lib/performance_analyzers/blockshash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/lib/performance_analyzers/blockshash_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/lib/performance_analyzers/heartbeat_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/lib/performance_analyzers/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/lib/perpetualtimer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/lib/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/lib/safety.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/lib/settings_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/lib/sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/lib/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/lib/verify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.647673 naruno-0.56.1/naruno/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/logs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.647673 naruno-0.56.1/naruno/node/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.647673 naruno-0.56.1/naruno/node/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/node/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/node/get_candidate_blocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.647673 naruno-0.56.1/naruno/node/server/
+-rw-r--r--   0 runner    (1001) docker     (123)    28423 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/node/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/node/unl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.647673 naruno-0.56.1/naruno/transactions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.647673 naruno-0.56.1/naruno/transactions/check/
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/transactions/check/check_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.647673 naruno-0.56.1/naruno/transactions/check/datas/
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/transactions/check/datas/check_datas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.647673 naruno-0.56.1/naruno/transactions/check/len/
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/transactions/check/len/check_len.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.647673 naruno-0.56.1/naruno/transactions/check/sign/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/transactions/check/sign/check_sign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.651673 naruno-0.56.1/naruno/transactions/check/type/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/transactions/check/type/check_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/transactions/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/transactions/get_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.651673 naruno-0.56.1/naruno/transactions/my_transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/transactions/my_transactions/check_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/transactions/my_transactions/get_my_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/transactions/my_transactions/get_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/transactions/my_transactions/save_my_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/transactions/my_transactions/save_to_my_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/transactions/my_transactions/sended_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/transactions/my_transactions/validate_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.651673 naruno-0.56.1/naruno/transactions/pending/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/transactions/pending/delete_pending.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/transactions/pending/get_pending.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/transactions/pending/save_pending.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/transactions/pending_to_validating.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/transactions/print_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/transactions/process_the_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/transactions/send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/transactions/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.651673 naruno-0.56.1/naruno/wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/wallet/delete_current_wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.651673 naruno-0.56.1/naruno/wallet/ellipticcurve/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/wallet/ellipticcurve/curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/wallet/ellipticcurve/ecdsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/wallet/ellipticcurve/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/wallet/ellipticcurve/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/wallet/ellipticcurve/privateKey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/wallet/ellipticcurve/publicKey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/wallet/ellipticcurve/signature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.651673 naruno-0.56.1/naruno/wallet/ellipticcurve/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/wallet/ellipticcurve/utils/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/wallet/ellipticcurve/utils/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/wallet/ellipticcurve/utils/der.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/wallet/ellipticcurve/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/wallet/ellipticcurve/utils/integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/wallet/ellipticcurve/utils/oid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/wallet/ellipticcurve/utils/pem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/wallet/get_saved_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/wallet/print_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/wallet/save_wallet_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/wallet/wallet_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/wallet/wallet_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/wallet/wallet_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-11 06:16:02.000000 naruno-0.56.1/naruno/wallet/wallet_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:16:11.627673 naruno-0.56.1/naruno.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-04-11 06:16:11.000000 naruno-0.56.1/naruno.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-04-11 06:16:11.000000 naruno-0.56.1/naruno.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 06:16:11.000000 naruno-0.56.1/naruno.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-11 06:16:11.000000 naruno-0.56.1/naruno.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 06:16:11.000000 naruno-0.56.1/naruno.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 06:16:11.651673 naruno-0.56.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-11 06:16:02.000000 naruno-0.56.1/setup.py
```

### Comparing `naruno-0.56.0/LICENCE-naruno-gui_lib__.md` & `naruno-0.56.1/LICENCE-naruno-gui_lib__.md`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/LICENCE-naruno-lib-mix__.md` & `naruno-0.56.1/LICENCE-naruno-lib-mix__.md`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/LICENCE-naruno-wallet-elipticcurve__.md` & `naruno-0.56.1/LICENCE-naruno-wallet-elipticcurve__.md`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/LICENSE-others__.md` & `naruno-0.56.1/LICENSE-others__.md`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/PKG-INFO` & `naruno-0.56.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naruno
-Version: 0.56.0
+Version: 0.56.1
 Summary: Naruno is a lightning-fast, secure, and scalable blockchain that is able to create transaction proofs and verification via raw data and timestamp. We remove the archive nodes and lazy web3 integrations. With Naruno everyone can get the proof (5-10MB) of their transactions via their nodes and after everyone can use in another node for verification the raw data and timestamp. Also you can integrate your web3 applications with 4 code lines (just python for now) via our remote app system.
 Home-page: https://github.com/Naruno/Naruno
 Author: Naruno Developers
 Author-email: onur.atakan.ulusoy@naruno.org
 License: MPL-2.0
 Description: <p align="center">
           <a href="https://github.com/Naruno/Naruno">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: naruno Version: 0.56.0 Summary: Naruno is a
+Metadata-Version: 2.1 Name: naruno Version: 0.56.1 Summary: Naruno is a
 lightning-fast, secure, and scalable blockchain that is able to create
 transaction proofs and verification via raw data and timestamp. We remove the
 archive nodes and lazy web3 integrations. With Naruno everyone can get the
 proof (5-10MB) of their transactions via their nodes and after everyone can use
 in another node for verification the raw data and timestamp. Also you can
 integrate your web3 applications with 4 code lines (just python for now) via
 our remote app system. Home-page: https://github.com/Naruno/Naruno Author:
```

### Comparing `naruno-0.56.0/README.md` & `naruno-0.56.1/README.md`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/accounts/account.py` & `naruno-0.56.1/naruno/accounts/account.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/accounts/commanders/delete_commander.py` & `naruno-0.56.1/naruno/accounts/commanders/delete_commander.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/accounts/commanders/get_comnder.py` & `naruno-0.56.1/naruno/accounts/commanders/get_comnder.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/accounts/commanders/save_commander.py` & `naruno-0.56.1/naruno/accounts/commanders/save_commander.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/accounts/get_accounts.py` & `naruno-0.56.1/naruno/accounts/get_accounts.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/accounts/get_balance.py` & `naruno-0.56.1/naruno/accounts/get_balance.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/accounts/get_sequence_number.py` & `naruno-0.56.1/naruno/accounts/get_sequence_number.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/accounts/save_accounts.py` & `naruno-0.56.1/naruno/accounts/save_accounts.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/api/buildozer/main.py` & `naruno-0.56.1/naruno/api/buildozer/main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/api/main.py` & `naruno-0.56.1/naruno/api/main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/apps/remote_app.py` & `naruno-0.56.1/naruno/apps/remote_app.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/blockchain/block/block_main.py` & `naruno-0.56.1/naruno/blockchain/block/block_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/blockchain/block/blocks_hash.py` & `naruno-0.56.1/naruno/blockchain/block/blocks_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/blockchain/block/change_transaction_fee.py` & `naruno-0.56.1/naruno/blockchain/block/change_transaction_fee.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/blockchain/block/create_block.py` & `naruno-0.56.1/naruno/blockchain/block/create_block.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/blockchain/block/get_block.py` & `naruno-0.56.1/naruno/blockchain/block/get_block.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/blockchain/block/get_block_from_blockchain_db.py` & `naruno-0.56.1/naruno/blockchain/block/get_block_from_blockchain_db.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/blockchain/block/get_minumum_transfer_amount.py` & `naruno-0.56.1/naruno/blockchain/block/get_minumum_transfer_amount.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/blockchain/block/hash/accounts_hash.py` & `naruno-0.56.1/naruno/blockchain/block/hash/accounts_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/blockchain/block/hash/blocks_hash.py` & `naruno-0.56.1/naruno/blockchain/block/hash/blocks_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/blockchain/block/hash/calculate_hash.py` & `naruno-0.56.1/naruno/blockchain/block/hash/calculate_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/blockchain/block/hash/tx_hash.py` & `naruno-0.56.1/naruno/blockchain/block/hash/tx_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/blockchain/block/just_one_tx.py` & `naruno-0.56.1/naruno/blockchain/block/just_one_tx.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/blockchain/block/max_data_size.py` & `naruno-0.56.1/naruno/blockchain/block/max_data_size.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/blockchain/block/max_tx_number.py` & `naruno-0.56.1/naruno/blockchain/block/max_tx_number.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/blockchain/block/save_block.py` & `naruno-0.56.1/naruno/blockchain/block/save_block.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/blockchain/block/save_block_to_blockchain_db.py` & `naruno-0.56.1/naruno/blockchain/block/save_block_to_blockchain_db.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/blockchain/block/shares.py` & `naruno-0.56.1/naruno/blockchain/block/shares.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/blockchain/candidate_block/candidate_block_main.py` & `naruno-0.56.1/naruno/blockchain/candidate_block/candidate_block_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/cli/main.py` & `naruno-0.56.1/naruno/cli/main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/config.py` & `naruno-0.56.1/naruno/config.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/consensus/consensus_main.py` & `naruno-0.56.1/naruno/consensus/consensus_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/consensus/finished/finished_main.py` & `naruno-0.56.1/naruno/consensus/finished/finished_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/consensus/finished/transactions/transactions_main.py` & `naruno-0.56.1/naruno/consensus/finished/transactions/transactions_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/consensus/finished/true_time/true_time_main.py` & `naruno-0.56.1/naruno/consensus/finished/true_time/true_time_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/consensus/ongoing/ongoing_main.py` & `naruno-0.56.1/naruno/consensus/ongoing/ongoing_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/consensus/rounds/round_1/checks/candidate_blocks/candidate_blocks_main.py` & `naruno-0.56.1/naruno/consensus/rounds/round_1/checks/candidate_blocks/candidate_blocks_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/consensus/rounds/round_1/checks/checks_main.py` & `naruno-0.56.1/naruno/consensus/rounds/round_1/checks/checks_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/consensus/rounds/round_1/checks/time/time_difference/time_difference_main.py` & `naruno-0.56.1/naruno/consensus/rounds/round_1/checks/time/time_difference/time_difference_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/consensus/rounds/round_1/process/process_main.py` & `naruno-0.56.1/naruno/consensus/rounds/round_1/process/process_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/consensus/rounds/round_1/process/transactions/checks/duplicated.py` & `naruno-0.56.1/naruno/consensus/rounds/round_1/process/transactions/checks/duplicated.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/consensus/rounds/round_1/process/transactions/find_newly/find_newly_main.py` & `naruno-0.56.1/naruno/consensus/rounds/round_1/process/transactions/find_newly/find_newly_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/consensus/rounds/round_1/process/transactions/find_validated/find_validated_main.py` & `naruno-0.56.1/naruno/consensus/rounds/round_1/process/transactions/find_validated/find_validated_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/consensus/rounds/round_1/process/transactions/transactions_main.py` & `naruno-0.56.1/naruno/consensus/rounds/round_1/process/transactions/transactions_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/consensus/rounds/round_1/round_1_main.py` & `naruno-0.56.1/naruno/consensus/rounds/round_1/round_1_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/candidate_blocks_hashes_main.py` & `naruno-0.56.1/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/candidate_blocks_hashes_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/consensus/rounds/round_2/checks/checks_main.py` & `naruno-0.56.1/naruno/consensus/rounds/round_2/checks/checks_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/consensus/rounds/round_2/checks/time/time_difference/time_difference_main.py` & `naruno-0.56.1/naruno/consensus/rounds/round_2/checks/time/time_difference/time_difference_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/candidate_blocks_hashes_main.py` & `naruno-0.56.1/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/candidate_blocks_hashes_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/consensus/rounds/round_2/process/process_main.py` & `naruno-0.56.1/naruno/consensus/rounds/round_2/process/process_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/consensus/rounds/round_2/process/rescue/rescue_main.py` & `naruno-0.56.1/naruno/consensus/rounds/round_2/process/rescue/rescue_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/consensus/rounds/round_2/process/validate/validate_main.py` & `naruno-0.56.1/naruno/consensus/rounds/round_2/process/validate/validate_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/consensus/rounds/round_2/round_2_main.py` & `naruno-0.56.1/naruno/consensus/rounds/round_2/round_2_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/consensus/sync/send_block.py` & `naruno-0.56.1/naruno/consensus/sync/send_block.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/consensus/sync/send_block_hash.py` & `naruno-0.56.1/naruno/consensus/sync/send_block_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/consensus/sync/sync.py` & `naruno-0.56.1/naruno/consensus/sync/sync.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui/main.py` & `naruno-0.56.1/naruno/gui/main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui/popup.py` & `naruno-0.56.1/naruno/gui/popup.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/fonts/POPPINS_LICENCE` & `naruno-0.56.1/naruno/gui_lib/fonts/POPPINS_LICENCE`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/fonts/Poppins-Black.ttf` & `naruno-0.56.1/naruno/gui_lib/fonts/Poppins-Black.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/fonts/Poppins-BlackItalic.ttf` & `naruno-0.56.1/naruno/gui_lib/fonts/Poppins-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/fonts/Poppins-Bold.ttf` & `naruno-0.56.1/naruno/gui_lib/fonts/Poppins-Bold.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/fonts/Poppins-BoldItalic.ttf` & `naruno-0.56.1/naruno/gui_lib/fonts/Poppins-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/fonts/Poppins-ExtraBold.ttf` & `naruno-0.56.1/naruno/gui_lib/fonts/Poppins-ExtraBold.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/fonts/Poppins-ExtraBoldItalic.ttf` & `naruno-0.56.1/naruno/gui_lib/fonts/Poppins-ExtraBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/fonts/Poppins-ExtraLight.ttf` & `naruno-0.56.1/naruno/gui_lib/fonts/Poppins-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/fonts/Poppins-ExtraLightItalic.ttf` & `naruno-0.56.1/naruno/gui_lib/fonts/Poppins-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/fonts/Poppins-Italic.ttf` & `naruno-0.56.1/naruno/gui_lib/fonts/Poppins-Italic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/fonts/Poppins-Light.ttf` & `naruno-0.56.1/naruno/gui_lib/fonts/Poppins-Light.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/fonts/Poppins-LightItalic.ttf` & `naruno-0.56.1/naruno/gui_lib/fonts/Poppins-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/fonts/Poppins-Medium.ttf` & `naruno-0.56.1/naruno/gui_lib/fonts/Poppins-Medium.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/fonts/Poppins-MediumItalic.ttf` & `naruno-0.56.1/naruno/gui_lib/fonts/Poppins-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/fonts/Poppins-Regular.ttf` & `naruno-0.56.1/naruno/gui_lib/fonts/Poppins-Regular.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/fonts/Poppins-SemiBold.ttf` & `naruno-0.56.1/naruno/gui_lib/fonts/Poppins-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/fonts/Poppins-SemiBoldItalic.ttf` & `naruno-0.56.1/naruno/gui_lib/fonts/Poppins-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/fonts/Poppins-Thin.ttf` & `naruno-0.56.1/naruno/gui_lib/fonts/Poppins-Thin.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/fonts/Poppins-ThinItalic.ttf` & `naruno-0.56.1/naruno/gui_lib/fonts/Poppins-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/images/logo.ico` & `naruno-0.56.1/naruno/gui_lib/images/logo.ico`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/images/logo.png` & `naruno-0.56.1/naruno/gui_lib/images/logo.png`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/images/logo_sm_orb_fw.png` & `naruno-0.56.1/naruno/gui_lib/images/logo_sm_orb_fw.png`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/images/logo_w_bc.png` & `naruno-0.56.1/naruno/gui_lib/images/logo_w_bc.png`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/images/logo_win.ico` & `naruno-0.56.1/naruno/gui_lib/images/logo_win.ico`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/libs/baseclass/node_screen.py` & `naruno-0.56.1/naruno/gui_lib/libs/baseclass/node_screen.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/libs/baseclass/operations_screen.py` & `naruno-0.56.1/naruno/gui_lib/libs/baseclass/operations_screen.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/libs/baseclass/root_screen.py` & `naruno-0.56.1/naruno/gui_lib/libs/baseclass/root_screen.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/libs/baseclass/settings_screen.py` & `naruno-0.56.1/naruno/gui_lib/libs/baseclass/settings_screen.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/libs/baseclass/tabnavigation.py` & `naruno-0.56.1/naruno/gui_lib/libs/baseclass/tabnavigation.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/libs/baseclass/wallet_screen.py` & `naruno-0.56.1/naruno/gui_lib/libs/baseclass/wallet_screen.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/libs/baseclass/welcome_screen.py` & `naruno-0.56.1/naruno/gui_lib/libs/baseclass/welcome_screen.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/libs/kv/node_screen.kv` & `naruno-0.56.1/naruno/gui_lib/libs/kv/node_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/libs/kv/operations_screen.kv` & `naruno-0.56.1/naruno/gui_lib/libs/kv/operations_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/libs/kv/root_screen.kv` & `naruno-0.56.1/naruno/gui_lib/libs/kv/root_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/libs/kv/settings_screen.kv` & `naruno-0.56.1/naruno/gui_lib/libs/kv/settings_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/libs/kv/tabnavigation.kv` & `naruno-0.56.1/naruno/gui_lib/libs/kv/tabnavigation.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/libs/kv/wallet_screen.kv` & `naruno-0.56.1/naruno/gui_lib/libs/kv/wallet_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/gui_lib/libs/kv/welcome_screen.kv` & `naruno-0.56.1/naruno/gui_lib/libs/kv/welcome_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/lib/backup/naruno_export.py` & `naruno-0.56.1/naruno/lib/backup/naruno_export.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/lib/backup/naruno_import.py` & `naruno-0.56.1/naruno/lib/backup/naruno_import.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/lib/clean_up.py` & `naruno-0.56.1/naruno/lib/clean_up.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/lib/config_system.py` & `naruno-0.56.1/naruno/lib/config_system.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/lib/encryption.py` & `naruno-0.56.1/naruno/lib/encryption.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/lib/export.py` & `naruno-0.56.1/naruno/lib/export.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/lib/log.py` & `naruno-0.56.1/naruno/lib/log.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/lib/mix/merkle_root.py` & `naruno-0.56.1/naruno/lib/mix/merkle_root.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/lib/mix/mixlib.py` & `naruno-0.56.1/naruno/lib/mix/mixlib.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/lib/notification.py` & `naruno-0.56.1/naruno/lib/notification.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/lib/performance_analyzers/accounts.py` & `naruno-0.56.1/naruno/lib/performance_analyzers/accounts.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/lib/performance_analyzers/block.py` & `naruno-0.56.1/naruno/lib/performance_analyzers/block.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/lib/performance_analyzers/blockshash.py` & `naruno-0.56.1/naruno/lib/performance_analyzers/blockshash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/lib/performance_analyzers/blockshash_part.py` & `naruno-0.56.1/naruno/lib/performance_analyzers/blockshash_part.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/lib/performance_analyzers/heartbeat_db.py` & `naruno-0.56.1/naruno/lib/performance_analyzers/heartbeat_db.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/lib/performance_analyzers/transactions.py` & `naruno-0.56.1/naruno/lib/performance_analyzers/transactions.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/lib/perpetualtimer.py` & `naruno-0.56.1/naruno/lib/perpetualtimer.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/lib/qr.py` & `naruno-0.56.1/naruno/lib/qr.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/lib/safety.py` & `naruno-0.56.1/naruno/lib/safety.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/lib/settings_system.py` & `naruno-0.56.1/naruno/lib/settings_system.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/lib/sign.py` & `naruno-0.56.1/naruno/lib/sign.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/lib/status.py` & `naruno-0.56.1/naruno/lib/status.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,18 @@
     Returns the status of the network.
     """
     a_settings = the_settings()
     currently_time = time.time()
 
     if (no_cache or a_settings["status_cache_time"] + cache_time <=
             currently_time) and (not a_settings["status_working"]
-                                 or a_settings["status_cache_time"] +
-                                 cache_time + wait_time + 2 <= currently_time):
+                                 or a_settings["status_cache_time"] + wait_time + 2 <= currently_time):
         a_settings["status_working"] = True
+        if not no_cache:
+            a_settings["status_cache_time"] = time.time()        
         save_settings(a_settings)
         first_block = (GetBlock(custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH)
                        if custom_first_block is None else custom_first_block)
 
         time.sleep(wait_time)
         new_block = (GetBlock(custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH)
                      if custom_new_block is None else custom_new_block)
@@ -60,16 +61,16 @@
 
         last_transaction_of_block = (
             str(new_block.validating_list[-1].dump_json())
             if len(new_block.validating_list) > 0 else "")
 
         status_json = {
             "status": "",
-            "first_block": str(first_block.__dict__),
-            "new_block": str(new_block.__dict__),
+            "first_block": str(first_block.dump_json()),
+            "new_block": str(new_block.dump_json()),
             "last_transaction_of_block": last_transaction_of_block,
             "transactions_of_us": transactions_of_us,
             "connected_nodes": connected_nodes,
         }
 
         status_json["status"] = ("Not working" if
                                  (first_block.sequence_number +
```

### Comparing `naruno-0.56.0/naruno/lib/verify.py` & `naruno-0.56.1/naruno/lib/verify.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/node/client/client.py` & `naruno-0.56.1/naruno/node/client/client.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/node/get_candidate_blocks.py` & `naruno-0.56.1/naruno/node/get_candidate_blocks.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/node/server/server.py` & `naruno-0.56.1/naruno/node/server/server.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/node/unl.py` & `naruno-0.56.1/naruno/node/unl.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/transactions/check/check_transaction.py` & `naruno-0.56.1/naruno/transactions/check/check_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/transactions/check/datas/check_datas.py` & `naruno-0.56.1/naruno/transactions/check/datas/check_datas.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/transactions/check/len/check_len.py` & `naruno-0.56.1/naruno/transactions/check/len/check_len.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/transactions/check/sign/check_sign.py` & `naruno-0.56.1/naruno/transactions/check/sign/check_sign.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/transactions/check/type/check_type.py` & `naruno-0.56.1/naruno/transactions/check/type/check_type.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/transactions/cleaner.py` & `naruno-0.56.1/naruno/transactions/cleaner.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/transactions/get_transaction.py` & `naruno-0.56.1/naruno/transactions/get_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/transactions/my_transactions/check_proof.py` & `naruno-0.56.1/naruno/transactions/my_transactions/check_proof.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/transactions/my_transactions/get_my_transaction.py` & `naruno-0.56.1/naruno/transactions/my_transactions/get_my_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/transactions/my_transactions/get_proof.py` & `naruno-0.56.1/naruno/transactions/my_transactions/get_proof.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/transactions/my_transactions/save_my_transaction.py` & `naruno-0.56.1/naruno/transactions/my_transactions/save_my_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/transactions/my_transactions/save_to_my_transaction.py` & `naruno-0.56.1/naruno/transactions/my_transactions/save_to_my_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/transactions/my_transactions/sended_transaction.py` & `naruno-0.56.1/naruno/transactions/my_transactions/sended_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/transactions/my_transactions/validate_transaction.py` & `naruno-0.56.1/naruno/transactions/my_transactions/validate_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/transactions/pending/delete_pending.py` & `naruno-0.56.1/naruno/transactions/pending/delete_pending.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/transactions/pending/get_pending.py` & `naruno-0.56.1/naruno/transactions/pending/get_pending.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/transactions/pending/save_pending.py` & `naruno-0.56.1/naruno/transactions/pending/save_pending.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/transactions/pending_to_validating.py` & `naruno-0.56.1/naruno/transactions/pending_to_validating.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/transactions/print_transactions.py` & `naruno-0.56.1/naruno/transactions/print_transactions.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/transactions/process_the_transaction.py` & `naruno-0.56.1/naruno/transactions/process_the_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/transactions/send.py` & `naruno-0.56.1/naruno/transactions/send.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/transactions/transaction.py` & `naruno-0.56.1/naruno/transactions/transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/wallet/delete_current_wallet.py` & `naruno-0.56.1/naruno/wallet/delete_current_wallet.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/wallet/ellipticcurve/curve.py` & `naruno-0.56.1/naruno/wallet/ellipticcurve/curve.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/wallet/ellipticcurve/ecdsa.py` & `naruno-0.56.1/naruno/wallet/ellipticcurve/ecdsa.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/wallet/ellipticcurve/math.py` & `naruno-0.56.1/naruno/wallet/ellipticcurve/math.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/wallet/ellipticcurve/privateKey.py` & `naruno-0.56.1/naruno/wallet/ellipticcurve/privateKey.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/wallet/ellipticcurve/publicKey.py` & `naruno-0.56.1/naruno/wallet/ellipticcurve/publicKey.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/wallet/ellipticcurve/signature.py` & `naruno-0.56.1/naruno/wallet/ellipticcurve/signature.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/wallet/ellipticcurve/utils/binary.py` & `naruno-0.56.1/naruno/wallet/ellipticcurve/utils/binary.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/wallet/ellipticcurve/utils/compatibility.py` & `naruno-0.56.1/naruno/wallet/ellipticcurve/utils/compatibility.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/wallet/ellipticcurve/utils/der.py` & `naruno-0.56.1/naruno/wallet/ellipticcurve/utils/der.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/wallet/ellipticcurve/utils/oid.py` & `naruno-0.56.1/naruno/wallet/ellipticcurve/utils/oid.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/wallet/get_saved_wallet.py` & `naruno-0.56.1/naruno/wallet/get_saved_wallet.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/wallet/print_wallets.py` & `naruno-0.56.1/naruno/wallet/print_wallets.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/wallet/save_wallet_list.py` & `naruno-0.56.1/naruno/wallet/save_wallet_list.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/wallet/wallet_create.py` & `naruno-0.56.1/naruno/wallet/wallet_create.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/wallet/wallet_delete.py` & `naruno-0.56.1/naruno/wallet/wallet_delete.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/wallet/wallet_import.py` & `naruno-0.56.1/naruno/wallet/wallet_import.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno/wallet/wallet_selector.py` & `naruno-0.56.1/naruno/wallet/wallet_selector.py`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/naruno.egg-info/PKG-INFO` & `naruno-0.56.1/naruno.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naruno
-Version: 0.56.0
+Version: 0.56.1
 Summary: Naruno is a lightning-fast, secure, and scalable blockchain that is able to create transaction proofs and verification via raw data and timestamp. We remove the archive nodes and lazy web3 integrations. With Naruno everyone can get the proof (5-10MB) of their transactions via their nodes and after everyone can use in another node for verification the raw data and timestamp. Also you can integrate your web3 applications with 4 code lines (just python for now) via our remote app system.
 Home-page: https://github.com/Naruno/Naruno
 Author: Naruno Developers
 Author-email: onur.atakan.ulusoy@naruno.org
 License: MPL-2.0
 Description: <p align="center">
           <a href="https://github.com/Naruno/Naruno">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: naruno Version: 0.56.0 Summary: Naruno is a
+Metadata-Version: 2.1 Name: naruno Version: 0.56.1 Summary: Naruno is a
 lightning-fast, secure, and scalable blockchain that is able to create
 transaction proofs and verification via raw data and timestamp. We remove the
 archive nodes and lazy web3 integrations. With Naruno everyone can get the
 proof (5-10MB) of their transactions via their nodes and after everyone can use
 in another node for verification the raw data and timestamp. Also you can
 integrate your web3 applications with 4 code lines (just python for now) via
 our remote app system. Home-page: https://github.com/Naruno/Naruno Author:
```

### Comparing `naruno-0.56.0/naruno.egg-info/SOURCES.txt` & `naruno-0.56.1/naruno.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `naruno-0.56.0/setup.py` & `naruno-0.56.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup
 
 setup(
     author="Naruno Developers",
     author_email="onur.atakan.ulusoy@naruno.org",
     packages=["naruno"],
     name="naruno",
-    version="0.56.0",
+    version="0.56.1",
     url="https://github.com/Naruno/Naruno",
     description=
     "Naruno is a lightning-fast, secure, and scalable blockchain that is able to create transaction proofs and verification via raw data and timestamp. We remove the archive nodes and lazy web3 integrations. With Naruno everyone can get the proof (5-10MB) of their transactions via their nodes and after everyone can use in another node for verification the raw data and timestamp. Also you can integrate your web3 applications with 4 code lines (just python for now) via our remote app system.",
     keywords=[
         "python",
         "cryptography",
         "blockchain",
```

