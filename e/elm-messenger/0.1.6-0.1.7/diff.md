# Comparing `tmp/elm-messenger-0.1.6.tar.gz` & `tmp/elm-messenger-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elm-messenger-0.1.6.tar", last modified: Fri May 12 15:52:53 2023, max compression
+gzip compressed data, was "elm-messenger-0.1.7.tar", last modified: Sun May 21 09:28:54 2023, max compression
```

## Comparing `elm-messenger-0.1.6.tar` & `elm-messenger-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-12 15:52:53.003374 elm-messenger-0.1.6/
--rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2023-05-04 10:50:53.000000 elm-messenger-0.1.6/MANIFEST.in
--rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-12 15:52:53.003374 elm-messenger-0.1.6/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      122 2023-05-04 10:50:53.000000 elm-messenger-0.1.6/Readme.md
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-12 15:52:53.000041 elm-messenger-0.1.6/elm_messenger.egg-info/
--rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-12 15:52:52.000000 elm-messenger-0.1.6/elm_messenger.egg-info/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      368 2023-05-12 15:52:53.000000 elm-messenger-0.1.6/elm_messenger.egg-info/SOURCES.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2023-05-12 15:52:52.000000 elm-messenger-0.1.6/elm_messenger.egg-info/dependency_links.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2023-05-12 15:52:52.000000 elm-messenger-0.1.6/elm_messenger.egg-info/entry_points.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        6 2023-05-12 15:52:52.000000 elm-messenger-0.1.6/elm_messenger.egg-info/requires.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2023-05-12 15:52:52.000000 elm-messenger-0.1.6/elm_messenger.egg-info/top_level.txt
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-12 15:52:53.003374 elm-messenger-0.1.6/messengercli/
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 10:50:53.000000 elm-messenger-0.1.6/messengercli/__init__.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2023-05-04 10:50:53.000000 elm-messenger-0.1.6/messengercli/command_line.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)    13779 2023-05-12 15:51:50.000000 elm-messenger-0.1.6/messengercli/messenger.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)     1170 2023-05-12 14:41:01.000000 elm-messenger-0.1.6/messengercli/updater.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)      407 2023-05-12 15:52:53.003374 elm-messenger-0.1.6/setup.cfg
--rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2023-05-04 10:50:53.000000 elm-messenger-0.1.6/setup.py
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-21 09:28:54.119096 elm-messenger-0.1.7/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2023-05-04 10:50:53.000000 elm-messenger-0.1.7/MANIFEST.in
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-21 09:28:54.119096 elm-messenger-0.1.7/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      122 2023-05-04 10:50:53.000000 elm-messenger-0.1.7/Readme.md
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-21 09:28:54.119096 elm-messenger-0.1.7/elm_messenger.egg-info/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-21 09:28:54.000000 elm-messenger-0.1.7/elm_messenger.egg-info/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      368 2023-05-21 09:28:54.000000 elm-messenger-0.1.7/elm_messenger.egg-info/SOURCES.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2023-05-21 09:28:54.000000 elm-messenger-0.1.7/elm_messenger.egg-info/dependency_links.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2023-05-21 09:28:54.000000 elm-messenger-0.1.7/elm_messenger.egg-info/entry_points.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        6 2023-05-21 09:28:54.000000 elm-messenger-0.1.7/elm_messenger.egg-info/requires.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2023-05-21 09:28:54.000000 elm-messenger-0.1.7/elm_messenger.egg-info/top_level.txt
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-21 09:28:54.119096 elm-messenger-0.1.7/messengercli/
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 10:50:53.000000 elm-messenger-0.1.7/messengercli/__init__.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2023-05-04 10:50:53.000000 elm-messenger-0.1.7/messengercli/command_line.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)    16909 2023-05-21 09:26:59.000000 elm-messenger-0.1.7/messengercli/messenger.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     1170 2023-05-12 14:41:01.000000 elm-messenger-0.1.7/messengercli/updater.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      407 2023-05-21 09:28:54.119096 elm-messenger-0.1.7/setup.cfg
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2023-05-04 10:50:53.000000 elm-messenger-0.1.7/setup.py
```

### Comparing `elm-messenger-0.1.6/messengercli/messenger.py` & `elm-messenger-0.1.7/messengercli/messenger.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,27 +8,31 @@
 import typer
 import os
 import shutil
 import json
 from .updater import Updater
 
 app = typer.Typer(add_completion=False, help="Messenger CLI")
-API_VERSION = "0.1.6"
+API_VERSION = "0.1.7"
 
 
 class Messenger:
     config = None
 
     def __init__(self) -> None:
         """
         Check if `messager.json` exists and load it.
         """
         if os.path.exists("messenger.json"):
             with open("messenger.json", "r") as f:
                 self.config = json.load(f)
+            if "version" not in self.config:
+                raise Exception("API version not found in the config file.")
+            if self.config["version"] != API_VERSION:
+                raise Exception(f"API version not matched. I'm using v{API_VERSION}.")
         else:
             raise Exception(
                 "messenger.json not found. Are you in the project initialized by the Messenger? Try `messenger init <your-project-name>`."
             )
 
     def dump_config(self):
         with open("messenger.json", "w") as f:
@@ -43,23 +47,38 @@
 
         Updater(
             [
                 ".messenger/scene/Sample/Common.elm",
                 ".messenger/scene/Sample/Export.elm",
                 ".messenger/scene/Sample/Global.elm",
                 ".messenger/scene/Sample/LayerBase.elm",
+                ".messenger/scene/Sample/LayerInit.elm",
             ],
             [
                 f"src/Scenes/{scene}/Common.elm",
                 f"src/Scenes/{scene}/Export.elm",
                 f"src/Scenes/{scene}/Global.elm",
                 f"src/Scenes/{scene}/LayerBase.elm",
+                f"src/Scenes/{scene}/LayerInit.elm",
             ],
         ).rep(scene)
 
+        # Modify Scene
+        with open("src/Lib/Scene/Base.elm", "r") as f:
+            scenebase = f.read()
+        new_scenebase = scenebase.replace(
+            "type SceneInitData\n    =",
+            f"type SceneInitData\n    = {scene}InitData {scene}Init\n    |",
+        ).replace(
+            "import Lib.Env.Env exposing (Env)",
+            f"import Lib.Env.Env exposing (Env)\nimport Scenes.{scene}.LayerInit exposing ({scene}Init)",
+        )
+        with open("src/Lib/Scene/Base.elm", "w") as f:
+            f.write(new_scenebase)
+
     def update_scenes(self):
         """
         Update scene settings (AllScenes and SceneSettings)
         """
         scenes = self.config["scenes"]
         sceneprotos = self.config["sceneprotos"]
         Updater([".messenger/scene/AllScenes.elm"], ["src/Scenes/AllScenes.elm"]).rep(
@@ -116,29 +135,35 @@
         Add a sceneproto
         """
         if scene in self.config["scenes"] or scene in self.config["sceneprotos"]:
             raise Exception("Sceneproto already exists.")
         self.config["sceneprotos"][scene] = {"levels": [], "layers": []}
         self.dump_config()
         os.mkdir(f"src/SceneProtos/{scene}")
+        os.mkdir(f"src/SceneProtos/{scene}/GameComponent")
+        os.mkdir(f"src/SceneProtos/{scene}/GameComponents")
 
         Updater(
             [
                 ".messenger/sceneproto/scene/Common.elm",
                 ".messenger/sceneproto/scene/Export.elm",
                 ".messenger/sceneproto/scene/Global.elm",
                 ".messenger/sceneproto/scene/LayerBase.elm",
                 ".messenger/sceneproto/scene/LayerInit.elm",
+                ".messenger/sceneproto/gamecomponent/Base.elm",
+                ".messenger/sceneproto/gamecomponent/Handler.elm",
             ],
             [
                 f"src/SceneProtos/{scene}/Common.elm",
                 f"src/SceneProtos/{scene}/Export.elm",
                 f"src/SceneProtos/{scene}/Global.elm",
                 f"src/SceneProtos/{scene}/LayerBase.elm",
                 f"src/SceneProtos/{scene}/LayerInit.elm",
+                f"src/SceneProtos/{scene}/GameComponent/Base.elm",
+                f"src/SceneProtos/{scene}/GameComponent/Handler.elm",
             ],
         ).rep(scene)
 
         # Modify Scene
         with open("src/Lib/Scene/Base.elm", "r") as f:
             scenebase = f.read()
         new_scenebase = scenebase.replace(
@@ -203,15 +228,15 @@
                     f"import SceneProtos.{sceneproto}.{l}.Export as {l}\nimport SceneProtos.{sceneproto}.{l}.Global as {l}G"
                     for l in layers
                 ]
             )
         ).rep(
             ",\n".join(
                 [
-                    f"{l}G.getLayerT <| {l}.initLayer (addCommonData nullCommonData env) NullLayerInitData"
+                    f"{l}G.getLayerT <| {l}.initLayer (addCommonData nullCommonData env) ({l}.initFromScene env layerInitData)"
                     for l in layers
                 ]
             )
         )
 
     def add_level(self, sceneproto: str, level: str):
         """
@@ -237,14 +262,45 @@
             [
                 ".messenger/component/Sample/Sample.elm",
                 ".messenger/component/Sample/Export.elm",
             ],
             [f"src/Components/{name}/{name}.elm", f"src/Components/{name}/Export.elm"],
         ).rep(name)
 
+    def add_gamecomponent(self, sceneproto: str, gc: str):
+        """
+        Add a GameComponent to a SceneProto
+        """
+        if sceneproto not in self.config["sceneprotos"]:
+            raise Exception("SceneProto doesn't exist.")
+        
+        os.mkdir(f"src/SceneProtos/{sceneproto}/GameComponents/{gc}")
+        Updater([
+            ".messenger/sceneproto/gamecomponent/Sample/Base.elm",
+            ".messenger/sceneproto/gamecomponent/Sample/Export.elm",
+            ".messenger/sceneproto/gamecomponent/Sample/Model.elm",
+        ],[
+            f"src/SceneProtos/{sceneproto}/GameComponents/{gc}/Base.elm",
+            f"src/SceneProtos/{sceneproto}/GameComponents/{gc}/Export.elm",
+            f"src/SceneProtos/{sceneproto}/GameComponents/{gc}/Model.elm"
+        ]).rep(sceneproto).rep(gc)
+
+        # Modify GameComponent
+        with open(f"src/SceneProtos/{sceneproto}/GameComponent/Base.elm", "r") as f:
+            scenebase = f.read()
+        new_scenebase = scenebase.replace(
+            "type GameComponentInitData\n    =",
+            f"type GameComponentInitData\n    = GC{gc}InitData {gc}Init\n    |",
+        ).replace(
+            "import Messenger.GeneralModel exposing (GeneralModel)",
+            f"import Messenger.GeneralModel exposing (GeneralModel)\nimport SceneProtos.{sceneproto}.GameComponents.{gc}.Base exposing ({gc}Init)",
+        )
+        with open(f"src/SceneProtos/{sceneproto}/GameComponent/Base.elm", "w") as f:
+            f.write(new_scenebase)
+
     def format(self):
         os.system("elm-format src/ --yes")
 
     def add_layer(self, scene: str, layer: str):
         """
         Add a layer to a scene
         """
@@ -294,15 +350,15 @@
                     f"import Scenes.{scene}.{l}.Export as {l}\nimport Scenes.{scene}.{l}.Global as {l}G"
                     for l in layers
                 ]
             )
         ).rep(
             ",\n".join(
                 [
-                    f"{l}G.getLayerT <| {l}.initLayer (addCommonData nullCommonData env) NullLayerInitData"
+                    f"{l}G.getLayerT <| {l}.initLayer (addCommonData nullCommonData env)  ({l}.initFromScene env layerInitData)"
                     for l in layers
                 ]
             )
         )
 
 
 @app.command()
@@ -410,10 +466,19 @@
         f"You are going to create a layer named {layer} under sceneproto {sceneproto}, continue?"
     )
     msg.add_sceneproto_layer(sceneproto, layer)
     msg.update_sceneproto_layers(sceneproto)
     msg.format()
     print("Done!")
 
+@app.command()
+def gamecomponent(sceneproto:str, gc:str):
+    msg = Messenger()
+    input(
+        f"You are going to create a game component named {gc} under sceneproto {sceneproto}, continue?"
+    )
+    msg.add_gamecomponent(sceneproto, gc)
+    msg.format()
+    print("Done!")
 
 if __name__ == "__main__":
     app()
```

### Comparing `elm-messenger-0.1.6/messengercli/updater.py` & `elm-messenger-0.1.7/messengercli/updater.py`

 * *Files identical despite different names*

