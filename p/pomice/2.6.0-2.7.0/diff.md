# Comparing `tmp/pomice-2.6.0.tar.gz` & `tmp/pomice-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pomice-2.6.0.tar", last modified: Sun May  7 23:28:20 2023, max compression
+gzip compressed data, was "pomice-2.7.0.tar", last modified: Sun May 21 14:43:59 2023, max compression
```

## Comparing `pomice-2.6.0.tar` & `pomice-2.7.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 23:28:20.265076 pomice-2.6.0/
--rw-rw-rw-   0        0        0    35823 2021-09-25 18:02:32.000000 pomice-2.6.0/LICENSE
--rw-rw-rw-   0        0        0     5445 2023-05-07 23:28:20.265076 pomice-2.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     4680 2023-04-23 18:14:31.000000 pomice-2.6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 23:28:20.231722 pomice-2.6.0/pomice/
--rw-rw-rw-   0        0        0      853 2023-05-07 23:27:35.000000 pomice-2.6.0/pomice/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-07 23:28:20.260114 pomice-2.6.0/pomice/applemusic/
--rw-rw-rw-   0        0        0      146 2023-04-29 18:05:44.000000 pomice-2.6.0/pomice/applemusic/__init__.py
--rw-rw-rw-   0        0        0     6682 2023-05-02 00:58:27.000000 pomice-2.6.0/pomice/applemusic/client.py
--rw-rw-rw-   0        0        0      321 2023-03-11 15:22:18.000000 pomice-2.6.0/pomice/applemusic/exceptions.py
--rw-rw-rw-   0        0        0     3573 2023-03-11 15:28:02.000000 pomice-2.6.0/pomice/applemusic/objects.py
--rw-rw-rw-   0        0        0     8043 2023-05-03 23:47:11.000000 pomice-2.6.0/pomice/enums.py
--rw-rw-rw-   0        0        0     6038 2023-03-13 23:36:22.000000 pomice-2.6.0/pomice/events.py
--rw-rw-rw-   0        0        0     2746 2023-03-12 15:44:18.000000 pomice-2.6.0/pomice/exceptions.py
--rw-rw-rw-   0        0        0    14832 2023-03-11 15:25:46.000000 pomice-2.6.0/pomice/filters.py
--rw-rw-rw-   0        0        0     5302 2023-04-23 18:14:31.000000 pomice-2.6.0/pomice/objects.py
--rw-rw-rw-   0        0        0    23940 2023-05-07 18:56:40.000000 pomice-2.6.0/pomice/player.py
--rw-rw-rw-   0        0        0    36635 2023-05-07 23:27:06.000000 pomice-2.6.0/pomice/pool.py
--rw-rw-rw-   0        0        0        0 2023-03-10 02:46:40.000000 pomice-2.6.0/pomice/py.typed
--rw-rw-rw-   0        0        0    12184 2023-03-27 02:26:04.000000 pomice-2.6.0/pomice/queue.py
--rw-rw-rw-   0        0        0     1069 2023-03-11 15:22:18.000000 pomice-2.6.0/pomice/routeplanner.py
-drwxrwxrwx   0        0        0        0 2023-05-07 23:28:20.263568 pomice-2.6.0/pomice/spotify/
--rw-rw-rw-   0        0        0      147 2023-03-11 15:22:18.000000 pomice-2.6.0/pomice/spotify/__init__.py
--rw-rw-rw-   0        0        0     6235 2023-05-02 01:01:06.000000 pomice-2.6.0/pomice/spotify/client.py
--rw-rw-rw-   0        0        0      301 2023-03-11 15:22:18.000000 pomice-2.6.0/pomice/spotify/exceptions.py
--rw-rw-rw-   0        0        0     3445 2023-04-23 18:14:31.000000 pomice-2.6.0/pomice/spotify/objects.py
--rw-rw-rw-   0        0        0     8697 2023-03-13 02:58:40.000000 pomice-2.6.0/pomice/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-07 23:28:20.255950 pomice-2.6.0/pomice.egg-info/
--rw-rw-rw-   0        0        0     5445 2023-05-07 23:28:20.000000 pomice-2.6.0/pomice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      628 2023-05-07 23:28:20.000000 pomice-2.6.0/pomice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 23:28:20.000000 pomice-2.6.0/pomice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-05-07 23:28:20.000000 pomice-2.6.0/pomice.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-07 23:28:20.000000 pomice-2.6.0/pomice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      369 2023-03-13 23:16:18.000000 pomice-2.6.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-07 23:28:20.265076 pomice-2.6.0/setup.cfg
--rw-rw-rw-   0        0        0     2185 2023-05-07 23:14:36.000000 pomice-2.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:59.394749 pomice-2.7.0/
+-rw-rw-rw-   0        0        0    35823 2021-09-25 18:02:32.000000 pomice-2.7.0/LICENSE
+-rw-rw-rw-   0        0        0     5445 2023-05-21 14:43:59.393717 pomice-2.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4680 2023-04-23 18:14:31.000000 pomice-2.7.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:59.194018 pomice-2.7.0/pomice/
+-rw-rw-rw-   0        0        0      853 2023-05-21 14:42:59.000000 pomice-2.7.0/pomice/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:59.333586 pomice-2.7.0/pomice/applemusic/
+-rw-rw-rw-   0        0        0      146 2023-04-29 18:05:44.000000 pomice-2.7.0/pomice/applemusic/__init__.py
+-rw-rw-rw-   0        0        0     6682 2023-05-02 00:58:27.000000 pomice-2.7.0/pomice/applemusic/client.py
+-rw-rw-rw-   0        0        0      321 2023-03-11 15:22:18.000000 pomice-2.7.0/pomice/applemusic/exceptions.py
+-rw-rw-rw-   0        0        0     3573 2023-03-11 15:28:02.000000 pomice-2.7.0/pomice/applemusic/objects.py
+-rw-rw-rw-   0        0        0     8043 2023-05-03 23:47:11.000000 pomice-2.7.0/pomice/enums.py
+-rw-rw-rw-   0        0        0     6038 2023-03-13 23:36:22.000000 pomice-2.7.0/pomice/events.py
+-rw-rw-rw-   0        0        0     2746 2023-03-12 15:44:18.000000 pomice-2.7.0/pomice/exceptions.py
+-rw-rw-rw-   0        0        0    17390 2023-05-21 14:42:36.000000 pomice-2.7.0/pomice/filters.py
+-rw-rw-rw-   0        0        0     5164 2023-05-08 14:41:29.000000 pomice-2.7.0/pomice/objects.py
+-rw-rw-rw-   0        0        0    26603 2023-05-21 14:42:39.000000 pomice-2.7.0/pomice/player.py
+-rw-rw-rw-   0        0        0    36694 2023-05-21 14:40:20.000000 pomice-2.7.0/pomice/pool.py
+-rw-rw-rw-   0        0        0        0 2023-03-10 02:46:40.000000 pomice-2.7.0/pomice/py.typed
+-rw-rw-rw-   0        0        0    12184 2023-03-27 02:26:04.000000 pomice-2.7.0/pomice/queue.py
+-rw-rw-rw-   0        0        0     1069 2023-03-11 15:22:18.000000 pomice-2.7.0/pomice/routeplanner.py
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:59.390759 pomice-2.7.0/pomice/spotify/
+-rw-rw-rw-   0        0        0      147 2023-03-11 15:22:18.000000 pomice-2.7.0/pomice/spotify/__init__.py
+-rw-rw-rw-   0        0        0     6235 2023-05-02 01:01:06.000000 pomice-2.7.0/pomice/spotify/client.py
+-rw-rw-rw-   0        0        0      301 2023-03-11 15:22:18.000000 pomice-2.7.0/pomice/spotify/exceptions.py
+-rw-rw-rw-   0        0        0     3445 2023-04-23 18:14:31.000000 pomice-2.7.0/pomice/spotify/objects.py
+-rw-rw-rw-   0        0        0     8697 2023-03-13 02:58:40.000000 pomice-2.7.0/pomice/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:59.245071 pomice-2.7.0/pomice.egg-info/
+-rw-rw-rw-   0        0        0     5445 2023-05-21 14:43:59.000000 pomice-2.7.0/pomice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      628 2023-05-21 14:43:59.000000 pomice-2.7.0/pomice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 14:43:59.000000 pomice-2.7.0/pomice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-05-21 14:43:59.000000 pomice-2.7.0/pomice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-21 14:43:59.000000 pomice-2.7.0/pomice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      369 2023-03-13 23:16:18.000000 pomice-2.7.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-21 14:43:59.395724 pomice-2.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     2185 2023-05-07 23:14:36.000000 pomice-2.7.0/setup.py
```

### Comparing `pomice-2.6.0/LICENSE` & `pomice-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pomice-2.6.0/PKG-INFO` & `pomice-2.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pomice
-Version: 2.6.0
+Version: 2.7.0
 Summary: The modern Lavalink wrapper designed for Discord.py
 Home-page: https://github.com/cloudwithax/pomice
 Author: cloudwithax
 License: GPL
 Keywords: pomice,lavalink,discord.py
 Classifier: Framework :: AsyncIO
 Classifier: Operating System :: OS Independent
```

### Comparing `pomice-2.6.0/README.md` & `pomice-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pomice-2.6.0/pomice/__init__.py` & `pomice-2.7.0/pomice/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     raise DiscordPyOutdated(
         "You must have discord.py (v2.0 or greater) to use this library. "
         "Uninstall your current version and install discord.py 2.0 "
         "using 'pip install discord.py'",
     )
 
-__version__ = "2.6.0"
+__version__ = "2.7.0"
 __title__ = "pomice"
 __author__ = "cloudwithax"
 __license__ = "GPL-3.0"
 __copyright__ = "Copyright (c) 2023, cloudwithax"
 
 from .enums import *
 from .events import *
```

### Comparing `pomice-2.6.0/pomice/applemusic/client.py` & `pomice-2.7.0/pomice/applemusic/client.py`

 * *Files identical despite different names*

### Comparing `pomice-2.6.0/pomice/applemusic/objects.py` & `pomice-2.7.0/pomice/applemusic/objects.py`

 * *Files identical despite different names*

### Comparing `pomice-2.6.0/pomice/enums.py` & `pomice-2.7.0/pomice/enums.py`

 * *Files identical despite different names*

### Comparing `pomice-2.6.0/pomice/events.py` & `pomice-2.7.0/pomice/events.py`

 * *Files identical despite different names*

### Comparing `pomice-2.6.0/pomice/exceptions.py` & `pomice-2.7.0/pomice/exceptions.py`

 * *Files identical despite different names*

### Comparing `pomice-2.6.0/pomice/filters.py` & `pomice-2.7.0/pomice/filters.py`

 * *Files 7% similar despite different names*

```diff
@@ -73,14 +73,20 @@
         data = [{"band": i, "gain": _dict[i]} for i in range(15)]
 
         return data
 
     def __repr__(self) -> str:
         return f"<Pomice.EqualizerFilter tag={self.tag} eq={self.eq} raw={self.raw}>"
 
+    def __eq__(self, __value: object) -> bool:
+        if not isinstance(__value, Equalizer):
+            return False
+
+        return self.raw == __value.raw
+
     @classmethod
     def flat(cls) -> "Equalizer":
         """Equalizer preset which represents a flat EQ board,
         with all levels set to their default values.
         """
 
         levels = [
@@ -227,14 +233,24 @@
         """
 
         return cls(tag="nightcore", speed=1.25, pitch=1.3)
 
     def __repr__(self) -> str:
         return f"<Pomice.TimescaleFilter tag={self.tag} speed={self.speed} pitch={self.pitch} rate={self.rate}>"
 
+    def __eq__(self, __value: object) -> bool:
+        if not isinstance(__value, Timescale):
+            return False
+
+        return (
+            self.speed == __value.speed
+            and self.pitch == __value.pitch
+            and self.rate == __value.rate
+        )
+
 
 class Karaoke(Filter):
     """Filter which filters the vocal track from any song and leaves the instrumental.
     Best for karaoke as the filter implies.
     """
 
     __slots__ = ("level", "mono_level", "filter_band", "filter_width")
@@ -266,14 +282,25 @@
 
     def __repr__(self) -> str:
         return (
             f"<Pomice.KaraokeFilter tag={self.tag} level={self.level} mono_level={self.mono_level} "
             f"filter_band={self.filter_band} filter_width={self.filter_width}>"
         )
 
+    def __eq__(self, __value: object) -> bool:
+        if not isinstance(__value, Karaoke):
+            return False
+
+        return (
+            self.level == __value.level
+            and self.mono_level == __value.mono_level
+            and self.filter_band == __value.filter_band
+            and self.filter_width == __value.filter_width
+        )
+
 
 class Tremolo(Filter):
     """Filter which produces a wavering tone in the music,
     causing it to sound like the music is changing in volume rapidly.
     """
 
     __slots__ = ("frequency", "depth")
@@ -301,14 +328,20 @@
         }
 
     def __repr__(self) -> str:
         return (
             f"<Pomice.TremoloFilter tag={self.tag} frequency={self.frequency} depth={self.depth}>"
         )
 
+    def __eq__(self, __value: object) -> bool:
+        if not isinstance(__value, Tremolo):
+            return False
+
+        return self.frequency == __value.frequency and self.depth == __value.depth
+
 
 class Vibrato(Filter):
     """Filter which produces a wavering tone in the music, similar to the Tremolo filter,
     but changes in pitch rather than volume.
     """
 
     __slots__ = ("frequency", "depth")
@@ -336,14 +369,20 @@
         }
 
     def __repr__(self) -> str:
         return (
             f"<Pomice.VibratoFilter tag={self.tag} frequency={self.frequency} depth={self.depth}>"
         )
 
+    def __eq__(self, __value: object) -> bool:
+        if not isinstance(__value, Vibrato):
+            return False
+
+        return self.frequency == __value.frequency and self.depth == __value.depth
+
 
 class Rotation(Filter):
     """Filter which produces a stereo-like panning effect, which sounds like
     the audio is being rotated around the listener's head
     """
 
     __slots__ = ("rotation_hertz",)
@@ -353,14 +392,20 @@
 
         self.rotation_hertz: float = rotation_hertz
         self.payload: dict = {"rotation": {"rotationHz": self.rotation_hertz}}
 
     def __repr__(self) -> str:
         return f"<Pomice.RotationFilter tag={self.tag} rotation_hertz={self.rotation_hertz}>"
 
+    def __eq__(self, __value: object) -> bool:
+        if not isinstance(__value, Rotation):
+            return False
+
+        return self.rotation_hertz == __value.rotation_hertz
+
 
 class ChannelMix(Filter):
     """Filter which manually adjusts the panning of the audio, which can make
     for some cool effects when done correctly.
     """
 
     __slots__ = (
@@ -414,14 +459,25 @@
 
     def __repr__(self) -> str:
         return (
             f"<Pomice.ChannelMix tag={self.tag} left_to_left={self.left_to_left} left_to_right={self.left_to_right} "
             f"right_to_left={self.right_to_left} right_to_right={self.right_to_right}>"
         )
 
+    def __eq__(self, __value: object) -> bool:
+        if not isinstance(__value, ChannelMix):
+            return False
+
+        return (
+            self.left_to_left == __value.left_to_left
+            and self.left_to_right == __value.left_to_right
+            and self.right_to_left == __value.right_to_left
+            and self.right_to_right == __value.right_to_right
+        )
+
 
 class Distortion(Filter):
     """Filter which generates a distortion effect. Useful for certain filter implementations where
     distortion is needed.
     """
 
     __slots__ = (
@@ -475,14 +531,29 @@
     def __repr__(self) -> str:
         return (
             f"<Pomice.Distortion tag={self.tag} sin_offset={self.sin_offset} sin_scale={self.sin_scale}> "
             f"cos_offset={self.cos_offset} cos_scale={self.cos_scale} tan_offset={self.tan_offset} "
             f"tan_scale={self.tan_scale} offset={self.offset} scale={self.scale}"
         )
 
+    def __eq__(self, __value: object) -> bool:
+        if not isinstance(__value, Distortion):
+            return False
+
+        return (
+            self.sin_offset == __value.sin_offset
+            and self.sin_scale == __value.sin_scale
+            and self.cos_offset == __value.cos_offset
+            and self.cos_scale == __value.cos_scale
+            and self.tan_offset == __value.tan_offset
+            and self.tan_scale == __value.tan_scale
+            and self.offset == __value.offset
+            and self.scale == __value.scale
+        )
+
 
 class LowPass(Filter):
     """Filter which supresses higher frequencies and allows lower frequencies to pass.
     You can also do this with the Equalizer filter, but this is an easier way to do it.
     """
 
     __slots__ = ("smoothing", "payload")
@@ -491,7 +562,13 @@
         super().__init__(tag=tag)
 
         self.smoothing: float = smoothing
         self.payload: dict = {"lowPass": {"smoothing": self.smoothing}}
 
     def __repr__(self) -> str:
         return f"<Pomice.LowPass tag={self.tag} smoothing={self.smoothing}>"
+
+    def __eq__(self, __value: object) -> bool:
+        if not isinstance(__value, LowPass):
+            return False
+
+        return self.smoothing == __value.smoothing
```

### Comparing `pomice-2.6.0/pomice/objects.py` & `pomice-2.7.0/pomice/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,17 +94,14 @@
         if not self.requester and self.ctx:
             self.requester = self.ctx.author
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, Track):
             return False
 
-        if self.ctx and other.ctx:
-            return other.track_id == self.track_id and other.ctx.message.id == self.ctx.message.id
-
         return other.track_id == self.track_id
 
     def __str__(self) -> str:
         return self.title
 
     def __repr__(self) -> str:
         return f"<Pomice.track title={self.title!r} uri=<{self.uri!r}> length={self.length}>"
```

### Comparing `pomice-2.6.0/pomice/player.py` & `pomice-2.7.0/pomice/player.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,14 +75,35 @@
         if not any(f for f in self._filters if f.tag == filter_tag):
             raise FilterTagInvalid("A filter with that tag was not found.")
 
         for index, filter in enumerate(self._filters):
             if filter.tag == filter_tag:
                 del self._filters[index]
 
+    def edit_filter(self, *, filter_tag: str, to_apply: Filter) -> None:
+        """Edits a filter in the list of filters applied using its filter tag and replaces it with the new filter."""
+        if not any(f for f in self._filters if f.tag == filter_tag):
+            raise FilterTagInvalid("A filter with that tag was not found.")
+
+        for index, filter in enumerate(self._filters):
+            if filter.tag == filter_tag:
+                if not type(filter) == type(to_apply):
+                    raise FilterInvalidArgument(
+                        "Edited filter is not the same type as the current filter.",
+                    )
+                if self._filters[index] == to_apply:
+                    raise FilterInvalidArgument("Edited filter is the same as the current filter.")
+
+                if to_apply.tag != filter_tag:
+                    raise FilterInvalidArgument(
+                        "Edited filter tag is not the same as the current filter tag.",
+                    )
+
+                self._filters[index] = to_apply
+
     def has_filter(self, *, filter_tag: str) -> bool:
         """Checks if a filter exists in the list of filters using its filter tag"""
         return any(f for f in self._filters if f.tag == filter_tag)
 
     def has_filter_type(self, *, filter_type: Filter) -> bool:
         """Checks if any filters applied match the specified filter type."""
         return any(f for f in self._filters if type(f) == type(filter_type))
@@ -378,14 +399,24 @@
         Context object on any track you search.
 
         You may also pass in a List of filters
         to be applied to your track once it plays.
         """
         return await self._node.get_tracks(query, ctx=ctx, search_type=search_type, filters=filters)
 
+    async def build_track(self, identifier: str, ctx: Optional[commands.Context] = None) -> Track:
+        """
+        Builds a track using a valid track identifier
+
+        You can also pass in a discord.py Context object to get a
+        Context object on the track it builds.
+        """
+
+        return await self._node.build_track(identifier, ctx=ctx)
+
     async def get_recommendations(
         self, *, track: Track, ctx: Optional[commands.Context] = None
     ) -> Optional[Union[List[Track], Playlist]]:
         """
         Gets recommendations from either YouTube or Spotify.
         You can pass in a discord.py Context object to get a
         Context object on all tracks that get recommended.
@@ -427,15 +458,15 @@
     async def destroy(self) -> None:
         """Disconnects and destroys the player, and runs internal cleanup."""
         try:
             await self.disconnect()
         except AttributeError:
             # 'NoneType' has no attribute '_get_voice_client_key' raised by self.cleanup() ->
             # assume we're already disconnected and cleaned up
-            assert not self.is_connected and not self.channel
+            assert self.channel is None and not self.is_connected
 
         self._node._players.pop(self.guild.id)
         if self.node.is_connected:
             await self._node.send(
                 method="DELETE",
                 path=self._player_endpoint_uri,
                 guild_id=self._guild.id,
@@ -633,14 +664,41 @@
         self._log.debug(f"Filter has been removed from player with tag {filter_tag}")
         if fast_apply:
             self._log.debug(f"Fast apply passed, now removing filter instantly.")
             await self.seek(self.position)
 
         return self._filters
 
+    async def edit_filter(
+        self, *, filter_tag: str, edited_filter: Filter, fast_apply: bool = False
+    ) -> Filters:
+        """Edits a filter from the player using its filter tag and a new filter of the same type.
+        The filter to be replaced must have the same tag as the one you are replacing it with.
+        This will only work if you are using a version of Lavalink that supports filters.
+
+        If you would like for the filter to apply instantly, set the `fast_apply` arg to `True`.
+
+        (You must have a song playing in order for `fast_apply` to work.)
+        """
+
+        self._filters.edit_filter(filter_tag=filter_tag, to_apply=edited_filter)
+        payload = self._filters.get_all_payloads()
+        await self._node.send(
+            method="PATCH",
+            path=self._player_endpoint_uri,
+            guild_id=self._guild.id,
+            data={"filters": payload},
+        )
+        self._log.debug(f"Filter with tag {filter_tag} has been edited to {edited_filter!r}")
+        if fast_apply:
+            self._log.debug(f"Fast apply passed, now editing filter instantly.")
+            await self.seek(self.position)
+
+        return self._filters
+
     async def reset_filters(self, *, fast_apply: bool = False) -> None:
         """Resets all currently applied filters to their default parameters.
          You must have filters applied in order for this to work.
          If you would like the filters to be removed instantly, set the `fast_apply` arg to `True`.
 
         (You must have a song playing in order for `fast_apply` to work.)
         """
```

### Comparing `pomice-2.6.0/pomice/pool.py` & `pomice-2.7.0/pomice/pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         pool: Type[NodePool],
         bot: commands.Bot,
         host: str,
         port: int,
         password: str,
         identifier: str,
         secure: bool = False,
-        heartbeat: int = 60,
+        heartbeat: int = 120,
         resume_key: Optional[str] = None,
         resume_timeout: int = 60,
         loop: Optional[asyncio.AbstractEventLoop] = None,
         session: Optional[aiohttp.ClientSession] = None,
         spotify_client_id: Optional[str] = None,
         spotify_client_secret: Optional[str] = None,
         apple_music: bool = False,
@@ -230,21 +230,23 @@
     @property
     def ping(self) -> float:
         """Alias for `Node.latency`, returns the latency of the node"""
         return self.latency
 
     def _setup_logging(self, level: LogLevel) -> logging.Logger:
         logger = logging.getLogger("pomice")
-        logger.setLevel(level)
+
         handler = None
 
         if self._log_handler:
             handler = self._log_handler
+            logger.setLevel(handler.level)
         else:
             handler = logging.StreamHandler()
+            logger.setLevel(level)
             dt_fmt = "%Y-%m-%d %H:%M:%S"
             formatter = logging.Formatter(
                 "[{asctime}] [{levelname:<8}] {name}: {message}",
                 dt_fmt,
                 style="{",
             )
             handler.setFormatter(formatter)
@@ -540,15 +542,15 @@
         You can also pass in a discord.py Context object to get a
         Context object on the track it builds.
         """
 
         data: dict = await self.send(
             method="GET",
             path="decodetrack",
-            query=f"encodedTrack={identifier}",
+            query=f"encodedTrack={quote(identifier)}",
         )
         return Track(
             track_id=identifier,
             ctx=ctx,
             info=data,
             track_type=TrackType(data["sourceName"]),
         )
@@ -956,15 +958,15 @@
         *,
         bot: commands.Bot,
         host: str,
         port: int,
         password: str,
         identifier: str,
         secure: bool = False,
-        heartbeat: int = 30,
+        heartbeat: int = 120,
         resume_key: Optional[str] = None,
         resume_timeout: int = 60,
         loop: Optional[asyncio.AbstractEventLoop] = None,
         spotify_client_id: Optional[str] = None,
         spotify_client_secret: Optional[str] = None,
         session: Optional[aiohttp.ClientSession] = None,
         apple_music: bool = False,
```

### Comparing `pomice-2.6.0/pomice/queue.py` & `pomice-2.7.0/pomice/queue.py`

 * *Files identical despite different names*

### Comparing `pomice-2.6.0/pomice/routeplanner.py` & `pomice-2.7.0/pomice/routeplanner.py`

 * *Files identical despite different names*

### Comparing `pomice-2.6.0/pomice/spotify/client.py` & `pomice-2.7.0/pomice/spotify/client.py`

 * *Files identical despite different names*

### Comparing `pomice-2.6.0/pomice/spotify/objects.py` & `pomice-2.7.0/pomice/spotify/objects.py`

 * *Files identical despite different names*

### Comparing `pomice-2.6.0/pomice/utils.py` & `pomice-2.7.0/pomice/utils.py`

 * *Files identical despite different names*

### Comparing `pomice-2.6.0/pomice.egg-info/PKG-INFO` & `pomice-2.7.0/pomice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pomice
-Version: 2.6.0
+Version: 2.7.0
 Summary: The modern Lavalink wrapper designed for Discord.py
 Home-page: https://github.com/cloudwithax/pomice
 Author: cloudwithax
 License: GPL
 Keywords: pomice,lavalink,discord.py
 Classifier: Framework :: AsyncIO
 Classifier: Operating System :: OS Independent
```

### Comparing `pomice-2.6.0/pomice.egg-info/SOURCES.txt` & `pomice-2.7.0/pomice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pomice-2.6.0/setup.py` & `pomice-2.7.0/setup.py`

 * *Files identical despite different names*

