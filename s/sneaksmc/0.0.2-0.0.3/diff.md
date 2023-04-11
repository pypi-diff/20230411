# Comparing `tmp/sneaksmc-0.0.2.tar.gz` & `tmp/sneaksmc-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sneaksmc-0.0.2.tar", last modified: Tue Apr 11 12:41:47 2023, max compression
+gzip compressed data, was "sneaksmc-0.0.3.tar", last modified: Tue Apr 11 13:53:02 2023, max compression
```

## Comparing `sneaksmc-0.0.2.tar` & `sneaksmc-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-11 12:41:47.096085 sneaksmc-0.0.2/
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      268 2023-04-11 12:41:47.096085 sneaksmc-0.0.2/PKG-INFO
--rw-rw-r--   0 tsy       (1000) tsy       (1000)       36 2023-03-01 09:47:59.000000 sneaksmc-0.0.2/README.rst
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      107 2023-04-11 12:41:47.096085 sneaksmc-0.0.2/setup.cfg
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      407 2023-04-11 12:40:54.000000 sneaksmc-0.0.2/setup.py
-drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-11 12:41:47.096085 sneaksmc-0.0.2/sneaksmc/
--rw-rw-r--   0 tsy       (1000) tsy       (1000)       75 2023-04-11 09:09:09.000000 sneaksmc-0.0.2/sneaksmc/__init__.py
--rw-rw-r--   0 tsy       (1000) tsy       (1000)     3122 2023-04-11 12:37:44.000000 sneaksmc-0.0.2/sneaksmc/client.py
--rw-rw-r--   0 tsy       (1000) tsy       (1000)     6379 2023-03-02 10:22:52.000000 sneaksmc-0.0.2/sneaksmc/crypt.py
--rw-rw-r--   0 tsy       (1000) tsy       (1000)    25182 2023-04-11 12:40:16.000000 sneaksmc-0.0.2/sneaksmc/server.py
-drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-11 12:41:47.096085 sneaksmc-0.0.2/sneaksmc.egg-info/
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      268 2023-04-11 12:41:46.000000 sneaksmc-0.0.2/sneaksmc.egg-info/PKG-INFO
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      265 2023-04-11 12:41:47.000000 sneaksmc-0.0.2/sneaksmc.egg-info/SOURCES.txt
--rw-rw-r--   0 tsy       (1000) tsy       (1000)        1 2023-04-11 12:41:46.000000 sneaksmc-0.0.2/sneaksmc.egg-info/dependency_links.txt
--rw-rw-r--   0 tsy       (1000) tsy       (1000)       13 2023-04-11 12:41:47.000000 sneaksmc-0.0.2/sneaksmc.egg-info/requires.txt
--rw-rw-r--   0 tsy       (1000) tsy       (1000)        9 2023-04-11 12:41:47.000000 sneaksmc-0.0.2/sneaksmc.egg-info/top_level.txt
+drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-11 13:53:02.884838 sneaksmc-0.0.3/
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      268 2023-04-11 13:53:02.884838 sneaksmc-0.0.3/PKG-INFO
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)       36 2023-03-01 09:47:59.000000 sneaksmc-0.0.3/README.rst
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      107 2023-04-11 13:53:02.884838 sneaksmc-0.0.3/setup.cfg
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      407 2023-04-11 13:52:45.000000 sneaksmc-0.0.3/setup.py
+drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-11 13:53:02.884838 sneaksmc-0.0.3/sneaksmc/
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)       75 2023-04-11 09:09:09.000000 sneaksmc-0.0.3/sneaksmc/__init__.py
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)     3461 2023-04-11 13:50:50.000000 sneaksmc-0.0.3/sneaksmc/client.py
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)     6390 2023-04-11 13:50:17.000000 sneaksmc-0.0.3/sneaksmc/crypt.py
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)    25027 2023-04-11 13:52:14.000000 sneaksmc-0.0.3/sneaksmc/server.py
+drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-11 13:53:02.884838 sneaksmc-0.0.3/sneaksmc.egg-info/
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      268 2023-04-11 13:53:02.000000 sneaksmc-0.0.3/sneaksmc.egg-info/PKG-INFO
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      265 2023-04-11 13:53:02.000000 sneaksmc-0.0.3/sneaksmc.egg-info/SOURCES.txt
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)        1 2023-04-11 13:53:02.000000 sneaksmc-0.0.3/sneaksmc.egg-info/dependency_links.txt
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)       13 2023-04-11 13:53:02.000000 sneaksmc-0.0.3/sneaksmc.egg-info/requires.txt
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)        9 2023-04-11 13:53:02.000000 sneaksmc-0.0.3/sneaksmc.egg-info/top_level.txt
```

### Comparing `sneaksmc-0.0.2/sneaksmc/client.py` & `sneaksmc-0.0.3/sneaksmc/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,81 @@
-# Clientk
 import http.client
 import time
-from .crypt import Cryptk
+from .crypt import Crypt
 
 
-class Clientk():
+def send_client_request(type="GET", url="empty", body="", receiver="", timeout=3.0):
+    """ Sends a request to another node/server.
+        Params:
+            @type       - The restful api type (get/put/post..).
+            @url        - The url that should correspond to this request.
+            @body       - The message body to send.
+            @receiver   - The server address which will receive this request.
+            @timeout    - The request timeout in seconds 
+                        (should be applied in case server can't be reached).
+        Returns the status code and message reply as a tuple (code, msg),
+         or (None, None) on error. """
+    try:
+        conn = http.client.HTTPConnection(receiver, timeout=timeout)
+        conn.request(type, url, body)
+        resp = conn.getresponse()
+        conn.close()
+        content = resp.read().decode()
+
+        return resp.status, content
+
+    except Exception as e:
+        print(e)
+    
+    return None, None
+
+
+class Client():
+    """ Client class to request and communicate with a sneaksmc coordinator. """
     def __init__(self) -> None:
-        """ Initialize client to request and communicate with SMC coordinator """
-        self.ck = Cryptk()
+        self.ck = Crypt()
         self.coordinator_node = None
     
-    def encrypt(self, msg):
-        pass
-        # public_key = self.get_public_key(self.coordinator_node)
-
-        # encrypted_msg = ck.encrypt(public_key, msg2encrypt)
-
-        # # Each message must have a certificate attached
-        # certificate = self.get_certificate()
-        # encrypted_cert = ck.encrypt(public_key, certificate)
-        # cert_length = len(encrypted_cert).to_bytes(4, 'little')
-        # fullmsg = cert_length+encrypted_cert+encrypted_msg
-    
     def request_analysis(self, coordinator_node):
         """ Sends a request to start an analysis operation to the given coordinator address node.
             Returns (response-code, response-msg) tuple from coordinator node. Raises exception on error. """
         self.coordinator_node = coordinator_node
-        pub_key = Cryptk.key2string(self.ck.get_public_key())
+        pub_key = Crypt.key2string(self.ck.get_public_key())
 
         # Send start analysis request to the coordinator node.
         # If the node is not coordinator then the request is dropped.
-        # Sends its public key as the result will be encrypted 
-        conn = http.client.HTTPConnection(self.coordinator_node, timeout=60)
-        conn.request("GET", "/start_analysis", body=pub_key)
-        resp = conn.getresponse()
-        conn.close()
-        content = resp.read().decode()
-        return (resp.status, content)
+        # Sends its public key as the result will be encrypted
+        r = send_client_request(type="GET", url="/start_analysis", body=pub_key, 
+                                    receiver=self.coordinator_node, timeout=3.0)
+        return r
         
     
     def get_result(self, tries=100, ms=50):
         """ Sends http request to coordinator node for the result of a requestes analysis operation.
-            Returns the result (if received) (response-code, response-msg) tuple, otherwise if not received, returns from last message sent.
-            Raises exception on error.
+            Returns the result (if received) (response-code, response-msg) tuple, otherwise if not received, 
+            returns from last message sent. Raises exception on error.
             Params:
-                @tries  : Max number of get-requests sent until result is ready
+                @tries  : Max number of get-requests sent until giving up
                 @ms     : Sleep in ms between each request try. """
 
         if self.coordinator_node == None:
             raise Exception("No SMC request has been sent to coordinator")
         if tries <= 0 or ms < 0:
             raise Exception("Invalid arguments tries=%d, ms=%d given" % (tries, ms))
 
-        pub_key = Cryptk.key2string(self.ck.get_public_key())
+        pub_key = Crypt.key2string(self.ck.get_public_key())
         response_code = 408
         response_msg = "Response timeout"
 
         # Request the result from coordinator. Asks every @ms until it receives the result.
         for i in range(0, tries):
-            conn = http.client.HTTPConnection(self.coordinator_node, timeout=60)
-            conn.request("GET", "/get_result", body=pub_key)
-            resp = conn.getresponse()
-            conn.close()
-            response_code = resp.status
-            response_msg = resp.read().decode()
+            r = send_client_request(type="GET", url="/get_result", body=pub_key, 
+                                    receiver=self.coordinator_node, timeout=3.0)
+            response_code = r[0]
+            response_msg = r[1]
             if response_code == 200:
                 break
             
             time.sleep(0.001*ms)
         
         return (response_code, response_msg)
```

### Comparing `sneaksmc-0.0.2/sneaksmc/crypt.py` & `sneaksmc-0.0.3/sneaksmc/crypt.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,70 +1,67 @@
 
-""" File containing all cryptk library module for secure multiparty computation over a distributed network. """
+""" File containing all cryption used for secure multiparty computation over a distributed network. """
 
-# ~ Libraries used
-# pip3 install pycrypto
-# pip3 install rsa
 
-# Cryptk/cryptk
 from Crypto.Cipher import AES
 import rsa
 import hashlib
 
 
 
-class Cryptk:
+class Crypt:
     
     key_size = 128
     iv_size = 16
 
     # Privates
     _keystring_magic = ':~:'
     _pad_chr = '\0' # pad msg with this character if needed
     
 
     def __init__(self):
         # Generate new rsa keys
-        public, private = rsa.newkeys(Cryptk.key_size*8) # Multiply by 8 to get size in bits
+        public, private = rsa.newkeys(Crypt.key_size*8) # Multiply by 8 to get size in bits
         self.private_key = private
         self.public_key = public
 
         # Privates
         self._keystring_magic = ':~:'
         self._encrypt_pkey = True # If sender should add its own public key to the blob sent
         
     
     def key2string(key):
         """ Converts key object to string, in order to send it easily over http and reconstruct it on the receiving side. """
         n = key.n
         e = key.e
-        return "%d%s%d" % (n, Cryptk._keystring_magic, e)
+        return "%d%s%d" % (n, Crypt._keystring_magic, e)
     
     def string2key(strkey):
         """ Converts string to key object defined within rsa library """
-        n, e = strkey.split(Cryptk._keystring_magic)
-        return Cryptk.construct_key(int(n), int(e))
+        n, e = strkey.split(Crypt._keystring_magic)
+        return Crypt.construct_key(int(n), int(e))
     
     def get_keysize(self):
-        # Returns key size for public and private key in bytes.
-        return Cryptk.key_size
+        """ Returns key size for public and private key in bytes. """
+        return Crypt.key_size
     
     def get_public_key(self):
+        """ Returns the public key class """
         return self.public_key
 
 
     def generate_key(self, key_size):
         """ Generates new random (usually 16 bytes) symmetric key, unique for each message sent """
         # New symmetric key
         # Length should be either 16, 24, 32 bytes
         # from https://stuvel.eu/python-rsa-doc/usage.html#generating-keys
         return rsa.randnum.read_random_bits(key_size*8) # Multiply by 8 to convert bytes to bits
     
     def construct_key(n, e):
-        # Constructs key object from n and e
+        """ Constructs key object from n and e. """
         return rsa.PublicKey(n, e)
     
 
     def encrypt(self, to_user_pkey, str_msg):
         """ 
         Encryption:
             Generate symmetric key used to crypt the data message.
@@ -73,15 +70,15 @@
         Returns: 
             Public-key-size(4 bytes) + IV + public-key + signature + key + data as a byte stream which has been encrypted to user.
         params:
             @to_user_pkey: users public key
             @msg: msg to encrypt """
         
         # Pad message as it must be a multiple of 16
-        padded_msg = Cryptk.Pad_message(str_msg)
+        padded_msg = Crypt.Pad_message(str_msg)
 
         # Symmetric key used to encrypt/decrypt the message
         symmetric_key = self.generate_key(16) # size must be either 16, 24 or 32 bytes
         sendIV = self.generate_key(16)
 
         AES_obj = AES.new(symmetric_key, AES.MODE_CBC, sendIV)
         encrypted_msg = AES_obj.encrypt(padded_msg.encode("UTF-8"))
@@ -90,68 +87,70 @@
         encrypted_key = rsa.encrypt(symmetric_key, to_user_pkey)
 
         signature = self.sign(str_msg.encode())
 
         # Send own public key with the message as well
         pk = b''
         if self._encrypt_pkey:
-            pk = Cryptk.key2string(self.get_public_key()).encode()
+            pk = Crypt.key2string(self.get_public_key()).encode()
         
         pk_size = len(pk).to_bytes(4, 'little')
 
         return pk_size + sendIV + pk + signature + encrypted_key + encrypted_msg
     
 
     def decrypt(self, cipher):
         """
         Decrypton:
             Decrypt the secret key.
             Decrypt the data message based on the secret key.
+        returns:
+            The decrypted message.
         params:
             @cipher: contains public key size, IV, public-key, signature, encrypted symmetric key and encrypted message, respectively """
 
         # Get sizes in bytes
-        iv_size = Cryptk.iv_size
+        iv_size = Crypt.iv_size
         keysize = self.get_keysize()
 
         # Retrieve data from stream
         pk_size = int.from_bytes(cipher[:4], 'little') # First 4 bytes is the size of the senders public key (key size varies so sending the size is needed)
         recvIV = cipher[4:iv_size+4]
         senders_pkey = cipher[iv_size+4:pk_size+iv_size + 4]
         signature = cipher[4+pk_size+iv_size:pk_size + iv_size + keysize+4]
         encrypted_key = cipher[4+pk_size + iv_size + keysize:pk_size + iv_size + keysize*2 + 4]
         encrypted_msg = cipher[4 + pk_size + iv_size + keysize*2:]
 
         if self._encrypt_pkey:
-            senders_pkey = Cryptk.string2key(senders_pkey.decode())
+            senders_pkey = Crypt.string2key(senders_pkey.decode())
 
         symmetric_key = rsa.decrypt(encrypted_key, self.private_key)
 
         AES_obj = AES.new(symmetric_key, AES.MODE_CBC, recvIV)
         msg = AES_obj.decrypt(encrypted_msg)
         # Remove padding on message
-        msg = Cryptk.Remove_pad(msg.decode())
+        msg = Crypt.Remove_pad(msg.decode())
 
         # Verify message authentication from sender
         # This is to make sure the message has not been altered during transmission
         self.verify(senders_pkey, msg.encode(), signature)
 
         return msg
     
     def Pad_message(msg):
         """ Pad message to a multiple of 16 bytes. Returns the padded message. """
         # Pads message with '*'
         length = len(msg)
         pad = abs(length%(-16)) + length
-        return msg.ljust(pad, Cryptk._pad_chr)
+        return msg.ljust(pad, Crypt._pad_chr)
 
     
     def Remove_pad(msg):
         """ Remove message padding if any. Returns the non padded message """
-        ls = msg.split(Cryptk._pad_chr)
+        ls = msg.split(Crypt._pad_chr)
         if len(ls) > 1:
             # In case the msg contains any '_pad_chr' that isn't padded,
             # we only remove the last sequence of '_pad_chr'
             del ls[-1]
             sumls = ""
             for i in ls:
                 sumls += i
```

### Comparing `sneaksmc-0.0.2/sneaksmc/server.py` & `sneaksmc-0.0.3/sneaksmc/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 from os import getcwd
 
 # Since we run this server as its own script, we have to add it to path...
 import sys
 import os
 SCRIPT_DIR = os.path.dirname(os.path.abspath(__file__))
 sys.path.append(os.path.dirname(SCRIPT_DIR))
-#from smccryptk import Cryptk
-from .crypt import Cryptk
+from .crypt import Crypt
 
 
 
 __location__ = os.path.realpath(os.path.join(os.getcwd(), os.path.dirname(__file__)))
 # Certificate file is a file that is only used by the coordinator node.
 # It consists of all the other node's certificates (ip address + public key).
 certificate_file = __location__+"/.certificates.txt"
@@ -29,15 +28,15 @@
 _server_auto_shutdown = 60*60*128            # seconds until automatic shutdown
 _server_ip = None
 _server_port = None
 _server_address = None
 _server_nodefile = None
 _server_iscoordinator = False
 _server_coordinator_addr = None
-ck = Cryptk()
+ck = Crypt()
 # Latest analysis result stored here
 _result_value = None
 # Offset that the coordinator sets on result to make sure no other nodes can read it.
 _analysis_offset_value = None
 
 _analysis_function = None
 _request_timeout_sec = 3
@@ -254,15 +253,15 @@
                 print(cert)
                 f.write(cert+"\n")
 
     
 
     def get_certificate(self):
         """ Returns this nodes certificate in string format consisting of ip, port and public-key (ip:port@publickey). """
-        key = Cryptk.key2string(ck.get_public_key())
+        key = Crypt.key2string(ck.get_public_key())
         return "%s:%d@%s" % (_server_ip, _server_port, key)
 
     def send_whole_response(self, code, content, content_type="text/plain"):
         """ Function to easily and correctly sending a response back after having received a request. """
 
         if isinstance(content, str):
             content = content.encode("utf-8")
@@ -320,15 +319,15 @@
     def init_public_key(self, ip):
         """ Requests the public key from ip address given. The key is then stored in a list to cache it. """
         status, content = self.send_client_request(url="/get_public_key", receiver=ip)
         if status != 200 or status == None:
             self.send_whole_response(400, "error")
             raise Exception("Could not get key with status %d" % (status))
 
-        public_key = Cryptk.string2key(content)
+        public_key = Crypt.string2key(content)
         print("Received public key: %s from ip: %s" % (str(public_key), ip))
         # Update connected ip list with public key
         for i in range(len(_server_connected_ips)):
             ipx, _ = _server_connected_ips[i]
             if ipx == ip:
                 _server_connected_ips[i] = (ip, public_key)
                 break
@@ -460,15 +459,15 @@
         # Have an exception list for validate requests
         #msg = self.validate_request(except_urls)
 
         if self.path.startswith("/invalid-certificate"):
             self.handle_invalid_certificate()
 
         elif self.path.startswith("/get_public_key"):
-            s = Cryptk.key2string(ck.get_public_key())
+            s = Crypt.key2string(ck.get_public_key())
             self.send_whole_response(200, s)
         
         elif self.path.startswith("/send_test"):
             #content_len = int(self.headers.get('Content-Length'))
             print(_server_connected_ips)
             self.send_encrypted_msg("0")
             self.send_whole_response(200, "ok")
@@ -530,15 +529,15 @@
 
             # Add all nodes from certificate-file into a list with address and their public key
             node_list = []
             with open(certificate_file, "r") as f:
                 for line in f.readlines():
                     print(line)
                     addr, strkey = line.split("@")
-                    node_list.append((addr, Cryptk.string2key(strkey)))
+                    node_list.append((addr, Crypt.string2key(strkey)))
             
             # Shuffle the node list to make the order random
             # TODO: ensure that the coordinator is not the first in the list,
             # Otherwise it would result in error as it tries to send to itself (sends to first node in list)
             random.shuffle(node_list)
 
             # Encrypt for each node who they should further their results to. The last node will further it back to the coordinator.
@@ -604,13 +603,11 @@
 
 if __name__ == "__main__":
     parser = arg_parser()
     args = parser.parse_args()
     n = args.nodefile
     i = args.server_ip
     p = args.port
-    print("n: %s, i: %s, p: %s" % (n,i,p))
     run_server(analysis_function=analysis, nodefile=n, ip=i, port=p, coordinator=args.coordinator)
-    #run_server(args.server_ip, args.port, args.coordinator, args.nodefile)
```

