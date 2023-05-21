# Comparing `tmp/scorecardpipeline-0.1.4.tar.gz` & `tmp/scorecardpipeline-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scorecardpipeline-0.1.4.tar", last modified: Sun May 21 06:43:12 2023, max compression
+gzip compressed data, was "scorecardpipeline-0.1.5.tar", last modified: Sun May 21 07:08:58 2023, max compression
```

## Comparing `scorecardpipeline-0.1.4.tar` & `scorecardpipeline-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-21 06:43:12.531588 scorecardpipeline-0.1.4/
--rw-r--r--   0 lubberit   (501) staff       (20)     1065 2023-05-04 06:14:30.000000 scorecardpipeline-0.1.4/LICENSE
--rw-r--r--   0 lubberit   (501) staff       (20)    33207 2023-05-21 06:43:12.531265 scorecardpipeline-0.1.4/PKG-INFO
--rw-r--r--   0 lubberit   (501) staff       (20)    32325 2023-05-21 06:41:54.000000 scorecardpipeline-0.1.4/README.md
-drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-21 06:43:12.529021 scorecardpipeline-0.1.4/scorecardpipeline/
--rw-r--r--   0 lubberit   (501) staff       (20)      318 2023-05-21 06:04:58.000000 scorecardpipeline-0.1.4/scorecardpipeline/__init__.py
--rw-r--r--   0 lubberit   (501) staff       (20)    20443 2023-05-21 06:04:42.000000 scorecardpipeline-0.1.4/scorecardpipeline/excel_writer.py
--rw-r--r--   0 lubberit   (501) staff       (20)    19272 2023-05-21 06:42:22.000000 scorecardpipeline-0.1.4/scorecardpipeline/model.py
--rw-r--r--   0 lubberit   (501) staff       (20)    21517 2023-05-21 06:04:50.000000 scorecardpipeline-0.1.4/scorecardpipeline/processing.py
--rw-r--r--   0 lubberit   (501) staff       (20)    19966 2023-05-21 06:04:53.000000 scorecardpipeline-0.1.4/scorecardpipeline/utils.py
-drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-21 06:43:12.530791 scorecardpipeline-0.1.4/scorecardpipeline.egg-info/
--rw-r--r--   0 lubberit   (501) staff       (20)    33207 2023-05-21 06:43:12.000000 scorecardpipeline-0.1.4/scorecardpipeline.egg-info/PKG-INFO
--rw-r--r--   0 lubberit   (501) staff       (20)      380 2023-05-21 06:43:12.000000 scorecardpipeline-0.1.4/scorecardpipeline.egg-info/SOURCES.txt
--rw-r--r--   0 lubberit   (501) staff       (20)        1 2023-05-21 06:43:12.000000 scorecardpipeline-0.1.4/scorecardpipeline.egg-info/dependency_links.txt
--rw-r--r--   0 lubberit   (501) staff       (20)      214 2023-05-21 06:43:12.000000 scorecardpipeline-0.1.4/scorecardpipeline.egg-info/requires.txt
--rw-r--r--   0 lubberit   (501) staff       (20)       18 2023-05-21 06:43:12.000000 scorecardpipeline-0.1.4/scorecardpipeline.egg-info/top_level.txt
--rw-r--r--   0 lubberit   (501) staff       (20)       38 2023-05-21 06:43:12.531686 scorecardpipeline-0.1.4/setup.cfg
--rw-r--r--   0 lubberit   (501) staff       (20)     1788 2023-05-21 06:05:12.000000 scorecardpipeline-0.1.4/setup.py
+drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-21 07:08:58.669523 scorecardpipeline-0.1.5/
+-rw-r--r--   0 lubberit   (501) staff       (20)     1065 2023-05-04 06:14:30.000000 scorecardpipeline-0.1.5/LICENSE
+-rw-r--r--   0 lubberit   (501) staff       (20)    33317 2023-05-21 07:08:58.669202 scorecardpipeline-0.1.5/PKG-INFO
+-rw-r--r--   0 lubberit   (501) staff       (20)    32435 2023-05-21 07:03:59.000000 scorecardpipeline-0.1.5/README.md
+drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-21 07:08:58.666802 scorecardpipeline-0.1.5/scorecardpipeline/
+-rw-r--r--   0 lubberit   (501) staff       (20)      318 2023-05-21 07:08:50.000000 scorecardpipeline-0.1.5/scorecardpipeline/__init__.py
+-rw-r--r--   0 lubberit   (501) staff       (20)    20443 2023-05-21 06:04:42.000000 scorecardpipeline-0.1.5/scorecardpipeline/excel_writer.py
+-rw-r--r--   0 lubberit   (501) staff       (20)    19272 2023-05-21 06:49:47.000000 scorecardpipeline-0.1.5/scorecardpipeline/model.py
+-rw-r--r--   0 lubberit   (501) staff       (20)    21517 2023-05-21 06:04:50.000000 scorecardpipeline-0.1.5/scorecardpipeline/processing.py
+-rw-r--r--   0 lubberit   (501) staff       (20)    20072 2023-05-21 06:49:29.000000 scorecardpipeline-0.1.5/scorecardpipeline/utils.py
+drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-21 07:08:58.668694 scorecardpipeline-0.1.5/scorecardpipeline.egg-info/
+-rw-r--r--   0 lubberit   (501) staff       (20)    33317 2023-05-21 07:08:58.000000 scorecardpipeline-0.1.5/scorecardpipeline.egg-info/PKG-INFO
+-rw-r--r--   0 lubberit   (501) staff       (20)      380 2023-05-21 07:08:58.000000 scorecardpipeline-0.1.5/scorecardpipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 lubberit   (501) staff       (20)        1 2023-05-21 07:08:58.000000 scorecardpipeline-0.1.5/scorecardpipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 lubberit   (501) staff       (20)      205 2023-05-21 07:08:58.000000 scorecardpipeline-0.1.5/scorecardpipeline.egg-info/requires.txt
+-rw-r--r--   0 lubberit   (501) staff       (20)       18 2023-05-21 07:08:58.000000 scorecardpipeline-0.1.5/scorecardpipeline.egg-info/top_level.txt
+-rw-r--r--   0 lubberit   (501) staff       (20)       38 2023-05-21 07:08:58.669613 scorecardpipeline-0.1.5/setup.cfg
+-rw-r--r--   0 lubberit   (501) staff       (20)     1788 2023-05-21 07:08:23.000000 scorecardpipeline-0.1.5/setup.py
```

### Comparing `scorecardpipeline-0.1.4/LICENSE` & `scorecardpipeline-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scorecardpipeline-0.1.4/PKG-INFO` & `scorecardpipeline-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scorecardpipeline
-Version: 0.1.4
+Version: 0.1.5
 Summary: 评分卡pipeline建模包，封装toad、scorecardpy、optbinning等评分卡建模相关组件，API风格与sklearn高度一致，自持自定义模型报告输出
 Home-page: https://github.com/itlubber/scorecardpipeline
 Author: itlubber
 Author-email: itlubber@qq.com
 License: MIT
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # scorecardpipeline
 
-评分卡pipeline建模包，封装toad、scorecardpy、optbinning等评分卡建模相关组件，API风格与sklearn高度一致，自持自定义模型报告输出
+评分卡pipeline建模包，封装toad、scorecardpy、optbinning等评分卡建模相关组件，API风格与sklearn高度一致，支持自定义模型报告输出
 
 > 仓库地址：https://github.com/itlubber/scorecardpipeline
 > 
 > 博文地址：https://itlubber.art/archives/itlubber-scorecard-end2end
 > 
 > 微信公共号推文：https://mp.weixin.qq.com/s/eCTp4h0fau77xOgf_V28wQ
 > 
@@ -37,21 +37,21 @@
 作为一名金融搬砖工作者，评分卡建模怎么也算是基操。本文主要对笔者日常使用的评分卡建模代码进行讲解，说明如何一步步从原始数据到最终评分卡模型以及如何解读产出的模型报告文档。
 
 本文所有代码已全部提交至笔者GITHUB公开仓库，各位看官按需取用，用完记得顺带给个star以鼓励笔者继续开源相关工作。
 
 本文使用笔者对toad、scorecardpy、optbinning等库进行二次封装后的代码进行实操，文中会对仓库中的部分代码细节进行说明。本文旨在对仓库评分卡建模流程进行说明，并提供一个可以直接运行的完整示例，让更多金融从业小伙伴掌握整套评分卡模型构建方法。
 
 
-## 代码说明
+## 项目说明
 
 ### 仓库地址
 
 https://github.com/itlubber/scorecardpipeline
 
-### 项目结构
+### 代码结构
 
 该仓库下代码主要用于提供评分卡建模相关的组件，项目结构如下：
 
 ```base
 >> tree
 .
 ├── LICENSE                         # 开源协议
@@ -71,14 +71,20 @@
 
 ### 简要说明
 
 + `processing` 中提供了数据前处理相关的方法：特征筛选方法（`FeatureSelection`、`StepwiseSelection`）、变量分箱方法（`Combiner`）、变量证据权重转换方法（`WOETransformer`），方法继承`sklearn.base`中的`BaseEstimator`和`TransformerMixin`，能够支持构建`pipeline`和超参数搜索
 + `model`中提供了基于`sklearn.linear_model.LogisticRegression`实现的`ITLubberLogisticRegression`，同时重写了`toad.ScoreCard`，以支持模型相关内容的输出
 + `excel_writer` 中提供了操作 `excel` 的一系列公共方法，包含设置条件格式、设置列宽、设置数字格式、插入指定样式的内容（`insert_value2sheet`）、插入图片数据（`insert_pic2sheet`）、插入`dataframe`数据内容（`insert_df2sheet`）、保存`excel`文件（`save`）等方法
 
+### `scorecardpipeline` 安装
+
+```bash
+pip install scorecardpipeline -i https://pypi.Python.org/simple/
+```
+
 
 ## 评分卡建模
 
 ### 数据准备
 
 笔者仓库下几乎所有评分卡相关项目默认使用`scorecardpy`库中提供的`germancredit`数据集进行示例，数据集中包含类别型变量、数值型变量、样本好坏标签，共`1000`条数据，数据集中不包含缺失值，在部分示例中会随机替换数据集中的内容为缺失值，模拟实际生产中的真实数据。
```

### Comparing `scorecardpipeline-0.1.4/README.md` & `scorecardpipeline-0.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # scorecardpipeline
 
-评分卡pipeline建模包，封装toad、scorecardpy、optbinning等评分卡建模相关组件，API风格与sklearn高度一致，自持自定义模型报告输出
+评分卡pipeline建模包，封装toad、scorecardpy、optbinning等评分卡建模相关组件，API风格与sklearn高度一致，支持自定义模型报告输出
 
 > 仓库地址：https://github.com/itlubber/scorecardpipeline
 > 
 > 博文地址：https://itlubber.art/archives/itlubber-scorecard-end2end
 > 
 > 微信公共号推文：https://mp.weixin.qq.com/s/eCTp4h0fau77xOgf_V28wQ
 > 
@@ -16,21 +16,21 @@
 作为一名金融搬砖工作者，评分卡建模怎么也算是基操。本文主要对笔者日常使用的评分卡建模代码进行讲解，说明如何一步步从原始数据到最终评分卡模型以及如何解读产出的模型报告文档。
 
 本文所有代码已全部提交至笔者GITHUB公开仓库，各位看官按需取用，用完记得顺带给个star以鼓励笔者继续开源相关工作。
 
 本文使用笔者对toad、scorecardpy、optbinning等库进行二次封装后的代码进行实操，文中会对仓库中的部分代码细节进行说明。本文旨在对仓库评分卡建模流程进行说明，并提供一个可以直接运行的完整示例，让更多金融从业小伙伴掌握整套评分卡模型构建方法。
 
 
-## 代码说明
+## 项目说明
 
 ### 仓库地址
 
 https://github.com/itlubber/scorecardpipeline
 
-### 项目结构
+### 代码结构
 
 该仓库下代码主要用于提供评分卡建模相关的组件，项目结构如下：
 
 ```base
 >> tree
 .
 ├── LICENSE                         # 开源协议
@@ -50,14 +50,20 @@
 
 ### 简要说明
 
 + `processing` 中提供了数据前处理相关的方法：特征筛选方法（`FeatureSelection`、`StepwiseSelection`）、变量分箱方法（`Combiner`）、变量证据权重转换方法（`WOETransformer`），方法继承`sklearn.base`中的`BaseEstimator`和`TransformerMixin`，能够支持构建`pipeline`和超参数搜索
 + `model`中提供了基于`sklearn.linear_model.LogisticRegression`实现的`ITLubberLogisticRegression`，同时重写了`toad.ScoreCard`，以支持模型相关内容的输出
 + `excel_writer` 中提供了操作 `excel` 的一系列公共方法，包含设置条件格式、设置列宽、设置数字格式、插入指定样式的内容（`insert_value2sheet`）、插入图片数据（`insert_pic2sheet`）、插入`dataframe`数据内容（`insert_df2sheet`）、保存`excel`文件（`save`）等方法
 
+### `scorecardpipeline` 安装
+
+```bash
+pip install scorecardpipeline -i https://pypi.Python.org/simple/
+```
+
 
 ## 评分卡建模
 
 ### 数据准备
 
 笔者仓库下几乎所有评分卡相关项目默认使用`scorecardpy`库中提供的`germancredit`数据集进行示例，数据集中包含类别型变量、数值型变量、样本好坏标签，共`1000`条数据，数据集中不包含缺失值，在部分示例中会随机替换数据集中的内容为缺失值，模拟实际生产中的真实数据。
```

### Comparing `scorecardpipeline-0.1.4/scorecardpipeline/excel_writer.py` & `scorecardpipeline-0.1.5/scorecardpipeline/excel_writer.py`

 * *Files identical despite different names*

### Comparing `scorecardpipeline-0.1.4/scorecardpipeline/model.py` & `scorecardpipeline-0.1.5/scorecardpipeline/model.py`

 * *Files identical despite different names*

### Comparing `scorecardpipeline-0.1.4/scorecardpipeline/processing.py` & `scorecardpipeline-0.1.5/scorecardpipeline/processing.py`

 * *Files identical despite different names*

### Comparing `scorecardpipeline-0.1.4/scorecardpipeline/utils.py` & `scorecardpipeline-0.1.5/scorecardpipeline/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         import torch
         torch.manual_seed(seed)
         torch.cuda.manual_seed(seed)
         torch.backends.cudnn.deterministic = True
         torch.backends.cudnn.benchmark = True
 
 
-def init_setting(font_path=None):
+def init_setting(font_path=None, seed=None, freeze_torch=False):
     pd.options.display.float_format = '{:.4f}'.format
     pd.set_option('display.max_colwidth', 300)
     plt.style.use('seaborn-ticks')
     if font_path:
         if not os.path.isfile(font_path):
             import wget
             font_path = wget.download("https://itlubber.art/upload/matplot_chinese.ttf", 'matplot_chinese.ttf')
@@ -55,14 +55,17 @@
     
     # for font in font_manager.fontManager.ttflist:
     #     if "hei" in font.fname.split("/")[-1].lower():
     #         plt.rcParams['font.family'] = font.name
     #         break
     
     plt.rcParams['axes.unicode_minus'] = False
+    
+    if seed:
+        seed_everything(seed, freeze_torch=freeze_torch)
 
 
 def load_pickle(file):
     return joblib.load(file)
 
 
 def save_pickle(obj, file):
```

### Comparing `scorecardpipeline-0.1.4/scorecardpipeline.egg-info/PKG-INFO` & `scorecardpipeline-0.1.5/scorecardpipeline.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scorecardpipeline
-Version: 0.1.4
+Version: 0.1.5
 Summary: 评分卡pipeline建模包，封装toad、scorecardpy、optbinning等评分卡建模相关组件，API风格与sklearn高度一致，自持自定义模型报告输出
 Home-page: https://github.com/itlubber/scorecardpipeline
 Author: itlubber
 Author-email: itlubber@qq.com
 License: MIT
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # scorecardpipeline
 
-评分卡pipeline建模包，封装toad、scorecardpy、optbinning等评分卡建模相关组件，API风格与sklearn高度一致，自持自定义模型报告输出
+评分卡pipeline建模包，封装toad、scorecardpy、optbinning等评分卡建模相关组件，API风格与sklearn高度一致，支持自定义模型报告输出
 
 > 仓库地址：https://github.com/itlubber/scorecardpipeline
 > 
 > 博文地址：https://itlubber.art/archives/itlubber-scorecard-end2end
 > 
 > 微信公共号推文：https://mp.weixin.qq.com/s/eCTp4h0fau77xOgf_V28wQ
 > 
@@ -37,21 +37,21 @@
 作为一名金融搬砖工作者，评分卡建模怎么也算是基操。本文主要对笔者日常使用的评分卡建模代码进行讲解，说明如何一步步从原始数据到最终评分卡模型以及如何解读产出的模型报告文档。
 
 本文所有代码已全部提交至笔者GITHUB公开仓库，各位看官按需取用，用完记得顺带给个star以鼓励笔者继续开源相关工作。
 
 本文使用笔者对toad、scorecardpy、optbinning等库进行二次封装后的代码进行实操，文中会对仓库中的部分代码细节进行说明。本文旨在对仓库评分卡建模流程进行说明，并提供一个可以直接运行的完整示例，让更多金融从业小伙伴掌握整套评分卡模型构建方法。
 
 
-## 代码说明
+## 项目说明
 
 ### 仓库地址
 
 https://github.com/itlubber/scorecardpipeline
 
-### 项目结构
+### 代码结构
 
 该仓库下代码主要用于提供评分卡建模相关的组件，项目结构如下：
 
 ```base
 >> tree
 .
 ├── LICENSE                         # 开源协议
@@ -71,14 +71,20 @@
 
 ### 简要说明
 
 + `processing` 中提供了数据前处理相关的方法：特征筛选方法（`FeatureSelection`、`StepwiseSelection`）、变量分箱方法（`Combiner`）、变量证据权重转换方法（`WOETransformer`），方法继承`sklearn.base`中的`BaseEstimator`和`TransformerMixin`，能够支持构建`pipeline`和超参数搜索
 + `model`中提供了基于`sklearn.linear_model.LogisticRegression`实现的`ITLubberLogisticRegression`，同时重写了`toad.ScoreCard`，以支持模型相关内容的输出
 + `excel_writer` 中提供了操作 `excel` 的一系列公共方法，包含设置条件格式、设置列宽、设置数字格式、插入指定样式的内容（`insert_value2sheet`）、插入图片数据（`insert_pic2sheet`）、插入`dataframe`数据内容（`insert_df2sheet`）、保存`excel`文件（`save`）等方法
 
+### `scorecardpipeline` 安装
+
+```bash
+pip install scorecardpipeline -i https://pypi.Python.org/simple/
+```
+
 
 ## 评分卡建模
 
 ### 数据准备
 
 笔者仓库下几乎所有评分卡相关项目默认使用`scorecardpy`库中提供的`germancredit`数据集进行示例，数据集中包含类别型变量、数值型变量、样本好坏标签，共`1000`条数据，数据集中不包含缺失值，在部分示例中会随机替换数据集中的内容为缺失值，模拟实际生产中的真实数据。
```

### Comparing `scorecardpipeline-0.1.4/setup.py` & `scorecardpipeline-0.1.5/setup.py`

 * *Files identical despite different names*

