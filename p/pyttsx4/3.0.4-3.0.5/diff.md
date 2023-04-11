# Comparing `tmp/pyttsx4-3.0.4-py3-none-any.whl.zip` & `tmp/pyttsx4-3.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 33201 bytes, number of entries: 16
+Zip file size: 33285 bytes, number of entries: 16
 -rw-r--r--  2.0 unx      814 b- defN 23-Apr-07 13:37 pyttsx4/__init__.py
 -rw-r--r--  2.0 unx     7429 b- defN 23-Apr-07 17:19 pyttsx4/driver.py
 -rw-r--r--  2.0 unx     7224 b- defN 23-Apr-07 13:37 pyttsx4/engine.py
--rw-r--r--  2.0 unx    29524 b- defN 23-Apr-07 13:37 pyttsx4/six.py
+-rw-r--r--  2.0 unx    29524 b- defN 23-Apr-11 03:46 pyttsx4/six.py
 -rw-r--r--  2.0 unx      431 b- defN 23-Apr-07 13:37 pyttsx4/voice.py
--rw-r--r--  2.0 unx      853 b- defN 23-Apr-07 13:37 pyttsx4/drivers/__init__.py
+-rw-r--r--  2.0 unx      853 b- defN 23-Apr-11 03:47 pyttsx4/drivers/__init__.py
 -rw-r--r--  2.0 unx    19495 b- defN 23-Apr-07 13:37 pyttsx4/drivers/_espeak.py
 -rw-r--r--  2.0 unx     6182 b- defN 23-Apr-07 13:37 pyttsx4/drivers/dummy.py
--rw-r--r--  2.0 unx     6801 b- defN 23-Apr-07 13:37 pyttsx4/drivers/espeak.py
+-rw-r--r--  2.0 unx     7448 b- defN 23-Apr-11 03:43 pyttsx4/drivers/espeak.py
 -rw-r--r--  2.0 unx     3729 b- defN 23-Apr-07 14:49 pyttsx4/drivers/nsss.py
--rw-r--r--  2.0 unx     6552 b- defN 23-Apr-08 05:21 pyttsx4/drivers/sapi5.py
--rw-r--r--  2.0 unx    17098 b- defN 23-Apr-08 05:24 pyttsx4-3.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     1821 b- defN 23-Apr-08 05:24 pyttsx4-3.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-08 05:24 pyttsx4-3.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-08 05:24 pyttsx4-3.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1244 b- defN 23-Apr-08 05:24 pyttsx4-3.0.4.dist-info/RECORD
-16 files, 109297 bytes uncompressed, 31181 bytes compressed:  71.5%
+-rw-r--r--  2.0 unx     6552 b- defN 23-Apr-11 03:47 pyttsx4/drivers/sapi5.py
+-rw-r--r--  2.0 unx    17098 b- defN 23-Apr-11 10:00 pyttsx4-3.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1821 b- defN 23-Apr-11 10:00 pyttsx4-3.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 10:00 pyttsx4-3.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-11 10:00 pyttsx4-3.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1244 b- defN 23-Apr-11 10:00 pyttsx4-3.0.5.dist-info/RECORD
+16 files, 109944 bytes uncompressed, 31265 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: pyttsx4/drivers/nsss.py
 Comment: 
 
 Filename: pyttsx4/drivers/sapi5.py
 Comment: 
 
-Filename: pyttsx4-3.0.4.dist-info/LICENSE
+Filename: pyttsx4-3.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: pyttsx4-3.0.4.dist-info/METADATA
+Filename: pyttsx4-3.0.5.dist-info/METADATA
 Comment: 
 
-Filename: pyttsx4-3.0.4.dist-info/WHEEL
+Filename: pyttsx4-3.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: pyttsx4-3.0.4.dist-info/top_level.txt
+Filename: pyttsx4-3.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: pyttsx4-3.0.4.dist-info/RECORD
+Filename: pyttsx4-3.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyttsx4/drivers/espeak.py

```diff
@@ -33,26 +33,28 @@
         self.setProperty('rate', 200)
         self.setProperty('volume', 1.0)
         self._proxy = proxy
         self._looping = True
         self._stopping = False
         self._data_buffer = b''
         self._numerise_buffer = []
+        self.to_filename = None
 
     def numerise(self, data):
         self._numerise_buffer.append(data)
         return ctypes.c_void_p(len(self._numerise_buffer))
 
     def decode_numeric(self, data):
         return self._numerise_buffer[int(data) - 1]
 
     def destroy(self):
         _espeak.SetSynthCallback(None)
 
     def say(self, text):
+        self.to_filename=None
         self._proxy.setBusy(True)
         self._proxy.notify('started-utterance')
         _espeak.Synth(toUtf8(text), flags=_espeak.ENDPAUSE |
                       _espeak.CHARS_UTF8)
 
     def stop(self):
         if _espeak.IsPlaying():
@@ -129,15 +131,19 @@
                 _espeak.Cancel()
                 self._stopping = False
                 self._proxy.notify('finished-utterance', completed=False)
                 self._proxy.setBusy(False)
             time.sleep(0.01)
 
     def save_to_file(self, text, filename):
-        code = self.numerise(filename)
+        self.to_filename = filename
+        if isinstance(filename, io.BytesIO):
+            code = None
+        else:
+            code = self.numerise(self.to_filename)
         _espeak.Synth(toUtf8(text), flags=_espeak.ENDPAUSE |
                     _espeak.CHARS_UTF8, user_data=code)
 
     def endLoop(self):
         self._looping = False
 
     def iterate(self):
@@ -159,25 +165,32 @@
             if event.type == _espeak.EVENT_LIST_TERMINATED:
                 break
             if event.type == _espeak.EVENT_WORD:
                 self._proxy.notify('started-word',
                                    location=event.text_position - 1,
                                    length=event.length)
             elif event.type == _espeak.EVENT_MSG_TERMINATED:
-                stream = NamedTemporaryFile()
-
-                with wave.open(stream, 'wb') as f:
-                    f.setnchannels(1)
-                    f.setsampwidth(2)
-                    f.setframerate(22050.0)
-                    f.writeframes(self._data_buffer)
 
-                if event.user_data:
+                if isinstance(self.to_filename,io.BytesIO):
+                    self.to_filename.write(self._data_buffer)
+                elif event.user_data:
+                    stream = NamedTemporaryFile()
+                    with wave.open(stream, 'wb') as f:
+                        f.setnchannels(1)
+                        f.setsampwidth(2)
+                        f.setframerate(22050.0)
+                        f.writeframes(self._data_buffer)
                     os.system('ffmpeg -y -i {} {} -loglevel quiet'.format(stream.name, self.decode_numeric(event.user_data)))
                 else:
+                    stream = NamedTemporaryFile()
+                    with wave.open(stream, 'wb') as f:
+                        f.setnchannels(1)
+                        f.setsampwidth(2)
+                        f.setframerate(22050.0)
+                        f.writeframes(self._data_buffer)
                     os.system('aplay {} -q'.format(stream.name))  # -q for quiet
 
                 self._data_buffer = b''
                 self._proxy.notify('finished-utterance', completed=True)
                 self._proxy.setBusy(False)
             i += 1
```

## Comparing `pyttsx4-3.0.4.dist-info/LICENSE` & `pyttsx4-3.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyttsx4-3.0.4.dist-info/METADATA` & `pyttsx4-3.0.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyttsx4
-Version: 3.0.4
+Version: 3.0.5
 Summary: Text to Speech (TTS) library for Python 3. Works without internet connection or delay. Supports multiple TTS engines, including Sapi5, nsss, and espeak.
 Home-page: https://github.com/Jiangshan00001/pyttsx4
 Author: Natesh M Bhat
 Author-email: 710806594@qq.com
 License: UNKNOWN
 Keywords: pyttsx,ivona,pyttsx for python3,TTS for python3,pyttsx3,text to speech for python,tts,text to speech,speech,speech synthesis,offline text to speech,offline tts,gtts
 Platform: UNKNOWN
```

## Comparing `pyttsx4-3.0.4.dist-info/RECORD` & `pyttsx4-3.0.5.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 pyttsx4/driver.py,sha256=uQI4OAbaRRKBEwBeh_cFW5nsev-8btlBP9xEGEaPLs4,7429
 pyttsx4/engine.py,sha256=UJBrPIcN3KXmBCABrb2uY4F_AeAaFlC5h6n_L3V0euA,7224
 pyttsx4/six.py,sha256=yVeu0rLX2Qv1P1UaJtvamDmMrjnxNsJkSuztEvVyGG8,29524
 pyttsx4/voice.py,sha256=GYZLgGtnmjLrg93Wh7_lqDcs6zMaTS_QRr3KZM7RZnY,431
 pyttsx4/drivers/__init__.py,sha256=EFf83iBpSVF4joEh4gQmq5Rl22tngVNuR1zBeWfCdjQ,853
 pyttsx4/drivers/_espeak.py,sha256=Gj0N4aFf3YGZO9fq8K5BFbiwkIExqDu1nBXUn7EZVzY,19495
 pyttsx4/drivers/dummy.py,sha256=d7K46sijjOxwmAJHbgEALwbYwGcktLfW1FcX1iG5I8E,6182
-pyttsx4/drivers/espeak.py,sha256=p2-L60Qrl6wVoSrGlQM6jWQhammXJL-UvCxsDoPZaow,6801
+pyttsx4/drivers/espeak.py,sha256=5QcaVaCyb3xLKXs6_fjnGv0-mioUXINzendba95mpgs,7448
 pyttsx4/drivers/nsss.py,sha256=n849K4ugK87S4ejtc_7xYp5W__maB6vfRX_sxIWlGIU,3729
 pyttsx4/drivers/sapi5.py,sha256=EiEEwvammMCS4YI7aWG0fmtQZm_0-bPJqC9nndUUpp4,6552
-pyttsx4-3.0.4.dist-info/LICENSE,sha256=JoTeFzAOCkNGhvHsf4r2BFIHpLRXo_4EsrnOZV58XVA,17098
-pyttsx4-3.0.4.dist-info/METADATA,sha256=Ad3b4iHnt_1tmKEKyilDODnbJmoI9frV63_XZen3i28,1821
-pyttsx4-3.0.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pyttsx4-3.0.4.dist-info/top_level.txt,sha256=RZW_EXmaQg7go8T0q583RzqdJUlYm0NeSHGpyq92tiY,8
-pyttsx4-3.0.4.dist-info/RECORD,,
+pyttsx4-3.0.5.dist-info/LICENSE,sha256=JoTeFzAOCkNGhvHsf4r2BFIHpLRXo_4EsrnOZV58XVA,17098
+pyttsx4-3.0.5.dist-info/METADATA,sha256=8bpbU-vrPfj6H6ZHwQx0sBwAxo9D-37DDFZKIR1tb8Y,1821
+pyttsx4-3.0.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pyttsx4-3.0.5.dist-info/top_level.txt,sha256=RZW_EXmaQg7go8T0q583RzqdJUlYm0NeSHGpyq92tiY,8
+pyttsx4-3.0.5.dist-info/RECORD,,
```

