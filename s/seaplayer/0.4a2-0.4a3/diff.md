# Comparing `tmp/seaplayer-0.4a2.tar.gz` & `tmp/seaplayer-0.4a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaplayer-0.4a2.tar", max compression
+gzip compressed data, was "seaplayer-0.4a3.tar", max compression
```

## Comparing `seaplayer-0.4a2.tar` & `seaplayer-0.4a3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1085 2023-04-25 14:05:19.406661 seaplayer-0.4a2/LICENSE
--rw-r--r--   0        0        0     1020 2023-05-18 20:26:18.598974 seaplayer-0.4a2/pyproject.toml
--rw-r--r--   0        0        0     1313 2023-05-18 14:07:36.121280 seaplayer-0.4a2/README.md
--rw-r--r--   0        0        0        0 2023-05-02 23:42:08.763410 seaplayer-0.4a2/seaplayer/__init__.py
--rw-r--r--   0        0        0      295 2023-05-17 19:11:05.795693 seaplayer-0.4a2/seaplayer/__main__.py
--rw-r--r--   0        0        0    14705 2023-05-10 21:24:30.252393 seaplayer-0.4a2/seaplayer/assets/image-not-found.png
--rw-r--r--   0        0        0     4485 2023-05-18 16:45:40.489905 seaplayer-0.4a2/seaplayer/codecs.py
--rw-r--r--   0        0        0     1855 2023-05-18 18:50:26.106124 seaplayer-0.4a2/seaplayer/codeсbase.py
--rw-r--r--   0        0        0     5851 2023-05-18 20:05:55.893843 seaplayer-0.4a2/seaplayer/config.py
--rw-r--r--   0        0        0        0 2023-05-03 15:09:20.919585 seaplayer-0.4a2/seaplayer/css/configurate.css
--rw-r--r--   0        0        0     1276 2023-05-18 19:49:57.345669 seaplayer-0.4a2/seaplayer/css/objects.css
--rw-r--r--   0        0        0      595 2023-05-18 18:14:38.497674 seaplayer-0.4a2/seaplayer/css/seaplayer.css
--rw-r--r--   0        0        0      278 2023-05-02 23:29:23.509840 seaplayer-0.4a2/seaplayer/css/unknown.css
--rw-r--r--   0        0        0      374 2023-05-10 16:57:45.981727 seaplayer-0.4a2/seaplayer/exceptions.py
--rw-r--r--   0        0        0     1278 2023-05-18 18:50:16.289839 seaplayer-0.4a2/seaplayer/functions.py
--rw-r--r--   0        0        0        0 2023-05-02 22:35:56.414811 seaplayer-0.4a2/seaplayer/modules/__init__.py
--rw-r--r--   0        0        0     2036 2023-05-12 20:40:27.939248 seaplayer-0.4a2/seaplayer/modules/colorizer.py
--rw-r--r--   0        0        0    12491 2023-05-18 20:18:31.524159 seaplayer-0.4a2/seaplayer/objects.py
--rw-r--r--   0        0        0     6228 2023-05-18 20:09:52.552803 seaplayer-0.4a2/seaplayer/screens.py
--rw-r--r--   0        0        0    16796 2023-05-18 20:27:03.188052 seaplayer-0.4a2/seaplayer/seaplayer.py
--rw-r--r--   0        0        0     4159 2023-05-18 12:58:01.336447 seaplayer-0.4a2/seaplayer/types.py
--rw-r--r--   0        0        0     2330 1970-01-01 00:00:00.000000 seaplayer-0.4a2/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-04-25 14:05:19.406661 seaplayer-0.4a3/LICENSE
+-rw-r--r--   0        0        0     1020 2023-05-19 19:33:28.838346 seaplayer-0.4a3/pyproject.toml
+-rw-r--r--   0        0        0     1313 2023-05-18 14:07:36.121280 seaplayer-0.4a3/README.md
+-rw-r--r--   0        0        0        0 2023-05-02 23:42:08.763410 seaplayer-0.4a3/seaplayer/__init__.py
+-rw-r--r--   0        0        0      295 2023-05-17 19:11:05.795693 seaplayer-0.4a3/seaplayer/__main__.py
+-rw-r--r--   0        0        0    14705 2023-05-10 21:24:30.252393 seaplayer-0.4a3/seaplayer/assets/image-not-found.png
+-rw-r--r--   0        0        0     4485 2023-05-18 16:45:40.489905 seaplayer-0.4a3/seaplayer/codecs.py
+-rw-r--r--   0        0        0     1855 2023-05-18 18:50:26.106124 seaplayer-0.4a3/seaplayer/codeсbase.py
+-rw-r--r--   0        0        0     5851 2023-05-18 20:05:55.893843 seaplayer-0.4a3/seaplayer/config.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:09:20.919585 seaplayer-0.4a3/seaplayer/css/configurate.css
+-rw-r--r--   0        0        0     1447 2023-05-19 19:05:56.985432 seaplayer-0.4a3/seaplayer/css/objects.css
+-rw-r--r--   0        0        0      595 2023-05-19 18:52:39.760564 seaplayer-0.4a3/seaplayer/css/seaplayer.css
+-rw-r--r--   0        0        0      278 2023-05-02 23:29:23.509840 seaplayer-0.4a3/seaplayer/css/unknown.css
+-rw-r--r--   0        0        0      382 2023-05-19 19:34:40.039165 seaplayer-0.4a3/seaplayer/exceptions.py
+-rw-r--r--   0        0        0     1278 2023-05-19 19:35:29.716179 seaplayer-0.4a3/seaplayer/functions.py
+-rw-r--r--   0        0        0        0 2023-05-02 22:35:56.414811 seaplayer-0.4a3/seaplayer/modules/__init__.py
+-rw-r--r--   0        0        0     2036 2023-05-12 20:40:27.939248 seaplayer-0.4a3/seaplayer/modules/colorizer.py
+-rw-r--r--   0        0        0    13356 2023-05-19 19:02:05.310349 seaplayer-0.4a3/seaplayer/objects.py
+-rw-r--r--   0        0        0     6778 2023-05-19 19:45:06.250790 seaplayer-0.4a3/seaplayer/screens.py
+-rw-r--r--   0        0        0    17707 2023-05-19 19:30:43.886684 seaplayer-0.4a3/seaplayer/seaplayer.py
+-rw-r--r--   0        0        0     4159 2023-05-18 12:58:01.336447 seaplayer-0.4a3/seaplayer/types.py
+-rw-r--r--   0        0        0     2330 1970-01-01 00:00:00.000000 seaplayer-0.4a3/PKG-INFO
```

### Comparing `seaplayer-0.4a2/LICENSE` & `seaplayer-0.4a3/LICENSE`

 * *Files identical despite different names*

### Comparing `seaplayer-0.4a2/pyproject.toml` & `seaplayer-0.4a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "SeaPlayer"
-version = "0.4a2"
+version = "0.4a3"
 description = "SeaPlayer is a player that works in the terminal."
 repository = "https://github.com/romanin-rf/SeaPlayer"
 authors = ["Romanin <semina054@gmail.com>"]
 keywords = ["tui", "player", "seaplayer", "wav", "mp3", "ogg", "midi"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "seaplayer" }]
```

### Comparing `seaplayer-0.4a2/README.md` & `seaplayer-0.4a3/README.md`

 * *Files identical despite different names*

### Comparing `seaplayer-0.4a2/seaplayer/assets/image-not-found.png` & `seaplayer-0.4a3/seaplayer/assets/image-not-found.png`

 * *Files identical despite different names*

### Comparing `seaplayer-0.4a2/seaplayer/codecs.py` & `seaplayer-0.4a3/seaplayer/codecs.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.4a2/seaplayer/codeсbase.py` & `seaplayer-0.4a3/seaplayer/codeсbase.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.4a2/seaplayer/config.py` & `seaplayer-0.4a3/seaplayer/config.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.4a2/seaplayer/css/objects.css` & `seaplayer-0.4a3/seaplayer/css/objects.css`

 * *Files 10% similar despite different names*

```diff
@@ -68,8 +68,19 @@
 
 .log-menu:focus {
     offset: 0 0 !important;
 }
 
 .log-menu.-hidden {
     offset-y: 100%;
+}
+
+Nofy {
+    dock: top;
+    layer: nofys;
+    width: auto;
+    margin: 2 4;
+    padding: 1 2;
+    background: $background;
+    color: $text;
+    height: auto;
 }
```

### Comparing `seaplayer-0.4a2/seaplayer/css/seaplayer.css` & `seaplayer-0.4a3/seaplayer/css/seaplayer.css`

 * *Files identical despite different names*

### Comparing `seaplayer-0.4a2/seaplayer/functions.py` & `seaplayer-0.4a3/seaplayer/functions.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.4a2/seaplayer/modules/colorizer.py` & `seaplayer-0.4a3/seaplayer/modules/colorizer.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.4a2/seaplayer/objects.py` & `seaplayer-0.4a3/seaplayer/objects.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from PIL import Image
 # > Graphics
 from PIL.Image import Resampling
 from ripix import AsyncPixels, Pixels
 from rich.progress import Progress, BarColumn, TextColumn
 from textual.widgets import Static, Label, ListItem, ListView, Input, TextLog
 # > Typing
-from typing import Optional, Tuple, TypeVar, Union, Any, Dict
+from typing import Optional, Tuple, TypeVar, Union, Any, Literal
 # > Local Import's
 from .types import MusicList
 from .codeсbase import CodecBase
 from .functions import (
     aiter,
     get_bar_status,
     get_sound_basename
@@ -293,18 +293,40 @@
     def __init__(self, *children, **kwargs):
         kwargs["classes"] = "configurate-list-view"
         super().__init__(*children, **kwargs)
         self.border_title = "Configurate"
 
 # ! Log Menu
 class LogMenu(TextLog):
-    def __init__(self, enable_logging: bool=True, **kwargs):
+    def __init__(self, chap_max_width: int=8, enable_logging: bool=True, **kwargs):
         self.enable_logging = enable_logging
+        self.chap_max_width = chap_max_width
+        
         if kwargs.get("classes", None) is not None:
             kwargs["classes"] = kwargs["classes"] + " log-menu -hidden"
         else:
             kwargs["classes"] = "log-menu -hidden"
+        
         super().__init__(**kwargs)
     
-    def wlog(self, chap: str, msg: str, *, cc: str="green") -> None:
-        if self.enable_logging:
-            self.write(f"[[{cc}]{chap.center(8)}[/]]: {msg}\n")
+    def write_log(self, chap: str, msg: str, *, chap_color: str="green") -> None:
+        if self.enable_logging: self.write(f"[[{chap_color}]{chap.center(self.chap_max_width)}[/]]: {msg}", shrink=False)
+    
+    def info(self, msg: str) -> None: self.write_log("INFO", msg, chap_color="green")
+    def error(self, msg: str) -> None: self.write_log("ERROR", msg, chap_color="red")
+    def warn(self, msg: str) -> None: self.write_log("WARN", msg, chap_color="orange")
+
+# ! Nofy
+class Nofy(Static):
+    def __init__(
+        self,
+        text: str,
+        life_time: float=3,
+        dosk: Literal["bottom", "left", "right", "top"]="top",
+        **kwargs
+    ) -> None:
+        super().__init__(text, **kwargs)
+        self.life_time = life_time
+        self.styles.dock = dosk
+    
+    def on_mount(self) -> None: self.set_timer(self.life_time, self.remove)
+    async def on_click(self) -> None: await self.remove()
```

### Comparing `seaplayer-0.4a2/seaplayer/screens.py` & `seaplayer-0.4a3/seaplayer/screens.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,20 @@
 from textual.screen import Screen
 from textual.widgets import Static, Header, Footer
 # > Typing
 from typing import Optional, Literal
 # > Local Imports
 from .types import Converter
 from .modules.colorizer import richefication
-from .objects import ConfigurateListView, ConfigurateListItem, InputField
+from .objects import (
+    Nofy,
+    InputField,
+    ConfigurateListView,
+    ConfigurateListItem
+)
 
 # ! Constants
 TEXT = b'CkFuIGVycm9yIGhhcyBvY2N1cnJlZC4gVG8gY29udGludWU6CgpQcmVzcyBFbnRlciB0byByZXR1cm4gdG8ge3N5c3RlbX0sIG9yCgpQcmVzcyBDVFJMK0FMVCtERUwgdG8gcmVzdGFydCB5b3VyIGNvbXB1dGVyLiBJZiB5b3UgZG8gdGhpcywKeW91IHdpbGwgbG9zZSBhbnkgdW5zYXZlZCBpbmZvcm1hdGlvbiBpbiBhbGwgb3BlbiBhcHBsaWNhdGlvbnMuCgpFcnJvcjogMEUgOiAwMTZGIDogQkZGOUIzRDQK'
 TEXT = base64.b64decode(TEXT).decode(errors="ignore").format(system=platform.system())
 UNKNOWN_OPEN_KEY = base64.b64decode(b"Yg==").decode(errors="ignore")
 
 # ! Initializing
@@ -30,23 +35,41 @@
         yield Static("Press any key to continue [blink]_[/]", id="unknown-any-key")
 
 
 class Configurate(Screen):
     """This Configurate Menu screen."""
     BINDINGS = [("escape", "app.pop_screen", "Back")]
     
+    # ! Nofy Functions
+    def nofy(
+        self,
+        text: str,
+        life_time: float=3,
+        dosk: Literal["bottom", "left", "right", "top"]="top"
+    ) -> None:
+        self.screen.mount(Nofy(text, life_time, dosk))
+    
+    async def aio_nofy(
+        self,
+        text: str,
+        life_time: float=3,
+        dosk: Literal["bottom", "left", "right", "top"]="top"
+    ) -> None:
+        await self.screen.mount(Nofy(text, life_time, dosk))
+    
     # ! Update Placeholder from InputField
     def _upfif(self, attr_name: str) -> str:
         return "Currect: " + str(eval(f"self.{attr_name}"))
     def gupfif(self, attr_name: str):
         return lambda: self._upfif(attr_name)
     
     # ! Update App Config
     async def _uac(self, attr_name: str, input: InputField, value: str) -> None:
         exec(f"self.{attr_name} = value")
+        await self.aio_nofy("Saved!")
     
     def guac(self, attr_name: str):
         async def an_uac(input: InputField, value: str) -> None: await self._uac(attr_name, input, value)
         return an_uac
 
     # ! Configurator Generators
     def create_configurator_type(
```

### Comparing `seaplayer-0.4a2/seaplayer/seaplayer.py` & `seaplayer-0.4a3/seaplayer/seaplayer.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,58 +22,69 @@
 from .functions import (
     aiter,
     check_status,
     image_from_bytes,
     get_sound_basename
 )
 from .objects import (
+    Nofy,
     LogMenu,
     InputField,
     MusicListView,
     AsyncImageLabel,
     MusicListViewItem,
     StandartImageLabel,
     IndeterminateProgress
 )
 
 # ! Metadata
 __title__ = "SeaPlayer"
-__version__ = "0.4a2"
+__version__ = "0.4a3"
 __author__ = "Romanin"
 __email__ = "semina054@gmail.com"
 __url__ = "https://github.com/romanin-rf/SeaPlayer"
 
 # ! Paths
 if getattr(sys, 'frozen', False) and hasattr(sys, '_MEIPASS'):
     LOCALDIR = os.path.dirname(sys.executable)
 else:
     LOCALDIR = os.path.dirname(os.path.dirname(__file__))
 
 CSS_LOCALDIR = os.path.join(os.path.dirname(__file__), "css")
 ASSETS_DIRPATH = os.path.join(os.path.dirname(__file__), "assets")
 
-CONFIG_DIRPATH = os.path.abspath(user_config_dir(__title__, __author__))
+CONFIG_DIRPATH = user_config_dir(__title__, __author__, ensure_exists=True)
 CONFIG_FILEPATH = os.path.join(CONFIG_DIRPATH, "config.properties")
 
-# ! Initialized Directoryes
-os.makedirs(CONFIG_DIRPATH, mode=644, exist_ok=True)
-
 # ! Assets Paths
 IMGPATH_IMAGE_NOT_FOUND = os.path.join(ASSETS_DIRPATH, "image-not-found.png")
 
 # ! Constants
 RESAMPLING_SAFE = {
     "nearest": Resampling.NEAREST,
     "bilinear": Resampling.BILINEAR,
     "bicubic": Resampling.BICUBIC,
     "lanczos": Resampling.LANCZOS,
     "hamming": Resampling.HAMMING,
     "box": Resampling.BOX
 }
 
+# ! Main Functions
+def build_bindings(config: SeaPlayerConfig):
+    yield Binding(config.key_quit, "quit", "Quit")
+    yield Binding("c,с", "push_screen('configurate')", "Configurate")
+    if config.log_menu_enable:
+        yield Binding("l,д", "app.toggle_class('.log-menu', '-hidden')", 'Logs')
+    yield Binding(config.key_rewind_back, "minus_rewind", f"Rewind -{config.rewind_count_seconds} sec")
+    yield Binding(config.key_rewind_forward, "plus_rewind", f"Rewind +{config.rewind_count_seconds} sec")
+    yield Binding(config.key_volume_down, "minus_volume", f"Volume -{round(config.volume_change_percent*100)}%")
+    yield Binding(config.key_volume_up, "plus_volume", f"Volume +{round(config.volume_change_percent*100)}%")
+    yield Binding("ctrl+s", "screenshot", "Screenshot")
+    yield Binding(UNKNOWN_OPEN_KEY, "push_screen('unknown')", "None", show=False)
+
 # ! Main
 class SeaPlayer(App):
     # ! Textual Configuration
     TITLE = f"{__title__} v{__version__}"
     CSS_PATH = [
         os.path.join(CSS_LOCALDIR, "seaplayer.css"),
         os.path.join(CSS_LOCALDIR, "configurate.css"),
@@ -86,27 +97,15 @@
     }
     
     # ! SeaPlayer Configuration
     config = SeaPlayerConfig(CONFIG_FILEPATH)
     max_volume_percent: float = config.max_volume_percent
     
     # ! Textual Keys Configuration
-    BINDINGS = [
-        Binding(config.key_quit, "quit", "Quit", priority=True),
-        Binding("c,с", "push_screen('configurate')", "Configurate", priority=True),
-        #Binding("l,д", "app.toggle_class('.log-menu', '-hidden')", 'Logs'),
-        Binding(config.key_rewind_back, "minus_rewind", f"Rewind -{config.rewind_count_seconds} sec"),
-        Binding(config.key_rewind_forward, "plus_rewind", f"Rewind +{config.rewind_count_seconds} sec"),
-        Binding(config.key_volume_down, "minus_volume", f"Volume -{round(config.volume_change_percent*100)}%"),
-        Binding(config.key_volume_up, "plus_volume", f"Volume +{round(config.volume_change_percent*100)}%"),
-        Binding("ctrl+s", "screenshot", "Screenshot"),
-        Binding(UNKNOWN_OPEN_KEY, "push_screen('unknown')", "None", show=False)
-    ]
-    if config.log_menu_enable:
-        BINDINGS.append(Binding("l,д", "app.toggle_class('.log-menu', '-hidden')", 'Logs', priority=True))
+    BINDINGS = list(build_bindings(config))
     
     # ! Template Configuration
     currect_sound_uuid: Optional[str] = None
     currect_sound: Optional[CodecBase] = None
     currect_volume = 1.0
     last_playback_status: Optional[Literal["Stoped", "Playing", "Paused"]] = None
     playback_mode: int = 0
@@ -114,20 +113,44 @@
     last_paths_globalized: List[str] = []
     started: bool = True
     
     # ! Codecs Configuration
     CODECS: List[Type[CodecBase]] = [ MP3Codec, WAVECodec, OGGCodec, MIDICodec ]
     CODECS_KWARGS: Dict[str, Any] = {"sound_font_path": config.sound_font_path}
     
+    # ! Init Objects
+    log_menu = LogMenu(enable_logging=config.log_menu_enable, wrap=True, highlight=True, markup=True)
+    
+    # ! Log Functions
+    info = log_menu.info
+    error = log_menu.error
+    warn = log_menu.warn
+    
     # ! Inherited Functions
     async def action_push_screen(self, screen: str) -> None:
         if self.SCREENS[screen].id != self.screen.id:
             await super().action_push_screen(screen)
     
     # ! Functions, Workers and other...
+    def nofy(
+        self,
+        text: str,
+        life_time: float=3,
+        dosk: Literal["bottom", "left", "right", "top"]="top"
+    ) -> None:
+        self.screen.mount(Nofy(text, life_time, dosk))
+    
+    async def aio_nofy(
+        self,
+        text: str,
+        life_time: float=3,
+        dosk: Literal["bottom", "left", "right", "top"]="top"
+    ) -> None:
+        await self.screen.mount(Nofy(text, life_time, dosk))
+    
     def gcs(self) -> Optional[CodecBase]:
         if (self.currect_sound is None) and (self.currect_sound_uuid is not None):
             self.currect_sound = self.music_list_view.music_list.get(self.currect_sound_uuid)
         return self.currect_sound
     
     async def aio_gcs(self):
         if (self.currect_sound is None) and (self.currect_sound_uuid is not None):
@@ -162,45 +185,47 @@
                 status = check_status(sound)
                 if (self.last_playback_status is not None) and (self.last_playback_status != status):
                     self.music_selected_label.update(await self.aio_get_sound_selected_label_text())
                 
                 if (status == "Stoped") and (self.last_playback_status == "Playing"):
                     if self.playback_mode == 1:
                         sound.play()
-                        self.log_menu.wlog("INFO", f"Replay sound: {repr(sound)}")
+                        self.info(f"Replay sound: {repr(sound)}")
                     elif self.playback_mode == 2:
                         if (sound:=await self.set_sound_for_playback(sound_uuid:=await self.music_list_view.aio_get_next_sound_uuid(self.currect_sound_uuid), True)) is not None:
                             self.playback_mode_blocked = True
                             await self.music_list_view.aio_select_list_item_from_sound_uuid(sound_uuid)
                             sound.play()
-                            self.log_menu.wlog("INFO", f"Playing the next sound: {repr(sound)}")
+                            self.info(f"Playing the next sound: {repr(sound)}")
                 
                 self.last_playback_status = status
             await asyncio.sleep(0.33)
     
     def compose(self) -> ComposeResult:
         # * Other
-        self.log_menu = LogMenu(enable_logging=(self.config.log_menu_enable), wrap=True, highlight=True, markup=True)
-        self.log_menu.wlog("INFO", f"Codecs: {repr(self.CODECS)}")
+        self.info(f"{__title__} v{__version__} from {__author__} ({__email__})")
+        self.info(f"Source         : {__url__}")
+        self.info(f"Codecs         : {repr(self.CODECS)}")
+        self.info(f"Config Path    : {repr(self.config.filepath)}")
+        self.info(f"CSS Dirpath    : {repr(CSS_LOCALDIR)}")
+        self.info(f"Assets Dirpath : {repr(ASSETS_DIRPATH)}")
         
         # * Play Screen
         self.music_play_screen = Static(classes="screen-box")
         self.music_play_screen.border_title = "Player"
         
-        img_image_not_found = Image.open(IMGPATH_IMAGE_NOT_FOUND)
-        
+        # * Image Object Init
         self.music_selected_label = Label(self.get_sound_selected_label_text(), classes="music-selected-label")
         if self.config.image_update_method == "sync":
-            self.music_image = StandartImageLabel(img_image_not_found, resample=RESAMPLING_SAFE[self.config.image_resample_method])
+            self.music_image = StandartImageLabel(Image.open(IMGPATH_IMAGE_NOT_FOUND), resample=RESAMPLING_SAFE[self.config.image_resample_method])
         elif self.config.image_update_method == "async":
-            self.music_image = AsyncImageLabel(img_image_not_found, resample=RESAMPLING_SAFE[self.config.image_resample_method])
+            self.music_image = AsyncImageLabel(Image.open(IMGPATH_IMAGE_NOT_FOUND), resample=RESAMPLING_SAFE[self.config.image_resample_method])
         else:
             raise RuntimeError("The configuration 'image_update_method' is incorrect.")
-        
-        self.log_menu.wlog("INFO", f"The picture from the media file is rendered using the {repr(self.config.image_update_method)} method.")
+        self.info(f"The picture from the media file is rendered using the {repr(self.config.image_update_method)} method.")
         
         # * Compositions Screen
         self.music_list_screen = Static(classes="screen-box")
         self.music_list_screen.border_title = "Playlist"
         
         self.music_list_view = MusicListView()
         
@@ -233,26 +258,30 @@
             self.update_loop_playback,
             name="PLAYBACK_CONTROLLER",
             group="CONTROL_UPDATER-LOOP",
             description="Control of playback modes and status updates."
         )
     
     async def add_sounds_to_list(self) -> None:
+        added_oks = 0
         async for path in aiter(self.last_paths_globalized):
             async for codec in aiter(self.CODECS):
                 if await codec.aio_is_this_codec(path):
                     try: sound = codec(path, **self.CODECS_KWARGS)
                     except: sound = None
                     if sound is not None:
                         if not await self.music_list_view.music_list.aio_exists_sha1(sound):
                             await self.music_list_view.aio_add_sound(sound)
-                            self.log_menu.wlog("INFO", f"Song added: {repr(sound)}")
+                            self.info(f"Song added: {repr(sound)}")
+                            added_oks += 1
                             break
             if sound is None:
-                self.log_menu.wlog("ERROR", f"The sound could not be loaded: {repr(path)}", cc="red")
+                self.error(f"The sound could not be loaded: {repr(path)}")
+        self.info(f"Added [cyan]{added_oks}[/cyan] songs!")
+        await self.aio_nofy(f"Added [cyan]{added_oks}[/cyan] songs!")
     
     async def currect_sound_stop(self, sound: Optional[CodecBase]=None):
         if sound is None: sound = await self.aio_gcs()
         if sound is not None:
             self.last_playback_status = "Stoped"
             sound.stop()
     
@@ -320,15 +349,15 @@
                     sound.stop()
             self.playback_mode_blocked = False
             
             self.currect_sound_uuid = sound_uuid
             if (sound:=self.music_list_view.get_sound(self.currect_sound_uuid)) is not None:
                 sound.set_volume(self.currect_volume)
                 await self.music_image.update_image(image_from_bytes(sound.icon_data))
-                self.log_menu.wlog("INFO", f"A new sound has been selected: {repr(sound)}")
+                self.info(f"A new sound has been selected: {repr(sound)}")
             self.currect_sound = sound
             self.music_selected_label.update(await self.aio_get_sound_selected_label_text())
             return sound
     
     async def on_list_view_selected(self, selected: MusicListView.Selected):
         if isinstance(selected.item, MusicListViewItem):
             await self.set_sound_for_playback(getattr(selected.item, "sound_uuid", None))
@@ -351,15 +380,16 @@
         if (sound:=await self.aio_gcs()) is not None:
             if (vol:=round(sound.get_volume()-self.config.volume_change_percent, 2)) >= 0:
                 self.currect_volume = vol
                 sound.set_volume(vol)
     
     async def action_screenshot(self) -> None:
         path = self.save_screenshot(path=LOCALDIR)
-        self.log_menu.wlog("INFO", f"Screenshot saved: {repr(path)}")
+        self.info(f"Screenshot saved to: {repr(path)}")
+        await self.aio_nofy(f"Screenshot saved to: [green]{repr(path)}[/]")
     
     async def action_quit(self):
         self.started = False
         if (sound:=await self.aio_gcs()) is not None:
             sound.unpause()
             sound.stop()
         return await super().action_quit()
```

### Comparing `seaplayer-0.4a2/seaplayer/types.py` & `seaplayer-0.4a3/seaplayer/types.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.4a2/PKG-INFO` & `seaplayer-0.4a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaplayer
-Version: 0.4a2
+Version: 0.4a3
 Summary: SeaPlayer is a player that works in the terminal.
 Home-page: https://github.com/romanin-rf/SeaPlayer
 License: MIT
 Keywords: tui,player,seaplayer,wav,mp3,ogg,midi
 Author: Romanin
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<4.0
```

