# Comparing `tmp/ascvid-1.3.0.tar.gz` & `tmp/ascvid-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascvid-1.3.0.tar", last modified: Sat Apr  8 16:52:44 2023, max compression
+gzip compressed data, was "ascvid-1.4.0.tar", last modified: Tue Apr 11 16:37:51 2023, max compression
```

## Comparing `ascvid-1.3.0.tar` & `ascvid-1.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-04-08 16:52:44.634208 ascvid-1.3.0/
--rw-r--r--   0 adam      (1003) adam      (1003)    35149 2023-04-05 16:13:01.000000 ascvid-1.3.0/LICENSE
--rw-r--r--   0 adam      (1003) adam      (1003)     3405 2023-04-08 16:52:44.630874 ascvid-1.3.0/PKG-INFO
--rw-r--r--   0 adam      (1003) adam      (1003)     2660 2023-04-08 16:52:21.000000 ascvid-1.3.0/README.rst
-drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-04-08 16:52:44.630874 ascvid-1.3.0/ascvid/
--rw-r--r--   0 adam      (1003) adam      (1003)       22 2023-04-06 09:16:15.000000 ascvid-1.3.0/ascvid/__init__.py
--rw-r--r--   0 adam      (1003) adam      (1003)       59 2023-04-05 16:35:01.000000 ascvid-1.3.0/ascvid/__main__.py
--rw-r--r--   0 adam      (1003) adam      (1003)      831 2023-04-07 16:57:03.000000 ascvid-1.3.0/ascvid/audio.py
--rw-r--r--   0 adam      (1003) adam      (1003)     2933 2023-04-08 16:44:11.000000 ascvid-1.3.0/ascvid/cli.py
--rw-r--r--   0 adam      (1003) adam      (1003)     1130 2023-04-08 09:37:55.000000 ascvid-1.3.0/ascvid/getcol.py
--rw-r--r--   0 adam      (1003) adam      (1003)      519 2023-04-06 15:39:53.000000 ascvid-1.3.0/ascvid/logger.py
--rw-r--r--   0 adam      (1003) adam      (1003)     5278 2023-04-08 16:44:37.000000 ascvid-1.3.0/ascvid/player.py
--rw-r--r--   0 adam      (1003) adam      (1003)     1314 2023-04-08 16:17:56.000000 ascvid-1.3.0/ascvid/run_terminal.py
--rw-r--r--   0 adam      (1003) adam      (1003)      641 2023-04-07 16:55:04.000000 ascvid-1.3.0/ascvid/timer.py
-drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-04-08 16:52:44.630874 ascvid-1.3.0/ascvid.egg-info/
--rw-r--r--   0 adam      (1003) adam      (1003)     3405 2023-04-08 16:52:44.000000 ascvid-1.3.0/ascvid.egg-info/PKG-INFO
--rw-r--r--   0 adam      (1003) adam      (1003)      367 2023-04-08 16:52:44.000000 ascvid-1.3.0/ascvid.egg-info/SOURCES.txt
--rw-r--r--   0 adam      (1003) adam      (1003)        1 2023-04-08 16:52:44.000000 ascvid-1.3.0/ascvid.egg-info/dependency_links.txt
--rw-r--r--   0 adam      (1003) adam      (1003)       43 2023-04-08 16:52:44.000000 ascvid-1.3.0/ascvid.egg-info/entry_points.txt
--rw-r--r--   0 adam      (1003) adam      (1003)       46 2023-04-08 16:52:44.000000 ascvid-1.3.0/ascvid.egg-info/requires.txt
--rw-r--r--   0 adam      (1003) adam      (1003)        7 2023-04-08 16:52:44.000000 ascvid-1.3.0/ascvid.egg-info/top_level.txt
--rw-r--r--   0 adam      (1003) adam      (1003)       38 2023-04-08 16:52:44.634208 ascvid-1.3.0/setup.cfg
--rw-r--r--   0 adam      (1003) adam      (1003)     3587 2023-04-08 16:51:52.000000 ascvid-1.3.0/setup.py
+drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-04-11 16:37:51.809427 ascvid-1.4.0/
+-rw-r--r--   0 adam      (1003) adam      (1003)    35149 2023-04-05 16:13:01.000000 ascvid-1.4.0/LICENSE
+-rw-r--r--   0 adam      (1003) adam      (1003)     3471 2023-04-11 16:37:51.806094 ascvid-1.4.0/PKG-INFO
+-rw-r--r--   0 adam      (1003) adam      (1003)     2660 2023-04-08 16:52:21.000000 ascvid-1.4.0/README.rst
+drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-04-11 16:37:51.806094 ascvid-1.4.0/ascvid/
+-rw-r--r--   0 adam      (1003) adam      (1003)       22 2023-04-06 09:16:15.000000 ascvid-1.4.0/ascvid/__init__.py
+-rw-r--r--   0 adam      (1003) adam      (1003)       59 2023-04-05 16:35:01.000000 ascvid-1.4.0/ascvid/__main__.py
+-rw-r--r--   0 adam      (1003) adam      (1003)      819 2023-04-10 19:20:07.000000 ascvid-1.4.0/ascvid/audio.py
+-rw-r--r--   0 adam      (1003) adam      (1003)     3031 2023-04-11 16:31:56.000000 ascvid-1.4.0/ascvid/cli.py
+-rw-r--r--   0 adam      (1003) adam      (1003)     1130 2023-04-08 09:37:55.000000 ascvid-1.4.0/ascvid/getcol.py
+-rw-r--r--   0 adam      (1003) adam      (1003)      519 2023-04-06 15:39:53.000000 ascvid-1.4.0/ascvid/logger.py
+-rw-r--r--   0 adam      (1003) adam      (1003)     6158 2023-04-11 16:29:07.000000 ascvid-1.4.0/ascvid/player.py
+-rw-r--r--   0 adam      (1003) adam      (1003)     1314 2023-04-08 16:17:56.000000 ascvid-1.4.0/ascvid/run_terminal.py
+-rw-r--r--   0 adam      (1003) adam      (1003)      641 2023-04-07 16:55:04.000000 ascvid-1.4.0/ascvid/timer.py
+drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-04-11 16:37:51.806094 ascvid-1.4.0/ascvid.egg-info/
+-rw-r--r--   0 adam      (1003) adam      (1003)     3471 2023-04-11 16:37:51.000000 ascvid-1.4.0/ascvid.egg-info/PKG-INFO
+-rw-r--r--   0 adam      (1003) adam      (1003)      367 2023-04-11 16:37:51.000000 ascvid-1.4.0/ascvid.egg-info/SOURCES.txt
+-rw-r--r--   0 adam      (1003) adam      (1003)        1 2023-04-11 16:37:51.000000 ascvid-1.4.0/ascvid.egg-info/dependency_links.txt
+-rw-r--r--   0 adam      (1003) adam      (1003)       43 2023-04-11 16:37:51.000000 ascvid-1.4.0/ascvid.egg-info/entry_points.txt
+-rw-r--r--   0 adam      (1003) adam      (1003)       57 2023-04-11 16:37:51.000000 ascvid-1.4.0/ascvid.egg-info/requires.txt
+-rw-r--r--   0 adam      (1003) adam      (1003)        7 2023-04-11 16:37:51.000000 ascvid-1.4.0/ascvid.egg-info/top_level.txt
+-rw-r--r--   0 adam      (1003) adam      (1003)       38 2023-04-11 16:37:51.809427 ascvid-1.4.0/setup.cfg
+-rw-r--r--   0 adam      (1003) adam      (1003)     3668 2023-04-11 16:34:44.000000 ascvid-1.4.0/setup.py
```

### Comparing `ascvid-1.3.0/LICENSE` & `ascvid-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ascvid-1.3.0/PKG-INFO` & `ascvid-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascvid
-Version: 1.3.0
+Version: 1.4.0
 Summary: ASCII Video player.
 Home-page: https://github.com/jenca-adam/ascvid
 Author: Adam Jenca
 Author-email: jenca.a@gjh.sk
 Keywords: Video,ASCII,Terminal
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -66,11 +66,12 @@
       -t, --title TEXT        Sets the title of the video. If not set, file name
                               will be used instead
       -h, --hide-title        hides the title
       -n, --new-window        Opens in a new terminal window
       -t, --term TEXT         Specify terminal in format '<terminal command> <run
                               command switch> {}'
       -o, --outfile TEXT      Specify output file
+      -d, --debug             Debug mode: show current/target fps
 
       --help                  Show this message and exit.
```

### Comparing `ascvid-1.3.0/README.rst` & `ascvid-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `ascvid-1.3.0/ascvid/audio.py` & `ascvid-1.4.0/ascvid/audio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import sounddevice as sd
 import time
 import moviepy.editor as mp
 from .timer import Timer
 class Audio:
     def __init__(self,clip):
         self.clip=clip
-        self.audio=clip.audio.to_soundarray()
-        self.fps=clip.audio.fps
+        self.audio=clip.to_soundarray()
+        self.fps=clip.fps
         self.start_time=-1
         self.resume_time=0
         self._playing=False
         self.timer=Timer()
     def play(self):
         self.timer.start()
         sd.play(self.audio,self.fps)
```

### Comparing `ascvid-1.3.0/ascvid/cli.py` & `ascvid-1.4.0/ascvid/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 @click.option("--fast","-F",is_flag=True,default=False,help="Toggles off resizing each frame individually, rather resizes the entire video. Use this if the video is lagging too much.")
 @click.option("--disable-controls","-d",is_flag=True,default=False,help="Disables pausing the video")
 @click.option("--title","-t",default=None,help="Sets the title of the video. If not set, file name will be used instead")
 @click.option("--hide-title","-h",default=False,is_flag=True,help="hides the title")
 @click.option("--new-window","-n",is_flag=True,help="Opens in a new terminal window")
 @click.option("--term","-t",default=None,help="Specify terminal in format '<terminal command> <run command switch> {}'")
 @click.option("--outfile","-o",default=None,help="Specify output file")
-def main(file,hide_cursor,no_audio,fps,char,no_color,ascii,no_truecolor,fast,disable_controls,title,hide_title,new_window,term,outfile):
+@click.option("--debug","-d",is_flag=True,help="Debug mode: show current/target FPS")
+def main(file,hide_cursor,no_audio,fps,char,no_color,ascii,no_truecolor,fast,disable_controls,title,hide_title,new_window,term,outfile,debug):
     if new_window:
         cmd = [sys.executable,"-m","ascvid",file]
         if hide_cursor:
             cmd.extend(["-H"])
         if no_audio:
             cmd.extend(["-A"])
         if fps is not None:
@@ -46,8 +47,8 @@
         run_term(' '.join(cmd),term)
         return
     if fps and fps!="max":
         fps=int(fps)
     play_audio=not no_audio
     colored = not no_color
     truecolor = not no_truecolor
-    play_vid(file,hide_cursor,play_audio,fps,char,colored,truecolor,ascii,fast,disable_controls,title,not hide_title,outfile)
+    play_vid(file,hide_cursor,play_audio,fps,char,colored,truecolor,ascii,fast,disable_controls,title,not hide_title,outfile,debug)
```

### Comparing `ascvid-1.3.0/ascvid/getcol.py` & `ascvid-1.4.0/ascvid/getcol.py`

 * *Files identical despite different names*

### Comparing `ascvid-1.3.0/ascvid/logger.py` & `ascvid-1.4.0/ascvid/logger.py`

 * *Files identical despite different names*

### Comparing `ascvid-1.3.0/ascvid/player.py` & `ascvid-1.4.0/ascvid/player.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 import sys
 import os
 import time
 import cursor
 import threading
 import getkey
 import queue
+import imageio
 from .getcol import closest_color
 from .logger import print_error,print_warning
 from . import audio
+from .timer import Timer
 CHARS = ' .\'`^",:;Il!i><~+_-?][}{1)(|\\/tfjrxnuvczXYUJCLQ0OZmwqpdbkhao*#MW&8%B@$\u2591\u2592\u2593\u2588'
 CLOSEST_CACHE = {}
 CHAR_CACHE = {}
 def fqget(q):
     if q.empty():
         return
     return q.get()
@@ -59,18 +61,22 @@
     if use_ascii:
         return get_character(color,colored,truecolor)
     if truecolor:
         r,g,b=color
         return f"\x1b[38;2;{r};{g};{b}m{char}"
     return f"{closest(color)}{char}"
 
-def show_frame(fr,char,colored,truecolor,use_ascii,resize,hast,tit,out):
+def show_frame(fr,char,colored,truecolor,use_ascii,resize,hast,tit,out,fps,nfps,deb):
     ts=os.get_terminal_size()
     tw=ts.columns
     th=ts.lines
+    if deb:
+        th-=1
+    if tit:
+        th-=1
     if hast:
         th-=1
     out.write('\033[H')
     out.flush()
     d=Image.fromarray(fr)
     if resize:
         dh=d.height//2
@@ -94,96 +100,118 @@
         line=''
         for x in range(d.width):
             r,g,b,*foo=pix[x,y]
             line+=get_pixel((r,g,b),colored,truecolor,use_ascii,char)
         lines.append(line+'\x1b[0m')
     clear(out)
     if hast:
-        print(tit,file=out)
+        print(tit,file=out,flush=True)
+    if deb:
+        print(f"{fps:.2f} FPS  => {nfps} FPS",flush=True,file=out)
     print('\n'.join(lines),end="",file=out)
 def mkpos(a):
     if a<0:
         return 0
     return a
-def play_vid(file,hide_cursor=True,play_audio=True,fps=None,char="\u2588",colored=True,truecolor=True,use_ascii=False,fast=False,disable_controls=False,title=None,show_title=True,out=None):
+def play_vid(file,hide_cursor=True,play_audio=True,fps=None,char="\u2588",colored=True,truecolor=True,use_ascii=False,fast=False,disable_controls=False,title=None,show_title=True,out=None,show_dbg=True):
     if out is None:
         out=sys.stdout
     else:
         out=open(out,"w")
     if title is None:
         title=file
 
-    vid=mp.VideoFileClip(file)
+    audio_clip=mp.AudioFileClip(file)
+    if len(audio_clip.reader.buffer)==0:
+        audio_clip=None
+    if fps not in (None,"max"):
+        vid=imageio.read(file,fps=fps,)
+    else:
+        vid=imageio.read(file,)
+    fps=vid.get_meta_data().get("fps",mp.VideoFileClip(file).fps)
     q=queue.Queue()
     settings=None
     if sys.platform.lower().startswith("linux"):
         import tty
         import termios
         settings=termios.tcgetattr(sys.stdin)
 
     if fast:
-        frame_count=int(vid.fps*vid.duration)
+        frame_count=vid.count_frames()
         if frame_count>=10000:
             response=print_warning(f"{file!r} has {frame_count} frames.",ask="Are you sure you want to resize them all at once [y*]")
             if response!="y":
                 sys.exit(1)
         tw=os.get_terminal_size().columns
         th=os.get_terminal_size().lines
-        vh=vid.h
-        vw=vid.w
+        if show_title:
+            th-=1
+        if show_dbg:
+            th-=1
+        vh,vw=vid.get_meta_data()["size"]
         dh=vh//2
         wd=vw-tw
         hd=dh-th
         scale=1
         if wd>0 and hd>0 and wd>=hd:
             scale=tw/vw
         elif wd>0 and hd>0:
             scale=th/dh
         elif wd>0:
             scale=tw/vw
         elif hd>0:
             scale=th/dh
 
-        vid=vid.resize((int(vw*scale),int(dh*scale)))
+        vid=imageio.read(file,size=(int(vw*scale),int(dh*scale)),fps=fps,)
 
-    fps = fps or vid.fps
-    if fps!=vid.fps and fps!="max":
-        vid=vid.set_fps(fps)
     process=None
     audio_stream=None
     if hide_cursor:
         cursor.hide()
-    if play_audio and vid.audio is not None:
-        audio_stream=audio.Audio(vid)
+    if play_audio and audio_clip is not None:
+        audio_stream=audio.Audio(audio_clip)
         audio_stream.play()
     if not disable_controls:
         check_thread=threading.Thread(target=check_paused(q),daemon=True)
         check_thread.start()
     clear(out)
-    try: 
-        for frame in vid.iter_frames():
+    frame_timer=Timer()
+    frame_iterator=vid.iter_data()
+    frindex=0
+    try:
+        frame_timer.start()
+        while True:
+            try:
+                frame=next(frame_iterator)
+            except StopIteration:
+                break
 
             if not disable_controls:
                 resp=fqget(q)
                 if resp==" ":
+                    frame_timer.pause()
                     if audio_stream is not None:
                         audio_stream.pause()
                     while q.get()!=" ":
                         pass
                     if audio_stream is not None:
                         audio_stream.resume()
-            t=time.time()
-            show_frame(frame,char,colored,truecolor,use_ascii,not fast,show_title,title,out)
-            if fps!="max":
-                time.sleep(mkpos(1/fps-(time.time()-t)))
+                    frame_timer.start()
+            current_fps=frindex/frame_timer.curtime
+            show_frame(frame,char,colored,truecolor,use_ascii,not fast,show_title,title,out,current_fps,fps,show_dbg)
+            if fps!="max" and current_fps>fps:
+                time.sleep(mkpos(1/fps))
+            frindex+=1
+    except KeyboardInterrupt:
+        clear(out)
     finally:
         cursor.show()
         out.write("\x1b[0m")
         out.flush()
         if settings is not None:
             time.sleep(0.2)
             termios.tcsetattr(sys.stdin.fileno(), termios.TCSADRAIN, settings)
+    clear(out)
 
-        clear(out)
```

### Comparing `ascvid-1.3.0/ascvid/run_terminal.py` & `ascvid-1.4.0/ascvid/run_terminal.py`

 * *Files identical despite different names*

### Comparing `ascvid-1.3.0/ascvid/timer.py` & `ascvid-1.4.0/ascvid/timer.py`

 * *Files identical despite different names*

### Comparing `ascvid-1.3.0/ascvid.egg-info/PKG-INFO` & `ascvid-1.4.0/ascvid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascvid
-Version: 1.3.0
+Version: 1.4.0
 Summary: ASCII Video player.
 Home-page: https://github.com/jenca-adam/ascvid
 Author: Adam Jenca
 Author-email: jenca.a@gjh.sk
 Keywords: Video,ASCII,Terminal
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -66,11 +66,12 @@
       -t, --title TEXT        Sets the title of the video. If not set, file name
                               will be used instead
       -h, --hide-title        hides the title
       -n, --new-window        Opens in a new terminal window
       -t, --term TEXT         Specify terminal in format '<terminal command> <run
                               command switch> {}'
       -o, --outfile TEXT      Specify output file
+      -d, --debug             Debug mode: show current/target fps
 
       --help                  Show this message and exit.
```

### Comparing `ascvid-1.3.0/setup.py` & `ascvid-1.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-setuptools.setup(name="ascvid",version="1.3.0",description="ASCII Video player.", long_description=
+setuptools.setup(name="ascvid",version="1.4.0",description="ASCII Video player.", long_description=
                  """
 .. image:: https://raw.githubusercontent.com/jenca-adam/ascvid/main/asc.png
 
 ``ascvid`` is an ASCII video player with quite exact results. It is mostly advised to be used under Linux, but it might work on Windows too (its behavior under Mac is untested, and it will likely not work well).
 Here is a little showcase of what it can do: 
 
 .. image:: https://raw.githubusercontent.com/jenca-adam/ascvid/main/rick.gif
@@ -50,19 +50,20 @@
       -t, --title TEXT        Sets the title of the video. If not set, file name
                               will be used instead
       -h, --hide-title        hides the title
       -n, --new-window        Opens in a new terminal window
       -t, --term TEXT         Specify terminal in format '<terminal command> <run
                               command switch> {}'
       -o, --outfile TEXT      Specify output file
+      -d, --debug             Debug mode: show current/target fps
 
       --help                  Show this message and exit.
    
     """,
-                 install_requires=["pillow","moviepy","cursor","numpy","click","sounddevice"],
+                 install_requires=["pillow","moviepy","cursor","numpy","click","sounddevice","av","imageio"],
                  packages=["ascvid"],
                  classifiers=["Development Status :: 4 - Beta","Environment :: Console","Intended Audience :: End Users/Desktop","License :: OSI Approved :: GNU General Public License v3 (GPLv3)","Operating System :: Microsoft :: Windows","Operating System :: POSIX :: Linux","Operating System :: Unix","Programming Language :: Python :: 3.10","Topic :: Multimedia :: Video :: Display"],keywords="Video,ASCII,Terminal",author="Adam Jenca",author_email="jenca.a@gjh.sk",url="https://github.com/jenca-adam/ascvid",entry_points={"console_scripts":["ascvid = ascvid.cli:main"]})
```

