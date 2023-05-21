# Comparing `tmp/gym_saturation-0.9.2.tar.gz` & `tmp/gym_saturation-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym_saturation-0.9.2.tar", max compression
+gzip compressed data, was "gym_saturation-0.9.3.tar", max compression
```

## Comparing `gym_saturation-0.9.2.tar` & `gym_saturation-0.9.3.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0    11360 2022-09-19 19:58:15.552724 gym_saturation-0.9.2/LICENSE
--rw-r--r--   0        0        0     6285 2023-04-11 17:02:37.334496 gym_saturation-0.9.2/README.rst
--rw-r--r--   0        0        0      991 2023-04-11 17:02:37.366490 gym_saturation-0.9.2/gym_saturation/__init__.py
--rw-r--r--   0        0        0     8636 2023-04-11 17:02:37.366490 gym_saturation-0.9.2/gym_saturation/agent_testing.py
--rw-r--r--   0        0        0     1242 2023-04-04 11:04:37.023214 gym_saturation-0.9.2/gym_saturation/conftest.py
--rw-r--r--   0        0        0     1296 2023-04-11 17:02:37.370489 gym_saturation-0.9.2/gym_saturation/constants.py
--rw-r--r--   0        0        0     1168 2023-03-24 12:49:21.170500 gym_saturation-0.9.2/gym_saturation/dummy_http_handler.py
--rw-r--r--   0        0        0      789 2023-01-08 12:44:28.449376 gym_saturation-0.9.2/gym_saturation/envs/__init__.py
--rw-r--r--   0        0        0     7506 2023-04-11 17:02:37.370489 gym_saturation-0.9.2/gym_saturation/envs/iprover_env.py
--rw-r--r--   0        0        0     7230 2023-04-11 17:02:37.374488 gym_saturation-0.9.2/gym_saturation/envs/saturation_env.py
--rw-r--r--   0        0        0     5401 2023-04-11 17:02:37.378488 gym_saturation-0.9.2/gym_saturation/envs/vampire_env.py
--rw-r--r--   0        0        0     2795 2023-04-11 17:02:37.378488 gym_saturation-0.9.2/gym_saturation/proof_state.py
--rw-r--r--   0        0        0        0 2021-07-22 09:53:47.848012 gym_saturation-0.9.2/gym_saturation/py.typed
--rw-r--r--   0        0        0     3893 2023-04-11 17:02:37.382487 gym_saturation-0.9.2/gym_saturation/relay_server.py
--rw-r--r--   0        0        0      267 2023-04-04 11:04:37.027214 gym_saturation-0.9.2/gym_saturation/resources/TPTP-mock/Problems/TST/TST001-1.p
--rw-r--r--   0        0        0       77 2023-04-04 11:04:37.027214 gym_saturation-0.9.2/gym_saturation/resources/TPTP-mock/Problems/TST/TST002-1.p
--rwxr-xr-x   0        0        0       62 2022-11-07 08:44:37.735015 gym_saturation-0.9.2/gym_saturation/resources/vampire-mock
--rw-r--r--   0        0        0     3647 2023-04-11 17:02:37.382487 gym_saturation-0.9.2/gym_saturation/utils.py
--rw-r--r--   0        0        0     4086 2023-04-11 17:02:37.382487 gym_saturation-0.9.2/gym_saturation/vampire_wrapper.py
--rw-r--r--   0        0        0     2570 2023-04-04 11:04:37.031214 gym_saturation-0.9.2/gym_saturation/wrappers/age_weight_bandit.py
--rw-r--r--   0        0        0     2641 2023-04-04 11:04:37.035214 gym_saturation-0.9.2/gym_saturation/wrappers/ast2vec_wrapper.py
--rw-r--r--   0        0        0     2395 2023-04-06 15:52:02.959734 gym_saturation-0.9.2/gym_saturation/wrappers/constant_parametric_actions.py
--rw-r--r--   0        0        0     2221 2023-04-04 11:04:37.035214 gym_saturation-0.9.2/gym_saturation/wrappers/duplicate_key_obs.py
--rw-r--r--   0        0        0     5435 2023-04-06 15:52:02.963734 gym_saturation-0.9.2/gym_saturation/wrappers/parametric_actions_wrapper.py
--rw-r--r--   0        0        0     3458 2023-04-11 17:02:37.386486 gym_saturation-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     7551 1970-01-01 00:00:00.000000 gym_saturation-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    11360 2022-09-19 19:58:15.552724 gym_saturation-0.9.3/LICENSE
+-rw-r--r--   0        0        0     6285 2023-04-11 17:02:37.334496 gym_saturation-0.9.3/README.rst
+-rw-r--r--   0        0        0      991 2023-04-21 11:53:58.871757 gym_saturation-0.9.3/gym_saturation/__init__.py
+-rw-r--r--   0        0        0     8636 2023-04-11 17:02:37.366490 gym_saturation-0.9.3/gym_saturation/agent_testing.py
+-rw-r--r--   0        0        0     1242 2023-04-04 11:04:37.023214 gym_saturation-0.9.3/gym_saturation/conftest.py
+-rw-r--r--   0        0        0     1296 2023-04-11 17:02:37.370489 gym_saturation-0.9.3/gym_saturation/constants.py
+-rw-r--r--   0        0        0     1168 2023-03-24 12:49:21.170500 gym_saturation-0.9.3/gym_saturation/dummy_http_handler.py
+-rw-r--r--   0        0        0      812 2023-04-21 11:53:16.683575 gym_saturation-0.9.3/gym_saturation/envs/__init__.py
+-rw-r--r--   0        0        0     7970 2023-04-21 11:53:16.683575 gym_saturation-0.9.3/gym_saturation/envs/iprover_env.py
+-rw-r--r--   0        0        0     7463 2023-04-21 11:53:16.687575 gym_saturation-0.9.3/gym_saturation/envs/saturation_env.py
+-rw-r--r--   0        0        0     5748 2023-04-21 11:53:16.687575 gym_saturation-0.9.3/gym_saturation/envs/vampire_env.py
+-rw-r--r--   0        0        0     2795 2023-04-11 17:02:37.378488 gym_saturation-0.9.3/gym_saturation/proof_state.py
+-rw-r--r--   0        0        0        0 2021-07-22 09:53:47.848012 gym_saturation-0.9.3/gym_saturation/py.typed
+-rw-r--r--   0        0        0     3893 2023-04-11 17:02:37.382487 gym_saturation-0.9.3/gym_saturation/relay_server.py
+-rw-r--r--   0        0        0      267 2023-04-04 11:04:37.027214 gym_saturation-0.9.3/gym_saturation/resources/TPTP-mock/Problems/TST/TST001-1.p
+-rw-r--r--   0        0        0       77 2023-04-04 11:04:37.027214 gym_saturation-0.9.3/gym_saturation/resources/TPTP-mock/Problems/TST/TST002-1.p
+-rwxr-xr-x   0        0        0       62 2022-11-07 08:44:37.735015 gym_saturation-0.9.3/gym_saturation/resources/vampire-mock
+-rw-r--r--   0        0        0     3647 2023-04-11 17:02:37.382487 gym_saturation-0.9.3/gym_saturation/utils.py
+-rw-r--r--   0        0        0     4086 2023-04-11 17:02:37.382487 gym_saturation-0.9.3/gym_saturation/vampire_wrapper.py
+-rw-r--r--   0        0        0     1106 2023-04-21 11:53:16.687575 gym_saturation-0.9.3/gym_saturation/wrappers/__init__.py
+-rw-r--r--   0        0        0     2570 2023-04-04 11:04:37.031214 gym_saturation-0.9.3/gym_saturation/wrappers/age_weight_bandit.py
+-rw-r--r--   0        0        0     2641 2023-04-04 11:04:37.035214 gym_saturation-0.9.3/gym_saturation/wrappers/ast2vec_wrapper.py
+-rw-r--r--   0        0        0     2395 2023-04-16 14:27:22.142190 gym_saturation-0.9.3/gym_saturation/wrappers/constant_parametric_actions.py
+-rw-r--r--   0        0        0     2221 2023-04-04 11:04:37.035214 gym_saturation-0.9.3/gym_saturation/wrappers/duplicate_key_obs.py
+-rw-r--r--   0        0        0     5435 2023-04-06 15:52:02.963734 gym_saturation-0.9.3/gym_saturation/wrappers/parametric_actions_wrapper.py
+-rw-r--r--   0        0        0     3458 2023-04-21 11:53:58.875757 gym_saturation-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     7551 1970-01-01 00:00:00.000000 gym_saturation-0.9.3/PKG-INFO
```

### Comparing `gym_saturation-0.9.2/LICENSE` & `gym_saturation-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gym_saturation-0.9.2/README.rst` & `gym_saturation-0.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `gym_saturation-0.9.2/gym_saturation/__init__.py` & `gym_saturation-0.9.3/gym_saturation/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 They are registered using a limit for the number of steps in an episode and the
 maximal possible reward is set to ``1.0`` (proof is found).
 """
 from gymnasium.envs.registration import register
 
 register(id="Vampire-v0", entry_point="gym_saturation.envs:VampireEnv")
 register(id="iProver-v0", entry_point="gym_saturation.envs:IProverEnv")
-__version__ = "0.9.2"
+__version__ = "0.9.3"
```

### Comparing `gym_saturation-0.9.2/gym_saturation/agent_testing.py` & `gym_saturation-0.9.3/gym_saturation/agent_testing.py`

 * *Files identical despite different names*

### Comparing `gym_saturation-0.9.2/gym_saturation/conftest.py` & `gym_saturation-0.9.3/gym_saturation/conftest.py`

 * *Files identical despite different names*

### Comparing `gym_saturation-0.9.2/gym_saturation/constants.py` & `gym_saturation-0.9.3/gym_saturation/constants.py`

 * *Files identical despite different names*

### Comparing `gym_saturation-0.9.2/gym_saturation/dummy_http_handler.py` & `gym_saturation-0.9.3/gym_saturation/dummy_http_handler.py`

 * *Files identical despite different names*

### Comparing `gym_saturation-0.9.2/gym_saturation/envs/iprover_env.py` & `gym_saturation-0.9.3/gym_saturation/envs/iprover_env.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,14 +83,21 @@
     Traceback (most recent call last):
      ...
     ValueError: run ``reset`` first!
     >>> check_env(env)
     cnf(c_53, ...).
     ...
     cnf(c_49, ...).
+
+    when episode truncated, all threads are terminated
+
+    >>> _ = env.reset()
+    >>> _, _, _, truncated, _ = env.step(4)
+    >>> truncated
+    True
     """
 
     def __init__(
         self,
         max_clauses: int = MAX_CLAUSES,
         render_mode: str = "human",
         prover_binary_path: str = "iproveropt",
@@ -107,15 +114,15 @@
         self.prover_binary_path = prover_binary_path
         self._relay_server: Optional[RelayServer] = None
         self.relay_server_thread: Optional[Thread] = None
         self.iprover_process: Optional[subprocess.Popen] = None
 
     def _restart_relay_server(self) -> None:
         if self._relay_server:
-            self.close()
+            self._terminate_threads()
         self._relay_server = RelayServer(("localhost", 0), RelayTCPHandler)
         self.relay_server_thread = Thread(
             target=self._relay_server.serve_forever
         )
         self.relay_server_thread.daemon = True
         self.relay_server_thread.start()
 
@@ -210,22 +217,32 @@
         )
         self.relay_server.output_queue.put(relayed_scores_message)
         data = self._get_json_data()
         self._parse_iprover_requests(data)
 
     def close(self) -> None:
         """Stop relay server."""
-        if self._relay_server:
-            self._relay_server.shutdown()
-        if self.relay_server_thread:
-            self.relay_server_thread.join()
+        self._terminate_threads()
 
     @property
     def relay_server(self) -> RelayServer:
         """
         Return the relay server object.
 
         :raises ValueError: if called before ``reset``
         """
         if self._relay_server:
             return self._relay_server
         raise ValueError("run ``reset`` first!")
+
+    def on_truncated(self) -> None:
+        """Terminate threads."""
+        self._terminate_threads()
+
+    def _terminate_threads(self) -> None:
+        if self._relay_server:
+            self._relay_server.shutdown()
+        if self.relay_server_thread:
+            self.relay_server_thread.join()
+        if self.iprover_process:
+            self.iprover_process.terminate()
+            self.iprover_process.wait()
```

### Comparing `gym_saturation-0.9.2/gym_saturation/envs/saturation_env.py` & `gym_saturation-0.9.3/gym_saturation/envs/saturation_env.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,18 @@
 SHORT_TEXT_SPACE = spaces.Text(256, charset=ALPHANUMERIC_WITH_UNDERSCORE)
 LONG_TEXT_SPACE = spaces.Text(
     4000,
     charset=ALPHANUMERIC_WITH_UNDERSCORE + "(), |~=!$",
 )
 
 
+class InvalidAction(Exception):
+    """Raised when step is called with invalid action."""
+
+
 class SaturationEnv(Env[Dict[str, Any], np.int64]):
     """
     Saturation algorithm in a reinforcement learning friendly way.
 
     It's an abstract class, so here we have only trivial smoke tests.
     One should override ``_do_deductions`` method in children classes.
 
@@ -157,23 +161,25 @@
             * observation: agent's observation of the current environment
             * reward: amount of reward returned after previous action
             * terminated: Whether the proof was found
             * truncated: Whether the maximal number of clauses in the proof
               state were reached
             * info: contains auxiliary diagnostic information (helpful for
               debugging, and sometimes learning)
-        :raises ValueError: if the ``action`` identifies an already processed
-            clause
+        :raises InvalidAction: if the ``action`` identifies an already
+            processed clause
         """
-        if self.state.action_mask[action] == 0.0:
-            raise ValueError(f"action {action} is not valid")
         if not (self.state.terminated or self.state.truncated):
+            if self.state.action_mask[action] == 0.0:
+                raise InvalidAction
             self.state.step_number += 1
             self._do_deductions(action)
             self.state.action_mask[action] = 0.0
+            if self.state.truncated:
+                self.on_truncated()
         return (
             {
                 REAL_OBS: tuple(self.state.clauses),
                 ACTION_MASK: self.state.action_mask,
             },
             1.0 if self.state.terminated else 0.0,
             self.state.terminated,
@@ -208,7 +214,10 @@
         """
         Get the task that the agent is performing in the current environment.
 
         :returns: a TPTP problem filename
         :raises ValueError: is task is not set
         """
         return self._task
+
+    def on_truncated(self) -> None:
+        """Prover-specific episode truncation."""
```

### Comparing `gym_saturation-0.9.2/gym_saturation/envs/vampire_env.py` & `gym_saturation-0.9.3/gym_saturation/envs/vampire_env.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,20 +48,21 @@
     >>> check_env(env)
     cnf(1, ...).
     ...
     cnf(5, ...).
 
     we can't repeat actions
 
+    >>> env = gym.make("Vampire-v0")
     >>> _ = env.reset()
     >>> _ = env.step(0)
     >>> env.step(0)
     Traceback (most recent call last):
      ...
-    ValueError: action 0 is not valid
+    gym_saturation.envs.saturation_env.InvalidAction
 
     sometimes Vampire can solve a problem during pre-processing
 
     >>> from gym_saturation.constants import MOCK_TPTP_PROBLEM
     >>> trivial_problem = os.path.join(os.path.dirname(MOCK_TPTP_PROBLEM),
     ...     "TST002-1.p")
     >>> env.set_task(trivial_problem)
@@ -155,7 +156,17 @@
             "literals": formula.strip(),
             "label": clause_label,
             "role": "lemma",
             "inference_rule": inference_rule,
             "inference_parents": inference_parents,
             "birth_step": self.state.step_number,
         }
+
+    def on_truncated(self) -> None:
+        """Terminate Vampire process."""
+        self._vampire.proc.terminate()
+        self._vampire.proc.wait()
+
+    def close(self) -> None:
+        """Terminate Vampire process."""
+        self._vampire.proc.terminate()
+        self._vampire.proc.wait()
```

### Comparing `gym_saturation-0.9.2/gym_saturation/proof_state.py` & `gym_saturation-0.9.3/gym_saturation/proof_state.py`

 * *Files identical despite different names*

### Comparing `gym_saturation-0.9.2/gym_saturation/relay_server.py` & `gym_saturation-0.9.3/gym_saturation/relay_server.py`

 * *Files identical despite different names*

### Comparing `gym_saturation-0.9.2/gym_saturation/utils.py` & `gym_saturation-0.9.3/gym_saturation/utils.py`

 * *Files identical despite different names*

### Comparing `gym_saturation-0.9.2/gym_saturation/vampire_wrapper.py` & `gym_saturation-0.9.3/gym_saturation/vampire_wrapper.py`

 * *Files identical despite different names*

### Comparing `gym_saturation-0.9.2/gym_saturation/wrappers/age_weight_bandit.py` & `gym_saturation-0.9.3/gym_saturation/wrappers/age_weight_bandit.py`

 * *Files identical despite different names*

### Comparing `gym_saturation-0.9.2/gym_saturation/wrappers/ast2vec_wrapper.py` & `gym_saturation-0.9.3/gym_saturation/wrappers/ast2vec_wrapper.py`

 * *Files identical despite different names*

### Comparing `gym_saturation-0.9.2/gym_saturation/wrappers/constant_parametric_actions.py` & `gym_saturation-0.9.3/gym_saturation/wrappers/constant_parametric_actions.py`

 * *Files identical despite different names*

### Comparing `gym_saturation-0.9.2/gym_saturation/wrappers/duplicate_key_obs.py` & `gym_saturation-0.9.3/gym_saturation/wrappers/duplicate_key_obs.py`

 * *Files identical despite different names*

### Comparing `gym_saturation-0.9.2/gym_saturation/wrappers/parametric_actions_wrapper.py` & `gym_saturation-0.9.3/gym_saturation/wrappers/parametric_actions_wrapper.py`

 * *Files identical despite different names*

### Comparing `gym_saturation-0.9.2/pyproject.toml` & `gym_saturation-0.9.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gym-saturation"
-version = "0.9.2"
+version = "0.9.3"
 description = "Gymnasium environments for saturation provers"
 authors = ["Boris Shminke <boris@shminke.ml>"]
 license = "Apache-2.0"
 repository = "https://github.com/inpefess/gym-saturation"
 readme = "README.rst"
 classifiers=[
 	"Programming Language :: Python :: 3.8",
@@ -132,15 +132,15 @@
     pytest
 """
 
 [tool.tbump]
 github_url = "https://github.com/inpfess/gym-saturation/"
 
 [tool.tbump.version]
-current = "0.9.2"
+current = "0.9.3"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   '''
```

### Comparing `gym_saturation-0.9.2/PKG-INFO` & `gym_saturation-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-saturation
-Version: 0.9.2
+Version: 0.9.3
 Summary: Gymnasium environments for saturation provers
 Home-page: https://github.com/inpefess/gym-saturation
 License: Apache-2.0
 Author: Boris Shminke
 Author-email: boris@shminke.ml
 Requires-Python: >=3.8.1,<3.12
 Classifier: Development Status :: 3 - Alpha
```

