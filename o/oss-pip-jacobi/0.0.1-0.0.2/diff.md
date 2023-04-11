# Comparing `tmp/oss_pip_jacobi-0.0.1-py3-none-any.whl.zip` & `tmp/oss_pip_jacobi-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1710 bytes, number of entries: 5
--rw-r--r--  2.0 unx      829 b- defN 23-Apr-11 14:40 jacobi/jacobiPltPrint.py
--rw-r--r--  2.0 unx      341 b- defN 23-Apr-11 14:44 oss_pip_jacobi-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 14:44 oss_pip_jacobi-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-11 14:44 oss_pip_jacobi-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      404 b- defN 23-Apr-11 14:44 oss_pip_jacobi-0.0.1.dist-info/RECORD
-5 files, 1673 bytes uncompressed, 948 bytes compressed:  43.3%
+Zip file size: 1740 bytes, number of entries: 5
+-rw-r--r--  2.0 unx     1195 b- defN 23-Apr-11 15:06 jacobi/jacobiPltPrint.py
+-rw-r--r--  2.0 unx      341 b- defN 23-Apr-11 15:06 oss_pip_jacobi-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 15:06 oss_pip_jacobi-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-11 15:06 oss_pip_jacobi-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      405 b- defN 23-Apr-11 15:06 oss_pip_jacobi-0.0.2.dist-info/RECORD
+5 files, 2040 bytes uncompressed, 978 bytes compressed:  52.1%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: jacobi/jacobiPltPrint.py
 Comment: 
 
-Filename: oss_pip_jacobi-0.0.1.dist-info/METADATA
+Filename: oss_pip_jacobi-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: oss_pip_jacobi-0.0.1.dist-info/WHEEL
+Filename: oss_pip_jacobi-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: oss_pip_jacobi-0.0.1.dist-info/top_level.txt
+Filename: oss_pip_jacobi-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: oss_pip_jacobi-0.0.1.dist-info/RECORD
+Filename: oss_pip_jacobi-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jacobi/jacobiPltPrint.py

```diff
@@ -1,8 +1,9 @@
 
+
 from numpy import zeros,array
 import matplotlib.pyplot as plt
 
 def jacobi(A,b,n):
   x1 =zeros(n)
   x2 =zeros(n)
   x3 =zeros(n)
@@ -14,20 +15,36 @@
   print("%7d %9.5f %9.5f %9.5f" % (0, x1[0], x2[0], x3[0]))
 
   for k in range(n - 1):
       x1[k + 1] = (b[0] + A[0,1] * x2[k] - A[0,2] * x3[k]) / A[0,0]
       x2[k + 1] = (b[1] + A[1,0] * x1[k] - A[1,2] * x3[k]) / A[1,1]
       x3[k + 1] = (b[2] + A[2,0] * x1[k] - A[2,1] * x2[k]) / A[2,2]
       print("%7d %9.5f %9.5f %9.5f" % (k + 1, x1[k + 1], x2[k + 1], x3[k + 1]))
-  
+  return x1,x2,x3
+
+def jacobi_plt_print(A,b,n):
+  x1 =zeros(n)
+  x2 =zeros(n)
+  x3 =zeros(n)
+
+  x1[0] = 0.0
+  x2[0] = 0.0
+  x3[0] = 0.0
+
+  for k in range(n - 1):
+      x1[k + 1] = (b[0] + A[0,1] * x2[k] - A[0,2] * x3[k]) / A[0,0]
+      x2[k + 1] = (b[1] + A[1,0] * x1[k] - A[1,2] * x3[k]) / A[1,1]
+      x3[k + 1] = (b[2] + A[2,0] * x1[k] - A[2,1] * x2[k]) / A[2,2]
+
   x = range(n)
   y = x1
   y1 = x2
   y2 = x3
   plt.plot(x, y, 'b--', label='x1')
   plt.plot(x, y1, 'r', label='x2')
   plt.plot(x, y2, 'g', label='x3')
   plt.legend()
   plt.title('jacobi')
   plt.xlabel('x')
   plt.ylabel('y')
   plt.show()
+
```

