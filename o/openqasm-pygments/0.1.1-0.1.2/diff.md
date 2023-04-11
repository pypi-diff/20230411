# Comparing `tmp/openqasm-pygments-0.1.1.tar.gz` & `tmp/openqasm-pygments-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openqasm-pygments-0.1.1.tar", last modified: Mon Jun 20 16:19:31 2022, max compression
+gzip compressed data, was "openqasm-pygments-0.1.2.tar", last modified: Tue Apr 11 16:26:52 2023, max compression
```

## Comparing `openqasm-pygments-0.1.1.tar` & `openqasm-pygments-0.1.2.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 16:19:31.769188 openqasm-pygments-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11352 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3033 2022-06-20 16:19:31.769188 openqasm-pygments-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2500 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     2394 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      971 2022-06-20 16:19:31.769188 openqasm-pygments-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 16:19:31.761187 openqasm-pygments-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 16:19:31.761187 openqasm-pygments-0.1.1/src/openqasm_pygments/
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/src/openqasm_pygments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14056 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/src/openqasm_pygments/_lexeme.py
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/src/openqasm_pygments/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4463 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/src/openqasm_pygments/openpulse.py
--rw-r--r--   0 runner    (1001) docker     (121)     3446 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/src/openqasm_pygments/qasm2.py
--rw-r--r--   0 runner    (1001) docker     (121)    14285 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/src/openqasm_pygments/qasm3.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 16:19:31.761187 openqasm-pygments-0.1.1/src/openqasm_pygments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3033 2022-06-20 16:19:31.000000 openqasm-pygments-0.1.1/src/openqasm_pygments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3813 2022-06-20 16:19:31.000000 openqasm-pygments-0.1.1/src/openqasm_pygments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-20 16:19:31.000000 openqasm-pygments-0.1.1/src/openqasm_pygments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-06-20 16:19:31.000000 openqasm-pygments-0.1.1/src/openqasm_pygments.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-06-20 16:19:31.000000 openqasm-pygments-0.1.1/src/openqasm_pygments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-06-20 16:19:31.000000 openqasm-pygments-0.1.1/src/openqasm_pygments.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 16:19:31.761187 openqasm-pygments-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1885 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 16:19:31.761187 openqasm-pygments-0.1.1/tests/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 16:19:31.765187 openqasm-pygments-0.1.1/tests/examples/openpulse/
--rw-r--r--   0 runner    (1001) docker     (121)      716 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/openpulse/capture.openpulse
--rw-r--r--   0 runner    (1001) docker     (121)     5616 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/openpulse/capture.openpulse.output
--rw-r--r--   0 runner    (1001) docker     (121)      855 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/openpulse/frames.openpulse
--rw-r--r--   0 runner    (1001) docker     (121)    10757 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/openpulse/frames.openpulse.output
--rw-r--r--   0 runner    (1001) docker     (121)      612 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/openpulse/geogate.openpulse
--rw-r--r--   0 runner    (1001) docker     (121)     7550 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/openpulse/geogate.openpulse.output
--rw-r--r--   0 runner    (1001) docker     (121)     1967 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/openpulse/neutral_atoms.openpulse
--rw-r--r--   0 runner    (1001) docker     (121)    15866 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/openpulse/neutral_atoms.openpulse.output
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/openpulse/timing.openpulse
--rw-r--r--   0 runner    (1001) docker     (121)     5888 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/openpulse/timing.openpulse.output
--rw-r--r--   0 runner    (1001) docker     (121)      817 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/openpulse/waveforms.openpulse
--rw-r--r--   0 runner    (1001) docker     (121)    11842 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/openpulse/waveforms.openpulse.output
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 16:19:31.765187 openqasm-pygments-0.1.1/tests/examples/qasm2/
--rw-r--r--   0 runner    (1001) docker     (121)      372 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm2/W-state.qasm
--rw-r--r--   0 runner    (1001) docker     (121)     8596 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm2/W-state.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)      713 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm2/adder.qasm
--rw-r--r--   0 runner    (1001) docker     (121)    14565 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm2/adder.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)     1170 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm2/bigadder.qasm
--rw-r--r--   0 runner    (1001) docker     (121)    19651 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm2/bigadder.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)      518 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm2/inverseqft1.qasm
--rw-r--r--   0 runner    (1001) docker     (121)    14242 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm2/inverseqft1.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm2/inverseqft2.qasm
--rw-r--r--   0 runner    (1001) docker     (121)    10527 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm2/inverseqft2.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)      889 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm2/ipea_3_pi_8.qasm
--rw-r--r--   0 runner    (1001) docker     (121)    26438 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm2/ipea_3_pi_8.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)      696 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm2/pea_3_pi_8.qasm
--rw-r--r--   0 runner    (1001) docker     (121)    20536 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm2/pea_3_pi_8.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)      357 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm2/qec.qasm
--rw-r--r--   0 runner    (1001) docker     (121)     7524 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm2/qec.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)     2041 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm2/qelib1.inc
--rw-r--r--   0 runner    (1001) docker     (121)    33157 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm2/qelib1.inc.output
--rw-r--r--   0 runner    (1001) docker     (121)      289 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm2/qft.qasm
--rw-r--r--   0 runner    (1001) docker     (121)     7587 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm2/qft.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm2/qpt.qasm
--rw-r--r--   0 runner    (1001) docker     (121)     3888 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm2/qpt.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm2/rb.qasm
--rw-r--r--   0 runner    (1001) docker     (121)     4785 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm2/rb.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)      372 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm2/teleport.qasm
--rw-r--r--   0 runner    (1001) docker     (121)     7976 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm2/teleport.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm2/teleportv2.qasm
--rw-r--r--   0 runner    (1001) docker     (121)     7933 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm2/teleportv2.qasm.output
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 16:19:31.769188 openqasm-pygments-0.1.1/tests/examples/qasm3/
--rw-r--r--   0 runner    (1001) docker     (121)      815 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/adder.qasm
--rw-r--r--   0 runner    (1001) docker     (121)    16897 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/adder.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/alignment.qasm
--rw-r--r--   0 runner    (1001) docker     (121)     4097 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/alignment.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)     4177 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/arrays.qasm
--rw-r--r--   0 runner    (1001) docker     (121)    25777 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/arrays.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/cphase.qasm
--rw-r--r--   0 runner    (1001) docker     (121)     4186 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/cphase.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/dd.qasm
--rw-r--r--   0 runner    (1001) docker     (121)     7984 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/dd.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)      648 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/defcal.qasm
--rw-r--r--   0 runner    (1001) docker     (121)    11508 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/defcal.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)      505 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/gateteleport.qasm
--rw-r--r--   0 runner    (1001) docker     (121)     6797 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/gateteleport.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)      686 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/inverseqft1.qasm
--rw-r--r--   0 runner    (1001) docker     (121)    20150 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/inverseqft1.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)      443 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/inverseqft2.qasm
--rw-r--r--   0 runner    (1001) docker     (121)    11602 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/inverseqft2.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)      953 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/ipe.qasm
--rw-r--r--   0 runner    (1001) docker     (121)     9064 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/ipe.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)     4668 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/msd.qasm
--rw-r--r--   0 runner    (1001) docker     (121)    61037 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/msd.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)     1353 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/pong.qasm
--rw-r--r--   0 runner    (1001) docker     (121)    17539 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/pong.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)      459 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/qec.qasm
--rw-r--r--   0 runner    (1001) docker     (121)    10163 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/qec.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/qft.qasm
--rw-r--r--   0 runner    (1001) docker     (121)     8590 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/qft.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/qpt.qasm
--rw-r--r--   0 runner    (1001) docker     (121)     3262 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/qpt.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/rb.qasm
--rw-r--r--   0 runner    (1001) docker     (121)     5062 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/rb.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)      841 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/rus.qasm
--rw-r--r--   0 runner    (1001) docker     (121)    10040 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/rus.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)     2834 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/scqec.qasm
--rw-r--r--   0 runner    (1001) docker     (121)    40116 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/scqec.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)     1310 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/t1.qasm
--rw-r--r--   0 runner    (1001) docker     (121)    12788 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/t1.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/teleport.qasm
--rw-r--r--   0 runner    (1001) docker     (121)     7857 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/teleport.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)      719 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/varteleport.qasm
--rw-r--r--   0 runner    (1001) docker     (121)    12384 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/varteleport.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)     2655 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/vqe.qasm
--rw-r--r--   0 runner    (1001) docker     (121)    34793 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/examples/qasm3/vqe.qasm.output
--rw-r--r--   0 runner    (1001) docker     (121)     1834 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (121)     7860 2022-06-20 16:19:14.000000 openqasm-pygments-0.1.1/tests/test_qasm3_lexer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:26:52.952030 openqasm-pygments-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-11 16:26:52.952030 openqasm-pygments-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-11 16:26:52.956030 openqasm-pygments-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:26:52.924030 openqasm-pygments-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:26:52.928030 openqasm-pygments-0.1.2/src/openqasm_pygments/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/src/openqasm_pygments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14056 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/src/openqasm_pygments/_lexeme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/src/openqasm_pygments/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/src/openqasm_pygments/openpulse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/src/openqasm_pygments/qasm2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14285 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/src/openqasm_pygments/qasm3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:26:52.932030 openqasm-pygments-0.1.2/src/openqasm_pygments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-11 16:26:52.000000 openqasm-pygments-0.1.2/src/openqasm_pygments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-04-11 16:26:52.000000 openqasm-pygments-0.1.2/src/openqasm_pygments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 16:26:52.000000 openqasm-pygments-0.1.2/src/openqasm_pygments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-11 16:26:52.000000 openqasm-pygments-0.1.2/src/openqasm_pygments.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-11 16:26:52.000000 openqasm-pygments-0.1.2/src/openqasm_pygments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-11 16:26:52.000000 openqasm-pygments-0.1.2/src/openqasm_pygments.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:26:52.932030 openqasm-pygments-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:26:52.924030 openqasm-pygments-0.1.2/tests/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:26:52.936030 openqasm-pygments-0.1.2/tests/examples/openpulse/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/openpulse/capture.openpulse
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/openpulse/capture.openpulse.output
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/openpulse/frames.openpulse
+-rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/openpulse/frames.openpulse.output
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/openpulse/geogate.openpulse
+-rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/openpulse/geogate.openpulse.output
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/openpulse/neutral_atoms.openpulse
+-rw-r--r--   0 runner    (1001) docker     (123)    15866 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/openpulse/neutral_atoms.openpulse.output
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/openpulse/timing.openpulse
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/openpulse/timing.openpulse.output
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/openpulse/waveforms.openpulse
+-rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/openpulse/waveforms.openpulse.output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:26:52.940030 openqasm-pygments-0.1.2/tests/examples/qasm2/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm2/W-state.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm2/W-state.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm2/adder.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)    14565 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm2/adder.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm2/bigadder.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)    19651 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm2/bigadder.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm2/inverseqft1.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)    14329 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm2/inverseqft1.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm2/inverseqft2.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm2/inverseqft2.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm2/ipea_3_pi_8.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)    26480 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm2/ipea_3_pi_8.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm2/pea_3_pi_8.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)    20599 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm2/pea_3_pi_8.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm2/qec.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm2/qec.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm2/qelib1.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    33283 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm2/qelib1.inc.output
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm2/qft.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm2/qft.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm2/qpt.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm2/qpt.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm2/rb.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm2/rb.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm2/teleport.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)     7964 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm2/teleport.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm2/teleportv2.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm2/teleportv2.qasm.output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:26:52.952030 openqasm-pygments-0.1.2/tests/examples/qasm3/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/adder.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)    16897 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/adder.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/alignment.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/alignment.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/arrays.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)    25777 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/arrays.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/cphase.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/cphase.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/dd.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)     7984 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/dd.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/defcal.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/defcal.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/gateteleport.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/gateteleport.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/inverseqft1.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)    20150 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/inverseqft1.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/inverseqft2.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)    11602 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/inverseqft2.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/ipe.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/ipe.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/msd.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)    61037 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/msd.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/pong.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)    17539 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/pong.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/qec.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)    10163 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/qec.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/qft.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/qft.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/qpt.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/qpt.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/rb.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/rb.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/rus.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/rus.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/scqec.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)    40116 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/scqec.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/t1.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/t1.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/teleport.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/teleport.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/varteleport.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)    12384 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/varteleport.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/vqe.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)    34793 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/examples/qasm3/vqe.qasm.output
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-04-11 16:26:35.000000 openqasm-pygments-0.1.2/tests/test_qasm3_lexer.py
```

### Comparing `openqasm-pygments-0.1.1/LICENSE` & `openqasm-pygments-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/PKG-INFO` & `openqasm-pygments-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openqasm-pygments
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pygments tools for OpenQASM
 Home-page: https://openqasm.github.io/openqasm-pygments
 Author: OpenQASM contributors
 License: Apache 2.0 License
 Project-URL: Bug Tracker, https://github.com/openqasm/openqasm-pygments/issues
 Project-URL: Documentation, https://openqasm.github.com/openqasm-pygments
 Project-URL: Source Code, https://github.com/openqasm/openqasm-pygments
```

### Comparing `openqasm-pygments-0.1.1/README.md` & `openqasm-pygments-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/pyproject.toml` & `openqasm-pygments-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/setup.cfg` & `openqasm-pygments-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = openqasm-pygments
-version = 0.1.1
+version = 0.1.2
 url = https://openqasm.github.io/openqasm-pygments
 description = Pygments tools for OpenQASM
 long_description = file: README.md
 long_description_content_type = text/markdown; variant=GFM
 license = Apache 2.0 License
 license_files = LICENSE
 project_urls =
```

### Comparing `openqasm-pygments-0.1.1/src/openqasm_pygments/_lexeme.py` & `openqasm-pygments-0.1.2/src/openqasm_pygments/_lexeme.py`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/src/openqasm_pygments/openpulse.py` & `openqasm-pygments-0.1.2/src/openqasm_pygments/openpulse.py`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/src/openqasm_pygments/qasm2.py` & `openqasm-pygments-0.1.2/src/openqasm_pygments/qasm2.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,16 +44,16 @@
                 words("sin cos tan exp ln sqrt".split(), prefix="\\b", suffix="\\b"),
                 token.Name.Builtin,
             ),
             (
                 words("reset measure barrier".split(), prefix="\\b", suffix="\\b"),
                 token.Operator.Word,
             ),
-            ("\bif\b", token.Keyword),
-            ("\bpi\b", token.Name.Constant),
+            (r"\bif\b", token.Keyword),
+            (r"\bpi\b", token.Name.Constant),
             (words("[ ] { } ( ) , : ;".split()), token.Punctuation),
             (words("== -> + - * / ^".split()), token.Operator),
             (_INTEGER, token.Number),
             (_REAL, token.Number.Float),
             # Preferentially tokenise identifiers that are used in calling contexts (gates and
             # functions) as callables.  Since we use the same highlighting for gates and functions,
             # it doesn't matter that we'll tokenise (e.g.) the identifier in `rz(...)` with the
```

### Comparing `openqasm-pygments-0.1.1/src/openqasm_pygments/qasm3.py` & `openqasm-pygments-0.1.2/src/openqasm_pygments/qasm3.py`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/src/openqasm_pygments.egg-info/PKG-INFO` & `openqasm-pygments-0.1.2/src/openqasm_pygments.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openqasm-pygments
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pygments tools for OpenQASM
 Home-page: https://openqasm.github.io/openqasm-pygments
 Author: OpenQASM contributors
 License: Apache 2.0 License
 Project-URL: Bug Tracker, https://github.com/openqasm/openqasm-pygments/issues
 Project-URL: Documentation, https://openqasm.github.com/openqasm-pygments
 Project-URL: Source Code, https://github.com/openqasm/openqasm-pygments
```

### Comparing `openqasm-pygments-0.1.1/src/openqasm_pygments.egg-info/SOURCES.txt` & `openqasm-pygments-0.1.2/src/openqasm_pygments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/conftest.py` & `openqasm-pygments-0.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/openpulse/capture.openpulse` & `openqasm-pygments-0.1.2/tests/examples/openpulse/capture.openpulse`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/openpulse/capture.openpulse.output` & `openqasm-pygments-0.1.2/tests/examples/openpulse/capture.openpulse.output`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/openpulse/frames.openpulse` & `openqasm-pygments-0.1.2/tests/examples/openpulse/frames.openpulse`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/openpulse/frames.openpulse.output` & `openqasm-pygments-0.1.2/tests/examples/openpulse/frames.openpulse.output`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/openpulse/geogate.openpulse` & `openqasm-pygments-0.1.2/tests/examples/openpulse/geogate.openpulse`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/openpulse/geogate.openpulse.output` & `openqasm-pygments-0.1.2/tests/examples/openpulse/geogate.openpulse.output`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/openpulse/neutral_atoms.openpulse` & `openqasm-pygments-0.1.2/tests/examples/openpulse/neutral_atoms.openpulse`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/openpulse/neutral_atoms.openpulse.output` & `openqasm-pygments-0.1.2/tests/examples/openpulse/neutral_atoms.openpulse.output`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/openpulse/timing.openpulse` & `openqasm-pygments-0.1.2/tests/examples/openpulse/timing.openpulse`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/openpulse/timing.openpulse.output` & `openqasm-pygments-0.1.2/tests/examples/openpulse/timing.openpulse.output`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/openpulse/waveforms.openpulse` & `openqasm-pygments-0.1.2/tests/examples/openpulse/waveforms.openpulse`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/openpulse/waveforms.openpulse.output` & `openqasm-pygments-0.1.2/tests/examples/openpulse/waveforms.openpulse.output`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm2/W-state.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm2/W-state.qasm.output`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm2/adder.qasm` & `openqasm-pygments-0.1.2/tests/examples/qasm2/adder.qasm`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm2/adder.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm2/adder.qasm.output`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm2/bigadder.qasm` & `openqasm-pygments-0.1.2/tests/examples/qasm2/bigadder.qasm`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm2/bigadder.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm2/bigadder.qasm.output`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm2/inverseqft1.qasm` & `openqasm-pygments-0.1.2/tests/examples/qasm2/inverseqft1.qasm`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm2/inverseqft1.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm2/inverseqft1.qasm.output`

 * *Files 6% similar despite different names*

```diff
@@ -55,24 +55,24 @@
 ' '                 Token.Text.Whitespace
 'c'                 Token.Name
 '['                 Token.Punctuation
 '0'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
+'if'                Token.Keyword
 '('                 Token.Punctuation
 'c'                 Token.Name
 '=='                Token.Operator
 '1'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'u1'                Token.Name.Function
 '('                 Token.Punctuation
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '2'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '1'                 Token.Literal.Number
@@ -98,68 +98,68 @@
 ' '                 Token.Text.Whitespace
 'c'                 Token.Name
 '['                 Token.Punctuation
 '1'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
+'if'                Token.Keyword
 '('                 Token.Punctuation
 'c'                 Token.Name
 '=='                Token.Operator
 '1'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'u1'                Token.Name.Function
 '('                 Token.Punctuation
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '4'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '2'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
+'if'                Token.Keyword
 '('                 Token.Punctuation
 'c'                 Token.Name
 '=='                Token.Operator
 '2'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'u1'                Token.Name.Function
 '('                 Token.Punctuation
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '2'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '2'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
+'if'                Token.Keyword
 '('                 Token.Punctuation
 'c'                 Token.Name
 '=='                Token.Operator
 '3'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'u1'                Token.Name.Function
 '('                 Token.Punctuation
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '2'                 Token.Literal.Number
 '+'                 Token.Operator
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '4'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '2'                 Token.Literal.Number
@@ -185,164 +185,164 @@
 ' '                 Token.Text.Whitespace
 'c'                 Token.Name
 '['                 Token.Punctuation
 '2'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
+'if'                Token.Keyword
 '('                 Token.Punctuation
 'c'                 Token.Name
 '=='                Token.Operator
 '1'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'u1'                Token.Name.Function
 '('                 Token.Punctuation
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '8'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '3'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
+'if'                Token.Keyword
 '('                 Token.Punctuation
 'c'                 Token.Name
 '=='                Token.Operator
 '2'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'u1'                Token.Name.Function
 '('                 Token.Punctuation
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '4'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '3'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
+'if'                Token.Keyword
 '('                 Token.Punctuation
 'c'                 Token.Name
 '=='                Token.Operator
 '3'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'u1'                Token.Name.Function
 '('                 Token.Punctuation
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '4'                 Token.Literal.Number
 '+'                 Token.Operator
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '8'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '3'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
+'if'                Token.Keyword
 '('                 Token.Punctuation
 'c'                 Token.Name
 '=='                Token.Operator
 '4'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'u1'                Token.Name.Function
 '('                 Token.Punctuation
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '2'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '3'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
+'if'                Token.Keyword
 '('                 Token.Punctuation
 'c'                 Token.Name
 '=='                Token.Operator
 '5'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'u1'                Token.Name.Function
 '('                 Token.Punctuation
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '2'                 Token.Literal.Number
 '+'                 Token.Operator
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '8'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '3'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
+'if'                Token.Keyword
 '('                 Token.Punctuation
 'c'                 Token.Name
 '=='                Token.Operator
 '6'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'u1'                Token.Name.Function
 '('                 Token.Punctuation
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '2'                 Token.Literal.Number
 '+'                 Token.Operator
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '4'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '3'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
+'if'                Token.Keyword
 '('                 Token.Punctuation
 'c'                 Token.Name
 '=='                Token.Operator
 '7'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'u1'                Token.Name.Function
 '('                 Token.Punctuation
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '2'                 Token.Literal.Number
 '+'                 Token.Operator
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '4'                 Token.Literal.Number
 '+'                 Token.Operator
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '8'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '3'                 Token.Literal.Number
```

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm2/inverseqft2.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm3/qec.qasm.output`

 * *Files 5% similar despite different names*

```diff
@@ -1,274 +1,263 @@
-'// QFT and measure, version 2' Token.Comment.Single
+'// Repetition code syndrome measurement' Token.Comment.Single
 '\n'                Token.Text.Whitespace
 'OPENQASM'          Token.Comment.Preproc
 ' '                 Token.Text.Whitespace
-'2.0'               Token.Literal
+'3'                 Token.Literal
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
 'include'           Token.Keyword.Namespace
 ' '                 Token.Text.Whitespace
-'"qelib1.inc"'      Token.Literal.String
+'"stdgates.inc"'    Token.Literal.String
 ';'                 Token.Punctuation
-'\n'                Token.Text.Whitespace
-'qreg'              Token.Keyword.Type
+'\n\n'              Token.Text.Whitespace
+'qubit'             Token.Keyword.Type
+'['                 Token.Punctuation
+'3'                 Token.Literal.Number
+']'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
+';'                 Token.Punctuation
+'\n'                Token.Text.Whitespace
+'qubit'             Token.Keyword.Type
 '['                 Token.Punctuation
-'4'                 Token.Literal.Number
+'2'                 Token.Literal.Number
 ']'                 Token.Punctuation
+' '                 Token.Text.Whitespace
+'a'                 Token.Name
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'creg'              Token.Keyword.Type
-' '                 Token.Text.Whitespace
-'c0'                Token.Name
+'bit'               Token.Keyword.Type
 '['                 Token.Punctuation
-'1'                 Token.Literal.Number
+'3'                 Token.Literal.Number
 ']'                 Token.Punctuation
+' '                 Token.Text.Whitespace
+'c'                 Token.Name
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'creg'              Token.Keyword.Type
-' '                 Token.Text.Whitespace
-'c1'                Token.Name
+'bit'               Token.Keyword.Type
 '['                 Token.Punctuation
-'1'                 Token.Literal.Number
+'2'                 Token.Literal.Number
 ']'                 Token.Punctuation
+' '                 Token.Text.Whitespace
+'syn'               Token.Name
 ';'                 Token.Punctuation
-'\n'                Token.Text.Whitespace
-'creg'              Token.Keyword.Type
+'\n\n'              Token.Text.Whitespace
+'def'               Token.Keyword.Declaration
 ' '                 Token.Text.Whitespace
-'c2'                Token.Name
+'syndrome'          Token.Name.Function
+'('                 Token.Punctuation
+'qubit'             Token.Keyword.Type
 '['                 Token.Punctuation
-'1'                 Token.Literal.Number
+'3'                 Token.Literal.Number
 ']'                 Token.Punctuation
-';'                 Token.Punctuation
-'\n'                Token.Text.Whitespace
-'creg'              Token.Keyword.Type
 ' '                 Token.Text.Whitespace
-'c3'                Token.Name
+'d'                 Token.Name
+','                 Token.Punctuation
+' '                 Token.Text.Whitespace
+'qubit'             Token.Keyword.Type
 '['                 Token.Punctuation
-'1'                 Token.Literal.Number
+'2'                 Token.Literal.Number
 ']'                 Token.Punctuation
-';'                 Token.Punctuation
-'\n'                Token.Text.Whitespace
-'h'                 Token.Name.Function
 ' '                 Token.Text.Whitespace
-'q'                 Token.Name
-';'                 Token.Punctuation
-'\n'                Token.Text.Whitespace
-'barrier'           Token.Operator.Word
+'a'                 Token.Name
+')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
-'q'                 Token.Name
-';'                 Token.Punctuation
-'\n'                Token.Text.Whitespace
-'h'                 Token.Name.Function
+'->'                Token.Operator
 ' '                 Token.Text.Whitespace
-'q'                 Token.Name
+'bit'               Token.Keyword.Type
 '['                 Token.Punctuation
-'0'                 Token.Literal.Number
+'2'                 Token.Literal.Number
+']'                 Token.Punctuation
+' '                 Token.Text.Whitespace
+'{'                 Token.Punctuation
+'\n  '              Token.Text.Whitespace
+'bit'               Token.Keyword.Type
+'['                 Token.Punctuation
+'2'                 Token.Literal.Number
 ']'                 Token.Punctuation
+' '                 Token.Text.Whitespace
+'b'                 Token.Name
 ';'                 Token.Punctuation
-'\n'                Token.Text.Whitespace
-'measure'           Token.Operator.Word
+'\n  '              Token.Text.Whitespace
+'cx'                Token.Name.Function
 ' '                 Token.Text.Whitespace
-'q'                 Token.Name
+'d'                 Token.Name
 '['                 Token.Punctuation
 '0'                 Token.Literal.Number
 ']'                 Token.Punctuation
+','                 Token.Punctuation
 ' '                 Token.Text.Whitespace
-'->'                Token.Operator
-' '                 Token.Text.Whitespace
-'c0'                Token.Name
+'a'                 Token.Name
 '['                 Token.Punctuation
 '0'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
-'\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
-'('                 Token.Punctuation
-'c0'                Token.Name
-'=='                Token.Operator
+'\n  '              Token.Text.Whitespace
+'cx'                Token.Name.Function
+' '                 Token.Text.Whitespace
+'d'                 Token.Name
+'['                 Token.Punctuation
 '1'                 Token.Literal.Number
-')'                 Token.Punctuation
+']'                 Token.Punctuation
+','                 Token.Punctuation
 ' '                 Token.Text.Whitespace
-'u1'                Token.Name.Function
-'('                 Token.Punctuation
-'pi'                Token.Name
-'/'                 Token.Operator
-'2'                 Token.Literal.Number
-')'                 Token.Punctuation
+'a'                 Token.Name
+'['                 Token.Punctuation
+'0'                 Token.Literal.Number
+']'                 Token.Punctuation
+';'                 Token.Punctuation
+'\n  '              Token.Text.Whitespace
+'cx'                Token.Name.Function
 ' '                 Token.Text.Whitespace
-'q'                 Token.Name
+'d'                 Token.Name
 '['                 Token.Punctuation
 '1'                 Token.Literal.Number
 ']'                 Token.Punctuation
-';'                 Token.Punctuation
-'\n'                Token.Text.Whitespace
-'h'                 Token.Name.Function
+','                 Token.Punctuation
 ' '                 Token.Text.Whitespace
-'q'                 Token.Name
+'a'                 Token.Name
 '['                 Token.Punctuation
 '1'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
-'\n'                Token.Text.Whitespace
-'measure'           Token.Operator.Word
+'\n  '              Token.Text.Whitespace
+'cx'                Token.Name.Function
 ' '                 Token.Text.Whitespace
-'q'                 Token.Name
+'d'                 Token.Name
+'['                 Token.Punctuation
+'2'                 Token.Literal.Number
+']'                 Token.Punctuation
+','                 Token.Punctuation
+' '                 Token.Text.Whitespace
+'a'                 Token.Name
 '['                 Token.Punctuation
 '1'                 Token.Literal.Number
 ']'                 Token.Punctuation
+';'                 Token.Punctuation
+'\n  '              Token.Text.Whitespace
+'measure'           Token.Operator.Word
+' '                 Token.Text.Whitespace
+'a'                 Token.Name
 ' '                 Token.Text.Whitespace
 '->'                Token.Operator
 ' '                 Token.Text.Whitespace
-'c1'                Token.Name
-'['                 Token.Punctuation
-'0'                 Token.Literal.Number
-']'                 Token.Punctuation
+'b'                 Token.Name
 ';'                 Token.Punctuation
-'\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
-'('                 Token.Punctuation
-'c0'                Token.Name
-'=='                Token.Operator
-'1'                 Token.Literal.Number
-')'                 Token.Punctuation
+'\n  '              Token.Text.Whitespace
+'return'            Token.Keyword
 ' '                 Token.Text.Whitespace
-'u1'                Token.Name.Function
-'('                 Token.Punctuation
-'pi'                Token.Name
-'/'                 Token.Operator
-'4'                 Token.Literal.Number
-')'                 Token.Punctuation
+'b'                 Token.Name
+';'                 Token.Punctuation
+'\n'                Token.Text.Whitespace
+'}'                 Token.Punctuation
+'\n'                Token.Text.Whitespace
+'reset'             Token.Operator.Word
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
-'['                 Token.Punctuation
-'2'                 Token.Literal.Number
-']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
-'('                 Token.Punctuation
-'c1'                Token.Name
-'=='                Token.Operator
-'1'                 Token.Literal.Number
-')'                 Token.Punctuation
+'reset'             Token.Operator.Word
 ' '                 Token.Text.Whitespace
-'u1'                Token.Name.Function
-'('                 Token.Punctuation
-'pi'                Token.Name
-'/'                 Token.Operator
-'2'                 Token.Literal.Number
-')'                 Token.Punctuation
+'a'                 Token.Name
+';'                 Token.Punctuation
+'\n'                Token.Text.Whitespace
+'x'                 Token.Name.Function
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
-'2'                 Token.Literal.Number
+'0'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
+' '                 Token.Text.Whitespace
+'// insert an error' Token.Comment.Single
 '\n'                Token.Text.Whitespace
-'h'                 Token.Name.Function
+'barrier'           Token.Operator.Word
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
-'['                 Token.Punctuation
-'2'                 Token.Literal.Number
-']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'measure'           Token.Operator.Word
+'syn'               Token.Name
 ' '                 Token.Text.Whitespace
-'q'                 Token.Name
-'['                 Token.Punctuation
-'2'                 Token.Literal.Number
-']'                 Token.Punctuation
+'='                 Token.Operator
 ' '                 Token.Text.Whitespace
-'->'                Token.Operator
+'syndrome'          Token.Name.Function
+'('                 Token.Punctuation
+'q'                 Token.Name
+','                 Token.Punctuation
 ' '                 Token.Text.Whitespace
-'c2'                Token.Name
-'['                 Token.Punctuation
-'0'                 Token.Literal.Number
-']'                 Token.Punctuation
+'a'                 Token.Name
+')'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
+'if'                Token.Keyword
+'('                 Token.Punctuation
+'int'               Token.Keyword.Type
+'['                 Token.Punctuation
+'2'                 Token.Literal.Number
+']'                 Token.Punctuation
 '('                 Token.Punctuation
-'c0'                Token.Name
+'syn'               Token.Name
+')'                 Token.Punctuation
 '=='                Token.Operator
 '1'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
-'u1'                Token.Name.Function
-'('                 Token.Punctuation
-'pi'                Token.Name
-'/'                 Token.Operator
-'8'                 Token.Literal.Number
-')'                 Token.Punctuation
+'x'                 Token.Name.Function
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
-'3'                 Token.Literal.Number
+'0'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
+'if'                Token.Keyword
 '('                 Token.Punctuation
-'c1'                Token.Name
+'int'               Token.Keyword.Type
+'['                 Token.Punctuation
+'2'                 Token.Literal.Number
+']'                 Token.Punctuation
+'('                 Token.Punctuation
+'syn'               Token.Name
+')'                 Token.Punctuation
 '=='                Token.Operator
-'1'                 Token.Literal.Number
+'2'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
-'u1'                Token.Name.Function
-'('                 Token.Punctuation
-'pi'                Token.Name
-'/'                 Token.Operator
-'4'                 Token.Literal.Number
-')'                 Token.Punctuation
+'x'                 Token.Name.Function
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
-'3'                 Token.Literal.Number
+'2'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
+'if'                Token.Keyword
+'('                 Token.Punctuation
+'int'               Token.Keyword.Type
+'['                 Token.Punctuation
+'2'                 Token.Literal.Number
+']'                 Token.Punctuation
 '('                 Token.Punctuation
-'c2'                Token.Name
+'syn'               Token.Name
+')'                 Token.Punctuation
 '=='                Token.Operator
-'1'                 Token.Literal.Number
+'3'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
-'u1'                Token.Name.Function
-'('                 Token.Punctuation
-'pi'                Token.Name
-'/'                 Token.Operator
-'2'                 Token.Literal.Number
-')'                 Token.Punctuation
+'x'                 Token.Name.Function
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
-'3'                 Token.Literal.Number
+'1'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'h'                 Token.Name.Function
+'c'                 Token.Name
+' '                 Token.Text.Whitespace
+'='                 Token.Operator
 ' '                 Token.Text.Whitespace
-'q'                 Token.Name
-'['                 Token.Punctuation
-'3'                 Token.Literal.Number
-']'                 Token.Punctuation
-';'                 Token.Punctuation
-'\n'                Token.Text.Whitespace
 'measure'           Token.Operator.Word
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
-'['                 Token.Punctuation
-'3'                 Token.Literal.Number
-']'                 Token.Punctuation
-' '                 Token.Text.Whitespace
-'->'                Token.Operator
-' '                 Token.Text.Whitespace
-'c3'                Token.Name
-'['                 Token.Punctuation
-'0'                 Token.Literal.Number
-']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
```

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm2/ipea_3_pi_8.qasm` & `openqasm-pygments-0.1.2/tests/examples/qasm2/ipea_3_pi_8.qasm`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm2/ipea_3_pi_8.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm2/ipea_3_pi_8.qasm.output`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 '{'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
 'cu1fixed'          Token.Name.Function
 ' '                 Token.Text.Whitespace
 '('                 Token.Punctuation
 '3'                 Token.Literal.Number
 '*'                 Token.Operator
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '8'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'c'                 Token.Name
 ','                 Token.Punctuation
 't'                 Token.Name
@@ -301,25 +301,25 @@
 ','                 Token.Punctuation
 'q'                 Token.Name
 '['                 Token.Punctuation
 '1'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
+'if'                Token.Keyword
 '('                 Token.Punctuation
 'c'                 Token.Name
 '=='                Token.Operator
 '1'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'u1'                Token.Name.Function
 '('                 Token.Punctuation
 '-'                 Token.Operator
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '2'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '0'                 Token.Literal.Number
@@ -387,69 +387,69 @@
 ','                 Token.Punctuation
 'q'                 Token.Name
 '['                 Token.Punctuation
 '1'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
+'if'                Token.Keyword
 '('                 Token.Punctuation
 'c'                 Token.Name
 '=='                Token.Operator
 '1'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'u1'                Token.Name.Function
 '('                 Token.Punctuation
 '-'                 Token.Operator
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '4'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '0'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
+'if'                Token.Keyword
 '('                 Token.Punctuation
 'c'                 Token.Name
 '=='                Token.Operator
 '2'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'u1'                Token.Name.Function
 '('                 Token.Punctuation
 '-'                 Token.Operator
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '2'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '0'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
+'if'                Token.Keyword
 '('                 Token.Punctuation
 'c'                 Token.Name
 '=='                Token.Operator
 '3'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'u1'                Token.Name.Function
 '('                 Token.Punctuation
 '-'                 Token.Operator
 '3'                 Token.Literal.Number
 '*'                 Token.Operator
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '4'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '0'                 Token.Literal.Number
@@ -504,163 +504,163 @@
 ','                 Token.Punctuation
 'q'                 Token.Name
 '['                 Token.Punctuation
 '1'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
+'if'                Token.Keyword
 '('                 Token.Punctuation
 'c'                 Token.Name
 '=='                Token.Operator
 '1'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'u1'                Token.Name.Function
 '('                 Token.Punctuation
 '-'                 Token.Operator
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '8'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '0'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
+'if'                Token.Keyword
 '('                 Token.Punctuation
 'c'                 Token.Name
 '=='                Token.Operator
 '2'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'u1'                Token.Name.Function
 '('                 Token.Punctuation
 '-'                 Token.Operator
 '2'                 Token.Literal.Number
 '*'                 Token.Operator
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '8'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '0'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
+'if'                Token.Keyword
 '('                 Token.Punctuation
 'c'                 Token.Name
 '=='                Token.Operator
 '3'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'u1'                Token.Name.Function
 '('                 Token.Punctuation
 '-'                 Token.Operator
 '3'                 Token.Literal.Number
 '*'                 Token.Operator
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '8'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '0'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
+'if'                Token.Keyword
 '('                 Token.Punctuation
 'c'                 Token.Name
 '=='                Token.Operator
 '4'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'u1'                Token.Name.Function
 '('                 Token.Punctuation
 '-'                 Token.Operator
 '4'                 Token.Literal.Number
 '*'                 Token.Operator
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '8'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '0'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
+'if'                Token.Keyword
 '('                 Token.Punctuation
 'c'                 Token.Name
 '=='                Token.Operator
 '5'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'u1'                Token.Name.Function
 '('                 Token.Punctuation
 '-'                 Token.Operator
 '5'                 Token.Literal.Number
 '*'                 Token.Operator
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '8'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '0'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
+'if'                Token.Keyword
 '('                 Token.Punctuation
 'c'                 Token.Name
 '=='                Token.Operator
 '6'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'u1'                Token.Name.Function
 '('                 Token.Punctuation
 '-'                 Token.Operator
 '6'                 Token.Literal.Number
 '*'                 Token.Operator
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '8'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '0'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
+'if'                Token.Keyword
 '('                 Token.Punctuation
 'c'                 Token.Name
 '=='                Token.Operator
 '7'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'u1'                Token.Name.Function
 '('                 Token.Punctuation
 '-'                 Token.Operator
 '7'                 Token.Literal.Number
 '*'                 Token.Operator
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '8'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '0'                 Token.Literal.Number
```

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm2/pea_3_pi_8.qasm` & `openqasm-pygments-0.1.2/tests/examples/qasm2/pea_3_pi_8.qasm`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm2/pea_3_pi_8.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm2/pea_3_pi_8.qasm.output`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 '{'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
 'cu1fixed'          Token.Name.Function
 ' '                 Token.Text.Whitespace
 '('                 Token.Punctuation
 '3'                 Token.Literal.Number
 '*'                 Token.Operator
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '8'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'c'                 Token.Name
 ','                 Token.Punctuation
 't'                 Token.Name
@@ -336,15 +336,15 @@
 '0'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
 'cu1'               Token.Name.Function
 '('                 Token.Punctuation
 '-'                 Token.Operator
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '2'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '0'                 Token.Literal.Number
@@ -363,15 +363,15 @@
 '1'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
 'cu1'               Token.Name.Function
 '('                 Token.Punctuation
 '-'                 Token.Operator
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '4'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '0'                 Token.Literal.Number
@@ -382,15 +382,15 @@
 '2'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
 'cu1'               Token.Name.Function
 '('                 Token.Punctuation
 '-'                 Token.Operator
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '2'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '1'                 Token.Literal.Number
@@ -409,15 +409,15 @@
 '2'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
 'cu1'               Token.Name.Function
 '('                 Token.Punctuation
 '-'                 Token.Operator
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '8'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '0'                 Token.Literal.Number
@@ -428,15 +428,15 @@
 '3'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
 'cu1'               Token.Name.Function
 '('                 Token.Punctuation
 '-'                 Token.Operator
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '4'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '1'                 Token.Literal.Number
@@ -447,15 +447,15 @@
 '3'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
 'cu1'               Token.Name.Function
 '('                 Token.Punctuation
 '-'                 Token.Operator
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '2'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '2'                 Token.Literal.Number
```

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm2/qec.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm2/qec.qasm.output`

 * *Files 2% similar despite different names*

```diff
@@ -136,45 +136,45 @@
 'a'                 Token.Name
 ' '                 Token.Text.Whitespace
 '->'                Token.Operator
 ' '                 Token.Text.Whitespace
 'syn'               Token.Name
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
+'if'                Token.Keyword
 '('                 Token.Punctuation
 'syn'               Token.Name
 '=='                Token.Operator
 '1'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'x'                 Token.Name.Function
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '0'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
+'if'                Token.Keyword
 '('                 Token.Punctuation
 'syn'               Token.Name
 '=='                Token.Operator
 '2'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'x'                 Token.Name.Function
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '2'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
+'if'                Token.Keyword
 '('                 Token.Punctuation
 'syn'               Token.Name
 '=='                Token.Operator
 '3'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'x'                 Token.Name.Function
```

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm2/qelib1.inc` & `openqasm-pygments-0.1.2/tests/examples/qasm2/qelib1.inc`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm2/qelib1.inc.output` & `openqasm-pygments-0.1.2/tests/examples/qasm2/qelib1.inc.output`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 ' '                 Token.Text.Whitespace
 '{'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'U'                 Token.Name.Builtin
 '('                 Token.Punctuation
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '2'                 Token.Literal.Number
 ','                 Token.Punctuation
 'phi'               Token.Name
 ','                 Token.Punctuation
 'lambda'            Token.Name
 ')'                 Token.Punctuation
@@ -148,19 +148,19 @@
 ' '                 Token.Text.Whitespace
 'a'                 Token.Name
 ' '                 Token.Text.Whitespace
 '{'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'u3'                Token.Name.Function
 '('                 Token.Punctuation
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 ','                 Token.Punctuation
 '0'                 Token.Literal.Number
 ','                 Token.Punctuation
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'a'                 Token.Name
 ';'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 '}'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
@@ -172,21 +172,21 @@
 ' '                 Token.Text.Whitespace
 'a'                 Token.Name
 ' '                 Token.Text.Whitespace
 '{'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'u3'                Token.Name.Function
 '('                 Token.Punctuation
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 ','                 Token.Punctuation
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '2'                 Token.Literal.Number
 ','                 Token.Punctuation
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '2'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'a'                 Token.Name
 ';'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
@@ -200,15 +200,15 @@
 ' '                 Token.Text.Whitespace
 'a'                 Token.Name
 ' '                 Token.Text.Whitespace
 '{'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'u1'                Token.Name.Function
 '('                 Token.Punctuation
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'a'                 Token.Name
 ';'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 '}'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
@@ -222,15 +222,15 @@
 ' '                 Token.Text.Whitespace
 '{'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'u2'                Token.Name.Function
 '('                 Token.Punctuation
 '0'                 Token.Literal.Number
 ','                 Token.Punctuation
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'a'                 Token.Name
 ';'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 '}'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
@@ -242,15 +242,15 @@
 ' '                 Token.Text.Whitespace
 'a'                 Token.Name
 ' '                 Token.Text.Whitespace
 '{'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'u1'                Token.Name.Function
 '('                 Token.Punctuation
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '2'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'a'                 Token.Name
 ';'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
@@ -265,15 +265,15 @@
 'a'                 Token.Name
 ' '                 Token.Text.Whitespace
 '{'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'u1'                Token.Name.Function
 '('                 Token.Punctuation
 '-'                 Token.Operator
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '2'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'a'                 Token.Name
 ';'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
@@ -287,15 +287,15 @@
 ' '                 Token.Text.Whitespace
 'a'                 Token.Name
 ' '                 Token.Text.Whitespace
 '{'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'u1'                Token.Name.Function
 '('                 Token.Punctuation
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '4'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'a'                 Token.Name
 ';'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
@@ -310,15 +310,15 @@
 'a'                 Token.Name
 ' '                 Token.Text.Whitespace
 '{'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'u1'                Token.Name.Function
 '('                 Token.Punctuation
 '-'                 Token.Operator
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '4'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'a'                 Token.Name
 ';'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
@@ -340,19 +340,19 @@
 '{'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'u3'                Token.Name.Function
 '('                 Token.Punctuation
 'theta'             Token.Name
 ','                 Token.Punctuation
 '-'                 Token.Operator
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '2'                 Token.Literal.Number
 ','                 Token.Punctuation
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '2'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'a'                 Token.Name
 ';'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
```

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm2/qft.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm2/qft.qasm.output`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 '['                 Token.Punctuation
 '0'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
 'cu1'               Token.Name.Function
 '('                 Token.Punctuation
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '2'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '1'                 Token.Literal.Number
@@ -79,15 +79,15 @@
 '['                 Token.Punctuation
 '1'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
 'cu1'               Token.Name.Function
 '('                 Token.Punctuation
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '4'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '2'                 Token.Literal.Number
@@ -97,15 +97,15 @@
 '['                 Token.Punctuation
 '0'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
 'cu1'               Token.Name.Function
 '('                 Token.Punctuation
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '2'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '2'                 Token.Literal.Number
@@ -123,15 +123,15 @@
 '['                 Token.Punctuation
 '2'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
 'cu1'               Token.Name.Function
 '('                 Token.Punctuation
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '8'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '3'                 Token.Literal.Number
@@ -141,15 +141,15 @@
 '['                 Token.Punctuation
 '0'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
 'cu1'               Token.Name.Function
 '('                 Token.Punctuation
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '4'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '3'                 Token.Literal.Number
@@ -159,15 +159,15 @@
 '['                 Token.Punctuation
 '1'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
 'cu1'               Token.Name.Function
 '('                 Token.Punctuation
-'pi'                Token.Name
+'pi'                Token.Name.Constant
 '/'                 Token.Operator
 '2'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '3'                 Token.Literal.Number
```

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm2/qpt.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm2/qpt.qasm.output`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm2/rb.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm2/rb.qasm.output`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm2/teleport.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm2/teleport.qasm.output`

 * *Files 2% similar despite different names*

```diff
@@ -145,30 +145,30 @@
 ' '                 Token.Text.Whitespace
 'c1'                Token.Name
 '['                 Token.Punctuation
 '0'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
+'if'                Token.Keyword
 '('                 Token.Punctuation
 'c0'                Token.Name
 '=='                Token.Operator
 '1'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'z'                 Token.Name.Function
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '2'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
+'if'                Token.Keyword
 '('                 Token.Punctuation
 'c1'                Token.Name
 '=='                Token.Operator
 '1'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'x'                 Token.Name.Function
```

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm2/teleportv2.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm2/teleportv2.qasm.output`

 * *Files 3% similar despite different names*

```diff
@@ -129,45 +129,45 @@
 ' '                 Token.Text.Whitespace
 'c'                 Token.Name
 '['                 Token.Punctuation
 '1'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
+'if'                Token.Keyword
 '('                 Token.Punctuation
 'c'                 Token.Name
 '=='                Token.Operator
 '1'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'z'                 Token.Name.Function
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '2'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
+'if'                Token.Keyword
 '('                 Token.Punctuation
 'c'                 Token.Name
 '=='                Token.Operator
 '2'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'x'                 Token.Name.Function
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
 '2'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'if'                Token.Name.Function
+'if'                Token.Keyword
 '('                 Token.Punctuation
 'c'                 Token.Name
 '=='                Token.Operator
 '3'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'y'                 Token.Name.Function
```

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/adder.qasm` & `openqasm-pygments-0.1.2/tests/examples/qasm3/adder.qasm`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/adder.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm3/adder.qasm.output`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/alignment.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm3/alignment.qasm.output`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/arrays.qasm` & `openqasm-pygments-0.1.2/tests/examples/qasm3/arrays.qasm`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/arrays.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm3/arrays.qasm.output`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/cphase.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm3/cphase.qasm.output`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/dd.qasm` & `openqasm-pygments-0.1.2/tests/examples/qasm3/dd.qasm`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/dd.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm3/dd.qasm.output`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/defcal.qasm` & `openqasm-pygments-0.1.2/tests/examples/qasm3/defcal.qasm`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/defcal.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm3/defcal.qasm.output`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/gateteleport.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm3/gateteleport.qasm.output`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/inverseqft1.qasm` & `openqasm-pygments-0.1.2/tests/examples/qasm3/inverseqft1.qasm`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/inverseqft1.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm3/inverseqft1.qasm.output`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/inverseqft2.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm3/inverseqft2.qasm.output`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/ipe.qasm` & `openqasm-pygments-0.1.2/tests/examples/qasm3/ipe.qasm`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/ipe.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm3/ipe.qasm.output`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/msd.qasm` & `openqasm-pygments-0.1.2/tests/examples/qasm3/msd.qasm`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/msd.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm3/msd.qasm.output`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/pong.qasm` & `openqasm-pygments-0.1.2/tests/examples/qasm3/pong.qasm`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/pong.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm3/pong.qasm.output`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/qec.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm2/inverseqft2.qasm.output`

 * *Files 12% similar despite different names*

```diff
@@ -1,263 +1,274 @@
-'// Repetition code syndrome measurement' Token.Comment.Single
+'// QFT and measure, version 2' Token.Comment.Single
 '\n'                Token.Text.Whitespace
 'OPENQASM'          Token.Comment.Preproc
 ' '                 Token.Text.Whitespace
-'3'                 Token.Literal
+'2.0'               Token.Literal
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
 'include'           Token.Keyword.Namespace
 ' '                 Token.Text.Whitespace
-'"stdgates.inc"'    Token.Literal.String
+'"qelib1.inc"'      Token.Literal.String
 ';'                 Token.Punctuation
-'\n\n'              Token.Text.Whitespace
-'qubit'             Token.Keyword.Type
-'['                 Token.Punctuation
-'3'                 Token.Literal.Number
-']'                 Token.Punctuation
+'\n'                Token.Text.Whitespace
+'qreg'              Token.Keyword.Type
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
-';'                 Token.Punctuation
-'\n'                Token.Text.Whitespace
-'qubit'             Token.Keyword.Type
 '['                 Token.Punctuation
-'2'                 Token.Literal.Number
+'4'                 Token.Literal.Number
 ']'                 Token.Punctuation
-' '                 Token.Text.Whitespace
-'a'                 Token.Name
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'bit'               Token.Keyword.Type
-'['                 Token.Punctuation
-'3'                 Token.Literal.Number
-']'                 Token.Punctuation
+'creg'              Token.Keyword.Type
 ' '                 Token.Text.Whitespace
-'c'                 Token.Name
-';'                 Token.Punctuation
-'\n'                Token.Text.Whitespace
-'bit'               Token.Keyword.Type
+'c0'                Token.Name
 '['                 Token.Punctuation
-'2'                 Token.Literal.Number
+'1'                 Token.Literal.Number
 ']'                 Token.Punctuation
-' '                 Token.Text.Whitespace
-'syn'               Token.Name
 ';'                 Token.Punctuation
-'\n\n'              Token.Text.Whitespace
-'def'               Token.Keyword.Declaration
+'\n'                Token.Text.Whitespace
+'creg'              Token.Keyword.Type
 ' '                 Token.Text.Whitespace
-'syndrome'          Token.Name.Function
-'('                 Token.Punctuation
-'qubit'             Token.Keyword.Type
+'c1'                Token.Name
 '['                 Token.Punctuation
-'3'                 Token.Literal.Number
+'1'                 Token.Literal.Number
 ']'                 Token.Punctuation
+';'                 Token.Punctuation
+'\n'                Token.Text.Whitespace
+'creg'              Token.Keyword.Type
 ' '                 Token.Text.Whitespace
-'d'                 Token.Name
-','                 Token.Punctuation
-' '                 Token.Text.Whitespace
-'qubit'             Token.Keyword.Type
+'c2'                Token.Name
 '['                 Token.Punctuation
-'2'                 Token.Literal.Number
+'1'                 Token.Literal.Number
 ']'                 Token.Punctuation
+';'                 Token.Punctuation
+'\n'                Token.Text.Whitespace
+'creg'              Token.Keyword.Type
 ' '                 Token.Text.Whitespace
-'a'                 Token.Name
-')'                 Token.Punctuation
-' '                 Token.Text.Whitespace
-'->'                Token.Operator
-' '                 Token.Text.Whitespace
-'bit'               Token.Keyword.Type
+'c3'                Token.Name
 '['                 Token.Punctuation
-'2'                 Token.Literal.Number
+'1'                 Token.Literal.Number
 ']'                 Token.Punctuation
+';'                 Token.Punctuation
+'\n'                Token.Text.Whitespace
+'h'                 Token.Name.Function
 ' '                 Token.Text.Whitespace
-'{'                 Token.Punctuation
-'\n  '              Token.Text.Whitespace
-'bit'               Token.Keyword.Type
-'['                 Token.Punctuation
-'2'                 Token.Literal.Number
-']'                 Token.Punctuation
+'q'                 Token.Name
+';'                 Token.Punctuation
+'\n'                Token.Text.Whitespace
+'barrier'           Token.Operator.Word
 ' '                 Token.Text.Whitespace
-'b'                 Token.Name
+'q'                 Token.Name
 ';'                 Token.Punctuation
-'\n  '              Token.Text.Whitespace
-'cx'                Token.Name.Function
+'\n'                Token.Text.Whitespace
+'h'                 Token.Name.Function
 ' '                 Token.Text.Whitespace
-'d'                 Token.Name
+'q'                 Token.Name
 '['                 Token.Punctuation
 '0'                 Token.Literal.Number
 ']'                 Token.Punctuation
-','                 Token.Punctuation
+';'                 Token.Punctuation
+'\n'                Token.Text.Whitespace
+'measure'           Token.Operator.Word
 ' '                 Token.Text.Whitespace
-'a'                 Token.Name
+'q'                 Token.Name
 '['                 Token.Punctuation
 '0'                 Token.Literal.Number
 ']'                 Token.Punctuation
-';'                 Token.Punctuation
-'\n  '              Token.Text.Whitespace
-'cx'                Token.Name.Function
 ' '                 Token.Text.Whitespace
-'d'                 Token.Name
-'['                 Token.Punctuation
-'1'                 Token.Literal.Number
-']'                 Token.Punctuation
-','                 Token.Punctuation
+'->'                Token.Operator
 ' '                 Token.Text.Whitespace
-'a'                 Token.Name
+'c0'                Token.Name
 '['                 Token.Punctuation
 '0'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
-'\n  '              Token.Text.Whitespace
-'cx'                Token.Name.Function
-' '                 Token.Text.Whitespace
-'d'                 Token.Name
-'['                 Token.Punctuation
+'\n'                Token.Text.Whitespace
+'if'                Token.Keyword
+'('                 Token.Punctuation
+'c0'                Token.Name
+'=='                Token.Operator
 '1'                 Token.Literal.Number
-']'                 Token.Punctuation
-','                 Token.Punctuation
+')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
-'a'                 Token.Name
+'u1'                Token.Name.Function
+'('                 Token.Punctuation
+'pi'                Token.Name.Constant
+'/'                 Token.Operator
+'2'                 Token.Literal.Number
+')'                 Token.Punctuation
+' '                 Token.Text.Whitespace
+'q'                 Token.Name
 '['                 Token.Punctuation
 '1'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
-'\n  '              Token.Text.Whitespace
-'cx'                Token.Name.Function
-' '                 Token.Text.Whitespace
-'d'                 Token.Name
-'['                 Token.Punctuation
-'2'                 Token.Literal.Number
-']'                 Token.Punctuation
-','                 Token.Punctuation
+'\n'                Token.Text.Whitespace
+'h'                 Token.Name.Function
 ' '                 Token.Text.Whitespace
-'a'                 Token.Name
+'q'                 Token.Name
 '['                 Token.Punctuation
 '1'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
-'\n  '              Token.Text.Whitespace
+'\n'                Token.Text.Whitespace
 'measure'           Token.Operator.Word
 ' '                 Token.Text.Whitespace
-'a'                 Token.Name
+'q'                 Token.Name
+'['                 Token.Punctuation
+'1'                 Token.Literal.Number
+']'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 '->'                Token.Operator
 ' '                 Token.Text.Whitespace
-'b'                 Token.Name
-';'                 Token.Punctuation
-'\n  '              Token.Text.Whitespace
-'return'            Token.Keyword
-' '                 Token.Text.Whitespace
-'b'                 Token.Name
+'c1'                Token.Name
+'['                 Token.Punctuation
+'0'                 Token.Literal.Number
+']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'}'                 Token.Punctuation
-'\n'                Token.Text.Whitespace
-'reset'             Token.Operator.Word
+'if'                Token.Keyword
+'('                 Token.Punctuation
+'c0'                Token.Name
+'=='                Token.Operator
+'1'                 Token.Literal.Number
+')'                 Token.Punctuation
+' '                 Token.Text.Whitespace
+'u1'                Token.Name.Function
+'('                 Token.Punctuation
+'pi'                Token.Name.Constant
+'/'                 Token.Operator
+'4'                 Token.Literal.Number
+')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
+'['                 Token.Punctuation
+'2'                 Token.Literal.Number
+']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'reset'             Token.Operator.Word
+'if'                Token.Keyword
+'('                 Token.Punctuation
+'c1'                Token.Name
+'=='                Token.Operator
+'1'                 Token.Literal.Number
+')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
-'a'                 Token.Name
-';'                 Token.Punctuation
-'\n'                Token.Text.Whitespace
-'x'                 Token.Name.Function
+'u1'                Token.Name.Function
+'('                 Token.Punctuation
+'pi'                Token.Name.Constant
+'/'                 Token.Operator
+'2'                 Token.Literal.Number
+')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
-'0'                 Token.Literal.Number
+'2'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
-' '                 Token.Text.Whitespace
-'// insert an error' Token.Comment.Single
 '\n'                Token.Text.Whitespace
-'barrier'           Token.Operator.Word
+'h'                 Token.Name.Function
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
+'['                 Token.Punctuation
+'2'                 Token.Literal.Number
+']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'syn'               Token.Name
-' '                 Token.Text.Whitespace
-'='                 Token.Operator
+'measure'           Token.Operator.Word
 ' '                 Token.Text.Whitespace
-'syndrome'          Token.Name.Function
-'('                 Token.Punctuation
 'q'                 Token.Name
-','                 Token.Punctuation
+'['                 Token.Punctuation
+'2'                 Token.Literal.Number
+']'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
-'a'                 Token.Name
-')'                 Token.Punctuation
+'->'                Token.Operator
+' '                 Token.Text.Whitespace
+'c2'                Token.Name
+'['                 Token.Punctuation
+'0'                 Token.Literal.Number
+']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
 'if'                Token.Keyword
 '('                 Token.Punctuation
-'int'               Token.Keyword.Type
-'['                 Token.Punctuation
-'2'                 Token.Literal.Number
-']'                 Token.Punctuation
-'('                 Token.Punctuation
-'syn'               Token.Name
-')'                 Token.Punctuation
+'c0'                Token.Name
 '=='                Token.Operator
 '1'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
-'x'                 Token.Name.Function
+'u1'                Token.Name.Function
+'('                 Token.Punctuation
+'pi'                Token.Name.Constant
+'/'                 Token.Operator
+'8'                 Token.Literal.Number
+')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
-'0'                 Token.Literal.Number
+'3'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
 'if'                Token.Keyword
 '('                 Token.Punctuation
-'int'               Token.Keyword.Type
-'['                 Token.Punctuation
-'2'                 Token.Literal.Number
-']'                 Token.Punctuation
-'('                 Token.Punctuation
-'syn'               Token.Name
-')'                 Token.Punctuation
+'c1'                Token.Name
 '=='                Token.Operator
-'2'                 Token.Literal.Number
+'1'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
-'x'                 Token.Name.Function
+'u1'                Token.Name.Function
+'('                 Token.Punctuation
+'pi'                Token.Name.Constant
+'/'                 Token.Operator
+'4'                 Token.Literal.Number
+')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
-'2'                 Token.Literal.Number
+'3'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
 'if'                Token.Keyword
 '('                 Token.Punctuation
-'int'               Token.Keyword.Type
-'['                 Token.Punctuation
-'2'                 Token.Literal.Number
-']'                 Token.Punctuation
-'('                 Token.Punctuation
-'syn'               Token.Name
-')'                 Token.Punctuation
+'c2'                Token.Name
 '=='                Token.Operator
-'3'                 Token.Literal.Number
+'1'                 Token.Literal.Number
 ')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
-'x'                 Token.Name.Function
+'u1'                Token.Name.Function
+'('                 Token.Punctuation
+'pi'                Token.Name.Constant
+'/'                 Token.Operator
+'2'                 Token.Literal.Number
+')'                 Token.Punctuation
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
 '['                 Token.Punctuation
-'1'                 Token.Literal.Number
+'3'                 Token.Literal.Number
 ']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
-'c'                 Token.Name
-' '                 Token.Text.Whitespace
-'='                 Token.Operator
+'h'                 Token.Name.Function
 ' '                 Token.Text.Whitespace
+'q'                 Token.Name
+'['                 Token.Punctuation
+'3'                 Token.Literal.Number
+']'                 Token.Punctuation
+';'                 Token.Punctuation
+'\n'                Token.Text.Whitespace
 'measure'           Token.Operator.Word
 ' '                 Token.Text.Whitespace
 'q'                 Token.Name
+'['                 Token.Punctuation
+'3'                 Token.Literal.Number
+']'                 Token.Punctuation
+' '                 Token.Text.Whitespace
+'->'                Token.Operator
+' '                 Token.Text.Whitespace
+'c3'                Token.Name
+'['                 Token.Punctuation
+'0'                 Token.Literal.Number
+']'                 Token.Punctuation
 ';'                 Token.Punctuation
 '\n'                Token.Text.Whitespace
```

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/qft.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm3/qft.qasm.output`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/qpt.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm3/qpt.qasm.output`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/rb.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm3/rb.qasm.output`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/rus.qasm` & `openqasm-pygments-0.1.2/tests/examples/qasm3/rus.qasm`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/rus.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm3/rus.qasm.output`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/scqec.qasm` & `openqasm-pygments-0.1.2/tests/examples/qasm3/scqec.qasm`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/scqec.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm3/scqec.qasm.output`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/t1.qasm` & `openqasm-pygments-0.1.2/tests/examples/qasm3/t1.qasm`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/t1.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm3/t1.qasm.output`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/teleport.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm3/teleport.qasm.output`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/varteleport.qasm` & `openqasm-pygments-0.1.2/tests/examples/qasm3/varteleport.qasm`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/varteleport.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm3/varteleport.qasm.output`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/vqe.qasm` & `openqasm-pygments-0.1.2/tests/examples/qasm3/vqe.qasm`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/examples/qasm3/vqe.qasm.output` & `openqasm-pygments-0.1.2/tests/examples/qasm3/vqe.qasm.output`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/test_examples.py` & `openqasm-pygments-0.1.2/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `openqasm-pygments-0.1.1/tests/test_qasm3_lexer.py` & `openqasm-pygments-0.1.2/tests/test_qasm3_lexer.py`

 * *Files identical despite different names*

