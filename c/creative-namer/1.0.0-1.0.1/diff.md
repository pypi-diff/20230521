# Comparing `tmp/creative-namer-1.0.0.tar.gz` & `tmp/creative-namer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "creative-namer-1.0.0.tar", last modified: Sat May 20 12:08:52 2023, max compression
+gzip compressed data, was "creative-namer-1.0.1.tar", last modified: Sat May 20 12:37:02 2023, max compression
```

## Comparing `creative-namer-1.0.0.tar` & `creative-namer-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-20 12:08:52.015135 creative-namer-1.0.0/
--rw-r--r--   0 chiubowen   (501) staff       (20)     1506 2023-05-20 12:08:52.015014 creative-namer-1.0.0/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     1334 2023-05-20 12:08:51.000000 creative-namer-1.0.0/README.md
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-20 12:08:52.014826 creative-namer-1.0.0/creative_namer.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     1506 2023-05-20 12:08:51.000000 creative-namer-1.0.0/creative_namer.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      266 2023-05-20 12:08:52.000000 creative-namer-1.0.0/creative_namer.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-20 12:08:51.000000 creative-namer-1.0.0/creative_namer.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       56 2023-05-20 12:08:51.000000 creative-namer-1.0.0/creative_namer.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       19 2023-05-20 12:08:51.000000 creative-namer-1.0.0/creative_namer.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       15 2023-05-20 12:08:51.000000 creative-namer-1.0.0/creative_namer.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     2826 2023-05-20 12:08:51.000000 creative-namer-1.0.0/creative_namer.py
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-20 12:08:52.015172 creative-namer-1.0.0/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      520 2023-05-20 12:08:51.000000 creative-namer-1.0.0/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-20 12:37:02.067996 creative-namer-1.0.1/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     2602 2023-05-20 12:37:02.067830 creative-namer-1.0.1/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     2430 2023-05-20 12:37:01.000000 creative-namer-1.0.1/README.md
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-20 12:37:02.067650 creative-namer-1.0.1/creative_namer.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     2602 2023-05-20 12:37:02.000000 creative-namer-1.0.1/creative_namer.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      266 2023-05-20 12:37:02.000000 creative-namer-1.0.1/creative_namer.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-20 12:37:02.000000 creative-namer-1.0.1/creative_namer.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       56 2023-05-20 12:37:02.000000 creative-namer-1.0.1/creative_namer.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       19 2023-05-20 12:37:02.000000 creative-namer-1.0.1/creative_namer.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       15 2023-05-20 12:37:02.000000 creative-namer-1.0.1/creative_namer.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     3470 2023-05-20 12:37:01.000000 creative-namer-1.0.1/creative_namer.py
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-20 12:37:02.068031 creative-namer-1.0.1/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      520 2023-05-20 12:37:01.000000 creative-namer-1.0.1/setup.py
```

### Comparing `creative-namer-1.0.0/creative_namer.py` & `creative-namer-1.0.1/creative_namer.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,20 +6,21 @@
 from datetime import datetime
 
 from openai_chat_thread import openai_chat_thread_taiwan
 
 DEFAULT_START_TAG = '--start_json--'
 DEFAULT_END_TAG = '--end_json--'
 DEFAULT_USER = 'cbh@cameo.tw'
+DEFAULT_N = 10
 
 
-def generate_project_names(project_description):
-    prompt = f"請用 json 格式回覆 5 個 github 最貼切「專案描述」的英文專案名稱\n" \
-             f"json內容要用小寫與底線隔開的英文\n" \
-             f"json格式是字典，key是編號 project_name_1 project_name_2 project_name_3 ... ，value是英文名字\n" \
+def generate_project_names(project_description, n=DEFAULT_N):
+    prompt = f"請用 json 格式創造出 n={n} 個 github 最貼切「專案描述」的英文專案名稱\n" \
+             f"json內容的英文名字是要用小寫與底線隔開的英文\n" \
+             f"json格式是字典，project_name_en_1 project_name_en_2 ...\n" \
              f"json內容的起始標記為 --start_json-- 與結束 --end_json-- 有明確標記\n" \
              f"\n「專案描述」:{project_description}\n"
     print(prompt)
     q = openai_chat_thread_taiwan(prompt, model='gpt-4')
     lst = []
     while True:
         response = q.get()
@@ -40,25 +41,28 @@
         return json.loads(json_string)
     else:
         print("JSON start or end marker not found.")
         return {}
 
 
 def to_underscore(str1):
-    return str1.replace('@', '_').replace(':', '_')
+    return str1.replace('@', '_').replace(':', '_').replace('.', '_')
 
 
-def creative_namer(project_description, user=DEFAULT_USER, start_tag=DEFAULT_START_TAG, end_tag=DEFAULT_END_TAG):
-    response = generate_project_names(project_description)
+def creative_namer(project_description, n=DEFAULT_N, user=DEFAULT_USER, start_tag=DEFAULT_START_TAG,
+                   end_tag=DEFAULT_END_TAG):
+    response = generate_project_names(project_description, n)
     dic_json = get_json_dic(response, start_tag, end_tag)
     id1 = str(uuid.uuid4())
     timestamp_utc = datetime.utcnow().strftime('%Y-%m-%dT%H:%M:%SZ')
-    path = to_underscore(f'./data/users/{DEFAULT_USER}/creative_namer/')
+    path = f'data/users/{to_underscore(DEFAULT_USER)}/creative_namer/'
     os.makedirs(path, exist_ok=True)
-    file_path = to_underscore(os.path.join(path, f'type_creative_namer_time_{timestamp_utc}_id_{id1}.json'))
+    file_path = os.path.join(path, f'type_creative_namer_time_{timestamp_utc}_id_{id1}')
+    file_path = to_underscore(file_path)
+    file_path += '.json'
     dic_output = {
         "user": user,
         "type": "creative_namer",
         "time": timestamp_utc,
         "id": id1,
         "file_path": file_path,
         'project_description': project_description,
@@ -67,12 +71,24 @@
     dic_combine = {**dic_output, **dic_json}
     with open(dic_combine["file_path"], 'w', encoding='utf-8') as f:
         json_content = json.dumps(dic_combine, ensure_ascii=False, indent=2)
         print(f'\n{start_tag}\n{json_content}\n{end_tag}\n')
         f.write(json_content)
 
 
-if __name__ == '__main__':
+def get_args_parser():
     parser = argparse.ArgumentParser()
     parser.add_argument("project_description", help="專案描述文字")
-    args = parser.parse_args()
-    creative_namer(args.project_description)
+    parser.add_argument("--n", type=int, default=DEFAULT_N, help="生成英文專案名稱的數量")
+    parser.add_argument("--user", default=DEFAULT_USER, help="使用者的電子郵件地址")
+    parser.add_argument("--start_tag", default=DEFAULT_START_TAG, help="JSON內容起始標記")
+    parser.add_argument("--end_tag", default=DEFAULT_END_TAG, help="JSON內容結束標記")
+    return parser
+
+
+def main():
+    args = get_args_parser().parse_args()
+    creative_namer(args.project_description, n=args.n, user=args.user, start_tag=args.start_tag, end_tag=args.end_tag)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `creative-namer-1.0.0/setup.py` & `creative-namer-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = [line.strip() for line in f.readlines()]
 
 setup(
     name="creative-namer",
-    version="1.0.0",
+    version="1.0.1",
     packages=find_packages(),
     py_modules=['creative_namer'],
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'creative_namer = creative_namer:main',
         ],
```

