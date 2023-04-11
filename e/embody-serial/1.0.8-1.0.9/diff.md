# Comparing `tmp/embody-serial-1.0.8.tar.gz` & `tmp/embody-serial-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embody-serial-1.0.8.tar", max compression
+gzip compressed data, was "embody-serial-1.0.9.tar", max compression
```

## Comparing `embody-serial-1.0.8.tar` & `embody-serial-1.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1068 2022-11-29 20:23:28.039808 embody-serial-1.0.8/LICENSE
--rw-r--r--   0        0        0     3799 2022-11-29 20:23:28.039808 embody-serial-1.0.8/README.md
--rw-r--r--   0        0        0     1982 2022-11-29 20:23:39.203988 embody-serial-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      248 2022-11-29 20:23:28.043808 embody-serial-1.0.8/src/embodyserial/__init__.py
--rw-r--r--   0        0        0      239 2022-11-29 20:23:28.043808 embody-serial-1.0.8/src/embodyserial/__main__.py
--rw-r--r--   0        0        0     7177 2022-11-29 20:23:28.043808 embody-serial-1.0.8/src/embodyserial/cli.py
--rw-r--r--   0        0        0    18585 2022-11-29 20:23:28.043808 embody-serial-1.0.8/src/embodyserial/embodyserial.py
--rw-r--r--   0        0        0      628 2022-11-29 20:23:28.043808 embody-serial-1.0.8/src/embodyserial/exceptions.py
--rw-r--r--   0        0        0     7514 2022-11-29 20:23:28.043808 embody-serial-1.0.8/src/embodyserial/helpers.py
--rw-r--r--   0        0        0      880 2022-11-29 20:23:28.043808 embody-serial-1.0.8/src/embodyserial/listeners.py
--rw-r--r--   0        0        0        0 2022-11-29 20:23:28.043808 embody-serial-1.0.8/src/embodyserial/py.typed
--rw-r--r--   0        0        0     4819 1970-01-01 00:00:00.000000 embody-serial-1.0.8/setup.py
--rw-r--r--   0        0        0     4644 1970-01-01 00:00:00.000000 embody-serial-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-12-08 16:33:13.159344 embody-serial-1.0.9/LICENSE
+-rw-r--r--   0        0        0     3799 2022-12-08 16:33:13.159344 embody-serial-1.0.9/README.md
+-rw-r--r--   0        0        0     1984 2022-12-08 16:33:24.763632 embody-serial-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      212 2022-12-08 16:33:13.163344 embody-serial-1.0.9/src/embodyserial/__init__.py
+-rw-r--r--   0        0        0      250 2022-12-08 16:33:24.763632 embody-serial-1.0.9/src/embodyserial/__main__.py
+-rw-r--r--   0        0        0     8747 2022-12-08 16:33:24.763632 embody-serial-1.0.9/src/embodyserial/cli.py
+-rw-r--r--   0        0        0    23622 2022-12-08 16:33:24.763632 embody-serial-1.0.9/src/embodyserial/embodyserial.py
+-rw-r--r--   0        0        0      628 2022-12-08 16:33:13.163344 embody-serial-1.0.9/src/embodyserial/exceptions.py
+-rw-r--r--   0        0        0     6988 2022-12-08 16:33:24.763632 embody-serial-1.0.9/src/embodyserial/helpers.py
+-rw-r--r--   0        0        0     1576 2022-12-08 16:33:13.163344 embody-serial-1.0.9/src/embodyserial/listeners.py
+-rw-r--r--   0        0        0        0 2022-12-08 16:33:13.163344 embody-serial-1.0.9/src/embodyserial/py.typed
+-rw-r--r--   0        0        0     4821 1970-01-01 00:00:00.000000 embody-serial-1.0.9/setup.py
+-rw-r--r--   0        0        0     4646 1970-01-01 00:00:00.000000 embody-serial-1.0.9/PKG-INFO
```

### Comparing `embody-serial-1.0.8/LICENSE` & `embody-serial-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `embody-serial-1.0.8/README.md` & `embody-serial-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `embody-serial-1.0.8/pyproject.toml` & `embody-serial-1.0.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "embody-serial"
-version = "1.0.8"
+version = "1.0.9"
 description = "Communicate with the embody device over a serial port"
 authors = ["Aidee Health AS <hello@aidee.io>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/aidee-health/embody-serial"
 repository = "https://github.com/aidee-health/embody-serial"
 packages = [
@@ -15,15 +15,15 @@
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/aidee-health/embody-serial/releases"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<=3.11"
-embody-codec = ">1.0.9"
+embody-codec = ">=1.0.12"
 pyserial = "^3.5"
 
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
```

### Comparing `embody-serial-1.0.8/src/embodyserial/cli.py` & `embody-serial-1.0.9/src/embodyserial/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """cli entry point for embodyserial.
 
 Parse command line arguments, invoke embody device.
 """
 import argparse
 import logging
 import sys
-import time
 
-from . import __version__
-from .embodyserial import EmbodySerial
-from .helpers import EmbodySendHelper
+from embodyserial import __version__
+from embodyserial.embodyserial import EmbodySerial
+from embodyserial.helpers import EmbodySendHelper
+from embodyserial.listeners import FileDownloadListener
 
 
 get_attributes_dict: dict[str, str] = {
     "serialno": "get_serial_no",
     "ble_mac": "get_bluetooth_mac",
     "model": "get_model",
     "vendor": "get_vendor",
@@ -59,16 +59,19 @@
                 f"Trace level set: {send_helper.set_trace_level(parsed_args.set_trace_level)}"
             )
             exit(0)
         elif parsed_args.list_files:
             __list_files(send_helper)
             exit(0)
         elif parsed_args.download_file:
-            return __download_file(
-                parsed_args.download_file, embody_serial, send_helper
+            __download_file(parsed_args.download_file, embody_serial, send_helper)
+            exit(0)
+        elif parsed_args.download_file_with_delay:
+            __download_file(
+                parsed_args.download_file_with_delay, embody_serial, send_helper, 0.01
             )
             exit(0)
         elif parsed_args.download_files:
             __download_files(embody_serial, send_helper)
             exit(0)
         elif parsed_args.delete_file:
             print(
@@ -91,15 +94,20 @@
 
     finally:
         embody_serial.shutdown()
 
 
 def __get_all_attributes(send_helper):
     for attrib in get_attributes_dict.keys():
-        print(f"{attrib}: {getattr(send_helper, get_attributes_dict.get(attrib))()}")
+        sys.stdout.write(f"{attrib}: ")
+        sys.stdout.flush()
+        try:
+            print(getattr(send_helper, get_attributes_dict.get(attrib))())
+        except Exception as e:
+            print(f"Error: {e}")
 
 
 def __list_files(send_helper):
     files = send_helper.get_files()
     if len(files) > 0:
         for name, size in send_helper.get_files():
             print(f"{name} ({round(size/1024)}KB)")
@@ -114,39 +122,76 @@
         return
     print(f"Found {len(files)} {'files' if len(files) > 1 else 'file'}")
     for file in files:
         __do_download_file(file, embody_serial, send_helper)
 
 
 def __download_file(
-    file_name: str, embody_serial: EmbodySerial, send_helper: EmbodySendHelper
+    file_name: str,
+    embody_serial: EmbodySerial,
+    send_helper: EmbodySendHelper,
+    delay: float = 0.0,
 ):
     filtered_files: list[tuple[str, int]] = [
         tup for tup in send_helper.get_files() if tup[0] == file_name
     ]
     if not filtered_files or len(filtered_files) == 0:
         print(f"Unknown file name {file_name}")
         return
-    __do_download_file(filtered_files[0], embody_serial, send_helper)
+    __do_download_file(filtered_files[0], embody_serial, send_helper, delay)
+
+
+def _show_cli_progress_bar(progress: float, total: int, kbps: float):
+    bar_length = 20
+    percent = progress / 100
+    hashes = "#" * int(round(percent * bar_length))
+    spaces = " " * (bar_length - len(hashes))
+    sys.stdout.write(
+        "\rProgress: [{}] {}% ({} kbps)".format(
+            hashes + spaces, int(round(percent * 100)), int(round(kbps))
+        )
+    )
+    sys.stdout.flush()
 
 
 def __do_download_file(
-    file: tuple[str, int], embody_serial: EmbodySerial, send_helper: EmbodySendHelper
+    file: tuple[str, int],
+    embody_serial: EmbodySerial,
+    send_helper: EmbodySendHelper,
+    delay: float = 0.0,
 ):
     print(f"Downloading: {file[0]}")
-    start = time.time()
-    try:
-        downloaded_file = embody_serial.download_file(file_name=file[0], size=file[1])
-        end = time.time()
-        print(
-            f"{file[0]} downloaded to {downloaded_file} ({round(file[1]/1024,2)}KB)"
-            f" @ ({round((file[1]/1024)/(end-start),2)}KB/s)"
-        )
-    except Exception as e:
-        print(f"Unable to download file: {e}")
+
+    class _DownloadListener(FileDownloadListener):
+        download_invocation_count = 0
+
+        def on_file_download_progress(
+            self, original_file_name: str, size: int, progress: float, kbps: float
+        ) -> None:
+            """Display progress in cli."""
+            if self.download_invocation_count % 10 == 0 or progress == 100:
+                _show_cli_progress_bar(progress, size, kbps)
+            self.download_invocation_count += 1
+
+        def on_file_download_complete(
+            self, original_file_name: str, path: str, kbps: float
+        ) -> None:
+            """Process file download completion."""
+            print(f" {original_file_name} downloaded to {path} (@{round(kbps)} kbps)")
+
+        def on_file_download_failed(
+            self, original_file_name: str, error: Exception
+        ) -> None:
+            """Process file download failure."""
+            print(f" {original_file_name} failed to download: {error}")
+
+    listener = _DownloadListener()
+    embody_serial.download_file(
+        file_name=file[0], size=file[1], download_listener=listener, delay=delay
+    )
 
 
 def __get_args(args):
     """Parse arguments passed in from shell."""
     return __get_parser().parse_args(args)
 
 
@@ -161,36 +206,34 @@
     log_levels = ["CRITICAL", "WARNING", "INFO", "DEBUG"]
     parser.add_argument(
         "--log-level",
         help=f"Log level ({log_levels})",
         choices=log_levels,
         default="WARNING",
     )
-    parser.add_argument(
-        "--channel",
-        help="Use serial or ble",
-        choices=["serial", "ble"],
-        default="serial",
-    )
-    parser.add_argument(
-        "--device", help="Device name (serial or ble name)", default=None
-    )
+    parser.add_argument("--device", help="Serial port name", default=None)
     parser.add_argument(
         "--get", help="Get attribute", choices=get_attributes_dict.keys(), default=None
     )
     parser.add_argument(
         "--get-all", help="Get all attributes", action="store_true", default=None
     )
     parser.add_argument(
         "--set-time", help="Set time (to now)", action="store_true", default=None
     )
     parser.add_argument(
         "--download-file", help="Download specified file", type=str, default=None
     )
     parser.add_argument(
+        "--download-file-with-delay",
+        help="Download specified file with simulated delay",
+        type=str,
+        default=None,
+    )
+    parser.add_argument(
         "--download-files", help="Download all files", action="store_true", default=None
     )
     parser.add_argument(
         "--set-trace-level", help="Set trace level", type=int, default=None
     )
     parser.add_argument(
         "--list-files",
```

### Comparing `embody-serial-1.0.8/src/embodyserial/embodyserial.py` & `embody-serial-1.0.9/src/embodyserial/embodyserial.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,30 +9,32 @@
 import tempfile
 import threading
 import time
 from abc import ABC
 from abc import abstractmethod
 from concurrent.futures import ThreadPoolExecutor
 from concurrent.futures import TimeoutError
+from dataclasses import dataclass
 from typing import Optional
 
 import serial
 import serial.tools.list_ports
 from embodycodec import codec
 from embodycodec import crc
 from embodycodec import types
 from serial.serialutil import SerialBase
 from serial.serialutil import SerialException
 from serial.tools import list_ports_common
 
-from .exceptions import CrcError
-from .exceptions import MissingResponseError
-from .listeners import ConnectionListener
-from .listeners import MessageListener
-from .listeners import ResponseMessageListener
+from embodyserial.exceptions import CrcError
+from embodyserial.exceptions import MissingResponseError
+from embodyserial.listeners import ConnectionListener
+from embodyserial.listeners import FileDownloadListener
+from embodyserial.listeners import MessageListener
+from embodyserial.listeners import ResponseMessageListener
 
 
 class EmbodySender(ABC):
     """Listener interface for being notified of incoming messages."""
 
     @abstractmethod
     def send_async(self, msg: codec.Message) -> None:
@@ -105,25 +107,34 @@
 
     def on_connected(self, connected: bool) -> None:
         """Implement connection listener interface and handle disconnect events"""
         logging.debug(f"Connection event: {connected}")
         if not connected:
             self.shutdown()
 
-    def download_file(self, file_name: str, size: int, timeout: int = 300) -> str:
+    def download_file(
+        self,
+        file_name: str,
+        size: int,
+        download_listener: Optional[FileDownloadListener] = None,
+        timeout: int = 300,
+        delay: float = 0.0,
+    ) -> str:
         """Download file from device and write to temporary file.
 
         Raises:
           MissingResponseError if no response.
           CrcError if invalid crc.
         """
         if size == 0:
             return tempfile.NamedTemporaryFile(delete=False).name
         self.send_async(codec.GetFileUart(types.File(file_name)))
-        return self.__reader.download_file(size, timeout)
+        return self.__reader.download_file(
+            file_name, size, download_listener, timeout, delay
+        )
 
     @staticmethod
     def __find_serial_port() -> str:
         """Find first matching serial port name."""
         manufacturers = ["Datek", "Aidee"]
         descriptions = ["IsenseU", "G3", "EmBody"]
         all_available_ports = serial.tools.list_ports.comports()
@@ -220,143 +231,234 @@
                 return None
             if wait_for_response_secs:
                 if self.__response_event.wait(wait_for_response_secs):
                     return self.__current_response_message
             return None
 
 
+@dataclass
+class _FileDownload:
+    file_size: int = -1
+    file_timeout: Optional[int] = None
+    original_file_name: Optional[str] = None
+    file_name: Optional[str] = None
+    file_error: Optional[Exception] = None
+    file_download_listener: Optional[FileDownloadListener] = None
+    file_delay: float = 0.0
+
+
 class _ReaderThread(threading.Thread):
     """Implement a serial port read loop and dispatch incoming messages to subscribers/listeners.
 
     Calls to close() will close the serial port it is also possible to just
     stop() this thread and continue the serial port instance otherwise.
     """
 
     def __init__(self, serial_instance: SerialBase) -> None:
         """Initialize thread."""
         super().__init__()
         self.daemon = True
         self.setName("reader")
         self.__serial = serial_instance
+        self.__read_timeout: Optional[int] = None
+        if hasattr(self.__serial, "timeout"):
+            self.__read_timeout = serial_instance.timeout
+
         self.__message_listener_executor = ThreadPoolExecutor(
             max_workers=1, thread_name_prefix="rcv-worker"
         )
         self.__response_message_listener_executor = ThreadPoolExecutor(
             max_workers=1, thread_name_prefix="rsp-worker"
         )
+        self.__file_download_listener_executor = ThreadPoolExecutor(
+            max_workers=1, thread_name_prefix="dwnld-worker"
+        )
         self.__message_listeners: list[MessageListener] = []
         self.__response_message_listeners: list[ResponseMessageListener] = []
         self.__connection_listeners: list[ConnectionListener] = []
         self.__file_mode = False
-        self.__file_size = -1
-        self.__file_timeout = 0
-        self.__file_name: Optional[str] = None
-        self.__file_error: Optional[Exception] = None
+        self.__f: Optional[_FileDownload] = None
         self.__file_event = threading.Event()
         self.alive = True
 
-    def download_file(self, size: int, timeout: int = 300) -> str:
+    def download_file(
+        self,
+        original_file_name: str,
+        size: int,
+        download_listener: Optional[FileDownloadListener] = None,
+        timeout: int = 300,
+        delay=0.0,
+    ) -> str:
         """Set reader in file mode and read file."""
+        if hasattr(self.__serial, "timeout"):
+            self.__serial.timeout = 10
         self.__reset_file_mode()
-        self.__file_timeout = timeout
-        self.__file_size = size
+        f = _FileDownload(
+            file_size=size,
+            file_timeout=timeout,
+            original_file_name=original_file_name,
+            file_download_listener=download_listener,
+            file_delay=delay,
+        )
+        self.__f = f
         self.__file_mode = True
         try:
-            if not self.__file_event.wait(timeout) or not self.__file_name:
+            if not self.__file_event.wait(timeout):
                 raise MissingResponseError("No file received within timeout")
-            if self.__file_error:
-                raise self.__file_error
-            return self.__file_name
+            if self.__f.file_error:
+                raise self.__f.file_error
+            if not self.__f.file_name:
+                raise MissingResponseError("No file received")
+            return self.__f.file_name
+        except Exception as e:
+            self.__async_notify_file_download_failed(f, e)
+            raise e
         finally:
             self.__reset_file_mode()
+            if hasattr(self.__serial, "timeout") and self.__read_timeout:
+                self.__serial.timeout = self.__read_timeout
 
     def __reset_file_mode(self) -> None:
         self.__file_event.clear()
-        self.__file_size = -1
-        self.__file_name = None
-        self.__file_error = None
         self.__file_mode = False
+        self.__f = None
 
     def stop(self) -> None:
         """Stop the reader thread"""
         if not self.alive:
             return
         self.alive = False
         if hasattr(self.__serial, "cancel_read"):
             self.__serial.cancel_read()
         self.__message_listener_executor.shutdown(wait=False, cancel_futures=False)
         self.__response_message_listener_executor.shutdown(
             wait=False, cancel_futures=False
         )
+        self.__file_download_listener_executor.shutdown(
+            wait=False, cancel_futures=False
+        )
         self.join(2)
 
     def run(self) -> None:
         """Reader loop"""
         if not hasattr(self.__serial, "cancel_read"):
             self.__serial.timeout = 300
         while self.alive and self.__serial.is_open:
             try:
                 raw_header = self.__serial.read(3)
                 if not raw_header or len(raw_header) < 3:
                     logging.info("Interrupted. Exiting reader thread.")
                     break
-                if self.__file_mode:
-                    self.__read_file(raw_header)
-                    self.__reset_file_mode()
+                if self.__file_mode and self.__f:
+                    self.__read_file(raw_header, self.__f)
                 else:
                     self.__read_protocol_message(raw_header)
             except serial.SerialException:
                 # probably some I/O problem such as disconnected USB serial adapters -> exit
                 logging.info("Serial port is closed (SerialException)")
                 break
             except OSError:
                 logging.info("OS Error reading from socket (OSError)")
                 break
         self.alive = False
         self.__notify_connection_listeners(connected=False)
 
-    def __read_file(self, first_bytes: bytes) -> None:
-        buffer_size = 1024
-        remaining_size = self.__file_size - len(first_bytes)
-        calculated_crc = crc.crc16(data=first_bytes)
-        tmp = tempfile.NamedTemporaryFile(delete=False, buffering=buffer_size)
+    def __read_file(self, first_bytes: bytes, f: _FileDownload) -> None:
+        buffer_size = 2048
+        remaining_size = f.file_size - len(first_bytes)
         start = time.time()
-        tmp.write(first_bytes)
+        in_memory_buffer = bytearray(first_bytes)
+        loop_count = 0
         try:
             while remaining_size > 0 and self.__serial.is_open:
                 chunk = self.__serial.read(min(buffer_size, remaining_size))
                 if not chunk:
                     raise MissingResponseError("File download failed")
-                calculated_crc = crc.crc16(data=chunk, existing_crc=calculated_crc)
-                tmp.write(chunk)
+                in_memory_buffer.extend(chunk)
                 remaining_size -= len(chunk)
-                logging.debug(
-                    f"Read file. Remaining: {remaining_size} of {self.__file_size}"
-                    f" bytes (in waiting: {self.__serial.in_waiting} bytes)"
-                )
-                time.sleep(0.001)
-                if time.time() - start > self.__file_timeout:
+                now = time.time()
+                if loop_count % 20 == 0:
+                    self.__async_notify_file_download_in_progress(
+                        f,
+                        f.file_size,
+                        round(((f.file_size - remaining_size) / f.file_size) * 100),
+                        round(((f.file_size - remaining_size) / 1024) / (now - start)),
+                    )
+                loop_count += 1
+                if f.file_timeout and now - start > f.file_timeout:
                     raise TimeoutError(
-                        f"Reading file took too long. Read {self.__file_size - remaining_size} bytes"
+                        f"Reading file took too long. Read {f.file_size - remaining_size} bytes"
                     )
+                if f.file_delay:
+                    time.sleep(f.file_delay)
             raw_crc_received = self.__serial.read(2)
             end = time.time()
-            logging.info(
-                f"Read {round(self.__file_size/1024,2)}KB in {end-start} secs - {round((self.__file_size/1024)/(end-start),2)}KB/s"
+            self.__async_notify_file_download_in_progress(
+                f,
+                f.file_size,
+                100,
+                round((f.file_size / 1024) / (end - start), 2),
+            )
+            logging.debug(
+                f"Read {round(f.file_size/1024,2)}KB in {end-start} secs "
+                f"- {round((f.file_size/1024)/(end-start),2)}KB/s"
             )
             (crc_received,) = struct.unpack(">H", raw_crc_received)
+            calculated_crc = crc.crc16(data=in_memory_buffer)
             if not crc_received == calculated_crc:
-                self.__file_error = CrcError(
-                    f"Invalid crc - expected {hex(crc_received)}, received {hex(calculated_crc)}"
+                f.file_error = CrcError(
+                    f"Invalid crc - expected {hex(crc_received)}, received/calculated {hex(calculated_crc)}"
                 )
-            else:
-                self.__file_name = tmp.name
-            self.__file_event.set()
-        finally:
+                self.__async_notify_file_download_failed(f, f.file_error)
+                return
+            tmp = tempfile.NamedTemporaryFile(delete=False)
+            tmp.write(in_memory_buffer)
+            tmp.flush()
             tmp.close()
+            f.file_name = tmp.name
+            self.__async_notify_file_download_completed(
+                f, round((f.file_size / 1024) / (end - start), 2)
+            )
+        except Exception as e:
+            f.file_error = e
+            self.__async_notify_file_download_failed(f, e)
+        finally:
+            self.__file_event.set()
+
+    def __async_notify_file_download_in_progress(
+        self, f: _FileDownload, size: int, progress: float, kbps: float
+    ):
+        if f.file_download_listener and f.original_file_name:
+            self.__file_download_listener_executor.submit(
+                _ReaderThread.__notify_file_download_progress,
+                f.file_download_listener,
+                f.original_file_name,
+                size,
+                progress,
+                kbps,
+            )
+
+    def __async_notify_file_download_completed(self, f: _FileDownload, kbps: float):
+        if f.file_download_listener and f.original_file_name and f.file_name:
+            self.__file_download_listener_executor.submit(
+                _ReaderThread.__notify_file_download_complete,
+                f.file_download_listener,
+                f.original_file_name,
+                f.file_name,
+                kbps,
+            )
+
+    def __async_notify_file_download_failed(self, f: _FileDownload, error: Exception):
+        if f.file_download_listener and f.original_file_name:
+            self.__file_download_listener_executor.submit(
+                _ReaderThread.__notify_file_download_failed,
+                f.file_download_listener,
+                f.original_file_name,
+                error,
+            )
 
     def __read_protocol_message(self, raw_header: bytes) -> None:
         """Read next message from input."""
         logging.debug(f"RECEIVE: Received header {raw_header.hex()}")
         msg_type, length = struct.unpack(">BH", raw_header)
         logging.debug(f"RECEIVE: Received msg type: {msg_type}, length: {length}")
         remaining_length = length - 3
@@ -443,14 +545,51 @@
         try:
             listener.on_connected(connected)
         except Exception as e:
             logging.warning(
                 f"Error notifying connection listener: {str(e)}", exc_info=True
             )
 
+    @staticmethod
+    def __notify_file_download_progress(
+        listener: FileDownloadListener,
+        original_file_name: str,
+        size: int,
+        progress: float,
+        kbps: float,
+    ) -> None:
+        try:
+            listener.on_file_download_progress(original_file_name, size, progress, kbps)
+        except Exception as e:
+            logging.warning(
+                f"Error notifying file download listener: {str(e)}", exc_info=True
+            )
+
+    @staticmethod
+    def __notify_file_download_complete(
+        listener: FileDownloadListener, original_file_name: str, path: str, kbps: float
+    ) -> None:
+        try:
+            listener.on_file_download_complete(original_file_name, path, kbps)
+        except Exception as e:
+            logging.warning(
+                f"Error notifying file download listener: {str(e)}", exc_info=True
+            )
+
+    @staticmethod
+    def __notify_file_download_failed(
+        listener: FileDownloadListener, original_file_name: str, error: Exception
+    ) -> None:
+        try:
+            listener.on_file_download_failed(original_file_name, error)
+        except Exception as e:
+            logging.warning(
+                f"Error notifying file download listener: {str(e)}", exc_info=True
+            )
+
 
 if __name__ == "__main__":
     """Main method for demo and testing"""
     logging.basicConfig(
         level=logging.DEBUG,
         format="%(asctime)s [%(thread)d/%(threadName)s] %(message)s",
     )
```

### Comparing `embody-serial-1.0.8/src/embodyserial/exceptions.py` & `embody-serial-1.0.9/src/embodyserial/exceptions.py`

 * *Files identical despite different names*

### Comparing `embody-serial-1.0.8/src/embodyserial/helpers.py` & `embody-serial-1.0.9/src/embodyserial/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from datetime import timezone
 from typing import Optional
 
 from embodycodec import attributes
 from embodycodec import codec
 from embodycodec import types
 
-from .embodyserial import EmbodySender
-from .exceptions import MissingResponseError
-from .exceptions import NackError
+from embodyserial.embodyserial import EmbodySender
+from embodyserial.exceptions import MissingResponseError
+from embodyserial.exceptions import NackError
 
 
 class EmbodySendHelper:
     """Facade to make send/receive more protocol agnostic with simple get/set methods."""
 
     def __init__(self, sender: EmbodySender, timeout: Optional[int] = 30) -> None:
         self.__sender = sender
@@ -89,17 +89,15 @@
         )
         response = response_attribute.formatted_value()
         assert response
         return response
 
     def get_files(self) -> list[tuple[str, int]]:
         """Get a list of tuples with file name and file size."""
-        response = self.__sender.send(
-            msg=codec.ListFiles(), timeout=self.__send_timeout
-        )
+        response = self.__sender.send(msg=codec.ListFiles(), timeout=120)
         if not response:
             raise MissingResponseError
         if isinstance(response, codec.NackResponse):
             raise NackError(response)
         assert isinstance(response, codec.ListFilesResponse)
 
         files: list[tuple[str, int]] = list()
@@ -140,39 +138,27 @@
             raise MissingResponseError()
         if isinstance(response, codec.NackResponse):
             raise NackError(response)
         assert isinstance(response, codec.ReformatDiskResponse)
         return True
 
     def reset_device(self) -> bool:
-        response = self.__sender.send(
+        self.__sender.send_async(
             msg=codec.ExecuteCommand(
                 command_id=codec.ExecuteCommand.RESET_DEVICE, value=b""
-            ),
-            timeout=self.__send_timeout,
+            )
         )
-        if not response:
-            raise MissingResponseError()
-        if isinstance(response, codec.NackResponse):
-            raise NackError(response)
-        assert isinstance(response, codec.ExecuteCommand)
         return True
 
     def reboot_device(self) -> bool:
-        response = self.__sender.send(
+        self.__sender.send_async(
             msg=codec.ExecuteCommand(
                 command_id=codec.ExecuteCommand.REBOOT_DEVICE, value=b""
-            ),
-            timeout=self.__send_timeout,
+            )
         )
-        if not response:
-            raise MissingResponseError()
-        if isinstance(response, codec.NackResponse):
-            raise NackError(response)
-        assert isinstance(response, codec.ExecuteCommand)
         return True
 
     def delete_all_files(self) -> bool:
         response = self.__sender.send(
             msg=codec.DeleteAllFiles(), timeout=self.__send_timeout
         )
         if not response:
```

### Comparing `embody-serial-1.0.8/src/embodyserial/listeners.py` & `embody-serial-1.0.9/src/embodyserial/listeners.py`

 * *Files 25% similar despite different names*

```diff
@@ -27,7 +27,32 @@
 class ConnectionListener(ABC):
     """Listener interface for being notified of connection changes."""
 
     @abstractmethod
     def on_connected(self, connected: bool) -> None:
         """Process connection status."""
         pass
+
+
+class FileDownloadListener(ABC):
+    """Listener interface for being notified of file download progress."""
+
+    @abstractmethod
+    def on_file_download_progress(
+        self, original_file_name: str, size: int, progress: float, kbps: float
+    ) -> None:
+        """Process file download progress."""
+        pass
+
+    @abstractmethod
+    def on_file_download_complete(
+        self, original_file_name: str, path: str, kbps: float
+    ) -> None:
+        """Process file download completion."""
+        pass
+
+    @abstractmethod
+    def on_file_download_failed(
+        self, original_file_name: str, error: Exception
+    ) -> None:
+        """Process file download failure."""
+        pass
```

### Comparing `embody-serial-1.0.8/setup.py` & `embody-serial-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 packages = \
 ['embodyserial']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['embody-codec>1.0.9', 'pyserial>=3.5,<4.0']
+['embody-codec>=1.0.12', 'pyserial>=3.5,<4.0']
 
 entry_points = \
 {'console_scripts': ['embody-serial = embodyserial.cli:main']}
 
 setup_kwargs = {
     'name': 'embody-serial',
-    'version': '1.0.8',
+    'version': '1.0.9',
     'description': 'Communicate with the embody device over a serial port',
     'long_description': '# Embody Serial\n\n[![PyPI](https://img.shields.io/pypi/v/embody-serial.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/embody-serial.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/embody-serial)][python version]\n[![License](https://img.shields.io/pypi/l/embody-serial)][license]\n\n[![Tests](https://github.com/aidee-health/embody-serial/workflows/Tests/badge.svg)][tests]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/embody-serial/\n[status]: https://pypi.org/project/embody-serial/\n[python version]: https://pypi.org/project/embody-serial\n[tests]: https://github.com/aidee-health/embody-serial/actions?workflow=Tests\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\n## Features\n\n- Connects to an EmBody device over the serial port\n- Uses the EmBody protocol to communicate with the device\n- Integrates with [the EmBody Protocol Codec](https://github.com/aidee-health/embody-protocol-codec) project\n- Asynchronous send without having to wait for response\n- Synchronous send where response message is returned\n- Send facade for protocol agnostic communication with device\n- Provides callback interfaces for incoming messages, response messages and connect/disconnect\n- All methods and callbacks are threadsafe\n- Separate threads for send, receive and callback processing\n- Type safe code using [mypy](https://mypy.readthedocs.io/) for type checking\n\n## Requirements\n\n- Python 3.9\n- Access to private Aidee Health repositories on Github\n\n## Installation\n\nYou can install _Embody Serial_ via [pip]:\n\n```console\n$ pip install embody-serial\n```\n\nThis adds `embody-serial` as a library, but also provides the CLI application with the same name.\n\n## Usage\n\nA very basic example where you send a message request and get a response:\n\n```python\nfrom embodyserial.embodyserial import EmbodySerial\nfrom embodyserial.helpers import EmbodySendHelper\n\nembody_serial = EmbodySerial()\nsend_helper = EmbodySendHelper(sender=embody_serial)\nprint(f"Serial no: {send_helper.get_serial_no()}")\nembody_serial.shutdown()\n```\n\nIf you want to see more of what happens under the hood, activate debug logging before setting up `EmbodySerial`:\n\n```python\nimport logging\n\nlogging.basicConfig(level=logging.DEBUG)\n```\n\n## Using the application from the command line\n\nThe application also provides a CLI application that is automatically added to the path when installing via pip.\n\nOnce installed with pip, type:\n\n```\nembody-serial --help\n```\n\nTo see which options are available.\n\n> **Note**\n> The serial port is automatically detected, but can be overridden by using the `--device` option.\n\n### Example - List all attribute values\n\n```shell\nembody-serial --get-all\n```\n\n### Example - Get serial no of device\n\n```shell\nembody-serial --get serialno\n```\n\n### Example - List files over serial port\n\n```shell\nembody-serial --list-files\n```\n\n### Example - Set time current time (UTC)\n\n```shell\nembody-serial --set-time\n```\n\n### Example - Download files\n\n```shell\nembody-serial --download-files\n```\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n[file an issue]: https://github.com/aidee-health/embody-serial/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/aidee-health/embody-serial/blob/main/LICENSE\n[contributor guide]: https://github.com/aidee-health/embody-serial/blob/main/CONTRIBUTING.md\n[command-line reference]: https://embody-serial.readthedocs.io/en/latest/usage.html\n',
     'author': 'Aidee Health AS',
     'author_email': 'hello@aidee.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/aidee-health/embody-serial',
```

### Comparing `embody-serial-1.0.8/PKG-INFO` & `embody-serial-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: embody-serial
-Version: 1.0.8
+Version: 1.0.9
 Summary: Communicate with the embody device over a serial port
 Home-page: https://github.com/aidee-health/embody-serial
 License: MIT
 Author: Aidee Health AS
 Author-email: hello@aidee.io
 Requires-Python: >=3.8,<=3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: embody-codec (>1.0.9)
+Requires-Dist: embody-codec (>=1.0.12)
 Requires-Dist: pyserial (>=3.5,<4.0)
 Project-URL: Changelog, https://github.com/aidee-health/embody-serial/releases
 Project-URL: Repository, https://github.com/aidee-health/embody-serial
 Description-Content-Type: text/markdown
 
 # Embody Serial
```

