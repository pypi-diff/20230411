# Comparing `tmp/galaxypad-1.0.0-py3-none-any.whl.zip` & `tmp/galaxypad-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 8851 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat       67 b- defN 23-Apr-01 11:42 galaxypad/__init__.py
--rw-rw-rw-  2.0 fat     1832 b- defN 23-Apr-02 19:47 galaxypad/__main__.py
--rw-rw-rw-  2.0 fat    15738 b- defN 23-Apr-02 18:36 galaxypad/pad.py
--rw-rw-rw-  2.0 fat     5163 b- defN 23-Apr-02 20:38 galaxypad-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-02 20:38 galaxypad-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       54 b- defN 23-Apr-02 20:38 galaxypad-1.0.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-02 20:38 galaxypad-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      631 b- defN 23-Apr-02 20:38 galaxypad-1.0.0.dist-info/RECORD
-8 files, 23587 bytes uncompressed, 7749 bytes compressed:  67.1%
+Zip file size: 7862 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat       67 b- defN 23-Apr-10 15:12 galaxypad/__init__.py
+-rw-rw-rw-  2.0 fat     1517 b- defN 23-Apr-10 17:18 galaxypad/__main__.py
+-rw-rw-rw-  2.0 fat    13233 b- defN 23-Apr-10 17:48 galaxypad/pad.py
+-rw-rw-rw-  2.0 fat     4804 b- defN 23-Apr-10 18:44 galaxypad-1.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-10 18:44 galaxypad-1.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       54 b- defN 23-Apr-10 18:44 galaxypad-1.0.1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-10 18:44 galaxypad-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      631 b- defN 23-Apr-10 18:44 galaxypad-1.0.1.dist-info/RECORD
+8 files, 20408 bytes uncompressed, 6760 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: galaxypad/__main__.py
 Comment: 
 
 Filename: galaxypad/pad.py
 Comment: 
 
-Filename: galaxypad-1.0.0.dist-info/METADATA
+Filename: galaxypad-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: galaxypad-1.0.0.dist-info/WHEEL
+Filename: galaxypad-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: galaxypad-1.0.0.dist-info/entry_points.txt
+Filename: galaxypad-1.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: galaxypad-1.0.0.dist-info/top_level.txt
+Filename: galaxypad-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: galaxypad-1.0.0.dist-info/RECORD
+Filename: galaxypad-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## galaxypad/__init__.py

```diff
@@ -1,4 +1,4 @@
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 __author__ = "Aurum"
 
 from .pad import *
```

## galaxypad/__main__.py

```diff
@@ -1,46 +1,42 @@
 import argparse
 import sys
 
 from . import pad
 
 
 def handle_dolphin(args):
-    output_folder_path: str = args.output_folder_path
-    save_data_path: str = args.save_data_path
-    save_data_index: int = args.save_data_index
-
     try:
         addr_pad_recorder_info_ptr: int = int(args.address, 0)
     except ValueError:
         print("Error! Address has an unknown number format!", file=sys.stderr)
         return
 
     print("Welcome to galaxypad! To find out how to set up the PAD recorder in a galaxy, please refer to the GitHub\n"
           "repository's README file! If you want to cancel the tool's execution, press CTRL+C any time. To stop\n"
           "recording, press 2 on the first player's Wiimote!\n"
           "------------------------------------------------------------------------------")
     try:
-        pad.record_pad_from_dolphin(output_folder_path, save_data_path, save_data_index, addr_pad_recorder_info_ptr)
+        pad.record_pad_from_dolphin(args.output_folder_path, addr_pad_recorder_info_ptr)
     except KeyboardInterrupt:
         print("Execution canceled.")
+    except RuntimeError as e:
+        print(f"An error occurred: {str(e)}")
 
 
 def main():
     parser = argparse.ArgumentParser(description="Record PAD playback in SMG2 from Dolphin memory.")
 
-    if len(sys.argv) == 1:
-        parser.print_help(sys.stderr)
-        sys.exit(1)
-
     parser.add_argument("-address", nargs="?", default=f"0x{pad.ADDR_PAD_RECORDER_INFO_PTR:08X}", help="address from which the tool retrieves PadRecordInfo*")
     parser.add_argument("output_folder_path", help="folder to save PAD files to")
-    parser.add_argument("save_data_path", help="GameData.bin file to extract game data from")
-    parser.add_argument("save_data_index", type=int, help="player save slot index, starts at 1, usually ends at 3")
     parser.set_defaults(func=handle_dolphin)
 
+    if len(sys.argv) == 1:
+        parser.print_help(sys.stderr)
+        sys.exit(1)
+
     args = parser.parse_args()
     args.func(args)
 
 
 if __name__ == '__main__':
     main()
```

## galaxypad/pad.py

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 from io import BytesIO
 
 import sys
+import time
 import os.path
 import struct
 import dolphin_memory_engine
 
-__all__ = ["write_pad_header", "write_game_data", "write_packet_header", "compress_kpad_states", "align_stream_32",
-           "calc_memory_checksum", "extract_save_file_header", "extract_save_block_offsets"]
+__all__ = ["write_pad_header", "write_game_data", "write_packet_header", "compress_kpad_states", "align_stream_32"]
 
 
 def validate_ptr(name: str):
     def inner(func):
         def wrapper(*args, **kwargs):
             if args[0] == 0:
                 raise IndexError(f"{name} is NULL!")
@@ -36,14 +36,16 @@
 ADDR_PAD_RECORDER_INFO_PTR = 0x80003FFC
 OFFSET_UPDATE_FRAME = 0x00
 OFFSET_READ_DATA_INFO = 0x04
 OFFSET_RECORDER_MODE = 0x08
 OFFSET_STAGE_NAME_PTR = 0x0C
 OFFSET_RESTART_ID = 0x10
 OFFSET_RESTART_ZONE_ID = 0x14
+OFFSET_BACKUP_GAME_DATA_PTR = 0x18
+OFFSET_BACKUP_GAME_DATA_SIZE = 0x1C
 
 
 def dolphin_get_game_id() -> str:
     """
     Reads and returns the game's ID name from Dolphin's emulated game memory.
 
     :return: the game's ID name.
@@ -144,14 +146,28 @@
         status = dolphin_memory_engine.read_bytes(status_ptr, 0xF0)
         statuses.append(status)
         status_ptr += 0xF0
 
     return statuses
 
 
+@validate_ptr("PadRecorderInfo*")
+def dolphin_read_backup_game_data(pad_recorder_info_ptr: int) -> bytes:
+    """
+    Reads the GameData backup associated with the PadRecordInfo in Dolphin's emulated game memory and returns it.
+
+    :param pad_recorder_info_ptr: the pointer to PadRecordInfo.
+    :return: the GameData backup read.
+    """
+    backup_ptr = dolphin_read_u32(pad_recorder_info_ptr + OFFSET_BACKUP_GAME_DATA_PTR)
+    backup_size = dolphin_read_u32(pad_recorder_info_ptr + OFFSET_BACKUP_GAME_DATA_SIZE)
+
+    return dolphin_memory_engine.read_bytes(backup_ptr, backup_size)
+
+
 # ----------------------------------------------------------------------------------------------------------------------
 # PAD writer helpers
 
 def write_pad_header(stream):
     """
     Writes a PAD format header to the specified stream.
 
@@ -221,181 +237,90 @@
     :param stream: the stream to write to.
     """
     padding_size = ((stream.tell() + 31) & ~31) - stream.tell()
     stream.write(bytes(padding_size))
 
 
 # ----------------------------------------------------------------------------------------------------------------------
-# GameData.bin helpers
-
-def calc_memory_checksum(data: bytes | bytearray, offset: int, length: int) -> int:
-    """
-    Calculates the ``MemoryUtil`` hash over the specified bytes and returns it. The number of bytes should be even.
-
-    :param data: the buffer containing the bytes to calculate the hash over.
-    :param offset: the offset from which to start calculating the hash.
-    :param length: the number of bytes to be hashed.
-    :return: the calculated hash.
-    """
-    hi = 0
-    lo = 0
-
-    for _ in range(length // 2):
-        word = data[offset] << 8 | data[offset+1]
-        offset += 2
-        hi += word
-        lo += ~word
-
-    return (hi & 0xFFFF) << 16 | lo & 0xFFFF
-
-
-def extract_save_file_header(data: bytes | bytearray, offset: int) -> tuple[int, int, int, int]:
-    """
-    Extracts the save data's header information and returns it. This consists of the saved hash, the number of players,
-    the number of save blocks and the total save data size.
-
-    :param data: the buffer containing the save data.
-    :param offset: the save data's starting offset into the buffer.
-    :return: a tuple consisting of the information.
-    """
-    return struct.unpack_from(">4I", data, offset)
-
-
-def extract_save_block_offsets(data: bytes | bytearray, offset: int, blocks_count: int) -> dict[str, int]:
-    """
-    Extracts name:offset pairs for the save data blocks contained in the specified save data.
-
-    :param data: the buffer containing the save data.
-    :param offset: the offset to the save data blocks.
-    :param blocks_count: the number of save data blocks.
-    :return: the table of name:offset pairs.
-    """
-    offsets: dict[str, int] = {}
+# GameData helpers
 
-    for _ in range(blocks_count):
-        raw_block_name, block_offset = struct.unpack_from(">12sI", data, offset)
-        block_name = raw_block_name.decode("ascii").strip("\0")
-        offset += 0x10
-
-        offsets[block_name] = block_offset
-
-    return offsets
-
-
-# ----------------------------------------------------------------------------------------------------------------------
-
-
-def extract_game_data_from_save_file(save_file_path: str, index: int) -> bytes | None:
-    # 1 - Validate path
-    if not os.path.exists(save_file_path):
-        print(f"Error! Save file '{save_file_path}' doesn't exist!", file=sys.stderr)
-        return None
-    if not os.path.isfile(save_file_path):
-        print(f"Error! Path '{save_file_path}' is not a file!", file=sys.stderr)
-        return None
-
-    # 2 - Read & validate GameData file
-    print(f"Loading save data from '{save_file_path}'...")
-
-    with open(save_file_path, "rb") as f:
-        data = f.read()
-
-    if len(data) < 16:
-        print("Error! Save data is too small!", file=sys.stderr)
-
-    calculated_hash = calc_memory_checksum(data, 0x4, len(data) - 4)
-    saved_hash, user_files_count, save_blocks_count, _ = extract_save_file_header(data, 0)
-
-    if saved_hash != calculated_hash:
-        print(f"Error! Save data appears to be corrupted!", file=sys.stderr)
-        return None
-
-    if index < 1 or index > user_files_count:
-        print(f"Error! Save data does not contain data for player #{index}", file=sys.stderr)
-        return None
-
-    # 3 - Locate & extract GameData
-    save_blocks = extract_save_block_offsets(data, 0x10, save_blocks_count)
-    game_data_name = f"user{index}"
-
-    if game_data_name not in save_blocks:
-        print(f"Error! Save data does not contain GameData block for player #{index}!", file=sys.stderr)
-        return None
-
-    src = BytesIO(data)
-    src.seek(save_blocks[game_data_name])
+def truncate_game_data(game_data: bytes) -> bytes:
+    src = BytesIO(game_data)
     game_data_header = src.read(4)
     sections_count = game_data_header[0x1]
 
     dest = BytesIO()
     dest.write(game_data_header)
 
     for _ in range(sections_count):
         section_header = src.read(12)
         section_data_length = struct.unpack_from(">I", section_header, 0x8)[0] - 12
         section_data = src.read(section_data_length)
 
         dest.write(section_header)
         dest.write(section_data)
 
-    print(f"Extracted game data for player #{index}!")
-
     return dest.getbuffer().tobytes()
 
 
-def record_pad_from_dolphin(output_folder_path: str, save_data_path: str, save_data_index: int,
-                            addr_pad_recorder_info_ptr: int = ADDR_PAD_RECORDER_INFO_PTR):
+# ----------------------------------------------------------------------------------------------------------------------
+# Main functionality
+
+def record_pad_from_dolphin(output_folder_path: str, addr_pad_recorder_info_ptr: int = ADDR_PAD_RECORDER_INFO_PTR):
     pad_recorder_info_ptr = 0
     recorder_state = RECORDER_MODE_WAITING
     game_id = UNINITIALIZED_GAME_ID
 
-    # 1 - Validate the paths
     if os.path.exists(output_folder_path) and not os.path.isdir(output_folder_path):
         print(f"Error! Path '{output_folder_path}' is not a folder!", file=sys.stderr)
 
-    # 2 - Load UserFile
-    game_data = extract_game_data_from_save_file(save_data_path, save_data_index)
-
-    if game_data is None:
-        return
-
-    # 3 - Hook to Dolphin and check if game ID is supported
+    # 2 - Hook to Dolphin and check if game ID is supported
     print("Waiting for Dolphin...")
 
     while not dolphin_memory_engine.is_hooked():
+        sleep_millis(500)
         dolphin_memory_engine.hook()
 
     while game_id == UNINITIALIZED_GAME_ID:
+        sleep_millis(500)
         game_id = dolphin_get_game_id()
 
     print(f"Hooked to Dolphin, game ID is {game_id}!")
 
     if game_id not in VALID_GAME_IDS:
         print("WARNING! Detected game's ID does not appear to be SMG2, tool may fail!")
 
-    # 4 - Find PadRecorderInfo and wait for recording
+    # 3 - Find PadRecorderInfo and wait for recording
     print(f"Searching for PadRecorderInfo* at 0x{addr_pad_recorder_info_ptr:08X}...")
 
     while pad_recorder_info_ptr == 0:
+        sleep_millis(250)
         pad_recorder_info_ptr = dolphin_read_u32(addr_pad_recorder_info_ptr)
 
     print("Waiting for PadRecordHelper...")
 
-    while recorder_state in [RECORDER_MODE_WAITING, RECORDER_MODE_PREPARING]:
+    while recorder_state == RECORDER_MODE_WAITING:
+        sleep_millis(250)
         recorder_state = dolphin_read_recorder_mode(pad_recorder_info_ptr)
 
     if recorder_state == RECORDER_MODE_STOPPED:
         print("Aborted recording! Wait for scene to reset, then start again!")
         dolphin_memory_engine.un_hook()
         return
 
+    game_data = dolphin_read_backup_game_data(pad_recorder_info_ptr)
+    game_data = truncate_game_data(game_data)
+
+    while recorder_state == RECORDER_MODE_PREPARING:
+        sleep_millis(250)
+        recorder_state = dolphin_read_recorder_mode(pad_recorder_info_ptr)
+
     # 5 - Get general information and prepare output
     stage_name = dolphin_read_stage_name(pad_recorder_info_ptr)
     restart_id = dolphin_read_restart_id(pad_recorder_info_ptr)
-    next_frame = -1
     total_frames = 0
 
     print(f"Started recording for spawn ID {restart_id} in {stage_name}!")
 
     pad_folder_path = os.path.join(output_folder_path, stage_name)
     pad_file_path = os.path.join(pad_folder_path, f"Dreamer{restart_id}.pad")
     os.makedirs(pad_folder_path, exist_ok=True)
@@ -403,25 +328,32 @@
     with open(pad_file_path, "wb") as f:
         write_pad_header(f)
         write_game_data(f, game_data)
 
         current_packet_index = 0
         previous_state = bytearray(240)
 
+        current_frame = dolphin_read_update_frame(pad_recorder_info_ptr)
+        next_frame = (current_frame + 1) & 0xFFFFFFFF
+
         while recorder_state == RECORDER_MODE_RECORDING:
             # Get current update frame
             current_frame = dolphin_read_update_frame(pad_recorder_info_ptr)
-            if next_frame == -1:
-                next_frame = current_frame
-            if current_frame != next_frame:
+
+            if current_frame == ((next_frame - 1) & 0xFFFFFFFF):
                 continue
+            elif current_frame != next_frame:
+                print("Aborted recording due to a synchronization error!")
+                return
+
             next_frame = (current_frame + 1) & 0xFFFFFFFF
 
             # Still recording?
             recorder_state = dolphin_read_recorder_mode(pad_recorder_info_ptr)
+
             if recorder_state != RECORDER_MODE_RECORDING:
                 break
 
             # Dump KPADStatus structs from memory
             status_dumps = dolphin_read_kpad_statuses(pad_recorder_info_ptr)
             status_count = len(status_dumps)
             total_frames += 1
@@ -433,15 +365,19 @@
             current_packet_index += 1
 
             # Dummy packet for player 2 input
             write_packet_header(f, current_packet_index, 0, 0)
             current_packet_index += 1
 
         # Write eof header and align storage
-        write_packet_header(f, current_packet_index + 32, 192, 0)
+        write_packet_header(f, current_packet_index + 192, 0, 0)
         align_stream_32(f)
 
         print("Stopped recording!")
 
     dolphin_memory_engine.un_hook()
 
     print(f"Dumped {total_frames} KPAD frames (approx. {total_frames // 60} seconds) to '{pad_file_path}'.")
+
+
+def sleep_millis(millis: int):
+    time.sleep(millis / 1000)
```

## Comparing `galaxypad-1.0.0.dist-info/METADATA` & `galaxypad-1.0.1.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxypad
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python tool to record PAD playback for Super Mario Galaxy 2
 Home-page: https://github.com/SunakazeKun/galaxypad
 Author: Aurum
 License: gpl-3.0
 Keywords: nintendo,super-mario-galaxy-2,pad,dolphin,modding
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -20,73 +20,57 @@
 **galaxypad** is a Python command-line tool to record input playback files (PAD files) for [Tip Networks](https://www.mariowiki.com/Tip_Network) and [Cosmic Spirits](https://www.mariowiki.com/Cosmic_Spirit) in **Super Mario Galaxy 2**. The tool reads relevant information from [Dolphin Emulator](https://dolphin-emu.org/)'s emulated game memory and automatically produces a PAD file after recording stopped. The tool requires at least **Python 3.10**. It should also work with 3.11 and newer versions, but this hasn't been tested. Furthermore, it uses [py-dolphin-memory-engine](https://github.com/henriquegemignani/py-dolphin-memory-engine) to interact with Dolphin's game memory. In order to record player input during gameplay, [Syati](https://github.com/SunakazeKun/Syati)'s *PadRecord* code is required to supply the information from the game to this tool.
 
 It is available on PyPI, meaning that you can easily install it with pip:
 ```
 pip install galaxypad
 ```
 
+# Limitations
+There are gameplay-related aspects that Tip Networks and Cosmic Spirits don't account for. Keep these in mind when you want to record and play inputs!
+
+- You should only record playback when playing as Mario. Both objects will be disabled when playing as Luigi.
+- Both objects disable the Star Pointer completely. Thus, Mario can't interact with objects that require the Star Pointer, for example Pull Stars and Grapple Flowers.
+- The game's pseudo-random number generator (PRNG) won't be reseeded to account for random events, such as enemies moving in random directions. Therefore, it can happen in some scenarios that the player gets damaged by enemies.
+
 # Usage
 In this section, it is assumed that the game you want to record player input in already uses Syati's *PadRecord* code. The general usage is this:
 ```
-usage: galaxypad [-h] [-address [ADDRESS]] output_folder_path save_data_path save_data_index
+usage: galaxypad [-h] [-address [ADDRESS]] output_folder_path
 
 Record PAD playback in SMG2 from Dolphin memory.
 
 positional arguments:
   output_folder_path  folder to save PAD files to
-  save_data_path      GameData.bin file to extract game data from
-  save_data_index     player save slot index, starts at 1, usually ends at 3
 
 options:
   -h, --help          show this help message and exit
   -address [ADDRESS]  address from which the tool retrieves PadRecordInfo*
 ```
 
 The ``-address`` option is not required, as the tool assumes ``PadRecordInfo*`` is supplied at ``0x80003FFC`` by default.
 
-By default, Dolphin Emulator saves Super Mario Galaxy 2 save files to ``C:/User/<YOURNAME>/Documents/Dolphin Emulator/Wii/title/00010000/<HEXID>/data/GameData.bin`` where ``<YOURNAME>`` is your username and ``<HEXID>`` is your game's ID. However, the ID depends on the version played:
-
-| Version | Hexadecimal Game ID |
-| ------- | ------------ |
-| **SB4E** (Americas) | ``53423445`` |
-| **SB4P** (Europe/Australia) | ``53423450`` |
-| **SB4J** (Japan) | ``5342344a`` |
-| **SB4K** (South Korea) | ``5342344b`` |
-| **SB4W** (Taiwan/Hong Kong) | ``53423457`` |
-
-
-Super Mario Galaxy 2 has three save slots with the following indexes.
-
-| Index | Slot |
-| ----- | ---- |
-| 1 | Left |
-| 2 | Center |
-| 3 | Right |
-
 # Recording
 Before you can record playback, you need to add the following things in your galaxy first:
 
 1. A player spawn point from which the recording should start. This spawn point should be used by Tip Networks and Cosmic Spirits too.
 2. A ``PadRecordHelper`` object in the same zone as the previously added spawn point. Its Obj_arg0 has to be set to the  added spawn point's MarioNo value.
 
 Now you are ready to use the tool:
 
 1. Launch the modded game in Dolphin and start this command-line tool like explained in previous sections.
 3. While the game is running, pay attention to the tool's console output to verify that everything is running correctly.
 4. Once you are in the desired galaxy, go to where you placed PadRecordHelper. It doesn't use a model, but an A button icon will be displayed on the screen when you are close to it.
-5. Once you press A, the scene will reset. After the scene reloaded, the recording will start.
+5. Once you press A, the scene will reset. After the scene has reloaded, the recording will start.
 6. If you desire to stop recording, press 2 on the first player's Wiimote.
 
-The tool keeps you informed about its current state and it should inform you when something goes wrong. Here's an example from one of my tests:
+The tool keeps you informed about its current state, and it should inform you when something goes wrong. Here's an example from one of my tests:
 ```
-Loading save data from 'D:\Dokumente\Dolphin Emulator\Wii\title\00010000\53423450\data\GameData.bin'...
-Extracted game data for player #1!
 Waiting for Dolphin...
 Hooked to Dolphin, game ID is SB4P!
 Searching for PadRecorderInfo* at 0x80003FFC...
 Waiting for PadRecordHelper...
-Started recording for spawn ID 2 in RedBlueExGalaxy!
+Started recording for spawn ID 0 in RedBlueExGalaxy!
 Stopped recording!
-Dumped 629 KPAD frames (approx. 10 seconds) to '.\RedBlueExGalaxy\Dreamer2.pad'.
+Dumped 3075 KPAD frames (approx. 51 seconds) to '.\RedBlueExGalaxy\Dreamer0.pad'.
 ```
 
 After recording, you can build a Ghost.arc containing the PAD file. However, this is beyond the scope of this tool. In final releases of your levels, you don't want players to interact with PadRecordHelper objects, so make sure to remove them once they are not needed anymore.
```

