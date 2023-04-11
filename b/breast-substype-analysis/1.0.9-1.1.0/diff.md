# Comparing `tmp/breast_substype_analysis-1.0.9-py3-none-any.whl.zip` & `tmp/breast_substype_analysis-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 20526 bytes, number of entries: 13
--rw-rw-rw-  2.0 fat        4 b- defN 23-Apr-04 13:15 app/__init__.py
+Zip file size: 20607 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat      137 b- defN 23-Apr-09 17:53 app/__init__.py
 -rw-rw-rw-  2.0 fat     5171 b- defN 23-Apr-04 13:15 app/autoencoder_model.py
 -rw-rw-rw-  2.0 fat      766 b- defN 23-Apr-04 13:15 app/config.py
 -rw-rw-rw-  2.0 fat     1342 b- defN 23-Apr-04 13:15 app/gcn_layer.py
--rw-rw-rw-  2.0 fat     1708 b- defN 23-Apr-04 13:15 app/gcn_model.py
--rw-rw-rw-  2.0 fat    46608 b- defN 23-Apr-09 17:45 app/routes.py
+-rw-rw-rw-  2.0 fat     1712 b- defN 23-Apr-09 17:46 app/gcn_model.py
+-rw-rw-rw-  2.0 fat    46586 b- defN 23-Apr-09 18:16 app/routes.py
 -rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-04 13:16 app/transformer.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-09 17:45 breast_substype_analysis-1.0.9.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1017 b- defN 23-Apr-09 17:45 breast_substype_analysis-1.0.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-09 17:45 breast_substype_analysis-1.0.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       51 b- defN 23-Apr-09 17:45 breast_substype_analysis-1.0.9.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        4 b- defN 23-Apr-09 17:45 breast_substype_analysis-1.0.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1092 b- defN 23-Apr-09 17:45 breast_substype_analysis-1.0.9.dist-info/RECORD
-13 files, 59046 bytes uncompressed, 18684 bytes compressed:  68.4%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-10 03:33 breast_substype_analysis-1.1.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1017 b- defN 23-Apr-10 03:33 breast_substype_analysis-1.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-10 03:33 breast_substype_analysis-1.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       51 b- defN 23-Apr-10 03:33 breast_substype_analysis-1.1.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Apr-10 03:33 breast_substype_analysis-1.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1094 b- defN 23-Apr-10 03:33 breast_substype_analysis-1.1.0.dist-info/RECORD
+13 files, 59163 bytes uncompressed, 18765 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: app/routes.py
 Comment: 
 
 Filename: app/transformer.py
 Comment: 
 
-Filename: breast_substype_analysis-1.0.9.dist-info/LICENSE
+Filename: breast_substype_analysis-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: breast_substype_analysis-1.0.9.dist-info/METADATA
+Filename: breast_substype_analysis-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: breast_substype_analysis-1.0.9.dist-info/WHEEL
+Filename: breast_substype_analysis-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: breast_substype_analysis-1.0.9.dist-info/entry_points.txt
+Filename: breast_substype_analysis-1.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: breast_substype_analysis-1.0.9.dist-info/top_level.txt
+Filename: breast_substype_analysis-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: breast_substype_analysis-1.0.9.dist-info/RECORD
+Filename: breast_substype_analysis-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## app/__init__.py

```diff
@@ -1,2 +1,8 @@
 
+from flask import Flask
+from config import Config
 
+app = Flask(__name__)
+app.config.from_object(Config)
+
+from app import routes
```

## app/gcn_model.py

```diff
@@ -5,15 +5,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # @Time    : 2021/8/8 16:20
 # @Author  : Xia shufan
 # @File    : gcn_model.py
 from torch import nn
 import torch.nn.functional as F
-from gcn_layer import GraphConvolution
+from app.gcn_layer import GraphConvolution
 
 class GCN(nn.Module):
     def __init__(self, n_in, n_hid, n_out, dropout=None):
         super(GCN, self).__init__()
         self.gc1 = GraphConvolution(n_in, n_hid)
         self.gc2 = GraphConvolution(n_hid, n_hid) # 使用了一个隐藏层,
         self.gc3 = GraphConvolution(n_hid, n_hid)
```

## app/routes.py

```diff
@@ -12,21 +12,21 @@
 
 import torch
 from flask import Flask, send_from_directory, Response
 from flask import request, send_file, session, flash, render_template, redirect, url_for
 from torchviz import make_dot  # https://blog.csdn.net/qq_46343832/article/details/122494685
 from werkzeug.security import generate_password_hash, check_password_hash
 from sklearn.metrics import f1_score, recall_score, precision_score
-from app.config import Config
+from config import Config
 
 import sys
 import os
 
 # 将 config 模块所在的目录添加到 Python 的搜索路径中
-# sys.path.append(os.path.join(os.path.dirname(__file__), 'app'))
+sys.path.append(os.path.join(os.path.dirname(__file__), 'app'))
 
 app = Flask(__name__, template_folder='templates', static_folder='static')
 # 添加配置信息
 app.config.from_object(Config)  # 这个我还没测试出来，因为models.py 总是有问题
 logger = logging.getLogger('my_logger')
 logger.debug('This is a debug message.')
 
@@ -225,15 +225,15 @@
         path = f'static/clean_data/clean_data.csv'
         # file = open(path, 'rb') # 这个是用来显示的
         return send_file(path, mimetype='text/html', as_attachment=True)
     else:
         return "404"
 
 
-from app.autoencoder_model import MMAE
+from autoencoder_model import MMAE
 import torch
 
 import torch.utils.data as Data
 
 
 # Define the route for the autoencoder model
 def work(Merge_data, in_feas, lr, bs, epochs, device, a, b, c, mode, topN, latent):
@@ -244,15 +244,14 @@
     X, Y = Merge_data.iloc[:, 1:].values, np.zeros(Merge_data.shape[0])
     TX, TY = torch.tensor(X, dtype=torch.float, device=device), torch.tensor(Y, dtype=torch.float, device=device)
     # train a AE model
     if mode == 0 or mode == 1:
         print('进入work函数的Training model...')
         Tensor_data = Data.TensorDataset(TX, TY)
         train_loader = Data.DataLoader(Tensor_data, batch_size=bs, shuffle=True)  # 设置每个批次bs大小，分批训练
-
         # initialize a model
         mmae = MMAE(in_feas, latent_dim=latent, a=a, b=b, c=c)
         mmae.to(device)
         mmae.train()  # 调用 train() 方法来将 mmae 对象设置为训练模式
         mmae.train_MMAE(train_loader, learning_rate=lr, device=device, epochs=epochs)
         mmae.eval()  # before save and test, fix the variables
         torch.save(mmae, 'static/model/AE/MMAE_model.pkl')  # 这种方式保存了mmae整个模型吗
@@ -418,16 +417,15 @@
         Merge_data = pd.merge(Merge_data, df_f3, on='Sample', how='inner')
         Merge_data.sort_values(by='Sample', ascending=True,
                                inplace=True)  # 具体来说，在pd.merge()函数中使用inner参数，会返回具有匹配键值的两个数据集的交集。在结果中，只包含具有相同Sample值的记录。
         work(Merge_data, in_feas, lr=lr, bs=batch_size, epochs=epoch, device=device, a=a, b=b, c=c, mode=mode,
              topN=topN, latent=latent)
         return render_template('AE.html')
         # Redirect the user back to the upload file page
-    return render_template(
-        'AE.html')  # 就不用这个做法了return redirect('/upload_file')， 再写个路由，@app.route('/upload_file')def upload_file():return render_template('upload_file.html')
+    return render_template('AE.html')  # 就不用这个做法了return redirect('/upload_file')， 再写个路由，@app.route('/upload_file')def upload_file():return render_template('upload_file.html')
 
 
 @app.route("/load_ae_model", methods=['POST', 'GET'])
 def load_ae_model():
     with open('df_f1.pkl', 'rb') as f1, open('df_f2.pkl', 'rb') as f2, open('df_f3.pkl', 'rb') as f3:
         df_f1 = pickle.load(f1)
         df_f2 = pickle.load(f2)
@@ -1059,15 +1057,15 @@
     sys.exit(0)
 
 def main():
     signal.signal(signal.SIGINT, my_exit)
     signal.signal(signal.SIGTERM, my_exit)
 
     parser = argparse.ArgumentParser()
-    parser.add_argument("-p", type=int, default=5431, help="指定端口号")
+    parser.add_argument("-p", type=int, default=5430, help="指定端口号")
     args = parser.parse_args()
 
     try:
         webbrowser.open('http://127.0.0.1:%d/' % (args.p))
         app.run(debug=True, host="0.0.0.0", port=args.p)
 
     except Exception as e:
```

## Comparing `breast_substype_analysis-1.0.9.dist-info/LICENSE` & `breast_substype_analysis-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `breast_substype_analysis-1.0.9.dist-info/METADATA` & `breast_substype_analysis-1.1.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breast-substype-analysis
-Version: 1.0.9
+Version: 1.1.0
 Summary: breast-subtype-analysis 是一个用于乳腺癌症分子分型预测的Python包。
 Author: xia shufan
 Author-email: 2757462803@qq.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `breast_substype_analysis-1.0.9.dist-info/RECORD` & `breast_substype_analysis-1.1.0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-app/__init__.py,sha256=26UWatnbm6ZIwQMuu9NNzQ0IW1ACO4Oe9caModuTpWM,4
+app/__init__.py,sha256=AGpmaXQARB9FOzT6k9tcrQNyCPvzLgVlor1Oo0y83m0,137
 app/autoencoder_model.py,sha256=y4KKS4lLGrL-By1JFfzyqOvhoV2C4CVq5MBGsfMb3r0,5171
 app/config.py,sha256=v0DGzKc5l0O2dNK-3KUAVlUgkT5abOEw7xPK9ELeKEU,766
 app/gcn_layer.py,sha256=NxeEYf0_kcvC7VPc8rst7D8d37wi3yjhjsBQQ2-wNGc,1342
-app/gcn_model.py,sha256=jWo6YTqph-tDjqnKckStNLXekuPgFH0ZDHwZkq4bFT4,1708
-app/routes.py,sha256=XL0M-VRNgkWolF5K2N2M7PuM0UY3Jht68pnKYNBLwY8,46608
+app/gcn_model.py,sha256=Xh9gOmQ9YXr8I5PXNbDWhIJg3Jy6UKGDfSlWuSzdVYA,1712
+app/routes.py,sha256=eFRoOTx42Facdx_i4w9isWJ4jugPGRoF8QVB4TcD0K4,46586
 app/transformer.py,sha256=7iHHzinvwrHNykIaRhfSxvmzL6dCP8ehhD8w_Z6cGfM,100
-breast_substype_analysis-1.0.9.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-breast_substype_analysis-1.0.9.dist-info/METADATA,sha256=jj4qqcrafPiiURU6f18s-kg5dj9bMxRVZhhTW8so-6Q,1017
-breast_substype_analysis-1.0.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-breast_substype_analysis-1.0.9.dist-info/entry_points.txt,sha256=w6wGhqT-FRurihant4rTOvBkd_h-7pvvl3_tweXeyOM,51
-breast_substype_analysis-1.0.9.dist-info/top_level.txt,sha256=io9g7LCbfmTG1SFKgEOGXmCFB9uMP2H5lerm0HiHWQE,4
-breast_substype_analysis-1.0.9.dist-info/RECORD,,
+breast_substype_analysis-1.1.0.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+breast_substype_analysis-1.1.0.dist-info/METADATA,sha256=ytkJnPYgj_y53cWNj8Rp8RmIqFytAYbV1_gYgVY0k88,1017
+breast_substype_analysis-1.1.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+breast_substype_analysis-1.1.0.dist-info/entry_points.txt,sha256=w6wGhqT-FRurihant4rTOvBkd_h-7pvvl3_tweXeyOM,51
+breast_substype_analysis-1.1.0.dist-info/top_level.txt,sha256=io9g7LCbfmTG1SFKgEOGXmCFB9uMP2H5lerm0HiHWQE,4
+breast_substype_analysis-1.1.0.dist-info/RECORD,,
```

