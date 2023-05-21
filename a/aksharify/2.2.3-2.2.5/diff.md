# Comparing `tmp/aksharify-2.2.3.tar.gz` & `tmp/aksharify-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aksharify-2.2.3.tar", last modified: Wed May 10 19:49:07 2023, max compression
+gzip compressed data, was "aksharify-2.2.5.tar", last modified: Sun May 21 09:23:44 2023, max compression
```

## Comparing `aksharify-2.2.3.tar` & `aksharify-2.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 19:49:07.866711 aksharify-2.2.3/
--rw-rw-rw-   0        0        0     1094 2023-05-09 13:06:55.000000 aksharify-2.2.3/LICENSE.md
--rw-rw-rw-   0        0        0     4425 2023-05-10 19:49:07.866711 aksharify-2.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     3909 2023-05-10 19:21:28.000000 aksharify-2.2.3/README.md
--rw-rw-rw-   0        0        0      622 2023-05-10 19:48:28.000000 aksharify-2.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-10 19:49:07.866711 aksharify-2.2.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-10 19:49:07.825653 aksharify-2.2.3/src/
--rw-rw-rw-   0        0        0        0 2023-05-09 16:00:52.000000 aksharify-2.2.3/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 19:49:07.864679 aksharify-2.2.3/src/aksharify.egg-info/
--rw-rw-rw-   0        0        0     4425 2023-05-10 19:49:07.000000 aksharify-2.2.3/src/aksharify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-05-10 19:49:07.000000 aksharify-2.2.3/src/aksharify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 19:49:07.000000 aksharify-2.2.3/src/aksharify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-10 19:49:07.000000 aksharify-2.2.3/src/aksharify.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-10 19:49:07.000000 aksharify-2.2.3/src/aksharify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3137 2023-05-10 19:42:24.000000 aksharify-2.2.3/src/aksharify.py
+drwxrwxrwx   0        0        0        0 2023-05-21 09:23:44.165078 aksharify-2.2.5/
+-rw-rw-rw-   0        0        0     1094 2023-05-09 13:06:55.000000 aksharify-2.2.5/LICENSE.md
+-rw-rw-rw-   0        0        0     4709 2023-05-21 09:23:44.163038 aksharify-2.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4193 2023-05-11 14:40:43.000000 aksharify-2.2.5/README.md
+-rw-rw-rw-   0        0        0      622 2023-05-21 09:22:31.000000 aksharify-2.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-21 09:23:44.165078 aksharify-2.2.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-21 09:23:44.086470 aksharify-2.2.5/src/
+-rw-rw-rw-   0        0        0        0 2023-05-09 16:00:52.000000 aksharify-2.2.5/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 09:23:44.158620 aksharify-2.2.5/src/aksharify.egg-info/
+-rw-rw-rw-   0        0        0     4709 2023-05-21 09:23:44.000000 aksharify-2.2.5/src/aksharify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-05-21 09:23:44.000000 aksharify-2.2.5/src/aksharify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 09:23:44.000000 aksharify-2.2.5/src/aksharify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-21 09:23:44.000000 aksharify-2.2.5/src/aksharify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-21 09:23:44.000000 aksharify-2.2.5/src/aksharify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3169 2023-05-21 08:47:16.000000 aksharify-2.2.5/src/aksharify.py
```

### Comparing `aksharify-2.2.3/LICENSE.md` & `aksharify-2.2.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aksharify-2.2.3/PKG-INFO` & `aksharify-2.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aksharify
-Version: 2.2.3
+Version: 2.2.5
 Summary: Ascii art module
 Author-email: Prime Patel <primespatel@gmail.com>
 Project-URL: Homepage, https://github.com/primepatel/aksharify
 Project-URL: Bug Tracker, https://github.com/primepatel/aksharify/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -42,16 +42,34 @@
 ```
 
 ## Usage
 
 ```python
 from aksharify import TextArt
 
+# input image file
 art = TextArt("Julia.png")
+
+# see image
 art.image.show()
+
+# set dimension of output text
+art.set_dim(80)
+
+# genetate text
+art.asciify()
+
+# output into .txt file
+art.text_output("output")
+
+# generate colored text using html
+art.colorify()
+
+# output into .html file
+art.color_output("output")
 ```
 
 _For examples from user community, please refer to the [primepatel.github.io/aksharify](https://primepatel.github.io/aksharify)_
 
 
 <!-- ROADMAP -->
 ## Roadmap
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aksharify Version: 2.2.3 Summary: Ascii art module
+Metadata-Version: 2.1 Name: aksharify Version: 2.2.5 Summary: Ascii art module
 Author-email: Prime Patel
 gmail.com> Project-URL: Homepage, https://github.com/primepatel/aksharify
 Project-URL: Bug Tracker, https://github.com/primepatel/aksharify/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE.md  # __Aksharify__ [![Contributors][contributors-shield]]
@@ -14,33 +14,36 @@
 It motivated me to explore the possibilities of such a prime number. I created
 a Python module that uses a predetermined character set to turn photos into
 ASCII art. It manipulates images using the PIL package, transforming them to
 grayscale before mapping pixel values to ASCII letters. Users can change the
 character set to get different effects.  ## Getting Started Before we begin,
 make sure you have one of recent versions of Python installed on your computer.
 ### Installation ```sh python -m pip install aksharify ``` ## Usage ```python
-from aksharify import TextArt art = TextArt("Julia.png") art.image.show() ```
-_For examples from user community, please refer to the [primepatel.github.io/
-aksharify](https://primepatel.github.io/aksharify)_  ## Roadmap - [x] NumberiFy
-- [-] Predifined order of characters - [-] Getting images from URL - [-
-] EmojiFy See the [open issues](https://github.com/github_username/repo_name/
-issues) for a full list of proposed features (and known issues).  ##
-Contributing Contributions are what make the open source community such a
-wonderful place to learn, be inspired, and create. Any contributions you make
-are `appreciated greatly`. If you have a suggestion that would make this
-better, please fork the repo and create a pull request. You can also simply
-open an issue with the tag "enhancement". Don't forget to give the project a
-star! Thanks again! 1. Fork the Project 2. Create your Feature Branch (`git
-checkout -b feature/AmazingFeature`) 3. Commit your Changes (`git commit -
-m 'Add some AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
-AmazingFeature`) 5. Open a Pull Request  ## License Distributed under the MIT
-License. See `LICENSE.txt` for more information.  ## Contact Prime Patel -
-[@primepatel](https://twitter.com/primespatel) - primespatel@gmail.com Project
-Link: [https://github.com/primepatel/aksharify](https://github.com/primepatel/
-aksharify)
+from aksharify import TextArt # input image file art = TextArt("Julia.png") #
+see image art.image.show() # set dimension of output text art.set_dim(80) #
+genetate text art.asciify() # output into .txt file art.text_output("output") #
+generate colored text using html art.colorify() # output into .html file
+art.color_output("output") ``` _For examples from user community, please refer
+to the [primepatel.github.io/aksharify](https://primepatel.github.io/
+aksharify)_  ## Roadmap - [x] NumberiFy - [-] Predifined order of characters -
+[-] Getting images from URL - [-] EmojiFy See the [open issues](https://
+github.com/github_username/repo_name/issues) for a full list of proposed
+features (and known issues).  ## Contributing Contributions are what make the
+open source community such a wonderful place to learn, be inspired, and create.
+Any contributions you make are `appreciated greatly`. If you have a suggestion
+that would make this better, please fork the repo and create a pull request.
+You can also simply open an issue with the tag "enhancement". Don't forget to
+give the project a star! Thanks again! 1. Fork the Project 2. Create your
+Feature Branch (`git checkout -b feature/AmazingFeature`) 3. Commit your
+Changes (`git commit -m 'Add some AmazingFeature'`) 4. Push to the Branch (`git
+push origin feature/AmazingFeature`) 5. Open a Pull Request  ## License
+Distributed under the MIT License. See `LICENSE.txt` for more information.  ##
+Contact Prime Patel - [@primepatel](https://twitter.com/primespatel) -
+primespatel@gmail.com Project Link: [https://github.com/primepatel/aksharify]
+(https://github.com/primepatel/aksharify)
                                                                   (back_to_top)
   [contributors-shield]: https://img.shields.io/github/contributors/primepatel/
 Aksharify.svg?style=for-the-badge [contributors-url]: https://github.com/
 primepatel/Aksharify/graphs/contributors [forks-shield]: https://
 img.shields.io/github/forks/primepatel/Aksharify.svg?style=for-the-badge
 [forks-url]: https://github.com/primepatel/Aksharify/network/members [stars-
 shield]: https://img.shields.io/github/stars/primepatel/
```

### Comparing `aksharify-2.2.3/README.md` & `aksharify-2.2.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -28,16 +28,34 @@
 ```
 
 ## Usage
 
 ```python
 from aksharify import TextArt
 
+# input image file
 art = TextArt("Julia.png")
+
+# see image
 art.image.show()
+
+# set dimension of output text
+art.set_dim(80)
+
+# genetate text
+art.asciify()
+
+# output into .txt file
+art.text_output("output")
+
+# generate colored text using html
+art.colorify()
+
+# output into .html file
+art.color_output("output")
 ```
 
 _For examples from user community, please refer to the [primepatel.github.io/aksharify](https://primepatel.github.io/aksharify)_
 
 
 <!-- ROADMAP -->
 ## Roadmap
```

#### html2text {}

```diff
@@ -7,33 +7,36 @@
 It motivated me to explore the possibilities of such a prime number. I created
 a Python module that uses a predetermined character set to turn photos into
 ASCII art. It manipulates images using the PIL package, transforming them to
 grayscale before mapping pixel values to ASCII letters. Users can change the
 character set to get different effects.  ## Getting Started Before we begin,
 make sure you have one of recent versions of Python installed on your computer.
 ### Installation ```sh python -m pip install aksharify ``` ## Usage ```python
-from aksharify import TextArt art = TextArt("Julia.png") art.image.show() ```
-_For examples from user community, please refer to the [primepatel.github.io/
-aksharify](https://primepatel.github.io/aksharify)_  ## Roadmap - [x] NumberiFy
-- [-] Predifined order of characters - [-] Getting images from URL - [-
-] EmojiFy See the [open issues](https://github.com/github_username/repo_name/
-issues) for a full list of proposed features (and known issues).  ##
-Contributing Contributions are what make the open source community such a
-wonderful place to learn, be inspired, and create. Any contributions you make
-are `appreciated greatly`. If you have a suggestion that would make this
-better, please fork the repo and create a pull request. You can also simply
-open an issue with the tag "enhancement". Don't forget to give the project a
-star! Thanks again! 1. Fork the Project 2. Create your Feature Branch (`git
-checkout -b feature/AmazingFeature`) 3. Commit your Changes (`git commit -
-m 'Add some AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
-AmazingFeature`) 5. Open a Pull Request  ## License Distributed under the MIT
-License. See `LICENSE.txt` for more information.  ## Contact Prime Patel -
-[@primepatel](https://twitter.com/primespatel) - primespatel@gmail.com Project
-Link: [https://github.com/primepatel/aksharify](https://github.com/primepatel/
-aksharify)
+from aksharify import TextArt # input image file art = TextArt("Julia.png") #
+see image art.image.show() # set dimension of output text art.set_dim(80) #
+genetate text art.asciify() # output into .txt file art.text_output("output") #
+generate colored text using html art.colorify() # output into .html file
+art.color_output("output") ``` _For examples from user community, please refer
+to the [primepatel.github.io/aksharify](https://primepatel.github.io/
+aksharify)_  ## Roadmap - [x] NumberiFy - [-] Predifined order of characters -
+[-] Getting images from URL - [-] EmojiFy See the [open issues](https://
+github.com/github_username/repo_name/issues) for a full list of proposed
+features (and known issues).  ## Contributing Contributions are what make the
+open source community such a wonderful place to learn, be inspired, and create.
+Any contributions you make are `appreciated greatly`. If you have a suggestion
+that would make this better, please fork the repo and create a pull request.
+You can also simply open an issue with the tag "enhancement". Don't forget to
+give the project a star! Thanks again! 1. Fork the Project 2. Create your
+Feature Branch (`git checkout -b feature/AmazingFeature`) 3. Commit your
+Changes (`git commit -m 'Add some AmazingFeature'`) 4. Push to the Branch (`git
+push origin feature/AmazingFeature`) 5. Open a Pull Request  ## License
+Distributed under the MIT License. See `LICENSE.txt` for more information.  ##
+Contact Prime Patel - [@primepatel](https://twitter.com/primespatel) -
+primespatel@gmail.com Project Link: [https://github.com/primepatel/aksharify]
+(https://github.com/primepatel/aksharify)
                                                                   (back_to_top)
   [contributors-shield]: https://img.shields.io/github/contributors/primepatel/
 Aksharify.svg?style=for-the-badge [contributors-url]: https://github.com/
 primepatel/Aksharify/graphs/contributors [forks-shield]: https://
 img.shields.io/github/forks/primepatel/Aksharify.svg?style=for-the-badge
 [forks-url]: https://github.com/primepatel/Aksharify/network/members [stars-
 shield]: https://img.shields.io/github/stars/primepatel/
```

### Comparing `aksharify-2.2.3/pyproject.toml` & `aksharify-2.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aksharify"
-version = "2.2.3"
+version = "2.2.5"
 authors = [
     {name="Prime Patel", email = "primespatel@gmail.com"}
 ]
 description = "Ascii art module"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `aksharify-2.2.3/src/aksharify.egg-info/PKG-INFO` & `aksharify-2.2.5/src/aksharify.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aksharify
-Version: 2.2.3
+Version: 2.2.5
 Summary: Ascii art module
 Author-email: Prime Patel <primespatel@gmail.com>
 Project-URL: Homepage, https://github.com/primepatel/aksharify
 Project-URL: Bug Tracker, https://github.com/primepatel/aksharify/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -42,16 +42,34 @@
 ```
 
 ## Usage
 
 ```python
 from aksharify import TextArt
 
+# input image file
 art = TextArt("Julia.png")
+
+# see image
 art.image.show()
+
+# set dimension of output text
+art.set_dim(80)
+
+# genetate text
+art.asciify()
+
+# output into .txt file
+art.text_output("output")
+
+# generate colored text using html
+art.colorify()
+
+# output into .html file
+art.color_output("output")
 ```
 
 _For examples from user community, please refer to the [primepatel.github.io/aksharify](https://primepatel.github.io/aksharify)_
 
 
 <!-- ROADMAP -->
 ## Roadmap
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aksharify Version: 2.2.3 Summary: Ascii art module
+Metadata-Version: 2.1 Name: aksharify Version: 2.2.5 Summary: Ascii art module
 Author-email: Prime Patel
 gmail.com> Project-URL: Homepage, https://github.com/primepatel/aksharify
 Project-URL: Bug Tracker, https://github.com/primepatel/aksharify/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE.md  # __Aksharify__ [![Contributors][contributors-shield]]
@@ -14,33 +14,36 @@
 It motivated me to explore the possibilities of such a prime number. I created
 a Python module that uses a predetermined character set to turn photos into
 ASCII art. It manipulates images using the PIL package, transforming them to
 grayscale before mapping pixel values to ASCII letters. Users can change the
 character set to get different effects.  ## Getting Started Before we begin,
 make sure you have one of recent versions of Python installed on your computer.
 ### Installation ```sh python -m pip install aksharify ``` ## Usage ```python
-from aksharify import TextArt art = TextArt("Julia.png") art.image.show() ```
-_For examples from user community, please refer to the [primepatel.github.io/
-aksharify](https://primepatel.github.io/aksharify)_  ## Roadmap - [x] NumberiFy
-- [-] Predifined order of characters - [-] Getting images from URL - [-
-] EmojiFy See the [open issues](https://github.com/github_username/repo_name/
-issues) for a full list of proposed features (and known issues).  ##
-Contributing Contributions are what make the open source community such a
-wonderful place to learn, be inspired, and create. Any contributions you make
-are `appreciated greatly`. If you have a suggestion that would make this
-better, please fork the repo and create a pull request. You can also simply
-open an issue with the tag "enhancement". Don't forget to give the project a
-star! Thanks again! 1. Fork the Project 2. Create your Feature Branch (`git
-checkout -b feature/AmazingFeature`) 3. Commit your Changes (`git commit -
-m 'Add some AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
-AmazingFeature`) 5. Open a Pull Request  ## License Distributed under the MIT
-License. See `LICENSE.txt` for more information.  ## Contact Prime Patel -
-[@primepatel](https://twitter.com/primespatel) - primespatel@gmail.com Project
-Link: [https://github.com/primepatel/aksharify](https://github.com/primepatel/
-aksharify)
+from aksharify import TextArt # input image file art = TextArt("Julia.png") #
+see image art.image.show() # set dimension of output text art.set_dim(80) #
+genetate text art.asciify() # output into .txt file art.text_output("output") #
+generate colored text using html art.colorify() # output into .html file
+art.color_output("output") ``` _For examples from user community, please refer
+to the [primepatel.github.io/aksharify](https://primepatel.github.io/
+aksharify)_  ## Roadmap - [x] NumberiFy - [-] Predifined order of characters -
+[-] Getting images from URL - [-] EmojiFy See the [open issues](https://
+github.com/github_username/repo_name/issues) for a full list of proposed
+features (and known issues).  ## Contributing Contributions are what make the
+open source community such a wonderful place to learn, be inspired, and create.
+Any contributions you make are `appreciated greatly`. If you have a suggestion
+that would make this better, please fork the repo and create a pull request.
+You can also simply open an issue with the tag "enhancement". Don't forget to
+give the project a star! Thanks again! 1. Fork the Project 2. Create your
+Feature Branch (`git checkout -b feature/AmazingFeature`) 3. Commit your
+Changes (`git commit -m 'Add some AmazingFeature'`) 4. Push to the Branch (`git
+push origin feature/AmazingFeature`) 5. Open a Pull Request  ## License
+Distributed under the MIT License. See `LICENSE.txt` for more information.  ##
+Contact Prime Patel - [@primepatel](https://twitter.com/primespatel) -
+primespatel@gmail.com Project Link: [https://github.com/primepatel/aksharify]
+(https://github.com/primepatel/aksharify)
                                                                   (back_to_top)
   [contributors-shield]: https://img.shields.io/github/contributors/primepatel/
 Aksharify.svg?style=for-the-badge [contributors-url]: https://github.com/
 primepatel/Aksharify/graphs/contributors [forks-shield]: https://
 img.shields.io/github/forks/primepatel/Aksharify.svg?style=for-the-badge
 [forks-url]: https://github.com/primepatel/Aksharify/network/members [stars-
 shield]: https://img.shields.io/github/stars/primepatel/
```

### Comparing `aksharify-2.2.3/src/aksharify.py` & `aksharify-2.2.5/src/aksharify.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     def replace(self, text, position):
         self.ascii_text = self.ascii_text[:position]+ text + self.ascii_text[position+len(text):]
     
     def colorify(self):
         color = self.image.getdata()
         if self.ascii_text[:2]=="0b":
             self.ascii_text = self.ascii_text[2:]
-        file = '<p>'
+        file = '<p style="font-family: monospace;">'
         for line_no in range(self.h):
             for pixel in range(line_no*self.w, line_no*self.w + self.w):
                 file += self.span(self.ascii_text[pixel], color[pixel])
             file += '<br>'
         file += "</p>"
         self.ascii_html = file
```

