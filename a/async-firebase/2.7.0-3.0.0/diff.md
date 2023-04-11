# Comparing `tmp/async_firebase-2.7.0.tar.gz` & `tmp/async_firebase-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_firebase-2.7.0.tar", max compression
+gzip compressed data, was "async_firebase-3.0.0.tar", max compression
```

## Comparing `async_firebase-2.7.0.tar` & `async_firebase-3.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1066 2023-04-06 09:24:20.661265 async_firebase-2.7.0/LICENSE
--rw-r--r--   0        0        0     4899 2023-04-06 09:24:20.661265 async_firebase-2.7.0/README.md
--rw-r--r--   0        0        0      194 2023-04-06 09:24:20.661265 async_firebase-2.7.0/async_firebase/__init__.py
--rw-r--r--   0        0        0     7954 2023-04-06 09:24:20.661265 async_firebase-2.7.0/async_firebase/base.py
--rw-r--r--   0        0        0    24099 2023-04-06 09:24:20.661265 async_firebase-2.7.0/async_firebase/client.py
--rw-r--r--   0        0        0     1547 2023-04-06 09:24:20.661265 async_firebase-2.7.0/async_firebase/encoders.py
--rw-r--r--   0        0        0     8142 2023-04-06 09:24:20.661265 async_firebase-2.7.0/async_firebase/errors.py
--rw-r--r--   0        0        0    15976 2023-04-06 09:24:20.661265 async_firebase-2.7.0/async_firebase/messages.py
--rw-r--r--   0        0        0    13053 2023-04-06 09:24:20.661265 async_firebase-2.7.0/async_firebase/utils.py
--rw-r--r--   0        0        0     1677 2023-04-06 09:24:20.661265 async_firebase-2.7.0/pyproject.toml
--rw-r--r--   0        0        0     5875 1970-01-01 00:00:00.000000 async_firebase-2.7.0/setup.py
--rw-r--r--   0        0        0     6365 1970-01-01 00:00:00.000000 async_firebase-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-11 14:48:15.268585 async_firebase-3.0.0/LICENSE
+-rw-r--r--   0        0        0     8292 2023-04-11 14:48:15.268585 async_firebase-3.0.0/README.md
+-rw-r--r--   0        0        0      194 2023-04-11 14:48:15.268585 async_firebase-3.0.0/async_firebase/__init__.py
+-rw-r--r--   0        0        0     7906 2023-04-11 14:48:15.268585 async_firebase-3.0.0/async_firebase/base.py
+-rw-r--r--   0        0        0    22997 2023-04-11 14:48:15.268585 async_firebase-3.0.0/async_firebase/client.py
+-rw-r--r--   0        0        0     1547 2023-04-11 14:48:15.268585 async_firebase-3.0.0/async_firebase/encoders.py
+-rw-r--r--   0        0        0     8142 2023-04-11 14:48:15.268585 async_firebase-3.0.0/async_firebase/errors.py
+-rw-r--r--   0        0        0    16820 2023-04-11 14:48:15.268585 async_firebase-3.0.0/async_firebase/messages.py
+-rw-r--r--   0        0        0    12977 2023-04-11 14:48:15.268585 async_firebase-3.0.0/async_firebase/utils.py
+-rw-r--r--   0        0        0     1677 2023-04-11 14:48:15.268585 async_firebase-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     9394 1970-01-01 00:00:00.000000 async_firebase-3.0.0/setup.py
+-rw-r--r--   0        0        0     9758 1970-01-01 00:00:00.000000 async_firebase-3.0.0/PKG-INFO
```

### Comparing `async_firebase-2.7.0/LICENSE` & `async_firebase-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `async_firebase-2.7.0/README.md` & `async_firebase-3.0.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 ## Installation
 ```shell script
 $ pip install async-firebase
 ```
 
 ## Getting started
+### async-firebase < 3.0.0
 To send push notification to Android:
 ```python3
 import asyncio
 
 from async_firebase import AsyncFirebaseClient
 
 
@@ -143,14 +144,139 @@
     print(response.success)
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
+### async-firebase >= 3.0.0
+To send push notification to Android:
+```python3
+import asyncio
+
+from async_firebase import AsyncFirebaseClient
+from async_firebase.messages import Message
+
+
+async def main():
+    client = AsyncFirebaseClient()
+    client.creds_from_service_account_file("secret-store/mobile-app-79225efac4bb.json")
+
+    # or using dictionary object
+    # client.creds_from_service_account_info({...}})
+
+    device_token: str = "..."
+
+    android_config = client.build_android_config(
+        priority="high",
+        ttl=2419200,
+        collapse_key="push",
+        data={"discount": "15%", "key_1": "value_1", "timestamp": "2021-02-24T12:00:15"},
+        title="Store Changes",
+        body="Recent store changes",
+    )
+    message = Message(android=android_config, token=device_token)
+    response = await client.push(message)
+
+    print(response.success, response.message_id)
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
+
+To send push notification to iOS:
+
+```python3
+import asyncio
+
+from async_firebase import AsyncFirebaseClient
+from async_firebase.messages import Message
+
+
+async def main():
+    client = AsyncFirebaseClient()
+    client.creds_from_service_account_file("secret-store/mobile-app-79225efac4bb.json")
+
+    # or using dictionary object
+    # client.creds_from_service_account_info({...}})
+
+    device_token: str = "..."
+
+    apns_config = client.build_apns_config(
+        priority="normal",
+        ttl=2419200,
+        apns_topic="store-updated",
+        collapse_key="push",
+        title="Store Changes",
+        alert="Recent store changes",
+        badge=1,
+        category="test-category",
+        custom_data={"discount": "15%", "key_1": "value_1", "timestamp": "2021-02-24T12:00:15"}
+    )
+    message = Message(apns=apns_config, token=device_token)
+    response = await client.push(message)
+
+    print(response.success)
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
+
+This prints:
+
+```shell script
+"projects/mobile-app/messages/0:2367799010922733%7606eb557606ebff"
+```
+
+To manual construct message:
+```python3
+import asyncio
+from datetime import datetime
+
+from async_firebase.messages import APNSConfig, APNSPayload, ApsAlert, Aps, Message
+from async_firebase import AsyncFirebaseClient
+
+
+async def main():
+    apns_config = APNSConfig(**{
+        "headers": {
+            "apns-expiration": str(int(datetime.utcnow().timestamp()) + 7200),
+            "apns-priority": "10",
+            "apns-topic": "test-topic",
+            "apns-collapse-id": "something",
+        },
+        "payload": APNSPayload(**{
+            "aps": Aps(**{
+                "alert": ApsAlert(title="some-title", body="alert-message"),
+                "badge": 0,
+                "sound": "default",
+                "content_available": True,
+                "category": "some-category",
+                "mutable_content": False,
+                "custom_data": {
+                    "link": "https://link-to-somewhere.com",
+                    "ticket_id": "YXZ-655512",
+                },
+            })
+        })
+    })
+
+    device_token: str = "..."
+
+    client = AsyncFirebaseClient()
+    client.creds_from_service_account_info({...})
+    message = Message(apns=apns_config, token=device_token)
+    response = await client.push(message)
+    print(response.success)
+
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
+
 ## License
 
 ``async-firebase`` is offered under the MIT license.
 
 ## Source code
 
 The latest developer version is available in a GitHub repository:
```

### Comparing `async_firebase-2.7.0/async_firebase/base.py` & `async_firebase-3.0.0/async_firebase/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 from pathlib import PurePath
 from urllib.parse import urlencode, urljoin
 
 import httpx
 from google.oauth2 import service_account  # type: ignore
 
 import pkg_resources  # type: ignore
-from async_firebase.messages import FcmPushMulticastResponse, FcmPushResponse
+from async_firebase.messages import FCMBatchResponse, FCMResponse
 from async_firebase.utils import (
-    FcmPushMulticastResponseHandler,
-    FcmPushResponseHandler,
+    FCMBatchResponseHandler,
+    FCMResponseHandler,
     serialize_mime_message,
 )
 
 
 class AsyncClientBase:
     """Base asynchronous client"""
 
@@ -147,19 +147,19 @@
             "X-GOOG-API-FORMAT-VERSION": "2",
             "X-FIREBASE-CLIENT": "async-firebase/{0}".format(pkg_resources.get_distribution("async-firebase").version),
         }
 
     async def send_request(
         self,
         uri: str,
-        response_handler: t.Union[FcmPushResponseHandler, FcmPushMulticastResponseHandler],
+        response_handler: t.Union[FCMResponseHandler, FCMBatchResponseHandler],
         json_payload: t.Optional[t.Dict[str, t.Any]] = None,
         headers: t.Optional[t.Dict[str, str]] = None,
         content: t.Union[str, bytes, t.Iterable[bytes], t.AsyncIterable[bytes], None] = None,
-    ) -> t.Union[FcmPushResponse, FcmPushMulticastResponse]:
+    ) -> t.Union[FCMResponse, FCMBatchResponse]:
         """
         Sends an HTTP call using the ``httpx`` library.
 
         :param uri: URI to be requested.
         :param response_handler: the model to handle response.
         :param json_payload: request JSON payload
         :param headers: request headers.
```

### Comparing `async_firebase-2.7.0/async_firebase/client.py` & `async_firebase-3.0.0/async_firebase/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,27 +20,27 @@
 from async_firebase.messages import (
     AndroidConfig,
     AndroidNotification,
     APNSConfig,
     APNSPayload,
     Aps,
     ApsAlert,
-    FcmPushMulticastResponse,
-    FcmPushResponse,
+    FCMBatchResponse,
+    FCMResponse,
     Message,
-    Notification,
+    MulticastMessage,
     PushNotification,
     WebpushConfig,
     WebpushFCMOptions,
     WebpushNotification,
     WebpushNotificationAction,
 )
 from async_firebase.utils import (
-    FcmPushMulticastResponseHandler,
-    FcmPushResponseHandler,
+    FCMBatchResponseHandler,
+    FCMResponseHandler,
     cleanup_firebase_message,
     serialize_mime_message,
 )
 
 DEFAULT_TTL = 604800
 MULTICAST_MESSAGE_MAX_DEVICE_TOKENS = 500
 
@@ -328,152 +328,141 @@
                 timestamp_millis=timestamp_millis,
                 vibrate=vibrate,
                 custom_data=custom_data or {},
             ),
             fcm_options=WebpushFCMOptions(link=link) if link else None,
         )
 
-    async def push(  # pylint: disable=too-many-locals
-        self,
-        device_token: str,
-        *,
-        android: t.Optional[AndroidConfig] = None,
-        apns: t.Optional[APNSConfig] = None,
-        condition: t.Optional[str] = None,
-        data: t.Optional[t.Dict[str, str]] = None,
-        notification: t.Optional[Notification] = None,
-        topic: t.Optional[str] = None,
-        webpush: t.Optional[WebpushConfig] = None,
-        dry_run: bool = False,
-    ) -> FcmPushResponse:
+    async def send(self, message: Message, *, dry_run: bool = False) -> FCMResponse:
         """
         Send push notification.
 
-        :param device_token: device token allows to send targeted notifications to a particular instance of app.
-        :param android: as instance of ``messages.AndroidConfig`` that contains Android-specific options.
-        :param apns: as instance of ``messages.APNSConfig`` that contains iOS-specific options.
-        :param condition: the Firebase condition to which the message should be sent.
-        :param data: a dictionary of data fields. All keys and values in the dictionary must be strings.
-        :param notification: an instance of ``messages.Notification`` that contains a notification that can be included
-            in a resulting message.
-        :param topic: name of the Firebase topic to which the message should be sent.
-        :param webpush: an instance of ``messages.WebpushConfig``.
+        :param message: the message that has to be sent.
         :param dry_run: indicating whether to run the operation in dry run mode (optional). Flag for testing the request
             without actually delivering the message. Default to ``False``.
 
         :raises:
 
-            ValueError is ``messages.PushNotification`` payload cannot be assembled
+            ValueError if ``messages.PushNotification`` payload cannot be assembled
+
+        :return: instance of ``messages.FCMResponse``
 
-        :return: response from Firebase. Example of response:
+            Example of raw response:
 
-            success::
+                success::
 
-                {
-                    'name': 'projects/mobile-app/messages/0:1612788010922733%7606eb247606eb24'
-                }
-
-            failure::
-
-                {
-                    'error': {
-                        'code': 400,
-                        'details': [
-                            {
-                                '@type': 'type.googleapis.com/google.rpc.BadRequest',
-                                'fieldViolations': [
-                                    {
-                                        'description': 'Value type for APS key [badge] is a number.',
-                                        'field': 'message.apns.payload.aps.badge'
-                                    }
-                                ]
-                            },
-                            {
-                                '@type': 'type.googleapis.com/google.firebase.fcm.v1.FcmError',
-                                'errorCode': 'INVALID_ARGUMENT'
-                            }
-                        ],
-                        'message': 'Value type for APS key [badge] is a number.',
-                        'status': 'INVALID_ARGUMENT'
+                    {
+                        'name': 'projects/mobile-app/messages/0:1612788010922733%7606eb247606eb24'
                     }
-                }
-        """
-        message = Message(
-            token=device_token,
-            data=data or {},
-            notification=notification,
-            android=android,
-            webpush=webpush,
-            apns=apns,
-            topic=topic,
-            condition=condition,
-        )
 
-        push_notification = self.assemble_push_notification(apns_config=apns, dry_run=dry_run, message=message)
+                failure::
+
+                    {
+                        'error': {
+                            'code': 400,
+                            'details': [
+                                {
+                                    '@type': 'type.googleapis.com/google.rpc.BadRequest',
+                                    'fieldViolations': [
+                                        {
+                                            'description': 'Value type for APS key [badge] is a number.',
+                                            'field': 'message.apns.payload.aps.badge'
+                                        }
+                                    ]
+                                },
+                                {
+                                    '@type': 'type.googleapis.com/google.firebase.fcm.v1.FcmError',
+                                    'errorCode': 'INVALID_ARGUMENT'
+                                }
+                            ],
+                            'message': 'Value type for APS key [badge] is a number.',
+                            'status': 'INVALID_ARGUMENT'
+                        }
+                    }
+        """
+        push_notification = self.assemble_push_notification(apns_config=message.apns, dry_run=dry_run, message=message)
 
         response = await self.send_request(
             uri=self.FCM_ENDPOINT.format(project_id=self._credentials.project_id),  # type: ignore
             json_payload=push_notification,
-            response_handler=FcmPushResponseHandler(),
+            response_handler=FCMResponseHandler(),
         )
-        if not isinstance(response, FcmPushResponse):
+        if not isinstance(response, FCMResponse):
             raise ValueError("Wrong return type, perhaps because of a response handler misuse.")
         return response
 
-    async def push_multicast(
+    async def send_multicast(
         self,
-        device_tokens: t.Union[t.List[str], t.Tuple[str]],
+        multicast_message: MulticastMessage,
         *,
-        android: t.Optional[AndroidConfig] = None,
-        apns: t.Optional[APNSConfig] = None,
-        data: t.Optional[t.Dict[str, str]] = None,
-        notification: t.Optional[Notification] = None,
-        webpush: t.Optional[WebpushConfig] = None,
         dry_run: bool = False,
-    ) -> FcmPushMulticastResponse:
+    ) -> FCMBatchResponse:
         """
         Send Multicast push notification.
 
-        :param device_tokens: the list of device tokens to send targeted notifications to a set of instances of app.
+        :param multicast_message: multicast message to send targeted notifications to a set of instances of app.
             May contain up to 500 device tokens.
-        :param android: as instance of ``messages.AndroidConfig`` that contains Android-specific options.
-        :param apns: as instance of ``messages.APNSConfig`` that contains iOS-specific options.
-        :param data: a dictionary of data fields. All keys and values in the dictionary must be strings.
-        :param notification: an instance of ``messages.Notification`` that contains a notification that can be included
-            in a resulting message.
-        :param webpush: an instance of ``messages.WebpushConfig``.
         :param dry_run: indicating whether to run the operation in dry run mode (optional). Flag for testing the request
             without actually delivering the message. Default to ``False``.
+
+        :raises:
+
+            ValueError if ``messages.PushNotification`` payload cannot be assembled
+            ValueError if ``messages.MulticastMessage`` contains more than MULTICAST_MESSAGE_MAX_DEVICE_TOKENS
+
+        :return: instance of ``messages.FCMBatchResponse``
         """
 
-        if len(device_tokens) > MULTICAST_MESSAGE_MAX_DEVICE_TOKENS:
+        if len(multicast_message.tokens) > MULTICAST_MESSAGE_MAX_DEVICE_TOKENS:
             raise ValueError(
                 f"A single ``messages.MulticastMessage`` may contain up to {MULTICAST_MESSAGE_MAX_DEVICE_TOKENS} "
                 "device tokens."
             )
 
+        messages = [
+            Message(
+                token=token,
+                data=multicast_message.data,
+                notification=multicast_message.notification,
+                android=multicast_message.android,
+                webpush=multicast_message.webpush,
+                apns=multicast_message.apns,
+            )
+            for token in multicast_message.tokens
+        ]
+
+        return await self.send_all(messages, dry_run=dry_run)
+
+    async def send_all(
+        self,
+        messages: t.Union[t.List[Message], t.Tuple[Message]],
+        *,
+        dry_run: bool = False,
+    ) -> FCMBatchResponse:
+        """
+        Send push notifications in a single batch.
+
+        :param messages: the list of messages to send.
+        :param dry_run: indicating whether to run the operation in dry run mode (optional). Flag for testing the request
+            without actually delivering the message. Default to ``False``.
+        :returns: instance of ``messages.FCMBatchResponse``
+        """
+
         multipart_message = MIMEMultipart("mixed")
         # Message should not write out it's own headers.
         setattr(multipart_message, "_write_headers", lambda self: None)
 
-        for device_token in device_tokens:
+        for message in messages:
             msg = MIMENonMultipart("application", "http")
             msg["Content-Transfer-Encoding"] = "binary"
             msg["Content-ID"] = self.get_request_id()
             push_notification = self.assemble_push_notification(
-                apns_config=apns,
+                apns_config=message.apns,
                 dry_run=dry_run,
-                message=Message(
-                    token=device_token,
-                    data=data or {},
-                    notification=notification,
-                    android=android,
-                    webpush=webpush,
-                    apns=apns,
-                ),
+                message=message,
             )
             body = self.serialize_batch_request(
                 httpx.Request(
                     method="POST",
                     url=urljoin(
                         self.BASE_URL, self.FCM_ENDPOINT.format(project_id=self._credentials.project_id)  # type: ignore
                     ),
@@ -487,12 +476,12 @@
         # encode the body: note that we can't use `as_string`, because it plays games with `From ` lines.
         body = serialize_mime_message(multipart_message, mangle_from=False)
 
         batch_response = await self.send_request(
             uri=self.FCM_BATCH_ENDPOINT,
             content=body,
             headers={"Content-Type": f"multipart/mixed; boundary={multipart_message.get_boundary()}"},
-            response_handler=FcmPushMulticastResponseHandler(),
+            response_handler=FCMBatchResponseHandler(),
         )
-        if not isinstance(batch_response, FcmPushMulticastResponse):
+        if not isinstance(batch_response, FCMBatchResponse):
             raise ValueError("Wrong return type, perhaps because of a response handler misuse.")
         return batch_response
```

### Comparing `async_firebase-2.7.0/async_firebase/encoders.py` & `async_firebase-3.0.0/async_firebase/encoders.py`

 * *Files identical despite different names*

### Comparing `async_firebase-2.7.0/async_firebase/errors.py` & `async_firebase-3.0.0/async_firebase/errors.py`

 * *Files identical despite different names*

### Comparing `async_firebase-2.7.0/async_firebase/messages.py` & `async_firebase-3.0.0/async_firebase/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -295,79 +295,101 @@
     webpush: an instance of ``messages.WebpushConfig`` (optional).
     apns: an instance of ``messages.ApnsConfig`` (optional).
     token: the registration token of the device to which the message should be sent.
     topic: name of the Firebase topic to which the message should be sent (optional).
     condition: the Firebase condition to which the message should be sent (optional).
     """
 
-    token: t.Optional[str]
+    token: str
     data: t.Dict[str, str] = field(default_factory=dict)
     notification: t.Optional[Notification] = field(default=None)
     android: t.Optional[AndroidConfig] = field(default=None)
     webpush: t.Optional[WebpushConfig] = field(default=None)
     apns: t.Optional[APNSConfig] = field(default=None)
     topic: t.Optional[str] = None
     condition: t.Optional[str] = None
 
 
 @dataclass
+class MulticastMessage:
+    """
+    A message that can be sent to multiple tokens via Firebase.
+
+    Attributes:
+    tokens: a list of registration tokens of targeted devices.
+    data: a dictionary of data fields (optional). All keys and values in the dictionary must be strings.
+    notification: an instance of ``messages.Notification`` (optional).
+    android: an instance of ``messages.AndroidConfig`` (optional).
+    webpush: an instance of ``messages.WebpushConfig`` (optional).
+    apns: an instance of ``messages.ApnsConfig`` (optional).
+    """
+
+    tokens: t.List[str]
+    data: t.Dict[str, str] = field(default_factory=dict)
+    notification: t.Optional[Notification] = field(default=None)
+    android: t.Optional[AndroidConfig] = field(default=None)
+    webpush: t.Optional[WebpushConfig] = field(default=None)
+    apns: t.Optional[APNSConfig] = field(default=None)
+
+
+@dataclass
 class PushNotification:
     """The payload that is sent to Firebase Cloud Messaging.
 
     Attributes:
     message: an instance of ``messages.Message`` or ``messages.MulticastMessage``.
     validate_only: a boolean indicating whether to run the operation in dry run mode (optional).
     """
 
     message: Message
     validate_only: t.Optional[bool] = field(default=False)
 
 
-class FcmPushResponse:
+class FCMResponse:
     """The response received from an individual batched request to the FCM API.
 
     The interface of this object is compatible with SendResponse object of
     the Google's firebase-admin-python package.
     """
 
     def __init__(
         self, fcm_response: t.Optional[t.Dict[str, str]] = None, exception: t.Optional[AsyncFirebaseError] = None
     ):
-        """Inits FcmPushResponse object.
+        """Inits FCMResponse object.
 
         :param fcm_response: a dictionary with the data that FCM returns as a payload
         :param exception: an exception that may happen when communicating with FCM
         """
         self.message_id = fcm_response.get("name") if fcm_response else None
         self.exception = exception
 
     @property
     def success(self) -> bool:
         """A boolean indicating if the request was successful."""
         return self.message_id is not None and not self.exception
 
 
-class FcmPushMulticastResponse:
+class FCMBatchResponse:
     """The response received from a batch request to the FCM API.
 
     The interface of this object is compatible with BatchResponse object of
     the Google's firebase-admin-python package.
     """
 
-    def __init__(self, responses: t.List[FcmPushResponse]):
-        """Inits FcmPushMulticastResponse.
+    def __init__(self, responses: t.List[FCMResponse]):
+        """Inits FCMBatchResponse.
 
-        :param responses: a list of FcmPushResponse objects
+        :param responses: a list of FCMResponse objects
         """
         self._responses = responses
         self._success_count = len([resp for resp in responses if resp.success])
 
     @property
     def responses(self):
-        """A list of ``FcmPushResponse`` objects (possibly empty)."""
+        """A list of ``FCMResponse`` objects (possibly empty)."""
         return self._responses
 
     @property
     def success_count(self):
         return self._success_count
 
     @property
```

### Comparing `async_firebase-2.7.0/async_firebase/utils.py` & `async_firebase-3.0.0/async_firebase/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     QuotaExceededError,
     SenderIdMismatchError,
     ThirdPartyAuthError,
     UnavailableError,
     UnknownError,
     UnregisteredError,
 )
-from async_firebase.messages import FcmPushMulticastResponse, FcmPushResponse
+from async_firebase.messages import FCMBatchResponse, FCMResponse
 
 
 def remove_null_values(dict_value: t.Dict[str, t.Any]) -> t.Dict[str, t.Any]:
     """Remove Falsy values from the dictionary."""
     return {k: v for k, v in dict_value.items() if v not in [None, [], {}]}
 
 
@@ -118,18 +118,18 @@
     """
     fp = io.StringIO()
     gen = Generator(fp, mangle_from_=mangle_from, maxheaderlen=max_header_len)
     gen.flatten(message, unixfrom=False)
     return fp.getvalue()
 
 
-FcmResponseType = t.TypeVar("FcmResponseType", FcmPushResponse, FcmPushMulticastResponse)
+FCMResponseType = t.TypeVar("FCMResponseType", FCMResponse, FCMBatchResponse)
 
 
-class FcmResponseHandler(ABC, t.Generic[FcmResponseType]):
+class FCMResponseHandlerBase(ABC, t.Generic[FCMResponseType]):
 
     ERROR_CODE_TO_EXCEPTION_TYPE: t.Dict[str, t.Type[AsyncFirebaseError]] = {
         FcmErrorCode.INVALID_ARGUMENT.value: errors.InvalidArgumentError,
         FcmErrorCode.FAILED_PRECONDITION.value: errors.FailedPreconditionError,
         FcmErrorCode.OUT_OF_RANGE.value: errors.OutOfRangeError,
         FcmErrorCode.UNAUTHENTICATED.value: errors.UnauthenticatedError,
         FcmErrorCode.PERMISSION_DENIED.value: errors.PermissionDeniedError,
@@ -163,36 +163,36 @@
         "QUOTA_EXCEEDED": QuotaExceededError,
         "SENDER_ID_MISMATCH": SenderIdMismatchError,
         "THIRD_PARTY_AUTH_ERROR": ThirdPartyAuthError,
         "UNREGISTERED": UnregisteredError,
     }
 
     @abstractmethod
-    def handle_response(self, response: httpx.Response) -> FcmResponseType:
+    def handle_response(self, response: httpx.Response) -> FCMResponseType:
         pass
 
     @abstractmethod
-    def handle_error(self, error: httpx.HTTPError) -> FcmResponseType:
+    def handle_error(self, error: httpx.HTTPError) -> FCMResponseType:
         pass
 
     @staticmethod
-    def _handle_response(response: httpx.Response) -> FcmPushResponse:
-        return FcmPushResponse(fcm_response=response.json())
+    def _handle_response(response: httpx.Response) -> FCMResponse:
+        return FCMResponse(fcm_response=response.json())
 
-    def _handle_error(self, error: httpx.HTTPError) -> FcmPushResponse:
+    def _handle_error(self, error: httpx.HTTPError) -> FCMResponse:
         exc = (
             (isinstance(error, httpx.HTTPStatusError) and self._handle_fcm_error(error))
             or (isinstance(error, httpx.HTTPError) and self._handle_request_error(error))
             or AsyncFirebaseError(
                 code=FcmErrorCode.UNKNOWN.value,
                 message="Unexpected error has happened when hitting the FCM API",
                 cause=error,
             )
         )
-        return FcmPushResponse(exception=exc)
+        return FCMResponse(exception=exc)
 
     def _handle_request_error(self, error: httpx.HTTPError):
         if isinstance(error, httpx.TimeoutException):
             return DeadlineExceededError(message=f"Timed out while making an API call: {error}", cause=error)
         elif isinstance(error, httpx.ConnectError):
             return UnavailableError(message=f"Failed to establish a connection: {error}", cause=error)
         elif not hasattr(error, "response"):
@@ -248,38 +248,38 @@
         if not error_data.get("message"):
             error_data[
                 "message"
             ] = f"Unexpected HTTP response with status: {response.status_code}; body: {response.content!r}"
         return error_data
 
 
-class FcmPushResponseHandler(FcmResponseHandler[FcmPushResponse]):
-    def handle_error(self, error: httpx.HTTPError) -> FcmPushResponse:
+class FCMResponseHandler(FCMResponseHandlerBase[FCMResponse]):
+    def handle_error(self, error: httpx.HTTPError) -> FCMResponse:
         return self._handle_error(error)
 
-    def handle_response(self, response: httpx.Response) -> FcmPushResponse:
+    def handle_response(self, response: httpx.Response) -> FCMResponse:
         return self._handle_response(response)
 
 
-class FcmPushMulticastResponseHandler(FcmResponseHandler[FcmPushMulticastResponse]):
+class FCMBatchResponseHandler(FCMResponseHandlerBase[FCMBatchResponse]):
     def handle_error(self, error: httpx.HTTPError):
         fcm_response = self._handle_error(error)
-        return FcmPushMulticastResponse(responses=[fcm_response])
+        return FCMBatchResponse(responses=[fcm_response])
 
     def handle_response(self, response: httpx.Response):
         fcm_push_responses = []
         responses = self._deserialize_batch_response(response)
         for single_resp in responses:
             if single_resp.status_code >= 300:
                 exc = httpx.HTTPStatusError("FCM Error", response=single_resp, request=response.request)
                 fcm_push_responses.append(self._handle_error(exc))
             else:
                 fcm_push_responses.append(self._handle_response(single_resp))
 
-        return FcmPushMulticastResponse(responses=fcm_push_responses)
+        return FCMBatchResponse(responses=fcm_push_responses)
 
     @staticmethod
     def _deserialize_batch_response(response: httpx.Response) -> t.List[httpx.Response]:
         """Convert batch response into list of `httpx.Response` responses for each multipart.
 
         :param response: string, headers and body as a string.
         :return: list of `httpx.Response` responses.
```

### Comparing `async_firebase-2.7.0/pyproject.toml` & `async_firebase-3.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "async-firebase"
-version = "2.7.0"
+version = "3.0.0"
 description = "Async Firebase Client - a Python asyncio client to interact with Firebase Cloud Messaging in an easy way."
 license = "MIT"
 authors = [
-    "Aleksandr Omyshev <oomyshev@healthjoy.com>"
+    "Oleksandr Omyshev <oomyshev@healthjoy.com>"
 ]
 maintainers = [
     "Healthjoy Developers <developers@healthjoy.com>",
-    "Aleksandr Omyshev <oomyshev@healthjoy.com>"
+    "Oleksandr Omyshev <oomyshev@healthjoy.com>"
 ]
 readme = "README.md"
 repository = "https://github.com/healthjoy/async-firebase"
 keywords = ["async", "asyncio", "firebase", "fcm", "python3", "push-notifications"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

### Comparing `async_firebase-2.7.0/setup.py` & `async_firebase-3.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 {'': ['*']}
 
 install_requires = \
 ['google-auth>=2.6.0,<2.7.0', 'httpx>=0.23.0,<1.0.0']
 
 setup_kwargs = {
     'name': 'async-firebase',
-    'version': '2.7.0',
+    'version': '3.0.0',
     'description': 'Async Firebase Client - a Python asyncio client to interact with Firebase Cloud Messaging in an easy way.',
-    'long_description': '# async-firebase is a lightweight asynchronous client to interact with Firebase Cloud Messaging for sending push notification to Android and iOS devices\n\n[![PyPI download month](https://img.shields.io/pypi/dm/async-firebase.svg)](https://pypi.python.org/pypi/async-firebase/)\n[![PyPI version fury.io](https://badge.fury.io/py/async-firebase.svg)](https://pypi.python.org/pypi/async-firebase/)\n[![PyPI license](https://img.shields.io/pypi/l/async-firebase.svg)](https://pypi.python.org/pypi/async-firebase/)\n[![PyPI pyversions](https://img.shields.io/pypi/pyversions/async-firebase.svg)](https://pypi.python.org/pypi/async-firebase/)\n[![CI](https://github.com/healthjoy/async-firebase/actions/workflows/ci.yml/badge.svg)](https://github.com/healthjoy/async-firebase/actions/workflows/ci.yml)\n[![Codacy coverage](https://img.shields.io/codacy/coverage/b6a59cdf5ca64eab9104928d4f9bbb97?logo=codacy)](https://app.codacy.com/gh/healthjoy/async-firebase/dashboard)\n\n\n  * Free software: MIT license\n  * Requires: Python 3.7+\n\n## Features\n\n  * Extremely lightweight and does not rely on ``firebase-admin`` which is hefty\n  * Send push notifications to Android and iOS devices\n  * Send Multicast push notification to Android and iOS devices\n  * Send Web push notifications\n  * Set TTL (time to live) for notifications\n  * Set priority for notifications\n  * Set collapse-key for notifications\n  * Dry-run mode for testing purpose\n\n## Installation\n```shell script\n$ pip install async-firebase\n```\n\n## Getting started\nTo send push notification to Android:\n```python3\nimport asyncio\n\nfrom async_firebase import AsyncFirebaseClient\n\n\nasync def main():\n    client = AsyncFirebaseClient()\n    client.creds_from_service_account_file("secret-store/mobile-app-79225efac4bb.json")\n\n    # or using dictionary object\n    # client.creds_from_service_account_info({...}})\n\n    device_token = "..."\n\n    android_config = client.build_android_config(\n        priority="high",\n        ttl=2419200,\n        collapse_key="push",\n        data={"discount": "15%", "key_1": "value_1", "timestamp": "2021-02-24T12:00:15"},\n        title="Store Changes",\n        body="Recent store changes",\n    )\n    response = await client.push(device_token=device_token, android=android_config)\n\n    print(response.success, response.message_id)\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\nTo send push notification to iOS:\n\n```python3\nimport asyncio\n\nfrom async_firebase import AsyncFirebaseClient\n\n\nasync def main():\n    client = AsyncFirebaseClient()\n    client.creds_from_service_account_file("secret-store/mobile-app-79225efac4bb.json")\n\n    # or using dictionary object\n    # client.creds_from_service_account_info({...}})\n\n    device_token = "..."\n\n    apns_config = client.build_apns_config(\n        priority="normal",\n        ttl=2419200,\n        apns_topic="store-updated",\n        collapse_key="push",\n        title="Store Changes",\n        alert="Recent store changes",\n        badge=1,\n        category="test-category",\n        custom_data={"discount": "15%", "key_1": "value_1", "timestamp": "2021-02-24T12:00:15"}\n    )\n    response = await client.push(device_token=device_token, apns=apns_config)\n\n    print(response.success)\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\nThis prints:\n\n```shell script\n"projects/mobile-app/messages/0:2367799010922733%7606eb557606ebff"\n```\n\nTo manual construct message:\n```python3\nimport asyncio\nfrom datetime import datetime\n\nfrom async_firebase.messages import APNSConfig, APNSPayload, ApsAlert, Aps\nfrom async_firebase import AsyncFirebaseClient\n\n\nasync def main():\n    apns_config = APNSConfig(**{\n        "headers": {\n            "apns-expiration": str(int(datetime.utcnow().timestamp()) + 7200),\n            "apns-priority": "10",\n            "apns-topic": "test-topic",\n            "apns-collapse-id": "something",\n        },\n        "payload": APNSPayload(**{\n            "aps": Aps(**{\n                "alert": ApsAlert(title="some-title", body="alert-message"),\n                "badge": 0,\n                "sound": "default",\n                "content_available": True,\n                "category": "some-category",\n                "mutable_content": False,\n                "custom_data": {\n                    "link": "https://link-to-somewhere.com",\n                    "ticket_id": "YXZ-655512",\n                },\n            })\n        })\n    })\n\n    device_token = "..."\n\n    client = AsyncFirebaseClient()\n    client.creds_from_service_account_info({...})\n    response = await client.push(device_token=device_token, apns=apns_config)\n    print(response.success)\n\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\n## License\n\n``async-firebase`` is offered under the MIT license.\n\n## Source code\n\nThe latest developer version is available in a GitHub repository:\n[https://github.com/healthjoy/async-firebase](https://github.com/healthjoy/async-firebase)\n',
-    'author': 'Aleksandr Omyshev',
+    'long_description': '# async-firebase is a lightweight asynchronous client to interact with Firebase Cloud Messaging for sending push notification to Android and iOS devices\n\n[![PyPI download month](https://img.shields.io/pypi/dm/async-firebase.svg)](https://pypi.python.org/pypi/async-firebase/)\n[![PyPI version fury.io](https://badge.fury.io/py/async-firebase.svg)](https://pypi.python.org/pypi/async-firebase/)\n[![PyPI license](https://img.shields.io/pypi/l/async-firebase.svg)](https://pypi.python.org/pypi/async-firebase/)\n[![PyPI pyversions](https://img.shields.io/pypi/pyversions/async-firebase.svg)](https://pypi.python.org/pypi/async-firebase/)\n[![CI](https://github.com/healthjoy/async-firebase/actions/workflows/ci.yml/badge.svg)](https://github.com/healthjoy/async-firebase/actions/workflows/ci.yml)\n[![Codacy coverage](https://img.shields.io/codacy/coverage/b6a59cdf5ca64eab9104928d4f9bbb97?logo=codacy)](https://app.codacy.com/gh/healthjoy/async-firebase/dashboard)\n\n\n  * Free software: MIT license\n  * Requires: Python 3.7+\n\n## Features\n\n  * Extremely lightweight and does not rely on ``firebase-admin`` which is hefty\n  * Send push notifications to Android and iOS devices\n  * Send Multicast push notification to Android and iOS devices\n  * Send Web push notifications\n  * Set TTL (time to live) for notifications\n  * Set priority for notifications\n  * Set collapse-key for notifications\n  * Dry-run mode for testing purpose\n\n## Installation\n```shell script\n$ pip install async-firebase\n```\n\n## Getting started\n### async-firebase < 3.0.0\nTo send push notification to Android:\n```python3\nimport asyncio\n\nfrom async_firebase import AsyncFirebaseClient\n\n\nasync def main():\n    client = AsyncFirebaseClient()\n    client.creds_from_service_account_file("secret-store/mobile-app-79225efac4bb.json")\n\n    # or using dictionary object\n    # client.creds_from_service_account_info({...}})\n\n    device_token = "..."\n\n    android_config = client.build_android_config(\n        priority="high",\n        ttl=2419200,\n        collapse_key="push",\n        data={"discount": "15%", "key_1": "value_1", "timestamp": "2021-02-24T12:00:15"},\n        title="Store Changes",\n        body="Recent store changes",\n    )\n    response = await client.push(device_token=device_token, android=android_config)\n\n    print(response.success, response.message_id)\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\nTo send push notification to iOS:\n\n```python3\nimport asyncio\n\nfrom async_firebase import AsyncFirebaseClient\n\n\nasync def main():\n    client = AsyncFirebaseClient()\n    client.creds_from_service_account_file("secret-store/mobile-app-79225efac4bb.json")\n\n    # or using dictionary object\n    # client.creds_from_service_account_info({...}})\n\n    device_token = "..."\n\n    apns_config = client.build_apns_config(\n        priority="normal",\n        ttl=2419200,\n        apns_topic="store-updated",\n        collapse_key="push",\n        title="Store Changes",\n        alert="Recent store changes",\n        badge=1,\n        category="test-category",\n        custom_data={"discount": "15%", "key_1": "value_1", "timestamp": "2021-02-24T12:00:15"}\n    )\n    response = await client.push(device_token=device_token, apns=apns_config)\n\n    print(response.success)\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\nThis prints:\n\n```shell script\n"projects/mobile-app/messages/0:2367799010922733%7606eb557606ebff"\n```\n\nTo manual construct message:\n```python3\nimport asyncio\nfrom datetime import datetime\n\nfrom async_firebase.messages import APNSConfig, APNSPayload, ApsAlert, Aps\nfrom async_firebase import AsyncFirebaseClient\n\n\nasync def main():\n    apns_config = APNSConfig(**{\n        "headers": {\n            "apns-expiration": str(int(datetime.utcnow().timestamp()) + 7200),\n            "apns-priority": "10",\n            "apns-topic": "test-topic",\n            "apns-collapse-id": "something",\n        },\n        "payload": APNSPayload(**{\n            "aps": Aps(**{\n                "alert": ApsAlert(title="some-title", body="alert-message"),\n                "badge": 0,\n                "sound": "default",\n                "content_available": True,\n                "category": "some-category",\n                "mutable_content": False,\n                "custom_data": {\n                    "link": "https://link-to-somewhere.com",\n                    "ticket_id": "YXZ-655512",\n                },\n            })\n        })\n    })\n\n    device_token = "..."\n\n    client = AsyncFirebaseClient()\n    client.creds_from_service_account_info({...})\n    response = await client.push(device_token=device_token, apns=apns_config)\n    print(response.success)\n\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\n### async-firebase >= 3.0.0\nTo send push notification to Android:\n```python3\nimport asyncio\n\nfrom async_firebase import AsyncFirebaseClient\nfrom async_firebase.messages import Message\n\n\nasync def main():\n    client = AsyncFirebaseClient()\n    client.creds_from_service_account_file("secret-store/mobile-app-79225efac4bb.json")\n\n    # or using dictionary object\n    # client.creds_from_service_account_info({...}})\n\n    device_token: str = "..."\n\n    android_config = client.build_android_config(\n        priority="high",\n        ttl=2419200,\n        collapse_key="push",\n        data={"discount": "15%", "key_1": "value_1", "timestamp": "2021-02-24T12:00:15"},\n        title="Store Changes",\n        body="Recent store changes",\n    )\n    message = Message(android=android_config, token=device_token)\n    response = await client.push(message)\n\n    print(response.success, response.message_id)\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\nTo send push notification to iOS:\n\n```python3\nimport asyncio\n\nfrom async_firebase import AsyncFirebaseClient\nfrom async_firebase.messages import Message\n\n\nasync def main():\n    client = AsyncFirebaseClient()\n    client.creds_from_service_account_file("secret-store/mobile-app-79225efac4bb.json")\n\n    # or using dictionary object\n    # client.creds_from_service_account_info({...}})\n\n    device_token: str = "..."\n\n    apns_config = client.build_apns_config(\n        priority="normal",\n        ttl=2419200,\n        apns_topic="store-updated",\n        collapse_key="push",\n        title="Store Changes",\n        alert="Recent store changes",\n        badge=1,\n        category="test-category",\n        custom_data={"discount": "15%", "key_1": "value_1", "timestamp": "2021-02-24T12:00:15"}\n    )\n    message = Message(apns=apns_config, token=device_token)\n    response = await client.push(message)\n\n    print(response.success)\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\nThis prints:\n\n```shell script\n"projects/mobile-app/messages/0:2367799010922733%7606eb557606ebff"\n```\n\nTo manual construct message:\n```python3\nimport asyncio\nfrom datetime import datetime\n\nfrom async_firebase.messages import APNSConfig, APNSPayload, ApsAlert, Aps, Message\nfrom async_firebase import AsyncFirebaseClient\n\n\nasync def main():\n    apns_config = APNSConfig(**{\n        "headers": {\n            "apns-expiration": str(int(datetime.utcnow().timestamp()) + 7200),\n            "apns-priority": "10",\n            "apns-topic": "test-topic",\n            "apns-collapse-id": "something",\n        },\n        "payload": APNSPayload(**{\n            "aps": Aps(**{\n                "alert": ApsAlert(title="some-title", body="alert-message"),\n                "badge": 0,\n                "sound": "default",\n                "content_available": True,\n                "category": "some-category",\n                "mutable_content": False,\n                "custom_data": {\n                    "link": "https://link-to-somewhere.com",\n                    "ticket_id": "YXZ-655512",\n                },\n            })\n        })\n    })\n\n    device_token: str = "..."\n\n    client = AsyncFirebaseClient()\n    client.creds_from_service_account_info({...})\n    message = Message(apns=apns_config, token=device_token)\n    response = await client.push(message)\n    print(response.success)\n\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\n## License\n\n``async-firebase`` is offered under the MIT license.\n\n## Source code\n\nThe latest developer version is available in a GitHub repository:\n[https://github.com/healthjoy/async-firebase](https://github.com/healthjoy/async-firebase)\n',
+    'author': 'Oleksandr Omyshev',
     'author_email': 'oomyshev@healthjoy.com',
     'maintainer': 'Healthjoy Developers',
     'maintainer_email': 'developers@healthjoy.com',
     'url': 'https://github.com/healthjoy/async-firebase',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
```

### Comparing `async_firebase-2.7.0/PKG-INFO` & `async_firebase-3.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: async-firebase
-Version: 2.7.0
+Version: 3.0.0
 Summary: Async Firebase Client - a Python asyncio client to interact with Firebase Cloud Messaging in an easy way.
 Home-page: https://github.com/healthjoy/async-firebase
 License: MIT
 Keywords: async,asyncio,firebase,fcm,python3,push-notifications
-Author: Aleksandr Omyshev
+Author: Oleksandr Omyshev
 Author-email: oomyshev@healthjoy.com
 Maintainer: Healthjoy Developers
 Maintainer-email: developers@healthjoy.com
 Requires-Python: >=3.7,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -57,14 +57,15 @@
 
 ## Installation
 ```shell script
 $ pip install async-firebase
 ```
 
 ## Getting started
+### async-firebase < 3.0.0
 To send push notification to Android:
 ```python3
 import asyncio
 
 from async_firebase import AsyncFirebaseClient
 
 
@@ -176,14 +177,139 @@
     print(response.success)
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
+### async-firebase >= 3.0.0
+To send push notification to Android:
+```python3
+import asyncio
+
+from async_firebase import AsyncFirebaseClient
+from async_firebase.messages import Message
+
+
+async def main():
+    client = AsyncFirebaseClient()
+    client.creds_from_service_account_file("secret-store/mobile-app-79225efac4bb.json")
+
+    # or using dictionary object
+    # client.creds_from_service_account_info({...}})
+
+    device_token: str = "..."
+
+    android_config = client.build_android_config(
+        priority="high",
+        ttl=2419200,
+        collapse_key="push",
+        data={"discount": "15%", "key_1": "value_1", "timestamp": "2021-02-24T12:00:15"},
+        title="Store Changes",
+        body="Recent store changes",
+    )
+    message = Message(android=android_config, token=device_token)
+    response = await client.push(message)
+
+    print(response.success, response.message_id)
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
+
+To send push notification to iOS:
+
+```python3
+import asyncio
+
+from async_firebase import AsyncFirebaseClient
+from async_firebase.messages import Message
+
+
+async def main():
+    client = AsyncFirebaseClient()
+    client.creds_from_service_account_file("secret-store/mobile-app-79225efac4bb.json")
+
+    # or using dictionary object
+    # client.creds_from_service_account_info({...}})
+
+    device_token: str = "..."
+
+    apns_config = client.build_apns_config(
+        priority="normal",
+        ttl=2419200,
+        apns_topic="store-updated",
+        collapse_key="push",
+        title="Store Changes",
+        alert="Recent store changes",
+        badge=1,
+        category="test-category",
+        custom_data={"discount": "15%", "key_1": "value_1", "timestamp": "2021-02-24T12:00:15"}
+    )
+    message = Message(apns=apns_config, token=device_token)
+    response = await client.push(message)
+
+    print(response.success)
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
+
+This prints:
+
+```shell script
+"projects/mobile-app/messages/0:2367799010922733%7606eb557606ebff"
+```
+
+To manual construct message:
+```python3
+import asyncio
+from datetime import datetime
+
+from async_firebase.messages import APNSConfig, APNSPayload, ApsAlert, Aps, Message
+from async_firebase import AsyncFirebaseClient
+
+
+async def main():
+    apns_config = APNSConfig(**{
+        "headers": {
+            "apns-expiration": str(int(datetime.utcnow().timestamp()) + 7200),
+            "apns-priority": "10",
+            "apns-topic": "test-topic",
+            "apns-collapse-id": "something",
+        },
+        "payload": APNSPayload(**{
+            "aps": Aps(**{
+                "alert": ApsAlert(title="some-title", body="alert-message"),
+                "badge": 0,
+                "sound": "default",
+                "content_available": True,
+                "category": "some-category",
+                "mutable_content": False,
+                "custom_data": {
+                    "link": "https://link-to-somewhere.com",
+                    "ticket_id": "YXZ-655512",
+                },
+            })
+        })
+    })
+
+    device_token: str = "..."
+
+    client = AsyncFirebaseClient()
+    client.creds_from_service_account_info({...})
+    message = Message(apns=apns_config, token=device_token)
+    response = await client.push(message)
+    print(response.success)
+
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
+
 ## License
 
 ``async-firebase`` is offered under the MIT license.
 
 ## Source code
 
 The latest developer version is available in a GitHub repository:
```

