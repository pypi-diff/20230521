# Comparing `tmp/openai_forward-0.2.0.tar.gz` & `tmp/openai_forward-0.2.1.tar.gz`

## Comparing `openai_forward-0.2.0.tar` & `openai_forward-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 openai_forward-0.2.0/openai_forward/__init__.py
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 openai_forward-0.2.0/openai_forward/__main__.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 openai_forward-0.2.0/openai_forward/app.py
--rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 openai_forward-0.2.0/openai_forward/base.py
--rw-r--r--   0        0        0     4438 2020-02-02 00:00:00.000000 openai_forward-0.2.0/openai_forward/config.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 openai_forward-0.2.0/openai_forward/openai.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.2.0/openai_forward/content/__init__.py
--rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 openai_forward-0.2.0/openai_forward/content/chat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.2.0/openai_forward/content/image.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.2.0/openai_forward/routers/__init__.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 openai_forward-0.2.0/openai_forward/routers/openai_v1.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 openai_forward-0.2.0/openai_forward/routers/schemas.py
--rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 openai_forward-0.2.0/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.2.0/LICENSE
--rw-r--r--   0        0        0     8074 2020-02-02 00:00:00.000000 openai_forward-0.2.0/README.md
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 openai_forward-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     9408 2020-02-02 00:00:00.000000 openai_forward-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 openai_forward-0.2.1/openai_forward/__init__.py
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 openai_forward-0.2.1/openai_forward/__main__.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 openai_forward-0.2.1/openai_forward/app.py
+-rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 openai_forward-0.2.1/openai_forward/base.py
+-rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 openai_forward-0.2.1/openai_forward/config.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 openai_forward-0.2.1/openai_forward/openai.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.2.1/openai_forward/content/__init__.py
+-rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 openai_forward-0.2.1/openai_forward/content/chat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.2.1/openai_forward/content/image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.2.1/openai_forward/routers/__init__.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 openai_forward-0.2.1/openai_forward/routers/openai_v1.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 openai_forward-0.2.1/openai_forward/routers/schemas.py
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 openai_forward-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.2.1/LICENSE
+-rw-r--r--   0        0        0     8223 2020-02-02 00:00:00.000000 openai_forward-0.2.1/README.md
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 openai_forward-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     9557 2020-02-02 00:00:00.000000 openai_forward-0.2.1/PKG-INFO
```

### Comparing `openai_forward-0.2.0/openai_forward/__main__.py` & `openai_forward-0.2.1/openai_forward/__main__.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.2.0/openai_forward/base.py` & `openai_forward-0.2.1/openai_forward/base.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.2.0/openai_forward/config.py` & `openai_forward-0.2.1/openai_forward/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             frame = frame.f_back
             depth += 1
         logger.opt(depth=depth, exception=record.exc_info).log(
             level, record.getMessage()
         )
 
 
-def setting_log(save_file=False, log_name=None, multi_process=True):
+def setting_log(save_file=False, log_name="openai_forward", multi_process=True):
     # TODO 修复时区配置
     if os.environ.get("TZ") == "Asia/Shanghai":
         os.environ['TZ'] = "UTC-8"
         if hasattr(time, 'tzset'):
             time.tzset()
 
     logging.root.handlers = [InterceptHandler()]
@@ -70,20 +70,22 @@
         logging.getLogger(name).handlers = []
         logging.getLogger(name).propagate = True
 
     config_handlers = [
         {"sink": sys.stdout, "level": "DEBUG"},
     ]
     if save_file:
-        config_handlers += {
-            "sink": f"./Log/{log_name}.log",
-            "enqueue": multi_process,
-            "rotation": "100 MB",
-            "level": "INFO",
-        }
+        config_handlers += [
+            {
+                "sink": f"./Log/{log_name}.log",
+                "enqueue": multi_process,
+                "rotation": "100 MB",
+                "level": "INFO",
+            }
+        ]
 
     logger_config = {"handlers": config_handlers}
     logger.configure(**logger_config)
 
 
 def yaml_dump(data, filepath, rel_path=False, mode='w'):
     abs_path = relp(filepath, parents=1) if rel_path else filepath
```

### Comparing `openai_forward-0.2.0/openai_forward/openai.py` & `openai_forward-0.2.1/openai_forward/openai.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.2.0/openai_forward/content/chat.py` & `openai_forward-0.2.1/openai_forward/content/chat.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.2.0/openai_forward/routers/openai_v1.py` & `openai_forward-0.2.1/openai_forward/routers/openai_v1.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.2.0/openai_forward/routers/schemas.py` & `openai_forward-0.2.1/openai_forward/routers/schemas.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.2.0/.gitignore` & `openai_forward-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `openai_forward-0.2.0/LICENSE` & `openai_forward-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_forward-0.2.0/README.md` & `openai_forward-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -61,29 +61,32 @@
 - [x] 支持转发OpenAI所有接口
 - [x] 支持流式响应
 - [x] 支持指定转发路由前缀
 - [x] docker部署
 - [x] pip 安装部署
 - [x] vercel 一键个人免费部署
   [![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fbeidongjiedeguang%2Fopenai-forward&project-name=openai-forward&repository-name=openai-forward&framework=other)
+- [x] cloudflare 部署
 
 **高级功能**  
 - [x] 实时记录聊天记录(包括流式响应的聊天内容)
 - [x] 允许输入多个openai api key 组成轮询池
 - [x] 自定义 api key (见高级配置)
 - [x] 支持请求IP验证(IP白名单与黑名单)
 
 ## 部署指南
 
-提供三种部署方式
+提供四种部署方式
 1. [vps + pip 安装部署](deploy.md#pip-推荐) (推荐)
 2. [vps + Docker](deploy.md#docker-推荐) (推荐) 
     > https://api.openai-forward.top 
-3. [一键Vercel部署](deploy.md#vercel-一键部署) 
-   > https://vercel.openai-forward.top 
+3. [一键Vercel部署](deploy.md#vercel-一键部署) (目前不推荐)
+   > ~~https://vercel.openai-forward.top~~  
+4. [cloudflare部署](deploy.md#cloudflare-部署) (推荐)
+   > https://cloudflare.openai-forward.top
 
 ## 应用
 
 ### [聊天应用](https://chat.beidongjiedeguang.top)
 
 基于开源项目[ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-Web)搭建自己的chatgpt服务  
 替换docker启动命令中的 `BASE_URL`为我们自己搭建的代理服务地址
```

#### html2text {}

```diff
@@ -13,26 +13,27 @@
 (#åºç¨) - [éç½®éé¡¹](#éç½®éé¡¹) - [èå¤©æ¥å¿](#èå¤©æ¥å¿) -
 [é«çº§éç½®](#é«çº§éç½®) ## åè½ **åºç¡åè½** - [x]
 æ¯æè½¬åOpenAIæææ¥å£ - [x] æ¯ææµå¼ååº - [x]
 æ¯ææå®è½¬åè·¯ç±åç¼ - [x] dockeré¨ç½² - [x] pip å®è£é¨ç½² - [x]
 vercel ä¸é®ä¸ªäººåè´¹é¨ç½² [![Deploy with Vercel](https://vercel.com/
 button)](https://vercel.com/new/clone?repository-
 url=https%3A%2F%2Fgithub.com%2Fbeidongjiedeguang%2Fopenai-forward&project-
-name=openai-forward&repository-name=openai-forward&framework=other)
-**é«çº§åè½** - [x] å®æ¶è®°å½èå¤©è®°å½
+name=openai-forward&repository-name=openai-forward&framework=other) - [x]
+cloudflare é¨ç½² **é«çº§åè½** - [x] å®æ¶è®°å½èå¤©è®°å½
 (åæ¬æµå¼ååºçèå¤©åå®¹) - [x] åè®¸è¾å¥å¤ä¸ªopenai api key
 ç»æè½®è¯¢æ±  - [x] èªå®ä¹ api key (è§é«çº§éç½®) - [x]
 æ¯æè¯·æ±IPéªè¯(IPç½ååä¸é»åå) ## é¨ç½²æå
-æä¾ä¸ç§é¨ç½²æ¹å¼ 1. [vps + pip å®è£é¨ç½²](deploy.md#pip-æ¨è)
+æä¾åç§é¨ç½²æ¹å¼ 1. [vps + pip å®è£é¨ç½²](deploy.md#pip-æ¨è)
 (æ¨è) 2. [vps + Docker](deploy.md#docker-æ¨è) (æ¨è) > https://
-api.openai-forward.top 3. [ä¸é®Vercelé¨ç½²](deploy.md#vercel-ä¸é®é¨ç½²) >
-https://vercel.openai-forward.top ## åºç¨ ### [èå¤©åºç¨](https://
-chat.beidongjiedeguang.top) åºäºå¼æºé¡¹ç®[ChatGPT-Next-Web](https://
-github.com/Yidadaa/ChatGPT-Next-Web)æ­å»ºèªå·±çchatgptæå¡
-æ¿æ¢dockerå¯å¨å½ä»¤ä¸­ç
+api.openai-forward.top 3. [ä¸é®Vercelé¨ç½²](deploy.md#vercel-ä¸é®é¨ç½²)
+(ç®åä¸æ¨è) > ~~https://vercel.openai-forward.top~~ 4. [cloudflareé¨ç½²]
+(deploy.md#cloudflare-é¨ç½²) (æ¨è) > https://cloudflare.openai-forward.top
+## åºç¨ ### [èå¤©åºç¨](https://chat.beidongjiedeguang.top)
+åºäºå¼æºé¡¹ç®[ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-
+Web)æ­å»ºèªå·±çchatgptæå¡ æ¿æ¢dockerå¯å¨å½ä»¤ä¸­ç
 `BASE_URL`ä¸ºæä»¬èªå·±æ­å»ºçä»£çæå¡å°å ```bash docker run -d \ -
 p 3000:3000 \ -e OPENAI_API_KEY="sk-******" \ -e BASE_URL="https://api.openai-
 forward.top" \ -e CODE="kunyuan" \ yidadaa/chatgpt-next-web ```
 è¿éé¨ç½²äºä¸ä¸ªï¼ä¾å¤§å®¶è½»åº¦ä½¿ç¨: https://
 chat.beidongjiedeguang.top , è®¿é®å¯ç : `kunyuan` ### å¨ä»£ç ä¸­ä½¿ç¨
 **JS/TS** ```diff import { Configuration } from "openai"; const configuration =
 new Configuration({ + basePath: "https://api.openai-forward.top/v1", apiKey:
```

### Comparing `openai_forward-0.2.0/pyproject.toml` & `openai_forward-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openai_forward-0.2.0/PKG-INFO` & `openai_forward-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_forward
-Version: 0.2.0
+Version: 0.2.1
 Summary: 🚀 Openai api forward · OpenAI 接口转发服务 · stream forwarding
 Project-URL: Homepage, https://github.com/beidongjiedeguang/openai-forward
 Project-URL: Documentation, https://github.com/beidongjiedeguang/openai-forward#openai-forward
 Project-URL: Issues, https://github.com/beidongjiedeguang/openai-forward/issues
 Project-URL: Source, https://github.com/beidongjiedeguang/openai-forward
 Author-email: kunyuan <beidongjiedeguang@gmail.com>
 License-Expression: MIT
@@ -95,29 +95,32 @@
 - [x] 支持转发OpenAI所有接口
 - [x] 支持流式响应
 - [x] 支持指定转发路由前缀
 - [x] docker部署
 - [x] pip 安装部署
 - [x] vercel 一键个人免费部署
   [![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fbeidongjiedeguang%2Fopenai-forward&project-name=openai-forward&repository-name=openai-forward&framework=other)
+- [x] cloudflare 部署
 
 **高级功能**  
 - [x] 实时记录聊天记录(包括流式响应的聊天内容)
 - [x] 允许输入多个openai api key 组成轮询池
 - [x] 自定义 api key (见高级配置)
 - [x] 支持请求IP验证(IP白名单与黑名单)
 
 ## 部署指南
 
-提供三种部署方式
+提供四种部署方式
 1. [vps + pip 安装部署](deploy.md#pip-推荐) (推荐)
 2. [vps + Docker](deploy.md#docker-推荐) (推荐) 
     > https://api.openai-forward.top 
-3. [一键Vercel部署](deploy.md#vercel-一键部署) 
-   > https://vercel.openai-forward.top 
+3. [一键Vercel部署](deploy.md#vercel-一键部署) (目前不推荐)
+   > ~~https://vercel.openai-forward.top~~  
+4. [cloudflare部署](deploy.md#cloudflare-部署) (推荐)
+   > https://cloudflare.openai-forward.top
 
 ## 应用
 
 ### [聊天应用](https://chat.beidongjiedeguang.top)
 
 基于开源项目[ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-Web)搭建自己的chatgpt服务  
 替换docker启动命令中的 `BASE_URL`为我们自己搭建的代理服务地址
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openai_forward Version: 0.2.0 Summary: ð Openai
+Metadata-Version: 2.1 Name: openai_forward Version: 0.2.1 Summary: ð Openai
 api forward Â· OpenAI æ¥å£è½¬åæå¡ Â· stream forwarding Project-URL:
 Homepage, https://github.com/beidongjiedeguang/openai-forward Project-URL:
 Documentation, https://github.com/beidongjiedeguang/openai-forward#openai-
 forward Project-URL: Issues, https://github.com/beidongjiedeguang/openai-
 forward/issues Project-URL: Source, https://github.com/beidongjiedeguang/
 openai-forward Author-email: kunyuan
 gmail.com> License-Expression: MIT License-File: LICENSE Keywords: OpenAI API
@@ -31,26 +31,27 @@
 (#åºç¨) - [éç½®éé¡¹](#éç½®éé¡¹) - [èå¤©æ¥å¿](#èå¤©æ¥å¿) -
 [é«çº§éç½®](#é«çº§éç½®) ## åè½ **åºç¡åè½** - [x]
 æ¯æè½¬åOpenAIæææ¥å£ - [x] æ¯ææµå¼ååº - [x]
 æ¯ææå®è½¬åè·¯ç±åç¼ - [x] dockeré¨ç½² - [x] pip å®è£é¨ç½² - [x]
 vercel ä¸é®ä¸ªäººåè´¹é¨ç½² [![Deploy with Vercel](https://vercel.com/
 button)](https://vercel.com/new/clone?repository-
 url=https%3A%2F%2Fgithub.com%2Fbeidongjiedeguang%2Fopenai-forward&project-
-name=openai-forward&repository-name=openai-forward&framework=other)
-**é«çº§åè½** - [x] å®æ¶è®°å½èå¤©è®°å½
+name=openai-forward&repository-name=openai-forward&framework=other) - [x]
+cloudflare é¨ç½² **é«çº§åè½** - [x] å®æ¶è®°å½èå¤©è®°å½
 (åæ¬æµå¼ååºçèå¤©åå®¹) - [x] åè®¸è¾å¥å¤ä¸ªopenai api key
 ç»æè½®è¯¢æ±  - [x] èªå®ä¹ api key (è§é«çº§éç½®) - [x]
 æ¯æè¯·æ±IPéªè¯(IPç½ååä¸é»åå) ## é¨ç½²æå
-æä¾ä¸ç§é¨ç½²æ¹å¼ 1. [vps + pip å®è£é¨ç½²](deploy.md#pip-æ¨è)
+æä¾åç§é¨ç½²æ¹å¼ 1. [vps + pip å®è£é¨ç½²](deploy.md#pip-æ¨è)
 (æ¨è) 2. [vps + Docker](deploy.md#docker-æ¨è) (æ¨è) > https://
-api.openai-forward.top 3. [ä¸é®Vercelé¨ç½²](deploy.md#vercel-ä¸é®é¨ç½²) >
-https://vercel.openai-forward.top ## åºç¨ ### [èå¤©åºç¨](https://
-chat.beidongjiedeguang.top) åºäºå¼æºé¡¹ç®[ChatGPT-Next-Web](https://
-github.com/Yidadaa/ChatGPT-Next-Web)æ­å»ºèªå·±çchatgptæå¡
-æ¿æ¢dockerå¯å¨å½ä»¤ä¸­ç
+api.openai-forward.top 3. [ä¸é®Vercelé¨ç½²](deploy.md#vercel-ä¸é®é¨ç½²)
+(ç®åä¸æ¨è) > ~~https://vercel.openai-forward.top~~ 4. [cloudflareé¨ç½²]
+(deploy.md#cloudflare-é¨ç½²) (æ¨è) > https://cloudflare.openai-forward.top
+## åºç¨ ### [èå¤©åºç¨](https://chat.beidongjiedeguang.top)
+åºäºå¼æºé¡¹ç®[ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-
+Web)æ­å»ºèªå·±çchatgptæå¡ æ¿æ¢dockerå¯å¨å½ä»¤ä¸­ç
 `BASE_URL`ä¸ºæä»¬èªå·±æ­å»ºçä»£çæå¡å°å ```bash docker run -d \ -
 p 3000:3000 \ -e OPENAI_API_KEY="sk-******" \ -e BASE_URL="https://api.openai-
 forward.top" \ -e CODE="kunyuan" \ yidadaa/chatgpt-next-web ```
 è¿éé¨ç½²äºä¸ä¸ªï¼ä¾å¤§å®¶è½»åº¦ä½¿ç¨: https://
 chat.beidongjiedeguang.top , è®¿é®å¯ç : `kunyuan` ### å¨ä»£ç ä¸­ä½¿ç¨
 **JS/TS** ```diff import { Configuration } from "openai"; const configuration =
 new Configuration({ + basePath: "https://api.openai-forward.top/v1", apiKey:
```

