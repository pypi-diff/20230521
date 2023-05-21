# Comparing `tmp/Wavelink-2.3.0.tar.gz` & `tmp/Wavelink-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Wavelink-2.3.0.tar", last modified: Sat May 20 08:58:01 2023, max compression
+gzip compressed data, was "Wavelink-2.3.1.tar", last modified: Sun May 21 00:10:17 2023, max compression
```

## Comparing `Wavelink-2.3.0.tar` & `Wavelink-2.3.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 08:58:01.231994 Wavelink-2.3.0/
--rw-rw-rw-   0        0        0     1108 2023-03-09 18:26:07.000000 Wavelink-2.3.0/LICENSE
--rw-rw-rw-   0        0        0     5772 2023-05-20 08:58:01.231494 Wavelink-2.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     4969 2023-03-09 18:33:50.000000 Wavelink-2.3.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-20 08:58:01.169060 Wavelink-2.3.0/Wavelink.egg-info/
--rw-rw-rw-   0        0        0     5772 2023-05-20 08:58:01.000000 Wavelink-2.3.0/Wavelink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-05-20 08:58:01.000000 Wavelink-2.3.0/Wavelink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 08:58:01.000000 Wavelink-2.3.0/Wavelink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-20 08:58:01.000000 Wavelink-2.3.0/Wavelink.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-20 08:58:01.000000 Wavelink-2.3.0/Wavelink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1006 2023-05-20 08:48:03.000000 Wavelink-2.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       49 2023-03-09 18:26:07.000000 Wavelink-2.3.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 08:58:01.231994 Wavelink-2.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-20 08:58:01.207765 Wavelink-2.3.0/wavelink/
--rw-rw-rw-   0        0        0     1495 2023-05-20 08:48:03.000000 Wavelink-2.3.0/wavelink/__init__.py
--rw-rw-rw-   0        0        0     2701 2023-03-09 18:26:07.000000 Wavelink-2.3.0/wavelink/backoff.py
--rw-rw-rw-   0        0        0     2225 2023-05-20 08:30:58.000000 Wavelink-2.3.0/wavelink/enums.py
--rw-rw-rw-   0        0        0     1995 2023-03-09 18:26:07.000000 Wavelink-2.3.0/wavelink/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-20 08:58:01.141550 Wavelink-2.3.0/wavelink/ext/
-drwxrwxrwx   0        0        0        0 2023-05-20 08:58:01.214288 Wavelink-2.3.0/wavelink/ext/spotify/
--rw-rw-rw-   0        0        0    16455 2023-04-01 01:28:43.000000 Wavelink-2.3.0/wavelink/ext/spotify/__init__.py
--rw-rw-rw-   0        0        0    20203 2023-03-09 18:26:07.000000 Wavelink-2.3.0/wavelink/filters.py
--rw-rw-rw-   0        0        0    17765 2023-04-04 07:37:42.000000 Wavelink-2.3.0/wavelink/node.py
--rw-rw-rw-   0        0        0     3461 2023-05-20 08:41:44.000000 Wavelink-2.3.0/wavelink/payloads.py
--rw-rw-rw-   0        0        0    20759 2023-05-20 08:25:37.000000 Wavelink-2.3.0/wavelink/player.py
--rw-rw-rw-   0        0        0    12384 2023-03-15 08:08:05.000000 Wavelink-2.3.0/wavelink/queue.py
--rw-rw-rw-   0        0        0    10102 2023-03-09 18:26:07.000000 Wavelink-2.3.0/wavelink/tracks.py
-drwxrwxrwx   0        0        0        0 2023-05-20 08:58:01.230357 Wavelink-2.3.0/wavelink/types/
--rw-rw-rw-   0        0        0      860 2023-03-09 18:26:07.000000 Wavelink-2.3.0/wavelink/types/events.py
--rw-rw-rw-   0        0        0      635 2023-03-09 18:26:07.000000 Wavelink-2.3.0/wavelink/types/request.py
--rw-rw-rw-   0        0        0      424 2023-03-09 18:26:07.000000 Wavelink-2.3.0/wavelink/types/state.py
--rw-rw-rw-   0        0        0      343 2023-03-09 18:26:07.000000 Wavelink-2.3.0/wavelink/types/track.py
--rw-rw-rw-   0        0        0     9570 2023-05-20 08:53:53.000000 Wavelink-2.3.0/wavelink/websocket.py
+drwxrwxrwx   0        0        0        0 2023-05-21 00:10:17.462276 Wavelink-2.3.1/
+-rw-rw-rw-   0        0        0     1108 2023-03-09 18:26:07.000000 Wavelink-2.3.1/LICENSE
+-rw-rw-rw-   0        0        0     5772 2023-05-21 00:10:17.461774 Wavelink-2.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4969 2023-03-09 18:33:50.000000 Wavelink-2.3.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-21 00:10:17.377169 Wavelink-2.3.1/Wavelink.egg-info/
+-rw-rw-rw-   0        0        0     5772 2023-05-21 00:10:17.000000 Wavelink-2.3.1/Wavelink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-05-21 00:10:17.000000 Wavelink-2.3.1/Wavelink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 00:10:17.000000 Wavelink-2.3.1/Wavelink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-21 00:10:17.000000 Wavelink-2.3.1/Wavelink.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-21 00:10:17.000000 Wavelink-2.3.1/Wavelink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1006 2023-05-21 00:09:01.000000 Wavelink-2.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       49 2023-03-09 18:26:07.000000 Wavelink-2.3.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-21 00:10:17.462776 Wavelink-2.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-21 00:10:17.436127 Wavelink-2.3.1/wavelink/
+-rw-rw-rw-   0        0        0     1495 2023-05-21 00:09:01.000000 Wavelink-2.3.1/wavelink/__init__.py
+-rw-rw-rw-   0        0        0     2701 2023-03-09 18:26:07.000000 Wavelink-2.3.1/wavelink/backoff.py
+-rw-rw-rw-   0        0        0     2225 2023-05-20 08:30:58.000000 Wavelink-2.3.1/wavelink/enums.py
+-rw-rw-rw-   0        0        0     1995 2023-03-09 18:26:07.000000 Wavelink-2.3.1/wavelink/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-21 00:10:17.351676 Wavelink-2.3.1/wavelink/ext/
+drwxrwxrwx   0        0        0        0 2023-05-21 00:10:17.442187 Wavelink-2.3.1/wavelink/ext/spotify/
+-rw-rw-rw-   0        0        0    16455 2023-04-01 01:28:43.000000 Wavelink-2.3.1/wavelink/ext/spotify/__init__.py
+-rw-rw-rw-   0        0        0    20203 2023-03-09 18:26:07.000000 Wavelink-2.3.1/wavelink/filters.py
+-rw-rw-rw-   0        0        0    17765 2023-04-04 07:37:42.000000 Wavelink-2.3.1/wavelink/node.py
+-rw-rw-rw-   0        0        0     3461 2023-05-20 08:41:44.000000 Wavelink-2.3.1/wavelink/payloads.py
+-rw-rw-rw-   0        0        0    20971 2023-05-21 00:07:39.000000 Wavelink-2.3.1/wavelink/player.py
+-rw-rw-rw-   0        0        0    12384 2023-03-15 08:08:05.000000 Wavelink-2.3.1/wavelink/queue.py
+-rw-rw-rw-   0        0        0    10102 2023-03-09 18:26:07.000000 Wavelink-2.3.1/wavelink/tracks.py
+drwxrwxrwx   0        0        0        0 2023-05-21 00:10:17.460773 Wavelink-2.3.1/wavelink/types/
+-rw-rw-rw-   0        0        0      860 2023-03-09 18:26:07.000000 Wavelink-2.3.1/wavelink/types/events.py
+-rw-rw-rw-   0        0        0      635 2023-03-09 18:26:07.000000 Wavelink-2.3.1/wavelink/types/request.py
+-rw-rw-rw-   0        0        0      424 2023-03-09 18:26:07.000000 Wavelink-2.3.1/wavelink/types/state.py
+-rw-rw-rw-   0        0        0      343 2023-03-09 18:26:07.000000 Wavelink-2.3.1/wavelink/types/track.py
+-rw-rw-rw-   0        0        0     9570 2023-05-20 08:53:53.000000 Wavelink-2.3.1/wavelink/websocket.py
```

### Comparing `Wavelink-2.3.0/LICENSE` & `Wavelink-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Wavelink-2.3.0/PKG-INFO` & `Wavelink-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Wavelink
-Version: 2.3.0
+Version: 2.3.1
 Summary: A robust and powerful Lavalink wrapper for discord.py
 Author-email: EvieePy <evieepy@gmail.com>
 Project-URL: Homepage, https://github.com/PythonistaGuild/Wavelink
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `Wavelink-2.3.0/README.rst` & `Wavelink-2.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `Wavelink-2.3.0/Wavelink.egg-info/PKG-INFO` & `Wavelink-2.3.1/Wavelink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Wavelink
-Version: 2.3.0
+Version: 2.3.1
 Summary: A robust and powerful Lavalink wrapper for discord.py
 Author-email: EvieePy <evieepy@gmail.com>
 Project-URL: Homepage, https://github.com/PythonistaGuild/Wavelink
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `Wavelink-2.3.0/Wavelink.egg-info/SOURCES.txt` & `Wavelink-2.3.1/Wavelink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Wavelink-2.3.0/pyproject.toml` & `Wavelink-2.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Wavelink"
-version = "2.3.0"
+version = "2.3.1"
 authors = [
   { name="EvieePy", email="evieepy@gmail.com" },
 ]
 dynamic = ["dependencies"]
 description = "A robust and powerful Lavalink wrapper for discord.py"
 readme = "README.rst"
 requires-python = ">=3.10"
```

### Comparing `Wavelink-2.3.0/wavelink/__init__.py` & `Wavelink-2.3.1/wavelink/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 __title__ = "WaveLink"
 __author__ = "PythonistaGuild, EvieePy"
 __license__ = "MIT"
 __copyright__ = "Copyright 2019-Present (c) PythonistaGuild, EvieePy"
-__version__ = "2.3.0"
+__version__ = "2.3.1"
 
 from .enums import *
 from .exceptions import *
 from .node import *
 from .payloads import *
 from .player import Player as Player
 from .tracks import *
```

### Comparing `Wavelink-2.3.0/wavelink/backoff.py` & `Wavelink-2.3.1/wavelink/backoff.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.3.0/wavelink/enums.py` & `Wavelink-2.3.1/wavelink/enums.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.3.0/wavelink/exceptions.py` & `Wavelink-2.3.1/wavelink/exceptions.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.3.0/wavelink/ext/spotify/__init__.py` & `Wavelink-2.3.1/wavelink/ext/spotify/__init__.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.3.0/wavelink/filters.py` & `Wavelink-2.3.1/wavelink/filters.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.3.0/wavelink/node.py` & `Wavelink-2.3.1/wavelink/node.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.3.0/wavelink/payloads.py` & `Wavelink-2.3.1/wavelink/payloads.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.3.0/wavelink/player.py` & `Wavelink-2.3.1/wavelink/player.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,14 +196,18 @@
         return self._autoplay
 
     @autoplay.setter
     def autoplay(self, value: bool) -> None:
         """Set AutoPlay to True or False."""
         self._autoplay = value
 
+    def is_connected(self) -> bool:
+        """Whether the player is connected to a voice channel."""
+        return self.channel is not None and self.channel is not MISSING
+
     def is_playing(self) -> bool:
         """Whether the Player is currently playing a track."""
         return self.current is not None
 
     def is_paused(self) -> bool:
         """Whether the Player is currently paused."""
         return self._paused
@@ -552,22 +556,24 @@
             await self.seek(int(self.position))
         logger.debug(f"Set filter:: {self._filter} ({self.channel.id})")
 
     async def _destroy(self) -> None:
         self.autoplay = False
         self._voice_state = {}
         self._player_state = {}
+
         self.cleanup()
+        self.channel = None
 
         await self.current_node._send(method='DELETE',
                                       path=f'sessions/{self.current_node._session_id}/players',
                                       guild_id=self._guild.id)
 
-        del self.current_node._players[self.guild.id]
-        logger.debug(f'Player {self.guild.id} was destroyed.')
+        del self.current_node._players[self._guild.id]
+        logger.debug(f'Player {self._guild.id} was destroyed.')
 
     async def disconnect(self, **kwargs) -> None:
         """|coro|
 
         Disconnect the Player from voice and cleanup the Player state.
         """
         await self.guild.change_voice_state(channel=None)
```

### Comparing `Wavelink-2.3.0/wavelink/queue.py` & `Wavelink-2.3.1/wavelink/queue.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.3.0/wavelink/tracks.py` & `Wavelink-2.3.1/wavelink/tracks.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.3.0/wavelink/types/events.py` & `Wavelink-2.3.1/wavelink/types/events.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.3.0/wavelink/types/request.py` & `Wavelink-2.3.1/wavelink/types/request.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.3.0/wavelink/websocket.py` & `Wavelink-2.3.1/wavelink/websocket.py`

 * *Files identical despite different names*

