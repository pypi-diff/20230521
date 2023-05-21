# Comparing `tmp/manim_voiceover-0.3.2.tar.gz` & `tmp/manim_voiceover-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manim_voiceover-0.3.2.tar", max compression
+gzip compressed data, was "manim_voiceover-0.3.3.tar", max compression
```

## Comparing `manim_voiceover-0.3.2.tar` & `manim_voiceover-0.3.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1088 2023-05-20 08:51:04.205343 manim_voiceover-0.3.2/LICENSE
--rw-r--r--   0        0        0     2832 2023-05-20 08:51:04.205343 manim_voiceover-0.3.2/README.md
--rw-r--r--   0        0        0      203 2023-05-20 08:51:04.209343 manim_voiceover-0.3.2/manim_voiceover/__init__.py
--rw-r--r--   0        0        0     1779 2023-05-20 08:51:04.209343 manim_voiceover-0.3.2/manim_voiceover/defaults.py
--rw-r--r--   0        0        0     6032 2023-05-20 08:51:04.209343 manim_voiceover-0.3.2/manim_voiceover/helper.py
--rw-r--r--   0        0        0      658 2023-05-20 08:51:04.209343 manim_voiceover-0.3.2/manim_voiceover/modify_audio.py
--rw-r--r--   0        0        0      343 2023-05-20 08:51:04.209343 manim_voiceover-0.3.2/manim_voiceover/services/__init__.py
--rw-r--r--   0        0        0     8752 2023-05-20 08:51:04.209343 manim_voiceover-0.3.2/manim_voiceover/services/azure.py
--rw-r--r--   0        0        0     7514 2023-05-20 08:51:04.209343 manim_voiceover-0.3.2/manim_voiceover/services/base.py
--rw-r--r--   0        0        0     2754 2023-05-20 08:51:04.209343 manim_voiceover-0.3.2/manim_voiceover/services/coqui.py
--rw-r--r--   0        0        0     2794 2023-05-20 08:51:04.209343 manim_voiceover-0.3.2/manim_voiceover/services/gtts.py
--rw-r--r--   0        0        0     1541 2023-05-20 08:51:04.209343 manim_voiceover-0.3.2/manim_voiceover/services/pyttsx3.py
--rw-r--r--   0        0        0     4022 2023-05-20 08:51:04.209343 manim_voiceover-0.3.2/manim_voiceover/services/recorder/__init__.py
--rw-r--r--   0        0        0     7812 2023-05-20 08:51:04.209343 manim_voiceover-0.3.2/manim_voiceover/services/recorder/utility.py
--rw-r--r--   0        0        0     6047 2023-05-20 08:51:04.209343 manim_voiceover-0.3.2/manim_voiceover/services/stitcher.py
--rw-r--r--   0        0        0     5045 2023-05-20 08:51:04.209343 manim_voiceover-0.3.2/manim_voiceover/tracker.py
--rw-r--r--   0        0        0      584 2023-05-20 08:51:04.209343 manim_voiceover-0.3.2/manim_voiceover/translate/__init__.py
--rw-r--r--   0        0        0     6395 2023-05-20 08:51:04.209343 manim_voiceover-0.3.2/manim_voiceover/translate/gettext_utils.py
--rw-r--r--   0        0        0     3815 2023-05-20 08:51:04.209343 manim_voiceover-0.3.2/manim_voiceover/translate/render.py
--rw-r--r--   0        0        0     2510 2023-05-20 08:51:04.209343 manim_voiceover-0.3.2/manim_voiceover/translate/translate.py
--rw-r--r--   0        0        0     7089 2023-05-20 08:51:04.209343 manim_voiceover-0.3.2/manim_voiceover/voiceover_scene.py
--rw-r--r--   0        0        0     3505 2023-05-20 08:51:04.213343 manim_voiceover-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     5450 1970-01-01 00:00:00.000000 manim_voiceover-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-05-21 19:43:51.921874 manim_voiceover-0.3.3/LICENSE
+-rw-r--r--   0        0        0     2832 2023-05-21 19:43:51.921874 manim_voiceover-0.3.3/README.md
+-rw-r--r--   0        0        0      203 2023-05-21 19:43:51.925874 manim_voiceover-0.3.3/manim_voiceover/__init__.py
+-rw-r--r--   0        0        0     1779 2023-05-21 19:43:51.925874 manim_voiceover-0.3.3/manim_voiceover/defaults.py
+-rw-r--r--   0        0        0     6048 2023-05-21 19:43:51.925874 manim_voiceover-0.3.3/manim_voiceover/helper.py
+-rw-r--r--   0        0        0      658 2023-05-21 19:43:51.925874 manim_voiceover-0.3.3/manim_voiceover/modify_audio.py
+-rw-r--r--   0        0        0      343 2023-05-21 19:43:51.925874 manim_voiceover-0.3.3/manim_voiceover/services/__init__.py
+-rw-r--r--   0        0        0     8972 2023-05-21 19:43:51.925874 manim_voiceover-0.3.3/manim_voiceover/services/azure.py
+-rw-r--r--   0        0        0     7794 2023-05-21 19:43:51.925874 manim_voiceover-0.3.3/manim_voiceover/services/base.py
+-rw-r--r--   0        0        0     2759 2023-05-21 19:43:51.925874 manim_voiceover-0.3.3/manim_voiceover/services/coqui.py
+-rw-r--r--   0        0        0     2799 2023-05-21 19:43:51.925874 manim_voiceover-0.3.3/manim_voiceover/services/gtts.py
+-rw-r--r--   0        0        0     1546 2023-05-21 19:43:51.925874 manim_voiceover-0.3.3/manim_voiceover/services/pyttsx3.py
+-rw-r--r--   0        0        0     3992 2023-05-21 19:43:51.925874 manim_voiceover-0.3.3/manim_voiceover/services/recorder/__init__.py
+-rw-r--r--   0        0        0     7901 2023-05-21 19:43:51.925874 manim_voiceover-0.3.3/manim_voiceover/services/recorder/utility.py
+-rw-r--r--   0        0        0     6047 2023-05-21 19:43:51.925874 manim_voiceover-0.3.3/manim_voiceover/services/stitcher.py
+-rw-r--r--   0        0        0     5053 2023-05-21 19:43:51.925874 manim_voiceover-0.3.3/manim_voiceover/tracker.py
+-rw-r--r--   0        0        0      584 2023-05-21 19:43:51.925874 manim_voiceover-0.3.3/manim_voiceover/translate/__init__.py
+-rw-r--r--   0        0        0     6395 2023-05-21 19:43:51.925874 manim_voiceover-0.3.3/manim_voiceover/translate/gettext_utils.py
+-rw-r--r--   0        0        0     3814 2023-05-21 19:43:51.925874 manim_voiceover-0.3.3/manim_voiceover/translate/render.py
+-rw-r--r--   0        0        0     2510 2023-05-21 19:43:51.925874 manim_voiceover-0.3.3/manim_voiceover/translate/translate.py
+-rw-r--r--   0        0        0     7104 2023-05-21 19:43:51.925874 manim_voiceover-0.3.3/manim_voiceover/voiceover_scene.py
+-rw-r--r--   0        0        0     3427 2023-05-21 19:43:51.929874 manim_voiceover-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     5372 1970-01-01 00:00:00.000000 manim_voiceover-0.3.3/PKG-INFO
```

### Comparing `manim_voiceover-0.3.2/LICENSE` & `manim_voiceover-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.2/README.md` & `manim_voiceover-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.2/manim_voiceover/defaults.py` & `manim_voiceover-0.3.3/manim_voiceover/defaults.py`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.2/manim_voiceover/helper.py` & `manim_voiceover-0.3.3/manim_voiceover/helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 def chunks(lst: list, n: int):
     """Yield successive n-sized chunks from lst."""
     for i in range(0, len(lst), n):
         yield lst[i : i + n]
 
 
-def remove_bookmarks(str):
-    return re.sub("<bookmark\s*mark\s*=['\"]\w*[\"']\s*/>", "", str)
+def remove_bookmarks(input: str) -> str:
+    return re.sub("<bookmark\s*mark\s*=['\"]\w*[\"']\s*/>", "", input)
 
 
 def wav2mp3(wav_path, mp3_path=None, remove_wav=True, bitrate="312k"):
     """Convert wav file to mp3 file"""
 
     if mp3_path is None:
         mp3_path = Path(wav_path).with_suffix(".mp3")
```

### Comparing `manim_voiceover-0.3.2/manim_voiceover/modify_audio.py` & `manim_voiceover-0.3.3/manim_voiceover/modify_audio.py`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.2/manim_voiceover/services/azure.py` & `manim_voiceover-0.3.3/manim_voiceover/services/azure.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,47 +82,48 @@
         inner = remove_bookmarks(inner)
         if cache_dir is None:
             cache_dir = self.cache_dir
 
         # Apply prosody
         prosody = kwargs.get("prosody", self.prosody)
 
+        ssml_beginning = r"""<speak version="1.0" xmlns="http://www.w3.org/2001/10/synthesis"
+    xmlns:mstts="https://www.w3.org/2001/mstts" xml:lang="en-US">
+    <voice name="%s">
+        """ % (
+            self.voice
+        )
+        ssml_end = r"""
+    </voice>
+</speak>
+        """
+
         if prosody is not None:
             if not isinstance(prosody, dict):
                 raise ValueError(
                     "The prosody argument must be a dict that contains at least one of the following keys: 'pitch', 'contour', 'range', 'rate', 'volume'."
                 )
 
-            opening_tag = (
+            prosody_opening_tag = (
                 "<prosody "
                 + " ".join(
                     ['%s="%s"' % (key, str(val)) for key, val in prosody.items()]
                 )
                 + ">"
             )
-            inner = opening_tag + inner + "</prosody>"
+            prosody_closing_tag = "</prosody>"
+            ssml_beginning = ssml_beginning + prosody_opening_tag
+            ssml_end = prosody_closing_tag + ssml_end
 
         if self.style is not None:
-            inner = r"""<mstts:express-as style="%s">
-    %s
-</mstts:express-as>""" % (
-                self.style,
-                inner,
-            )
+            style_opening_tag = '<mstts:express-as style="%s">' % self.style
+            style_closing_tag = "</mstts:express-as>"
+            ssml_beginning = ssml_beginning + style_opening_tag
+            ssml_end = style_closing_tag + ssml_end
 
-        ssml_beginning = r"""<speak version="1.0" xmlns="http://www.w3.org/2001/10/synthesis"
-    xmlns:mstts="https://www.w3.org/2001/mstts" xml:lang="en-US">
-    <voice name="%s">
-        """ % (
-            self.voice
-        )
-        ssml_end = r"""
-    </voice>
-</speak>
-        """
         ssml = ssml_beginning + inner + ssml_end
         initial_offset = len(ssml_beginning)
 
         input_data = {
             "input_text": text,
             "ssml": ssml,
             "service": "azure",
@@ -135,15 +136,15 @@
         }
 
         cached_result = self.get_cached_result(input_data, cache_dir)
         if cached_result is not None:
             return cached_result
 
         if path is None:
-            audio_path = self.get_data_hash(input_data) + ".mp3"
+            audio_path = self.get_audio_basename(input_data) + ".mp3"
         else:
             audio_path = path
 
         try:
             azure_subscription_key = os.environ["AZURE_SUBSCRIPTION_KEY"]
             azure_service_region = os.environ["AZURE_SERVICE_REGION"]
         except KeyError:
```

### Comparing `manim_voiceover-0.3.2/manim_voiceover/services/base.py` & `manim_voiceover-0.3.3/manim_voiceover/services/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,63 @@
 from abc import ABC, abstractmethod
+import typing as t
 import os
 import json
 import sys
 import hashlib
-import humanhash
 from pathlib import Path
 from manim import config, logger
+from slugify import slugify
 from manim_voiceover.defaults import (
     DEFAULT_VOICEOVER_CACHE_DIR,
     DEFAULT_VOICEOVER_CACHE_JSON_FILENAME,
 )
-from manim_voiceover.helper import append_to_json_file, prompt_ask_missing_extras
+from manim_voiceover.helper import (
+    append_to_json_file,
+    prompt_ask_missing_extras,
+    remove_bookmarks,
+)
 from manim_voiceover.modify_audio import adjust_speed
 from manim_voiceover.tracker import AUDIO_OFFSET_RESOLUTION
 
 
 def timestamps_to_word_boundaries(segments):
     word_boundaries = []
     current_text_offset = 0
     for segment in segments:
-        for dict_ in segment["word_timestamps"]:
+        for dict_ in segment["words"]:
             word = dict_["word"]
             word_boundaries.append(
                 {
-                    "audio_offset": int(dict_["timestamp"] * AUDIO_OFFSET_RESOLUTION),
+                    "audio_offset": int(dict_["start"] * AUDIO_OFFSET_RESOLUTION),
                     # "duration_milliseconds": 0,
                     "text_offset": current_text_offset,
-                    "word_length": len(dict_["word"]),
+                    "word_length": len(word),
                     "text": word,
                     "boundary_type": "Word",
                 }
             )
-            current_text_offset += len(dict_["word"])
+            current_text_offset += len(word)
             # If word is not punctuation, add a space
             # if word not in [".", ",", "!", "?", ";", ":", "(", ")"]:
             # current_text_offset += 1
 
     return word_boundaries
 
 
 class SpeechService(ABC):
     """Abstract base class for a speech service."""
 
     def __init__(
         self,
         global_speed: float = 1.00,
-        cache_dir: str = None,
-        transcription_model: str = None,
+        cache_dir: t.Optional[str] = None,
+        transcription_model: t.Optional[str] = None,
         transcription_kwargs: dict = {},
-        **kwargs
+        **kwargs,
     ):
         """
         Args:
             global_speed (float, optional): The speed at which to play the audio.
                 Defaults to 1.00.
             cache_dir (str, optional): The directory to save the audio
                 files to. Defaults to ``voiceovers/``.
@@ -86,20 +91,20 @@
         original_audio = dict_["original_audio"]
 
         # Check whether word boundaries exist and if not run stt
         if "word_boundaries" not in dict_ and self._whisper_model is not None:
             transcription_result = self._whisper_model.transcribe(
                 str(Path(self.cache_dir) / original_audio), **self.transcription_kwargs
             )
-            logger.info("Transcription: " + transcription_result["text"])
+            logger.info("Transcription: " + transcription_result.text)
             word_boundaries = timestamps_to_word_boundaries(
-                transcription_result["segments"]
+                transcription_result.segments_to_dicts()
             )
             dict_["word_boundaries"] = word_boundaries
-            dict_["transcribed_text"] = transcription_result["text"]
+            dict_["transcribed_text"] = transcription_result.text
 
         # Audio callback
         self.audio_callback(original_audio, dict_, **kwargs)
 
         if self.global_speed != 1:
             split_path = os.path.splitext(original_audio)
             adjusted_path = split_path[0] + "_adjusted" + split_path[1]
@@ -148,18 +153,23 @@
                 )
                 self._whisper_model = whisper.load_model(model)
             else:
                 self._whisper_model = None
 
         self.transcription_kwargs = kwargs
 
-    def get_data_hash(self, data: dict) -> str:
+    def get_audio_basename(self, data: dict) -> str:
         dumped_data = json.dumps(data)
         data_hash = hashlib.sha256(dumped_data.encode("utf-8")).hexdigest()
-        return humanhash.humanize(data_hash)
+        suffix = data_hash[:8]
+        input_text = data["input_text"]
+        input_text = remove_bookmarks(input_text)
+        slug = slugify(input_text, max_length=50, word_boundary=True, save_order=True)
+        ret = f"{slug}-{suffix}"
+        return ret
 
     @abstractmethod
     def generate_from_text(
         self, text: str, cache_dir: str = None, path: str = None
     ) -> dict:
         """Implement this method for each speech service. Refer to `AzureService` for an example.
```

### Comparing `manim_voiceover-0.3.2/manim_voiceover/services/coqui.py` & `manim_voiceover-0.3.3/manim_voiceover/services/coqui.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         input_data = {"input_text": text, "service": "coqui"}
 
         cached_result = self.get_cached_result(input_data, cache_dir)
         if cached_result is not None:
             return cached_result
 
         if path is None:
-            audio_path = self.get_data_hash(input_data) + ".mp3"
+            audio_path = self.get_audio_basename(input_data) + ".mp3"
         else:
             audio_path = path
 
         if not kwargs:
             kwargs = self.init_kwargs
 
         output_path = str(Path(cache_dir) / audio_path)
```

### Comparing `manim_voiceover-0.3.2/manim_voiceover/services/gtts.py` & `manim_voiceover-0.3.3/manim_voiceover/services/gtts.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         input_data = {"input_text": input_text, "service": "gtts"}
 
         cached_result = self.get_cached_result(input_data, cache_dir)
         if cached_result is not None:
             return cached_result
 
         if path is None:
-            audio_path = self.get_data_hash(input_data) + ".mp3"
+            audio_path = self.get_audio_basename(input_data) + ".mp3"
         else:
             audio_path = path
 
         if "lang" not in kwargs:
             kwargs["lang"] = self.lang
         if "tld" not in kwargs:
             kwargs["tld"] = self.tld
```

### Comparing `manim_voiceover-0.3.2/manim_voiceover/services/pyttsx3.py` & `manim_voiceover-0.3.3/manim_voiceover/services/pyttsx3.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         input_data = {"input_text": text, "service": "pyttsx3"}
 
         cached_result = self.get_cached_result(input_data, cache_dir)
         if cached_result is not None:
             return cached_result
 
         if path is None:
-            audio_path = self.get_data_hash(input_data) + ".mp3"
+            audio_path = self.get_audio_basename(input_data) + ".mp3"
         else:
             audio_path = path
 
         self.engine.save_to_file(text, str(Path(cache_dir) / audio_path))
         self.engine.runAndWait()
         self.engine.stop()
```

### Comparing `manim_voiceover-0.3.2/manim_voiceover/services/recorder/__init__.py` & `manim_voiceover-0.3.3/manim_voiceover/services/recorder/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,17 +43,15 @@
             chunk (int, optional): Chunk size. Defaults to 512.
             device_index (int, optional): Device index, if you don't want to choose it every time you render. Defaults to None.
             transcription_model (str, optional): The `OpenAI Whisper model <https://github.com/openai/whisper#available-models-and-languages>`_ to use for transcription. Defaults to "base".
             trim_silence_threshold (float, optional): Threshold for trimming silence in decibels. Defaults to -40.0 dB.
             trim_buffer_start (int, optional): Buffer duration for trimming silence at the start. Defaults to 200 ms.
             trim_buffer_end (int, optional): Buffer duration for trimming silence at the end. Defaults to 200 ms.
         """
-        prompt_ask_missing_extras(
-            ["pyaudio", "pynput", "playsound"], "recorder", "RecorderService"
-        )
+        prompt_ask_missing_extras(["pyaudio", "pynput"], "recorder", "RecorderService")
 
         self.recorder = Recorder(
             format=format,
             channels=channels,
             rate=rate,
             chunk=chunk,
             device_index=device_index,
@@ -88,15 +86,15 @@
             "service": "recorder",
         }
         cached_result = self.get_cached_result(input_data, cache_dir)
         if cached_result is not None:
             return cached_result
 
         if path is None:
-            audio_path = self.get_data_hash(input_data) + ".mp3"
+            audio_path = self.get_audio_basename(input_data) + ".mp3"
         else:
             audio_path = path
 
         self.recorder._trigger_set_device()
         box = msg_box("Voiceover:\n\n" + input_text)
         self.recorder.record(str(Path(cache_dir) / audio_path), box)
```

### Comparing `manim_voiceover-0.3.2/manim_voiceover/services/recorder/utility.py` & `manim_voiceover-0.3.3/manim_voiceover/services/recorder/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from pydub import AudioSegment
 from manim import logger
 
 from manim_voiceover.helper import trim_silence, wav2mp3
 
 from pynput import keyboard
 import pyaudio
-import playsound
+from pydub import AudioSegment
+from pydub.playback import play
 
 
 class MyListener(keyboard.Listener):
     def __init__(self):
         super(MyListener, self).__init__(self.on_press, self.on_release)
         self.key_pressed = None
 
@@ -231,15 +232,16 @@
  r to [r]e-record
  a to [a]ccept the recording
 """
             )
             try:
                 key = input()[-1].lower()
                 if key == "l":
-                    playsound.playsound(path)
+                    audio = AudioSegment.from_file(path)
+                    play(audio)
                 elif key == "r":
                     if message is not None:
                         print(message)
 
                     self._record(path)
                 elif key == "a":
                     break
```

### Comparing `manim_voiceover-0.3.2/manim_voiceover/services/stitcher.py` & `manim_voiceover-0.3.3/manim_voiceover/services/stitcher.py`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.2/manim_voiceover/tracker.py` & `manim_voiceover-0.3.3/manim_voiceover/tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,19 +83,19 @@
         for mark, dist in self.bookmark_distances.items():
             # Normalize text offset
             elapsed = self.time_interpolator.interpolate(
                 dist * transcribed_text_len / net_text_len
             )
             self.bookmark_times[mark] = self.start_t + elapsed
 
-    def get_remaining_duration(self, buff: int = 0) -> int:
+    def get_remaining_duration(self, buff: float = 0.0) -> float:
         """Returns the remaining duration of the voiceover.
 
         Args:
-            buff (int, optional): A buffer to add to the remaining duration. Defaults to 0.
+            buff (float, optional): A buffer to add to the remaining duration. Defaults to 0.
 
         Returns:
             int: The remaining duration of the voiceover in seconds.
         """
         # result= max(self.end_t - self.scene.last_t, 0)
         result = max(self.end_t - self.scene.renderer.time + buff, 0)
         # print(result)
```

### Comparing `manim_voiceover-0.3.2/manim_voiceover/translate/__init__.py` & `manim_voiceover-0.3.3/manim_voiceover/translate/__init__.py`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.2/manim_voiceover/translate/gettext_utils.py` & `manim_voiceover-0.3.3/manim_voiceover/translate/gettext_utils.py`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.2/manim_voiceover/translate/render.py` & `manim_voiceover-0.3.3/manim_voiceover/translate/render.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,14 @@
     # default="",
     required=True,
     help="Scene to translate",
 )
 
 
 def main():
-
     args = parser.parse_args()
     file = args.file
     domain = args.domain
     localedir = args.localedir
     quality = args.quality
     scene = args.scene
```

### Comparing `manim_voiceover-0.3.2/manim_voiceover/translate/translate.py` & `manim_voiceover-0.3.3/manim_voiceover/translate/translate.py`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.2/manim_voiceover/voiceover_scene.py` & `manim_voiceover-0.3.3/manim_voiceover/voiceover_scene.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from math import ceil
 from contextlib import contextmanager
 from pathlib import Path
 from typing import Optional, Generator
 import re
+import typing as t
 
 from manim import Scene, config
 from manim_voiceover.services.base import SpeechService
 from manim_voiceover.tracker import VoiceoverTracker
-from manim_voiceover.helper import chunks
+from manim_voiceover.helper import chunks, remove_bookmarks
 
 
 # SCRIPT_FILE_PATH = "media/script.txt"
 
 
 class VoiceoverScene(Scene):
     """A scene class that can be used to add voiceover to a scene."""
@@ -67,16 +68,15 @@
         self.current_tracker = tracker
 
         # if self.create_script:
         #     self.save_to_script_file(text)
 
         if self.create_subcaption:
             if subcaption is None:
-                # Remove placeholders
-                subcaption = re.sub(r"<[^<>]+/>", "", text)
+                subcaption = remove_bookmarks(text)
 
             self.add_wrapped_subcaption(
                 subcaption,
                 tracker.duration,
                 subcaption_buff=subcaption_buff,
                 max_subcaption_len=max_subcaption_len,
             )
@@ -159,15 +159,15 @@
         Args:
             mark (str): The `mark` attribute of the bookmark to wait for.
         """
         self.safe_wait(self.current_tracker.time_until_bookmark(mark))
 
     @contextmanager
     def voiceover(
-        self, text: str = None, ssml: str = None, **kwargs
+        self, text: t.Optional[str] = None, ssml: t.Optional[str] = None, **kwargs
     ) -> Generator[VoiceoverTracker, None, None]:
         """The main function to be used for adding voiceover to a scene.
 
         Args:
             text (str, optional): The text to be spoken. Defaults to None.
             ssml (str, optional): The SSML to be spoken. Defaults to None.
```

### Comparing `manim_voiceover-0.3.2/pyproject.toml` & `manim_voiceover-0.3.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "manim-voiceover"
-version = "0.3.2"
+version = "0.3.3"
 description = "Manim plugin for all things voiceover"
 authors = ["The Manim Community Developers <contact@manim.community>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "manim_voiceover" }]
 repository = "https://github.com/ManimCommunity/manim-voiceover"
 homepage = "https://voiceover.manim.community"
@@ -50,40 +50,38 @@
 azure-cognitiveservices-speech = { version = "^1.24.0", optional = true }
 PyAudio = { version = "^0.2.12", optional = true }
 gTTS = { version = "^2.2.4", optional = true }
 pyttsx3 = { version = "^2.90", optional = true }
 # torch = { version = "*", optional = true }
 # TTS = { version = "*", optional = true }
 pynput = { version = "^1.7.6", optional = true }
-playsound = { version = "^1.3.0", optional = true }
 # deep-translator = { version = "^1.9.2", optional = true }
 deepl = { version = "^1.12.0", optional = true }
-humanhash3 = "^0.0.6"
 pip = ">=21.0.1"
-openai-whisper = { version = "^20230117", optional = true }
-stable-ts = { version ="^1.0.3", optional = true }
+openai-whisper = { version = "^20230314", optional = true }
+stable-ts = { version ="^2.6.2", optional = true }
+python-slugify = "^8.0.1"
 
 [tool.poetry.extras]
 azure = ["azure-cognitiveservices-speech"]
 gtts = ["gTTS"]
 pyttsx3 = ["pyttsx3"]
 # coqui = ["torch", "TTS"]
 coqui = [] # Removed TTS as deps for now
-recorder = ["PyAudio", "pynput", "playsound"]
+recorder = ["PyAudio", "pynput"]
 translate = ["deepl"]
 transcribe = ["openai-whisper", "stable-ts"]
 all = [
     "azure-cognitiveservices-speech",
     "gTTS",
     "pyttsx3",
     "torch",
     "TTS",
     "PyAudio",
     "pynput",
-    "playsound",
     "deepl",
     "openai-whisper",
     "stable-ts",
 ]
 
 [tool.poetry.group.dev.dependencies]
 Pygments = "^2.13.0"
```

### Comparing `manim_voiceover-0.3.2/PKG-INFO` & `manim_voiceover-0.3.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manim-voiceover
-Version: 0.3.2
+Version: 0.3.3
 Summary: Manim plugin for all things voiceover
 Home-page: https://voiceover.manim.community
 License: MIT
 Keywords: text-to-speech,tts,voiceover,manim,recording,speech synthesis,math animations
 Author: The Manim Community Developers
 Author-email: contact@manim.community
 Requires-Python: >=3.8,<4
@@ -33,26 +33,25 @@
 Provides-Extra: recorder
 Provides-Extra: transcribe
 Provides-Extra: translate
 Requires-Dist: PyAudio (>=0.2.12,<0.3.0) ; extra == "recorder" or extra == "all"
 Requires-Dist: azure-cognitiveservices-speech (>=1.24.0,<2.0.0) ; extra == "azure" or extra == "all"
 Requires-Dist: deepl (>=1.12.0,<2.0.0) ; extra == "translate" or extra == "all"
 Requires-Dist: gTTS (>=2.2.4,<3.0.0) ; extra == "gtts" or extra == "all"
-Requires-Dist: humanhash3 (>=0.0.6,<0.0.7)
 Requires-Dist: manim
 Requires-Dist: mutagen (>=1.46.0,<2.0.0)
-Requires-Dist: openai-whisper (>=20230117,<20230118) ; extra == "transcribe" or extra == "all"
+Requires-Dist: openai-whisper (>=20230314,<20230315) ; extra == "transcribe" or extra == "all"
 Requires-Dist: pip (>=21.0.1)
-Requires-Dist: playsound (>=1.3.0,<2.0.0) ; extra == "recorder" or extra == "all"
 Requires-Dist: pydub (>=0.25.1,<0.26.0)
 Requires-Dist: pynput (>=1.7.6,<2.0.0) ; extra == "recorder" or extra == "all"
 Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
+Requires-Dist: python-slugify (>=8.0.1,<9.0.0)
 Requires-Dist: pyttsx3 (>=2.90,<3.0) ; extra == "pyttsx3" or extra == "all"
 Requires-Dist: sox (>=1.4.1,<2.0.0)
-Requires-Dist: stable-ts (>=1.0.3,<2.0.0) ; extra == "transcribe" or extra == "all"
+Requires-Dist: stable-ts (>=2.6.2,<3.0.0) ; extra == "transcribe" or extra == "all"
 Project-URL: Documentation, https://voiceover.manim.community
 Project-URL: Repository, https://github.com/ManimCommunity/manim-voiceover
 Description-Content-Type: text/markdown
 
 # Manim Voiceover
 
 <p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: manim-voiceover Version: 0.3.2 Summary: Manim
+Metadata-Version: 2.1 Name: manim-voiceover Version: 0.3.3 Summary: Manim
 plugin for all things voiceover Home-page: https://voiceover.manim.community
 License: MIT Keywords: text-to-speech,tts,voiceover,manim,recording,speech
 synthesis,math animations Author: The Manim Community Developers Author-email:
 contact@manim.community Requires-Python: >=3.8,<4 Classifier: Development
 Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
@@ -17,23 +17,22 @@
 Scientific/Engineering :: Visualization Provides-Extra: all Provides-Extra:
 azure Provides-Extra: coqui Provides-Extra: gtts Provides-Extra: pyttsx3
 Provides-Extra: recorder Provides-Extra: transcribe Provides-Extra: translate
 Requires-Dist: PyAudio (>=0.2.12,<0.3.0) ; extra == "recorder" or extra ==
 "all" Requires-Dist: azure-cognitiveservices-speech (>=1.24.0,<2.0.0) ; extra
 == "azure" or extra == "all" Requires-Dist: deepl (>=1.12.0,<2.0.0) ; extra ==
 "translate" or extra == "all" Requires-Dist: gTTS (>=2.2.4,<3.0.0) ; extra ==
-"gtts" or extra == "all" Requires-Dist: humanhash3 (>=0.0.6,<0.0.7) Requires-
-Dist: manim Requires-Dist: mutagen (>=1.46.0,<2.0.0) Requires-Dist: openai-
-whisper (>=20230117,<20230118) ; extra == "transcribe" or extra == "all"
-Requires-Dist: pip (>=21.0.1) Requires-Dist: playsound (>=1.3.0,<2.0.0) ; extra
-== "recorder" or extra == "all" Requires-Dist: pydub (>=0.25.1,<0.26.0)
-Requires-Dist: pynput (>=1.7.6,<2.0.0) ; extra == "recorder" or extra == "all"
-Requires-Dist: python-dotenv (>=0.21.0,<0.22.0) Requires-Dist: pyttsx3
+"gtts" or extra == "all" Requires-Dist: manim Requires-Dist: mutagen
+(>=1.46.0,<2.0.0) Requires-Dist: openai-whisper (>=20230314,<20230315) ; extra
+== "transcribe" or extra == "all" Requires-Dist: pip (>=21.0.1) Requires-Dist:
+pydub (>=0.25.1,<0.26.0) Requires-Dist: pynput (>=1.7.6,<2.0.0) ; extra ==
+"recorder" or extra == "all" Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
+Requires-Dist: python-slugify (>=8.0.1,<9.0.0) Requires-Dist: pyttsx3
 (>=2.90,<3.0) ; extra == "pyttsx3" or extra == "all" Requires-Dist: sox
-(>=1.4.1,<2.0.0) Requires-Dist: stable-ts (>=1.0.3,<2.0.0) ; extra ==
+(>=1.4.1,<2.0.0) Requires-Dist: stable-ts (>=2.6.2,<3.0.0) ; extra ==
 "transcribe" or extra == "all" Project-URL: Documentation, https://
 voiceover.manim.community Project-URL: Repository, https://github.com/
 ManimCommunity/manim-voiceover Description-Content-Type: text/markdown # Manim
 Voiceover
 [Github_Actions_Status] [PyPI_Latest_Release] [Downloads] [Documentation
 Status] [License] [Discord]
 Manim Voiceover is a [Manim](https://manim.community) plugin for all things
```

