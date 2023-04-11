# Comparing `tmp/hcgf-0.0.7.tar.gz` & `tmp/hcgf-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcgf-0.0.7.tar", last modified: Tue Apr  4 17:32:43 2023, max compression
+gzip compressed data, was "hcgf-0.1.0.tar", last modified: Tue Apr 11 16:14:49 2023, max compression
```

## Comparing `hcgf-0.0.7.tar` & `hcgf-0.1.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwsr-x   0 wyd       (1013) anaconda  (1000)        0 2023-04-04 17:32:43.337711 hcgf-0.0.7/
--rw-rw-r--   0 wyd       (1013) anaconda  (1000)    11357 2023-03-25 10:33:36.000000 hcgf-0.0.7/LICENSE
--rw-rw-r--   0 wyd       (1013) anaconda  (1000)     4197 2023-04-04 17:32:43.337711 hcgf-0.0.7/PKG-INFO
--rw-rw-r--   0 wyd       (1013) anaconda  (1000)     3790 2023-04-04 17:26:48.000000 hcgf-0.0.7/README.md
-drwxrwsr-x   0 wyd       (1013) anaconda  (1000)        0 2023-04-04 17:32:43.333711 hcgf-0.0.7/hcgf/
--rw-rw-r--   0 wyd       (1013) anaconda  (1000)      154 2023-04-04 17:11:07.000000 hcgf-0.0.7/hcgf/__init__.py
-drwxrwsr-x   0 wyd       (1013) anaconda  (1000)        0 2023-04-04 17:32:43.334711 hcgf-0.0.7/hcgf/data_model/
--rw-rw-r--   0 wyd       (1013) anaconda  (1000)      923 2023-04-03 08:46:08.000000 hcgf-0.0.7/hcgf/data_model/__init__.py
-drwxrwsr-x   0 wyd       (1013) anaconda  (1000)        0 2023-04-04 17:32:43.334711 hcgf-0.0.7/hcgf/dataloader/
--rw-rw-r--   0 wyd       (1013) anaconda  (1000)      123 2023-03-25 10:33:36.000000 hcgf-0.0.7/hcgf/dataloader/__init__.py
--rw-rw-r--   0 wyd       (1013) anaconda  (1000)     3694 2023-04-03 09:06:49.000000 hcgf-0.0.7/hcgf/dataloader/data_collector.py
--rw-rw-r--   0 wyd       (1013) anaconda  (1000)     2737 2023-03-27 01:17:21.000000 hcgf-0.0.7/hcgf/dataloader/data_loader.py
--rw-rw-r--   0 wyd       (1013) anaconda  (1000)     1476 2023-04-03 09:05:55.000000 hcgf-0.0.7/hcgf/dataloader/dataset.py
-drwxrwsr-x   0 wyd       (1013) anaconda  (1000)        0 2023-04-04 17:32:43.335711 hcgf-0.0.7/hcgf/rm/
--rw-rw-r--   0 wyd       (1013) anaconda  (1000)        0 2023-04-02 15:08:12.000000 hcgf-0.0.7/hcgf/rm/__init__.py
--rw-rw-r--   0 wyd       (1013) anaconda  (1000)     1375 2023-04-02 15:08:12.000000 hcgf-0.0.7/hcgf/rm/reward_model.py
-drwxrwsr-x   0 wyd       (1013) anaconda  (1000)        0 2023-04-04 17:32:43.335711 hcgf-0.0.7/hcgf/sft/
--rw-rw-r--   0 wyd       (1013) anaconda  (1000)       28 2023-03-25 10:33:36.000000 hcgf-0.0.7/hcgf/sft/__init__.py
-drwxrwsr-x   0 wyd       (1013) anaconda  (1000)        0 2023-04-04 17:32:43.336711 hcgf-0.0.7/hcgf/sft/chatglm/
--rw-rw-r--   0 wyd       (1013) anaconda  (1000)      170 2023-04-03 07:50:12.000000 hcgf-0.0.7/hcgf/sft/chatglm/__init__.py
--rw-rw-r--   0 wyd       (1013) anaconda  (1000)     4111 2023-04-02 15:16:15.000000 hcgf-0.0.7/hcgf/sft/chatglm/configuration_chatglm.py
--rw-rw-r--   0 wyd       (1013) anaconda  (1000)    56515 2023-04-03 09:42:38.000000 hcgf-0.0.7/hcgf/sft/chatglm/modeling_chatglm.py
--rw-rw-r--   0 wyd       (1013) anaconda  (1000)    15053 2023-04-02 15:20:38.000000 hcgf-0.0.7/hcgf/sft/chatglm/quantization.py
--rw-rw-r--   0 wyd       (1013) anaconda  (1000)    17734 2023-04-02 15:17:10.000000 hcgf-0.0.7/hcgf/sft/chatglm/tokenization_chatglm.py
--rw-rw-r--   0 wyd       (1013) anaconda  (1000)     8918 2023-04-04 17:23:12.000000 hcgf-0.0.7/hcgf/sft/lora_ft.py
-drwxrwsr-x   0 wyd       (1013) anaconda  (1000)        0 2023-04-04 17:32:43.336711 hcgf-0.0.7/hcgf/trainer/
--rw-rw-r--   0 wyd       (1013) anaconda  (1000)       28 2023-03-25 10:33:36.000000 hcgf-0.0.7/hcgf/trainer/__init__.py
--rw-rw-r--   0 wyd       (1013) anaconda  (1000)     6066 2023-03-27 09:50:58.000000 hcgf-0.0.7/hcgf/trainer/trainer.py
-drwxrwsr-x   0 wyd       (1013) anaconda  (1000)        0 2023-04-04 17:32:43.336711 hcgf-0.0.7/hcgf/utils/
--rw-rw-r--   0 wyd       (1013) anaconda  (1000)      128 2023-04-03 09:51:01.000000 hcgf-0.0.7/hcgf/utils/__init__.py
--rw-rw-r--   0 wyd       (1013) anaconda  (1000)     2048 2023-04-04 15:51:29.000000 hcgf-0.0.7/hcgf/utils/utils.py
-drwxrwsr-x   0 wyd       (1013) anaconda  (1000)        0 2023-04-04 17:32:43.334711 hcgf-0.0.7/hcgf.egg-info/
--rw-rw-r--   0 wyd       (1013) anaconda  (1000)     4197 2023-04-04 17:32:43.000000 hcgf-0.0.7/hcgf.egg-info/PKG-INFO
--rw-rw-r--   0 wyd       (1013) anaconda  (1000)      751 2023-04-04 17:32:43.000000 hcgf-0.0.7/hcgf.egg-info/SOURCES.txt
--rw-rw-r--   0 wyd       (1013) anaconda  (1000)        1 2023-04-04 17:32:43.000000 hcgf-0.0.7/hcgf.egg-info/dependency_links.txt
--rw-rw-r--   0 wyd       (1013) anaconda  (1000)        5 2023-04-04 17:32:43.000000 hcgf-0.0.7/hcgf.egg-info/top_level.txt
--rw-rw-r--   0 wyd       (1013) anaconda  (1000)       38 2023-04-04 17:32:43.337711 hcgf-0.0.7/setup.cfg
--rw-rw-r--   0 wyd       (1013) anaconda  (1000)      883 2023-04-04 17:10:58.000000 hcgf-0.0.7/setup.py
-drwxrwsr-x   0 wyd       (1013) anaconda  (1000)        0 2023-04-04 17:32:43.336711 hcgf-0.0.7/tests/
--rw-rw-r--   0 wyd       (1013) anaconda  (1000)     4688 2023-04-02 15:10:18.000000 hcgf-0.0.7/tests/test_dataloader.py
--rw-rw-r--   0 wyd       (1013) anaconda  (1000)     1955 2023-04-04 17:06:00.000000 hcgf-0.0.7/tests/test_lora_ft.py
--rw-rw-r--   0 wyd       (1013) anaconda  (1000)     1304 2023-03-25 12:55:42.000000 hcgf-0.0.7/tests/test_trainer.py
--rw-rw-r--   0 wyd       (1013) anaconda  (1000)      453 2023-04-03 09:56:55.000000 hcgf-0.0.7/tests/test_utils.py
+drwxrwsr-x   0 wyd       (1013) anaconda  (1000)        0 2023-04-11 16:14:49.586121 hcgf-0.1.0/
+-rw-rw-r--   0 wyd       (1013) anaconda  (1000)    11357 2023-03-25 10:33:36.000000 hcgf-0.1.0/LICENSE
+-rw-rw-r--   0 wyd       (1013) anaconda  (1000)     5261 2023-04-11 16:14:49.586121 hcgf-0.1.0/PKG-INFO
+-rw-rw-r--   0 wyd       (1013) anaconda  (1000)     4854 2023-04-11 16:12:21.000000 hcgf-0.1.0/README.md
+drwxrwsr-x   0 wyd       (1013) anaconda  (1000)        0 2023-04-11 16:14:49.583121 hcgf-0.1.0/hcgf/
+-rw-rw-r--   0 wyd       (1013) anaconda  (1000)      154 2023-04-11 15:52:10.000000 hcgf-0.1.0/hcgf/__init__.py
+drwxrwsr-x   0 wyd       (1013) anaconda  (1000)        0 2023-04-11 16:14:49.584121 hcgf-0.1.0/hcgf/data_model/
+-rw-rw-r--   0 wyd       (1013) anaconda  (1000)      923 2023-04-03 08:46:08.000000 hcgf-0.1.0/hcgf/data_model/__init__.py
+drwxrwsr-x   0 wyd       (1013) anaconda  (1000)        0 2023-04-11 16:14:49.584121 hcgf-0.1.0/hcgf/dataloader/
+-rw-rw-r--   0 wyd       (1013) anaconda  (1000)      123 2023-03-25 10:33:36.000000 hcgf-0.1.0/hcgf/dataloader/__init__.py
+-rw-rw-r--   0 wyd       (1013) anaconda  (1000)     3916 2023-04-11 15:27:44.000000 hcgf-0.1.0/hcgf/dataloader/data_collector.py
+-rw-rw-r--   0 wyd       (1013) anaconda  (1000)     2737 2023-03-27 01:17:21.000000 hcgf-0.1.0/hcgf/dataloader/data_loader.py
+-rw-rw-r--   0 wyd       (1013) anaconda  (1000)     1476 2023-04-03 09:05:55.000000 hcgf-0.1.0/hcgf/dataloader/dataset.py
+drwxrwsr-x   0 wyd       (1013) anaconda  (1000)        0 2023-04-11 16:14:49.584121 hcgf-0.1.0/hcgf/rm/
+-rw-rw-r--   0 wyd       (1013) anaconda  (1000)        0 2023-04-02 15:08:12.000000 hcgf-0.1.0/hcgf/rm/__init__.py
+-rw-rw-r--   0 wyd       (1013) anaconda  (1000)     1375 2023-04-02 15:08:12.000000 hcgf-0.1.0/hcgf/rm/reward_model.py
+drwxrwsr-x   0 wyd       (1013) anaconda  (1000)        0 2023-04-11 16:14:49.584121 hcgf-0.1.0/hcgf/sft/
+-rw-rw-r--   0 wyd       (1013) anaconda  (1000)       28 2023-03-25 10:33:36.000000 hcgf-0.1.0/hcgf/sft/__init__.py
+drwxrwsr-x   0 wyd       (1013) anaconda  (1000)        0 2023-04-11 16:14:49.585121 hcgf-0.1.0/hcgf/sft/chatglm/
+-rw-rw-r--   0 wyd       (1013) anaconda  (1000)      170 2023-04-03 07:50:12.000000 hcgf-0.1.0/hcgf/sft/chatglm/__init__.py
+-rw-rw-r--   0 wyd       (1013) anaconda  (1000)     4269 2023-04-10 02:05:09.000000 hcgf-0.1.0/hcgf/sft/chatglm/configuration_chatglm.py
+-rw-rw-r--   0 wyd       (1013) anaconda  (1000)    56527 2023-04-10 02:06:50.000000 hcgf-0.1.0/hcgf/sft/chatglm/modeling_chatglm.py
+-rw-rw-r--   0 wyd       (1013) anaconda  (1000)    15053 2023-04-10 02:09:24.000000 hcgf-0.1.0/hcgf/sft/chatglm/quantization.py
+-rw-rw-r--   0 wyd       (1013) anaconda  (1000)    16684 2023-04-10 02:10:14.000000 hcgf-0.1.0/hcgf/sft/chatglm/tokenization_chatglm.py
+-rw-rw-r--   0 wyd       (1013) anaconda  (1000)     9221 2023-04-11 15:27:44.000000 hcgf-0.1.0/hcgf/sft/lora_ft.py
+drwxrwsr-x   0 wyd       (1013) anaconda  (1000)        0 2023-04-11 16:14:49.585121 hcgf-0.1.0/hcgf/trainer/
+-rw-rw-r--   0 wyd       (1013) anaconda  (1000)       28 2023-03-25 10:33:36.000000 hcgf-0.1.0/hcgf/trainer/__init__.py
+-rw-rw-r--   0 wyd       (1013) anaconda  (1000)     6066 2023-04-10 15:52:51.000000 hcgf-0.1.0/hcgf/trainer/trainer.py
+drwxrwsr-x   0 wyd       (1013) anaconda  (1000)        0 2023-04-11 16:14:49.586121 hcgf-0.1.0/hcgf/utils/
+-rw-rw-r--   0 wyd       (1013) anaconda  (1000)      128 2023-04-03 09:51:01.000000 hcgf-0.1.0/hcgf/utils/__init__.py
+-rw-rw-r--   0 wyd       (1013) anaconda  (1000)     2048 2023-04-04 15:51:29.000000 hcgf-0.1.0/hcgf/utils/utils.py
+drwxrwsr-x   0 wyd       (1013) anaconda  (1000)        0 2023-04-11 16:14:49.584121 hcgf-0.1.0/hcgf.egg-info/
+-rw-rw-r--   0 wyd       (1013) anaconda  (1000)     5261 2023-04-11 16:14:49.000000 hcgf-0.1.0/hcgf.egg-info/PKG-INFO
+-rw-rw-r--   0 wyd       (1013) anaconda  (1000)      751 2023-04-11 16:14:49.000000 hcgf-0.1.0/hcgf.egg-info/SOURCES.txt
+-rw-rw-r--   0 wyd       (1013) anaconda  (1000)        1 2023-04-11 16:14:49.000000 hcgf-0.1.0/hcgf.egg-info/dependency_links.txt
+-rw-rw-r--   0 wyd       (1013) anaconda  (1000)        5 2023-04-11 16:14:49.000000 hcgf-0.1.0/hcgf.egg-info/top_level.txt
+-rw-rw-r--   0 wyd       (1013) anaconda  (1000)       38 2023-04-11 16:14:49.586121 hcgf-0.1.0/setup.cfg
+-rw-rw-r--   0 wyd       (1013) anaconda  (1000)      883 2023-04-11 15:51:53.000000 hcgf-0.1.0/setup.py
+drwxrwsr-x   0 wyd       (1013) anaconda  (1000)        0 2023-04-11 16:14:49.586121 hcgf-0.1.0/tests/
+-rw-rw-r--   0 wyd       (1013) anaconda  (1000)     4640 2023-04-11 15:33:54.000000 hcgf-0.1.0/tests/test_dataloader.py
+-rw-rw-r--   0 wyd       (1013) anaconda  (1000)     1451 2023-04-11 15:52:57.000000 hcgf-0.1.0/tests/test_lora_ft.py
+-rw-rw-r--   0 wyd       (1013) anaconda  (1000)     1419 2023-04-04 17:34:59.000000 hcgf-0.1.0/tests/test_trainer.py
+-rw-rw-r--   0 wyd       (1013) anaconda  (1000)      453 2023-04-03 09:56:55.000000 hcgf-0.1.0/tests/test_utils.py
```

### Comparing `hcgf-0.0.7/LICENSE` & `hcgf-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hcgf-0.0.7/PKG-INFO` & `hcgf-0.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcgf
-Version: 0.0.7
+Version: 0.1.0
 Summary: Humanable ChatGPT/GLM Fine-tuning.
 Home-page: https://github.com/hscspring/hcgf
 Author: Yam
 Author-email: haoshaochun@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -29,18 +29,18 @@
 
 
 
 ## 微调
 
 ### 准备数据
 
-每一行一个json，必须包含`prompt`和`completion`两个字段。示例如下：
+每一行一个dict的`.json`文件，必须包含`prompt`和`completion`两个字段。示例如下：
 
 ```bash
-{"prompt": "你是谁？\n", "completion": "不告诉你。"}
+{"prompt": "你是谁？", "completion": "不告诉你。"}
 ```
 
 
 ### 正常微调
 
 至少需要一张16G显存的卡。如果不指定显卡，默认为`cuda`。
 
@@ -57,39 +57,39 @@
 
 #===== 切换模式 =====#
 gl = hcgf.GlmLora("THUDM/chatglm-6b", device="cuda:0")
 gl.load_data("/path/to/data.json").tune()
 # 切换到推理模式
 gl.eval()
 gl.chat("你是谁？")
-# 切换回微调模式，还是用原来的数据重新跑
+# 切换回微调模式，还是用原来的数据继续跑
 gl.tune()
 # 如果有新的数据集，参考上面的写法，先加载数据
 gl.load_data("/path/to/new_data.json").tune()
+# 如果在原来的基础上用新数据继续微调，先加载之前的pt文件，再加载数据微调
+gl.load_pretrained("/path/to/lora_pt").load_data("/path/to/new_data.json").tune()
 ```
 
 
 ### 8bit微调
 
-至少需要一张12G显存的卡。不指定device。
+至少需要一张12G显存的卡。不指定device。只需要初始化时改一下即可，其他操作和上面正常微调一样。
 
 需要安装依赖: `bitsandbytes`
 
-只需要初始化时改一下即可，其他操作和上面正常微调一样。
-
 ```python
 gl = hcgf.GlmLora("THUDM/chatglm-6b", load_in_8bit=True)
 ```
 
 ### 继续微调
 
 先加载之前的`pt`文件，然后加载数据微调。
 
 ```python
-gl.load_pretrained("/path/to/lora_pt").load_data("/path/to/new_data").tune()
+gl.load_pretrained("/path/to/lora_pt").load_data("/path/to/new_data.json").tune()
 ```
 
 ### 参数说明
 
 主要有三个方法的参数，有值的表示默认值。
 
 ```python
@@ -106,15 +106,17 @@
     out_dir: str = "./output/",
     print_every: int = 10,                  # 每隔多少个Step打印一次输出（Step、Loss、LearningRate）
 )
 chat(
     inp: str, 
     history: List[Tuple[str, str]] = None,  # (问，答)Pair对
     max_len: int = 512,                     # 上下文的最大长度，超过就不生成了
-    stop: List[str] = []                    # 停止文本，可以是标点、特定词或句子等
+    temperature: float = 0.95,              # 越小越确定，越大越随机，比如你微调后可以把它改成0.2
+    top_p: float = 0.7,                     # 同上，两者不要同时调
+    stop: List[str] = []                    # 停止文本，可以是标点、特定词或句子等，输出不包含停止文本
 )
 
 ```
 
 ### 配置
 
 有几个影响显存的参数可以配置：`max_seq_len`，`batch_size`。
@@ -171,7 +173,29 @@
 # 全部测试
 python -m pytest
 # 测试训练和推理，比较慢
 python -m pytest -s -m slow
 # 测试其他的
 python -m pytest -m "not slow"
 ```
+
+
+## 版本说明
+
+如果你用的是旧版本的ChatGLM（icetk tokenizer），可以安装`hcgf==0.0.7`版本，同时，需要手动指定`model_id`参数为模型文件实际路径。
+
+即将`"THUDM/chatglm-6b"`替换为`transformers` `cache`的对应snapshots下的id。或者，建议手动clone仓库：
+
+```bash
+git lfs install
+git clone https://huggingface.co/THUDM/chatglm-6b
+```
+
+然后切换到早期使用icetk的commit。这时候要替换的就是这个仓库的路径了。
+
+
+## 更新日志
+
+- **v0.1.0** `20230412`
+  - 支持ChatGLM新版Tokenizer
+  - 使用官方调整后的MASK方式
+- **v0.0.7** `20230405`
```

### Comparing `hcgf-0.0.7/README.md` & `hcgf-0.1.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 
 
 
 ## 微调
 
 ### 准备数据
 
-每一行一个json，必须包含`prompt`和`completion`两个字段。示例如下：
+每一行一个dict的`.json`文件，必须包含`prompt`和`completion`两个字段。示例如下：
 
 ```bash
-{"prompt": "你是谁？\n", "completion": "不告诉你。"}
+{"prompt": "你是谁？", "completion": "不告诉你。"}
 ```
 
 
 ### 正常微调
 
 至少需要一张16G显存的卡。如果不指定显卡，默认为`cuda`。
 
@@ -44,39 +44,39 @@
 
 #===== 切换模式 =====#
 gl = hcgf.GlmLora("THUDM/chatglm-6b", device="cuda:0")
 gl.load_data("/path/to/data.json").tune()
 # 切换到推理模式
 gl.eval()
 gl.chat("你是谁？")
-# 切换回微调模式，还是用原来的数据重新跑
+# 切换回微调模式，还是用原来的数据继续跑
 gl.tune()
 # 如果有新的数据集，参考上面的写法，先加载数据
 gl.load_data("/path/to/new_data.json").tune()
+# 如果在原来的基础上用新数据继续微调，先加载之前的pt文件，再加载数据微调
+gl.load_pretrained("/path/to/lora_pt").load_data("/path/to/new_data.json").tune()
 ```
 
 
 ### 8bit微调
 
-至少需要一张12G显存的卡。不指定device。
+至少需要一张12G显存的卡。不指定device。只需要初始化时改一下即可，其他操作和上面正常微调一样。
 
 需要安装依赖: `bitsandbytes`
 
-只需要初始化时改一下即可，其他操作和上面正常微调一样。
-
 ```python
 gl = hcgf.GlmLora("THUDM/chatglm-6b", load_in_8bit=True)
 ```
 
 ### 继续微调
 
 先加载之前的`pt`文件，然后加载数据微调。
 
 ```python
-gl.load_pretrained("/path/to/lora_pt").load_data("/path/to/new_data").tune()
+gl.load_pretrained("/path/to/lora_pt").load_data("/path/to/new_data.json").tune()
 ```
 
 ### 参数说明
 
 主要有三个方法的参数，有值的表示默认值。
 
 ```python
@@ -93,15 +93,17 @@
     out_dir: str = "./output/",
     print_every: int = 10,                  # 每隔多少个Step打印一次输出（Step、Loss、LearningRate）
 )
 chat(
     inp: str, 
     history: List[Tuple[str, str]] = None,  # (问，答)Pair对
     max_len: int = 512,                     # 上下文的最大长度，超过就不生成了
-    stop: List[str] = []                    # 停止文本，可以是标点、特定词或句子等
+    temperature: float = 0.95,              # 越小越确定，越大越随机，比如你微调后可以把它改成0.2
+    top_p: float = 0.7,                     # 同上，两者不要同时调
+    stop: List[str] = []                    # 停止文本，可以是标点、特定词或句子等，输出不包含停止文本
 )
 
 ```
 
 ### 配置
 
 有几个影响显存的参数可以配置：`max_seq_len`，`batch_size`。
@@ -157,8 +159,30 @@
 ```bash
 # 全部测试
 python -m pytest
 # 测试训练和推理，比较慢
 python -m pytest -s -m slow
 # 测试其他的
 python -m pytest -m "not slow"
-```
+```
+
+
+## 版本说明
+
+如果你用的是旧版本的ChatGLM（icetk tokenizer），可以安装`hcgf==0.0.7`版本，同时，需要手动指定`model_id`参数为模型文件实际路径。
+
+即将`"THUDM/chatglm-6b"`替换为`transformers` `cache`的对应snapshots下的id。或者，建议手动clone仓库：
+
+```bash
+git lfs install
+git clone https://huggingface.co/THUDM/chatglm-6b
+```
+
+然后切换到早期使用icetk的commit。这时候要替换的就是这个仓库的路径了。
+
+
+## 更新日志
+
+- **v0.1.0** `20230412`
+  - 支持ChatGLM新版Tokenizer
+  - 使用官方调整后的MASK方式
+- **v0.0.7** `20230405`
```

### Comparing `hcgf-0.0.7/hcgf/data_model/__init__.py` & `hcgf-0.1.0/hcgf/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `hcgf-0.0.7/hcgf/dataloader/data_collector.py` & `hcgf-0.1.0/hcgf/dataloader/data_collector.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,24 +6,33 @@
 
 
 class GlmDataCollector:
 
     """
     GLM special tokens:
 
+    # old version
+    150004 <sop>  # bos
+    150005 <eop>  # eop
+    20002  </s>    # eos
+    20000  <unk>
+    20003  <pad>
     150000 [MASK]
     150001 [gMASK]
     150002 [sMASK]
 
-    20000 <unk>
-    20003 <pad>
-
-    150004 <sop>  # bos
-    20002 </s>    # eos
-    150005 <eop>  # eop
+    # new version
+    130000 [MASK]  # mask
+    130001 [gMASK] # gmask
+    130004 <sop>   # bos
+    130005 <eop>   # eop
+    2      </s>    # eos
+    3      <pad>   # pad
+    0      <unk>   # unk
+    130002 [sMASK] # smask
     """
 
     @classmethod
     def get_masks(cls, longest_seq_len: int, cxt_len: int, dtype=torch.int32):
         """
         Referenced from ChatGLMModel.get_masks
         """
@@ -45,16 +54,17 @@
         dtype=torch.int64,
     ):
         """
         Referenced from ChatGLMMModel.get_position_ids
         """
         position_ids = torch.arange(longest_seq_len, dtype=dtype)
         if position_encoding_2d:
-            if not use_gmask:
-                position_ids[cxt_len:] = mask_position
+            # NOTE: if position_encoding_2d, use_gmask is not used
+            # https://github.com/THUDM/ChatGLM-6B/issues/498#event-8971243132
+            position_ids[cxt_len:] = mask_position
             block_position_ids = torch.cat((
                 torch.zeros(cxt_len, dtype=dtype),
                 torch.arange(longest_seq_len - cxt_len, dtype=dtype) + 1
             ))
             position_ids = torch.stack(
                 (position_ids, block_position_ids), dim=0)
         else:
@@ -76,34 +86,31 @@
         label_list = []
         # 长的在前
         for seq_len, item in sorted(
                 zip(len_ids, data_items), key=lambda x: -x[0]):
             ids = item.input_ids
             cxt_len = item.cxt_len
 
-            MASK, gMASK = 150000, 150001
+            MASK, gMASK = 130000, 130001
             mask_token = MASK if MASK in ids else gMASK
             mask_position = ids.index(mask_token)
             use_gmask = False if MASK in ids else True
 
             _masks = cls.get_masks(longest_seq_len, cxt_len)
-            # 150004 == bos_token_id
             # equal to cxt_len - 1
-            cxt_idx = ids.index(150004)
+            cxt_idx = ids.index(130004)
             _pids = cls.get_position_ids(
                 longest_seq_len, cxt_idx, mask_position, use_gmask,
                 position_encoding_2d=True, dtype=input_dtype
             )
 
             padding_len = longest_seq_len - seq_len
-            _labels = [-100] * (cxt_len - 1) + ids[(cxt_len - 1):] + [-100] * padding_len
-            # 20002 == eos_token_id
-            # 20003 == pad_token_id
-            # 150005 == eop_token_id
-            _ids = ids + [20002] * padding_len
+            _labels = [-100] * (cxt_len - 1) + \
+                ids[(cxt_len - 1):] + [-100] * padding_len
+            _ids = ids + [2] * padding_len
 
             if input_dtype == torch.int32:
                 TensorIns = torch.IntTensor
             else:
                 TensorIns = torch.LongTensor
 
             id_list.append(TensorIns(_ids))
```

### Comparing `hcgf-0.0.7/hcgf/dataloader/data_loader.py` & `hcgf-0.1.0/hcgf/dataloader/data_loader.py`

 * *Files identical despite different names*

### Comparing `hcgf-0.0.7/hcgf/dataloader/dataset.py` & `hcgf-0.1.0/hcgf/dataloader/dataset.py`

 * *Files identical despite different names*

### Comparing `hcgf-0.0.7/hcgf/rm/reward_model.py` & `hcgf-0.1.0/hcgf/rm/reward_model.py`

 * *Files identical despite different names*

### Comparing `hcgf-0.0.7/hcgf/sft/chatglm/configuration_chatglm.py` & `hcgf-0.1.0/hcgf/sft/chatglm/configuration_chatglm.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,14 +55,16 @@
             hidden_size=4096,
             num_layers=28,
             num_attention_heads=32,
             layernorm_epsilon=1e-5,
             use_cache=False,
             bos_token_id=150004,
             eos_token_id=150005,
+            mask_token_id=150000,
+            gmask_token_id=150001,
             pad_token_id=0,
             max_sequence_length=2048,
             inner_hidden_size=16384,
             position_encoding_2d=True,
             quantization_bit=0,
             pre_seq_len=None,
             prefix_projection=False,
@@ -75,18 +77,20 @@
         self.max_sequence_length = max_sequence_length
         self.layernorm_epsilon = layernorm_epsilon
         self.inner_hidden_size = inner_hidden_size
         self.use_cache = use_cache
         self.bos_token_id = bos_token_id
         self.eos_token_id = eos_token_id
         self.pad_token_id = pad_token_id
+        self.mask_token_id = mask_token_id
+        self.gmask_token_id = gmask_token_id
         self.position_encoding_2d = position_encoding_2d
         self.quantization_bit = quantization_bit
         self.pre_seq_len = pre_seq_len
         self.prefix_projection = prefix_projection
 
         super().__init__(
             pad_token_id=pad_token_id,
             bos_token_id=bos_token_id,
             eos_token_id=eos_token_id,
             **kwargs
-        )
+        )
```

### Comparing `hcgf-0.0.7/hcgf/sft/chatglm/modeling_chatglm.py` & `hcgf-0.1.0/hcgf/sft/chatglm/modeling_chatglm.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 ]
 
 
 class InvalidScoreLogitsProcessor(LogitsProcessor):
     def __call__(self, input_ids: torch.LongTensor, scores: torch.FloatTensor) -> torch.FloatTensor:
         if torch.isnan(scores).any() or torch.isinf(scores).any():
             scores.zero_()
-            scores[..., 20005] = 5e4
+            scores[..., 5] = 5e4
         return scores
 
 
 def load_tf_weights_in_chatglm_6b(model, config, tf_checkpoint_path):
     """Load tf checkpoints in a pytorch model."""
     try:
         import re
@@ -276,18 +276,16 @@
     output_size = (query_layer.size(1), query_layer.size(2), query_layer.size(0), key_layer.size(0))
 
     # [sq, b, np, hn] -> [sq, b * np, hn]
     query_layer = query_layer.view(output_size[2], output_size[0] * output_size[1], -1)
     # [sk, b, np, hn] -> [sk, b * np, hn]
     key_layer = key_layer.view(output_size[3], output_size[0] * output_size[1], -1)
 
-    matmul_result = torch.empty(
-        output_size[0] * output_size[1],
-        output_size[2],
-        output_size[3],
+    matmul_result = torch.zeros(
+        1, 1, 1,
         dtype=query_layer.dtype,
         device=query_layer.device,
     )
 
     matmul_result = torch.baddbmm(
         matmul_result,
         query_layer.transpose(0, 1),  # [b * np, sq, hn]
@@ -676,25 +674,25 @@
 
         return attention_mask
 
     def get_position_ids(self, input_ids, mask_positions, device, gmask=False):
         batch_size, seq_length = input_ids.shape
         context_lengths = [seq.tolist().index(self.config.bos_token_id) for seq in input_ids]
         if self.position_encoding_2d:
-            position_ids = torch.arange(seq_length, dtype=torch.long, device=device).expand(batch_size, seq_length)
+            position_ids = torch.arange(seq_length, dtype=torch.long, device=device).unsqueeze(0).repeat(batch_size, 1)
             for i, context_length in enumerate(context_lengths):
                 position_ids[i, context_length:] = mask_positions[i]
             block_position_ids = [torch.cat((
                 torch.zeros(context_length, dtype=torch.long, device=device),
                 torch.arange(seq_length - context_length, dtype=torch.long, device=device) + 1
             )) for context_length in context_lengths]
             block_position_ids = torch.stack(block_position_ids, dim=0)
             position_ids = torch.stack((position_ids, block_position_ids), dim=1)
         else:
-            position_ids = torch.arange(seq_length, dtype=torch.long, device=device).expand(batch_size, seq_length)
+            position_ids = torch.arange(seq_length, dtype=torch.long, device=device).unsqueeze(0).repeat(batch_size, 1)
             if not gmask:
                 for i, context_length in enumerate(context_lengths):
                     position_ids[context_length:] = mask_positions[i]
 
         return position_ids
 
     def _set_gradient_checkpointing(self, module, value=False):
@@ -905,17 +903,17 @@
                 attention_mask = self.get_masks(
                     input_ids,
                     device=input_ids.device
                 )
 
 
             if position_ids is None:
-                MASK, gMASK = 150000, 150001
-                mask_token = MASK if MASK in input_ids else gMASK
-                use_gmask = False if MASK in input_ids else gMASK
+                MASK, gMASK = self.config.mask_token_id, self.config.gmask_token_id
+                mask_token = gMASK if gMASK in input_ids else MASK
+                use_gmask = True if gMASK in input_ids else False
 
                 mask_positions = [seq.tolist().index(mask_token) for seq in input_ids]
                 position_ids = self.get_position_ids(
                     input_ids,
                     mask_positions=mask_positions,
                     device=input_ids.device,
                     gmask=use_gmask
@@ -1068,17 +1066,17 @@
             past: Optional[torch.Tensor] = None,
             past_key_values: Optional[torch.Tensor] = None,
             attention_mask: Optional[torch.Tensor] = None,
             position_ids: Optional[torch.Tensor] = None,
             **kwargs
     ) -> dict:
         batch_size, seq_length = input_ids.shape
-        MASK, gMASK = 150000, 150001
-        mask_token = MASK if MASK in input_ids else gMASK
-        use_gmask = False if MASK in input_ids else gMASK
+        MASK, gMASK = self.config.mask_token_id, self.config.gmask_token_id
+        mask_token = gMASK if gMASK in input_ids else MASK
+        use_gmask = True if gMASK in input_ids else False
         seqs = input_ids.tolist()
         mask_positions = [seq.index(mask_token) for seq in seqs]
 
         # only last token for input_ids if past is not None
         if past is not None or past_key_values is not None:
             last_token = input_ids[:, -1].unsqueeze(-1)
             if attention_mask is not None and attention_mask.dtype == torch.bool:
```

### Comparing `hcgf-0.0.7/hcgf/sft/chatglm/quantization.py` & `hcgf-0.1.0/hcgf/sft/chatglm/quantization.py`

 * *Files identical despite different names*

### Comparing `hcgf-0.0.7/hcgf/sft/chatglm/tokenization_chatglm.py` & `hcgf-0.1.0/hcgf/sft/chatglm/tokenization_chatglm.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,96 +1,82 @@
 """Tokenization classes for ChatGLM."""
 from typing import List, Optional, Union
 import os
 
 from transformers.tokenization_utils import PreTrainedTokenizer
-from icetk.text_tokenizer import TextTokenizer
-import icetk.sentencepiece_model_pb2 as sp_model
 from transformers.utils import logging, PaddingStrategy
 from transformers.tokenization_utils_base import EncodedInput, BatchEncoding
 from typing import Dict
+import sentencepiece as spm
 import numpy as np
 
 logger = logging.get_logger(__name__)
 
 PRETRAINED_POSITIONAL_EMBEDDINGS_SIZES = {
     "THUDM/chatglm-6b": 2048,
 }
 
 
+class TextTokenizer:
+    def __init__(self, model_path):
+        self.sp = spm.SentencePieceProcessor()
+        self.sp.Load(model_path)
+        self.num_tokens = self.sp.vocab_size()
+
+    def encode(self, text):
+        return self.sp.EncodeAsIds(text)
+
+    def decode(self, ids: List[int]):
+        return self.sp.DecodeIds(ids)
+
+    def tokenize(self, text):
+        return self.sp.EncodeAsPieces(text)
+
+    def convert_tokens_to_ids(self, tokens):
+        return [self.sp.PieceToId(token) for token in tokens]
+
+    def convert_token_to_id(self, token):
+        return self.sp.PieceToId(token)
+
+    def convert_id_to_token(self, idx):
+        return self.sp.IdToPiece(idx)
+
+    def __len__(self):
+        return self.num_tokens
+
+
 class SPTokenizer:
     def __init__(
-        self,
-        vocab_file,
-        max_blank_length=80,
-        byte_fallback=True,
+            self,
+            vocab_file,
+            num_image_tokens=20000,
+            max_blank_length=80,
+            byte_fallback=True,
     ):
         assert vocab_file is not None
         self.vocab_file = vocab_file
+        self.num_image_tokens = num_image_tokens
         self.special_tokens = ["[MASK]", "[gMASK]", "[sMASK]", "<unused_0>", "<sop>", "<eop>", "<ENC>", "<dBLOCK>"]
         self.max_blank_length = max_blank_length
         self.byte_fallback = byte_fallback
-        self.text_tokenizer = self._build_text_tokenizer(encode_special_tokens=False)
-        self.special_text_tokenizer = self._build_text_tokenizer(encode_special_tokens=True)
-
-    @staticmethod
-    def _configure_tokenizer(
-        text_tokenizer: TextTokenizer,
-        special_tokens: List[str],
-        max_blank_length: int,
-        byte_fallback: bool,
-        encode_special_tokens=False,
-    ):
-        # special token
-        special_token_type = 4 if encode_special_tokens else 3  # 3 - CONTROL, 4 - USER_DEFINE
-        for token in special_tokens:
-            text_tokenizer.proto.pieces.append(
-                sp_model.ModelProto.SentencePiece(piece=token, score=0.0, type=special_token_type)
-            )
-        # whitespaces
-        for token in [SPTokenizer.get_tab_token()] + [
-            SPTokenizer.get_blank_token(i) for i in range(2, max_blank_length + 1)
-        ]:
-            text_tokenizer.proto.pieces.append(sp_model.ModelProto.SentencePiece(piece=token, score=0.0, type=4))
-        # byte fallback
-        if byte_fallback:
-            text_tokenizer.proto.trainer_spec.byte_fallback = True
-            for i in range(256):
-                text_tokenizer.proto.pieces.append(
-                    sp_model.ModelProto.SentencePiece(piece="<0x{:02X}>".format(i), score=0.0, type=6)
-                )
-        text_tokenizer.refresh()
-
-    def _build_text_tokenizer(self, encode_special_tokens=False):
-        tokenizer = TextTokenizer(self.vocab_file)
-        self._configure_tokenizer(
-            tokenizer, self.special_tokens, self.max_blank_length, self.byte_fallback, encode_special_tokens
-        )
-        return tokenizer
+        self.text_tokenizer = TextTokenizer(vocab_file)
 
-    def _get_text_tokenizer(self, encode_special_tokens=False):
-        if encode_special_tokens:
-            return self.special_text_tokenizer
-        else:
-            return self.text_tokenizer
+    def _get_text_tokenizer(self):
+        return self.text_tokenizer
 
     @staticmethod
     def get_blank_token(length: int):
         assert length >= 2
         return f"<|blank_{length}|>"
 
     @staticmethod
     def get_tab_token():
         return f"<|tab|>"
 
     @property
-    def num_image_tokens(self):
-        return 20000
-
-    @property
     def num_text_tokens(self):
         return self.text_tokenizer.num_tokens
 
     @property
     def num_tokens(self):
         return self.num_image_tokens + self.num_text_tokens
 
@@ -105,54 +91,54 @@
         if linebreak:
             text = text.replace("\n", "<n>")
         if whitespaces:
             text = self._encode_whitespaces(text, max_len=self.max_blank_length)
         return text
 
     def encode(
-        self, text: str, linebreak=True, whitespaces=True, special_tokens=False, add_dummy_prefix=True
+            self, text: str, linebreak=True, whitespaces=True, add_dummy_prefix=True
     ) -> List[int]:
         """
         @param text: Text to encode.
         @param linebreak: Whether to encode newline (\n) in text.
         @param whitespaces: Whether to encode multiple whitespaces or tab in text, useful for source code encoding.
         @param special_tokens: Whether to encode special token ([MASK], [gMASK], etc.) in text.
         @param add_dummy_prefix: Whether to add dummy blank space in the beginning.
         """
         text = self._preprocess(text, linebreak, whitespaces)
         if not add_dummy_prefix:
             text = "<n>" + text
-        tmp = self._get_text_tokenizer(encode_special_tokens=special_tokens).encode(text)
+        tmp = self._get_text_tokenizer().encode(text)
         tokens = [x + self.num_image_tokens for x in tmp]
         return tokens if add_dummy_prefix else tokens[2:]
 
-    def decode(self, text_ids: List[int], special_tokens=False) -> str:
+    def decode(self, text_ids: List[int]) -> str:
         ids = [int(_id) - self.num_image_tokens for _id in text_ids]
         ids = [_id for _id in ids if _id >= 0]
-        text = self._get_text_tokenizer(encode_special_tokens=special_tokens).decode(ids)
+        text = self._get_text_tokenizer().decode(ids)
         text = text.replace("<n>", "\n")
         text = text.replace(SPTokenizer.get_tab_token(), "\t")
         for i in range(2, self.max_blank_length + 1):
             text = text.replace(self.get_blank_token(i), " " * i)
         return text
 
     def tokenize(
-        self, text: str, linebreak=True, whitespaces=True, special_tokens=False, add_dummy_prefix=True
+            self, text: str, linebreak=True, whitespaces=True, add_dummy_prefix=True
     ) -> List[str]:
         """
         @param text: Text to encode.
         @param linebreak: Whether to encode newline (\n) in text.
         @param whitespaces: Whether to encode multiple whitespaces or tab in text, useful for source code encoding.
         @param special_tokens: Whether to encode special token ([MASK], [gMASK], etc.) in text.
         @param add_dummy_prefix: Whether to add dummy blank space in the beginning.
         """
         text = self._preprocess(text, linebreak, whitespaces)
         if not add_dummy_prefix:
             text = "<n>" + text
-        tokens = self._get_text_tokenizer(encode_special_tokens=special_tokens).tokenize(text)
+        tokens = self._get_text_tokenizer().tokenize(text)
         return tokens if add_dummy_prefix else tokens[2:]
 
     def __getitem__(self, x: Union[int, str]):
         if isinstance(x, int):
             if x < self.num_image_tokens:
                 return "<image_{}>".format(x)
             else:
@@ -179,44 +165,57 @@
     model_input_names = ["input_ids", "attention_mask", "position_ids"]
 
     def __init__(
             self,
             vocab_file,
             do_lower_case=False,
             remove_space=False,
-            bos_token='sop',
-            eos_token='eos',
-            eop_token='eop',
+            bos_token='<sop>',
+            eos_token='</s>',
+            eop_token='<eop>',
             mask_token='[MASK]',
             gmask_token='[gMASK]',
             padding_side="left",
+            num_image_tokens=20000,
             **kwargs
     ) -> None:
         super().__init__(
             do_lower_case=do_lower_case,
             remove_space=remove_space,
             padding_side=padding_side,
+            bos_token=bos_token,
+            eos_token=eos_token,
+            eop_token=eop_token,
+            mask_token=mask_token,
+            gmask_token=gmask_token,
+            num_image_tokens=num_image_tokens,
             **kwargs
         )
 
         self.do_lower_case = do_lower_case
         self.remove_space = remove_space
         self.vocab_file = vocab_file
 
         self.bos_token = bos_token
         self.eos_token = eos_token
         self.eop_token = eop_token
         self.mask_token = mask_token
         self.gmask_token = gmask_token
 
-        self.sp_tokenizer = SPTokenizer(vocab_file)
+        self.sp_tokenizer = SPTokenizer(vocab_file, num_image_tokens=num_image_tokens)
 
         """ Initialisation """
 
     @property
+    def gmask_token_id(self) -> Optional[int]:
+        if self.gmask_token is None:
+            return None
+        return self.convert_tokens_to_ids(self.gmask_token)
+
+    @property
     def eop_token_id(self) -> Optional[int]:
         """
         `Optional[int]`: Id of the end of sentence token in the vocabulary. Returns `None` if the token has not been
         set.
         """
         if self.eop_token is None:
             return None
@@ -248,33 +247,28 @@
         """ Returns a tokenized string. """
         text = self.preprocess_text(text)
 
         seq = self.sp_tokenizer.tokenize(text)
 
         return seq
 
-    def decode(
+    def _decode(
             self,
-            token_ids: Union[List[int], List[List[int]]],
+            token_ids: Union[int, List[int]],
             skip_special_tokens: bool = False,
             clean_up_tokenization_spaces: bool = True,
-            spaces_between_special_tokens: bool = True,
             **kwargs
     ) -> str:
-        if isinstance(token_ids[0], list):
-            tokens = []
-            for single_token_ids in token_ids:
-                if self.pad_token_id in single_token_ids:  # remove pad
-                    single_token_ids = list(filter((self.pad_token_id).__ne__, single_token_ids))
-                tokens.append(self.sp_tokenizer.decode(single_token_ids))
-            return (tokens)
-        else:
-            if self.pad_token_id in token_ids:  # remove pad
-                token_ids = list(filter((self.pad_token_id).__ne__, token_ids))
-            return self.sp_tokenizer.decode(token_ids)
+        if isinstance(token_ids, int):
+            token_ids = [token_ids]
+        if len(token_ids) == 0:
+            return ""
+        if self.pad_token_id in token_ids:  # remove pad
+            token_ids = list(filter((self.pad_token_id).__ne__, token_ids))
+        return self.sp_tokenizer.decode(token_ids)
 
     def _convert_token_to_id(self, token):
         """ Converts a token (str) in an id using the vocab. """
         return self.sp_tokenizer[token]
 
     def _convert_id_to_token(self, index):
         """Converts an index (integer) in a token (str) using the vocab."""
@@ -337,20 +331,20 @@
             if not token_ids_1 or token_ids_1[-1] != eop_id:
                 token_ids_1 += [eop_id]
             token_ids_0 += token_ids_1
 
         return token_ids_0
 
     def _pad(
-        self,
-        encoded_inputs: Union[Dict[str, EncodedInput], BatchEncoding],
-        max_length: Optional[int] = None,
-        padding_strategy: PaddingStrategy = PaddingStrategy.DO_NOT_PAD,
-        pad_to_multiple_of: Optional[int] = None,
-        return_attention_mask: Optional[bool] = None,
+            self,
+            encoded_inputs: Union[Dict[str, EncodedInput], BatchEncoding],
+            max_length: Optional[int] = None,
+            padding_strategy: PaddingStrategy = PaddingStrategy.DO_NOT_PAD,
+            pad_to_multiple_of: Optional[int] = None,
+            return_attention_mask: Optional[bool] = None,
     ) -> dict:
         """
         Pad encoded inputs (on left/right and up to predefined length or max length in the batch)
         Args:
             encoded_inputs:
                 Dictionary of tokenized inputs (`List[int]`) or batch of tokenized inputs (`List[List[int]]`).
             max_length: maximum length of the returned list and optionally padding length (see below).
```

### Comparing `hcgf-0.0.7/hcgf/sft/lora_ft.py` & `hcgf-0.1.0/hcgf/sft/lora_ft.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 from typing import Optional, List, Tuple
 import copy
 
 import torch
 import torch.nn as nn
 from transformers.modeling_utils import PreTrainedModel
 from transformers.generation.utils import (
-    LogitsProcessorList, 
-    StoppingCriteriaList, 
+    LogitsProcessorList,
+    StoppingCriteriaList,
     StoppingCriteria
 )
 from peft import get_peft_model, LoraConfig, TaskType
 
 from ..utils import print_trainable_parameters, create_token_tensor_list
 from ..dataloader import GlmDataLoader
 from ..data_model import Tensor
 from ..trainer import Trainer
 
 
 from .chatglm import (
-    ChatGLMForConditionalGeneration, 
-    ChatGLMTokenizer, 
+    ChatGLMForConditionalGeneration,
+    ChatGLMTokenizer,
     InvalidScoreLogitsProcessor
 )
 
 
 class CustomStoppingCriteria(StoppingCriteria):
 
     def __init__(
-        self, 
-        stop_tensor_list: List[Tensor["L", torch.LongTensor]], 
-        device: torch.device, 
+        self,
+        stop_tensor_list: List[Tensor["L", torch.LongTensor]],
+        device: torch.device,
         encounters: int = 1
     ):
         super().__init__()
         self.stops = [stop.to(device) for stop in stop_tensor_list]
         self.encounters = encounters
 
     def __call__(
-        self, 
-        input_ids: Tensor["B,L", torch.LongTensor], 
+        self,
+        input_ids: Tensor["B,L", torch.LongTensor],
         scores: torch.FloatTensor
     ):
         count = 0
         for stop in self.stops:
             if torch.all((stop == input_ids[0][-len(stop):])).item():
                 count += 1
             if count >= self.encounters:
@@ -69,15 +69,15 @@
         print(f"Loading tokenizer and model of {model_id}")
         self.load_in_8bit = load_in_8bit
         if self.load_in_8bit:
             import bitsandbytes as bnb
             self.device = None
             model = self._load_8bit_glm(model_id)
         else:
-            self.device = device or "cuda"
+            self.device = device or "cuda:0"
             model = self._load_glm(model_id)
         self.tokenizer = ChatGLMTokenizer.from_pretrained(model_id)
         self.config = LoraConfig(
             # peft config
             peft_type="LORA",
             task_type=TaskType.CAUSAL_LM,
             inference_mode=False,
@@ -96,15 +96,15 @@
         self.stop_tokens = ["问题："]
         self.builtin_stop_tensor_list = self.init_stop_tensor_list()
 
     def __cast_small_to(self, dtype: torch.Type):
         for name, param in self.model.named_parameters():
             if param.ndim == 1 and param.dtype != dtype:
                 param.data = param.data.to(dtype)
-    
+
     def __cast_lora_to(self, dtype: torch.Type):
         for name, param in self.model.named_parameters():
             if "lora_" in name:
                 param.data = param.data.to(dtype)
 
     def _load_8bit_glm(self, model_id: str) -> PreTrainedModel:
         model = ChatGLMForConditionalGeneration.from_pretrained(
@@ -180,87 +180,102 @@
         if quant_bit is not None:
             self.model.quantize(quant_bit)
         # 8bit do not use device, device is None
         if self.device is not None:
             self.model.to(self.device).eval()
         else:
             self.model.eval()
-    
+
     @torch.no_grad()
     def stream_chat(
-        self, 
-        query: str, 
-        history: List[Tuple[str, str]] = None, 
+        self,
+        query: str,
+        history: List[Tuple[str, str]] = None,
         max_length: int = 2048,
-        do_sample=True, 
-        top_p=0.7, 
-        temperature=0.95, 
-        logits_processor=None, 
+        do_sample=True,
+        top_p=0.7,
+        temperature=0.95,
+        logits_processor=None,
         stopping_criteria=None,
         **kwargs
     ):
         "From ChatGLM Model"
         if logits_processor is None:
             logits_processor = LogitsProcessorList()
         logits_processor.append(InvalidScoreLogitsProcessor())
         if stopping_criteria is None:
             stopping_criteria = StoppingCriteriaList()
         gen_kwargs = {
-            "max_length": max_length, 
-            "do_sample": do_sample, 
+            "max_length": max_length,
+            "do_sample": do_sample,
             "top_p": top_p,
-            "temperature": temperature, 
+            "temperature": temperature,
             "logits_processor": logits_processor,
             "stopping_criteria": stopping_criteria,
             **kwargs
         }
         if not history:
             prompt = query
         else:
             prompt = ""
             for i, (old_query, response) in enumerate(history):
-                prompt += "[Round {}]\n 问：{}\n 答：{}\n".format(i, old_query, response)
+                prompt += "[Round {}]\n 问：{}\n 答：{}\n".format(
+                    i, old_query, response)
             prompt += "[Round {}]\n 问：{}\n 答：".format(len(history), query)
         inputs = self.tokenizer([prompt], return_tensors="pt")
-        inputs = inputs.to(self.model.device)
+        inputs = inputs.to(self.curr_device)
+
         for outputs in self.model.stream_generate(
             inputs["input_ids"], **gen_kwargs
         ):
             outputs = outputs.tolist()[0][len(inputs["input_ids"][0]):]
             response = self.tokenizer.decode(outputs)
             response = self.model.process_response(response)
             new_history = history + [(query, response)]
             yield response, new_history
 
     def chat(
-        self, 
-        inp: str, 
-        history: List[Tuple[str, str]] = None, 
-        max_len: int = 512, 
+        self,
+        inp: str,
+        history: List[Tuple[str, str]] = None,
+        max_len: int = 512,
+        temperature: float = 0.95,
+        top_p: float = 0.7,
         stop: List[str] = []
     ):
         if not history:
             history = []
-        
+
         if stop:
             stop_tokens = [v for v in stop if v not in self.stop_tokens]
-            custom_stop_tensor_list = create_token_tensor_list(self.tokenizer, stop_tokens)
+            custom_stop_tensor_list = create_token_tensor_list(
+                self.tokenizer, stop_tokens)
             stop_tensor_list = self.builtin_stop_tensor_list + custom_stop_tensor_list
         else:
             stop_tensor_list = self.builtin_stop_tensor_list
 
-        custom_stop_list = [CustomStoppingCriteria(stop_tensor_list, self.model.device)]
-        
+        custom_stop_list = [
+            CustomStoppingCriteria(
+                stop_tensor_list,
+                self.curr_device)]
+
         for response, history in self.stream_chat(
             inp, history, max_len,
+            top_p=top_p, temperature=temperature,
             stopping_criteria=StoppingCriteriaList(custom_stop_list),
         ):
             ...
         return response, history
-    
+
+    @property
+    def curr_device(self) -> torch.device:
+        if self.device is None:
+            return self.model.device
+        return self.device
+
     def init_stop_tensor_list(self) -> List[Tensor["L", torch.LongTensor]]:
         init_tensor_list = [
             torch.LongTensor([20002]),  # eos
-            torch.LongTensor([150005]), # eop
+            torch.LongTensor([150005]),  # eop
         ]
         new_add = create_token_tensor_list(self.tokenizer, self.stop_tokens)
-        return init_tensor_list + new_add
+        return init_tensor_list + new_add
```

### Comparing `hcgf-0.0.7/hcgf/trainer/trainer.py` & `hcgf-0.1.0/hcgf/trainer/trainer.py`

 * *Files identical despite different names*

### Comparing `hcgf-0.0.7/hcgf/utils/utils.py` & `hcgf-0.1.0/hcgf/utils/utils.py`

 * *Files identical despite different names*

### Comparing `hcgf-0.0.7/hcgf.egg-info/PKG-INFO` & `hcgf-0.1.0/hcgf.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcgf
-Version: 0.0.7
+Version: 0.1.0
 Summary: Humanable ChatGPT/GLM Fine-tuning.
 Home-page: https://github.com/hscspring/hcgf
 Author: Yam
 Author-email: haoshaochun@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -29,18 +29,18 @@
 
 
 
 ## 微调
 
 ### 准备数据
 
-每一行一个json，必须包含`prompt`和`completion`两个字段。示例如下：
+每一行一个dict的`.json`文件，必须包含`prompt`和`completion`两个字段。示例如下：
 
 ```bash
-{"prompt": "你是谁？\n", "completion": "不告诉你。"}
+{"prompt": "你是谁？", "completion": "不告诉你。"}
 ```
 
 
 ### 正常微调
 
 至少需要一张16G显存的卡。如果不指定显卡，默认为`cuda`。
 
@@ -57,39 +57,39 @@
 
 #===== 切换模式 =====#
 gl = hcgf.GlmLora("THUDM/chatglm-6b", device="cuda:0")
 gl.load_data("/path/to/data.json").tune()
 # 切换到推理模式
 gl.eval()
 gl.chat("你是谁？")
-# 切换回微调模式，还是用原来的数据重新跑
+# 切换回微调模式，还是用原来的数据继续跑
 gl.tune()
 # 如果有新的数据集，参考上面的写法，先加载数据
 gl.load_data("/path/to/new_data.json").tune()
+# 如果在原来的基础上用新数据继续微调，先加载之前的pt文件，再加载数据微调
+gl.load_pretrained("/path/to/lora_pt").load_data("/path/to/new_data.json").tune()
 ```
 
 
 ### 8bit微调
 
-至少需要一张12G显存的卡。不指定device。
+至少需要一张12G显存的卡。不指定device。只需要初始化时改一下即可，其他操作和上面正常微调一样。
 
 需要安装依赖: `bitsandbytes`
 
-只需要初始化时改一下即可，其他操作和上面正常微调一样。
-
 ```python
 gl = hcgf.GlmLora("THUDM/chatglm-6b", load_in_8bit=True)
 ```
 
 ### 继续微调
 
 先加载之前的`pt`文件，然后加载数据微调。
 
 ```python
-gl.load_pretrained("/path/to/lora_pt").load_data("/path/to/new_data").tune()
+gl.load_pretrained("/path/to/lora_pt").load_data("/path/to/new_data.json").tune()
 ```
 
 ### 参数说明
 
 主要有三个方法的参数，有值的表示默认值。
 
 ```python
@@ -106,15 +106,17 @@
     out_dir: str = "./output/",
     print_every: int = 10,                  # 每隔多少个Step打印一次输出（Step、Loss、LearningRate）
 )
 chat(
     inp: str, 
     history: List[Tuple[str, str]] = None,  # (问，答)Pair对
     max_len: int = 512,                     # 上下文的最大长度，超过就不生成了
-    stop: List[str] = []                    # 停止文本，可以是标点、特定词或句子等
+    temperature: float = 0.95,              # 越小越确定，越大越随机，比如你微调后可以把它改成0.2
+    top_p: float = 0.7,                     # 同上，两者不要同时调
+    stop: List[str] = []                    # 停止文本，可以是标点、特定词或句子等，输出不包含停止文本
 )
 
 ```
 
 ### 配置
 
 有几个影响显存的参数可以配置：`max_seq_len`，`batch_size`。
@@ -171,7 +173,29 @@
 # 全部测试
 python -m pytest
 # 测试训练和推理，比较慢
 python -m pytest -s -m slow
 # 测试其他的
 python -m pytest -m "not slow"
 ```
+
+
+## 版本说明
+
+如果你用的是旧版本的ChatGLM（icetk tokenizer），可以安装`hcgf==0.0.7`版本，同时，需要手动指定`model_id`参数为模型文件实际路径。
+
+即将`"THUDM/chatglm-6b"`替换为`transformers` `cache`的对应snapshots下的id。或者，建议手动clone仓库：
+
+```bash
+git lfs install
+git clone https://huggingface.co/THUDM/chatglm-6b
+```
+
+然后切换到早期使用icetk的commit。这时候要替换的就是这个仓库的路径了。
+
+
+## 更新日志
+
+- **v0.1.0** `20230412`
+  - 支持ChatGLM新版Tokenizer
+  - 使用官方调整后的MASK方式
+- **v0.0.7** `20230405`
```

### Comparing `hcgf-0.0.7/hcgf.egg-info/SOURCES.txt` & `hcgf-0.1.0/hcgf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcgf-0.0.7/setup.py` & `hcgf-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hcgf",
-    version="0.0.7",
+    version="0.1.0",
     author="Yam",
     author_email="haoshaochun@gmail.com",
     description="Humanable ChatGPT/GLM Fine-tuning.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hscspring/hcgf",
     include_package_data=True,
```

### Comparing `hcgf-0.0.7/tests/test_dataloader.py` & `hcgf-0.1.0/tests/test_dataloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,33 +33,33 @@
     assert len(v.input_ids) == expected
 
 
 arr_dtype = np.int64
 
 input_ids = np.array(
     [
-        [20005, 94874, 94874, 94874, 150001, 150004, 20005, 88443, 20002],
-        [20005, 94874, 150001, 150004, 20005, 84480, 20002, 20002, 20002],
+        [5, 94874, 94874, 94874, 130001, 130004, 5, 88443, 2],
+        [5, 94874, 130001, 130004, 5, 84480, 2, 2, 2],
     ],
     dtype=arr_dtype
 )
 
 labels = np.array(
     [
-        [-100, -100, -100, -100, -100, 150004, 20005, 88443, 20002],
-        [-100, -100, -100, 150004, 20005, 84480, 20002, -100, -100],
+        [-100, -100, -100, -100, -100, 130004, 5, 88443, 2],
+        [-100, -100, -100, 130004, 5, 84480, 2, -100, -100],
     ],
     dtype=arr_dtype
 )
 
 position_ids = np.array(
     [
-        [[0, 1, 2, 3, 4, 5, 6, 7, 8],
+        [[0, 1, 2, 3, 4, 4, 4, 4, 4],
          [0, 0, 0, 0, 0, 1, 2, 3, 4]],
-        [[0, 1, 2, 3, 4, 5, 6, 7, 8],
+        [[0, 1, 2, 2, 2, 2, 2, 2, 2],
          [0, 0, 0, 1, 2, 3, 4, 5, 6]],
     ],
     dtype=arr_dtype
 )
 
 attention_mask = np.array(
     [
```

### Comparing `hcgf-0.0.7/tests/test_trainer.py` & `hcgf-0.1.0/tests/test_trainer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from dataclasses import dataclass
+import os
+import shutil
 import pytest
 
 import torch
 import torch.nn as nn
 
 from hcgf.trainer.trainer import Trainer
 
@@ -49,17 +51,20 @@
 
 
 @pytest.mark.parametrize("lr", [1e-1])
 @pytest.mark.parametrize("num_epochs", [1, 2])
 @pytest.mark.parametrize("warmup_steps", [None, 10])
 @pytest.mark.parametrize("accumulate_steps", [1, 8])
 def test_trainer(lr, num_epochs, warmup_steps, accumulate_steps):
+    out_path = "./test_output/"
     trainer = Trainer(
         lr,
         num_epochs,
         warmup_steps,
         accumulate_steps,
-        "test_output/",
+        out_path,
         "cpu",
         10,
     )
     trainer.train(model, train_loader, train_loader)
+    if os.path.exists(out_path):
+        shutil.rmtree(out_path)
```

