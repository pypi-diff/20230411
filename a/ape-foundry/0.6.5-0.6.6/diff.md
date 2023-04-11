# Comparing `tmp/ape-foundry-0.6.5.tar.gz` & `tmp/ape-foundry-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-foundry-0.6.5.tar", last modified: Mon Apr  3 23:16:38 2023, max compression
+gzip compressed data, was "ape-foundry-0.6.6.tar", last modified: Tue Apr 11 14:47:15 2023, max compression
```

## Comparing `ape-foundry-0.6.5.tar` & `ape-foundry-0.6.6.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 23:16:38.361388 ape-foundry-0.6.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 23:16:38.349388 ape-foundry-0.6.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 23:16:38.349388 ape-foundry-0.6.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 23:16:38.349388 ape-foundry-0.6.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-04-03 23:16:38.361388 ape-foundry-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 23:16:38.349388 ape-foundry-0.6.5/ape_foundry/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/ape_foundry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/ape_foundry/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/ape_foundry/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    26359 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/ape_foundry/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/ape_foundry/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-03 23:16:38.000000 ape-foundry-0.6.5/ape_foundry/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 23:16:38.349388 ape-foundry-0.6.5/ape_foundry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-04-03 23:16:38.000000 ape-foundry-0.6.5/ape_foundry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-04-03 23:16:38.000000 ape-foundry-0.6.5/ape_foundry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 23:16:38.000000 ape-foundry-0.6.5/ape_foundry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 23:16:38.000000 ape-foundry-0.6.5/ape_foundry.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-03 23:16:38.000000 ape-foundry-0.6.5/ape_foundry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-03 23:16:38.000000 ape-foundry-0.6.5/ape_foundry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-03 23:16:38.361388 ape-foundry-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 23:16:38.349388 ape-foundry-0.6.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/ape-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 23:16:38.345388 ape-foundry-0.6.5/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 23:16:38.345388 ape-foundry-0.6.5/tests/data/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 23:16:38.345388 ape-foundry-0.6.5/tests/data/contracts/ethereum/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 23:16:38.349388 ape-foundry-0.6.5/tests/data/contracts/ethereum/local/
--rw-r--r--   0 runner    (1001) docker     (123)    28687 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/local/contract_a.json
--rw-r--r--   0 runner    (1001) docker     (123)    27536 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/local/contract_b.json
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/local/contract_c.json
--rw-r--r--   0 runner    (1001) docker     (123)    33356 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/local/solidity_contract.json
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/local/token_a.json
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/local/token_b.json
--rw-r--r--   0 runner    (1001) docker     (123)    28197 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/local/vyper_contract.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 23:16:38.345388 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 23:16:38.361388 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json
--rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json
--rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json
--rw-r--r--   0 runner    (1001) docker     (123)    17042 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json
--rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json
--rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json
--rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4a672a16dEf4BAa3907BBF6f43C868297b111e5B.json
--rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json
--rw-r--r--   0 runner    (1001) docker     (123)    19792 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json
--rw-r--r--   0 runner    (1001) docker     (123)    44429 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json
--rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json
--rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json
--rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json
--rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json
--rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json
--rw-r--r--   0 runner    (1001) docker     (123)    14160 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json
--rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json
--rw-r--r--   0 runner    (1001) docker     (123)    16307 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 23:16:38.361388 ape-foundry-0.6.5/tests/data/python/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/python/pytest_test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/python/pytest_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 23:16:38.361388 ape-foundry-0.6.5/tests/data/sources/
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/sources/TokenA.vy
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/data/sources/TokenB.vy
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/expected_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)     6875 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/test_fork_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/test_gas_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-04-03 23:15:39.000000 ape-foundry-0.6.5/tests/test_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:47:15.393011 ape-foundry-0.6.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:47:15.385011 ape-foundry-0.6.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:47:15.385011 ape-foundry-0.6.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:47:15.385011 ape-foundry-0.6.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-04-11 14:47:15.397011 ape-foundry-0.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:47:15.385011 ape-foundry-0.6.6/ape_foundry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/ape_foundry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/ape_foundry/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/ape_foundry/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26360 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/ape_foundry/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/ape_foundry/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 14:47:15.000000 ape-foundry-0.6.6/ape_foundry/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:47:15.385011 ape-foundry-0.6.6/ape_foundry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-04-11 14:47:15.000000 ape-foundry-0.6.6/ape_foundry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-04-11 14:47:15.000000 ape-foundry-0.6.6/ape_foundry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:47:15.000000 ape-foundry-0.6.6/ape_foundry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:47:15.000000 ape-foundry-0.6.6/ape_foundry.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-11 14:47:15.000000 ape-foundry-0.6.6/ape_foundry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-11 14:47:15.000000 ape-foundry-0.6.6/ape_foundry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-11 14:47:15.397011 ape-foundry-0.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:47:15.389011 ape-foundry-0.6.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/ape-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:47:15.385011 ape-foundry-0.6.6/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:47:15.385011 ape-foundry-0.6.6/tests/data/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:47:15.385011 ape-foundry-0.6.6/tests/data/contracts/ethereum/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:47:15.389011 ape-foundry-0.6.6/tests/data/contracts/ethereum/local/
+-rw-r--r--   0 runner    (1001) docker     (123)    28687 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/local/contract_a.json
+-rw-r--r--   0 runner    (1001) docker     (123)    27536 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/local/contract_b.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/local/contract_c.json
+-rw-r--r--   0 runner    (1001) docker     (123)    33356 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/local/solidity_contract.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/local/token_a.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/local/token_b.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28197 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/local/vyper_contract.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:47:15.385011 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:47:15.393011 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17042 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x4a672a16dEf4BAa3907BBF6f43C868297b111e5B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19792 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json
+-rw-r--r--   0 runner    (1001) docker     (123)    44429 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14160 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16307 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:47:15.393011 ape-foundry-0.6.6/tests/data/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/python/pytest_test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/python/pytest_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:47:15.393011 ape-foundry-0.6.6/tests/data/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/sources/TokenA.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/data/sources/TokenB.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/expected_traces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6875 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/test_fork_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/test_gas_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-04-11 14:46:27.000000 ape-foundry-0.6.6/tests/test_trace.py
```

### Comparing `ape-foundry-0.6.5/.github/ISSUE_TEMPLATE/bug.md` & `ape-foundry-0.6.6/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/.github/ISSUE_TEMPLATE/feature.md` & `ape-foundry-0.6.6/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/.github/ISSUE_TEMPLATE/work-item.md` & `ape-foundry-0.6.6/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/.github/release-drafter.yml` & `ape-foundry-0.6.6/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/.github/workflows/codeql.yml` & `ape-foundry-0.6.6/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/.github/workflows/commitlint.yaml` & `ape-foundry-0.6.6/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/.github/workflows/prtitle.yaml` & `ape-foundry-0.6.6/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/.github/workflows/publish.yaml` & `ape-foundry-0.6.6/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/.github/workflows/stale-prs.yml` & `ape-foundry-0.6.6/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/.github/workflows/test.yaml` & `ape-foundry-0.6.6/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/.gitignore` & `ape-foundry-0.6.6/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/.pre-commit-config.yaml` & `ape-foundry-0.6.6/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 -   repo: https://github.com/pre-commit/mirrors-isort
     rev: v5.10.1
     hooks:
       - id: isort
 
 -   repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
       - id: black
         name: black
 
 -   repo: https://github.com/pycqa/flake8
-    rev: 5.0.4
+    rev: 6.0.0
     hooks:
     -   id: flake8
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
     rev: v0.991
     hooks:
     -   id: mypy
```

### Comparing `ape-foundry-0.6.5/CONTRIBUTING.md` & `ape-foundry-0.6.6/CONTRIBUTING.md`

 * *Files 4% similar despite different names*

```diff
@@ -42,8 +42,8 @@
 
 It's a good idea to make pull requests early on.
 A pull request represents the start of a discussion, and doesn't necessarily need to be the final, finished submission.
 
 If you are opening a work-in-progress pull request to verify that it passes CI tests, please consider
 [marking it as a draft](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-requests#draft-pull-requests).
 
-Join the Ethereum Python [Discord](https://discord.gg/PcEJ54yX) if you have any questions.
+Join the ApeWorX [Discord](https://discord.gg/apeworx) if you have any questions.
```

### Comparing `ape-foundry-0.6.5/LICENSE` & `ape-foundry-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/PKG-INFO` & `ape-foundry-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-foundry
-Version: 0.6.5
+Version: 0.6.6
 Summary: ape-foundry: Ape network provider for Foundry
 Home-page: https://github.com/ApeWorX/ape-foundry
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ape-foundry-0.6.5/README.md` & `ape-foundry-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/ape_foundry/__init__.py` & `ape-foundry-0.6.6/ape_foundry/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,30 +24,38 @@
 @plugins.register(plugins.ProviderPlugin)
 def providers():
     yield "ethereum", LOCAL_NETWORK_NAME, FoundryProvider
 
     for network in NETWORKS:
         yield "ethereum", f"{network}-fork", FoundryForkProvider
 
-    yield "fantom", LOCAL_NETWORK_NAME, FoundryProvider
-    yield "fantom", "opera-fork", FoundryForkProvider
-    yield "fantom", "testnet-fork", FoundryForkProvider
-
     yield "arbitrum", LOCAL_NETWORK_NAME, FoundryProvider
     yield "arbitrum", "mainnet-fork", FoundryForkProvider
     yield "arbitrum", "goerli-fork", FoundryForkProvider
 
-    yield "polygon", LOCAL_NETWORK_NAME, FoundryProvider
-    yield "polygon", "mainnet-fork", FoundryForkProvider
-    yield "polygon", "mumbai-fork", FoundryForkProvider
+    yield "avalanche", LOCAL_NETWORK_NAME, FoundryProvider
+    yield "avalanche", "mainnet-fork", FoundryForkProvider
+    yield "avalanche", "fuji-fork", FoundryForkProvider
+
+    yield "bsc", LOCAL_NETWORK_NAME, FoundryProvider
+    yield "bsc", "mainnet-fork", FoundryForkProvider
+    yield "bsc", "testnet-fork", FoundryForkProvider
+
+    yield "fantom", LOCAL_NETWORK_NAME, FoundryProvider
+    yield "fantom", "opera-fork", FoundryForkProvider
+    yield "fantom", "testnet-fork", FoundryForkProvider
 
     yield "optimism", LOCAL_NETWORK_NAME, FoundryProvider
     yield "optimism", "mainnet-fork", FoundryForkProvider
     yield "optimism", "goerli-fork", FoundryForkProvider
 
+    yield "polygon", LOCAL_NETWORK_NAME, FoundryProvider
+    yield "polygon", "mainnet-fork", FoundryForkProvider
+    yield "polygon", "mumbai-fork", FoundryForkProvider
+
 
 __all__ = [
     "FoundryNetworkConfig",
     "FoundryProvider",
     "FoundryProviderError",
     "FoundrySubprocessError",
 ]
```

### Comparing `ape-foundry-0.6.5/ape_foundry/constants.py` & `ape-foundry-0.6.6/ape_foundry/constants.py`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/ape_foundry/exceptions.py` & `ape-foundry-0.6.6/ape_foundry/exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/ape_foundry/provider.py` & `ape-foundry-0.6.6/ape_foundry/provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -527,15 +527,15 @@
         ):
             return ContractLogicError(txn=txn)
 
         elif message == "Transaction ran out of gas":
             return OutOfGasError(txn=txn)
 
         elif message.startswith("execution reverted: "):
-            raise ContractLogicError(message.replace("execution reverted: ", "").strip(), txn=txn)
+            return ContractLogicError(message.replace("execution reverted: ", "").strip(), txn=txn)
 
         return VirtualMachineError(message, txn=txn)
 
     def set_block_gas_limit(self, gas_limit: int) -> bool:
         return self._make_request("evm_setBlockGasLimit", [hex(gas_limit)]) is True
 
     def set_code(self, address: AddressType, code: ContractCode) -> bool:
```

### Comparing `ape-foundry-0.6.5/ape_foundry.egg-info/PKG-INFO` & `ape-foundry-0.6.6/ape_foundry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-foundry
-Version: 0.6.5
+Version: 0.6.6
 Summary: ape-foundry: Ape network provider for Foundry
 Home-page: https://github.com/ApeWorX/ape-foundry
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ape-foundry-0.6.5/ape_foundry.egg-info/SOURCES.txt` & `ape-foundry-0.6.6/ape_foundry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/ape_foundry.egg-info/requires.txt` & `ape-foundry-0.6.6/ape_foundry.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,49 +6,49 @@
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
 hypothesis<7.0,>=6.2.0
 ape-alchemy
 ape-polygon
-black>=22.12.0
-mypy>=0.991
+black<24,>=23.3.0
+mypy<1,>=0.991
 types-requests
 types-setuptools
 types-PyYAML
-flake8>=5.0.4
-isort>=5.10.1
+flake8<7,>=6.0.0
+isort<6,>=5.10.1
 mdformat>=0.7.16
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
-Sphinx<4,>=3.4.3
-sphinx_rtd_theme<1,>=0.1.9
+Sphinx<7,>=6.1.3
+sphinx_rtd_theme<2,>=1.2.0
 towncrier<20,>=19.2.0
 setuptools
 setuptools-scm
 wheel
 twine
 commitizen
 pre-commit
 IPython
 ipdb
 
 [doc]
-Sphinx<4,>=3.4.3
-sphinx_rtd_theme<1,>=0.1.9
+Sphinx<7,>=6.1.3
+sphinx_rtd_theme<2,>=1.2.0
 towncrier<20,>=19.2.0
 
 [lint]
-black>=22.12.0
-mypy>=0.991
+black<24,>=23.3.0
+mypy<1,>=0.991
 types-requests
 types-setuptools
 types-PyYAML
-flake8>=5.0.4
-isort>=5.10.1
+flake8<7,>=6.0.0
+isort<6,>=5.10.1
 mdformat>=0.7.16
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 
 [release]
 setuptools
 setuptools-scm
```

### Comparing `ape-foundry-0.6.5/pyproject.toml` & `ape-foundry-0.6.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/setup.py` & `ape-foundry-0.6.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-import os.path
 
 from setuptools import find_packages, setup
 
 extras_require = {
     "test": [  # `test` GitHub Action jobs uses this
         "pytest>=6.0",  # Core testing package
         "pytest-xdist",  # multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
         "ape-alchemy",  # For running fork tests
         "ape-polygon",  # For running polygon fork tests
     ],
     "lint": [
-        "black>=22.12.0",  # auto-formatter and linter
-        "mypy>=0.991",  # Static type analyzer
+        "black>=23.3.0,<24",  # auto-formatter and linter
+        "mypy>=0.991,<1",  # Static type analyzer
         "types-requests",  # Needed due to mypy typeshed
         "types-setuptools",  # Needed due to mypy typeshed
         "types-PyYAML",  # Needed due to mypy typeshed
-        "flake8>=5.0.4",  # Style linter
-        "isort>=5.10.1",  # Import sorting linter
+        "flake8>=6.0.0,<7",  # Style linter
+        "isort>=5.10.1,<6",  # Import sorting linter
         "mdformat>=0.7.16",  # Auto-formatter for markdown
         "mdformat-gfm>=0.3.5",  # Needed for formatting GitHub-flavored markdown
         "mdformat-frontmatter>=0.4.1",  # Needed for frontmatters-style headers in issue templates
     ],
     "doc": [
-        "Sphinx>=3.4.3,<4",  # Documentation generator
-        "sphinx_rtd_theme>=0.1.9,<1",  # Readthedocs.org theme
+        "Sphinx>=6.1.3,<7",  # Documentation generator
+        "sphinx_rtd_theme>=1.2.0,<2",  # Readthedocs.org theme
         "towncrier>=19.2.0, <20",  # Generate release notes
     ],
     "release": [  # `release` GitHub Action job uses this
         "setuptools",  # Installation tool
         "setuptools-scm",  # Installation tool
         "wheel",  # Packaging tool
         "twine",  # Package upload tool
@@ -49,29 +48,26 @@
     extras_require["test"]
     + extras_require["lint"]
     + extras_require["doc"]
     + extras_require["release"]
     + extras_require["dev"]
 )
 
-readme_path, readme_content_type = "./README.md", "text/x-rst"
-if os.path.exists("./README.md"):
-    readme_path, readme_content_type = "./README.md", "text/markdown"
 
-with open(readme_path) as readme:
+with open("./README.md") as readme:
     long_description = readme.read()
 
 
 setup(
     name="ape-foundry",
     use_scm_version=True,
     setup_requires=["setuptools_scm"],
     description="""ape-foundry: Ape network provider for Foundry""",
     long_description=long_description,
-    long_description_content_type=readme_content_type,
+    long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-foundry",
     include_package_data=True,
     install_requires=[
         "eth-ape>=0.6.7,<0.7",
         "evm-trace>=0.1.0a13",
```

### Comparing `ape-foundry-0.6.5/tests/ape-config.yaml` & `ape-foundry-0.6.6/tests/ape-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/conftest.py` & `ape-foundry-0.6.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/local/contract_a.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/local/contract_a.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/local/contract_b.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/local/contract_b.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/local/contract_c.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/local/contract_c.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/local/solidity_contract.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/local/solidity_contract.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/local/token_a.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/local/token_a.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/local/token_b.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/local/token_b.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/local/vyper_contract.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/local/vyper_contract.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json` & `ape-foundry-0.6.6/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/python/pytest_tests.py` & `ape-foundry-0.6.6/tests/data/python/pytest_tests.py`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/sources/TokenA.vy` & `ape-foundry-0.6.6/tests/data/sources/TokenA.vy`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/data/sources/TokenB.vy` & `ape-foundry-0.6.6/tests/data/sources/TokenB.vy`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/expected_traces.py` & `ape-foundry-0.6.6/tests/expected_traces.py`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/test_fork_provider.py` & `ape-foundry-0.6.6/tests/test_fork_provider.py`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/test_gas_report.py` & `ape-foundry-0.6.6/tests/test_gas_report.py`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/test_provider.py` & `ape-foundry-0.6.6/tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.6.5/tests/test_trace.py` & `ape-foundry-0.6.6/tests/test_trace.py`

 * *Files identical despite different names*

