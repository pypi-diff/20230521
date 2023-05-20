# Comparing `tmp/obsidian_pdf_gen-1.6.2.tar.gz` & `tmp/obsidian_pdf_gen-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\obsidian_pdf_gen-1.6.2.tar", last modified: Thu Apr 20 05:54:30 2023, max compression
+gzip compressed data, was "dist\obsidian_pdf_gen-1.7.1.tar", last modified: Sat May 20 23:28:21 2023, max compression
```

## Comparing `obsidian_pdf_gen-1.6.2.tar` & `obsidian_pdf_gen-1.7.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 05:54:30.000000 obsidian_pdf_gen-1.6.2/
--rw-rw-rw-   0        0        0       33 2023-03-29 03:45:25.000000 obsidian_pdf_gen-1.6.2/MANIFEST.in
--rw-rw-rw-   0        0        0      310 2023-04-20 05:54:30.000000 obsidian_pdf_gen-1.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     2930 2023-04-20 04:42:09.000000 obsidian_pdf_gen-1.6.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 05:54:30.000000 obsidian_pdf_gen-1.6.2/obsidian_pdf_gen/
-drwxrwxrwx   0        0        0        0 2023-04-20 05:54:30.000000 obsidian_pdf_gen-1.6.2/obsidian_pdf_gen/config/
--rw-rw-rw-   0        0        0        0 2023-03-29 03:45:25.000000 obsidian_pdf_gen-1.6.2/obsidian_pdf_gen/config/__init__.py
--rw-rw-rw-   0        0        0     1219 2023-03-29 03:45:25.000000 obsidian_pdf_gen-1.6.2/obsidian_pdf_gen/config/note_configs.yaml
-drwxrwxrwx   0        0        0        0 2023-04-20 05:54:30.000000 obsidian_pdf_gen-1.6.2/obsidian_pdf_gen/generate_pdf/
--rw-rw-rw-   0        0        0        0 2023-03-29 03:45:25.000000 obsidian_pdf_gen-1.6.2/obsidian_pdf_gen/generate_pdf/__init__.py
--rw-rw-rw-   0        0        0    46236 2023-04-20 04:35:29.000000 obsidian_pdf_gen-1.6.2/obsidian_pdf_gen/generate_pdf/md_notes_pdf.py
-drwxrwxrwx   0        0        0        0 2023-04-20 05:54:30.000000 obsidian_pdf_gen-1.6.2/obsidian_pdf_gen/media_retriever/
--rw-rw-rw-   0        0        0        0 2023-03-29 03:45:25.000000 obsidian_pdf_gen-1.6.2/obsidian_pdf_gen/media_retriever/__init__.py
--rw-rw-rw-   0        0        0     1515 2023-04-20 04:34:58.000000 obsidian_pdf_gen-1.6.2/obsidian_pdf_gen/media_retriever/tools.py
-drwxrwxrwx   0        0        0        0 2023-04-20 05:54:30.000000 obsidian_pdf_gen-1.6.2/obsidian_pdf_gen.egg-info/
--rw-rw-rw-   0        0        0      310 2023-04-20 05:54:29.000000 obsidian_pdf_gen-1.6.2/obsidian_pdf_gen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      560 2023-04-20 05:54:30.000000 obsidian_pdf_gen-1.6.2/obsidian_pdf_gen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 05:54:29.000000 obsidian_pdf_gen-1.6.2/obsidian_pdf_gen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-04-20 05:54:29.000000 obsidian_pdf_gen-1.6.2/obsidian_pdf_gen.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-04-20 05:54:29.000000 obsidian_pdf_gen-1.6.2/obsidian_pdf_gen.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-20 05:54:29.000000 obsidian_pdf_gen-1.6.2/obsidian_pdf_gen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-20 05:54:29.000000 obsidian_pdf_gen-1.6.2/obsidian_pdf_gen.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-04-20 05:54:30.000000 obsidian_pdf_gen-1.6.2/setup.cfg
--rw-rw-rw-   0        0        0      693 2023-04-20 05:48:20.000000 obsidian_pdf_gen-1.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 23:28:21.000000 obsidian_pdf_gen-1.7.1/
+-rw-rw-rw-   0        0        0       33 2023-03-29 03:45:25.000000 obsidian_pdf_gen-1.7.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      310 2023-05-20 23:28:21.000000 obsidian_pdf_gen-1.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2918 2023-05-20 23:28:17.000000 obsidian_pdf_gen-1.7.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 23:28:21.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen/
+drwxrwxrwx   0        0        0        0 2023-05-20 23:28:21.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen/config/
+-rw-rw-rw-   0        0        0        0 2023-03-29 03:45:25.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen/config/__init__.py
+-rw-rw-rw-   0        0        0     1370 2023-05-20 23:28:17.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen/config/note_configs.yaml
+drwxrwxrwx   0        0        0        0 2023-05-20 23:28:21.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen/generate_pdf/
+-rw-rw-rw-   0        0        0        0 2023-03-29 03:45:25.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen/generate_pdf/__init__.py
+-rw-rw-rw-   0        0        0    50976 2023-05-20 23:28:17.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen/generate_pdf/md_notes_pdf.py
+drwxrwxrwx   0        0        0        0 2023-05-20 23:28:21.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen/media_retriever/
+-rw-rw-rw-   0        0        0        0 2023-03-29 03:45:25.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen/media_retriever/__init__.py
+-rw-rw-rw-   0        0        0     1515 2023-04-20 04:34:58.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen/media_retriever/tools.py
+drwxrwxrwx   0        0        0        0 2023-05-20 23:28:21.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-05-20 23:28:21.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      560 2023-05-20 23:28:21.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 23:28:21.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-05-20 23:28:21.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-05-20 23:28:21.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-20 23:28:21.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-13 05:45:58.000000 obsidian_pdf_gen-1.7.1/obsidian_pdf_gen.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-05-20 23:28:21.000000 obsidian_pdf_gen-1.7.1/setup.cfg
+-rw-rw-rw-   0        0        0      693 2023-05-20 23:28:17.000000 obsidian_pdf_gen-1.7.1/setup.py
```

### Comparing `obsidian_pdf_gen-1.6.2/README.md` & `obsidian_pdf_gen-1.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![ObsidianPDFGenCI](https://github.com/mhbl3/obsidian_pdf_gen/actions/workflows/python-app.yml/badge.svg?branch=main)](https://github.com/mhbl3/obsidian_pdf_gen/actions/workflows/python-app.yml)
+[![ObsidianPDFGenCI](https://github.com/mhbl3/obsidian-pdf-gen/actions/workflows/python-app.yml/badge.svg)](https://github.com/mhbl3/obsidian-pdf-gen/actions/workflows/python-app.yml)
 # obsidian_pdf_gen
  Python PDF generator of Obsidian notes
 # Basic setup and pdf generation Pc/Mac/Linux
 ## Installation
 ### GitHub
 ```shell
 git clone https://github.com/mhbl3/obsidian_pdf_gen.git
@@ -41,8 +41,8 @@
 # Basic Setup and pdf generation for iOS
 Make sure to have the [a-shell](https://apps.apple.com/us/app/a-shell/id1473805438) app downloaded from the Appstore, it's **free**!
 ## Install the python package in a-shell
 Using this [shortcut](https://www.icloud.com/shortcuts/6bca6376fa49422885d8972bb9ea4a46), you can install the package. There will be two options either installing through PIP or installing by downloading the release of this repo, and then PIP installing in the app
 ## Setting your default vault and select it.
 On iOS you need to setup your default vault. You can use this [shortcut](https://www.icloud.com/shortcuts/4b22c1fc8afd47ccb1d088a3f951f9b9) to `pickFolder` a folder outside of the a-shell folder. Use this to navigate to your vault
 ## Generating a pdf
-When in Obsidian use the share sheet to generate a pdf of the note that you're on by selecting **Generate Obsidian Note PDF**. This should be an option in your share sheet after downloading this [shortcuts](https://www.icloud.com/shortcuts/e2106e7b1ce54f11a9511f8d33994131)
+When in Obsidian use the share sheet to generate a pdf of the note that you're on by selecting **Generate Obsidian Note PDF**. This should be an option in your share sheet after downloading this [shortcuts](https://www.icloud.com/shortcuts/a28954ec37c34e778f6047912761983f)
```

### Comparing `obsidian_pdf_gen-1.6.2/obsidian_pdf_gen/config/note_configs.yaml` & `obsidian_pdf_gen-1.7.1/obsidian_pdf_gen/config/note_configs.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -18,14 +18,20 @@
   # More fonts available: https://www.scijournal.org/articles/latex-font
 
   # Possible sizes: 8pt, 9pt, 10pt (default), 11pt, 12pt, 14pt, 17pt, 20pt.
   # As explained https://texblog.org/2012/08/29/changing-the-font-size-in-latex/
   # NOTE: Only font sizes of 10pt, 11pt, and 12 pt are compatible with colored headers.
   size: 10 # intgeter, no need to add "pt"
 
+code:
+  frame rule: 0.4pt
+  # If true a label will be added to the code block (the language of the code)
+  label: True
+  font family: monospace
+
 # Available latex colors: https://www.overleaf.com/learn/latex/Using_colours_in_LaTeX
 Header Colors:
   \#: red
   \##: orange
   \###: yellow
   \####: Green
   \#####: blue
```

### Comparing `obsidian_pdf_gen-1.6.2/obsidian_pdf_gen/generate_pdf/md_notes_pdf.py` & `obsidian_pdf_gen-1.7.1/obsidian_pdf_gen/generate_pdf/md_notes_pdf.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,26 +23,33 @@
 with path_to_config.open("r") as f:
     CONFIG = yaml.safe_load(f)
 
 
 class ObsiPdfGenerator:
     """Generator of pdfs from Obsidian notes."""
 
-    def __init__(self, colorfull_headers: bool = False, include_toc: bool = False):
+    def __init__(
+        self,
+        colorfull_headers: bool = False,
+        include_toc: bool = False,
+        img_width: float = 1.5,
+    ):
         """Initialization of the class responsible for creating the latex doc that will be used to create the pdf.
 
         Args:
             colorfull_headers (bool, optional): Whether or not to have colorful headers in the pdf. Defaults to False.
             include_toc (bool, optional): If `True` the Table of Content will be included in the pdf. Defaults to False.
+            img_width (float, optional): Image width in inches. Defaults to 1.5.
         """
         font_style = CONFIG["font"].get("style", None)
         font_size = CONFIG["font"]["size"]
         inline_code_lang = CONFIG["inline code"]["default language"]
         hl_color = CONFIG.get("highlight color", "yellow")
         document_class = CONFIG["document class"].get("name")
+        self.img_width = img_width
         force_document_class = CONFIG["document class"].get("force document class")
         toc_latex = "\\tableofcontents\n" if include_toc else ""
 
         if not force_document_class:
             if font_size in [10, 11, 12]:
                 document_class = "article"
             else:
@@ -89,14 +96,19 @@
     boxrule=0pt,
     boxsep=0pt,
     breakable,
     enhanced jigsaw,
     borderline west={{4pt}}{{0pt}}{{gray}},
 }}
 
+\\newtcbox{{\pill}}[1][blue]{{on line,
+arc=7pt,colback=#1!10!white,colframe=#1!50!black,
+before upper={{\\rule[-3pt]{{0pt}}{{10pt}}}},boxrule=1pt,
+boxsep=0pt,left=6pt,right=6pt,top=2pt,bottom=2pt}}
+
 \\usepackage{{amsmath}}
 \\usepackage[dvipsnames]{{xcolor}} % to access the named colour LightGray
 \\usepackage{{soul}}
 \\usepackage{{sectsty}}
 \\definecolor{{LightGray}}{{rgb}}{{0.9, 0.9, 0.9}}
 \\definecolor{{inlinecodecolor}}{{rgb}}{{0, 0.3, 0.6}}
 \\usepackage{{lmodern}}
@@ -204,15 +216,17 @@
                     else:
                         raise FileNotFoundError(
                             f"File '{note_path}' not found in current directory and subdirectories"
                         )
 
                 if use_chapters:
                     # Add the note file name as the chapter name
-                    latex_chapter = "\\chapter{" + note_title + "}\n"
+                    latex_chapter = (
+                        "\\chapter{" + note_title + "}\\label{ch:" + note_title + "}\n"
+                    )
                     tex.append(latex_chapter)
                 # Loop through every line
                 lines_to_skip = []
                 for ln, line in enumerate(lines):
                     if ln in lines_to_skip:
                         continue
                     # Apply different changes to line
@@ -226,15 +240,17 @@
                     lines_to_skip += additional_lines_to_skip
                     logger.debug(f"lines_to_skip : {lines_to_skip}")
                     tex.append(line)
                     if include_linked_notes:
                         if len(additional_notes) > 0:
                             for graphic in additional_notes:
                                 if ".png" in graphic:
-                                    line = self._include_graphic(graphic)
+                                    line = self._include_graphic(
+                                        graphic, self.img_width
+                                    )
                                     # pop the last line to remve "[[my image.png]]" being present in doc
                                     tex.pop(-1)
                                     tex.append(line)
                         # Add new notes to go through
                         additional_md_notes = [
                             a_note for a_note in additional_notes if ".md" in a_note
                         ]
@@ -306,14 +322,19 @@
                 line = line.replace(
                     f"`{word}`",
                     "\\inlinecode[bgcolor=LightGray, fontsize=\\scriptsize]{"
                     + word
                     + "}",
                 )
 
+        # Find and replace tags
+        for word in line.split():
+            if word.startswith("#") and len(word) > 1 and word.count("#") == 1:
+                line = line.replace(word, f"\\pill{{{word}}}")
+
         # Reverse these fixes if they are in a math block
         if ((line.count("$") % 1 == 0) and (line.count("$") > 1)) or (
             (line.count("$$") % 1 == 0) and ((line.count("$$") > 1))
         ):
             contents_of_math = re.findall(r"\$\$(.*?)\$\$", line) + re.findall(
                 r"\$(.*?)\$", line
             )
@@ -402,14 +423,28 @@
             for ln, next_line in enumerate(note_content[current_line_idx + 1 :], 1):
                 lines_to_skip.append(ln)
                 if next_line.lstrip().startswith("---"):
                     break
             line = ""
             return line, lines_to_skip, []
         additional_notes = self.check_for_linked_notes(line)
+        if len(additional_notes) > 0:
+            links = re.findall(r"\[\[(.*?)\]\]", line)
+            for link in links:
+                logger.debug(f"link: {link}")
+                # In case there are multiple separators, but this does happen really when linking notes.
+                # It does happen for pictures, to the best of my knownledge.
+                alias_idx = -1 if link.count("|") <= 1 else 1
+                split_link_file = self.extract_note_title(link.split("|")[0])
+                split_link_alias = link.split("|")[alias_idx].lstrip()
+                split_link = f"\\hyperref[ch:{split_link_file}]{{{split_link_alias}}}"
+                line = line.replace(f"[[{link}]]", split_link)
+                logger.debug(f"line: {line}")
+                note_content[current_line_idx] = line
+
         logger.debug(f"is_table: {is_table}")
         if is_table:
             return line, lines_to_skip, additional_notes
         line, lines_to_skip = self.convert_callouts_block_text(
             current_line_idx, note_content
         )
         if len(lines_to_skip) > 0:
@@ -498,31 +533,37 @@
             Tuple[str, list, list]: Return the transformed line, a list of lines to skip and a list of additional notes.
         """
         line = self.replace_text_style(line)
         line, is_section = self.replace_md_headers(line)
         line, lines_to_skip, is_math = self.keep_math(
             line, current_line_idx, note_content
         )
+        line, additional_lines_to_skip = self.find_replace_footnotes(
+            line, note_content, current_line_idx
+        )
+        lines_to_skip += additional_lines_to_skip
         logger.debug(f"is_math: {is_math}")
         if is_math:
             return line, lines_to_skip, additional_notes
 
         line = self.handle_special_characters(line)
         logger.debug(f"is_section: {is_section}")
         if is_section:
             return line, lines_to_skip, additional_notes
-        line, lines_to_skip, is_codeblock = self.replace_md_code_block(
+        line, additional_lines_to_skip, is_codeblock = self.replace_md_code_block(
             line, current_line_idx, note_content
         )
+        lines_to_skip += additional_lines_to_skip
         logger.debug(f"is_codeblock: {is_codeblock}")
         if is_codeblock:
             return line, lines_to_skip, additional_notes
-        line, lines_to_skip, is_bullet_point = self.replace_md_bullet_point(
+        line, additional_lines_to_skip, is_bullet_point = self.replace_md_bullet_point(
             line, current_line_idx, note_content, CONFIG["indent"]
         )
+        lines_to_skip += additional_lines_to_skip
         if is_bullet_point:
             return line, lines_to_skip, additional_notes
 
         # Remove leading spaces
         line = line.lstrip()
         return line, lines_to_skip, additional_notes
 
@@ -814,33 +855,47 @@
         Args:
             line (str): The current line.
             language (str): The language of the code block.
 
         Returns:
             str: Return the transformed line.
         """
+        python3 = "true" if language.lower() == "python" else "false"
         if (language != "") and (language.lower() != "plaintext"):
+            label = CONFIG["code"]["label"]
+            if label:
+                label = language
+            else:
+                label = "none"
             line = f"""
 \\begin{{minted}}[
 frame=lines,
 framesep=2mm,
+label={label},
+framerule={CONFIG["code"]["frame rule"]},
+python3={python3},
 baselinestretch=1.2,
+breaklines=true,
 bgcolor=LightGray,
 fontsize=\\footnotesize,
+fontfamily={CONFIG["code"]["font family"]},
 linenos
 ]{{{language}}}
 {line}
 \\end{{minted}}
             """
         else:
             line = f"""
 \\begin{{minted}}[
 frame=lines,
 framesep=2mm,
 baselinestretch=1.2,
+framerule={CONFIG["code"]["frame rule"]},
+fontfamily={CONFIG["code"]["font family"]},
+breaklines=true,
 bgcolor=LightGray,
 fontsize=\\footnotesize,
 linenos
 ]{{text}}
 {line}
 \\end{{minted}}
             """
@@ -869,14 +924,55 @@
         self.document = self.document.format(self.note_tex)
         logger.debug(self.document)
         # Save file
         with open(path, "w", encoding="utf-8") as f:
             f.write(self.document)
 
     @staticmethod
+    def find_replace_footnotes(
+        line: str, lines: list, current_line_idx: int
+    ) -> Tuple[str, list]:
+        """Find all footnotes in the text and return the text without the footnotes and the list of footnotes.
+
+        Args:
+            line (str): Line to search for footnotes.
+            lines (list): List containing line to search for footnotes
+            current_line_idx (int): Index of the current line in the list of lines.
+
+        Returns:
+            Tuple[str, list]: Text with replaced footnotes, and list of lines to skip.
+        """
+        footnotes = re.findall(r"\[\^(\d+)\]", line)
+        lines_to_skip = []
+        for footnote in footnotes:
+            foot_note_in_line = f"[^{footnote}]"
+            logger.debug(f"foot_note_in_line: {foot_note_in_line}")
+            # Search through the lines after the current line for the footnote definition
+            # Manage when the next line is the last line
+            length_lines = (
+                len(lines) if current_line_idx + 1 < len(lines) else len(lines) + 1
+            )
+            for line_idx in range(current_line_idx + 1, length_lines):
+                if (length_lines > len(lines)) and (line_idx >= len(lines)):
+                    continue
+                check_text = f"{foot_note_in_line}:"
+                if check_text in lines[line_idx]:
+                    # Extract the footnote definition
+                    footnote_definition = (
+                        lines[line_idx].lstrip(f"{check_text}").lstrip()
+                    )
+                    lines_to_skip.append(line_idx)
+                    line = line.replace(
+                        foot_note_in_line,
+                        f"\\footnote[{footnote}]{{{footnote_definition}}}",
+                    )
+                    break
+        return line, lines_to_skip
+
+    @staticmethod
     def generate_pdf(
         path: str = "./notes.tex",
         clear: bool = False,
         toc: bool = False,
         quiet: bool = True,
         use_same_directory: bool = True,
     ):
@@ -984,28 +1080,31 @@
                 logger.debug(f"actual_path: {actual_path}")
                 if actual_path is not None:
                     saved_paths.append(actual_path)
                     return saved_paths
         return saved_paths
 
     @staticmethod
-    def _include_graphic(file_path: str) -> str:
+    def _include_graphic(file_path: str, img_width: float) -> str:
         """Includes a graphic into latex document.
 
         Args:
             file_path (str): String corresponding to the path of the file.
+            img_width (float, optional): Image width in inches.
 
         Returns:
             str: Returned string with latex code.
         """
         # Convert backward slashes to forward ones
         file_path = str(pathlib.Path(file_path).as_posix())
         file_path = f'"{file_path}"'
         line = (
-            "\\begin{figure}[H]\\centering\n\t\\includegraphics[width=1\\linewidth]{"
+            "\\begin{figure}[H]\\centering\n\t\\includegraphics"
+            + f"[width={img_width}"
+            + "\\linewidth]{"
             + file_path
             + "}\n"
         )
         line += "\\end{figure}"
 
         return line
 
@@ -1079,14 +1178,21 @@
     )
     parser.add_argument(
         "--reset-vault",
         default=False,
         action="store_true",
         help="Reset the default vault of the config file",
     )
+    # Get the default image width
+    parser.add_argument(
+        "--img-width",
+        default=1,
+        type=float,
+        help="Default width for images embedded in the pdf (in inches)",
+    )
     # For version of package
     parser.add_argument(
         "--version",
         default=False,
         action="store_true",
         help="Show installed version of the obsidian_pdf_gen package",
     )
@@ -1099,26 +1205,29 @@
     use_chapters = _return_bool_value(args.use_chapters)
     quiet = _return_bool_value(args.quiet)
     include_linked_notes = (
         _return_bool_value(args.include_linked_notes)
         if args.include_linked_notes
         else _return_bool_value(args.iln)
     )
+    img_width = args.img_width
+    if isinstance(img_width, str):
+        img_width = float(img_width)
 
     if args.version:
         print(
             f"Obsidian PDF Generator version: {pkg_resources.get_distribution('obsidian_pdf_gen').version}"
         )
 
     note_path = args.note_paths if args.note_paths else args.n
     open_pdf = _return_bool_value(args.o)
 
     # If there is a note path, then we are using the command line to generate a pdf
     if note_path:
-        tex = ObsiPdfGenerator(ch, toc)
+        tex = ObsiPdfGenerator(ch, toc, img_width)
         # If specified, change to vault directory
         change_to_vault_directory()
         tex.add_note(args.note, note_path, use_chapters, include_linked_notes)
         try:
             # fix output path if there is an issue
             output_path = args.output
             if output_path is None:
```

### Comparing `obsidian_pdf_gen-1.6.2/obsidian_pdf_gen/media_retriever/tools.py` & `obsidian_pdf_gen-1.7.1/obsidian_pdf_gen/media_retriever/tools.py`

 * *Files identical despite different names*

### Comparing `obsidian_pdf_gen-1.6.2/obsidian_pdf_gen.egg-info/SOURCES.txt` & `obsidian_pdf_gen-1.7.1/obsidian_pdf_gen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `obsidian_pdf_gen-1.6.2/setup.py` & `obsidian_pdf_gen-1.7.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="obsidian_pdf_gen",
-    version="1.6.2",
+    version="1.7.1",
     author="Marc-Henri Bleu-Laine",
     url="https://github.com/mhbl3/obsidian-pdf-gen",
     description="A python package to convert Obsidian Markdown files into stylish PDFs",
     packages=[
         "obsidian_pdf_gen",
         "obsidian_pdf_gen.generate_pdf",
         "obsidian_pdf_gen.config",
```

