# Comparing `tmp/aij-1.0.7.tar.gz` & `tmp/aij-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-1.0.7.tar", last modified: Tue May 16 14:26:12 2023, max compression
+gzip compressed data, was "aij-1.0.8.tar", last modified: Sun May 21 19:36:43 2023, max compression
```

## Comparing `aij-1.0.7.tar` & `aij-1.0.8.tar`

### file list

```diff
@@ -1,33 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 14:26:14.000000 aij-1.0.7/
--rw-rw-rw-   0        0        0     1100 2023-05-05 12:30:16.000000 aij-1.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0    30052 2023-05-16 14:26:14.000000 aij-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0    27745 2023-05-10 22:39:42.000000 aij-1.0.7/README.md
--rw-rw-rw-   0        0        0     6363 2023-05-16 14:25:48.000000 aij-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 14:26:14.000000 aij-1.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-16 14:26:14.000000 aij-1.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 14:26:14.000000 aij-1.0.7/src/aij.egg-info/
--rw-rw-rw-   0        0        0    30052 2023-05-16 14:26:14.000000 aij-1.0.7/src/aij.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      506 2023-05-16 14:26:14.000000 aij-1.0.7/src/aij.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 14:26:14.000000 aij-1.0.7/src/aij.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-05-16 14:26:14.000000 aij-1.0.7/src/aij.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      213 2023-05-16 14:26:14.000000 aij-1.0.7/src/aij.egg-info/requires.txt
--rw-rw-rw-   0        0        0       41 2023-05-16 14:26:14.000000 aij-1.0.7/src/aij.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-16 14:26:14.000000 aij-1.0.7/src/intro/
--rw-rw-rw-   0        0        0        0 2023-05-16 08:04:50.000000 aij-1.0.7/src/intro/__init__.py
--rw-rw-rw-   0        0        0     4532 2023-05-15 21:53:56.000000 aij-1.0.7/src/intro/intro.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:26:14.000000 aij-1.0.7/src/messaging/
--rw-rw-rw-   0        0        0      213 2023-05-16 14:04:28.000000 aij-1.0.7/src/messaging/__init__.py
--rw-rw-rw-   0        0        0     4151 2023-05-16 14:18:30.000000 aij-1.0.7/src/messaging/views.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:26:14.000000 aij-1.0.7/src/news/
--rw-rw-rw-   0        0        0      466 2023-05-16 13:53:54.000000 aij-1.0.7/src/news/__init__.py
--rw-rw-rw-   0        0        0     4292 2023-05-16 14:24:04.000000 aij-1.0.7/src/news/models.py
--rw-rw-rw-   0        0        0     4768 2023-05-16 14:26:00.000000 aij-1.0.7/src/news/views.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:26:14.000000 aij-1.0.7/src/setup/
--rw-rw-rw-   0        0        0     2974 2023-05-16 09:54:22.000000 aij-1.0.7/src/setup/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:26:14.000000 aij-1.0.7/src/speech/
--rw-rw-rw-   0        0        0      163 2023-05-15 20:59:02.000000 aij-1.0.7/src/speech/__init__.py
--rw-rw-rw-   0        0        0     1070 2023-05-15 21:51:26.000000 aij-1.0.7/src/speech/talk.py
--rw-rw-rw-   0        0        0      880 2023-05-15 21:52:02.000000 aij-1.0.7/src/speech/whisperx.py
--rw-rw-rw-   0        0        0      579 2023-05-14 21:57:48.000000 aij-1.0.7/src/speech/whisperxx.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:26:14.000000 aij-1.0.7/src/webcam/
--rw-rw-rw-   0        0        0    17500 2023-05-15 20:59:02.000000 aij-1.0.7/src/webcam/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 19:36:43.760583 aij-1.0.8/
+-rw-rw-rw-   0        0        0     1100 2023-05-21 18:35:40.000000 aij-1.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0    30052 2023-05-21 19:36:43.759586 aij-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0    27745 2023-05-21 18:35:40.000000 aij-1.0.8/README.md
+-rw-rw-rw-   0        0        0     6363 2023-05-21 19:36:29.000000 aij-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-21 19:36:43.761593 aij-1.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-21 19:36:43.701261 aij-1.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-05-21 19:36:43.741925 aij-1.0.8/src/aij.egg-info/
+-rw-rw-rw-   0        0        0    30052 2023-05-21 19:36:43.000000 aij-1.0.8/src/aij.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      382 2023-05-21 19:36:43.000000 aij-1.0.8/src/aij.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 19:36:43.000000 aij-1.0.8/src/aij.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-05-21 19:36:43.000000 aij-1.0.8/src/aij.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      213 2023-05-21 19:36:43.000000 aij-1.0.8/src/aij.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       46 2023-05-21 19:36:43.000000 aij-1.0.8/src/aij.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-21 19:36:43.742929 aij-1.0.8/src/chat/
+-rw-rw-rw-   0        0        0      563 2023-05-21 19:33:03.000000 aij-1.0.8/src/chat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 19:36:43.744445 aij-1.0.8/src/intro/
+-rw-rw-rw-   0        0        0     4607 2023-05-21 19:15:32.000000 aij-1.0.8/src/intro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 19:36:43.747473 aij-1.0.8/src/messaging/
+-rw-rw-rw-   0        0        0     4444 2023-05-21 19:19:30.000000 aij-1.0.8/src/messaging/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 19:36:43.750012 aij-1.0.8/src/news/
+-rw-rw-rw-   0        0        0     9588 2023-05-21 19:19:41.000000 aij-1.0.8/src/news/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 19:36:43.752014 aij-1.0.8/src/setup/
+-rw-rw-rw-   0        0        0     3080 2023-05-21 19:19:56.000000 aij-1.0.8/src/setup/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 19:36:43.754534 aij-1.0.8/src/speech/
+-rw-rw-rw-   0        0        0     1289 2023-05-21 19:35:54.000000 aij-1.0.8/src/speech/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 19:36:43.756581 aij-1.0.8/src/webcam/
+-rw-rw-rw-   0        0        0    17592 2023-05-21 19:07:03.000000 aij-1.0.8/src/webcam/__init__.py
```

### Comparing `aij-1.0.7/LICENSE.txt` & `aij-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-1.0.7/PKG-INFO` & `aij-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.0.7
+Version: 1.0.8
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.0.7/README.md` & `aij-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `aij-1.0.7/pyproject.toml` & `aij-1.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.7"
+version = "1.0.8"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist"  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `aij-1.0.7/src/aij.egg-info/PKG-INFO` & `aij-1.0.8/src/aij.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.0.7
+Version: 1.0.8
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.0.7/src/intro/intro.py` & `aij-1.0.8/src/intro/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,15 +69,16 @@
         x = 0
         y = 0
 
         # Generate the animation frames
         num_frames = self.fps * self.duration
         for i in range(num_frames):
             # Create a blank frame
-            frame = np.zeros((self.animation_height, self.animation_width, 3), dtype=np.uint8)
+            frame = np.zeros(
+                (self.animation_height, self.animation_width, 3), dtype=np.uint8)
 
             # Choose a random image and resize it to 1920x1080 pixels (Full HD).
             # Make sure the aspect ratio is maintained while resizing
             img = self.images[i % len(self.images)]
             img = cv2.resize(img, (1920, 1080), interpolation=cv2.INTER_AREA)
 
             # Update the image position
@@ -104,15 +105,16 @@
 
         # merge the audio and video files
         os.system(
             'ffmpeg -i animation.mp4 -i ' + self.audio_intro_abs +
             ' -c:v copy -c:a aac -strict experimental animation_with_audio.mp4')
 
         # Print the path of the animation video
-        print('Animation video generated at: ' + os.getcwd() + SEP + 'animation_with_audio.mp4')
+        print('Animation video generated at: ' +
+            os.getcwd() + SEP + 'animation_with_audio.mp4')
 
 
 def main():
     """
     This function is the entry point of the program
     @param: None
     @return: None
@@ -125,7 +127,11 @@
     print('Doing some other work here...')
 
     # Wait for the animation thread to finish
     animation_thread.join()
 
     # Destroy all windows
     cv2.destroyAllWindows()
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `aij-1.0.7/src/messaging/views.py` & `aij-1.0.8/src/messaging/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 
 from kivy.app import App
 from kivy.core.window import Window
 from kivy.uix.boxlayout import BoxLayout
 from kivy.uix.button import Button
 from kivy.uix.label import Label
 
+from dotenv import load_dotenv
+
+load_dotenv()  # take environment variables from .env.
 
 class AIJMessagingServer(App):
     """
     A class to create a GUI for the publisher and subscriber
     """
 
     def build(self):
@@ -23,15 +26,16 @@
         self.title = 'AIJ News'
         self.icon = 'logo.png'
 
         # create a layout for the publisher
         self.publisher_layout = BoxLayout(orientation='vertical', padding=10)
 
         # create a label for the publisher
-        self.publisher_label = Label(text='RabbitMQ Messaging Server', size_hint=(1, 0.90))
+        self.publisher_label = Label(
+            text='RabbitMQ Messaging Server', size_hint=(1, 0.90))
 
         # create a button for the publisher
         self.publisher_button = Button(text='Start', size_hint=(1, 0.10))
 
         # change the background color of the button to red
         self.publisher_button.background_color = (1, 0, 0, 1)
 
@@ -87,18 +91,20 @@
         self.publisher_button.bind(on_press=self.start)
 
         # change the background color of the button to red
         self.publisher_button.background_color = (1, 0, 0, 1)
 
     def listen(self):
         # connect to RabbitMQ server and read logs using pika
-        connection = pika.BlockingConnection(pika.ConnectionParameters('localhost'))
+        connection = pika.BlockingConnection(
+            pika.ConnectionParameters('localhost'))
         channel = connection.channel()
         # print all the channel logs
-        channel.basic_consume(queue='logs', on_message_callback=self.print_logs, auto_ack=True)
+        channel.basic_consume(
+            queue='logs', on_message_callback=self.print_logs, auto_ack=True)
 
         # start listening to the logs
         channel.start_consuming()
 
     def print_logs(self, ch, method, properties, body):
         """
         The method to print the logs
@@ -112,7 +118,17 @@
         """
         The method to stop the RabbitMQ server when the app is closed
         The key event is triggered when the escape key is pressed
         """
         if key == 27:
             os.system('rabbitmqctl stop')
             return True
+
+
+def main():
+    # start an instance of AIJMessagingServer class
+    msg = AIJMessagingServer()
+    msg.run()
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `aij-1.0.7/src/setup/__init__.py` & `aij-1.0.8/src/setup/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 import os
 import urllib.request
 
+from dotenv import load_dotenv
+
+load_dotenv()  # take environment variables from .env.
+
 user_profile = os.environ['USERPROFILE']
 SEP = os.path.sep
 
 
 def kernel():
     """
     Get the operating system kernel name
@@ -63,15 +67,16 @@
             os.system('sudo pacman -S python')
             os.system('sudo pacman -S rabbitmq')
             os.system('sudo pacman -S redis')
 
     elif kernel() == 'Windows':
 
         # install the scoop package manager
-        urllib.request.urlretrieve('https://get.scoop.sh', f'{user_profile}{SEP}scoop.ps1')
+        urllib.request.urlretrieve(
+            'https://get.scoop.sh', f'{user_profile}{SEP}scoop.ps1')
 
         # add scoop to the PATH environment variable
         os.system(f'set-executionpolicy remotesigned -scope currentuser')
 
         # install scoop
         os.system(f'{user_profile}{SEP}scoop.ps1')
```

### Comparing `aij-1.0.7/src/webcam/__init__.py` & `aij-1.0.8/src/webcam/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 import mediapipe as mp
 
 from gtts import gTTS
 from pygame import mixer
 
 from newsapi import NewsApiClient        
 
+from dotenv import load_dotenv
+
+load_dotenv()  # take environment variables from .env.
+
 # Constants and global variables
 api = NewsApiClient(api_key=os.environ['NEWSAPI_ORG'])
 user_profile = os.environ['USERPROFILE']
 SEP = os.path.sep
 LOGO_URL = "https://raw.githubusercontent.com/codesapienbe/aij-webcam/master/logo.png"
 CSV_URL = "https://raw.githubusercontent.com/codesapienbe/aij-webcam/master/news.csv"
```

