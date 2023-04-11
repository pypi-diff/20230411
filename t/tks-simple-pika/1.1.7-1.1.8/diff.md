# Comparing `tmp/tks_simple_pika-1.1.7-py2.py3-none-any.whl.zip` & `tmp/tks_simple_pika-1.1.8-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3890 bytes, number of entries: 6
--rw-r--r--  2.0 unx     2622 b- defN 23-Apr-05 08:49 tks_simple_pika_consumer.py
+Zip file size: 3877 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     2611 b- defN 23-Apr-11 07:06 tks_simple_pika_consumer.py
 -rw-r--r--  2.0 unx     2701 b- defN 23-Apr-04 08:25 tks_simple_pika_publisher.py
--rw-r--r--  2.0 unx     1882 b- defN 23-Apr-05 08:49 tks_simple_pika-1.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-05 08:49 tks_simple_pika-1.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       51 b- defN 23-Apr-05 08:49 tks_simple_pika-1.1.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      500 b- defN 23-Apr-05 08:49 tks_simple_pika-1.1.7.dist-info/RECORD
-6 files, 7866 bytes uncompressed, 2982 bytes compressed:  62.1%
+-rw-r--r--  2.0 unx     1882 b- defN 23-Apr-11 07:07 tks_simple_pika-1.1.8.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-11 07:07 tks_simple_pika-1.1.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       51 b- defN 23-Apr-11 07:07 tks_simple_pika-1.1.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      500 b- defN 23-Apr-11 07:07 tks_simple_pika-1.1.8.dist-info/RECORD
+6 files, 7855 bytes uncompressed, 2969 bytes compressed:  62.2%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: tks_simple_pika_consumer.py
 Comment: 
 
 Filename: tks_simple_pika_publisher.py
 Comment: 
 
-Filename: tks_simple_pika-1.1.7.dist-info/METADATA
+Filename: tks_simple_pika-1.1.8.dist-info/METADATA
 Comment: 
 
-Filename: tks_simple_pika-1.1.7.dist-info/WHEEL
+Filename: tks_simple_pika-1.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: tks_simple_pika-1.1.7.dist-info/top_level.txt
+Filename: tks_simple_pika-1.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: tks_simple_pika-1.1.7.dist-info/RECORD
+Filename: tks_simple_pika-1.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tks_simple_pika_consumer.py

```diff
@@ -32,26 +32,26 @@
               ..... Here actions from you businees logic
             consumer.callback = __callback.__get__(consumer, TksSimplePikaConsumer)
             consumer.consumer_start()
         '''
         print(" [x] %r %s %s %s" % (body, ch, method, properties))
 
 
-    async def consumer_start(self) -> None:
-        await asyncio.sleep(0.5)
+    def consumer_start(self) -> None:
+        #await asyncio.sleep(0.5)
         try:
             connection = pika.BlockingConnection(pika.ConnectionParameters(host=self.RABBITMQ_HOST,port=self.RABBITMQ_PORT))
             channel = connection.channel()
             channel.exchange_declare(exchange=self.RABBITMQ_EXCHANGE,
                                      exchange_type=self.RABBITMQ_EXCHANGE_TYPE)
             result = channel.queue_declare(queue='', exclusive=True)
             queue_name = result.method.queue
             channel.queue_bind(exchange=self.RABBITMQ_EXCHANGE, queue=queue_name)
             channel.basic_consume(queue=queue_name, on_message_callback=self.callback, auto_ack=self.RABBITMQ_CHANNEL_AUTO_ACK)
-            await channel.start_consuming()
+            channel.start_consuming()
         except Exception as e:
             logger.error(e)
 
     def validate_envs(self):
         if None != config('RABBITMQ_HOST'):
             self.RABBITMQ_HOST = config('RABBITMQ_HOST')
         else:
```

## Comparing `tks_simple_pika-1.1.7.dist-info/METADATA` & `tks_simple_pika-1.1.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tks-simple-pika
-Version: 1.1.7
+Version: 1.1.8
 Summary: Library for a simple implementation of a RabbitMQ consumer and producer using the python pika library
 Home-page: 
 Author: Oscar Fernandez Robles
 Author-email: oskijob@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: pika
```

