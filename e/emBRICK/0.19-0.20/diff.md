# Comparing `tmp/emBRICK-0.19.tar.gz` & `tmp/emBRICK-0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emBRICK-0.19.tar", last modified: Wed Feb 15 14:25:27 2023, max compression
+gzip compressed data, was "emBRICK-0.20.tar", last modified: Tue Apr 11 11:14:51 2023, max compression
```

## Comparing `emBRICK-0.19.tar` & `emBRICK-0.20.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-02-15 14:25:27.222026 emBRICK-0.19/
--rw-rw-rw-   0        0        0     1091 2023-02-15 14:25:27.222541 emBRICK-0.19/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-02-15 14:25:27.202688 emBRICK-0.19/emBRICK/
--rw-rw-rw-   0        0        0        1 2021-04-12 11:58:59.000000 emBRICK-0.19/emBRICK/__init__.py
--rw-rw-rw-   0        0        0    39656 2023-02-15 14:04:48.000000 emBRICK-0.19/emBRICK/bricks.py
--r--r--r--   0        0        0    15285 2023-02-07 16:00:09.000000 emBRICK-0.19/emBRICK/ethernet.py
--r--r--r--   0        0        0    15864 2023-02-15 14:13:16.000000 emBRICK-0.19/emBRICK/modbus_rtu.py
--rw-rw-rw-   0        0        0    12003 2021-10-11 13:00:45.000000 emBRICK-0.19/emBRICK/modbus_tcp.py
-drwxrwxrwx   0        0        0        0 2023-02-15 14:25:27.219317 emBRICK-0.19/emBRICK.egg-info/
--rw-rw-rw-   0        0        0     1091 2023-02-15 14:25:27.000000 emBRICK-0.19/emBRICK.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2023-02-15 14:25:27.000000 emBRICK-0.19/emBRICK.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-15 14:25:27.000000 emBRICK-0.19/emBRICK.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-02-15 14:25:27.000000 emBRICK-0.19/emBRICK.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-02-15 14:25:27.000000 emBRICK-0.19/emBRICK.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-02-15 14:25:27.222734 emBRICK-0.19/setup.cfg
--rw-rw-rw-   0        0        0     2076 2023-02-15 14:16:45.000000 emBRICK-0.19/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 11:14:51.082891 emBRICK-0.20/
+-rw-rw-rw-   0        0        0     1088 2023-02-13 10:03:34.000000 emBRICK-0.20/LICENSE
+-rw-rw-rw-   0        0        0     1114 2023-04-11 11:14:51.082963 emBRICK-0.20/PKG-INFO
+-rw-rw-rw-   0        0        0     2825 2023-02-13 10:03:34.000000 emBRICK-0.20/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 11:14:51.077364 emBRICK-0.20/emBRICK/
+-rw-rw-rw-   0        0        0        1 2021-04-12 11:58:59.000000 emBRICK-0.20/emBRICK/__init__.py
+-rw-rw-rw-   0        0        0     1332 2023-04-06 15:14:43.000000 emBRICK-0.20/emBRICK/binary_utils.py
+-rw-rw-rw-   0        0        0    39747 2023-04-11 10:27:42.000000 emBRICK-0.20/emBRICK/bricks.py
+-r--r--r--   0        0        0    15285 2023-02-07 16:00:09.000000 emBRICK-0.20/emBRICK/ethernet.py
+-rw-rw-rw-   0        0        0    15561 2023-04-11 10:06:20.000000 emBRICK-0.20/emBRICK/modbus_rtu.py
+-rw-rw-rw-   0        0        0    11572 2023-04-11 10:22:59.000000 emBRICK-0.20/emBRICK/modbus_tcp.py
+drwxrwxrwx   0        0        0        0 2023-04-11 11:14:51.081834 emBRICK-0.20/emBRICK.egg-info/
+-rw-rw-rw-   0        0        0     1114 2023-04-11 11:14:51.000000 emBRICK-0.20/emBRICK.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-04-11 11:14:51.000000 emBRICK-0.20/emBRICK.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 11:14:51.000000 emBRICK-0.20/emBRICK.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-11 11:14:51.000000 emBRICK-0.20/emBRICK.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-11 11:14:51.000000 emBRICK-0.20/emBRICK.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-11 11:14:51.083819 emBRICK-0.20/setup.cfg
+-rw-rw-rw-   0        0        0     2076 2023-04-11 08:41:03.000000 emBRICK-0.20/setup.py
```

### Comparing `emBRICK-0.19/PKG-INFO` & `emBRICK-0.20/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emBRICK
-Version: 0.19
+Version: 0.20
 Summary: Driver to build a connection RemoteMaster <-> LWCS over Ethernet, Modbus TCP & RTU
 Home-page: https://github.com/IMACS-GmbH/emBRICK/tree/main/Protocol%20Stacks/remoteBUS/Python%20via%20TCP-IP%20or%20RSxxx
 Download-URL: https://github.com/IMACS-GmbH/emBRICK/raw/main/Protocol%20Stacks/remoteBUS/Python%20via%20TCP-IP%20or%20RSxxx/emBRICK-0.15.tar.gz
 Author: IMACS
 Author-email: serkan.sen@imacs-gmbh.de
 License: MIT
 Keywords: IMACS,EMBRICK,PYTHON,TCP/IP,Modbus,RTU,TCP
@@ -15,7 +15,8 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+License-File: LICENSE
```

### Comparing `emBRICK-0.19/emBRICK/bricks.py` & `emBRICK-0.20/emBRICK/bricks.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,28 +14,29 @@
 
 brick_info = ''
 lock.acquire()
 def findBricks():
     '''
     Check connected Bricks and configure the corresponding objects
     '''
+    
+    # TODO: braucht man das global hier? 
     global brick_info
-    bricks = {}
 
     bricks = {2181: CAE_G8Di8Do, 4602: CAE_B3U4I, 4603: CAE_B3U4I, 2470: CAE_G2Mi2Ao, 2471: CAE_G2Mi2Ao,
               2472: CAE_G2Mi2Ao, 2431: CAE_G4Ai4Tmp, 2432: CAE_G4Ai4Tmp, 2433: CAE_G4Ai4Tmp, 2434: CAE_G4Ai4Tmp,
               2435: CAE_G4Ai4Tmp, 2436: CAE_G4Ai4Tmp}
     '''
     bricks = {2181: G8Di8Do, 4602: B3U4I, 4603: B3U4I, 2470: G2Mi2Ao, 2471: G2Mi2Ao, 2472: G2Mi2Ao, 2431: G4Ai4Tmp,
               2432: G4Ai4Tmp, 2433: G4Ai4Tmp, 2434: G4Ai4Tmp, 2435: G4Ai4Tmp, 2436: G4Ai4Tmp}
     '''
     for node in connect.unit_id:
         for i in range(connect.master["local" + str(node)].number_bricks):
             id = connect.slave["master" + str(node)]["Brick" + str(i + 1)].brick_id
-            found = bricks.get(id, "None")
+            found = bricks.get(id, "None") # find brick name in dictionary or otherwise return "None"
             if found == "None":
                 error = open("error.txt", "a+")
                 error.write(f'{datetime.now()} ERROR: No Brick with ID {id} found.\n')
                 error.close()
                 brick_info += f'NOT FOUND! Brick {i+1}: {connect.slave["master" + str(node)]["Brick" + str(i+1)].name} '\
                 f'ID: {connect.slave["master" + str(node)]["Brick" + str(i+1)].brick_id // 1000}-{connect.slave["master" + str(node)]["Brick" + str(i+1)].brick_id % 1000} '\
                 f'Hardware Revision: {connect.slave["master" + str(node)]["Brick" + str(i+1)].hard_rev}\n'
```

### Comparing `emBRICK-0.19/emBRICK/ethernet.py` & `emBRICK-0.20/emBRICK/ethernet.py`

 * *Files identical despite different names*

### Comparing `emBRICK-0.19/emBRICK/modbus_rtu.py` & `emBRICK-0.20/emBRICK/modbus_rtu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,52 +1,27 @@
 #!/usr/bin/evn python3
 # Import Threading Module
 import threading
 import time
 import math
 import json
 from datetime import datetime
+import emBRICK.binary_utils as binary_utils 
+
 # Import pymodbus for the Modbus RTU Module
 from pymodbus.client.sync import ModbusSerialClient as ModbusClient
 lock = threading.Lock()
 
 filename = "error"
 ERROR = open(filename, "w+")
 
 brick_name = {2181: "CAE_G8Di8Do", 4602: "CAE_B3U4I", 4603: "CAE_B3U4I", 2470: "CAE_G2Mi2Ao", 2471: "CAE_G2Mi2Ao",
             2472: "CAE_G2Mi2Ao", 2431: "CAE_G4Ai4Tmp", 2432: "CAE_G4Ai4Tmp", 2433: "CAE_G4Ai4Tmp", 2434: "CAE_G4Ai4Tmp",
             2435: "CAE_G4Ai4Tmp", 2436: "CAE_G4Ai4Tmp"}
 
-
-def splitBytes(list16bit):
-    ''' Function to split a list with 16 bit elements into 8 bit element list '''
-    list8bit = []
-    for value in list16bit:
-        a = (value >> 8) & 0xFF
-        b = value & 0xFF
-        list8bit.append(a)
-        list8bit.append(b)
-    return list8bit
-
-
-def addBytes(list8bit):
-    ''' Function to add two 8 bit element from a list to one 16 bit element and put them in a list '''
-    list16bit = []
-    if not len(list8bit) // 2:
-        list8bit.append(0)
-    for num in range(len(list8bit)):
-        if not num % 2:
-            byte0 = list8bit[num] << 8
-        else:
-            byte1 = list8bit[num]
-            byte = byte0 + byte1
-            list16bit.append(byte)
-    return list16bit
-
-
 class local_master:
     ''' Sorting the information about the local master '''
     __slots__ = ['number_bricks','state','master_id','prot_ver','soft_ver', 'manu_id', 'res1', 'res2']
     def __init__(self, number_bricks, state, master_id, prot_ver, soft_ver, manu_id, res1, res2):
         self.number_bricks = number_bricks
         self.state = state
         self.master_id = master_id
@@ -103,26 +78,27 @@
             ERROR.write(f'{datetime.now()}\tERROR: Connection with Port {self.port} failed!')
             ERROR.close()
             exit()
         # Initialize the Functions to start the Program
         bB_update.getLWCsInfo()
         for id in self.unit_id:
             self.master["local" + str(id)] = local_master(bB_update.local_data[id][0], bB_update.local_data[id][1], ((bB_update.local_data[id][2] << 8) + bB_update.local_data[id][3]),
-                        bB_update.local_data[id][4],bB_update.local_data[id][5], bB_update.local_data[id][6], bB_update.local_data[id][7], bB_update.local_data[id][8])                 
+                        bB_update.local_data[id][4],bB_update.local_data[id][5], bB_update.local_data[id][6], bB_update.local_data[id][7], bB_update.local_data[id][8])                
+            
             self.slave["master" + str(id)] = {}
             for i in range(self.master["local" + str(id)].number_bricks):
                 found = brick_name.get((bB_update.local_data[id][9+(i*11)+5] << 8) + bB_update.local_data[id][9+(i*11)+6], "Not found!")
                 self.slave["master" + str(id)]["Brick"+ str(i+1)] = slave_module(bB_update.local_data[id][9+(i*11)+0], bB_update.local_data[id][9+(i*11)+1], bB_update.local_data[id][9+(i*11)+2],
                         bB_update.local_data[id][9+(i*11)+3], bB_update.local_data[id][9+(i*11)+4], (bB_update.local_data[id][9+(i*11)+5] << 8) + bB_update.local_data[id][9+(i*11)+6],
                         (bB_update.local_data[id][9+(i*11)+7] << 8) + bB_update.local_data[id][9+(i*11)+8],\
                         bB_update.local_data[id][9+(i*11)+9], bB_update.local_data[id][9+(i*11)+10], found )
         bB_update.update_first()
         bB.createEmptyList()
         updatcycle = threading.Thread(target=bB_update.update)
-        updatcycle.daemon = True.
+        updatcycle.daemon = True
         updatcycle.start()
         init()
         #time.sleep(1)
         #t1.join()
 
 connect = connection()
 
@@ -138,15 +114,15 @@
         for id in connect.unit_id:
             i = 0
             # Reads in the Init Data in the address range 1000h ... 107 ch
             while(i < 5):
                 responce = connect.node.read_input_registers(4096,104, unit = id)
                 if not responce.isError():
                     data_16byte = responce.registers
-                    self.local_data[id] = splitBytes(data_16byte)
+                    self.local_data[id] = binary_utils.convert16bitTo8bitList(data_16byte)
                     break
                 else:
                     ERROR.write(f'{datetime.now()}\tERROR: Connection to the Coupling-Master with Modbus Address {id} failed!\n')
                     i += 1
                 if i == 5:
                     ERROR.write(f'{datetime.now()}\tERROR: Connection to the Coupling-Master with Modbus Address {id} failed!\n')
                     connect.unit_id.remove(id)
@@ -164,15 +140,15 @@
                 time.sleep(0.005)
                 if not responce.isError():
                     self.updates[id] = responce.registers
                 else:
                     ERROR.write(f'{datetime.now()}\tERROR: Checksum Error or Timeout\n')
                     i += 1
                 if self.updates[id] != 0:
-                    self.updated[id] = splitBytes(self.updates[id])
+                    self.updated[id] = binary_utils.convert16bitTo8bitList(self.updates[id])
                     break
             if i == 5:
                 ERROR.write(f'{datetime.now()}\tERROR: Connection with LWCs on Modbus Address {id} not possible\n')
                 connect.unit_id.remove(id)
         if len(connect.unit_id) == 0:
             ERROR.close()
             exit()
@@ -182,36 +158,41 @@
         # Update the emBricks in the individual updaterate
         while True:
             if not connect.node.is_socket_open() == True:
                 connect.node.connect()
             for id in connect.unit_id:
                 if not bB.put[id] == []:
                     with lock:
-                        bB.set[id] = addBytes(bB.put[id])
+                        bB.set[id] = binary_utils.convert8bitTo16bitList(bB.put[id])
                 arguments = {
                     'read_address': 0,
                     'read_count': bB.buffer_length[id],
                     'write_address': 0,
                     'write_registers': bB.set[id],
                 }
 
-                responce = connect.node.readwrite_registers(unit=id, **arguments)
-                if not responce.isError():
-                    self.updates[id] = responce.registers
-                else:
-                    ERROR.write(f'{datetime.now()}\tERROR: Checksum Error or Timeout Error\n')
+                try:
+                    response = connect.node.readwrite_registers(unit=id, **arguments)
+                    self.updates[id] = response.registers
+                except ConnectionException as e:
+                    ERROR.write(f'{datetime.now()}\tERROR: Connection error: {e}\n')
+                except ModbusException as e:
+                    ERROR.write(f'{datetime.now()}\tERROR: Modbus error: {e}\n')
+                except Exception as e:
+                    ERROR.write(f'{datetime.now()}\tERROR: Unknown error: {e}\n')
 
                 if self.updates[id] != 0:
                     lock.acquire()
-                    self.updated[id] = splitBytes(self.updates[id])
+                    self.updated[id] = binary_utils.convert16bitTo8bitList(self.updates[id])
 
                     lock.release()
                 if self.stopThread:
                     ERROR.close()
                     raise SystemExit()
+            time.sleep(connect.updateRate)
 
 
 bB_update = brickBus_communication()
 
 
 
 class functions:
```

### Comparing `emBRICK-0.19/emBRICK/modbus_tcp.py` & `emBRICK-0.20/emBRICK/modbus_tcp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,53 +1,34 @@
 #!/usr/bin/evn python3
 # Import Threading Module
 import threading
 import time
+import emBRICK.binary_utils as binary_utils
 # Import pymodbus for the Modbus TCP Module
 from pymodbus.client.sync import ModbusTcpClient as ModbusClient
 # For Current Date
 from datetime import datetime
-lock = threading.RLock()
+
+# wird scheinbbar nicht verwendet
+#lock = threading.RLock()
 filename = 'error.txt'
 
-def splitBytes(list16bit):
-    # Function to split a list with 16 bit elements into 8 bit element list
-    list8bit = []
-    for value in list16bit:
-        a = (value >> 8) & 0xff
-        b = value & 0xff
-        list8bit.append(a)
-        list8bit.append(b)
-    return list8bit
-
-def addBytes(list8bit):
-    list16bit = []
-    if not len(list8bit) // 2:
-        list8bit.append(0)
-    for num in range(len(list8bit)):
-        if not num % 2:
-            byte0 = list8bit[num] << 8
-        else:
-            byte1 = list8bit[num]
-            byte = byte0 + byte1
-            list16bit.append(byte)
-    return list16bit
 
 class data_from_local_master:
     # Reading the init Data from Local Master and split the 16 bit elements into 8 bit
     def __init__(self):
         #self.datain16byte = []
         self.data16 = {}
         self.data8 = {}
     def getData(self):
         for n in range(len(connect.node)):
             # Reads in the Init Data in the address range 1000h ... 107 ch
             responce = connect.node[n].read_input_registers(4096,104, unit = connect.unit_id)
             self.data16[n] = responce.registers
-            self.data8[n] = splitBytes(self.data16[n])
+            self.data8[n] = binary_utils.convert16bitTo8bitList(self.data16[n])
 getInfo = data_from_local_master()
 
 class local_master:
     # Sorting the information about the local master
     def __init__(self):
         self.number_of_bricks = []
         self.status = []
@@ -147,46 +128,46 @@
             responce = self.node[n].read_input_registers(0, 120, unit=self.unit_id)
             time.sleep(0.005)
             try:
                 self.updates[n] = responce.registers
             except:
                 continue
             if self.updates[n] != 0:
-                self.updated[n] = splitBytes(self.updates[n])
+                self.updated[n] = binary_utils.convert16bitTo8bitList(self.updates[n])
         #bB.createEmptyList()
 
     def update(self):
         # Update the emBricks in the individual updaterate
         while True:
             for n in range(len(self.node)):
                 num_bricks = local.number_of_bricks[n]
                 if not bB.put[n] == []:
-                    bB.set[n] = addBytes(bB.put[n])
+                    bB.set[n] = binary_utils.convert8bitTo16bitList(bB.put[n])
                     # print('Set:', bB.set[n])
                     arguments = {
                         'read_address': 0,
                         'read_count': bB.buffer_length[n],
                         'write_address': 0,
                         'write_registers': bB.set[n],
                     }
                     responce = self.node[n].readwrite_registers(unit=self.unit_id, **arguments)
                     try:
                         self.updates[n] = responce.registers
                     except:
                         continue
                     if self.updates[n] != 0:
-                        self.updated[n] = splitBytes(self.updates[n])
+                        self.updated[n] = binary_utils.convert16bitTo8bitList(self.updates[n])
                 else:
                     responce = self.node.read_input_registers(0, bB.buffer_length, unit=n)
                     try:
                         self.updates[n] = responce.registers
                     except:
                         continue
                     if self.updates[n] != 0:
-                        self.updated[n] = splitBytes(self.updates[n])
+                        self.updated[n] = binary_utils.convert16bitTo8bitList(self.updates[n])
             time.sleep(connect.updateRate)
 
 
 connect = connection()
 
 
 class functions:
```

### Comparing `emBRICK-0.19/emBRICK.egg-info/PKG-INFO` & `emBRICK-0.20/emBRICK.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emBRICK
-Version: 0.19
+Version: 0.20
 Summary: Driver to build a connection RemoteMaster <-> LWCS over Ethernet, Modbus TCP & RTU
 Home-page: https://github.com/IMACS-GmbH/emBRICK/tree/main/Protocol%20Stacks/remoteBUS/Python%20via%20TCP-IP%20or%20RSxxx
 Download-URL: https://github.com/IMACS-GmbH/emBRICK/raw/main/Protocol%20Stacks/remoteBUS/Python%20via%20TCP-IP%20or%20RSxxx/emBRICK-0.15.tar.gz
 Author: IMACS
 Author-email: serkan.sen@imacs-gmbh.de
 License: MIT
 Keywords: IMACS,EMBRICK,PYTHON,TCP/IP,Modbus,RTU,TCP
@@ -15,7 +15,8 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+License-File: LICENSE
```

### Comparing `emBRICK-0.19/setup.py` & `emBRICK-0.20/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'emBRICK',         # How you named your package folder (MyLib)
   packages = ['emBRICK'],   # Chose the same as "name"
-  version = '0.19',      # Start with a small number and increase it with every change you make
+  version = '0.20',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Driver to build a connection RemoteMaster <-> LWCS over Ethernet, Modbus TCP & RTU',   # Give a short description about your library
   author = 'IMACS',                   # Type in your name
   author_email = 'serkan.sen@imacs-gmbh.de',      # Type in your E-Mail
   url = 'https://github.com/IMACS-GmbH/emBRICK/tree/main/Protocol%20Stacks/remoteBUS/Python%20via%20TCP-IP%20or%20RSxxx',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/IMACS-GmbH/emBRICK/raw/main/Protocol%20Stacks/remoteBUS/Python%20via%20TCP-IP%20or%20RSxxx/emBRICK-0.15.tar.gz',    # I explain this later on
   keywords = ['IMACS', 'EMBRICK', 'PYTHON','TCP/IP','Modbus', 'RTU','TCP'],   # Keywords that define your package best
```

