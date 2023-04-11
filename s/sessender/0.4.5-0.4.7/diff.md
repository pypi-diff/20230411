# Comparing `tmp/sessender-0.4.5.tar.gz` & `tmp/sessender-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sessender-0.4.5.tar", last modified: Mon Apr 10 13:03:09 2023, max compression
+gzip compressed data, was "sessender-0.4.7.tar", last modified: Tue Apr 11 08:26:09 2023, max compression
```

## Comparing `sessender-0.4.5.tar` & `sessender-0.4.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:03:09.867876 sessender-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-10 13:02:59.000000 sessender-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-10 13:03:09.867876 sessender-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-10 13:02:59.000000 sessender-0.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:03:09.867876 sessender-0.4.5/sessender.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-10 13:03:09.000000 sessender-0.4.5/sessender.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-10 13:03:09.000000 sessender-0.4.5/sessender.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 13:03:09.000000 sessender-0.4.5/sessender.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-10 13:03:09.000000 sessender-0.4.5/sessender.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-10 13:02:59.000000 sessender-0.4.5/sessender.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 13:03:09.867876 sessender-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-10 13:02:59.000000 sessender-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:09.075970 sessender-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-11 08:25:55.000000 sessender-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-11 08:26:09.075970 sessender-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-11 08:25:55.000000 sessender-0.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:26:09.075970 sessender-0.4.7/sessender.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-11 08:26:08.000000 sessender-0.4.7/sessender.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-11 08:26:09.000000 sessender-0.4.7/sessender.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:26:08.000000 sessender-0.4.7/sessender.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 08:26:08.000000 sessender-0.4.7/sessender.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-04-11 08:25:55.000000 sessender-0.4.7/sessender.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:26:09.075970 sessender-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-11 08:25:55.000000 sessender-0.4.7/setup.py
```

### Comparing `sessender-0.4.5/LICENSE` & `sessender-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sessender-0.4.5/sessender.py` & `sessender-0.4.7/sessender.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,33 +11,37 @@
 
 class SesSender:
     def __init__(self):
         try:
             self.smtp_username = os.getenv('SES_USERNAME')
             self.smtp_password = os.getenv('SES_PASS')
             self.smtp_host = os.getenv('SES_HOST')
-            self.smtp_port = os.getenv('SES_PORT')
-            self.recipient = os.getenv('EMAIL_RECIPIENT')
-            self.sender = os.getenv('EMAIL_SENDER')
+            self.smtp_port = os.getenv('SES_PORT', 587) # Use a default value of 587 for the port number
+            self.default_recipient = os.getenv('EMAIL_RECIPIENT', None)
+            self.default_sender = os.getenv('EMAIL_SENDER', None)
 
             # Configure logging
             logging.basicConfig(filename='seslog.txt', level=logging.DEBUG, format='%(asctime)s - %(levelname)s - %(message)s')
 
         except Exception as e:
             error_msg = f"Error initializing Sessender:\n{traceback.format_exc()}"
             print(error_msg)
             logging.error(error_msg)
             raise e
 
-    def send_email(self, subject, message=None, html_message=None, attachment=None):
+    def send_email(self, subject, message=None, html_message=None, attachment=None, sender=None, recipients=None, cc=None, bcc=None):
         try:
             # Create a message
             msg = MIMEMultipart()
-            msg['From'] = self.sender
-            msg['To'] = self.recipient
+            msg['From'] = sender or self.default_sender
+            msg['To'] = ', '.join(recipients) if recipients else self.default_recipient
+            if cc:
+                msg['Cc'] = ', '.join(cc)
+            if bcc:
+                msg['Bcc'] = ', '.join(bcc)
             msg['Subject'] = subject
 
             # Attach plain text or HTML message
             if html_message:
                 msg.attach(MIMEText(html_message, 'html'))
             elif message:
                 msg.attach(MIMEText(message))
@@ -46,18 +50,24 @@
             if attachment:
                 with open(attachment, 'rb') as f:
                     part = MIMEApplication(f.read(), Name=os.path.basename(attachment))
                     part['Content-Disposition'] = f'attachment; filename="{os.path.basename(attachment)}"'
                     msg.attach(part)
 
             # Connect to the SMTP server and send the message
+            all_recipients = recipients or [self.default_recipient]
+            if cc:
+                all_recipients += cc
+            if bcc:
+                all_recipients += bcc
+
             with smtplib.SMTP(self.smtp_host, int(self.smtp_port)) as smtp:
                 smtp.starttls()
                 smtp.login(self.smtp_username, self.smtp_password)
-                smtp.sendmail(self.sender, self.recipient, msg.as_string())
+                smtp.sendmail(msg['From'], all_recipients, msg.as_string())
 
             # Log success
             logging.info(f"Email sent: {subject}")
 
         except:
             # Log error
             error_msg = f"Error sending email:\n{traceback.format_exc()}"
```

### Comparing `sessender-0.4.5/setup.py` & `sessender-0.4.7/setup.py`

 * *Files identical despite different names*

