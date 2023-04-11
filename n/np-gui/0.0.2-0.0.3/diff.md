# Comparing `tmp/np_gui-0.0.2.tar.gz` & `tmp/np_gui-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_gui-0.0.2.tar", max compression
+gzip compressed data, was "np_gui-0.0.3.tar", max compression
```

## Comparing `np_gui-0.0.2.tar` & `np_gui-0.0.3.tar`

### file list

```diff
@@ -1,750 +1,305 @@
--rw-r--r--   0        0        0     1781 2023-04-10 23:46:40.784386 np_gui-0.0.2/README.md
--rw-r--r--   0        0        0       59 2023-04-10 21:31:13.544683 np_gui-0.0.2/np_gui/.git/COMMIT_EDITMSG
--rw-r--r--   0        0        0       23 2023-04-07 17:25:22.153178 np_gui-0.0.2/np_gui/.git/HEAD
--rw-r--r--   0        0        0       92 2023-04-07 17:25:22.153178 np_gui-0.0.2/np_gui/.git/config
--rw-r--r--   0        0        0       73 2023-04-07 17:25:22.153178 np_gui-0.0.2/np_gui/.git/description
--rwxr-xr-x   0        0        0      478 2023-04-07 17:25:22.149178 np_gui-0.0.2/np_gui/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0        0        0      896 2023-04-07 17:25:22.153178 np_gui-0.0.2/np_gui/.git/hooks/commit-msg.sample
--rwxr-xr-x   0        0        0     4655 2023-04-07 17:25:22.153178 np_gui-0.0.2/np_gui/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0        0        0      189 2023-04-07 17:25:22.149178 np_gui-0.0.2/np_gui/.git/hooks/post-update.sample
--rwxr-xr-x   0        0        0      424 2023-04-07 17:25:22.153178 np_gui-0.0.2/np_gui/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0        0        0     1643 2023-04-07 17:25:22.153178 np_gui-0.0.2/np_gui/.git/hooks/pre-commit.sample
--rwxr-xr-x   0        0        0      416 2023-04-07 17:25:22.149178 np_gui-0.0.2/np_gui/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0        0        0     1374 2023-04-07 17:25:22.153178 np_gui-0.0.2/np_gui/.git/hooks/pre-push.sample
--rwxr-xr-x   0        0        0     4898 2023-04-07 17:25:22.149178 np_gui-0.0.2/np_gui/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0        0        0      544 2023-04-07 17:25:22.153178 np_gui-0.0.2/np_gui/.git/hooks/pre-receive.sample
--rwxr-xr-x   0        0        0     1492 2023-04-07 17:25:22.149178 np_gui-0.0.2/np_gui/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0        0        0     2783 2023-04-07 17:25:22.153178 np_gui-0.0.2/np_gui/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0        0        0     3650 2023-04-07 17:25:22.153178 np_gui-0.0.2/np_gui/.git/hooks/update.sample
--rw-r--r--   0        0        0    35065 2023-04-10 21:31:13.528683 np_gui-0.0.2/np_gui/.git/index
--rw-r--r--   0        0        0      240 2023-04-07 17:25:22.149178 np_gui-0.0.2/np_gui/.git/info/exclude
--rw-r--r--   0        0        0      407 2023-04-10 21:31:13.544683 np_gui-0.0.2/np_gui/.git/logs/HEAD
--rw-r--r--   0        0        0      407 2023-04-10 21:31:13.544683 np_gui-0.0.2/np_gui/.git/logs/refs/heads/master
--rw-r--r--   0        0        0      108 2023-04-07 17:26:16.100323 np_gui-0.0.2/np_gui/.git/objects/00/1f8338e6e11764ad37bb83d791d1efa98d96fe
--rw-r--r--   0        0        0      335 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/00/ba8f1f945e6ed05eb92c065cc9e85e6086fe82
--rw-r--r--   0        0        0     9098 2023-04-07 17:26:16.220321 np_gui-0.0.2/np_gui/.git/objects/00/f3f5a680fa8de33428812a86992d2e500690cb
--rw-r--r--   0        0        0       99 2023-04-07 17:26:16.160322 np_gui-0.0.2/np_gui/.git/objects/01/dc810d9fcf5cc45bf04bc9ffaa0055ba71b435
--rw-r--r--   0        0        0      412 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/03/790b5786744b033f13b8f0ccccdca2f79e5a7c
--rw-r--r--   0        0        0      237 2023-04-07 17:26:16.152322 np_gui-0.0.2/np_gui/.git/objects/04/36df5138c20bafe3ffea2e0954602312d8b9d1
--rw-r--r--   0        0        0     7063 2023-04-07 17:26:16.228321 np_gui-0.0.2/np_gui/.git/objects/05/94be6ebe5760366bbdba8c18d95e265851e08f
--rw-r--r--   0        0        0      219 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/07/f3e06427f6313e350b9fc6ef8b26676990fdc2
--rw-r--r--   0        0        0      189 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/08/bbbf71e87b546c20a076bc9a5bd3db83bee35e
--rw-r--r--   0        0        0      310 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/09/92e17be3c808b3da891366671f3558f2e573b7
--rw-r--r--   0        0        0      236 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/0b/daac7f658e75da29b011c93c74df4f39ec9225
--rw-r--r--   0        0        0     3230 2023-04-07 17:26:16.100323 np_gui-0.0.2/np_gui/.git/objects/0c/1d089682c47a4c7a4d973c2ffe4f325aa286a8
--rw-r--r--   0        0        0      293 2023-04-07 17:26:16.100323 np_gui-0.0.2/np_gui/.git/objects/0c/430ffe3e400c379cfaf35283d95fc1ca25915e
--rw-r--r--   0        0        0   525549 2023-04-07 17:26:16.200321 np_gui-0.0.2/np_gui/.git/objects/0d/04b502439cc71d41bc9dd93b50545a22ecbc13
--rw-r--r--   0        0        0      887 2023-04-10 21:31:13.508683 np_gui-0.0.2/np_gui/.git/objects/0d/2f18f4f868fd7172a78c62903ab798a4738257
--rw-r--r--   0        0        0      309 2023-04-07 17:26:16.296320 np_gui-0.0.2/np_gui/.git/objects/0d/3ccb7c8854fd447932a5cd60bacf1216eb95eb
--rw-r--r--   0        0        0      296 2023-04-07 17:26:16.156322 np_gui-0.0.2/np_gui/.git/objects/0d/54c4086b8e54bf55b7ddb1587708fdcb934552
--rw-r--r--   0        0        0      353 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/0d/8c4d03263302e82840b8fdb5375bc83ae2cbf8
--rw-r--r--   0        0        0     3150 2023-04-07 17:26:16.220321 np_gui-0.0.2/np_gui/.git/objects/0d/cf1133cd7b82c81d790bd3b165e4bef0497364
--rw-r--r--   0        0        0    16319 2023-04-07 17:26:16.172321 np_gui-0.0.2/np_gui/.git/objects/0e/93a39aa13183bc13439f3986aa774c759debd3
--rw-r--r--   0        0        0      405 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/0e/d100e43c20a795386fffec2e38b738b913300b
--rw-r--r--   0        0        0     3224 2023-04-07 17:26:16.208321 np_gui-0.0.2/np_gui/.git/objects/0e/ddaeb07d19bffb50884d7bd7996418b6461a09
--rw-r--r--   0        0        0      203 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/0f/d75a690d7d51e73ee18f8430ca2319a02be326
--rw-r--r--   0        0        0      350 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/10/81342ccebd09c1ead735564d1d03bb4a5128e1
--rw-r--r--   0        0        0      203 2023-04-07 17:26:16.156322 np_gui-0.0.2/np_gui/.git/objects/10/9b372b6634ab37c7c2fc84cb69fbdfbcfca651
--rw-r--r--   0        0        0      365 2023-04-07 17:26:16.152322 np_gui-0.0.2/np_gui/.git/objects/10/b508193aae46a8e91b8120417abf1387380780
--rw-r--r--   0        0        0      182 2023-04-10 21:31:13.524683 np_gui-0.0.2/np_gui/.git/objects/10/c63be410386ca4de77ce5539ce72ce76de8796
--rw-r--r--   0        0        0      172 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/11/43e564808ca46fd3b6728ea7b29e65669e6cde
--rw-r--r--   0        0        0     1364 2023-04-10 21:31:13.504683 np_gui-0.0.2/np_gui/.git/objects/11/c011fe297f2395dd1787a60a64f1b9b8b24916
--rw-r--r--   0        0        0      149 2023-04-07 17:26:16.100323 np_gui-0.0.2/np_gui/.git/objects/11/fd399cbab597743a77be794d4965b4359e1c7e
--rw-r--r--   0        0        0      368 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/13/5101d2967e39efdea88037958ea1ca730ca41e
--rw-r--r--   0        0        0    15262 2023-04-07 17:26:16.204321 np_gui-0.0.2/np_gui/.git/objects/13/706529075e87c7e1fe16f36b9bc94e4869ef2d
--rw-r--r--   0        0        0      303 2023-04-07 17:26:16.208321 np_gui-0.0.2/np_gui/.git/objects/15/08eb44781aaccb3bb04f8f1b9a204356d8bc38
--rw-r--r--   0        0        0      188 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/15/b15f176a3c1b6d658bb8822c058b610b4b20db
--rw-r--r--   0        0        0      220 2023-04-07 17:26:16.156322 np_gui-0.0.2/np_gui/.git/objects/16/7ed398e727d7038c9b562ef8d9001b8295ccc8
--rw-r--r--   0        0        0      323 2023-04-07 17:26:16.156322 np_gui-0.0.2/np_gui/.git/objects/16/8941bd5497e7458a6d5b8eef8e55615c106187
--rw-r--r--   0        0        0       89 2023-04-07 17:26:16.300320 np_gui-0.0.2/np_gui/.git/objects/17/627b11cc4ef90eaf6a04082895c029bf9542f6
--rw-r--r--   0        0        0      335 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/17/e8632fbb914d5e8b851574e26ec93979cb41fa
--rw-r--r--   0        0        0      302 2023-04-07 17:26:16.156322 np_gui-0.0.2/np_gui/.git/objects/18/7053361943f1ab3fed47738f4a8ab1a4f3ee21
--rw-r--r--   0        0        0      178 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/18/b8aabd6df1df6baff18a03b5f7ccb1ed095753
--rw-r--r--   0        0        0      299 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/19/5d564c9549aa6494cca1e88464b0c986d0c3c5
--rw-r--r--   0        0        0      170 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/1a/c68478bc906074743ba889f2180a0f3a82e551
--rw-r--r--   0        0        0      248 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/1c/484b83e18a4d90dc29548c6b6d23c7ad1f382c
--rw-r--r--   0        0        0      137 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/1c/c5c2bdda01f0b6c14ddc7b4c0634c09363b7d6
--rw-r--r--   0        0        0     2593 2023-04-07 17:26:16.216321 np_gui-0.0.2/np_gui/.git/objects/1d/768259cdbc1200244462dcd508e120087972fb
--rw-r--r--   0        0        0      380 2023-04-07 17:26:16.152322 np_gui-0.0.2/np_gui/.git/objects/1e/4100a5d3930080e2575cd47f501e347d322362
--rw-r--r--   0        0        0     2423 2023-04-07 17:26:16.224321 np_gui-0.0.2/np_gui/.git/objects/1e/418c8c2229d12b62df6fec6412818c2ea4c263
--rw-r--r--   0        0        0       94 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/1e/8b72de24f3e9fbabe96b993fef33c540d5961a
--rw-r--r--   0        0        0   216238 2023-04-07 17:26:16.288320 np_gui-0.0.2/np_gui/.git/objects/1f/eb3766de2f80e661f4502baac1f65f5e162b42
--rw-r--r--   0        0        0      105 2023-04-07 17:26:16.220321 np_gui-0.0.2/np_gui/.git/objects/20/f36035bbb0e1542e6e80718f8481d2efe59aae
--rw-r--r--   0        0        0      171 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/21/67d3ed7945410a523061a1d38636b726608e1c
--rw-r--r--   0        0        0      307 2023-04-07 17:26:16.152322 np_gui-0.0.2/np_gui/.git/objects/23/776c1541203723abe5a83bad39a7243a18df5b
--rw-r--r--   0        0        0      252 2023-04-07 17:26:16.208321 np_gui-0.0.2/np_gui/.git/objects/23/fc755efa2bc76d22dacf9e5be84d562ffd584f
--rw-r--r--   0        0        0      205 2023-04-07 17:26:16.152322 np_gui-0.0.2/np_gui/.git/objects/24/84bf8f696c81119a1465e72aa8341247d7add5
--rw-r--r--   0        0        0      307 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/24/f82fe319519b00e8d66c3ec1c9848f62c537eb
--rw-r--r--   0        0        0      299 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/25/526d1b07fd0c758a83f41c708c8d6bee932bcc
--rw-r--r--   0        0        0      291 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/26/09816ab2801d115ff31d2173f942fcfe8c5792
--rw-r--r--   0        0        0      281 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/26/46d9d7b87813ff940f1fffeec1df38c389b9d0
--rw-r--r--   0        0        0      221 2023-04-07 17:26:16.216321 np_gui-0.0.2/np_gui/.git/objects/26/e1335951dd1032f79e39a3d07d1d5d099e076b
--rw-r--r--   0        0        0      176 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/27/0e8ad651d3198426a52a741c240ad4bc83145e
--rw-r--r--   0        0        0     1051 2023-04-07 17:26:16.220321 np_gui-0.0.2/np_gui/.git/objects/27/9cbdb60342ad4a676f29539c18b9f50fb88518
--rw-r--r--   0        0        0      328 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/27/b616680a23e81dd7d669ea7b83bf2c15db7262
--rw-r--r--   0        0        0      255 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/28/1b31c308ea2950e0e84ca850d3d39677537f3e
--rw-r--r--   0        0        0      516 2023-04-07 17:26:16.100323 np_gui-0.0.2/np_gui/.git/objects/28/247f8d1f8f288eb1b0ea22d82562e612761712
--rw-r--r--   0        0        0      219 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/28/39c763483cc8611157636a902a44a8f3033fc7
--rw-r--r--   0        0        0      264 2023-04-07 17:26:16.100323 np_gui-0.0.2/np_gui/.git/objects/28/f583e2165abb5d0c8e2e1ad669163d0c38ed1d
--rw-r--r--   0        0        0      224 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/29/c0b8c1b95f39663c6286ac46f87b58bd9c4c3d
--rw-r--r--   0        0        0      275 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/2a/42de29ca6b0e616c5de5f683567c14cf1f149b
--rw-r--r--   0        0        0      338 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/2c/96759353e659f10a12c142425cfbd195239c48
--rw-r--r--   0        0        0      296 2023-04-07 17:26:16.156322 np_gui-0.0.2/np_gui/.git/objects/2c/c07b3cbc513d7d0da02aa498d3f4fdbdad772d
--rw-r--r--   0        0        0      353 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/2d/001d28fdeda2abc04b373ae8688c0f19fcb96d
--rw-r--r--   0        0        0      167 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/2d/546af64a65f6507a929f3ce5c39709cfdd39e6
--rw-r--r--   0        0        0      300 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/2d/c9a6e0f721811c7b45d59029fe46401e7937de
--rw-r--r--   0        0        0      210 2023-04-07 17:26:16.156322 np_gui-0.0.2/np_gui/.git/objects/2d/d3d8e560e3a5fe5e4818ed8035f882163bd987
--rw-r--r--   0        0        0      275 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/2e/13c842bb56f37ee0fcf2457d6a638a1aceb473
--rw-r--r--   0        0        0     1848 2023-04-07 17:26:16.228321 np_gui-0.0.2/np_gui/.git/objects/2e/4b30d921c3343a19744726882b85cdf3621f5c
--rw-r--r--   0        0        0      369 2023-04-07 17:26:16.204321 np_gui-0.0.2/np_gui/.git/objects/2f/fd96f5232673b9427f89a28e36996e1ee8233f
--rw-r--r--   0        0        0      290 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/30/569bb11604212765937cdb59598e6994b23f02
--rw-r--r--   0        0        0      265 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/30/6eb267393e3bc5a6d7d7035ed7498c9ba1d5be
--rw-r--r--   0        0        0      279 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/32/1ffdab21749534ced86460535ce7b85dc8e949
--rw-r--r--   0        0        0      231 2023-04-07 17:26:16.100323 np_gui-0.0.2/np_gui/.git/objects/32/5cf993929a2c06ef9b5722f4bb893f7b415b2b
--rw-r--r--   0        0        0    12952 2023-04-07 17:26:16.204321 np_gui-0.0.2/np_gui/.git/objects/32/5fb1d6f511cd1b93a8926b03238a9ac40f4a80
--rw-r--r--   0        0        0      392 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/33/4557d3dbc72c3b3d630d25027dfe55a6b08372
--rw-r--r--   0        0        0      226 2023-04-07 17:26:16.160322 np_gui-0.0.2/np_gui/.git/objects/33/ab39ac5d8879ea06e69faa75077d603c75e124
--rw-r--r--   0        0        0      130 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/34/569ba182b68041cacfd3c0df5fa06768ddeb8b
--rw-r--r--   0        0        0      186 2023-04-07 17:26:16.152322 np_gui-0.0.2/np_gui/.git/objects/34/7d9bb090a971c0862df6ea00751443c1ff988b
--rw-r--r--   0        0        0      197 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/34/c3ce89ccb73f687194cb8c4c176bd1586c8a97
--rw-r--r--   0        0        0      258 2023-04-07 17:26:16.156322 np_gui-0.0.2/np_gui/.git/objects/35/d89c5904bb598d20b0f7256ff9c78de99cdedc
--rw-r--r--   0        0        0      380 2023-04-07 17:26:16.156322 np_gui-0.0.2/np_gui/.git/objects/36/c9d1e77da84280881025cb501270a2585d07d5
--rw-r--r--   0        0        0      388 2023-04-07 17:26:16.156322 np_gui-0.0.2/np_gui/.git/objects/37/6a18444b3b81cd85606566d457e58f72428214
--rw-r--r--   0        0        0      106 2023-04-07 17:26:16.300320 np_gui-0.0.2/np_gui/.git/objects/38/7e944c0e4f312ae9b427a3a740aff752e9e90d
--rw-r--r--   0        0        0      387 2023-04-07 17:26:16.152322 np_gui-0.0.2/np_gui/.git/objects/38/815535e243f4f5d211307932ee6775c315d7b2
--rw-r--r--   0        0        0      412 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/39/2584a7d4ea1aa426c745a2707d9bd9d5065a77
--rw-r--r--   0        0        0      370 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/39/5ed45165cd127c78dab829847308d76522e027
--rw-r--r--   0        0        0      153 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/39/c200d2c7e7d2bd7ab2f49c4667b34c818aa8aa
--rw-r--r--   0        0        0      182 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/39/d8a5cfd40b92a5113e63a83094b74db0f79d29
--rw-r--r--   0        0        0      202 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/3b/855bd6f22ab79c16083dd8ccbe12197cebc1f3
--rw-r--r--   0        0        0      256 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/3b/c85e40ac22cb3d6935a28c3478f0ea319c9fdf
--rw-r--r--   0        0        0      156 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/3b/d33cc750e31958d31601a72a5303b2f46fc58e
--rw-r--r--   0        0        0      219 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/3c/87f3c1eb90695afc70d6b83fb99678f623341e
--rw-r--r--   0        0        0    15335 2023-04-07 17:26:16.204321 np_gui-0.0.2/np_gui/.git/objects/3c/a8edf522757fafe25bea2f0b7344f4d8acd582
--rw-r--r--   0        0        0      273 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/3e/4d31b9299286d991e00cdb893e60cedcad66d8
--rw-r--r--   0        0        0      149 2023-04-07 17:26:16.296320 np_gui-0.0.2/np_gui/.git/objects/3e/bb27a818208673f2476e7ddddaef4e2355156d
--rw-r--r--   0        0        0      284 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/3f/0bb25e783c6f4450dbd53f169900909672f672
--rw-r--r--   0        0        0      133 2023-04-07 17:26:16.100323 np_gui-0.0.2/np_gui/.git/objects/3f/d7fdcd6c28ab7f7940b8005e480fc13d9dee05
--rw-r--r--   0        0        0      371 2023-04-07 17:26:16.152322 np_gui-0.0.2/np_gui/.git/objects/40/3c22dc0b25732eac208a9f9d7c84d89cf9542e
--rw-r--r--   0        0        0     1313 2023-04-07 17:26:16.224321 np_gui-0.0.2/np_gui/.git/objects/40/66129bf24ca86c1eb0cb8cf55f8730b92ca4d8
--rw-r--r--   0        0        0      154 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/41/083940f0747df26bca0e3dcf77c12f571bf209
--rw-r--r--   0        0        0      296 2023-04-07 17:26:16.100323 np_gui-0.0.2/np_gui/.git/objects/42/57884f7f419ba9f7d07a827d6a74e8e3dde39f
--rw-r--r--   0        0        0      292 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/42/646416f76601483b882bccbe25747a5065dc74
--rw-r--r--   0        0        0      278 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/42/c86b5717aa4c9166078d1e96442e23b8609524
--rw-r--r--   0        0        0      263 2023-04-07 17:26:16.152322 np_gui-0.0.2/np_gui/.git/objects/42/e49964f468a03bb8aa5f0e3e7e78d6dcf93060
--rw-r--r--   0        0        0      356 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/43/0aca1d191113b577c298141a7e9ad1717dafd9
--rw-r--r--   0        0        0      307 2023-04-07 17:26:16.156322 np_gui-0.0.2/np_gui/.git/objects/43/596aef1f3c3b433979d67407cf5e14af1b70ee
--rw-r--r--   0        0        0     1322 2023-04-07 17:26:16.296320 np_gui-0.0.2/np_gui/.git/objects/46/2db4bd2978821d5961fc58cda742a30fa86621
--rw-r--r--   0        0        0      267 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/48/4ac08755bb72fc3909ff88a3ad5c2a1ccd83a2
--rw-r--r--   0        0        0      191 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/48/a78a80a0feac93e46f342fc93db9e2af71168d
--rw-r--r--   0        0        0      266 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/49/553fca5ae950b4b50b5f72bfa9835f50618a4d
--rw-r--r--   0        0        0      267 2023-04-07 17:26:16.100323 np_gui-0.0.2/np_gui/.git/objects/49/920fc5f3505862e0e32b9e38922c7ccafa27ab
--rw-r--r--   0        0        0      543 2023-04-07 17:26:16.172321 np_gui-0.0.2/np_gui/.git/objects/4a/fbfb72ff6198d0f1381c8cf3f2c022242ce9cc
--rw-r--r--   0        0        0      234 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/4b/73afaeccf038a8433dafcde44d5b7679e73860
--rw-r--r--   0        0        0      226 2023-04-07 17:26:16.156322 np_gui-0.0.2/np_gui/.git/objects/4b/f12f8848c08094fdcef03c75db473551611617
--rw-r--r--   0        0        0     1812 2023-04-10 21:31:13.504683 np_gui-0.0.2/np_gui/.git/objects/4c/aa8b073c2ad3d74f0ea5498247b92e94f7350f
--rw-r--r--   0        0        0      317 2023-04-07 17:26:16.100323 np_gui-0.0.2/np_gui/.git/objects/4c/bc3a92df76587ad02fe1ef39502e4563fc55bc
--rw-r--r--   0        0        0     5141 2023-04-07 17:26:16.220321 np_gui-0.0.2/np_gui/.git/objects/4d/42199a7930812764ea8a28908bd6b5c4c60f2f
--rw-r--r--   0        0        0      286 2023-04-07 17:26:16.156322 np_gui-0.0.2/np_gui/.git/objects/4d/9618d5c36f9b6d7069be82021b01a829dd424a
--rw-r--r--   0        0        0      211 2023-04-07 17:26:16.160322 np_gui-0.0.2/np_gui/.git/objects/4e/091d434c0823ce0ade18afb029893ac344d7a1
--rw-r--r--   0        0        0      178 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/4f/6f20ac8a9c4e665dfc7e11efbf3a8a3d4b7da6
--rw-r--r--   0        0        0      347 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/4f/bb8753850b7e88c0ef7b7b65c920055376c861
--rw-r--r--   0        0        0      387 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/50/a8196caece5913b1adfde6dfb80410db81aeca
--rw-r--r--   0        0        0      226 2023-04-07 17:26:16.156322 np_gui-0.0.2/np_gui/.git/objects/52/2215e3f6f10f96f67ccc98191385252a03365f
--rw-r--r--   0        0        0      200 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/53/3de7b795a4c1886a60cf0679f0d065dbeebad1
--rw-r--r--   0        0        0   568499 2023-04-07 17:26:16.280320 np_gui-0.0.2/np_gui/.git/objects/53/fbd10dcbfbf956da1a7e79568e0330d0dfbdcc
--rw-r--r--   0        0        0     1116 2023-04-07 17:26:16.216321 np_gui-0.0.2/np_gui/.git/objects/55/add2b7e4d203fa8b0885c0217a4bb8c9e361fd
--rw-r--r--   0        0        0      239 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/57/61b7e4c3b7ea4f1b77cae0b2d47e841ea65100
--rw-r--r--   0        0        0     2754 2023-04-07 17:26:16.228321 np_gui-0.0.2/np_gui/.git/objects/57/9ac9df617dde14d731ec2580a416050b0f4568
--rw-r--r--   0        0        0      270 2023-04-07 17:26:16.100323 np_gui-0.0.2/np_gui/.git/objects/57/de0e519ce8e9c543a2e85c8a4f7b1de7bdd855
--rw-r--r--   0        0        0      237 2023-04-07 17:26:16.100323 np_gui-0.0.2/np_gui/.git/objects/58/54ee253723a970fbeda894c0f6423531781005
--rw-r--r--   0        0        0      228 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/59/63c17c93305fc97a6d935bcf0e7d2cd72d1f69
--rw-r--r--   0        0        0      249 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/5b/354a2e0f6ddc9d186b1d5289c2be2db3804563
--rw-r--r--   0        0        0      361 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/5b/5c1b3ff6039c4515d09820fe68c2138ea4d280
--rw-r--r--   0        0        0      184 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/5c/e309a810a24f0dcf40e9d77a154d57c6ec842a
--rw-r--r--   0        0        0      241 2023-04-07 17:26:16.100323 np_gui-0.0.2/np_gui/.git/objects/5d/c0ca55843384e4079c71486850631fc735a0dd
--rw-r--r--   0        0        0      165 2023-04-07 17:26:16.100323 np_gui-0.0.2/np_gui/.git/objects/5e/5d49bacfd25cfef8122112a896f8f501bb8375
--rw-r--r--   0        0        0      246 2023-04-07 17:26:16.160322 np_gui-0.0.2/np_gui/.git/objects/5e/99675426c614c58a9e2a98cd46994d62a53daa
--rw-r--r--   0        0        0      350 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/5e/aedcf4155acaa49606be68fbab75bcab5ae06c
--rw-r--r--   0        0        0      258 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/5e/ecaa117ae7ae5100e17d94da2fab2b44beeb71
--rw-r--r--   0        0        0      262 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/5f/cfc96fe8df9aa29fb2afa96e5dc3938aed9419
--rw-r--r--   0        0        0      273 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/60/2510ea0347e2dcc7acebd92f03d328f048d6ac
--rw-r--r--   0        0        0     4188 2023-04-07 17:26:16.208321 np_gui-0.0.2/np_gui/.git/objects/60/3f6a8798e7f7b07f32dfd1e0ad785b85bc7010
--rw-r--r--   0        0        0      186 2023-04-07 17:26:16.208321 np_gui-0.0.2/np_gui/.git/objects/61/5393ac8dda791f331ec6961b84316afcabb1cd
--rw-r--r--   0        0        0      243 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/61/ac52662ce5131011b5a1c4f93ab7d0e374f02f
--rw-r--r--   0        0        0      392 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/62/01c60c62f6422b5daf1f15d69f3870a9507977
--rw-r--r--   0        0        0   103605 2023-04-07 17:26:16.212321 np_gui-0.0.2/np_gui/.git/objects/62/4bca829eef53e924e47d572c5b87022c86657d
--rw-r--r--   0        0        0      128 2023-04-07 17:26:16.296320 np_gui-0.0.2/np_gui/.git/objects/62/62ae55a38ea96ecbfdea31b78c97ab2901b3d3
--rw-r--r--   0        0        0      278 2023-04-07 17:26:16.100323 np_gui-0.0.2/np_gui/.git/objects/63/74ee5dfec542460a643d0f227a9ee0699c05be
--rw-r--r--   0        0        0     1053 2023-04-07 17:26:16.200321 np_gui-0.0.2/np_gui/.git/objects/64/5fc7b63ec6ce2c2993d67949e964504fb29395
--rw-r--r--   0        0        0      186 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/64/959b967991cc96d2adc088db1ac0a18e19f26b
--rw-r--r--   0        0        0      361 2023-04-07 17:26:16.156322 np_gui-0.0.2/np_gui/.git/objects/64/e06b01228ef2b21bba6dece4f5128710189817
--rw-r--r--   0        0        0      370 2023-04-07 17:26:16.156322 np_gui-0.0.2/np_gui/.git/objects/65/8ffd88875bf7232974d3336e0ddcba791258dd
--rw-r--r--   0        0        0       90 2023-04-07 17:26:16.296320 np_gui-0.0.2/np_gui/.git/objects/66/6711ca61d33b2d5580db1eb9c5d67fbc782ff5
--rw-r--r--   0        0        0      266 2023-04-07 17:26:16.100323 np_gui-0.0.2/np_gui/.git/objects/66/a3936df784c7ae9dfb8bf41b1dfad6f3aeeb7e
--rw-r--r--   0        0        0      270 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/66/d0ab5f0bcc68e712e5945e0a2979090bbc9792
--rw-r--r--   0        0        0      417 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/67/97c705dcdd095450864560f88a49aa97c8098b
--rw-r--r--   0        0        0      179 2023-04-07 17:26:16.100323 np_gui-0.0.2/np_gui/.git/objects/68/bcac7d83a1103dbb3d5a5ff66a6c4eac196b1b
--rw-r--r--   0        0        0      226 2023-04-07 17:26:16.152322 np_gui-0.0.2/np_gui/.git/objects/68/d774c9247b07c66a98fb402c29f4b6b15244d8
--rw-r--r--   0        0        0   717791 2023-04-07 17:26:16.260320 np_gui-0.0.2/np_gui/.git/objects/68/de97c3e31d279a8efdf84bd0715f04366bd9d4
--rw-r--r--   0        0        0      350 2023-04-07 17:26:16.228321 np_gui-0.0.2/np_gui/.git/objects/68/ebffa887dfb5a0ee10257bd15e1d73f54ff3c1
--rw-r--r--   0        0        0     1376 2023-04-07 17:26:16.224321 np_gui-0.0.2/np_gui/.git/objects/6d/72961051eba439a573224713613f34beebe7d5
--rw-r--r--   0        0        0      222 2023-04-07 17:26:16.152322 np_gui-0.0.2/np_gui/.git/objects/6d/7abd6a062f89d902baa1b4e62d7eefe3a6127a
--rw-r--r--   0        0        0      374 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/6d/ff6a0d206023dc07131d32ce4dc0d1d2be07e7
--rw-r--r--   0        0        0      426 2023-04-07 17:26:16.216321 np_gui-0.0.2/np_gui/.git/objects/6e/36b195b2d3083c18c06bafa280ce86729aa546
--rw-r--r--   0        0        0      224 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/6e/4c3aacb8629b139e69221206ef6860327a5999
--rw-r--r--   0        0        0      295 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/6e/ed470685fff746365446c654565a51ad5c6078
--rw-r--r--   0        0        0      207 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/6f/07f88ee675592399a091ad7be4b45c38c1092f
--rw-r--r--   0        0        0      241 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/6f/a2dec1eed5f2d20947a509fc32b535442f0501
--rw-r--r--   0        0        0      399 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/6f/ba6fac86107c00da55fad43c980276852c1757
--rw-r--r--   0        0        0      452 2023-04-07 17:26:16.228321 np_gui-0.0.2/np_gui/.git/objects/6f/cf05b4b76f8b9774c317ac8ada402f8a7087de
--rw-r--r--   0        0        0      199 2023-04-07 17:26:16.220321 np_gui-0.0.2/np_gui/.git/objects/70/536a6683577925167e84e0b0f6a06228754d0a
--rw-r--r--   0        0        0      362 2023-04-07 17:26:16.156322 np_gui-0.0.2/np_gui/.git/objects/70/73eb8c8cf7160c7ee9aeed67a20247916e4f8b
--rw-r--r--   0        0        0      293 2023-04-07 17:26:16.152322 np_gui-0.0.2/np_gui/.git/objects/70/ca2c4ff1c8dd07e030046f2374b7c719d717e1
--rw-r--r--   0        0        0       99 2023-04-07 17:26:16.212321 np_gui-0.0.2/np_gui/.git/objects/71/07cec93a979b9a5f64843235a16651d563ce2d
--rw-r--r--   0        0        0       87 2023-04-07 17:26:16.100323 np_gui-0.0.2/np_gui/.git/objects/71/b7dc2f984b6ab15f4d3df2cd212c04144ea4ec
--rw-r--r--   0        0        0      504 2023-04-07 17:26:16.160322 np_gui-0.0.2/np_gui/.git/objects/72/d8580bb77ce2a936b2dc1611f526113777f8e0
--rw-r--r--   0        0        0      268 2023-04-07 17:26:16.160322 np_gui-0.0.2/np_gui/.git/objects/73/a8325d5d447d2e8ec63ad1697a2e90a0917453
--rw-r--r--   0        0        0     5902 2023-04-07 17:26:16.216321 np_gui-0.0.2/np_gui/.git/objects/73/b3f374235d2b9108df69992543b725d281830d
--rw-r--r--   0        0        0      104 2023-04-07 17:26:16.220321 np_gui-0.0.2/np_gui/.git/objects/73/c929623d670f58c11c300a877cb839f5955127
--rw-r--r--   0        0        0      253 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/74/68008313f5be4ba91c30bed9d836f4061aa928
--rw-r--r--   0        0        0      171 2023-04-07 17:26:16.132322 np_gui-0.0.2/np_gui/.git/objects/74/af167ca5f2a8d88745d6797a0f7bc543974500
--rw-r--r--   0        0        0      250 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/77/227a4352ff306e27f56f075723a8311c325232
--rw-r--r--   0        0        0      931 2023-04-07 17:26:16.224321 np_gui-0.0.2/np_gui/.git/objects/79/e30a1f1999c22b29515767c063825cc39c58dd
--rw-r--r--   0        0        0      182 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/7b/5a5e5db74ca159d5543d4ff501e4610e71b007
--rw-r--r--   0        0        0     3289 2023-04-10 21:31:13.504683 np_gui-0.0.2/np_gui/.git/objects/7b/9bb5ff74e21d54bf198702fc5f28b95a970363
--rw-r--r--   0        0        0      362 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/7b/d0a07d11323ff8f875ffa673d00d8d60e240cf
--rw-r--r--   0        0        0      135 2023-04-07 17:26:16.100323 np_gui-0.0.2/np_gui/.git/objects/7c/44c6f019a5c9033813a1bdb635a277e9a007ed
--rw-r--r--   0        0        0      232 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/7c/e662b35418fabf5fc623103c5b9c3ee4502cda
--rw-r--r--   0        0        0     6273 2023-04-07 17:26:16.212321 np_gui-0.0.2/np_gui/.git/objects/7d/bc787d386c6e6de6913a4faa1b648cfe6432cf
--rw-r--r--   0        0        0      428 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/7d/d45f3bc180699ff981b37dfb14688eb78ca675
--rw-r--r--   0        0        0      119 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/7e/1b0385684be0697364205f42de1432b8ac0bdd
--rw-r--r--   0        0        0   169464 2023-04-07 17:26:16.236321 np_gui-0.0.2/np_gui/.git/objects/7f/21122c47c9a5676d4c89f259e97335ae489d57
--rw-r--r--   0        0        0     1214 2023-04-07 17:26:16.216321 np_gui-0.0.2/np_gui/.git/objects/7f/a655b2377cee22ec9fc2f3e4c37346e876811d
--rw-r--r--   0        0        0      239 2023-04-10 21:31:13.524683 np_gui-0.0.2/np_gui/.git/objects/80/416a53f75e5f3db988c00f39c4774ee960b5ca
--rw-r--r--   0        0        0      432 2023-04-07 17:26:16.216321 np_gui-0.0.2/np_gui/.git/objects/80/49bfee8f5d245aa171373c48f3591ef0644878
--rw-r--r--   0        0        0      186 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/81/5ac6f2bdb1ad45d501d3f35c8cd611ae4824c1
--rw-r--r--   0        0        0      121 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/82/61872dbda5acca3f3c1ab956fa8efd745a19a7
--rw-r--r--   0        0        0      263 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/83/a02292b6e06febce7a8544a1c5f823c6deffd3
--rw-r--r--   0        0        0     1226 2023-04-07 17:26:16.224321 np_gui-0.0.2/np_gui/.git/objects/83/b523cba01c5fe06efe78c786c68b99e006a1ef
--rw-r--r--   0        0        0      225 2023-04-07 17:26:16.100323 np_gui-0.0.2/np_gui/.git/objects/83/cb24902e8481440cfdd96bcfa08e484007fea6
--rw-r--r--   0        0        0      185 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/84/406c70d49b8b20fa384439f1ae59e7b362f385
--rw-r--r--   0        0        0      500 2023-04-07 17:26:16.296320 np_gui-0.0.2/np_gui/.git/objects/84/4ed73248be6b9bba23a42c9eca4f1f1b8bbaba
--rw-r--r--   0        0        0      276 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/84/fc6011b4c773e73bffce7f7ea7e23dd56e3186
--rw-r--r--   0        0        0      388 2023-04-07 17:26:16.160322 np_gui-0.0.2/np_gui/.git/objects/85/3d99ded57aee5e2420efc8fe40581970bb9a4b
--rw-r--r--   0        0        0     4227 2023-04-07 17:26:16.212321 np_gui-0.0.2/np_gui/.git/objects/86/3704b310d1539241ef20e26ccce6af27f0ffce
--rw-r--r--   0        0        0      326 2023-04-07 17:26:16.300320 np_gui-0.0.2/np_gui/.git/objects/86/7c400721db0c0512ecf56db608e9a41cae1321
--rw-r--r--   0        0        0      289 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/86/a52c628f6d333cf3e6c8d5db9eff8a05ed8dd8
--rw-r--r--   0        0        0     1226 2023-04-07 17:26:16.212321 np_gui-0.0.2/np_gui/.git/objects/87/f8bd121b2352751b730a3d04fff0e1ecd946b2
--rw-r--r--   0        0        0      105 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/89/06bc6ad32b3d5962c61be8613870a0e6f2a722
--rw-r--r--   0        0        0      147 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/89/41f71921a07eccb037f684bbb084ed7c103f9d
--rw-r--r--   0        0        0      390 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/89/6caa304279b47572781df2ee6275c0af8008f3
--rw-r--r--   0        0        0      365 2023-04-07 17:26:16.152322 np_gui-0.0.2/np_gui/.git/objects/89/fe7144bf7d84edc1fb689c6bb539bf94804491
--rw-r--r--   0        0        0       95 2023-04-07 17:26:16.100323 np_gui-0.0.2/np_gui/.git/objects/8b/933036464e9b843a6ba38a9bd37af8db758662
--rw-r--r--   0        0        0      162 2023-04-07 17:26:16.300320 np_gui-0.0.2/np_gui/.git/objects/8c/0b152262f2aa15461387f07c0402c673b1851a
--rw-r--r--   0        0        0      365 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/8c/b0b5d5d7532de13f3f06d7883d7c7eb6e717aa
--rw-r--r--   0        0        0     3792 2023-04-07 17:26:16.208321 np_gui-0.0.2/np_gui/.git/objects/8c/bf1b161a6527c8c6ad1c4f1fdc156e065ab262
--rw-r--r--   0        0        0      318 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/8d/5ad0d96dd099b60a21227dd7a618bb17225bc1
--rw-r--r--   0        0        0     1726 2023-04-07 17:26:16.224321 np_gui-0.0.2/np_gui/.git/objects/8d/6c78666cf9fb53cb7cbda107057f7e1f74ecfe
--rw-r--r--   0        0        0      347 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/8e/37ad553c96d5471de9a7dce25950808b42647c
--rw-r--r--   0        0        0     4765 2023-04-07 17:26:16.208321 np_gui-0.0.2/np_gui/.git/objects/91/c7bd8edfa0720adbefd523d9273d945d88e140
--rw-r--r--   0        0        0      241 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/91/ecc9f95678e124db03c9530352f9a398122577
--rw-r--r--   0        0        0      179 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/93/2bf90187f3db9459826604132a0b6d81316e10
--rw-r--r--   0        0        0      236 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/93/4d3546cfa6be67abb176e988292c7bf505f557
--rw-r--r--   0        0        0      447 2023-04-07 17:26:16.224321 np_gui-0.0.2/np_gui/.git/objects/93/b2c8c086a53e63f7e906241a07198b2ff073bb
--rw-r--r--   0        0        0      758 2023-04-10 21:31:13.504683 np_gui-0.0.2/np_gui/.git/objects/94/b2fe90389ca2a9b49f0f8e10fd59daa55ccfa1
--rw-r--r--   0        0        0      298 2023-04-07 17:26:16.216321 np_gui-0.0.2/np_gui/.git/objects/94/bda2139156340fc42bb1cb678e49ac9ac8d3c6
--rw-r--r--   0        0        0     1324 2023-04-07 17:26:16.204321 np_gui-0.0.2/np_gui/.git/objects/94/fa42f6a19f759b9f917de9ace864594eb4504c
--rw-r--r--   0        0        0     1517 2023-04-07 17:26:16.224321 np_gui-0.0.2/np_gui/.git/objects/95/1cf810df0ce59ad5e170048bcf5ae334a21903
--rw-r--r--   0        0        0      367 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/96/61af2897d03b8bee195e6a6efd35b954434c51
--rw-r--r--   0        0        0     3250 2023-04-07 17:26:16.216321 np_gui-0.0.2/np_gui/.git/objects/96/9d3ce8e5fed0dbc813992555812aa644fd6704
--rw-r--r--   0        0        0      288 2023-04-07 17:26:16.152322 np_gui-0.0.2/np_gui/.git/objects/98/b321936c584909e69ebfd55d42475e5f251575
--rw-r--r--   0        0        0      335 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/98/b7a14f653299b4afe59a5fe6264e02775cf95b
--rw-r--r--   0        0        0     2874 2023-04-07 17:26:16.216321 np_gui-0.0.2/np_gui/.git/objects/99/f14a2ee856d0ec3078dd78700f43524f4a702c
--rw-r--r--   0        0        0      240 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/9a/54f7e1fa2a17ed615c2e2e52e17df8713102e5
--rw-r--r--   0        0        0     1388 2023-04-07 17:26:16.228321 np_gui-0.0.2/np_gui/.git/objects/9a/a62fc22baa68906867164da4d6819dfaf72907
--rw-r--r--   0        0        0     9760 2023-04-07 17:26:16.100323 np_gui-0.0.2/np_gui/.git/objects/9b/0c5d24797113260de88fecbf34e34eac684419
--rw-r--r--   0        0        0      278 2023-04-07 17:26:16.152322 np_gui-0.0.2/np_gui/.git/objects/9b/f1fa830c6709e657d681546d26c37b1b049c13
--rw-r--r--   0        0        0      123 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/9c/06d9cf6f4651649a2e2b64b87bd205e7c069f1
--rw-r--r--   0        0        0      313 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/9c/658561b058c4018093d97cb5251882118c817a
--rw-r--r--   0        0        0      140 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/9c/84890262bb671fed3f026f0b89880b45522c2c
--rw-r--r--   0        0        0      356 2023-04-07 17:26:16.152322 np_gui-0.0.2/np_gui/.git/objects/9d/0fb399e061416b897ad48d3e3c379ee84edbc7
--rw-r--r--   0        0        0      287 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/9d/893277c7535ff29a3d31a25db1969adc8b4e6e
--rw-r--r--   0        0        0      895 2023-04-07 17:26:16.176321 np_gui-0.0.2/np_gui/.git/objects/9d/ee52bf5c9334619fddf41655c5b4d9f36d23ba
--rw-r--r--   0        0        0      312 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/9f/882099f08b8e6dc79d8c0591e300362841212d
--rw-r--r--   0        0        0      290 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/9f/c340849088b562ae530cb53ec3248992bd591a
--rw-r--r--   0        0        0      219 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/a0/043769531ae36e82087b3d906351fdd6438cee
--rw-r--r--   0        0        0      191 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/a0/5eb844817026e52126743c604abd33e2826805
--rw-r--r--   0        0        0      390 2023-04-07 17:26:16.156322 np_gui-0.0.2/np_gui/.git/objects/a0/9291bb66aa7389f46e6731d2d30bdcedf1a373
--rw-r--r--   0        0        0      135 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/a0/94df282308cefbe2acdabf231d67891b899ecc
--rw-r--r--   0        0        0      388 2023-04-07 17:26:16.152322 np_gui-0.0.2/np_gui/.git/objects/a0/d8f5cb0274d415eff4776e5c0a07139dc31f65
--rw-r--r--   0        0        0      206 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/a1/aba4771189ad91fb9c8c3e38f8e297e3533899
--rw-r--r--   0        0        0      157 2023-04-07 17:26:16.152322 np_gui-0.0.2/np_gui/.git/objects/a3/f80474b3a2141e0cb86e2beeab654e5a86b059
--rw-r--r--   0        0        0      373 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/a4/85d703f6fee063c94c7449e59427eb65d3d42b
--rw-r--r--   0        0        0      162 2023-04-07 17:26:16.156322 np_gui-0.0.2/np_gui/.git/objects/a5/af665a945fe2fe90ba3cb4ab309770cb8b8a1b
--rw-r--r--   0        0        0     4416 2023-04-07 17:26:16.228321 np_gui-0.0.2/np_gui/.git/objects/a6/071cf103f9f5579b5380f432d7a71547fe430d
--rw-r--r--   0        0        0      331 2023-04-07 17:26:16.156322 np_gui-0.0.2/np_gui/.git/objects/a6/5032d2eac28d7eb06e72f63f1ad77049131d8a
--rw-r--r--   0        0        0      279 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/a6/89c589f46b71a7371355158162314d28beaff1
--rw-r--r--   0        0        0      146 2023-04-07 17:26:16.300320 np_gui-0.0.2/np_gui/.git/objects/a6/8ff3364a04bc97e5366a2e683af66ee3757836
--rw-r--r--   0        0        0      209 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/a7/26572bc5c612020e8ccb8262bec7bb38815d92
--rw-r--r--   0        0        0      262 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/a7/2a08a187a66b3f6b30b5232c6a6455817e712a
--rw-r--r--   0        0        0      196 2023-04-07 17:26:16.152322 np_gui-0.0.2/np_gui/.git/objects/a7/b30f721238dc5272764837ae9f5c79671a05e0
--rw-r--r--   0        0        0      269 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/a8/024d9e1ced5f8bc62669441301936a5ba43a9f
--rw-r--r--   0        0        0      118 2023-04-07 17:26:16.100323 np_gui-0.0.2/np_gui/.git/objects/a8/14b5b1393cabfc00da432d953226c89a33b5f3
--rw-r--r--   0        0        0      412 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/a8/21265a679d77c1bb68ac6ca3b6a64d33e383d8
--rw-r--r--   0        0        0      306 2023-04-07 17:26:16.208321 np_gui-0.0.2/np_gui/.git/objects/a8/58a410e4faa62ce324d814e4b816fff83a6fb3
--rw-r--r--   0        0        0      204 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/a9/16710595330e51c0c2129e2af52c39c085c102
--rw-r--r--   0        0        0      251 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/a9/92e14fe59e712d4729dd219c4a54e8dc6bbbba
--rw-r--r--   0        0        0      882 2023-04-07 17:26:16.216321 np_gui-0.0.2/np_gui/.git/objects/a9/ca1c82cd661cfa1583e86fa881644d029d061f
--rw-r--r--   0        0        0      248 2023-04-07 17:26:16.100323 np_gui-0.0.2/np_gui/.git/objects/a9/e343dbf6b5afe45038c6224d9b74b81a27b1a0
--rw-r--r--   0        0        0      474 2023-04-07 17:26:16.216321 np_gui-0.0.2/np_gui/.git/objects/a9/ef0793b06408e258f02b20779ad4b71677996d
--rw-r--r--   0        0        0      364 2023-04-07 17:26:16.160322 np_gui-0.0.2/np_gui/.git/objects/a9/f249f378ce6359727a5f22db618d9d667c1c9e
--rw-r--r--   0        0        0      236 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/aa/84a5ed4d84b01dd1b65ad604d87913210d8eb0
--rw-r--r--   0        0        0      245 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/aa/f7a98614d3f88dbe31c80bcc64df7127a7eb4e
--rw-r--r--   0        0        0      318 2023-04-07 17:26:16.100323 np_gui-0.0.2/np_gui/.git/objects/ab/443202cd292c0c9a37d9681b7fd4aace17dcaf
--rw-r--r--   0        0        0     2064 2023-04-07 17:26:16.224321 np_gui-0.0.2/np_gui/.git/objects/ab/50aed569b864b6accf34abc48e3f0119072ec1
--rw-r--r--   0        0        0      296 2023-04-07 17:26:16.228321 np_gui-0.0.2/np_gui/.git/objects/ac/8f1f2e7b6507a33ea9074f8a91d4f06d640451
--rw-r--r--   0        0        0      215 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/ac/f7888226025c57194bc9bb4d9ec088e460688c
--rw-r--r--   0        0        0      374 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/ad/1add4accbedff114849e3d6e412c532745ad22
--rw-r--r--   0        0        0      372 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/ad/768d39a2ec6868b3a77a0ddf3cc44ca3316a2b
--rw-r--r--   0        0        0      214 2023-04-07 17:26:16.156322 np_gui-0.0.2/np_gui/.git/objects/ad/9a6a0ab97b0ccfc061bee86b2e1a14591d4c80
--rw-r--r--   0        0        0      260 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/ad/b481b284bd912e114ad03b77ddc1b545450cf7
--rw-r--r--   0        0        0      246 2023-04-07 17:26:16.156322 np_gui-0.0.2/np_gui/.git/objects/ad/da9b71336f7e914a400858c148fb249c15a7c3
--rw-r--r--   0        0        0      356 2023-04-07 17:26:16.152322 np_gui-0.0.2/np_gui/.git/objects/ad/f2b83014d70a80a4f4be9945bf4b83da40e188
--rw-r--r--   0        0        0      236 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/ae/e2b7fa0dbf74d7fbbf085750fc0fd31290a83b
--rw-r--r--   0        0        0      912 2023-04-07 17:26:16.228321 np_gui-0.0.2/np_gui/.git/objects/af/5a804d593607e51ca637bebcbc9633f261691d
--rw-r--r--   0        0        0      188 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/b1/accde437c3ca493369ba921e44d99c1df7d4fe
--rw-r--r--   0        0        0       55 2023-04-07 17:26:16.300320 np_gui-0.0.2/np_gui/.git/objects/b2/4e45a64e3c9e5e68d2b1c9a15764b990def7a2
--rw-r--r--   0        0        0      408 2023-04-07 17:26:16.152322 np_gui-0.0.2/np_gui/.git/objects/b2/dc9c54f31a67255b5149873327cbe7cb2e8df2
--rw-r--r--   0        0        0      246 2023-04-07 17:26:16.156322 np_gui-0.0.2/np_gui/.git/objects/b2/f98087ce8639cda58fa6de59112a60226351ca
--rw-r--r--   0        0        0      386 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/b4/939d2d1f5683c275393330b925106e073703d1
--rw-r--r--   0        0        0       99 2023-04-07 17:26:16.296320 np_gui-0.0.2/np_gui/.git/objects/b4/e656a7444748b374dd8d35f597ac295e007473
--rw-r--r--   0        0        0      262 2023-04-07 17:26:16.100323 np_gui-0.0.2/np_gui/.git/objects/b5/0abcd237a44dcd6a77498cff02386ca2e60c0c
--rw-r--r--   0        0        0      291 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/b5/4e23a265fca65d7e396f6017e0c785f084d0c5
--rw-r--r--   0        0        0      288 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/b6/0efa5367707f19ee227b1775269ed1b354263c
--rw-r--r--   0        0        0      282 2023-04-07 17:26:16.156322 np_gui-0.0.2/np_gui/.git/objects/b6/6a729aef825db25c1991f1b7c27d0075469e7a
--rw-r--r--   0        0        0      357 2023-04-07 17:26:16.156322 np_gui-0.0.2/np_gui/.git/objects/b7/6565c3229e31ba183a6b4223e71b392b1a8ead
--rw-r--r--   0        0        0    23529 2023-04-07 17:26:16.216321 np_gui-0.0.2/np_gui/.git/objects/b8/12b350783f1787c3a3760f45226875526131ed
--rw-r--r--   0        0        0      570 2023-04-07 17:26:16.228321 np_gui-0.0.2/np_gui/.git/objects/b8/8f108df9a4d81e94bb8d0a3ecded420c9999f7
--rw-r--r--   0        0        0      300 2023-04-07 17:26:16.156322 np_gui-0.0.2/np_gui/.git/objects/b8/ceaac683ce553da24d63ee5352583079123b2e
--rw-r--r--   0        0        0      152 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/b9/75f69d842274cdb717980c47190f1bfc1aa465
--rw-r--r--   0        0        0     9804 2023-04-10 21:31:13.504683 np_gui-0.0.2/np_gui/.git/objects/b9/e8dcf0bbc28cc9b716c64d372f02da5fbf4d8a
--rw-r--r--   0        0        0      242 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/ba/067f1ad3242573d257077ecf3664b61a3fedc0
--rw-r--r--   0        0        0      392 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/ba/40f5dd6d6a0b44424b4cd2f52aae2dc16cfe91
--rw-r--r--   0        0        0      268 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/ba/d24ba4bf841acc23f1e3d3b53e788a4d238252
--rw-r--r--   0        0        0      210 2023-04-07 17:26:16.216321 np_gui-0.0.2/np_gui/.git/objects/bb/a17fa6bc6aa2e1a0f08088b7bd685077463e8e
--rw-r--r--   0        0        0      300 2023-04-07 17:26:16.156322 np_gui-0.0.2/np_gui/.git/objects/bc/a49aeb86bf0e009f544bfb52e548359bc73deb
--rw-r--r--   0        0        0      307 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/bc/d1c67d67b763dbe877cd11be6b54b157d8e265
--rw-r--r--   0        0        0    89674 2023-04-07 17:26:16.220321 np_gui-0.0.2/np_gui/.git/objects/be/22be0309951eac928d0c9464b69419c4130397
--rw-r--r--   0        0        0      225 2023-04-07 17:26:16.152322 np_gui-0.0.2/np_gui/.git/objects/be/41ba5ffab64161d9b5c6daf3c4feec8805f35c
--rw-r--r--   0        0        0      258 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/c0/3fffaf8d503fdd080f75e35e579b7dee939043
--rw-r--r--   0        0        0      121 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/c1/6f0a2abe37e26f8bc3fb066fcb948250de2f7e
--rw-r--r--   0        0        0      248 2023-04-07 17:26:16.156322 np_gui-0.0.2/np_gui/.git/objects/c2/023e3518d26fbb7fd43caf2f89b9b0ea4a6004
--rw-r--r--   0        0        0      171 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/c3/28bab809df9d1fa7e31cfc9f834f0286f7e557
--rw-r--r--   0        0        0     1588 2023-04-07 17:26:16.096323 np_gui-0.0.2/np_gui/.git/objects/c3/2c1344d92909ded9583ba6345784effe44b53a
--rw-r--r--   0        0        0     8672 2023-04-07 17:26:16.228321 np_gui-0.0.2/np_gui/.git/objects/c3/c1d6ad1ff6773f3af11f82b00d3aa80f3c2c74
--rw-r--r--   0        0        0      135 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/c3/e7b6ebc89e651bd1a729ae15453a098c76c390
--rw-r--r--   0        0        0      261 2023-04-07 17:26:16.296320 np_gui-0.0.2/np_gui/.git/objects/c5/fcdf0fa94c289ac7c27ec7ef92f4a30e184ce6
--rw-r--r--   0        0        0      207 2023-04-07 17:26:16.152322 np_gui-0.0.2/np_gui/.git/objects/c6/8f266787cac7c492d925970752e1b35a496382
--rw-r--r--   0        0        0      312 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/c6/a482857c990fa45d5733163a5fb9a42e432b41
--rw-r--r--   0        0        0       58 2023-04-07 17:26:16.296320 np_gui-0.0.2/np_gui/.git/objects/c6/e32ced40c40b4cdc4e8c691862fe853ce00c70
--rw-r--r--   0        0        0      267 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/c6/fa0577d96165a7b3cde82351e9b65fdd460f6a
--rw-r--r--   0        0        0      195 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/c7/73284111041288138572ae40e2274a63ece623
--rw-r--r--   0        0        0      299 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/c7/d9129abc643d86e3e63d1547dd301452c15f44
--rw-r--r--   0        0        0      216 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/c8/63ddc1dc247a8e9549be8686b7d793d4e2645b
--rw-r--r--   0        0        0     1140 2023-04-07 17:26:16.228321 np_gui-0.0.2/np_gui/.git/objects/c9/524a39a654e5682491ec28f3b74691d367c631
--rw-r--r--   0        0        0      249 2023-04-07 17:26:16.100323 np_gui-0.0.2/np_gui/.git/objects/cb/951fab21992a389c556e66fde1caf42d84bebf
--rw-r--r--   0        0        0      297 2023-04-07 17:26:16.152322 np_gui-0.0.2/np_gui/.git/objects/cb/e916e924c656cfe505628d642a07a9c0b7192c
--rw-r--r--   0        0        0     7493 2023-04-07 17:26:16.296320 np_gui-0.0.2/np_gui/.git/objects/cd/144dacd2cea10437ca2f4f81e6bcb818f8fce8
--rw-r--r--   0        0        0      379 2023-04-07 17:26:16.160322 np_gui-0.0.2/np_gui/.git/objects/cd/2af817276ff4d56b247e8dfc103df840ed33f1
--rw-r--r--   0        0        0      132 2023-04-07 17:26:16.172321 np_gui-0.0.2/np_gui/.git/objects/cd/2f08be4a16d2f1d1974301ae0a9fa21fe0b381
--rw-r--r--   0        0        0      195 2023-04-07 17:26:16.132322 np_gui-0.0.2/np_gui/.git/objects/cd/6c58bf1544c7650e4cfe7ec997beb88bd58976
--rw-r--r--   0        0        0     7031 2023-04-10 21:31:13.508683 np_gui-0.0.2/np_gui/.git/objects/cd/cc60c9492124b2997eb3f9bf80ee269c17497f
--rw-r--r--   0        0        0       87 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/ce/7c8452c2e56a7bc1f6bca043016d204da0ca54
--rw-r--r--   0        0        0      336 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/ce/f521d3c412bd7fac110d444b903247f5d780d5
--rw-r--r--   0        0        0      185 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/cf/efd8fb9c8c0e5d4e1bab5857224ff80f501f87
--rw-r--r--   0        0        0      289 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/d1/20a714fad348a8d26b9a362803b3def686a3ea
--rw-r--r--   0        0        0      298 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/d2/99d11ef2f246a1f1dc68f4806b9506f4f83ee0
--rw-r--r--   0        0        0      232 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/d2/a2425dc08f7ea6e2eee76bcfcd427864ce1436
--rw-r--r--   0        0        0    12583 2023-04-07 17:26:16.224321 np_gui-0.0.2/np_gui/.git/objects/d2/ba89ea73f92343e7939d2edf87f63272567146
--rw-r--r--   0        0        0      120 2023-04-07 17:26:16.300320 np_gui-0.0.2/np_gui/.git/objects/d3/10a91072e0d346eb5d26cc2528385b0e262866
--rw-r--r--   0        0        0      252 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/d4/c7de9b2bf50ed3cd2af0f8ef20237115c433f0
--rw-r--r--   0        0        0      258 2023-04-07 17:26:16.152322 np_gui-0.0.2/np_gui/.git/objects/d4/ec58e61e2f66c9352560d01f02da8cc54ff62f
--rw-r--r--   0        0        0      162 2023-04-07 17:26:16.300320 np_gui-0.0.2/np_gui/.git/objects/d7/7051c914c7f3eb04325a4f2af497f66dd08c52
--rw-r--r--   0        0        0       66 2023-04-07 17:26:16.228321 np_gui-0.0.2/np_gui/.git/objects/d9/176a9b93c98987bd2dfd3dc98a27da0d14e82a
--rw-r--r--   0        0        0       97 2023-04-07 17:26:16.212321 np_gui-0.0.2/np_gui/.git/objects/d9/6755fdaf8bb2214971e0db9c1fd3077d7c419d
--rw-r--r--   0        0        0      410 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/da/9f957a222fd5a0c817730b777b4685745719de
--rw-r--r--   0        0        0      284 2023-04-07 17:26:16.100323 np_gui-0.0.2/np_gui/.git/objects/da/a6aa486eac8d35b01eff601982cbb9b5f977d4
--rw-r--r--   0        0        0      303 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/dc/74d8fe668cbaef0dfb4614e64ec46a27ec2559
--rw-r--r--   0        0        0      368 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/dc/d7ffc55358447926c2a7b66365e8e63bdf34af
--rw-r--r--   0        0        0      287 2023-04-07 17:26:16.156322 np_gui-0.0.2/np_gui/.git/objects/dc/f4a5a7e555d1d940b7fd10a514bcda02cb6224
--rw-r--r--   0        0        0      326 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/dd/30469ede79144bcf634dec2d72f59ea5d7e6aa
--rw-r--r--   0        0        0      295 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/dd/57ceb05dccfd9c35dc73034ea5da576342815a
--rw-r--r--   0        0        0     2795 2023-04-10 21:31:13.508683 np_gui-0.0.2/np_gui/.git/objects/dd/5e3265458dfc3b5b8292c010f8096279aa04d2
--rw-r--r--   0        0        0      307 2023-04-07 17:26:16.160322 np_gui-0.0.2/np_gui/.git/objects/de/4c51e743b0288b1bb9c1018ad407f7b606888e
--rw-r--r--   0        0        0     3007 2023-04-07 17:26:16.224321 np_gui-0.0.2/np_gui/.git/objects/e0/0881e53af3f94a333c22a09828a27668e12380
--rw-r--r--   0        0        0      306 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/e0/fa1cce4d58a69389e0653d8053f82966bdbbfa
--rw-r--r--   0        0        0      230 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/e1/4b45b75cdab6fb961aae2ce52503be6328cc4e
--rw-r--r--   0        0        0      817 2023-04-07 17:26:16.288320 np_gui-0.0.2/np_gui/.git/objects/e3/23b245ccb6c1923f7ea87838cbad6430037588
--rw-r--r--   0        0        0      633 2023-04-07 17:26:16.216321 np_gui-0.0.2/np_gui/.git/objects/e4/653f2364523e4195f75c9728ea0cc90bef3144
--rw-r--r--   0        0        0      172 2023-04-07 17:26:16.100323 np_gui-0.0.2/np_gui/.git/objects/e4/b0abe3fb03afa683278463e32bff5809abdc1a
--rw-r--r--   0        0        0      311 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/e4/d6960d6a4241020f1266523f9520d642bf9155
--rw-r--r--   0        0        0      125 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/e5/684297395be21d21f5e73d328e0b1527f56914
--rw-r--r--   0        0        0     1379 2023-04-07 17:26:16.160322 np_gui-0.0.2/np_gui/.git/objects/e5/8c1074764f4809a09dcba175d231b5005517fe
--rw-r--r--   0        0        0       15 2023-04-07 17:26:16.216321 np_gui-0.0.2/np_gui/.git/objects/e6/9de29bb2d1d6434b8b29ae775ad8c2e48c5391
--rw-r--r--   0        0        0      101 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/e6/b9e803f11b9a2c9c6404b7fff8aa2e4bd74a9b
--rw-r--r--   0        0        0    46491 2023-04-07 17:26:16.204321 np_gui-0.0.2/np_gui/.git/objects/e6/d4de2b0f07905e0c80035ac9f57383449d0e5e
--rw-r--r--   0        0        0      148 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/e7/44ae488cfc42eeb38dff2a3d6c9d9557291346
--rw-r--r--   0        0        0   409349 2023-04-07 17:26:16.176321 np_gui-0.0.2/np_gui/.git/objects/e8/580861a89ac9730eb1db2a47ad25771e8d1188
--rw-r--r--   0        0        0      170 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/e8/6584a2797dfa4f7daf78cf643a4063a6fc2129
--rw-r--r--   0        0        0      211 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/e9/52bb769c64d5fe616a398de9e0d811f207c5b1
--rw-r--r--   0        0        0      403 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/eb/4becfe11711e4f25b814ecc88aa57c52c71e70
--rw-r--r--   0        0        0      317 2023-04-07 17:26:16.160322 np_gui-0.0.2/np_gui/.git/objects/eb/bffc23c524d0f544eddcd84b9d347b56d930f2
--rw-r--r--   0        0        0      121 2023-04-07 17:26:16.100323 np_gui-0.0.2/np_gui/.git/objects/eb/e3698e0b5b2e06e1619288c3c71b4bbe6f41bb
--rw-r--r--   0        0        0      245 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/ec/a5a38d564ec28a0000b29515f727832e753356
--rw-r--r--   0        0        0      166 2023-04-07 17:26:16.156322 np_gui-0.0.2/np_gui/.git/objects/ec/b0af680ed6133aed8a57c2319fd67b3235e6f9
--rw-r--r--   0        0        0     1255 2023-04-07 17:26:16.224321 np_gui-0.0.2/np_gui/.git/objects/ed/7521cf8f376aedf8deff2e6077acd5b3636f1a
--rw-r--r--   0        0        0      235 2023-04-07 17:26:16.156322 np_gui-0.0.2/np_gui/.git/objects/ee/13c24991e3ba79e4e660dc5a0420a7e2dbbae9
--rw-r--r--   0        0        0      285 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/ee/dae3e9a5eb7fa28d2282aa04336ad542424724
--rw-r--r--   0        0        0      235 2023-04-07 17:26:16.100323 np_gui-0.0.2/np_gui/.git/objects/ef/f48cdc6867c8ba7f6261565b527a7c67d72d42
--rw-r--r--   0        0        0      282 2023-04-07 17:26:16.152322 np_gui-0.0.2/np_gui/.git/objects/f0/89cb3add649f6b73676e14d77dbe2a913c6845
--rw-r--r--   0        0        0      245 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/f1/3f937e42fff5246959459e7ffb28173c7344ca
--rw-r--r--   0        0        0      228 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/f1/99ac0bf3ac83a85f8432ac2d4508919862a9d6
--rw-r--r--   0        0        0      385 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/f1/ae17657eb0aa6dd469ffe4a0094bf0e1536da9
--rw-r--r--   0        0        0      302 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/f2/3c031dc2337d4728b2c850a511a164bbd10269
--rw-r--r--   0        0        0      243 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/f3/4aef6860b23535c9c6ed92868f6e5a4de27ee7
--rw-r--r--   0        0        0      283 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/f3/65ae4d5589056b626c07f7ea0297c9f2c80c26
--rw-r--r--   0        0        0      228 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/f3/b51763747d51b104ffa105407f4a63303e092e
--rw-r--r--   0        0        0      360 2023-04-07 17:26:16.152322 np_gui-0.0.2/np_gui/.git/objects/f3/c39a5c2b02a2e5f525e43aba2baa86e1534245
--rw-r--r--   0        0        0     1247 2023-04-07 17:26:16.216321 np_gui-0.0.2/np_gui/.git/objects/f5/25a19c806874b9d35e2f3c0a3f1df0274e6252
--rw-r--r--   0        0        0      228 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/f5/6ef098af5f5c2a18a96ea7017a3f522139b52b
--rw-r--r--   0        0        0      255 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/f5/8b1ef6a22d8476b338cc2f14c01dd88b338ace
--rw-r--r--   0        0        0     5599 2023-04-07 17:26:16.204321 np_gui-0.0.2/np_gui/.git/objects/f5/8bc582ed47d97f785314420ca5be8e5f79771c
--rw-r--r--   0        0        0      196 2023-04-07 17:26:16.140322 np_gui-0.0.2/np_gui/.git/objects/f6/11b569343fa3d84f0b9ae079196f162d021ce3
--rw-r--r--   0        0        0      357 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/f6/d64a57676f8c36472687b8876b4358fa5fcbe2
--rw-r--r--   0        0        0      123 2023-04-07 17:26:16.296320 np_gui-0.0.2/np_gui/.git/objects/f7/a2b64cf354a862153179a35b68373e30380ace
--rw-r--r--   0        0        0      169 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/f8/35cc20d598a9ec8b6fddbe4c846f8b6fd4b42a
--rw-r--r--   0        0        0      293 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/f8/7820be957dd8135c359e9ed8a175c51ff4b8e1
--rw-r--r--   0        0        0     1577 2023-04-07 17:26:16.216321 np_gui-0.0.2/np_gui/.git/objects/f9/749ff7a391bc6b85fd0fe719e9c4f881058c1f
--rw-r--r--   0        0        0      188 2023-04-07 17:26:16.156322 np_gui-0.0.2/np_gui/.git/objects/f9/e48ce06c4baaec8bd10a7de447c7560a9d5092
--rw-r--r--   0        0        0      265 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/fa/8628f9e42c65276466ffd37cf442186a015036
--rw-r--r--   0        0        0     1388 2023-04-07 17:26:16.224321 np_gui-0.0.2/np_gui/.git/objects/fa/9be82b44d16a0cdf1d7fe7931ee91071ea9640
--rw-r--r--   0        0        0     4353 2023-04-07 17:26:16.216321 np_gui-0.0.2/np_gui/.git/objects/fa/df4f6655e9c534176fc6f71dd797f45dccb2be
--rw-r--r--   0        0        0      194 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/fc/be1334d23d9fac76ba5678564e3472569ca29a
--rw-r--r--   0        0        0      200 2023-04-10 21:31:13.544683 np_gui-0.0.2/np_gui/.git/objects/fd/0052ba8805ee5a573134b3d0be8bb9f5010dfc
--rw-r--r--   0        0        0     1944 2023-04-07 17:26:16.224321 np_gui-0.0.2/np_gui/.git/objects/fd/0aae6386addf84721ec0d5fec2e997013ec6bf
--rw-r--r--   0        0        0      179 2023-04-07 17:26:16.148322 np_gui-0.0.2/np_gui/.git/objects/fd/e599de0715a33ef1021a5f71db315404476cb8
--rw-r--r--   0        0        0      332 2023-04-07 17:26:16.144322 np_gui-0.0.2/np_gui/.git/objects/ff/662ee0b29398fb8ee59ef994de785b162694dc
--rw-r--r--   0        0        0      343 2023-04-07 17:26:16.136322 np_gui-0.0.2/np_gui/.git/objects/ff/a227be54599d4436e13f4fc4d6d984d87eb1ad
--rw-r--r--   0        0        0      103 2023-04-07 17:26:16.208321 np_gui-0.0.2/np_gui/.git/objects/ff/ca608bd9656ffc33102fbdc85d45b345880354
--rw-r--r--   0        0        0       41 2023-04-10 21:31:13.544683 np_gui-0.0.2/np_gui/.git/refs/heads/master
--rw-r--r--   0        0        0     1454 2023-04-10 21:22:19.221466 np_gui-0.0.2/np_gui/__init__.py
--rw-r--r--   0        0        0      120 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char0.png
--rw-r--r--   0        0        0      123 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char1.png
--rw-r--r--   0        0        0      106 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char10.png
--rw-r--r--   0        0        0      136 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char11.png
--rw-r--r--   0        0        0       79 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char12.png
--rw-r--r--   0        0        0       97 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char13.png
--rw-r--r--   0        0        0      164 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char14.png
--rw-r--r--   0        0        0      244 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char15.png
--rw-r--r--   0        0        0      152 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char16.png
--rw-r--r--   0        0        0      242 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char17.png
--rw-r--r--   0        0        0      258 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char18.png
--rw-r--r--   0        0        0      221 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char19.png
--rw-r--r--   0        0        0      229 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char2.png
--rw-r--r--   0        0        0      205 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char20.png
--rw-r--r--   0        0        0      276 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char21.png
--rw-r--r--   0        0        0      214 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char22.png
--rw-r--r--   0        0        0      264 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char23.png
--rw-r--r--   0        0        0      273 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char24.png
--rw-r--r--   0        0        0      110 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char25.png
--rw-r--r--   0        0        0      157 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char26.png
--rw-r--r--   0        0        0      217 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char27.png
--rw-r--r--   0        0        0       88 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char28.png
--rw-r--r--   0        0        0      228 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char29.png
--rw-r--r--   0        0        0      297 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char3.png
--rw-r--r--   0        0        0      218 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char30.png
--rw-r--r--   0        0        0      496 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char31.png
--rw-r--r--   0        0        0      298 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char32.png
--rw-r--r--   0        0        0      247 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char33.png
--rw-r--r--   0        0        0      252 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char34.png
--rw-r--r--   0        0        0      246 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char35.png
--rw-r--r--   0        0        0      178 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char36.png
--rw-r--r--   0        0        0      156 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char37.png
--rw-r--r--   0        0        0      269 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char38.png
--rw-r--r--   0        0        0      158 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char39.png
--rw-r--r--   0        0        0      408 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char4.png
--rw-r--r--   0        0        0      114 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char40.png
--rw-r--r--   0        0        0      161 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char41.png
--rw-r--r--   0        0        0      330 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char42.png
--rw-r--r--   0        0        0      141 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char43.png
--rw-r--r--   0        0        0      323 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char44.png
--rw-r--r--   0        0        0      392 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char5.png
--rw-r--r--   0        0        0       93 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char6.png
--rw-r--r--   0        0        0      228 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char7.png
--rw-r--r--   0        0        0      221 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char8.png
--rw-r--r--   0        0        0      216 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_0_char9.png
--rw-r--r--   0        0        0      285 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char0.png
--rw-r--r--   0        0        0      290 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char1.png
--rw-r--r--   0        0        0      367 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char10.png
--rw-r--r--   0        0        0      279 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char11.png
--rw-r--r--   0        0        0      270 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char12.png
--rw-r--r--   0        0        0      112 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char13.png
--rw-r--r--   0        0        0      172 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char14.png
--rw-r--r--   0        0        0      111 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char15.png
--rw-r--r--   0        0        0      225 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char16.png
--rw-r--r--   0        0        0       94 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char17.png
--rw-r--r--   0        0        0      134 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char18.png
--rw-r--r--   0        0        0      198 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char19.png
--rw-r--r--   0        0        0      204 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char2.png
--rw-r--r--   0        0        0      218 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char20.png
--rw-r--r--   0        0        0      192 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char21.png
--rw-r--r--   0        0        0      216 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char22.png
--rw-r--r--   0        0        0      202 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char23.png
--rw-r--r--   0        0        0      167 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char24.png
--rw-r--r--   0        0        0      318 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char25.png
--rw-r--r--   0        0        0      173 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char26.png
--rw-r--r--   0        0        0      137 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char27.png
--rw-r--r--   0        0        0      156 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char28.png
--rw-r--r--   0        0        0      256 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char29.png
--rw-r--r--   0        0        0      342 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char3.png
--rw-r--r--   0        0        0      113 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char30.png
--rw-r--r--   0        0        0      186 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char31.png
--rw-r--r--   0        0        0      156 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char32.png
--rw-r--r--   0        0        0      213 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char33.png
--rw-r--r--   0        0        0      216 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char34.png
--rw-r--r--   0        0        0      221 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char35.png
--rw-r--r--   0        0        0      139 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char36.png
--rw-r--r--   0        0        0      222 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char37.png
--rw-r--r--   0        0        0      140 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char38.png
--rw-r--r--   0        0        0      152 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char39.png
--rw-r--r--   0        0        0      275 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char4.png
--rw-r--r--   0        0        0      236 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char40.png
--rw-r--r--   0        0        0      282 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char41.png
--rw-r--r--   0        0        0      264 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char42.png
--rw-r--r--   0        0        0      287 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char43.png
--rw-r--r--   0        0        0      230 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char44.png
--rw-r--r--   0        0        0      186 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char45.png
--rw-r--r--   0        0        0       78 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char46.png
--rw-r--r--   0        0        0      189 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char47.png
--rw-r--r--   0        0        0      179 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char48.png
--rw-r--r--   0        0        0      291 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char5.png
--rw-r--r--   0        0        0      147 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char6.png
--rw-r--r--   0        0        0      207 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char7.png
--rw-r--r--   0        0        0      315 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char8.png
--rw-r--r--   0        0        0      392 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_1_char9.png
--rw-r--r--   0        0        0      124 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char0.png
--rw-r--r--   0        0        0       84 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char1.png
--rw-r--r--   0        0        0      366 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char10.png
--rw-r--r--   0        0        0      385 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char11.png
--rw-r--r--   0        0        0      383 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char12.png
--rw-r--r--   0        0        0      353 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char13.png
--rw-r--r--   0        0        0      352 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char14.png
--rw-r--r--   0        0        0      292 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char15.png
--rw-r--r--   0        0        0      308 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char16.png
--rw-r--r--   0        0        0      248 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char17.png
--rw-r--r--   0        0        0      247 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char18.png
--rw-r--r--   0        0        0      255 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char19.png
--rw-r--r--   0        0        0      327 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char2.png
--rw-r--r--   0        0        0      229 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char20.png
--rw-r--r--   0        0        0      173 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char21.png
--rw-r--r--   0        0        0      171 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char22.png
--rw-r--r--   0        0        0      194 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char23.png
--rw-r--r--   0        0        0      162 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char24.png
--rw-r--r--   0        0        0      245 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char25.png
--rw-r--r--   0        0        0      354 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char26.png
--rw-r--r--   0        0        0      354 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char27.png
--rw-r--r--   0        0        0      348 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char28.png
--rw-r--r--   0        0        0      372 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char29.png
--rw-r--r--   0        0        0      122 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char3.png
--rw-r--r--   0        0        0      372 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char30.png
--rw-r--r--   0        0        0      333 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char31.png
--rw-r--r--   0        0        0      227 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char32.png
--rw-r--r--   0        0        0      397 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char33.png
--rw-r--r--   0        0        0      279 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char34.png
--rw-r--r--   0        0        0      272 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char35.png
--rw-r--r--   0        0        0      293 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char36.png
--rw-r--r--   0        0        0      259 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char37.png
--rw-r--r--   0        0        0      347 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char38.png
--rw-r--r--   0        0        0      216 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char39.png
--rw-r--r--   0        0        0      390 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char4.png
--rw-r--r--   0        0        0      282 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char40.png
--rw-r--r--   0        0        0      243 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char41.png
--rw-r--r--   0        0        0      242 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char42.png
--rw-r--r--   0        0        0      261 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char43.png
--rw-r--r--   0        0        0      168 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char5.png
--rw-r--r--   0        0        0      235 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char6.png
--rw-r--r--   0        0        0      232 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char7.png
--rw-r--r--   0        0        0      208 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char8.png
--rw-r--r--   0        0        0      370 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_2_char9.png
--rw-r--r--   0        0        0      271 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char0.png
--rw-r--r--   0        0        0      246 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char1.png
--rw-r--r--   0        0        0      164 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char10.png
--rw-r--r--   0        0        0      187 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char11.png
--rw-r--r--   0        0        0      156 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char12.png
--rw-r--r--   0        0        0      312 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char13.png
--rw-r--r--   0        0        0      235 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char14.png
--rw-r--r--   0        0        0      275 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char15.png
--rw-r--r--   0        0        0      271 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char16.png
--rw-r--r--   0        0        0      292 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char17.png
--rw-r--r--   0        0        0      286 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char18.png
--rw-r--r--   0        0        0      267 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char19.png
--rw-r--r--   0        0        0      273 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char2.png
--rw-r--r--   0        0        0      128 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char20.png
--rw-r--r--   0        0        0      287 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char21.png
--rw-r--r--   0        0        0      220 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char22.png
--rw-r--r--   0        0        0      219 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char23.png
--rw-r--r--   0        0        0      233 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char24.png
--rw-r--r--   0        0        0      208 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char25.png
--rw-r--r--   0        0        0      348 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char26.png
--rw-r--r--   0        0        0      225 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char27.png
--rw-r--r--   0        0        0      333 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char28.png
--rw-r--r--   0        0        0      315 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char29.png
--rw-r--r--   0        0        0      249 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char3.png
--rw-r--r--   0        0        0      218 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char30.png
--rw-r--r--   0        0        0      372 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char31.png
--rw-r--r--   0        0        0      268 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char32.png
--rw-r--r--   0        0        0      345 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char33.png
--rw-r--r--   0        0        0      245 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char34.png
--rw-r--r--   0        0        0      316 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char35.png
--rw-r--r--   0        0        0      258 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char36.png
--rw-r--r--   0        0        0      330 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char37.png
--rw-r--r--   0        0        0      270 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char38.png
--rw-r--r--   0        0        0      298 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char39.png
--rw-r--r--   0        0        0      253 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char4.png
--rw-r--r--   0        0        0      233 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char40.png
--rw-r--r--   0        0        0      341 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char41.png
--rw-r--r--   0        0        0      278 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char42.png
--rw-r--r--   0        0        0      337 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char43.png
--rw-r--r--   0        0        0      272 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char44.png
--rw-r--r--   0        0        0      249 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char45.png
--rw-r--r--   0        0        0      225 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char46.png
--rw-r--r--   0        0        0      198 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char47.png
--rw-r--r--   0        0        0      206 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char48.png
--rw-r--r--   0        0        0      265 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char5.png
--rw-r--r--   0        0        0      259 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char6.png
--rw-r--r--   0        0        0      279 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char7.png
--rw-r--r--   0        0        0      253 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char8.png
--rw-r--r--   0        0        0      167 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_3_char9.png
--rw-r--r--   0        0        0      250 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char0.png
--rw-r--r--   0        0        0      263 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char1.png
--rw-r--r--   0        0        0      336 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char10.png
--rw-r--r--   0        0        0      379 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char11.png
--rw-r--r--   0        0        0      306 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char12.png
--rw-r--r--   0        0        0      350 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char13.png
--rw-r--r--   0        0        0      327 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char14.png
--rw-r--r--   0        0        0      365 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char15.png
--rw-r--r--   0        0        0      240 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char16.png
--rw-r--r--   0        0        0      255 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char17.png
--rw-r--r--   0        0        0      171 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char18.png
--rw-r--r--   0        0        0      185 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char19.png
--rw-r--r--   0        0        0      227 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char2.png
--rw-r--r--   0        0        0      180 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char20.png
--rw-r--r--   0        0        0      178 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char21.png
--rw-r--r--   0        0        0      127 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char22.png
--rw-r--r--   0        0        0      122 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char23.png
--rw-r--r--   0        0        0      171 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char24.png
--rw-r--r--   0        0        0      173 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char25.png
--rw-r--r--   0        0        0      154 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char26.png
--rw-r--r--   0        0        0      175 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char27.png
--rw-r--r--   0        0        0      156 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char28.png
--rw-r--r--   0        0        0      112 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char29.png
--rw-r--r--   0        0        0      240 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char3.png
--rw-r--r--   0        0        0      179 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char30.png
--rw-r--r--   0        0        0      210 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char31.png
--rw-r--r--   0        0        0      240 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char32.png
--rw-r--r--   0        0        0      210 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char33.png
--rw-r--r--   0        0        0      392 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char34.png
--rw-r--r--   0        0        0      315 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char35.png
--rw-r--r--   0        0        0      242 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char36.png
--rw-r--r--   0        0        0      204 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char37.png
--rw-r--r--   0        0        0      167 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char38.png
--rw-r--r--   0        0        0      193 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char39.png
--rw-r--r--   0        0        0      218 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char4.png
--rw-r--r--   0        0        0      163 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char40.png
--rw-r--r--   0        0        0      202 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char41.png
--rw-r--r--   0        0        0      163 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char42.png
--rw-r--r--   0        0        0      180 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char43.png
--rw-r--r--   0        0        0      143 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char44.png
--rw-r--r--   0        0        0      208 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char45.png
--rw-r--r--   0        0        0      170 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char46.png
--rw-r--r--   0        0        0      345 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char47.png
--rw-r--r--   0        0        0      219 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char48.png
--rw-r--r--   0        0        0      340 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char49.png
--rw-r--r--   0        0        0      243 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char5.png
--rw-r--r--   0        0        0      262 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char6.png
--rw-r--r--   0        0        0      277 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char7.png
--rw-r--r--   0        0        0      345 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char8.png
--rw-r--r--   0        0        0      388 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_4_char9.png
--rw-r--r--   0        0        0      207 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char0.png
--rw-r--r--   0        0        0      367 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char1.png
--rw-r--r--   0        0        0      368 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char10.png
--rw-r--r--   0        0        0      273 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char11.png
--rw-r--r--   0        0        0      287 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char12.png
--rw-r--r--   0        0        0      258 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char13.png
--rw-r--r--   0        0        0      336 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char14.png
--rw-r--r--   0        0        0      189 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char15.png
--rw-r--r--   0        0        0      336 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char16.png
--rw-r--r--   0        0        0      190 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char17.png
--rw-r--r--   0        0        0      360 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char18.png
--rw-r--r--   0        0        0      206 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char19.png
--rw-r--r--   0        0        0      238 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char2.png
--rw-r--r--   0        0        0      351 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char20.png
--rw-r--r--   0        0        0      268 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char21.png
--rw-r--r--   0        0        0      368 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char22.png
--rw-r--r--   0        0        0      282 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char23.png
--rw-r--r--   0        0        0      342 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char24.png
--rw-r--r--   0        0        0      276 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char25.png
--rw-r--r--   0        0        0      370 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char26.png
--rw-r--r--   0        0        0      276 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char27.png
--rw-r--r--   0        0        0      203 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char28.png
--rw-r--r--   0        0        0      197 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char29.png
--rw-r--r--   0        0        0      238 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char3.png
--rw-r--r--   0        0        0      226 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char30.png
--rw-r--r--   0        0        0      193 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char31.png
--rw-r--r--   0        0        0      152 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char32.png
--rw-r--r--   0        0        0      148 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char33.png
--rw-r--r--   0        0        0      280 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char34.png
--rw-r--r--   0        0        0      226 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char35.png
--rw-r--r--   0        0        0      221 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char36.png
--rw-r--r--   0        0        0      172 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char37.png
--rw-r--r--   0        0        0      267 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char38.png
--rw-r--r--   0        0        0      211 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char4.png
--rw-r--r--   0        0        0      187 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char5.png
--rw-r--r--   0        0        0      303 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char6.png
--rw-r--r--   0        0        0      228 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char7.png
--rw-r--r--   0        0        0      360 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char8.png
--rw-r--r--   0        0        0      266 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_5_char9.png
--rw-r--r--   0        0        0      209 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_6_char0.png
--rw-r--r--   0        0        0      289 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_6_char1.png
--rw-r--r--   0        0        0      350 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_6_char10.png
--rw-r--r--   0        0        0      337 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_6_char11.png
--rw-r--r--   0        0        0      341 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_6_char12.png
--rw-r--r--   0        0        0      280 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_6_char13.png
--rw-r--r--   0        0        0      311 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_6_char14.png
--rw-r--r--   0        0        0      262 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_6_char15.png
--rw-r--r--   0        0        0      359 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_6_char16.png
--rw-r--r--   0        0        0      297 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_6_char17.png
--rw-r--r--   0        0        0       90 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_6_char18.png
--rw-r--r--   0        0        0      226 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_6_char2.png
--rw-r--r--   0        0        0      287 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_6_char3.png
--rw-r--r--   0        0        0      208 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_6_char4.png
--rw-r--r--   0        0        0      253 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_6_char5.png
--rw-r--r--   0        0        0      194 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_6_char6.png
--rw-r--r--   0        0        0      484 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_6_char7.png
--rw-r--r--   0        0        0      344 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_6_char8.png
--rw-r--r--   0        0        0      368 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/line_6_char9.png
--rw-r--r--   0        0        0     8692 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/metadata.csv
--rw-r--r--   0        0        0   426999 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/my_alphabet.png
--rw-r--r--   0        0        0      792 2023-04-07 15:50:41.222883 np_gui-0.0.2/np_gui/alphabet/liberation_serif/transcription.txt
--rw-r--r--   0        0        0      246 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/liberation_serif_alphabet_data
--rw-r--r--   0        0        0      792 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/my_alphabet.txt
--rw-r--r--   0        0        0    18291 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/my_alphabet_liberation_serif.odt
--rw-r--r--   0        0        0   426999 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/my_alphabet_liberation_serif.png
--rw-r--r--   0        0        0     1633 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/utf8_sequence_0-0x10ffff_assigned_printable/LICENSE
--rw-r--r--   0        0        0  1115699 2023-04-07 15:50:41.218884 np_gui-0.0.2/np_gui/alphabet/utf8_sequence_0-0x10ffff_assigned_printable/utf8_sequence_0-0x10ffff_assigned_printable.txt
--rw-r--r--   0        0        0     4127 2023-04-09 21:38:45.641967 np_gui-0.0.2/np_gui/colors.py
--rw-r--r--   0        0        0     8110 2023-04-09 22:40:46.825641 np_gui-0.0.2/np_gui/image_annotation.py
--rw-r--r--   0        0        0    23218 2023-04-08 18:48:07.876574 np_gui-0.0.2/np_gui/np_clickable_image.py
--rw-r--r--   0        0        0      563 2023-04-10 21:20:08.354885 np_gui-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2433 1970-01-01 00:00:00.000000 np_gui-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2773 2023-04-11 12:23:04.710895 np_gui-0.0.3/README.md
+-rw-r--r--   0        0        0     1454 2023-04-10 21:22:19.221466 np_gui-0.0.3/np_gui/__init__.py
+-rw-r--r--   0        0        0      120 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char0.png
+-rw-r--r--   0        0        0      123 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char1.png
+-rw-r--r--   0        0        0      106 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char10.png
+-rw-r--r--   0        0        0      136 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char11.png
+-rw-r--r--   0        0        0       79 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char12.png
+-rw-r--r--   0        0        0       97 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char13.png
+-rw-r--r--   0        0        0      164 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char14.png
+-rw-r--r--   0        0        0      244 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char15.png
+-rw-r--r--   0        0        0      152 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char16.png
+-rw-r--r--   0        0        0      242 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char17.png
+-rw-r--r--   0        0        0      258 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char18.png
+-rw-r--r--   0        0        0      221 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char19.png
+-rw-r--r--   0        0        0      229 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char2.png
+-rw-r--r--   0        0        0      205 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char20.png
+-rw-r--r--   0        0        0      276 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char21.png
+-rw-r--r--   0        0        0      214 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char22.png
+-rw-r--r--   0        0        0      264 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char23.png
+-rw-r--r--   0        0        0      273 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char24.png
+-rw-r--r--   0        0        0      110 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char25.png
+-rw-r--r--   0        0        0      157 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char26.png
+-rw-r--r--   0        0        0      217 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char27.png
+-rw-r--r--   0        0        0       88 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char28.png
+-rw-r--r--   0        0        0      228 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char29.png
+-rw-r--r--   0        0        0      297 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char3.png
+-rw-r--r--   0        0        0      218 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char30.png
+-rw-r--r--   0        0        0      496 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char31.png
+-rw-r--r--   0        0        0      298 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char32.png
+-rw-r--r--   0        0        0      247 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char33.png
+-rw-r--r--   0        0        0      252 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char34.png
+-rw-r--r--   0        0        0      246 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char35.png
+-rw-r--r--   0        0        0      178 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char36.png
+-rw-r--r--   0        0        0      156 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char37.png
+-rw-r--r--   0        0        0      269 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char38.png
+-rw-r--r--   0        0        0      158 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char39.png
+-rw-r--r--   0        0        0      408 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char4.png
+-rw-r--r--   0        0        0      114 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char40.png
+-rw-r--r--   0        0        0      161 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char41.png
+-rw-r--r--   0        0        0      330 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char42.png
+-rw-r--r--   0        0        0      141 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char43.png
+-rw-r--r--   0        0        0      323 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char44.png
+-rw-r--r--   0        0        0      392 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char5.png
+-rw-r--r--   0        0        0       93 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char6.png
+-rw-r--r--   0        0        0      228 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char7.png
+-rw-r--r--   0        0        0      221 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char8.png
+-rw-r--r--   0        0        0      216 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_0_char9.png
+-rw-r--r--   0        0        0      285 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char0.png
+-rw-r--r--   0        0        0      290 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char1.png
+-rw-r--r--   0        0        0      367 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char10.png
+-rw-r--r--   0        0        0      279 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char11.png
+-rw-r--r--   0        0        0      270 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char12.png
+-rw-r--r--   0        0        0      112 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char13.png
+-rw-r--r--   0        0        0      172 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char14.png
+-rw-r--r--   0        0        0      111 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char15.png
+-rw-r--r--   0        0        0      225 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char16.png
+-rw-r--r--   0        0        0       94 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char17.png
+-rw-r--r--   0        0        0      134 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char18.png
+-rw-r--r--   0        0        0      198 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char19.png
+-rw-r--r--   0        0        0      204 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char2.png
+-rw-r--r--   0        0        0      218 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char20.png
+-rw-r--r--   0        0        0      192 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char21.png
+-rw-r--r--   0        0        0      216 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char22.png
+-rw-r--r--   0        0        0      202 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char23.png
+-rw-r--r--   0        0        0      167 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char24.png
+-rw-r--r--   0        0        0      318 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char25.png
+-rw-r--r--   0        0        0      173 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char26.png
+-rw-r--r--   0        0        0      137 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char27.png
+-rw-r--r--   0        0        0      156 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char28.png
+-rw-r--r--   0        0        0      256 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char29.png
+-rw-r--r--   0        0        0      342 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char3.png
+-rw-r--r--   0        0        0      113 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char30.png
+-rw-r--r--   0        0        0      186 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char31.png
+-rw-r--r--   0        0        0      156 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char32.png
+-rw-r--r--   0        0        0      213 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char33.png
+-rw-r--r--   0        0        0      216 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char34.png
+-rw-r--r--   0        0        0      221 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char35.png
+-rw-r--r--   0        0        0      139 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char36.png
+-rw-r--r--   0        0        0      222 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char37.png
+-rw-r--r--   0        0        0      140 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char38.png
+-rw-r--r--   0        0        0      152 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char39.png
+-rw-r--r--   0        0        0      275 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char4.png
+-rw-r--r--   0        0        0      236 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char40.png
+-rw-r--r--   0        0        0      282 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char41.png
+-rw-r--r--   0        0        0      264 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char42.png
+-rw-r--r--   0        0        0      287 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char43.png
+-rw-r--r--   0        0        0      230 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char44.png
+-rw-r--r--   0        0        0      186 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char45.png
+-rw-r--r--   0        0        0       78 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char46.png
+-rw-r--r--   0        0        0      189 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char47.png
+-rw-r--r--   0        0        0      179 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char48.png
+-rw-r--r--   0        0        0      291 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char5.png
+-rw-r--r--   0        0        0      147 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char6.png
+-rw-r--r--   0        0        0      207 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char7.png
+-rw-r--r--   0        0        0      315 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char8.png
+-rw-r--r--   0        0        0      392 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_1_char9.png
+-rw-r--r--   0        0        0      124 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char0.png
+-rw-r--r--   0        0        0       84 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char1.png
+-rw-r--r--   0        0        0      366 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char10.png
+-rw-r--r--   0        0        0      385 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char11.png
+-rw-r--r--   0        0        0      383 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char12.png
+-rw-r--r--   0        0        0      353 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char13.png
+-rw-r--r--   0        0        0      352 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char14.png
+-rw-r--r--   0        0        0      292 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char15.png
+-rw-r--r--   0        0        0      308 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char16.png
+-rw-r--r--   0        0        0      248 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char17.png
+-rw-r--r--   0        0        0      247 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char18.png
+-rw-r--r--   0        0        0      255 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char19.png
+-rw-r--r--   0        0        0      327 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char2.png
+-rw-r--r--   0        0        0      229 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char20.png
+-rw-r--r--   0        0        0      173 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char21.png
+-rw-r--r--   0        0        0      171 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char22.png
+-rw-r--r--   0        0        0      194 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char23.png
+-rw-r--r--   0        0        0      162 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char24.png
+-rw-r--r--   0        0        0      245 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char25.png
+-rw-r--r--   0        0        0      354 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char26.png
+-rw-r--r--   0        0        0      354 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char27.png
+-rw-r--r--   0        0        0      348 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char28.png
+-rw-r--r--   0        0        0      372 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char29.png
+-rw-r--r--   0        0        0      122 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char3.png
+-rw-r--r--   0        0        0      372 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char30.png
+-rw-r--r--   0        0        0      333 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char31.png
+-rw-r--r--   0        0        0      227 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char32.png
+-rw-r--r--   0        0        0      397 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char33.png
+-rw-r--r--   0        0        0      279 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char34.png
+-rw-r--r--   0        0        0      272 2023-04-07 15:50:41.218884 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char35.png
+-rw-r--r--   0        0        0      293 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char36.png
+-rw-r--r--   0        0        0      259 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char37.png
+-rw-r--r--   0        0        0      347 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char38.png
+-rw-r--r--   0        0        0      216 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char39.png
+-rw-r--r--   0        0        0      390 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char4.png
+-rw-r--r--   0        0        0      282 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char40.png
+-rw-r--r--   0        0        0      243 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char41.png
+-rw-r--r--   0        0        0      242 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char42.png
+-rw-r--r--   0        0        0      261 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char43.png
+-rw-r--r--   0        0        0      168 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char5.png
+-rw-r--r--   0        0        0      235 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char6.png
+-rw-r--r--   0        0        0      232 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char7.png
+-rw-r--r--   0        0        0      208 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char8.png
+-rw-r--r--   0        0        0      370 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_2_char9.png
+-rw-r--r--   0        0        0      271 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char0.png
+-rw-r--r--   0        0        0      246 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char1.png
+-rw-r--r--   0        0        0      164 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char10.png
+-rw-r--r--   0        0        0      187 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char11.png
+-rw-r--r--   0        0        0      156 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char12.png
+-rw-r--r--   0        0        0      312 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char13.png
+-rw-r--r--   0        0        0      235 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char14.png
+-rw-r--r--   0        0        0      275 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char15.png
+-rw-r--r--   0        0        0      271 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char16.png
+-rw-r--r--   0        0        0      292 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char17.png
+-rw-r--r--   0        0        0      286 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char18.png
+-rw-r--r--   0        0        0      267 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char19.png
+-rw-r--r--   0        0        0      273 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char2.png
+-rw-r--r--   0        0        0      128 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char20.png
+-rw-r--r--   0        0        0      287 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char21.png
+-rw-r--r--   0        0        0      220 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char22.png
+-rw-r--r--   0        0        0      219 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char23.png
+-rw-r--r--   0        0        0      233 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char24.png
+-rw-r--r--   0        0        0      208 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char25.png
+-rw-r--r--   0        0        0      348 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char26.png
+-rw-r--r--   0        0        0      225 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char27.png
+-rw-r--r--   0        0        0      333 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char28.png
+-rw-r--r--   0        0        0      315 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char29.png
+-rw-r--r--   0        0        0      249 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char3.png
+-rw-r--r--   0        0        0      218 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char30.png
+-rw-r--r--   0        0        0      372 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char31.png
+-rw-r--r--   0        0        0      268 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char32.png
+-rw-r--r--   0        0        0      345 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char33.png
+-rw-r--r--   0        0        0      245 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char34.png
+-rw-r--r--   0        0        0      316 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char35.png
+-rw-r--r--   0        0        0      258 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char36.png
+-rw-r--r--   0        0        0      330 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char37.png
+-rw-r--r--   0        0        0      270 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char38.png
+-rw-r--r--   0        0        0      298 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char39.png
+-rw-r--r--   0        0        0      253 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char4.png
+-rw-r--r--   0        0        0      233 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char40.png
+-rw-r--r--   0        0        0      341 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char41.png
+-rw-r--r--   0        0        0      278 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char42.png
+-rw-r--r--   0        0        0      337 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char43.png
+-rw-r--r--   0        0        0      272 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char44.png
+-rw-r--r--   0        0        0      249 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char45.png
+-rw-r--r--   0        0        0      225 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char46.png
+-rw-r--r--   0        0        0      198 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char47.png
+-rw-r--r--   0        0        0      206 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char48.png
+-rw-r--r--   0        0        0      265 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char5.png
+-rw-r--r--   0        0        0      259 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char6.png
+-rw-r--r--   0        0        0      279 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char7.png
+-rw-r--r--   0        0        0      253 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char8.png
+-rw-r--r--   0        0        0      167 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_3_char9.png
+-rw-r--r--   0        0        0      250 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char0.png
+-rw-r--r--   0        0        0      263 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char1.png
+-rw-r--r--   0        0        0      336 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char10.png
+-rw-r--r--   0        0        0      379 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char11.png
+-rw-r--r--   0        0        0      306 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char12.png
+-rw-r--r--   0        0        0      350 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char13.png
+-rw-r--r--   0        0        0      327 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char14.png
+-rw-r--r--   0        0        0      365 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char15.png
+-rw-r--r--   0        0        0      240 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char16.png
+-rw-r--r--   0        0        0      255 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char17.png
+-rw-r--r--   0        0        0      171 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char18.png
+-rw-r--r--   0        0        0      185 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char19.png
+-rw-r--r--   0        0        0      227 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char2.png
+-rw-r--r--   0        0        0      180 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char20.png
+-rw-r--r--   0        0        0      178 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char21.png
+-rw-r--r--   0        0        0      127 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char22.png
+-rw-r--r--   0        0        0      122 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char23.png
+-rw-r--r--   0        0        0      171 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char24.png
+-rw-r--r--   0        0        0      173 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char25.png
+-rw-r--r--   0        0        0      154 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char26.png
+-rw-r--r--   0        0        0      175 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char27.png
+-rw-r--r--   0        0        0      156 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char28.png
+-rw-r--r--   0        0        0      112 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char29.png
+-rw-r--r--   0        0        0      240 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char3.png
+-rw-r--r--   0        0        0      179 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char30.png
+-rw-r--r--   0        0        0      210 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char31.png
+-rw-r--r--   0        0        0      240 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char32.png
+-rw-r--r--   0        0        0      210 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char33.png
+-rw-r--r--   0        0        0      392 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char34.png
+-rw-r--r--   0        0        0      315 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char35.png
+-rw-r--r--   0        0        0      242 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char36.png
+-rw-r--r--   0        0        0      204 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char37.png
+-rw-r--r--   0        0        0      167 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char38.png
+-rw-r--r--   0        0        0      193 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char39.png
+-rw-r--r--   0        0        0      218 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char4.png
+-rw-r--r--   0        0        0      163 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char40.png
+-rw-r--r--   0        0        0      202 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char41.png
+-rw-r--r--   0        0        0      163 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char42.png
+-rw-r--r--   0        0        0      180 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char43.png
+-rw-r--r--   0        0        0      143 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char44.png
+-rw-r--r--   0        0        0      208 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char45.png
+-rw-r--r--   0        0        0      170 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char46.png
+-rw-r--r--   0        0        0      345 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char47.png
+-rw-r--r--   0        0        0      219 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char48.png
+-rw-r--r--   0        0        0      340 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char49.png
+-rw-r--r--   0        0        0      243 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char5.png
+-rw-r--r--   0        0        0      262 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char6.png
+-rw-r--r--   0        0        0      277 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char7.png
+-rw-r--r--   0        0        0      345 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char8.png
+-rw-r--r--   0        0        0      388 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_4_char9.png
+-rw-r--r--   0        0        0      207 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char0.png
+-rw-r--r--   0        0        0      367 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char1.png
+-rw-r--r--   0        0        0      368 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char10.png
+-rw-r--r--   0        0        0      273 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char11.png
+-rw-r--r--   0        0        0      287 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char12.png
+-rw-r--r--   0        0        0      258 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char13.png
+-rw-r--r--   0        0        0      336 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char14.png
+-rw-r--r--   0        0        0      189 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char15.png
+-rw-r--r--   0        0        0      336 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char16.png
+-rw-r--r--   0        0        0      190 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char17.png
+-rw-r--r--   0        0        0      360 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char18.png
+-rw-r--r--   0        0        0      206 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char19.png
+-rw-r--r--   0        0        0      238 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char2.png
+-rw-r--r--   0        0        0      351 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char20.png
+-rw-r--r--   0        0        0      268 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char21.png
+-rw-r--r--   0        0        0      368 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char22.png
+-rw-r--r--   0        0        0      282 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char23.png
+-rw-r--r--   0        0        0      342 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char24.png
+-rw-r--r--   0        0        0      276 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char25.png
+-rw-r--r--   0        0        0      370 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char26.png
+-rw-r--r--   0        0        0      276 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char27.png
+-rw-r--r--   0        0        0      203 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char28.png
+-rw-r--r--   0        0        0      197 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char29.png
+-rw-r--r--   0        0        0      238 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char3.png
+-rw-r--r--   0        0        0      226 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char30.png
+-rw-r--r--   0        0        0      193 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char31.png
+-rw-r--r--   0        0        0      152 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char32.png
+-rw-r--r--   0        0        0      148 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char33.png
+-rw-r--r--   0        0        0      280 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char34.png
+-rw-r--r--   0        0        0      226 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char35.png
+-rw-r--r--   0        0        0      221 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char36.png
+-rw-r--r--   0        0        0      172 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char37.png
+-rw-r--r--   0        0        0      267 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char38.png
+-rw-r--r--   0        0        0      211 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char4.png
+-rw-r--r--   0        0        0      187 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char5.png
+-rw-r--r--   0        0        0      303 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char6.png
+-rw-r--r--   0        0        0      228 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char7.png
+-rw-r--r--   0        0        0      360 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char8.png
+-rw-r--r--   0        0        0      266 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_5_char9.png
+-rw-r--r--   0        0        0      209 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char0.png
+-rw-r--r--   0        0        0      289 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char1.png
+-rw-r--r--   0        0        0      350 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char10.png
+-rw-r--r--   0        0        0      337 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char11.png
+-rw-r--r--   0        0        0      341 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char12.png
+-rw-r--r--   0        0        0      280 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char13.png
+-rw-r--r--   0        0        0      311 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char14.png
+-rw-r--r--   0        0        0      262 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char15.png
+-rw-r--r--   0        0        0      359 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char16.png
+-rw-r--r--   0        0        0      297 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char17.png
+-rw-r--r--   0        0        0       90 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char18.png
+-rw-r--r--   0        0        0      226 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char2.png
+-rw-r--r--   0        0        0      287 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char3.png
+-rw-r--r--   0        0        0      208 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char4.png
+-rw-r--r--   0        0        0      253 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char5.png
+-rw-r--r--   0        0        0      194 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char6.png
+-rw-r--r--   0        0        0      484 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char7.png
+-rw-r--r--   0        0        0      344 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char8.png
+-rw-r--r--   0        0        0      368 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/line_6_char9.png
+-rw-r--r--   0        0        0     8692 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/metadata.csv
+-rw-r--r--   0        0        0   426999 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/my_alphabet.png
+-rw-r--r--   0        0        0      792 2023-04-07 15:50:41.222883 np_gui-0.0.3/np_gui/alphabet/liberation_serif/transcription.txt
+-rw-r--r--   0        0        0     4127 2023-04-09 21:38:45.641967 np_gui-0.0.3/np_gui/colors.py
+-rw-r--r--   0        0        0     8110 2023-04-09 22:40:46.825641 np_gui-0.0.3/np_gui/image_annotation.py
+-rw-r--r--   0        0        0    23218 2023-04-08 18:48:07.876574 np_gui-0.0.3/np_gui/np_clickable_image.py
+-rw-r--r--   0        0        0      564 2023-04-11 14:47:45.313214 np_gui-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3370 1970-01-01 00:00:00.000000 np_gui-0.0.3/PKG-INFO
```

### Comparing `np_gui-0.0.2/README.md` & `np_gui-0.0.3/np_gui/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-# npGUI
+""" 
++++++++++++++++++++++
+The np_gui package
++++++++++++++++++++++
 
 This package implements Graphical User Interfaces from a NumPy user
 perspective: every image corresponds to an ndarray.
 
-The main goal of this package is to provide a 
-simple way (given certain background and tastes) to build *prototypes* of graphical user interfaces.
-In particular, we do not claim for computational performance.
-
----
-## Main features
-The core class is
+The core class is \
 ClickableImage whose instances' attributes are: 
 
 
 * a dictionary of parameter values,
 * a callable that returns an image of fixed shape,
 * regions in that shape defined as boolean images of the same shape 
 * and their corresponding callbacks.
@@ -30,23 +27,16 @@
 its altered values; whence the interaction with the user.
 
 These objects can be stacked vertically and horizontally to compose more
 complex ones. A certain number of subclasses are proposed as basic 
 building blocks. The stacked blocks may have parameter keywords in common,
 which allows for interactions between them.
 
-## Installation
-This package can be installed with pip as follows.
-
-```
-$ pip install np_gui
-```
-
-To avoid [depency hell](https://en.wikipedia.org/wiki/Dependency_hell), you might consider installing this package in a virtual environment.
-
-## Documentation
-
-A detailed documentation of this package is available in pdf and html
-format within the ./doc/ folder of [its GitHub repository](https://github.com/completementgaga/npGUI).
+The code is organized in three submodules as follows.
 
+* **np_clickable_images** contains the definition of the ClickableImage \
+class and some subclasses,
+* **colors** contains some color management facilities and
+* **image_annotation** regards putting text in an image.
 
 
+"""
```

### Comparing `np_gui-0.0.2/np_gui/alphabet/liberation_serif/metadata.csv` & `np_gui-0.0.3/np_gui/alphabet/liberation_serif/metadata.csv`

 * *Files identical despite different names*

### Comparing `np_gui-0.0.2/np_gui/alphabet/liberation_serif/my_alphabet.png` & `np_gui-0.0.3/np_gui/alphabet/liberation_serif/my_alphabet.png`

 * *Files identical despite different names*

### Comparing `np_gui-0.0.2/np_gui/alphabet/liberation_serif/transcription.txt` & `np_gui-0.0.3/np_gui/alphabet/liberation_serif/transcription.txt`

 * *Files identical despite different names*

### Comparing `np_gui-0.0.2/np_gui/colors.py` & `np_gui-0.0.3/np_gui/colors.py`

 * *Files identical despite different names*

### Comparing `np_gui-0.0.2/np_gui/image_annotation.py` & `np_gui-0.0.3/np_gui/image_annotation.py`

 * *Files identical despite different names*

### Comparing `np_gui-0.0.2/np_gui/np_clickable_image.py` & `np_gui-0.0.3/np_gui/np_clickable_image.py`

 * *Files identical despite different names*

### Comparing `np_gui-0.0.2/PKG-INFO` & `np_gui-0.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: np-gui
-Version: 0.0.2
+Version: 0.0.3
 Summary: This package implements Graphical User Interfaces from a NumPy user perspective.
 License: MIT
 Author: Gaël Cousin
 Author-email: gcousin333@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10.6,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: matplotlib (>=3.5.1,<4.0.0)
-Requires-Dist: numpy (>=1.24.2,<2.0.0)
-Requires-Dist: scikit-image (>=0.20.0,<0.21.0)
-Requires-Dist: typeguard (>=3.0.2,<4.0.0)
+Requires-Dist: matplotlib (>=3.0.0,<4.0.0)
+Requires-Dist: numpy (>=1.21.0,<2.0.0)
+Requires-Dist: scikit-image (==0.19.0)
+Requires-Dist: typeguard (>=3.0.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 # npGUI
 
 This package implements Graphical User Interfaces from a NumPy user
 perspective: every image corresponds to an ndarray.
 
@@ -62,10 +61,49 @@
 To avoid [depency hell](https://en.wikipedia.org/wiki/Dependency_hell), you might consider installing this package in a virtual environment.
 
 ## Documentation
 
 A detailed documentation of this package is available in pdf and html
 format within the ./doc/ folder of [its GitHub repository](https://github.com/completementgaga/npGUI).
 
+## Demo
+
+Some demonstration scripts are provided on the [GitHub repository](https://github.com/completementgaga/npGUI).
+
+These are:
+* ./demo/puzzles/puzzles.py 
+    | Preview of the puzzles.py demo.|
+    |:-----------------------------:|
+    |<img src="./screenshots/puzzles_screenshot.png"  width="300em" title="clock.py preview">|
+
+* ./demo/clock/clock.py
+
+    | Preview of the clock.py demo.|
+    |:-----------------------------:|
+    |<img src="./screenshots/clock_screenshot.png"  width="300em" title="clock.py preview">|
+
+## Further developments of the project
+This package could benefit from several enhancements, among other things:
+ 
+ * develop additional specialized subclasses of ClickableImage,
+ * include keyboard interactions,
+ * lighten its memory usage.
+
+Feel free to open the discussion through issues and pull requests on the [GitHub repository](https://github.com/completementgaga/npGUI).
+
+Feedbacks are also welcome by e-mail or by giving the project a star.
+
+
+
+
+
+
+
+
+
+
+
+
+
```

