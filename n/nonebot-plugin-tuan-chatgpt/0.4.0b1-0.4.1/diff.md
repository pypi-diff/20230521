# Comparing `tmp/nonebot_plugin_tuan_chatgpt-0.4.0b1.tar.gz` & `tmp/nonebot_plugin_tuan_chatgpt-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_tuan_chatgpt-0.4.0b1.tar", max compression
+gzip compressed data, was "nonebot_plugin_tuan_chatgpt-0.4.1.tar", max compression
```

## Comparing `nonebot_plugin_tuan_chatgpt-0.4.0b1.tar` & `nonebot_plugin_tuan_chatgpt-0.4.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1063 2023-05-13 01:12:30.653881 nonebot_plugin_tuan_chatgpt-0.4.0b1/LICENSE.md
--rw-r--r--   0        0        0    16966 2023-05-13 01:12:30.653881 nonebot_plugin_tuan_chatgpt-0.4.0b1/README.md
--rw-r--r--   0        0        0     8709 2023-05-13 01:12:30.937884 nonebot_plugin_tuan_chatgpt-0.4.0b1/nonebot_plugin_tuan_chatgpt/__init__.py
--rw-r--r--   0        0        0     2146 2023-05-13 01:12:30.937884 nonebot_plugin_tuan_chatgpt-0.4.0b1/nonebot_plugin_tuan_chatgpt/config.py
--rw-r--r--   0        0        0      729 2023-05-13 01:12:30.937884 nonebot_plugin_tuan_chatgpt-0.4.0b1/nonebot_plugin_tuan_chatgpt/perf_timer.py
--rw-r--r--   0        0        0    17746 2023-05-13 01:12:30.937884 nonebot_plugin_tuan_chatgpt-0.4.0b1/nonebot_plugin_tuan_chatgpt/text_to_img.py
--rw-r--r--   0        0        0    24940 2023-05-13 01:12:30.937884 nonebot_plugin_tuan_chatgpt-0.4.0b1/nonebot_plugin_tuan_chatgpt/utils.py
--rw-r--r--   0        0        0      580 2023-05-13 01:12:30.937884 nonebot_plugin_tuan_chatgpt-0.4.0b1/pyproject.toml
--rw-r--r--   0        0        0    17947 1970-01-01 00:00:00.000000 nonebot_plugin_tuan_chatgpt-0.4.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-21 12:00:22.095329 nonebot_plugin_tuan_chatgpt-0.4.1/LICENSE.md
+-rw-r--r--   0        0        0    16744 2023-05-21 12:00:22.095329 nonebot_plugin_tuan_chatgpt-0.4.1/README.md
+-rw-r--r--   0        0        0     9084 2023-05-21 12:00:22.435354 nonebot_plugin_tuan_chatgpt-0.4.1/nonebot_plugin_tuan_chatgpt/__init__.py
+-rw-r--r--   0        0        0     2146 2023-05-21 12:00:22.435354 nonebot_plugin_tuan_chatgpt-0.4.1/nonebot_plugin_tuan_chatgpt/config.py
+-rw-r--r--   0        0        0      729 2023-05-21 12:00:22.435354 nonebot_plugin_tuan_chatgpt-0.4.1/nonebot_plugin_tuan_chatgpt/perf_timer.py
+-rw-r--r--   0        0        0    17746 2023-05-21 12:00:22.435354 nonebot_plugin_tuan_chatgpt-0.4.1/nonebot_plugin_tuan_chatgpt/text_to_img.py
+-rw-r--r--   0        0        0    24940 2023-05-21 12:00:22.435354 nonebot_plugin_tuan_chatgpt-0.4.1/nonebot_plugin_tuan_chatgpt/utils.py
+-rw-r--r--   0        0        0      574 2023-05-21 12:00:22.435354 nonebot_plugin_tuan_chatgpt-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    17723 1970-01-01 00:00:00.000000 nonebot_plugin_tuan_chatgpt-0.4.1/PKG-INFO
```

### Comparing `nonebot_plugin_tuan_chatgpt-0.4.0b1/LICENSE.md` & `nonebot_plugin_tuan_chatgpt-0.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tuan_chatgpt-0.4.0b1/README.md` & `nonebot_plugin_tuan_chatgpt-0.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 基于 openai 于3月1日放开的最新模型 gpt-3.5-turbo-0301 开发，能够实现近乎于网页端的体验。
 
 基于Nonebot 2.0, onebot v11开发，已作为插件在Paimon bot测试。
 
 功能：
 
 - **和团子聊天！ Powered by Chatgpt** （可 ~~调教~~ 修改成其他人设）
-- **随机人设**   （ 聊天5次后自动换 每次都有新感受 —— 团子（ 猫娘 / 克苏鲁 / 派蒙 ver.））
+- **随机人设**   （ 聊天5次后自动换 每次都有新感受 预设 —— 团子（ 猫娘 / 克苏鲁 / 派蒙 ver.））
 - **查看赛博地址**  （看看代理能用不 ~~毕竟openai时不时就抽风一下~~）
 - 长回答渲染图片
 - 查看历史问题  （~~看看群友都发了什么怪东西~~）
 - 发言频率限制  （可修改）
 - 长回答自动分割 （可修改）
 - 群友发言长度限制  （可修改 不仅避免腾讯检测 还能省 token）
 - 记忆限制  （可修改 默认记忆7条对话 ~~反正群友也是金鱼 还能防止被群友调教成猫娘~~）
@@ -56,27 +56,26 @@
 
 
 ## 🎉 使用
 
 ### 指令表
 注意：指令中的团子根据设置的nickname为准。也可以通过 @团子 代替。
 
-现在没有默认触发词了，如果没有设置nickname，就只能通过 @ 触发了
+现在没有默认触发词嘞，如果没有设置nickname，就只能通过 @ 触发了
 
 指令的相同触发词可自行查看代码中 aliases 部分。
 
 
 
-| 指令 | 权限 | 需要@ | 范围 | 说明 |
-|:-----:|:----:|:----:|:----:|:----:|
-| 团子[聊天内容] | 群员 | 否 | 群聊 / 私聊 | 来和团子聊天吧！ |
-| @团子[聊天内容] | 同上 |  是 | 同上 | 同上 |
-| 团子 看看位置 / 你在哪儿 | 群员 | 否 | 群聊 / 私聊 | 查看团子赛博地址 |
-| 团子 历史记录 / history | 主人 | 否 | 群聊 / 私聊 | 查看历史提问（不包括回答） |
-| 团子 清除记忆 / 清除历史记录 | 主人 | 否 | 群聊 / 私聊 | 清除团子的记忆 |
+| 指令 | 权限 | 范围 | 说明 |
+|:-----:|:----:|:----:|:----:|
+| 团子[聊天内容] | 群员 |群聊 / 私聊 | 来和团子聊天吧！ |
+| 团子 看看位置 / 你在哪儿 | 群员 | 群聊 / 私聊 | 查看团子赛博地址 |
+| 团子 历史记录 / history | 主人 |  群聊 / 私聊 | 查看历史提问（不包括回答） |
+| 团子 清除记忆 / 清除历史记录 | 群员 | 群聊 / 私聊 | 清除团子的记忆 |
 
 
 
 ## 💿 安装
 
 
 <details>
@@ -123,15 +122,15 @@
 
 环境配置：
 
 打开nonebot的`.env` 文件，写入您的 `chatgpt_api` 以及 `nickname`
 
 如果希望启用代理，则需要在`.env` 文件中，写入 `chat_use_proxy = True` 以及 `chat_proxy_address_https = "代理地址"` 或 `chat_proxy_address_http = "代理地址"`  (处理逻辑类似openai，优先使用https。但是https经常会报错（aiohttp和urllib3都可能会造成问题），推荐只使用http)
 
-如果希望启用api转发 (类似 [腾讯云函数搭建 OpenAI 国内代理](https://github.com/Ice-Hazymoon/openai-scf-proxy) 通过云函数等方式实现反代 )，则需要写入写入 `chat_use_api_forward = True` 以及 `chat_api_address = "代理地址"` 
+如果希望启用api转发 (类似 [腾讯云函数搭建 OpenAI 国内代理](https://github.com/Ice-Hazymoon/openai-scf-proxy) 通过云函数等方式实现反代 )，则需要写入 `chat_use_api_forward = True` 以及 `chat_api_address = "代理地址"` 
 
 但是不推荐两者同时启用
 
 如果希望启用图片渲染，则需要写入 `chat_use_img2text=True`, 以及在工程目录的 `/data/tuan_chatgpt` 文件夹（`/data` 文件夹与 `bot.py` / `env` / 运行`nb run` 的地方同级 ）中分别添加字体文件和背景文件到 `/font` 以及 `/bachground` 文件夹中。
 默认的字体文件可参考本仓库，背景文件则会从中随机抽取。文件夹不存在时会自动创建，也可自行设定文件夹路径。
 也可以直接下载 Release 的 [tuan_chatgpt.zip](https://github.com/TheLZY/nonebot_plugin_tuan_chatgpt/files/11163988/tuan_chatgpt.zip) 扔到 `/data` 里去
 
@@ -230,15 +229,16 @@
 - [x] 支持使用代理
 - [x] 增加代理测试 通过返回的ip地址判断代理是否有效 绝赞赛博旅行中！  <!--  http://icanhazip.com/ --> 
 - [x] 私聊做发言频率限制。
 - [x] 错误处理 <!--（比如代理的检测之类的 以及报错方式 团子被玩坏了！这一定不是团子的错！（繁体） 可以写个函数error message    - 倒是可以照着官方的写 不过还是得先在telegrambot上测试一下 ）-->
 - [x] 异步调用优化  （自动重试 / 返回报错  <!-- - 但是估计得自己造轮子...不知道官方有没有提供 --> ）
 - [x] 随机人设 感觉会很有意思（
 - [x] 通过@触发 
-- [ ] 修改人设 ？ 
+- [ ] 切换人设 （想来不是很麻烦，但是预设有点少。。。青雀 加了也白加.jpg 在增加人设的时候一起用吧）
+- [ ] 修改人设 ？ 可以保存一个json文件到 data/charactor 目录下，以及利用指令修改。
 - [ ] markdown 渲染 ？ 
 - [x] ~~自定义触发方式？ 这个倒是可以和修改触发人设一起联动...不过感觉动态修改有点麻烦。~~ 在nickname里面加吧。还是不造轮子了。
 - [ ] ~~Openai 抽风处理（暂时只输出 3*177 个长度的回答 可以根据相同字数出现次数来 同一个字连续出现6次判定为抽风？）~~ 最近没遇到 鉴定为不瞎改就不会有问题
 - [ ] ~~长回答合并转发~~ 似乎更容易被风控 算了。 [参考](https://github.com/Ailitonia/omega-miya/issues/16#issuecomment-827432967)
 
 <!-- - [ ] 全局变量似乎有数据不一致的问题 是否需要加锁？ 毕竟只是一个小小的字典 就算出现一点顺序错误也无伤大雅 --> 
 
@@ -249,28 +249,22 @@
 如果希望更改人设，可以修改 `utils.py` 文件中的 `MessageBox` 中的 `charactor` 相关部分
 
 （正在思考怎么用聊天来添加人设 不过感觉要涉及的东西比较多
 
 ### 一些碎碎念
 
 <!-- 
-代码重构，符合OOC ？ 但是感觉复杂度并不高，可以，但没必要 -->
+代码重构，符合OOC ？ 但是感觉复杂度并不高，可以，慢慢来叭 -->
 
-<!-- 
-其实也可以是收到 @ ，然后没有别的程序被触发的时候就回复。因为paimon bot似乎会自动将nickname转义为 @ ？ -->
-
-<!-- 虽然这样对于一些有转移功能的bot来说比较方便，两种触发方式都能回答
+<!-- Message的处理：
+可以直接用get_message, 但是这样无法获取触发词
 但是有一个问题 别人叫你团子爹怎么怎么的时候，她收到的可能就是爹怎么怎么。。。
 
-但是并不是所有的都会。
-要适配所有bot的话可能写两遍是最合理的。。。
-
-而且有可能会在写错命令的时候误运行
-
-不过按理来说也不是不行，只需要把priority调低就行 -->
+自己写还是算嘞，不造轮子
+-->
 
 
 conversation_remember_num 最好不要调得太高，记住太多话了就会变成性冷淡机器人 😥
 
 出现了 wake up 词也会变回去，不过现在应该多说两句话就好了
 
 长回答处理？ 转发的方式似乎容易被风控。发太多了也容易被风控。
@@ -387,8 +381,8 @@
 
 [nonebot-plugin-oachat](https://github.com/Gin2O/nonebot_plugin_oachat) by @[Gin2O](https://github.com/Gin2O)
 
 [ChatGPT 中文调教指南]( https://github.com/PlexPt/awesome-chatgpt-prompts-zh) by @[PlexPt](https://github.com/PlexPt)
 
 [Little Paimon with chatgpt](https://github.com/meatjam/LittlePaimon) by @[meatjam](https://github.com/meatjam)
 
-[nonebot_plugin_biliav](https://github.com/knva/nonebot_plugin_biliav) by @[knva](https://github.com/knva)
+[nonebot_plugin_biliav](https://github.com/knva/nonebot_plugin_biliav) by @[knva](https://github.com/knva)
```

#### html2text {}

```diff
@@ -5,54 +5,53 @@
                     README_EN.md) [license] [pypi] [python]
 ## ð ä»ç» æ¥ä¸å¢å­èå¤©å§ï¼ åºäº openai
 äº3æ1æ¥æ¾å¼çææ°æ¨¡å gpt-3.5-turbo-0301
 å¼åï¼è½å¤å®ç°è¿ä¹äºç½é¡µç«¯çä½éªã åºäºNonebot 2.0, onebot
 v11å¼åï¼å·²ä½ä¸ºæä»¶å¨Paimon botæµè¯ã åè½ï¼ -
 **åå¢å­èå¤©ï¼ Powered by Chatgpt** ï¼å¯ ~~è°æ~~
 ä¿®æ¹æå¶ä»äººè®¾ï¼ - **éæºäººè®¾** ï¼ èå¤©5æ¬¡åèªå¨æ¢
-æ¯æ¬¡é½ææ°æå ââ å¢å­ï¼ ç«å¨ / åèé² / æ´¾è ver.ï¼ï¼ -
-**æ¥çèµåå°å** ï¼ççä»£çè½ç¨ä¸
+æ¯æ¬¡é½ææ°æå é¢è®¾ ââ å¢å­ï¼ ç«å¨ / åèé² / æ´¾è
+ver.ï¼ï¼ - **æ¥çèµåå°å** ï¼ççä»£çè½ç¨ä¸
 ~~æ¯ç«openaiæ¶ä¸æ¶å°±æ½é£ä¸ä¸~~ï¼ - é¿åç­æ¸²æå¾ç -
 æ¥çåå²é®é¢ ï¼~~ççç¾¤åé½åäºä»ä¹æªä¸è¥¿~~ï¼ -
 åè¨é¢çéå¶ ï¼å¯ä¿®æ¹ï¼ - é¿åç­èªå¨åå² ï¼å¯ä¿®æ¹ï¼ -
 ç¾¤ååè¨é¿åº¦éå¶ ï¼å¯ä¿®æ¹ ä¸ä»é¿åè¾è®¯æ£æµ è¿è½ç
 tokenï¼ - è®°å¿éå¶ ï¼å¯ä¿®æ¹ é»è®¤è®°å¿7æ¡å¯¹è¯
 ~~åæ­£ç¾¤åä¹æ¯éé±¼ è¿è½é²æ­¢è¢«ç¾¤åè°ææç«å¨~~ï¼ -
 èªå¨éè¯ éè¯¯å¤ç ï¼æ¯ç«æçæ¢¯å­ä¸ç¨³å®ï¼ - æ¯æä»£çå
 api è½¬å ç±äºæ¬äººè½åç²¾åæéï¼å¯¹äºæ½å¨çé®é¢ &
 è½æåçå°æ¹ï¼æ¬¢è¿æ¥æ issue & pull requestã ä¸¾ä¸ªæ å­ ð°ï¼
 ![èå¤©ææ](https://raw.githubusercontent.com/TheLZY/
 nonebot_plugin_tuan_chatgpt/master/examples/example2.png) ## ð ä½¿ç¨ ###
 æä»¤è¡¨
 æ³¨æï¼æä»¤ä¸­çå¢å­æ ¹æ®è®¾ç½®çnicknameä¸ºåãä¹å¯ä»¥éè¿
 @å¢å­ ä»£æ¿ã
-ç°å¨æ²¡æé»è®¤è§¦åè¯äºï¼å¦ææ²¡æè®¾ç½®nicknameï¼å°±åªè½éè¿ @
+ç°å¨æ²¡æé»è®¤è§¦åè¯åï¼å¦ææ²¡æè®¾ç½®nicknameï¼å°±åªè½éè¿ @
 è§¦åäº æä»¤çç¸åè§¦åè¯å¯èªè¡æ¥çä»£ç ä¸­ aliases é¨åã |
-æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:--
---:| | å¢å­[èå¤©åå®¹] | ç¾¤å | å¦ | ç¾¤è / ç§è |
-æ¥åå¢å­èå¤©å§ï¼ | | @å¢å­[èå¤©åå®¹] | åä¸ | æ¯ | åä¸ |
-åä¸ | | å¢å­ ççä½ç½® / ä½ å¨åªå¿ | ç¾¤å | å¦ | ç¾¤è / ç§è
-| æ¥çå¢å­èµåå°å | | å¢å­ åå²è®°å½ / history | ä¸»äºº | å¦ |
-ç¾¤è / ç§è | æ¥çåå²æé®ï¼ä¸åæ¬åç­ï¼ | | å¢å­
-æ¸é¤è®°å¿ / æ¸é¤åå²è®°å½ | ä¸»äºº | å¦ | ç¾¤è / ç§è |
-æ¸é¤å¢å­çè®°å¿ | ## ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ ``` nb plugin
-install nonebot-plugin-tuan-chatgpt # åçº§ï¼ nb plugin update nonebot-
-plugin-tuan-chatgpt ```   ä½¿ç¨ git å®è£  å®è£ï¼å¨ nonebot2
-é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, ä½¿ç¨ git å®è£ ``` git clone
-https://github.com/TheLZY/nonebot_plugin_tuan_chatgpt.git ``` åçº§ï¼ ``` git
-pull ```   ä½¿ç¨ pip å®è£ ``` pip install nonebot-plugin-tuan-chatgpt ```
-ç¯å¢éç½®ï¼ æå¼nonebotç`.env` æä»¶ï¼åå¥æ¨ç `chatgpt_api`
-ä»¥å `nickname` å¦æå¸æå¯ç¨ä»£çï¼åéè¦å¨`.env`
-æä»¶ä¸­ï¼åå¥ `chat_use_proxy = True` ä»¥å `chat_proxy_address_https =
-"ä»£çå°å"` æ `chat_proxy_address_http = "ä»£çå°å"`
+æä»¤ | æé | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:| | å¢å­
+[èå¤©åå®¹] | ç¾¤å |ç¾¤è / ç§è | æ¥åå¢å­èå¤©å§ï¼ | | å¢å­
+ççä½ç½® / ä½ å¨åªå¿ | ç¾¤å | ç¾¤è / ç§è |
+æ¥çå¢å­èµåå°å | | å¢å­ åå²è®°å½ / history | ä¸»äºº | ç¾¤è /
+ç§è | æ¥çåå²æé®ï¼ä¸åæ¬åç­ï¼ | | å¢å­ æ¸é¤è®°å¿ /
+æ¸é¤åå²è®°å½ | ç¾¤å | ç¾¤è / ç§è | æ¸é¤å¢å­çè®°å¿ | ## ð¿
+å®è£  ä½¿ç¨ nb-cli å®è£ ``` nb plugin install nonebot-plugin-tuan-chatgpt
+# åçº§ï¼ nb plugin update nonebot-plugin-tuan-chatgpt ```   ä½¿ç¨ git
+å®è£  å®è£ï¼å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, ä½¿ç¨
+git å®è£ ``` git clone https://github.com/TheLZY/
+nonebot_plugin_tuan_chatgpt.git ``` åçº§ï¼ ``` git pull ```   ä½¿ç¨ pip
+å®è£ ``` pip install nonebot-plugin-tuan-chatgpt ```  ç¯å¢éç½®ï¼
+æå¼nonebotç`.env` æä»¶ï¼åå¥æ¨ç `chatgpt_api` ä»¥å `nickname`
+å¦æå¸æå¯ç¨ä»£çï¼åéè¦å¨`.env` æä»¶ä¸­ï¼åå¥
+`chat_use_proxy = True` ä»¥å `chat_proxy_address_https = "ä»£çå°å"` æ
+`chat_proxy_address_http = "ä»£çå°å"`
 (å¤çé»è¾ç±»ä¼¼openaiï¼ä¼åä½¿ç¨httpsãä½æ¯httpsç»å¸¸ä¼æ¥éï¼aiohttpåurllib3é½å¯è½ä¼é æé®é¢ï¼ï¼æ¨èåªä½¿ç¨http)
 å¦æå¸æå¯ç¨apiè½¬å (ç±»ä¼¼ [è¾è®¯äºå½æ°æ­å»º OpenAI å½åä»£ç]
 (https://github.com/Ice-Hazymoon/openai-scf-proxy)
-éè¿äºå½æ°ç­æ¹å¼å®ç°åä»£ )ï¼åéè¦åå¥åå¥
-`chat_use_api_forward = True` ä»¥å `chat_api_address = "ä»£çå°å"`
+éè¿äºå½æ°ç­æ¹å¼å®ç°åä»£ )ï¼åéè¦åå¥ `chat_use_api_forward
+= True` ä»¥å `chat_api_address = "ä»£çå°å"`
 ä½æ¯ä¸æ¨èä¸¤èåæ¶å¯ç¨
 å¦æå¸æå¯ç¨å¾çæ¸²æï¼åéè¦åå¥ `chat_use_img2text=True`,
 ä»¥åå¨å·¥ç¨ç®å½ç `/data/tuan_chatgpt` æä»¶å¤¹ï¼`/data` æä»¶å¤¹ä¸
 `bot.py` / `env` / è¿è¡`nb run` çå°æ¹åçº§
 ï¼ä¸­åå«æ·»å å­ä½æä»¶åèæ¯æä»¶å° `/font` ä»¥å `/bachground`
 æä»¶å¤¹ä¸­ã
 é»è®¤çå­ä½æä»¶å¯åèæ¬ä»åºï¼èæ¯æä»¶åä¼ä»ä¸­éæºæ½åãæä»¶å¤¹ä¸å­å¨æ¶ä¼èªå¨åå»ºï¼ä¹å¯èªè¡è®¾å®æä»¶å¤¹è·¯å¾ã
@@ -105,15 +104,19 @@
 nonebot_plugin_tuan_chatgpt/master/examples/example_history.png) ## ð¡ TODO -
 [x] åç¾¤è®°å¿ï¼æ¯ä¸ªç¾¤ä»¥åç§èï¼è®°å¿ä¸ä¼ä¸²ï¼ - [x]
 åç­åé ï¼éè¿åæ®µå®ç°ãå¯è½ä¼èèæ¢æå¾çåéï¼ - [x]
 æ¯æä½¿ç¨ä»£ç - [x] å¢å ä»£çæµè¯
 éè¿è¿åçipå°åå¤æ­ä»£çæ¯å¦ææ ç»èµèµåæè¡ä¸­ï¼  - [x]
 ç§èååè¨é¢çéå¶ã - [x] éè¯¯å¤ç  - [x] å¼æ­¥è°ç¨ä¼å
 ï¼èªå¨éè¯ / è¿åæ¥é  ï¼ - [x] éæºäººè®¾ æè§ä¼å¾æææï¼
-- [x] éè¿@è§¦å - [ ] ä¿®æ¹äººè®¾ ï¼ - [ ] markdown æ¸²æ ï¼ - [x]
+- [x] éè¿@è§¦å - [ ] åæ¢äººè®¾
+ï¼æ³æ¥ä¸æ¯å¾éº»ç¦ï¼ä½æ¯é¢è®¾æç¹å°ãããéé
+å äºä¹ç½å .jpg å¨å¢å äººè®¾çæ¶åä¸èµ·ç¨å§ï¼ - [ ] ä¿®æ¹äººè®¾
+ï¼ å¯ä»¥ä¿å­ä¸ä¸ªjsonæä»¶å° data/charactor
+ç®å½ä¸ï¼ä»¥åå©ç¨æä»¤ä¿®æ¹ã - [ ] markdown æ¸²æ ï¼ - [x]
 ~~èªå®ä¹è§¦åæ¹å¼ï¼
 è¿ä¸ªåæ¯å¯ä»¥åä¿®æ¹è§¦åäººè®¾ä¸èµ·èå¨...ä¸è¿æè§å¨æä¿®æ¹æç¹éº»ç¦ã~~
 å¨nicknameéé¢å å§ãè¿æ¯ä¸é è½®å­äºã - [ ] ~~Openai
 æ½é£å¤çï¼ææ¶åªè¾åº 3*177 ä¸ªé¿åº¦çåç­
 å¯ä»¥æ ¹æ®ç¸åå­æ°åºç°æ¬¡æ°æ¥
 åä¸ä¸ªå­è¿ç»­åºç°6æ¬¡å¤å®ä¸ºæ½é£ï¼ï¼~~ æè¿æ²¡éå°
 é´å®ä¸ºä¸çæ¹å°±ä¸ä¼æé®é¢ - [ ] ~~é¿åç­åå¹¶è½¬å~~
```

### Comparing `nonebot_plugin_tuan_chatgpt-0.4.0b1/nonebot_plugin_tuan_chatgpt/__init__.py` & `nonebot_plugin_tuan_chatgpt-0.4.1/nonebot_plugin_tuan_chatgpt/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from .utils import *
 from .config import config, NICKNAME, init_name
 from .text_to_img import text2img_main
 import openai
 
 import asyncio
 import re
+import random
 
 __plugin_meta__ = PluginMetadata(
     name='团子聊天',
     description='团子聊天 QQ bot ver. powered by Chatgpt',
     usage='团子[聊天内容]',
     extra={
         'author': 'TheLZY',
@@ -196,16 +197,22 @@
     global messagebox
     if isinstance(event, GroupMessageEvent):
         chat_id = f"chat-group{event.group_id}"
     else:
         chat_id = f'chat-user{event.user_id}'
 
     messagebox.clean(id = chat_id)
+
+    clean_message_list = [f'清除成功啦~ 快来和{NICKNAME}聊天吧~',
+                          f'已经全忘惹~ 快来和{NICKNAME}聊天吧~',
+                          f'发生什么事啦？ 唔，总之，来和{NICKNAME}聊天吧~',
+                          f'{NICKNAME}已经什么都不记得啦~ 快来和我聊天吧~']
+    clean_message = random.choice(clean_message_list)
     
-    await clean_history.finish(f'成功清除记忆~ 快来和{NICKNAME}聊天吧~')
+    await chat_service_clean.finish(clean_message)
 
 @chat_service_position.handle()
 async def check_position(event: MessageEvent):
     
     proxy = None
     try:
         if config.chat_proxy_address_https:
```

### Comparing `nonebot_plugin_tuan_chatgpt-0.4.0b1/nonebot_plugin_tuan_chatgpt/config.py` & `nonebot_plugin_tuan_chatgpt-0.4.1/nonebot_plugin_tuan_chatgpt/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tuan_chatgpt-0.4.0b1/nonebot_plugin_tuan_chatgpt/perf_timer.py` & `nonebot_plugin_tuan_chatgpt-0.4.1/nonebot_plugin_tuan_chatgpt/perf_timer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tuan_chatgpt-0.4.0b1/nonebot_plugin_tuan_chatgpt/text_to_img.py` & `nonebot_plugin_tuan_chatgpt-0.4.1/nonebot_plugin_tuan_chatgpt/text_to_img.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tuan_chatgpt-0.4.0b1/nonebot_plugin_tuan_chatgpt/utils.py` & `nonebot_plugin_tuan_chatgpt-0.4.1/nonebot_plugin_tuan_chatgpt/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tuan_chatgpt-0.4.0b1/pyproject.toml` & `nonebot_plugin_tuan_chatgpt-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_tuan_chatgpt"
-version = "0.4.0-beta1"
+version = "0.4.1"
 description = "\"Chat with tuanzi ~\""
 authors = ["TheLZY"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/TheLZY/nonebot_plugin_tuan_chatgpt"
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_plugin_tuan_chatgpt-0.4.0b1/PKG-INFO` & `nonebot_plugin_tuan_chatgpt-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-tuan-chatgpt
-Version: 0.4.0b1
+Version: 0.4.1
 Summary: "Chat with tuanzi ~"
 Home-page: https://github.com/TheLZY/nonebot_plugin_tuan_chatgpt
 License: MIT
 Author: TheLZY
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -57,15 +57,15 @@
 基于 openai 于3月1日放开的最新模型 gpt-3.5-turbo-0301 开发，能够实现近乎于网页端的体验。
 
 基于Nonebot 2.0, onebot v11开发，已作为插件在Paimon bot测试。
 
 功能：
 
 - **和团子聊天！ Powered by Chatgpt** （可 ~~调教~~ 修改成其他人设）
-- **随机人设**   （ 聊天5次后自动换 每次都有新感受 —— 团子（ 猫娘 / 克苏鲁 / 派蒙 ver.））
+- **随机人设**   （ 聊天5次后自动换 每次都有新感受 预设 —— 团子（ 猫娘 / 克苏鲁 / 派蒙 ver.））
 - **查看赛博地址**  （看看代理能用不 ~~毕竟openai时不时就抽风一下~~）
 - 长回答渲染图片
 - 查看历史问题  （~~看看群友都发了什么怪东西~~）
 - 发言频率限制  （可修改）
 - 长回答自动分割 （可修改）
 - 群友发言长度限制  （可修改 不仅避免腾讯检测 还能省 token）
 - 记忆限制  （可修改 默认记忆7条对话 ~~反正群友也是金鱼 还能防止被群友调教成猫娘~~）
@@ -81,27 +81,26 @@
 
 
 ## 🎉 使用
 
 ### 指令表
 注意：指令中的团子根据设置的nickname为准。也可以通过 @团子 代替。
 
-现在没有默认触发词了，如果没有设置nickname，就只能通过 @ 触发了
+现在没有默认触发词嘞，如果没有设置nickname，就只能通过 @ 触发了
 
 指令的相同触发词可自行查看代码中 aliases 部分。
 
 
 
-| 指令 | 权限 | 需要@ | 范围 | 说明 |
-|:-----:|:----:|:----:|:----:|:----:|
-| 团子[聊天内容] | 群员 | 否 | 群聊 / 私聊 | 来和团子聊天吧！ |
-| @团子[聊天内容] | 同上 |  是 | 同上 | 同上 |
-| 团子 看看位置 / 你在哪儿 | 群员 | 否 | 群聊 / 私聊 | 查看团子赛博地址 |
-| 团子 历史记录 / history | 主人 | 否 | 群聊 / 私聊 | 查看历史提问（不包括回答） |
-| 团子 清除记忆 / 清除历史记录 | 主人 | 否 | 群聊 / 私聊 | 清除团子的记忆 |
+| 指令 | 权限 | 范围 | 说明 |
+|:-----:|:----:|:----:|:----:|
+| 团子[聊天内容] | 群员 |群聊 / 私聊 | 来和团子聊天吧！ |
+| 团子 看看位置 / 你在哪儿 | 群员 | 群聊 / 私聊 | 查看团子赛博地址 |
+| 团子 历史记录 / history | 主人 |  群聊 / 私聊 | 查看历史提问（不包括回答） |
+| 团子 清除记忆 / 清除历史记录 | 群员 | 群聊 / 私聊 | 清除团子的记忆 |
 
 
 
 ## 💿 安装
 
 
 <details>
@@ -148,15 +147,15 @@
 
 环境配置：
 
 打开nonebot的`.env` 文件，写入您的 `chatgpt_api` 以及 `nickname`
 
 如果希望启用代理，则需要在`.env` 文件中，写入 `chat_use_proxy = True` 以及 `chat_proxy_address_https = "代理地址"` 或 `chat_proxy_address_http = "代理地址"`  (处理逻辑类似openai，优先使用https。但是https经常会报错（aiohttp和urllib3都可能会造成问题），推荐只使用http)
 
-如果希望启用api转发 (类似 [腾讯云函数搭建 OpenAI 国内代理](https://github.com/Ice-Hazymoon/openai-scf-proxy) 通过云函数等方式实现反代 )，则需要写入写入 `chat_use_api_forward = True` 以及 `chat_api_address = "代理地址"` 
+如果希望启用api转发 (类似 [腾讯云函数搭建 OpenAI 国内代理](https://github.com/Ice-Hazymoon/openai-scf-proxy) 通过云函数等方式实现反代 )，则需要写入 `chat_use_api_forward = True` 以及 `chat_api_address = "代理地址"` 
 
 但是不推荐两者同时启用
 
 如果希望启用图片渲染，则需要写入 `chat_use_img2text=True`, 以及在工程目录的 `/data/tuan_chatgpt` 文件夹（`/data` 文件夹与 `bot.py` / `env` / 运行`nb run` 的地方同级 ）中分别添加字体文件和背景文件到 `/font` 以及 `/bachground` 文件夹中。
 默认的字体文件可参考本仓库，背景文件则会从中随机抽取。文件夹不存在时会自动创建，也可自行设定文件夹路径。
 也可以直接下载 Release 的 [tuan_chatgpt.zip](https://github.com/TheLZY/nonebot_plugin_tuan_chatgpt/files/11163988/tuan_chatgpt.zip) 扔到 `/data` 里去
 
@@ -255,15 +254,16 @@
 - [x] 支持使用代理
 - [x] 增加代理测试 通过返回的ip地址判断代理是否有效 绝赞赛博旅行中！  <!--  http://icanhazip.com/ --> 
 - [x] 私聊做发言频率限制。
 - [x] 错误处理 <!--（比如代理的检测之类的 以及报错方式 团子被玩坏了！这一定不是团子的错！（繁体） 可以写个函数error message    - 倒是可以照着官方的写 不过还是得先在telegrambot上测试一下 ）-->
 - [x] 异步调用优化  （自动重试 / 返回报错  <!-- - 但是估计得自己造轮子...不知道官方有没有提供 --> ）
 - [x] 随机人设 感觉会很有意思（
 - [x] 通过@触发 
-- [ ] 修改人设 ？ 
+- [ ] 切换人设 （想来不是很麻烦，但是预设有点少。。。青雀 加了也白加.jpg 在增加人设的时候一起用吧）
+- [ ] 修改人设 ？ 可以保存一个json文件到 data/charactor 目录下，以及利用指令修改。
 - [ ] markdown 渲染 ？ 
 - [x] ~~自定义触发方式？ 这个倒是可以和修改触发人设一起联动...不过感觉动态修改有点麻烦。~~ 在nickname里面加吧。还是不造轮子了。
 - [ ] ~~Openai 抽风处理（暂时只输出 3*177 个长度的回答 可以根据相同字数出现次数来 同一个字连续出现6次判定为抽风？）~~ 最近没遇到 鉴定为不瞎改就不会有问题
 - [ ] ~~长回答合并转发~~ 似乎更容易被风控 算了。 [参考](https://github.com/Ailitonia/omega-miya/issues/16#issuecomment-827432967)
 
 <!-- - [ ] 全局变量似乎有数据不一致的问题 是否需要加锁？ 毕竟只是一个小小的字典 就算出现一点顺序错误也无伤大雅 --> 
 
@@ -274,28 +274,22 @@
 如果希望更改人设，可以修改 `utils.py` 文件中的 `MessageBox` 中的 `charactor` 相关部分
 
 （正在思考怎么用聊天来添加人设 不过感觉要涉及的东西比较多
 
 ### 一些碎碎念
 
 <!-- 
-代码重构，符合OOC ？ 但是感觉复杂度并不高，可以，但没必要 -->
+代码重构，符合OOC ？ 但是感觉复杂度并不高，可以，慢慢来叭 -->
 
-<!-- 
-其实也可以是收到 @ ，然后没有别的程序被触发的时候就回复。因为paimon bot似乎会自动将nickname转义为 @ ？ -->
-
-<!-- 虽然这样对于一些有转移功能的bot来说比较方便，两种触发方式都能回答
+<!-- Message的处理：
+可以直接用get_message, 但是这样无法获取触发词
 但是有一个问题 别人叫你团子爹怎么怎么的时候，她收到的可能就是爹怎么怎么。。。
 
-但是并不是所有的都会。
-要适配所有bot的话可能写两遍是最合理的。。。
-
-而且有可能会在写错命令的时候误运行
-
-不过按理来说也不是不行，只需要把priority调低就行 -->
+自己写还是算嘞，不造轮子
+-->
 
 
 conversation_remember_num 最好不要调得太高，记住太多话了就会变成性冷淡机器人 😥
 
 出现了 wake up 词也会变回去，不过现在应该多说两句话就好了
 
 长回答处理？ 转发的方式似乎容易被风控。发太多了也容易被风控。
@@ -413,7 +407,8 @@
 [nonebot-plugin-oachat](https://github.com/Gin2O/nonebot_plugin_oachat) by @[Gin2O](https://github.com/Gin2O)
 
 [ChatGPT 中文调教指南]( https://github.com/PlexPt/awesome-chatgpt-prompts-zh) by @[PlexPt](https://github.com/PlexPt)
 
 [Little Paimon with chatgpt](https://github.com/meatjam/LittlePaimon) by @[meatjam](https://github.com/meatjam)
 
 [nonebot_plugin_biliav](https://github.com/knva/nonebot_plugin_biliav) by @[knva](https://github.com/knva)
+
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-tuan-chatgpt Version: 0.4.0b1
-Summary: "Chat with tuanzi ~" Home-page: https://github.com/TheLZY/
+Metadata-Version: 2.1 Name: nonebot-plugin-tuan-chatgpt Version: 0.4.1 Summary:
+"Chat with tuanzi ~" Home-page: https://github.com/TheLZY/
 nonebot_plugin_tuan_chatgpt License: MIT Author: TheLZY Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: Pillow (>=9.5.0,<10.0.0) Requires-Dist: aiohttp
 (>=3.8.4,<4.0.0) Requires-Dist: nonebot-adapter-onebot (>=2.2.0,<3.0.0)
@@ -19,54 +19,53 @@
                     README_EN.md) [license] [pypi] [python]
 ## ð ä»ç» æ¥ä¸å¢å­èå¤©å§ï¼ åºäº openai
 äº3æ1æ¥æ¾å¼çææ°æ¨¡å gpt-3.5-turbo-0301
 å¼åï¼è½å¤å®ç°è¿ä¹äºç½é¡µç«¯çä½éªã åºäºNonebot 2.0, onebot
 v11å¼åï¼å·²ä½ä¸ºæä»¶å¨Paimon botæµè¯ã åè½ï¼ -
 **åå¢å­èå¤©ï¼ Powered by Chatgpt** ï¼å¯ ~~è°æ~~
 ä¿®æ¹æå¶ä»äººè®¾ï¼ - **éæºäººè®¾** ï¼ èå¤©5æ¬¡åèªå¨æ¢
-æ¯æ¬¡é½ææ°æå ââ å¢å­ï¼ ç«å¨ / åèé² / æ´¾è ver.ï¼ï¼ -
-**æ¥çèµåå°å** ï¼ççä»£çè½ç¨ä¸
+æ¯æ¬¡é½ææ°æå é¢è®¾ ââ å¢å­ï¼ ç«å¨ / åèé² / æ´¾è
+ver.ï¼ï¼ - **æ¥çèµåå°å** ï¼ççä»£çè½ç¨ä¸
 ~~æ¯ç«openaiæ¶ä¸æ¶å°±æ½é£ä¸ä¸~~ï¼ - é¿åç­æ¸²æå¾ç -
 æ¥çåå²é®é¢ ï¼~~ççç¾¤åé½åäºä»ä¹æªä¸è¥¿~~ï¼ -
 åè¨é¢çéå¶ ï¼å¯ä¿®æ¹ï¼ - é¿åç­èªå¨åå² ï¼å¯ä¿®æ¹ï¼ -
 ç¾¤ååè¨é¿åº¦éå¶ ï¼å¯ä¿®æ¹ ä¸ä»é¿åè¾è®¯æ£æµ è¿è½ç
 tokenï¼ - è®°å¿éå¶ ï¼å¯ä¿®æ¹ é»è®¤è®°å¿7æ¡å¯¹è¯
 ~~åæ­£ç¾¤åä¹æ¯éé±¼ è¿è½é²æ­¢è¢«ç¾¤åè°ææç«å¨~~ï¼ -
 èªå¨éè¯ éè¯¯å¤ç ï¼æ¯ç«æçæ¢¯å­ä¸ç¨³å®ï¼ - æ¯æä»£çå
 api è½¬å ç±äºæ¬äººè½åç²¾åæéï¼å¯¹äºæ½å¨çé®é¢ &
 è½æåçå°æ¹ï¼æ¬¢è¿æ¥æ issue & pull requestã ä¸¾ä¸ªæ å­ ð°ï¼
 ![èå¤©ææ](https://raw.githubusercontent.com/TheLZY/
 nonebot_plugin_tuan_chatgpt/master/examples/example2.png) ## ð ä½¿ç¨ ###
 æä»¤è¡¨
 æ³¨æï¼æä»¤ä¸­çå¢å­æ ¹æ®è®¾ç½®çnicknameä¸ºåãä¹å¯ä»¥éè¿
 @å¢å­ ä»£æ¿ã
-ç°å¨æ²¡æé»è®¤è§¦åè¯äºï¼å¦ææ²¡æè®¾ç½®nicknameï¼å°±åªè½éè¿ @
+ç°å¨æ²¡æé»è®¤è§¦åè¯åï¼å¦ææ²¡æè®¾ç½®nicknameï¼å°±åªè½éè¿ @
 è§¦åäº æä»¤çç¸åè§¦åè¯å¯èªè¡æ¥çä»£ç ä¸­ aliases é¨åã |
-æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:--
---:| | å¢å­[èå¤©åå®¹] | ç¾¤å | å¦ | ç¾¤è / ç§è |
-æ¥åå¢å­èå¤©å§ï¼ | | @å¢å­[èå¤©åå®¹] | åä¸ | æ¯ | åä¸ |
-åä¸ | | å¢å­ ççä½ç½® / ä½ å¨åªå¿ | ç¾¤å | å¦ | ç¾¤è / ç§è
-| æ¥çå¢å­èµåå°å | | å¢å­ åå²è®°å½ / history | ä¸»äºº | å¦ |
-ç¾¤è / ç§è | æ¥çåå²æé®ï¼ä¸åæ¬åç­ï¼ | | å¢å­
-æ¸é¤è®°å¿ / æ¸é¤åå²è®°å½ | ä¸»äºº | å¦ | ç¾¤è / ç§è |
-æ¸é¤å¢å­çè®°å¿ | ## ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ ``` nb plugin
-install nonebot-plugin-tuan-chatgpt # åçº§ï¼ nb plugin update nonebot-
-plugin-tuan-chatgpt ```   ä½¿ç¨ git å®è£  å®è£ï¼å¨ nonebot2
-é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, ä½¿ç¨ git å®è£ ``` git clone
-https://github.com/TheLZY/nonebot_plugin_tuan_chatgpt.git ``` åçº§ï¼ ``` git
-pull ```   ä½¿ç¨ pip å®è£ ``` pip install nonebot-plugin-tuan-chatgpt ```
-ç¯å¢éç½®ï¼ æå¼nonebotç`.env` æä»¶ï¼åå¥æ¨ç `chatgpt_api`
-ä»¥å `nickname` å¦æå¸æå¯ç¨ä»£çï¼åéè¦å¨`.env`
-æä»¶ä¸­ï¼åå¥ `chat_use_proxy = True` ä»¥å `chat_proxy_address_https =
-"ä»£çå°å"` æ `chat_proxy_address_http = "ä»£çå°å"`
+æä»¤ | æé | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:| | å¢å­
+[èå¤©åå®¹] | ç¾¤å |ç¾¤è / ç§è | æ¥åå¢å­èå¤©å§ï¼ | | å¢å­
+ççä½ç½® / ä½ å¨åªå¿ | ç¾¤å | ç¾¤è / ç§è |
+æ¥çå¢å­èµåå°å | | å¢å­ åå²è®°å½ / history | ä¸»äºº | ç¾¤è /
+ç§è | æ¥çåå²æé®ï¼ä¸åæ¬åç­ï¼ | | å¢å­ æ¸é¤è®°å¿ /
+æ¸é¤åå²è®°å½ | ç¾¤å | ç¾¤è / ç§è | æ¸é¤å¢å­çè®°å¿ | ## ð¿
+å®è£  ä½¿ç¨ nb-cli å®è£ ``` nb plugin install nonebot-plugin-tuan-chatgpt
+# åçº§ï¼ nb plugin update nonebot-plugin-tuan-chatgpt ```   ä½¿ç¨ git
+å®è£  å®è£ï¼å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, ä½¿ç¨
+git å®è£ ``` git clone https://github.com/TheLZY/
+nonebot_plugin_tuan_chatgpt.git ``` åçº§ï¼ ``` git pull ```   ä½¿ç¨ pip
+å®è£ ``` pip install nonebot-plugin-tuan-chatgpt ```  ç¯å¢éç½®ï¼
+æå¼nonebotç`.env` æä»¶ï¼åå¥æ¨ç `chatgpt_api` ä»¥å `nickname`
+å¦æå¸æå¯ç¨ä»£çï¼åéè¦å¨`.env` æä»¶ä¸­ï¼åå¥
+`chat_use_proxy = True` ä»¥å `chat_proxy_address_https = "ä»£çå°å"` æ
+`chat_proxy_address_http = "ä»£çå°å"`
 (å¤çé»è¾ç±»ä¼¼openaiï¼ä¼åä½¿ç¨httpsãä½æ¯httpsç»å¸¸ä¼æ¥éï¼aiohttpåurllib3é½å¯è½ä¼é æé®é¢ï¼ï¼æ¨èåªä½¿ç¨http)
 å¦æå¸æå¯ç¨apiè½¬å (ç±»ä¼¼ [è¾è®¯äºå½æ°æ­å»º OpenAI å½åä»£ç]
 (https://github.com/Ice-Hazymoon/openai-scf-proxy)
-éè¿äºå½æ°ç­æ¹å¼å®ç°åä»£ )ï¼åéè¦åå¥åå¥
-`chat_use_api_forward = True` ä»¥å `chat_api_address = "ä»£çå°å"`
+éè¿äºå½æ°ç­æ¹å¼å®ç°åä»£ )ï¼åéè¦åå¥ `chat_use_api_forward
+= True` ä»¥å `chat_api_address = "ä»£çå°å"`
 ä½æ¯ä¸æ¨èä¸¤èåæ¶å¯ç¨
 å¦æå¸æå¯ç¨å¾çæ¸²æï¼åéè¦åå¥ `chat_use_img2text=True`,
 ä»¥åå¨å·¥ç¨ç®å½ç `/data/tuan_chatgpt` æä»¶å¤¹ï¼`/data` æä»¶å¤¹ä¸
 `bot.py` / `env` / è¿è¡`nb run` çå°æ¹åçº§
 ï¼ä¸­åå«æ·»å å­ä½æä»¶åèæ¯æä»¶å° `/font` ä»¥å `/bachground`
 æä»¶å¤¹ä¸­ã
 é»è®¤çå­ä½æä»¶å¯åèæ¬ä»åºï¼èæ¯æä»¶åä¼ä»ä¸­éæºæ½åãæä»¶å¤¹ä¸å­å¨æ¶ä¼èªå¨åå»ºï¼ä¹å¯èªè¡è®¾å®æä»¶å¤¹è·¯å¾ã
@@ -119,15 +118,19 @@
 nonebot_plugin_tuan_chatgpt/master/examples/example_history.png) ## ð¡ TODO -
 [x] åç¾¤è®°å¿ï¼æ¯ä¸ªç¾¤ä»¥åç§èï¼è®°å¿ä¸ä¼ä¸²ï¼ - [x]
 åç­åé ï¼éè¿åæ®µå®ç°ãå¯è½ä¼èèæ¢æå¾çåéï¼ - [x]
 æ¯æä½¿ç¨ä»£ç - [x] å¢å ä»£çæµè¯
 éè¿è¿åçipå°åå¤æ­ä»£çæ¯å¦ææ ç»èµèµåæè¡ä¸­ï¼  - [x]
 ç§èååè¨é¢çéå¶ã - [x] éè¯¯å¤ç  - [x] å¼æ­¥è°ç¨ä¼å
 ï¼èªå¨éè¯ / è¿åæ¥é  ï¼ - [x] éæºäººè®¾ æè§ä¼å¾æææï¼
-- [x] éè¿@è§¦å - [ ] ä¿®æ¹äººè®¾ ï¼ - [ ] markdown æ¸²æ ï¼ - [x]
+- [x] éè¿@è§¦å - [ ] åæ¢äººè®¾
+ï¼æ³æ¥ä¸æ¯å¾éº»ç¦ï¼ä½æ¯é¢è®¾æç¹å°ãããéé
+å äºä¹ç½å .jpg å¨å¢å äººè®¾çæ¶åä¸èµ·ç¨å§ï¼ - [ ] ä¿®æ¹äººè®¾
+ï¼ å¯ä»¥ä¿å­ä¸ä¸ªjsonæä»¶å° data/charactor
+ç®å½ä¸ï¼ä»¥åå©ç¨æä»¤ä¿®æ¹ã - [ ] markdown æ¸²æ ï¼ - [x]
 ~~èªå®ä¹è§¦åæ¹å¼ï¼
 è¿ä¸ªåæ¯å¯ä»¥åä¿®æ¹è§¦åäººè®¾ä¸èµ·èå¨...ä¸è¿æè§å¨æä¿®æ¹æç¹éº»ç¦ã~~
 å¨nicknameéé¢å å§ãè¿æ¯ä¸é è½®å­äºã - [ ] ~~Openai
 æ½é£å¤çï¼ææ¶åªè¾åº 3*177 ä¸ªé¿åº¦çåç­
 å¯ä»¥æ ¹æ®ç¸åå­æ°åºç°æ¬¡æ°æ¥
 åä¸ä¸ªå­è¿ç»­åºç°6æ¬¡å¤å®ä¸ºæ½é£ï¼ï¼~~ æè¿æ²¡éå°
 é´å®ä¸ºä¸çæ¹å°±ä¸ä¼æé®é¢ - [ ] ~~é¿åç­åå¹¶è½¬å~~
```

