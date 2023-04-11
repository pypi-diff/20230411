# Comparing `tmp/rdoclient-1.4.3.tar.gz` & `tmp/rdoclient-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdoclient-1.4.3.tar", last modified: Mon Jul 18 10:35:55 2022, max compression
+gzip compressed data, was "rdoclient-1.5.0.tar", last modified: Tue Apr 11 16:14:46 2023, max compression
```

## Comparing `rdoclient-1.4.3.tar` & `rdoclient-1.5.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-07-18 10:35:55.190806 rdoclient-1.4.3/
--rw-rw-rw-   0        0        0     1096 2022-07-18 10:10:40.000000 rdoclient-1.4.3/LICENSE
--rw-rw-rw-   0        0        0     5197 2022-07-18 10:35:55.185984 rdoclient-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     4142 2022-07-18 10:10:40.000000 rdoclient-1.4.3/README.rst
-drwxrwxrwx   0        0        0        0 2022-07-18 10:35:55.160768 rdoclient-1.4.3/rdoclient/
--rw-rw-rw-   0        0        0     3587 2022-07-18 10:24:11.000000 rdoclient-1.4.3/rdoclient/__init__.py
--rw-rw-rw-   0        0        0   142279 2022-07-18 10:26:53.000000 rdoclient-1.4.3/rdoclient/rdoclient.py
-drwxrwxrwx   0        0        0        0 2022-07-18 10:35:55.183951 rdoclient-1.4.3/rdoclient.egg-info/
--rw-rw-rw-   0        0        0     5197 2022-07-18 10:35:55.000000 rdoclient-1.4.3/rdoclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2022-07-18 10:35:55.000000 rdoclient-1.4.3/rdoclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-18 10:35:55.000000 rdoclient-1.4.3/rdoclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2022-07-18 10:35:55.000000 rdoclient-1.4.3/rdoclient.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-07-18 10:35:55.000000 rdoclient-1.4.3/rdoclient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-07-18 10:35:55.190806 rdoclient-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1408 2022-07-18 10:24:03.000000 rdoclient-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 16:14:46.969122 rdoclient-1.5.0/
+-rw-rw-rw-   0        0        0     1096 2022-07-18 10:10:40.000000 rdoclient-1.5.0/LICENSE
+-rw-rw-rw-   0        0        0     5277 2023-04-11 16:14:46.967905 rdoclient-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4118 2023-04-11 15:05:31.000000 rdoclient-1.5.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-11 16:14:46.951663 rdoclient-1.5.0/rdoclient/
+-rw-rw-rw-   0        0        0     3875 2023-04-11 14:56:57.000000 rdoclient-1.5.0/rdoclient/__init__.py
+-rw-rw-rw-   0        0        0   146434 2023-04-11 15:04:29.000000 rdoclient-1.5.0/rdoclient/rdoclient.py
+drwxrwxrwx   0        0        0        0 2023-04-11 16:14:46.966913 rdoclient-1.5.0/rdoclient.egg-info/
+-rw-rw-rw-   0        0        0     5277 2023-04-11 16:14:46.000000 rdoclient-1.5.0/rdoclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-04-11 16:14:46.000000 rdoclient-1.5.0/rdoclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 16:14:46.000000 rdoclient-1.5.0/rdoclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-11 16:14:46.000000 rdoclient-1.5.0/rdoclient.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-11 16:14:46.000000 rdoclient-1.5.0/rdoclient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 16:14:46.969122 rdoclient-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1510 2023-04-11 15:57:30.000000 rdoclient-1.5.0/setup.py
```

### Comparing `rdoclient-1.4.3/LICENSE` & `rdoclient-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rdoclient-1.4.3/PKG-INFO` & `rdoclient-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdoclient
-Version: 1.4.3
+Version: 1.5.0
 Summary: The official RANDOM.ORG JSON-RPC API (Release 4) implementation for Python 2 and 3.
 Home-page: https://www.random.org/
 Author: RANDOM.ORG
 Author-email: contact@random.org
 License: MIT
 Project-URL: Documentation, https://api.random.org/json-rpc/4
 Project-URL: Source Code, https://github.com/RandomOrg/JSON-RPC-Python
@@ -14,14 +14,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
 License-File: LICENSE
 
 JSON-RPC-Python
 ===============
 
@@ -47,15 +49,15 @@
 Requires the `six <https://six.readthedocs.io/>`_ lib:
 
 .. code-block:: bash
 
     $ pip install six
 
 
-Note that the required dependencies 'requests' and 'six' are installed automatically, when using pip install for 'rdoclient' version >= 1.2 (Update: November 2020).  
+Note that the required dependencies 'requests' and 'six' are installed automatically, when using pip install for 'rdoclient' version >= 1.2.  
 
 Usage
 -----
 
 The default setup is best for non-time-critical serialized requests, e.g., batch clients:
 
 .. code-block:: pycon
```

### Comparing `rdoclient-1.4.3/README.rst` & `rdoclient-1.5.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 Requires the `six <https://six.readthedocs.io/>`_ lib:
 
 .. code-block:: bash
 
     $ pip install six
 
 
-Note that the required dependencies 'requests' and 'six' are installed automatically, when using pip install for 'rdoclient' version >= 1.2 (Update: November 2020).  
+Note that the required dependencies 'requests' and 'six' are installed automatically, when using pip install for 'rdoclient' version >= 1.2.  
 
 Usage
 -----
 
 The default setup is best for non-time-critical serialized requests, e.g., batch clients:
 
 .. code-block:: pycon
```

### Comparing `rdoclient-1.4.3/rdoclient/__init__.py` & `rdoclient-1.5.0/rdoclient/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,33 +44,37 @@
     [3, 5, 2, 4, 8]
 
 For a full list of available randomness generation functions see 
 rdoclient.py documentation and https://api.random.org/json-rpc/4
 """
 
 __title__ = 'rdoclient'
-__version__ = '1.4.3'
+__version__ = '1.5.0'
 __build__ = 0x010000
 __author__ = 'RANDOM.ORG'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2014 RANDOM.ORG'
 
 from .rdoclient import (RandomOrgClient, RandomOrgCache, RandomOrgSendTimeoutError, 
                         RandomOrgKeyNonExistentError, RandomOrgKeyNotRunningError, 
                         RandomOrgInsufficientRequestsError, RandomOrgInsufficientBitsError, 
                         RandomOrgKeyInvalidAccessError, RandomOrgKeyInvalidVersionError, 
                         RandomOrgTicketNonExistentError, RandomOrgTicketAPIKeyMismatchError, 
-                        RandomOrgTicketAlreadyUsedError, RandomOrgTooManySingletonTicketsError)
+                        RandomOrgTicketAlreadyUsedError, RandomOrgTooManySingletonTicketsError,
+                        RandomOrgTicketNotYetUsedError, RandomOrgLicenseDataRequiredError,
+                        RandomOrgLicenseDataNotAllowedError)
 
 __all__ = [ 'RandomOrgClient', 'RandomOrgCache', 'RandomOrgSendTimeoutError', 
            'RandomOrgKeyNonExistentError', 'RandomOrgKeyNotRunningError', 
            'RandomOrgInsufficientRequestsError', 'RandomOrgInsufficientBitsError', 
            'RandomOrgKeyInvalidAccessError', 'RandomOrgKeyInvalidVersionError', 
            'RandomOrgTicketNonExistentError', 'RandomOrgTicketAPIKeyMismatchError', 
-           'RandomOrgTicketAlreadyUsedError', 'RandomOrgTooManySingletonTicketsError' ]
+           'RandomOrgTicketAlreadyUsedError', 'RandomOrgTooManySingletonTicketsError',
+           'RandomOrgTicketNotYetUsedError', 'RandomOrgLicenseDataRequiredError',
+           'RandomOrgLicenseDataNotAllowedError' ]
 
 import logging
 
 try:
     from logging import NullHandler
 except ImportError:
     class NullHandler(logging.Handler):
```

### Comparing `rdoclient-1.4.3/rdoclient/rdoclient.py` & `rdoclient-1.5.0/rdoclient/rdoclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,15 @@
 _SIGNED_DECIMAL_FRACTION_METHOD  = 'generateSignedDecimalFractions'
 _SIGNED_GAUSSIAN_METHOD          = 'generateSignedGaussians'
 _SIGNED_STRING_METHOD            = 'generateSignedStrings'
 _SIGNED_UUID_METHOD              = 'generateSignedUUIDs'
 _SIGNED_BLOB_METHOD              = 'generateSignedBlobs'
 _GET_RESULT_METHOD               = 'getResult'
 _CREATE_TICKETS_METHOD           = 'createTickets'
+_REVEAL_TICKETS_METHOD           = 'revealTickets'
 _LIST_TICKETS_METHOD             = 'listTickets'
 _GET_TICKET_METHOD               = 'getTicket'
 _VERIFY_SIGNATURE_METHOD         = 'verifySignature'
 
 # Blob format literals
 _BLOB_FORMAT_BASE64              = 'base64'
 _BLOB_FORMAT_HEX                 = 'hex'
@@ -194,14 +195,23 @@
     RandomOrgClient key has reached the maximum number 
     of singleton tickets allowed. 
     
     Exception raised by the RandomOrgClient class when the maximum 
     number of singleton tickets associated with the API key specified 
     has been reached. 
     """
+    
+class RandomOrgTicketNotYetUsedError(Exception):
+    """
+    RandomOrgClient ticket has not yet been used.
+    
+    Exception raised by the RandomOrgClient class when the ticket
+    specified in the reveal_tickets method has not yet been used
+    to generate values. 
+    """
 
 class RandomOrgLicenseDataRequiredError(Exception):
     """
     RandomOrgClient key requires the license data parameter. 
     
     Exception raised by the RandomOrgClient class when the license data 
     parameter of a signed method returning random values is not supplied, 
@@ -1972,15 +1982,81 @@
             true, the full random and signature objects from the response that 
             was used to satisfy the ticket is returned.        
         """
         
         params = { 'apiKey':self._api_key, 'n':n, 'showResult':show_result }
         request = self._generate_request(_CREATE_TICKETS_METHOD, params)
         response = self._send_request(request)
-        return self._extract_tickets(response)
+        return self._extract_result(response)
+    
+    def reveal_tickets(self, ticket_id):
+        """
+        Change the show_result value of a ticket and its predecessors to
+        "True".
+        
+        This method marks a specific ticket and all its predecessors in its
+        chain as being revealed, meaning that subsequent calls to get_ticket
+        will return the full details of the tickets, including the random
+        values produced when the tickets were used. Using reveal_tickets
+        effectively changes the value of show_result (which was specified
+        when the first ticket in the chain was created using create_tickets)
+        from "False" to "True". The reason that not only the ticket specified
+        (but also its predecessors in its chain) are revealed is to ensure
+        maximum transparency. The method does not affect any successors to
+        the ticket in the chain. Returns a number value that specifies how
+        many tickets were revealed. This will include the ticket specified
+        as well as all its predecessors. If this method is invoked on a ticket
+        that is already revealed (or which was created with show_result set
+        to True), then the value returned will be zero. See:
+        https://api.random.org/json-rpc/4/signed#revealTickets
+        
+        Raises a RandomOrgSendTimeoutError if time spent waiting before
+        request is sent exceeds this instance's blocking_timeout.
+        
+        Raises a RandomOrgKeyNonExistentError if this API key does not 
+        exist.
+        
+        Raises a RandomOrgKeyNotRunningError if this API key is stopped. 
+        
+        Raises a RandomOrgInsufficientRequestsError if this API key's 
+        server requests allowance has been exceeded and the instance is
+        backing off until midnight UTC.
+        
+        Raises a RandomOrgInsufficientBitsError if this API key's 
+        server bits allowance has been exceeded.
+        
+        Raises a RandomOrgKeyInvalidAccessError if this API key is not 
+        valid for this method.
+        
+        Raises a RandomOrgKeyInvalidVersionError if this API key is not 
+        valid for the version of the API invoked.
+        
+        Raises a RandomOrgTicketNonExistentError if the ticket used 
+        does not exist.
+        
+        Raises a RandomOrgTicketNotYetUsedError if the ticket specified
+        has not yet been used.
+        
+        Raises a ValueError on RANDOM.ORG Errors, error descriptions:
+        https://api.random.org/json-rpc/4/error-codes
+        
+        Raises a RuntimeError on JSON-RPC Errors, error descriptions:
+        https://api.random.org/json-rpc/4/error-codes
+        
+        Can also raise connection errors as described here:
+        https://requests.readthedocs.io/en/latest/api/#exceptions
+        
+        Keyword arguments:
+        
+        ticket_id -- A string value that uniquely identifies the ticket.
+        """
+        params = { 'apiKey':self._api_key, 'ticketId':ticket_id }
+        request = self._generate_request(_REVEAL_TICKETS_METHOD, params)
+        response = self._send_request(request)
+        return self._extract_result(response)
     
     def list_tickets(self, ticket_type):
         """
         Obtain information about tickets linked with your API key.
         
         This method obtains information about tickets that exist 
         for a given API key. See:
@@ -2025,15 +2101,15 @@
             that do not have a previous ticket but that do have a next ticket. 
             Specifying tail will cause list_tickets to return tickets that have a 
             previous ticket but do not have a next ticket. 
         """
         params = { 'apiKey':self._api_key, 'ticketType':ticket_type }
         request = self._generate_request(_LIST_TICKETS_METHOD, params)
         response = self._send_request(request)
-        return self._extract_tickets(response)
+        return self._extract_result(response)
     
     def get_ticket(self, ticket_id):
         """
         Obtain information about a single ticket. 
         
         This method obtains information about a single ticket. If
         the ticket has showResult set to true and has been used, 
@@ -2078,15 +2154,15 @@
         ticket_id -- A string containing a ticket identifier returned by a prior 
         call to the create_tickets method.
         """
         
         params = { 'ticketId':ticket_id }
         request = self._generate_request(_GET_TICKET_METHOD, params)
         response = self._send_request(request)
-        return self._extract_tickets(response)
+        return self._extract_result(response)
     
     
     # Signature verification for signed methods, see:
     # https://api.random.org/json-rpc/4/signed
     
     def verify_signature(self, random, signature):
         """
@@ -2821,69 +2897,79 @@
                                                        + ': ' + message) }
             
             # RandomOrgKeyInvalidVersionError, key is not valid for the 
             # version of the API you are invoking, from RANDOM.ORG Errors: 
             # https://api.random.org/json-rpc/4/error-codes
             elif code == 405:
                 return { 'exception':
-                        RandomOrgKeyInvalidVersionError('Error' + str(code) 
+                        RandomOrgKeyInvalidVersionError('Error ' + str(code) 
                                                         + ': ' + message)}
             
             # RandomOrgTicketNonExistentError, the ticket specified does
             # not exist, from RANDOM.ORG Errors: 
             # https://api.random.org/json-rpc/4/error-codes 
             elif code == 420:
                 return { 'exception':
-                        RandomOrgTicketNonExistentError('Error' + str(code) 
+                        RandomOrgTicketNonExistentError('Error ' + str(code) 
                                                         + ': ' + message)}
             
             # RandomOrgTicketAPIKeyMismatchError, the ticket specified 
             # exists but is not for the API key you specified, 
             # from RANDOM.ORG Errors: 
             # https://api.random.org/json-rpc/4/error-codes
             elif code == 421:
                 return { 'exception':
-                        RandomOrgTicketAPIKeyMismatchError('Error' + str(code) 
+                        RandomOrgTicketAPIKeyMismatchError('Error ' + str(code) 
                                                            + ': ' + message)}
             
             # RandomOrgTicketAlreadyUsedError, the ticket specified has 
             # already been used, from RANDOM.ORG Errors: 
             # https://api.random.org/json-rpc/4/error-codes
             elif code == 422:
                 return { 'exception':
-                        RandomOrgTicketAlreadyUsedError('Error' + str(code) 
+                        RandomOrgTicketAlreadyUsedError('Error ' + str(code) 
                                                         + ': ' + message)}
             
             # RandomOrgTooManySingletonTicketsError, the maximum number 
             # of singleton tickets available for your API key has been 
             # reached, from RANDOM.ORG Errors: 
             # https://api.random.org/json-rpc/4/error-codes
             elif code == 423:
                 return { 'exception':
-                        RandomOrgTooManySingletonTicketsError('Error' 
+                        RandomOrgTooManySingletonTicketsError('Error ' 
                                                               + str(code) 
                                                               + ': '
                                                               + message)}
     
             # RandomOrgLicenseDataRequiredError, your API key requires the 
             # license_data parameter be used, from RANDOM.ORG Errors:
             # https://api.random.org/json-rpc/4/error-codes
             elif code == 424:
                 return { 'exception':
-                        RandomOrgLicenseDataRequiredError('Error' 
+                        RandomOrgLicenseDataRequiredError('Error ' 
                                                           + str(code) 
                                                           + ': ' + message)}
             
             # RandomOrgLicenseDataNotAllowedError, your API key does not 
             # support the use of the license_data parameter, 
             # from RANDOM.ORG Errors: 
             # https://api.random.org/json-rpc/4/error-codes
             elif code == 425:
                 return { 'exception':
-                        RandomOrgLicenseDataNotAllowedError('Error' 
+                        RandomOrgLicenseDataNotAllowedError('Error ' 
+                                                            + str(code) 
+                                                            + ': ' 
+                                                            + message)}
+                
+            # RandomOrgTicketNotYetUsedError, the ticket you specified has
+            # not yet been used, from RANDOM.ORG Errors: 
+            # https://api.random.org/json-rpc/4/error-codes
+            elif code == 426:
+                return { 'exception':
+                        RandomOrgTicketNotYetUsedError('Error ' 
                                                             + str(code) 
                                                             + ': ' 
                                                             + message)}
              
             # ValueError, error codes listed under RANDOM.ORG Errors:
             # https://api.random.org/json-rpc/4/error-codes
             else:
@@ -2949,16 +3035,17 @@
                     'random':response['result']['random'], 
                     'signature':response['result']['signature']}
         
     def _extract_verification_response(self, response):
         # Gets verification boolean.
         return bool(response['result']['authenticity'])
     
-    def _extract_tickets(self, response):
-        # Gets list of tickets for create_tickets method
+    def _extract_result(self, response):
+        # Gets 'result' property of a return object. Primarily used
+        # for ticket-related methods.
         return response['result']
     
     def _extract_ints(self, response, decimal=True):
         # json to integer list.
         if decimal:
             return list(map(int, self._extract_response(response)))
         else:
```

### Comparing `rdoclient-1.4.3/rdoclient.egg-info/PKG-INFO` & `rdoclient-1.5.0/rdoclient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdoclient
-Version: 1.4.3
+Version: 1.5.0
 Summary: The official RANDOM.ORG JSON-RPC API (Release 4) implementation for Python 2 and 3.
 Home-page: https://www.random.org/
 Author: RANDOM.ORG
 Author-email: contact@random.org
 License: MIT
 Project-URL: Documentation, https://api.random.org/json-rpc/4
 Project-URL: Source Code, https://github.com/RandomOrg/JSON-RPC-Python
@@ -14,14 +14,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
 License-File: LICENSE
 
 JSON-RPC-Python
 ===============
 
@@ -47,15 +49,15 @@
 Requires the `six <https://six.readthedocs.io/>`_ lib:
 
 .. code-block:: bash
 
     $ pip install six
 
 
-Note that the required dependencies 'requests' and 'six' are installed automatically, when using pip install for 'rdoclient' version >= 1.2 (Update: November 2020).  
+Note that the required dependencies 'requests' and 'six' are installed automatically, when using pip install for 'rdoclient' version >= 1.2.  
 
 Usage
 -----
 
 The default setup is best for non-time-critical serialized requests, e.g., batch clients:
 
 .. code-block:: pycon
```

