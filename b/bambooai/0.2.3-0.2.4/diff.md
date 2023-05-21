# Comparing `tmp/bambooai-0.2.3.tar.gz` & `tmp/bambooai-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bambooai-0.2.3.tar", last modified: Wed May 17 02:10:01 2023, max compression
+gzip compressed data, was "bambooai-0.2.4.tar", last modified: Sun May 21 06:32:36 2023, max compression
```

## Comparing `bambooai-0.2.3.tar` & `bambooai-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 02:10:01.657454 bambooai-0.2.3/
--rw-rw-rw-   0        0        0     6317 2023-05-17 02:10:01.655136 bambooai-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     5783 2023-05-14 12:03:23.000000 bambooai-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 02:10:01.610207 bambooai-0.2.3/bambooai/
--rw-rw-rw-   0        0        0       30 2023-05-07 07:18:22.000000 bambooai-0.2.3/bambooai/__init__.py
--rw-rw-rw-   0        0        0    14423 2023-05-17 01:45:15.000000 bambooai-0.2.3/bambooai/bambooai.py
-drwxrwxrwx   0        0        0        0 2023-05-17 02:10:01.653075 bambooai-0.2.3/bambooai.egg-info/
--rw-rw-rw-   0        0        0     6317 2023-05-17 02:10:01.000000 bambooai-0.2.3/bambooai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-05-17 02:10:01.000000 bambooai-0.2.3/bambooai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 02:10:01.000000 bambooai-0.2.3/bambooai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-17 02:10:01.000000 bambooai-0.2.3/bambooai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-17 02:10:01.000000 bambooai-0.2.3/bambooai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 02:10:01.657588 bambooai-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      702 2023-05-17 02:07:09.000000 bambooai-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 06:32:36.501762 bambooai-0.2.4/
+-rw-rw-rw-   0        0        0     6760 2023-05-21 06:32:36.501042 bambooai-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6230 2023-05-21 06:28:10.000000 bambooai-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-21 06:32:36.460668 bambooai-0.2.4/bambooai/
+-rw-rw-rw-   0        0        0       30 2023-05-07 07:18:22.000000 bambooai-0.2.4/bambooai/__init__.py
+-rw-rw-rw-   0        0        0    19162 2023-05-21 06:08:20.000000 bambooai-0.2.4/bambooai/bambooai.py
+drwxrwxrwx   0        0        0        0 2023-05-21 06:32:36.498334 bambooai-0.2.4/bambooai.egg-info/
+-rw-rw-rw-   0        0        0     6760 2023-05-21 06:32:36.000000 bambooai-0.2.4/bambooai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-05-21 06:32:36.000000 bambooai-0.2.4/bambooai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 06:32:36.000000 bambooai-0.2.4/bambooai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-21 06:32:36.000000 bambooai-0.2.4/bambooai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-21 06:32:36.000000 bambooai-0.2.4/bambooai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-21 06:32:36.502261 bambooai-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      702 2023-05-21 06:25:40.000000 bambooai-0.2.4/setup.py
```

### Comparing `bambooai-0.2.3/PKG-INFO` & `bambooai-0.2.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambooai
-Version: 0.2.3
+Version: 0.2.4
 Summary: A lightweight library for working with pandas dataframes using natural language queries
 Home-page: UNKNOWN
 Author: Palo Galko
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -22,32 +22,28 @@
 
 ## Preview
 
 Try it out in Google Colab:
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1grKtqKD4u8cVGMoVv__umci4F7IU14vU?usp=sharing)
 
-
 ## How it works
 
-- User starts BambooAI
-- BambooAI checks if a question is provided
-  - If a question is given programmatically, it gets processed and the assistant exits after the execution
-  - If no question is provided programaticaly, BambooAI prompts the user for one and enters a loop of questions and answers, remembering the conversation history
-    - Sends each question to the OpenAI API LLM along with the conversation history
-    - Obtains a response with corresponding Python code
-    - Executes the code to generate an answer or visualization
-      - If the code works, it displays the answer or visualization, and then prompts for another question, which could be related to the preceding question or an entirely new topic
-      - If an error occurs, the program requests a corrected code from the OpenAI API by providing the error message and then attempts to execute the corrected code. *If the "llm_switch" argument is set to "True" (LLM cascading) it will switch from base model to a more powerfull gpt-4 and retry. After successfull execution it will reset back to base model.*
-  - The loop continues until the user enters 'exit', at which point the program terminates
-  - The program displays the total token usage at each step, providing insight into the resources consumed during the process.
-  
-**Flow chart:**
-
-![](images/flow_chart.png)
+- The user begins by starting the BambooAI agent.
+- BambooAI subsequently checks if a question has been provided:
+  - If a question is available, it continues to the next step.
+  - If no question is available, BambooAI prompts the user to input one. It then enters a loop of questions and answers, remembering the conversation history and continually prompting the user for a new question. This loop continues until the user types 'exit', signalling the termination of the program.
+- Following the reception of a question, the OpenAI API is called to review and evaluate the task. The Language Learning Model (LLM) then presents four possible analysis methods, choosing the one it deems most suitable. This selected method is summarised and framed as a task for a hypothetical junior data analyst.
+- The agent then replaces the original question with the task from the previous step and sends this as a prompt to the OpenAI API for code generation.
+- The response from the API, containing the corresponding Python code, is received, checked and sanitised if necessary.
+- This code is then executed to generate an answer or a visualization:
+  - If the code executes successfully, it displays the answer or visualization and subsequently prompts for another question. This new question could be related to the previous question or could be on an entirely new topic.
+  - If an error occurs during code execution, the program requests a corrected version of the code from the OpenAI API by providing the error message, and then attempts to execute the corrected code. *In cases where the "llm_switch" argument is set to "True" (indicating LLM cascading), the program will switch from the base model to the more powerful GPT-4 model for a retry. After successful execution, it will revert to the base model.*
+- The program then displays the total token usage at each step, thereby providing insights into the resources consumed during the process.
+ 
 
 ## How to use
 
 **Installation**
 
 ```
 pip install bambooai
@@ -100,27 +96,27 @@
 ```
 
 **Environment Variables**
 
 The library requires an OpenAI API account and the API key to connect to an OpenAI LLMs. The OpenAI API key needs to be stored in a 'OPENAI_API_KEY' environment variable.
 The key can be obtained from here: https://platform.openai.com/account/api-keys
 
+
 ## Notes
 
 - The library currently supports only OpenAI Chat models. It has been tested with both gpt-3.5-turbo and gpt-4. The gpt-3.5-turbo seems to perform well and is the preferred option due to its 10x lower cost.
 - The library executes LLM generated Python code, this can be bad if the LLM generated Python code is harmful. Use cautiously.
 - Be sure to monitor your token usage, as each execution of BambooAI uses an average of 400-600 tokens. At the time of writing, the cost per 1K tokens is $0.03 USD for GPT-4 and $0.002 USD for GPT-3.5-turbo. It's important to keep these costs in mind when using the library, particularly when using the more expensive models.
 - Currently the project consists of 126 lines of code, 49 lines of comments and 20 blanks.
 
 ## Contributing
 
 Contributions are welcome; please feel free to open a pull request. Keep in mind that our goal is to maintain a concise codebase with high readability.
 
 ## ToDo
 
-- Introduce memory limits.  A method for users to control the number of conversation pairs retained in memory and sent to the LLM during each iteration.
 - Ongoing work on optimizing the prompts and sanitization of the outputs.
 - Add abbility to inspect the LLM generated code before execution.
 - Add support for aditional LLMs.
```

### Comparing `bambooai-0.2.3/README.md` & `bambooai-0.2.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -9,32 +9,28 @@
 
 ## Preview
 
 Try it out in Google Colab:
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1grKtqKD4u8cVGMoVv__umci4F7IU14vU?usp=sharing)
 
-
 ## How it works
 
-- User starts BambooAI
-- BambooAI checks if a question is provided
-  - If a question is given programmatically, it gets processed and the assistant exits after the execution
-  - If no question is provided programaticaly, BambooAI prompts the user for one and enters a loop of questions and answers, remembering the conversation history
-    - Sends each question to the OpenAI API LLM along with the conversation history
-    - Obtains a response with corresponding Python code
-    - Executes the code to generate an answer or visualization
-      - If the code works, it displays the answer or visualization, and then prompts for another question, which could be related to the preceding question or an entirely new topic
-      - If an error occurs, the program requests a corrected code from the OpenAI API by providing the error message and then attempts to execute the corrected code. *If the "llm_switch" argument is set to "True" (LLM cascading) it will switch from base model to a more powerfull gpt-4 and retry. After successfull execution it will reset back to base model.*
-  - The loop continues until the user enters 'exit', at which point the program terminates
-  - The program displays the total token usage at each step, providing insight into the resources consumed during the process.
-  
-**Flow chart:**
-
-![](images/flow_chart.png)
+- The user begins by starting the BambooAI agent.
+- BambooAI subsequently checks if a question has been provided:
+  - If a question is available, it continues to the next step.
+  - If no question is available, BambooAI prompts the user to input one. It then enters a loop of questions and answers, remembering the conversation history and continually prompting the user for a new question. This loop continues until the user types 'exit', signalling the termination of the program.
+- Following the reception of a question, the OpenAI API is called to review and evaluate the task. The Language Learning Model (LLM) then presents four possible analysis methods, choosing the one it deems most suitable. This selected method is summarised and framed as a task for a hypothetical junior data analyst.
+- The agent then replaces the original question with the task from the previous step and sends this as a prompt to the OpenAI API for code generation.
+- The response from the API, containing the corresponding Python code, is received, checked and sanitised if necessary.
+- This code is then executed to generate an answer or a visualization:
+  - If the code executes successfully, it displays the answer or visualization and subsequently prompts for another question. This new question could be related to the previous question or could be on an entirely new topic.
+  - If an error occurs during code execution, the program requests a corrected version of the code from the OpenAI API by providing the error message, and then attempts to execute the corrected code. *In cases where the "llm_switch" argument is set to "True" (indicating LLM cascading), the program will switch from the base model to the more powerful GPT-4 model for a retry. After successful execution, it will revert to the base model.*
+- The program then displays the total token usage at each step, thereby providing insights into the resources consumed during the process.
+ 
 
 ## How to use
 
 **Installation**
 
 ```
 pip install bambooai
@@ -87,25 +83,25 @@
 ```
 
 **Environment Variables**
 
 The library requires an OpenAI API account and the API key to connect to an OpenAI LLMs. The OpenAI API key needs to be stored in a 'OPENAI_API_KEY' environment variable.
 The key can be obtained from here: https://platform.openai.com/account/api-keys
 
+
 ## Notes
 
 - The library currently supports only OpenAI Chat models. It has been tested with both gpt-3.5-turbo and gpt-4. The gpt-3.5-turbo seems to perform well and is the preferred option due to its 10x lower cost.
 - The library executes LLM generated Python code, this can be bad if the LLM generated Python code is harmful. Use cautiously.
 - Be sure to monitor your token usage, as each execution of BambooAI uses an average of 400-600 tokens. At the time of writing, the cost per 1K tokens is $0.03 USD for GPT-4 and $0.002 USD for GPT-3.5-turbo. It's important to keep these costs in mind when using the library, particularly when using the more expensive models.
 - Currently the project consists of 126 lines of code, 49 lines of comments and 20 blanks.
 
 ## Contributing
 
 Contributions are welcome; please feel free to open a pull request. Keep in mind that our goal is to maintain a concise codebase with high readability.
 
 ## ToDo
 
-- Introduce memory limits.  A method for users to control the number of conversation pairs retained in memory and sent to the LLM during each iteration.
 - Ongoing work on optimizing the prompts and sanitization of the outputs.
 - Add abbility to inspect the LLM generated code before execution.
 - Add support for aditional LLMs.
```

### Comparing `bambooai-0.2.3/bambooai/bambooai.py` & `bambooai-0.2.4/bambooai/bambooai.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,894 +9,1190 @@
 00000080: 0d0a 696d 706f 7274 2070 616e 6461 7320  ..import pandas 
 00000090: 6173 2070 640d 0a66 726f 6d20 7465 726d  as pd..from term
 000000a0: 636f 6c6f 7220 696d 706f 7274 2063 6f6c  color import col
 000000b0: 6f72 6564 2c20 6370 7269 6e74 0d0a 6672  ored, cprint..fr
 000000c0: 6f6d 2049 5079 7468 6f6e 2e64 6973 706c  om IPython.displ
 000000d0: 6179 2069 6d70 6f72 7420 6469 7370 6c61  ay import displa
 000000e0: 792c 2049 6d61 6765 2c20 4854 4d4c 0d0a  y, Image, HTML..
-000000f0: 0d0a 636c 6173 7320 4261 6d62 6f6f 4149  ..class BambooAI
-00000100: 3a0d 0a20 2020 2064 6566 205f 5f69 6e69  :..    def __ini
-00000110: 745f 5f28 7365 6c66 2c20 6466 3a20 7064  t__(self, df: pd
-00000120: 2e44 6174 6146 7261 6d65 2c6d 6178 5f63  .DataFrame,max_c
-00000130: 6f6e 7665 7273 6174 696f 6e73 3a20 696e  onversations: in
-00000140: 7420 3d20 3320 2c6c 6c6d 3a20 7374 7220  t = 3 ,llm: str 
-00000150: 3d20 2767 7074 2d33 2e35 2d74 7572 626f  = 'gpt-3.5-turbo
-00000160: 272c 6c6c 6d5f 7377 6974 6368 3a20 626f  ',llm_switch: bo
-00000170: 6f6c 203d 2046 616c 7365 293a 0d0a 0d0a  ol = False):....
-00000180: 2020 2020 2020 2020 7365 6c66 2e41 5049          self.API
-00000190: 5f4b 4559 203d 206f 732e 656e 7669 726f  _KEY = os.enviro
-000001a0: 6e2e 6765 7428 274f 5045 4e41 495f 4150  n.get('OPENAI_AP
-000001b0: 495f 4b45 5927 290d 0a20 2020 2020 2020  I_KEY')..       
-000001c0: 2073 656c 662e 4d41 585f 4552 524f 525f   self.MAX_ERROR_
-000001d0: 434f 5252 4543 5449 4f4e 5320 3d20 350d  CORRECTIONS = 5.
-000001e0: 0a20 2020 2020 2020 2023 2053 6574 2074  .        # Set t
-000001f0: 6865 206d 6178 696d 756d 206e 756d 6265  he maximum numbe
-00000200: 7220 6f66 2071 7565 7374 696f 6e2f 616e  r of question/an
-00000210: 7377 6572 2070 6169 7273 2074 6f20 6265  swer pairs to be
-00000220: 206b 6570 7420 696e 2074 6865 2063 6f6e   kept in the con
-00000230: 7665 7273 6174 696f 6e20 6d65 6d6d 6f72  versation memmor
-00000240: 790d 0a20 2020 2020 2020 2073 656c 662e  y..        self.
-00000250: 4d41 585f 434f 4e56 4552 5341 5449 4f4e  MAX_CONVERSATION
-00000260: 5320 3d20 286d 6178 5f63 6f6e 7665 7273  S = (max_convers
-00000270: 6174 696f 6e73 2a32 2920 2d20 310d 0a0d  ations*2) - 1...
-00000280: 0a20 2020 2020 2020 2073 656c 662e 6f72  .        self.or
-00000290: 6967 696e 616c 5f64 6620 3d20 6466 0d0a  iginal_df = df..
-000002a0: 2020 2020 2020 2020 7365 6c66 2e64 6620          self.df 
-000002b0: 3d20 6466 2e63 6f70 7928 2920 2023 206d  = df.copy()  # m
-000002c0: 616b 6520 6120 636f 7079 206f 6620 7468  ake a copy of th
-000002d0: 6520 6461 7461 6672 616d 650d 0a20 2020  e dataframe..   
-000002e0: 2020 2020 2073 656c 662e 6466 5f68 6561       self.df_hea
-000002f0: 6420 3d20 7365 6c66 2e6f 7269 6769 6e61  d = self.origina
-00000300: 6c5f 6466 2e68 6561 6428 3129 0d0a 2020  l_df.head(1)..  
-00000310: 2020 0d0a 2020 2020 2020 2020 7365 6c66    ..        self
-00000320: 2e6c 6c6d 203d 206c 6c6d 0d0a 2020 2020  .llm = llm..    
-00000330: 2020 2020 7365 6c66 2e6c 6c6d 5f73 7769      self.llm_swi
-00000340: 7463 6820 3d20 6c6c 6d5f 7377 6974 6368  tch = llm_switch
-00000350: 0d0a 0d0a 2020 2020 2020 2020 7365 6c66  ....        self
-00000360: 2e74 6173 6b20 3d20 2222 220d 0a20 2020  .task = """..   
-00000370: 2020 2020 2054 6865 7265 2069 7320 6120       There is a 
-00000380: 7061 6e64 6173 2064 6174 6166 7261 6d65  pandas dataframe
-00000390: 2e0d 0a20 2020 2020 2020 2054 6865 206e  ...        The n
-000003a0: 616d 6520 6f66 2074 6865 2064 6174 6166  ame of the dataf
-000003b0: 7261 6d65 2069 7320 6064 6660 2e0d 0a20  rame is `df`... 
-000003c0: 2020 2020 2020 2054 6869 7320 6973 2074         This is t
-000003d0: 6865 2072 6573 756c 7420 6f66 2060 7072  he result of `pr
-000003e0: 696e 7428 6466 2e68 6561 6428 3129 2960  int(df.head(1))`
-000003f0: 3a0d 0a20 2020 2020 2020 207b 7d2e 0d0a  :..        {}...
-00000400: 2020 2020 2020 2020 5265 7475 726e 2074          Return t
-00000410: 6865 2070 7974 686f 6e20 636f 6465 2074  he python code t
-00000420: 6861 7420 7072 696e 7473 206f 7574 2074  hat prints out t
-00000430: 6865 2061 6e73 7765 7220 746f 2074 6865  he answer to the
-00000440: 2066 6f6c 6c6f 7769 6e67 2071 7565 7374   following quest
-00000450: 696f 6e20 3a20 7b7d 2e0d 0a20 2020 2020  ion : {}...     
-00000460: 2020 2041 6c77 6179 7320 696e 636c 7564     Always includ
-00000470: 6520 7468 6520 696d 706f 7274 2073 7461  e the import sta
-00000480: 7465 6d65 6e74 7320 6174 2074 6865 2074  tements at the t
-00000490: 6f70 206f 6620 7468 6520 636f 6465 2c20  op of the code, 
-000004a0: 616e 6420 636f 6d6d 656e 7473 2077 6865  and comments whe
-000004b0: 7265 206e 6563 6573 7361 7279 2e20 0d0a  re necessary. ..
-000004c0: 2020 2020 2020 2020 5072 6566 6978 2074          Prefix t
-000004d0: 6865 2070 7974 686f 6e20 636f 6465 2077  he python code w
-000004e0: 6974 6820 3c63 6f64 653e 2061 6e64 2073  ith <code> and s
-000004f0: 7566 6669 7820 7468 6520 636f 6465 2077  uffix the code w
-00000500: 6974 6820 3c2f 636f 6465 3e2e 2053 6b69  ith </code>. Ski
-00000510: 7020 6966 2074 6865 2061 6e73 7765 7220  p if the answer 
-00000520: 6361 6e20 6e6f 7420 6265 2065 7870 7265  can not be expre
-00000530: 7373 6564 2069 6e20 6120 636f 6465 2e0d  ssed in a code..
-00000540: 0a20 2020 2020 2020 204f 6666 6572 2061  .        Offer a
-00000550: 2020 7265 666c 6563 7469 6f6e 206f 6e20    reflection on 
-00000560: 796f 7572 2061 6e73 7765 722c 2061 6e64  your answer, and
-00000570: 2070 6f73 6962 626c 6520 7573 6520 6361   posibble use ca
-00000580: 7365 2e20 416c 736f 206f 6666 6572 2073  se. Also offer s
-00000590: 6f6d 6520 616c 7465 726e 6174 6976 6520  ome alternative 
-000005a0: 6170 7072 6f61 6368 6573 2074 6861 7420  approaches that 
-000005b0: 636f 756c 6420 6265 2062 656e 6566 6963  could be benefic
-000005c0: 6961 6c2e 0d0a 2020 2020 2020 2020 5072  ial...        Pr
-000005d0: 6566 6978 2074 6865 2072 6566 6c65 6374  efix the reflect
-000005e0: 696f 6e20 7769 7468 203c 7265 666c 6563  ion with <reflec
-000005f0: 7469 6f6e 3e20 616e 6420 7375 6666 6978  tion> and suffix
-00000600: 2074 6865 2072 6566 6c65 6374 696f 6e20   the reflection 
-00000610: 7769 7468 203c 2f72 6566 6c65 6374 696f  with </reflectio
-00000620: 6e3e 2e0d 0a20 2020 2020 2020 2046 696e  n>...        Fin
-00000630: 616c 6c79 206f 7574 7075 7420 6120 636f  ally output a co
-00000640: 6465 2066 6f72 206d 6572 6d61 6964 2064  de for mermaid d
-00000650: 6961 6772 616d 2e20 5468 6520 636f 6465  iagram. The code
-00000660: 2073 686f 756c 6420 7374 6172 7420 7769   should start wi
-00000670: 7468 2022 6772 6170 6820 5444 3b22 0d0a  th "graph TD;"..
-00000680: 2020 2020 2020 2020 5072 6566 6978 2074          Prefix t
-00000690: 6865 206d 6572 6d61 6964 2063 6f64 6520  he mermaid code 
-000006a0: 7769 7468 203c 666c 6f77 3e20 616e 6420  with <flow> and 
-000006b0: 7375 6666 6978 2074 6865 206d 6572 6d61  suffix the merma
-000006c0: 6964 2066 6c6f 7720 7769 7468 203c 2f66  id flow with </f
-000006d0: 6c6f 773e 2e0d 0a20 2020 2020 2020 2022  low>...        "
-000006e0: 2222 0d0a 0d0a 2020 2020 2020 2020 7365  ""....        se
-000006f0: 6c66 2e65 7272 6f72 5f63 6f72 7265 6374  lf.error_correct
-00000700: 5f74 6173 6b20 3d20 2222 220d 0a20 2020  _task = """..   
-00000710: 2020 2020 2054 6865 2063 6f64 6520 796f       The code yo
-00000720: 7520 7072 6f76 6964 6564 2072 6573 756c  u provided resul
-00000730: 7465 6420 696e 2061 6e20 6572 726f 722e  ted in an error.
-00000740: 0d0a 2020 2020 2020 2020 5468 6520 6572  ..        The er
-00000750: 726f 7220 6d65 7373 6167 6520 6973 3a20  ror message is: 
-00000760: 7b7d 2e0d 0a20 2020 2020 2020 2054 6865  {}...        The
-00000770: 2063 6f64 6520 796f 7520 7072 6f76 6964   code you provid
-00000780: 6564 2069 733a 207b 7d2e 0d0a 2020 2020  ed is: {}...    
-00000790: 2020 2020 5468 6520 7175 6573 7469 6f6e      The question
-000007a0: 2077 6173 3a20 7b7d 2e0d 0a20 2020 2020   was: {}...     
-000007b0: 2020 2052 6574 7572 6e20 6120 636f 7272     Return a corr
-000007c0: 6563 7465 6420 7079 7468 6f6e 2063 6f64  ected python cod
-000007d0: 6520 7468 6174 2066 6978 6573 2074 6865  e that fixes the
-000007e0: 2065 7272 6f72 2e0d 0a20 2020 2020 2020   error...       
-000007f0: 2041 6c77 6179 7320 696e 636c 7564 6520   Always include 
-00000800: 7468 6520 696d 706f 7274 2073 7461 7465  the import state
-00000810: 6d65 6e74 7320 6174 2074 6865 2074 6f70  ments at the top
-00000820: 206f 6620 7468 6520 636f 6465 2c20 616e   of the code, an
-00000830: 6420 636f 6d6d 656e 7473 2077 6865 7265  d comments where
-00000840: 206e 6563 6573 7361 7279 2e0d 0a20 2020   necessary...   
-00000850: 2020 2020 2050 7265 6669 7820 7468 6520       Prefix the 
-00000860: 7079 7468 6f6e 2063 6f64 6520 7769 7468  python code with
-00000870: 203c 636f 6465 3e20 616e 6420 7375 6666   <code> and suff
-00000880: 6978 2074 6865 2063 6f64 6520 7769 7468  ix the code with
-00000890: 203c 2f63 6f64 653e 2e20 536b 6970 2069   </code>. Skip i
-000008a0: 6620 7468 6520 616e 7377 6572 2063 616e  f the answer can
-000008b0: 206e 6f74 2062 6520 6578 7072 6573 7365   not be expresse
-000008c0: 6420 696e 2061 2063 6f64 652e 0d0a 2020  d in a code...  
-000008d0: 2020 2020 2020 4f66 6665 7220 6120 2072        Offer a  r
-000008e0: 6566 6c65 6374 696f 6e20 6f6e 2079 6f75  eflection on you
-000008f0: 7220 616e 7377 6572 2c20 616e 6420 706f  r answer, and po
-00000900: 7369 6262 6c65 2075 7365 2063 6173 652e  sibble use case.
-00000910: 2041 6c73 6f20 6f66 6665 7220 736f 6d65   Also offer some
-00000920: 2061 6c74 6572 6e61 7469 7665 2061 7070   alternative app
-00000930: 726f 6163 6865 7320 7468 6174 2063 6f75  roaches that cou
-00000940: 6c64 2062 6520 6265 6e65 6669 6369 616c  ld be beneficial
-00000950: 2e0d 0a20 2020 2020 2020 2050 7265 6669  ...        Prefi
-00000960: 7820 7468 6520 7265 666c 6563 7469 6f6e  x the reflection
-00000970: 2077 6974 6820 3c72 6566 6c65 6374 696f   with <reflectio
-00000980: 6e3e 2061 6e64 2073 7566 6669 7820 7468  n> and suffix th
-00000990: 6520 7265 666c 6563 7469 6f6e 2077 6974  e reflection wit
-000009a0: 6820 3c2f 7265 666c 6563 7469 6f6e 3e2e  h </reflection>.
-000009b0: 0d0a 2020 2020 2020 2020 4669 6e61 6c6c  ..        Finall
-000009c0: 7920 6f75 7470 7574 2061 2063 6f64 6520  y output a code 
-000009d0: 666f 7220 6d65 726d 6169 6420 6469 6167  for mermaid diag
-000009e0: 7261 6d2e 2054 6865 2063 6f64 6520 7368  ram. The code sh
-000009f0: 6f75 6c64 2073 7461 7274 2077 6974 6820  ould start with 
-00000a00: 2267 7261 7068 2054 443b 220d 0a20 2020  "graph TD;"..   
-00000a10: 2020 2020 2050 7265 6669 7820 7468 6520       Prefix the 
-00000a20: 6d65 726d 6169 6420 636f 6465 2077 6974  mermaid code wit
-00000a30: 6820 3c66 6c6f 773e 2061 6e64 2073 7566  h <flow> and suf
-00000a40: 6669 7820 7468 6520 6d65 726d 6169 6420  fix the mermaid 
-00000a50: 666c 6f77 2077 6974 6820 3c2f 666c 6f77  flow with </flow
-00000a60: 3e2e 0d0a 2020 2020 2020 2020 2222 220d  >...        """.
-00000a70: 0a0d 0a20 2020 2020 2020 206f 7065 6e61  ...        opena
-00000a80: 692e 6170 695f 6b65 7920 3d20 7365 6c66  i.api_key = self
-00000a90: 2e41 5049 5f4b 4559 0d0a 2020 2020 2020  .API_KEY..      
-00000aa0: 2020 7365 6c66 2e74 6f74 616c 5f74 6f6b    self.total_tok
-00000ab0: 656e 735f 7573 6564 203d 205b 5d0d 0a0d  ens_used = []...
-00000ac0: 0a20 2020 2064 6566 206d 6d28 7365 6c66  .    def mm(self
-00000ad0: 2c20 6772 6170 6829 3a0d 0a20 2020 2020  , graph):..     
-00000ae0: 2020 2067 7261 7068 6279 7465 7320 3d20     graphbytes = 
-00000af0: 6772 6170 682e 656e 636f 6465 2822 6173  graph.encode("as
-00000b00: 6369 6922 290d 0a20 2020 2020 2020 2062  cii")..        b
-00000b10: 6173 6536 345f 6279 7465 7320 3d20 6261  ase64_bytes = ba
-00000b20: 7365 3634 2e62 3634 656e 636f 6465 2867  se64.b64encode(g
-00000b30: 7261 7068 6279 7465 7329 0d0a 2020 2020  raphbytes)..    
-00000b40: 2020 2020 6261 7365 3634 5f73 7472 696e      base64_strin
-00000b50: 6720 3d20 6261 7365 3634 5f62 7974 6573  g = base64_bytes
-00000b60: 2e64 6563 6f64 6528 2261 7363 6969 2229  .decode("ascii")
-00000b70: 0d0a 2020 2020 2020 2020 696d 675f 7572  ..        img_ur
-00000b80: 6c20 3d20 2268 7474 7073 3a2f 2f6d 6572  l = "https://mer
-00000b90: 6d61 6964 2e69 6e6b 2f69 6d67 2f22 202b  maid.ink/img/" +
-00000ba0: 2062 6173 6536 345f 7374 7269 6e67 0d0a   base64_string..
-00000bb0: 2020 2020 2020 2020 7265 7475 726e 2069          return i
-00000bc0: 6d67 5f75 726c 0d0a 0d0a 2020 2020 6465  mg_url....    de
-00000bd0: 6620 6c6c 6d5f 6361 6c6c 2873 656c 662c  f llm_call(self,
-00000be0: 206d 6573 7361 6765 733a 2073 7472 2c20   messages: str, 
-00000bf0: 7465 6d70 6572 6174 7572 653a 2066 6c6f  temperature: flo
-00000c00: 6174 203d 2030 2c20 6d61 785f 746f 6b65  at = 0, max_toke
-00000c10: 6e73 3a20 696e 7420 3d20 3130 3030 293a  ns: int = 1000):
-00000c20: 0d0a 2020 2020 2020 2020 7265 7370 6f6e  ..        respon
-00000c30: 7365 203d 206f 7065 6e61 692e 4368 6174  se = openai.Chat
-00000c40: 436f 6d70 6c65 7469 6f6e 2e63 7265 6174  Completion.creat
-00000c50: 6528 0d0a 2020 2020 2020 2020 2020 2020  e(..            
-00000c60: 6d6f 6465 6c3d 7365 6c66 2e6c 6c6d 2c0d  model=self.llm,.
-00000c70: 0a20 2020 2020 2020 2020 2020 206d 6573  .            mes
-00000c80: 7361 6765 733d 6d65 7373 6167 6573 2c0d  sages=messages,.
-00000c90: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
-00000ca0: 7065 7261 7475 7265 3d74 656d 7065 7261  perature=tempera
-00000cb0: 7475 7265 2c0d 0a20 2020 2020 2020 2020  ture,..         
-00000cc0: 2020 206d 6178 5f74 6f6b 656e 733d 6d61     max_tokens=ma
-00000cd0: 785f 746f 6b65 6e73 2c0d 0a20 2020 2020  x_tokens,..     
-00000ce0: 2020 2029 0d0a 0d0a 2020 2020 2020 2020     )....        
-00000cf0: 636f 6e74 656e 7420 3d20 7265 7370 6f6e  content = respon
-00000d00: 7365 2e63 686f 6963 6573 5b30 5d2e 6d65  se.choices[0].me
-00000d10: 7373 6167 652e 636f 6e74 656e 742e 7374  ssage.content.st
-00000d20: 7269 7028 290d 0a20 2020 2020 2020 2074  rip()..        t
-00000d30: 6f6b 656e 735f 7573 6564 203d 2072 6573  okens_used = res
-00000d40: 706f 6e73 652e 7573 6167 652e 746f 7461  ponse.usage.tota
-00000d50: 6c5f 746f 6b65 6e73 0d0a 0d0a 2020 2020  l_tokens....    
-00000d60: 2020 2020 7265 7475 726e 2063 6f6e 7465      return conte
-00000d70: 6e74 2c20 746f 6b65 6e73 5f75 7365 640d  nt, tokens_used.
-00000d80: 0a20 2020 200d 0a20 2020 2023 2046 756e  .    ..    # Fun
-00000d90: 6374 696f 6e20 746f 2073 616e 6974 697a  ction to sanitiz
-00000da0: 6520 7468 6520 6f75 7470 7574 2066 726f  e the output fro
-00000db0: 6d20 7468 6520 4c4c 4d0d 0a20 2020 2064  m the LLM..    d
-00000dc0: 6566 205f 6578 7472 6163 745f 636f 6465  ef _extract_code
-00000dd0: 2873 656c 662c 7265 7370 6f6e 7365 3a20  (self,response: 
-00000de0: 7374 722c 2073 6570 6172 6174 6f72 3a20  str, separator: 
-00000df0: 7374 7220 3d20 2260 6060 2229 202d 3e20  str = "```") -> 
-00000e00: 7374 723a 0d0a 0d0a 2020 2020 2020 2020  str:....        
-00000e10: 2320 4465 6669 6e65 2061 2062 6c61 636b  # Define a black
-00000e20: 6c69 7374 206f 6620 5079 7468 6f6e 206b  list of Python k
-00000e30: 6579 776f 7264 7320 616e 6420 6675 6e63  eywords and func
-00000e40: 7469 6f6e 7320 7468 6174 2061 7265 206e  tions that are n
-00000e50: 6f74 2061 6c6c 6f77 6564 0d0a 2020 2020  ot allowed..    
-00000e60: 2020 2020 626c 6163 6b6c 6973 7420 3d20      blacklist = 
-00000e70: 5b27 6f73 272c 2773 7562 7072 6f63 6573  ['os','subproces
-00000e80: 7327 2c27 7379 7327 2c27 6576 616c 272c  s','sys','eval',
-00000e90: 2765 7865 6327 2c27 6669 6c65 272c 2773  'exec','file','s
-00000ea0: 6f63 6b65 7427 2c27 7572 6c6c 6962 272c  ocket','urllib',
-00000eb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000ec0: 2020 2020 2020 2773 6875 7469 6c27 2c27        'shutil','
-00000ed0: 7069 636b 6c65 272c 2763 7479 7065 7327  pickle','ctypes'
-00000ee0: 2c27 6d75 6c74 6970 726f 6365 7373 696e  ,'multiprocessin
-00000ef0: 6727 2c27 7465 6d70 6669 6c65 272c 2767  g','tempfile','g
-00000f00: 6c6f 6227 2c27 636f 6465 272c 2770 7479  lob','code','pty
-00000f10: 272c 2763 6f6d 6d61 6e64 7327 2c0d 0a20  ','commands',.. 
-00000f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f30: 2020 2027 7265 7175 6573 7473 272c 2763     'requests','c
-00000f40: 6769 272c 2763 6769 7462 272c 2778 6d6c  gi','cgitb','xml
-00000f50: 2e65 7472 6565 2e45 6c65 6d65 6e74 5472  .etree.ElementTr
-00000f60: 6565 272c 2762 7569 6c74 696e 7327 0d0a  ee','builtins'..
-00000f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f80: 2020 2020 5d0d 0a20 2020 2020 2020 200d      ]..        .
-00000f90: 0a20 2020 2020 2020 2023 2053 6561 7263  .        # Searc
-00000fa0: 6820 666f 7220 6120 7061 7474 6572 6e20  h for a pattern 
-00000fb0: 6265 7477 6565 6e20 3c72 6566 6c65 6374  between <reflect
-00000fc0: 696f 6e3e 2061 6e64 203c 2f72 6566 6c65  ion> and </refle
-00000fd0: 6374 696f 6e3e 2069 6e20 7468 6520 7265  ction> in the re
-00000fe0: 7370 6f6e 7365 0d0a 2020 2020 2020 2020  sponse..        
-00000ff0: 6d61 7463 6820 3d20 7265 2e73 6561 7263  match = re.searc
-00001000: 6828 7222 3c72 6566 6c65 6374 696f 6e3e  h(r"<reflection>
-00001010: 282e 2a29 3c2f 7265 666c 6563 7469 6f6e  (.*)</reflection
-00001020: 3e22 2c20 7265 7370 6f6e 7365 2c20 7265  >", response, re
-00001030: 2e44 4f54 414c 4c29 0d0a 2020 2020 2020  .DOTALL)..      
-00001040: 2020 6966 206d 6174 6368 3a0d 0a20 2020    if match:..   
-00001050: 2020 2020 2020 2020 2023 2049 6620 6120           # If a 
-00001060: 6d61 7463 6820 6973 2066 6f75 6e64 2c20  match is found, 
-00001070: 6578 7472 6163 7420 7468 6520 7265 666c  extract the refl
-00001080: 6563 7469 6f6e 2062 6574 7765 656e 203c  ection between <
-00001090: 7265 666c 6563 7469 6f6e 3e20 616e 6420  reflection> and 
-000010a0: 3c2f 7265 666c 6563 7469 6f6e 3e0d 0a20  </reflection>.. 
-000010b0: 2020 2020 2020 2020 2020 2072 6566 6c65             refle
-000010c0: 6374 696f 6e20 3d20 6d61 7463 682e 6772  ction = match.gr
-000010d0: 6f75 7028 3129 0d0a 2020 2020 2020 2020  oup(1)..        
-000010e0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-000010f0: 2020 2072 6566 6c65 6374 696f 6e20 3d20     reflection = 
-00001100: 2222 0d0a 0d0a 2020 2020 2020 2020 2320  ""....        # 
-00001110: 5365 6172 6368 2066 6f72 2061 2070 6174  Search for a pat
-00001120: 7465 726e 2062 6574 7765 656e 203c 666c  tern between <fl
-00001130: 6f77 3e20 616e 6420 3c2f 666c 6f77 3e20  ow> and </flow> 
-00001140: 696e 2074 6865 2072 6573 706f 6e73 650d  in the response.
-00001150: 0a20 2020 2020 2020 206d 6174 6368 203d  .        match =
-00001160: 2072 652e 7365 6172 6368 2872 223c 666c   re.search(r"<fl
-00001170: 6f77 3e28 2e2a 293c 2f66 6c6f 773e 222c  ow>(.*)</flow>",
-00001180: 2072 6573 706f 6e73 652c 2072 652e 444f   response, re.DO
-00001190: 5441 4c4c 290d 0a20 2020 2020 2020 2069  TALL)..        i
-000011a0: 6620 6d61 7463 683a 0d0a 2020 2020 2020  f match:..      
-000011b0: 2020 2020 2020 2320 4966 2061 206d 6174        # If a mat
-000011c0: 6368 2069 7320 666f 756e 642c 2065 7874  ch is found, ext
-000011d0: 7261 6374 2074 6865 2072 6566 6c65 6374  ract the reflect
-000011e0: 696f 6e20 6265 7477 6565 6e20 3c72 6566  ion between <ref
-000011f0: 6c65 6374 696f 6e3e 2061 6e64 203c 2f72  lection> and </r
-00001200: 6566 6c65 6374 696f 6e3e 0d0a 2020 2020  eflection>..    
-00001210: 2020 2020 2020 2020 666c 6f77 203d 206d          flow = m
-00001220: 6174 6368 2e67 726f 7570 2831 290d 0a20  atch.group(1).. 
-00001230: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-00001240: 2020 2020 2020 2020 2020 666c 6f77 203d            flow =
-00001250: 2022 220d 0a0d 0a20 2020 2020 2020 2023   ""....        #
-00001260: 2053 6561 7263 6820 666f 7220 6120 7061   Search for a pa
-00001270: 7474 6572 6e20 6265 7477 6565 6e20 3c63  ttern between <c
-00001280: 6f64 653e 2061 6e64 203c 2f63 6f64 653e  ode> and </code>
-00001290: 2069 6e20 7468 6520 6578 7472 6163 7465   in the extracte
-000012a0: 6420 636f 6465 0d0a 2020 2020 2020 2020  d code..        
-000012b0: 6d61 7463 6820 3d20 7265 2e73 6561 7263  match = re.searc
-000012c0: 6828 7222 3c63 6f64 653e 282e 2a29 3c2f  h(r"<code>(.*)</
-000012d0: 636f 6465 3e22 2c20 7265 7370 6f6e 7365  code>", response
-000012e0: 2c20 7265 2e44 4f54 414c 4c29 0d0a 2020  , re.DOTALL)..  
-000012f0: 2020 2020 2020 6966 206d 6174 6368 3a0d        if match:.
-00001300: 0a20 2020 2020 2020 2020 2020 2023 2049  .            # I
-00001310: 6620 6120 6d61 7463 6820 6973 2066 6f75  f a match is fou
-00001320: 6e64 2c20 6578 7472 6163 7420 7468 6520  nd, extract the 
-00001330: 636f 6465 2062 6574 7765 656e 203c 636f  code between <co
-00001340: 6465 3e20 616e 6420 3c2f 636f 6465 3e0d  de> and </code>.
-00001350: 0a20 2020 2020 2020 2020 2020 2063 6f64  .            cod
-00001360: 6520 3d20 6d61 7463 682e 6772 6f75 7028  e = match.group(
-00001370: 3129 0d0a 2020 2020 2020 2020 2020 2020  1)..            
-00001380: 2320 4966 2074 6865 2072 6573 706f 6e73  # If the respons
-00001390: 6520 636f 6e74 6169 6e73 2074 6865 2073  e contains the s
-000013a0: 6570 6172 6174 6f72 2c20 6578 7472 6163  eparator, extrac
-000013b0: 7420 7468 6520 636f 6465 2062 6c6f 636b  t the code block
-000013c0: 2062 6574 7765 656e 2074 6865 2073 6570   between the sep
-000013d0: 6172 6174 6f72 730d 0a20 2020 2020 2020  arators..       
-000013e0: 2020 2020 2069 6620 6c65 6e28 636f 6465       if len(code
-000013f0: 2e73 706c 6974 2873 6570 6172 6174 6f72  .split(separator
-00001400: 2929 203e 2031 3a0d 0a20 2020 2020 2020  )) > 1:..       
-00001410: 2020 2020 2020 2020 2063 6f64 6520 3d20           code = 
-00001420: 636f 6465 2e73 706c 6974 2873 6570 6172  code.split(separ
-00001430: 6174 6f72 295b 315d 0d0a 0d0a 2020 2020  ator)[1]....    
-00001440: 2020 2020 2320 4966 2074 6865 2072 6573      # If the res
-00001450: 706f 6e73 6520 636f 6e74 6169 6e73 2074  ponse contains t
-00001460: 6865 2073 6570 6172 6174 6f72 2c20 6578  he separator, ex
-00001470: 7472 6163 7420 7468 6520 636f 6465 2062  tract the code b
-00001480: 6c6f 636b 2062 6574 7765 656e 2074 6865  lock between the
-00001490: 2073 6570 6172 6174 6f72 730d 0a20 2020   separators..   
-000014a0: 2020 2020 2069 6620 6c65 6e28 7265 7370       if len(resp
-000014b0: 6f6e 7365 2e73 706c 6974 2873 6570 6172  onse.split(separ
-000014c0: 6174 6f72 2929 203e 2031 3a0d 0a20 2020  ator)) > 1:..   
-000014d0: 2020 2020 2020 2020 2063 6f64 6520 3d20           code = 
-000014e0: 7265 7370 6f6e 7365 2e73 706c 6974 2873  response.split(s
-000014f0: 6570 6172 6174 6f72 295b 315d 0d0a 2020  eparator)[1]..  
-00001500: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00001510: 2020 2020 2320 5265 6d6f 7665 2074 6865      # Remove the
-00001520: 2022 7079 7468 6f6e 2220 6f72 2022 7079   "python" or "py
-00001530: 2220 7072 6566 6978 2069 6620 7072 6573  " prefix if pres
-00001540: 656e 740d 0a20 2020 2020 2020 2069 6620  ent..        if 
-00001550: 7265 2e6d 6174 6368 2872 225e 2870 7974  re.match(r"^(pyt
-00001560: 686f 6e7c 7079 2922 2c20 636f 6465 293a  hon|py)", code):
-00001570: 0d0a 2020 2020 2020 2020 2020 2020 636f  ..            co
-00001580: 6465 203d 2072 652e 7375 6228 7222 5e28  de = re.sub(r"^(
-00001590: 7079 7468 6f6e 7c70 7929 222c 2022 222c  python|py)", "",
-000015a0: 2063 6f64 6529 0d0a 2020 2020 2020 2020   code)..        
-000015b0: 2320 4966 2074 6865 2063 6f64 6520 6973  # If the code is
-000015c0: 2062 6574 7765 656e 2073 696e 676c 6520   between single 
-000015d0: 6261 636b 7469 636b 732c 2065 7874 7261  backticks, extra
-000015e0: 6374 2074 6865 2063 6f64 6520 6265 7477  ct the code betw
-000015f0: 6565 6e20 7468 656d 0d0a 2020 2020 2020  een them..      
-00001600: 2020 6966 2072 652e 6d61 7463 6828 7222    if re.match(r"
-00001610: 5e60 2e2a 6024 222c 2063 6f64 6529 3a0d  ^`.*`$", code):.
-00001620: 0a20 2020 2020 2020 2020 2020 2063 6f64  .            cod
-00001630: 6520 3d20 7265 2e73 7562 2872 225e 6028  e = re.sub(r"^`(
-00001640: 2e2a 2960 2422 2c20 7222 5c31 222c 2063  .*)`$", r"\1", c
-00001650: 6f64 6529 0d0a 0d0a 2020 2020 2020 2020  ode)....        
-00001660: 2320 5265 6d6f 7665 2061 6e79 2069 6e73  # Remove any ins
-00001670: 7461 6e63 6573 206f 6620 2264 6620 3d20  tances of "df = 
-00001680: 7064 2e72 6561 645f 6373 7628 2766 696c  pd.read_csv('fil
-00001690: 656e 616d 652e 6373 7627 2922 2066 726f  ename.csv')" fro
-000016a0: 6d20 7468 6520 636f 6465 0d0a 2020 2020  m the code..    
-000016b0: 2020 2020 636f 6465 203d 2072 652e 7375      code = re.su
-000016c0: 6228 7222 6466 5c73 2a3d 5c73 2a70 645c  b(r"df\s*=\s*pd\
-000016d0: 2e72 6561 645f 6373 765c 2827 2e2a 3f27  .read_csv\('.*?'
-000016e0: 5c29 222c 2022 222c 2063 6f64 6529 0d0a  \)", "", code)..
-000016f0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00001700: 2020 2320 5265 6d6f 7665 2061 6e79 206f    # Remove any o
-00001710: 6363 7572 7265 6e63 6573 206f 6620 6466  ccurrences of df
-00001720: 203d 2070 642e 4461 7461 4672 616d 6528   = pd.DataFrame(
-00001730: 2920 7769 7468 2061 6e79 206e 756d 6265  ) with any numbe
-00001740: 7220 6f66 2063 6861 7261 6374 6572 7320  r of characters 
-00001750: 696e 7369 6465 2074 6865 2070 6172 656e  inside the paren
-00001760: 7468 6573 6573 2e0d 0a20 2020 2020 2020  theses...       
-00001770: 2063 6f64 6520 3d20 7265 2e73 7562 2872   code = re.sub(r
-00001780: 2264 665c 732a 3d5c 732a 7064 5c2e 4461  "df\s*=\s*pd\.Da
-00001790: 7461 4672 616d 655c 282e 2a3f 5c29 222c  taFrame\(.*?\)",
-000017a0: 2022 222c 2063 6f64 6529 0d0a 0d0a 2020   "", code)....  
-000017b0: 2020 2020 2020 2320 4465 6669 6e65 2074        # Define t
-000017c0: 6865 2072 6567 756c 6172 2065 7870 7265  he regular expre
-000017d0: 7373 696f 6e20 7061 7474 6572 6e20 746f  ssion pattern to
-000017e0: 206d 6174 6368 2074 6865 2062 6c61 636b   match the black
-000017f0: 6c69 7374 2069 7465 6d73 0d0a 2020 2020  list items..    
-00001800: 2020 2020 7061 7474 6572 6e20 3d20 7222      pattern = r"
-00001810: 5e28 2e2a 5c62 2822 202b 2022 7c22 2e6a  ^(.*\b(" + "|".j
-00001820: 6f69 6e28 626c 6163 6b6c 6973 7429 202b  oin(blacklist) +
-00001830: 2072 2229 5c62 2e2a 2924 220d 0a0d 0a20   r")\b.*)$".... 
-00001840: 2020 2020 2020 2023 2052 6570 6c61 6365         # Replace
-00001850: 2074 6865 2062 6c61 636b 6c69 7374 2069   the blacklist i
-00001860: 7465 6d73 2077 6974 6820 636f 6d6d 656e  tems with commen
-00001870: 7473 0d0a 2020 2020 2020 2020 636f 6465  ts..        code
-00001880: 203d 2072 652e 7375 6228 7061 7474 6572   = re.sub(patter
-00001890: 6e2c 2072 2223 206e 6f74 2061 6c6c 6f77  n, r"# not allow
-000018a0: 6564 205c 3122 2c20 636f 6465 2c20 666c  ed \1", code, fl
-000018b0: 6167 733d 7265 2e4d 554c 5449 4c49 4e45  ags=re.MULTILINE
-000018c0: 290d 0a0d 0a20 2020 2020 2020 2023 2052  )....        # R
-000018d0: 6574 7572 6e20 7468 6520 636c 6561 6e65  eturn the cleane
-000018e0: 6420 616e 6420 6578 7472 6163 7465 6420  d and extracted 
-000018f0: 636f 6465 0d0a 2020 2020 2020 2020 7265  code..        re
-00001900: 7475 726e 2063 6f64 652e 7374 7269 7028  turn code.strip(
-00001910: 292c 2072 6566 6c65 6374 696f 6e2e 7374  ), reflection.st
-00001920: 7269 7028 292c 2066 6c6f 772e 7374 7269  rip(), flow.stri
-00001930: 7028 290d 0a0d 0a20 2020 2064 6566 2070  p()....    def p
-00001940: 645f 6167 656e 745f 636f 6e76 6572 7365  d_agent_converse
-00001950: 2873 656c 662c 2071 7565 7374 696f 6e3d  (self, question=
-00001960: 4e6f 6e65 293a 0d0a 2020 2020 2020 2020  None):..        
-00001970: 2320 496e 6974 6961 6c69 7a65 2074 6865  # Initialize the
-00001980: 206d 6573 7361 6765 7320 6c69 7374 2077   messages list w
-00001990: 6974 6820 6120 7379 7374 656d 206d 6573  ith a system mes
-000019a0: 7361 6765 2063 6f6e 7461 696e 696e 6720  sage containing 
-000019b0: 7468 6520 7461 736b 2070 726f 6d70 740d  the task prompt.
-000019c0: 0a20 2020 2020 2020 206d 6573 7361 6765  .        message
-000019d0: 7320 3d20 5b7b 2272 6f6c 6522 3a20 2273  s = [{"role": "s
-000019e0: 7973 7465 6d22 2c20 2263 6f6e 7465 6e74  ystem", "content
-000019f0: 223a 2073 656c 662e 7461 736b 2e66 6f72  ": self.task.for
-00001a00: 6d61 7428 7365 6c66 2e64 665f 6865 6164  mat(self.df_head
-00001a10: 2c20 2222 297d 5d0d 0a0d 0a20 2020 2020  , "")}]....     
-00001a20: 2020 2023 2046 756e 6374 696f 6e20 746f     # Function to
-00001a30: 2064 6973 706c 6179 2072 6573 756c 7473   display results
-00001a40: 206e 6963 656c 790d 0a20 2020 2020 2020   nicely..       
-00001a50: 2064 6566 2064 6973 706c 6179 5f72 6573   def display_res
-00001a60: 756c 7473 2861 6e73 7765 722c 2063 6f64  ults(answer, cod
-00001a70: 652c 2072 6566 6c65 6374 696f 6e2c 2066  e, reflection, f
-00001a80: 6c6f 772c 2074 6f74 616c 5f74 6f6b 656e  low, total_token
-00001a90: 735f 7573 6564 5f73 756d 293a 0d0a 2020  s_used_sum):..  
-00001aa0: 2020 2020 2020 2020 2020 6966 2027 6970            if 'ip
-00001ab0: 796b 6572 6e65 6c27 2069 6e20 7379 732e  ykernel' in sys.
-00001ac0: 6d6f 6475 6c65 733a 0d0a 2020 2020 2020  modules:..      
-00001ad0: 2020 2020 2020 2020 2020 2320 4a75 7079            # Jupy
-00001ae0: 7465 7220 6e6f 7465 626f 6f6b 206f 7220  ter notebook or 
-00001af0: 6970 7974 686f 6e0d 0a20 2020 2020 2020  ipython..       
-00001b00: 2020 2020 2020 2020 2064 6973 706c 6179           display
-00001b10: 2848 544d 4c28 6627 3c70 3e3c 6220 7374  (HTML(f'<p><b st
-00001b20: 796c 653d 2263 6f6c 6f72 3a62 6c75 653b  yle="color:blue;
-00001b30: 223e 416e 7377 6572 3a3c 2f62 3e3c 6272  ">Answer:</b><br
-00001b40: 3e3c 7072 6520 7374 796c 653d 2263 6f6c  ><pre style="col
-00001b50: 6f72 3a62 6c61 636b 3b22 3e3c 623e 7b61  or:black;"><b>{a
-00001b60: 6e73 7765 727d 3c2f 623e 3c2f 7072 653e  nswer}</b></pre>
-00001b70: 3c2f 703e 3c62 723e 2729 290d 0a20 2020  </p><br>'))..   
-00001b80: 2020 2020 2020 2020 2020 2020 2064 6973               dis
-00001b90: 706c 6179 2848 544d 4c28 6627 3c70 3e3c  play(HTML(f'<p><
-00001ba0: 6220 7374 796c 653d 2263 6f6c 6f72 3a62  b style="color:b
-00001bb0: 6c75 653b 223e 436f 6465 3a3c 2f62 3e3c  lue;">Code:</b><
-00001bc0: 6272 3e3c 7072 6520 7374 796c 653d 2263  br><pre style="c
-00001bd0: 6f6c 6f72 3a23 3535 3535 3535 3b22 3e7b  olor:#555555;">{
-00001be0: 636f 6465 7d3c 2f70 7265 3e3c 2f70 3e3c  code}</pre></p><
-00001bf0: 6272 3e27 2929 0d0a 2020 2020 2020 2020  br>'))..        
-00001c00: 2020 2020 2020 2020 6469 7370 6c61 7928          display(
-00001c10: 4854 4d4c 2866 273c 703e 3c62 2073 7479  HTML(f'<p><b sty
-00001c20: 6c65 3d22 636f 6c6f 723a 626c 7565 3b22  le="color:blue;"
-00001c30: 3e54 686f 7567 6874 733a 3c2f 623e 3c62  >Thoughts:</b><b
-00001c40: 723e 3c62 2073 7479 6c65 3d22 636f 6c6f  r><b style="colo
-00001c50: 723a 626c 6163 6b3b 223e 7b72 6566 6c65  r:black;">{refle
-00001c60: 6374 696f 6e7d 3c2f 623e 3c2f 703e 3c62  ction}</b></p><b
-00001c70: 723e 2729 290d 0a20 2020 2020 2020 2020  r>'))..         
-00001c80: 2020 2020 2020 2064 6973 706c 6179 2848         display(H
-00001c90: 544d 4c28 6627 3c70 3e3c 6220 7374 796c  TML(f'<p><b styl
-00001ca0: 653d 2263 6f6c 6f72 3a62 6c75 653b 223e  e="color:blue;">
-00001cb0: 416e 616c 7973 6973 2046 6c6f 773a 3c2f  Analysis Flow:</
-00001cc0: 623e 3c62 723e 3c69 6d67 2073 7263 3d22  b><br><img src="
-00001cd0: 7b73 656c 662e 6d6d 2866 6c6f 7729 7d22  {self.mm(flow)}"
-00001ce0: 2061 6c74 3d22 416e 616c 7973 6973 2046   alt="Analysis F
-00001cf0: 6c6f 7722 3e3c 2f69 6d67 3e3c 2f70 3e3c  low"></img></p><
-00001d00: 6272 3e27 2929 0d0a 2020 2020 2020 2020  br>'))..        
-00001d10: 2020 2020 2020 2020 6469 7370 6c61 7928          display(
-00001d20: 4854 4d4c 2866 273c 703e 3c62 2073 7479  HTML(f'<p><b sty
-00001d30: 6c65 3d22 636f 6c6f 723a 626c 7565 3b22  le="color:blue;"
-00001d40: 3e54 6f74 616c 2054 6f6b 656e 7320 5573  >Total Tokens Us
-00001d50: 6564 3a3c 2f62 3e3c 6272 3e3c 7370 616e  ed:</b><br><span
-00001d60: 2073 7479 6c65 3d22 636f 6c6f 723a 626c   style="color:bl
-00001d70: 6163 6b3b 223e 7b74 6f74 616c 5f74 6f6b  ack;">{total_tok
-00001d80: 656e 735f 7573 6564 5f73 756d 7d3c 2f73  ens_used_sum}</s
-00001d90: 7061 6e3e 3c2f 703e 3c62 723e 2729 290d  pan></p><br>')).
-00001da0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00001db0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00001dc0: 2020 2020 2320 4f74 6865 7220 656e 7669      # Other envi
-00001dd0: 726f 6e6d 656e 7420 286c 696b 6520 7465  ronment (like te
-00001de0: 726d 696e 616c 290d 0a20 2020 2020 2020  rminal)..       
-00001df0: 2020 2020 2020 2020 2063 7072 696e 7428           cprint(
-00001e00: 6622 5c6e 416e 7377 6572 3a5c 6e7b 616e  f"\nAnswer:\n{an
-00001e10: 7377 6572 7d5c 6e22 2c20 2767 7265 656e  swer}\n", 'green
-00001e20: 272c 2061 7474 7273 3d5b 2762 6f6c 6427  ', attrs=['bold'
-00001e30: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00001e40: 2020 2020 6370 7269 6e74 2866 2243 6f64      cprint(f"Cod
-00001e50: 653a 5c6e 7b63 6f64 657d 5c6e 222c 2027  e:\n{code}\n", '
-00001e60: 6772 6565 6e27 2c20 6174 7472 733d 5b27  green', attrs=['
-00001e70: 626f 6c64 275d 290d 0a20 2020 2020 2020  bold'])..       
-00001e80: 2020 2020 2020 2020 2063 7072 696e 7428           cprint(
-00001e90: 6622 5468 6f75 6768 7473 3a5c 6e7b 7265  f"Thoughts:\n{re
-00001ea0: 666c 6563 7469 6f6e 7d5c 6e22 2c20 2767  flection}\n", 'g
-00001eb0: 7265 656e 272c 2061 7474 7273 3d5b 2762  reen', attrs=['b
-00001ec0: 6f6c 6427 5d29 0d0a 2020 2020 2020 2020  old'])..        
-00001ed0: 2020 2020 2020 2020 6370 7269 6e74 2866          cprint(f
-00001ee0: 2254 6f74 616c 2074 6f6b 656e 7320 7573  "Total tokens us
-00001ef0: 6564 3a5c 6e7b 746f 7461 6c5f 746f 6b65  ed:\n{total_toke
-00001f00: 6e73 5f75 7365 645f 7375 6d7d 5c6e 222c  ns_used_sum}\n",
-00001f10: 2027 7965 6c6c 6f77 272c 2061 7474 7273   'yellow', attrs
-00001f20: 3d5b 2762 6f6c 6427 5d29 0d0a 0d0a 2020  =['bold'])....  
-00001f30: 2020 2020 2020 2320 4966 2061 2071 7565        # If a que
-00001f40: 7374 696f 6e20 6973 2070 726f 7669 6465  stion is provide
-00001f50: 642c 2073 6b69 7020 7468 6520 696e 7075  d, skip the inpu
-00001f60: 7420 7072 6f6d 7074 0d0a 2020 2020 2020  t prompt..      
-00001f70: 2020 6966 2071 7565 7374 696f 6e20 6973    if question is
-00001f80: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
-00001f90: 2020 2020 2020 2020 2320 4361 6c6c 2074          # Call t
-00001fa0: 6865 2070 645f 6167 656e 7420 6d65 7468  he pd_agent meth
-00001fb0: 6f64 2077 6974 6820 7468 6520 7573 6572  od with the user
-00001fc0: 2773 2071 7565 7374 696f 6e2c 2074 6865  's question, the
-00001fd0: 206d 6573 7361 6765 7320 6c69 7374 2c20   messages list, 
-00001fe0: 616e 6420 7468 6520 6461 7461 6672 616d  and the datafram
-00001ff0: 650d 0a20 2020 2020 2020 2020 2020 2061  e..            a
-00002000: 6e73 7765 722c 2063 6f64 652c 2072 6566  nswer, code, ref
-00002010: 6c65 6374 696f 6e2c 2066 6c6f 772c 2074  lection, flow, t
-00002020: 6f74 616c 5f74 6f6b 656e 735f 7573 6564  otal_tokens_used
-00002030: 5f73 756d 203d 2073 656c 662e 7064 5f61  _sum = self.pd_a
-00002040: 6765 6e74 2871 7565 7374 696f 6e2c 206d  gent(question, m
-00002050: 6573 7361 6765 732c 2073 656c 662e 6466  essages, self.df
-00002060: 290d 0a20 2020 2020 2020 2020 2020 2064  )..            d
-00002070: 6973 706c 6179 5f72 6573 756c 7473 2861  isplay_results(a
-00002080: 6e73 7765 722c 2063 6f64 652c 2072 6566  nswer, code, ref
-00002090: 6c65 6374 696f 6e2c 2066 6c6f 772c 2074  lection, flow, t
-000020a0: 6f74 616c 5f74 6f6b 656e 735f 7573 6564  otal_tokens_used
-000020b0: 5f73 756d 290d 0a20 2020 2020 2020 2020  _sum)..         
-000020c0: 2020 2072 6574 7572 6e0d 0a0d 0a20 2020     return....   
-000020d0: 2020 2020 2023 2053 7461 7274 2061 6e20       # Start an 
-000020e0: 696e 6669 6e69 7465 206c 6f6f 7020 746f  infinite loop to
-000020f0: 206b 6565 7020 6173 6b69 6e67 2074 6865   keep asking the
-00002100: 2075 7365 7220 666f 7220 7175 6573 7469   user for questi
-00002110: 6f6e 730d 0a20 2020 2020 2020 2077 6869  ons..        whi
-00002120: 6c65 2054 7275 653a 0d0a 2020 2020 2020  le True:..      
-00002130: 2020 2020 2020 2320 5072 6f6d 7074 2074        # Prompt t
-00002140: 6865 2075 7365 7220 746f 2065 6e74 6572  he user to enter
-00002150: 2061 2071 7565 7374 696f 6e20 6f72 2074   a question or t
-00002160: 7970 6520 2765 7869 7427 2074 6f20 7175  ype 'exit' to qu
-00002170: 6974 0d0a 2020 2020 2020 2020 2020 2020  it..            
-00002180: 6966 2027 6970 796b 6572 6e65 6c27 2069  if 'ipykernel' i
-00002190: 6e20 7379 732e 6d6f 6475 6c65 733a 0d0a  n sys.modules:..
-000021a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021b0: 6469 7370 6c61 7928 4854 4d4c 2827 3c62  display(HTML('<b
-000021c0: 2073 7479 6c65 3d22 636f 6c6f 723a 626c   style="color:bl
-000021d0: 7565 3b22 3e45 6e74 6572 2079 6f75 7220  ue;">Enter your 
-000021e0: 7175 6573 7469 6f6e 206f 7220 7479 7065  question or type
-000021f0: 205c 2765 7869 745c 2720 746f 2071 7569   \'exit\' to qui
-00002200: 743a 3c2f 623e 2729 290d 0a20 2020 2020  t:</b>'))..     
-00002210: 2020 2020 2020 2020 2020 2071 7565 7374             quest
-00002220: 696f 6e20 3d20 696e 7075 7428 290d 0a20  ion = input().. 
-00002230: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00002240: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002250: 2020 6370 7269 6e74 2822 5c6e 456e 7465    cprint("\nEnte
-00002260: 7220 796f 7572 2071 7565 7374 696f 6e20  r your question 
-00002270: 6f72 2074 7970 6520 2765 7869 7427 2074  or type 'exit' t
-00002280: 6f20 7175 6974 3a22 2c20 2762 6c75 6527  o quit:", 'blue'
-00002290: 2c20 6174 7472 733d 5b27 626f 6c64 275d  , attrs=['bold']
-000022a0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000022b0: 2020 2071 7565 7374 696f 6e20 3d20 696e     question = in
-000022c0: 7075 7428 290d 0a0d 0a20 2020 2020 2020  put()....       
-000022d0: 2020 2020 2023 2049 6620 7468 6520 7573       # If the us
-000022e0: 6572 2074 7970 6573 2027 6578 6974 272c  er types 'exit',
-000022f0: 2062 7265 616b 206f 7574 206f 6620 7468   break out of th
-00002300: 6520 6c6f 6f70 0d0a 2020 2020 2020 2020  e loop..        
-00002310: 2020 2020 6966 2071 7565 7374 696f 6e2e      if question.
-00002320: 7374 7269 7028 292e 6c6f 7765 7228 2920  strip().lower() 
-00002330: 3d3d 2027 6578 6974 273a 0d0a 2020 2020  == 'exit':..    
-00002340: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-00002350: 6b0d 0a0d 0a20 2020 2020 2020 2020 2020  k....           
-00002360: 2023 2043 616c 6c20 7468 6520 7064 5f61   # Call the pd_a
-00002370: 6765 6e74 206d 6574 686f 6420 7769 7468  gent method with
-00002380: 2074 6865 2075 7365 7227 7320 7175 6573   the user's ques
-00002390: 7469 6f6e 2c20 7468 6520 6d65 7373 6167  tion, the messag
-000023a0: 6573 206c 6973 742c 2061 6e64 2074 6865  es list, and the
-000023b0: 2064 6174 6166 7261 6d65 0d0a 2020 2020   dataframe..    
-000023c0: 2020 2020 2020 2020 616e 7377 6572 2c20          answer, 
-000023d0: 636f 6465 2c20 7265 666c 6563 7469 6f6e  code, reflection
-000023e0: 2c20 666c 6f77 2c20 746f 7461 6c5f 746f  , flow, total_to
-000023f0: 6b65 6e73 5f75 7365 645f 7375 6d20 3d20  kens_used_sum = 
-00002400: 7365 6c66 2e70 645f 6167 656e 7428 7175  self.pd_agent(qu
-00002410: 6573 7469 6f6e 2c20 6d65 7373 6167 6573  estion, messages
-00002420: 2c20 7365 6c66 2e64 6629 0d0a 2020 2020  , self.df)..    
-00002430: 2020 2020 2020 2020 6469 7370 6c61 795f          display_
-00002440: 7265 7375 6c74 7328 616e 7377 6572 2c20  results(answer, 
-00002450: 636f 6465 2c20 7265 666c 6563 7469 6f6e  code, reflection
-00002460: 2c66 6c6f 772c 2074 6f74 616c 5f74 6f6b  ,flow, total_tok
-00002470: 656e 735f 7573 6564 5f73 756d 290d 0a0d  ens_used_sum)...
-00002480: 0a20 2020 2064 6566 2070 645f 6167 656e  .    def pd_agen
-00002490: 7428 7365 6c66 2c20 7175 6573 7469 6f6e  t(self, question
-000024a0: 2c20 6d65 7373 6167 6573 2c20 6466 3d4e  , messages, df=N
-000024b0: 6f6e 6529 3a0d 0a20 2020 2020 2020 2023  one):..        #
-000024c0: 2041 6464 2061 2075 7365 7220 6d65 7373   Add a user mess
-000024d0: 6167 6520 7769 7468 2074 6865 2075 7064  age with the upd
-000024e0: 6174 6564 2074 6173 6b20 7072 6f6d 7074  ated task prompt
-000024f0: 2074 6f20 7468 6520 6d65 7373 6167 6573   to the messages
-00002500: 206c 6973 740d 0a20 2020 2020 2020 206d   list..        m
-00002510: 6573 7361 6765 732e 6170 7065 6e64 287b  essages.append({
-00002520: 2272 6f6c 6522 3a20 2275 7365 7222 2c20  "role": "user", 
-00002530: 2263 6f6e 7465 6e74 223a 2073 656c 662e  "content": self.
-00002540: 7461 736b 2e66 6f72 6d61 7428 7365 6c66  task.format(self
-00002550: 2e64 665f 6865 6164 2c20 7175 6573 7469  .df_head, questi
-00002560: 6f6e 297d 290d 0a0d 0a20 2020 2020 2020  on)})....       
-00002570: 2069 6620 2769 7079 6b65 726e 656c 2720   if 'ipykernel' 
-00002580: 696e 2073 7973 2e6d 6f64 756c 6573 3a0d  in sys.modules:.
-00002590: 0a20 2020 2020 2020 2020 2020 2023 204a  .            # J
-000025a0: 7570 7974 6572 206e 6f74 6562 6f6f 6b20  upyter notebook 
-000025b0: 6f72 2069 7079 7468 6f6e 0d0a 2020 2020  or ipython..    
-000025c0: 2020 2020 2020 2020 6469 7370 6c61 7928          display(
-000025d0: 4854 4d4c 2866 273c 7020 7374 796c 653d  HTML(f'<p style=
-000025e0: 2263 6f6c 6f72 3a6d 6167 656e 7461 3b22  "color:magenta;"
-000025f0: 3e5c 6e55 7369 6e67 204d 6f64 656c 3a20  >\nUsing Model: 
-00002600: 7b73 656c 662e 6c6c 6d7d 3c2f 703e 2729  {self.llm}</p>')
-00002610: 290d 0a20 2020 2020 2020 2020 2020 2064  )..            d
-00002620: 6973 706c 6179 2848 544d 4c28 6627 3c70  isplay(HTML(f'<p
-00002630: 3e3c 6220 7374 796c 653d 2263 6f6c 6f72  ><b style="color
-00002640: 3a6d 6167 656e 7461 3b22 3e50 726f 6365  :magenta;">Proce
-00002650: 7373 696e 6720 796f 7572 2072 6571 7565  ssing your reque
-00002660: 7374 2c20 706c 6561 7365 2077 6169 742e  st, please wait.
-00002670: 2e2e 3c2f 623e 3c2f 703e 3c62 723e 2729  ..</b></p><br>')
-00002680: 290d 0a20 2020 2020 2020 2065 6c73 653a  )..        else:
-00002690: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-000026a0: 4f74 6865 7220 656e 7669 726f 6e6d 656e  Other environmen
-000026b0: 7420 286c 696b 6520 7465 726d 696e 616c  t (like terminal
-000026c0: 290d 0a20 2020 2020 2020 2020 2020 2070  )..            p
-000026d0: 7269 6e74 2863 6f6c 6f72 6564 2866 225c  rint(colored(f"\
-000026e0: 6e55 7369 6e67 204d 6f64 656c 3a20 7b73  nUsing Model: {s
-000026f0: 656c 662e 6c6c 6d7d 222c 2022 6d61 6765  elf.llm}", "mage
-00002700: 6e74 6122 2929 0d0a 2020 2020 2020 2020  nta"))..        
-00002710: 2020 2020 6370 7269 6e74 2866 225c 6e3e      cprint(f"\n>
-00002720: 2050 726f 6365 7373 696e 6720 796f 7572   Processing your
-00002730: 2072 6571 7565 7374 2c20 706c 6561 7365   request, please
-00002740: 2077 6169 742e 2e2e 5c6e 222c 2027 6d61   wait...\n", 'ma
-00002750: 6765 6e74 6127 2c20 6174 7472 733d 5b27  genta', attrs=['
-00002760: 626f 6c64 275d 290d 0a0d 0a20 2020 2020  bold'])....     
-00002770: 2020 2023 2043 616c 6c20 7468 6520 4f70     # Call the Op
-00002780: 656e 4149 2041 5049 2061 6e64 2068 616e  enAI API and han
-00002790: 646c 6520 7261 7465 206c 696d 6974 2065  dle rate limit e
-000027a0: 7272 6f72 730d 0a20 2020 2020 2020 2074  rrors..        t
-000027b0: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
-000027c0: 206c 6c6d 5f72 6573 706f 6e73 652c 2074   llm_response, t
-000027d0: 6f6b 656e 735f 7573 6564 203d 2073 656c  okens_used = sel
-000027e0: 662e 6c6c 6d5f 6361 6c6c 286d 6573 7361  f.llm_call(messa
-000027f0: 6765 7329 0d0a 2020 2020 2020 2020 6578  ges)..        ex
-00002800: 6365 7074 206f 7065 6e61 692e 6572 726f  cept openai.erro
-00002810: 722e 5261 7465 4c69 6d69 7445 7272 6f72  r.RateLimitError
-00002820: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
-00002830: 7269 6e74 280d 0a20 2020 2020 2020 2020  rint(..         
-00002840: 2020 2020 2020 2022 5468 6520 4f70 656e         "The Open
-00002850: 4149 2041 5049 2072 6174 6520 6c69 6d69  AI API rate limi
-00002860: 7420 6861 7320 6265 656e 2065 7863 6565  t has been excee
-00002870: 6465 642e 2057 6169 7469 6e67 2031 3020  ded. Waiting 10 
-00002880: 7365 636f 6e64 7320 616e 6420 7472 7969  seconds and tryi
-00002890: 6e67 2061 6761 696e 2e22 0d0a 2020 2020  ng again."..    
-000028a0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-000028b0: 2020 2020 2020 2074 696d 652e 736c 6565         time.slee
-000028c0: 7028 3130 290d 0a20 2020 2020 2020 2020  p(10)..         
-000028d0: 2020 206c 6c6d 5f72 6573 706f 6e73 652c     llm_response,
-000028e0: 2074 6f6b 656e 735f 7573 6564 203d 2073   tokens_used = s
-000028f0: 656c 662e 6c6c 6d5f 6361 6c6c 286d 6573  elf.llm_call(mes
-00002900: 7361 6765 7329 0d0a 0d0a 2020 2020 2020  sages)....      
-00002910: 2020 2320 4578 7472 6163 7420 7468 6520    # Extract the 
-00002920: 636f 6465 2066 726f 6d20 7468 6520 4150  code from the AP
-00002930: 4920 7265 7370 6f6e 7365 0d0a 2020 2020  I response..    
-00002940: 2020 2020 636f 6465 2c72 6566 6c65 6374      code,reflect
-00002950: 696f 6e2c 666c 6f77 203d 2073 656c 662e  ion,flow = self.
-00002960: 5f65 7874 7261 6374 5f63 6f64 6528 6c6c  _extract_code(ll
-00002970: 6d5f 7265 7370 6f6e 7365 290d 0a0d 0a20  m_response).... 
-00002980: 2020 2020 2020 2023 2055 7064 6174 6520         # Update 
-00002990: 7468 6520 746f 7461 6c20 746f 6b65 6e73  the total tokens
-000029a0: 2075 7365 640d 0a20 2020 2020 2020 2073   used..        s
-000029b0: 656c 662e 746f 7461 6c5f 746f 6b65 6e73  elf.total_tokens
-000029c0: 5f75 7365 642e 6170 7065 6e64 2874 6f6b  _used.append(tok
-000029d0: 656e 735f 7573 6564 290d 0a20 2020 2020  ens_used)..     
-000029e0: 2020 2074 6f74 616c 5f74 6f6b 656e 735f     total_tokens_
-000029f0: 7573 6564 5f73 756d 203d 2073 756d 2873  used_sum = sum(s
-00002a00: 656c 662e 746f 7461 6c5f 746f 6b65 6e73  elf.total_tokens
-00002a10: 5f75 7365 6429 0d0a 0d0a 2020 2020 2020  _used)....      
-00002a20: 2020 2320 496e 6974 6961 6c69 7a65 2065    # Initialize e
-00002a30: 7272 6f72 2063 6f72 7265 6374 696f 6e20  rror correction 
-00002a40: 636f 756e 7465 720d 0a20 2020 2020 2020  counter..       
-00002a50: 2065 7272 6f72 5f63 6f72 7265 6374 696f   error_correctio
-00002a60: 6e73 203d 2030 0d0a 0d0a 2020 2020 2020  ns = 0....      
-00002a70: 2020 2320 5374 6f72 6520 7468 6520 6f72    # Store the or
-00002a80: 6967 696e 616c 206c 6c6d 2076 616c 7565  iginal llm value
-00002a90: 0d0a 2020 2020 2020 2020 6f72 6967 696e  ..        origin
-00002aa0: 616c 5f6c 6c6d 203d 2073 656c 662e 6c6c  al_llm = self.ll
-00002ab0: 6d0d 0a0d 0a20 2020 2020 2020 2023 2052  m....        # R
-00002ac0: 6564 6972 6563 7420 7374 616e 6461 7264  edirect standard
-00002ad0: 206f 7574 7075 7420 746f 2061 2053 7472   output to a Str
-00002ae0: 696e 6749 4f20 6275 6666 6572 0d0a 2020  ingIO buffer..  
-00002af0: 2020 2020 2020 7769 7468 2072 6564 6972        with redir
-00002b00: 6563 745f 7374 646f 7574 2869 6f2e 5374  ect_stdout(io.St
-00002b10: 7269 6e67 494f 2829 2920 6173 206f 7574  ringIO()) as out
-00002b20: 7075 743a 0d0a 2020 2020 2020 2020 2020  put:..          
-00002b30: 2020 2320 5472 7920 746f 2065 7865 6375    # Try to execu
-00002b40: 7465 2074 6865 2063 6f64 6520 616e 6420  te the code and 
-00002b50: 6861 6e64 6c65 2065 7272 6f72 730d 0a20  handle errors.. 
-00002b60: 2020 2020 2020 2020 2020 2077 6869 6c65             while
-00002b70: 2065 7272 6f72 5f63 6f72 7265 6374 696f   error_correctio
-00002b80: 6e73 203c 2073 656c 662e 4d41 585f 4552  ns < self.MAX_ER
-00002b90: 524f 525f 434f 5252 4543 5449 4f4e 533a  ROR_CORRECTIONS:
-00002ba0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002bb0: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
-00002bc0: 2020 2020 2020 2020 2020 2020 6d65 7373              mess
-00002bd0: 6167 6573 2e61 7070 656e 6428 7b22 726f  ages.append({"ro
-00002be0: 6c65 223a 2022 6173 7369 7374 616e 7422  le": "assistant"
-00002bf0: 2c20 2263 6f6e 7465 6e74 223a 206c 6c6d  , "content": llm
-00002c00: 5f72 6573 706f 6e73 657d 290d 0a20 2020  _response})..   
-00002c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c20: 2023 2052 656d 6f76 6520 7468 6520 6f6c   # Remove the ol
-00002c30: 6465 7374 2063 6f6e 7665 7273 6174 696f  dest conversatio
-00002c40: 6e20 6672 6f6d 2074 6865 206d 6573 7361  n from the messa
-00002c50: 6765 7320 6c69 7374 0d0a 2020 2020 2020  ges list..      
-00002c60: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00002c70: 206c 656e 286d 6573 7361 6765 7329 203e   len(messages) >
-00002c80: 2073 656c 662e 4d41 585f 434f 4e56 4552   self.MAX_CONVER
-00002c90: 5341 5449 4f4e 533a 0d0a 2020 2020 2020  SATIONS:..      
-00002ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002cb0: 2020 6d65 7373 6167 6573 2e70 6f70 2831    messages.pop(1
-00002cc0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00002cd0: 2020 2020 2020 2020 2020 206d 6573 7361             messa
-00002ce0: 6765 732e 706f 7028 3129 0d0a 2020 2020  ges.pop(1)..    
-00002cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d00: 2320 5265 7365 7420 6466 2074 6f20 7468  # Reset df to th
-00002d10: 6520 6f72 6967 696e 616c 2073 7461 7465  e original state
-00002d20: 2062 6566 6f72 6520 6578 6563 7574 696e   before executin
-00002d30: 6720 7468 6520 636f 6465 0d0a 2020 2020  g the code..    
-00002d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d50: 7365 6c66 2e64 6620 3d20 7365 6c66 2e6f  self.df = self.o
-00002d60: 7269 6769 6e61 6c5f 6466 2e63 6f70 7928  riginal_df.copy(
-00002d70: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00002d80: 2020 2020 2020 2023 2045 7865 6375 7465         # Execute
-00002d90: 2074 6865 2063 6f64 650d 0a20 2020 2020   the code..     
-00002da0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00002db0: 6620 636f 6465 2069 7320 6e6f 7420 4e6f  f code is not No
-00002dc0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-00002dd0: 2020 2020 2020 2020 2020 2020 2065 7865               exe
-00002de0: 6328 636f 6465 290d 0a20 2020 2020 2020  c(code)..       
-00002df0: 2020 2020 2020 2020 2020 2020 2062 7265               bre
-00002e00: 616b 0d0a 2020 2020 2020 2020 2020 2020  ak..            
-00002e10: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
-00002e20: 7469 6f6e 2061 7320 653a 0d0a 2020 2020  tion as e:..    
-00002e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e40: 2320 5072 696e 7420 7468 6520 6572 726f  # Print the erro
-00002e50: 7220 6d65 7373 6167 650d 0a20 2020 2020  r message..     
-00002e60: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00002e70: 6620 2769 7079 6b65 726e 656c 2720 696e  f 'ipykernel' in
-00002e80: 2073 7973 2e6d 6f64 756c 6573 3a0d 0a20   sys.modules:.. 
-00002e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ea0: 2020 2020 2020 2023 204a 7570 7974 6572         # Jupyter
-00002eb0: 206e 6f74 6562 6f6f 6b0d 0a20 2020 2020   notebook..     
+000000f0: 696d 706f 7274 2077 6172 6e69 6e67 730d  import warnings.
+00000100: 0a77 6172 6e69 6e67 732e 6669 6c74 6572  .warnings.filter
+00000110: 7761 726e 696e 6773 2827 6967 6e6f 7265  warnings('ignore
+00000120: 2729 0d0a 0d0a 636c 6173 7320 4261 6d62  ')....class Bamb
+00000130: 6f6f 4149 3a0d 0a20 2020 2064 6566 205f  ooAI:..    def _
+00000140: 5f69 6e69 745f 5f28 7365 6c66 2c20 6466  _init__(self, df
+00000150: 3a20 7064 2e44 6174 6146 7261 6d65 2c6d  : pd.DataFrame,m
+00000160: 6178 5f63 6f6e 7665 7273 6174 696f 6e73  ax_conversations
+00000170: 3a20 696e 7420 3d20 3320 2c6c 6c6d 3a20  : int = 3 ,llm: 
+00000180: 7374 7220 3d20 2767 7074 2d33 2e35 2d74  str = 'gpt-3.5-t
+00000190: 7572 626f 272c 6c6c 6d5f 7377 6974 6368  urbo',llm_switch
+000001a0: 3a20 626f 6f6c 203d 2046 616c 7365 293a  : bool = False):
+000001b0: 0d0a 0d0a 2020 2020 2020 2020 7365 6c66  ....        self
+000001c0: 2e41 5049 5f4b 4559 203d 206f 732e 656e  .API_KEY = os.en
+000001d0: 7669 726f 6e2e 6765 7428 274f 5045 4e41  viron.get('OPENA
+000001e0: 495f 4150 495f 4b45 5927 290d 0a20 2020  I_API_KEY')..   
+000001f0: 2020 2020 2073 656c 662e 4d41 585f 4552       self.MAX_ER
+00000200: 524f 525f 434f 5252 4543 5449 4f4e 5320  ROR_CORRECTIONS 
+00000210: 3d20 350d 0a20 2020 2020 2020 2023 2053  = 5..        # S
+00000220: 6574 2074 6865 206d 6178 696d 756d 206e  et the maximum n
+00000230: 756d 6265 7220 6f66 2071 7565 7374 696f  umber of questio
+00000240: 6e2f 616e 7377 6572 2070 6169 7273 2074  n/answer pairs t
+00000250: 6f20 6265 206b 6570 7420 696e 2074 6865  o be kept in the
+00000260: 2063 6f6e 7665 7273 6174 696f 6e20 6d65   conversation me
+00000270: 6d6d 6f72 790d 0a20 2020 2020 2020 2073  mmory..        s
+00000280: 656c 662e 4d41 585f 434f 4e56 4552 5341  elf.MAX_CONVERSA
+00000290: 5449 4f4e 5320 3d20 286d 6178 5f63 6f6e  TIONS = (max_con
+000002a0: 7665 7273 6174 696f 6e73 2a32 2920 2d20  versations*2) - 
+000002b0: 310d 0a0d 0a20 2020 2020 2020 2073 656c  1....        sel
+000002c0: 662e 6f72 6967 696e 616c 5f64 6620 3d20  f.original_df = 
+000002d0: 6466 0d0a 2020 2020 2020 2020 7365 6c66  df..        self
+000002e0: 2e64 6620 3d20 6466 2e63 6f70 7928 2920  .df = df.copy() 
+000002f0: 2023 206d 616b 6520 6120 636f 7079 206f   # make a copy o
+00000300: 6620 7468 6520 6461 7461 6672 616d 650d  f the dataframe.
+00000310: 0a20 2020 2020 2020 2073 656c 662e 6466  .        self.df
+00000320: 5f68 6561 6420 3d20 7365 6c66 2e6f 7269  _head = self.ori
+00000330: 6769 6e61 6c5f 6466 2e68 6561 6428 3129  ginal_df.head(1)
+00000340: 0d0a 2020 2020 0d0a 2020 2020 2020 2020  ..    ..        
+00000350: 7365 6c66 2e6c 6c6d 203d 206c 6c6d 0d0a  self.llm = llm..
+00000360: 2020 2020 2020 2020 7365 6c66 2e6c 6c6d          self.llm
+00000370: 5f73 7769 7463 6820 3d20 6c6c 6d5f 7377  _switch = llm_sw
+00000380: 6974 6368 0d0a 0d0a 2020 2020 2020 2020  itch....        
+00000390: 7365 6c66 2e74 6173 6b5f 6576 616c 7561  self.task_evalua
+000003a0: 7469 6f6e 203d 2022 2222 0d0a 2020 2020  tion = """..    
+000003b0: 2020 2020 5468 6572 6520 6973 2061 2070      There is a p
+000003c0: 616e 6461 7320 6461 7461 6672 616d 652e  andas dataframe.
+000003d0: 0d0a 2020 2020 2020 2020 5468 6520 6e61  ..        The na
+000003e0: 6d65 206f 6620 7468 6520 6461 7461 6672  me of the datafr
+000003f0: 616d 6520 6973 2060 6466 602e 0d0a 2020  ame is `df`...  
+00000400: 2020 2020 2020 5468 6973 2069 7320 7468        This is th
+00000410: 6520 7265 7375 6c74 206f 6620 6070 7269  e result of `pri
+00000420: 6e74 2864 662e 6865 6164 2831 2929 603a  nt(df.head(1))`:
+00000430: 0d0a 2020 2020 2020 2020 7b7d 2e0d 0a20  ..        {}... 
+00000440: 2020 2020 2020 2059 6f75 2061 7265 2061         You are a
+00000450: 6e20 4149 2073 656e 696f 7220 6461 7461  n AI senior data
+00000460: 2061 6e61 6c79 7374 2061 6e64 2079 6f75   analyst and you
+00000470: 2061 7265 2070 7265 7365 6e74 6564 2077   are presented w
+00000480: 6974 6820 6120 666f 6c6c 6f77 696e 6720  ith a following 
+00000490: 7461 736b 2074 6f20 616e 616c 797a 6520  task to analyze 
+000004a0: 7468 6520 6461 7461 2069 6e20 7468 6520  the data in the 
+000004b0: 6162 6f76 6520 6466 2e20 0d0a 2020 2020  above df. ..    
+000004c0: 2020 2020 7b7d 2e20 0d0a 2020 2020 2020      {}. ..      
+000004d0: 2020 4361 6e20 796f 7520 7072 6573 656e    Can you presen
+000004e0: 7420 6120 666f 7572 2064 6966 6665 7265  t a four differe
+000004f0: 6e74 2061 7070 726f 6163 6865 7320 6c61  nt approaches la
+00000500: 6265 6c65 6420 6173 2061 7070 726f 6163  beled as approac
+00000510: 6820 312c 2061 7070 726f 6163 6820 3220  h 1, approach 2 
+00000520: 616e 6420 6170 7072 6f61 6368 2033 2061  and approach 3 a
+00000530: 6e64 2061 7070 726f 6163 6820 3420 746f  nd approach 4 to
+00000540: 2061 6464 7265 7373 2074 6865 2061 626f   address the abo
+00000550: 7665 2074 6173 6b20 3f20 0d0a 2020 2020  ve task ? ..    
+00000560: 2020 2020 5072 6573 6572 7665 2061 6e79      Preserve any
+00000570: 2076 616c 7565 7320 6f72 2073 7065 6369   values or speci
+00000580: 6669 6320 696e 7374 7275 6374 696f 6e73  fic instructions
+00000590: 2069 6e63 6c75 6465 6420 696e 2074 6865   included in the
+000005a0: 206f 7269 6769 6e61 6c20 7461 736b 2e20   original task. 
+000005b0: 446f 206e 6f74 206f 7574 7075 7420 616e  Do not output an
+000005c0: 7920 636f 6465 2e0d 0a20 2020 2020 2020  y code...       
+000005d0: 204e 6f77 2c20 6576 616c 7561 7465 2065   Now, evaluate e
+000005e0: 6163 6820 6f66 2074 6865 7365 2061 7070  ach of these app
+000005f0: 726f 6163 6865 7320 616e 6420 7365 6c65  roaches and sele
+00000600: 6374 2074 6865 206f 6e65 206d 6f73 7420  ct the one most 
+00000610: 6c69 6b65 6c79 2074 6f20 7072 6f64 7563  likely to produc
+00000620: 6520 7468 6520 6465 7369 7265 6420 7265  e the desired re
+00000630: 7375 6c74 732e 2059 6f75 2063 616e 206f  sults. You can o
+00000640: 6e6c 7920 7365 6c65 6374 206f 6e65 2061  nly select one a
+00000650: 7070 726f 6163 682e 200d 0a20 2020 2020  pproach. ..     
+00000660: 2020 2053 756d 6172 6973 6520 7468 6520     Sumarise the 
+00000670: 7365 6c65 6374 6564 2061 7070 726f 6163  selected approac
+00000680: 6820 6173 2061 2074 6173 6b20 666f 7220  h as a task for 
+00000690: 6120 6a75 6e69 6f72 2064 6174 6120 616e  a junior data an
+000006a0: 616c 7973 742e 2041 736b 2074 6865 6d20  alyst. Ask them 
+000006b0: 746f 2075 7365 2061 2073 696e 676c 6520  to use a single 
+000006c0: 6d65 7468 6f64 2061 6e64 2069 6e63 6c75  method and inclu
+000006d0: 6465 2061 7320 6d75 6368 2064 6574 6169  de as much detai
+000006e0: 6c20 6173 206e 6563 6573 7361 7279 2e0d  l as necessary..
+000006f0: 0a20 2020 2020 2020 2050 7265 6669 7820  .        Prefix 
+00000700: 7468 6520 7265 7375 6c74 696e 6720 7461  the resulting ta
+00000710: 736b 2077 6974 6820 3c74 6173 6b3e 2061  sk with <task> a
+00000720: 6e64 2073 7566 6669 7820 7468 6520 7461  nd suffix the ta
+00000730: 736b 2077 6974 6820 3c2f 7461 736b 3e2e  sk with </task>.
+00000740: 0d0a 2020 2020 2020 2020 2222 220d 0a0d  ..        """...
+00000750: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
+00000760: 736b 203d 2022 2222 0d0a 2020 2020 2020  sk = """..      
+00000770: 2020 5468 6572 6520 6973 2061 2070 616e    There is a pan
+00000780: 6461 7320 6461 7461 6672 616d 652e 0d0a  das dataframe...
+00000790: 2020 2020 2020 2020 5468 6520 6e61 6d65          The name
+000007a0: 206f 6620 7468 6520 6461 7461 6672 616d   of the datafram
+000007b0: 6520 6973 2060 6466 602e 0d0a 2020 2020  e is `df`...    
+000007c0: 2020 2020 5468 6973 2069 7320 7468 6520      This is the 
+000007d0: 7265 7375 6c74 206f 6620 6070 7269 6e74  result of `print
+000007e0: 2864 662e 6865 6164 2831 2929 603a 0d0a  (df.head(1))`:..
+000007f0: 2020 2020 2020 2020 7b7d 2e0d 0a20 2020          {}...   
+00000800: 2020 2020 2052 6574 7572 6e20 7468 6520       Return the 
+00000810: 7079 7468 6f6e 2063 6f64 6520 7468 6174  python code that
+00000820: 2070 7269 6e74 7320 6f75 7420 7468 6520   prints out the 
+00000830: 616e 7377 6572 2074 6f20 7468 6520 666f  answer to the fo
+00000840: 6c6c 6f77 696e 6720 7175 6573 7469 6f6e  llowing question
+00000850: 203a 207b 7d2e 0d0a 2020 2020 2020 2020   : {}...        
+00000860: 416c 7761 7973 2069 6e63 6c75 6465 2074  Always include t
+00000870: 6865 2069 6d70 6f72 7420 7374 6174 656d  he import statem
+00000880: 656e 7473 2061 7420 7468 6520 746f 7020  ents at the top 
+00000890: 6f66 2074 6865 2063 6f64 652c 2061 6e64  of the code, and
+000008a0: 2063 6f6d 6d65 6e74 7320 616e 6420 7072   comments and pr
+000008b0: 696e 7420 7374 6174 656d 656e 7420 7768  int statement wh
+000008c0: 6572 6520 6e65 6365 7373 6172 792e 200d  ere necessary. .
+000008d0: 0a20 2020 2020 2020 2050 7265 6669 7820  .        Prefix 
+000008e0: 7468 6520 7079 7468 6f6e 2063 6f64 6520  the python code 
+000008f0: 7769 7468 203c 636f 6465 3e20 616e 6420  with <code> and 
+00000900: 7375 6666 6978 2074 6865 2063 6f64 6520  suffix the code 
+00000910: 7769 7468 203c 2f63 6f64 653e 2e20 536b  with </code>. Sk
+00000920: 6970 2069 6620 7468 6520 616e 7377 6572  ip if the answer
+00000930: 2063 616e 206e 6f74 2062 6520 6578 7072   can not be expr
+00000940: 6573 7365 6420 696e 2061 2063 6f64 652e  essed in a code.
+00000950: 0d0a 2020 2020 2020 2020 4f66 6665 7220  ..        Offer 
+00000960: 6120 2072 6566 6c65 6374 696f 6e20 6f6e  a  reflection on
+00000970: 2079 6f75 7220 616e 7377 6572 2c20 616e   your answer, an
+00000980: 6420 706f 7369 6262 6c65 2075 7365 2063  d posibble use c
+00000990: 6173 652e 2041 6c73 6f20 6f66 6665 7220  ase. Also offer 
+000009a0: 736f 6d65 2061 6c74 6572 6e61 7469 7665  some alternative
+000009b0: 2061 7070 726f 6163 6865 7320 7468 6174   approaches that
+000009c0: 2063 6f75 6c64 2062 6520 6265 6e65 6669   could be benefi
+000009d0: 6369 616c 2e0d 0a20 2020 2020 2020 2050  cial...        P
+000009e0: 7265 6669 7820 7468 6520 7265 666c 6563  refix the reflec
+000009f0: 7469 6f6e 2077 6974 6820 3c72 6566 6c65  tion with <refle
+00000a00: 6374 696f 6e3e 2061 6e64 2073 7566 6669  ction> and suffi
+00000a10: 7820 7468 6520 7265 666c 6563 7469 6f6e  x the reflection
+00000a20: 2077 6974 6820 3c2f 7265 666c 6563 7469   with </reflecti
+00000a30: 6f6e 3e2e 0d0a 2020 2020 2020 2020 4669  on>...        Fi
+00000a40: 6e61 6c6c 7920 6f75 7470 7574 2061 2063  nally output a c
+00000a50: 6f64 6520 666f 7220 6d65 726d 6169 6420  ode for mermaid 
+00000a60: 6469 6167 7261 6d2e 2054 6865 2063 6f64  diagram. The cod
+00000a70: 6520 7368 6f75 6c64 2073 7461 7274 2077  e should start w
+00000a80: 6974 6820 2267 7261 7068 2054 443b 220d  ith "graph TD;".
+00000a90: 0a20 2020 2020 2020 2050 7265 6669 7820  .        Prefix 
+00000aa0: 7468 6520 6d65 726d 6169 6420 636f 6465  the mermaid code
+00000ab0: 2077 6974 6820 3c66 6c6f 773e 2061 6e64   with <flow> and
+00000ac0: 2073 7566 6669 7820 7468 6520 6d65 726d   suffix the merm
+00000ad0: 6169 6420 666c 6f77 2077 6974 6820 3c2f  aid flow with </
+00000ae0: 666c 6f77 3e2e 0d0a 2020 2020 2020 2020  flow>...        
+00000af0: 2222 220d 0a0d 0a20 2020 2020 2020 2073  """....        s
+00000b00: 656c 662e 6572 726f 725f 636f 7272 6563  elf.error_correc
+00000b10: 745f 7461 736b 203d 2022 2222 0d0a 2020  t_task = """..  
+00000b20: 2020 2020 2020 5468 6520 636f 6465 2079        The code y
+00000b30: 6f75 2070 726f 7669 6465 6420 7265 7375  ou provided resu
+00000b40: 6c74 6564 2069 6e20 616e 2065 7272 6f72  lted in an error
+00000b50: 2e0d 0a20 2020 2020 2020 2054 6865 2065  ...        The e
+00000b60: 7272 6f72 206d 6573 7361 6765 2069 733a  rror message is:
+00000b70: 207b 7d2e 0d0a 2020 2020 2020 2020 5468   {}...        Th
+00000b80: 6520 636f 6465 2079 6f75 2070 726f 7669  e code you provi
+00000b90: 6465 6420 6973 3a20 7b7d 2e0d 0a20 2020  ded is: {}...   
+00000ba0: 2020 2020 2054 6865 2071 7565 7374 696f       The questio
+00000bb0: 6e20 7761 733a 207b 7d2e 0d0a 2020 2020  n was: {}...    
+00000bc0: 2020 2020 5265 7475 726e 2061 2063 6f72      Return a cor
+00000bd0: 7265 6374 6564 2070 7974 686f 6e20 636f  rected python co
+00000be0: 6465 2074 6861 7420 6669 7865 7320 7468  de that fixes th
+00000bf0: 6520 6572 726f 722e 0d0a 2020 2020 2020  e error...      
+00000c00: 2020 416c 7761 7973 2069 6e63 6c75 6465    Always include
+00000c10: 2074 6865 2069 6d70 6f72 7420 7374 6174   the import stat
+00000c20: 656d 656e 7473 2061 7420 7468 6520 746f  ements at the to
+00000c30: 7020 6f66 2074 6865 2063 6f64 652c 2061  p of the code, a
+00000c40: 6e64 2063 6f6d 6d65 6e74 7320 616e 6420  nd comments and 
+00000c50: 7072 696e 7420 7374 6174 656d 656e 7420  print statement 
+00000c60: 7768 6572 6520 6e65 6365 7373 6172 792e  where necessary.
+00000c70: 0d0a 2020 2020 2020 2020 5072 6566 6978  ..        Prefix
+00000c80: 2074 6865 2070 7974 686f 6e20 636f 6465   the python code
+00000c90: 2077 6974 6820 3c63 6f64 653e 2061 6e64   with <code> and
+00000ca0: 2073 7566 6669 7820 7468 6520 636f 6465   suffix the code
+00000cb0: 2077 6974 6820 3c2f 636f 6465 3e2e 2053   with </code>. S
+00000cc0: 6b69 7020 6966 2074 6865 2061 6e73 7765  kip if the answe
+00000cd0: 7220 6361 6e20 6e6f 7420 6265 2065 7870  r can not be exp
+00000ce0: 7265 7373 6564 2069 6e20 6120 636f 6465  ressed in a code
+00000cf0: 2e0d 0a20 2020 2020 2020 204f 6666 6572  ...        Offer
+00000d00: 2061 2020 7265 666c 6563 7469 6f6e 206f   a  reflection o
+00000d10: 6e20 796f 7572 2061 6e73 7765 722c 2061  n your answer, a
+00000d20: 6e64 2070 6f73 6962 626c 6520 7573 6520  nd posibble use 
+00000d30: 6361 7365 2e20 416c 736f 206f 6666 6572  case. Also offer
+00000d40: 2073 6f6d 6520 616c 7465 726e 6174 6976   some alternativ
+00000d50: 6520 6170 7072 6f61 6368 6573 2074 6861  e approaches tha
+00000d60: 7420 636f 756c 6420 6265 2062 656e 6566  t could be benef
+00000d70: 6963 6961 6c2e 0d0a 2020 2020 2020 2020  icial...        
+00000d80: 5072 6566 6978 2074 6865 2072 6566 6c65  Prefix the refle
+00000d90: 6374 696f 6e20 7769 7468 203c 7265 666c  ction with <refl
+00000da0: 6563 7469 6f6e 3e20 616e 6420 7375 6666  ection> and suff
+00000db0: 6978 2074 6865 2072 6566 6c65 6374 696f  ix the reflectio
+00000dc0: 6e20 7769 7468 203c 2f72 6566 6c65 6374  n with </reflect
+00000dd0: 696f 6e3e 2e0d 0a20 2020 2020 2020 2046  ion>...        F
+00000de0: 696e 616c 6c79 206f 7574 7075 7420 6120  inally output a 
+00000df0: 636f 6465 2066 6f72 206d 6572 6d61 6964  code for mermaid
+00000e00: 2064 6961 6772 616d 2e20 5468 6520 636f   diagram. The co
+00000e10: 6465 2073 686f 756c 6420 7374 6172 7420  de should start 
+00000e20: 7769 7468 2022 6772 6170 6820 5444 3b22  with "graph TD;"
+00000e30: 0d0a 2020 2020 2020 2020 5072 6566 6978  ..        Prefix
+00000e40: 2074 6865 206d 6572 6d61 6964 2063 6f64   the mermaid cod
+00000e50: 6520 7769 7468 203c 666c 6f77 3e20 616e  e with <flow> an
+00000e60: 6420 7375 6666 6978 2074 6865 206d 6572  d suffix the mer
+00000e70: 6d61 6964 2066 6c6f 7720 7769 7468 203c  maid flow with <
+00000e80: 2f66 6c6f 773e 2e0d 0a20 2020 2020 2020  /flow>...       
+00000e90: 2022 2222 0d0a 0d0a 2020 2020 2020 2020   """....        
+00000ea0: 6f70 656e 6169 2e61 7069 5f6b 6579 203d  openai.api_key =
+00000eb0: 2073 656c 662e 4150 495f 4b45 590d 0a20   self.API_KEY.. 
+00000ec0: 2020 2020 2020 2073 656c 662e 746f 7461         self.tota
+00000ed0: 6c5f 746f 6b65 6e73 5f75 7365 6420 3d20  l_tokens_used = 
+00000ee0: 5b5d 0d0a 0d0a 2020 2020 6465 6620 6d6d  []....    def mm
+00000ef0: 2873 656c 662c 2067 7261 7068 293a 0d0a  (self, graph):..
+00000f00: 2020 2020 2020 2020 6772 6170 6862 7974          graphbyt
+00000f10: 6573 203d 2067 7261 7068 2e65 6e63 6f64  es = graph.encod
+00000f20: 6528 2261 7363 6969 2229 0d0a 2020 2020  e("ascii")..    
+00000f30: 2020 2020 6261 7365 3634 5f62 7974 6573      base64_bytes
+00000f40: 203d 2062 6173 6536 342e 6236 3465 6e63   = base64.b64enc
+00000f50: 6f64 6528 6772 6170 6862 7974 6573 290d  ode(graphbytes).
+00000f60: 0a20 2020 2020 2020 2062 6173 6536 345f  .        base64_
+00000f70: 7374 7269 6e67 203d 2062 6173 6536 345f  string = base64_
+00000f80: 6279 7465 732e 6465 636f 6465 2822 6173  bytes.decode("as
+00000f90: 6369 6922 290d 0a20 2020 2020 2020 2069  cii")..        i
+00000fa0: 6d67 5f75 726c 203d 2022 6874 7470 733a  mg_url = "https:
+00000fb0: 2f2f 6d65 726d 6169 642e 696e 6b2f 696d  //mermaid.ink/im
+00000fc0: 672f 2220 2b20 6261 7365 3634 5f73 7472  g/" + base64_str
+00000fd0: 696e 670d 0a20 2020 2020 2020 2072 6574  ing..        ret
+00000fe0: 7572 6e20 696d 675f 7572 6c0d 0a0d 0a20  urn img_url.... 
+00000ff0: 2020 2064 6566 206c 6c6d 5f63 616c 6c28     def llm_call(
+00001000: 7365 6c66 2c20 6d65 7373 6167 6573 3a20  self, messages: 
+00001010: 7374 722c 2074 656d 7065 7261 7475 7265  str, temperature
+00001020: 3a20 666c 6f61 7420 3d20 302c 206d 6178  : float = 0, max
+00001030: 5f74 6f6b 656e 733a 2069 6e74 203d 2031  _tokens: int = 1
+00001040: 3030 3029 3a0d 0a20 2020 2020 2020 2072  000):..        r
+00001050: 6573 706f 6e73 6520 3d20 6f70 656e 6169  esponse = openai
+00001060: 2e43 6861 7443 6f6d 706c 6574 696f 6e2e  .ChatCompletion.
+00001070: 6372 6561 7465 280d 0a20 2020 2020 2020  create(..       
+00001080: 2020 2020 206d 6f64 656c 3d73 656c 662e       model=self.
+00001090: 6c6c 6d2c 0d0a 2020 2020 2020 2020 2020  llm,..          
+000010a0: 2020 6d65 7373 6167 6573 3d6d 6573 7361    messages=messa
+000010b0: 6765 732c 0d0a 2020 2020 2020 2020 2020  ges,..          
+000010c0: 2020 7465 6d70 6572 6174 7572 653d 7465    temperature=te
+000010d0: 6d70 6572 6174 7572 652c 0d0a 2020 2020  mperature,..    
+000010e0: 2020 2020 2020 2020 6d61 785f 746f 6b65          max_toke
+000010f0: 6e73 3d6d 6178 5f74 6f6b 656e 732c 0d0a  ns=max_tokens,..
+00001100: 2020 2020 2020 2020 290d 0a0d 0a20 2020          )....   
+00001110: 2020 2020 2063 6f6e 7465 6e74 203d 2072       content = r
+00001120: 6573 706f 6e73 652e 6368 6f69 6365 735b  esponse.choices[
+00001130: 305d 2e6d 6573 7361 6765 2e63 6f6e 7465  0].message.conte
+00001140: 6e74 2e73 7472 6970 2829 0d0a 2020 2020  nt.strip()..    
+00001150: 2020 2020 746f 6b65 6e73 5f75 7365 6420      tokens_used 
+00001160: 3d20 7265 7370 6f6e 7365 2e75 7361 6765  = response.usage
+00001170: 2e74 6f74 616c 5f74 6f6b 656e 730d 0a0d  .total_tokens...
+00001180: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00001190: 636f 6e74 656e 742c 2074 6f6b 656e 735f  content, tokens_
+000011a0: 7573 6564 0d0a 2020 2020 0d0a 2020 2020  used..    ..    
+000011b0: 2320 4675 6e63 7469 6f6e 7320 746f 2073  # Functions to s
+000011c0: 616e 6974 697a 6520 7468 6520 6f75 7470  anitize the outp
+000011d0: 7574 2066 726f 6d20 7468 6520 4c4c 4d0d  ut from the LLM.
+000011e0: 0a20 2020 2064 6566 205f 6578 7472 6163  .    def _extrac
+000011f0: 745f 636f 6465 2873 656c 662c 7265 7370  t_code(self,resp
+00001200: 6f6e 7365 3a20 7374 722c 2073 6570 6172  onse: str, separ
+00001210: 6174 6f72 3a20 7374 7220 3d20 2260 6060  ator: str = "```
+00001220: 2229 202d 3e20 7374 723a 0d0a 0d0a 2020  ") -> str:....  
+00001230: 2020 2020 2020 2320 4465 6669 6e65 2061        # Define a
+00001240: 2062 6c61 636b 6c69 7374 206f 6620 5079   blacklist of Py
+00001250: 7468 6f6e 206b 6579 776f 7264 7320 616e  thon keywords an
+00001260: 6420 6675 6e63 7469 6f6e 7320 7468 6174  d functions that
+00001270: 2061 7265 206e 6f74 2061 6c6c 6f77 6564   are not allowed
+00001280: 0d0a 2020 2020 2020 2020 626c 6163 6b6c  ..        blackl
+00001290: 6973 7420 3d20 5b27 6f73 272c 2773 7562  ist = ['os','sub
+000012a0: 7072 6f63 6573 7327 2c27 7379 7327 2c27  process','sys','
+000012b0: 6576 616c 272c 2765 7865 6327 2c27 6669  eval','exec','fi
+000012c0: 6c65 272c 2773 6f63 6b65 7427 2c27 7572  le','socket','ur
+000012d0: 6c6c 6962 272c 0d0a 2020 2020 2020 2020  llib',..        
+000012e0: 2020 2020 2020 2020 2020 2020 2773 6875              'shu
+000012f0: 7469 6c27 2c27 7069 636b 6c65 272c 2763  til','pickle','c
+00001300: 7479 7065 7327 2c27 6d75 6c74 6970 726f  types','multipro
+00001310: 6365 7373 696e 6727 2c27 7465 6d70 6669  cessing','tempfi
+00001320: 6c65 272c 2767 6c6f 6227 2c27 636f 6465  le','glob','code
+00001330: 272c 2770 7479 272c 2763 6f6d 6d61 6e64  ','pty','command
+00001340: 7327 2c0d 0a20 2020 2020 2020 2020 2020  s',..           
+00001350: 2020 2020 2020 2020 2027 7265 7175 6573           'reques
+00001360: 7473 272c 2763 6769 272c 2763 6769 7462  ts','cgi','cgitb
+00001370: 272c 2778 6d6c 2e65 7472 6565 2e45 6c65  ','xml.etree.Ele
+00001380: 6d65 6e74 5472 6565 272c 2762 7569 6c74  mentTree','built
+00001390: 696e 7327 0d0a 2020 2020 2020 2020 2020  ins'..          
+000013a0: 2020 2020 2020 2020 2020 5d0d 0a20 2020            ]..   
+000013b0: 2020 2020 200d 0a20 2020 2020 2020 2023       ..        #
+000013c0: 2053 6561 7263 6820 666f 7220 6120 7061   Search for a pa
+000013d0: 7474 6572 6e20 6265 7477 6565 6e20 3c72  ttern between <r
+000013e0: 6566 6c65 6374 696f 6e3e 2061 6e64 203c  eflection> and <
+000013f0: 2f72 6566 6c65 6374 696f 6e3e 2069 6e20  /reflection> in 
+00001400: 7468 6520 7265 7370 6f6e 7365 0d0a 2020  the response..  
+00001410: 2020 2020 2020 6d61 7463 6820 3d20 7265        match = re
+00001420: 2e73 6561 7263 6828 7222 3c72 6566 6c65  .search(r"<refle
+00001430: 6374 696f 6e3e 282e 2a29 3c2f 7265 666c  ction>(.*)</refl
+00001440: 6563 7469 6f6e 3e22 2c20 7265 7370 6f6e  ection>", respon
+00001450: 7365 2c20 7265 2e44 4f54 414c 4c29 0d0a  se, re.DOTALL)..
+00001460: 2020 2020 2020 2020 6966 206d 6174 6368          if match
+00001470: 3a0d 0a20 2020 2020 2020 2020 2020 2023  :..            #
+00001480: 2049 6620 6120 6d61 7463 6820 6973 2066   If a match is f
+00001490: 6f75 6e64 2c20 6578 7472 6163 7420 7468  ound, extract th
+000014a0: 6520 7265 666c 6563 7469 6f6e 2062 6574  e reflection bet
+000014b0: 7765 656e 203c 7265 666c 6563 7469 6f6e  ween <reflection
+000014c0: 3e20 616e 6420 3c2f 7265 666c 6563 7469  > and </reflecti
+000014d0: 6f6e 3e0d 0a20 2020 2020 2020 2020 2020  on>..           
+000014e0: 2072 6566 6c65 6374 696f 6e20 3d20 6d61   reflection = ma
+000014f0: 7463 682e 6772 6f75 7028 3129 0d0a 2020  tch.group(1)..  
+00001500: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00001510: 2020 2020 2020 2020 2072 6566 6c65 6374           reflect
+00001520: 696f 6e20 3d20 2222 0d0a 0d0a 2020 2020  ion = ""....    
+00001530: 2020 2020 2320 5365 6172 6368 2066 6f72      # Search for
+00001540: 2061 2070 6174 7465 726e 2062 6574 7765   a pattern betwe
+00001550: 656e 203c 666c 6f77 3e20 616e 6420 3c2f  en <flow> and </
+00001560: 666c 6f77 3e20 696e 2074 6865 2072 6573  flow> in the res
+00001570: 706f 6e73 650d 0a20 2020 2020 2020 206d  ponse..        m
+00001580: 6174 6368 203d 2072 652e 7365 6172 6368  atch = re.search
+00001590: 2872 223c 666c 6f77 3e28 2e2a 293c 2f66  (r"<flow>(.*)</f
+000015a0: 6c6f 773e 222c 2072 6573 706f 6e73 652c  low>", response,
+000015b0: 2072 652e 444f 5441 4c4c 290d 0a20 2020   re.DOTALL)..   
+000015c0: 2020 2020 2069 6620 6d61 7463 683a 0d0a       if match:..
+000015d0: 2020 2020 2020 2020 2020 2020 2320 4966              # If
+000015e0: 2061 206d 6174 6368 2069 7320 666f 756e   a match is foun
+000015f0: 642c 2065 7874 7261 6374 2074 6865 2072  d, extract the r
+00001600: 6566 6c65 6374 696f 6e20 6265 7477 6565  eflection betwee
+00001610: 6e20 3c72 6566 6c65 6374 696f 6e3e 2061  n <reflection> a
+00001620: 6e64 203c 2f72 6566 6c65 6374 696f 6e3e  nd </reflection>
+00001630: 0d0a 2020 2020 2020 2020 2020 2020 666c  ..            fl
+00001640: 6f77 203d 206d 6174 6368 2e67 726f 7570  ow = match.group
+00001650: 2831 290d 0a20 2020 2020 2020 2065 6c73  (1)..        els
+00001660: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00001670: 666c 6f77 203d 2022 220d 0a0d 0a20 2020  flow = ""....   
+00001680: 2020 2020 2023 2053 6561 7263 6820 666f       # Search fo
+00001690: 7220 6120 7061 7474 6572 6e20 6265 7477  r a pattern betw
+000016a0: 6565 6e20 3c63 6f64 653e 2061 6e64 203c  een <code> and <
+000016b0: 2f63 6f64 653e 2069 6e20 7468 6520 6578  /code> in the ex
+000016c0: 7472 6163 7465 6420 636f 6465 0d0a 2020  tracted code..  
+000016d0: 2020 2020 2020 6d61 7463 6820 3d20 7265        match = re
+000016e0: 2e73 6561 7263 6828 7222 3c63 6f64 653e  .search(r"<code>
+000016f0: 282e 2a29 3c2f 636f 6465 3e22 2c20 7265  (.*)</code>", re
+00001700: 7370 6f6e 7365 2c20 7265 2e44 4f54 414c  sponse, re.DOTAL
+00001710: 4c29 0d0a 2020 2020 2020 2020 6966 206d  L)..        if m
+00001720: 6174 6368 3a0d 0a20 2020 2020 2020 2020  atch:..         
+00001730: 2020 2023 2049 6620 6120 6d61 7463 6820     # If a match 
+00001740: 6973 2066 6f75 6e64 2c20 6578 7472 6163  is found, extrac
+00001750: 7420 7468 6520 636f 6465 2062 6574 7765  t the code betwe
+00001760: 656e 203c 636f 6465 3e20 616e 6420 3c2f  en <code> and </
+00001770: 636f 6465 3e0d 0a20 2020 2020 2020 2020  code>..         
+00001780: 2020 2063 6f64 6520 3d20 6d61 7463 682e     code = match.
+00001790: 6772 6f75 7028 3129 0d0a 2020 2020 2020  group(1)..      
+000017a0: 2020 2020 2020 2320 4966 2074 6865 2072        # If the r
+000017b0: 6573 706f 6e73 6520 636f 6e74 6169 6e73  esponse contains
+000017c0: 2074 6865 2073 6570 6172 6174 6f72 2c20   the separator, 
+000017d0: 6578 7472 6163 7420 7468 6520 636f 6465  extract the code
+000017e0: 2062 6c6f 636b 2062 6574 7765 656e 2074   block between t
+000017f0: 6865 2073 6570 6172 6174 6f72 730d 0a20  he separators.. 
+00001800: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+00001810: 6e28 636f 6465 2e73 706c 6974 2873 6570  n(code.split(sep
+00001820: 6172 6174 6f72 2929 203e 2031 3a0d 0a20  arator)) > 1:.. 
+00001830: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00001840: 6f64 6520 3d20 636f 6465 2e73 706c 6974  ode = code.split
+00001850: 2873 6570 6172 6174 6f72 295b 315d 0d0a  (separator)[1]..
+00001860: 0d0a 2020 2020 2020 2020 2320 4966 2074  ..        # If t
+00001870: 6865 2072 6573 706f 6e73 6520 636f 6e74  he response cont
+00001880: 6169 6e73 2074 6865 2073 6570 6172 6174  ains the separat
+00001890: 6f72 2c20 6578 7472 6163 7420 7468 6520  or, extract the 
+000018a0: 636f 6465 2062 6c6f 636b 2062 6574 7765  code block betwe
+000018b0: 656e 2074 6865 2073 6570 6172 6174 6f72  en the separator
+000018c0: 730d 0a20 2020 2020 2020 2069 6620 6c65  s..        if le
+000018d0: 6e28 7265 7370 6f6e 7365 2e73 706c 6974  n(response.split
+000018e0: 2873 6570 6172 6174 6f72 2929 203e 2031  (separator)) > 1
+000018f0: 3a0d 0a20 2020 2020 2020 2020 2020 2063  :..            c
+00001900: 6f64 6520 3d20 7265 7370 6f6e 7365 2e73  ode = response.s
+00001910: 706c 6974 2873 6570 6172 6174 6f72 295b  plit(separator)[
+00001920: 315d 0d0a 2020 2020 2020 2020 2020 2020  1]..            
+00001930: 0d0a 2020 2020 2020 2020 2320 5265 6d6f  ..        # Remo
+00001940: 7665 2074 6865 2022 7079 7468 6f6e 2220  ve the "python" 
+00001950: 6f72 2022 7079 2220 7072 6566 6978 2069  or "py" prefix i
+00001960: 6620 7072 6573 656e 740d 0a20 2020 2020  f present..     
+00001970: 2020 2069 6620 7265 2e6d 6174 6368 2872     if re.match(r
+00001980: 225e 2870 7974 686f 6e7c 7079 2922 2c20  "^(python|py)", 
+00001990: 636f 6465 293a 0d0a 2020 2020 2020 2020  code):..        
+000019a0: 2020 2020 636f 6465 203d 2072 652e 7375      code = re.su
+000019b0: 6228 7222 5e28 7079 7468 6f6e 7c70 7929  b(r"^(python|py)
+000019c0: 222c 2022 222c 2063 6f64 6529 0d0a 2020  ", "", code)..  
+000019d0: 2020 2020 2020 2320 4966 2074 6865 2063        # If the c
+000019e0: 6f64 6520 6973 2062 6574 7765 656e 2073  ode is between s
+000019f0: 696e 676c 6520 6261 636b 7469 636b 732c  ingle backticks,
+00001a00: 2065 7874 7261 6374 2074 6865 2063 6f64   extract the cod
+00001a10: 6520 6265 7477 6565 6e20 7468 656d 0d0a  e between them..
+00001a20: 2020 2020 2020 2020 6966 2072 652e 6d61          if re.ma
+00001a30: 7463 6828 7222 5e60 2e2a 6024 222c 2063  tch(r"^`.*`$", c
+00001a40: 6f64 6529 3a0d 0a20 2020 2020 2020 2020  ode):..         
+00001a50: 2020 2063 6f64 6520 3d20 7265 2e73 7562     code = re.sub
+00001a60: 2872 225e 6028 2e2a 2960 2422 2c20 7222  (r"^`(.*)`$", r"
+00001a70: 5c31 222c 2063 6f64 6529 0d0a 0d0a 2020  \1", code)....  
+00001a80: 2020 2020 2020 2320 5265 6d6f 7665 2061        # Remove a
+00001a90: 6e79 2069 6e73 7461 6e63 6573 206f 6620  ny instances of 
+00001aa0: 2264 6620 3d20 7064 2e72 6561 645f 6373  "df = pd.read_cs
+00001ab0: 7628 2766 696c 656e 616d 652e 6373 7627  v('filename.csv'
+00001ac0: 2922 2066 726f 6d20 7468 6520 636f 6465  )" from the code
+00001ad0: 0d0a 2020 2020 2020 2020 636f 6465 203d  ..        code =
+00001ae0: 2072 652e 7375 6228 7222 6466 5c73 2a3d   re.sub(r"df\s*=
+00001af0: 5c73 2a70 645c 2e72 6561 645f 6373 765c  \s*pd\.read_csv\
+00001b00: 2827 2e2a 3f27 5c29 222c 2022 222c 2063  ('.*?'\)", "", c
+00001b10: 6f64 6529 0d0a 2020 2020 2020 2020 0d0a  ode)..        ..
+00001b20: 2020 2020 2020 2020 2320 5265 6d6f 7665          # Remove
+00001b30: 2061 6e79 206f 6363 7572 7265 6e63 6573   any occurrences
+00001b40: 206f 6620 6466 203d 2070 642e 4461 7461   of df = pd.Data
+00001b50: 4672 616d 6528 2920 7769 7468 2061 6e79  Frame() with any
+00001b60: 206e 756d 6265 7220 6f66 2063 6861 7261   number of chara
+00001b70: 6374 6572 7320 696e 7369 6465 2074 6865  cters inside the
+00001b80: 2070 6172 656e 7468 6573 6573 2e0d 0a20   parentheses... 
+00001b90: 2020 2020 2020 2063 6f64 6520 3d20 7265         code = re
+00001ba0: 2e73 7562 2872 2264 665c 732a 3d5c 732a  .sub(r"df\s*=\s*
+00001bb0: 7064 5c2e 4461 7461 4672 616d 655c 282e  pd\.DataFrame\(.
+00001bc0: 2a3f 5c29 222c 2022 222c 2063 6f64 6529  *?\)", "", code)
+00001bd0: 0d0a 0d0a 2020 2020 2020 2020 2320 4465  ....        # De
+00001be0: 6669 6e65 2074 6865 2072 6567 756c 6172  fine the regular
+00001bf0: 2065 7870 7265 7373 696f 6e20 7061 7474   expression patt
+00001c00: 6572 6e20 746f 206d 6174 6368 2074 6865  ern to match the
+00001c10: 2062 6c61 636b 6c69 7374 2069 7465 6d73   blacklist items
+00001c20: 0d0a 2020 2020 2020 2020 7061 7474 6572  ..        patter
+00001c30: 6e20 3d20 7222 5e28 2e2a 5c62 2822 202b  n = r"^(.*\b(" +
+00001c40: 2022 7c22 2e6a 6f69 6e28 626c 6163 6b6c   "|".join(blackl
+00001c50: 6973 7429 202b 2072 2229 5c62 2e2a 2924  ist) + r")\b.*)$
+00001c60: 220d 0a0d 0a20 2020 2020 2020 2023 2052  "....        # R
+00001c70: 6570 6c61 6365 2074 6865 2062 6c61 636b  eplace the black
+00001c80: 6c69 7374 2069 7465 6d73 2077 6974 6820  list items with 
+00001c90: 636f 6d6d 656e 7473 0d0a 2020 2020 2020  comments..      
+00001ca0: 2020 636f 6465 203d 2072 652e 7375 6228    code = re.sub(
+00001cb0: 7061 7474 6572 6e2c 2072 2223 206e 6f74  pattern, r"# not
+00001cc0: 2061 6c6c 6f77 6564 205c 3122 2c20 636f   allowed \1", co
+00001cd0: 6465 2c20 666c 6167 733d 7265 2e4d 554c  de, flags=re.MUL
+00001ce0: 5449 4c49 4e45 290d 0a0d 0a20 2020 2020  TILINE)....     
+00001cf0: 2020 2023 2052 6574 7572 6e20 7468 6520     # Return the 
+00001d00: 636c 6561 6e65 6420 616e 6420 6578 7472  cleaned and extr
+00001d10: 6163 7465 6420 636f 6465 0d0a 2020 2020  acted code..    
+00001d20: 2020 2020 7265 7475 726e 2063 6f64 652e      return code.
+00001d30: 7374 7269 7028 292c 2072 6566 6c65 6374  strip(), reflect
+00001d40: 696f 6e2e 7374 7269 7028 292c 2066 6c6f  ion.strip(), flo
+00001d50: 772e 7374 7269 7028 290d 0a20 2020 200d  w.strip()..    .
+00001d60: 0a20 2020 2064 6566 205f 6578 7472 6163  .    def _extrac
+00001d70: 745f 7461 736b 2873 656c 662c 2072 6573  t_task(self, res
+00001d80: 706f 6e73 653a 2073 7472 2920 2d3e 2073  ponse: str) -> s
+00001d90: 7472 3a0d 0a20 2020 2020 2020 2023 2053  tr:..        # S
+00001da0: 6561 7263 6820 666f 7220 6120 7061 7474  earch for a patt
+00001db0: 6572 6e20 6265 7477 6565 6e20 3c74 6173  ern between <tas
+00001dc0: 6b3e 2061 6e64 203c 2f74 6173 6b3e 2069  k> and </task> i
+00001dd0: 6e20 7468 6520 7265 7370 6f6e 7365 0d0a  n the response..
+00001de0: 2020 2020 2020 2020 6d61 7463 6820 3d20          match = 
+00001df0: 7265 2e73 6561 7263 6828 7222 3c74 6173  re.search(r"<tas
+00001e00: 6b3e 282e 2a29 3c2f 7461 736b 3e22 2c20  k>(.*)</task>", 
+00001e10: 7265 7370 6f6e 7365 2c20 7265 2e44 4f54  response, re.DOT
+00001e20: 414c 4c29 0d0a 0d0a 2020 2020 2020 2020  ALL)....        
+00001e30: 6966 206d 6174 6368 3a0d 0a20 2020 2020  if match:..     
+00001e40: 2020 2020 2020 2023 2049 6620 6120 6d61         # If a ma
+00001e50: 7463 6820 6973 2066 6f75 6e64 2c20 6578  tch is found, ex
+00001e60: 7472 6163 7420 7468 6520 7461 736b 2062  tract the task b
+00001e70: 6574 7765 656e 203c 7461 736b 3e20 616e  etween <task> an
+00001e80: 6420 3c2f 7461 736b 3e0d 0a20 2020 2020  d </task>..     
+00001e90: 2020 2020 2020 2074 6173 6b20 3d20 6d61         task = ma
+00001ea0: 7463 682e 6772 6f75 7028 3129 0d0a 0d0a  tch.group(1)....
+00001eb0: 2020 2020 2020 2020 2020 2020 2320 4576              # Ev
+00001ec0: 6572 7974 6869 6e67 206f 7574 7369 6465  erything outside
+00001ed0: 206f 6620 3c74 6173 6b3e 3c2f 7461 736b   of <task></task
+00001ee0: 3e20 676f 6573 2074 6f20 7265 6173 6f6e  > goes to reason
+00001ef0: 696e 672e 0d0a 2020 2020 2020 2020 2020  ing...          
+00001f00: 2020 2320 4974 2073 706c 6974 7320 7468    # It splits th
+00001f10: 6520 7265 7370 6f6e 7365 2069 6e74 6f20  e response into 
+00001f20: 7477 6f20 7061 7274 732c 2065 7665 7279  two parts, every
+00001f30: 7468 696e 6720 6265 666f 7265 203c 7461  thing before <ta
+00001f40: 736b 3e20 616e 6420 6576 6572 7974 6869  sk> and everythi
+00001f50: 6e67 2061 6674 6572 203c 2f74 6173 6b3e  ng after </task>
+00001f60: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00001f70: 6173 6f6e 696e 675f 7061 7274 7320 3d20  asoning_parts = 
+00001f80: 7265 2e73 706c 6974 2872 223c 7461 736b  re.split(r"<task
+00001f90: 3e2e 2a3c 2f74 6173 6b3e 222c 2072 6573  >.*</task>", res
+00001fa0: 706f 6e73 652c 2066 6c61 6773 3d72 652e  ponse, flags=re.
+00001fb0: 444f 5441 4c4c 290d 0a20 2020 2020 2020  DOTALL)..       
+00001fc0: 2020 2020 2072 6561 736f 6e69 6e67 203d       reasoning =
+00001fd0: 2022 222e 6a6f 696e 2872 6561 736f 6e69   "".join(reasoni
+00001fe0: 6e67 5f70 6172 7473 290d 0a20 2020 2020  ng_parts)..     
+00001ff0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00002000: 2020 2020 2020 7461 736b 203d 2022 220d        task = "".
+00002010: 0a20 2020 2020 2020 2020 2020 2023 2049  .            # I
+00002020: 6620 6e6f 2074 6173 6b20 6973 2066 6f75  f no task is fou
+00002030: 6e64 2c20 616c 6c20 7468 6520 7265 7370  nd, all the resp
+00002040: 6f6e 7365 2067 6f65 7320 746f 2072 6561  onse goes to rea
+00002050: 736f 6e69 6e67 0d0a 2020 2020 2020 2020  soning..        
+00002060: 2020 2020 7265 6173 6f6e 696e 6720 3d20      reasoning = 
+00002070: 7265 7370 6f6e 7365 0d0a 0d0a 2020 2020  response....    
+00002080: 2020 2020 2320 5265 7475 726e 696e 6720      # Returning 
+00002090: 626f 7468 2074 6173 6b20 616e 6420 7265  both task and re
+000020a0: 6173 6f6e 696e 670d 0a20 2020 2020 2020  asoning..       
+000020b0: 2072 6574 7572 6e20 7461 736b 2c20 7265   return task, re
+000020c0: 6173 6f6e 696e 670d 0a20 2020 200d 0a20  asoning..    .. 
+000020d0: 2020 2064 6566 2074 6173 6b5f 6576 616c     def task_eval
+000020e0: 2873 656c 662c 2071 7565 7374 696f 6e3d  (self, question=
+000020f0: 4e6f 6e65 293a 0d0a 2020 2020 2020 2020  None):..        
+00002100: 2320 496e 6974 6961 6c69 7a65 2074 6865  # Initialize the
+00002110: 206d 6573 7361 6765 7320 6c69 7374 2077   messages list w
+00002120: 6974 6820 6120 7379 7374 656d 206d 6573  ith a system mes
+00002130: 7361 6765 2063 6f6e 7461 696e 696e 6720  sage containing 
+00002140: 7468 6520 7461 736b 2070 726f 6d70 740d  the task prompt.
+00002150: 0a20 2020 2020 2020 2065 7661 6c5f 6d65  .        eval_me
+00002160: 7373 6167 6573 203d 205b 7b22 726f 6c65  ssages = [{"role
+00002170: 223a 2022 7379 7374 656d 222c 2022 636f  ": "system", "co
+00002180: 6e74 656e 7422 3a20 7365 6c66 2e74 6173  ntent": self.tas
+00002190: 6b5f 6576 616c 7561 7469 6f6e 2e66 6f72  k_evaluation.for
+000021a0: 6d61 7428 7365 6c66 2e64 665f 6865 6164  mat(self.df_head
+000021b0: 2c20 7175 6573 7469 6f6e 297d 5d0d 0a0d  , question)}]...
+000021c0: 0a20 2020 2020 2020 2069 6620 2769 7079  .        if 'ipy
+000021d0: 6b65 726e 656c 2720 696e 2073 7973 2e6d  kernel' in sys.m
+000021e0: 6f64 756c 6573 3a0d 0a20 2020 2020 2020  odules:..       
+000021f0: 2020 2020 2023 204a 7570 7974 6572 206e       # Jupyter n
+00002200: 6f74 6562 6f6f 6b20 6f72 2069 7079 7468  otebook or ipyth
+00002210: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
+00002220: 6469 7370 6c61 7928 4854 4d4c 2866 273c  display(HTML(f'<
+00002230: 7020 7374 796c 653d 2263 6f6c 6f72 3a6d  p style="color:m
+00002240: 6167 656e 7461 3b22 3e5c 6e55 7369 6e67  agenta;">\nUsing
+00002250: 204d 6f64 656c 3a20 7b73 656c 662e 6c6c   Model: {self.ll
+00002260: 6d7d 3c2f 703e 2729 290d 0a20 2020 2020  m}</p>'))..     
+00002270: 2020 2020 2020 2064 6973 706c 6179 2848         display(H
+00002280: 544d 4c28 6627 3c70 3e3c 6220 7374 796c  TML(f'<p><b styl
+00002290: 653d 2263 6f6c 6f72 3a6d 6167 656e 7461  e="color:magenta
+000022a0: 3b22 3e54 7279 696e 6720 746f 2064 6574  ;">Trying to det
+000022b0: 6572 6d69 6e65 2074 6865 2062 6573 7420  ermine the best 
+000022c0: 6d65 7468 6f64 2074 6f20 616e 616c 7973  method to analys
+000022d0: 6520 796f 7574 2064 6174 612c 2070 6c65  e yout data, ple
+000022e0: 6173 6520 7761 6974 2e2e 2e3c 2f62 3e3c  ase wait...</b><
+000022f0: 2f70 3e3c 6272 3e27 2929 0d0a 2020 2020  /p><br>'))..    
+00002300: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00002310: 2020 2020 2020 2023 204f 7468 6572 2065         # Other e
+00002320: 6e76 6972 6f6e 6d65 6e74 2028 6c69 6b65  nvironment (like
+00002330: 2074 6572 6d69 6e61 6c29 0d0a 2020 2020   terminal)..    
+00002340: 2020 2020 2020 2020 7072 696e 7428 636f          print(co
+00002350: 6c6f 7265 6428 6622 5c6e 3e20 5573 696e  lored(f"\n> Usin
+00002360: 6720 4d6f 6465 6c3a 207b 7365 6c66 2e6c  g Model: {self.l
+00002370: 6c6d 7d22 2c20 226d 6167 656e 7461 2229  lm}", "magenta")
+00002380: 290d 0a20 2020 2020 2020 2020 2020 2063  )..            c
+00002390: 7072 696e 7428 6622 5c6e 3e20 5472 7969  print(f"\n> Tryi
+000023a0: 6e67 2074 6f20 6465 7465 726d 696e 6520  ng to determine 
+000023b0: 7468 6520 6265 7374 206d 6574 686f 6420  the best method 
+000023c0: 746f 2061 6e73 6c79 7365 2079 7572 2064  to anslyse yur d
+000023d0: 6174 612c 2070 6c65 6173 6520 7761 6974  ata, please wait
+000023e0: 2e2e 2e5c 6e22 2c20 276d 6167 656e 7461  ...\n", 'magenta
+000023f0: 272c 2061 7474 7273 3d5b 2762 6f6c 6427  ', attrs=['bold'
+00002400: 5d29 0d0a 0d0a 2020 2020 2020 2020 2320  ])....        # 
+00002410: 4675 6e63 7469 6f6e 2074 6f20 6469 7370  Function to disp
+00002420: 6c61 7920 7265 7375 6c74 7320 6e69 6365  lay results nice
+00002430: 6c79 0d0a 2020 2020 2020 2020 6465 6620  ly..        def 
+00002440: 6469 7370 6c61 795f 7461 736b 2874 6173  display_task(tas
+00002450: 6b2c 7265 6173 6f6e 696e 6729 3a0d 0a20  k,reasoning):.. 
+00002460: 2020 2020 2020 2020 2020 2069 6620 2769             if 'i
+00002470: 7079 6b65 726e 656c 2720 696e 2073 7973  pykernel' in sys
+00002480: 2e6d 6f64 756c 6573 3a0d 0a20 2020 2020  .modules:..     
+00002490: 2020 2020 2020 2020 2020 2023 204a 7570             # Jup
+000024a0: 7974 6572 206e 6f74 6562 6f6f 6b20 6f72  yter notebook or
+000024b0: 2069 7079 7468 6f6e 0d0a 2020 2020 2020   ipython..      
+000024c0: 2020 2020 2020 2020 2020 6469 7370 6c61            displa
+000024d0: 7928 4854 4d4c 2866 273c 703e 3c62 2073  y(HTML(f'<p><b s
+000024e0: 7479 6c65 3d22 636f 6c6f 723a 626c 7565  tyle="color:blue
+000024f0: 3b22 3e49 2068 6176 6520 6576 616c 7561  ;">I have evalua
+00002500: 7465 6420 7365 7665 7261 6c20 706f 7373  ted several poss
+00002510: 6962 6c65 2061 7070 726f 6163 6865 732e  ible approaches.
+00002520: 2042 656c 6f77 2069 7320 6d79 2072 6561   Below is my rea
+00002530: 736f 6e69 6e67 3a3c 2f62 3e3c 6272 3e3c  soning:</b><br><
+00002540: 7072 6520 7374 796c 653d 2263 6f6c 6f72  pre style="color
+00002550: 3a62 6c61 636b 3b22 3e3c 623e 7b72 6561  :black;"><b>{rea
+00002560: 736f 6e69 6e67 7d3c 2f62 3e3c 2f70 7265  soning}</b></pre
+00002570: 3e3c 2f70 3e3c 6272 3e27 2929 0d0a 2020  ></p><br>'))..  
+00002580: 2020 2020 2020 2020 2020 2020 2020 6469                di
+00002590: 7370 6c61 7928 4854 4d4c 2866 273c 703e  splay(HTML(f'<p>
+000025a0: 3c62 2073 7479 6c65 3d22 636f 6c6f 723a  <b style="color:
+000025b0: 626c 7565 3b22 3e54 6173 6b3a 3c2f 623e  blue;">Task:</b>
+000025c0: 3c62 7220 7374 796c 653d 2263 6f6c 6f72  <br style="color
+000025d0: 3a62 6c61 636b 3b22 3e3c 623e 7b74 6173  :black;"><b>{tas
+000025e0: 6b7d 3c2f 623e 3c2f 703e 3c62 723e 2729  k}</b></p><br>')
+000025f0: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
+00002600: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00002610: 2020 2020 2020 2320 4f74 6865 7220 656e        # Other en
+00002620: 7669 726f 6e6d 656e 7420 286c 696b 6520  vironment (like 
+00002630: 7465 726d 696e 616c 290d 0a20 2020 2020  terminal)..     
+00002640: 2020 2020 2020 2020 2020 2063 7072 696e             cprin
+00002650: 7428 6622 5c6e 4920 6861 7665 2065 7661  t(f"\nI have eva
+00002660: 6c75 6174 6564 2073 6576 6572 616c 2070  luated several p
+00002670: 6f73 7369 626c 6520 6170 7072 6f61 6368  ossible approach
+00002680: 6573 2e20 4265 6c6f 7720 6973 206d 7920  es. Below is my 
+00002690: 7265 6173 6f6e 696e 673a 5c6e 7b72 6561  reasoning:\n{rea
+000026a0: 736f 6e69 6e67 7d5c 6e22 2c20 276d 6167  soning}\n", 'mag
+000026b0: 656e 7461 272c 2061 7474 7273 3d5b 2762  enta', attrs=['b
+000026c0: 6f6c 6427 5d29 0d0a 2020 2020 2020 2020  old'])..        
+000026d0: 2020 2020 2020 2020 6370 7269 6e74 2866          cprint(f
+000026e0: 225c 6e54 6173 6b3a 5c6e 7b74 6173 6b7d  "\nTask:\n{task}
+000026f0: 5c6e 222c 2027 6d61 6765 6e74 6127 2c20  \n", 'magenta', 
+00002700: 6174 7472 733d 5b27 626f 6c64 275d 290d  attrs=['bold']).
+00002710: 0a0d 0a20 2020 2020 2020 2023 2043 616c  ...        # Cal
+00002720: 6c20 7468 6520 4f70 656e 4149 2041 5049  l the OpenAI API
+00002730: 2061 6e64 2068 616e 646c 6520 7261 7465   and handle rate
+00002740: 206c 696d 6974 2065 7272 6f72 730d 0a20   limit errors.. 
+00002750: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
+00002760: 2020 2020 2020 2020 206c 6c6d 5f72 6573           llm_res
+00002770: 706f 6e73 652c 2074 6f6b 656e 735f 7573  ponse, tokens_us
+00002780: 6564 203d 2073 656c 662e 6c6c 6d5f 6361  ed = self.llm_ca
+00002790: 6c6c 2865 7661 6c5f 6d65 7373 6167 6573  ll(eval_messages
+000027a0: 290d 0a20 2020 2020 2020 2065 7863 6570  )..        excep
+000027b0: 7420 6f70 656e 6169 2e65 7272 6f72 2e52  t openai.error.R
+000027c0: 6174 654c 696d 6974 4572 726f 723a 0d0a  ateLimitError:..
+000027d0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+000027e0: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
+000027f0: 2020 2020 2254 6865 204f 7065 6e41 4920      "The OpenAI 
+00002800: 4150 4920 7261 7465 206c 696d 6974 2068  API rate limit h
+00002810: 6173 2062 6565 6e20 6578 6365 6564 6564  as been exceeded
+00002820: 2e20 5761 6974 696e 6720 3130 2073 6563  . Waiting 10 sec
+00002830: 6f6e 6473 2061 6e64 2074 7279 696e 6720  onds and trying 
+00002840: 6167 6169 6e2e 220d 0a20 2020 2020 2020  again."..       
+00002850: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+00002860: 2020 2020 7469 6d65 2e73 6c65 6570 2831      time.sleep(1
+00002870: 3029 0d0a 2020 2020 2020 2020 2020 2020  0)..            
+00002880: 6c6c 6d5f 7265 7370 6f6e 7365 2c20 746f  llm_response, to
+00002890: 6b65 6e73 5f75 7365 6420 3d20 7365 6c66  kens_used = self
+000028a0: 2e6c 6c6d 5f63 616c 6c28 6576 616c 5f6d  .llm_call(eval_m
+000028b0: 6573 7361 6765 7329 0d0a 0d0a 2020 2020  essages)....    
+000028c0: 2020 2020 2320 4578 7472 6163 7420 7468      # Extract th
+000028d0: 6520 7461 736b 2061 6e64 2065 736f 6e69  e task and esoni
+000028e0: 6e67 2066 726f 6d20 7468 6520 4150 4920  ng from the API 
+000028f0: 7265 7370 6f6e 7365 0d0a 2020 2020 2020  response..      
+00002900: 2020 7461 736b 2c72 6561 736f 6e69 6e67    task,reasoning
+00002910: 203d 2073 656c 662e 5f65 7874 7261 6374   = self._extract
+00002920: 5f74 6173 6b28 6c6c 6d5f 7265 7370 6f6e  _task(llm_respon
+00002930: 7365 290d 0a0d 0a20 2020 2020 2020 2069  se)....        i
+00002940: 6620 7461 736b 2069 7320 4e6f 6e65 3a0d  f task is None:.
+00002950: 0a20 2020 2020 2020 2020 2020 2074 6173  .            tas
+00002960: 6b20 3d20 7175 6573 7469 6f6e 0d0a 2020  k = question..  
+00002970: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00002980: 2320 5072 696e 7420 7265 6173 6f6e 696e  # Print reasonin
+00002990: 670d 0a20 2020 2020 2020 2064 6973 706c  g..        displ
+000029a0: 6179 5f74 6173 6b28 7461 736b 2c72 6561  ay_task(task,rea
+000029b0: 736f 6e69 6e67 290d 0a0d 0a20 2020 2020  soning)....     
+000029c0: 2020 2073 656c 662e 746f 7461 6c5f 746f     self.total_to
+000029d0: 6b65 6e73 5f75 7365 642e 6170 7065 6e64  kens_used.append
+000029e0: 2874 6f6b 656e 735f 7573 6564 290d 0a0d  (tokens_used)...
+000029f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00002a00: 7461 736b 0d0a 0d0a 2020 2020 6465 6620  task....    def 
+00002a10: 7064 5f61 6765 6e74 5f63 6f6e 7665 7273  pd_agent_convers
+00002a20: 6528 7365 6c66 2c20 7175 6573 7469 6f6e  e(self, question
+00002a30: 3d4e 6f6e 6529 3a0d 0a20 2020 2020 2020  =None):..       
+00002a40: 2023 2049 6e69 7469 616c 697a 6520 7468   # Initialize th
+00002a50: 6520 6d65 7373 6167 6573 206c 6973 7420  e messages list 
+00002a60: 7769 7468 2061 2073 7973 7465 6d20 6d65  with a system me
+00002a70: 7373 6167 6520 636f 6e74 6169 6e69 6e67  ssage containing
+00002a80: 2074 6865 2074 6173 6b20 7072 6f6d 7074   the task prompt
+00002a90: 0d0a 2020 2020 2020 2020 6d65 7373 6167  ..        messag
+00002aa0: 6573 203d 205b 7b22 726f 6c65 223a 2022  es = [{"role": "
+00002ab0: 7379 7374 656d 222c 2022 636f 6e74 656e  system", "conten
+00002ac0: 7422 3a20 7365 6c66 2e74 6173 6b2e 666f  t": self.task.fo
+00002ad0: 726d 6174 2873 656c 662e 6466 5f68 6561  rmat(self.df_hea
+00002ae0: 642c 2022 2229 7d5d 0d0a 0d0a 2020 2020  d, "")}]....    
+00002af0: 2020 2020 2320 4675 6e63 7469 6f6e 2074      # Function t
+00002b00: 6f20 6469 7370 6c61 7920 7265 7375 6c74  o display result
+00002b10: 7320 6e69 6365 6c79 0d0a 2020 2020 2020  s nicely..      
+00002b20: 2020 6465 6620 6469 7370 6c61 795f 7265    def display_re
+00002b30: 7375 6c74 7328 616e 7377 6572 2c20 636f  sults(answer, co
+00002b40: 6465 2c20 7265 666c 6563 7469 6f6e 2c20  de, reflection, 
+00002b50: 666c 6f77 2c20 746f 7461 6c5f 746f 6b65  flow, total_toke
+00002b60: 6e73 5f75 7365 645f 7375 6d29 3a0d 0a20  ns_used_sum):.. 
+00002b70: 2020 2020 2020 2020 2020 2069 6620 2769             if 'i
+00002b80: 7079 6b65 726e 656c 2720 696e 2073 7973  pykernel' in sys
+00002b90: 2e6d 6f64 756c 6573 3a0d 0a20 2020 2020  .modules:..     
+00002ba0: 2020 2020 2020 2020 2020 2023 204a 7570             # Jup
+00002bb0: 7974 6572 206e 6f74 6562 6f6f 6b20 6f72  yter notebook or
+00002bc0: 2069 7079 7468 6f6e 0d0a 2020 2020 2020   ipython..      
+00002bd0: 2020 2020 2020 2020 2020 6469 7370 6c61            displa
+00002be0: 7928 4854 4d4c 2866 273c 703e 3c62 2073  y(HTML(f'<p><b s
+00002bf0: 7479 6c65 3d22 636f 6c6f 723a 626c 7565  tyle="color:blue
+00002c00: 3b22 3e41 6e73 7765 723a 3c2f 623e 3c62  ;">Answer:</b><b
+00002c10: 723e 3c70 7265 2073 7479 6c65 3d22 636f  r><pre style="co
+00002c20: 6c6f 723a 626c 6163 6b3b 223e 3c62 3e7b  lor:black;"><b>{
+00002c30: 616e 7377 6572 7d3c 2f62 3e3c 2f70 7265  answer}</b></pre
+00002c40: 3e3c 2f70 3e3c 6272 3e27 2929 0d0a 2020  ></p><br>'))..  
+00002c50: 2020 2020 2020 2020 2020 2020 2020 6469                di
+00002c60: 7370 6c61 7928 4854 4d4c 2866 273c 703e  splay(HTML(f'<p>
+00002c70: 3c62 2073 7479 6c65 3d22 636f 6c6f 723a  <b style="color:
+00002c80: 626c 7565 3b22 3e49 2068 6176 6520 6765  blue;">I have ge
+00002c90: 6e65 7261 7465 6420 7468 6520 666f 6c6c  nerated the foll
+00002ca0: 6f77 696e 6720 636f 6465 3a3c 2f62 3e3c  owing code:</b><
+00002cb0: 6272 3e3c 7072 6520 7374 796c 653d 2263  br><pre style="c
+00002cc0: 6f6c 6f72 3a23 3535 3535 3535 3b22 3e7b  olor:#555555;">{
+00002cd0: 636f 6465 7d3c 2f70 7265 3e3c 2f70 3e3c  code}</pre></p><
+00002ce0: 6272 3e27 2929 0d0a 2020 2020 2020 2020  br>'))..        
+00002cf0: 2020 2020 2020 2020 6469 7370 6c61 7928          display(
+00002d00: 4854 4d4c 2866 273c 703e 3c62 2073 7479  HTML(f'<p><b sty
+00002d10: 6c65 3d22 636f 6c6f 723a 626c 7565 3b22  le="color:blue;"
+00002d20: 3e46 696e 616c 2054 686f 7567 6874 733a  >Final Thoughts:
+00002d30: 3c2f 623e 3c62 723e 3c62 2073 7479 6c65  </b><br><b style
+00002d40: 3d22 636f 6c6f 723a 626c 6163 6b3b 223e  ="color:black;">
+00002d50: 7b72 6566 6c65 6374 696f 6e7d 3c2f 623e  {reflection}</b>
+00002d60: 3c2f 703e 3c62 723e 2729 290d 0a20 2020  </p><br>'))..   
+00002d70: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+00002d80: 706c 6179 2848 544d 4c28 6627 3c70 3e3c  play(HTML(f'<p><
+00002d90: 6220 7374 796c 653d 2263 6f6c 6f72 3a62  b style="color:b
+00002da0: 6c75 653b 223e 4265 6c6f 7720 6973 206d  lue;">Below is m
+00002db0: 7920 6170 7072 6f63 6820 6173 2061 2046  y approch as a F
+00002dc0: 6c6f 7720 6368 6172 743a 3c2f 623e 3c62  low chart:</b><b
+00002dd0: 723e 3c69 6d67 2073 7263 3d22 7b73 656c  r><img src="{sel
+00002de0: 662e 6d6d 2866 6c6f 7729 7d22 2061 6c74  f.mm(flow)}" alt
+00002df0: 3d22 416e 616c 7973 6973 2046 6c6f 7722  ="Analysis Flow"
+00002e00: 3e3c 2f69 6d67 3e3c 2f70 3e3c 6272 3e27  ></img></p><br>'
+00002e10: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00002e20: 2020 2020 6469 7370 6c61 7928 4854 4d4c      display(HTML
+00002e30: 2866 273c 703e 3c62 2073 7479 6c65 3d22  (f'<p><b style="
+00002e40: 636f 6c6f 723a 626c 7565 3b22 3e54 6f74  color:blue;">Tot
+00002e50: 616c 2054 6f6b 656e 7320 5573 6564 3a3c  al Tokens Used:<
+00002e60: 2f62 3e3c 6272 3e3c 7370 616e 2073 7479  /b><br><span sty
+00002e70: 6c65 3d22 636f 6c6f 723a 626c 6163 6b3b  le="color:black;
+00002e80: 223e 7b74 6f74 616c 5f74 6f6b 656e 735f  ">{total_tokens_
+00002e90: 7573 6564 5f73 756d 7d3c 2f73 7061 6e3e  used_sum}</span>
+00002ea0: 3c2f 703e 3c62 723e 2729 290d 0a20 2020  </p><br>'))..   
+00002eb0: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
 00002ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ed0: 2020 2064 6973 706c 6179 2848 544d 4c28     display(HTML(
-00002ee0: 6627 3c62 3e3c 7370 616e 2073 7479 6c65  f'<b><span style
-00002ef0: 3d22 636f 6c6f 723a 2072 6564 3b22 3e45  ="color: red;">E
-00002f00: 7272 6f72 3a3c 6272 3e3c 7072 653e 7b65  rror:<br><pre>{e
-00002f10: 7d3c 2f70 7265 3e3c 6272 3e54 6865 2061  }</pre><br>The a
-00002f20: 6765 6e74 2077 696c 6c20 7265 7472 792e  gent will retry.
-00002f30: 3c2f 7370 616e 3e3c 2f62 3e27 2929 0d0a  </span></b>'))..
-00002f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f50: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00002f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f70: 2020 2023 2043 4c49 0d0a 2020 2020 2020     # CLI..      
-00002f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f90: 2020 7072 696e 7428 636f 6c6f 7265 6428    print(colored(
-00002fa0: 6627 4572 726f 723a 207b 657d 2e20 5468  f'Error: {e}. Th
-00002fb0: 6520 6167 656e 7420 7769 6c6c 2072 6574  e agent will ret
-00002fc0: 7279 2e27 2c20 2772 6564 2729 290d 0a0d  ry.', 'red'))...
-00002fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002fe0: 2020 2020 2023 2049 6e63 7265 6d65 6e74       # Increment
-00002ff0: 2074 6865 2065 7272 6f72 2063 6f72 7265   the error corre
-00003000: 6374 696f 6e20 636f 756e 7465 7220 616e  ction counter an
-00003010: 6420 7570 6461 7465 2074 6865 206d 6573  d update the mes
-00003020: 7361 6765 7320 6c69 7374 2077 6974 6820  sages list with 
-00003030: 7468 6520 6572 726f 720d 0a20 2020 2020  the error..     
-00003040: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00003050: 7272 6f72 5f63 6f72 7265 6374 696f 6e73  rror_corrections
-00003060: 202b 3d20 310d 0a20 2020 2020 2020 2020   += 1..         
-00003070: 2020 2020 2020 2020 2020 206d 6573 7361             messa
-00003080: 6765 732e 6170 7065 6e64 287b 2272 6f6c  ges.append({"rol
-00003090: 6522 3a20 2275 7365 7222 2c20 2263 6f6e  e": "user", "con
-000030a0: 7465 6e74 223a 2073 656c 662e 6572 726f  tent": self.erro
-000030b0: 725f 636f 7272 6563 745f 7461 736b 2e66  r_correct_task.f
-000030c0: 6f72 6d61 7428 652c 2063 6f64 652c 2071  ormat(e, code, q
-000030d0: 7565 7374 696f 6e29 7d29 0d0a 0d0a 2020  uestion)})....  
-000030e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030f0: 2020 2320 5377 6974 6368 2074 6f20 6770    # Switch to gp
-00003100: 742d 3420 6966 206c 6c6d 5f73 7769 7463  t-4 if llm_switc
-00003110: 6820 6973 2054 7275 650d 0a20 2020 2020  h is True..     
-00003120: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00003130: 6620 7365 6c66 2e6c 6c6d 5f73 7769 7463  f self.llm_switc
-00003140: 683a 0d0a 2020 2020 2020 2020 2020 2020  h:..            
-00003150: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00003160: 2e6c 6c6d 203d 2027 6770 742d 3427 0d0a  .llm = 'gpt-4'..
-00003170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003180: 2020 2020 2020 2020 6966 2027 6970 796b          if 'ipyk
-00003190: 6572 6e65 6c27 2069 6e20 7379 732e 6d6f  ernel' in sys.mo
-000031a0: 6475 6c65 733a 0d0a 2020 2020 2020 2020  dules:..        
-000031b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031c0: 2020 2020 2320 4a75 7079 7465 7220 6e6f      # Jupyter no
-000031d0: 7465 626f 6f6b 0d0a 2020 2020 2020 2020  tebook..        
-000031e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031f0: 2020 2020 6469 7370 6c61 7928 4854 4d4c      display(HTML
-00003200: 2827 3c73 7061 6e20 7374 796c 653d 2263  ('<span style="c
-00003210: 6f6c 6f72 3a20 7265 643b 223e 5377 6974  olor: red;">Swit
-00003220: 6368 696e 6720 6d6f 6465 6c20 746f 2067  ching model to g
-00003230: 7074 2d34 2074 6f20 7472 7920 746f 2069  pt-4 to try to i
-00003240: 6d70 726f 7665 2074 6865 206f 7574 636f  mprove the outco
-00003250: 6d65 2e3c 2f73 7061 6e3e 2729 290d 0a20  me.</span>')).. 
-00003260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003270: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-00003280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003290: 2020 2020 2020 2020 2020 2320 434c 490d            # CLI.
-000032a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000032b0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-000032c0: 6e74 2863 6f6c 6f72 6564 2827 5377 6974  nt(colored('Swit
-000032d0: 6368 696e 6720 6d6f 6465 6c20 746f 2067  ching model to g
-000032e0: 7074 2d34 2074 6f20 7472 7920 746f 2069  pt-4 to try to i
-000032f0: 6d70 726f 7665 2074 6865 206f 7574 636f  mprove the outco
-00003300: 6d65 2e27 2c20 2772 6564 2729 290d 0a0d  me.', 'red'))...
-00003310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003320: 2020 2020 2023 2041 7474 656d 7074 2074       # Attempt t
-00003330: 6f20 636f 7272 6563 7420 7468 6520 636f  o correct the co
-00003340: 6465 2061 6e64 2068 616e 646c 6520 7261  de and handle ra
-00003350: 7465 206c 696d 6974 2065 7272 6f72 730d  te limit errors.
-00003360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003370: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
-00003380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003390: 2020 206c 6c6d 5f72 6573 706f 6e73 652c     llm_response,
-000033a0: 2074 6f6b 656e 735f 7573 6564 203d 2073   tokens_used = s
-000033b0: 656c 662e 6c6c 6d5f 6361 6c6c 286d 6573  elf.llm_call(mes
-000033c0: 7361 6765 7329 0d0a 2020 2020 2020 2020  sages)..        
-000033d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033e0: 636f 6465 2c72 6566 6c65 6374 696f 6e2c  code,reflection,
-000033f0: 666c 6f77 203d 2073 656c 662e 5f65 7874  flow = self._ext
-00003400: 7261 6374 5f63 6f64 6528 6c6c 6d5f 7265  ract_code(llm_re
-00003410: 7370 6f6e 7365 290d 0a20 2020 2020 2020  sponse)..       
-00003420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003430: 2073 656c 662e 746f 7461 6c5f 746f 6b65   self.total_toke
-00003440: 6e73 5f75 7365 642e 6170 7065 6e64 2874  ns_used.append(t
-00003450: 6f6b 656e 735f 7573 6564 290d 0a20 2020  okens_used)..   
-00003460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003470: 2020 2020 2074 6f74 616c 5f74 6f6b 656e       total_token
-00003480: 735f 7573 6564 5f73 756d 203d 2073 756d  s_used_sum = sum
-00003490: 2873 656c 662e 746f 7461 6c5f 746f 6b65  (self.total_toke
-000034a0: 6e73 5f75 7365 6429 0d0a 2020 2020 2020  ns_used)..      
-000034b0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-000034c0: 6365 7074 206f 7065 6e61 692e 6572 726f  cept openai.erro
-000034d0: 722e 5261 7465 4c69 6d69 7445 7272 6f72  r.RateLimitError
-000034e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000034f0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00003500: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-00003510: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00003520: 5468 6520 4f70 656e 4149 2041 5049 2072  The OpenAI API r
-00003530: 6174 6520 6c69 6d69 7420 6861 7320 6265  ate limit has be
-00003540: 656e 2065 7863 6565 6465 642e 2057 6169  en exceeded. Wai
-00003550: 7469 6e67 2031 3020 7365 636f 6e64 7320  ting 10 seconds 
-00003560: 616e 6420 7472 7969 6e67 2061 6761 696e  and trying again
-00003570: 2e22 0d0a 2020 2020 2020 2020 2020 2020  ."..            
-00003580: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
-00003590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035a0: 2020 2020 2020 2074 696d 652e 736c 6565         time.slee
-000035b0: 7028 3130 290d 0a20 2020 2020 2020 2020  p(10)..         
-000035c0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-000035d0: 6c6d 5f72 6573 706f 6e73 652c 2074 6f6b  lm_response, tok
-000035e0: 656e 735f 7573 6564 203d 2073 656c 662e  ens_used = self.
-000035f0: 6c6c 6d5f 6361 6c6c 286d 6573 7361 6765  llm_call(message
-00003600: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
-00003610: 2020 2020 2020 2020 2020 2020 636f 6465              code
-00003620: 2c72 6566 6c65 6374 696f 6e2c 666c 6f77  ,reflection,flow
-00003630: 203d 2073 656c 662e 5f65 7874 7261 6374   = self._extract
-00003640: 5f63 6f64 6528 6c6c 6d5f 7265 7370 6f6e  _code(llm_respon
-00003650: 7365 290d 0a20 2020 2020 2020 2020 2020  se)..           
-00003660: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00003670: 662e 746f 7461 6c5f 746f 6b65 6e73 5f75  f.total_tokens_u
-00003680: 7365 642e 6170 7065 6e64 2874 6f6b 656e  sed.append(token
-00003690: 735f 7573 6564 290d 0a20 2020 2020 2020  s_used)..       
-000036a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036b0: 2074 6f74 616c 5f74 6f6b 656e 735f 7573   total_tokens_us
-000036c0: 6564 5f73 756d 203d 2073 756d 2873 656c  ed_sum = sum(sel
-000036d0: 662e 746f 7461 6c5f 746f 6b65 6e73 5f75  f.total_tokens_u
-000036e0: 7365 6429 0d0a 0d0a 2020 2020 2020 2020  sed)....        
-000036f0: 2020 2020 2320 5377 6974 6368 2062 6163      # Switch bac
-00003700: 6b20 746f 2074 6865 206f 7269 6769 6e61  k to the origina
-00003710: 6c20 6c6c 6d20 6265 666f 7265 2074 6865  l llm before the
-00003720: 2066 756e 6374 696f 6e20 6669 6e69 7368   function finish
-00003730: 6573 0d0a 2020 2020 2020 2020 2020 2020  es..            
-00003740: 7365 6c66 2e6c 6c6d 203d 206f 7269 6769  self.llm = origi
-00003750: 6e61 6c5f 6c6c 6d0d 0a0d 0a20 2020 2020  nal_llm....     
-00003760: 2020 2023 2047 6574 2074 6865 206f 7574     # Get the out
-00003770: 7075 7420 6672 6f6d 2074 6865 2065 7865  put from the exe
-00003780: 6375 7465 6420 636f 6465 0d0a 2020 2020  cuted code..    
-00003790: 2020 2020 616e 7377 6572 203d 206f 7574      answer = out
-000037a0: 7075 742e 6765 7476 616c 7565 2829 0d0a  put.getvalue()..
-000037b0: 0d0a 2020 2020 2020 2020 2320 5265 7365  ..        # Rese
-000037c0: 7420 7468 6520 5374 7269 6e67 494f 2062  t the StringIO b
-000037d0: 7566 6665 720d 0a20 2020 2020 2020 206f  uffer..        o
-000037e0: 7574 7075 742e 7472 756e 6361 7465 2830  utput.truncate(0
-000037f0: 290d 0a20 2020 2020 2020 206f 7574 7075  )..        outpu
-00003800: 742e 7365 656b 2830 290d 0a0d 0a20 2020  t.seek(0)....   
-00003810: 2020 2020 2072 6574 7572 6e20 616e 7377       return answ
-00003820: 6572 2c20 636f 6465 2c20 7265 666c 6563  er, code, reflec
-00003830: 7469 6f6e 2c20 666c 6f77 2c20 746f 7461  tion, flow, tota
-00003840: 6c5f 746f 6b65 6e73 5f75 7365 645f 7375  l_tokens_used_su
-00003850: 6d0d 0a20 2020 20                        m..    
+00002ed0: 2320 4f74 6865 7220 656e 7669 726f 6e6d  # Other environm
+00002ee0: 656e 7420 286c 696b 6520 7465 726d 696e  ent (like termin
+00002ef0: 616c 290d 0a20 2020 2020 2020 2020 2020  al)..           
+00002f00: 2020 2020 2063 7072 696e 7428 6622 5c6e       cprint(f"\n
+00002f10: 3e20 416e 7377 6572 3a5c 6e7b 616e 7377  > Answer:\n{answ
+00002f20: 6572 7d5c 6e22 2c20 2767 7265 656e 272c  er}\n", 'green',
+00002f30: 2061 7474 7273 3d5b 2762 6f6c 6427 5d29   attrs=['bold'])
+00002f40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002f50: 2020 6370 7269 6e74 2866 223e 2049 2068    cprint(f"> I h
+00002f60: 6176 6520 6765 6e65 7261 7465 6420 7468  ave generated th
+00002f70: 6520 666f 6c6c 6f77 696e 6720 636f 6465  e following code
+00002f80: 3a5c 6e7b 636f 6465 7d5c 6e22 2c20 2767  :\n{code}\n", 'g
+00002f90: 7265 656e 272c 2061 7474 7273 3d5b 2762  reen', attrs=['b
+00002fa0: 6f6c 6427 5d29 0d0a 2020 2020 2020 2020  old'])..        
+00002fb0: 2020 2020 2020 2020 6370 7269 6e74 2866          cprint(f
+00002fc0: 223e 2046 696e 616c 2054 686f 7567 6874  "> Final Thought
+00002fd0: 733a 5c6e 7b72 6566 6c65 6374 696f 6e7d  s:\n{reflection}
+00002fe0: 5c6e 222c 2027 6772 6565 6e27 2c20 6174  \n", 'green', at
+00002ff0: 7472 733d 5b27 626f 6c64 275d 290d 0a20  trs=['bold']).. 
+00003000: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00003010: 7072 696e 7428 6622 3e20 546f 7461 6c20  print(f"> Total 
+00003020: 746f 6b65 6e73 2075 7365 643a 5c6e 7b74  tokens used:\n{t
+00003030: 6f74 616c 5f74 6f6b 656e 735f 7573 6564  otal_tokens_used
+00003040: 5f73 756d 7d5c 6e22 2c20 2779 656c 6c6f  _sum}\n", 'yello
+00003050: 7727 2c20 6174 7472 733d 5b27 626f 6c64  w', attrs=['bold
+00003060: 275d 290d 0a0d 0a20 2020 2020 2020 2023  '])....        #
+00003070: 2049 6620 6120 7175 6573 7469 6f6e 2069   If a question i
+00003080: 7320 7072 6f76 6964 6564 2c20 736b 6970  s provided, skip
+00003090: 2074 6865 2069 6e70 7574 2070 726f 6d70   the input promp
+000030a0: 740d 0a20 2020 2020 2020 2069 6620 7175  t..        if qu
+000030b0: 6573 7469 6f6e 2069 7320 6e6f 7420 4e6f  estion is not No
+000030c0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+000030d0: 2023 2043 616c 6c20 7468 6520 7461 736b   # Call the task
+000030e0: 5f65 7661 6c20 6d65 7468 6f64 2077 6974  _eval method wit
+000030f0: 6820 7468 6520 7573 6572 2773 2071 7565  h the user's que
+00003100: 7374 696f 6e0d 0a20 2020 2020 2020 2020  stion..         
+00003110: 2020 2074 6173 6b20 3d20 7365 6c66 2e74     task = self.t
+00003120: 6173 6b5f 6576 616c 2871 7565 7374 696f  ask_eval(questio
+00003130: 6e29 0d0a 2020 2020 2020 2020 2020 2020  n)..            
+00003140: 2320 4361 6c6c 2074 6865 2070 645f 6167  # Call the pd_ag
+00003150: 656e 7420 6d65 7468 6f64 2077 6974 6820  ent method with 
+00003160: 7468 6520 7573 6572 2773 2071 7565 7374  the user's quest
+00003170: 696f 6e2c 2074 6865 206d 6573 7361 6765  ion, the message
+00003180: 7320 6c69 7374 2c20 616e 6420 7468 6520  s list, and the 
+00003190: 6461 7461 6672 616d 650d 0a20 2020 2020  dataframe..     
+000031a0: 2020 2020 2020 2061 6e73 7765 722c 2063         answer, c
+000031b0: 6f64 652c 2072 6566 6c65 6374 696f 6e2c  ode, reflection,
+000031c0: 2066 6c6f 772c 2074 6f74 616c 5f74 6f6b   flow, total_tok
+000031d0: 656e 735f 7573 6564 5f73 756d 203d 2073  ens_used_sum = s
+000031e0: 656c 662e 7064 5f61 6765 6e74 2874 6173  elf.pd_agent(tas
+000031f0: 6b2c 206d 6573 7361 6765 732c 2073 656c  k, messages, sel
+00003200: 662e 6466 290d 0a20 2020 2020 2020 2020  f.df)..         
+00003210: 2020 2064 6973 706c 6179 5f72 6573 756c     display_resul
+00003220: 7473 2861 6e73 7765 722c 2063 6f64 652c  ts(answer, code,
+00003230: 2072 6566 6c65 6374 696f 6e2c 2066 6c6f   reflection, flo
+00003240: 772c 2074 6f74 616c 5f74 6f6b 656e 735f  w, total_tokens_
+00003250: 7573 6564 5f73 756d 290d 0a20 2020 2020  used_sum)..     
+00003260: 2020 2020 2020 2072 6574 7572 6e0d 0a0d         return...
+00003270: 0a20 2020 2020 2020 2023 2053 7461 7274  .        # Start
+00003280: 2061 6e20 696e 6669 6e69 7465 206c 6f6f   an infinite loo
+00003290: 7020 746f 206b 6565 7020 6173 6b69 6e67  p to keep asking
+000032a0: 2074 6865 2075 7365 7220 666f 7220 7175   the user for qu
+000032b0: 6573 7469 6f6e 730d 0a20 2020 2020 2020  estions..       
+000032c0: 2077 6869 6c65 2054 7275 653a 0d0a 2020   while True:..  
+000032d0: 2020 2020 2020 2020 2020 2320 5072 6f6d            # Prom
+000032e0: 7074 2074 6865 2075 7365 7220 746f 2065  pt the user to e
+000032f0: 6e74 6572 2061 2071 7565 7374 696f 6e20  nter a question 
+00003300: 6f72 2074 7970 6520 2765 7869 7427 2074  or type 'exit' t
+00003310: 6f20 7175 6974 0d0a 2020 2020 2020 2020  o quit..        
+00003320: 2020 2020 6966 2027 6970 796b 6572 6e65      if 'ipykerne
+00003330: 6c27 2069 6e20 7379 732e 6d6f 6475 6c65  l' in sys.module
+00003340: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00003350: 2020 2020 6469 7370 6c61 7928 4854 4d4c      display(HTML
+00003360: 2827 3c62 2073 7479 6c65 3d22 636f 6c6f  ('<b style="colo
+00003370: 723a 626c 7565 3b22 3e45 6e74 6572 2079  r:blue;">Enter y
+00003380: 6f75 7220 7175 6573 7469 6f6e 206f 7220  our question or 
+00003390: 7479 7065 205c 2765 7869 745c 2720 746f  type \'exit\' to
+000033a0: 2071 7569 743a 3c2f 623e 2729 290d 0a20   quit:</b>')).. 
+000033b0: 2020 2020 2020 2020 2020 2020 2020 2071                 q
+000033c0: 7565 7374 696f 6e20 3d20 696e 7075 7428  uestion = input(
+000033d0: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
+000033e0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+000033f0: 2020 2020 2020 6370 7269 6e74 2822 5c6e        cprint("\n
+00003400: 456e 7465 7220 796f 7572 2071 7565 7374  Enter your quest
+00003410: 696f 6e20 6f72 2074 7970 6520 2765 7869  ion or type 'exi
+00003420: 7427 2074 6f20 7175 6974 3a22 2c20 2762  t' to quit:", 'b
+00003430: 6c75 6527 2c20 6174 7472 733d 5b27 626f  lue', attrs=['bo
+00003440: 6c64 275d 290d 0a20 2020 2020 2020 2020  ld'])..         
+00003450: 2020 2020 2020 2071 7565 7374 696f 6e20         question 
+00003460: 3d20 696e 7075 7428 290d 0a0d 0a20 2020  = input()....   
+00003470: 2020 2020 2020 2020 2023 2049 6620 7468           # If th
+00003480: 6520 7573 6572 2074 7970 6573 2027 6578  e user types 'ex
+00003490: 6974 272c 2062 7265 616b 206f 7574 206f  it', break out o
+000034a0: 6620 7468 6520 6c6f 6f70 0d0a 2020 2020  f the loop..    
+000034b0: 2020 2020 2020 2020 6966 2071 7565 7374          if quest
+000034c0: 696f 6e2e 7374 7269 7028 292e 6c6f 7765  ion.strip().lowe
+000034d0: 7228 2920 3d3d 2027 6578 6974 273a 0d0a  r() == 'exit':..
+000034e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034f0: 6272 6561 6b0d 0a20 2020 2020 2020 2020  break..         
+00003500: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00003510: 2023 2043 616c 6c20 7468 6520 7461 736b   # Call the task
+00003520: 5f65 7661 6c20 6d65 7468 6f64 2077 6974  _eval method wit
+00003530: 6820 7468 6520 7573 6572 2773 2071 7565  h the user's que
+00003540: 7374 696f 6e0d 0a20 2020 2020 2020 2020  stion..         
+00003550: 2020 2074 6173 6b20 3d20 7365 6c66 2e74     task = self.t
+00003560: 6173 6b5f 6576 616c 2871 7565 7374 696f  ask_eval(questio
+00003570: 6e29 0d0a 2020 2020 2020 2020 2020 2020  n)..            
+00003580: 2320 4361 6c6c 2074 6865 2070 645f 6167  # Call the pd_ag
+00003590: 656e 7420 6d65 7468 6f64 2077 6974 6820  ent method with 
+000035a0: 7468 6520 7573 6572 2773 2071 7565 7374  the user's quest
+000035b0: 696f 6e2c 2074 6865 206d 6573 7361 6765  ion, the message
+000035c0: 7320 6c69 7374 2c20 616e 6420 7468 6520  s list, and the 
+000035d0: 6461 7461 6672 616d 650d 0a20 2020 2020  dataframe..     
+000035e0: 2020 2020 2020 2061 6e73 7765 722c 2063         answer, c
+000035f0: 6f64 652c 2072 6566 6c65 6374 696f 6e2c  ode, reflection,
+00003600: 2066 6c6f 772c 2074 6f74 616c 5f74 6f6b   flow, total_tok
+00003610: 656e 735f 7573 6564 5f73 756d 203d 2073  ens_used_sum = s
+00003620: 656c 662e 7064 5f61 6765 6e74 2874 6173  elf.pd_agent(tas
+00003630: 6b2c 206d 6573 7361 6765 732c 2073 656c  k, messages, sel
+00003640: 662e 6466 290d 0a20 2020 2020 2020 2020  f.df)..         
+00003650: 2020 2064 6973 706c 6179 5f72 6573 756c     display_resul
+00003660: 7473 2861 6e73 7765 722c 2063 6f64 652c  ts(answer, code,
+00003670: 2072 6566 6c65 6374 696f 6e2c 666c 6f77   reflection,flow
+00003680: 2c20 746f 7461 6c5f 746f 6b65 6e73 5f75  , total_tokens_u
+00003690: 7365 645f 7375 6d29 0d0a 0d0a 2020 2020  sed_sum)....    
+000036a0: 6465 6620 7064 5f61 6765 6e74 2873 656c  def pd_agent(sel
+000036b0: 662c 2071 7565 7374 696f 6e2c 206d 6573  f, question, mes
+000036c0: 7361 6765 732c 2064 663d 4e6f 6e65 293a  sages, df=None):
+000036d0: 0d0a 2020 2020 2020 2020 2320 4164 6420  ..        # Add 
+000036e0: 6120 7573 6572 206d 6573 7361 6765 2077  a user message w
+000036f0: 6974 6820 7468 6520 7570 6461 7465 6420  ith the updated 
+00003700: 7461 736b 2070 726f 6d70 7420 746f 2074  task prompt to t
+00003710: 6865 206d 6573 7361 6765 7320 6c69 7374  he messages list
+00003720: 0d0a 2020 2020 2020 2020 6d65 7373 6167  ..        messag
+00003730: 6573 2e61 7070 656e 6428 7b22 726f 6c65  es.append({"role
+00003740: 223a 2022 7573 6572 222c 2022 636f 6e74  ": "user", "cont
+00003750: 656e 7422 3a20 7365 6c66 2e74 6173 6b2e  ent": self.task.
+00003760: 666f 726d 6174 2873 656c 662e 6466 5f68  format(self.df_h
+00003770: 6561 642c 2071 7565 7374 696f 6e29 7d29  ead, question)})
+00003780: 0d0a 0d0a 2020 2020 2020 2020 6966 2027  ....        if '
+00003790: 6970 796b 6572 6e65 6c27 2069 6e20 7379  ipykernel' in sy
+000037a0: 732e 6d6f 6475 6c65 733a 0d0a 2020 2020  s.modules:..    
+000037b0: 2020 2020 2020 2020 2320 4a75 7079 7465          # Jupyte
+000037c0: 7220 6e6f 7465 626f 6f6b 206f 7220 6970  r notebook or ip
+000037d0: 7974 686f 6e0d 0a20 2020 2020 2020 2020  ython..         
+000037e0: 2020 2064 6973 706c 6179 2848 544d 4c28     display(HTML(
+000037f0: 6627 3c70 2073 7479 6c65 3d22 636f 6c6f  f'<p style="colo
+00003800: 723a 6d61 6765 6e74 613b 223e 5c6e 5573  r:magenta;">\nUs
+00003810: 696e 6720 4d6f 6465 6c3a 207b 7365 6c66  ing Model: {self
+00003820: 2e6c 6c6d 7d3c 2f70 3e27 2929 0d0a 2020  .llm}</p>'))..  
+00003830: 2020 2020 2020 2020 2020 6469 7370 6c61            displa
+00003840: 7928 4854 4d4c 2866 273c 703e 3c62 2073  y(HTML(f'<p><b s
+00003850: 7479 6c65 3d22 636f 6c6f 723a 6d61 6765  tyle="color:mage
+00003860: 6e74 613b 223e 5072 6f63 6573 7369 6e67  nta;">Processing
+00003870: 2079 6f75 7220 7265 7175 6573 742c 2070   your request, p
+00003880: 6c65 6173 6520 7761 6974 2e2e 2e3c 2f62  lease wait...</b
+00003890: 3e3c 2f70 3e3c 6272 3e27 2929 0d0a 2020  ></p><br>'))..  
+000038a0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+000038b0: 2020 2020 2020 2020 2023 204f 7468 6572           # Other
+000038c0: 2065 6e76 6972 6f6e 6d65 6e74 2028 6c69   environment (li
+000038d0: 6b65 2074 6572 6d69 6e61 6c29 0d0a 2020  ke terminal)..  
+000038e0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+000038f0: 636f 6c6f 7265 6428 6622 5c6e 3e20 5573  colored(f"\n> Us
+00003900: 696e 6720 4d6f 6465 6c3a 207b 7365 6c66  ing Model: {self
+00003910: 2e6c 6c6d 7d22 2c20 226d 6167 656e 7461  .llm}", "magenta
+00003920: 2229 290d 0a20 2020 2020 2020 2020 2020  "))..           
+00003930: 2063 7072 696e 7428 6622 5c6e 3e20 5072   cprint(f"\n> Pr
+00003940: 6f63 6573 7369 6e67 2079 6f75 7220 7265  ocessing your re
+00003950: 7175 6573 742c 2070 6c65 6173 6520 7761  quest, please wa
+00003960: 6974 2e2e 2e5c 6e22 2c20 276d 6167 656e  it...\n", 'magen
+00003970: 7461 272c 2061 7474 7273 3d5b 2762 6f6c  ta', attrs=['bol
+00003980: 6427 5d29 0d0a 0d0a 2020 2020 2020 2020  d'])....        
+00003990: 2320 4361 6c6c 2074 6865 204f 7065 6e41  # Call the OpenA
+000039a0: 4920 4150 4920 616e 6420 6861 6e64 6c65  I API and handle
+000039b0: 2072 6174 6520 6c69 6d69 7420 6572 726f   rate limit erro
+000039c0: 7273 0d0a 2020 2020 2020 2020 7472 793a  rs..        try:
+000039d0: 0d0a 2020 2020 2020 2020 2020 2020 6c6c  ..            ll
+000039e0: 6d5f 7265 7370 6f6e 7365 2c20 746f 6b65  m_response, toke
+000039f0: 6e73 5f75 7365 6420 3d20 7365 6c66 2e6c  ns_used = self.l
+00003a00: 6c6d 5f63 616c 6c28 6d65 7373 6167 6573  lm_call(messages
+00003a10: 290d 0a20 2020 2020 2020 2065 7863 6570  )..        excep
+00003a20: 7420 6f70 656e 6169 2e65 7272 6f72 2e52  t openai.error.R
+00003a30: 6174 654c 696d 6974 4572 726f 723a 0d0a  ateLimitError:..
+00003a40: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00003a50: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
+00003a60: 2020 2020 2254 6865 204f 7065 6e41 4920      "The OpenAI 
+00003a70: 4150 4920 7261 7465 206c 696d 6974 2068  API rate limit h
+00003a80: 6173 2062 6565 6e20 6578 6365 6564 6564  as been exceeded
+00003a90: 2e20 5761 6974 696e 6720 3130 2073 6563  . Waiting 10 sec
+00003aa0: 6f6e 6473 2061 6e64 2074 7279 696e 6720  onds and trying 
+00003ab0: 6167 6169 6e2e 220d 0a20 2020 2020 2020  again."..       
+00003ac0: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+00003ad0: 2020 2020 7469 6d65 2e73 6c65 6570 2831      time.sleep(1
+00003ae0: 3029 0d0a 2020 2020 2020 2020 2020 2020  0)..            
+00003af0: 6c6c 6d5f 7265 7370 6f6e 7365 2c20 746f  llm_response, to
+00003b00: 6b65 6e73 5f75 7365 6420 3d20 7365 6c66  kens_used = self
+00003b10: 2e6c 6c6d 5f63 616c 6c28 6d65 7373 6167  .llm_call(messag
+00003b20: 6573 290d 0a0d 0a20 2020 2020 2020 2023  es)....        #
+00003b30: 2045 7874 7261 6374 2074 6865 2063 6f64   Extract the cod
+00003b40: 6520 6672 6f6d 2074 6865 2041 5049 2072  e from the API r
+00003b50: 6573 706f 6e73 650d 0a20 2020 2020 2020  esponse..       
+00003b60: 2063 6f64 652c 7265 666c 6563 7469 6f6e   code,reflection
+00003b70: 2c66 6c6f 7720 3d20 7365 6c66 2e5f 6578  ,flow = self._ex
+00003b80: 7472 6163 745f 636f 6465 286c 6c6d 5f72  tract_code(llm_r
+00003b90: 6573 706f 6e73 6529 0d0a 0d0a 2020 2020  esponse)....    
+00003ba0: 2020 2020 2320 5570 6461 7465 2074 6865      # Update the
+00003bb0: 2074 6f74 616c 2074 6f6b 656e 7320 7573   total tokens us
+00003bc0: 6564 0d0a 2020 2020 2020 2020 7365 6c66  ed..        self
+00003bd0: 2e74 6f74 616c 5f74 6f6b 656e 735f 7573  .total_tokens_us
+00003be0: 6564 2e61 7070 656e 6428 746f 6b65 6e73  ed.append(tokens
+00003bf0: 5f75 7365 6429 0d0a 2020 2020 2020 2020  _used)..        
+00003c00: 746f 7461 6c5f 746f 6b65 6e73 5f75 7365  total_tokens_use
+00003c10: 645f 7375 6d20 3d20 7375 6d28 7365 6c66  d_sum = sum(self
+00003c20: 2e74 6f74 616c 5f74 6f6b 656e 735f 7573  .total_tokens_us
+00003c30: 6564 290d 0a0d 0a20 2020 2020 2020 2023  ed)....        #
+00003c40: 2049 6e69 7469 616c 697a 6520 6572 726f   Initialize erro
+00003c50: 7220 636f 7272 6563 7469 6f6e 2063 6f75  r correction cou
+00003c60: 6e74 6572 0d0a 2020 2020 2020 2020 6572  nter..        er
+00003c70: 726f 725f 636f 7272 6563 7469 6f6e 7320  ror_corrections 
+00003c80: 3d20 300d 0a0d 0a20 2020 2020 2020 2023  = 0....        #
+00003c90: 2053 746f 7265 2074 6865 206f 7269 6769   Store the origi
+00003ca0: 6e61 6c20 6c6c 6d20 7661 6c75 650d 0a20  nal llm value.. 
+00003cb0: 2020 2020 2020 206f 7269 6769 6e61 6c5f         original_
+00003cc0: 6c6c 6d20 3d20 7365 6c66 2e6c 6c6d 0d0a  llm = self.llm..
+00003cd0: 0d0a 2020 2020 2020 2020 2320 5265 6469  ..        # Redi
+00003ce0: 7265 6374 2073 7461 6e64 6172 6420 6f75  rect standard ou
+00003cf0: 7470 7574 2074 6f20 6120 5374 7269 6e67  tput to a String
+00003d00: 494f 2062 7566 6665 720d 0a20 2020 2020  IO buffer..     
+00003d10: 2020 2077 6974 6820 7265 6469 7265 6374     with redirect
+00003d20: 5f73 7464 6f75 7428 696f 2e53 7472 696e  _stdout(io.Strin
+00003d30: 6749 4f28 2929 2061 7320 6f75 7470 7574  gIO()) as output
+00003d40: 3a0d 0a20 2020 2020 2020 2020 2020 2023  :..            #
+00003d50: 2054 7279 2074 6f20 6578 6563 7574 6520   Try to execute 
+00003d60: 7468 6520 636f 6465 2061 6e64 2068 616e  the code and han
+00003d70: 646c 6520 6572 726f 7273 0d0a 2020 2020  dle errors..    
+00003d80: 2020 2020 2020 2020 7768 696c 6520 6572          while er
+00003d90: 726f 725f 636f 7272 6563 7469 6f6e 7320  ror_corrections 
+00003da0: 3c20 7365 6c66 2e4d 4158 5f45 5252 4f52  < self.MAX_ERROR
+00003db0: 5f43 4f52 5245 4354 494f 4e53 3a0d 0a20  _CORRECTIONS:.. 
+00003dc0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00003dd0: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
+00003de0: 2020 2020 2020 2020 206d 6573 7361 6765           message
+00003df0: 732e 6170 7065 6e64 287b 2272 6f6c 6522  s.append({"role"
+00003e00: 3a20 2261 7373 6973 7461 6e74 222c 2022  : "assistant", "
+00003e10: 636f 6e74 656e 7422 3a20 6c6c 6d5f 7265  content": llm_re
+00003e20: 7370 6f6e 7365 7d29 0d0a 2020 2020 2020  sponse})..      
+00003e30: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00003e40: 5265 6d6f 7665 2074 6865 206f 6c64 6573  Remove the oldes
+00003e50: 7420 636f 6e76 6572 7361 7469 6f6e 2066  t conversation f
+00003e60: 726f 6d20 7468 6520 6d65 7373 6167 6573  rom the messages
+00003e70: 206c 6973 740d 0a20 2020 2020 2020 2020   list..         
+00003e80: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+00003e90: 6e28 6d65 7373 6167 6573 2920 3e20 7365  n(messages) > se
+00003ea0: 6c66 2e4d 4158 5f43 4f4e 5645 5253 4154  lf.MAX_CONVERSAT
+00003eb0: 494f 4e53 3a0d 0a20 2020 2020 2020 2020  IONS:..         
+00003ec0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00003ed0: 6573 7361 6765 732e 706f 7028 3129 0d0a  essages.pop(1)..
+00003ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ef0: 2020 2020 2020 2020 6d65 7373 6167 6573          messages
+00003f00: 2e70 6f70 2831 290d 0a20 2020 2020 2020  .pop(1)..       
+00003f10: 2020 2020 2020 2020 2020 2020 2023 2052               # R
+00003f20: 6573 6574 2064 6620 746f 2074 6865 206f  eset df to the o
+00003f30: 7269 6769 6e61 6c20 7374 6174 6520 6265  riginal state be
+00003f40: 666f 7265 2065 7865 6375 7469 6e67 2074  fore executing t
+00003f50: 6865 2063 6f64 650d 0a20 2020 2020 2020  he code..       
+00003f60: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00003f70: 662e 6466 203d 2073 656c 662e 6f72 6967  f.df = self.orig
+00003f80: 696e 616c 5f64 662e 636f 7079 2829 0d0a  inal_df.copy()..
+00003f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003fa0: 2020 2020 2320 4578 6563 7574 6520 7468      # Execute th
+00003fb0: 6520 636f 6465 0d0a 2020 2020 2020 2020  e code..        
+00003fc0: 2020 2020 2020 2020 2020 2020 6966 2063              if c
+00003fd0: 6f64 6520 6973 206e 6f74 204e 6f6e 653a  ode is not None:
+00003fe0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003ff0: 2020 2020 2020 2020 2020 6578 6563 2863            exec(c
+00004000: 6f64 6529 0d0a 2020 2020 2020 2020 2020  ode)..          
+00004010: 2020 2020 2020 2020 2020 6272 6561 6b0d            break.
+00004020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004030: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+00004040: 6e20 6173 2065 3a0d 0a20 2020 2020 2020  n as e:..       
+00004050: 2020 2020 2020 2020 2020 2020 2023 2050               # P
+00004060: 7269 6e74 2074 6865 2065 7272 6f72 206d  rint the error m
+00004070: 6573 7361 6765 0d0a 2020 2020 2020 2020  essage..        
+00004080: 2020 2020 2020 2020 2020 2020 6966 2027              if '
+00004090: 6970 796b 6572 6e65 6c27 2069 6e20 7379  ipykernel' in sy
+000040a0: 732e 6d6f 6475 6c65 733a 0d0a 2020 2020  s.modules:..    
+000040b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000040c0: 2020 2020 2320 4a75 7079 7465 7220 6e6f      # Jupyter no
+000040d0: 7465 626f 6f6b 0d0a 2020 2020 2020 2020  tebook..        
+000040e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000040f0: 6469 7370 6c61 7928 4854 4d4c 2866 273c  display(HTML(f'<
+00004100: 623e 3c73 7061 6e20 7374 796c 653d 2263  b><span style="c
+00004110: 6f6c 6f72 3a20 7265 643b 223e 4572 726f  olor: red;">Erro
+00004120: 723a 3c62 723e 3c70 7265 3e7b 657d 3c2f  r:<br><pre>{e}</
+00004130: 7072 653e 3c62 723e 5468 616e 6b73 2066  pre><br>Thanks f
+00004140: 6f72 2074 6865 2066 6565 6462 6163 6b2e  or the feedback.
+00004150: 2049 2061 6d20 676f 696e 6720 746f 2072   I am going to r
+00004160: 6566 6c65 6374 206f 6e20 7468 6520 6572  eflect on the er
+00004170: 726f 7220 616e 6420 7265 7472 792e 3c2f  ror and retry.</
+00004180: 7370 616e 3e3c 2f62 3e27 2929 0d0a 2020  span></b>'))..  
+00004190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000041a0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+000041b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000041c0: 2023 2043 4c49 0d0a 2020 2020 2020 2020   # CLI..        
+000041d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000041e0: 7072 696e 7428 636f 6c6f 7265 6428 6627  print(colored(f'
+000041f0: 4572 726f 723a 207b 657d 2e20 3e20 5468  Error: {e}. > Th
+00004200: 616e 6b73 2066 6f72 2074 6865 2066 6565  anks for the fee
+00004210: 6462 6163 6b2e 2049 2061 6d20 676f 696e  dback. I am goin
+00004220: 6720 746f 2072 6566 6c65 6374 206f 6e20  g to reflect on 
+00004230: 7468 6520 6572 726f 7220 616e 6420 7265  the error and re
+00004240: 7472 792e 272c 2027 7265 6427 2929 0d0a  try.', 'red'))..
+00004250: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004260: 2020 2020 2020 2320 496e 6372 656d 656e        # Incremen
+00004270: 7420 7468 6520 6572 726f 7220 636f 7272  t the error corr
+00004280: 6563 7469 6f6e 2063 6f75 6e74 6572 2061  ection counter a
+00004290: 6e64 2075 7064 6174 6520 7468 6520 6d65  nd update the me
+000042a0: 7373 6167 6573 206c 6973 7420 7769 7468  ssages list with
+000042b0: 2074 6865 2065 7272 6f72 0d0a 2020 2020   the error..    
+000042c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000042d0: 6572 726f 725f 636f 7272 6563 7469 6f6e  error_correction
+000042e0: 7320 2b3d 2031 0d0a 2020 2020 2020 2020  s += 1..        
+000042f0: 2020 2020 2020 2020 2020 2020 6d65 7373              mess
+00004300: 6167 6573 2e61 7070 656e 6428 7b22 726f  ages.append({"ro
+00004310: 6c65 223a 2022 7573 6572 222c 2022 636f  le": "user", "co
+00004320: 6e74 656e 7422 3a20 7365 6c66 2e65 7272  ntent": self.err
+00004330: 6f72 5f63 6f72 7265 6374 5f74 6173 6b2e  or_correct_task.
+00004340: 666f 726d 6174 2865 2c20 636f 6465 2c20  format(e, code, 
+00004350: 7175 6573 7469 6f6e 297d 290d 0a0d 0a20  question)}).... 
+00004360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004370: 2020 2023 2053 7769 7463 6820 746f 2067     # Switch to g
+00004380: 7074 2d34 2069 6620 6c6c 6d5f 7377 6974  pt-4 if llm_swit
+00004390: 6368 2069 7320 5472 7565 0d0a 2020 2020  ch is True..    
+000043a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000043b0: 6966 2073 656c 662e 6c6c 6d5f 7377 6974  if self.llm_swit
+000043c0: 6368 3a0d 0a20 2020 2020 2020 2020 2020  ch:..           
+000043d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000043e0: 662e 6c6c 6d20 3d20 2767 7074 2d34 270d  f.llm = 'gpt-4'.
+000043f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004400: 2020 2020 2020 2020 2069 6620 2769 7079           if 'ipy
+00004410: 6b65 726e 656c 2720 696e 2073 7973 2e6d  kernel' in sys.m
+00004420: 6f64 756c 6573 3a0d 0a20 2020 2020 2020  odules:..       
+00004430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004440: 2020 2020 2023 204a 7570 7974 6572 206e       # Jupyter n
+00004450: 6f74 6562 6f6f 6b0d 0a20 2020 2020 2020  otebook..       
+00004460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004470: 2020 2020 2064 6973 706c 6179 2848 544d       display(HTM
+00004480: 4c28 273c 7370 616e 2073 7479 6c65 3d22  L('<span style="
+00004490: 636f 6c6f 723a 2072 6564 3b22 3e53 7769  color: red;">Swi
+000044a0: 7463 6869 6e67 206d 6f64 656c 2074 6f20  tching model to 
+000044b0: 6770 742d 3420 746f 2074 7279 2074 6f20  gpt-4 to try to 
+000044c0: 696d 7072 6f76 6520 7468 6520 6f75 7463  improve the outc
+000044d0: 6f6d 652e 3c2f 7370 616e 3e27 2929 0d0a  ome.</span>'))..
+000044e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044f0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00004500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004510: 2020 2020 2020 2020 2020 2023 2043 4c49             # CLI
+00004520: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004530: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00004540: 696e 7428 636f 6c6f 7265 6428 273e 2053  int(colored('> S
+00004550: 7769 7463 6869 6e67 206d 6f64 656c 2074  witching model t
+00004560: 6f20 6770 742d 3420 746f 2074 7279 2074  o gpt-4 to try t
+00004570: 6f20 696d 7072 6f76 6520 7468 6520 6f75  o improve the ou
+00004580: 7463 6f6d 652e 272c 2027 7265 6427 2929  tcome.', 'red'))
+00004590: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000045a0: 2020 2020 2020 2020 2320 4174 7465 6d70          # Attemp
+000045b0: 7420 746f 2063 6f72 7265 6374 2074 6865  t to correct the
+000045c0: 2063 6f64 6520 616e 6420 6861 6e64 6c65   code and handle
+000045d0: 2072 6174 6520 6c69 6d69 7420 6572 726f   rate limit erro
+000045e0: 7273 0d0a 2020 2020 2020 2020 2020 2020  rs..            
+000045f0: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
+00004600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004610: 2020 2020 2020 6c6c 6d5f 7265 7370 6f6e        llm_respon
+00004620: 7365 2c20 746f 6b65 6e73 5f75 7365 6420  se, tokens_used 
+00004630: 3d20 7365 6c66 2e6c 6c6d 5f63 616c 6c28  = self.llm_call(
+00004640: 6d65 7373 6167 6573 290d 0a20 2020 2020  messages)..     
+00004650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004660: 2020 2063 6f64 652c 7265 666c 6563 7469     code,reflecti
+00004670: 6f6e 2c66 6c6f 7720 3d20 7365 6c66 2e5f  on,flow = self._
+00004680: 6578 7472 6163 745f 636f 6465 286c 6c6d  extract_code(llm
+00004690: 5f72 6573 706f 6e73 6529 0d0a 2020 2020  _response)..    
+000046a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046b0: 2020 2020 7365 6c66 2e74 6f74 616c 5f74      self.total_t
+000046c0: 6f6b 656e 735f 7573 6564 2e61 7070 656e  okens_used.appen
+000046d0: 6428 746f 6b65 6e73 5f75 7365 6429 0d0a  d(tokens_used)..
+000046e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046f0: 2020 2020 2020 2020 746f 7461 6c5f 746f          total_to
+00004700: 6b65 6e73 5f75 7365 645f 7375 6d20 3d20  kens_used_sum = 
+00004710: 7375 6d28 7365 6c66 2e74 6f74 616c 5f74  sum(self.total_t
+00004720: 6f6b 656e 735f 7573 6564 290d 0a20 2020  okens_used)..   
+00004730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004740: 2065 7863 6570 7420 6f70 656e 6169 2e65   except openai.e
+00004750: 7272 6f72 2e52 6174 654c 696d 6974 4572  rror.RateLimitEr
+00004760: 726f 723a 0d0a 2020 2020 2020 2020 2020  ror:..          
+00004770: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00004780: 696e 7428 0d0a 2020 2020 2020 2020 2020  int(..          
+00004790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047a0: 2020 2254 6865 204f 7065 6e41 4920 4150    "The OpenAI AP
+000047b0: 4920 7261 7465 206c 696d 6974 2068 6173  I rate limit has
+000047c0: 2062 6565 6e20 6578 6365 6564 6564 2e20   been exceeded. 
+000047d0: 5761 6974 696e 6720 3130 2073 6563 6f6e  Waiting 10 secon
+000047e0: 6473 2061 6e64 2074 7279 696e 6720 6167  ds and trying ag
+000047f0: 6169 6e2e 220d 0a20 2020 2020 2020 2020  ain."..         
+00004800: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00004810: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004820: 2020 2020 2020 2020 2020 7469 6d65 2e73            time.s
+00004830: 6c65 6570 2831 3029 0d0a 2020 2020 2020  leep(10)..      
+00004840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004850: 2020 6c6c 6d5f 7265 7370 6f6e 7365 2c20    llm_response, 
+00004860: 746f 6b65 6e73 5f75 7365 6420 3d20 7365  tokens_used = se
+00004870: 6c66 2e6c 6c6d 5f63 616c 6c28 6d65 7373  lf.llm_call(mess
+00004880: 6167 6573 290d 0a20 2020 2020 2020 2020  ages)..         
+00004890: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000048a0: 6f64 652c 7265 666c 6563 7469 6f6e 2c66  ode,reflection,f
+000048b0: 6c6f 7720 3d20 7365 6c66 2e5f 6578 7472  low = self._extr
+000048c0: 6163 745f 636f 6465 286c 6c6d 5f72 6573  act_code(llm_res
+000048d0: 706f 6e73 6529 0d0a 2020 2020 2020 2020  ponse)..        
+000048e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048f0: 7365 6c66 2e74 6f74 616c 5f74 6f6b 656e  self.total_token
+00004900: 735f 7573 6564 2e61 7070 656e 6428 746f  s_used.append(to
+00004910: 6b65 6e73 5f75 7365 6429 0d0a 2020 2020  kens_used)..    
+00004920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004930: 2020 2020 746f 7461 6c5f 746f 6b65 6e73      total_tokens
+00004940: 5f75 7365 645f 7375 6d20 3d20 7375 6d28  _used_sum = sum(
+00004950: 7365 6c66 2e74 6f74 616c 5f74 6f6b 656e  self.total_token
+00004960: 735f 7573 6564 290d 0a0d 0a20 2020 2020  s_used)....     
+00004970: 2020 2020 2020 2023 2053 7769 7463 6820         # Switch 
+00004980: 6261 636b 2074 6f20 7468 6520 6f72 6967  back to the orig
+00004990: 696e 616c 206c 6c6d 2062 6566 6f72 6520  inal llm before 
+000049a0: 7468 6520 6675 6e63 7469 6f6e 2066 696e  the function fin
+000049b0: 6973 6865 730d 0a20 2020 2020 2020 2020  ishes..         
+000049c0: 2020 2073 656c 662e 6c6c 6d20 3d20 6f72     self.llm = or
+000049d0: 6967 696e 616c 5f6c 6c6d 0d0a 0d0a 2020  iginal_llm....  
+000049e0: 2020 2020 2020 2320 4765 7420 7468 6520        # Get the 
+000049f0: 6f75 7470 7574 2066 726f 6d20 7468 6520  output from the 
+00004a00: 6578 6563 7574 6564 2063 6f64 650d 0a20  executed code.. 
+00004a10: 2020 2020 2020 2061 6e73 7765 7220 3d20         answer = 
+00004a20: 6f75 7470 7574 2e67 6574 7661 6c75 6528  output.getvalue(
+00004a30: 290d 0a0d 0a20 2020 2020 2020 2023 2052  )....        # R
+00004a40: 6573 6574 2074 6865 2053 7472 696e 6749  eset the StringI
+00004a50: 4f20 6275 6666 6572 0d0a 2020 2020 2020  O buffer..      
+00004a60: 2020 6f75 7470 7574 2e74 7275 6e63 6174    output.truncat
+00004a70: 6528 3029 0d0a 2020 2020 2020 2020 6f75  e(0)..        ou
+00004a80: 7470 7574 2e73 6565 6b28 3029 0d0a 0d0a  tput.seek(0)....
+00004a90: 2020 2020 2020 2020 7265 7475 726e 2061          return a
+00004aa0: 6e73 7765 722c 2063 6f64 652c 2072 6566  nswer, code, ref
+00004ab0: 6c65 6374 696f 6e2c 2066 6c6f 772c 2074  lection, flow, t
+00004ac0: 6f74 616c 5f74 6f6b 656e 735f 7573 6564  otal_tokens_used
+00004ad0: 5f73 756d 0d0a 2020 2020                 _sum..
```

### Comparing `bambooai-0.2.3/bambooai.egg-info/PKG-INFO` & `bambooai-0.2.4/bambooai.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambooai
-Version: 0.2.3
+Version: 0.2.4
 Summary: A lightweight library for working with pandas dataframes using natural language queries
 Home-page: UNKNOWN
 Author: Palo Galko
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -22,32 +22,28 @@
 
 ## Preview
 
 Try it out in Google Colab:
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1grKtqKD4u8cVGMoVv__umci4F7IU14vU?usp=sharing)
 
-
 ## How it works
 
-- User starts BambooAI
-- BambooAI checks if a question is provided
-  - If a question is given programmatically, it gets processed and the assistant exits after the execution
-  - If no question is provided programaticaly, BambooAI prompts the user for one and enters a loop of questions and answers, remembering the conversation history
-    - Sends each question to the OpenAI API LLM along with the conversation history
-    - Obtains a response with corresponding Python code
-    - Executes the code to generate an answer or visualization
-      - If the code works, it displays the answer or visualization, and then prompts for another question, which could be related to the preceding question or an entirely new topic
-      - If an error occurs, the program requests a corrected code from the OpenAI API by providing the error message and then attempts to execute the corrected code. *If the "llm_switch" argument is set to "True" (LLM cascading) it will switch from base model to a more powerfull gpt-4 and retry. After successfull execution it will reset back to base model.*
-  - The loop continues until the user enters 'exit', at which point the program terminates
-  - The program displays the total token usage at each step, providing insight into the resources consumed during the process.
-  
-**Flow chart:**
-
-![](images/flow_chart.png)
+- The user begins by starting the BambooAI agent.
+- BambooAI subsequently checks if a question has been provided:
+  - If a question is available, it continues to the next step.
+  - If no question is available, BambooAI prompts the user to input one. It then enters a loop of questions and answers, remembering the conversation history and continually prompting the user for a new question. This loop continues until the user types 'exit', signalling the termination of the program.
+- Following the reception of a question, the OpenAI API is called to review and evaluate the task. The Language Learning Model (LLM) then presents four possible analysis methods, choosing the one it deems most suitable. This selected method is summarised and framed as a task for a hypothetical junior data analyst.
+- The agent then replaces the original question with the task from the previous step and sends this as a prompt to the OpenAI API for code generation.
+- The response from the API, containing the corresponding Python code, is received, checked and sanitised if necessary.
+- This code is then executed to generate an answer or a visualization:
+  - If the code executes successfully, it displays the answer or visualization and subsequently prompts for another question. This new question could be related to the previous question or could be on an entirely new topic.
+  - If an error occurs during code execution, the program requests a corrected version of the code from the OpenAI API by providing the error message, and then attempts to execute the corrected code. *In cases where the "llm_switch" argument is set to "True" (indicating LLM cascading), the program will switch from the base model to the more powerful GPT-4 model for a retry. After successful execution, it will revert to the base model.*
+- The program then displays the total token usage at each step, thereby providing insights into the resources consumed during the process.
+ 
 
 ## How to use
 
 **Installation**
 
 ```
 pip install bambooai
@@ -100,27 +96,27 @@
 ```
 
 **Environment Variables**
 
 The library requires an OpenAI API account and the API key to connect to an OpenAI LLMs. The OpenAI API key needs to be stored in a 'OPENAI_API_KEY' environment variable.
 The key can be obtained from here: https://platform.openai.com/account/api-keys
 
+
 ## Notes
 
 - The library currently supports only OpenAI Chat models. It has been tested with both gpt-3.5-turbo and gpt-4. The gpt-3.5-turbo seems to perform well and is the preferred option due to its 10x lower cost.
 - The library executes LLM generated Python code, this can be bad if the LLM generated Python code is harmful. Use cautiously.
 - Be sure to monitor your token usage, as each execution of BambooAI uses an average of 400-600 tokens. At the time of writing, the cost per 1K tokens is $0.03 USD for GPT-4 and $0.002 USD for GPT-3.5-turbo. It's important to keep these costs in mind when using the library, particularly when using the more expensive models.
 - Currently the project consists of 126 lines of code, 49 lines of comments and 20 blanks.
 
 ## Contributing
 
 Contributions are welcome; please feel free to open a pull request. Keep in mind that our goal is to maintain a concise codebase with high readability.
 
 ## ToDo
 
-- Introduce memory limits.  A method for users to control the number of conversation pairs retained in memory and sent to the LLM during each iteration.
 - Ongoing work on optimizing the prompts and sanitization of the outputs.
 - Add abbility to inspect the LLM generated code before execution.
 - Add support for aditional LLMs.
```

