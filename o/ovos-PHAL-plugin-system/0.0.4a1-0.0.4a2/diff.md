# Comparing `tmp/ovos-PHAL-plugin-system-0.0.4a1.tar.gz` & `tmp/ovos-PHAL-plugin-system-0.0.4a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-system-0.0.4a1.tar", last modified: Mon Apr 10 18:17:32 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-system-0.0.4a2.tar", last modified: Tue Apr 11 16:19:49 2023, max compression
```

## Comparing `ovos-PHAL-plugin-system-0.0.4a1.tar` & `ovos-PHAL-plugin-system-0.0.4a2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:17:32.746103 ovos-PHAL-plugin-system-0.0.4a1/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-10 18:17:32.746103 ovos-PHAL-plugin-system-0.0.4a1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:17:32.746103 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-10 18:17:24.000000 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:17:32.746103 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-10 18:17:24.000000 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/ui/Reboot.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-10 18:17:24.000000 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/ui/Restart.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-10 18:17:24.000000 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/ui/Shutdown.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-10 18:17:24.000000 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/ui/Status.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:17:32.746103 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/ui/animations/
--rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-04-10 18:17:24.000000 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/ui/animations/loading.json
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-04-10 18:17:24.000000 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/ui/animations/status-fail.json
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-04-10 18:17:24.000000 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/ui/animations/status-success.json
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-10 18:17:26.000000 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:17:32.746103 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-10 18:17:32.000000 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-10 18:17:32.000000 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 18:17:32.000000 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-10 18:17:32.000000 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-10 18:17:32.000000 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-10 18:17:32.000000 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 18:17:32.000000 ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 18:17:32.746103 ovos-PHAL-plugin-system-0.0.4a1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2736 2023-04-10 18:17:24.000000 ovos-PHAL-plugin-system-0.0.4a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:19:49.870209 ovos-PHAL-plugin-system-0.0.4a2/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-11 16:19:49.870209 ovos-PHAL-plugin-system-0.0.4a2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:19:49.866209 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/
+-rw-r--r--   0 runner    (1001) docker     (123)    12031 2023-04-11 16:19:39.000000 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:19:49.870209 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-11 16:19:39.000000 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/ui/Reboot.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-11 16:19:39.000000 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/ui/Restart.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-11 16:19:39.000000 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/ui/Shutdown.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-11 16:19:39.000000 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/ui/Status.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:19:49.870209 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/ui/animations/
+-rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-04-11 16:19:39.000000 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/ui/animations/loading.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-04-11 16:19:39.000000 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/ui/animations/status-fail.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-04-11 16:19:39.000000 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/ui/animations/status-success.json
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-11 16:19:43.000000 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:19:49.866209 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-11 16:19:49.000000 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-11 16:19:49.000000 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 16:19:49.000000 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-11 16:19:49.000000 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-11 16:19:49.000000 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-11 16:19:49.000000 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 16:19:49.000000 ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 16:19:49.870209 ovos-PHAL-plugin-system-0.0.4a2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2736 2023-04-11 16:19:39.000000 ovos-PHAL-plugin-system-0.0.4a2/setup.py
```

### Comparing `ovos-PHAL-plugin-system-0.0.4a1/PKG-INFO` & `ovos-PHAL-plugin-system-0.0.4a2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-system
-Version: 0.0.4a1
+Version: 0.0.4a2
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-system
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/__init__.py` & `ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 from ovos_backend_client.identity import IdentityManager
 from ovos_config.config import update_mycroft_config
 from ovos_config.locale import set_default_lang
 from ovos_config.locations import OLD_USER_CONFIG, USER_CONFIG, WEB_CONFIG_CACHE
 from ovos_config.meta import get_xdg_base
 from ovos_plugin_manager.phal import PHALPlugin
 from ovos_utils.gui import GUIInterface
-from ovos_utils.system import system_shutdown, system_reboot, ssh_enable, ssh_disable, ntp_sync, restart_service, \
-    is_process_running
+from ovos_utils.system import system_shutdown, system_reboot, ssh_enable,\
+    ssh_disable, ntp_sync, restart_service, is_process_running, \
+    check_service_active
 from ovos_utils.xdg_utils import xdg_state_home, xdg_cache_home, xdg_data_home
 from ovos_utils.log import LOG
 
 
 class SystemEventsValidator:
     @staticmethod
     def validate(config=None):
@@ -32,24 +33,27 @@
     validator = SystemEventsValidator
 
     def __init__(self, bus=None, config=None):
         super().__init__(bus=bus, name="ovos-PHAL-plugin-system", config=config)
         self.gui = GUIInterface(bus=self.bus, skill_id=self.name)
 
         self.bus.on("system.ntp.sync", self.handle_ntp_sync_request)
+        self.bus.on("system.ssh.status", self.handle_ssh_status)
         self.bus.on("system.ssh.enable", self.handle_ssh_enable_request)
         self.bus.on("system.ssh.disable", self.handle_ssh_disable_request)
         self.bus.on("system.reboot", self.handle_reboot_request)
         self.bus.on("system.shutdown", self.handle_shutdown_request)
         self.bus.on("system.factory.reset", self.handle_factory_reset_request)
         self.bus.on("system.factory.reset.register", self.handle_reset_register)
         self.bus.on("system.configure.language", self.handle_configure_language_request)
         self.bus.on("system.mycroft.service.restart",
                     self.handle_mycroft_restart_request)
         self.service_name = config.get("core_service") or "mycroft.service"
+        # In Debian, ssh stays active, but sshd is removed when ssh is disabled
+        self.ssh_service = config.get("ssh_service") or "sshd.service"
         self.use_root = config.get("sudo", True)
 
         self.factory_reset_plugs = []
 
         # trigger register events from phal plugins
         self.bus.emit(Message("system.factory.reset.ping"))
 
@@ -241,14 +245,21 @@
 
     def handle_mycroft_restart_request(self, message):
         if message.data.get("display", True):
             page = join(dirname(__file__), "ui", "Restart.qml")
             self.gui.show_page(page, override_animations=True, override_idle=True)
         restart_service(self.service_name, sudo=self.use_root)
 
+    def handle_ssh_status(self, message):
+        """
+        Check SSH service status and emit a response
+        """
+        enabled = check_service_active(self.ssh_service)
+        self.bus.emit(message.response(data={'enabled': enabled}))
+
     def shutdown(self):
         self.bus.remove("system.ntp.sync", self.handle_ntp_sync_request)
         self.bus.remove("system.ssh.enable", self.handle_ssh_enable_request)
         self.bus.remove("system.ssh.disable", self.handle_ssh_disable_request)
         self.bus.remove("system.reboot", self.handle_reboot_request)
         self.bus.remove("system.shutdown", self.handle_shutdown_request)
         self.bus.remove("system.factory.reset", self.handle_factory_reset_request)
```

### Comparing `ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/ui/Reboot.qml` & `ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/ui/Reboot.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/ui/Restart.qml` & `ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/ui/Restart.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/ui/Shutdown.qml` & `ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/ui/Shutdown.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/ui/Status.qml` & `ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/ui/Status.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/ui/animations/loading.json` & `ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/ui/animations/loading.json`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/ui/animations/status-fail.json` & `ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/ui/animations/status-fail.json`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system/ui/animations/status-success.json` & `ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system/ui/animations/status-success.json`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system.egg-info/PKG-INFO` & `ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-system
-Version: 0.0.4a1
+Version: 0.0.4a2
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-system
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-system-0.0.4a1/ovos_PHAL_plugin_system.egg-info/SOURCES.txt` & `ovos-PHAL-plugin-system-0.0.4a2/ovos_PHAL_plugin_system.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a1/setup.py` & `ovos-PHAL-plugin-system-0.0.4a2/setup.py`

 * *Files identical despite different names*

