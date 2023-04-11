# Comparing `tmp/fschat-0.1.8.tar.gz` & `tmp/fschat-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fschat-0.1.8.tar", last modified: Fri Apr  7 00:05:39 2023, max compression
+gzip compressed data, was "fschat-0.1.9.tar", last modified: Sat Apr  8 15:48:39 2023, max compression
```

## Comparing `fschat-0.1.8.tar` & `fschat-0.1.9.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-07 00:05:39.678459 fschat-0.1.8/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-04-03 18:06:47.000000 fschat-0.1.8/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10443 2023-04-07 00:05:39.678459 fschat-0.1.8/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9969 2023-04-07 00:00:31.000000 fschat-0.1.8/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-07 00:05:39.670459 fschat-0.1.8/fastchat/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 18:06:47.000000 fschat-0.1.8/fastchat/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       88 2023-04-03 18:06:47.000000 fschat-0.1.8/fastchat/constants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6432 2023-04-06 02:45:48.000000 fschat-0.1.8/fastchat/conversation.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-07 00:05:39.674459 fschat-0.1.8/fastchat/data/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 18:06:47.000000 fschat-0.1.8/fastchat/data/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1819 2023-04-03 18:06:47.000000 fschat-0.1.8/fastchat/data/alpaca-converter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4465 2023-04-06 02:45:48.000000 fschat-0.1.8/fastchat/data/clean_sharegpt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      615 2023-04-03 18:06:47.000000 fschat-0.1.8/fastchat/data/inspect.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2684 2023-04-06 02:45:48.000000 fschat-0.1.8/fastchat/data/optional_clean.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2023-04-03 18:06:47.000000 fschat-0.1.8/fastchat/data/pretty_json.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3403 2023-04-03 18:06:47.000000 fschat-0.1.8/fastchat/data/split_long_conversation.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-07 00:05:39.674459 fschat-0.1.8/fastchat/eval/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5042 2023-04-07 00:00:29.000000 fschat-0.1.8/fastchat/eval/eval_gpt_review.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3661 2023-04-03 18:06:47.000000 fschat-0.1.8/fastchat/eval/generate_webpage_data_from_table.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3054 2023-04-07 00:00:29.000000 fschat-0.1.8/fastchat/eval/get_model_answer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2345 2023-04-03 18:06:47.000000 fschat-0.1.8/fastchat/eval/qa_baseline_gpt35.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-07 00:05:39.674459 fschat-0.1.8/fastchat/model/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 18:06:47.000000 fschat-0.1.8/fastchat/model/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2023-04-07 00:00:29.000000 fschat-0.1.8/fastchat/model/apply_delta.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2167 2023-04-07 00:00:29.000000 fschat-0.1.8/fastchat/model/make_delta.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-07 00:05:39.674459 fschat-0.1.8/fastchat/serve/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 18:06:47.000000 fschat-0.1.8/fastchat/serve/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6408 2023-04-07 00:01:16.000000 fschat-0.1.8/fastchat/serve/cli.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3632 2023-04-07 00:00:31.000000 fschat-0.1.8/fastchat/serve/compression.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9942 2023-04-03 18:06:47.000000 fschat-0.1.8/fastchat/serve/controller.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2717 2023-04-03 18:06:47.000000 fschat-0.1.8/fastchat/serve/gradio_css.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7343 2023-04-03 18:06:47.000000 fschat-0.1.8/fastchat/serve/gradio_patch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16246 2023-04-07 00:00:29.000000 fschat-0.1.8/fastchat/serve/gradio_web_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8756 2023-04-07 00:00:29.000000 fschat-0.1.8/fastchat/serve/model_worker.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3997 2023-04-07 00:00:29.000000 fschat-0.1.8/fastchat/serve/monkey_patch_non_inplace.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      734 2023-04-03 18:06:47.000000 fschat-0.1.8/fastchat/serve/register_worker.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2028 2023-04-03 18:06:47.000000 fschat-0.1.8/fastchat/serve/test_message.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-07 00:05:39.674459 fschat-0.1.8/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3982 2023-04-06 14:12:17.000000 fschat-0.1.8/fastchat/train/llama_flash_attn_monkey_patch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12308 2023-04-07 00:00:29.000000 fschat-0.1.8/fastchat/train/train.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3657 2023-04-06 05:27:02.000000 fschat-0.1.8/fastchat/train/train_lora.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      420 2023-04-03 18:06:47.000000 fschat-0.1.8/fastchat/train/train_mem.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3988 2023-04-06 14:12:04.000000 fschat-0.1.8/fastchat/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-07 00:05:39.678459 fschat-0.1.8/fschat.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10443 2023-04-07 00:05:39.000000 fschat-0.1.8/fschat.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1196 2023-04-07 00:05:39.000000 fschat-0.1.8/fschat.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-07 00:05:39.000000 fschat-0.1.8/fschat.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      115 2023-04-07 00:05:39.000000 fschat-0.1.8/fschat.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-04-07 00:05:39.000000 fschat-0.1.8/fschat.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      938 2023-04-07 00:05:29.000000 fschat-0.1.8/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-07 00:05:39.678459 fschat-0.1.8/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-08 15:48:39.062306 fschat-0.1.9/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-04-03 18:06:47.000000 fschat-0.1.9/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11862 2023-04-08 15:48:39.062306 fschat-0.1.9/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11388 2023-04-08 15:47:09.000000 fschat-0.1.9/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-08 15:48:39.058306 fschat-0.1.9/fastchat/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       88 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/constants.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6432 2023-04-08 06:26:44.000000 fschat-0.1.9/fastchat/conversation.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-08 15:48:39.058306 fschat-0.1.9/fastchat/data/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/data/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1819 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/data/alpaca-converter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4465 2023-04-08 06:26:44.000000 fschat-0.1.9/fastchat/data/clean_sharegpt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      615 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/data/inspect.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2684 2023-04-08 06:26:44.000000 fschat-0.1.9/fastchat/data/optional_clean.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/data/pretty_json.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3403 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/data/split_long_conversation.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-08 15:48:39.058306 fschat-0.1.9/fastchat/eval/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5042 2023-04-08 06:26:44.000000 fschat-0.1.9/fastchat/eval/eval_gpt_review.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3661 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/eval/generate_webpage_data_from_table.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3054 2023-04-08 06:26:44.000000 fschat-0.1.9/fastchat/eval/get_model_answer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2345 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/eval/qa_baseline_gpt35.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-08 15:48:39.062306 fschat-0.1.9/fastchat/model/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/model/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2036 2023-04-08 06:26:44.000000 fschat-0.1.9/fastchat/model/apply_delta.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2303 2023-04-08 06:26:44.000000 fschat-0.1.9/fastchat/model/make_delta.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-08 15:48:39.062306 fschat-0.1.9/fastchat/serve/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/serve/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6691 2023-04-08 15:47:09.000000 fschat-0.1.9/fastchat/serve/cli.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3748 2023-04-08 15:47:09.000000 fschat-0.1.9/fastchat/serve/compression.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9942 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/serve/controller.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2717 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/serve/gradio_css.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7343 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/serve/gradio_patch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16383 2023-04-08 06:26:44.000000 fschat-0.1.9/fastchat/serve/gradio_web_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6775 2023-04-08 06:26:44.000000 fschat-0.1.9/fastchat/serve/model_worker.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3997 2023-04-08 06:26:44.000000 fschat-0.1.9/fastchat/serve/monkey_patch_non_inplace.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      734 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/serve/register_worker.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      904 2023-04-08 06:26:44.000000 fschat-0.1.9/fastchat/serve/serve_chatglm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2028 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/serve/test_message.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-08 15:48:39.062306 fschat-0.1.9/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3982 2023-04-08 06:26:44.000000 fschat-0.1.9/fastchat/train/llama_flash_attn_monkey_patch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12308 2023-04-08 06:26:44.000000 fschat-0.1.9/fastchat/train/train.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3657 2023-04-08 06:26:44.000000 fschat-0.1.9/fastchat/train/train_lora.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      420 2023-04-03 18:06:47.000000 fschat-0.1.9/fastchat/train/train_mem.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4186 2023-04-08 15:47:09.000000 fschat-0.1.9/fastchat/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-08 15:48:39.062306 fschat-0.1.9/fschat.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11862 2023-04-08 15:48:39.000000 fschat-0.1.9/fschat.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1228 2023-04-08 15:48:39.000000 fschat-0.1.9/fschat.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-08 15:48:39.000000 fschat-0.1.9/fschat.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      115 2023-04-08 15:48:39.000000 fschat-0.1.9/fschat.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-04-08 15:48:39.000000 fschat-0.1.9/fschat.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      938 2023-04-08 15:48:30.000000 fschat-0.1.9/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-08 15:48:39.062306 fschat-0.1.9/setup.cfg
```

### Comparing `fschat-0.1.8/LICENSE` & `fschat-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fschat-0.1.8/PKG-INFO` & `fschat-0.1.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fschat
-Version: 0.1.8
+Version: 0.1.9
 Summary: An open platform for training, serving, and evaluating large language model based chatbots.
 Project-URL: Homepage, https://github.com/lm-sys/fastchat
 Project-URL: Bug Tracker, https://github.com/lm-sys/fastchat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -49,111 +49,133 @@
 
 1. Clone this repository and navigate to the FastChat folder
 ```bash
 git clone https://github.com/lm-sys/FastChat.git
 cd FastChat
 ```
 
+If you are running on Mac:
+```bash
+brew install rust
+```
+
 2. Install Package
 ```bash
 pip3 install --upgrade pip  # enable PEP 660 support
 pip3 install -e .
 ```
 
 ## Vicuna Weights
 We release [Vicuna](https://vicuna.lmsys.org/) weights as delta weights to comply with the LLaMA model license.
 You can add our delta to the original LLaMA weights to obtain the Vicuna weights. Instructions:
 
 1. Get the original LLaMA weights in the huggingface format by following the instructions [here](https://huggingface.co/docs/transformers/main/model_doc/llama).
-2. Use the following scripts to get Vicuna weights by applying our delta. They will automatically download delta weights from our Hugging Face account.
+2. Use the following scripts to get Vicuna weights by applying our delta. They will automatically download delta weights from our Hugging Face [account](https://huggingface.co/lmsys).
 
 **NOTE**:
 Our released weights are only compatible with the latest main branch of huggingface/transformers.
 We install the correct version of transformers when fastchat is installed.
 
 ### Vicuna-13B
 This conversion command needs around 60 GB of CPU RAM.
+If you do not have enough memory, you can create a large swap file that allows the operating system to automatically utilize the disk as virtual memory.
 ```bash
 python3 -m fastchat.model.apply_delta \
     --base /path/to/llama-13b \
     --target /output/path/to/vicuna-13b \
     --delta lmsys/vicuna-13b-delta-v0
 ```
 
 ### Vicuna-7B
 This conversion command needs around 30 GB of CPU RAM.
+If you do not have enough memory, you can create a large swap file that allows the operating system to automatically utilize the disk as virtual memory.
 ```bash
 python3 -m fastchat.model.apply_delta \
     --base /path/to/llama-7b \
     --target /output/path/to/vicuna-7b \
     --delta lmsys/vicuna-7b-delta-v0
 ```
 
 ## Inference with Command Line Interface
 
-### Single GPU
+#### Single GPU
 The command below requires around 28GB of GPU memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B.
 ```
 python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights
 ```
 
-### Multiple GPUs
+#### Multiple GPUs
 If you do not have enough GPU memory, you can use model parallelism to aggregate memory from multiple GPUs on the same machine.
 ```
 python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights --num-gpus 2
 ```
 
-### CPU Only
+#### CPU Only
 This runs on the CPU only and does not require GPU. It requires around 60GB of CPU memory for Vicuna-13B and around 30GB of CPU memory for Vicuna-7B.
 ```
 python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights --device cpu
 ```
 
-### Metal Backend (Mac computers with Apple silicon or AMD GPUs)
+#### Metal Backend (Mac Computers with Apple Silicon or AMD GPUs)
 Use `--device mps` to enable GPU acceleration on Mac computers and use `--load-8bit` to turn on 8-bit compression.
 ```
 python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights --device mps --load-8bit
 ```
+Vicuna-7B can run on a 32GB M1 Macbook with 1 - 2 words / second.
 
-### Others (Quantization, Low-end Devices, and More Platforms)
+#### No Enough Memory or Other Platforms
 If you do not have enough memory, you can enable 8-bit compression by adding `--load-8bit` to commands above.
-It works with CPU, GPU, and Metal.
 This can reduce the memory usage by around half with slightly degraded model quality.
+It is compatible with the CPU, GPU, and Metal backend.
+Vicuna-13B with 8-bit compression can run on a single NVIDIA 3090/4090/V100(16GB) GPU.
 
 ```
 python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights --load-8bit
 ```
 
 Besides, we are actively exploring more methods to make the model easier to run on more platforms.
 Contributions and pull requests are welcome.
 
 ## Serving with Web GUI
 
-### Launch a controller
+To serve using the web UI, you need three main components: web servers that interface with users, model workers that host one or more models, and a controller to coordinate the webserver and model workers. Here are the commands to follow in your terminal:
+
+**Note for Windows users:** Windows users will need Python 3.7 and above and to set the following environmental variable prior to launching the worker.
+
+```
+PYTHONUTF8=1
+```
+
+#### Launch the controller
 ```bash
 python3 -m fastchat.serve.controller
 ```
 
-### Launch a model worker
+This controller manages the distributed workers.
+
+#### Launch the model worker
 ```bash
 python3 -m fastchat.serve.model_worker --model-path /path/to/vicuna/weights
 ```
-Wait until the process finishes loading the model and you see "Uvicorn running on ...".
+Wait until the process finishes loading the model and you see "Uvicorn running on ...". You can launch multiple model workers to serve multiple models concurrently. The model worker will connect to the controller automatically.
 
-### Send a test message
+To ensure that your model worker is connected to your controller properly, send a test message using the following command:
 ```bash
 python3 -m fastchat.serve.test_message --model-name vicuna-13b
 ```
 
-### Launch a gradio web server.
+#### Launch the Gradio web server
 ```bash
 python3 -m fastchat.serve.gradio_web_server
 ```
 
-### You can open your browser and chat with a model now.
+This is the user interface that users will interact with.
+
+By following these steps, you will be able to serve your models using the web UI. You can open your browser and chat with a model now.
+
 
 ## Evaluation
 
 Our AI-enhanced [evaluation](fastchat/eval) pipeline is based on GPT-4. Here are some high-level instructions for using the pipeline:
 
 First, generate answers from different models. Use `qa_baseline_gpt35.py` for ChatGPT, or specify the model checkpoint and run `model_qa.py` for Vicuna and other models.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fschat Version: 0.1.8 Summary: An open platform for
+Metadata-Version: 2.1 Name: fschat Version: 0.1.9 Summary: An open platform for
 training, serving, and evaluating large language model based chatbots. Project-
 URL: Homepage, https://github.com/lm-sys/fastchat Project-URL: Bug Tracker,
 https://github.com/lm-sys/fastchat/issues Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE # FastChat An open platform for training, serving, and evaluating large
 language model based chatbots. ## Release
@@ -15,70 +15,89 @@
 (#install) - [Vicuna Weights](#vicuna-weights) - [Inference with Command Line
 Interface](#inference-with-command-line-interface) - [Serving with Web GUI]
 (#serving-with-web-gui) - [Evaluation](#evaluation) - [Fine-tuning](#fine-
 tuning) ## Install ### Method 1: With pip ```bash # Install FastChat pip3
 install fschat # Install the latest main branch of huggingface/transformers
 pip3 install git+https://github.com/huggingface/transformers ``` ### Method 2:
 From source 1. Clone this repository and navigate to the FastChat folder
-```bash git clone https://github.com/lm-sys/FastChat.git cd FastChat ``` 2.
-Install Package ```bash pip3 install --upgrade pip # enable PEP 660 support
-pip3 install -e . ``` ## Vicuna Weights We release [Vicuna](https://
-vicuna.lmsys.org/) weights as delta weights to comply with the LLaMA model
-license. You can add our delta to the original LLaMA weights to obtain the
-Vicuna weights. Instructions: 1. Get the original LLaMA weights in the
-huggingface format by following the instructions [here](https://huggingface.co/
-docs/transformers/main/model_doc/llama). 2. Use the following scripts to get
-Vicuna weights by applying our delta. They will automatically download delta
-weights from our Hugging Face account. **NOTE**: Our released weights are only
-compatible with the latest main branch of huggingface/transformers. We install
-the correct version of transformers when fastchat is installed. ### Vicuna-13B
-This conversion command needs around 60 GB of CPU RAM. ```bash python3 -
+```bash git clone https://github.com/lm-sys/FastChat.git cd FastChat ``` If you
+are running on Mac: ```bash brew install rust ``` 2. Install Package ```bash
+pip3 install --upgrade pip # enable PEP 660 support pip3 install -e . ``` ##
+Vicuna Weights We release [Vicuna](https://vicuna.lmsys.org/) weights as delta
+weights to comply with the LLaMA model license. You can add our delta to the
+original LLaMA weights to obtain the Vicuna weights. Instructions: 1. Get the
+original LLaMA weights in the huggingface format by following the instructions
+[here](https://huggingface.co/docs/transformers/main/model_doc/llama). 2. Use
+the following scripts to get Vicuna weights by applying our delta. They will
+automatically download delta weights from our Hugging Face [account](https://
+huggingface.co/lmsys). **NOTE**: Our released weights are only compatible with
+the latest main branch of huggingface/transformers. We install the correct
+version of transformers when fastchat is installed. ### Vicuna-13B This
+conversion command needs around 60 GB of CPU RAM. If you do not have enough
+memory, you can create a large swap file that allows the operating system to
+automatically utilize the disk as virtual memory. ```bash python3 -
 m fastchat.model.apply_delta \ --base /path/to/llama-13b \ --target /output/
 path/to/vicuna-13b \ --delta lmsys/vicuna-13b-delta-v0 ``` ### Vicuna-7B This
-conversion command needs around 30 GB of CPU RAM. ```bash python3 -
+conversion command needs around 30 GB of CPU RAM. If you do not have enough
+memory, you can create a large swap file that allows the operating system to
+automatically utilize the disk as virtual memory. ```bash python3 -
 m fastchat.model.apply_delta \ --base /path/to/llama-7b \ --target /output/
 path/to/vicuna-7b \ --delta lmsys/vicuna-7b-delta-v0 ``` ## Inference with
-Command Line Interface ### Single GPU The command below requires around 28GB of
-GPU memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B. ``` python3 -
-m fastchat.serve.cli --model-name /path/to/vicuna/weights ``` ### Multiple GPUs
-If you do not have enough GPU memory, you can use model parallelism to
+Command Line Interface #### Single GPU The command below requires around 28GB
+of GPU memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B. ``` python3
+-m fastchat.serve.cli --model-name /path/to/vicuna/weights ``` #### Multiple
+GPUs If you do not have enough GPU memory, you can use model parallelism to
 aggregate memory from multiple GPUs on the same machine. ``` python3 -
-m fastchat.serve.cli --model-name /path/to/vicuna/weights --num-gpus 2 ``` ###
+m fastchat.serve.cli --model-name /path/to/vicuna/weights --num-gpus 2 ``` ####
 CPU Only This runs on the CPU only and does not require GPU. It requires around
 60GB of CPU memory for Vicuna-13B and around 30GB of CPU memory for Vicuna-7B.
 ``` python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights --device
-cpu ``` ### Metal Backend (Mac computers with Apple silicon or AMD GPUs) Use `-
--device mps` to enable GPU acceleration on Mac computers and use `--load-8bit`
-to turn on 8-bit compression. ``` python3 -m fastchat.serve.cli --model-name /
-path/to/vicuna/weights --device mps --load-8bit ``` ### Others (Quantization,
-Low-end Devices, and More Platforms) If you do not have enough memory, you can
-enable 8-bit compression by adding `--load-8bit` to commands above. It works
-with CPU, GPU, and Metal. This can reduce the memory usage by around half with
-slightly degraded model quality. ``` python3 -m fastchat.serve.cli --model-name
-/path/to/vicuna/weights --load-8bit ``` Besides, we are actively exploring more
-methods to make the model easier to run on more platforms. Contributions and
-pull requests are welcome. ## Serving with Web GUI ### Launch a controller
-```bash python3 -m fastchat.serve.controller ``` ### Launch a model worker
-```bash python3 -m fastchat.serve.model_worker --model-path /path/to/vicuna/
-weights ``` Wait until the process finishes loading the model and you see
-"Uvicorn running on ...". ### Send a test message ```bash python3 -
-m fastchat.serve.test_message --model-name vicuna-13b ``` ### Launch a gradio
-web server. ```bash python3 -m fastchat.serve.gradio_web_server ``` ### You can
-open your browser and chat with a model now. ## Evaluation Our AI-enhanced
-[evaluation](fastchat/eval) pipeline is based on GPT-4. Here are some high-
-level instructions for using the pipeline: First, generate answers from
-different models. Use `qa_baseline_gpt35.py` for ChatGPT, or specify the model
-checkpoint and run `model_qa.py` for Vicuna and other models. Then, use GPT-
-4 to generate reviews automatically, which can be done manually if the GPT-
-4 API is not available to you. Once you have your evaluation data, visualize
-the results by running `generate_webpage_data_from_table.py`, which generates
-data for a static website. Finally, serve a static website under the `webpage`
-directory. You can simply use `python3 -m http.server` to serve the website
-locally. Besides the evaluation workflow, we also document the data format used
-for evaluation, which is encoded with JSON Lines and includes information on
+cpu ``` #### Metal Backend (Mac Computers with Apple Silicon or AMD GPUs) Use
+`--device mps` to enable GPU acceleration on Mac computers and use `--load-
+8bit` to turn on 8-bit compression. ``` python3 -m fastchat.serve.cli --model-
+name /path/to/vicuna/weights --device mps --load-8bit ``` Vicuna-7B can run on
+a 32GB M1 Macbook with 1 - 2 words / second. #### No Enough Memory or Other
+Platforms If you do not have enough memory, you can enable 8-bit compression by
+adding `--load-8bit` to commands above. This can reduce the memory usage by
+around half with slightly degraded model quality. It is compatible with the
+CPU, GPU, and Metal backend. Vicuna-13B with 8-bit compression can run on a
+single NVIDIA 3090/4090/V100(16GB) GPU. ``` python3 -m fastchat.serve.cli --
+model-name /path/to/vicuna/weights --load-8bit ``` Besides, we are actively
+exploring more methods to make the model easier to run on more platforms.
+Contributions and pull requests are welcome. ## Serving with Web GUI To serve
+using the web UI, you need three main components: web servers that interface
+with users, model workers that host one or more models, and a controller to
+coordinate the webserver and model workers. Here are the commands to follow in
+your terminal: **Note for Windows users:** Windows users will need Python 3.7
+and above and to set the following environmental variable prior to launching
+the worker. ``` PYTHONUTF8=1 ``` #### Launch the controller ```bash python3 -
+m fastchat.serve.controller ``` This controller manages the distributed
+workers. #### Launch the model worker ```bash python3 -
+m fastchat.serve.model_worker --model-path /path/to/vicuna/weights ``` Wait
+until the process finishes loading the model and you see "Uvicorn running on
+...". You can launch multiple model workers to serve multiple models
+concurrently. The model worker will connect to the controller automatically. To
+ensure that your model worker is connected to your controller properly, send a
+test message using the following command: ```bash python3 -
+m fastchat.serve.test_message --model-name vicuna-13b ``` #### Launch the
+Gradio web server ```bash python3 -m fastchat.serve.gradio_web_server ``` This
+is the user interface that users will interact with. By following these steps,
+you will be able to serve your models using the web UI. You can open your
+browser and chat with a model now. ## Evaluation Our AI-enhanced [evaluation]
+(fastchat/eval) pipeline is based on GPT-4. Here are some high-level
+instructions for using the pipeline: First, generate answers from different
+models. Use `qa_baseline_gpt35.py` for ChatGPT, or specify the model checkpoint
+and run `model_qa.py` for Vicuna and other models. Then, use GPT-4 to generate
+reviews automatically, which can be done manually if the GPT-4 API is not
+available to you. Once you have your evaluation data, visualize the results by
+running `generate_webpage_data_from_table.py`, which generates data for a
+static website. Finally, serve a static website under the `webpage` directory.
+You can simply use `python3 -m http.server` to serve the website locally.
+Besides the evaluation workflow, we also document the data format used for
+evaluation, which is encoded with JSON Lines and includes information on
 models, prompts, reviewers, questions, answers, and reviews. You can customize
 the evaluation process or contribute to our project by accessing relevant
 [data](fastchat/eval/table/). Check [evaluation](fastchat/eval) for detailed
 instructions. ## Fine-tuning ### Data Vicuna is created by fine-tuning a LLaMA
 base model using approximately 70K user-shared conversations gathered from
 ShareGPT.com with public APIs. To ensure data quality, we convert the HTML back
 to markdown and filter out some inappropriate or low-quality samples.
```

### Comparing `fschat-0.1.8/README.md` & `fschat-0.1.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -37,111 +37,133 @@
 
 1. Clone this repository and navigate to the FastChat folder
 ```bash
 git clone https://github.com/lm-sys/FastChat.git
 cd FastChat
 ```
 
+If you are running on Mac:
+```bash
+brew install rust
+```
+
 2. Install Package
 ```bash
 pip3 install --upgrade pip  # enable PEP 660 support
 pip3 install -e .
 ```
 
 ## Vicuna Weights
 We release [Vicuna](https://vicuna.lmsys.org/) weights as delta weights to comply with the LLaMA model license.
 You can add our delta to the original LLaMA weights to obtain the Vicuna weights. Instructions:
 
 1. Get the original LLaMA weights in the huggingface format by following the instructions [here](https://huggingface.co/docs/transformers/main/model_doc/llama).
-2. Use the following scripts to get Vicuna weights by applying our delta. They will automatically download delta weights from our Hugging Face account.
+2. Use the following scripts to get Vicuna weights by applying our delta. They will automatically download delta weights from our Hugging Face [account](https://huggingface.co/lmsys).
 
 **NOTE**:
 Our released weights are only compatible with the latest main branch of huggingface/transformers.
 We install the correct version of transformers when fastchat is installed.
 
 ### Vicuna-13B
 This conversion command needs around 60 GB of CPU RAM.
+If you do not have enough memory, you can create a large swap file that allows the operating system to automatically utilize the disk as virtual memory.
 ```bash
 python3 -m fastchat.model.apply_delta \
     --base /path/to/llama-13b \
     --target /output/path/to/vicuna-13b \
     --delta lmsys/vicuna-13b-delta-v0
 ```
 
 ### Vicuna-7B
 This conversion command needs around 30 GB of CPU RAM.
+If you do not have enough memory, you can create a large swap file that allows the operating system to automatically utilize the disk as virtual memory.
 ```bash
 python3 -m fastchat.model.apply_delta \
     --base /path/to/llama-7b \
     --target /output/path/to/vicuna-7b \
     --delta lmsys/vicuna-7b-delta-v0
 ```
 
 ## Inference with Command Line Interface
 
-### Single GPU
+#### Single GPU
 The command below requires around 28GB of GPU memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B.
 ```
 python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights
 ```
 
-### Multiple GPUs
+#### Multiple GPUs
 If you do not have enough GPU memory, you can use model parallelism to aggregate memory from multiple GPUs on the same machine.
 ```
 python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights --num-gpus 2
 ```
 
-### CPU Only
+#### CPU Only
 This runs on the CPU only and does not require GPU. It requires around 60GB of CPU memory for Vicuna-13B and around 30GB of CPU memory for Vicuna-7B.
 ```
 python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights --device cpu
 ```
 
-### Metal Backend (Mac computers with Apple silicon or AMD GPUs)
+#### Metal Backend (Mac Computers with Apple Silicon or AMD GPUs)
 Use `--device mps` to enable GPU acceleration on Mac computers and use `--load-8bit` to turn on 8-bit compression.
 ```
 python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights --device mps --load-8bit
 ```
+Vicuna-7B can run on a 32GB M1 Macbook with 1 - 2 words / second.
 
-### Others (Quantization, Low-end Devices, and More Platforms)
+#### No Enough Memory or Other Platforms
 If you do not have enough memory, you can enable 8-bit compression by adding `--load-8bit` to commands above.
-It works with CPU, GPU, and Metal.
 This can reduce the memory usage by around half with slightly degraded model quality.
+It is compatible with the CPU, GPU, and Metal backend.
+Vicuna-13B with 8-bit compression can run on a single NVIDIA 3090/4090/V100(16GB) GPU.
 
 ```
 python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights --load-8bit
 ```
 
 Besides, we are actively exploring more methods to make the model easier to run on more platforms.
 Contributions and pull requests are welcome.
 
 ## Serving with Web GUI
 
-### Launch a controller
+To serve using the web UI, you need three main components: web servers that interface with users, model workers that host one or more models, and a controller to coordinate the webserver and model workers. Here are the commands to follow in your terminal:
+
+**Note for Windows users:** Windows users will need Python 3.7 and above and to set the following environmental variable prior to launching the worker.
+
+```
+PYTHONUTF8=1
+```
+
+#### Launch the controller
 ```bash
 python3 -m fastchat.serve.controller
 ```
 
-### Launch a model worker
+This controller manages the distributed workers.
+
+#### Launch the model worker
 ```bash
 python3 -m fastchat.serve.model_worker --model-path /path/to/vicuna/weights
 ```
-Wait until the process finishes loading the model and you see "Uvicorn running on ...".
+Wait until the process finishes loading the model and you see "Uvicorn running on ...". You can launch multiple model workers to serve multiple models concurrently. The model worker will connect to the controller automatically.
 
-### Send a test message
+To ensure that your model worker is connected to your controller properly, send a test message using the following command:
 ```bash
 python3 -m fastchat.serve.test_message --model-name vicuna-13b
 ```
 
-### Launch a gradio web server.
+#### Launch the Gradio web server
 ```bash
 python3 -m fastchat.serve.gradio_web_server
 ```
 
-### You can open your browser and chat with a model now.
+This is the user interface that users will interact with.
+
+By following these steps, you will be able to serve your models using the web UI. You can open your browser and chat with a model now.
+
 
 ## Evaluation
 
 Our AI-enhanced [evaluation](fastchat/eval) pipeline is based on GPT-4. Here are some high-level instructions for using the pipeline:
 
 First, generate answers from different models. Use `qa_baseline_gpt35.py` for ChatGPT, or specify the model checkpoint and run `model_qa.py` for Vicuna and other models.
```

#### html2text {}

```diff
@@ -9,70 +9,89 @@
 (#install) - [Vicuna Weights](#vicuna-weights) - [Inference with Command Line
 Interface](#inference-with-command-line-interface) - [Serving with Web GUI]
 (#serving-with-web-gui) - [Evaluation](#evaluation) - [Fine-tuning](#fine-
 tuning) ## Install ### Method 1: With pip ```bash # Install FastChat pip3
 install fschat # Install the latest main branch of huggingface/transformers
 pip3 install git+https://github.com/huggingface/transformers ``` ### Method 2:
 From source 1. Clone this repository and navigate to the FastChat folder
-```bash git clone https://github.com/lm-sys/FastChat.git cd FastChat ``` 2.
-Install Package ```bash pip3 install --upgrade pip # enable PEP 660 support
-pip3 install -e . ``` ## Vicuna Weights We release [Vicuna](https://
-vicuna.lmsys.org/) weights as delta weights to comply with the LLaMA model
-license. You can add our delta to the original LLaMA weights to obtain the
-Vicuna weights. Instructions: 1. Get the original LLaMA weights in the
-huggingface format by following the instructions [here](https://huggingface.co/
-docs/transformers/main/model_doc/llama). 2. Use the following scripts to get
-Vicuna weights by applying our delta. They will automatically download delta
-weights from our Hugging Face account. **NOTE**: Our released weights are only
-compatible with the latest main branch of huggingface/transformers. We install
-the correct version of transformers when fastchat is installed. ### Vicuna-13B
-This conversion command needs around 60 GB of CPU RAM. ```bash python3 -
+```bash git clone https://github.com/lm-sys/FastChat.git cd FastChat ``` If you
+are running on Mac: ```bash brew install rust ``` 2. Install Package ```bash
+pip3 install --upgrade pip # enable PEP 660 support pip3 install -e . ``` ##
+Vicuna Weights We release [Vicuna](https://vicuna.lmsys.org/) weights as delta
+weights to comply with the LLaMA model license. You can add our delta to the
+original LLaMA weights to obtain the Vicuna weights. Instructions: 1. Get the
+original LLaMA weights in the huggingface format by following the instructions
+[here](https://huggingface.co/docs/transformers/main/model_doc/llama). 2. Use
+the following scripts to get Vicuna weights by applying our delta. They will
+automatically download delta weights from our Hugging Face [account](https://
+huggingface.co/lmsys). **NOTE**: Our released weights are only compatible with
+the latest main branch of huggingface/transformers. We install the correct
+version of transformers when fastchat is installed. ### Vicuna-13B This
+conversion command needs around 60 GB of CPU RAM. If you do not have enough
+memory, you can create a large swap file that allows the operating system to
+automatically utilize the disk as virtual memory. ```bash python3 -
 m fastchat.model.apply_delta \ --base /path/to/llama-13b \ --target /output/
 path/to/vicuna-13b \ --delta lmsys/vicuna-13b-delta-v0 ``` ### Vicuna-7B This
-conversion command needs around 30 GB of CPU RAM. ```bash python3 -
+conversion command needs around 30 GB of CPU RAM. If you do not have enough
+memory, you can create a large swap file that allows the operating system to
+automatically utilize the disk as virtual memory. ```bash python3 -
 m fastchat.model.apply_delta \ --base /path/to/llama-7b \ --target /output/
 path/to/vicuna-7b \ --delta lmsys/vicuna-7b-delta-v0 ``` ## Inference with
-Command Line Interface ### Single GPU The command below requires around 28GB of
-GPU memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B. ``` python3 -
-m fastchat.serve.cli --model-name /path/to/vicuna/weights ``` ### Multiple GPUs
-If you do not have enough GPU memory, you can use model parallelism to
+Command Line Interface #### Single GPU The command below requires around 28GB
+of GPU memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B. ``` python3
+-m fastchat.serve.cli --model-name /path/to/vicuna/weights ``` #### Multiple
+GPUs If you do not have enough GPU memory, you can use model parallelism to
 aggregate memory from multiple GPUs on the same machine. ``` python3 -
-m fastchat.serve.cli --model-name /path/to/vicuna/weights --num-gpus 2 ``` ###
+m fastchat.serve.cli --model-name /path/to/vicuna/weights --num-gpus 2 ``` ####
 CPU Only This runs on the CPU only and does not require GPU. It requires around
 60GB of CPU memory for Vicuna-13B and around 30GB of CPU memory for Vicuna-7B.
 ``` python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights --device
-cpu ``` ### Metal Backend (Mac computers with Apple silicon or AMD GPUs) Use `-
--device mps` to enable GPU acceleration on Mac computers and use `--load-8bit`
-to turn on 8-bit compression. ``` python3 -m fastchat.serve.cli --model-name /
-path/to/vicuna/weights --device mps --load-8bit ``` ### Others (Quantization,
-Low-end Devices, and More Platforms) If you do not have enough memory, you can
-enable 8-bit compression by adding `--load-8bit` to commands above. It works
-with CPU, GPU, and Metal. This can reduce the memory usage by around half with
-slightly degraded model quality. ``` python3 -m fastchat.serve.cli --model-name
-/path/to/vicuna/weights --load-8bit ``` Besides, we are actively exploring more
-methods to make the model easier to run on more platforms. Contributions and
-pull requests are welcome. ## Serving with Web GUI ### Launch a controller
-```bash python3 -m fastchat.serve.controller ``` ### Launch a model worker
-```bash python3 -m fastchat.serve.model_worker --model-path /path/to/vicuna/
-weights ``` Wait until the process finishes loading the model and you see
-"Uvicorn running on ...". ### Send a test message ```bash python3 -
-m fastchat.serve.test_message --model-name vicuna-13b ``` ### Launch a gradio
-web server. ```bash python3 -m fastchat.serve.gradio_web_server ``` ### You can
-open your browser and chat with a model now. ## Evaluation Our AI-enhanced
-[evaluation](fastchat/eval) pipeline is based on GPT-4. Here are some high-
-level instructions for using the pipeline: First, generate answers from
-different models. Use `qa_baseline_gpt35.py` for ChatGPT, or specify the model
-checkpoint and run `model_qa.py` for Vicuna and other models. Then, use GPT-
-4 to generate reviews automatically, which can be done manually if the GPT-
-4 API is not available to you. Once you have your evaluation data, visualize
-the results by running `generate_webpage_data_from_table.py`, which generates
-data for a static website. Finally, serve a static website under the `webpage`
-directory. You can simply use `python3 -m http.server` to serve the website
-locally. Besides the evaluation workflow, we also document the data format used
-for evaluation, which is encoded with JSON Lines and includes information on
+cpu ``` #### Metal Backend (Mac Computers with Apple Silicon or AMD GPUs) Use
+`--device mps` to enable GPU acceleration on Mac computers and use `--load-
+8bit` to turn on 8-bit compression. ``` python3 -m fastchat.serve.cli --model-
+name /path/to/vicuna/weights --device mps --load-8bit ``` Vicuna-7B can run on
+a 32GB M1 Macbook with 1 - 2 words / second. #### No Enough Memory or Other
+Platforms If you do not have enough memory, you can enable 8-bit compression by
+adding `--load-8bit` to commands above. This can reduce the memory usage by
+around half with slightly degraded model quality. It is compatible with the
+CPU, GPU, and Metal backend. Vicuna-13B with 8-bit compression can run on a
+single NVIDIA 3090/4090/V100(16GB) GPU. ``` python3 -m fastchat.serve.cli --
+model-name /path/to/vicuna/weights --load-8bit ``` Besides, we are actively
+exploring more methods to make the model easier to run on more platforms.
+Contributions and pull requests are welcome. ## Serving with Web GUI To serve
+using the web UI, you need three main components: web servers that interface
+with users, model workers that host one or more models, and a controller to
+coordinate the webserver and model workers. Here are the commands to follow in
+your terminal: **Note for Windows users:** Windows users will need Python 3.7
+and above and to set the following environmental variable prior to launching
+the worker. ``` PYTHONUTF8=1 ``` #### Launch the controller ```bash python3 -
+m fastchat.serve.controller ``` This controller manages the distributed
+workers. #### Launch the model worker ```bash python3 -
+m fastchat.serve.model_worker --model-path /path/to/vicuna/weights ``` Wait
+until the process finishes loading the model and you see "Uvicorn running on
+...". You can launch multiple model workers to serve multiple models
+concurrently. The model worker will connect to the controller automatically. To
+ensure that your model worker is connected to your controller properly, send a
+test message using the following command: ```bash python3 -
+m fastchat.serve.test_message --model-name vicuna-13b ``` #### Launch the
+Gradio web server ```bash python3 -m fastchat.serve.gradio_web_server ``` This
+is the user interface that users will interact with. By following these steps,
+you will be able to serve your models using the web UI. You can open your
+browser and chat with a model now. ## Evaluation Our AI-enhanced [evaluation]
+(fastchat/eval) pipeline is based on GPT-4. Here are some high-level
+instructions for using the pipeline: First, generate answers from different
+models. Use `qa_baseline_gpt35.py` for ChatGPT, or specify the model checkpoint
+and run `model_qa.py` for Vicuna and other models. Then, use GPT-4 to generate
+reviews automatically, which can be done manually if the GPT-4 API is not
+available to you. Once you have your evaluation data, visualize the results by
+running `generate_webpage_data_from_table.py`, which generates data for a
+static website. Finally, serve a static website under the `webpage` directory.
+You can simply use `python3 -m http.server` to serve the website locally.
+Besides the evaluation workflow, we also document the data format used for
+evaluation, which is encoded with JSON Lines and includes information on
 models, prompts, reviewers, questions, answers, and reviews. You can customize
 the evaluation process or contribute to our project by accessing relevant
 [data](fastchat/eval/table/). Check [evaluation](fastchat/eval) for detailed
 instructions. ## Fine-tuning ### Data Vicuna is created by fine-tuning a LLaMA
 base model using approximately 70K user-shared conversations gathered from
 ShareGPT.com with public APIs. To ensure data quality, we convert the HTML back
 to markdown and filter out some inappropriate or low-quality samples.
```

### Comparing `fschat-0.1.8/fastchat/conversation.py` & `fschat-0.1.9/fastchat/conversation.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.8/fastchat/data/alpaca-converter.py` & `fschat-0.1.9/fastchat/data/alpaca-converter.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.8/fastchat/data/clean_sharegpt.py` & `fschat-0.1.9/fastchat/data/clean_sharegpt.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.8/fastchat/data/inspect.py` & `fschat-0.1.9/fastchat/data/inspect.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.8/fastchat/data/optional_clean.py` & `fschat-0.1.9/fastchat/data/optional_clean.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.8/fastchat/data/split_long_conversation.py` & `fschat-0.1.9/fastchat/data/split_long_conversation.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.8/fastchat/eval/eval_gpt_review.py` & `fschat-0.1.9/fastchat/eval/eval_gpt_review.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.8/fastchat/eval/generate_webpage_data_from_table.py` & `fschat-0.1.9/fastchat/eval/generate_webpage_data_from_table.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.8/fastchat/eval/get_model_answer.py` & `fschat-0.1.9/fastchat/eval/get_model_answer.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.8/fastchat/eval/qa_baseline_gpt35.py` & `fschat-0.1.9/fastchat/eval/qa_baseline_gpt35.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.8/fastchat/model/apply_delta.py` & `fschat-0.1.9/fastchat/model/apply_delta.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 """
+Apply the delta weights on top of a base model.
+
 Usage:
 python3 -m fastchat.model.apply_delta --base ~/model_weights/llama-13b --target ~/model_weights/vicuna-13b --delta lmsys/vicuna-13b-delta
 """
 import argparse
 
 import torch
 from tqdm import tqdm
 from transformers import AutoTokenizer, AutoModelForCausalLM
 
 
 def apply_delta(base_model_path, target_model_path, delta_path):
-    print("Loading base model")
+    print(f"Loading the base model from {base_model_path}")
     base = AutoModelForCausalLM.from_pretrained(
         base_model_path, torch_dtype=torch.float16, low_cpu_mem_usage=True)
 
-    print("Loading delta")
+    print(f"Loading the delta from {delta_path}")
     delta = AutoModelForCausalLM.from_pretrained(delta_path, torch_dtype=torch.float16, low_cpu_mem_usage=True)
     delta_tokenizer = AutoTokenizer.from_pretrained(delta_path, use_fast=False)
 
     DEFAULT_PAD_TOKEN = "[PAD]"
     base_tokenizer = AutoTokenizer.from_pretrained(base_model_path, use_fast=False)
     num_new_tokens = base_tokenizer.add_special_tokens(dict(pad_token=DEFAULT_PAD_TOKEN))
 
     base.resize_token_embeddings(len(base_tokenizer))
     input_embeddings = base.get_input_embeddings().weight.data
     output_embeddings = base.get_output_embeddings().weight.data
     input_embeddings[-num_new_tokens:] = 0
     output_embeddings[-num_new_tokens:] = 0
 
-    print("Applying delta")
+    print("Applying the delta")
     for name, param in tqdm(base.state_dict().items(), desc="Applying delta"):
         assert name in delta.state_dict()
         param.data += delta.state_dict()[name]
 
-    print("Saving target model")
+    print(f"Saving the target model to {target_model_path}")
     base.save_pretrained(target_model_path)
     delta_tokenizer.save_pretrained(target_model_path)
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--base-model-path", type=str, required=True)
```

### Comparing `fschat-0.1.8/fastchat/model/make_delta.py` & `fschat-0.1.9/fastchat/model/make_delta.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 """
+Make the delta weights by subtracting base weights.
+
 Usage:
 python3 -m fastchat.model.make_delta --base ~/model_weights/llama-13b --target ~/model_weights/vicuna-13b --delta ~/model_weights/vicuna-13b-delta --hub-repo-id lmsys/vicuna-13b-delta
 """
 import argparse
 
 import torch
 from tqdm import tqdm
 from transformers import AutoTokenizer, AutoModelForCausalLM
 
 
 def make_delta(base_model_path, target_model_path, delta_path):
-    print("Loading base model")
+    print(f"Loading the base model from {base_model_path}")
     base = AutoModelForCausalLM.from_pretrained(
         base_model_path, torch_dtype=torch.float16, low_cpu_mem_usage=True)
 
-    print("Loading target model")
+    print(f"Loading the target model from {target_model_path}")
     target = AutoModelForCausalLM.from_pretrained(target_model_path, torch_dtype=torch.float16, low_cpu_mem_usage=True)
 
     DEFAULT_PAD_TOKEN = "[PAD]"
     base_tokenizer = AutoTokenizer.from_pretrained(base_model_path, use_fast=False)
     num_new_tokens = base_tokenizer.add_special_tokens(dict(pad_token=DEFAULT_PAD_TOKEN))
 
     base.resize_token_embeddings(len(base_tokenizer))
     input_embeddings = base.get_input_embeddings().weight.data
     output_embeddings = base.get_output_embeddings().weight.data
     input_embeddings[-num_new_tokens:] = 0
     output_embeddings[-num_new_tokens:] = 0
 
-    print("Calculating delta")
+    print("Calculating the delta")
     for name, param in tqdm(target.state_dict().items(), desc="Calculating delta"):
         assert name in base.state_dict()
         param.data -= base.state_dict()[name]
 
-    print("Saving delta")
+    print(f"Saving the delta to {delta_path}")
     if args.hub_repo_id:
         kwargs = {"push_to_hub": True, "repo_id": args.hub_repo_id}
     else:
         kwargs = {}
     target.save_pretrained(delta_path, **kwargs)
     target_tokenizer = AutoTokenizer.from_pretrained(target_model_path, use_fast=False)
     target_tokenizer.save_pretrained(delta_path, **kwargs)
```

### Comparing `fschat-0.1.8/fastchat/serve/cli.py` & `fschat-0.1.9/fastchat/serve/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,72 +1,69 @@
 """
+Chat with a model with command line interface.
+
 Usage:
 python3 -m fastchat.serve.cli --model ~/model_weights/llama-7b
 """
 import argparse
 import time
 
 import torch
-from transformers import AutoTokenizer, AutoModelForCausalLM, LlamaTokenizer
+from transformers import AutoTokenizer, AutoModelForCausalLM, LlamaTokenizer, AutoModel
 
 from fastchat.conversation import conv_templates, SeparatorStyle
 from fastchat.serve.compression import compress_module
 from fastchat.serve.monkey_patch_non_inplace import replace_llama_attn_with_non_inplace_operations
+from fastchat.serve.serve_chatglm import chatglm_generate_stream
 
 
 def load_model(model_name, device, num_gpus, load_8bit=False, debug=False):
     if device == "cpu":
         kwargs = {}
     elif device == "cuda":
         kwargs = {"torch_dtype": torch.float16}
-        if load_8bit:
-            if num_gpus != "auto" and int(num_gpus) != 1:
-                print("8-bit weights are not supported on multiple GPUs. Revert to use one GPU.")
-            kwargs.update({"load_in_8bit": True, "device_map": "auto"})
+        if num_gpus == "auto":
+            kwargs["device_map"] = "auto"
         else:
-            if num_gpus == "auto":
-                kwargs["device_map"] = "auto"
-            else:
-                num_gpus = int(num_gpus)
-                if num_gpus != 1:
-                    kwargs.update({
-                        "device_map": "auto",
-                        "max_memory": {i: "13GiB" for i in range(num_gpus)},
-                    })
+            num_gpus = int(num_gpus)
+            if num_gpus != 1:
+                kwargs.update({
+                    "device_map": "auto",
+                    "max_memory": {i: "13GiB" for i in range(num_gpus)},
+                })
     elif device == "mps":
         kwargs = {"torch_dtype": torch.float16}
         # Avoid bugs in mps backend by not using in-place operations.
         replace_llama_attn_with_non_inplace_operations()
     else:
         raise ValueError(f"Invalid device: {device}")
 
-    tokenizer = AutoTokenizer.from_pretrained(model_name, use_fast=False)
-    model = AutoModelForCausalLM.from_pretrained(model_name,
-        low_cpu_mem_usage=True, **kwargs)
-
-    # calling model.cuda() mess up weights if loading 8-bit weights
-    if device == "cuda" and num_gpus == 1 and not load_8bit:
-        model.to("cuda")
-    elif device == "mps":
-        model.to("mps")
+    if "chatglm" in model_name:
+        tokenizer = AutoTokenizer.from_pretrained(model_name, trust_remote_code=True)
+        model = AutoModel.from_pretrained(model_name, trust_remote_code=True).half().cuda()
+    else:
+        tokenizer = AutoTokenizer.from_pretrained(model_name, use_fast=False)
+        model = AutoModelForCausalLM.from_pretrained(model_name,
+            low_cpu_mem_usage=True, **kwargs)
+
+    if load_8bit:
+        compress_module(model, device)
 
-    if (device == "mps" or device == "cpu") and load_8bit:
-        compress_module(model)
+    if (device == "cuda" and num_gpus == 1) or device == "mps":
+        model.to(device)
 
     if debug:
         print(model)
 
     return model, tokenizer
 
 
 @torch.inference_mode()
-def generate_stream(tokenizer, model, params, device,
+def generate_stream(model, tokenizer, params, device,
                     context_len=2048, stream_interval=2):
-    """Adapted from fastchat/serve/model_worker.py::generate_stream"""
-
     prompt = params["prompt"]
     l_prompt = len(prompt)
     temperature = float(params.get("temperature", 1.0))
     max_new_tokens = int(params.get("max_new_tokens", 256))
     stop_str = params.get("stop", None)
 
     input_ids = tokenizer(prompt).input_ids
@@ -126,42 +123,51 @@
 
 def main(args):
     model_name = args.model_name
 
     # Model
     model, tokenizer = load_model(args.model_name, args.device,
         args.num_gpus, args.load_8bit, args.debug)
+    is_chatglm = "chatglm" in str(type(model)).lower()
 
     # Chat
     conv = conv_templates[args.conv_template].copy()
     while True:
         try:
             inp = input(f"{conv.roles[0]}: ")
         except EOFError:
             inp = ""
         if not inp:
             print("exit...")
             break
 
         conv.append_message(conv.roles[0], inp)
         conv.append_message(conv.roles[1], None)
-        prompt = conv.get_prompt()
+
+        if is_chatglm:
+            prompt = conv.messages[conv.offset:]
+            generate_stream_func = chatglm_generate_stream
+            skip_echo_len = len(conv.messages[-2][1]) + 1
+        else:
+            generate_stream_func = generate_stream
+            prompt = conv.get_prompt()
+            skip_echo_len = len(prompt) + 1
 
         params = {
             "model": model_name,
             "prompt": prompt,
             "temperature": args.temperature,
             "max_new_tokens": args.max_new_tokens,
             "stop": conv.sep if conv.sep_style == SeparatorStyle.SINGLE else conv.sep2,
         }
 
         print(f"{conv.roles[1]}: ", end="", flush=True)
         pre = 0
-        for outputs in generate_stream(tokenizer, model, params, args.device):
-            outputs = outputs[len(prompt) + 1:].strip()
+        for outputs in generate_stream_func(model, tokenizer, params, args.device):
+            outputs = outputs[skip_echo_len:].strip()
             outputs = outputs.split(" ")
             now = len(outputs)
             if now - 1 > pre:
                 print(" ".join(outputs[pre:now-1]), end=" ", flush=True)
                 pre = now - 1
         print(" ".join(outputs[pre:]), flush=True)
 
@@ -172,14 +178,16 @@
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--model-name", type=str, default="facebook/opt-350m")
     parser.add_argument("--device", type=str, choices=["cpu", "cuda", "mps"], default="cuda")
     parser.add_argument("--num-gpus", type=str, default="1")
-    parser.add_argument("--load-8bit", action="store_true")
-    parser.add_argument("--conv-template", type=str, default="v1")
+    parser.add_argument("--load-8bit", action="store_true",
+        help="Use 8-bit quantization.")
+    parser.add_argument("--conv-template", type=str, default="v1",
+        help="Conversation prompt template.")
     parser.add_argument("--temperature", type=float, default=0.7)
     parser.add_argument("--max-new-tokens", type=int, default=512)
     parser.add_argument("--debug", action="store_true")
     args = parser.parse_args()
     main(args)
```

### Comparing `fschat-0.1.8/fastchat/serve/compression.py` & `fschat-0.1.9/fastchat/serve/compression.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,32 +17,35 @@
 
 
 default_compression_config = CompressionConfig(
     num_bits=8, group_size=256, group_dim=1, symmetric=True, enabled=True)
 
 
 class CLinear(nn.Module):
-    def __init__(self, weight, bias):
+    """Compressed Linear Layer."""
+
+    def __init__(self, weight, bias, device):
         super().__init__()
 
-        self.weight = compress(weight.data, default_compression_config)
+        self.weight = compress(weight.data.to(device), default_compression_config)
         self.bias = bias
 
     def forward(self, input: Tensor) -> Tensor:
         weight = decompress(self.weight, default_compression_config)
         return F.linear(input, weight, self.bias)
 
 
-def compress_module(module):
+def compress_module(module, target_device):
     for attr_str in dir(module):
         target_attr = getattr(module, attr_str)
         if type(target_attr) == torch.nn.Linear:
-            setattr(module, attr_str, CLinear(target_attr.weight, target_attr.bias))
+            setattr(module, attr_str,
+                CLinear(target_attr.weight, target_attr.bias, target_device))
     for name, child in module.named_children():
-        compress_module(child)
+        compress_module(child, target_device)
 
 
 def compress(tensor, config):
     """Simulate group-wise quantization."""
     if not config.enabled:
         return tensor
```

### Comparing `fschat-0.1.8/fastchat/serve/controller.py` & `fschat-0.1.9/fastchat/serve/controller.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.8/fastchat/serve/gradio_css.py` & `fschat-0.1.9/fastchat/serve/gradio_css.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.8/fastchat/serve/gradio_patch.py` & `fschat-0.1.9/fastchat/serve/gradio_patch.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.8/fastchat/serve/gradio_web_server.py` & `fschat-0.1.9/fastchat/serve/gradio_web_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -197,22 +197,27 @@
     # No available worker
     if worker_addr == "":
         state.messages[-1][-1] = server_error_msg
         yield (state, state.to_gradio_chatbot(), disable_btn, disable_btn, disable_btn, enable_btn, enable_btn)
         return
 
     # Construct prompt
-    prompt = state.get_prompt()
+    if "chatglm" in model_name:
+        prompt = state.messages[state.offset:]
+        skip_echo_len = len(state.messages[-2][1]) + 1
+    else:
+        prompt = state.get_prompt()
+        skip_echo_len = len(prompt) + 1
 
     # Make requests
     pload = {
         "model": model_name,
         "prompt": prompt,
         "temperature": float(temperature),
-        "max_new_tokens": min(int(max_new_tokens), 1536),
+        "max_new_tokens": int(max_new_tokens),
         "stop": state.sep if state.sep_style == SeparatorStyle.SINGLE else state.sep2,
     }
     logger.info(f"==== request ====\n{pload}")
 
     state.messages[-1][-1] = "▌"
     yield (state, state.to_gradio_chatbot()) + (disable_btn,) * 5
 
@@ -220,15 +225,15 @@
         # Stream output
         response = requests.post(worker_addr + "/worker_generate_stream",
             headers=headers, json=pload, stream=True, timeout=10)
         for chunk in response.iter_lines(decode_unicode=False, delimiter=b"\0"):
             if chunk:
                 data = json.loads(chunk.decode())
                 if data["error_code"] == 0:
-                    output = data["text"][len(prompt) + 1:].strip()
+                    output = data["text"][skip_echo_len:].strip()
                     output = post_process_code(output)
                     state.messages[-1][-1] = output + "▌"
                     yield (state, state.to_gradio_chatbot()) + (disable_btn,) * 5
                 else:
                     output = data["text"] + f" (error_code: {data['error_code']})"
                     state.messages[-1][-1] = output
                     yield (state, state.to_gradio_chatbot()) + (disable_btn, disable_btn, disable_btn, enable_btn, enable_btn)
@@ -262,20 +267,19 @@
 # 🏔️ Chat with Open Large Language Models
 - Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90% ChatGPT Quality. [[Blog post]](https://vicuna.lmsys.org) [[GitHub]](https://github.com/lm-sys/FastChat)
 - Koala: A Dialogue Model for Academic Research. [[Blog post]](https://bair.berkeley.edu/blog/2023/04/03/koala/) [[GitHub]](https://github.com/young-geng/EasyLM)
 - This demo server. [[GitHub]](https://github.com/lm-sys/FastChat)
 
 ### Terms of use
 By using this service, users are required to agree to the following terms: The service is a research preview intended for non-commercial use only. It only provides limited safety measures and may generate offensive content. It must not be used for any illegal, harmful, violent, racist, or sexual purposes. The service may collect user dialogue data for future research.
-Please click the "Flag" button if you get any inappropriate answer! We will collect those to keep improving our moderator.
-For an optimal experience, please use desktop computers for this demo, as mobile devices may compromise its quality.
 
 ### Choose a model to chat with
 - [Vicuna](https://vicuna.lmsys.org): a chat assistant fine-tuned from LLaMA on user-shared conversations. This one is expected to perform best according to our evaluation.
 - [Koala](https://bair.berkeley.edu/blog/2023/04/03/koala/): a chatbot fine-tuned from LLaMA on user-shared conversations and open-source datasets. This one performs similarly to Vicuna.
+- [ChatGLM](https://chatglm.cn/blog): An Open Bilingual Dialogue Language Model | 开源双语对话语言模型
 - [Alpaca](https://crfm.stanford.edu/2023/03/13/alpaca.html): a model fine-tuned from LLaMA on 52K instruction-following demonstrations.
 - [LLaMA](https://arxiv.org/abs/2302.13971): open and efficient foundation language models
 
 Note: If you are waiting in the queue, check out more benchmark results from GPT-4 on a static website [here](https://vicuna.lmsys.org/eval).
 """)
 
 
@@ -368,22 +372,23 @@
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--host", type=str, default="0.0.0.0")
     parser.add_argument("--port", type=int)
     parser.add_argument("--controller-url", type=str, default="http://localhost:21001")
-    parser.add_argument("--concurrency-count", type=int, default=4)
+    parser.add_argument("--concurrency-count", type=int, default=10)
     parser.add_argument("--model-list-mode", type=str, default="once",
         choices=["once", "reload"])
     parser.add_argument("--share", action="store_true")
-    parser.add_argument("--moderate", action="store_true")
+    parser.add_argument("--moderate", action="store_true",
+        help="Enable content moderation")
     args = parser.parse_args()
     logger.info(f"args: {args}")
 
     models = get_model_list()
 
     logger.info(args)
     demo = build_demo()
     demo.queue(concurrency_count=args.concurrency_count, status_update_rate=10,
-               api_open=False).launch(
-        server_name=args.host, server_port=args.port, share=args.share)
+               api_open=False).launch(server_name=args.host, server_port=args.port,
+                                      share=args.share, max_threads=200)
```

### Comparing `fschat-0.1.8/fastchat/serve/model_worker.py` & `fschat-0.1.9/fastchat/serve/model_worker.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 from fastapi.responses import StreamingResponse
 import requests
 from transformers import AutoTokenizer, AutoModelForCausalLM, LlamaTokenizer
 import torch
 import uvicorn
 
 from fastchat.constants import WORKER_HEART_BEAT_INTERVAL
-from fastchat.serve.cli import load_model
+from fastchat.serve.cli import load_model, generate_stream
+from fastchat.serve.serve_chatglm import chatglm_generate_stream
 from fastchat.utils import (build_logger, server_error_msg,
     pretty_print_semaphore)
 
 GB = 1 << 30
 
 worker_id = str(uuid.uuid4())[:6]
 logger = build_logger("model_worker", f"model_worker_{worker_id}.log")
@@ -58,14 +59,20 @@
         if hasattr(self.model.config, "max_sequence_length"):
             self.context_len = self.model.config.max_sequence_length
         elif hasattr(self.model.config, "max_position_embeddings"):
             self.context_len = self.model.config.max_position_embeddings
         else:
             self.context_len = 2048
 
+        is_chatglm = "chatglm" in str(type(self.model)).lower()
+        if is_chatglm:
+            self.generate_stream_func = chatglm_generate_stream
+        else:
+            self.generate_stream_func = generate_stream
+
         if not no_register:
             self.register_to_controller()
             self.heart_beat_thread = threading.Thread(
                 target=heart_beat_worker, args=(self,))
             self.heart_beat_thread.start()
 
     def register_to_controller(self):
@@ -111,86 +118,23 @@
     def get_status(self):
         return {
             "model_names": [self.model_name],
             "speed": 1,
             "queue_length": self.get_queue_length(),
         }
 
-    @torch.inference_mode()
-    def generate_stream(self, params):
-        #cur_mem = torch.cuda.memory_allocated()
-        #max_mem = torch.cuda.max_memory_allocated()
-        #logging.info(f"cur mem: {cur_mem/GB:.2f} GB, max_mem: {max_mem/GB:.2f} GB")
-
-        tokenizer, model = self.tokenizer, self.model
-
-        prompt = params["prompt"]
-        l_prompt = len(prompt)
-        temperature = float(params.get("temperature", 1.0))
-        max_new_tokens = min(int(params.get("max_new_tokens", 256)), 1024)
-        stop_str = params.get("stop", None)
-
-        input_ids = tokenizer(prompt).input_ids
-        output_ids = list(input_ids)
-
-        max_src_len = self.context_len - max_new_tokens - 8
-        input_ids = input_ids[-max_src_len:]
-
-        for i in range(max_new_tokens):
-            if i == 0:
-                out = model(
-                    torch.as_tensor([input_ids], device=self.device), use_cache=True)
-                logits = out.logits
-                past_key_values = out.past_key_values
-            else:
-                attention_mask = torch.ones(
-                    1, past_key_values[0][0].shape[-2] + 1, device=self.device)
-                out = model(input_ids=torch.as_tensor([[token]], device=self.device),
-                            use_cache=True,
-                            attention_mask=attention_mask,
-                            past_key_values=past_key_values)
-                logits = out.logits
-                past_key_values = out.past_key_values
-
-            last_token_logits = logits[0][-1]
-            if temperature < 1e-4:
-                token = int(torch.argmax(last_token_logits))
-            else:
-                probs = torch.softmax(last_token_logits / temperature, dim=-1)
-                token = int(torch.multinomial(probs, num_samples=1))
-
-            output_ids.append(token)
-
-            if token == tokenizer.eos_token_id:
-                stopped = True
-            else:
-                stopped = False
-
-            if i % args.stream_interval == 0 or i == max_new_tokens - 1 or stopped:
-                output = tokenizer.decode(output_ids, skip_special_tokens=True)
-                pos = output.rfind(stop_str, l_prompt)
-                if pos != -1:
-                    output = output[:pos]
-                    stopped = True
-
+    def generate_stream_gate(self, params):
+        try:
+            for output in self.generate_stream_func(self.model, self.tokenizer,
+                    params, self.device, self.context_len, args.stream_interval):
                 ret = {
                     "text": output,
                     "error_code": 0,
                 }
                 yield json.dumps(ret).encode() + b"\0"
-
-            if stopped:
-                break
-
-        del past_key_values
-
-    def generate_stream_gate(self, params):
-        try:
-            for x in self.generate_stream(params):
-                yield x
         except torch.cuda.OutOfMemoryError:
             ret = {
                 "text": server_error_msg,
                 "error_code": 1,
             }
             yield json.dumps(ret).encode() + b"\0"
 
@@ -199,30 +143,30 @@
 
 
 def release_model_semaphore():
     model_semaphore.release()
 
 
 @app.post("/worker_generate_stream")
-async def generate_stream(request: Request):
+async def api_generate_stream(request: Request):
     global model_semaphore, global_counter
     global_counter += 1
     params = await request.json()
 
     if model_semaphore is None:
         model_semaphore = asyncio.Semaphore(args.limit_model_concurrency)
     await model_semaphore.acquire()
     generator = worker.generate_stream_gate(params)
     background_tasks = BackgroundTasks()
     background_tasks.add_task(release_model_semaphore)
     return StreamingResponse(generator, background=background_tasks)
 
 
 @app.post("/worker_get_status")
-async def get_status(request: Request):
+async def api_get_status(request: Request):
     return worker.get_status()
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--host", type=str, default="localhost")
     parser.add_argument("--port", type=int, default=21002)
```

### Comparing `fschat-0.1.8/fastchat/serve/monkey_patch_non_inplace.py` & `fschat-0.1.9/fastchat/serve/monkey_patch_non_inplace.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.8/fastchat/serve/register_worker.py` & `fschat-0.1.9/fastchat/serve/register_worker.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.8/fastchat/serve/test_message.py` & `fschat-0.1.9/fastchat/serve/test_message.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.8/fastchat/train/llama_flash_attn_monkey_patch.py` & `fschat-0.1.9/fastchat/train/llama_flash_attn_monkey_patch.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.8/fastchat/train/train.py` & `fschat-0.1.9/fastchat/train/train.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.8/fastchat/train/train_lora.py` & `fschat-0.1.9/fastchat/train/train_lora.py`

 * *Files identical despite different names*

### Comparing `fschat-0.1.8/fastchat/utils.py` & `fschat-0.1.9/fastchat/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     formatter = logging.Formatter(
         fmt="%(asctime)s | %(levelname)s | %(name)s | %(message)s",
         datefmt="%Y-%m-%d %H:%M:%S",
     )
 
     # Set the format of root handlers
     if not logging.getLogger().handlers:
-        logging.basicConfig(level=logging.INFO)
+        logging.basicConfig(level=logging.INFO, encoding='utf-8')
     logging.getLogger().handlers[0].setFormatter(formatter)
 
     # Redirect stdout and stderr to loggers
     stdout_logger = logging.getLogger("stdout")
     stdout_logger.setLevel(logging.INFO)
     sl = StreamToLogger(stdout_logger, logging.INFO)
     sys.stdout = sl
@@ -76,21 +76,23 @@
         for line in temp_linebuf.splitlines(True):
             # From the io.TextIOWrapper docs:
             #   On output, if newline is None, any '\n' characters written
             #   are translated to the system default line separator.
             # By default sys.stdout.write() expects '\n' newlines and then
             # translates them so this is still cross platform.
             if line[-1] == '\n':
-                self.logger.log(self.log_level, line.rstrip())
+                encoded_message = line.encode('utf-8', 'ignore').decode('utf-8')
+                self.logger.log(self.log_level, encoded_message.rstrip())
             else:
                 self.linebuf += line
 
     def flush(self):
         if self.linebuf != '':
-            self.logger.log(self.log_level, self.linebuf.rstrip())
+            encoded_message = self.linebuf.encode('utf-8', 'ignore').decode('utf-8')
+            self.logger.log(self.log_level, encoded_message.rstrip())
         self.linebuf = ''
 
 
 def disable_torch_init():
     """
     Disable the redundant torch default initialization to accelerate model creation.
     """
```

### Comparing `fschat-0.1.8/fschat.egg-info/PKG-INFO` & `fschat-0.1.9/fschat.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fschat
-Version: 0.1.8
+Version: 0.1.9
 Summary: An open platform for training, serving, and evaluating large language model based chatbots.
 Project-URL: Homepage, https://github.com/lm-sys/fastchat
 Project-URL: Bug Tracker, https://github.com/lm-sys/fastchat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -49,111 +49,133 @@
 
 1. Clone this repository and navigate to the FastChat folder
 ```bash
 git clone https://github.com/lm-sys/FastChat.git
 cd FastChat
 ```
 
+If you are running on Mac:
+```bash
+brew install rust
+```
+
 2. Install Package
 ```bash
 pip3 install --upgrade pip  # enable PEP 660 support
 pip3 install -e .
 ```
 
 ## Vicuna Weights
 We release [Vicuna](https://vicuna.lmsys.org/) weights as delta weights to comply with the LLaMA model license.
 You can add our delta to the original LLaMA weights to obtain the Vicuna weights. Instructions:
 
 1. Get the original LLaMA weights in the huggingface format by following the instructions [here](https://huggingface.co/docs/transformers/main/model_doc/llama).
-2. Use the following scripts to get Vicuna weights by applying our delta. They will automatically download delta weights from our Hugging Face account.
+2. Use the following scripts to get Vicuna weights by applying our delta. They will automatically download delta weights from our Hugging Face [account](https://huggingface.co/lmsys).
 
 **NOTE**:
 Our released weights are only compatible with the latest main branch of huggingface/transformers.
 We install the correct version of transformers when fastchat is installed.
 
 ### Vicuna-13B
 This conversion command needs around 60 GB of CPU RAM.
+If you do not have enough memory, you can create a large swap file that allows the operating system to automatically utilize the disk as virtual memory.
 ```bash
 python3 -m fastchat.model.apply_delta \
     --base /path/to/llama-13b \
     --target /output/path/to/vicuna-13b \
     --delta lmsys/vicuna-13b-delta-v0
 ```
 
 ### Vicuna-7B
 This conversion command needs around 30 GB of CPU RAM.
+If you do not have enough memory, you can create a large swap file that allows the operating system to automatically utilize the disk as virtual memory.
 ```bash
 python3 -m fastchat.model.apply_delta \
     --base /path/to/llama-7b \
     --target /output/path/to/vicuna-7b \
     --delta lmsys/vicuna-7b-delta-v0
 ```
 
 ## Inference with Command Line Interface
 
-### Single GPU
+#### Single GPU
 The command below requires around 28GB of GPU memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B.
 ```
 python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights
 ```
 
-### Multiple GPUs
+#### Multiple GPUs
 If you do not have enough GPU memory, you can use model parallelism to aggregate memory from multiple GPUs on the same machine.
 ```
 python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights --num-gpus 2
 ```
 
-### CPU Only
+#### CPU Only
 This runs on the CPU only and does not require GPU. It requires around 60GB of CPU memory for Vicuna-13B and around 30GB of CPU memory for Vicuna-7B.
 ```
 python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights --device cpu
 ```
 
-### Metal Backend (Mac computers with Apple silicon or AMD GPUs)
+#### Metal Backend (Mac Computers with Apple Silicon or AMD GPUs)
 Use `--device mps` to enable GPU acceleration on Mac computers and use `--load-8bit` to turn on 8-bit compression.
 ```
 python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights --device mps --load-8bit
 ```
+Vicuna-7B can run on a 32GB M1 Macbook with 1 - 2 words / second.
 
-### Others (Quantization, Low-end Devices, and More Platforms)
+#### No Enough Memory or Other Platforms
 If you do not have enough memory, you can enable 8-bit compression by adding `--load-8bit` to commands above.
-It works with CPU, GPU, and Metal.
 This can reduce the memory usage by around half with slightly degraded model quality.
+It is compatible with the CPU, GPU, and Metal backend.
+Vicuna-13B with 8-bit compression can run on a single NVIDIA 3090/4090/V100(16GB) GPU.
 
 ```
 python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights --load-8bit
 ```
 
 Besides, we are actively exploring more methods to make the model easier to run on more platforms.
 Contributions and pull requests are welcome.
 
 ## Serving with Web GUI
 
-### Launch a controller
+To serve using the web UI, you need three main components: web servers that interface with users, model workers that host one or more models, and a controller to coordinate the webserver and model workers. Here are the commands to follow in your terminal:
+
+**Note for Windows users:** Windows users will need Python 3.7 and above and to set the following environmental variable prior to launching the worker.
+
+```
+PYTHONUTF8=1
+```
+
+#### Launch the controller
 ```bash
 python3 -m fastchat.serve.controller
 ```
 
-### Launch a model worker
+This controller manages the distributed workers.
+
+#### Launch the model worker
 ```bash
 python3 -m fastchat.serve.model_worker --model-path /path/to/vicuna/weights
 ```
-Wait until the process finishes loading the model and you see "Uvicorn running on ...".
+Wait until the process finishes loading the model and you see "Uvicorn running on ...". You can launch multiple model workers to serve multiple models concurrently. The model worker will connect to the controller automatically.
 
-### Send a test message
+To ensure that your model worker is connected to your controller properly, send a test message using the following command:
 ```bash
 python3 -m fastchat.serve.test_message --model-name vicuna-13b
 ```
 
-### Launch a gradio web server.
+#### Launch the Gradio web server
 ```bash
 python3 -m fastchat.serve.gradio_web_server
 ```
 
-### You can open your browser and chat with a model now.
+This is the user interface that users will interact with.
+
+By following these steps, you will be able to serve your models using the web UI. You can open your browser and chat with a model now.
+
 
 ## Evaluation
 
 Our AI-enhanced [evaluation](fastchat/eval) pipeline is based on GPT-4. Here are some high-level instructions for using the pipeline:
 
 First, generate answers from different models. Use `qa_baseline_gpt35.py` for ChatGPT, or specify the model checkpoint and run `model_qa.py` for Vicuna and other models.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fschat Version: 0.1.8 Summary: An open platform for
+Metadata-Version: 2.1 Name: fschat Version: 0.1.9 Summary: An open platform for
 training, serving, and evaluating large language model based chatbots. Project-
 URL: Homepage, https://github.com/lm-sys/fastchat Project-URL: Bug Tracker,
 https://github.com/lm-sys/fastchat/issues Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE # FastChat An open platform for training, serving, and evaluating large
 language model based chatbots. ## Release
@@ -15,70 +15,89 @@
 (#install) - [Vicuna Weights](#vicuna-weights) - [Inference with Command Line
 Interface](#inference-with-command-line-interface) - [Serving with Web GUI]
 (#serving-with-web-gui) - [Evaluation](#evaluation) - [Fine-tuning](#fine-
 tuning) ## Install ### Method 1: With pip ```bash # Install FastChat pip3
 install fschat # Install the latest main branch of huggingface/transformers
 pip3 install git+https://github.com/huggingface/transformers ``` ### Method 2:
 From source 1. Clone this repository and navigate to the FastChat folder
-```bash git clone https://github.com/lm-sys/FastChat.git cd FastChat ``` 2.
-Install Package ```bash pip3 install --upgrade pip # enable PEP 660 support
-pip3 install -e . ``` ## Vicuna Weights We release [Vicuna](https://
-vicuna.lmsys.org/) weights as delta weights to comply with the LLaMA model
-license. You can add our delta to the original LLaMA weights to obtain the
-Vicuna weights. Instructions: 1. Get the original LLaMA weights in the
-huggingface format by following the instructions [here](https://huggingface.co/
-docs/transformers/main/model_doc/llama). 2. Use the following scripts to get
-Vicuna weights by applying our delta. They will automatically download delta
-weights from our Hugging Face account. **NOTE**: Our released weights are only
-compatible with the latest main branch of huggingface/transformers. We install
-the correct version of transformers when fastchat is installed. ### Vicuna-13B
-This conversion command needs around 60 GB of CPU RAM. ```bash python3 -
+```bash git clone https://github.com/lm-sys/FastChat.git cd FastChat ``` If you
+are running on Mac: ```bash brew install rust ``` 2. Install Package ```bash
+pip3 install --upgrade pip # enable PEP 660 support pip3 install -e . ``` ##
+Vicuna Weights We release [Vicuna](https://vicuna.lmsys.org/) weights as delta
+weights to comply with the LLaMA model license. You can add our delta to the
+original LLaMA weights to obtain the Vicuna weights. Instructions: 1. Get the
+original LLaMA weights in the huggingface format by following the instructions
+[here](https://huggingface.co/docs/transformers/main/model_doc/llama). 2. Use
+the following scripts to get Vicuna weights by applying our delta. They will
+automatically download delta weights from our Hugging Face [account](https://
+huggingface.co/lmsys). **NOTE**: Our released weights are only compatible with
+the latest main branch of huggingface/transformers. We install the correct
+version of transformers when fastchat is installed. ### Vicuna-13B This
+conversion command needs around 60 GB of CPU RAM. If you do not have enough
+memory, you can create a large swap file that allows the operating system to
+automatically utilize the disk as virtual memory. ```bash python3 -
 m fastchat.model.apply_delta \ --base /path/to/llama-13b \ --target /output/
 path/to/vicuna-13b \ --delta lmsys/vicuna-13b-delta-v0 ``` ### Vicuna-7B This
-conversion command needs around 30 GB of CPU RAM. ```bash python3 -
+conversion command needs around 30 GB of CPU RAM. If you do not have enough
+memory, you can create a large swap file that allows the operating system to
+automatically utilize the disk as virtual memory. ```bash python3 -
 m fastchat.model.apply_delta \ --base /path/to/llama-7b \ --target /output/
 path/to/vicuna-7b \ --delta lmsys/vicuna-7b-delta-v0 ``` ## Inference with
-Command Line Interface ### Single GPU The command below requires around 28GB of
-GPU memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B. ``` python3 -
-m fastchat.serve.cli --model-name /path/to/vicuna/weights ``` ### Multiple GPUs
-If you do not have enough GPU memory, you can use model parallelism to
+Command Line Interface #### Single GPU The command below requires around 28GB
+of GPU memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B. ``` python3
+-m fastchat.serve.cli --model-name /path/to/vicuna/weights ``` #### Multiple
+GPUs If you do not have enough GPU memory, you can use model parallelism to
 aggregate memory from multiple GPUs on the same machine. ``` python3 -
-m fastchat.serve.cli --model-name /path/to/vicuna/weights --num-gpus 2 ``` ###
+m fastchat.serve.cli --model-name /path/to/vicuna/weights --num-gpus 2 ``` ####
 CPU Only This runs on the CPU only and does not require GPU. It requires around
 60GB of CPU memory for Vicuna-13B and around 30GB of CPU memory for Vicuna-7B.
 ``` python3 -m fastchat.serve.cli --model-name /path/to/vicuna/weights --device
-cpu ``` ### Metal Backend (Mac computers with Apple silicon or AMD GPUs) Use `-
--device mps` to enable GPU acceleration on Mac computers and use `--load-8bit`
-to turn on 8-bit compression. ``` python3 -m fastchat.serve.cli --model-name /
-path/to/vicuna/weights --device mps --load-8bit ``` ### Others (Quantization,
-Low-end Devices, and More Platforms) If you do not have enough memory, you can
-enable 8-bit compression by adding `--load-8bit` to commands above. It works
-with CPU, GPU, and Metal. This can reduce the memory usage by around half with
-slightly degraded model quality. ``` python3 -m fastchat.serve.cli --model-name
-/path/to/vicuna/weights --load-8bit ``` Besides, we are actively exploring more
-methods to make the model easier to run on more platforms. Contributions and
-pull requests are welcome. ## Serving with Web GUI ### Launch a controller
-```bash python3 -m fastchat.serve.controller ``` ### Launch a model worker
-```bash python3 -m fastchat.serve.model_worker --model-path /path/to/vicuna/
-weights ``` Wait until the process finishes loading the model and you see
-"Uvicorn running on ...". ### Send a test message ```bash python3 -
-m fastchat.serve.test_message --model-name vicuna-13b ``` ### Launch a gradio
-web server. ```bash python3 -m fastchat.serve.gradio_web_server ``` ### You can
-open your browser and chat with a model now. ## Evaluation Our AI-enhanced
-[evaluation](fastchat/eval) pipeline is based on GPT-4. Here are some high-
-level instructions for using the pipeline: First, generate answers from
-different models. Use `qa_baseline_gpt35.py` for ChatGPT, or specify the model
-checkpoint and run `model_qa.py` for Vicuna and other models. Then, use GPT-
-4 to generate reviews automatically, which can be done manually if the GPT-
-4 API is not available to you. Once you have your evaluation data, visualize
-the results by running `generate_webpage_data_from_table.py`, which generates
-data for a static website. Finally, serve a static website under the `webpage`
-directory. You can simply use `python3 -m http.server` to serve the website
-locally. Besides the evaluation workflow, we also document the data format used
-for evaluation, which is encoded with JSON Lines and includes information on
+cpu ``` #### Metal Backend (Mac Computers with Apple Silicon or AMD GPUs) Use
+`--device mps` to enable GPU acceleration on Mac computers and use `--load-
+8bit` to turn on 8-bit compression. ``` python3 -m fastchat.serve.cli --model-
+name /path/to/vicuna/weights --device mps --load-8bit ``` Vicuna-7B can run on
+a 32GB M1 Macbook with 1 - 2 words / second. #### No Enough Memory or Other
+Platforms If you do not have enough memory, you can enable 8-bit compression by
+adding `--load-8bit` to commands above. This can reduce the memory usage by
+around half with slightly degraded model quality. It is compatible with the
+CPU, GPU, and Metal backend. Vicuna-13B with 8-bit compression can run on a
+single NVIDIA 3090/4090/V100(16GB) GPU. ``` python3 -m fastchat.serve.cli --
+model-name /path/to/vicuna/weights --load-8bit ``` Besides, we are actively
+exploring more methods to make the model easier to run on more platforms.
+Contributions and pull requests are welcome. ## Serving with Web GUI To serve
+using the web UI, you need three main components: web servers that interface
+with users, model workers that host one or more models, and a controller to
+coordinate the webserver and model workers. Here are the commands to follow in
+your terminal: **Note for Windows users:** Windows users will need Python 3.7
+and above and to set the following environmental variable prior to launching
+the worker. ``` PYTHONUTF8=1 ``` #### Launch the controller ```bash python3 -
+m fastchat.serve.controller ``` This controller manages the distributed
+workers. #### Launch the model worker ```bash python3 -
+m fastchat.serve.model_worker --model-path /path/to/vicuna/weights ``` Wait
+until the process finishes loading the model and you see "Uvicorn running on
+...". You can launch multiple model workers to serve multiple models
+concurrently. The model worker will connect to the controller automatically. To
+ensure that your model worker is connected to your controller properly, send a
+test message using the following command: ```bash python3 -
+m fastchat.serve.test_message --model-name vicuna-13b ``` #### Launch the
+Gradio web server ```bash python3 -m fastchat.serve.gradio_web_server ``` This
+is the user interface that users will interact with. By following these steps,
+you will be able to serve your models using the web UI. You can open your
+browser and chat with a model now. ## Evaluation Our AI-enhanced [evaluation]
+(fastchat/eval) pipeline is based on GPT-4. Here are some high-level
+instructions for using the pipeline: First, generate answers from different
+models. Use `qa_baseline_gpt35.py` for ChatGPT, or specify the model checkpoint
+and run `model_qa.py` for Vicuna and other models. Then, use GPT-4 to generate
+reviews automatically, which can be done manually if the GPT-4 API is not
+available to you. Once you have your evaluation data, visualize the results by
+running `generate_webpage_data_from_table.py`, which generates data for a
+static website. Finally, serve a static website under the `webpage` directory.
+You can simply use `python3 -m http.server` to serve the website locally.
+Besides the evaluation workflow, we also document the data format used for
+evaluation, which is encoded with JSON Lines and includes information on
 models, prompts, reviewers, questions, answers, and reviews. You can customize
 the evaluation process or contribute to our project by accessing relevant
 [data](fastchat/eval/table/). Check [evaluation](fastchat/eval) for detailed
 instructions. ## Fine-tuning ### Data Vicuna is created by fine-tuning a LLaMA
 base model using approximately 70K user-shared conversations gathered from
 ShareGPT.com with public APIs. To ensure data quality, we convert the HTML back
 to markdown and filter out some inappropriate or low-quality samples.
```

### Comparing `fschat-0.1.8/fschat.egg-info/SOURCES.txt` & `fschat-0.1.9/fschat.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 fastchat/serve/controller.py
 fastchat/serve/gradio_css.py
 fastchat/serve/gradio_patch.py
 fastchat/serve/gradio_web_server.py
 fastchat/serve/model_worker.py
 fastchat/serve/monkey_patch_non_inplace.py
 fastchat/serve/register_worker.py
+fastchat/serve/serve_chatglm.py
 fastchat/serve/test_message.py
 fastchat/train/llama_flash_attn_monkey_patch.py
 fastchat/train/train.py
 fastchat/train/train_lora.py
 fastchat/train/train_mem.py
 fschat.egg-info/PKG-INFO
 fschat.egg-info/SOURCES.txt
```

### Comparing `fschat-0.1.8/pyproject.toml` & `fschat-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fschat"
-version = "0.1.8"
+version = "0.1.9"
 description = "An open platform for training, serving, and evaluating large language model based chatbots."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
 ]
```

