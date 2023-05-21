# Comparing `tmp/obsidian_pdf_gen-1.7.1.tar.gz` & `tmp/obsidian_pdf_gen-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\obsidian_pdf_gen-1.7.1.tar", last modified: Sat May 20 23:28:21 2023, max compression
+gzip compressed data, was "dist\obsidian_pdf_gen-1.7.2.tar", last modified: Sun May 21 15:47:42 2023, max compression
```

## Comparing `obsidian_pdf_gen-1.7.1.tar` & `obsidian_pdf_gen-1.7.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 23:28:21.000000 obsidian_pdf_gen-1.7.1/
--rw-rw-rw-   0        0        0       33 2023-03-29 03:45:25.000000 obsidian_pdf_gen-1.7.1/MANIFEST.in
--rw-rw-rw-   0        0        0      310 2023-05-20 23:28:21.000000 obsidian_pdf_gen-1.7.1/PKG-INFO
--rw-rw-rw-   0        0        0     2918 2023-05-20 23:28:17.000000 obsidian_pdf_gen-1.7.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 23:28:21.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen/
-drwxrwxrwx   0        0        0        0 2023-05-20 23:28:21.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen/config/
--rw-rw-rw-   0        0        0        0 2023-03-29 03:45:25.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen/config/__init__.py
--rw-rw-rw-   0        0        0     1370 2023-05-20 23:28:17.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen/config/note_configs.yaml
-drwxrwxrwx   0        0        0        0 2023-05-20 23:28:21.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen/generate_pdf/
--rw-rw-rw-   0        0        0        0 2023-03-29 03:45:25.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen/generate_pdf/__init__.py
--rw-rw-rw-   0        0        0    50976 2023-05-20 23:28:17.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen/generate_pdf/md_notes_pdf.py
-drwxrwxrwx   0        0        0        0 2023-05-20 23:28:21.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen/media_retriever/
--rw-rw-rw-   0        0        0        0 2023-03-29 03:45:25.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen/media_retriever/__init__.py
--rw-rw-rw-   0        0        0     1515 2023-04-20 04:34:58.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen/media_retriever/tools.py
-drwxrwxrwx   0        0        0        0 2023-05-20 23:28:21.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen.egg-info/
--rw-rw-rw-   0        0        0      310 2023-05-20 23:28:21.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      560 2023-05-20 23:28:21.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 23:28:21.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-05-20 23:28:21.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-05-20 23:28:21.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-20 23:28:21.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-13 05:45:58.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-05-20 23:28:21.000000 obsidian_pdf_gen-1.7.1/setup.cfg
--rw-rw-rw-   0        0        0      693 2023-05-20 23:28:17.000000 obsidian_pdf_gen-1.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 15:47:42.000000 obsidian_pdf_gen-1.7.2/
+-rw-rw-rw-   0        0        0       33 2023-03-29 03:45:25.000000 obsidian_pdf_gen-1.7.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      310 2023-05-21 15:47:42.000000 obsidian_pdf_gen-1.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2918 2023-05-20 23:28:17.000000 obsidian_pdf_gen-1.7.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-21 15:47:42.000000 obsidian_pdf_gen-1.7.2/obsidian_pdf_gen/
+drwxrwxrwx   0        0        0        0 2023-05-21 15:47:42.000000 obsidian_pdf_gen-1.7.2/obsidian_pdf_gen/config/
+-rw-rw-rw-   0        0        0        0 2023-03-29 03:45:25.000000 obsidian_pdf_gen-1.7.2/obsidian_pdf_gen/config/__init__.py
+-rw-rw-rw-   0        0        0     1370 2023-05-20 23:28:17.000000 obsidian_pdf_gen-1.7.2/obsidian_pdf_gen/config/note_configs.yaml
+drwxrwxrwx   0        0        0        0 2023-05-21 15:47:42.000000 obsidian_pdf_gen-1.7.2/obsidian_pdf_gen/generate_pdf/
+-rw-rw-rw-   0        0        0        0 2023-03-29 03:45:25.000000 obsidian_pdf_gen-1.7.2/obsidian_pdf_gen/generate_pdf/__init__.py
+-rw-rw-rw-   0        0        0    50222 2023-05-21 15:47:31.000000 obsidian_pdf_gen-1.7.2/obsidian_pdf_gen/generate_pdf/md_notes_pdf.py
+drwxrwxrwx   0        0        0        0 2023-05-21 15:47:42.000000 obsidian_pdf_gen-1.7.2/obsidian_pdf_gen/media_retriever/
+-rw-rw-rw-   0        0        0        0 2023-03-29 03:45:25.000000 obsidian_pdf_gen-1.7.2/obsidian_pdf_gen/media_retriever/__init__.py
+-rw-rw-rw-   0        0        0     1515 2023-04-20 04:34:58.000000 obsidian_pdf_gen-1.7.2/obsidian_pdf_gen/media_retriever/tools.py
+drwxrwxrwx   0        0        0        0 2023-05-21 15:47:42.000000 obsidian_pdf_gen-1.7.2/obsidian_pdf_gen.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-05-21 15:47:42.000000 obsidian_pdf_gen-1.7.2/obsidian_pdf_gen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      560 2023-05-21 15:47:42.000000 obsidian_pdf_gen-1.7.2/obsidian_pdf_gen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 15:47:42.000000 obsidian_pdf_gen-1.7.2/obsidian_pdf_gen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-05-21 15:47:42.000000 obsidian_pdf_gen-1.7.2/obsidian_pdf_gen.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-05-21 15:47:42.000000 obsidian_pdf_gen-1.7.2/obsidian_pdf_gen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-21 15:47:42.000000 obsidian_pdf_gen-1.7.2/obsidian_pdf_gen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-13 05:45:58.000000 obsidian_pdf_gen-1.7.2/obsidian_pdf_gen.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-05-21 15:47:42.000000 obsidian_pdf_gen-1.7.2/setup.cfg
+-rw-rw-rw-   0        0        0      693 2023-05-21 15:47:31.000000 obsidian_pdf_gen-1.7.2/setup.py
```

### Comparing `obsidian_pdf_gen-1.7.1/README.md` & `obsidian_pdf_gen-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `obsidian_pdf_gen-1.7.1/obsidian_pdf_gen/config/note_configs.yaml` & `obsidian_pdf_gen-1.7.2/obsidian_pdf_gen/config/note_configs.yaml`

 * *Files identical despite different names*

### Comparing `obsidian_pdf_gen-1.7.1/obsidian_pdf_gen/generate_pdf/md_notes_pdf.py` & `obsidian_pdf_gen-1.7.2/obsidian_pdf_gen/generate_pdf/md_notes_pdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
 \\renewlist{{itemize}}{{itemize}}{{9}}
 
 \\usepackage{{graphicx}}
 
 \\usepackage{{csquotes}}
 
-\\usepackage{{hyperref}}
+\\usepackage[hidelinks]{{hyperref}}
 
 \\usepackage[T1]{{fontenc}}
 
 \\usepackage[most]{{tcolorbox}}
 \\definecolor{{block-gray}}{{gray}}{{0.95}}
 \\newtcolorbox{{advtcolorbox}}{{
     %colback=block-gray,
@@ -268,135 +268,104 @@
 \\section{{{note_title}}}
 {note}
 """
 
     @staticmethod
     def replace_text_style(line: str) -> str:
         """Replace a bunch of markdown syntax to latex.
+            Saves all the non-transformed text, applies the
+            transformations and reverts then when needed.
 
         Args:
             line (str): Current line of the note.
 
         Returns:
-            str: Trsnsformed line.
+            str: Transformed line.
         """
         # check if math equation is present
         if ((line.count("$") % 1 == 0) and (line.count("$") > 1)) or (
             (line.count("$$") % 1 == 0) and ((line.count("$$") > 1))
         ):
-            original_content = re.findall(r"\$\$(.*?)\$\$", line) + re.findall(
+            original_content_math = re.findall(r"\$\$(.*?)\$\$", line) + re.findall(
                 r"\$(.*?)\$", line
             )
-
         # Find italic words
         all_italics = re.findall(r"_(.*?)_", line)
-        for word in all_italics:
-            line = line.replace(f"_{word}_", f"\\textit{{{word}}}")
-
         # Find bold words
         all_bolds = re.findall(r"\*\*(.*?)\*\*", line)
-        for word in all_bolds:
-            line = line.replace(f"**{word}**", f"\\textbf{{{word}}}")
-
         # Find highlighted words
         all_hls = re.findall(r"==(.*?)==", line)
-        for word in all_hls:
-            line = line.replace(f"=={word}==", f"\\hl{{{word}}}")
-
-        # Replace hyperlinks
+        link_bool = False
         if (
             "[" in line
             and "]" in line
             and "(" in line
             and ")" in line
             and ("http" in line or "www" in line)
         ):
             links = re.findall(r"\]\((.*?)\)", line)
             text_for_links = re.findall(r"\[(.*?)\]\(", line)
-            for txt, link in zip(text_for_links, links):
-                line = line.replace(f"[{txt}]({link})", f"\\href{{{link}}}{{{txt}}}")
-
+            link_bool = True
         # Find all inline code
         all_inline = re.findall(r"`(.+?)`", line)
-        for word in all_inline:
+
+        # Apply latex changes to special characters
+        line = line.replace("&", "\\&")
+        line = line.replace("%", "\\%")
+        # line = line.replace("$", "\\$")
+        # line = line.replace(">", "\\>")
+        # line = line.replace("<", "\\<")
+        line = line.replace("#", "\\#")
+        line = line.replace("---", "\\noindent\\rule[0.5ex]{\\linewidth}{1pt}")
+        line = line.replace("***", "\\noindent\\rule[0.5ex]{\\linewidth}{1pt}")
+        line = line.replace("_", "\\_")
+
+        for word, word_new in zip(all_italics, re.findall(r"\\_(.*?)\\_", line)):
+            line = line.replace(f"\\_{word_new}\\_", f"\\textit{{{word}}}")
+        for word, word_new in zip(all_bolds, re.findall(r"\*\*(.*?)\*\*", line)):
+            line = line.replace(f"**{word_new}**", f"\\textbf{{{word}}}")
+        for word, word_new in zip(all_hls, re.findall(r"==(.*?)==", line)):
+            line = line.replace(f"=={word_new}==", f"\\hl{{{word}}}")
+
+        # Replace hyperlinks
+        if link_bool:
+            links_new = re.findall(r"\]\((.*?)\)", line)
+            text_for_links_new = re.findall(r"\[(.*?)\]\(", line)
+            for txt, link, txt_new, link_new in zip(
+                text_for_links, links, text_for_links_new, links_new
+            ):
+                line = line.replace(
+                    f"[{txt_new}]({link_new})", f"\\href{{{link}}}{{{txt}}}"
+                )
+
+        for word, word_new in zip(all_inline, re.findall(r"`(.+?)`", line)):
             if word != "`":
                 line = line.replace(
-                    f"`{word}`",
+                    f"`{word_new}`",
                     "\\inlinecode[bgcolor=LightGray, fontsize=\\scriptsize]{"
                     + word
                     + "}",
                 )
-
         # Find and replace tags
         for word in line.split():
-            if word.startswith("#") and len(word) > 1 and word.count("#") == 1:
+            if (
+                (word.startswith("#") or word.startswith("\\#"))
+                and len(word) > 1
+                and ((word.count("#") == 1) or (word.count("\\#") == 1))
+            ):
                 line = line.replace(word, f"\\pill{{{word}}}")
-
         # Reverse these fixes if they are in a math block
         if ((line.count("$") % 1 == 0) and (line.count("$") > 1)) or (
             (line.count("$$") % 1 == 0) and ((line.count("$$") > 1))
         ):
             contents_of_math = re.findall(r"\$\$(.*?)\$\$", line) + re.findall(
                 r"\$(.*?)\$", line
             )
             for e, content in enumerate(contents_of_math):
-                line = line.replace(content, original_content[e])
-
-        return line
-
-    @staticmethod
-    def handle_special_characters(line: str) -> str:
-        """Handle special characters, and replaces markown with latex syntax.
-
-        Args:
-            line (str): Current line of the note.
-
-        Returns:
-            str: Transformed line.
-        """
-        replace_underscore = True
-        # check if math equation is present
-        if ((line.count("$") % 1 == 0) and (line.count("$") > 1)) or (
-            (line.count("$$") % 1 == 0) and ((line.count("$$") > 1))
-        ):
-            original_content = re.findall(r"\$\$(.*?)\$\$", line) + re.findall(
-                r"\$(.*?)\$", line
-            )
-        # Check if inline code is present
-        if (line.count("`") % 1 == 0) and (line.count("`") > 1):
-            original_content_inline = re.findall(r"`(.*?)`", line)
-
-        line = line.replace("&", "\\&")
-        line = line.replace("%", "\\%")
-        # line = line.replace("$", "\\$")
-        line = line.replace(">", "\\>")
-        line = line.replace("<", "\\<")
-        line = line.replace("#", "\\#")
-        line = line.replace("---", "\\noindent\\rule[0.5ex]{\\linewidth}{1pt}")
-        line = line.replace("***", "\\noindent\\rule[0.5ex]{\\linewidth}{1pt}")
-        # Reverse these fixes if they are in a math block
-        if ((line.count("$") % 1 == 0) and (line.count("$") > 1)) or (
-            (line.count("$$") % 1 == 0) and ((line.count("$$") > 1))
-        ):
-            contents_of_math = re.findall(r"\$\$(.*?)\$\$", line) + re.findall(
-                r"\$(.*?)\$", line
-            )
-            for e, content in enumerate(contents_of_math):
-                line = line.replace(content, original_content[e])
-            replace_underscore = False
-        if (line.count("`") % 1 == 0) and (line.count("`") > 1):
-            content_of_inline = re.findall(r"`(.*?)`", line)
-            for e, content in enumerate(content_of_inline):
-                line = line.replace(content, original_content_inline[e])
-            replace_underscore = False
-        if replace_underscore:
-            line = line.replace("_", "\\_")
-        # line = line.replace("\\", "\\\\")
-        # line = line.replace("{", "\\{")
-        # line = line.replace("}", "\\}")
+                line = line.replace(content, original_content_math[e])
         return line
 
     # Find and add linked notes
 
     def _apply_transformation(
         self, line: str, current_line_idx: int, note_content: list
     ) -> Tuple[str, list, list]:
@@ -485,31 +454,30 @@
             logger.debug(
                 f"lines_to_skip in convert_callouts_block_text: {lines_to_skip}"
             )
             # Remove text in between [! and ] and replace it with a empty text
             txt_to_replace = re.findall(r"\[!(.*?)\]", line)
             if len(txt_to_replace) > 0:
                 txt_to_replace = txt_to_replace[0]
-                line = self.handle_special_characters(
-                    self.replace_text_style(
-                        line.replace(f"[!{txt_to_replace}]", "").lstrip(">").lstrip()
-                    )
+                line = self.replace_text_style(
+                    line.replace(f"[!{txt_to_replace}]", "").lstrip(">").lstrip()
                 )
+                logger.debug(f"line-convert_callouts_block_text-1-true = {line}")
                 line = "\\begin{tcolorbox}" + f"[title={line}]\n"
             else:
-                line = "\\begin{advtcolorbox}\n" + self.handle_special_characters(
+                line = "\\begin{advtcolorbox}\n" + (
                     self.replace_text_style(line.lstrip(">").lstrip() + "\n")
                 )
+                logger.debug(f"line-convert_callouts_block_text-1-false = {line}")
 
             for idx_blocks in lines_to_skip[1:]:
-                line += self.handle_special_characters(
-                    self.replace_text_style(
-                        note_content[idx_blocks].lstrip(">").lstrip() + "\n"
-                    )
+                line += self.replace_text_style(
+                    note_content[idx_blocks].lstrip(">").lstrip() + "\n"
                 )
+                logger.debug(f"line-convert_callouts_block_text-2 = {line}")
 
             if len(txt_to_replace) > 0:
                 line += "\\end{tcolorbox}\n"
             else:
                 line += "\\end{advtcolorbox}\n"
         logger.debug(f"line in convert_callouts_block_text: {line}")
         return line, lines_to_skip
@@ -528,31 +496,33 @@
             current_line_idx (int): The current line number.
             note_content (list): List of lines in the note.
             additional_notes (list): List of the name of additional notes to add.
 
         Returns:
             Tuple[str, list, list]: Return the transformed line, a list of lines to skip and a list of additional notes.
         """
-        line = self.replace_text_style(line)
+        lines_to_skip = []
         line, is_section = self.replace_md_headers(line)
+        logger.debug(f"is_section: {is_section}")
+        if is_section:
+            return line, lines_to_skip, additional_notes
+
+        line = self.replace_text_style(line)
+        logger.debug(f"line-apply_conv_rt = {line}")
         line, lines_to_skip, is_math = self.keep_math(
             line, current_line_idx, note_content
         )
         line, additional_lines_to_skip = self.find_replace_footnotes(
             line, note_content, current_line_idx
         )
         lines_to_skip += additional_lines_to_skip
         logger.debug(f"is_math: {is_math}")
         if is_math:
             return line, lines_to_skip, additional_notes
 
-        line = self.handle_special_characters(line)
-        logger.debug(f"is_section: {is_section}")
-        if is_section:
-            return line, lines_to_skip, additional_notes
         line, additional_lines_to_skip, is_codeblock = self.replace_md_code_block(
             line, current_line_idx, note_content
         )
         lines_to_skip += additional_lines_to_skip
         logger.debug(f"is_codeblock: {is_codeblock}")
         if is_codeblock:
             return line, lines_to_skip, additional_notes
@@ -749,14 +719,17 @@
         if lsline.startswith("-"):
             line = "\\begin{itemize}\n" + "\\item " + line.lstrip("- ")
             for ln, line_after_line in enumerate(
                 lines[current_line_idx + 1 :], current_line_idx + 1
             ):
                 logger.debug(f"ln = {ln}")
                 line_after_line = self.replace_text_style(line_after_line)
+                logger.debug(
+                    f"line_after_line-replace_md_bullet_point = {line_after_line}"
+                )
                 if line_after_line.lstrip().startswith("-"):
                     ls_line_after_line = line_after_line.lstrip()
                     space_diff = len(line_after_line) - len(ls_line_after_line)
                     if line_after_line.startswith("\t"):
                         space_diff = (
                             len(line_after_line) - len(line_after_line.lstrip("\t"))
                         ) * indent
```

### Comparing `obsidian_pdf_gen-1.7.1/obsidian_pdf_gen/media_retriever/tools.py` & `obsidian_pdf_gen-1.7.2/obsidian_pdf_gen/media_retriever/tools.py`

 * *Files identical despite different names*

### Comparing `obsidian_pdf_gen-1.7.1/obsidian_pdf_gen.egg-info/SOURCES.txt` & `obsidian_pdf_gen-1.7.2/obsidian_pdf_gen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `obsidian_pdf_gen-1.7.1/setup.py` & `obsidian_pdf_gen-1.7.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="obsidian_pdf_gen",
-    version="1.7.1",
+    version="1.7.2",
     author="Marc-Henri Bleu-Laine",
     url="https://github.com/mhbl3/obsidian-pdf-gen",
     description="A python package to convert Obsidian Markdown files into stylish PDFs",
     packages=[
         "obsidian_pdf_gen",
         "obsidian_pdf_gen.generate_pdf",
         "obsidian_pdf_gen.config",
```

