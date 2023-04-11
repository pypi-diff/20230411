# Comparing `tmp/ledgerblue-0.1.8.tar.gz` & `tmp/ledgerblue-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ledgerblue-0.1.8.tar", last modified: Mon Oct 17 21:48:20 2016, max compression
+gzip compressed data, was "dist/ledgerblue-0.1.9.tar", last modified: Sun Jan 22 17:08:51 2017, max compression
```

## Comparing `ledgerblue-0.1.8.tar` & `ledgerblue-0.1.9.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxrwxr-x   0 nba       (1000) nba       (1000)        0 2016-10-17 21:48:20.000000 ledgerblue-0.1.8/
--rw-rw-r--   0 nba       (1000) nba       (1000)     1362 2016-10-17 21:48:20.000000 ledgerblue-0.1.8/PKG-INFO
--rw-rw-r--   0 nba       (1000) nba       (1000)       19 2016-10-11 10:52:30.000000 ledgerblue-0.1.8/MANIFEST.in
-drwxrwxr-x   0 nba       (1000) nba       (1000)        0 2016-10-17 21:48:20.000000 ledgerblue-0.1.8/ledgerblue.egg-info/
--rw-rw-r--   0 nba       (1000) nba       (1000)     1362 2016-10-17 21:48:20.000000 ledgerblue-0.1.8/ledgerblue.egg-info/PKG-INFO
--rw-rw-r--   0 nba       (1000) nba       (1000)       11 2016-10-17 21:48:20.000000 ledgerblue-0.1.8/ledgerblue.egg-info/top_level.txt
--rw-rw-r--   0 nba       (1000) nba       (1000)        1 2016-10-11 11:10:11.000000 ledgerblue-0.1.8/ledgerblue.egg-info/not-zip-safe
--rw-rw-r--   0 nba       (1000) nba       (1000)      108 2016-10-17 21:48:20.000000 ledgerblue-0.1.8/ledgerblue.egg-info/requires.txt
--rw-rw-r--   0 nba       (1000) nba       (1000)      644 2016-10-17 21:48:20.000000 ledgerblue-0.1.8/ledgerblue.egg-info/SOURCES.txt
--rw-rw-r--   0 nba       (1000) nba       (1000)        1 2016-10-17 21:48:20.000000 ledgerblue-0.1.8/ledgerblue.egg-info/dependency_links.txt
-drwxrwxr-x   0 nba       (1000) nba       (1000)        0 2016-10-17 21:48:20.000000 ledgerblue-0.1.8/ledgerblue/
--rw-rw-r--   0 nba       (1000) nba       (1000)     4765 2016-10-11 10:52:30.000000 ledgerblue-0.1.8/ledgerblue/hexParser.py
--rw-rw-r--   0 nba       (1000) nba       (1000)     6609 2016-10-11 10:52:30.000000 ledgerblue-0.1.8/ledgerblue/deployed.py
--rw-rw-r--   0 nba       (1000) nba       (1000)      760 2016-10-11 10:52:30.000000 ledgerblue-0.1.8/ledgerblue/__init__.py
--rw-rw-r--   0 nba       (1000) nba       (1000)     1764 2016-10-11 10:52:30.000000 ledgerblue-0.1.8/ledgerblue/loadMCU.py
--rw-rw-r--   0 nba       (1000) nba       (1000)     3908 2016-10-11 10:52:30.000000 ledgerblue-0.1.8/ledgerblue/ecWrapper.py
--rw-rw-r--   0 nba       (1000) nba       (1000)     1957 2016-10-11 10:52:30.000000 ledgerblue-0.1.8/ledgerblue/verifyApp.py
--rw-rw-r--   0 nba       (1000) nba       (1000)     3442 2016-10-11 10:59:08.000000 ledgerblue-0.1.8/ledgerblue/runScript.py
--rw-rw-r--   0 nba       (1000) nba       (1000)     2289 2016-10-11 10:52:30.000000 ledgerblue-0.1.8/ledgerblue/deleteApp.py
--rw-rw-r--   0 nba       (1000) nba       (1000)     5550 2016-10-11 16:08:36.000000 ledgerblue-0.1.8/ledgerblue/comm.py
--rw-rw-r--   0 nba       (1000) nba       (1000)     5243 2016-10-11 10:52:30.000000 ledgerblue-0.1.8/ledgerblue/loadApp.py
--rw-rw-r--   0 nba       (1000) nba       (1000)     2066 2016-10-11 11:09:58.000000 ledgerblue-0.1.8/ledgerblue/listApps.py
--rw-rw-r--   0 nba       (1000) nba       (1000)     1976 2016-10-11 10:52:30.000000 ledgerblue-0.1.8/ledgerblue/signApp.py
--rw-rw-r--   0 nba       (1000) nba       (1000)     7941 2016-10-11 10:57:34.000000 ledgerblue-0.1.8/ledgerblue/hexLoader.py
--rw-rw-r--   0 nba       (1000) nba       (1000)     1307 2016-10-11 16:21:54.000000 ledgerblue-0.1.8/ledgerblue/derivePassphrase.py
--rw-rw-r--   0 nba       (1000) nba       (1000)      977 2016-10-11 16:08:36.000000 ledgerblue-0.1.8/ledgerblue/commException.py
--rw-rw-r--   0 nba       (1000) nba       (1000)     3607 2016-10-11 10:52:30.000000 ledgerblue-0.1.8/ledgerblue/ledgerWrapper.py
--rw-rw-r--   0 nba       (1000) nba       (1000)     6132 2016-10-11 10:52:54.000000 ledgerblue-0.1.8/ledgerblue/checkGenuine.py
--rw-rw-r--   0 nba       (1000) nba       (1000)      960 2016-10-13 12:26:27.000000 ledgerblue-0.1.8/setup.py
--rw-rw-r--   0 nba       (1000) nba       (1000)      737 2016-10-11 10:52:30.000000 ledgerblue-0.1.8/README.md
--rw-rw-r--   0 nba       (1000) nba       (1000)       59 2016-10-17 21:48:20.000000 ledgerblue-0.1.8/setup.cfg
+drwxrwxr-x   0 nba       (1000) nba       (1000)        0 2017-01-22 17:08:51.000000 ledgerblue-0.1.9/
+-rw-rw-r--   0 nba       (1000) nba       (1000)      960 2017-01-02 09:25:49.000000 ledgerblue-0.1.9/setup.py
+-rw-rw-r--   0 nba       (1000) nba       (1000)       19 2016-10-11 10:52:30.000000 ledgerblue-0.1.9/MANIFEST.in
+-rw-rw-r--   0 nba       (1000) nba       (1000)     2257 2017-01-22 17:08:51.000000 ledgerblue-0.1.9/PKG-INFO
+-rw-rw-r--   0 nba       (1000) nba       (1000)     1432 2017-01-08 23:32:12.000000 ledgerblue-0.1.9/README.md
+drwxrwxr-x   0 nba       (1000) nba       (1000)        0 2017-01-22 17:08:51.000000 ledgerblue-0.1.9/ledgerblue/
+-rw-rw-r--   0 nba       (1000) nba       (1000)     2053 2017-01-09 12:38:51.000000 ledgerblue-0.1.9/ledgerblue/listApps.py
+-rw-rw-r--   0 nba       (1000) nba       (1000)     2122 2017-01-09 10:04:11.000000 ledgerblue-0.1.9/ledgerblue/verifyEndorsement2.py
+-rw-rw-r--   0 nba       (1000) nba       (1000)     6132 2016-10-11 10:52:54.000000 ledgerblue-0.1.9/ledgerblue/checkGenuine.py
+-rw-rw-r--   0 nba       (1000) nba       (1000)     2289 2016-10-11 10:52:30.000000 ledgerblue-0.1.9/ledgerblue/deleteApp.py
+-rw-rw-r--   0 nba       (1000) nba       (1000)     6487 2017-01-14 15:46:54.000000 ledgerblue-0.1.9/ledgerblue/loadApp.py
+-rw-rw-r--   0 nba       (1000) nba       (1000)     6609 2016-10-11 10:52:30.000000 ledgerblue-0.1.9/ledgerblue/deployed.py
+-rw-rw-r--   0 nba       (1000) nba       (1000)     1957 2016-10-11 10:52:30.000000 ledgerblue-0.1.9/ledgerblue/verifyApp.py
+-rw-rw-r--   0 nba       (1000) nba       (1000)      977 2016-10-11 16:08:36.000000 ledgerblue-0.1.9/ledgerblue/commException.py
+-rw-rw-r--   0 nba       (1000) nba       (1000)     1390 2017-01-02 09:25:49.000000 ledgerblue-0.1.9/ledgerblue/derivePassphrase.py
+-rw-rw-r--   0 nba       (1000) nba       (1000)     9132 2017-01-14 15:44:45.000000 ledgerblue-0.1.9/ledgerblue/hexParser.py
+-rw-rw-r--   0 nba       (1000) nba       (1000)     1375 2017-01-22 17:05:16.000000 ledgerblue-0.1.9/ledgerblue/hashApp.py
+-rw-rw-r--   0 nba       (1000) nba       (1000)      760 2016-10-11 10:52:30.000000 ledgerblue-0.1.9/ledgerblue/__init__.py
+-rw-rw-r--   0 nba       (1000) nba       (1000)     4163 2017-01-08 22:56:04.000000 ledgerblue-0.1.9/ledgerblue/ecWrapper.py
+-rw-rw-r--   0 nba       (1000) nba       (1000)     1976 2016-10-11 10:52:30.000000 ledgerblue-0.1.9/ledgerblue/signApp.py
+-rw-rw-r--   0 nba       (1000) nba       (1000)     8356 2017-01-14 15:43:56.000000 ledgerblue-0.1.9/ledgerblue/hexLoader.py
+-rw-rw-r--   0 nba       (1000) nba       (1000)     3590 2017-01-22 17:05:16.000000 ledgerblue-0.1.9/ledgerblue/runScript.py
+-rw-rw-r--   0 nba       (1000) nba       (1000)     5552 2017-01-14 15:42:02.000000 ledgerblue-0.1.9/ledgerblue/comm.py
+-rw-rw-r--   0 nba       (1000) nba       (1000)     1878 2017-01-22 17:05:16.000000 ledgerblue-0.1.9/ledgerblue/endorsementSetup.py
+-rw-rw-r--   0 nba       (1000) nba       (1000)     3607 2016-10-11 10:52:30.000000 ledgerblue-0.1.9/ledgerblue/ledgerWrapper.py
+-rw-rw-r--   0 nba       (1000) nba       (1000)     1738 2017-01-14 15:47:09.000000 ledgerblue-0.1.9/ledgerblue/loadMCU.py
+-rw-rw-r--   0 nba       (1000) nba       (1000)     2007 2017-01-09 10:00:53.000000 ledgerblue-0.1.9/ledgerblue/verifyEndorsement1.py
+-rw-rw-r--   0 nba       (1000) nba       (1000)       59 2017-01-22 17:08:51.000000 ledgerblue-0.1.9/setup.cfg
+drwxrwxr-x   0 nba       (1000) nba       (1000)        0 2017-01-22 17:08:51.000000 ledgerblue-0.1.9/ledgerblue.egg-info/
+-rw-rw-r--   0 nba       (1000) nba       (1000)       11 2017-01-22 17:08:51.000000 ledgerblue-0.1.9/ledgerblue.egg-info/top_level.txt
+-rw-rw-r--   0 nba       (1000) nba       (1000)        1 2017-01-22 17:08:51.000000 ledgerblue-0.1.9/ledgerblue.egg-info/dependency_links.txt
+-rw-rw-r--   0 nba       (1000) nba       (1000)        1 2016-10-11 11:10:11.000000 ledgerblue-0.1.9/ledgerblue.egg-info/not-zip-safe
+-rw-rw-r--   0 nba       (1000) nba       (1000)     2257 2017-01-22 17:08:51.000000 ledgerblue-0.1.9/ledgerblue.egg-info/PKG-INFO
+-rw-rw-r--   0 nba       (1000) nba       (1000)      763 2017-01-22 17:08:51.000000 ledgerblue-0.1.9/ledgerblue.egg-info/SOURCES.txt
+-rw-rw-r--   0 nba       (1000) nba       (1000)      108 2017-01-22 17:08:51.000000 ledgerblue-0.1.9/ledgerblue.egg-info/requires.txt
```

### Comparing `ledgerblue-0.1.8/ledgerblue.egg-info/SOURCES.txt` & `ledgerblue-0.1.9/ledgerblue.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -5,22 +5,26 @@
 ledgerblue/checkGenuine.py
 ledgerblue/comm.py
 ledgerblue/commException.py
 ledgerblue/deleteApp.py
 ledgerblue/deployed.py
 ledgerblue/derivePassphrase.py
 ledgerblue/ecWrapper.py
+ledgerblue/endorsementSetup.py
+ledgerblue/hashApp.py
 ledgerblue/hexLoader.py
 ledgerblue/hexParser.py
 ledgerblue/ledgerWrapper.py
 ledgerblue/listApps.py
 ledgerblue/loadApp.py
 ledgerblue/loadMCU.py
 ledgerblue/runScript.py
 ledgerblue/signApp.py
 ledgerblue/verifyApp.py
+ledgerblue/verifyEndorsement1.py
+ledgerblue/verifyEndorsement2.py
 ledgerblue.egg-info/PKG-INFO
 ledgerblue.egg-info/SOURCES.txt
 ledgerblue.egg-info/dependency_links.txt
 ledgerblue.egg-info/not-zip-safe
 ledgerblue.egg-info/requires.txt
 ledgerblue.egg-info/top_level.txt
```

### Comparing `ledgerblue-0.1.8/ledgerblue/deployed.py` & `ledgerblue-0.1.9/ledgerblue/deployed.py`

 * *Files identical despite different names*

### Comparing `ledgerblue-0.1.8/ledgerblue/__init__.py` & `ledgerblue-0.1.9/ledgerblue/__init__.py`

 * *Files identical despite different names*

### Comparing `ledgerblue-0.1.8/ledgerblue/loadMCU.py` & `ledgerblue-0.1.9/ledgerblue/loadMCU.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,9 +43,9 @@
 
 dongle = getDongle(args.apdu)
 
 #relative load
 loader = HexLoader(dongle, 0xe0, False, None, False)
 
 loader.validateTargetId(args.targetId)
-hash = loader.load(0xFF, 0xF0, parser.getAreas(), args.bootAddr)
+hash = loader.load(0xFF, 0xF0, parser)
 loader.run(parser.getAreas(), args.bootAddr)
```

### Comparing `ledgerblue-0.1.8/ledgerblue/ecWrapper.py` & `ledgerblue-0.1.9/ledgerblue/ecWrapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -75,14 +75,22 @@
 			# libsecp256k1 style secret
 			out = b"\x03" if ((point.y & 1) != 0) else b"\x02"
 			out += point.x.to_bytes(32, 'big')
 			hash = hashlib.sha256()
 			hash.update(out)
 			return hash.digest()
 
+	def tweak_add(self, scalar):
+		if USE_SECP:
+			self.obj = self.obj.tweak_add(scalar)
+		else:
+			scalar = int.from_bytes(scalar, 'big')
+			privKey = ECPrivateKey(scalar, CURVE_SECP256K1)
+			self.obj = ECPublicKey(self.obj.W + privKey.get_public_key().W)
+
 	def ecdsa_verify(self, msg, raw_sig, raw=False, digest=hashlib.sha256):
 		if USE_SECP:
 			return self.obj.ecdsa_verify(msg, raw_sig, raw, digest)
 		else:
 			if not raw:
 				h = digest()
 				h.update(msg)
```

### Comparing `ledgerblue-0.1.8/ledgerblue/verifyApp.py` & `ledgerblue-0.1.9/ledgerblue/verifyApp.py`

 * *Files identical despite different names*

### Comparing `ledgerblue-0.1.8/ledgerblue/runScript.py` & `ledgerblue-0.1.9/ledgerblue/runScript.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,80 +21,85 @@
 from .deployed import getDeployedSecretV2
 from .ecWrapper import PrivateKey
 from Crypto.Cipher import AES
 import argparse
 import sys
 import fileinput
 
+
 def auto_int(x):
     return int(x, 0)
 
 parser = argparse.ArgumentParser()
 parser.add_argument("--fileName", help="Set the file name to load")
 parser.add_argument("--apdu", help="Display APDU log", action='store_true')
-parser.add_argument("--scp", help="open secure channel to exchange apdu", action='store_true')
+parser.add_argument(
+    "--scp", help="open secure channel to exchange apdu", action='store_true')
 parser.add_argument("--targetId", help="Set the chip target ID", type=auto_int)
 parser.add_argument("--rootPrivateKey", help="Set the root private key")
 
 args = parser.parse_args()
 
-if args.targetId == None:
-	args.targetId = 0x31100002
+if args.targetId is None:
+    args.targetId = 0x31100002
 if not args.fileName:
-	#raise Exception("Missing fileName")
-	file = sys.stdin
+    #raise Exception("Missing fileName")
+    file = sys.stdin
 else:
-	file = open(args.fileName, "r")
+    file = open(args.fileName, "r")
+
 
 class SCP:
-	def __init__(self, dongle, targetId, rootPrivateKey):
-		self.key = getDeployedSecretV2(dongle, rootPrivateKey, targetId)
-		self.iv = b'\x00' * 16;
-		
-	def encryptAES(self, data):
-		paddedData = data + b'\x80'
-		while (len(paddedData) % 16) != 0:
-			paddedData += b'\x00'
-		cipher = AES.new(self.key, AES.MODE_CBC, self.iv)
-		encryptedData = cipher.encrypt(paddedData)
-		self.iv = encryptedData[len(encryptedData) - 16:]
-		return encryptedData
-
-        def decryptAES(self, data):
-                if len(data) == 0:
-                        return data
-                cipher = AES.new(self.key, AES.MODE_CBC, self.iv)
-                decryptedData = cipher.decrypt(data)
-                l = len(decryptedData) - 1
-                while (decryptedData[l] != chr(0x80)):
-                        l-=1
-                decryptedData = decryptedData[0:l]
-                self.iv = data[len(data) - 16:]
-                return decryptedData
+
+    def __init__(self, dongle, targetId, rootPrivateKey):
+        self.key = getDeployedSecretV2(dongle, rootPrivateKey, targetId)
+        self.iv = b'\x00' * 16
+
+    def encryptAES(self, data):
+        paddedData = data + b'\x80'
+        while (len(paddedData) % 16) != 0:
+            paddedData += b'\x00'
+        cipher = AES.new(self.key, AES.MODE_CBC, self.iv)
+        encryptedData = cipher.encrypt(paddedData)
+        self.iv = encryptedData[len(encryptedData) - 16:]
+        return encryptedData
+
+    def decryptAES(self, data):
+        if len(data) == 0:
+            return data
+        cipher = AES.new(self.key, AES.MODE_CBC, self.iv)
+        decryptedData = cipher.decrypt(data)
+        l = len(decryptedData) - 1
+        while (decryptedData[l] != chr(0x80)):
+            l -= 1
+        decryptedData = decryptedData[0:l]
+        self.iv = data[len(data) - 16:]
+        return decryptedData
 
 dongle = getDongle(args.apdu)
 if args.scp:
-	if args.rootPrivateKey == None:
-		privateKey = PrivateKey()
-		publicKey = binascii.hexlify(privateKey.pubkey.serialize(compressed=False))
-		print("Generated random root public key : %s" % publicKey)
-		args.rootPrivateKey = privateKey.serialize()
-	scp = SCP(dongle, args.targetId, bytearray.fromhex(args.rootPrivateKey))
+    if args.rootPrivateKey is None:
+        privateKey = PrivateKey()
+        publicKey = binascii.hexlify(
+            privateKey.pubkey.serialize(compressed=False))
+        print("Generated random root public key : %s" % publicKey)
+        args.rootPrivateKey = privateKey.serialize()
+    scp = SCP(dongle, args.targetId, bytearray.fromhex(args.rootPrivateKey))
 
 for data in file:
-	data = data.rstrip('\r\n').decode('hex')
-	if len(data) < 5:
-		continue
-	if args.scp:
-		data = bytearray(data)
-		if data[4] > 0 and len(data)>5:
-			apduData = data[5 : 5 + data[4]]
-			apduData = scp.encryptAES(str(apduData))
-			result = dongle.exchange(data[0:4] + bytearray([len(apduData)]) + bytearray(apduData))
-		else:
-			result = dongle.exchange(data[0:5])
-		result = scp.decryptAES(str(result))
-		if args.apdu:
-			print "<= Clear " + result.encode('hex')	
-	else:
-		dongle.exchange(bytearray(data))	
-
+    data = data.rstrip('\r\n').decode('hex')
+    if len(data) < 5:
+        continue
+    if args.scp:
+        data = bytearray(data)
+        if data[4] > 0 and len(data) > 5:
+            apduData = data[5: 5 + data[4]]
+            apduData = scp.encryptAES(str(apduData))
+            result = dongle.exchange(
+                data[0:4] + bytearray([len(apduData)]) + bytearray(apduData))
+        else:
+            result = dongle.exchange(data[0:5])
+        result = scp.decryptAES(str(result))
+        if args.apdu:
+            print("<= Clear " + result.encode('hex'))
+    else:
+        dongle.exchange(bytearray(data))
```

### Comparing `ledgerblue-0.1.8/ledgerblue/deleteApp.py` & `ledgerblue-0.1.9/ledgerblue/deleteApp.py`

 * *Files identical despite different names*

### Comparing `ledgerblue-0.1.8/ledgerblue/comm.py` & `ledgerblue-0.1.9/ledgerblue/comm.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 		start = time.time()
 		data = ""
 		while len(data) == 0:
 			data = self.device.read(65)
 			if not len(data):
 				if time.time() - start > timeout:
 					raise CommException("Timeout")
-				time.sleep(0.02)
+				time.sleep(0.0001)
 		return bytearray(data)
 
 	def close(self):
 		if self.opened:
 			try:
 				self.device.close()
 			except:
```

### Comparing `ledgerblue-0.1.8/ledgerblue/loadApp.py` & `ledgerblue-0.1.9/ledgerblue/loadApp.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,17 +13,19 @@
 *  distributed under the License is distributed on an "AS IS" BASIS,
 *  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 *  See the License for the specific language governing permissions and
 *  limitations under the License.
 ********************************************************************************
 """
 
+DEFAULT_ALIGNMENT = 1024
+
 from .ecWrapper import PrivateKey
 from .comm import getDongle
-from .hexParser import IntelHexParser
+from .hexParser import IntelHexParser, IntelHexPrinter
 from .hexLoader import HexLoader
 from .deployed import getDeployedSecretV1, getDeployedSecretV2
 import argparse
 import struct
 import binascii
 import sys
 
@@ -55,14 +57,17 @@
 parser.add_argument("--signature", help="Optional application's signature (hex encoded)")
 parser.add_argument("--appFlags", help="Set the application flags", type=auto_int)
 parser.add_argument("--bootAddr", help="Set the boot address", type=auto_int)
 parser.add_argument("--rootPrivateKey", help="Set the root private key")
 parser.add_argument("--apdu", help="Display APDU log", action='store_true')
 parser.add_argument("--deployLegacy", help="Use legacy deployment API", action='store_true')
 parser.add_argument("--apilevel", help="Use given API level when interacting with the device", type=auto_int)
+parser.add_argument("--delete", help="Delete app before installing it", action='store_true')
+parser.add_argument("--params", help="Store icon and install parameters in a parameter section before the code", action='store_true')
+parser.add_argument("--appVersion", help="Set the application version (text)")
 
 args = parser.parse_args()
 
 if args.apilevel == None:
 	args.apilevel = 5
 if args.targetId == None:
 	args.targetId = 0x31000002
@@ -111,37 +116,56 @@
 else:
 	if args.curve != None:
 		print("Curve not supported using this API level, ignoring")
 	if args.path != None:
 		if len(args.path) > 1:
 			print("Multiple path levels not supported using this API level, ignoring")
 		else:
-			path = parse_bip32_path(args.path[0], args.apilevel)
+			path = parse_bip32_path(args.path[0], args.apilevel)	
+
+icon = None
+if not args.icon is None:
+	icon = bytearray.fromhex(args.icon)
+	
+signature = None
+if not args.signature is None:
+	signature = bytearray.fromhex(args.signature)
+	
+#prepend app's data with the icon content (could also add other various install parameters)
+printer = IntelHexPrinter(parser)
+#todo build a TLV zone to keep install params
+#todo dney nvm_write in that section ?
+paramsSectionContent = []
+if icon:
+	paramsSectionContent = icon
+
+# prepend the param section (arbitrary)
+if (args.params):
+	#take care of aligning the parameters sections to avoid possible invalid dereference of aligned words in the program nvram.
+	#also use the default MPU alignment
+	param_start = printer.minAddr()-len(paramsSectionContent)-(DEFAULT_ALIGNMENT-(len(paramsSectionContent)%DEFAULT_ALIGNMENT))
+	printer.addArea(param_start, paramsSectionContent)
+
+# account for added regions (install parameters, icon ...)
+appLength = printer.maxAddr() - printer.minAddr()
+
 
 dongle = getDongle(args.apdu)
 
 if args.deployLegacy:
 	secret = getDeployedSecretV1(dongle, bytearray.fromhex(args.rootPrivateKey), args.targetId)
 else:
 	secret = getDeployedSecretV2(dongle, bytearray.fromhex(args.rootPrivateKey), args.targetId)
 loader = HexLoader(dongle, 0xe0, True, secret)
 
-if (not (args.appFlags & 2)):
-	loader.deleteApp(args.appName)
-
-appLength = 0
-for area in parser.getAreas():
-	appLength += len(area.getData())	
-
-icon = None
-if args.icon != None:
-	icon = bytes(bytearray.fromhex(args.icon))
-
-signature = None
-if args.signature != None:
-	signature = bytes(bytearray.fromhex(args.signature))
+if (not (args.appFlags & 2)) and args.delete:
+		loader.deleteApp(args.appName)
 
+#heuristic to guess how to pass the icon
+if (args.params):
+	loader.createApp(args.appFlags, appLength, args.appName, None, path, 0, len(paramsSectionContent), args.appVersion)
+else:
+	loader.createApp(args.appFlags, appLength, args.appName, icon, path, None, None, args.appVersion)
 
-loader.createApp(args.appFlags, appLength, args.appName, icon, path)
-hash = loader.load(0x0, 0xE0, parser.getAreas(), args.bootAddr)
+hash = loader.load(0x0, 0xF0, printer)
 print("Application hash : " + hash)
-loader.run(parser.getAreas(), args.bootAddr, signature)
+loader.run(printer, args.bootAddr, signature)
```

### Comparing `ledgerblue-0.1.8/ledgerblue/listApps.py` & `ledgerblue-0.1.9/ledgerblue/listApps.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,40 +19,39 @@
 
 from .ecWrapper import PrivateKey
 from .comm import getDongle
 from .deployed import getDeployedSecretV1, getDeployedSecretV2
 from .hexLoader import HexLoader
 import argparse
 import binascii
-import sys
+
 
 def auto_int(x):
-    return int(x, 0)
+	return int(x, 0)
 
 parser = argparse.ArgumentParser()
 parser.add_argument("--targetId", help="Set the chip target ID", type=auto_int)
 parser.add_argument("--rootPrivateKey", help="Set the root private key")
 parser.add_argument("--apdu", help="Display APDU log", action='store_true')
 parser.add_argument("--deployLegacy", help="Use legacy deployment API", action='store_true')
 
 args = parser.parse_args()
 
-if args.targetId == None:
+if args.targetId is None:
 	args.targetId = 0x31000002
-if args.rootPrivateKey == None:
+if args.rootPrivateKey is None:
 	privateKey = PrivateKey()
 	publicKey = binascii.hexlify(privateKey.pubkey.serialize(compressed=False))
 	print("Generated random root public key : %s" % publicKey)
 	args.rootPrivateKey = privateKey.serialize()
 
 dongle = getDongle(args.apdu)
 
 if args.deployLegacy:
 	secret = getDeployedSecretV1(dongle, bytearray.fromhex(args.rootPrivateKey), args.targetId)
 else:
 	secret = getDeployedSecretV2(dongle, bytearray.fromhex(args.rootPrivateKey), args.targetId)
 loader = HexLoader(dongle, 0xe0, True, secret)
 apps = loader.listApp()
 while len(apps) != 0:
-	print apps
+	print(apps)
 	apps = loader.listApp(False)
-
```

### Comparing `ledgerblue-0.1.8/ledgerblue/signApp.py` & `ledgerblue-0.1.9/ledgerblue/signApp.py`

 * *Files identical despite different names*

### Comparing `ledgerblue-0.1.8/ledgerblue/hexLoader.py` & `ledgerblue-0.1.9/ledgerblue/hexLoader.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 """
 
 from Crypto.Cipher import AES
 import struct
 import hashlib
 import binascii
 
+LOAD_SEGMENT_CHUNK_HEADER_LENGTH = 3
+MIN_PADDING_LENGTH = 1
+
 class HexLoader:
 	def __init__(self, card, cla=0xF0, secure=False, key=None, relative=True):
 		self.card = card
 		self.cla = cla
 		self.secure = secure
 		self.key = key
 		self.iv = b"\x00" * 16
@@ -85,15 +88,15 @@
 	def encryptAES(self, data):
 		if not self.secure:
 			return data
 		paddedData = data + b'\x80'
 		while (len(paddedData) % 16) != 0:
 			paddedData += b'\x00'
 		cipher = AES.new(self.key, AES.MODE_CBC, self.iv)
-		encryptedData = cipher.encrypt(paddedData)
+		encryptedData = cipher.encrypt(str(paddedData))
 		self.iv = encryptedData[len(encryptedData) - 16:]
 		return encryptedData
 
 	def decryptAES(self, data):
 		if not self.secure or len(data) == 0:
 			return data
 		cipher = AES.new(self.key, AES.MODE_CBC, self.iv)
@@ -132,23 +135,35 @@
 	def boot(self, bootadr, signature=None):
 		# Force jump into Thumb mode
 		bootadr |= 1
 		data = b'\x09' + struct.pack('>I', bootadr)
 		if (signature != None):
 			data += chr(len(signature)) + signature
 		data = self.encryptAES(data)
-		self.exchange(self.cla, 0x00, 0x00, 0x00, data)						
+		self.exchange(self.cla, 0x00, 0x00, 0x00, data)
+
+	def createApp(self, appflags, applength, appname, icon=None, path=None, iconOffset=None, iconSize=None, appversion=None):
+		data = b'\x0B' + struct.pack('>I', applength) + struct.pack('>I', appflags) + struct.pack('>B', len(appname)) + appname
+		if iconOffset is None:
+			if not (icon is None):
+				data += struct.pack('>B', len(icon)) + icon
+			else:
+				data += b'\x00'
 
-	def createApp(self, appflags, applength, appname, icon=None, path=None):
-		data = b'\x0B' + struct.pack('>I', applength) + struct.pack('>I', appflags) + struct.pack('>B', len(appname)) +  appname
-		if (icon != None):
-			data += struct.pack('>B', len(icon))+ icon
-		if (path != None):
+		if not (path is None):
 			data += struct.pack('>B', len(path)) + path
-                        
+		else:
+			data += b'\x00'
+
+		if not iconOffset is None:
+			data += struct.pack('>I', iconOffset) + struct.pack('>H', iconSize)
+
+		if not appversion is None:
+			data += struct.pack('>B', len(appversion)) + appversion
+
 		data = self.encryptAES(data)
 		self.exchange(self.cla, 0x00, 0x00, 0x00, data)						
 
 	def deleteApp(self, appname):
 		data = b'\x0C' +  struct.pack('>B',len(appname)) +  appname
 		data = self.encryptAES(data)
 		self.exchange(self.cla, 0x00, 0x00, 0x00, data)						
@@ -171,43 +186,43 @@
 			item['flags'] = response[offset] << 24 | response[offset + 1] << 16 | response[offset + 2] << 8 | response[offset + 3]
 			offset += 4
 			item['hash'] = response[offset : offset + 32]
 			offset += 32
 			result.append(item)
 		return result
 
-	def load(self, erase_u8, max_length_per_apdu, hexAreas, bootaddr):
+	def load(self, erase_u8, max_length_per_apdu, hexFile):
 		initialAddress = 0
-		if (len(hexAreas) != 0) and self.relative:
-			initialAddress = hexAreas[0].getStart()
+		if self.relative:
+			initialAddress = hexFile.minAddr()
 		sha256 = hashlib.new('sha256')
-		for area in hexAreas:
+		for area in hexFile.getAreas():
 			startAddress = area.getStart() - initialAddress
 			data = area.getData()
 			self.selectSegment(startAddress)
 			if len(data) == 0:
 				continue
 			if len(data) > 0x10000:
 				raise Exception("Invalid data size for loader")
 			crc = self.crc16(bytearray(data))
 			offset = 0
 			length = len(data)
 			while (length > 0):
-				if length > max_length_per_apdu:
-					chunkLen = max_length_per_apdu
+				if length > max_length_per_apdu - LOAD_SEGMENT_CHUNK_HEADER_LENGTH - MIN_PADDING_LENGTH:
+					chunkLen = max_length_per_apdu - LOAD_SEGMENT_CHUNK_HEADER_LENGTH - MIN_PADDING_LENGTH
 				else:
 					chunkLen = length
 				chunk = data[offset : offset + chunkLen]
 				sha256.update(chunk)
 				self.loadSegmentChunk(offset, bytes(chunk))
 				offset += chunkLen
 				length -= chunkLen
 			self.flushSegment()
 			self.crcSegment(0, len(data), crc)
 		return sha256.hexdigest()
 
-	def run(self, hexAreas, bootaddr, signature=None):
+	def run(self, hexFile, bootaddr, signature=None):
 		initialAddress = 0
-		if (len(hexAreas) != 0) and self.relative:
-			initialAddress = hexAreas[0].getStart()		
+		if self.relative:
+			initialAddress = hexFile.minAddr()
 		self.boot(bootaddr - initialAddress, signature)
```

### Comparing `ledgerblue-0.1.8/ledgerblue/derivePassphrase.py` & `ledgerblue-0.1.9/ledgerblue/derivePassphrase.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 *  limitations under the License.
 ********************************************************************************
 """
 
 from .comm import getDongle
 import argparse
 import getpass
+import unicodedata
 
 def auto_int(x):
     return int(x, 0)
 
 parser = argparse.ArgumentParser()
 parser.add_argument("--persistent", help="Persist passphrase as secondary PIN", action='store_true')
 
@@ -33,10 +34,11 @@
 
 passphrase = getpass.getpass("Enter BIP39 passphrase : ")
 if len(passphrase) != 0:
 	if args.persistent:
 		p1 = 0x02
 	else:
 		p1 = 0x01
-	apdu = bytearray([0xE0, 0xD0, p1, 0x00, len(passphrase)]) + bytearray(passphrase)
+	passphrase = unicodedata.normalize('NFKD', passphrase)
+	apdu = bytearray([0xE0, 0xD0, p1, 0x00, len(passphrase)]) + bytearray(passphrase, 'utf8')
 	dongle.exchange(apdu, timeout=300)
```

### Comparing `ledgerblue-0.1.8/ledgerblue/commException.py` & `ledgerblue-0.1.9/ledgerblue/commException.py`

 * *Files identical despite different names*

### Comparing `ledgerblue-0.1.8/ledgerblue/ledgerWrapper.py` & `ledgerblue-0.1.9/ledgerblue/ledgerWrapper.py`

 * *Files identical despite different names*

### Comparing `ledgerblue-0.1.8/ledgerblue/checkGenuine.py` & `ledgerblue-0.1.9/ledgerblue/checkGenuine.py`

 * *Files identical despite different names*

### Comparing `ledgerblue-0.1.8/setup.py` & `ledgerblue-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup, find_packages
 from os.path import dirname, join
 import os
 
 here = dirname(__file__)
 setup(
     name='ledgerblue',
-    version='0.1.8',
+    version='0.1.9',
     author='Ledger',
     author_email='hello@ledger.fr',
     description='Python library to communicate with Ledger Blue/Nano S',
     long_description=open(join(here, 'README.md')).read(),
     url='https://github.com/LedgerHQ/blue-loader-python',
     packages=find_packages(),
     install_requires=['hidapi>=0.7.99', 'pycrypto>=2.6.1', 'future', 'ecpy>=0.8.1', 'pillow>=3.4.0'],
```

### Comparing `ledgerblue-0.1.8/README.md` & `ledgerblue-0.1.9/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -6,13 +6,38 @@
 
 ```
 virtualenv ledger
 source ledger/bin/activate
 pip install ledgerblue
 ```
 
+## Installation pre-requisites
+
+
+  * libudev-dev
+  * libusb-1.0-0-dev 
+  * python-dev (python 2.7)
+  * virtualenv
+
 This package can optionally work with [libsecp256k1](https://github.com/ludbb/secp256k1-py) Python bindings compiled with ECDH support. If you wish to enable libsecp256k1 bindings, make sure to install libsecp256k1 as follows
 
 ```
-SECP_BUNDLED_EXPERIMENTAL=1 pip --no-cache-dir install secp256k1
+SECP_BUNDLED_EXPERIMENTAL=1 pip --no-cache-dir --no-binary secp256k1 install secp256k1
 ``` 
 
+## Giving permissions on udev 
+
+When running on Linux, make sure the following rules have been added to /etc/udev/rules.d/
+
+```
+SUBSYSTEMS=="usb", ATTRS{idVendor}=="2c97", ATTRS{idProduct}=="0000", MODE="0660", TAG+="uaccess", TAG+="udev-acl" OWNER="<UNIX username>"
+SUBSYSTEMS=="usb", ATTRS{idVendor}=="2c97", ATTRS{idProduct}=="0001", MODE="0660", TAG+="uaccess", TAG+="udev-acl" OWNER="<UNIX username>"
+
+```
+
+## Target ID
+
+Use the following Target IDs (--targetId option) when running commands directly 
+
+  * 0x31100002 on Nano S
+  * 0x31000002 on Blue 
+
```

