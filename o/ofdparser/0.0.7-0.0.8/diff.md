# Comparing `tmp/ofdparser-0.0.7.tar.gz` & `tmp/ofdparser-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofdparser-0.0.7.tar", last modified: Sat Apr  8 08:12:11 2023, max compression
+gzip compressed data, was "ofdparser-0.0.8.tar", last modified: Tue Apr 11 09:59:31 2023, max compression
```

## Comparing `ofdparser-0.0.7.tar` & `ofdparser-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 08:12:11.774612 ofdparser-0.0.7/
--rw-rw-rw-   0        0        0     1086 2023-02-18 03:44:37.000000 ofdparser-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     1028 2023-04-08 08:12:11.773366 ofdparser-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      565 2023-04-08 08:06:39.000000 ofdparser-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 08:12:11.725492 ofdparser-0.0.7/ofdparser/
--rw-rw-rw-   0        0        0       32 2023-03-28 06:51:58.000000 ofdparser-0.0.7/ofdparser/__init__.py
--rw-rw-rw-   0        0        0    47795 2023-04-08 08:01:23.000000 ofdparser-0.0.7/ofdparser/ofdparser.py
-drwxrwxrwx   0        0        0        0 2023-04-08 08:12:11.770383 ofdparser-0.0.7/ofdparser.egg-info/
--rw-rw-rw-   0        0        0     1028 2023-04-08 08:12:11.000000 ofdparser-0.0.7/ofdparser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-04-08 08:12:11.000000 ofdparser-0.0.7/ofdparser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 08:12:11.000000 ofdparser-0.0.7/ofdparser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-08 08:12:11.000000 ofdparser-0.0.7/ofdparser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-08 08:12:11.774612 ofdparser-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      996 2023-04-08 08:03:46.000000 ofdparser-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-08 08:12:11.772356 ofdparser-0.0.7/test/
--rw-rw-rw-   0        0        0        0 2023-03-28 06:38:57.000000 ofdparser-0.0.7/test/__init__.py
--rw-rw-rw-   0        0        0      978 2023-03-28 06:51:04.000000 ofdparser-0.0.7/test/test.py
+drwxrwxrwx   0        0        0        0 2023-04-11 09:59:31.329822 ofdparser-0.0.8/
+-rw-rw-rw-   0        0        0     1086 2023-02-18 03:44:37.000000 ofdparser-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1013 2023-04-11 09:59:31.327738 ofdparser-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2023-04-08 08:20:48.000000 ofdparser-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 09:59:31.107443 ofdparser-0.0.8/ofdparser/
+-rw-rw-rw-   0        0        0       32 2023-03-28 06:51:58.000000 ofdparser-0.0.8/ofdparser/__init__.py
+-rw-rw-rw-   0        0        0    53659 2023-04-11 09:45:41.000000 ofdparser-0.0.8/ofdparser/ofdparser.py
+drwxrwxrwx   0        0        0        0 2023-04-11 09:59:31.178393 ofdparser-0.0.8/ofdparser.egg-info/
+-rw-rw-rw-   0        0        0     1013 2023-04-11 09:59:30.000000 ofdparser-0.0.8/ofdparser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-04-11 09:59:30.000000 ofdparser-0.0.8/ofdparser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 09:59:30.000000 ofdparser-0.0.8/ofdparser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-11 09:59:30.000000 ofdparser-0.0.8/ofdparser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 09:59:31.329822 ofdparser-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      996 2023-04-11 09:58:27.000000 ofdparser-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 09:59:31.277785 ofdparser-0.0.8/test/
+-rw-rw-rw-   0        0        0        0 2023-03-28 06:38:57.000000 ofdparser-0.0.8/test/__init__.py
+-rw-rw-rw-   0        0        0      978 2023-03-28 06:51:04.000000 ofdparser-0.0.8/test/test.py
```

### Comparing `ofdparser-0.0.7/LICENSE` & `ofdparser-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ofdparser-0.0.7/PKG-INFO` & `ofdparser-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofdparser
-Version: 0.0.7
+Version: 0.0.8
 Summary: ofdparser
 Home-page: https://github.com/renoyuan/pyofdpaerser
 Author: renoyuan
 Author-email: renoyuan@foxmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyofdpaerser
 安装
-pip install pyofdpaerser
+pip install ofdparser
 
 项目链接： https://github.com/renoyuan/pyofdpaerser
 
 解析ofd 文件
 
 1 输出坐标和文本信息图片解析
     文本信息包括字体，字号，颜色
@@ -28,15 +28,15 @@
     
 2 ofd 转pdf
 
 3 新增对内嵌字体的转换 
 
 demo
 ```
-from pyofdpaerser,ofdpaser import OfdParser
+from ofdparser import OfdParser
 # 转pdf输出
 pdfbytes = OfdParser(ofdb64).ofd2pdf()
 
 # print(data_dict)
 # print(pdfbytes)
 with open(f"pdfs/{name}.pdf","wb") as f:
     f.write(pdfbytes)
```

### Comparing `ofdparser-0.0.7/README.md` & `ofdparser-0.0.8/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # pyofdpaerser
 安装
-pip install pyofdpaerser
+pip install ofdparser
 
 项目链接： https://github.com/renoyuan/pyofdpaerser
 
 解析ofd 文件
 
 1 输出坐标和文本信息图片解析
     文本信息包括字体，字号，颜色
@@ -12,15 +12,15 @@
     
 2 ofd 转pdf
 
 3 新增对内嵌字体的转换 
 
 demo
 ```
-from pyofdpaerser,ofdpaser import OfdParser
+from ofdparser import OfdParser
 # 转pdf输出
 pdfbytes = OfdParser(ofdb64).ofd2pdf()
 
 # print(data_dict)
 # print(pdfbytes)
 with open(f"pdfs/{name}.pdf","wb") as f:
     f.write(pdfbytes)
```

### Comparing `ofdparser-0.0.7/ofdparser/ofdparser.py` & `ofdparser-0.0.8/ofdparser/ofdparser.py`

 * *Files 4% similar despite different names*

```diff
@@ -166,16 +166,17 @@
         imageFile = imagePath+"/"+i+".png"
         renderPM.drawToFile(d, imageFile, fmt)
         
         print(i)
 
 
 class OfdParser(object):
-    def __init__(self,ofdb64,zip_path="") -> None:
+    def __init__(self,ofdb64,zip_path="",dpi=200) -> None:
         self.zip_path = ""
+        self.dpi = dpi
         self.ofdbyte = base64.b64decode(ofdb64) 
         if not zip_path:
             pid=os.getpid()
             zip_path = f"{os.getcwd()}/{pid}_{str(uuid1())}.ofd"
         self.zip_path = zip_path
         # fp = tempfile.TemporaryFile()
         # fp.write(ofdbyte)
@@ -642,22 +643,22 @@
                 page_ID +=1
             # print(cell_list)
         
         # json.dump(page_list,open("a.josn","w",encoding="utf-8"),indent=4,ensure_ascii=False)
         return page_list
 
     # 转json格式
-    def odf2json(self, page_list:list,dpi=200) ->dict:
+    def odf2json(self, page_list:list) ->dict:
         """
         坐标默认为毫米单位 
         dpi 有则转化为px
         """
         Op = 1 # 转换算子单位
         
-        dpi = 200
+        dpi = self.dpi # 200
         if dpi:
             Op = dpi/25.4
         
         # 行信息构建
         for paga in page_list:
             
             document_id = 'v1' + '_' + _genShortId()
@@ -668,15 +669,15 @@
             pageInfo["docID"] = document_id
             size = paga.get("page_size")
             if size:
                 size = [size[2],size[3]]
             else:
                 size = [0,0]
             pageInfo["imageQuality"] = {
-                "size": size
+                "size": [size[0]*Op, size[1]*Op]
             }
             pageInfo["lineList"] = []
             
             images = paga.get("images",[])
             if images:
                 for iamge in images:
                     pos = iamge.get('pos')
@@ -699,19 +700,43 @@
                 line["sortNo"] = lineNo
                 line["rowNo"] = lineNo
                 line["objType_postpreprocess"] = "text_postpreprocess"
                 
             
                 
                 # print(values)
-                line['objContent'] = values.get("text")
+                text = values.get("text")
+                line['objContent'] = text
                 pos = values.get("pos")
                 
                 offset = float(pos[3])*Op
-                pos = [float(pos[1])*Op, float(pos[0])*Op,float(pos[3])*Op,float(pos[2])*Op]
+                
+                DeltaX = values.get("DeltaX","")
+                DeltaY = values.get("DeltaY","")
+                X = values.get("X","")
+                Y = values.get("Y","")
+                CTM = values.get("CTM","") # 因为ofd 的傻逼 增加这个字符缩放
+                resizeX =1
+                resizeY =1
+                if CTM :
+                    # print(CTM)
+                    resizeX = float(CTM.split(" ")[0])
+                    resizeY = float(CTM.split(" ")[3])
+                
+                x_list = self.cmp_offset(values.get("pos")[0],X,DeltaX,text,resizeX)
+                y_list = self.cmp_offset(values.get("pos")[1],Y,DeltaY,text,resizeY)
+                # print("x_list",x_list,Op,CTM)
+                # print("pos",pos,float(X),float(x_list[-1]))
+                w = (float(x_list[-1])- float(X)-float(pos[0]))*Op
+                # print(text,w)
+                if w == 0:
+                    
+                    w = (float(x_list[-1])- float(X))*Op
+                # pos = [float(pos[1])*Op, float(pos[0])*Op,float(pos[3])*Op,float(pos[2])*Op]
+                pos = [float(y_list[0])*Op, float(x_list[0])*Op,float(pos[3])*Op,w]
                 offsetPost = [offset*(i+1) for i in range(len(values.get("text")))]
                 pos.append(offsetPost)
                 line['objPos'] = pos
             
                 line['objType'] = 'text'
                 pageInfo["lineList"].append(line)
             
@@ -729,30 +754,146 @@
                     "rowNo": cell.get("lineNo"),
                     "objType_postpreprocess": "table_postpreprocess"
                     
                     }
             pageInfo["contIndex"] = contIndex
             pageList.append(pageInfo)
         return pageList
+    
+    def sort_x(self,lineList):
+        lineList_bak = copy.deepcopy(lineList)
+        for idx,line in enumerate(lineList) :
+            for line2 in lineList_bak[idx:]:
+                if abs(line.get("objPos")[0] - line2.get("objPos")[0]) < 3 :
+                    line.get("objPos")[0] = line2.get("objPos")[0]
+                    
+        lineList.sort(key=lambda line:(line.get("objPos")[0],line.get("objPos")[1]))
+        return lineList
+    
+    # 合并行 并重排序 排除竖版块
+    def merge_line_pipeline(self, page_list):
+        page_list_new = []
+        for page_info in  page_list:
+            lineList = page_info.get("lineList")
+            lineList = self.sort_x(lineList)
+            page_list_new.append(
+                {
+                "pageNo": page_info.get("pageNo"),
+                "docID": page_info.get("docID"),
+                "imageQuality": page_info.get("imageQuality"),
+                
+                "lineList":self.merge_line(lineList),
+                "images": page_info.get("images"),
+                "contIndex": page_info.get("contIndex"),
+                
+                }
+                   
+               )
+           
+        
+        return page_list_new
+    
+    # 合并行  
+    def merge_line(self,lineList):
+        
+        lineList_new = []
+        non_id = []
+        for idx,line_info in enumerate(lineList) :
+            objPos = line_info.get("objPos")
+            if objPos[2]/objPos[3] >1: # 排除竖版块
+                if line_info and line_info.get("lineId") not in non_id:
+                    lineList_new.append(line_info)
+                    # print("line_info",line_info)
+                non_id.append(line_info.get("lineId"))
+                continue
+            
+            else:
+                # 找是否有符合条件的，有则合并无则返回
+                line_new = None
+                for line_info2 in lineList[idx:]:
+                    objPos2 = line_info2.get("objPos")
+                    if objPos == objPos2:
+                        line_new = line_info2
+                    if objPos[2]/objPos[3] >1 :
+                        # print("合并行")
+                        continue
+                    # print(line_info.get("objContent"))
+                    # print("objPos","objPos2")
+                    # print(objPos,objPos2)
+                    if objPos2[1] > objPos[1] and abs(objPos2[0] - objPos[0])<objPos[2]/2 and 0 < abs(objPos2[1] - objPos[1] - objPos[3]) < objPos[2]:
+                        # print("合并")
+                        # print(line_info.get("objContent") +  line_info2.get("objContent") )
+                        non_id.append(line_info2.get("lineId"))
+                        new_objContent = line_info.get("objContent") +  line_info2.get("objContent")
+                        # print("new_objContent",new_objContent)
+                        new_objPos = self.merge_pos (line_info.get("objPos"),line_info2.get("objPos"))
+                        
+                        line_new = {
+                            "lineId":line_info.get("lineId"),
+                            "lineNo":line_info.get("lineNo"),
+                            "objType_postpreprocess":line_info.get("objType_postpreprocess"),
+                            "objContent": new_objContent ,
+                            "objPos": new_objPos,
+                            "objType":line_info.get("objType") 
+                        }
+                        # print(line_new)
+                        # print(line_info.get("objContent") ,  line_info2.get("objContent"))
+                        
+                    
+                if line_new and line_new.get("lineId") not in non_id:
+                    # print(line_new)
+                    lineList_new.append(line_new)
+                    non_id.append(line_new.get("lineId"))
+                else:
+                    
+                    # print("banline_new",line_new)
+                    pass
+        
+        # print("non_id",non_id)
+        return lineList_new
+        
+    def merge_pos(self,pos1,pos2):
+        # print(pos1,pos2)
+        y = min(pos1[0],pos2[0])
+        x = min(pos1[1],pos2[1]) 
+        bottom = max( (pos1[2]),(pos2[0]+pos2[2]))
+        top = max( (pos1[1]+pos1[3]),(pos2[1]+pos2[3]))
+        h = bottom -y
+        w = top -x
+        offset_l = pos1[4]
+        offset = (pos2[1] - (pos1[1]+pos1[3]) )+ pos1[4][-1]
+        if len(pos2) == 4:
+            
+            for i in pos2[4]:
+                offset_l.append(offset+i)
+        pos = [y,x,h,w,offset_l]
+        
+        return pos
         
     # ofd2json流程
     def parserodf2json(self):
         try:
+            zip_path = self.zip_path
+            with open(zip_path,"wb") as f:
+                f.write(self.ofdbyte)
             unzip_path = self.unzip_file(self.zip_path)
             page_list = self.parse_ofd(unzip_path)
-            dict = self.odf2json(page_list,200)
+            page_list_new = self.odf2json(page_list)
+            #  结果后处理合并接近的块
+            page_list_new = self.merge_line_pipeline(page_list_new)
+            
             
            
         finally:
              # 删除文件
             if os.path.exists(unzip_path):
                 shutil.rmtree(unzip_path)
             if os.path.exists(self.zip_path):
                 os.remove(self.zip_path)
-        return dict
+        return page_list_new
     
     # task 
     @staticmethod
     def draw_task(c,parms):
         
         font_path,Glyph_id,char_,_cahr_x,_cahr_y,w,h = parms
         imageFile = draw_Glyph(font_path,Glyph_id,char_)
@@ -1064,69 +1205,65 @@
 
 
 
 if __name__ == "__main__":
     import time
     import json
     import base64
-    dirPath = "/home/0305data/OFD数据"
-    dirPath = "/home/data/调用成功但返回报错样本-0308"
-    dirPath = "/home/zhongjiayi/azx_projects/dataprocessengine/ofd"
-    dirPath = "/home/reno/input/22"
-    dirPath = "/home/0305data/ofd数据收集/0323"
-    dirPath = "/home/data/0305data/ofd数据收集/0404"
+
     dirPath = "/home/data/0305data/OFD数据总"
     # dir_ = os.listdir(dirPath)
     t_t = time.time()
     dir_ = []
     for root, dirs, files in os.walk(dirPath):
         for file in files:
             file_path = os.path.join(root, file)
             dir_.append(file_path)
 
     
     f_path = f"/home/data/0305data/ofd数据收集/0404/e20b0612-9807-481b-81b4-2ce57ace833c.ofd"
+    f_path = f"/home/data/0305data/OFD数据总/增值税电子专票4.ofd"
     f = open(f_path,"rb")
     ofdb64 = str(base64.b64encode(f.read()),"utf-8")
-    OfdParser(ofdb64,f_path).unzip_file("/home/data/0305data/ofd数据收集/0404/e20b0612-9807-481b-81b4-2ce57ace833c.ofd","e20b0612-9807-481b-81b4-2ce57ace833c")
+    OfdParser(ofdb64,f_path).unzip_file(f"{f_path}","增值税电子专票4")
     # pdfbytes = OfdParser(ofdb64).ofd2pdf(need_image=True) # 插入图片 支持jpg ,jpeg ，png 
-    pdfbytes = OfdParser(ofdb64).ofd2pdf() # 不插入图片
+    # pdfbytes = OfdParser(ofdb64).ofd2pdf() # 不插入图片
+    json_ =json.dump( OfdParser(ofdb64).parserodf2json(), open(f"json/增值税电子专票4.json","w",encoding="utf-8"), indent=4, ensure_ascii=False)
     # print(pdfbytes)
     # ocr_json = OfdParser(ofdb64).parserodf2json() #
     # print(ocr_json)
-    with open(f"test.pdf","wb") as f:
-            f.write(pdfbytes)
+    # with open(f"test.pdf","wb") as f:
+    #         f.write(pdfbytes)
     # 批量调
     count = 0
     for i in dir_:
         name =  i.split("/")[-1]
-        # break
+        break
         if i.split(".")[-1].lower() != "ofd":
             continue
         # f = open("增值税电子专票5.ofd","rb")
         f = open(f"{i}","rb")
         print(i)
         count += 1
+        # 传入b64 字符串
         ofdb64 = str(base64.b64encode(f.read()),"utf-8")
         # print(ofdb64)
         f.close
         t = time.time()
         
-        # 传入b64 字符串
-        
-        # 输出ocr 格式解析结果
-        # data_dict = OfdParser(ofdb64).parserodf2json()
-        
-        # 转pdf输出
-        pdfbytes = OfdParser(ofdb64).ofd2pdf()
-        
-        # print(data_dict)
-        # print(pdfbytes)
-        with open(f"pdfs/{name}.pdf","wb") as f:
-            f.write(pdfbytes)
+
+        # # 转pdf输出
+        # pdfbytes = OfdParser(ofdb64).ofd2pdf()
+        # with open(f"pdfs/{name}.pdf","wb") as f:
+        #     f.write(pdfbytes)
+            
+        # 转json输出
+        json_ =json.dump( OfdParser(ofdb64).parserodf2json(), open(f"json/{name}.json","w",encoding="utf-8"), indent=4, ensure_ascii=False)
+       
+       
         print(f"ofd解析耗时{(time.time()-t)*1000}/ms")	
         # json.dump(data_dict,open("data_dict.json","w",encoding="utf-8"),ensure_ascii=False,indent=4)
         # pbmpath = "image_80.pbm"
         # jb2path = "增值税电子专票5/Doc_0/Res/image_80.jb2"
         # pdfbytes = OfdParser(ofdb64).readjb2(jb2path,pbmpath)
     print(f"ofd解析 文件 {count} -------------- 总耗时{(time.time()-t_t)*1000}/ms")
```

### Comparing `ofdparser-0.0.7/ofdparser.egg-info/PKG-INFO` & `ofdparser-0.0.8/ofdparser.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofdparser
-Version: 0.0.7
+Version: 0.0.8
 Summary: ofdparser
 Home-page: https://github.com/renoyuan/pyofdpaerser
 Author: renoyuan
 Author-email: renoyuan@foxmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyofdpaerser
 安装
-pip install pyofdpaerser
+pip install ofdparser
 
 项目链接： https://github.com/renoyuan/pyofdpaerser
 
 解析ofd 文件
 
 1 输出坐标和文本信息图片解析
     文本信息包括字体，字号，颜色
@@ -28,15 +28,15 @@
     
 2 ofd 转pdf
 
 3 新增对内嵌字体的转换 
 
 demo
 ```
-from pyofdpaerser,ofdpaser import OfdParser
+from ofdparser import OfdParser
 # 转pdf输出
 pdfbytes = OfdParser(ofdb64).ofd2pdf()
 
 # print(data_dict)
 # print(pdfbytes)
 with open(f"pdfs/{name}.pdf","wb") as f:
     f.write(pdfbytes)
```

### Comparing `ofdparser-0.0.7/setup.py` & `ofdparser-0.0.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools #导入setuptools打包工具
  
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="ofdparser", # 项目名称
-    version="0.0.7",    #包版本号，便于维护版本
+    version="0.0.8",    #包版本号，便于维护版本
     author="renoyuan",    #作者，可以写自己的姓名
     author_email="renoyuan@foxmail.com",    #作者联系方式，可写自己的邮箱地址
     description="ofdparser",#包的简述
     long_description=long_description,    #包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/renoyuan/pyofdpaerser",    #自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
```

### Comparing `ofdparser-0.0.7/test/test.py` & `ofdparser-0.0.8/test/test.py`

 * *Files identical despite different names*

