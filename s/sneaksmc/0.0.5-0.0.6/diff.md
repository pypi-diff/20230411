# Comparing `tmp/sneaksmc-0.0.5.tar.gz` & `tmp/sneaksmc-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sneaksmc-0.0.5.tar", last modified: Tue Apr 11 18:46:29 2023, max compression
+gzip compressed data, was "sneaksmc-0.0.6.tar", last modified: Tue Apr 11 20:25:21 2023, max compression
```

## Comparing `sneaksmc-0.0.5.tar` & `sneaksmc-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-11 18:46:29.077136 sneaksmc-0.0.5/
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      268 2023-04-11 18:46:29.077136 sneaksmc-0.0.5/PKG-INFO
--rw-rw-r--   0 tsy       (1000) tsy       (1000)       79 2023-04-11 13:58:02.000000 sneaksmc-0.0.5/README.rst
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      107 2023-04-11 18:46:29.077136 sneaksmc-0.0.5/setup.cfg
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      407 2023-04-11 18:45:03.000000 sneaksmc-0.0.5/setup.py
-drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-11 18:46:29.077136 sneaksmc-0.0.5/sneaksmc/
--rw-rw-r--   0 tsy       (1000) tsy       (1000)       73 2023-04-11 13:54:48.000000 sneaksmc-0.0.5/sneaksmc/__init__.py
--rw-rw-r--   0 tsy       (1000) tsy       (1000)     3461 2023-04-11 13:50:50.000000 sneaksmc-0.0.5/sneaksmc/client.py
--rw-rw-r--   0 tsy       (1000) tsy       (1000)     6390 2023-04-11 13:50:17.000000 sneaksmc-0.0.5/sneaksmc/crypt.py
--rw-rw-r--   0 tsy       (1000) tsy       (1000)    25031 2023-04-11 18:44:11.000000 sneaksmc-0.0.5/sneaksmc/server.py
-drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-11 18:46:29.077136 sneaksmc-0.0.5/sneaksmc.egg-info/
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      268 2023-04-11 18:46:28.000000 sneaksmc-0.0.5/sneaksmc.egg-info/PKG-INFO
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      265 2023-04-11 18:46:29.000000 sneaksmc-0.0.5/sneaksmc.egg-info/SOURCES.txt
--rw-rw-r--   0 tsy       (1000) tsy       (1000)        1 2023-04-11 18:46:28.000000 sneaksmc-0.0.5/sneaksmc.egg-info/dependency_links.txt
--rw-rw-r--   0 tsy       (1000) tsy       (1000)       13 2023-04-11 18:46:28.000000 sneaksmc-0.0.5/sneaksmc.egg-info/requires.txt
--rw-rw-r--   0 tsy       (1000) tsy       (1000)        9 2023-04-11 18:46:28.000000 sneaksmc-0.0.5/sneaksmc.egg-info/top_level.txt
+drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-11 20:25:21.782092 sneaksmc-0.0.6/
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      268 2023-04-11 20:25:21.782092 sneaksmc-0.0.6/PKG-INFO
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)       79 2023-04-11 13:58:02.000000 sneaksmc-0.0.6/README.rst
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      107 2023-04-11 20:25:21.782092 sneaksmc-0.0.6/setup.cfg
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      407 2023-04-11 20:25:02.000000 sneaksmc-0.0.6/setup.py
+drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-11 20:25:21.782092 sneaksmc-0.0.6/sneaksmc/
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)       73 2023-04-11 13:54:48.000000 sneaksmc-0.0.6/sneaksmc/__init__.py
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)     3461 2023-04-11 13:50:50.000000 sneaksmc-0.0.6/sneaksmc/client.py
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)     6390 2023-04-11 13:50:17.000000 sneaksmc-0.0.6/sneaksmc/crypt.py
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)    23642 2023-04-11 20:23:45.000000 sneaksmc-0.0.6/sneaksmc/server.py
+drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-11 20:25:21.782092 sneaksmc-0.0.6/sneaksmc.egg-info/
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      268 2023-04-11 20:25:21.000000 sneaksmc-0.0.6/sneaksmc.egg-info/PKG-INFO
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      265 2023-04-11 20:25:21.000000 sneaksmc-0.0.6/sneaksmc.egg-info/SOURCES.txt
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)        1 2023-04-11 20:25:21.000000 sneaksmc-0.0.6/sneaksmc.egg-info/dependency_links.txt
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)       13 2023-04-11 20:25:21.000000 sneaksmc-0.0.6/sneaksmc.egg-info/requires.txt
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)        9 2023-04-11 20:25:21.000000 sneaksmc-0.0.6/sneaksmc.egg-info/top_level.txt
```

### Comparing `sneaksmc-0.0.5/sneaksmc/client.py` & `sneaksmc-0.0.6/sneaksmc/client.py`

 * *Files identical despite different names*

### Comparing `sneaksmc-0.0.5/sneaksmc/crypt.py` & `sneaksmc-0.0.6/sneaksmc/crypt.py`

 * *Files identical despite different names*

### Comparing `sneaksmc-0.0.5/sneaksmc/server.py` & `sneaksmc-0.0.6/sneaksmc/server.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,49 +2,45 @@
 import json
 import signal
 import socketserver
 import threading
 import argparse
 import random
 from http.server import BaseHTTPRequestHandler,HTTPServer
-import http.client
 from os import getcwd
-
-# Since we run this server as its own script, we have to add it to path...
-#import sys
 import os
-#SCRIPT_DIR = os.path.dirname(os.path.abspath(__file__))
-#sys.path.append(os.path.dirname(SCRIPT_DIR))
 from .crypt import Crypt
-
-
+from .client import send_client_request
 
 __location__ = os.path.realpath(os.path.join(os.getcwd(), os.path.dirname(__file__)))
 # Certificate file is a file that is only used by the coordinator node.
 # It consists of all the other node's certificates (ip address + public key).
 certificate_file = __location__+"/.certificates.txt"
 
 
 _server_connected_ips = []              # List to cache ips/addresses of other nodes in the distributed network
-_server_auto_shutdown = 60*60*128            # seconds until automatic shutdown
+_server_auto_shutdown = 60*60*128       # seconds until automatic shutdown
 _server_ip = None
 _server_port = None
 _server_address = None
 _server_nodefile = None
 _server_iscoordinator = False
 _server_coordinator_addr = None
 ck = Crypt()
 # Latest analysis result stored here
 _result_value = None
 # Offset that the coordinator sets on result to make sure no other nodes can read it.
-_analysis_offset_value = None
+scramble_list = []
 
 _analysis_function = None
 _request_timeout_sec = 3
 
+def get_scramble():
+    return random.randint(-1000000, 1000000)
+
 def get_machine_info():
     """ Returns machine host name and public ip. If no public ip is found 
         then returns ip as localhost (127.0.0.1)"""
 
     import socket
     s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     s.settimeout(0)
@@ -217,38 +213,30 @@
 
                 r.append((line, None)) # None is just empty space atm but will be the public key
         return r
 
     def request_certificate(addr):
         """ Request certificate from address given. Returns the certificate on success otherwise None. """
         try:
-            conn = http.client.HTTPConnection(addr, timeout=_request_timeout_sec)
-            conn.request("GET", "/certificate")
-            resp = conn.getresponse()
-            conn.close()
-            content = resp.read().decode()
-
-            if resp.status != 200:
-                print("Could not get certificate from %s, status code: %d" % (addr, resp.status))
+            status, content = send_client_request(type="GET", url="/certificate", receiver=addr, timeout=_request_timeout_sec)
+            if status != 200:
+                print("Could not get certificate from %s, status code: %d" % (addr, status))
                 return None
 
             return content
 
         except Exception as e:
             print(e)
         
         return None
 
     def request_nodelist_certificates():
         """ Initialize certificate file. 
             Requests the certificate for each node in the nodefile given (whitelist). """
 
-        # TODO: check if file already exist. This means that coordinator node has been restarted and the other nodes 
-        #       has already sent its certificate to this node.
-
         with open(certificate_file, "w") as f:
             for addr, _ in _server_connected_ips:
                 cert = Smcserver.request_certificate(addr)
                 if cert is None:
                     # Something went wrong getting this nodes certificate
                     continue
                 print(cert)
@@ -280,50 +268,32 @@
             content_type = "application/json"
 
         self.send_response(code)
         self.send_header('Content-type', content_type)
         self.send_header('Content-length',len(content))
         self.end_headers()
         self.wfile.write(content)
-
-
-    def send_client_request(self, type="GET", url="empty", body_="", receiver=""):
-        """ Function to easily send a request to another node/server. This node would then act as a client thats sends a request. """
-        try:
-            conn = http.client.HTTPConnection(receiver, timeout=_request_timeout_sec)
-            conn.request(type, url, body=body_)
-            resp = conn.getresponse()
-            conn.close()
-            content = resp.read().decode()
-
-            return resp.status, content
-
-        except Exception as e:
-            print(e)
-        
-        return None, None
     
     def get_public_key(self, ip):
         """ Checks if the public key from given ip address has already been cached. Otherwise calls init_public_key()
             which eventually returns its public key. """
         for i in range(len(_server_connected_ips)):
             ipx, publickey = _server_connected_ips[i]
             if ipx == ip:
                 if publickey == None:
                     publickey = self.init_public_key(ip)
                 return publickey
         
         # This ip is not stored previously (typically client), so it should be added
-        # TODO: add this ip to _server_connected_ips
         return self.init_public_key(ip)
                 
 
     def init_public_key(self, ip):
         """ Requests the public key from ip address given. The key is then stored in a list to cache it. """
-        status, content = self.send_client_request(url="/get_public_key", receiver=ip)
+        status, content = send_client_request(url="/get_public_key", receiver=ip)
         if status != 200 or status == None:
             self.send_whole_response(400, "error")
             raise Exception("Could not get key with status %d" % (status))
 
         public_key = Crypt.string2key(content)
         print("Received public key: %s from ip: %s" % (str(public_key), ip))
         # Update connected ip list with public key
@@ -332,14 +302,16 @@
             if ipx == ip:
                 _server_connected_ips[i] = (ip, public_key)
                 break
 
         return public_key
     
     def create_encrypted_msg(self, msg2encrypt, ip):
+        """ Encrypts the message to the given ip address (node).
+            Attaches this nodes certificate to the message as well. """
         public_key = self.get_public_key(ip)
 
         encrypted_msg = ck.encrypt(public_key, msg2encrypt)
 
         # Each message must have a certificate attached
         certificate = self.get_certificate()
         encrypted_cert = ck.encrypt(public_key, certificate)
@@ -347,24 +319,23 @@
         fullmsg = cert_length+encrypted_cert+encrypted_msg
         return fullmsg
     
     def send_encrypted_msg(self, msg, url="/add", ip=None):
         """ Encrypts the given msg to the given ip (using their public key) and sends the encrypted message. """
 
         fullmsg = self.create_encrypted_msg(msg, ip)
-
-        status, response = self.send_client_request(type="POST", url=url, body_=fullmsg, receiver=ip)
+        status, response = send_client_request(type="POST", url=url, body=fullmsg, receiver=ip)
 
         if status != 200:
             raise Exception("Status code was not 200 when sending encrypted msg to (%s), status code: %d response: %s" % (ip, status, response))
 
         return status, response
 
     def decrypt_msg(self, data=None):
-        """ Returns the message decrypted. """
+        """ Returns the message decrypted and the senders certificate decrypted. """
         
         if data == None:
             content_length = int(self.headers.get('Content-Length'))
             data = self.rfile.read(content_length)
 
         cert_size = int.from_bytes(data[:4], 'little')+4
         certificate = data[4:cert_size]
@@ -392,63 +363,61 @@
             certificate, decrypted_msg = msg
             self.handle_invalid_certificate(certificate, decrypted_msg)
 
         elif self.path.startswith("/analysis_done"):
             global _result_value, _analysis_offset_value
 
             print("got analysis done")
-            #data_dict = self.decrypt_msg()
             data_dict = json.loads(msg)
-            data_value = data_dict['data']
-            # Write result to text file which makes it easy for coordinator to read and retrieve the result.
-            with open("result.txt", "w") as f:
-                f.write(str(data_value))
-
-            _result_value = str(data_value - _analysis_offset_value)
+            result = data_dict['data']
+            # Remove all scrambles from result
+            for scramble in scramble_list:
+                result -= scramble
+            # Save result value
+            _result_value = str(result)
             self.send_whole_response(200, "ok")
         
         elif self.path.startswith("/analysis"):
             print("Received analysis request")
             self.send_whole_response(200, "ok")
 
-            # Decrypt the message
-            #data = self.decrypt_msg()
-
             # The decrypted message will be a dictonary in string format.
             # It must be converted back from string to dictionary.
             dict = json.loads(msg)
 
             # The dictionary will then contain the next set of instructions (who to further the results to)
             # which the coordinator node has encrypted for this node only.
             send_list = dict['send_list']
             # Pop itself from the send list, as it has been received
-            sendto_ip = send_list.pop(0)
+            msg = send_list.pop(0)
             # Decrypt this data in order to get the ip address of who to send the remaining list + analysis-result to.
-            #sendto_ip = self.decrypt_msg(data=sendto_ip.encode('latin-1'))
-            certificate, sendto_ip = self.decrypt_msg(data=sendto_ip.encode('latin-1'))
+            certificate, msg = self.decrypt_msg(data=msg.encode('latin-1'))
+            
+            # Convert string back to dictionary
+            msg = json.loads(msg)
+            scramble = msg['scramble']
+            sendto_ip = msg['next']
 
+            # Validate the coordinators certificate before we trust the msg received
             if not self.validate_certificate(certificate):
                 self.handle_invalid_certificate(certificate)
                 return
 
             print("msg received: " + sendto_ip)
 
             # Perform the analysis function on this nodes data and update the analysis value 'data' in the dictionary.
-            # TODO: Call an analysis function that has been overriden by user which updates the data value in the dictionary.
-            dict['data'] = _analysis_function(dict['data'])
+            dict['data'] = _analysis_function(dict['data']) + scramble
 
             # Dump the dictionary back to string in order to send it over the internet to the next node.
             s = json.dumps(dict)
             print(s)
 
-            # Send back
-            # If list is empty, send analysis-done url
-            # Check if its the last node in the list.
-            # Last node will send the result to coordinator.
-            url = "/analysis_done" if len(send_list) == 0 else "/analysis"
+            # Further the result
+            # send /analysis_done url if next node is the coordinator, otherwise send /analysis
+            url = "/analysis_done" if sendto_ip == _server_coordinator_addr else "/analysis"
             self.send_encrypted_msg(s, url=url, ip=sendto_ip)
 
 
 
     def do_GET(self):
         global _result_value, _server_iscoordinator
 
@@ -504,76 +473,77 @@
             #     raise Exception("Connected node %s is not whitelisted within nodefile for coordinator" % str(self.client_address))
 
             self.send_whole_response(200, self.get_certificate())
            
         
         elif self.path.startswith("/start_analysis"):
             """ Start analysis request. Only coordinator will receive this request from a client. """
-            global _analysis_offset_value
+            global scramble_list
 
             if not _server_iscoordinator:
                 self.send_whole_response(404, "Only coordinator should get a start_analysis request")
                 return
 
 
             content_length = int(self.headers.get('content-length', 0))
             value = self.rfile.read(content_length).decode()
 
             # Send a dictionary containing encrypted list of receivers (send_list)
             # and some analysis data sum (data) which is initialized with a given offset such that no node can know the current data sum.
             enc = []
-            _analysis_offset_value = random.randint(-1000000, 1000000)
-            enc_dict = {'send_list': enc, 'data': _analysis_offset_value}
+            # List of encrypted scramble values to each participant to hide their result
+            # from other nodes.
+            enc_dict = {'send_list': enc, 'data': 0}
 
             # Create sequence list of nodes to perform analysis of its data
             # This is such that the nodes know which node to forward the data to.
-            # TODO: fix this if any special order is needed or shuffle the node list
 
             # Add all nodes from certificate-file into a list with address and their public key
             node_list = []
             with open(certificate_file, "r") as f:
                 for line in f.readlines():
                     print(line)
                     addr, strkey = line.split("@")
                     node_list.append((addr, Crypt.string2key(strkey)))
             
             # Shuffle the node list to make the order random
-            # TODO: ensure that the coordinator is not the first in the list,
-            # Otherwise it would result in error as it tries to send to itself (sends to first node in list)
             random.shuffle(node_list)
 
             # Encrypt for each node who they should further their results to. The last node will further it back to the coordinator.
             for i in range(len(node_list)):
                 addr, key = node_list[i]
                 print(addr)
                 # Last node sends back to coordinator again (loops around)
                 if i >= len(node_list)-1:
-                    # TODO: should encrypt with coordinator's certificate here as well.
-                    #msg = ck.encrypt(key, _server_address)
-                    msg = self.create_encrypted_msg(_server_address, addr)
+                    scramble = get_scramble()
+                    scramble_list.append(scramble)
+                    msg = {'next': _server_address, 'scramble': scramble}
+                    msg = json.dumps(msg)
+                    msg = self.create_encrypted_msg(msg, addr)
                     enc.append(msg.decode('latin-1'))
                     break
                 
                 # Set it to the next node in the list
                 sendto_ip, _ = node_list[i+1]
-                # TODO: remove key in loop, as it's not needed anymore
-                msg = self.create_encrypted_msg(sendto_ip, addr)
-                #msg = ck.encrypt(key, sendto_ip)
+                scramble = get_scramble()
+                scramble_list.append(scramble)
+                msg = {'next': sendto_ip, 'scramble': scramble}
+                # Convert to string
+                msg = json.dumps(msg)
+                msg = self.create_encrypted_msg(msg, addr)
                 enc.append(msg.decode('latin-1'))
 
             # Dump the dictionary to string such that it can be sent over http
             order = json.dumps(enc_dict)
 
             # Send the string dictionary to the first node in the list.
             first_node, first_node_public_key = node_list[0]
 
             status, content = self.send_encrypted_msg(order, url="/analysis", ip=first_node)
 
-            #order = ck.encrypt(first_node_public_key, order)
-            #status, content = self.send_client_request(type="POST", url="/analysis", body_=order, receiver=first_node)
             if status != 200:
                 self.send_whole_response(404, "Error occurred: %s" % content)
                 raise Exception("Error starting analysis: %s" % content)
 
             # Send ok response back to client.
             # The client have to ask for the result in a separate request.
             self.send_whole_response(200, "ok")
```

