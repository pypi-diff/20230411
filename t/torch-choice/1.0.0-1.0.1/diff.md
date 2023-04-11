# Comparing `tmp/torch_choice-1.0.0.tar.gz` & `tmp/torch_choice-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_choice-1.0.0.tar", last modified: Sat Apr  8 20:07:23 2023, max compression
+gzip compressed data, was "torch_choice-1.0.1.tar", last modified: Tue Apr 11 02:20:16 2023, max compression
```

## Comparing `torch_choice-1.0.0.tar` & `torch_choice-1.0.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:07:23.225548 torch_choice-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-04-08 20:07:23.225548 torch_choice-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-04-08 20:07:08.000000 torch_choice-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 20:07:23.225548 torch_choice-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-08 20:07:08.000000 torch_choice-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:07:23.221548 torch_choice-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-04-08 20:07:08.000000 torch_choice-1.0.0/tests/test_choice_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-08 20:07:08.000000 torch_choice-1.0.0/tests/test_conditional_logit_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-04-08 20:07:08.000000 torch_choice-1.0.0/tests/test_nested_logit_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:07:23.221548 torch_choice-1.0.0/torch_choice/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-08 20:07:08.000000 torch_choice-1.0.0/torch_choice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:07:23.221548 torch_choice-1.0.0/torch_choice/data/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-08 20:07:08.000000 torch_choice-1.0.0/torch_choice/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22241 2023-04-08 20:07:08.000000 torch_choice-1.0.0/torch_choice/data/choice_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-04-08 20:07:08.000000 torch_choice-1.0.0/torch_choice/data/joint_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-08 20:07:08.000000 torch_choice-1.0.0/torch_choice/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:07:23.221548 torch_choice-1.0.0/torch_choice/model/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-08 20:07:08.000000 torch_choice-1.0.0/torch_choice/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-04-08 20:07:08.000000 torch_choice-1.0.0/torch_choice/model/coefficient.py
--rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-04-08 20:07:08.000000 torch_choice-1.0.0/torch_choice/model/conditional_logit_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-08 20:07:08.000000 torch_choice-1.0.0/torch_choice/model/formula_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    21452 2023-04-08 20:07:08.000000 torch_choice-1.0.0/torch_choice/model/nested_logit_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:07:23.221548 torch_choice-1.0.0/torch_choice/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-08 20:07:08.000000 torch_choice-1.0.0/torch_choice/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22785 2023-04-08 20:07:08.000000 torch_choice-1.0.0/torch_choice/utils/easy_data_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-08 20:07:08.000000 torch_choice-1.0.0/torch_choice/utils/run_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    13678 2023-04-08 20:07:08.000000 torch_choice-1.0.0/torch_choice/utils/run_helper_temp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-04-08 20:07:08.000000 torch_choice-1.0.0/torch_choice/utils/std.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:07:23.221548 torch_choice-1.0.0/torch_choice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-04-08 20:07:23.000000 torch_choice-1.0.0/torch_choice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-08 20:07:23.000000 torch_choice-1.0.0/torch_choice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 20:07:23.000000 torch_choice-1.0.0/torch_choice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-08 20:07:23.000000 torch_choice-1.0.0/torch_choice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:20:16.029373 torch_choice-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-04-11 02:20:16.029373 torch_choice-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10542 2023-04-11 02:20:06.000000 torch_choice-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 02:20:16.029373 torch_choice-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-11 02:20:06.000000 torch_choice-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:20:16.025373 torch_choice-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-04-11 02:20:06.000000 torch_choice-1.0.1/tests/test_choice_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-11 02:20:06.000000 torch_choice-1.0.1/tests/test_conditional_logit_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-04-11 02:20:06.000000 torch_choice-1.0.1/tests/test_nested_logit_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:20:16.025373 torch_choice-1.0.1/torch_choice/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 02:20:06.000000 torch_choice-1.0.1/torch_choice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:20:16.025373 torch_choice-1.0.1/torch_choice/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-11 02:20:06.000000 torch_choice-1.0.1/torch_choice/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22873 2023-04-11 02:20:06.000000 torch_choice-1.0.1/torch_choice/data/choice_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-04-11 02:20:06.000000 torch_choice-1.0.1/torch_choice/data/joint_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-11 02:20:06.000000 torch_choice-1.0.1/torch_choice/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:20:16.025373 torch_choice-1.0.1/torch_choice/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-11 02:20:06.000000 torch_choice-1.0.1/torch_choice/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-04-11 02:20:06.000000 torch_choice-1.0.1/torch_choice/model/coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17035 2023-04-11 02:20:06.000000 torch_choice-1.0.1/torch_choice/model/conditional_logit_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-11 02:20:06.000000 torch_choice-1.0.1/torch_choice/model/formula_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23065 2023-04-11 02:20:06.000000 torch_choice-1.0.1/torch_choice/model/nested_logit_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:20:16.029373 torch_choice-1.0.1/torch_choice/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-11 02:20:06.000000 torch_choice-1.0.1/torch_choice/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22785 2023-04-11 02:20:06.000000 torch_choice-1.0.1/torch_choice/utils/easy_data_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-11 02:20:06.000000 torch_choice-1.0.1/torch_choice/utils/run_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13678 2023-04-11 02:20:06.000000 torch_choice-1.0.1/torch_choice/utils/run_helper_temp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-04-11 02:20:06.000000 torch_choice-1.0.1/torch_choice/utils/std.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:20:16.025373 torch_choice-1.0.1/torch_choice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-04-11 02:20:16.000000 torch_choice-1.0.1/torch_choice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-11 02:20:16.000000 torch_choice-1.0.1/torch_choice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 02:20:16.000000 torch_choice-1.0.1/torch_choice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-11 02:20:16.000000 torch_choice-1.0.1/torch_choice.egg-info/top_level.txt
```

### Comparing `torch_choice-1.0.0/PKG-INFO` & `torch_choice-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,14 @@
-Metadata-Version: 2.1
-Name: torch_choice
-Version: 1.0.0
-Summary: A Pytorch Backend Library for Choice Modelling
-Home-page: 
-Author: Tianyu Du
-Author-email: tianyudu@stanford.edu
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-
 # torch-choice
 
 > Authors: Tianyu Du, Ayush Kanodia and Susan Athey; Contact: tianyudu@stanford.edu
 
+**Note on Installation**: This is a work in progress. We recommend installing the package from source to get the latest version and bug-fix patches.
+We are actively working on this package and will be adding more features and examples. Please feel free to reach out to us with any questions or suggestions.
+
 > Acknowledgements: We would like to thank Erik Sverdrup, Charles Pebereau and Keshav Agrawal for their feedback.
 
 `torch-choice` is a library for flexible, fast choice modeling with PyTorch: it has logit and nested logit models, designed for both estimation and prediction. See the [complete documentation](https://gsbdbi.github.io/torch-choice/) for more details.
 Unique features:
 1. GPU support via torch for speed
 2. Specify customized models
 3. Specify availability sets
```

### Comparing `torch_choice-1.0.0/README.md` & `torch_choice-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,27 @@
+Metadata-Version: 2.1
+Name: torch_choice
+Version: 1.0.1
+Summary: A Pytorch Backend Library for Choice Modelling
+Home-page: 
+Author: Tianyu Du
+Author-email: tianyudu@stanford.edu
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
+
 # torch-choice
 
 > Authors: Tianyu Du, Ayush Kanodia and Susan Athey; Contact: tianyudu@stanford.edu
 
+**Note on Installation**: This is a work in progress. We recommend installing the package from source to get the latest version and bug-fix patches.
+We are actively working on this package and will be adding more features and examples. Please feel free to reach out to us with any questions or suggestions.
+
 > Acknowledgements: We would like to thank Erik Sverdrup, Charles Pebereau and Keshav Agrawal for their feedback.
 
 `torch-choice` is a library for flexible, fast choice modeling with PyTorch: it has logit and nested logit models, designed for both estimation and prediction. See the [complete documentation](https://gsbdbi.github.io/torch-choice/) for more details.
 Unique features:
 1. GPU support via torch for speed
 2. Specify customized models
 3. Specify availability sets
```

### Comparing `torch_choice-1.0.0/setup.py` & `torch_choice-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="torch_choice",
-    version="1.0.0",
+    version="1.0.1",
     description="A Pytorch Backend Library for Choice Modelling",
     long_description=README,
     long_description_content_type="text/markdown",
     url="",
     author="Tianyu Du",
     author_email="tianyudu@stanford.edu",
     license="MIT",
```

### Comparing `torch_choice-1.0.0/tests/test_choice_dataset.py` & `torch_choice-1.0.1/tests/test_choice_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.0/tests/test_conditional_logit_model.py` & `torch_choice-1.0.1/tests/test_conditional_logit_model.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.0/tests/test_nested_logit_model.py` & `torch_choice-1.0.1/tests/test_nested_logit_model.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.0/torch_choice/data/choice_dataset.py` & `torch_choice-1.0.1/torch_choice/data/choice_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import torch
 
 
 class ChoiceDataset(torch.utils.data.Dataset):
     def __init__(self,
                  item_index: torch.LongTensor,
                  num_items: int = None,
+                 num_users: int = None,
                  label: Optional[torch.LongTensor] = None,
                  user_index: Optional[torch.LongTensor] = None,
                  session_index: Optional[torch.LongTensor] = None,
                  item_availability: Optional[torch.BoolTensor] = None,
                  **kwargs) -> None:
         """
         Initialization methods for the dataset object, researchers should supply all information about the dataset
@@ -38,14 +39,18 @@
         Args:
             item_index (torch.LongTensor): a tensor of shape (batch_size) indicating the relevant item in each row
                 of the dataset, the relevant item can be:
                 (1) the item bought in this choice instance,
                 (2) or the item reviewed by the user. In the later case, we need the `label` tensor to specify the rating score.
                 NOTE: The support for second case is under-development, currently, we are only supporting binary label.
 
+            num_items (Optional[int]): the number of items in the dataset. If `None` is provided (default), the number of items will be inferred from the number of unique numbers in `item_index`.
+
+            num_users (Optional[int]): the number of users in the dataset. If `None` is provided (default), the number of users will be inferred from the number of unique numbers in `user_index`.
+
             label (Optional[torch.LongTensor], optional): a tensor of shape (batch_size) indicating the label for prediction in
                 each choice instance. While you want to predict the item bought, you can leave the `label` argument
                 as `None` in the initialization method, and the model will use `item_index` as the object to be predicted.
                 But if you are, for example, predicting the rating an user gave an item, label must be provided.
                 Defaults to None.
 
             user_index (Optional[torch.LongTensor], optional): a tensor of shape num_purchases (batch_size) indicating
@@ -86,18 +91,17 @@
             6. itemsession observables starting with `itemsession_`, this is a more intuitive alias to the price
                 observable.
         """
         # ENHANCEMENT(Tianyu): add item_names for summary.
         super(ChoiceDataset, self).__init__()
         self.label = label
         self.item_index = item_index
-        if num_items is not None:
-            self.provided_num_items = num_items
-        else:
-            self.provided_num_items = None
+        self._num_items = num_items
+        self._num_users = num_users
+
         self.user_index = user_index
         self.session_index = session_index
 
         if self.session_index is None:
             # if any([x.startswith('session_') or x.startswith('price_') for x in kwargs.keys()]):
             # if any session sensitive observable is provided, but session index is not,
             # infer each row in the dataset to be a session.
@@ -185,16 +189,18 @@
     @property
     def num_users(self) -> int:
         """Returns number of users involved in this dataset, returns 1 if there is no user identity.
 
         Returns:
             int: the number of users involved in this dataset.
         """
-        # query from user_index
-        if self.user_index is not None:
+        if self._num_users is not None:
+            return self._num_users
+        elif self.user_index is not None:
+            # infer from the number of unique items in  user_index.
             return len(torch.unique(self.user_index))
         else:
             return 1
 
         # for key, val in self.__dict__.items():
         #     if torch.is_tensor(val):
         #         if self._is_user_attribute(key) or self._is_taste_attribute(key):
@@ -204,19 +210,20 @@
     @property
     def num_items(self) -> int:
         """Returns the number of items involved in this dataset.
 
         Returns:
             int: the number of items involved in this dataset.
         """
-        if self.provided_num_items is None:
+        if self._num_items is not None:
+            # return the _num_items provided in the constructor.
+            return self._num_items
+        else:
             # infer the number of items from item_index.
             return len(torch.unique(self.item_index))
-        else:
-            return self.provided_num_items
 
         # for key, val in self.__dict__.items():
         #     if torch.is_tensor(val):
         #         if self._is_item_attribute(key):
         #             return val.shape[0]
         #         elif self._is_taste_attribute(key) or self._is_price_attribute(key):
         #             return val.shape[1]
@@ -350,16 +357,16 @@
 
     def __repr__(self) -> str:
         """A method to get a string representation of the dataset.
 
         Returns:
             str: the string representation of the dataset.
         """
-        info = [
-            f'{key}={self._size_repr(item)}' for key, item in self.__dict__.items()]
+        # don't print shapes of internal attributes like _num_users and _num_items.
+        info = [f'{key}={self._size_repr(item)}' for key, item in self.__dict__.items() if not key.startswith('_')]
         return f"{self.__class__.__name__}({', '.join(info)}, device={self.device})"
 
     # ==================================================================================================================
     # methods for checking attribute categories.
     # ==================================================================================================================
     @staticmethod
     def _is_item_attribute(key: str) -> bool:
```

### Comparing `torch_choice-1.0.0/torch_choice/data/joint_dataset.py` & `torch_choice-1.0.1/torch_choice/data/joint_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.0/torch_choice/data/utils.py` & `torch_choice-1.0.1/torch_choice/data/utils.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.0/torch_choice/model/coefficient.py` & `torch_choice-1.0.1/torch_choice/model/coefficient.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.0/torch_choice/model/conditional_logit_model.py` & `torch_choice-1.0.1/torch_choice/model/nested_logit_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,368 +1,425 @@
 """
-Conditional Logit Model.
+Implementation of the nested logit model, see page 86 of the book
+"discrete choice methods with simulation" by Train. for more details.
 
 Author: Tianyu Du
-Date: Aug. 8, 2021
-Update: Apr. 28, 2022
+Update; Apr. 7, 2023
 """
-import warnings
-from copy import deepcopy
-from typing import Dict, Optional, Tuple, Union
+from typing import Dict, List, Optional
 
 import torch
 import torch.nn as nn
-import torch.nn.functional as F
 
 from torch_choice.data.choice_dataset import ChoiceDataset
+from torch_choice.data.joint_dataset import JointDataset
 from torch_choice.model.coefficient import Coefficient
 from torch_choice.model.formula_parser import parse_formula
 
 
-class ConditionalLogitModel(nn.Module):
-    """The more generalized version of conditional logit model, the model allows for research specific
-    variable types(groups) and different levels of variations for coefficient.
-
-    The model allows for the following levels for variable variations:
-    NOTE: unless the `-full` flag is specified (which means we want to explicitly model coefficients
-        for all items), for all variation levels related to item (item specific and user-item specific),
-        the model force coefficients for the first item to be zero. This design follows standard
-        econometric practice.
-
-    - constant: constant over all users and items,
-
-    - user: user-specific parameters but constant across all items,
-
-    - item: item-specific parameters but constant across all users, parameters for the first item are
-        forced to be zero.
-    - item-full: item-specific parameters but constant across all users, explicitly model for all items.
-
-    - user-item: parameters that are specific to both user and item, parameter for the first item
-        for all users are forced to be zero.
-    - user-item-full: parameters that are specific to both user and item, explicitly model for all items.
-    """
-
+class NestedLogitModel(nn.Module):
     def __init__(self,
-                 formula: Optional[str]=None,
-                 dataset: Optional[ChoiceDataset]=None,
-                 coef_variation_dict: Optional[Dict[str, str]]=None,
-                 num_param_dict: Optional[Dict[str, int]]=None,
-                 num_items: Optional[int]=None,
+                 nest_to_item: Dict[object, List[int]],
+                 # method 1: specify variation and num param. dictionary.
+                 nest_coef_variation_dict: Optional[Dict[str, str]]=None,
+                 nest_num_param_dict: Optional[Dict[str, int]]=None,
+                 item_coef_variation_dict: Optional[Dict[str, str]]=None,
+                 item_num_param_dict: Optional[Dict[str, int]]=None,
+                 # method 2: specify formula and dataset.
+                 item_formula: Optional[str]=None,
+                 nest_formula: Optional[str]=None,
+                 dataset: Optional[JointDataset]=None,
                  num_users: Optional[int]=None,
+                 shared_lambda: bool=False,
                  regularization: Optional[str]=None,
                  regularization_weight: Optional[float]=None
                  ) -> None:
-        """
+        """Initialization method of the nested logit model.
+
         Args:
-            formula (str): a string representing the utility formula.
+            nest_to_item (Dict[object, List[int]]): a dictionary maps a nest ID to a list
+                of items IDs of the queried nest.
+
+            nest_coef_variation_dict (Dict[str, str]): a dictionary maps a variable type
+                (i.e., variable group) to the level of variation for the coefficient of this type
+                of variables.
+            nest_num_param_dict (Dict[str, int]): a dictionary maps a variable type name to
+                the number of parameters in this variable group.
+
+            item_coef_variation_dict (Dict[str, str]): the same as nest_coef_variation_dict but
+                for item features.
+            item_num_param_dict (Dict[str, int]): the same as nest_num_param_dict but for item
+                features.
+
+            {nest, item}_formula (str): a string representing the utility formula for the {nest, item} level logit model.
                 The formula consists of '(variable_name|variation)'s separated by '+', for example:
                 "(var1|item) + (var2|user) + (var3|constant)"
                 where the first part of each term is the name of the variable
                 and the second part is the variation of the coefficient.
                 The variation can be one of the following:
                 'constant', 'item', 'item-full', 'user', 'user-item', 'user-item-full'.
                 All spaces in the formula will be ignored, hence please do not use spaces in variable/observable names.
-            data (ChoiceDataset): a ChoiceDataset object for training the model, the parser will infer dimensions of variables
-                and sizes of coefficients from the ChoiceDataset.
-            coef_variation_dict (Dict[str, str]): variable type to variation level dictionary. Keys of this dictionary
-                should be variable names in the dataset (i.e., these starting with `itemsession_`, `price_`, `user_`, etc), or `intercept`
-                if the researcher requires an intercept term.
-                For each variable name X_var (e.g., `user_income`) or `intercept`, the corresponding dictionary key should
-                be one of the following values, this value specifies the "level of variation" of the coefficient.
-
-                - `constant`: the coefficient constant over all users and items: $X \beta$.
-
-                - `user`: user-specific parameters but constant across all items: $X \beta_{u}$.
-
-                - `item`: item-specific parameters but constant across all users, $X \beta_{i}$.
-                    Note that the coefficients for the first item are forced to be zero following the standard practice
-                    in econometrics.
-
-                - `item-full`: the same configuration as `item`, but does not force the coefficients of the first item to
-                    be zeros.
-
-                The following configurations are supported by the package, but we don't recommend using them due to the
-                    large number of parameters.
-                - `user-item`: parameters that are specific to both user and item, parameter for the first item
-                    for all users are forced to be zero.
-
-                - `user-item-full`: parameters that are specific to both user and item, explicitly model for all items.
-            num_param_dict (Optional[Dict[str, int]]): variable type to number of parameters dictionary with keys exactly the same
-                as the `coef_variation_dict`. Values of `num_param_dict` records numbers of features in each kind of variable.
-                If None is supplied, num_param_dict will be a dictionary with the same keys as the `coef_variation_dict` dictionary
-                and values of all ones. Default to be None.
-            num_items (int): number of items in the dataset.
-            num_users (int): number of users in the dataset.
+            dataset (JointDataset): a JointDataset object for training the model, the parser will infer dimensions of variables
+                and sizes of coefficients for the nest level model from dataset.datasets['nest']. The parser will infer dimensions of variables and sizes of coefficients for the item level model from dataset.datasets['item'].
+
+            num_users (Optional[int], optional): number of users to be modelled, this is only
+                required if any of variable type requires user-specific variations.
+                Defaults to None.
+
+            shared_lambda (bool): a boolean indicating whether to enforce the elasticity lambda, which
+                is the coefficient for inclusive values, to be constant for all nests.
+                The lambda enters the nest-level selection as the following
+                Utility of choosing nest k = lambda * inclusive value of nest k
+                                               + linear combination of some other nest level features
+                If set to True, a single lambda will be learned for all nests, otherwise, the
+                model learns an individual lambda for each nest.
+                Defaults to False.
+
             regularization (Optional[str]): this argument takes values from {'L1', 'L2', None}, which specifies the type of
                 regularization added to the log-likelihood.
                 - 'L1' will subtract regularization_weight * 1-norm of parameters from the log-likelihood.
                 - 'L2' will subtract regularization_weight * 2-norm of parameters from the log-likelihood.
                 - None does not modify the log-likelihood.
                 Defaults to None.
+
             regularization_weight (Optional[float]): the weight of parameter norm subtracted from the log-likelihood.
                 This term controls the strength of regularization. This argument is required if and only if regularization
                 is not None.
                 Defaults to None.
         """
-        if coef_variation_dict is None and formula is None:
-            raise ValueError("Either coef_variation_dict or formula should be provided to specify the model.")
-
-        if (coef_variation_dict is not None) and (formula is not None):
-            raise ValueError("Only one of coef_variation_dict or formula should be provided to specify the model.")
-
-        if (formula is not None) and (dataset is None):
-            raise ValueError("If formula is provided, data should be provided to specify the model.")
-
-        # Use the formula to infer model, override dictionaries.
-        if formula is not None:
-            coef_variation_dict, num_param_dict = parse_formula(formula, dataset)
-
-        super(ConditionalLogitModel, self).__init__()
-
-        if num_param_dict is None:
-            num_param_dict = {key:1 for key in coef_variation_dict.keys()}
+        # handle nest level model.
+        using_formula_to_initiate = (item_formula is not None) and (nest_formula is not None)
+        if using_formula_to_initiate:
+            # make sure that the research does not specify duplicated information, which might cause conflict.
+            if (nest_coef_variation_dict is not None) or (item_coef_variation_dict is not None):
+                raise ValueError('You specify the {item, nest}_formula to initiate the model, you should not specify the {item, nest}_coef_variation_dict at the same time.')
+            if (nest_num_param_dict is not None) or (item_num_param_dict is not None):
+                raise ValueError('You specify the {item, nest}_formula to initiate the model, you should not specify the {item, nest}_num_param_dict at the same time.')
+            if dataset is None:
+                raise ValueError('Dataset is required if {item, nest}_formula is specified to initiate the model.')
 
-        assert coef_variation_dict.keys() == num_param_dict.keys()
+            nest_coef_variation_dict, nest_num_param_dict = parse_formula(nest_formula, dataset.datasets['nest'])
+            item_coef_variation_dict, item_num_param_dict = parse_formula(item_formula, dataset.datasets['item'])
 
-        self.variable_types = list(deepcopy(num_param_dict).keys())
-
-        self.coef_variation_dict = deepcopy(coef_variation_dict)
-        self.num_param_dict = deepcopy(num_param_dict)
-
-        self.num_items = num_items
+        else:
+            # check for conflicting information.
+            if (nest_formula is not None) or (item_formula is not None):
+                raise ValueError('You should not specify {item, nest}_formula and {item, nest}_coef_variation_dict at the same time.')
+            # make sure that the research specifies all the required information.
+            if (nest_coef_variation_dict is None) or (item_coef_variation_dict is None):
+                raise ValueError('You should specify the {item, nest}_coef_variation_dict to initiate the model.')
+            if (nest_num_param_dict is None) or (item_num_param_dict is None):
+                raise ValueError('You should specify the {item, nest}_num_param_dict to initiate the model.')
+
+        super(NestedLogitModel, self).__init__()
+        self.nest_to_item = nest_to_item
+        self.nest_coef_variation_dict = nest_coef_variation_dict
+        self.nest_num_param_dict = nest_num_param_dict
+        self.item_coef_variation_dict = item_coef_variation_dict
+        self.item_num_param_dict = item_num_param_dict
         self.num_users = num_users
 
+        self.nests = list(nest_to_item.keys())
+        self.num_nests = len(self.nests)
+        self.num_items = sum(len(items) for items in nest_to_item.values())
+
+        # nest coefficients.
+        self.nest_coef_dict = self._build_coef_dict(self.nest_coef_variation_dict,
+                                                    self.nest_num_param_dict,
+                                                    self.num_nests)
+
+        # item coefficients.
+        self.item_coef_dict = self._build_coef_dict(self.item_coef_variation_dict,
+                                                    self.item_num_param_dict,
+                                                    self.num_items)
+
+        self.shared_lambda = shared_lambda
+        if self.shared_lambda:
+            self.lambda_weight = nn.Parameter(torch.ones(1), requires_grad=True)
+        else:
+            self.lambda_weight = nn.Parameter(torch.ones(self.num_nests) / 2, requires_grad=True)
+        # breakpoint()
+        # self.iv_weights = nn.Parameter(torch.ones(1), requires_grad=True)
+        # used to warn users if forgot to call clamp.
+        self._clamp_called_flag = True
+
         self.regularization = regularization
         assert self.regularization in ['L1', 'L2', None], f"Provided regularization={self.regularization} is not allowed, allowed values are ['L1', 'L2', None]."
         self.regularization_weight = regularization_weight
         if (self.regularization is not None) and (self.regularization_weight is None):
             raise ValueError(f'You specified regularization type {self.regularization} without providing regularization_weight.')
         if (self.regularization is None) and (self.regularization_weight is not None):
             raise ValueError(f'You specified no regularization but you provide regularization_weight={self.regularization_weight}, you should leave regularization_weight as None if you do not want to regularize the model.')
 
-        # check number of parameters specified are all positive.
-        for var_type, num_params in self.num_param_dict.items():
-            assert num_params > 0, f'num_params needs to be positive, got: {num_params}.'
-
-        # infer the number of parameters for intercept if the researcher forgets.
-        if 'intercept' in self.coef_variation_dict.keys() and 'intercept' not in self.num_param_dict.keys():
-            warnings.warn("'intercept' key found in coef_variation_dict but not in num_param_dict, num_param_dict['intercept'] has been set to 1.")
-            self.num_param_dict['intercept'] = 1
-
-        # construct trainable parameters.
-        coef_dict = dict()
-        for var_type, variation in self.coef_variation_dict.items():
-            coef_dict[var_type] = Coefficient(variation=variation,
-                                              num_items=self.num_items,
-                                              num_users=self.num_users,
-                                              num_params=self.num_param_dict[var_type])
-        # A ModuleDict is required to properly register all trainable parameters.
-        # self.parameter() will fail if a python dictionary is used instead.
-        self.coef_dict = nn.ModuleDict(coef_dict)
-
-    def __repr__(self) -> str:
-        """Return a string representation of the model.
-
-        Returns:
-            str: the string representation of the model.
-        """
-        out_str_lst = ['Conditional logistic discrete choice model, expects input features:\n']
-        for var_type, num_params in self.num_param_dict.items():
-            out_str_lst.append(f'X[{var_type}] with {num_params} parameters, with {self.coef_variation_dict[var_type]} level variation.')
-        return super().__repr__() + '\n' + '\n'.join(out_str_lst) + '\n' + f'device={self.device}'
-
     @property
     def num_params(self) -> int:
         """Get the total number of parameters. For example, if there is only an user-specific coefficient to be multiplied
         with the K-dimensional observable, then the total number of parameters would be K x number of users, assuming no
         intercept is involved.
 
         Returns:
             int: the total number of learnable parameters.
         """
         return sum(w.numel() for w in self.parameters())
 
-    def summary(self):
-        """Print out the current model parameter."""
-        for var_type, coefficient in self.coef_dict.items():
-            if coefficient is not None:
-                print('Variable Type: ', var_type)
-                print(coefficient.coef)
-
-    def forward(self,
-                batch: ChoiceDataset,
-                manual_coef_value_dict: Optional[Dict[str, torch.Tensor]] = None
-                ) -> torch.Tensor:
-        """
-        Forward pass of the model.
+    def _build_coef_dict(self,
+                         coef_variation_dict: Dict[str, str],
+                         num_param_dict: Dict[str, int],
+                         num_items: int) -> nn.ModuleDict:
+        """Builds a coefficient dictionary containing all trainable components of the model, mapping coefficient names
+            to the corresponding Coefficient Module.
+            num_items could be the actual number of items or the number of nests depends on the use case.
+            NOTE: torch-choice users don't directly interact with this method.
 
         Args:
-            batch: a `ChoiceDataset` object.
+            coef_variation_dict (Dict[str, str]): a dictionary mapping coefficient names (e.g., theta_user) to the level
+                of variation (e.g., 'user').
+            num_param_dict (Dict[str, int]): a dictionary mapping coefficient names to the number of parameters in this
+                coefficient. Be aware that, for example, if there is one K-dimensional coefficient for every user, then
+                the `num_param` should be K instead of K x number of users.
+            num_items (int): the total number of items in the prediction problem. `num_items` should be the number of nests if _build_coef_dict() is used for nest-level prediction.
 
-            manual_coef_value_dict (Optional[Dict[str, torch.Tensor]], optional): a dictionary with
-                keys in {'u', 'i'} etc and tensors as values. If provided, the model will force
-                coefficient to be the provided values and compute utility conditioned on the provided
-                coefficient values. This feature is useful when the research wishes to plug in particular
-                values of coefficients and examine the utility values. If not provided, the model will
-                use the learned coefficient values in self.coef_dict.
-                Defaults to None.
+        Returns:
+            nn.ModuleDict: a PyTorch ModuleDict object mapping from coefficient names to training Coefficient.
+        """
+        coef_dict = dict()
+        for var_type, variation in coef_variation_dict.items():
+            num_params = num_param_dict[var_type]
+            coef_dict[var_type] = Coefficient(variation=variation,
+                                              num_items=num_items,
+                                              num_users=self.num_users,
+                                              num_params=num_params)
+        return nn.ModuleDict(coef_dict)
+
+
+    def forward(self, batch: ChoiceDataset) -> torch.Tensor:
+        """An standard forward method for the model, the user feeds a ChoiceDataset batch and the model returns the
+            predicted log-likelihood tensor. The main forward passing happens in the _forward() method, but we provide
+            this wrapper forward() method for a cleaner API, as forward() only requires a single batch argument.
+            For more details about the forward passing, please refer to the _forward() method.
+
+        # TODO: the ConditionaLogitModel returns predicted utility, the NestedLogitModel behaves the same?
+
+        Args:
+            batch (ChoiceDataset): a ChoiceDataset object containing the data batch.
 
         Returns:
-            torch.Tensor: a tensor of shape (num_trips, num_items) whose (t, i) entry represents
-                the utility from item i in trip t for the user involved in that trip.
+            torch.Tensor: a tensor of shape (num_trips, num_items) including the log probability
+            of choosing item i in trip t.
         """
-        x_dict = batch.x_dict
+        return self._forward(batch['nest'].x_dict,
+                             batch['item'].x_dict,
+                             batch['item'].user_index,
+                             batch['item'].item_availability)
+
+    def _forward(self,
+                 nest_x_dict: Dict[str, torch.Tensor],
+                 item_x_dict: Dict[str, torch.Tensor],
+                 user_index: Optional[torch.LongTensor] = None,
+                 item_availability: Optional[torch.BoolTensor] = None
+                 ) -> torch.Tensor:
+        """"Computes log P[t, i] = the log probability for the user involved in trip t to choose item i.
+        Let n denote the ID of the user involved in trip t, then P[t, i] = P_{ni} on page 86 of the
+        book "discrete choice methods with simulation" by Train.
 
-        if 'intercept' in self.coef_variation_dict.keys():
-            # intercept term has no input tensor, which has only 1 feature.
-            x_dict['intercept'] = torch.ones((len(batch), self.num_items, 1), device=batch.device)
+        The `_forward` method is an internal API, users should refer to the `forward` method.
 
-        # compute the utility from each item in each choice session.
-        total_utility = torch.zeros((len(batch), self.num_items), device=batch.device)
-        # for each type of variables, apply the corresponding coefficient to input x.
+        Args:
+            nest_x_dict (torch.Tensor): a dictionary mapping from nest-level feature names to the corresponding feature tensor.
 
-        for var_type, coef in self.coef_dict.items():
-            total_utility += coef(
-                x_dict[var_type], batch.user_index,
-                manual_coef_value=None if manual_coef_value_dict is None else manual_coef_value_dict[var_type])
+            item_x_dict (torch.Tensor): a dictionary mapping from item-level feature names to the corresponding feature tensor.
 
-        assert total_utility.shape == (len(batch), self.num_items)
+                More details on the shape of the tensors can be found in the docstring of the `x_dict` method of `ChoiceDataset`.
 
-        if batch.item_availability is not None:
+            user_index (torch.LongTensor): a tensor of shape (num_trips,) indicating which user is
+                making decision in each trip. Setting user_index = None assumes the same user is
+                making decisions in all trips.
+            item_availability (torch.BoolTensor): a boolean tensor with shape (num_trips, num_items)
+                indicating the aviliability of items in each trip. If item_availability[t, i] = False,
+                the utility of choosing item i in trip t, V[t, i], will be set to -inf.
+                Given the decomposition V[t, i] = W[t, k(i)] + Y[t, i] + eps, V[t, i] is set to -inf
+                by setting Y[t, i] = -inf for unavilable items.
+
+        Returns:
+            torch.Tensor: a tensor of shape (num_trips, num_items) including the log probability
+            of choosing item i in trip t.
+        """
+        if self.shared_lambda:
+            self.lambdas = self.lambda_weight.expand(self.num_nests)
+        else:
+            self.lambdas = self.lambda_weight
+
+        # if not self._clamp_called_flag:
+        #     warnings.warn('Did you forget to call clamp_lambdas() after optimizer.step()?')
+
+        # The overall utility of item can be decomposed into V[item] = W[nest] + Y[item] + eps.
+        T = list(item_x_dict.values())[0].shape[0]
+        device = list(item_x_dict.values())[0].device
+        # compute nest-specific utility with shape (T, num_nests).
+        W = torch.zeros(T, self.num_nests).to(device)
+
+        for variable in self.nest_coef_variation_dict.keys():
+            if self.is_intercept_term(variable):
+                nest_x_dict['intercept'] = torch.ones((T, self.num_nests, 1)).to(device)
+                break
+
+        for variable in self.item_coef_variation_dict.keys():
+            if self.is_intercept_term(variable):
+                item_x_dict['intercept'] = torch.ones((T, self.num_items, 1)).to(device)
+                break
+
+        for var_type, coef in self.nest_coef_dict.items():
+            corresponding_observable = var_type.split("[")[0]
+            W += coef(nest_x_dict[corresponding_observable], user_index)
+
+        # compute item-specific utility (T, num_items).
+        Y = torch.zeros(T, self.num_items).to(device)
+        for var_type, coef in self.item_coef_dict.items():
+            corresponding_observable = var_type.split("[")[0]
+            Y += coef(item_x_dict[corresponding_observable], user_index)
+
+        if item_availability is not None:
+            Y[~item_availability] =torch.finfo(Y.dtype).min / 2
+
+        # =============================================================================
+        # compute the inclusive value of each nest.
+        inclusive_value = dict()
+        for k, Bk in self.nest_to_item.items():
+            # for nest k, divide the Y of all items in Bk by lambda_k.
+            Y[:, Bk] /= self.lambdas[k]
+            # compute inclusive value for nest k.
             # mask out unavilable items.
-            total_utility[~batch.item_availability[batch.session_index, :]] = torch.finfo(total_utility.dtype).min / 2
-        return total_utility
+            inclusive_value[k] = torch.logsumexp(Y[:, Bk], dim=1, keepdim=False)  # (T,)
+        # boardcast inclusive value from (T, num_nests) to (T, num_items).
+        # for trip t, I[t, i] is the inclusive value of the nest item i belongs to.
+        I = torch.zeros(T, self.num_items).to(device)
+        for k, Bk in self.nest_to_item.items():
+            I[:, Bk] = inclusive_value[k].view(-1, 1)  # (T, |Bk|)
+
+        # logP_item[t, i] = log P(ni|Bk), where Bk is the nest item i is in, n is the user in trip t.
+        logP_item = Y - I  # (T, num_items)
+
+        # =============================================================================
+        # logP_nest[t, i] = log P(Bk), for item i in trip t, the probability of choosing the nest/bucket
+        # item i belongs to. logP_nest has shape (T, num_items)
+        # logit[t, i] = W[n, k] + lambda[k] I[n, k], where n is the user involved in trip t, k is
+        # the nest item i belongs to.
+        logit = torch.zeros(T, self.num_items).to(device)
+        for k, Bk in self.nest_to_item.items():
+            logit[:, Bk] = (W[:, k] + self.lambdas[k] * inclusive_value[k]).view(-1, 1)  # (T, |Bk|)
+        # only count each nest once in the logsumexp within the nest level model.
+        cols = [x[0] for x in self.nest_to_item.values()]
+        logP_nest = logit - torch.logsumexp(logit[:, cols], dim=1, keepdim=True)
+
+        # =============================================================================
+        # compute the joint log P_{ni} as in the textbook.
+        logP = logP_item + logP_nest
+        self._clamp_called_flag = False
+        return logP
 
+    def log_likelihood(self, *args):
+        """Computes the log likelihood of the model, please refer to the negative_log_likelihood() method.
 
-    def negative_log_likelihood(self, batch: ChoiceDataset, y: torch.Tensor, is_train: bool=True) -> torch.Tensor:
-        """Computes the log-likelihood for the batch and label.
-        TODO: consider remove y, change to label.
-        TODO: consider move this method outside the model, the role of the model is to compute the utility.
+        Returns:
+            _type_: the log likelihood of the model.
+        """
+        return - self.negative_log_likelihood(*args)
+
+    def negative_log_likelihood(self,
+                                batch: ChoiceDataset,
+                                y: torch.LongTensor,
+                                is_train: bool=True) -> torch.scalar_tensor:
+        """Computes the negative log likelihood of the model. Please note the log-likelihood is summed over all samples
+            in batch instead of the average.
 
         Args:
-            batch (ChoiceDataset): a ChoiceDataset object containing the data.
-            y (torch.Tensor): the label.
-            is_train (bool, optional): whether to trace the gradient. Defaults to True.
+            batch (ChoiceDataset): the ChoiceDataset object containing the data.
+            y (torch.LongTensor): the label.
+            is_train (bool, optional): which mode of the model to be used for the forward passing, if we need Hessian
+                of the NLL through auto-grad, `is_train` should be set to True. If we merely need a performance metric,
+                then `is_train` can be set to False for better performance.
+                Defaults to True.
 
         Returns:
-            torch.Tensor: the negative log-likelihood.
+            torch.scalar_tensor: the negative log likelihood of the model.
         """
+        # compute the negative log-likelihood loss directly.
         if is_train:
             self.train()
         else:
             self.eval()
         # (num_trips, num_items)
-        total_utility = self.forward(batch)
-        logP = torch.log_softmax(total_utility, dim=1)
+        logP = self.forward(batch)
         nll = - logP[torch.arange(len(y)), y].sum()
         return nll
 
     def loss(self, *args, **kwargs):
         """The loss function to be optimized. This is a wrapper of `negative_log_likelihood` + regularization loss if required."""
         nll = self.negative_log_likelihood(*args, **kwargs)
         if self.regularization is not None:
             L = {'L1': 1, 'L2': 2}[self.regularization]
-            for param in self.parameters():
+            for name, param in self.named_parameters():
+                if name == 'lambda_weight':
+                    # we don't regularize the lambda term, we only regularize coefficients.
+                    continue
                 nll += self.regularization_weight * torch.norm(param, p=L)
         return nll
 
     @property
     def device(self) -> torch.device:
         """Returns the device of the coefficient.
 
         Returns:
             torch.device: the device of the model.
         """
-        return next(iter(self.coef_dict.values())).device
+        return next(iter(self.item_coef_dict.values())).device
 
-    # NOTE: the method for computing Hessian and standard deviation has been moved to std.py.
-    # @staticmethod
-    # def flatten_coef_dict(coef_dict: Dict[str, Union[torch.Tensor, torch.nn.Parameter]]) -> Tuple[torch.Tensor, dict]:
-    #     """Flattens the coef_dict into a 1-dimension tensor, used for hessian computation.
+    @staticmethod
+    def is_intercept_term(variable: str):
+        # check if the given variable is an intercept (fixed effect) term.
+        # intercept (fixed effect) terms are defined as 'intercept[*]' and looks like 'intercept[user]', 'intercept[item]', etc.
+        return (variable.startswith('intercept[') and variable.endswith(']'))
 
-    #     Args:
-    #         coef_dict (Dict[str, Union[torch.Tensor, torch.nn.Parameter]]): a dictionary holding learnable parameters.
+    def get_coefficient(self, variable: str, level: Optional[str] = None) -> torch.Tensor:
+        """Retrieve the coefficient tensor for the given variable.
 
-    #     Returns:
-    #         Tuple[torch.Tensor, dict]: 1. the flattened tensors with shape (num_params,), 2. an indexing dictionary
-    #             used for reconstructing the original coef_dict from the flatten tensor.
-    #     """
-    #     type2idx = dict()
-    #     param_list = list()
-    #     start = 0
-
-    #     for var_type in coef_dict.keys():
-    #         num_params = coef_dict[var_type].coef.numel()
-    #         # track which portion of all_param tensor belongs to this variable type.
-    #         type2idx[var_type] = (start, start + num_params)
-    #         start += num_params
-    #         # use reshape instead of view to make a copy.
-    #         param_list.append(coef_dict[var_type].coef.clone().reshape(-1,))
+        Args:
+            variable (str): the variable name.
+            level (str): from which level of model to extract the coefficient, can be 'item' or 'nest'. The `level` argument will be discarded if `variable` is `lambda`.
 
-    #     all_param = torch.cat(param_list)  # (self.num_params(), )
-    #     return all_param, type2idx
+        Returns:
+            torch.Tensor: the corresponding coefficient tensor of the requested variable.
+        """
+        if variable == 'lambda':
+            return self.lambda_weight.detach().clone()
 
-    # @staticmethod
-    # def unwrap_coef_dict(param: torch.Tensor, type2idx: Dict[str, Tuple[int, int]]) -> Dict[str, torch.Tensor]:
-    #     """Rebuilds coef_dict from output of self.flatten_coef_dict method.
+        if level not in ['item', 'nest']:
+            raise ValueError(f"Level should be either 'item' or 'nest', got {level}.")
 
-    #     Args:
-    #         param (torch.Tensor): the flattened coef_dict from self.flatten_coef_dict.
-    #         type2idx (Dict[str, Tuple[int, int]]): the indexing dictionary from self.flatten_coef_dict.
+        return self.state_dict()[f'{level}_coef_dict.{variable}.coef'].detach().clone()
 
-    #     Returns:
-    #         Dict[str, torch.Tensor]: the re-constructed coefficient dictionary.
+    # def clamp_lambdas(self):
     #     """
-    #     coef_dict = dict()
-    #     for var_type in type2idx.keys():
-    #         start, end = type2idx[var_type]
-    #         # no need to reshape here, Coefficient handles it.
-    #         coef_dict[var_type] = param[start:end]
-    #     return coef_dict
-
-    # def compute_hessian(self, x_dict, availability, user_index, y) -> torch.Tensor:
-    #     """Computes the Hessian of negative log-likelihood (total cross-entropy loss) with respect
-    #     to all parameters in this model. The Hessian can be later used for constructing the standard deviation of
-    #     parameters.
-
-    #     Args:
-    #         x_dict ,availability, user_index: see definitions in self.forward method.
-    #         y (torch.LongTensor): a tensor with shape (num_trips,) of IDs of items actually purchased.
-
-    #     Returns:
-    #         torch.Tensor: a (self.num_params, self.num_params) tensor of the Hessian matrix.
+    #     Restrict values of lambdas to 0 < lambda <= 1 to guarantee the utility maximization property
+    #     of the model.
+    #     This method should be called everytime after optimizer.step().
+    #     We add a self_clamp_called_flag to remind researchers if this method is not called.
     #     """
-    #     all_coefs, type2idx = self.flatten_coef_dict(self.coef_dict)
+    #     for k in range(len(self.lambdas)):
+    #         self.lambdas[k] = torch.clamp(self.lambdas[k], 1e-5, 1)
+    #     self._clam_called_flag = True
 
-    #     def compute_nll(P: torch.Tensor) -> float:
-    #         coef_dict = self.unwrap_coef_dict(P, type2idx)
-    #         y_pred = self._forward(x_dict=x_dict,
-    #                                availability=availability,
-    #                                user_index=user_index,
-    #                                manual_coef_value_dict=coef_dict)
-    #         # the reduction needs to be 'sum' to obtain NLL.
-    #         loss = F.cross_entropy(y_pred, y, reduction='sum')
-    #         return loss
-
-    #     H = torch.autograd.functional.hessian(compute_nll, all_coefs)
-    #     assert H.shape == (self.num_params, self.num_params)
-    #     return H
-
-    # def compute_std(self, x_dict, availability, user_index, y) -> Dict[str, torch.Tensor]:
-    #     """Computes
-
-    #     Args:f
-    #         See definitions in self.compute_hessian.
-
-    #     Returns:
-    #         Dict[str, torch.Tensor]: a dictionary whose keys are the same as self.coef_dict.keys()
-    #         the values are standard errors of coefficients in each coefficient group.
+    # @staticmethod
+    # def add_constant(x: torch.Tensor, where: str='prepend') -> torch.Tensor:
+    #     """A helper function used to add constant to feature tensor,
+    #     x has shape (batch_size, num_classes, num_parameters),
+    #     returns a tensor of shape (*, num_parameters+1).
     #     """
-    #     _, type2idx = self.flatten_coef_dict(self.coef_dict)
-    #     H = self.compute_hessian(x_dict, availability, user_index, y)
-    #     std_all = torch.sqrt(torch.diag(torch.inverse(H)))
-    #     std_dict = dict()
-    #     for var_type in type2idx.keys():
-    #         # get std of variables belonging to each type.
-    #         start, end = type2idx[var_type]
-    #         std_dict[var_type] = std_all[start:end]
-    #     return std_dict
+    #     batch_size, num_classes, num_parameters = x.shape
+    #     ones = torch.ones((batch_size, num_classes, 1))
+    #     if where == 'prepend':
+    #         new = torch.cat((ones, x), dim=-1)
+    #     elif where == 'append':
+    #         new = torch.cat((x, ones), dim=-1)
+    #     else:
+    #         raise Exception
+    #     return new
```

### Comparing `torch_choice-1.0.0/torch_choice/model/formula_parser.py` & `torch_choice-1.0.1/torch_choice/model/formula_parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import copy
+from typing import Dict, Tuple
+
 from torch_choice.data.choice_dataset import ChoiceDataset
-from typing import Tuple, Dict
 
 
 def parse_formula(formula: str, data: ChoiceDataset) -> Tuple[Dict[str, int], Dict[str, int]]:
     """Generates the coef_variation_dict and the num_samples_dict for Conditional/Nested logit models from a R-like
     formula and a ChoiceDataset.
     The parser reads variations of coefficients for different observables from the formula, then the parser retrieves
     the number of parameters for each coefficient (i.e., the dimension of each observable) from the ChoiceDataset.
@@ -33,26 +35,33 @@
     # example: (var1|item) + (var2|item) + (var3|item)
     formula = formula.replace(' ', '')  # delete all spaces.
     term_list = formula.split('+')  # a list of elements like (var2|item).
     for term in term_list:
         # e.g., term: (var|item)
         term = term.strip('()')  # (var|item) --> var|item
         # get the variable/observable and its variation.
-        variable, specificity = term.split('|')[0], term.split('|')[1]
+        corresponding_observable, specificity = term.split('|')[0], term.split('|')[1]
+        variable = copy.deepcopy(corresponding_observable)
+
         if variable == '1':
-            # the R-way of saying intercept, change it to intercept.
-            variable = 'intercept'
+            variable = 'intercept'  # the R-fashion for specifying intercept is 1, but we use `intercept` internally instead.
+
+        # rename variable to incorporate the variation.
+        variable = f"{variable}[{specificity}]"
+
+        if variable in coef_variation_dict.keys():
+            raise ValueError(f"variable[level of variation]={variable} is specified more than once in the formula, please remove the redundant one.")
 
         assert specificity in ['constant', 'item', 'item-full', 'user', 'user-item', 'user-item-full'], f'Component {term} must be one of constant, item, item-full, user, user-item, user-item-full.'
 
         # add to the coef_variation_dict dictionary.
         coef_variation_dict[variable] = specificity
 
         # retrieve the dimension of observable (i.e., number of parameters).
-        if variable == 'intercept':
+        if variable.startswith('intercept[') and variable.endswith(']'):
             # intercept only has one parameter.
             num_param_dict[variable] = 1
         else:
             # get the dimension of variable/observable from the data.
-            num_param_dict[variable] = getattr(data, variable).shape[-1]
+            num_param_dict[variable] = getattr(data, corresponding_observable).shape[-1]
 
     return coef_variation_dict, num_param_dict
```

### Comparing `torch_choice-1.0.0/torch_choice/utils/easy_data_wrapper.py` & `torch_choice-1.0.1/torch_choice/utils/easy_data_wrapper.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.0/torch_choice/utils/run_helper.py` & `torch_choice-1.0.1/torch_choice/utils/run_helper.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.0/torch_choice/utils/run_helper_temp.py` & `torch_choice-1.0.1/torch_choice/utils/run_helper_temp.py`

 * *Files identical despite different names*

### Comparing `torch_choice-1.0.0/torch_choice.egg-info/PKG-INFO` & `torch_choice-1.0.1/torch_choice.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: torch-choice
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Pytorch Backend Library for Choice Modelling
 Home-page: 
 Author: Tianyu Du
 Author-email: tianyudu@stanford.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 
 # torch-choice
 
 > Authors: Tianyu Du, Ayush Kanodia and Susan Athey; Contact: tianyudu@stanford.edu
 
+**Note on Installation**: This is a work in progress. We recommend installing the package from source to get the latest version and bug-fix patches.
+We are actively working on this package and will be adding more features and examples. Please feel free to reach out to us with any questions or suggestions.
+
 > Acknowledgements: We would like to thank Erik Sverdrup, Charles Pebereau and Keshav Agrawal for their feedback.
 
 `torch-choice` is a library for flexible, fast choice modeling with PyTorch: it has logit and nested logit models, designed for both estimation and prediction. See the [complete documentation](https://gsbdbi.github.io/torch-choice/) for more details.
 Unique features:
 1. GPU support via torch for speed
 2. Specify customized models
 3. Specify availability sets
```

### Comparing `torch_choice-1.0.0/torch_choice.egg-info/SOURCES.txt` & `torch_choice-1.0.1/torch_choice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

