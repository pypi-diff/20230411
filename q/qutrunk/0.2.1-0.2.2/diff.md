# Comparing `tmp/qutrunk-0.2.1.tar.gz` & `tmp/qutrunk-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qutrunk-0.2.1.tar", max compression
+gzip compressed data, was "qutrunk-0.2.2.tar", max compression
```

## Comparing `qutrunk-0.2.1.tar` & `qutrunk-0.2.2.tar`

### file list

```diff
@@ -1,197 +1,198 @@
--rw-r--r--   0        0        0    11645 2022-09-20 01:34:52.470190 qutrunk-0.2.1/LICENSE
--rw-r--r--   0        0        0     1557 2023-02-09 01:49:01.896005 qutrunk-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       79 2023-02-09 01:49:01.897999 qutrunk-0.2.1/qutrunk/__init__.py
--rw-r--r--   0        0        0        0 2023-01-12 01:38:12.511816 qutrunk-0.2.1/qutrunk/algorithm/__init__.py
--rw-r--r--   0        0        0     5925 2023-01-12 01:38:12.512813 qutrunk-0.2.1/qutrunk/algorithm/vqe.py
--rw-r--r--   0        0        0      401 2023-01-12 06:35:41.099501 qutrunk-0.2.1/qutrunk/backends/__init__.py
--rw-r--r--   0        0        0      609 2022-11-10 02:57:39.182340 qutrunk-0.2.1/qutrunk/backends/backend.py
--rw-r--r--   0        0        0       55 2022-11-10 08:35:57.552046 qutrunk-0.2.1/qutrunk/backends/braket/__init__.py
--rw-r--r--   0        0        0     5205 2023-01-12 01:38:12.515806 qutrunk-0.2.1/qutrunk/backends/braket/adapter.py
--rw-r--r--   0        0        0     5915 2023-01-12 01:38:12.517800 qutrunk-0.2.1/qutrunk/backends/braket/braket.py
--rw-r--r--   0        0        0     1676 2023-01-12 01:38:12.519795 qutrunk-0.2.1/qutrunk/backends/braket/braket_job.py
--rw-r--r--   0        0        0      277 2023-01-12 01:38:12.521790 qutrunk-0.2.1/qutrunk/backends/braket/exception.py
--rw-r--r--   0        0        0       29 2022-09-21 02:59:51.006253 qutrunk-0.2.1/qutrunk/backends/ibm/__init__.py
--rw-r--r--   0        0        0     4829 2023-01-12 01:38:12.522787 qutrunk-0.2.1/qutrunk/backends/ibm/ibm.py
--rw-r--r--   0        0        0    13273 2022-11-10 02:57:39.237192 qutrunk-0.2.1/qutrunk/backends/ibm/ibm_client.py
--rw-r--r--   0        0        0       33 2023-01-12 01:38:12.523784 qutrunk-0.2.1/qutrunk/backends/local/__init__.py
--rw-r--r--   0        0        0      452 2023-01-12 01:38:14.347905 qutrunk-0.2.1/qutrunk/backends/local/exceptions.py
--rw-r--r--   0        0        0     5218 2023-02-09 01:49:01.936928 qutrunk-0.2.1/qutrunk/backends/local/local.py
--rw-r--r--   0        0        0    31544 2023-02-09 01:49:01.938891 qutrunk-0.2.1/qutrunk/backends/local/local_impl.py
--rw-r--r--   0        0        0    62217 2023-02-07 06:25:06.685198 qutrunk-0.2.1/qutrunk/backends/local/sim_distribute.py
--rw-r--r--   0        0        0    48378 2023-02-07 02:35:02.834476 qutrunk-0.2.1/qutrunk/backends/local/sim_gpu.py
--rw-r--r--   0        0        0    52886 2023-02-09 01:49:01.957839 qutrunk-0.2.1/qutrunk/backends/local/sim_local.py
--rw-r--r--   0        0        0       35 2023-01-12 01:38:12.529768 qutrunk-0.2.1/qutrunk/backends/qusaas/__init__.py
--rw-r--r--   0        0        0     8820 2023-02-09 01:49:01.974828 qutrunk-0.2.1/qutrunk/backends/qusaas/httpclient.py
--rw-r--r--   0        0        0     7334 2023-01-12 01:38:12.531762 qutrunk-0.2.1/qutrunk/backends/qusaas/qusaas.py
--rw-r--r--   0        0        0       81 2023-01-12 01:38:12.533767 qutrunk-0.2.1/qutrunk/backends/qusprout/__init__.py
--rw-r--r--   0        0        0     9691 2023-02-09 01:49:01.995738 qutrunk-0.2.1/qutrunk/backends/qusprout/qusprout.py
--rw-r--r--   0        0        0     6268 2023-02-09 01:49:02.007733 qutrunk-0.2.1/qutrunk/backends/qusprout/rpcclient.py
--rw-r--r--   0        0        0     3540 2023-02-09 01:49:02.053583 qutrunk-0.2.1/qutrunk/backends/result.py
--rw-r--r--   0        0        0      275 2023-01-12 01:38:12.538744 qutrunk-0.2.1/qutrunk/circuit/__init__.py
--rw-r--r--   0        0        0     1351 2022-09-19 07:38:17.407904 qutrunk-0.2.1/qutrunk/circuit/bit.py
--rw-r--r--   0        0        0    22544 2023-02-09 01:49:02.079514 qutrunk-0.2.1/qutrunk/circuit/circuit.py
--rw-r--r--   0        0        0     1103 2022-10-26 06:05:52.209786 qutrunk-0.2.1/qutrunk/circuit/classical_bit.py
--rw-r--r--   0        0        0     1713 2023-02-07 02:35:02.835474 qutrunk-0.2.1/qutrunk/circuit/classical_reg.py
--rw-r--r--   0        0        0     5710 2023-02-07 01:12:53.803682 qutrunk-0.2.1/qutrunk/circuit/command.py
--rw-r--r--   0        0        0     1531 2022-11-10 02:57:39.314999 qutrunk-0.2.1/qutrunk/circuit/counter.py
--rw-r--r--   0        0        0     1227 2023-02-07 01:13:16.077272 qutrunk-0.2.1/qutrunk/circuit/gates/__init__.py
--rw-r--r--   0        0        0      804 2023-02-09 01:49:02.099463 qutrunk-0.2.1/qutrunk/circuit/gates/_utils.py
--rw-r--r--   0        0        0     1198 2022-09-09 01:27:43.223147 qutrunk-0.2.1/qutrunk/circuit/gates/barrier.py
--rw-r--r--   0        0        0     3982 2023-02-09 01:49:02.130159 qutrunk-0.2.1/qutrunk/circuit/gates/basicgate.py
--rw-r--r--   0        0        0     2404 2023-01-12 06:35:41.121441 qutrunk-0.2.1/qutrunk/circuit/gates/cr.py
--rw-r--r--   0        0        0     3929 2023-01-12 01:38:12.544729 qutrunk-0.2.1/qutrunk/circuit/gates/h.py
--rw-r--r--   0        0        0     1715 2022-11-10 03:12:25.842346 qutrunk-0.2.1/qutrunk/circuit/gates/i.py
--rw-r--r--   0        0        0     1836 2023-01-12 06:35:41.122439 qutrunk-0.2.1/qutrunk/circuit/gates/iswap.py
--rw-r--r--   0        0        0      927 2022-09-09 01:27:43.246087 qutrunk-0.2.1/qutrunk/circuit/gates/measure.py
--rw-r--r--   0        0        0     7840 2023-01-12 06:35:41.124433 qutrunk-0.2.1/qutrunk/circuit/gates/meta.py
--rw-r--r--   0        0        0     4049 2023-01-12 01:38:12.549715 qutrunk-0.2.1/qutrunk/circuit/gates/p.py
--rw-r--r--   0        0        0     2108 2022-11-10 02:57:39.388788 qutrunk-0.2.1/qutrunk/circuit/gates/r.py
--rw-r--r--   0        0        0     1222 2023-02-07 01:13:16.077272 qutrunk-0.2.1/qutrunk/circuit/gates/reset.py
--rw-r--r--   0        0        0     4469 2023-01-12 01:38:12.551720 qutrunk-0.2.1/qutrunk/circuit/gates/rx.py
--rw-r--r--   0        0        0     2744 2022-11-10 02:57:39.404744 qutrunk-0.2.1/qutrunk/circuit/gates/rxx.py
--rw-r--r--   0        0        0     4244 2023-01-12 01:38:12.553704 qutrunk-0.2.1/qutrunk/circuit/gates/ry.py
--rw-r--r--   0        0        0     2280 2022-11-10 02:57:39.427683 qutrunk-0.2.1/qutrunk/circuit/gates/ryy.py
--rw-r--r--   0        0        0     4237 2023-01-12 01:38:12.555698 qutrunk-0.2.1/qutrunk/circuit/gates/rz.py
--rw-r--r--   0        0        0     2226 2022-11-10 02:57:39.443640 qutrunk-0.2.1/qutrunk/circuit/gates/rzz.py
--rw-r--r--   0        0        0     1492 2023-01-12 01:38:12.556696 qutrunk-0.2.1/qutrunk/circuit/gates/s.py
--rw-r--r--   0        0        0     1505 2023-01-12 01:38:12.558690 qutrunk-0.2.1/qutrunk/circuit/gates/sdg.py
--rw-r--r--   0        0        0     1494 2022-11-10 02:57:39.448628 qutrunk-0.2.1/qutrunk/circuit/gates/sqrtswap.py
--rw-r--r--   0        0        0     3816 2023-01-12 01:38:12.560685 qutrunk-0.2.1/qutrunk/circuit/gates/sqrtx.py
--rw-r--r--   0        0        0     4114 2023-01-12 01:38:12.561683 qutrunk-0.2.1/qutrunk/circuit/gates/swap.py
--rw-r--r--   0        0        0     1530 2022-11-10 03:12:25.849327 qutrunk-0.2.1/qutrunk/circuit/gates/sxdg.py
--rw-r--r--   0        0        0     1513 2023-01-12 01:38:12.563677 qutrunk-0.2.1/qutrunk/circuit/gates/t.py
--rw-r--r--   0        0        0     1504 2023-01-12 01:38:12.565672 qutrunk-0.2.1/qutrunk/circuit/gates/tdg.py
--rw-r--r--   0        0        0     4166 2023-02-07 02:35:02.837469 qutrunk-0.2.1/qutrunk/circuit/gates/u1.py
--rw-r--r--   0        0        0     1997 2023-02-07 02:35:02.839463 qutrunk-0.2.1/qutrunk/circuit/gates/u2.py
--rw-r--r--   0        0        0     7934 2023-02-07 02:35:02.840460 qutrunk-0.2.1/qutrunk/circuit/gates/u3.py
--rw-r--r--   0        0        0     4657 2023-02-09 01:49:02.146120 qutrunk-0.2.1/qutrunk/circuit/gates/x.py
--rw-r--r--   0        0        0     1535 2022-11-10 03:12:25.897059 qutrunk-0.2.1/qutrunk/circuit/gates/x1.py
--rw-r--r--   0        0        0     3775 2023-01-12 01:38:12.568668 qutrunk-0.2.1/qutrunk/circuit/gates/y.py
--rw-r--r--   0        0        0     1528 2022-11-10 03:12:25.900081 qutrunk-0.2.1/qutrunk/circuit/gates/y1.py
--rw-r--r--   0        0        0     4603 2023-01-12 06:35:41.131415 qutrunk-0.2.1/qutrunk/circuit/gates/z.py
--rw-r--r--   0        0        0     1315 2022-11-10 03:12:25.904071 qutrunk-0.2.1/qutrunk/circuit/gates/z1.py
--rw-r--r--   0        0        0      306 2022-11-10 03:12:25.907041 qutrunk-0.2.1/qutrunk/circuit/ops/__init__.py
--rw-r--r--   0        0        0     1564 2023-02-07 01:13:16.124912 qutrunk-0.2.1/qutrunk/circuit/ops/addition.py
--rw-r--r--   0        0        0     2793 2023-01-12 01:38:12.573650 qutrunk-0.2.1/qutrunk/circuit/ops/amp.py
--rw-r--r--   0        0        0     2537 2023-02-07 01:13:16.125910 qutrunk-0.2.1/qutrunk/circuit/ops/classical.py
--rw-r--r--   0        0        0     1186 2023-01-12 01:38:12.577640 qutrunk-0.2.1/qutrunk/circuit/ops/decrement.py
--rw-r--r--   0        0        0     1204 2023-01-12 01:38:12.578637 qutrunk-0.2.1/qutrunk/circuit/ops/increment.py
--rw-r--r--   0        0        0      253 2022-11-10 02:57:39.511459 qutrunk-0.2.1/qutrunk/circuit/ops/operator.py
--rw-r--r--   0        0        0     1189 2022-11-10 03:12:25.915649 qutrunk-0.2.1/qutrunk/circuit/ops/plus.py
--rw-r--r--   0        0        0     2827 2022-11-10 02:57:39.542376 qutrunk-0.2.1/qutrunk/circuit/ops/qaa.py
--rw-r--r--   0        0        0     3335 2023-02-09 01:49:02.185841 qutrunk-0.2.1/qutrunk/circuit/ops/qft.py
--rw-r--r--   0        0        0     2063 2023-02-07 02:35:02.842455 qutrunk-0.2.1/qutrunk/circuit/ops/qpe.py
--rw-r--r--   0        0        0     1696 2023-02-09 01:49:02.205878 qutrunk-0.2.1/qutrunk/circuit/parameter.py
--rw-r--r--   0        0        0      707 2022-10-26 06:05:52.562882 qutrunk-0.2.1/qutrunk/circuit/qubit.py
--rw-r--r--   0        0        0     3493 2023-02-07 02:35:02.843452 qutrunk-0.2.1/qutrunk/circuit/qureg.py
--rw-r--r--   0        0        0      225 2023-01-12 01:38:12.581630 qutrunk-0.2.1/qutrunk/config/__init__.py
--rw-r--r--   0        0        0      402 2023-01-12 06:35:41.145378 qutrunk-0.2.1/qutrunk/config/config.yaml
--rw-r--r--   0        0        0       25 2022-11-10 03:12:25.926908 qutrunk-0.2.1/qutrunk/config/qubox.yaml
--rw-r--r--   0        0        0      142 2022-09-21 02:59:51.026189 qutrunk-0.2.1/qutrunk/converters/__init__.py
--rw-r--r--   0        0        0    14239 2022-09-21 02:59:51.027747 qutrunk-0.2.1/qutrunk/converters/ast_to_dag.py
--rw-r--r--   0        0        0     1158 2022-09-19 07:38:17.429846 qutrunk-0.2.1/qutrunk/converters/circuit_to_dag.py
--rw-r--r--   0        0        0     2129 2022-09-21 02:59:51.029744 qutrunk-0.2.1/qutrunk/converters/dag_to_circuit.py
--rw-r--r--   0        0        0     1556 2022-11-10 02:57:39.577283 qutrunk-0.2.1/qutrunk/converters/mapping.py
--rw-r--r--   0        0        0       36 2022-09-21 02:59:51.032737 qutrunk-0.2.1/qutrunk/dagcircuit/__init__.py
--rw-r--r--   0        0        0     6661 2022-09-19 07:38:17.431843 qutrunk-0.2.1/qutrunk/dagcircuit/dagcircuit.py
--rw-r--r--   0        0        0     1703 2022-09-21 02:59:51.033734 qutrunk-0.2.1/qutrunk/dagcircuit/dagnode.py
--rw-r--r--   0        0        0        0 2022-10-11 02:47:27.766837 qutrunk-0.2.1/qutrunk/example/__init__.py
--rw-r--r--   0        0        0      867 2023-02-08 03:32:41.018865 qutrunk-0.2.1/qutrunk/example/bell_pair.py
--rw-r--r--   0        0        0      132 2022-11-10 02:57:39.581286 qutrunk-0.2.1/qutrunk/example/bell_pair.qasm
--rw-r--r--   0        0        0      185 2022-11-10 02:57:39.583267 qutrunk-0.2.1/qutrunk/example/bell_pair.qusl
--rw-r--r--   0        0        0     1642 2023-02-07 02:35:02.846444 qutrunk-0.2.1/qutrunk/example/bernstein_vazirani.py
--rw-r--r--   0        0        0      818 2023-01-12 01:38:12.585619 qutrunk-0.2.1/qutrunk/example/deutsch.py
--rw-r--r--   0        0        0      881 2023-02-07 02:35:02.848439 qutrunk-0.2.1/qutrunk/example/ghz.py
--rw-r--r--   0        0        0     1611 2023-01-12 06:35:41.151362 qutrunk-0.2.1/qutrunk/example/grover.py
--rw-r--r--   0        0        0     1690 2023-01-12 06:35:41.153356 qutrunk-0.2.1/qutrunk/example/grover_distribute.py
--rw-r--r--   0        0        0     1690 2023-02-09 01:49:21.377087 qutrunk-0.2.1/qutrunk/example/grover_gpu.py
--rw-r--r--   0        0        0   105205 2023-01-12 06:35:41.156348 qutrunk-0.2.1/qutrunk/example/jupyter/algorithm.ipynb
--rw-r--r--   0        0        0     3835 2023-01-12 06:35:41.157345 qutrunk-0.2.1/qutrunk/example/jupyter/awslocal_qrng.ipynb
--rw-r--r--   0        0        0    29003 2023-02-09 01:49:02.232964 qutrunk-0.2.1/qutrunk/example/jupyter/backend.ipynb
--rw-r--r--   0        0        0     8929 2023-01-12 01:38:12.594594 qutrunk-0.2.1/qutrunk/example/jupyter/circuit.ipynb
--rw-r--r--   0        0        0    21163 2023-02-09 01:53:11.697650 qutrunk-0.2.1/qutrunk/example/jupyter/gate.ipynb
--rw-r--r--   0        0        0    10786 2023-02-09 01:49:51.276309 qutrunk-0.2.1/qutrunk/example/jupyter/ops.ipynb
--rw-r--r--   0        0        0    39718 2023-02-09 01:49:02.301056 qutrunk-0.2.1/qutrunk/example/jupyter/qutrunk_mindspore.ipynb
--rw-r--r--   0        0        0    47588 2023-01-12 06:48:19.753276 qutrunk-0.2.1/qutrunk/example/jupyter/qutrunk_paddle.ipynb
--rw-r--r--   0        0        0    61424 2023-02-09 01:49:02.349255 qutrunk-0.2.1/qutrunk/example/jupyter/qutrunk_pytorch.ipynb
--rw-r--r--   0        0        0    35762 2023-02-07 02:35:02.851431 qutrunk-0.2.1/qutrunk/example/jupyter/qutrunk_tensorflow.ipynb
--rw-r--r--   0        0        0      867 2023-02-07 02:35:02.853426 qutrunk-0.2.1/qutrunk/example/phase_estimation.py
--rw-r--r--   0        0        0      714 2023-02-07 01:12:54.042576 qutrunk-0.2.1/qutrunk/example/phase_kickback.py
--rw-r--r--   0        0        0     1240 2023-02-07 02:35:02.855422 qutrunk-0.2.1/qutrunk/example/superdense.py
--rw-r--r--   0        0        0      406 2022-11-10 02:57:39.636125 qutrunk-0.2.1/qutrunk/exceptions.py
--rw-r--r--   0        0        0      355 2022-09-21 02:59:51.052290 qutrunk-0.2.1/qutrunk/qasm/__init__.py
--rw-r--r--   0        0        0      315 2022-09-21 02:59:51.054139 qutrunk-0.2.1/qutrunk/qasm/exceptions.py
--rw-r--r--   0        0        0     5086 2022-05-23 06:54:12.076393 qutrunk-0.2.1/qutrunk/qasm/libs/qelib1.inc
--rw-r--r--   0        0        0      837 2022-11-10 02:57:39.638134 qutrunk-0.2.1/qutrunk/qasm/libs/qulib1.inc
--rw-r--r--   0        0        0     2235 2022-08-23 03:06:14.307069 qutrunk-0.2.1/qutrunk/qasm/libs/stdgates.inc
--rw-r--r--   0        0        0     1356 2022-08-23 02:59:56.717189 qutrunk-0.2.1/qutrunk/qasm/node/__init__.py
--rw-r--r--   0        0        0      957 2022-08-23 02:59:56.718213 qutrunk-0.2.1/qutrunk/qasm/node/barrier.py
--rw-r--r--   0        0        0     2106 2022-09-21 02:59:51.056136 qutrunk-0.2.1/qutrunk/qasm/node/binaryop.py
--rw-r--r--   0        0        0     1500 2022-09-21 02:59:51.058131 qutrunk-0.2.1/qutrunk/qasm/node/binaryoperator.py
--rw-r--r--   0        0        0     1040 2022-08-23 02:59:56.720212 qutrunk-0.2.1/qutrunk/qasm/node/cnot.py
--rw-r--r--   0        0        0     1494 2022-08-23 02:59:56.720212 qutrunk-0.2.1/qutrunk/qasm/node/creg.py
--rw-r--r--   0        0        0     1669 2022-08-23 02:59:56.721178 qutrunk-0.2.1/qutrunk/qasm/node/customunitary.py
--rw-r--r--   0        0        0     1098 2022-09-19 07:38:17.441814 qutrunk-0.2.1/qutrunk/qasm/node/expressionlist.py
--rw-r--r--   0        0        0     2806 2022-09-09 01:27:43.312907 qutrunk-0.2.1/qutrunk/qasm/node/external.py
--rw-r--r--   0        0        0     1285 2022-08-23 02:59:56.723199 qutrunk-0.2.1/qutrunk/qasm/node/format.py
--rw-r--r--   0        0        0     2154 2022-08-23 02:59:56.723199 qutrunk-0.2.1/qutrunk/qasm/node/gate.py
--rw-r--r--   0        0        0     1366 2022-09-19 07:38:17.443808 qutrunk-0.2.1/qutrunk/qasm/node/gatebody.py
--rw-r--r--   0        0        0     2856 2022-08-23 02:59:56.725194 qutrunk-0.2.1/qutrunk/qasm/node/id.py
--rw-r--r--   0        0        0     1053 2022-08-23 02:59:56.726164 qutrunk-0.2.1/qutrunk/qasm/node/idlist.py
--rw-r--r--   0        0        0     1231 2022-08-23 02:59:56.728158 qutrunk-0.2.1/qutrunk/qasm/node/if_.py
--rw-r--r--   0        0        0     1325 2022-08-23 02:59:56.728158 qutrunk-0.2.1/qutrunk/qasm/node/indexedid.py
--rw-r--r--   0        0        0     1575 2022-08-23 02:59:56.729162 qutrunk-0.2.1/qutrunk/qasm/node/intnode.py
--rw-r--r--   0        0        0     1134 2022-09-21 02:59:51.059153 qutrunk-0.2.1/qutrunk/qasm/node/measure.py
--rw-r--r--   0        0        0     2029 2022-08-23 02:59:56.731151 qutrunk-0.2.1/qutrunk/qasm/node/node.py
--rw-r--r--   0        0        0      883 2022-08-23 02:59:56.732149 qutrunk-0.2.1/qutrunk/qasm/node/nodeexception.py
--rw-r--r--   0        0        0     1981 2022-09-19 07:38:17.444806 qutrunk-0.2.1/qutrunk/qasm/node/opaque.py
--rw-r--r--   0        0        0     1822 2022-09-09 01:27:43.313904 qutrunk-0.2.1/qutrunk/qasm/node/prefix.py
--rw-r--r--   0        0        0     1116 2022-09-19 07:38:17.445803 qutrunk-0.2.1/qutrunk/qasm/node/primarylist.py
--rw-r--r--   0        0        0     1013 2022-09-19 07:38:17.446800 qutrunk-0.2.1/qutrunk/qasm/node/program.py
--rw-r--r--   0        0        0     1494 2022-08-23 02:59:56.736138 qutrunk-0.2.1/qutrunk/qasm/node/qreg.py
--rw-r--r--   0        0        0     1949 2022-08-23 03:06:14.309060 qutrunk-0.2.1/qutrunk/qasm/node/real.py
--rw-r--r--   0        0        0      957 2022-09-19 07:38:17.448795 qutrunk-0.2.1/qutrunk/qasm/node/reset.py
--rw-r--r--   0        0        0     1441 2022-09-21 02:59:51.061157 qutrunk-0.2.1/qutrunk/qasm/node/unaryoperator.py
--rw-r--r--   0        0        0     1109 2022-08-23 02:59:56.738151 qutrunk-0.2.1/qutrunk/qasm/node/universalunitary.py
--rw-r--r--   0        0        0     1812 2022-09-21 02:59:51.063155 qutrunk-0.2.1/qutrunk/qasm/qasm.py
--rw-r--r--   0        0        0     5500 2022-09-19 07:38:17.450804 qutrunk-0.2.1/qutrunk/qasm/qasmlexer.py
--rw-r--r--   0        0        0    40599 2022-09-21 02:59:51.064177 qutrunk-0.2.1/qutrunk/qasm/qasmparser.py
--rw-r--r--   0        0        0        0 2023-01-12 01:38:12.727239 qutrunk-0.2.1/qutrunk/thrift/__init__.py
--rw-r--r--   0        0        0       35 2023-01-12 01:38:14.092588 qutrunk-0.2.1/qutrunk/thrift/code/__init__.py
--rw-r--r--   0        0        0      703 2023-01-12 06:35:41.431613 qutrunk-0.2.1/qutrunk/thrift/code/constants.py
--rw-r--r--   0        0        0     4363 2023-01-12 06:35:41.432609 qutrunk-0.2.1/qutrunk/thrift/code/ttypes.py
--rw-r--r--   0        0        0     1433 2023-01-12 01:38:14.083613 qutrunk-0.2.1/qutrunk/thrift/idl/ecode.thrift
--rw-r--r--   0        0        0      645 2023-01-12 06:35:41.434605 qutrunk-0.2.1/qutrunk/thrift/idl/gen_py.sh
--rw-r--r--   0        0        0     1509 2023-02-09 01:49:02.363221 qutrunk-0.2.1/qutrunk/thrift/idl/qusprout.thrift
--rw-r--r--   0        0        0     7120 2023-02-09 01:49:02.365459 qutrunk-0.2.1/qutrunk/thrift/idl/qusproutdata.thrift
--rw-r--r--   0        0        0       53 2023-01-12 01:38:14.066657 qutrunk-0.2.1/qutrunk/thrift/qusprout/__init__.py
--rw-r--r--   0        0        0      411 2023-01-12 06:35:41.451559 qutrunk-0.2.1/qutrunk/thrift/qusprout/constants.py
--rw-r--r--   0        0        0     5649 2023-02-09 01:49:02.367457 qutrunk-0.2.1/qutrunk/thrift/qusprout/QuSproutServer-remote
--rw-r--r--   0        0        0    78824 2023-02-09 01:49:02.386237 qutrunk-0.2.1/qutrunk/thrift/qusprout/QuSproutServer.py
--rw-r--r--   0        0        0      532 2023-01-12 06:35:41.453553 qutrunk-0.2.1/qutrunk/thrift/qusprout/ttypes.py
--rw-r--r--   0        0        0       35 2023-01-12 01:38:14.058680 qutrunk-0.2.1/qutrunk/thrift/qusproutdata/__init__.py
--rw-r--r--   0        0        0      411 2023-01-12 06:35:41.455548 qutrunk-0.2.1/qutrunk/thrift/qusproutdata/constants.py
--rw-r--r--   0        0        0   109466 2023-02-09 01:49:02.390226 qutrunk-0.2.1/qutrunk/thrift/qusproutdata/ttypes.py
--rw-r--r--   0        0        0       74 2022-09-19 07:38:17.480710 qutrunk-0.2.1/qutrunk/tools/__init__.py
--rw-r--r--   0        0        0      621 2022-11-10 02:57:39.830660 qutrunk-0.2.1/qutrunk/tools/algorithm.py
--rw-r--r--   0        0        0      887 2023-01-12 01:38:12.747187 qutrunk-0.2.1/qutrunk/tools/check.py
--rw-r--r--   0        0        0     1046 2023-01-12 01:38:12.748184 qutrunk-0.2.1/qutrunk/tools/check_sprout.py
--rw-r--r--   0        0        0      838 2023-01-12 06:35:41.462529 qutrunk-0.2.1/qutrunk/tools/env_reader.py
--rw-r--r--   0        0        0      374 2022-09-21 02:59:51.137762 qutrunk-0.2.1/qutrunk/tools/function_time.py
--rw-r--r--   0        0        0      502 2023-01-12 01:38:12.751176 qutrunk-0.2.1/qutrunk/tools/get_config.py
--rw-r--r--   0        0        0      221 2022-07-12 02:20:50.337008 qutrunk-0.2.1/qutrunk/tools/ide_parameter.json
--rw-r--r--   0        0        0     2806 2022-11-10 02:57:39.851612 qutrunk-0.2.1/qutrunk/tools/produce_algorithm.py
--rw-r--r--   0        0        0     1829 2023-01-12 06:35:41.465521 qutrunk-0.2.1/qutrunk/tools/qusl_parse.py
--rw-r--r--   0        0        0     3883 2023-02-07 01:13:16.396269 qutrunk-0.2.1/qutrunk/tools/random_circuit.py
--rw-r--r--   0        0        0      412 2022-11-10 03:12:26.048947 qutrunk-0.2.1/qutrunk/tools/read_qubox.py
--rw-r--r--   0        0        0      197 2022-07-12 02:20:50.340977 qutrunk-0.2.1/qutrunk/tools/result.json
--rw-r--r--   0        0        0     1761 2022-09-21 02:59:51.149732 qutrunk-0.2.1/qutrunk/tools/set_config.py
--rw-r--r--   0        0        0      100 2022-09-21 02:59:51.150702 qutrunk-0.2.1/qutrunk/visualizations/__init__.py
--rw-r--r--   0        0        0     1401 2022-09-09 09:24:47.015761 qutrunk-0.2.1/qutrunk/visualizations/circuit_visualization.py
--rw-r--r--   0        0        0    10244 2022-09-13 02:15:54.903738 qutrunk-0.2.1/qutrunk/visualizations/layer.py
--rw-r--r--   0        0        0    30985 2023-02-07 01:13:16.397270 qutrunk-0.2.1/qutrunk/visualizations/text.py
--rw-r--r--   0        0        0    18338 2022-09-21 02:59:51.153706 qutrunk-0.2.1/qutrunk/visualizations/text_draw_element.py
--rw-r--r--   0        0        0      750 2022-09-19 07:38:17.494671 qutrunk-0.2.1/qutrunk/visualizations/utils.py
--rw-r--r--   0        0        0     6085 2023-02-09 01:49:21.376089 qutrunk-0.2.1/README.md
--rw-r--r--   0        0        0     7695 2023-02-09 01:56:48.717311 qutrunk-0.2.1/setup.py
--rw-r--r--   0        0        0     7411 2023-02-09 01:56:48.717311 qutrunk-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11645 2022-09-20 01:34:52.470190 qutrunk-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1557 2023-04-11 07:06:37.378449 qutrunk-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       79 2023-04-11 07:06:25.858202 qutrunk-0.2.2/qutrunk/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-12 01:38:12.511816 qutrunk-0.2.2/qutrunk/algorithm/__init__.py
+-rw-r--r--   0        0        0     5925 2023-01-12 01:38:12.512813 qutrunk-0.2.2/qutrunk/algorithm/vqe.py
+-rw-r--r--   0        0        0      401 2023-01-12 06:35:41.099501 qutrunk-0.2.2/qutrunk/backends/__init__.py
+-rw-r--r--   0        0        0      609 2022-11-10 02:57:39.182340 qutrunk-0.2.2/qutrunk/backends/backend.py
+-rw-r--r--   0        0        0       55 2022-11-10 08:35:57.552046 qutrunk-0.2.2/qutrunk/backends/braket/__init__.py
+-rw-r--r--   0        0        0     5205 2023-01-12 01:38:12.515806 qutrunk-0.2.2/qutrunk/backends/braket/adapter.py
+-rw-r--r--   0        0        0     6241 2023-04-11 07:05:32.974725 qutrunk-0.2.2/qutrunk/backends/braket/braket.py
+-rw-r--r--   0        0        0     1676 2023-01-12 01:38:12.519795 qutrunk-0.2.2/qutrunk/backends/braket/braket_job.py
+-rw-r--r--   0        0        0      277 2023-01-12 01:38:12.521790 qutrunk-0.2.2/qutrunk/backends/braket/exception.py
+-rw-r--r--   0        0        0       29 2022-09-21 02:59:51.006253 qutrunk-0.2.2/qutrunk/backends/ibm/__init__.py
+-rw-r--r--   0        0        0     5155 2023-04-11 07:05:32.976720 qutrunk-0.2.2/qutrunk/backends/ibm/ibm.py
+-rw-r--r--   0        0        0    13273 2023-03-02 02:50:48.481197 qutrunk-0.2.2/qutrunk/backends/ibm/ibm_client.py
+-rw-r--r--   0        0        0       33 2023-01-12 01:38:12.523784 qutrunk-0.2.2/qutrunk/backends/local/__init__.py
+-rw-r--r--   0        0        0      452 2023-01-12 01:38:14.347905 qutrunk-0.2.2/qutrunk/backends/local/exceptions.py
+-rw-r--r--   0        0        0     5218 2023-04-11 01:33:44.033688 qutrunk-0.2.2/qutrunk/backends/local/local.py
+-rw-r--r--   0        0        0    32028 2023-04-11 07:05:32.978714 qutrunk-0.2.2/qutrunk/backends/local/local_impl.py
+-rw-r--r--   0        0        0    62217 2023-02-07 06:25:06.685198 qutrunk-0.2.2/qutrunk/backends/local/sim_distribute.py
+-rw-r--r--   0        0        0    48378 2023-02-07 02:35:02.834476 qutrunk-0.2.2/qutrunk/backends/local/sim_gpu.py
+-rw-r--r--   0        0        0    52886 2023-02-13 01:34:40.066314 qutrunk-0.2.2/qutrunk/backends/local/sim_local.py
+-rw-r--r--   0        0        0       35 2023-01-12 01:38:12.529768 qutrunk-0.2.2/qutrunk/backends/qusaas/__init__.py
+-rw-r--r--   0        0        0     8820 2023-04-11 01:33:44.111794 qutrunk-0.2.2/qutrunk/backends/qusaas/httpclient.py
+-rw-r--r--   0        0        0     7670 2023-04-11 07:05:32.979711 qutrunk-0.2.2/qutrunk/backends/qusaas/qusaas.py
+-rw-r--r--   0        0        0       81 2023-01-12 01:38:12.533767 qutrunk-0.2.2/qutrunk/backends/qusprout/__init__.py
+-rw-r--r--   0        0        0    10003 2023-04-11 07:05:32.980709 qutrunk-0.2.2/qutrunk/backends/qusprout/qusprout.py
+-rw-r--r--   0        0        0     6268 2023-04-11 01:33:44.143065 qutrunk-0.2.2/qutrunk/backends/qusprout/rpcclient.py
+-rw-r--r--   0        0        0     3540 2023-02-13 01:34:40.073253 qutrunk-0.2.2/qutrunk/backends/result.py
+-rw-r--r--   0        0        0      288 2023-04-11 07:05:32.981706 qutrunk-0.2.2/qutrunk/circuit/__init__.py
+-rw-r--r--   0        0        0     1351 2022-09-19 07:38:17.407904 qutrunk-0.2.2/qutrunk/circuit/bit.py
+-rw-r--r--   0        0        0    22544 2023-04-11 01:33:44.174323 qutrunk-0.2.2/qutrunk/circuit/circuit.py
+-rw-r--r--   0        0        0     1103 2022-10-26 06:05:52.209786 qutrunk-0.2.2/qutrunk/circuit/classical_bit.py
+-rw-r--r--   0        0        0     1713 2023-02-07 02:35:02.835474 qutrunk-0.2.2/qutrunk/circuit/classical_reg.py
+-rw-r--r--   0        0        0     6303 2023-04-11 07:05:32.982703 qutrunk-0.2.2/qutrunk/circuit/command.py
+-rw-r--r--   0        0        0     1531 2023-04-11 01:33:44.221218 qutrunk-0.2.2/qutrunk/circuit/counter.py
+-rw-r--r--   0        0        0     1227 2023-02-07 01:13:16.077272 qutrunk-0.2.2/qutrunk/circuit/gates/__init__.py
+-rw-r--r--   0        0        0      804 2023-02-13 01:34:40.077259 qutrunk-0.2.2/qutrunk/circuit/gates/_utils.py
+-rw-r--r--   0        0        0     1198 2022-09-09 01:27:43.223147 qutrunk-0.2.2/qutrunk/circuit/gates/barrier.py
+-rw-r--r--   0        0        0     3982 2023-02-13 01:34:40.080249 qutrunk-0.2.2/qutrunk/circuit/gates/basicgate.py
+-rw-r--r--   0        0        0     2404 2023-04-11 01:33:44.236828 qutrunk-0.2.2/qutrunk/circuit/gates/cr.py
+-rw-r--r--   0        0        0     3929 2023-01-12 01:38:12.544729 qutrunk-0.2.2/qutrunk/circuit/gates/h.py
+-rw-r--r--   0        0        0     1715 2022-11-10 03:12:25.842346 qutrunk-0.2.2/qutrunk/circuit/gates/i.py
+-rw-r--r--   0        0        0     1836 2023-01-12 06:35:41.122439 qutrunk-0.2.2/qutrunk/circuit/gates/iswap.py
+-rw-r--r--   0        0        0      927 2022-09-09 01:27:43.246087 qutrunk-0.2.2/qutrunk/circuit/gates/measure.py
+-rw-r--r--   0        0        0     7840 2023-04-11 01:33:44.268144 qutrunk-0.2.2/qutrunk/circuit/gates/meta.py
+-rw-r--r--   0        0        0     4049 2023-01-12 01:38:12.549715 qutrunk-0.2.2/qutrunk/circuit/gates/p.py
+-rw-r--r--   0        0        0     2108 2022-11-10 02:57:39.388788 qutrunk-0.2.2/qutrunk/circuit/gates/r.py
+-rw-r--r--   0        0        0     1222 2023-02-07 01:13:16.077272 qutrunk-0.2.2/qutrunk/circuit/gates/reset.py
+-rw-r--r--   0        0        0     4469 2023-01-12 01:38:12.551720 qutrunk-0.2.2/qutrunk/circuit/gates/rx.py
+-rw-r--r--   0        0        0     2744 2022-11-10 02:57:39.404744 qutrunk-0.2.2/qutrunk/circuit/gates/rxx.py
+-rw-r--r--   0        0        0     4244 2023-01-12 01:38:12.553704 qutrunk-0.2.2/qutrunk/circuit/gates/ry.py
+-rw-r--r--   0        0        0     2280 2022-11-10 02:57:39.427683 qutrunk-0.2.2/qutrunk/circuit/gates/ryy.py
+-rw-r--r--   0        0        0     4237 2023-01-12 01:38:12.555698 qutrunk-0.2.2/qutrunk/circuit/gates/rz.py
+-rw-r--r--   0        0        0     2226 2022-11-10 02:57:39.443640 qutrunk-0.2.2/qutrunk/circuit/gates/rzz.py
+-rw-r--r--   0        0        0     1492 2023-01-12 01:38:12.556696 qutrunk-0.2.2/qutrunk/circuit/gates/s.py
+-rw-r--r--   0        0        0     1505 2023-01-12 01:38:12.558690 qutrunk-0.2.2/qutrunk/circuit/gates/sdg.py
+-rw-r--r--   0        0        0     1494 2022-11-10 02:57:39.448628 qutrunk-0.2.2/qutrunk/circuit/gates/sqrtswap.py
+-rw-r--r--   0        0        0     3816 2023-01-12 01:38:12.560685 qutrunk-0.2.2/qutrunk/circuit/gates/sqrtx.py
+-rw-r--r--   0        0        0     4114 2023-01-12 01:38:12.561683 qutrunk-0.2.2/qutrunk/circuit/gates/swap.py
+-rw-r--r--   0        0        0     1530 2022-11-10 03:12:25.849327 qutrunk-0.2.2/qutrunk/circuit/gates/sxdg.py
+-rw-r--r--   0        0        0     1513 2023-01-12 01:38:12.563677 qutrunk-0.2.2/qutrunk/circuit/gates/t.py
+-rw-r--r--   0        0        0     1504 2023-01-12 01:38:12.565672 qutrunk-0.2.2/qutrunk/circuit/gates/tdg.py
+-rw-r--r--   0        0        0     4166 2023-02-07 02:35:02.837469 qutrunk-0.2.2/qutrunk/circuit/gates/u1.py
+-rw-r--r--   0        0        0     1997 2023-02-07 02:35:02.839463 qutrunk-0.2.2/qutrunk/circuit/gates/u2.py
+-rw-r--r--   0        0        0     7934 2023-02-07 02:35:02.840460 qutrunk-0.2.2/qutrunk/circuit/gates/u3.py
+-rw-r--r--   0        0        0     4874 2023-04-11 07:05:32.984698 qutrunk-0.2.2/qutrunk/circuit/gates/x.py
+-rw-r--r--   0        0        0     1535 2022-11-10 03:12:25.897059 qutrunk-0.2.2/qutrunk/circuit/gates/x1.py
+-rw-r--r--   0        0        0     3775 2023-01-12 01:38:12.568668 qutrunk-0.2.2/qutrunk/circuit/gates/y.py
+-rw-r--r--   0        0        0     1528 2022-11-10 03:12:25.900081 qutrunk-0.2.2/qutrunk/circuit/gates/y1.py
+-rw-r--r--   0        0        0     4823 2023-04-11 07:05:32.985695 qutrunk-0.2.2/qutrunk/circuit/gates/z.py
+-rw-r--r--   0        0        0     1315 2022-11-10 03:12:25.904071 qutrunk-0.2.2/qutrunk/circuit/gates/z1.py
+-rw-r--r--   0        0        0      306 2022-11-10 03:12:25.907041 qutrunk-0.2.2/qutrunk/circuit/ops/__init__.py
+-rw-r--r--   0        0        0     1564 2023-02-07 01:13:16.124912 qutrunk-0.2.2/qutrunk/circuit/ops/addition.py
+-rw-r--r--   0        0        0     2793 2023-01-12 01:38:12.573650 qutrunk-0.2.2/qutrunk/circuit/ops/amp.py
+-rw-r--r--   0        0        0     2537 2023-02-07 01:13:16.125910 qutrunk-0.2.2/qutrunk/circuit/ops/classical.py
+-rw-r--r--   0        0        0     1186 2023-01-12 01:38:12.577640 qutrunk-0.2.2/qutrunk/circuit/ops/decrement.py
+-rw-r--r--   0        0        0     1204 2023-01-12 01:38:12.578637 qutrunk-0.2.2/qutrunk/circuit/ops/increment.py
+-rw-r--r--   0        0        0      253 2022-11-10 02:57:39.511459 qutrunk-0.2.2/qutrunk/circuit/ops/operator.py
+-rw-r--r--   0        0        0     1189 2022-11-10 03:12:25.915649 qutrunk-0.2.2/qutrunk/circuit/ops/plus.py
+-rw-r--r--   0        0        0     2827 2023-04-11 01:33:44.330626 qutrunk-0.2.2/qutrunk/circuit/ops/qaa.py
+-rw-r--r--   0        0        0     3335 2023-02-13 01:34:40.083448 qutrunk-0.2.2/qutrunk/circuit/ops/qft.py
+-rw-r--r--   0        0        0     2063 2023-02-07 02:35:02.842455 qutrunk-0.2.2/qutrunk/circuit/ops/qpe.py
+-rw-r--r--   0        0        0     1729 2023-04-11 07:05:32.987690 qutrunk-0.2.2/qutrunk/circuit/parameter.py
+-rw-r--r--   0        0        0      707 2022-10-26 06:05:52.562882 qutrunk-0.2.2/qutrunk/circuit/qubit.py
+-rw-r--r--   0        0        0     3493 2023-04-11 01:33:44.387541 qutrunk-0.2.2/qutrunk/circuit/qureg.py
+-rw-r--r--   0        0        0      225 2023-01-12 01:38:12.581630 qutrunk-0.2.2/qutrunk/config/__init__.py
+-rw-r--r--   0        0        0      402 2023-01-12 06:35:41.145378 qutrunk-0.2.2/qutrunk/config/config.yaml
+-rw-r--r--   0        0        0       25 2022-11-10 03:12:25.926908 qutrunk-0.2.2/qutrunk/config/qubox.yaml
+-rw-r--r--   0        0        0      142 2022-09-21 02:59:51.026189 qutrunk-0.2.2/qutrunk/converters/__init__.py
+-rw-r--r--   0        0        0    14239 2022-09-21 02:59:51.027747 qutrunk-0.2.2/qutrunk/converters/ast_to_dag.py
+-rw-r--r--   0        0        0     1158 2022-09-19 07:38:17.429846 qutrunk-0.2.2/qutrunk/converters/circuit_to_dag.py
+-rw-r--r--   0        0        0     2129 2022-09-21 02:59:51.029744 qutrunk-0.2.2/qutrunk/converters/dag_to_circuit.py
+-rw-r--r--   0        0        0     1556 2022-11-10 02:57:39.577283 qutrunk-0.2.2/qutrunk/converters/mapping.py
+-rw-r--r--   0        0        0       36 2022-09-21 02:59:51.032737 qutrunk-0.2.2/qutrunk/dagcircuit/__init__.py
+-rw-r--r--   0        0        0     6661 2022-09-19 07:38:17.431843 qutrunk-0.2.2/qutrunk/dagcircuit/dagcircuit.py
+-rw-r--r--   0        0        0     1703 2023-04-11 01:33:44.389836 qutrunk-0.2.2/qutrunk/dagcircuit/dagnode.py
+-rw-r--r--   0        0        0        0 2022-10-11 02:47:27.766837 qutrunk-0.2.2/qutrunk/example/__init__.py
+-rw-r--r--   0        0        0      867 2023-04-11 01:33:44.391833 qutrunk-0.2.2/qutrunk/example/bell_pair.py
+-rw-r--r--   0        0        0      132 2022-11-10 02:57:39.581286 qutrunk-0.2.2/qutrunk/example/bell_pair.qasm
+-rw-r--r--   0        0        0      185 2022-11-10 02:57:39.583267 qutrunk-0.2.2/qutrunk/example/bell_pair.qusl
+-rw-r--r--   0        0        0     1642 2023-04-11 01:33:44.432115 qutrunk-0.2.2/qutrunk/example/bernstein_vazirani.py
+-rw-r--r--   0        0        0      818 2023-04-11 01:33:44.432115 qutrunk-0.2.2/qutrunk/example/deutsch.py
+-rw-r--r--   0        0        0      881 2023-04-11 01:33:44.432115 qutrunk-0.2.2/qutrunk/example/ghz.py
+-rw-r--r--   0        0        0     1611 2023-04-11 01:33:44.487997 qutrunk-0.2.2/qutrunk/example/grover.py
+-rw-r--r--   0        0        0     1690 2023-04-11 01:33:44.534855 qutrunk-0.2.2/qutrunk/example/grover_distribute.py
+-rw-r--r--   0        0        0     1690 2023-04-11 01:33:44.565977 qutrunk-0.2.2/qutrunk/example/grover_gpu.py
+-rw-r--r--   0        0        0   105205 2023-01-12 06:35:41.156348 qutrunk-0.2.2/qutrunk/example/jupyter/algorithm.ipynb
+-rw-r--r--   0        0        0     3835 2023-01-12 06:35:41.157345 qutrunk-0.2.2/qutrunk/example/jupyter/awslocal_qrng.ipynb
+-rw-r--r--   0        0        0    29003 2023-04-11 01:33:44.612978 qutrunk-0.2.2/qutrunk/example/jupyter/backend.ipynb
+-rw-r--r--   0        0        0     8929 2023-01-12 01:38:12.594594 qutrunk-0.2.2/qutrunk/example/jupyter/circuit.ipynb
+-rw-r--r--   0        0        0    21165 2023-02-13 01:34:40.088685 qutrunk-0.2.2/qutrunk/example/jupyter/gate.ipynb
+-rw-r--r--   0        0        0    10786 2023-02-09 01:49:51.276309 qutrunk-0.2.2/qutrunk/example/jupyter/ops.ipynb
+-rw-r--r--   0        0        0    39718 2023-04-11 01:33:44.690974 qutrunk-0.2.2/qutrunk/example/jupyter/qutrunk_mindspore.ipynb
+-rw-r--r--   0        0        0    47588 2023-04-11 01:33:44.722240 qutrunk-0.2.2/qutrunk/example/jupyter/qutrunk_paddle.ipynb
+-rw-r--r--   0        0        0    61424 2023-04-11 01:33:44.800406 qutrunk-0.2.2/qutrunk/example/jupyter/qutrunk_pytorch.ipynb
+-rw-r--r--   0        0        0    35762 2023-02-07 02:35:02.851431 qutrunk-0.2.2/qutrunk/example/jupyter/qutrunk_tensorflow.ipynb
+-rw-r--r--   0        0        0      867 2023-04-11 01:33:44.800406 qutrunk-0.2.2/qutrunk/example/phase_estimation.py
+-rw-r--r--   0        0        0      714 2023-04-11 01:33:44.815917 qutrunk-0.2.2/qutrunk/example/phase_kickback.py
+-rw-r--r--   0        0        0     1240 2023-04-11 01:33:44.831666 qutrunk-0.2.2/qutrunk/example/superdense.py
+-rw-r--r--   0        0        0     1305 2023-04-11 07:05:32.989685 qutrunk-0.2.2/qutrunk/example/teleport.py
+-rw-r--r--   0        0        0      406 2022-11-10 02:57:39.636125 qutrunk-0.2.2/qutrunk/exceptions.py
+-rw-r--r--   0        0        0      355 2022-09-21 02:59:51.052290 qutrunk-0.2.2/qutrunk/qasm/__init__.py
+-rw-r--r--   0        0        0      315 2022-09-21 02:59:51.054139 qutrunk-0.2.2/qutrunk/qasm/exceptions.py
+-rw-r--r--   0        0        0     5086 2022-05-23 06:54:12.076393 qutrunk-0.2.2/qutrunk/qasm/libs/qelib1.inc
+-rw-r--r--   0        0        0      837 2022-11-10 02:57:39.638134 qutrunk-0.2.2/qutrunk/qasm/libs/qulib1.inc
+-rw-r--r--   0        0        0     2235 2022-08-23 03:06:14.307069 qutrunk-0.2.2/qutrunk/qasm/libs/stdgates.inc
+-rw-r--r--   0        0        0     1356 2022-08-23 02:59:56.717189 qutrunk-0.2.2/qutrunk/qasm/node/__init__.py
+-rw-r--r--   0        0        0      957 2022-08-23 02:59:56.718213 qutrunk-0.2.2/qutrunk/qasm/node/barrier.py
+-rw-r--r--   0        0        0     2106 2022-09-21 02:59:51.056136 qutrunk-0.2.2/qutrunk/qasm/node/binaryop.py
+-rw-r--r--   0        0        0     1500 2022-09-21 02:59:51.058131 qutrunk-0.2.2/qutrunk/qasm/node/binaryoperator.py
+-rw-r--r--   0        0        0     1040 2022-08-23 02:59:56.720212 qutrunk-0.2.2/qutrunk/qasm/node/cnot.py
+-rw-r--r--   0        0        0     1494 2022-08-23 02:59:56.720212 qutrunk-0.2.2/qutrunk/qasm/node/creg.py
+-rw-r--r--   0        0        0     1669 2022-08-23 02:59:56.721178 qutrunk-0.2.2/qutrunk/qasm/node/customunitary.py
+-rw-r--r--   0        0        0     1098 2022-09-19 07:38:17.441814 qutrunk-0.2.2/qutrunk/qasm/node/expressionlist.py
+-rw-r--r--   0        0        0     2806 2022-09-09 01:27:43.312907 qutrunk-0.2.2/qutrunk/qasm/node/external.py
+-rw-r--r--   0        0        0     1285 2022-08-23 02:59:56.723199 qutrunk-0.2.2/qutrunk/qasm/node/format.py
+-rw-r--r--   0        0        0     2154 2022-08-23 02:59:56.723199 qutrunk-0.2.2/qutrunk/qasm/node/gate.py
+-rw-r--r--   0        0        0     1366 2022-09-19 07:38:17.443808 qutrunk-0.2.2/qutrunk/qasm/node/gatebody.py
+-rw-r--r--   0        0        0     2856 2022-08-23 02:59:56.725194 qutrunk-0.2.2/qutrunk/qasm/node/id.py
+-rw-r--r--   0        0        0     1053 2022-08-23 02:59:56.726164 qutrunk-0.2.2/qutrunk/qasm/node/idlist.py
+-rw-r--r--   0        0        0     1231 2022-08-23 02:59:56.728158 qutrunk-0.2.2/qutrunk/qasm/node/if_.py
+-rw-r--r--   0        0        0     1325 2022-08-23 02:59:56.728158 qutrunk-0.2.2/qutrunk/qasm/node/indexedid.py
+-rw-r--r--   0        0        0     1575 2022-08-23 02:59:56.729162 qutrunk-0.2.2/qutrunk/qasm/node/intnode.py
+-rw-r--r--   0        0        0     1134 2022-09-21 02:59:51.059153 qutrunk-0.2.2/qutrunk/qasm/node/measure.py
+-rw-r--r--   0        0        0     2029 2022-08-23 02:59:56.731151 qutrunk-0.2.2/qutrunk/qasm/node/node.py
+-rw-r--r--   0        0        0      883 2022-08-23 02:59:56.732149 qutrunk-0.2.2/qutrunk/qasm/node/nodeexception.py
+-rw-r--r--   0        0        0     1981 2022-09-19 07:38:17.444806 qutrunk-0.2.2/qutrunk/qasm/node/opaque.py
+-rw-r--r--   0        0        0     1822 2022-09-09 01:27:43.313904 qutrunk-0.2.2/qutrunk/qasm/node/prefix.py
+-rw-r--r--   0        0        0     1116 2022-09-19 07:38:17.445803 qutrunk-0.2.2/qutrunk/qasm/node/primarylist.py
+-rw-r--r--   0        0        0     1013 2022-09-19 07:38:17.446800 qutrunk-0.2.2/qutrunk/qasm/node/program.py
+-rw-r--r--   0        0        0     1494 2022-08-23 02:59:56.736138 qutrunk-0.2.2/qutrunk/qasm/node/qreg.py
+-rw-r--r--   0        0        0     1949 2022-08-23 03:06:14.309060 qutrunk-0.2.2/qutrunk/qasm/node/real.py
+-rw-r--r--   0        0        0      957 2022-09-19 07:38:17.448795 qutrunk-0.2.2/qutrunk/qasm/node/reset.py
+-rw-r--r--   0        0        0     1441 2022-09-21 02:59:51.061157 qutrunk-0.2.2/qutrunk/qasm/node/unaryoperator.py
+-rw-r--r--   0        0        0     1109 2022-08-23 02:59:56.738151 qutrunk-0.2.2/qutrunk/qasm/node/universalunitary.py
+-rw-r--r--   0        0        0     1812 2022-09-21 02:59:51.063155 qutrunk-0.2.2/qutrunk/qasm/qasm.py
+-rw-r--r--   0        0        0     5500 2022-09-19 07:38:17.450804 qutrunk-0.2.2/qutrunk/qasm/qasmlexer.py
+-rw-r--r--   0        0        0    40599 2022-09-21 02:59:51.064177 qutrunk-0.2.2/qutrunk/qasm/qasmparser.py
+-rw-r--r--   0        0        0        0 2023-01-12 01:38:12.727239 qutrunk-0.2.2/qutrunk/thrift/__init__.py
+-rw-r--r--   0        0        0       35 2023-01-12 01:38:14.092588 qutrunk-0.2.2/qutrunk/thrift/code/__init__.py
+-rw-r--r--   0        0        0      703 2023-01-12 06:35:41.431613 qutrunk-0.2.2/qutrunk/thrift/code/constants.py
+-rw-r--r--   0        0        0     4363 2023-01-12 06:35:41.432609 qutrunk-0.2.2/qutrunk/thrift/code/ttypes.py
+-rw-r--r--   0        0        0     1433 2023-01-12 01:38:14.083613 qutrunk-0.2.2/qutrunk/thrift/idl/ecode.thrift
+-rw-r--r--   0        0        0      645 2023-01-12 06:35:41.434605 qutrunk-0.2.2/qutrunk/thrift/idl/gen_py.sh
+-rw-r--r--   0        0        0     1509 2023-02-13 01:34:40.098660 qutrunk-0.2.2/qutrunk/thrift/idl/qusprout.thrift
+-rw-r--r--   0        0        0     7435 2023-04-11 07:05:32.991683 qutrunk-0.2.2/qutrunk/thrift/idl/qusproutdata.thrift
+-rw-r--r--   0        0        0       53 2023-01-12 01:38:14.066657 qutrunk-0.2.2/qutrunk/thrift/qusprout/__init__.py
+-rw-r--r--   0        0        0      411 2023-01-12 06:35:41.451559 qutrunk-0.2.2/qutrunk/thrift/qusprout/constants.py
+-rw-r--r--   0        0        0     5649 2023-02-13 01:34:40.102291 qutrunk-0.2.2/qutrunk/thrift/qusprout/QuSproutServer-remote
+-rw-r--r--   0        0        0    78824 2023-02-13 01:34:40.103921 qutrunk-0.2.2/qutrunk/thrift/qusprout/QuSproutServer.py
+-rw-r--r--   0        0        0      532 2023-01-12 06:35:41.453553 qutrunk-0.2.2/qutrunk/thrift/qusprout/ttypes.py
+-rw-r--r--   0        0        0       35 2023-01-12 01:38:14.058680 qutrunk-0.2.2/qutrunk/thrift/qusproutdata/__init__.py
+-rw-r--r--   0        0        0      411 2023-01-12 06:35:41.455548 qutrunk-0.2.2/qutrunk/thrift/qusproutdata/constants.py
+-rw-r--r--   0        0        0   113590 2023-04-11 07:05:32.994672 qutrunk-0.2.2/qutrunk/thrift/qusproutdata/ttypes.py
+-rw-r--r--   0        0        0       74 2022-09-19 07:38:17.480710 qutrunk-0.2.2/qutrunk/tools/__init__.py
+-rw-r--r--   0        0        0      621 2022-11-10 02:57:39.830660 qutrunk-0.2.2/qutrunk/tools/algorithm.py
+-rw-r--r--   0        0        0      887 2023-01-12 01:38:12.747187 qutrunk-0.2.2/qutrunk/tools/check.py
+-rw-r--r--   0        0        0     1046 2023-01-12 01:38:12.748184 qutrunk-0.2.2/qutrunk/tools/check_sprout.py
+-rw-r--r--   0        0        0      838 2023-04-11 01:33:44.862782 qutrunk-0.2.2/qutrunk/tools/env_reader.py
+-rw-r--r--   0        0        0      374 2023-04-11 01:33:44.862782 qutrunk-0.2.2/qutrunk/tools/function_time.py
+-rw-r--r--   0        0        0      502 2023-01-12 01:38:12.751176 qutrunk-0.2.2/qutrunk/tools/get_config.py
+-rw-r--r--   0        0        0      221 2022-07-12 02:20:50.337008 qutrunk-0.2.2/qutrunk/tools/ide_parameter.json
+-rw-r--r--   0        0        0     2806 2023-04-11 01:33:44.878477 qutrunk-0.2.2/qutrunk/tools/produce_algorithm.py
+-rw-r--r--   0        0        0     1829 2023-01-12 06:35:41.465521 qutrunk-0.2.2/qutrunk/tools/qusl_parse.py
+-rw-r--r--   0        0        0     3883 2023-02-07 01:13:16.396269 qutrunk-0.2.2/qutrunk/tools/random_circuit.py
+-rw-r--r--   0        0        0      412 2022-11-10 03:12:26.048947 qutrunk-0.2.2/qutrunk/tools/read_qubox.py
+-rw-r--r--   0        0        0      197 2022-07-12 02:20:50.340977 qutrunk-0.2.2/qutrunk/tools/result.json
+-rw-r--r--   0        0        0     1761 2022-09-21 02:59:51.149732 qutrunk-0.2.2/qutrunk/tools/set_config.py
+-rw-r--r--   0        0        0      100 2022-09-21 02:59:51.150702 qutrunk-0.2.2/qutrunk/visualizations/__init__.py
+-rw-r--r--   0        0        0     1401 2022-09-09 09:24:47.015761 qutrunk-0.2.2/qutrunk/visualizations/circuit_visualization.py
+-rw-r--r--   0        0        0    10244 2022-09-13 02:15:54.903738 qutrunk-0.2.2/qutrunk/visualizations/layer.py
+-rw-r--r--   0        0        0    31188 2023-04-11 07:05:32.996667 qutrunk-0.2.2/qutrunk/visualizations/text.py
+-rw-r--r--   0        0        0    18338 2022-09-21 02:59:51.153706 qutrunk-0.2.2/qutrunk/visualizations/text_draw_element.py
+-rw-r--r--   0        0        0      750 2022-09-19 07:38:17.494671 qutrunk-0.2.2/qutrunk/visualizations/utils.py
+-rw-r--r--   0        0        0     6085 2023-02-10 01:16:43.384143 qutrunk-0.2.2/README.md
+-rw-r--r--   0        0        0     7695 2023-04-11 07:55:05.236706 qutrunk-0.2.2/setup.py
+-rw-r--r--   0        0        0     7411 2023-04-11 07:55:05.236706 qutrunk-0.2.2/PKG-INFO
```

### Comparing `qutrunk-0.2.1/LICENSE` & `qutrunk-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/pyproject.toml` & `qutrunk-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qutrunk"
-version = "0.2.1"
+version = "0.2.2"
 description = "qutrunk is an open source library for quantum computing."
 authors = ["qudoorzh2022 <qudoorzh2022@163.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "http://www.qudoor.com/"
 repository = "https://github.com/queco-quantum/qutrunk"
 documentation = "http://developer.queco.cn/qutrunk_api/"
```

### Comparing `qutrunk-0.2.1/qutrunk/algorithm/vqe.py` & `qutrunk-0.2.2/qutrunk/algorithm/vqe.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/backends/backend.py` & `qutrunk-0.2.2/qutrunk/backends/backend.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/backends/braket/adapter.py` & `qutrunk-0.2.2/qutrunk/backends/braket/adapter.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/backends/braket/braket.py` & `qutrunk-0.2.2/qutrunk/backends/braket/braket.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,22 +45,29 @@
         self._name = name
         self._description = description
         self._online_date = online_date
         self._status = device.status
         self._circuit = None
         self.task_id = uuid.uuid4().hex
 
+    def check_cmd_valid(self, circuit):
+        if circuit and circuit.cmds:
+            for cmd in circuit.cmds:
+                if cmd.measurecond and cmd.measurecond.enable:
+                    raise Exception("%s does not support condition gate." % self.name)
+                
     def send_circuit(self, circuit, final=False):
         """Send the quantum circuit to Braket backend.
 
         Args:
             circuit: Quantum circuit to send.
             final: True if quantum circuit finish, default False, \
             when final==True The backend program will release the computing resources.
         """
+        self.check_cmd_valid(circuit)
         self._circuit = circuit
 
     def run(self, shots=1024):
         """Run quantum circuit.
 
         Args:
             shots: Circuit run times, for sampling, default: 1024.
```

### Comparing `qutrunk-0.2.1/qutrunk/backends/braket/braket_job.py` & `qutrunk-0.2.2/qutrunk/backends/braket/braket_job.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/backends/ibm/ibm.py` & `qutrunk-0.2.2/qutrunk/backends/ibm/ibm.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,24 +53,31 @@
         self._allocated_qubits = set()
         # quantum circuit for json format
         self._json = []
         # measured qubit id
         self._measured_ids = []
         self.task_id = uuid.uuid4().hex
 
+    def check_cmd_valid(self, circuit):
+        if circuit and circuit.cmds:
+            for cmd in circuit.cmds:
+                if cmd.measurecond and cmd.measurecond.enable:
+                    raise Exception("%s does not support condition gate." % self.name)
+                
     def send_circuit(self, circuit, final=False):
         """Send the quantum circuit to IBM backend.
 
         Args:
             circuit: Quantum circuit to send.
             final: True if quantum circuit finish, default False.
 
         Returns:
             The result return from IBM Backend.
         """
+        self.check_cmd_valid(circuit)
         self._allocated_qubits.add(len(circuit.qreg))
 
         for ct in circuit.cmds:
             self._circuit_to_json(ct)
 
         for measured_id in self._measured_ids:
             self._json.append(
```

### Comparing `qutrunk-0.2.1/qutrunk/backends/ibm/ibm_client.py` & `qutrunk-0.2.2/qutrunk/backends/ibm/ibm_client.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/backends/local/local.py` & `qutrunk-0.2.2/qutrunk/backends/local/local.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/backends/local/local_impl.py` & `qutrunk-0.2.2/qutrunk/backends/local/local_impl.py`

 * *Files 3% similar despite different names*

```diff
@@ -177,20 +177,33 @@
             term_coeff_list: the coefficients of each term in the sum of Pauli products.
 
         Returns:
             the expected value of a sum of products of Pauli operators. 
         """
         return self.sim.get_expec_pauli_sum(oper_type_list, term_coeff_list)
 
+    def reach_measure_condition(self, cond):
+        index = self.run_times
+        if index < len(self.result.measures):
+            for idx, value in self.result.measures[index].measure.items():
+                if idx == cond.idx and value == cond.cond_value:
+                    return True
+
+        return False
+    
     def exec_cmd(self, cmd):
         # TODO: need to improve.
+        if cmd.measurecond and cmd.measurecond.enable:
+            if self.reach_measure_condition(cmd.measurecond) == False:
+                return
+
         if str(cmd.gate) == "Measure":
             res = self.sim.measure(cmd.targets[0])
-            index = self.run_times
             meassize = len(self.result.measures)
+            index = self.run_times
             if index >= meassize:
                 mrs = MeasureQubits()
                 mrs.add_measure(cmd.targets[0], res)
                 self.result.measures.append(mrs)
             else:
                 self.result.measures[index].add_measure(cmd.targets[0], res)
             return
```

### Comparing `qutrunk-0.2.1/qutrunk/backends/local/sim_distribute.py` & `qutrunk-0.2.2/qutrunk/backends/local/sim_distribute.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/backends/local/sim_gpu.py` & `qutrunk-0.2.2/qutrunk/backends/local/sim_gpu.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/backends/local/sim_local.py` & `qutrunk-0.2.2/qutrunk/backends/local/sim_local.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/backends/qusaas/httpclient.py` & `qutrunk-0.2.2/qutrunk/backends/qusaas/httpclient.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/backends/qusaas/qusaas.py` & `qutrunk-0.2.2/qutrunk/backends/qusaas/qusaas.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,22 +47,30 @@
 
         """
         self.circuit = None
         self.run_mode = run_mode
         self._api_server = QuSaasApiServer(ak, sk)
         self.task_id = self._api_server._taskid
 
+    def check_cmd_valid(self, circuit):
+        if circuit and circuit.cmds:
+            for cmd in circuit.cmds:
+                if cmd.measurecond and cmd.measurecond.enable:
+                    raise Exception("%s does not support condition gate." % self.name)
+                
     def send_circuit(self, circuit, final=False):
         """Send the quantum circuit to qusprout backend.
 
         Args:
             circuit: Quantum circuit to send.
             final: True if quantum circuit finish, default False, \
             when final==True The backend program will release the computing resources.
         """
+        self.check_cmd_valid(circuit)
+        
         start = circuit.cmd_cursor
         stop = len(circuit.cmds)
 
         cmds = circuit.cmds[start:stop]
 
         circuit.forward(stop - start)
```

### Comparing `qutrunk-0.2.1/qutrunk/backends/qusprout/qusprout.py` & `qutrunk-0.2.2/qutrunk/backends/qusprout/qusprout.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,22 +134,26 @@
                     )
                 if cmd.cmdex.mat is not None:
                     _mat = qusproutdata.Matrix(
                         cmd.cmdex.mat.reals, cmd.cmdex.mat.imags, cmd.cmdex.mat.unitary
                     )
                 cmdex = qusproutdata.Cmdex(amp=_amp, mat=_mat)
 
+            cond = None
+            if cmd.measurecond:
+                cond = qusproutdata.MeasureCond(cmd.measurecond.enable, cmd.measurecond.idx, cmd.measurecond.cond_value)
             c = qusproutdata.Cmd(
                 str(cmd.gate),
                 cmd.targets,
                 cmd.controls,
                 cmd.rotation,
                 cmd.qasm(),
                 cmd.inverse,
                 cmdex,
+                cond,
             )
             cmds.append(c)
 
         circuit.forward(stop - start)
 
         exectype = qusproutdata.ExecCmdType.ExecTypeDefault
         if self.run_mode == "cpu_mpi":
@@ -160,14 +164,16 @@
             exectype = qusproutdata.ExecCmdType.ExecTypeCpuSingle
 
         # 服务端初始化
         if start == 0:
             res, elapsed = self._api_server.init(
                 circuit.num_qubits, circuit.density, exectype
             )
+            if res.base.code != 0:
+                raise Exception(f"Circuit init failed, {res.base.msg}")
             if self.circuit.counter:
                 self.circuit.counter.acc_run_time(elapsed)
 
         if len(cmds) == 0 and (not final):
             return
 
         # 发送至服务
```

### Comparing `qutrunk-0.2.1/qutrunk/backends/qusprout/rpcclient.py` & `qutrunk-0.2.2/qutrunk/backends/qusprout/rpcclient.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/backends/result.py` & `qutrunk-0.2.2/qutrunk/backends/result.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/bit.py` & `qutrunk-0.2.2/qutrunk/circuit/bit.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/circuit.py` & `qutrunk-0.2.2/qutrunk/circuit/circuit.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/classical_bit.py` & `qutrunk-0.2.2/qutrunk/circuit/classical_bit.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/classical_reg.py` & `qutrunk-0.2.2/qutrunk/circuit/classical_reg.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/command.py` & `qutrunk-0.2.2/qutrunk/circuit/command.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,25 +30,39 @@
     """
     def __init__(self):
         self.reals = []
         self.imags = []
         self.unitary = False
 
 
+class MeasureCond:
+    """Command Measure Condition.
+
+    Args:
+        enable: Function switch.
+        idx: Measure index.
+        cond_value: Condition value.
+    """
+    def __init__(self, enable=False, idx=None, cond_value=None):
+        self.enable = enable
+        self.idx = idx
+        self.cond_value = cond_value
+
+
 class CmdEx:
     """Command extension.
 
     Args:
         amp: Amplitude object.
     """
     def __init__(self, amp=None, mat=None):
         self.amp = amp
         self.mat = mat
-
-
+        
+        
 class Command:
     """Converts the quantum gate operation into a specific command.
 
     Args:
         gate: Quantum gate operator.
         targets: Target qubits.
         controls: Control qubits.
@@ -60,14 +74,15 @@
         self,
         gate,
         targets=None,
         controls=None,
         rotation=None,
         inverse=False,
         cmdex=None,
+        measurecond=None,
     ):
         # TODO: modify controls and rotation to tuple?
         if targets is None:
             self.targets = []
         else:
             self.targets = list(targets)
 
@@ -86,19 +101,20 @@
         self.inverse = inverse
 
         self.parameters = {}
         for i, r in enumerate(self.rotation):
             if isinstance(r, Parameter):
                 # map index to parameter
                 self.parameters[i] = r
-                r.host = self
+                r.hosts.append(self)
 
         # Command extention data
         # TODO: extra
         self.cmdex = cmdex
+        self.measurecond = measurecond
 
     def __eq__(self, other):
         """Two command are the same if they have the same qasm."""
         # TODO: need to improve
         if type(self) is not type(other):
             return False
 
@@ -150,14 +166,15 @@
         if name == "AMP":
             return f"AMP({self.gate.classicvector}, {self.gate.startind}, {self.gate.numamps}) * q"
             # return 'AMP({}, {}, {}) * q'.format(self.gate.classicvector, self.gate.startind, self.gate.numamps)
 
         params = []
         param_str = ""
         inv_str = ""
+        cond_str = ""
 
         # only append control bit count as param when it's more than one
         if self.cmdex and self.cmdex.mat:
             params += self.gate.matrix
 
         ctrl_cnt = len(self.controls)
         if ctrl_cnt:
@@ -175,15 +192,18 @@
         # add parentheses when qubits count is more than one
         if len(qubits_index) > 1:
             qubits_str = "(" + qubits_str + ")"
 
         if self.inverse:
             inv_str += ".inv()"
 
-        return name + param_str + inv_str + " * " + qubits_str
+        if self.measurecond:
+            cond_str += f".condition(q[{self.measurecond.idx}], {self.measurecond.cond_value})"
+
+        return name + param_str + inv_str + cond_str + " * " + qubits_str
 
     @property
     def name(self) -> str:
         """Command name."""
         return self.gate
 
     @property
```

### Comparing `qutrunk-0.2.1/qutrunk/circuit/counter.py` & `qutrunk-0.2.2/qutrunk/circuit/counter.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/__init__.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/__init__.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/_utils.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/_utils.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/barrier.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/barrier.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/basicgate.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/basicgate.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/cr.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/cr.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/h.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/h.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/i.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/i.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/iswap.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/iswap.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/measure.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/measure.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/meta.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/meta.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/p.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/p.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/r.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/r.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/reset.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/reset.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/rx.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/rx.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/rxx.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/rxx.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/ry.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/ry.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/ryy.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/ryy.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/rz.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/rz.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/rzz.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/rzz.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/s.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/s.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/sdg.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/sdg.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/sqrtswap.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/sqrtswap.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/sqrtx.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/sqrtx.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/swap.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/swap.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/sxdg.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/sxdg.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/t.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/t.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/tdg.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/tdg.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/u1.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/u1.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/u2.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/u2.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/u3.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/u3.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/x.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/x.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from qutrunk.circuit import Command
+from qutrunk.circuit import Command, MeasureCond
 from .basicgate import BasicGate, Observable, PauliType
 from qutrunk.circuit.qubit import QuBit
 
 
 class XGate(BasicGate, Observable):
     r"""Apply the single-qubit Pauli-X (also known as the X, sigma-X, NOT or bit-flip) gate.
 
@@ -19,14 +19,15 @@
         .. code-block:: python
 
             X * qr[0]
     """
 
     def __init__(self):
         super().__init__()
+        self.measurecond = None
 
     def __str__(self):
         return "X"
 
     def __or__(self, qubit):
         """Quantum logic gate operation.
 
@@ -41,15 +42,15 @@
         Raises:
             NotImplementedError: If the argument is not a Qubit object.
         """
         if not isinstance(qubit, QuBit):
             raise TypeError("The argument must be Qubit object.")
 
         targets = [qubit.index]
-        cmd = Command(self, targets, inverse=self.is_inverse)
+        cmd = Command(self, targets, inverse=self.is_inverse, measurecond=self.measurecond)
         self.commit(qubit.circuit, cmd)
 
     def __mul__(self, qubit):
         """Overwrite * operator to achieve quantum logic gate operation, reuse __or__ operator implement."""
         self.__or__(qubit)
 
     @property
@@ -84,15 +85,18 @@
         
         Args:
             ctrl_cnt: The number of control qubits, default: 1.
         """
         gate = MCX(ctrl_cnt)
         gate.is_inverse = self.is_inverse
         return gate
-
+    
+    def condition(self, qubit, cond_value):
+        self.measurecond = MeasureCond(True, qubit.index, cond_value)
+        return self
 
 PauliX = X = NOT = XGate()
 
 
 class MCX(BasicGate):
     """Multi-control X(NOT) gate.
```

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/x1.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/x1.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/y.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/y.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/y1.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/y1.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/z.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/z.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """Z gates."""
 
 import numpy as np
 
 from .basicgate import BasicGate, Observable, PauliType
-from qutrunk.circuit import Qureg, QuBit, Command
+from qutrunk.circuit import Qureg, QuBit, Command, MeasureCond
 
 
 class ZGate(BasicGate, Observable):
     """Apply the single-qubit Pauli-Z (also known as the Z, sigma-Z or phase-flip) gate.
 
     Example:
         .. code-block:: python
 
             Z * qr[0]
     """
 
     def __init__(self):
         """Create new Z gate."""
         super().__init__()
+        self.measurecond = None
 
     def __str__(self):
         return "Z"
 
     def __or__(self, qubit):
         """Quantum logic gate operation.
 
@@ -36,15 +37,15 @@
         Raises:
             TypeError: If the argument is not a Qubit object.
         """
         if not isinstance(qubit, QuBit):
             raise TypeError("The argument must be Qubit object.")
 
         targets = [qubit.index]
-        cmd = Command(self, targets, inverse=self.is_inverse)
+        cmd = Command(self, targets, inverse=self.is_inverse, measurecond=self.measurecond)
         self.commit(qubit.circuit, cmd)
 
     def __mul__(self, qubit):
         """Overwrite * operator to achieve quantum logic gate operation, \
             reuse __or__ operator implement."""
         self.__or__(qubit)
 
@@ -81,15 +82,19 @@
         Args:
             ctrl_cnt: The number of control qubits, default: 1.
         """
         gate = MCZ(ctrl_cnt)
         gate.is_inverse = self.is_inverse
         return gate
 
+    def condition(self, qubit, cond_value):
+        self.measurecond = MeasureCond(True, qubit.index, cond_value)
+        return self
 
+     
 PauliZ = Z = ZGate()
 
 
 class MCZ(BasicGate):
     """Multi-control Z gate.
 
     Args:
```

### Comparing `qutrunk-0.2.1/qutrunk/circuit/gates/z1.py` & `qutrunk-0.2.2/qutrunk/circuit/gates/z1.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/ops/addition.py` & `qutrunk-0.2.2/qutrunk/circuit/ops/addition.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/ops/amp.py` & `qutrunk-0.2.2/qutrunk/circuit/ops/amp.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/ops/classical.py` & `qutrunk-0.2.2/qutrunk/circuit/ops/classical.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/ops/decrement.py` & `qutrunk-0.2.2/qutrunk/circuit/ops/decrement.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/ops/increment.py` & `qutrunk-0.2.2/qutrunk/circuit/ops/increment.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/ops/plus.py` & `qutrunk-0.2.2/qutrunk/circuit/ops/plus.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/ops/qaa.py` & `qutrunk-0.2.2/qutrunk/circuit/ops/qaa.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/ops/qft.py` & `qutrunk-0.2.2/qutrunk/circuit/ops/qft.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/ops/qpe.py` & `qutrunk-0.2.2/qutrunk/circuit/ops/qpe.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/parameter.py` & `qutrunk-0.2.2/qutrunk/circuit/parameter.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         obj._hash = hash(obj._uuid)
 
         return obj
 
     def __init__(self, name):
         self.name = name
         self.value = None
-        self._host = None
+        self._hosts = []
 
     def __copy__(self):
         return self
 
     def __deepcopy__(self, memo=None):
         return self
 
@@ -48,30 +48,30 @@
     def __str__(self):
         return self.name
 
     def __repr__(self):
         return f"{self.__class__.__name__}({self.name})"
 
     @property
-    def host(self):
+    def hosts(self):
         """Get parameter host."""
-        return self._host
+        return self._hosts
 
-    @host.setter
-    def host(self, host):
+    @hosts.setter
+    def hosts(self, hosts):
         """Set parameter host.
-        
+
         Args:
-            host: The Host using this parameter. 
+            hosts: The Host using this parameter.
         """
-        self._host = host
+        self._hosts = hosts
 
     def update(self, value):
         """Update parameter value.
         
         Args:
             value: Parameter value.
         """
         self.value = value
-        if self._host:
-            self._host.update_parameter(self)
-
+        if self._hosts:
+            for host in self._hosts:
+                host.update_parameter(self)
```

### Comparing `qutrunk-0.2.1/qutrunk/circuit/qubit.py` & `qutrunk-0.2.2/qutrunk/circuit/qubit.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/circuit/qureg.py` & `qutrunk-0.2.2/qutrunk/circuit/qureg.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/converters/ast_to_dag.py` & `qutrunk-0.2.2/qutrunk/converters/ast_to_dag.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/converters/circuit_to_dag.py` & `qutrunk-0.2.2/qutrunk/converters/circuit_to_dag.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/converters/dag_to_circuit.py` & `qutrunk-0.2.2/qutrunk/converters/dag_to_circuit.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/converters/mapping.py` & `qutrunk-0.2.2/qutrunk/converters/mapping.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/dagcircuit/dagcircuit.py` & `qutrunk-0.2.2/qutrunk/dagcircuit/dagcircuit.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/dagcircuit/dagnode.py` & `qutrunk-0.2.2/qutrunk/dagcircuit/dagnode.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/example/bell_pair.py` & `qutrunk-0.2.2/qutrunk/example/bell_pair.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/example/bernstein_vazirani.py` & `qutrunk-0.2.2/qutrunk/example/bernstein_vazirani.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/example/deutsch.py` & `qutrunk-0.2.2/qutrunk/example/deutsch.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/example/ghz.py` & `qutrunk-0.2.2/qutrunk/example/ghz.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/example/grover.py` & `qutrunk-0.2.2/qutrunk/example/grover.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/example/grover_distribute.py` & `qutrunk-0.2.2/qutrunk/example/grover_distribute.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/example/grover_gpu.py` & `qutrunk-0.2.2/qutrunk/example/grover_gpu.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/example/jupyter/algorithm.ipynb` & `qutrunk-0.2.2/qutrunk/example/jupyter/algorithm.ipynb`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/example/jupyter/awslocal_qrng.ipynb` & `qutrunk-0.2.2/qutrunk/example/jupyter/awslocal_qrng.ipynb`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/example/jupyter/backend.ipynb` & `qutrunk-0.2.2/qutrunk/example/jupyter/backend.ipynb`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/example/jupyter/circuit.ipynb` & `qutrunk-0.2.2/qutrunk/example/jupyter/circuit.ipynb`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/example/jupyter/gate.ipynb` & `qutrunk-0.2.2/qutrunk/example/jupyter/gate.ipynb`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -1316,8 +1316,8 @@
 00005230: 6165 6538 6237 6232 3436 6466 3866 3930  aee8b7b246df8f90
 00005240: 3339 6166 6234 3134 3461 3166 3666 6438  39afb4144a1f6fd8
 00005250: 6432 6361 3137 6131 3830 3738 3662 3639  d2ca17a180786b69
 00005260: 6163 6331 3430 6432 3832 6237 3161 3439  acc140d282b71a49
 00005270: 220d 0a20 2020 7d0d 0a20 207d 0d0a 207d  "..   }..  }.. }
 00005280: 2c0d 0a20 226e 6266 6f72 6d61 7422 3a20  ,.. "nbformat": 
 00005290: 342c 0d0a 2022 6e62 666f 726d 6174 5f6d  4,.. "nbformat_m
-000052a0: 696e 6f72 223a 2032 0d0a 7d              inor": 2..}
+000052a0: 696e 6f72 223a 2032 0d0a 7d0d 0a         inor": 2..}..
```

### Comparing `qutrunk-0.2.1/qutrunk/example/jupyter/ops.ipynb` & `qutrunk-0.2.2/qutrunk/example/jupyter/ops.ipynb`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/example/jupyter/qutrunk_mindspore.ipynb` & `qutrunk-0.2.2/qutrunk/example/jupyter/qutrunk_mindspore.ipynb`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/example/jupyter/qutrunk_paddle.ipynb` & `qutrunk-0.2.2/qutrunk/example/jupyter/qutrunk_paddle.ipynb`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/example/jupyter/qutrunk_pytorch.ipynb` & `qutrunk-0.2.2/qutrunk/example/jupyter/qutrunk_pytorch.ipynb`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/example/jupyter/qutrunk_tensorflow.ipynb` & `qutrunk-0.2.2/qutrunk/example/jupyter/qutrunk_tensorflow.ipynb`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/example/phase_estimation.py` & `qutrunk-0.2.2/qutrunk/example/phase_estimation.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/example/phase_kickback.py` & `qutrunk-0.2.2/qutrunk/example/phase_kickback.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/example/superdense.py` & `qutrunk-0.2.2/qutrunk/example/superdense.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/libs/qelib1.inc` & `qutrunk-0.2.2/qutrunk/qasm/libs/qelib1.inc`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/libs/qulib1.inc` & `qutrunk-0.2.2/qutrunk/qasm/libs/qulib1.inc`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/libs/stdgates.inc` & `qutrunk-0.2.2/qutrunk/qasm/libs/stdgates.inc`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/node/__init__.py` & `qutrunk-0.2.2/qutrunk/qasm/node/__init__.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/node/barrier.py` & `qutrunk-0.2.2/qutrunk/qasm/node/barrier.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/node/binaryop.py` & `qutrunk-0.2.2/qutrunk/qasm/node/binaryop.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/node/binaryoperator.py` & `qutrunk-0.2.2/qutrunk/qasm/node/binaryoperator.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/node/cnot.py` & `qutrunk-0.2.2/qutrunk/qasm/node/cnot.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/node/creg.py` & `qutrunk-0.2.2/qutrunk/qasm/node/creg.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/node/customunitary.py` & `qutrunk-0.2.2/qutrunk/qasm/node/customunitary.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/node/expressionlist.py` & `qutrunk-0.2.2/qutrunk/qasm/node/expressionlist.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/node/external.py` & `qutrunk-0.2.2/qutrunk/qasm/node/external.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/node/format.py` & `qutrunk-0.2.2/qutrunk/qasm/node/format.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/node/gate.py` & `qutrunk-0.2.2/qutrunk/qasm/node/gate.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/node/gatebody.py` & `qutrunk-0.2.2/qutrunk/qasm/node/gatebody.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/node/id.py` & `qutrunk-0.2.2/qutrunk/qasm/node/id.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/node/idlist.py` & `qutrunk-0.2.2/qutrunk/qasm/node/idlist.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/node/if_.py` & `qutrunk-0.2.2/qutrunk/qasm/node/if_.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/node/indexedid.py` & `qutrunk-0.2.2/qutrunk/qasm/node/indexedid.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/node/intnode.py` & `qutrunk-0.2.2/qutrunk/qasm/node/intnode.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/node/measure.py` & `qutrunk-0.2.2/qutrunk/qasm/node/measure.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/node/node.py` & `qutrunk-0.2.2/qutrunk/qasm/node/node.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/node/nodeexception.py` & `qutrunk-0.2.2/qutrunk/qasm/node/nodeexception.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/node/opaque.py` & `qutrunk-0.2.2/qutrunk/qasm/node/opaque.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/node/prefix.py` & `qutrunk-0.2.2/qutrunk/qasm/node/prefix.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/node/primarylist.py` & `qutrunk-0.2.2/qutrunk/qasm/node/primarylist.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/node/program.py` & `qutrunk-0.2.2/qutrunk/qasm/node/program.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/node/qreg.py` & `qutrunk-0.2.2/qutrunk/qasm/node/qreg.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/node/real.py` & `qutrunk-0.2.2/qutrunk/qasm/node/real.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/node/reset.py` & `qutrunk-0.2.2/qutrunk/qasm/node/reset.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/node/unaryoperator.py` & `qutrunk-0.2.2/qutrunk/qasm/node/unaryoperator.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/node/universalunitary.py` & `qutrunk-0.2.2/qutrunk/qasm/node/universalunitary.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/qasm.py` & `qutrunk-0.2.2/qutrunk/qasm/qasm.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/qasmlexer.py` & `qutrunk-0.2.2/qutrunk/qasm/qasmlexer.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/qasm/qasmparser.py` & `qutrunk-0.2.2/qutrunk/qasm/qasmparser.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/thrift/code/constants.py` & `qutrunk-0.2.2/qutrunk/thrift/code/constants.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/thrift/code/ttypes.py` & `qutrunk-0.2.2/qutrunk/thrift/code/ttypes.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/thrift/idl/ecode.thrift` & `qutrunk-0.2.2/qutrunk/thrift/idl/ecode.thrift`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/thrift/idl/gen_py.sh` & `qutrunk-0.2.2/qutrunk/thrift/idl/gen_py.sh`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/thrift/idl/qusprout.thrift` & `qutrunk-0.2.2/qutrunk/thrift/idl/qusprout.thrift`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/thrift/idl/qusproutdata.thrift` & `qutrunk-0.2.2/qutrunk/thrift/idl/qusproutdata.thrift`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,26 @@
 struct Cmdex {
     //振幅数据
     1: optional Amplitude amp
     //矩阵数据
     2: optional Matrix mat
 }
 
+//测量执行条件
+struct MeasureCond {
+    //条件开关
+    1: required bool enable
+
+    //测量的量子比特位
+    2: required i32 idx
+
+    //条件
+    3: required i32 cond_value
+}
+
 //指令数据
 struct Cmd {
     //指令门类型
     1: required string gate
 
     //目标集
     2: required list<i32> targets
@@ -70,14 +82,17 @@
     5: required string desc
 
     //是否执行逆操作
     6: required bool inverse
 
     //扩展命令
     7: optional Cmdex cmdex
+
+    //测量执行条件
+    8: optional MeasureCond cond
 }
 
 //指令集
 struct Circuit {
     //指令集
     1: required list<Cmd> cmds
 }
@@ -205,14 +220,17 @@
 //执行任务
 struct RunCircuitReq {
     //任务id
     1: required string id
 
     //运行次数
     2: required i32 shots
+
+    //释放后端
+    3: optional i32 free
 }
 
 struct RunCircuitResp {
     //返回码
     1: required ecode.BaseCode base 
 
     //返回结果
```

### Comparing `qutrunk-0.2.1/qutrunk/thrift/qusprout/QuSproutServer-remote` & `qutrunk-0.2.2/qutrunk/thrift/qusprout/QuSproutServer-remote`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/thrift/qusprout/QuSproutServer.py` & `qutrunk-0.2.2/qutrunk/thrift/qusprout/QuSproutServer.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/thrift/qusprout/ttypes.py` & `qutrunk-0.2.2/qutrunk/thrift/qusprout/ttypes.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/thrift/qusproutdata/ttypes.py` & `qutrunk-0.2.2/qutrunk/thrift/qusproutdata/ttypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -392,36 +392,123 @@
     def __eq__(self, other):
         return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not (self == other)
 
 
+class MeasureCond(object):
+    """
+    Attributes:
+     - enable
+     - idx
+     - cond_value
+
+    """
+
+
+    def __init__(self, enable=None, idx=None, cond_value=None,):
+        self.enable = enable
+        self.idx = idx
+        self.cond_value = cond_value
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.BOOL:
+                    self.enable = iprot.readBool()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.I32:
+                    self.idx = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.I32:
+                    self.cond_value = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('MeasureCond')
+        if self.enable is not None:
+            oprot.writeFieldBegin('enable', TType.BOOL, 1)
+            oprot.writeBool(self.enable)
+            oprot.writeFieldEnd()
+        if self.idx is not None:
+            oprot.writeFieldBegin('idx', TType.I32, 2)
+            oprot.writeI32(self.idx)
+            oprot.writeFieldEnd()
+        if self.cond_value is not None:
+            oprot.writeFieldBegin('cond_value', TType.I32, 3)
+            oprot.writeI32(self.cond_value)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        if self.enable is None:
+            raise TProtocolException(message='Required field enable is unset!')
+        if self.idx is None:
+            raise TProtocolException(message='Required field idx is unset!')
+        if self.cond_value is None:
+            raise TProtocolException(message='Required field cond_value is unset!')
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, value)
+             for key, value in self.__dict__.items()]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
 class Cmd(object):
     """
     Attributes:
      - gate
      - targets
      - controls
      - rotation
      - desc
      - inverse
      - cmdex
+     - cond
 
     """
 
 
-    def __init__(self, gate=None, targets=None, controls=None, rotation=None, desc=None, inverse=None, cmdex=None,):
+    def __init__(self, gate=None, targets=None, controls=None, rotation=None, desc=None, inverse=None, cmdex=None, cond=None,):
         self.gate = gate
         self.targets = targets
         self.controls = controls
         self.rotation = rotation
         self.desc = desc
         self.inverse = inverse
         self.cmdex = cmdex
+        self.cond = cond
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
         iprot.readStructBegin()
         while True:
@@ -475,14 +562,20 @@
                     iprot.skip(ftype)
             elif fid == 7:
                 if ftype == TType.STRUCT:
                     self.cmdex = Cmdex()
                     self.cmdex.read(iprot)
                 else:
                     iprot.skip(ftype)
+            elif fid == 8:
+                if ftype == TType.STRUCT:
+                    self.cond = MeasureCond()
+                    self.cond.read(iprot)
+                else:
+                    iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
@@ -522,14 +615,18 @@
             oprot.writeFieldBegin('inverse', TType.BOOL, 6)
             oprot.writeBool(self.inverse)
             oprot.writeFieldEnd()
         if self.cmdex is not None:
             oprot.writeFieldBegin('cmdex', TType.STRUCT, 7)
             self.cmdex.write(oprot)
             oprot.writeFieldEnd()
+        if self.cond is not None:
+            oprot.writeFieldBegin('cond', TType.STRUCT, 8)
+            self.cond.write(oprot)
+            oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.gate is None:
             raise TProtocolException(message='Required field gate is unset!')
         if self.targets is None:
@@ -1707,21 +1804,23 @@
 
 
 class RunCircuitReq(object):
     """
     Attributes:
      - id
      - shots
+     - free
 
     """
 
 
-    def __init__(self, id=None, shots=None,):
+    def __init__(self, id=None, shots=None, free=None,):
         self.id = id
         self.shots = shots
+        self.free = free
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
         iprot.readStructBegin()
         while True:
@@ -1734,14 +1833,19 @@
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.I32:
                     self.shots = iprot.readI32()
                 else:
                     iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.I32:
+                    self.free = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
@@ -1752,14 +1856,18 @@
             oprot.writeFieldBegin('id', TType.STRING, 1)
             oprot.writeString(self.id.encode('utf-8') if sys.version_info[0] == 2 else self.id)
             oprot.writeFieldEnd()
         if self.shots is not None:
             oprot.writeFieldBegin('shots', TType.I32, 2)
             oprot.writeI32(self.shots)
             oprot.writeFieldEnd()
+        if self.free is not None:
+            oprot.writeFieldBegin('free', TType.I32, 3)
+            oprot.writeI32(self.free)
+            oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.id is None:
             raise TProtocolException(message='Required field id is unset!')
         if self.shots is None:
@@ -2848,24 +2956,32 @@
 )
 all_structs.append(Cmdex)
 Cmdex.thrift_spec = (
     None,  # 0
     (1, TType.STRUCT, 'amp', [Amplitude, None], None, ),  # 1
     (2, TType.STRUCT, 'mat', [Matrix, None], None, ),  # 2
 )
+all_structs.append(MeasureCond)
+MeasureCond.thrift_spec = (
+    None,  # 0
+    (1, TType.BOOL, 'enable', None, None, ),  # 1
+    (2, TType.I32, 'idx', None, None, ),  # 2
+    (3, TType.I32, 'cond_value', None, None, ),  # 3
+)
 all_structs.append(Cmd)
 Cmd.thrift_spec = (
     None,  # 0
     (1, TType.STRING, 'gate', 'UTF8', None, ),  # 1
     (2, TType.LIST, 'targets', (TType.I32, None, False), None, ),  # 2
     (3, TType.LIST, 'controls', (TType.I32, None, False), None, ),  # 3
     (4, TType.LIST, 'rotation', (TType.DOUBLE, None, False), None, ),  # 4
     (5, TType.STRING, 'desc', 'UTF8', None, ),  # 5
     (6, TType.BOOL, 'inverse', None, None, ),  # 6
     (7, TType.STRUCT, 'cmdex', [Cmdex, None], None, ),  # 7
+    (8, TType.STRUCT, 'cond', [MeasureCond, None], None, ),  # 8
 )
 all_structs.append(Circuit)
 Circuit.thrift_spec = (
     None,  # 0
     (1, TType.LIST, 'cmds', (TType.STRUCT, [Cmd, None], False), None, ),  # 1
 )
 all_structs.append(MeasureQubit)
```

### Comparing `qutrunk-0.2.1/qutrunk/tools/algorithm.py` & `qutrunk-0.2.2/qutrunk/tools/algorithm.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/tools/check.py` & `qutrunk-0.2.2/qutrunk/tools/check.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/tools/check_sprout.py` & `qutrunk-0.2.2/qutrunk/tools/check_sprout.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/tools/env_reader.py` & `qutrunk-0.2.2/qutrunk/tools/env_reader.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/tools/produce_algorithm.py` & `qutrunk-0.2.2/qutrunk/tools/produce_algorithm.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/tools/qusl_parse.py` & `qutrunk-0.2.2/qutrunk/tools/qusl_parse.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/tools/random_circuit.py` & `qutrunk-0.2.2/qutrunk/tools/random_circuit.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/tools/set_config.py` & `qutrunk-0.2.2/qutrunk/tools/set_config.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/visualizations/circuit_visualization.py` & `qutrunk-0.2.2/qutrunk/visualizations/circuit_visualization.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/visualizations/layer.py` & `qutrunk-0.2.2/qutrunk/visualizations/layer.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/visualizations/text.py` & `qutrunk-0.2.2/qutrunk/visualizations/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,14 +204,19 @@
         """
         # implement h, cx, measure gate
         op = node.op  # Command object
         current_cons = []
         connection_label = None
         # condition control
         conditional = False
+        
+        condstr = ""
+        cond = op.measurecond
+        if cond and cond.enable == True:
+            condstr = "(q[" + str(cond.idx) + "]==" + str(cond.cond_value) + ")"
 
         def add_connected_gate(node, gates, layer, current_cons):
             for i, gate in enumerate(gates):
                 actual_index = self.qubits.index(node.qargs[i])
                 if actual_index not in [i for i, j in current_cons]:
                     layer.set_qubit(node.qargs[i], gate)
                     current_cons.append((actual_index, gate))
@@ -265,15 +270,15 @@
             gates = self.set_ctrl_state(
                 node, conditional, ctrl_text, bool(controlled_bot)
             )
             gates.append(BoxOnQuWire("Toffoli", conditional=conditional))
             add_connected_gate(node, gates, layer, current_cons)
         # X gate
         elif isinstance(op.gate, XGate):
-            layer.set_qubit(node.qargs[0], BoxOnQuWire("X", conditional=conditional))
+            layer.set_qubit(node.qargs[0], BoxOnQuWire("X"+condstr, conditional=conditional))
         # BarrierGate gate
         elif isinstance(op.gate, BarrierGate):
             for qubit in node.qargs:
                 if qubit in self.qubits:
                     layer.set_qubit(qubit, BarrierBox())
         # CZ gate
         elif isinstance(op.gate, MCZ):
@@ -296,15 +301,15 @@
                 node, conditional, ctrl_text, bool(controlled_bot)
             )
             gates.append(BoxOnQuWire("MCX", conditional=conditional))
             add_connected_gate(node, gates, layer, current_cons)
         elif isinstance(op.gate, P):
             layer.set_qubit(node.qargs[0], BoxOnQuWire("P", conditional=conditional))
         elif isinstance(op.gate, ZGate):
-            layer.set_qubit(node.qargs[0], BoxOnQuWire("Z", conditional=conditional))
+            layer.set_qubit(node.qargs[0], BoxOnQuWire("Z"+condstr, conditional=conditional))
         elif isinstance(op.gate, R):
             label = f"R({op.gate.theta:.2},{op.gate.phi:.2})"
             layer.set_qubit(node.qargs[0], BoxOnQuWire(label, conditional=conditional))
         elif isinstance(op.gate, Rx):
             layer.set_qubit(node.qargs[0], BoxOnQuWire("Rx", conditional=conditional))
         elif isinstance(op.gate, Ry):
             layer.set_qubit(node.qargs[0], BoxOnQuWire("Ry", conditional=conditional))
```

### Comparing `qutrunk-0.2.1/qutrunk/visualizations/text_draw_element.py` & `qutrunk-0.2.2/qutrunk/visualizations/text_draw_element.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/qutrunk/visualizations/utils.py` & `qutrunk-0.2.2/qutrunk/visualizations/utils.py`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/README.md` & `qutrunk-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `qutrunk-0.2.1/setup.py` & `qutrunk-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 extras_require = \
 {'braket': ['amazon-braket-sdk>=1.32.0,<2.0.0'],
  'gpu': ['numba>=0.56.4,<0.57.0'],
  'parallel': ['mpi4py>=3.1.4,<4.0.0']}
 
 setup_kwargs = {
     'name': 'qutrunk',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'qutrunk is an open source library for quantum computing.',
     'long_description': '## QuTrunk\n\n[![Documentation Status](https://img.shields.io/badge/docs-latest-brightgreen.svg)](http://developer.queco.cn/qutrunk_api/)\n[![License](https://img.shields.io/badge/license-Apache%202-blue.svg)](LICENSE)\n[![Download Code](https://img.shields.io/badge/download-zip-green.svg)](https://github.com/queco-quantum/qutrunk/archive/refs/heads/main.zip)\n\n\n### **概述**\n---\n* QuTrunk 是启科量子自主研发的一款免费、开源、跨平台的量子计算编程框架，包括量子编程API、量子命令转译、量子计算后端接口等。\n* QuTrunk 使用 Python 作为宿主语言，利用 Python 的语法特性实现针对量子程序的 DSL (领域专用语言)，所有使用 Python 编程的 IDE 均可使用安装。\n* QuTrunk 基于量子逻辑门、量子线路等概念提供量子编程所需各类 API，这些 API 由相应的模块实现。例如 QCircuit 实现量子线路，Qubit 实现量子比特，Qureg 实现量子寄存器，Command 实现每个量子门操作的指令，Backend 实现运行量子线路的后端模块，gate 模块实现各类基础量子门操作。\n* QuTrunk 还可以作为其他上层量子计算应用的基础，例如：量子算法、量子可视化编程、量子机器学习等。\n\nQuTrunk内部模块划分及层次结构如下：  \n\n<div align=center>\n<img src="http://developer.queco.cn/media/images/qutrunkTuPian.original.png"/>\n</div>\n\n\n### **核心模块**\n---\n* cicuit: 量子线路，通过应用各类基础门操作以及算符操作构建量子线路，代表了整个量子算法的实现。\n* qubit: 代表单个量子比特，是量子门和量子算符操作的目标对象。\n* qureg: 用于申请量子计算资源，维护若干个量子比特，用于实现某个具体的量子算法。\n* gate: 量子逻辑门模块，提供各类基础量子门操作，包括:*H*, *X*, *Y*, *Z*，*P*, *R*, *Rx*, *Ry*, *Rz*, *S*, *Sdg*, *T*, *Tdg*, *CNOT*, *Toffoli*, *Swap*等。\n* operator: 量子算符操作，通过若干基础量子门实现某些通用量子操作，比如振幅放大QAA, 量子傅立叶变换QFT等。\n* command: 对量子线路中所有门级操作做参数化处理，对接目标后端模块，用于运行整个量子线路。\n* qasm: 兼容OpenQASM 2.0标准，实现量子线路到OpenQASM指令的序列化和反序列化。\n* qusl: QuTrunk量子汇编标准，实现与qasm类似功能。\n* backend: 量子计算后端模块，用于执行量子线路，支持Python本地后端，qusprout和qusaas两种远程后端以及第三方后端(目前支持IBM和AWS Braket)。\n* qusprout: 对接启科研制的qubox设备，使用经典计算资源并针对量子计算特点做优化，提供高性能量子模拟计算服务。\n* qusaas: 对接启科量子计算云平台，接入多种量子计算资源，包括经典计算资源，离子阱量子计算机（研发中）。\n\n\n### 主要特点\n---\n* 基于量子逻辑门、量子算符和量子线路实现量子程序开发。\n* 提供QuSL量子汇编指令标准，QuSL量子汇编与Python代码完全兼容。\n* 设备独立，同一个量子线路只需替换后端类型即可以在不同的量子后端上运行。\n* 提供多种量子计算体验，本地量子计算提供Python计算后端，远程后端提供OMP多线程、MPI多节点并行、GPU加速等计算模式，同时预留了接口对接启科量子自行研制的离子阱量子计算机。\n* 兼容多种量子汇编指令格式：OpenQASM 2.0标准和QuSL汇编标准。\n* 支持量子可视化编程（需要配合启科量子研发的量子集成开发环境 QuBranch）。\n\n\n### **下载和安装**\n---\n#### **pip安装** \n\nQuTrunk 已发布于 PyPI 官网，可以通过 pip 命令进行安装。\n注意在正式使用 QuTurnk 之前，您需要先安装 Python（版本 3.8+）。\n\n  ```shell\n  pip install qutrunk\n  \n  # 可选安装：braket——支持AWS Braket作为量子计算后端\n  pip install \'qutrunk[braket]\'\n\n  # 可选安装：parallel——支持多节点并行计算\n  pip install \'qutrunk[parallel]\'\n\n  # 可选安装：gpu——支持gpu计算加速(目前支持到：cuda 11)\n  pip install \'qutrunk[gpu]\'\n  ```\n\n验证QuTrunk是否安装成功，打开终端进入python交互模式，执行如下语句：\n\n``` python\nimport qutrunk\nqutrunk.run_check()\n```\n输出结果为："QuTrunk is installed successfully! You can use QuTrunk now."表明QuTrunk安装成功。\n\n\n### **示例代码**\n---\n以下示例展示了利用 QuTrunk 运行 bell-pair 量子算法：\n\n  ```python\n  # import package\n  from qutrunk.circuit import QCircuit\n  from qutrunk.circuit.gates import H, CNOT, Measure, All\n\n  # allocate resource\n  qc = QCircuit()\n  qr = qc.allocate(2) \n\n  # apply quantum gates\n  H * qr[0]   \n  CNOT * (qr[0], qr[1])\n  All(Measure) * qr\n\n  # print circuit\n  qc.print()   \n  # run circuit\n  res = qc.run(shots=1024) \n  # print result\n  print(res.get_counts()) \n  # draw circuit\n  qc.draw()\n  ```\n\n运行结果：\n<div>\n<img src="http://developer.queco.cn/media/images/bell_pairYunXingJieGuo.original.png"/>\n</div>\n\n### **量子可视化编程**  \n---\nQuBranch是由启科量子基于vscode开发的量子编程集成开发环境, QuTrunk与QuBranch相互配合可以实现量子可视化编程,\n具体步骤参见[量子可视化编程](http://developer.queco.cn/learn/doc/detail?id=12&childrenid=14)\n\n### **文档**\n---\n* [QuTrunk 快速上手教程](http://developer.queco.cn/learn/doc/detail?id=12&childrenid=14)\n* [QuTrunk API](http://developer.queco.cn/qutrunk_api/)\n\n\n### **如何参与开发**\n---\n1. 阅读源代码，了解我们当前的开发方向\n2. 找到自己感兴趣的功能或模块\n3. 进行开发，开发完成后自测功能是否正确\n4. Fork代码库，将修复代码提交到fork的代码库\n5. 发起pull request\n6. 更多详情请参见[链接](./CONTRIBUTING.md)\n\n\n### **许可证**\n---\nQuTrunk是自由和开源的，在Apache 2.0许可证版本下发布。\n',
     'author': 'qudoorzh2022',
     'author_email': 'qudoorzh2022@163.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'http://www.qudoor.com/',
```

### Comparing `qutrunk-0.2.1/PKG-INFO` & `qutrunk-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qutrunk
-Version: 0.2.1
+Version: 0.2.2
 Summary: qutrunk is an open source library for quantum computing.
 Home-page: http://www.qudoor.com/
 License: Apache-2.0
 Keywords: qutrunk,quantum,sdk
 Author: qudoorzh2022
 Author-email: qudoorzh2022@163.com
 Requires-Python: >=3.8,<3.11
```

