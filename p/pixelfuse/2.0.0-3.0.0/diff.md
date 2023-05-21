# Comparing `tmp/pixelfuse-2.0.0.tar.gz` & `tmp/pixelfuse-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixelfuse-2.0.0.tar", max compression
+gzip compressed data, was "pixelfuse-3.0.0.tar", max compression
```

## Comparing `pixelfuse-2.0.0.tar` & `pixelfuse-3.0.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-04-27 14:02:02.368880 pixelfuse-2.0.0/LICENSE
--rw-r--r--   0        0        0     4845 2023-04-27 14:02:02.368880 pixelfuse-2.0.0/README.md
--rw-r--r--   0        0        0       89 2023-04-27 14:02:02.368880 pixelfuse-2.0.0/pixelfuse/__init__.py
--rw-r--r--   0        0        0      112 2023-04-27 14:02:02.368880 pixelfuse-2.0.0/pixelfuse/__main__.py
--rw-r--r--   0        0        0     4219 2023-04-27 14:02:02.368880 pixelfuse-2.0.0/pixelfuse/cli.py
--rw-r--r--   0        0        0     3599 2023-04-27 14:02:02.368880 pixelfuse-2.0.0/pixelfuse/src/f2v.py
--rw-r--r--   0        0        0     4118 2023-04-27 14:02:02.368880 pixelfuse-2.0.0/pixelfuse/src/v2f.py
--rw-r--r--   0        0        0      667 2023-04-27 14:02:02.368880 pixelfuse-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     5672 1970-01-01 00:00:00.000000 pixelfuse-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-21 14:35:28.833560 pixelfuse-3.0.0/LICENSE
+-rw-r--r--   0        0        0     5924 2023-05-21 14:35:28.833560 pixelfuse-3.0.0/README.md
+-rw-r--r--   0        0        0      216 2023-05-21 14:35:28.833560 pixelfuse-3.0.0/pixelfuse/__init__.py
+-rw-r--r--   0        0        0      112 2023-05-21 14:35:28.833560 pixelfuse-3.0.0/pixelfuse/__main__.py
+-rw-r--r--   0        0        0     5048 2023-05-21 14:35:28.833560 pixelfuse-3.0.0/pixelfuse/cli.py
+-rw-r--r--   0        0        0     4672 2023-05-21 14:35:28.833560 pixelfuse-3.0.0/pixelfuse/src/f2lfv.py
+-rw-r--r--   0        0        0     3599 2023-05-21 14:35:28.833560 pixelfuse-3.0.0/pixelfuse/src/f2v.py
+-rw-r--r--   0        0        0     4137 2023-05-21 14:35:28.833560 pixelfuse-3.0.0/pixelfuse/src/lfv2f.py
+-rw-r--r--   0        0        0     4111 2023-05-21 14:35:28.833560 pixelfuse-3.0.0/pixelfuse/src/v2f.py
+-rw-r--r--   0        0        0      667 2023-05-21 14:35:28.833560 pixelfuse-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6751 1970-01-01 00:00:00.000000 pixelfuse-3.0.0/PKG-INFO
```

### Comparing `pixelfuse-2.0.0/LICENSE` & `pixelfuse-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pixelfuse-2.0.0/README.md` & `pixelfuse-3.0.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # 📄🔄🎞️ PixelFuse
 
 Convert any file to video and video to file.
 
-**WARNING: videos created from files are extremely fragile**
+**WARNING: videos created from files are very fragile. But if you create videos with the `--lessf` flag, the videos are not so fragile anymore**
 
 ## 💿 Installation
 
 * Set up using `pip`:
 ```bash
 pip install pixelfuse
 ```
@@ -29,17 +29,18 @@
 As output you get the file `output.avi` - video 640x480, 1.0 FPS, codec HFYU [like this](https://drive.google.com/file/d/1OTZ9rF-6SI73BiLEwY4gJeJ2RVddLsfn/edit)
 
 As for the parameters:
 * `path: Path` - mandatory, the path to the file you want to convert
 * `fps: float` - frame rate, default is `1.0`
 * `width: int` - Video length, default is `480px`
 * `height: int` - Video height, `640px` by default
-* `fourcc: str` - Codec, a string of 4 characters, **WARNING: Use lossless codecs ONLY**, default is "`HFYU`".
+* `fourcc: str` - Codec, a string of 4 characters, **WARNING: Use lossless codecs ONLY(except for the `--lessf` flag)**, default is "`HFYU`".
 * `output: Path` - Path to output file, default is "`output.avi`", **note you need to use file extension compatible with codec, for example if you use `HFYU` codec you can NOT specify `output` as `output.mp4`**
 * `verbose: int` - Output level, from 0 to 3, default is 2
+* `lessf: bool` - Changes the way the video is recorded so that the video becomes less fragile, with this flag you can use lossy compression, default is `False`
 
 ### 🆕 Convert files to video(`filesToVideo`)
 
 To convert a file into a video just write the following command:
 ```bash
 python -m pixelfuse filesToVideo "test/example.text.txt" "test/example.image.jpg"
 ```
@@ -53,40 +54,45 @@
 As output you get the file `output.avi` - video 640x480, 1.0 FPS, codec HFYU [like this](https://drive.google.com/file/d/1OTZ9rF-6SI73BiLEwY4gJeJ2RVddLsfn/edit)
 
 As for the parameters:
 * `paths: list[Path]` - mandatory, the paths to the files you want to convert
 * `fps: float` - frame rate, default is `1.0`
 * `width: int` - Video length, default is `480px`
 * `height: int` - Video height, `640px` by default
-* `fourcc: str` - Codec, a string of 4 characters, **WARNING: Use lossless codecs ONLY**, default is "`HFYU`".
+* `fourcc: str` - Codec, a string of 4 characters, **WARNING: Use lossless codecs ONLY(except for the `--lessf` flag)**, default is "`HFYU`".
 * `output: Path` - Path to output file, default is "`output.avi`", **note you need to use file extension compatible with codec, for example if you use `HFYU` codec you can NOT specify `output` as `output.mp4`**
 * `verbose: int` - Output level, from 0 to 3, default is 2
+* `lessf: bool` - Changes the way the video is recorded so that the video becomes less fragile, with this flag you can use lossy compression, default is `False`
 
 ### Convert video to file(`videoToFile`)
 
 To get your file(s) back now you need to use this command:
 ```bash
 python -m pixelfuse videoToFile "test/example.video.avi"
 ```
 
 Where ["test/example.video.avi"](./test/example.video.avi) is the video you want to convert into file(s)
 
 As output, you will get the file with the name it was converted into a video. For example, if you converted the file "example.image.jpg", when you convert the video back to a file you get a file named example.image.jpg
 
-Or a folder with files, if you converted several files. By default, the folder name is the name of the video file without path or extension, but you can specify something else with the `exctractDir` parameter
+Or a folder with files, if you converted several files. By default, the folder name is the name of the video file without path or extension, but you can specify something else with the `extractDir` parameter
 
 Regarding the parameters:
 * `path: Path` - Mandatory, the path to the video you want to convert back to a file
 * `verbose: int` - Output level, from 0 to 2, default is 2
-* `exctractDir: str` - Path to extract archive files
+* `extractDir: str` - Path to extract archive files
+* `lessf: bool` - If the video was encoded with this flag, you need to use it. Otherwise the decoding will end with an error
 
 ## ⚠️ Warning
 
-Because of the way this converter works, the video output is **very, very** fragile
+Because of the way this converter works, the video output is **very, very** fragile, **about the `--lessf` flag below**.
 
-In order for you to be able to convert the file back, every pixel **MUST remain unchanged**, that is what you should avoid:
-* Use ONLY lossless codecs, as all other codecs corrupt the pixels. E.g. FFMPEG `FFV1`, Huffman `HFYU`, Lagarith `LAGS`, etc.
-* Do not convert videos to other formats, as this will most likely cause pixel damage
-* Keep in mind that if you upload videos to YouTube, it will re-encode the video(and, guess what, damage the pixels), so if you want to download videos from YouTube, you'll need to use [Google Takeout](https://takeout.google.com/)
-* Do not trim the video, it will trim some of the information, and therefore the file you converted
-* Do not apply filters to the video, for example. Anything that can change pixels will damage the file and you won't be able to decode it
-* Never convert zip archives, for some unknown reason the decoder (or encoder) cannot handle these archives properly, if you want to convert multiple files you better use the `filesToVideo` command
+In order for you to convert the file back, every pixel **MUST remain unchanged**, here is what you should avoid:
+* Use ONLY lossless codecs, as all other codecs corrupt the pixels. For example, FFMPEG `FFV1`, Huffman `HFYU`, Lagarith `LAGS` etc.
+* Do not convert videos to other formats, as this is likely to corrupt the pixels.
+* Remember that if you upload a video to YouTube, it will re-encode the video (and, guess what, damage the pixels), so if you want to download videos from YouTube, you need to use [Google Takeout](https://takeout.google.com/)
+* Don't trim the video, it will cut off some of the information and therefore the converted file.
+* Do not apply filters to the video, for example. Anything that can change pixels will damage the file and you won't be able to decode it.
+* Never convert zip archives, for some unknown reason the decoder (or encoder) cannot process these archives correctly. If you want to convert multiple files, it is better to use `filesToVideo` command.
+
+### About `--lessf` flag
+If you use this flag, the file will be encoded differently (using black and white squiggles), so you can compress videos with lossy codecs and post them on YouTube and download them without Google Takeout. It is also better not to apply filters, but for that matter **maybe** the file can still be decoded, but it is better not to do it. Otherwise, the restrictions for the --lessf flag are the same as for the normal encoding method
```

### Comparing `pixelfuse-2.0.0/pixelfuse/cli.py` & `pixelfuse-3.0.0/pixelfuse/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,29 +4,32 @@
 from pathlib import Path
 import tarfile
 from typing import Optional
 
 import typer
 from rich import print
 from rich.console import Console
+from pixelfuse.src.f2lfv import ToLessFragileVideo
 
 from pixelfuse.src.f2v import ToVideo
+from pixelfuse.src.lfv2f import LFVToFile
 from pixelfuse.src.v2f import ToFile
 
 app = typer.Typer()
 
 @app.command(name="filesToVideo")
 def filesToVideo(
     paths: list[Path]=typer.Argument(..., help="PathS to be converted to video. It can be either a file path or a folder path"),
     fps: Optional[float]=typer.Option(1., help="Frame rate of video"),
     width: Optional[int]=typer.Option(640, help="Video length"),
     height: Optional[int]=typer.Option(480, help="Video height"),
-    fourcc: Optional[str]=typer.Option("HFYU", help="Codec, a string of 4 characters, WARNING: Use lossless codecs ONLY"),
+    fourcc: Optional[str]=typer.Option("HFYU", help="Codec, a string of 4 characters, WARNING: Use lossless codecs ONLY(except for the --lessf flag)"),
     output: Optional[Path]=typer.Option("output.avi", help="Path to output file, note you need to use file extension compatible with codec, for example if you use HFYU codec you can NOT specify output as output.mp4"),
-    verbose: Optional[int]=typer.Option(2, help="Output level from 0 to 3")
+    verbose: Optional[int]=typer.Option(2, help="Output level from 0 to 3"),
+    LessF: Optional[bool]=typer.Option(False, help="Changes the way the video is recorded so that the video becomes less fragile, with this flag you can use lossy compression")
 ):
     console = Console()
 
     with console.status("[green]Creating archive...", spinner="dots12"):
         archive = tarfile.open(output.with_suffix(".tar.gz"), 'w:gz')
         hashmap = {}
 
@@ -47,31 +50,34 @@
                         console.print(f"[green]Added to archive:[/green] [magenta italic]{file}[/magenta italic] | {hashmap[file][:7]}")
             except FileNotFoundError:
                 continue
 
         archive.close()
 
     try:
-        c = ToVideo(output.with_suffix(".tar.gz"), fps, width, height, fourcc, output, verbose, hashmap)
+        enc = ToLessFragileVideo if LessF else ToVideo
+        c = enc(output.with_suffix(".tar.gz"), fps, width, height, fourcc, output, verbose, hashmap)
         c.convert()
         output.with_suffix(".tar.gz").unlink()
     except FileNotFoundError:
         print(f"[red bold]File {path} doesn't exist")
     except Exception as e:
         print("[red bold]Unknown error:")
         print(e)
 
 @app.command(name="videoToFile")
 def convertToFile(
     path: Path=typer.Argument(..., help="The path to the video you want to convert back to a file"),
     verbose: Optional[int]=typer.Option(2, help="Output level, from 0 to 2"),
-    exctractDir: Optional[str]=typer.Option(None, help="Path to extract archive files"),
+    extractDir: Optional[str]=typer.Option(None, help="Path to extract archive files"),
+    LessF: Optional[bool]=typer.Option(False, help="If the video was encoded with this flag, you need to use it. Otherwise the decoding will end with an error")
 ):
     try:
-        c = ToFile(path, verbose, exctractDir)
+        dec = LFVToFile if LessF else ToFile
+        c = dec(path, verbose, extractDir)
         c.convert()
     except FileExistsError as e:
         print(f"[red bold]{e}")
     except UnicodeDecodeError as e:
         print(f"[red bold]Cannot decode frames:[/red bold] {e}")
     except Exception as e:
         print(f"[red bold]Unknown error:")
@@ -79,19 +85,21 @@
 
 @app.command(name="fileToVideo")
 def convertToVideo(
     path: Path=typer.Argument(..., help="The path to the file you want to convert"),
     fps: Optional[float]=typer.Option(1., help="Frame rate of video"),
     width: Optional[int]=typer.Option(640, help="Video length"),
     height: Optional[int]=typer.Option(480, help="Video height"),
-    fourcc: Optional[str]=typer.Option("HFYU", help="Codec, a string of 4 characters, WARNING: Use lossless codecs ONLY"),
+    fourcc: Optional[str]=typer.Option("HFYU", help="Codec, a string of 4 characters, WARNING: Use lossless codecs ONLY(except for the --lessf flag)"),
     output: Optional[Path]=typer.Option("output.avi", help="Path to output file, note you need to use file extension compatible with codec, for example if you use HFYU codec you can NOT specify output as output.mp4"),
     verbose: Optional[int]=typer.Option(2, help="Output level from 0 to 3"),
+    LessF: Optional[bool]=typer.Option(False, help="Changes the way the video is recorded so that the video becomes less fragile, with this flag you can use lossy compression, default is `False`")
 ):
     try:
-        c = ToVideo(path, fps, width, height, fourcc, output, verbose)
+        enc = ToLessFragileVideo if LessF else ToVideo
+        c = enc(path, fps, width, height, fourcc, output, verbose)
         c.convert()
     except FileNotFoundError:
         print(f"[red bold]File {path} doesn't exist")
     except Exception as e:
         print("[red bold]Unknown error:")
         print(e)
```

### Comparing `pixelfuse-2.0.0/pixelfuse/src/f2v.py` & `pixelfuse-3.0.0/pixelfuse/src/f2v.py`

 * *Files identical despite different names*

### Comparing `pixelfuse-2.0.0/pixelfuse/src/v2f.py` & `pixelfuse-3.0.0/pixelfuse/src/v2f.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 import numpy as np
 from rich.console import Console
 
 from pixelfuse import compatible_encoders, decoder
 
 
 class ToFile:
-    def __init__(self, filename: Path, verbose, exctractDir):
+    def __init__(self, filename: Path, verbose, extractDir):
         self.cap = cv2.VideoCapture(filename.name)
         self.console = Console()
         self.verbose = verbose
-        self.exctractDir = exctractDir
+        self.extractDir = extractDir
 
         if not self.cap.isOpened(): 
             raise FileNotFoundError("Error opening video file")
 
     def writeTempFile(self):
         self.print("Start reading video", 1)
         ret, frame = self.cap.read()
@@ -32,15 +32,15 @@
 
         while(ret):
             if all(frame[0, 0] == [128, 4, 149]):
                 self.print("Found [128  4 149] meta frame", 1)
                 self.meta = pickle.loads(bytes(frame.flatten()))
 
                 if self.meta["encoder"] not in compatible_encoders:
-                    self.print_verbose(f"[yellow bold]Endcoder {self.meta['encoder']} isn't compatible with {decoder}", 0)
+                    self.print_verbose(f"[yellow bold]Encoder {self.meta['encoder']} isn't compatible with {decoder}", 0)
 
             if toWriteFrame is not None and self.meta is not None:
                 self.print(f"Preprocessing last {toWriteFrame[0, 0]} frame...", 1)
 
                 toWriteFrame = toWriteFrame.flatten().reshape((-1, 3))
                 while np.all(toWriteFrame[-1] == 0):
                     toWriteFrame = toWriteFrame[:-1]
@@ -75,17 +75,17 @@
         self.print(f"Remove temp file {self.temp.name}", 2)
         os.remove(self.temp.name)
 
     def extract(self):
         if self.meta["hashmap"] is not None:
             self.print(f"Extracting files...", 2)
             archive = tarfile.open(self.temp.name, "r:gz")
-            if self.exctractDir is None:
-                self.exctractDir = self.meta["filename"].split(".")[0]
-            archive.extractall(self.exctractDir)
+            if self.extractDir is None:
+                self.extractDir = self.meta["filename"].split(".")[0]
+            archive.extractall(self.extractDir)
             archive.close()
 
             self.print(f"Remove temp file {self.temp.name}", 2)
 
             os.remove(self.temp.name)
 
     def verify(self):
@@ -94,16 +94,16 @@
 
             if self.meta["checksum"] != hashlib.sha512(Path(self.meta["filename"]).read_bytes()).hexdigest():
                 self.print("[bold yellow]Checksums doesn't match!", 1)
 
             return
 
         for filename in self.meta["hashmap"]:
-            self.print(f"Verifing {filename}...", 2)
-            hashsum = hashlib.sha512(Path(self.exctractDir, filename).read_bytes()).hexdigest()
+            self.print(f"Verifying {filename}...", 2)
+            hashsum = hashlib.sha512(Path(self.extractDir, filename).read_bytes()).hexdigest()
             
             if hashsum != self.meta["hashmap"][filename]:
                 self.print(f"[bold yellow]{filename} checksum doesn't match!", 1)
 
     def convert(self):
         with self.console.status("[green]Decoding video..."):
             self.writeTempFile()
```

### Comparing `pixelfuse-2.0.0/pyproject.toml` & `pixelfuse-3.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pixelfuse"
-version = "2.0.0"
+version = "3.0.0"
 description = "Convert any file to video and video to file"
 authors = ["Roman <romantovt31@gmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 homepage = "https://github.com/TheTS-labs/PixelFuse"
 repository = "https://github.com/TheTS-labs/PixelFuse"
 keywords = ["video", "file", "converter"]
```

### Comparing `pixelfuse-2.0.0/PKG-INFO` & `pixelfuse-3.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixelfuse
-Version: 2.0.0
+Version: 3.0.0
 Summary: Convert any file to video and video to file
 Home-page: https://github.com/TheTS-labs/PixelFuse
 License: GPL-3.0
 Keywords: video,file,converter
 Author: Roman
 Author-email: romantovt31@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -20,15 +20,15 @@
 Project-URL: Repository, https://github.com/TheTS-labs/PixelFuse
 Description-Content-Type: text/markdown
 
 # 📄🔄🎞️ PixelFuse
 
 Convert any file to video and video to file.
 
-**WARNING: videos created from files are extremely fragile**
+**WARNING: videos created from files are very fragile. But if you create videos with the `--lessf` flag, the videos are not so fragile anymore**
 
 ## 💿 Installation
 
 * Set up using `pip`:
 ```bash
 pip install pixelfuse
 ```
@@ -51,17 +51,18 @@
 As output you get the file `output.avi` - video 640x480, 1.0 FPS, codec HFYU [like this](https://drive.google.com/file/d/1OTZ9rF-6SI73BiLEwY4gJeJ2RVddLsfn/edit)
 
 As for the parameters:
 * `path: Path` - mandatory, the path to the file you want to convert
 * `fps: float` - frame rate, default is `1.0`
 * `width: int` - Video length, default is `480px`
 * `height: int` - Video height, `640px` by default
-* `fourcc: str` - Codec, a string of 4 characters, **WARNING: Use lossless codecs ONLY**, default is "`HFYU`".
+* `fourcc: str` - Codec, a string of 4 characters, **WARNING: Use lossless codecs ONLY(except for the `--lessf` flag)**, default is "`HFYU`".
 * `output: Path` - Path to output file, default is "`output.avi`", **note you need to use file extension compatible with codec, for example if you use `HFYU` codec you can NOT specify `output` as `output.mp4`**
 * `verbose: int` - Output level, from 0 to 3, default is 2
+* `lessf: bool` - Changes the way the video is recorded so that the video becomes less fragile, with this flag you can use lossy compression, default is `False`
 
 ### 🆕 Convert files to video(`filesToVideo`)
 
 To convert a file into a video just write the following command:
 ```bash
 python -m pixelfuse filesToVideo "test/example.text.txt" "test/example.image.jpg"
 ```
@@ -75,41 +76,45 @@
 As output you get the file `output.avi` - video 640x480, 1.0 FPS, codec HFYU [like this](https://drive.google.com/file/d/1OTZ9rF-6SI73BiLEwY4gJeJ2RVddLsfn/edit)
 
 As for the parameters:
 * `paths: list[Path]` - mandatory, the paths to the files you want to convert
 * `fps: float` - frame rate, default is `1.0`
 * `width: int` - Video length, default is `480px`
 * `height: int` - Video height, `640px` by default
-* `fourcc: str` - Codec, a string of 4 characters, **WARNING: Use lossless codecs ONLY**, default is "`HFYU`".
+* `fourcc: str` - Codec, a string of 4 characters, **WARNING: Use lossless codecs ONLY(except for the `--lessf` flag)**, default is "`HFYU`".
 * `output: Path` - Path to output file, default is "`output.avi`", **note you need to use file extension compatible with codec, for example if you use `HFYU` codec you can NOT specify `output` as `output.mp4`**
 * `verbose: int` - Output level, from 0 to 3, default is 2
+* `lessf: bool` - Changes the way the video is recorded so that the video becomes less fragile, with this flag you can use lossy compression, default is `False`
 
 ### Convert video to file(`videoToFile`)
 
 To get your file(s) back now you need to use this command:
 ```bash
 python -m pixelfuse videoToFile "test/example.video.avi"
 ```
 
 Where ["test/example.video.avi"](./test/example.video.avi) is the video you want to convert into file(s)
 
 As output, you will get the file with the name it was converted into a video. For example, if you converted the file "example.image.jpg", when you convert the video back to a file you get a file named example.image.jpg
 
-Or a folder with files, if you converted several files. By default, the folder name is the name of the video file without path or extension, but you can specify something else with the `exctractDir` parameter
+Or a folder with files, if you converted several files. By default, the folder name is the name of the video file without path or extension, but you can specify something else with the `extractDir` parameter
 
 Regarding the parameters:
 * `path: Path` - Mandatory, the path to the video you want to convert back to a file
 * `verbose: int` - Output level, from 0 to 2, default is 2
-* `exctractDir: str` - Path to extract archive files
+* `extractDir: str` - Path to extract archive files
+* `lessf: bool` - If the video was encoded with this flag, you need to use it. Otherwise the decoding will end with an error
 
 ## ⚠️ Warning
 
-Because of the way this converter works, the video output is **very, very** fragile
+Because of the way this converter works, the video output is **very, very** fragile, **about the `--lessf` flag below**.
 
-In order for you to be able to convert the file back, every pixel **MUST remain unchanged**, that is what you should avoid:
-* Use ONLY lossless codecs, as all other codecs corrupt the pixels. E.g. FFMPEG `FFV1`, Huffman `HFYU`, Lagarith `LAGS`, etc.
-* Do not convert videos to other formats, as this will most likely cause pixel damage
-* Keep in mind that if you upload videos to YouTube, it will re-encode the video(and, guess what, damage the pixels), so if you want to download videos from YouTube, you'll need to use [Google Takeout](https://takeout.google.com/)
-* Do not trim the video, it will trim some of the information, and therefore the file you converted
-* Do not apply filters to the video, for example. Anything that can change pixels will damage the file and you won't be able to decode it
-* Never convert zip archives, for some unknown reason the decoder (or encoder) cannot handle these archives properly, if you want to convert multiple files you better use the `filesToVideo` command
+In order for you to convert the file back, every pixel **MUST remain unchanged**, here is what you should avoid:
+* Use ONLY lossless codecs, as all other codecs corrupt the pixels. For example, FFMPEG `FFV1`, Huffman `HFYU`, Lagarith `LAGS` etc.
+* Do not convert videos to other formats, as this is likely to corrupt the pixels.
+* Remember that if you upload a video to YouTube, it will re-encode the video (and, guess what, damage the pixels), so if you want to download videos from YouTube, you need to use [Google Takeout](https://takeout.google.com/)
+* Don't trim the video, it will cut off some of the information and therefore the converted file.
+* Do not apply filters to the video, for example. Anything that can change pixels will damage the file and you won't be able to decode it.
+* Never convert zip archives, for some unknown reason the decoder (or encoder) cannot process these archives correctly. If you want to convert multiple files, it is better to use `filesToVideo` command.
 
+### About `--lessf` flag
+If you use this flag, the file will be encoded differently (using black and white squiggles), so you can compress videos with lossy codecs and post them on YouTube and download them without Google Takeout. It is also better not to apply filters, but for that matter **maybe** the file can still be decoded, but it is better not to do it. Otherwise, the restrictions for the --lessf flag are the same as for the normal encoding method
```

