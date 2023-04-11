# Comparing `tmp/gym_saturation-0.9.1.tar.gz` & `tmp/gym_saturation-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym_saturation-0.9.1.tar", max compression
+gzip compressed data, was "gym_saturation-0.9.2.tar", max compression
```

## Comparing `gym_saturation-0.9.1.tar` & `gym_saturation-0.9.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11360 2022-09-19 19:58:15.552724 gym_saturation-0.9.1/LICENSE
--rw-r--r--   0        0        0     6058 2023-04-06 15:52:02.939733 gym_saturation-0.9.1/README.rst
--rw-r--r--   0        0        0      991 2023-04-06 15:52:02.955734 gym_saturation-0.9.1/gym_saturation/__init__.py
--rw-r--r--   0        0        0     8632 2023-04-04 11:04:37.019214 gym_saturation-0.9.1/gym_saturation/agent_testing.py
--rw-r--r--   0        0        0     1242 2023-04-04 11:04:37.023214 gym_saturation-0.9.1/gym_saturation/conftest.py
--rw-r--r--   0        0        0      770 2023-04-06 15:52:02.959734 gym_saturation-0.9.1/gym_saturation/constants.py
--rw-r--r--   0        0        0     1168 2023-03-24 12:49:21.170500 gym_saturation-0.9.1/gym_saturation/dummy_http_handler.py
--rw-r--r--   0        0        0      789 2023-01-08 12:44:28.449376 gym_saturation-0.9.1/gym_saturation/envs/__init__.py
--rw-r--r--   0        0        0     8097 2023-04-06 15:52:02.959734 gym_saturation-0.9.1/gym_saturation/envs/iprover_env.py
--rw-r--r--   0        0        0     7488 2023-04-06 15:52:02.959734 gym_saturation-0.9.1/gym_saturation/envs/saturation_env.py
--rw-r--r--   0        0        0     5548 2023-04-04 11:04:37.023214 gym_saturation-0.9.1/gym_saturation/envs/vampire_env.py
--rw-r--r--   0        0        0     2244 2023-03-01 16:21:18.184137 gym_saturation-0.9.1/gym_saturation/proof_state.py
--rw-r--r--   0        0        0        0 2021-07-22 09:53:47.848012 gym_saturation-0.9.1/gym_saturation/py.typed
--rw-r--r--   0        0        0     3570 2023-02-25 20:38:38.888596 gym_saturation-0.9.1/gym_saturation/relay_server.py
--rw-r--r--   0        0        0      267 2023-04-04 11:04:37.027214 gym_saturation-0.9.1/gym_saturation/resources/TPTP-mock/Problems/TST/TST001-1.p
--rw-r--r--   0        0        0       77 2023-04-04 11:04:37.027214 gym_saturation-0.9.1/gym_saturation/resources/TPTP-mock/Problems/TST/TST002-1.p
--rwxr-xr-x   0        0        0       62 2022-11-07 08:44:37.735015 gym_saturation-0.9.1/gym_saturation/resources/vampire-mock
--rw-r--r--   0        0        0     4099 2023-04-05 14:12:19.638325 gym_saturation-0.9.1/gym_saturation/utils.py
--rw-r--r--   0        0        0     4068 2023-04-04 11:04:37.031214 gym_saturation-0.9.1/gym_saturation/vampire_wrapper.py
--rw-r--r--   0        0        0     2570 2023-04-04 11:04:37.031214 gym_saturation-0.9.1/gym_saturation/wrappers/age_weight_bandit.py
--rw-r--r--   0        0        0     2641 2023-04-04 11:04:37.035214 gym_saturation-0.9.1/gym_saturation/wrappers/ast2vec_wrapper.py
--rw-r--r--   0        0        0     2395 2023-04-06 15:52:02.959734 gym_saturation-0.9.1/gym_saturation/wrappers/constant_parametric_actions.py
--rw-r--r--   0        0        0     2221 2023-04-04 11:04:37.035214 gym_saturation-0.9.1/gym_saturation/wrappers/duplicate_key_obs.py
--rw-r--r--   0        0        0     5435 2023-04-06 15:52:02.963734 gym_saturation-0.9.1/gym_saturation/wrappers/parametric_actions_wrapper.py
--rw-r--r--   0        0        0     3457 2023-04-06 15:52:02.963734 gym_saturation-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     7324 1970-01-01 00:00:00.000000 gym_saturation-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    11360 2022-09-19 19:58:15.552724 gym_saturation-0.9.2/LICENSE
+-rw-r--r--   0        0        0     6285 2023-04-11 17:02:37.334496 gym_saturation-0.9.2/README.rst
+-rw-r--r--   0        0        0      991 2023-04-11 17:02:37.366490 gym_saturation-0.9.2/gym_saturation/__init__.py
+-rw-r--r--   0        0        0     8636 2023-04-11 17:02:37.366490 gym_saturation-0.9.2/gym_saturation/agent_testing.py
+-rw-r--r--   0        0        0     1242 2023-04-04 11:04:37.023214 gym_saturation-0.9.2/gym_saturation/conftest.py
+-rw-r--r--   0        0        0     1296 2023-04-11 17:02:37.370489 gym_saturation-0.9.2/gym_saturation/constants.py
+-rw-r--r--   0        0        0     1168 2023-03-24 12:49:21.170500 gym_saturation-0.9.2/gym_saturation/dummy_http_handler.py
+-rw-r--r--   0        0        0      789 2023-01-08 12:44:28.449376 gym_saturation-0.9.2/gym_saturation/envs/__init__.py
+-rw-r--r--   0        0        0     7506 2023-04-11 17:02:37.370489 gym_saturation-0.9.2/gym_saturation/envs/iprover_env.py
+-rw-r--r--   0        0        0     7230 2023-04-11 17:02:37.374488 gym_saturation-0.9.2/gym_saturation/envs/saturation_env.py
+-rw-r--r--   0        0        0     5401 2023-04-11 17:02:37.378488 gym_saturation-0.9.2/gym_saturation/envs/vampire_env.py
+-rw-r--r--   0        0        0     2795 2023-04-11 17:02:37.378488 gym_saturation-0.9.2/gym_saturation/proof_state.py
+-rw-r--r--   0        0        0        0 2021-07-22 09:53:47.848012 gym_saturation-0.9.2/gym_saturation/py.typed
+-rw-r--r--   0        0        0     3893 2023-04-11 17:02:37.382487 gym_saturation-0.9.2/gym_saturation/relay_server.py
+-rw-r--r--   0        0        0      267 2023-04-04 11:04:37.027214 gym_saturation-0.9.2/gym_saturation/resources/TPTP-mock/Problems/TST/TST001-1.p
+-rw-r--r--   0        0        0       77 2023-04-04 11:04:37.027214 gym_saturation-0.9.2/gym_saturation/resources/TPTP-mock/Problems/TST/TST002-1.p
+-rwxr-xr-x   0        0        0       62 2022-11-07 08:44:37.735015 gym_saturation-0.9.2/gym_saturation/resources/vampire-mock
+-rw-r--r--   0        0        0     3647 2023-04-11 17:02:37.382487 gym_saturation-0.9.2/gym_saturation/utils.py
+-rw-r--r--   0        0        0     4086 2023-04-11 17:02:37.382487 gym_saturation-0.9.2/gym_saturation/vampire_wrapper.py
+-rw-r--r--   0        0        0     2570 2023-04-04 11:04:37.031214 gym_saturation-0.9.2/gym_saturation/wrappers/age_weight_bandit.py
+-rw-r--r--   0        0        0     2641 2023-04-04 11:04:37.035214 gym_saturation-0.9.2/gym_saturation/wrappers/ast2vec_wrapper.py
+-rw-r--r--   0        0        0     2395 2023-04-06 15:52:02.959734 gym_saturation-0.9.2/gym_saturation/wrappers/constant_parametric_actions.py
+-rw-r--r--   0        0        0     2221 2023-04-04 11:04:37.035214 gym_saturation-0.9.2/gym_saturation/wrappers/duplicate_key_obs.py
+-rw-r--r--   0        0        0     5435 2023-04-06 15:52:02.963734 gym_saturation-0.9.2/gym_saturation/wrappers/parametric_actions_wrapper.py
+-rw-r--r--   0        0        0     3458 2023-04-11 17:02:37.386486 gym_saturation-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     7551 1970-01-01 00:00:00.000000 gym_saturation-0.9.2/PKG-INFO
```

### Comparing `gym_saturation-0.9.1/LICENSE` & `gym_saturation-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gym_saturation-0.9.1/README.rst` & `gym_saturation-0.9.2/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -20,16 +20,15 @@
 
 ``gym-saturation`` is a collection of `Gymnasium
 <https://gymnasium.farama.org/>`__ environments for reinforcement learning
 (RL) agents striving to prove theorems. Currently, only theorems
 written in `TPTP library <https://tptp.org>`__ formal language are
 supported.
 
-There are two environments in ``gym-saturation``: `VampireEnv <https://gym-saturation.readthedocs.io/en/latest/environments/vampire-env.html#vampire-env>`__ and
-`IProverEnv <https://gym-saturation.readthedocs.io/en/latest/environments/iprover-env.html#iprover-env>`__. ``VampireEnv`` is a wrapper around a recent `Vampire
+There are two environments in ``gym-saturation`` following the same API: `SaturationEnv <https://gym-saturation.readthedocs.io/en/latest/environments/saturation-env.html>`__: ``VampireEnv`` is a wrapper around a recent `Vampire
 <https://github.com/vprover/vampire>`__ prover, and ``IProverEnv``
 relies on an experimental version of `iProver
 <https://gitlab.com/korovin/iprover/>`__.
 
 In contrast to monolithic architecture of a typical Automated Theorem
 Prover (ATP), ``gym-saturation`` gives different agents opportunities
 to select clauses themselves and train from their experience.
@@ -45,32 +44,32 @@
 ==============
 
 .. attention:: If you want to use ``VampireEnv`` you should have a
    Vampire binary on your machine. For example, download the
    latest `release
    <https://github.com/vprover/vampire/releases/tag/v4.7>`__.
 
-   To use ``IProverEnv``, please build iProver from source using
-   `this branch
-   <https://gitlab.com/korovin/iprover/-/tree/2022_sockets>`__.
+   To use ``IProverEnv``, please download the experimental iProver 
+   `release
+   <https://gitlab.com/inpefess/iprover/-/releases/2022.11.03>`__ or build it from `this commit <https://gitlab.com/korovin/iprover/-/commit/32c76fc0ec665a06324d11dc9d4bf902871d5f15>`__.
 
 The best way to install this package is to use ``pip``:
 
 .. code:: sh
 
    pip install gym-saturation
 
 Another option is to use ``conda``:
 
 .. code:: sh
 
    conda install -c conda-forge gym-saturation
    
-One can also run it in a Docker container (with a pre-packed
-``vampire`` binary):
+One can also run it in a Docker container (pre-packed with
+``vampire`` and ``iproveropt`` binaries):
 
 .. code:: sh
 
    docker build -t gym-saturation https://github.com/inpefess/gym-saturation.git
    docker run -it --rm -p 8888:8888 gym-saturation jupyter-lab --ip=0.0.0.0 --port=8888
 
 How to use
@@ -90,15 +89,15 @@
   terminated, truncated = False, False
   while not (terminated or truncated):
       # apply policy (a valid random action here)
       action = env.action_space.sample(mask=observation["action_mask"])
       observation, reward, terminated, truncated, info = env.step(action)
   env.close()
 
-Or have a look at the basic `tutorial <https://gym-saturation.readthedocs.io/en/latest/tutorials/auto_examples/plot_age_agent.html>`__.
+Or have a look at the basic `tutorial <https://gym-saturation.readthedocs.io/en/latest/auto_examples/plot_age_agent.html>`__.
   
 For a bit more comprehensive experiments, please navigate the documentation `page <https://gym-saturation.readthedocs.io/en/latest/tutorials/experiments.html>`__.
 
 How to Contribute
 =================
 
 `Pull requests <https://github.com/inpefess/gym-saturation/pulls>`__ are
@@ -110,18 +109,22 @@
    cd gym-saturation
    # activate python virtual environment with Python 3.8+
    pip install -U pip
    pip install -U setuptools wheel poetry
    poetry install
    # recommended but not necessary
    pre-commit install
-   # install vampire binary
+   # install Vampire binary
    wget https://github.com/vprover/vampire/releases/download/v4.7/vampire4.7.zip -O vampire.zip
    unzip vampire.zip
    # then use vampire_z3_rel_static_HEAD_6295 as an argument or add it to $PATH
+   # install iProver binary
+   wget https://gitlab.com/api/v4/projects/39846772/jobs/artifacts/2022.11.03/download?job=build-job -O iprover.zip
+   unzip iprover.zip
+   # then use iproveropt
 
 All the tests in this package are
 `doctests <https://docs.python.org/3/library/doctest.html>`__. One can
 run them with the following command:
 
 .. code:: sh
```

### Comparing `gym_saturation-0.9.1/gym_saturation/__init__.py` & `gym_saturation-0.9.2/gym_saturation/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 They are registered using a limit for the number of steps in an episode and the
 maximal possible reward is set to ``1.0`` (proof is found).
 """
 from gymnasium.envs.registration import register
 
 register(id="Vampire-v0", entry_point="gym_saturation.envs:VampireEnv")
 register(id="iProver-v0", entry_point="gym_saturation.envs:IProverEnv")
-__version__ = "0.9.1"
+__version__ = "0.9.2"
```

### Comparing `gym_saturation-0.9.1/gym_saturation/agent_testing.py` & `gym_saturation-0.9.2/gym_saturation/agent_testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,15 +256,15 @@
         print(f"Proof state size limit reached in {step_count} step(s).")
 
 
 def test_agent(args: Optional[List[str]] = None) -> None:
     """
     The main function for this module.
 
-    >>> from gym_saturation.utils import MOCK_TPTP_PROBLEM
+    >>> from gym_saturation.constants import MOCK_TPTP_PROBLEM
     >>> test_agent(["--problem_filename", MOCK_TPTP_PROBLEM])
     Problem file: ...TST001-1.p
     Proof of length 10 found in 6 step(s):
     ...
     cnf(20, lemma, $false, inference(subsumption_resolution, [], [19, 5])).
     >>> import os
     >>> trivial_problem = os.path.join(os.path.dirname(MOCK_TPTP_PROBLEM),
```

### Comparing `gym_saturation-0.9.1/gym_saturation/conftest.py` & `gym_saturation-0.9.2/gym_saturation/conftest.py`

 * *Files identical despite different names*

### Comparing `gym_saturation-0.9.1/gym_saturation/dummy_http_handler.py` & `gym_saturation-0.9.2/gym_saturation/dummy_http_handler.py`

 * *Files identical despite different names*

### Comparing `gym_saturation-0.9.1/gym_saturation/envs/__init__.py` & `gym_saturation-0.9.2/gym_saturation/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `gym_saturation-0.9.1/gym_saturation/envs/iprover_env.py` & `gym_saturation-0.9.2/gym_saturation/envs/iprover_env.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,35 +13,31 @@
 # limitations under the License.
 
 # noqa: D205, D400
 """
 Saturation Environment with iProver back-end
 ============================================
 """
-import asyncio
 import json
 import os
-import random
 import re
-import socket
 import subprocess
-import time
 from threading import Thread
 from typing import Any, Dict, List, Optional, Tuple
 
 import numpy as np
 
 from gym_saturation.constants import ACTION_MASK, REAL_OBS
 from gym_saturation.envs.saturation_env import MAX_CLAUSES, SaturationEnv
 from gym_saturation.relay_server import RelayServer, RelayTCPHandler
 
 
-async def _iprover_start(
-    iprover_port: int, problem_filename: str, iprover_binary_path: str
-) -> asyncio.subprocess.Process:
+def _iprover_start(
+    iprover_port: int, problem_filename: str, prover_binary_path: str
+) -> subprocess.Popen:
     tptp_folder = os.path.join(os.path.dirname(problem_filename), "..", "..")
     arguments = [
         "--interactive_mode",
         "true",
         "--enigma_ip_address",
         "127.0.0.1",
         "--enigma_port",
@@ -62,69 +58,67 @@
         "external_agent",
         "--preprocessing_flag",
         "false",
         "--include_path",
         tptp_folder,
         problem_filename,
     ]
-    return await asyncio.create_subprocess_exec(
-        iprover_binary_path, *arguments, stdout=subprocess.DEVNULL
+    return subprocess.Popen(
+        [prover_binary_path] + arguments, stdout=subprocess.DEVNULL
     )
 
 
 class IProverEnv(SaturationEnv):
     """
     An RL environment around iProver.
 
-    Refer to :ref:`iprover_env` for more documentation.
+    Refer to :ref:`saturation_env` for more documentation.
 
-    >>> env = IProverEnv()
-    >>> observation, info = env.reset()
-    >>> for action in [0, 1, 2, 3, 4, 6, 9]:
-    ...     observation, reward, terminated, truncated, info = env.step(action)
-    >>> print(reward, terminated, truncated)
-    1.0 True False
-    >>> env.close()
+    >>> from gymnasium.utils.env_checker import check_env
+    >>> import gymnasium as gym
+    >>> env = gym.make(
+    ...     "iProver-v0",
+    ...     max_clauses=5
+    ... ).unwrapped
+    >>> env.relay_server
+    Traceback (most recent call last):
+     ...
+    ValueError: run ``reset`` first!
+    >>> check_env(env)
+    cnf(c_53, ...).
+    ...
+    cnf(c_49, ...).
     """
 
     def __init__(
         self,
         max_clauses: int = MAX_CLAUSES,
         render_mode: str = "human",
-        port_pair: Optional[Tuple[int, int]] = None,
-        iprover_binary_path: str = "iproveropt",
+        prover_binary_path: str = "iproveropt",
     ):
         """
         Initialise the environment.
 
         :param max_clauses: maximal number of clauses in proof state
         :param render_mode: a mode of running ``render`` method
-        :param port_pair: iProver will connect to the first port,
-            a port to listen for agent's connection is the second one
-        :param iprover_binary_path: a path to iProver binary;
+        :param prover_binary_path: a path to iProver binary;
             by default, we assume it to be ``iproveropt`` and in the $PATH
         """
         super().__init__(max_clauses, render_mode)
-        (
-            self.iprover_port,
-            self.agent_port,
-        ) = (  # pylint: disable=unbalanced-tuple-unpacking
-            (
-                random.randint(10000, 2**16 - 1),
-                random.randint(10000, 2**16 - 1),
-            )
-            if port_pair is None
-            else port_pair
-        )
-        self.iprover_binary_path = iprover_binary_path
-        self.relay_server = RelayServer(
-            self.iprover_port, ("localhost", self.agent_port), RelayTCPHandler
-        )
+        self.prover_binary_path = prover_binary_path
+        self._relay_server: Optional[RelayServer] = None
+        self.relay_server_thread: Optional[Thread] = None
+        self.iprover_process: Optional[subprocess.Popen] = None
+
+    def _restart_relay_server(self) -> None:
+        if self._relay_server:
+            self.close()
+        self._relay_server = RelayServer(("localhost", 0), RelayTCPHandler)
         self.relay_server_thread = Thread(
-            target=self.relay_server.serve_forever
+            target=self._relay_server.serve_forever
         )
         self.relay_server_thread.daemon = True
         self.relay_server_thread.start()
 
     def _parse_batch_clauses(
         self, batch_clauses: List[Dict[str, Any]]
     ) -> None:
@@ -168,77 +162,70 @@
     def reset(
         self,
         *,
         seed: Optional[int] = None,
         options: Optional[Dict[str, Any]] = None,
     ) -> Tuple[Dict[str, Any], Dict[str, Any]]:  # noqa: D102
         super().reset(seed=seed)
-        asyncio.run(
-            _iprover_start(
-                self.iprover_port, self.get_task(), self.iprover_binary_path
-            )
+        if self.iprover_process:
+            self.iprover_process.terminate()
+        self._restart_relay_server()
+        self.iprover_process = _iprover_start(
+            self.relay_server.server_address[1],
+            self.get_task(),
+            self.prover_binary_path,
         )
-        time.sleep(2)
         data = self._get_json_data()
         self._parse_iprover_requests(data)
         return {
             REAL_OBS: tuple(self.state.clauses),
             ACTION_MASK: self.state.action_mask,
         }, {}
 
-    def _get_raw_data(self) -> bytes:
-        with socket.create_connection(
-            ("localhost", self.agent_port)
-        ) as tcp_socket:
-            tcp_socket.sendall(b"READ")
-            raw_data = tcp_socket.recv(4096)
-            while b"\x00" not in raw_data[-3:]:
-                raw_data += tcp_socket.recv(4096)
-        return raw_data
-
     def _get_json_data(self) -> List[Dict[str, Any]]:
         json_data = [{"query": "None"}]
         while json_data[-1]["query"] not in {
             "given_clause_request",
             "szs_status",
             "proof_out",
         }:
-            raw_data = self._get_raw_data()
-            raw_jsons = [
-                request.replace("\n", "")
-                for request in raw_data.decode("utf8").split("\x00")
-            ]
-            for raw_json in raw_jsons:
-                if raw_json:
-                    parsed_json = json.loads(
-                        raw_json.replace("\n", "").replace("\x00", "")
-                    )
-                    json_data.append(parsed_json)
+            parsed_json = self.relay_server.input_queue.get()
+            self.relay_server.input_queue.task_done()
+            json_data.append(parsed_json)
         return json_data[1:]
 
     def _parse_iprover_requests(
         self, iprover_requests: List[Dict[str, Any]]
     ) -> None:
         for iprover_request in iprover_requests:
             if "clauses" in iprover_request:
                 self._parse_batch_clauses(iprover_request["clauses"])
 
     def _do_deductions(self, action: np.int64) -> None:
-        given_clause_label = self.state.clause_labels[action][2:]
-        scores = (
-            f"""{{"given_clause": {given_clause_label},"""
-            + """"passive_is_empty": false}\n\x00\n"""
+        iprover_scores_message = {
+            "given_clause": int(self.state.clause_labels[action][2:]),
+            "passive_is_empty": False,
+        }
+        relayed_scores_message = bytes(
+            json.dumps(iprover_scores_message) + "\n\x00\n", "utf8"
         )
-        with socket.create_connection(
-            ("localhost", self.agent_port)
-        ) as tcp_socket:
-            tcp_socket.sendall(scores.encode("utf8"))
+        self.relay_server.output_queue.put(relayed_scores_message)
         data = self._get_json_data()
-        if data:
-            self._parse_iprover_requests(data)
+        self._parse_iprover_requests(data)
 
     def close(self) -> None:
         """Stop relay server."""
-        self.relay_server.data_connection.close()
-        self.relay_server.shutdown()
-        self.relay_server.server_close()
-        self.relay_server_thread.join()
+        if self._relay_server:
+            self._relay_server.shutdown()
+        if self.relay_server_thread:
+            self.relay_server_thread.join()
+
+    @property
+    def relay_server(self) -> RelayServer:
+        """
+        Return the relay server object.
+
+        :raises ValueError: if called before ``reset``
+        """
+        if self._relay_server:
+            return self._relay_server
+        raise ValueError("run ``reset`` first!")
```

### Comparing `gym_saturation-0.9.1/gym_saturation/envs/saturation_env.py` & `gym_saturation-0.9.2/gym_saturation/envs/saturation_env.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,21 +21,17 @@
 from abc import abstractmethod
 from typing import Any, Dict, Optional, Tuple
 
 import numpy as np
 from gymnasium import Env, spaces
 from gymnasium.spaces.text import alphanumeric
 
-from gym_saturation.constants import ACTION_MASK, REAL_OBS
+from gym_saturation.constants import ACTION_MASK, MOCK_TPTP_PROBLEM, REAL_OBS
 from gym_saturation.proof_state import ProofState
-from gym_saturation.utils import (
-    FALSEHOOD_SYMBOL,
-    MOCK_TPTP_PROBLEM,
-    pretty_print,
-)
+from gym_saturation.utils import pretty_print
 
 MAX_CLAUSES = 1000
 ALPHANUMERIC_WITH_UNDERSCORE = "".join(alphanumeric) + "_"
 SHORT_TEXT_SPACE = spaces.Text(256, charset=ALPHANUMERIC_WITH_UNDERSCORE)
 LONG_TEXT_SPACE = spaces.Text(
     4000,
     charset=ALPHANUMERIC_WITH_UNDERSCORE + "(), |~=!$",
@@ -166,34 +162,26 @@
             * info: contains auxiliary diagnostic information (helpful for
               debugging, and sometimes learning)
         :raises ValueError: if the ``action`` identifies an already processed
             clause
         """
         if self.state.action_mask[action] == 0.0:
             raise ValueError(f"action {action} is not valid")
-        self.state.step_number += 1
-        self._do_deductions(action)
-        self.state.action_mask[action] = 0.0
-        truncated = len(self.state.clauses) > int(self.action_space.n)
-        terminated = (
-            max(
-                clause["literals"] == FALSEHOOD_SYMBOL
-                for clause in self.state.clauses
-            )
-            or self.state.action_mask.max() == 0.0
-        ) and not truncated
-        reward = 1.0 if terminated else 0.0
+        if not (self.state.terminated or self.state.truncated):
+            self.state.step_number += 1
+            self._do_deductions(action)
+            self.state.action_mask[action] = 0.0
         return (
             {
                 REAL_OBS: tuple(self.state.clauses),
                 ACTION_MASK: self.state.action_mask,
             },
-            reward,
-            terminated,
-            truncated,
+            1.0 if self.state.terminated else 0.0,
+            self.state.terminated,
+            self.state.truncated,
             {},
         )
 
     # pylint: disable=inconsistent-return-statements
     def render(self):  # noqa: D102
         tptp_string = "\n".join(
             map(
```

### Comparing `gym_saturation-0.9.1/gym_saturation/envs/vampire_env.py` & `gym_saturation-0.9.2/gym_saturation/envs/vampire_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,84 +24,85 @@
 
 from gym_saturation.envs.saturation_env import (
     ACTION_MASK,
     MAX_CLAUSES,
     REAL_OBS,
     SaturationEnv,
 )
-from gym_saturation.utils import FALSEHOOD_SYMBOL
 from gym_saturation.vampire_wrapper import VampireWrapper
 
 
 class VampireEnv(SaturationEnv):
     """
     An RL environment around a Vampire prover.
 
-    Refer to :ref:`vampire_env` for more documentation.
+    Refer to :ref:`saturation_env` for more documentation.
 
     We can run a full Gymnasium environment check:
 
     >>> from gymnasium.utils.env_checker import check_env
     >>> import gymnasium as gym
     >>> env = gym.make(
     ...     "Vampire-v0",
     ...     max_clauses=5
     ... ).unwrapped
     >>> check_env(env)
     cnf(1, ...).
     ...
     cnf(5, ...).
 
+    we can't repeat actions
+
+    >>> _ = env.reset()
+    >>> _ = env.step(0)
+    >>> env.step(0)
+    Traceback (most recent call last):
+     ...
+    ValueError: action 0 is not valid
+
     sometimes Vampire can solve a problem during pre-processing
 
-    >>> from gym_saturation.utils import MOCK_TPTP_PROBLEM
+    >>> from gym_saturation.constants import MOCK_TPTP_PROBLEM
     >>> trivial_problem = os.path.join(os.path.dirname(MOCK_TPTP_PROBLEM),
     ...     "TST002-1.p")
     >>> env.set_task(trivial_problem)
     >>> _, _ = env.reset()
+    >>> env.state.terminated
+    True
     >>> _, _, terminated, _, _ = env.step(0)
     >>> terminated
     True
 
-    we can't repeat actions
-
-    >>> _ = env.reset()
-    >>> _ = env.step(0)
-    >>> env.step(0)
-    Traceback (most recent call last):
-     ...
-    ValueError: action 0 is not valid
-
     a test of an unexpected reply from Vampire
 
-    >>> from gym_saturation.utils import MOCK_TPTP_FOLDER
+    >>> from gym_saturation.constants import MOCK_TPTP_FOLDER
     >>> vampire_binary = os.path.join(MOCK_TPTP_FOLDER, "..", "vampire-mock")
-    >>> vampire_env = VampireEnv(vampire_binary_path=vampire_binary)
+    >>> vampire_env = VampireEnv(prover_binary_path=vampire_binary)
     >>> vampire_env.reset()
     Traceback (most recent call last):
      ...
     ValueError: ('Unexpected response type: ', 'who could expect that?')
     """
 
     def __init__(
         self,
         max_clauses: int = MAX_CLAUSES,
         render_mode: str = "human",
-        vampire_binary_path: str = "vampire",
+        prover_binary_path: str = "vampire",
     ):
         """
         Initialise a :ref:`VampireWrapper <vampire-wrapper>`.
 
         :param max_clauses: maximal number of clauses in proof state
         :param render_mode: a mode of running ``render`` method
-        :param vampire_binary_path: a path to Vampire binary;
+        :param prover_binary_path: a path to Vampire binary;
             by default we expect it to be in the $PATH
         """
         super().__init__(max_clauses, render_mode)
-        self._vampire = VampireWrapper(vampire_binary_path)
+        self._vampire = VampireWrapper(prover_binary_path)
 
     def _parse_vampire_response(
         self, vampire_response: Tuple[Tuple[str, str, str], ...]
     ) -> None:
         for response_type, clause_label, clause_text in vampire_response:
             if response_type in {"new", "final", "input", "fn def discovered"}:
                 self.state.add_clause(
@@ -132,19 +133,14 @@
         self._parse_vampire_response(vampire_response)
         return {
             REAL_OBS: tuple(self.state.clauses),
             ACTION_MASK: self.state.action_mask,
         }, {}
 
     def _do_deductions(self, action: np.int64) -> None:
-        if any(
-            clause["literals"] == FALSEHOOD_SYMBOL
-            for clause in self.state.clauses
-        ):
-            return
         self._parse_vampire_response(
             self._vampire.pick_a_clause(self.state.clause_labels[action])
         )
 
     def _parse_vampire_clause(
         self, clause_label: str, clause_text: str
     ) -> Dict[str, Any]:
```

### Comparing `gym_saturation-0.9.1/gym_saturation/proof_state.py` & `gym_saturation-0.9.2/gym_saturation/proof_state.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 ============
 """
 from dataclasses import dataclass
 from typing import Any, Dict, List
 
 import numpy as np
 
+from gym_saturation.constants import FALSEHOOD_SYMBOL
+
 
 @dataclass
 class ProofState:
     """
     An object to store all relevant info about a saturation prover state.
 
     :param clauses: clauses (both processed and not) for access by index
@@ -60,7 +62,23 @@
 
         :param clause_label: a label of the clause to set action mask
         :param mask_value: ``0.0`` (processed/removed) or ``1.0`` (unprocessed)
         """
         clause_index = self.clause_labels.index(clause_label)
         if clause_index < self.action_mask.shape[0]:
             self.action_mask[clause_index] = mask_value
+
+    @property
+    def terminated(self) -> bool:
+        """Refutation found or satisfiability established."""
+        return (
+            max(
+                clause["literals"] == FALSEHOOD_SYMBOL
+                for clause in self.clauses
+            )
+            or self.action_mask.max() == 0.0
+        ) and not self.truncated
+
+    @property
+    def truncated(self) -> bool:
+        """More clauses generated than expected."""
+        return len(self.clauses) > self.action_mask.shape[0]
```

### Comparing `gym_saturation-0.9.1/gym_saturation/utils.py` & `gym_saturation-0.9.2/gym_saturation/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,33 +13,18 @@
 # limitations under the License.
 
 # noqa: D205, D400
 """
 Logic Operations Utility Functions
 ===================================
 """
-import os
-import sys
 from itertools import chain
 from typing import Any, Dict, Tuple
 
-if sys.version_info.major == 3 and sys.version_info.minor >= 9:
-    # pylint: disable=no-name-in-module
-    from importlib.resources import files  # type: ignore
-else:  # pragma: no cover
-    from importlib_resources import files  # pylint: disable=import-error
-
-
-FALSEHOOD_SYMBOL = "$false"
-MOCK_TPTP_FOLDER = str(
-    files("gym_saturation").joinpath(os.path.join("resources", "TPTP-mock"))
-)
-MOCK_TPTP_PROBLEM = os.path.join(
-    MOCK_TPTP_FOLDER, "Problems", "TST", "TST001-1.p"
-)
+from gym_saturation.constants import FALSEHOOD_SYMBOL
 
 
 def pretty_print(clause: Dict[str, Any]) -> str:
     """
     Print a logical formula back to TPTP language.
 
     :param clause: a logical clause to print
```

### Comparing `gym_saturation-0.9.1/gym_saturation/vampire_wrapper.py` & `gym_saturation-0.9.2/gym_saturation/vampire_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 
 class VampireWrapper:
     """
     A wrapper around Vampire binary running in a manual clause selection mode.
 
     .. _vampire-wrapper :
 
-    >>> from gym_saturation.utils import MOCK_TPTP_PROBLEM, MOCK_TPTP_FOLDER
+    >>> from gym_saturation.constants import (MOCK_TPTP_PROBLEM,
+    ...     MOCK_TPTP_FOLDER)
     >>> vampire = VampireWrapper("vampire")
     >>> vampire.pick_a_clause("2")
     Traceback (most recent call last):
      ...
     ValueError: start solving a problem first!
     >>> result = vampire.start(MOCK_TPTP_PROBLEM, MOCK_TPTP_FOLDER)
     >>> vampire.pick_a_clause("wrong")
```

### Comparing `gym_saturation-0.9.1/gym_saturation/wrappers/age_weight_bandit.py` & `gym_saturation-0.9.2/gym_saturation/wrappers/age_weight_bandit.py`

 * *Files identical despite different names*

### Comparing `gym_saturation-0.9.1/gym_saturation/wrappers/ast2vec_wrapper.py` & `gym_saturation-0.9.2/gym_saturation/wrappers/ast2vec_wrapper.py`

 * *Files identical despite different names*

### Comparing `gym_saturation-0.9.1/gym_saturation/wrappers/constant_parametric_actions.py` & `gym_saturation-0.9.2/gym_saturation/wrappers/constant_parametric_actions.py`

 * *Files identical despite different names*

### Comparing `gym_saturation-0.9.1/gym_saturation/wrappers/duplicate_key_obs.py` & `gym_saturation-0.9.2/gym_saturation/wrappers/duplicate_key_obs.py`

 * *Files identical despite different names*

### Comparing `gym_saturation-0.9.1/gym_saturation/wrappers/parametric_actions_wrapper.py` & `gym_saturation-0.9.2/gym_saturation/wrappers/parametric_actions_wrapper.py`

 * *Files identical despite different names*

### Comparing `gym_saturation-0.9.1/pyproject.toml` & `gym_saturation-0.9.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gym-saturation"
-version = "0.9.1"
+version = "0.9.2"
 description = "Gymnasium environments for saturation provers"
 authors = ["Boris Shminke <boris@shminke.ml>"]
 license = "Apache-2.0"
 repository = "https://github.com/inpefess/gym-saturation"
 readme = "README.rst"
 classifiers=[
 	"Programming Language :: Python :: 3.8",
@@ -56,15 +56,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
-addopts = "--doctest-modules --cov gym_saturation --cov-report xml --cov-fail-under=99 --junit-xml test-results/gym-saturation.xml"
+addopts = "--doctest-modules --cov gym_saturation --cov-report xml --cov-fail-under=100 --junit-xml test-results/gym-saturation.xml"
 testpaths = ["gym_saturation"]
 doctest_optionflags = "NORMALIZE_WHITESPACE ELLIPSIS"
 
 [tool.pylint.MASTER]
 load-plugins = [
     "pylint.extensions.docparams",
     "pylint.extensions.mccabe",
@@ -132,15 +132,15 @@
     pytest
 """
 
 [tool.tbump]
 github_url = "https://github.com/inpfess/gym-saturation/"
 
 [tool.tbump.version]
-current = "0.9.1"
+current = "0.9.2"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   '''
```

### Comparing `gym_saturation-0.9.1/PKG-INFO` & `gym_saturation-0.9.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-saturation
-Version: 0.9.1
+Version: 0.9.2
 Summary: Gymnasium environments for saturation provers
 Home-page: https://github.com/inpefess/gym-saturation
 License: Apache-2.0
 Author: Boris Shminke
 Author-email: boris@shminke.ml
 Requires-Python: >=3.8.1,<3.12
 Classifier: Development Status :: 3 - Alpha
@@ -51,16 +51,15 @@
 
 ``gym-saturation`` is a collection of `Gymnasium
 <https://gymnasium.farama.org/>`__ environments for reinforcement learning
 (RL) agents striving to prove theorems. Currently, only theorems
 written in `TPTP library <https://tptp.org>`__ formal language are
 supported.
 
-There are two environments in ``gym-saturation``: `VampireEnv <https://gym-saturation.readthedocs.io/en/latest/environments/vampire-env.html#vampire-env>`__ and
-`IProverEnv <https://gym-saturation.readthedocs.io/en/latest/environments/iprover-env.html#iprover-env>`__. ``VampireEnv`` is a wrapper around a recent `Vampire
+There are two environments in ``gym-saturation`` following the same API: `SaturationEnv <https://gym-saturation.readthedocs.io/en/latest/environments/saturation-env.html>`__: ``VampireEnv`` is a wrapper around a recent `Vampire
 <https://github.com/vprover/vampire>`__ prover, and ``IProverEnv``
 relies on an experimental version of `iProver
 <https://gitlab.com/korovin/iprover/>`__.
 
 In contrast to monolithic architecture of a typical Automated Theorem
 Prover (ATP), ``gym-saturation`` gives different agents opportunities
 to select clauses themselves and train from their experience.
@@ -76,32 +75,32 @@
 ==============
 
 .. attention:: If you want to use ``VampireEnv`` you should have a
    Vampire binary on your machine. For example, download the
    latest `release
    <https://github.com/vprover/vampire/releases/tag/v4.7>`__.
 
-   To use ``IProverEnv``, please build iProver from source using
-   `this branch
-   <https://gitlab.com/korovin/iprover/-/tree/2022_sockets>`__.
+   To use ``IProverEnv``, please download the experimental iProver 
+   `release
+   <https://gitlab.com/inpefess/iprover/-/releases/2022.11.03>`__ or build it from `this commit <https://gitlab.com/korovin/iprover/-/commit/32c76fc0ec665a06324d11dc9d4bf902871d5f15>`__.
 
 The best way to install this package is to use ``pip``:
 
 .. code:: sh
 
    pip install gym-saturation
 
 Another option is to use ``conda``:
 
 .. code:: sh
 
    conda install -c conda-forge gym-saturation
    
-One can also run it in a Docker container (with a pre-packed
-``vampire`` binary):
+One can also run it in a Docker container (pre-packed with
+``vampire`` and ``iproveropt`` binaries):
 
 .. code:: sh
 
    docker build -t gym-saturation https://github.com/inpefess/gym-saturation.git
    docker run -it --rm -p 8888:8888 gym-saturation jupyter-lab --ip=0.0.0.0 --port=8888
 
 How to use
@@ -121,15 +120,15 @@
   terminated, truncated = False, False
   while not (terminated or truncated):
       # apply policy (a valid random action here)
       action = env.action_space.sample(mask=observation["action_mask"])
       observation, reward, terminated, truncated, info = env.step(action)
   env.close()
 
-Or have a look at the basic `tutorial <https://gym-saturation.readthedocs.io/en/latest/tutorials/auto_examples/plot_age_agent.html>`__.
+Or have a look at the basic `tutorial <https://gym-saturation.readthedocs.io/en/latest/auto_examples/plot_age_agent.html>`__.
   
 For a bit more comprehensive experiments, please navigate the documentation `page <https://gym-saturation.readthedocs.io/en/latest/tutorials/experiments.html>`__.
 
 How to Contribute
 =================
 
 `Pull requests <https://github.com/inpefess/gym-saturation/pulls>`__ are
@@ -141,18 +140,22 @@
    cd gym-saturation
    # activate python virtual environment with Python 3.8+
    pip install -U pip
    pip install -U setuptools wheel poetry
    poetry install
    # recommended but not necessary
    pre-commit install
-   # install vampire binary
+   # install Vampire binary
    wget https://github.com/vprover/vampire/releases/download/v4.7/vampire4.7.zip -O vampire.zip
    unzip vampire.zip
    # then use vampire_z3_rel_static_HEAD_6295 as an argument or add it to $PATH
+   # install iProver binary
+   wget https://gitlab.com/api/v4/projects/39846772/jobs/artifacts/2022.11.03/download?job=build-job -O iprover.zip
+   unzip iprover.zip
+   # then use iproveropt
 
 All the tests in this package are
 `doctests <https://docs.python.org/3/library/doctest.html>`__. One can
 run them with the following command:
 
 .. code:: sh
```

