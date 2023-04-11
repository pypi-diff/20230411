# Comparing `tmp/lcapygui-0.5.tar.gz` & `tmp/lcapygui-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lcapygui-0.5.tar", last modified: Sat Mar  4 06:33:37 2023, max compression
+gzip compressed data, was "lcapygui-0.6.tar", last modified: Tue Apr 11 21:09:29 2023, max compression
```

## Comparing `lcapygui-0.5.tar` & `lcapygui-0.6.tar`

### file list

```diff
@@ -1,71 +1,80 @@
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-03-04 06:33:37.763208 lcapygui-0.5/
--rw-rw-r--   0 mph       (1000) mph       (1000)      933 2023-03-04 06:33:37.763208 lcapygui-0.5/PKG-INFO
--rw-rw-r--   0 mph       (1000) mph       (1000)      361 2023-03-04 06:33:37.000000 lcapygui-0.5/README.md
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-03-04 06:33:37.759208 lcapygui-0.5/lcapygui/
--rw-rw-r--   0 mph       (1000) mph       (1000)      567 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/__init__.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      434 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/annotation.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      246 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/annotations.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-03-04 06:33:37.763208 lcapygui-0.5/lcapygui/components/
--rw-rw-r--   0 mph       (1000) mph       (1000)       99 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/components/__init__.py
--rw-rw-r--   0 mph       (1000) mph       (1000)       92 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/components/admittance.py
--rw-rw-r--   0 mph       (1000) mph       (1000)       91 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/components/capacitor.py
--rw-rw-r--   0 mph       (1000) mph       (1000)       94 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/components/cccs.py
--rw-rw-r--   0 mph       (1000) mph       (1000)       94 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/components/ccvs.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     6290 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/components/component.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      884 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/components/connection.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2366 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/components/cpt_maker.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      334 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/components/current_source.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      739 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/components/diode.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      415 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/components/ground.py
--rw-rw-r--   0 mph       (1000) mph       (1000)       91 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/components/impedance.py
--rw-rw-r--   0 mph       (1000) mph       (1000)       90 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/components/inductor.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2702 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/components/opamp.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      113 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/components/port.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      113 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/components/resistor.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3803 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/components/sketch.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3342 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/components/svgparse.py
--rw-rw-r--   0 mph       (1000) mph       (1000)       94 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/components/vccs.py
--rw-rw-r--   0 mph       (1000) mph       (1000)       94 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/components/vcvs.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      334 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/components/voltage_source.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      125 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/components/wire.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1237 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/node.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1842 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/nodes.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-03-04 06:33:37.763208 lcapygui-0.5/lcapygui/scripts/
--rw-rw-r--   0 mph       (1000) mph       (1000)        0 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/scripts/__init__.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1618 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/scripts/lcapytk.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-03-04 06:33:37.763208 lcapygui-0.5/lcapygui/ui/
--rw-rw-r--   0 mph       (1000) mph       (1000)        0 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/ui/__init__.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1669 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/ui/preferences.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-03-04 06:33:37.763208 lcapygui-0.5/lcapygui/ui/tk/
--rw-rw-r--   0 mph       (1000) mph       (1000)        0 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/ui/tk/__init__.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2939 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/ui/tk/cpt_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3683 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/ui/tk/cpt_properties_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1800 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/ui/tk/drawing.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1390 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/ui/tk/equations_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     4003 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/ui/tk/expr_advanced_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1798 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/ui/tk/expr_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      187 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/ui/tk/exprimage.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1760 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/ui/tk/help_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1206 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/ui/tk/inspect_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1916 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/ui/tk/labelentries.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      846 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/ui/tk/lateximage.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3005 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/ui/tk/layer.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    19139 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/ui/tk/lcapytk.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     9398 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/ui/tk/lcapytkm.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      251 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/ui/tk/message_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      907 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/ui/tk/node_properties_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      788 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/ui/tk/plot_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2323 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/ui/tk/plot_properties_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3698 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/ui/tk/preferences_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    16736 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/ui/uimodelbase.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    14686 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui/ui/uimodelmph.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-03-04 06:33:37.759208 lcapygui-0.5/lcapygui.egg-info/
--rw-rw-r--   0 mph       (1000) mph       (1000)      933 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui.egg-info/PKG-INFO
--rw-rw-r--   0 mph       (1000) mph       (1000)     1827 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui.egg-info/SOURCES.txt
--rw-rw-r--   0 mph       (1000) mph       (1000)        1 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui.egg-info/dependency_links.txt
--rw-rw-r--   0 mph       (1000) mph       (1000)       60 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui.egg-info/entry_points.txt
--rw-rw-r--   0 mph       (1000) mph       (1000)      152 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui.egg-info/requires.txt
--rw-rw-r--   0 mph       (1000) mph       (1000)        9 2023-03-04 06:33:37.000000 lcapygui-0.5/lcapygui.egg-info/top_level.txt
--rw-rw-r--   0 mph       (1000) mph       (1000)      103 2023-03-04 06:33:37.000000 lcapygui-0.5/pyproject.toml
--rw-rw-r--   0 mph       (1000) mph       (1000)      287 2023-03-04 06:33:37.763208 lcapygui-0.5/setup.cfg
--rw-rw-r--   0 mph       (1000) mph       (1000)     1350 2023-03-04 06:33:37.000000 lcapygui-0.5/setup.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-04-11 21:09:29.452365 lcapygui-0.6/
+-rw-rw-r--   0 mph       (1000) mph       (1000)      933 2023-04-11 21:09:29.452365 lcapygui-0.6/PKG-INFO
+-rw-rw-r--   0 mph       (1000) mph       (1000)      361 2023-04-11 21:09:29.000000 lcapygui-0.6/README.md
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-04-11 21:09:29.448365 lcapygui-0.6/lcapygui/
+-rw-rw-r--   0 mph       (1000) mph       (1000)      567 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/__init__.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      443 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/annotation.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      246 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/annotations.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-04-11 21:09:29.448365 lcapygui-0.6/lcapygui/components/
+-rw-rw-r--   0 mph       (1000) mph       (1000)       99 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/__init__.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)       89 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/admittance.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      620 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/annotation.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      169 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/bipole.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      641 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/bjt.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)       88 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/capacitor.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      162 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/cccs.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      162 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/ccvs.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    12801 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/component.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3762 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/connection.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      177 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/controlledcomponent.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      107 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/cpe.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3368 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/cpt_maker.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      331 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/current_source.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      758 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/diode.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      136 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/ferritebead.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)       88 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/impedance.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)       87 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/inductor.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      215 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/jfet.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1610 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/mosfet.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3953 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/opamp.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      188 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/opencircuit.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      132 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/port.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      110 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/resistor.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4522 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/sketch.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3342 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/svgparse.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1401 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/transistor.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      104 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/vccs.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      104 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/vcvs.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      331 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/voltage_source.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      365 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/wire.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1237 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/node.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1842 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/nodes.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-04-11 21:09:29.448365 lcapygui-0.6/lcapygui/scripts/
+-rw-rw-r--   0 mph       (1000) mph       (1000)        0 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/scripts/__init__.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1621 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/scripts/lcapytk.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-04-11 21:09:29.448365 lcapygui-0.6/lcapygui/ui/
+-rw-rw-r--   0 mph       (1000) mph       (1000)        0 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/__init__.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1825 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/preferences.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-04-11 21:09:29.452365 lcapygui-0.6/lcapygui/ui/tk/
+-rw-rw-r--   0 mph       (1000) mph       (1000)        0 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/__init__.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2939 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/cpt_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4648 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/cpt_properties_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1800 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/drawing.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1390 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/equations_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4003 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/expr_advanced_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1798 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/expr_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      187 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/exprimage.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1760 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/help_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1206 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/inspect_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2239 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/labelentries.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      846 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/lateximage.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    19504 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/lcapytk.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     9431 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/lcapytkm.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      251 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/message_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      907 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/node_properties_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      788 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/plot_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2323 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/plot_properties_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4324 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/preferences_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4078 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/sketcher.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    20204 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/uimodelbase.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    15207 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/uimodelmph.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-04-11 21:09:29.448365 lcapygui-0.6/lcapygui.egg-info/
+-rw-rw-r--   0 mph       (1000) mph       (1000)      933 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui.egg-info/PKG-INFO
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2123 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui.egg-info/SOURCES.txt
+-rw-rw-r--   0 mph       (1000) mph       (1000)        1 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui.egg-info/dependency_links.txt
+-rw-rw-r--   0 mph       (1000) mph       (1000)       60 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui.egg-info/entry_points.txt
+-rw-rw-r--   0 mph       (1000) mph       (1000)      150 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui.egg-info/requires.txt
+-rw-rw-r--   0 mph       (1000) mph       (1000)        9 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui.egg-info/top_level.txt
+-rw-rw-r--   0 mph       (1000) mph       (1000)      103 2023-04-11 21:09:29.000000 lcapygui-0.6/pyproject.toml
+-rw-rw-r--   0 mph       (1000) mph       (1000)      287 2023-04-11 21:09:29.452365 lcapygui-0.6/setup.cfg
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1348 2023-04-11 21:09:29.000000 lcapygui-0.6/setup.py
```

### Comparing `lcapygui-0.5/PKG-INFO` & `lcapygui-0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcapygui
-Version: 0.5
+Version: 0.6
 Summary: A GUI for lcapy
 Home-page: https://github.com/mph-/lcapy-gui
 Author: Michael Hayes, Jordan Hay
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mph-/lcapy-gui
 Description: # lcapy-gui
```

### Comparing `lcapygui-0.5/lcapygui/__init__.py` & `lcapygui-0.6/lcapygui/__init__.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.5/lcapygui/components/cpt_maker.py` & `lcapygui-0.6/lcapygui/components/cpt_maker.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,104 +1,137 @@
 from .admittance import Admittance
+from .bjt import BJT
 from .capacitor import Capacitor
+from .connection import Connection
+from .cpe import CPE
 from .current_source import CurrentSource
 from .diode import Diode
-from .ground import Ground
+from .ferritebead import FerriteBead
 from .impedance import Impedance
 from .inductor import Inductor
+from .jfet import JFET
+from .mosfet import MOSFET
 from .opamp import Opamp
+from .opencircuit import OpenCircuit
 from .port import Port
 from .resistor import Resistor
 from .voltage_source import VoltageSource
 from .wire import Wire
 from .vcvs import VCVS
 from .vccs import VCCS
 from .ccvs import CCVS
 from .cccs import CCCS
 
 from .sketch import Sketch
 
+# Could use importlib.import_module to programmatically import
+# the component classes.
+
 
 class CptMaker:
 
     cpts = {
-        'Ground': Ground,
         'C': Capacitor,
+        'CPE': CPE,
         'D': Diode,
         'E': VCVS,
         'Opamp': Opamp,
         'F': CCCS,
+        'FB': FerriteBead,
         'G': VCCS,
         'H': CCVS,
         'I': CurrentSource,
+        'J': JFET,
         'L': Inductor,
+        'M': MOSFET,
+        'O': OpenCircuit,
         'P': Port,
+        'Q': BJT,
         'R': Resistor,
         'NR': Resistor,         # Noise free resistor
         'V': VoltageSource,
         'W': Wire,
+        'X': Connection,
         'Y': Admittance,
         'Z': Impedance
     }
 
     def __init__(self):
 
         self.sketches = {}
 
-    def _make_sketch(self, cpt, create=False):
-
-        if create:
-            sketch = Sketch.create(cpt.sketch_key, cpt.sketch_net)
-
-        sketch = Sketch.load(cpt.sketch_key)
-        if sketch is None:
-            raise FileNotFoundError(
-                'Could not find data file for ' + cpt.sketch_key)
-        return sketch
-
-    def _make_cpt(self, cpt_type, kind='', style=''):
+    def _make_cpt(self, cpt_type, kind='', style='', name=None,
+                  nodes=None, opts=None):
 
-        cls = self.cpts[cpt_type]
-
-        try:
-            cpt = cls(kind=kind, style=style)
-        except TypeError:
-            cpt = cls(None, kind=kind, style=style)
+        if cpt_type == 'W' and kind != '':
+            cls = Connection
+        elif cpt_type == 'E' and kind == 'opamp':
+            cls = Opamp
+        else:
+            cls = self.cpts[cpt_type]
 
+        cpt = cls(kind=kind, style=style,
+                  name=name, nodes=nodes, opts=opts)
         return cpt
 
-    def _add_sketch(self, cpt, create=False):
+    def _add_sketch(self, cpt):
 
         sketch_key = cpt.sketch_key
 
         try:
             sketch = self.sketches[sketch_key]
         except KeyError:
-            sketch = self._make_sketch(cpt, create)
+            sketch = Sketch.load(cpt.sketch_key)
+            if sketch is None:
+                raise FileNotFoundError(
+                    'Could not find data file for ' + cpt.sketch_key)
+            self.sketches[sketch_key] = sketch
 
-        self.sketches[sketch_key] = sketch
-
-        # TODO: remove duck type
+        # TODO: remove duck typing
         cpt.sketch = sketch
 
-    def __call__(self, cpt_type, kind='', style='', create=False):
+    def __call__(self, cpt_type, kind='', style='', name=None,
+                 nodes=None, opts=None, add_sketch=True):
 
-        cpt = self._make_cpt(cpt_type, kind, style)
+        cpt = self._make_cpt(cpt_type, kind, style, name, nodes, opts)
 
-        self._add_sketch(cpt, create)
+        if add_sketch:
+            self._add_sketch(cpt)
 
         return cpt
 
 
 cpt_maker = CptMaker()
 
 
-def cpt_make(cpt_type, kind='', style='', create=False):
-    """Factory to create the path required to draw a component
-    of `cpt_type`."""
+def cpt_make_from_cpt(cpt):
+
+    ctype = cpt.type
 
-    return cpt_maker(cpt_type, kind, style, create)
+    # Convert wire with implicit connection to a connection component.
+    if ctype == 'W':
+        for kind in Connection.kinds:
+            if kind[1:] in cpt.opts:
+                ctype = 'X'
+                break
+
+    return cpt_maker(ctype, kind=cpt._kind, name=cpt.name,
+                     nodes=cpt.nodes, opts=cpt.opts)
+
+
+def cpt_make_from_type(cpt_type, cpt_name='', kind='', style='',
+                       add_sketch=True):
+
+    return cpt_maker(cpt_type, name=cpt_name, kind=kind, style=style,
+                     add_sketch=add_sketch)
 
 
 def cpt_remake(cpt):
 
     return cpt_maker._add_sketch(cpt)
+
+
+def cpt_sketch_make(cpt):
+
+    # Could make method of cpt.
+    sketch = Sketch.create(cpt.sketch_key, cpt.sketch_net)
+    return sketch
```

### Comparing `lcapygui-0.5/lcapygui/components/sketch.py` & `lcapygui-0.6/lcapygui/components/sketch.py`

 * *Files 17% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         sketch_paths = []
         for svga_path in svg.paths:
             sketch_path = SketchPath(
                 svga_path.path, svga_path.style, svga_path.symbol)
             sketch_path = sketch_path.transform(Affine2D(svga_path.transform))
             sketch_paths.append(sketch_path)
 
-        sketch = cls(sketch_paths, svg.width, svg.height).align()
+        sketch = cls(sketch_paths, svg.width, svg.height).align(sketch_key)
         return sketch
 
     @classmethod
     def create(cls, sketch_key, sketch_net):
 
         dirname = join('lcapygui', 'data', 'svg')
         svg_filename = join(dirname, sketch_key + '.svg')
@@ -79,27 +79,45 @@
             net += '; right'
 
         a.add(net)
 
         a.draw(str(svg_filename), label_values=False, label_ids=False,
                label_nodes=False, draw_nodes=False)
 
-    def offsets(self):
+    def offsets1(self, sketch_key):
+
+        if sketch_key == 'opamp':
+            return 0, self.height / 2
+
+        # TODO, use sketch_key to help find offset.
 
         xoffset = None
         yoffset = None
 
         # Look for pair of horizontal wires
+        candidates = []
         for path in self.paths:
-            if len(path.path) == 4 and all(path.path.codes == (1, 2, 1, 2)):
+            if len(path.path) >= 4 and all(path.path.codes[0:4] == (1, 2, 1, 2)):
                 vertices = path.path.vertices
                 if vertices[0][1] == vertices[1][1]:
                     xoffset = vertices[0][0]
                     yoffset = vertices[0][1]
-                    return 0, yoffset
+                    candidates.append((xoffset, yoffset))
+
+        if candidates != []:
+            # Search for horizontal line with longest extent.
+            # This is needed for fet/bjt.
+            xmin = 1000
+            yoffset = 0
+            for candidate in candidates:
+                if candidate[0] < xmin:
+                    xmin = candidate[0]
+                    yoffset = candidate[1]
+
+            return 0, yoffset
 
         # Look for vertical wire (for ground, sground, cground, rground)
         # Note, if look for horizontal wire first, get incorrect offset for rground
         for path in self.paths:
             if len(path.path) == 2 and all(path.path.codes == (1, 2)):
                 vertices = path.path.vertices
                 if vertices[0][0] == vertices[1][0]:
@@ -114,18 +132,23 @@
                 if vertices[0][1] == vertices[1][1]:
                     xoffset = vertices[0][0]
                     yoffset = vertices[0][1]
                     return 0, yoffset
 
         return self.width / 2, self.height / 2
 
-    def align(self):
+    def offsets(self, sketch_key):
+
+        xoffset, yoffset = self.offsets1(sketch_key)
+        return xoffset, yoffset
+
+    def align(self, sketch_key):
         """Remove yoffset from component."""
 
-        xoffset, yoffset = self.offsets()
+        xoffset, yoffset = self.offsets(sketch_key)
 
         if xoffset is None:
             return self
 
         paths = []
         for path in self.paths:
             paths.append(path.transform(
```

### Comparing `lcapygui-0.5/lcapygui/components/svgparse.py` & `lcapygui-0.6/lcapygui/components/svgparse.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.5/lcapygui/node.py` & `lcapygui-0.6/lcapygui/node.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.5/lcapygui/nodes.py` & `lcapygui-0.6/lcapygui/nodes.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.5/lcapygui/scripts/lcapytk.py` & `lcapygui-0.6/lcapygui/scripts/lcapytk.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,23 +36,23 @@
                         version=__doc__.split('\n')[0])
     parser.add_argument('--pdb', action='store_true',
                         default=False,
                         help="enter python debugger on exception")
     parser.add_argument('--debug', type=int,
                         dest='debug', default=None,
                         help="enable debugging")
-    parser.add_argument('filename', type=str, nargs='?',
-                        help='schematic filename', default=None)
+    parser.add_argument('filenames', type=str, nargs='*',
+                        help='schematic filename(s)', default=[])
 
     args = parser.parse_args()
 
     if args.pdb:
         sys.excepthook = schtex_exception
 
-    e = LcapyTk(args.filename, debug=args.debug)
+    e = LcapyTk(args.filenames, debug=args.debug)
     e.display()
 
     return 0
 
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `lcapygui-0.5/lcapygui/ui/preferences.py` & `lcapygui-0.6/lcapygui/ui/preferences.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,16 @@
         self.node_size = 0.1
         self.node_color = 'black'
         self.grid = 'on'
         self.lw = 1.2
         self.show_units = 'false'
         self.xsize = 36
         self.ysize = 22
+        self.snap_grid = 'true'
+        self.voltage_dir = 'RP'
 
         self.load()
 
     @property
     def _dirname(self):
 
         return Path('~/.lcapy/').expanduser()
@@ -51,23 +53,25 @@
         s = json.dumps(self, default=lambda o: o.__dict__,
                        sort_keys=True, indent=4)
 
         self._filename.write_text(s)
 
     def schematic_preferences(self):
 
-        opts = ('draw_nodes', 'label_nodes', 'style')
+        opts = ('draw_nodes', 'label_nodes', 'style', 'voltage_dir')
 
         foo = []
         for opt in opts:
             foo.append(opt + '=' + getattr(self, opt))
         s = ', '.join(foo)
 
         if self.label_cpts == 'name':
             s += ', label_ids=true'
+            s += ', label_values=false'
         elif self.label_cpts == 'value':
+            s += ', label_ids=false'
             s += ', label_values=true'
         elif self.label_cpts == 'value+name':
             s += ', label_ids=true'
             s += ', label_values=true'
 
         return s
```

### Comparing `lcapygui-0.5/lcapygui/ui/tk/cpt_dialog.py` & `lcapygui-0.6/lcapygui/ui/tk/cpt_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.5/lcapygui/ui/tk/cpt_properties_dialog.py` & `lcapygui-0.6/lcapygui/ui/tk/cpt_properties_dialog.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-from ...components.vcvs import VCVS
-from ...components.vccs import VCCS
-from ...components.ccvs import CCVS
-from ...components.cccs import CCCS
 from tkinter import Tk, Button
 from .labelentries import LabelEntry, LabelEntries
 
 
 class CptPropertiesDialog:
 
     def __init__(self, ui, cpt, update=None, title=''):
@@ -31,33 +27,41 @@
                 'style', 'Style', style_name, list(self.gcpt.styles.values()),
                 command=self.on_update))
 
         entries.append(LabelEntry('name', 'Name', self.cpt.name,
                                   command=self.on_update))
 
         for m, arg in enumerate(self.gcpt.args):
+            if arg == 'Control':
+                continue
             entries.append(LabelEntry(arg, arg, self.cpt.args[m],
                                       command=self.on_update))
 
         if cpt.is_capacitor:
-            entries.append(LabelEntry('v0', 'v0', self.cpt.cpt.v0,
+            v0 = str(self.cpt.cpt.v0) if self.cpt.cpt.has_ic else ''
+            entries.append(LabelEntry('v0', 'v0', v0,
                                       command=self.on_update))
         elif cpt.is_inductor:
-            entries.append(LabelEntry('i0', 'i0', self.cpt.cpt.i0,
+            i0 = str(self.cpt.cpt.i0) if self.cpt.cpt.has_ic else ''
+            entries.append(LabelEntry('i0', 'i0', i0,
                                       command=self.on_update))
-        elif isinstance(cpt, (VCVS, VCCS, CCVS, CCCS)):
-            names = [c.name for c in ui.model.components if c.name[0] != 'W']
+        elif cpt.is_dependent_source and self.gcpt.type != 'Eopamp':
+            names = ui.model.possible_control_names()
             entries.append(LabelEntry('control', 'Control',
                                       self.gcpt.control, names,
                                       command=self.on_update))
 
         for k, v in self.gcpt.fields.items():
             entries.append(LabelEntry(k, v, getattr(self.gcpt, k),
                                       command=self.on_update))
 
+        for k, v in self.gcpt.extra_fields.items():
+            entries.append(LabelEntry(k, v, getattr(self.gcpt, k),
+                                      command=self.on_update))
+
         self.labelentries = LabelEntries(self.master, ui, entries)
 
         button = Button(self.master, text="OK", command=self.on_ok)
         button.grid(row=self.labelentries.row)
 
     def on_update(self, arg=None):
 
@@ -74,33 +78,54 @@
         name = self.labelentries.get('name')
         if name.startswith(self.gcpt.name[0]):
             self.gcpt.name = self.labelentries.get('name')
         else:
             self.ui.show_error_dialog('Cannot change component type')
 
         for m, arg in enumerate(self.gcpt.args):
+            if arg == 'Control':
+                continue
             value = self.labelentries.get(arg)
             self.cpt.args[m] = value
 
         try:
             if self.cpt.is_capacitor:
-                self.cpt.cpt.v0 = self.labelentries.get('v0')
+                v0 = self.labelentries.get('v0')
+                self.cpt.args[-1] = v0
+                if v0 == '':
+                    v0 = None
+                else:
+                    v0 = float(v0)
+                cpt = self.cpt.cpt
+                # Create new oneport (this should be improved).
+                self.cpt._cpt = cpt.__class__(cpt.C, v0)
             elif self.cpt.is_inductor:
-                self.cpt.cpt.i0 = self.labelentries.get('i0')
+                i0 = self.labelentries.get('i0')
+                self.cpt.args[-1] = i0
+                if i0 == '':
+                    i0 = None
+                else:
+                    i0 = float(i0)
+                cpt = self.cpt.cpt
+                # Create new oneport (this should be improved).
+                self.cpt._cpt = cpt.__class__(cpt.L, i0)
         except KeyError:
             pass
 
         try:
             self.gcpt.control = self.labelentries.get('control')
         except KeyError:
             pass
 
         for k, v in self.gcpt.fields.items():
             setattr(self.gcpt, k, self.labelentries.get(k))
 
+        for k, v in self.gcpt.extra_fields.items():
+            setattr(self.gcpt, k, self.labelentries.get(k))
+
         if self.update:
             self.update(self.cpt)
 
     def on_ok(self):
 
         self.on_update()
```

### Comparing `lcapygui-0.5/lcapygui/ui/tk/drawing.py` & `lcapygui-0.6/lcapygui/ui/tk/drawing.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.5/lcapygui/ui/tk/equations_dialog.py` & `lcapygui-0.6/lcapygui/ui/tk/equations_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.5/lcapygui/ui/tk/expr_advanced_dialog.py` & `lcapygui-0.6/lcapygui/ui/tk/expr_advanced_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.5/lcapygui/ui/tk/expr_dialog.py` & `lcapygui-0.6/lcapygui/ui/tk/expr_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.5/lcapygui/ui/tk/help_dialog.py` & `lcapygui-0.6/lcapygui/ui/tk/help_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.5/lcapygui/ui/tk/inspect_dialog.py` & `lcapygui-0.6/lcapygui/ui/tk/inspect_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.5/lcapygui/ui/tk/labelentries.py` & `lcapygui-0.6/lcapygui/ui/tk/labelentries.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from tkinter import StringVar, Label, Entry, OptionMenu
+from tkinter.ttk import Checkbutton
 
 
 class LabelEntry:
 
     def __init__(self, name, text, default, options=None, command=None):
 
         self.name = name
@@ -30,19 +31,23 @@
 
             label = Label(master, text=labelentry.text + ': ', anchor='w')
             if isinstance(labelentry.options, (tuple, list)):
                 entry = OptionMenu(
                     master, var, *labelentry.options,
                     command=labelentry.command)
             else:
-                entry = Entry(master, textvariable=var)
-                # if labelentry.command:
-                #    var.trace_add('write', labelentry.command)
-                if labelentry.command:
-                    entry.bind('<Return>', labelentry.command)
+                if isinstance(labelentry.default, bool):
+                    entry = Checkbutton(
+                        master, variable=var, command=labelentry.command)
+                else:
+                    entry = Entry(master, textvariable=var)
+                    # if labelentry.command:
+                    #    var.trace_add('write', labelentry.command)
+                    if labelentry.command:
+                        entry.bind('<Return>', labelentry.command)
 
             label.grid(row=self.row, sticky='w')
             entry.grid(row=self.row, column=1, sticky='w')
 
             self.row += 1
 
     def get_var(self, name):
@@ -63,11 +68,15 @@
     def get(self, name):
 
         val = self.get_text(name)
         if val is None:
             return val
 
         cls = self.get_cls(name)
+
+        if cls is bool:
+            val = {'1': True, '0': False}[val]
+
         try:
             return cls(val)
         except Exception:
             self.ui.show_error_dialog('Invalid value %s for %s' % (val, name))
```

### Comparing `lcapygui-0.5/lcapygui/ui/tk/lateximage.py` & `lcapygui-0.6/lcapygui/ui/tk/lateximage.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.5/lcapygui/ui/tk/lcapytk.py` & `lcapygui-0.6/lcapygui/ui/tk/lcapytk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from tkinter import Canvas, Tk, Menu, Frame, TOP, BOTH, BOTTOM, X
 from tkinter.ttk import Notebook
 from matplotlib.figure import Figure
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
 from matplotlib.backends.backend_tkagg import NavigationToolbar2Tk
 from os.path import basename
 from ..uimodelmph import UIModelMPH
-from .layer import Layer
+from .sketcher import Sketcher
 from .drawing import Drawing
 
 
 class LcapyTk(Tk):
 
     SCALE = 0.01
 
     GEOMETRY = '1200x800'
     # Note, need to reduce height from 8 to 7.2 to fit toolbar.
     FIGSIZE = (12, 7.2)
 
     NAME = 'lcapy-tk'
 
-    def __init__(self, filename=None, uimodel_class=None, debug=0):
+    def __init__(self, filenames=None, uimodel_class=None, debug=0):
 
         from ... import __version__
 
         super().__init__()
         self.debug = debug
         self.version = __version__
         self.model = None
@@ -40,14 +40,16 @@
         # Create the drop down menus
         self.menu = Menu(self, bg='lightgrey', fg='black')
 
         # File menu
         self.file_menu = Menu(self.menu, tearoff=0,
                               bg='lightgrey', fg='black')
 
+        self.file_menu.add_command(label='Clone', command=self.on_clone,
+                                   underline=0)
         self.file_menu.add_command(label='New', command=self.on_new,
                                    underline=0, accelerator='Ctrl+n')
         self.file_menu.add_command(label='Open', command=self.on_load,
                                    underline=0, accelerator='Ctrl+o')
         self.file_menu.add_command(label='Open library', command=self.on_library,
                                    underline=6, accelerator='Ctrl+l')
         self.file_menu.add_command(label='Save', command=self.on_save,
@@ -129,15 +131,15 @@
         # Component menu
         self.component_menu = Menu(self.menu, tearoff=0,
                                    bg='lightgrey', fg='black')
         component_menu = self.component_menu
 
         for key, val in self.uimodel_class.component_map.items():
             acc = key if len(key) == 1 else ''
-            component_menu.add_command(label=val[0],
+            component_menu.add_command(label=val[1],
                                        command=lambda foo=key: self.on_add_cpt(
                                            foo),
                                        accelerator=acc)
             # Callback called twice for some mysterious reason
             # self.component_menu.bind(key,
             #            lambda arg, foo=key: self.on_add_cpt(foo))
 
@@ -147,15 +149,15 @@
         # Connection menu
         self.connection_menu = Menu(self.menu, tearoff=0,
                                     bg='lightgrey', fg='black')
         connection_menu = self.connection_menu
 
         for key, val in self.uimodel_class.connection_map.items():
             acc = key if len(key) == 1 else ''
-            connection_menu.add_command(label=val[0], command=lambda
+            connection_menu.add_command(label=val[1], command=lambda
                                         foo=key: self.on_add_con(foo),
                                         accelerator=acc)
 
         self.menu.add_cascade(label='Connection', underline=0,
                               menu=self.connection_menu)
 
         # Model menu
@@ -186,29 +188,36 @@
         # Notebook tabs
         self.notebook = Notebook(self)
 
         self.canvases = []
 
         self.canvas = None
 
-        self.load(filename)
+        if filenames is None:
+            filenames = []
+
+        for filename in filenames:
+            self.load(filename)
+
+        if filenames == []:
+            model = self.new()
 
     def clear(self, grid='on'):
 
         self.canvas.drawing.clear(grid)
 
     def display(self):
 
         self.mainloop()
 
     def enter(self, canvas):
 
         self.canvas = canvas
         self.model = canvas.model
-        self.layer = canvas.layer
+        self.sketcher = canvas.sketcher
 
         if self.debug:
             print(self.notebook.tab(self.notebook.select(), "text"))
 
     def load(self, filename):
 
         model = self.new()
@@ -246,15 +255,15 @@
         toolbar = NavigationToolbar2Tk(graph, canvas, pack_toolbar=False)
         toolbar.update()
         toolbar.pack(side=BOTTOM, fill=X)
 
         drawing = Drawing(self, fig, model, self.debug)
         canvas.drawing = drawing
         canvas.tab = tab
-        canvas.layer = Layer(canvas.drawing.ax)
+        canvas.sketcher = Sketcher(canvas.drawing.ax, self.debug)
 
         tab.canvas = canvas
 
         self.canvases.append(canvas)
 
         self.notebook.select(len(self.canvases) - 1)
 
@@ -315,14 +324,18 @@
                 self.model.on_right_double_click(event.xdata, event.ydata)
         else:
             if event.button == 1:
                 self.model.on_left_click(event.xdata, event.ydata)
             elif event.button == 3:
                 self.model.on_right_click(event.xdata, event.ydata)
 
+    def on_clone(self):
+
+        self.model.on_clone()
+
     def on_copy(self, *args):
 
         self.model.on_copy()
 
     def on_cut(self, *args):
 
         self.model.on_cut()
```

### Comparing `lcapygui-0.5/lcapygui/ui/tk/lcapytkm.py` & `lcapygui-0.6/lcapygui/ui/tk/lcapytkm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from matplotlib.pyplot import subplots, rcParams, show
 from matplotlib.backend_tools import ToolBase
 from numpy import arange
 from sys import exit
-from .layer import Layer
+from .sketcher import Layer
 
 
 class Tool(ToolBase):
 
     def __init__(self, toolmanager, name, func):
         super(Tool, self).__init__(toolmanager, name)
         self.func = func
@@ -121,20 +121,20 @@
                                                          func=tool[2])
             self.fig.canvas.manager.toolbar.add_tool(tool[0], 'toolgroup')
 
         self.fig.canvas.mpl_connect('close_event', self.on_close)
 
         self.draw_grid()
 
-        layer = Layer(self.ax)
+        sketcher = Layer(self.ax)
 
-        self.cursor_layer = layer
-        self.active_layer = layer
-        self.component_layer = layer
-        self.grid_layer = layer
+        self.cursor_sketcher = sketcher
+        self.active_sketcher = sketcher
+        self.component_sketcher = sketcher
+        self.grid_sketcher = sketcher
 
         self.cid = self.fig.canvas.mpl_connect('button_press_event',
                                                self.on_click_event)
 
         self.kp_cid = self.fig.canvas.mpl_connect('key_press_event',
                                                   self.on_key_press_event)
 
@@ -165,15 +165,15 @@
         self.ax.grid(color='lightblue')
 
         self.ax.tick_params(which='both', left=False, bottom=False,
                             top=False, labelbottom=False)
 
     def clear(self):
 
-        self.component_layer.clear()
+        self.component_sketcher.clear()
         self.draw_grid()
 
     def refresh(self):
 
         self.fig.canvas.draw()
 
     def on_key_press_event(self, event):
```

### Comparing `lcapygui-0.5/lcapygui/ui/tk/node_properties_dialog.py` & `lcapygui-0.6/lcapygui/ui/tk/node_properties_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.5/lcapygui/ui/tk/plot_dialog.py` & `lcapygui-0.6/lcapygui/ui/tk/plot_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.5/lcapygui/ui/tk/plot_properties_dialog.py` & `lcapygui-0.6/lcapygui/ui/tk/plot_properties_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.5/lcapygui/ui/tk/preferences_dialog.py` & `lcapygui-0.6/lcapygui/ui/tk/preferences_dialog.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,14 +24,18 @@
                               self.model.preferences.label_cpts,
                               ('none', 'name',  'value', 'name+value'),
                               command=self.on_update),
                    LabelEntry('style', 'Style',
                               self.model.preferences.style,
                               ('american', 'british', 'european'),
                               command=self.on_update),
+                   LabelEntry('voltage_dir', 'Voltage dir',
+                              self.model.preferences.voltage_dir,
+                              ('RP', 'EF'),
+                              command=self.on_update),
                    LabelEntry('grid', 'Grid',
                               self.model.preferences.grid,
                               ('on', 'off'),
                               command=self.on_update),
                    LabelEntry('lw', 'Line width',
                               self.model.preferences.lw,
                               command=self.on_update),
@@ -43,35 +47,42 @@
                               ('true', 'false'),
                               command=self.on_update),
                    LabelEntry('xsize', 'Width',
                               self.model.preferences.xsize,
                               command=self.on_update),
                    LabelEntry('ysize', 'Height',
                               self.model.preferences.ysize,
-                              command=self.on_update)
+                              command=self.on_update),
+                   LabelEntry('snap_grid', 'Snap to grid',
+                              self.model.preferences.snap_grid,
+                              ('true', 'false'),
+                              command=self.on_update),
                    ]
 
         self.labelentries = LabelEntries(self.master, ui, entries)
 
         button = Button(self.master, text="OK", command=self.on_ok)
         button.grid(row=self.labelentries.row)
 
     def on_update(self, arg=None):
 
         self.model.preferences.label_nodes = self.labelentries.get(
             'label_nodes')
         self.model.preferences.draw_nodes = self.labelentries.get('draw_nodes')
         self.model.preferences.label_cpts = self.labelentries.get('label_cpts')
         self.model.preferences.style = self.labelentries.get('style')
+        self.model.preferences.voltage_dir = self.labelentries.get(
+            'voltage_dir')
         self.model.preferences.grid = self.labelentries.get('grid')
         self.model.preferences.lw = self.labelentries.get('lw')
         self.model.preferences.node_size = self.labelentries.get('node_size')
         self.model.preferences.show_units = self.labelentries.get('show_units')
         self.model.preferences.xsize = self.labelentries.get('xsize')
         self.model.preferences.ysize = self.labelentries.get('ysize')
+        self.model.preferences.snap_grid = self.labelentries.get('snap_grid')
 
         # Do not set show_units; this needs fixing in Lcapy since
         # str(expr) includes the units and this causes problems...
 
         if self.update:
             # Could check for changes
             self.update()
```

### Comparing `lcapygui-0.5/lcapygui/ui/uimodelbase.py` & `lcapygui-0.6/lcapygui/ui/uimodelbase.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,68 @@
 from ..annotation import Annotation
 from ..annotations import Annotations
 from .preferences import Preferences
-from ..components.cpt_maker import cpt_make, cpt_remake
+from ..components.opamp import Opamp
+from ..components.cpt_maker import cpt_make_from_cpt, cpt_make_from_type, cpt_remake
 
 from copy import copy
 from math import atan2, degrees, sqrt
-from lcapy import Circuit
-from lcapy.mnacpts import Cpt, Eopamp
+from lcapy import Circuit, expr
+from lcapy.mnacpts import Cpt
 from lcapy.nodes import parse_nodes
 from lcapy.schemmisc import Pos
+from lcapy.opts import Opts
 
 
 class UIModelBase:
 
     STEP = 2
     SNAP = 1
     SCALE = 0.25
 
+    # Short-cut key, name, type, kind
     component_map = {
-        'c': ('Capacitor', 'C', ''),
-        'd': ('Diode', 'D', ''),
-        'i': ('Current source', 'I', ''),
-        'l': ('Inductor', 'L', ''),
-        'r': ('Resistor', 'R', ''),
-        'nr': ('Noiseless resistor', 'R', ''),
-        'v': ('Voltage source', 'V', ''),
-        'w': ('Wire', 'W', ''),
-        'e': ('VCVS', 'E', ''),
-        'f': ('CCCS', 'F', ''),
-        'g': ('VCCS', 'G', ''),
-        'h': ('CCVS', 'H', ''),
-        'opamp': ('Opamp', 'Opamp', ''),
-        'p': ('Port', 'P', ''),
-        'y': ('Admittance', 'Y', ''),
-        'z': ('Impedance', 'Z', ''),
+        'c': ('c', 'Capacitor', 'C', ''),
+        'd': ('d', 'Diode', 'D', ''),
+        'fb': ('', 'Ferrite bead', 'FB', ''),
+        'i': ('i', 'Current source', 'I', ''),
+        'j': ('j', 'JFET', 'J', ''),
+        'l': ('l', 'Inductor', 'L', ''),
+        'm': ('m', 'MOSFET', 'M', ''),
+        'q': ('q', 'BJT', 'Q', ''),
+        'r': ('r', 'Resistor', 'R', ''),
+        'nr': ('', 'Noiseless resistor', 'R', ''),
+        'v': ('v', 'Voltage source', 'V', ''),
+        'w': ('w', 'Wire', 'W', ''),
+        'e': ('e', 'VCVS', 'E', ''),
+        'f': ('f', 'CCCS', 'F', ''),
+        'g': ('g', 'VCCS', 'G', ''),
+        'h': ('h', 'CCVS', 'H', ''),
+        'o': ('o', 'Open circuit', 'O', ''),
+        'opamp': ('', 'Opamp', 'Opamp', ''),
+        'p': ('p', 'Port', 'P', ''),
+        'y': ('y', 'Admittance', 'Y', ''),
+        'z': ('z', 'Impedance', 'Z', ''),
+        'cpe': ('', 'CPE', 'CPE', ''),
     }
 
     connection_map = {
-        '0': ('0V', 'Ground', ''),
-        '0V': ('0V', 'Ground', '0V'),
-        'ground': ('Ground', 'Ground', ''),
-        'sground': ('Signal ground', 'Ground', 'sground'),
-        'rground': ('Rail ground', 'Ground', 'rground'),
-        'cground': ('Chassis ground', 'Ground', 'cground'),
-        # 'vdd': ('VDD', 'A', 'vdd'),
-        # 'vss': ('VSS', 'A', 'vss'),
-        # 'input': ('Input', 'A', 'input'),
-        # 'output': ('Output', 'A', 'output'),
-        # 'bidir': ('Bidirectional', 'A', 'bidir')
+        '0': ('0', '0V', 'W', ''),
+        '0V': ('', '0V', 'W', '0V'),
+        'ground': ('', 'Ground', 'W', ''),
+        'sground': ('', 'Signal ground', 'W', 'sground'),
+        'rground': ('', 'Rail ground', 'W', 'rground'),
+        'cground': ('', 'Chassis ground', 'W', 'cground'),
+        'vdd': ('', 'VDD', 'W', 'vdd'),
+        'vss': ('', 'VSS', 'W', 'vss'),
+        'vcc': ('', 'VCC', 'W', 'vcc'),
+        'vee': ('', 'VEE', 'W', 'vee'),
+        'input': ('', 'Input', 'W', 'input'),
+        'output': ('', 'Output', 'W', 'output'),
+        'bidir': ('', 'Bidirectional', 'W', 'bidir')
     }
 
     def __init__(self, ui):
 
         self.circuit = Circuit()
         self.ui = ui
         self._analysis_circuit = None
@@ -111,42 +122,36 @@
                 ymin = node.y
             if node.y > ymax:
                 ymax = node.y
         return xmin, ymin, xmax, ymax
 
     def choose_cpt_name(self, cpt_type):
 
+        if cpt_type == 'Opamp':
+            cpt_type = 'E'
+
         num = 1
         while True:
             name = cpt_type + str(num)
             if name not in self.circuit.elements:
                 return name
             num += 1
 
-    def choose_node_name(self, nodes):
-
-        num = 1
-        while True:
-            name = str(num)
-            if name not in nodes:
-                return name
-            num += 1
-
     def con_create(self, con_key, x1, y1, x2, y2):
         """Create a new connection."""
 
         try:
-            cpt_type = self.connection_map[con_key][1]
+            cpt_type = self.connection_map[con_key][2]
         except KeyError:
             return None
 
         if cpt_type == '':
             return None
 
-        return self.thing_create(cpt_type, x1, y1, x2, y2)
+        return self.thing_create(cpt_type, x1, y1, x2, y2, kind='-' + con_key)
 
     def copy(self, cpt):
 
         self.clipboard = cpt
 
     @property
     def cpt_selected(self):
@@ -158,15 +163,15 @@
 
         s = sqrt((x1 - x2)**2 + (y1 - y2)**2)
         if s < 0.2:
             self.exception('Nodes too close to create component')
             return
 
         try:
-            cpt_type = self.component_map[cpt_key][1]
+            cpt_type = self.component_map[cpt_key][2]
         except KeyError:
             return None
 
         if cpt_type == '':
             return None
 
         return self.thing_create(cpt_type, x1, y1, x2, y2)
@@ -191,41 +196,48 @@
 
     def cpt_draw(self, cpt):
 
         gcpt = cpt.gcpt
         if gcpt is None:
             return
 
-        gcpt.draw(self, self.ui.layer)
+        gcpt.draw(self, self.ui.sketcher)
 
         label_cpts = self.preferences.label_cpts
 
         if gcpt.type in ('A', 'O', 'W'):
             label_cpts = 'none'
 
         name = cpt.name
 
         try:
-            value = cpt.args[0]
+            if cpt.type in ('F', 'H'):
+                value = cpt.args[1]
+            elif cpt.type in ('P', ):
+                value = None
+            else:
+                value = cpt.args[0]
         except IndexError:
             value = None
 
         if value is None:
             value = ''
+            value_latex = ''
+        else:
+            value_latex = '$' + expr(value).latex() + '$'
 
+        label = ''
         if label_cpts == 'name+value':
-            if name != value:
-                label = name + '=' + value
+            if name != value and gcpt.has_value:
+                label = name + '=' + value_latex
             else:
                 label = name
         elif label_cpts == 'value':
             if value != '':
-                label = value
-            else:
-                label = name
+                label = value_latex
         elif label_cpts == 'name':
             label = name
         elif label_cpts == 'none':
             label = ''
         else:
             raise RuntimeError('Unhandled label_cpts=' + label_cpts)
 
@@ -233,55 +245,96 @@
             ann = Annotation(self.ui, gcpt.label_position.x,
                              gcpt.label_position.y, label)
             ann.draw(fontsize=18)
             gcpt.annotations.append(ann)
 
         draw_nodes = self.preferences.draw_nodes
         if draw_nodes != 'none':
-            for node in cpt.nodes:
+            for node in gcpt.drawn_nodes:
                 if node.port:
                     self.node_draw(node)
                     continue
 
                 if draw_nodes == 'connections' and node.count < 3:
                     continue
                 if draw_nodes == 'primary' and not node.is_primary:
                     continue
                 self.node_draw(node)
 
         label_nodes = self.preferences.label_nodes
         if label_nodes != 'none':
-            for node in cpt.nodes:
+            for node in gcpt.labelled_nodes:
+                if node.name[0] == '_':
+                    continue
 
                 if label_nodes == 'alpha' and not node.name[0].isalpha():
                     continue
 
                 x, y = node.pos.x, node.pos.y
-                x += 0.3
-                y += 0.3
+                # Should be x -= 0.1 but need to right justify.
+                x += 0.1
+                y += 0.1
                 ann = Annotation(self.ui, x, y, node.name)
                 ann.draw(fontsize=18)
                 gcpt.annotations.append(ann)
 
-    def cpt_find(self, n1, n2):
+    def cpt_find(self, node_name1, node_name2):
 
-        cpt2 = None
+        fcpt = None
         for cpt in self.circuit:
-            if (cpt.nodes[0].name == n1 and cpt.nodes[1].name == n2):
-                cpt2 = cpt
+            if (cpt.nodes[0].name == node_name1 and cpt.nodes[1].name == node_name2):
+                fcpt = cpt
                 break
-        if cpt2 is None:
+        if fcpt is None:
             self.exception(
-                'Cannot find a component with nodes %s and %s' % (n1, n2))
-        return cpt2
+                'Cannot find a component with nodes %s and %s' % (node_name1, node_name2))
+        return fcpt
 
     def cpt_remake(self, cpt):
 
-        newcpt = cpt._change_kind(cpt.gcpt.kind)
-        newcpt.gcpt = cpt.gcpt
+        gcpt = cpt.gcpt
+
+        if cpt.is_dependent_source and gcpt.type != 'Eopamp':
+            try:
+                newcpt = cpt._change_control(gcpt.control)
+            except Exception:
+                self.exception('Control component %s for %s deleted' %
+                               (gcpt.control, cpt.name))
+                return
+        elif gcpt.cpt_kind == cpt._kind:
+            newcpt = cpt
+        elif gcpt.type != 'Eopamp':
+            try:
+                newcpt = cpt._change_kind(gcpt.cpt_kind)
+            except Exception:
+                self.exception('Cannot change kind for %s' % cpt.name)
+                return
+        else:
+            newcpt = cpt
+
+        if gcpt.name != cpt.name:
+            try:
+                newcpt = newcpt._change_name(gcpt.name)
+            except Exception:
+                self.exception('Cannot change name for %s' % cpt.name)
+                return
+
+        if gcpt.mirror ^ ('mirror' in newcpt.opts):
+            # TODO, add mirror method...
+            if gcpt.type == 'Eopamp':
+                newcpt.nodes[2], newcpt.nodes[3] = newcpt.nodes[3], newcpt.nodes[2]
+            elif gcpt.type in ('J', 'M', 'Q'):
+                newcpt.nodes[2], newcpt.nodes[0] = newcpt.nodes[0], newcpt.nodes[2]
+            else:
+                print('Trying to change mirror for ' + str(newcpt))
+
+        newcpt.opts.clear()
+        newcpt.opts.add(gcpt.attr_string_update(self.STEP))
+
+        newcpt.gcpt = gcpt
         cpt_remake(newcpt.gcpt)
 
     def cut(self, cpt):
 
         self.delete(cpt)
         self.clipboard = cpt
 
@@ -314,47 +367,71 @@
         with open(filename) as f:
             line = f.readline()
             if line.startswith(r'\begin{tikz'):
                 self.ui.show_error_dialog('Cannot load Circuitikz macro file')
                 return
 
         try:
-            self.circuit = Circuit(filename)
+            circuit = Circuit(filename)
         except Exception as e:
             self.exception(e)
             return
 
+        return self.load_from_circuit(circuit)
+
+    def load_from_circuit(self, circuit):
+
+        self.circuit = circuit
         positions = None
         for cpt in self.circuit.elements.values():
             if cpt.type == 'XX' and 'nodes' in cpt.opts:
                 positions = parse_nodes(cpt.opts['nodes'])
+                break
 
-        if positions is None:
-            self.exception('Node positions not defined')
-            return
+        if positions is not None:
+            for k, v in self.circuit.nodes.items():
+                v.pos = positions[k]
+
+        else:
+
+            # Node positions not defined.
+
+            sch = self.circuit.sch
+
+            try:
+                # This will fail if have detached components.
+                calculated = sch._positions_calculate()
+            except (AttributeError, ValueError, RuntimeError) as e:
+                self.exception(e)
+                return
+
+            width, height = sch.width * self.STEP, sch.height * self.STEP
 
-        for k, v in self.circuit.nodes.items():
-            v.pos = positions[k]
+            # Centre the schematic.
+            xsize = self.ui.canvas.drawing.xsize
+            ysize = self.ui.canvas.drawing.ysize
+            offsetx, offsety = self.snap((xsize - width) / 2,
+                                         (ysize - height) / 2)
+            for node in sch.nodes.values():
+                node.pos.x += offsetx
+                node.pos.y += offsety
+                # May have split nodes...
+                if node.name in circuit.nodes:
+                    circuit.nodes[node.name].pos = node.pos
 
         self.remove_directives()
 
         for cpt in self.circuit.elements.values():
             if cpt.type == 'XX':
                 cpt.gcpt = None
                 continue
             try:
-                cpt_type = cpt.type
-                if isinstance(cpt, Eopamp):
-                    cpt_type = 'Opamp'
-                gcpt = cpt_make(cpt_type, kind=cpt._kind)
-                # FIXME.
-                gcpt.name = cpt.name
-                gcpt.nodes = cpt.nodes
+                gcpt = cpt_make_from_cpt(cpt)
             except Exception as e:
-                cgpt = None
+                gcpt = None
                 self.exception(e)
 
             cpt.gcpt = gcpt
 
         self.invalidate()
         self.redraw()
 
@@ -365,14 +442,20 @@
     def paste(self, x1, y1, x2, y2):
 
         if self.clipboard is None:
             return
 
         return self.thing_create(self.clipboard.type, x1, y1, x2, y2)
 
+    def possible_control_names(self):
+
+        cpts = self.circuit.elements.values()
+        names = [c.name for c in cpts if c.name[0] != 'W']
+        return names
+
     def remove_directives(self):
 
         elt_list = list(self.circuit.elements.values())
         if elt_list == []:
             return
 
         cpt = elt_list[-1]
@@ -409,57 +492,57 @@
         s = '# Created by ' + self.ui.NAME + ' V' + self.ui.version + '\n'
 
         # Define node positions
         foo = [str(node) for node in self.circuit.nodes.values()]
         s += '; nodes={' + ', '.join(foo) + '}' + '\n'
 
         for cpt in self.circuit.elements.values():
-            s += str(cpt)
-            if cpt.gcpt is not None:
-                s += '; ' + cpt.gcpt.attr_string(self.STEP) + '\n'
+            s += str(cpt) + '\n'
 
         # FIXME, remove other preference string
         # Note, need a newline so string treated as a netlist string
         s += '; ' + self.preferences.schematic_preferences() + '\n'
         return s
 
-    def thing_create(self, cpt_type, x1, y1, x2, y2):
-
-        gcpt = cpt_make(cpt_type)
+    def thing_create(self, cpt_type, x1, y1, x2, y2, kind=''):
 
-        cpt_name = self.choose_cpt_name(gcpt.type)
-        gcpt.name = cpt_name
-        net_parts = [cpt_name]
+        cpt_name = self.choose_cpt_name(cpt_type)
+        gcpt = cpt_make_from_type(cpt_type, cpt_name, kind=kind)
+        if gcpt is None:
+            return
 
-        nodes = list(self.circuit.nodes)
+        all_node_names = list(self.circuit.nodes)
+        node_names = []
         positions = gcpt.assign_positions(x1, y1, x2, y2)
 
         for m, position in enumerate(positions):
             node = self.circuit.nodes.by_position(position)
             if node is None:
-                node_name = self.choose_node_name(nodes)
-                nodes.append(node_name)
+                node_name = gcpt.choose_node_name(m, all_node_names)
+                all_node_names.append(node_name)
             else:
                 node_name = node.name
-            net_parts.append(node_name)
+            node_names.append(node_name)
 
-        net = ' '.join(net_parts)
+        netitem = gcpt.netitem(node_names, x1, y1, x2, y2, self.STEP)
 
         if self.ui.debug:
-            print('Adding ' + net)
+            print('Adding ' + netitem)
 
-        cct = self.circuit.add(net)
+        cct = self.circuit.add(netitem)
         cpt = cct[cpt_name]
 
         for m, position in enumerate(positions):
             cpt.nodes[m].pos = Pos(position)
 
+        attr_string = netitem.split(';', 1)[1]
+        gcpt.update(nodes=cpt.nodes, opts=Opts(attr_string))
+
         # Duck type
         cpt.gcpt = gcpt
-        gcpt.nodes = cpt.nodes
 
         self.cpt_draw(cpt)
 
         self.history.append((cpt, 'A'))
 
         return cpt
 
@@ -539,15 +622,15 @@
         return x, y
 
     def unselect(self):
         pass
 
     def view(self):
 
-        cct = self.circuit
+        cct = Circuit(self.schematic())
         cct.draw()
 
     def voltage_annotate(self, cpt):
 
         ann1 = Annotation(self.ui, *cpt.nodes[0].pos, '+')
         ann2 = Annotation(self.ui, *cpt.nodes[1].pos, '-')
 
@@ -559,20 +642,24 @@
     @property
     def ground_node(self):
 
         return self.node_find('0')
 
     def node_draw(self, node):
 
+        if node.pos is None:
+            print('Pos unknown for ' + str(node))
+            return
+
         if node.port:
-            self.ui.layer.stroke_circle(
+            self.ui.sketcher.stroke_circle(
                 node.x, node.y, self.preferences.node_size,
                 color=self.preferences.node_color, alpha=1)
         else:
-            self.ui.layer.stroke_filled_circle(
+            self.ui.sketcher.stroke_filled_circle(
                 node.x, node.y, self.preferences.node_size,
                 color=self.preferences.node_color, alpha=1)
 
     def node_find(self, nodename):
 
         for node in self.circuit.nodes.values():
             if node.name == nodename:
```

### Comparing `lcapygui-0.5/lcapygui/ui/uimodelmph.py` & `lcapygui-0.6/lcapygui/ui/uimodelmph.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from .uimodelbase import UIModelBase
 from lcapy.mnacpts import Cpt
+from lcapy import Circuit
 
 
 class Cursor:
 
     def __init__(self, ui, x, y):
 
-        self.layer = ui.layer
+        self.sketcher = ui.sketcher
         self.patch = None
         self.x = x
         self.y = y
 
     @property
     def position(self):
 
         return self.x, self.y
 
     def draw(self, color='red', radius=0.3):
 
-        self.patch = self.layer.stroke_filled_circle(self.x, self.y,
-                                                     radius,
-                                                     color=color,
-                                                     alpha=0.5)
+        self.patch = self.sketcher.stroke_filled_circle(self.x, self.y,
+                                                        radius,
+                                                        color=color,
+                                                        alpha=0.5)
 
     def remove(self):
 
         self.patch.remove()
 
 
 class Cursors(list):
@@ -76,34 +77,22 @@
             'ctrl+y': self.on_redo,
             'ctrl+z': self.on_undo,
             'ctrl+9': self.on_pdb,
             'escape': self.on_unselect,
             'delete': self.on_delete,
             'backspace': self.on_delete}
 
-        self.key_bindings_with_key = {
-            '0': self.on_add_con,
-            'c': self.on_add_cpt,
-            'd': self.on_add_cpt,
-            'e': self.on_add_cpt,
-            'f': self.on_add_cpt,
-            'g': self.on_add_cpt,
-            'h': self.on_add_cpt,
-            'i': self.on_add_cpt,
-            'l': self.on_add_cpt,
-            'o': self.on_add_cpt,
-            'p': self.on_add_cpt,
-            'r': self.on_add_cpt,
-            'v': self.on_add_cpt,
-            'w': self.on_add_cpt}
+        self.key_bindings_with_key = {}
+        for k, v in self.component_map.items():
+            self.key_bindings_with_key[k] = self.on_add_cpt
+        for k, v in self.connection_map.items():
+            self.key_bindings_with_key[k] = self.on_add_con
 
     def add_cursor(self, x, y):
 
-        x, y = self.snap(x, y)
-
         cursor = Cursor(self.ui, x, y)
 
         if len(self.cursors) == 0:
             cursor.draw('red')
             self.cursors.append(cursor)
 
         elif len(self.cursors) == 1:
@@ -140,53 +129,53 @@
 
         for cpt in self.circuit.elements.values():
 
             gcpt = cpt.gcpt
             if gcpt is None:
                 continue
 
-            lsq = gcpt.length() ** 2
-            mid = gcpt.midpoint
-            xm, ym = mid.x, mid.y
-            rsq = (xm - x)**2 + (ym - y)**2
-            if rsq < 0.1 * lsq:
+            if gcpt.is_within_bbox(x, y):
                 return cpt
+
         return None
 
     def closest_node(self, x, y):
 
         for node in self.circuit.nodes.values():
             x1, y1 = node.pos.x, node.pos.y
             rsq = (x1 - x)**2 + (y1 - y)**2
             if rsq < 0.1:
                 return node
         return None
 
-    def draw_node_select(self, x, y):
-
-        x, y = self.snap(x, y)
-
-        if self.node_cursor is not None:
-            self.node_cursor.remove()
-
-        cursor = Cursor(self.ui, x, y)
-        cursor.draw('black', 0.2)
-        self.node_cursor = cursor
-        self.ui.refresh()
-
-    def exception(self, message):
+    def exception(self, e):
+        message = str(e)
+        if self.filename != '':
+            message += ' in ' + self.filename
         self.ui.show_error_dialog(message)
+        if self.ui.debug:
+            import pdb
+            pdb.set_trace()
 
     def unselect(self):
 
         self.cursors.remove()
         self.ui.refresh()
 
     def on_add_node(self, x, y):
 
+        # Snap to known node then snap to grid.
+        node = self.closest_node(x, y)
+        if node is None:
+            if self.preferences.snap_grid == 'true':
+                x, y = self.snap(x, y)
+            # Could be smarter and try to align with nearby node.
+        else:
+            x, y = node.x, node.y
+
         self.add_cursor(x, y)
 
     def on_add_cpt(self, cpt_key):
 
         if self.ui.debug:
             print(cpt_key)
 
@@ -237,14 +226,40 @@
         if bbox is None:
             return
         xmin, ymin, xmax, ymax = bbox
 
         self.ui.set_view(xmin - 2, ymin - 2, xmax + 2, ymax + 2)
         self.ui.refresh()
 
+    def on_clone(self):
+
+        def new_name(filename):
+
+            from os.path import splitext
+
+            base, ext = splitext(filename)
+            parts = base.split('_')
+            if len(parts) == 0:
+                suffix = '1'
+            else:
+                try:
+                    suffix = str(int(parts[-1]) + 1)
+                    base = '_'.join(parts[0:-1])
+                except ValueError:
+                    suffix = '1'
+            return base + '_' + suffix + ext
+
+        filename = new_name(self.filename)
+        self.save(filename)
+
+        model = self.ui.new()
+        model.load(filename)
+        self.ui.set_filename(filename)
+        self.ui.refresh()
+
     def on_close(self):
 
         self.ui.quit()
 
     def on_copy(self):
 
         if self.selected is None:
@@ -255,17 +270,20 @@
         self.copy(self.selected)
 
     def on_cpt_changed(self, cpt):
 
         self.invalidate()
         # Component name may have changed
         self.clear()
+
         if isinstance(cpt, Cpt):
+
             # If kind has changed need to remake the sketch
             # and remake the cpt.
+            # If name changed need to remake the cpt.
             self.cpt_remake(cpt)
         else:
             # Node name may have changed...
             pass
 
         self.redraw()
         self.cursors.draw()
@@ -376,16 +394,18 @@
         self.on_select(x, y)
 
         if self.cpt_selected:
             cpt = self.selected
             if self.ui.debug:
                 print('Selected ' + cpt.name)
             self.cursors.remove()
-            self.add_cursor(cpt.nodes[0].pos.x, cpt.nodes[0].pos.y)
-            self.add_cursor(cpt.nodes[1].pos.x, cpt.nodes[1].pos.y)
+            self.add_cursor(cpt.gcpt.node1.pos.x, cpt.gcpt.node1.pos.y)
+            node2 = cpt.gcpt.node2
+            if node2 is not None:
+                self.add_cursor(node2.pos.x, node2.pos.y)
         else:
             if self.ui.debug:
                 print('Add node at (%s, %s)' % (x, y))
             self.on_add_node(x, y)
 
     def on_left_double_click(self, x, y):
 
@@ -446,15 +466,15 @@
 
     def on_new(self):
 
         self.ui.new()
 
     def on_noise_model(self):
 
-        cct = self.analysis_circuit.noise_model()
+        cct = self.circuit.noise_model()
         self.on_show_new_circuit(cct)
 
     def on_paste(self):
 
         if len(self.cursors) < 2:
             # TODO, place cpt where mouse is...
             return
@@ -539,20 +559,17 @@
         if filename == '' or filename == ():
             return
         self.ui.screenshot(filename)
 
     def on_select(self, x, y):
 
         cpt = self.closest_cpt(x, y)
-        node = self.closest_node(x, y)
 
-        if cpt and node:
-            self.ui.show_error_dialog(
-                'Selected both node %s and cpt %s' % (node, cpt))
-            return
+        if cpt is None:
+            node = self.closest_node(x, y)
 
         if cpt:
             self.select(cpt)
         elif node:
             self.select(node)
         else:
             self.select(None)
@@ -577,15 +594,16 @@
 
     def on_view_macros(self):
 
         from lcapy.system import tmpfilename
         from os import remove
 
         schtex_filename = tmpfilename('.schtex')
-        cct = self.circuit
+
+        cct = Circuit(self.schematic())
         cct.draw(schtex_filename)
 
         with open(schtex_filename) as f:
             content = f.read()
         remove(schtex_filename)
 
         self.ui.show_message_dialog(content)
```

### Comparing `lcapygui-0.5/lcapygui.egg-info/PKG-INFO` & `lcapygui-0.6/lcapygui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcapygui
-Version: 0.5
+Version: 0.6
 Summary: A GUI for lcapy
 Home-page: https://github.com/mph-/lcapy-gui
 Author: Michael Hayes, Jordan Hay
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mph-/lcapy-gui
 Description: # lcapy-gui
```

### Comparing `lcapygui-0.5/lcapygui.egg-info/SOURCES.txt` & `lcapygui-0.6/lcapygui.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -11,30 +11,39 @@
 lcapygui.egg-info/SOURCES.txt
 lcapygui.egg-info/dependency_links.txt
 lcapygui.egg-info/entry_points.txt
 lcapygui.egg-info/requires.txt
 lcapygui.egg-info/top_level.txt
 lcapygui/components/__init__.py
 lcapygui/components/admittance.py
+lcapygui/components/annotation.py
+lcapygui/components/bipole.py
+lcapygui/components/bjt.py
 lcapygui/components/capacitor.py
 lcapygui/components/cccs.py
 lcapygui/components/ccvs.py
 lcapygui/components/component.py
 lcapygui/components/connection.py
+lcapygui/components/controlledcomponent.py
+lcapygui/components/cpe.py
 lcapygui/components/cpt_maker.py
 lcapygui/components/current_source.py
 lcapygui/components/diode.py
-lcapygui/components/ground.py
+lcapygui/components/ferritebead.py
 lcapygui/components/impedance.py
 lcapygui/components/inductor.py
+lcapygui/components/jfet.py
+lcapygui/components/mosfet.py
 lcapygui/components/opamp.py
+lcapygui/components/opencircuit.py
 lcapygui/components/port.py
 lcapygui/components/resistor.py
 lcapygui/components/sketch.py
 lcapygui/components/svgparse.py
+lcapygui/components/transistor.py
 lcapygui/components/vccs.py
 lcapygui/components/vcvs.py
 lcapygui/components/voltage_source.py
 lcapygui/components/wire.py
 lcapygui/scripts/__init__.py
 lcapygui/scripts/lcapytk.py
 lcapygui/ui/__init__.py
@@ -49,15 +58,15 @@
 lcapygui/ui/tk/expr_advanced_dialog.py
 lcapygui/ui/tk/expr_dialog.py
 lcapygui/ui/tk/exprimage.py
 lcapygui/ui/tk/help_dialog.py
 lcapygui/ui/tk/inspect_dialog.py
 lcapygui/ui/tk/labelentries.py
 lcapygui/ui/tk/lateximage.py
-lcapygui/ui/tk/layer.py
 lcapygui/ui/tk/lcapytk.py
 lcapygui/ui/tk/lcapytkm.py
 lcapygui/ui/tk/message_dialog.py
 lcapygui/ui/tk/node_properties_dialog.py
 lcapygui/ui/tk/plot_dialog.py
 lcapygui/ui/tk/plot_properties_dialog.py
-lcapygui/ui/tk/preferences_dialog.py
+lcapygui/ui/tk/preferences_dialog.py
+lcapygui/ui/tk/sketcher.py
```

### Comparing `lcapygui-0.5/setup.py` & `lcapygui-0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 setup(
     name='lcapygui',
     packages=find_packages(include=[
         "lcapygui",
         "lcapygui.*"
     ]),
-    version="0.5",
+    version="0.6",
     description="A GUI for lcapy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Michael Hayes, Jordan Hay",
     license="MIT",
     url="https://github.com/mph-/lcapy-gui",
     project_urls={
@@ -27,15 +27,15 @@
     ],
     install_requires=[
         "setuptools",
         "importlib",
         "importlib-metadata",
         "importlib-resources",
         "pathlib",
-        "lcapy>=1.13.1",
+        "lcapy>=1.14",
         "numpy",
         "tk",
         "pillow>=9.4.0",
         "matplotlib",
         "svgpathtools",
         "svgpath2mpl",
         "tkhtmlview"
```

