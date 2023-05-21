# Comparing `tmp/tomcru-0.2.8.tar.gz` & `tmp/tomcru-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomcru-0.2.8.tar", max compression
+gzip compressed data, was "tomcru-0.2.9.tar", max compression
```

## Comparing `tomcru-0.2.8.tar` & `tomcru-0.2.9.tar`

### file list

```diff
@@ -1,111 +1,112 @@
--rw-r--r--   0        0        0     1065 2023-04-17 18:29:36.244599 tomcru-0.2.8/LICENSE
--rw-r--r--   0        0        0      183 2023-04-17 18:29:36.244599 tomcru-0.2.8/README.md
--rw-r--r--   0        0        0      632 2023-05-19 12:55:57.747413 tomcru-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      474 2023-04-29 11:53:00.162328 tomcru-0.2.8/tomcru/__init__.py
--rw-r--r--   0        0        0      885 2023-04-20 17:28:59.003207 tomcru-0.2.8/tomcru/appbuilders/envmapping.py
--rw-r--r--   0        0        0     1587 2023-04-29 18:55:53.024675 tomcru-0.2.8/tomcru/appbuilders/faas/InjectableAppBase.py
--rw-r--r--   0        0        0     2936 2023-04-29 11:52:43.934414 tomcru-0.2.8/tomcru/appbuilders/faas/sam_app/SamAppBuilder.py
--rw-r--r--   0        0        0       70 2023-04-17 18:29:36.248599 tomcru-0.2.8/tomcru/appbuilders/faas/sam_app/__init__.py
--rw-r--r--   0        0        0      848 2023-04-27 10:14:15.980656 tomcru-0.2.8/tomcru/appbuilders/faas/static_app/StaticAppBuilder.py
--rw-r--r--   0        0        0       79 2023-04-17 18:29:36.248599 tomcru-0.2.8/tomcru/appbuilders/faas/static_app/__init__.py
--rw-r--r--   0        0        0     9980 2023-04-29 12:03:31.807647 tomcru-0.2.8/tomcru/cfgparsers/BaseCfgParser.py
--rw-r--r--   0        0        0     3070 2023-04-29 01:53:19.641911 tomcru-0.2.8/tomcru/cfgparsers/EnvParser.py
--rw-r--r--   0        0        0     1144 2023-04-20 10:17:05.036609 tomcru-0.2.8/tomcru/cfgparsers/MergeCfgParser.py
--rw-r--r--   0        0        0     5042 2023-05-15 22:40:30.130155 tomcru-0.2.8/tomcru/cfgparsers/SwaggerCfgParser.py
--rw-r--r--   0        0        0      322 2023-04-23 19:46:42.543716 tomcru-0.2.8/tomcru/cfgparsers/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 19:28:55.917588 tomcru-0.2.8/tomcru/core/__init__.py
--rw-r--r--   0        0        0     3291 2023-04-29 12:02:24.479889 tomcru-0.2.8/tomcru/core/cfg/api.py
--rw-r--r--   0        0        0     1164 2023-05-15 22:40:30.130155 tomcru-0.2.8/tomcru/core/cfg/authorizers.py
--rw-r--r--   0        0        0     3716 2023-04-29 12:01:41.192048 tomcru-0.2.8/tomcru/core/cfg/integrations.py
--rw-r--r--   0        0        0     2041 2023-04-29 11:52:34.486450 tomcru-0.2.8/tomcru/core/cfg/proj.py
--rw-r--r--   0        0        0      670 2023-04-29 16:16:10.250867 tomcru-0.2.8/tomcru/core/modloader.py
--rw-r--r--   0        0        0      833 2023-04-25 19:30:27.561274 tomcru-0.2.8/tomcru/core/obj_store.py
--rw-r--r--   0        0        0     2989 2023-04-29 17:03:04.510715 tomcru-0.2.8/tomcru/core/project.py
--rw-r--r--   0        0        0     2227 2023-04-29 16:20:26.534540 tomcru-0.2.8/tomcru/core/servmgr.py
--rw-r--r--   0        0        0     3802 2023-05-07 01:20:10.626850 tomcru-0.2.8/tomcru/core/utils/MyMetaLoader.py
--rw-r--r--   0        0        0      104 2023-04-20 13:43:12.977618 tomcru-0.2.8/tomcru/core/utils/__init__.py
--rw-r--r--   0        0        0     1135 2023-04-20 13:44:18.245442 tomcru-0.2.8/tomcru/core/utils/toml_custom.py
--rw-r--r--   0        0        0     2462 2023-04-17 18:29:36.252599 tomcru-0.2.8/tomcru/core/utils/yaml_custom.py
--rw-r--r--   0        0        0       72 2023-05-05 20:11:13.811402 tomcru-0.2.8/tomcru/etc/proxies/aws-sdk/index.js
--rw-r--r--   0        0        0      261 2023-05-05 20:10:34.172421 tomcru-0.2.8/tomcru/etc/proxies/aws-sdk/package.json
--rw-r--r--   0        0        0      558 2023-05-05 23:50:53.045569 tomcru-0.2.8/tomcru/etc/proxies/aws-sdk/proxylib.js
--rw-r--r--   0        0        0      873 2023-05-06 16:59:17.798252 tomcru-0.2.8/tomcru/etc/proxies/aws-sdk/serv/ddb.js
--rw-r--r--   0        0        0      703 2023-05-06 16:12:42.134096 tomcru-0.2.8/tomcru/etc/proxies/t_proxy.js
--rw-r--r--   0        0        0      540 2023-04-25 19:12:49.028297 tomcru-0.2.8/tomcru/services/ServiceBase.py
--rw-r--r--   0        0        0        0 2023-04-17 18:29:36.248599 tomcru-0.2.8/tomcru/services/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 18:29:36.248599 tomcru-0.2.8/tomcru/services/aws/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 00:05:26.709577 tomcru-0.2.8/tomcru/services/aws/hosted/apigw/__init__.py
--rw-r--r--   0        0        0     7113 2023-05-19 12:44:40.817875 tomcru-0.2.8/tomcru/services/aws/hosted/apigw/api_shared/ApiGWBuilderBase.py
--rw-r--r--   0        0        0        0 2023-04-29 03:09:12.832374 tomcru-0.2.8/tomcru/services/aws/hosted/apigw/api_shared/__init__.py
--rw-r--r--   0        0        0      835 2023-04-29 11:52:34.482450 tomcru-0.2.8/tomcru/services/aws/hosted/apigw/api_shared/integration/ExternalLambdaAuthorizerIntegration.py
--rw-r--r--   0        0        0     1604 2023-05-19 12:51:39.546701 tomcru-0.2.8/tomcru/services/aws/hosted/apigw/api_shared/integration/FlaskCorsAfterRequestHook.py
--rw-r--r--   0        0        0     2688 2023-05-01 08:08:53.636339 tomcru-0.2.8/tomcru/services/aws/hosted/apigw/api_shared/integration/LambdaAuthorizerIntegration.py
--rw-r--r--   0        0        0     3268 2023-05-18 00:03:07.541297 tomcru-0.2.8/tomcru/services/aws/hosted/apigw/api_shared/integration/OIDCAuthorizerIntegration.py
--rw-r--r--   0        0        0      711 2023-04-29 11:52:34.510450 tomcru-0.2.8/tomcru/services/aws/hosted/apigw/api_shared/integration/TomcruApiGWHttpIntegration.py
--rw-r--r--   0        0        0      322 2023-04-29 03:05:19.325205 tomcru-0.2.8/tomcru/services/aws/hosted/apigw/api_shared/integration/__init__.py
--rw-r--r--   0        0        0     5236 2023-05-19 12:44:01.661611 tomcru-0.2.8/tomcru/services/aws/hosted/apigw/flask_b/ApiGWFlaskBuilder.py
--rw-r--r--   0        0        0       85 2023-04-21 15:34:30.512217 tomcru-0.2.8/tomcru/services/aws/hosted/apigw/flask_b/__init__.py
--rw-r--r--   0        0        0      691 2023-04-17 18:29:36.248599 tomcru-0.2.8/tomcru/services/aws/hosted/apigw/flask_b/controllers/EmeProxyController.py
--rw-r--r--   0        0        0      213 2023-04-17 18:29:36.248599 tomcru-0.2.8/tomcru/services/aws/hosted/apigw/flask_b/controllers/HomeController.py
--rw-r--r--   0        0        0      236 2023-04-17 18:29:36.248599 tomcru-0.2.8/tomcru/services/aws/hosted/apigw/flask_b/controllers/SwaggerController.py
--rw-r--r--   0        0        0     3904 2023-05-18 00:27:37.541718 tomcru-0.2.8/tomcru/services/aws/hosted/apigw/flask_b/integration/LambdaIntegration.py
--rw-r--r--   0        0        0     1827 2023-05-18 00:24:53.528626 tomcru-0.2.8/tomcru/services/aws/hosted/apigw/flask_b/integration/MockedIntegration.py
--rw-r--r--   0        0        0     2553 2023-04-29 11:52:43.966414 tomcru-0.2.8/tomcru/services/aws/hosted/apigw/flask_b/integration/SwaggerIntegration.py
--rw-r--r--   0        0        0      148 2023-04-23 17:59:42.203687 tomcru-0.2.8/tomcru/services/aws/hosted/apigw/flask_b/integration/__init__.py
--rw-r--r--   0        0        0      352 2023-04-21 15:34:30.504217 tomcru-0.2.8/tomcru/services/aws/hosted/apigw/ws_b/ApiGWWebsocketBuilder.py
--rw-r--r--   0        0        0       97 2023-04-21 15:34:35.936203 tomcru-0.2.8/tomcru/services/aws/hosted/apigw/ws_b/__init__.py
--rw-r--r--   0        0        0     2994 2023-04-29 11:52:43.946414 tomcru-0.2.8/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/WsAppBuilder.py
--rw-r--r--   0        0        0       70 2023-04-17 18:29:36.248599 tomcru-0.2.8/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/__init__.py
--rw-r--r--   0        0        0     1750 2023-04-29 11:53:00.170328 tomcru-0.2.8/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/_jank.py
--rw-r--r--   0        0        0     3296 2023-04-29 11:52:34.474450 tomcru-0.2.8/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/apps/EmeWsApp.py
--rw-r--r--   0        0        0     3510 2023-04-29 11:52:43.962414 tomcru-0.2.8/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/LambdaIntegration.py
--rw-r--r--   0        0        0      205 2023-05-18 00:24:37.405021 tomcru-0.2.8/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/TomcruApiGWWsIntegration.py
--rw-r--r--   0        0        0      686 2023-04-17 18:29:36.248599 tomcru-0.2.8/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/WsEnRouteCachedAuthorizer.py
--rw-r--r--   0        0        0      853 2023-04-25 19:16:13.145908 tomcru-0.2.8/tomcru/services/aws/hosted/apigw_manager_b/ApiGWMgr.py
--rw-r--r--   0        0        0       58 2023-04-23 13:47:38.385293 tomcru-0.2.8/tomcru/services/aws/hosted/apigw_manager_b/__init__.py
--rw-r--r--   0        0        0     1477 2023-05-07 02:33:51.682008 tomcru-0.2.8/tomcru/services/aws/hosted/boto3_b/Boto3Builder.py
--rw-r--r--   0        0        0       70 2023-04-17 18:29:36.248599 tomcru-0.2.8/tomcru/services/aws/hosted/boto3_b/__init__.py
--rw-r--r--   0        0        0      622 2023-05-03 19:16:05.271285 tomcru-0.2.8/tomcru/services/aws/hosted/boto3_b/boto3.py
--rw-r--r--   0        0        0     1782 2023-04-29 22:03:41.543858 tomcru-0.2.8/tomcru/services/aws/hosted/cloudfront/flask_b/CloudfrontFlaskBuilder.py
--rw-r--r--   0        0        0      100 2023-04-29 15:54:06.512215 tomcru-0.2.8/tomcru/services/aws/hosted/cloudfront/flask_b/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 18:57:16.415271 tomcru-0.2.8/tomcru/services/aws/hosted/ddb/__init__.py
--rw-r--r--   0        0        0      993 2023-05-04 12:19:56.412205 tomcru-0.2.8/tomcru/services/aws/hosted/ddb/proxy.py
--rw-r--r--   0        0        0     8695 2023-05-13 22:09:34.428940 tomcru-0.2.8/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DDBSqlAlchemyTable.py
--rw-r--r--   0        0        0      971 2023-05-04 22:52:05.711536 tomcru-0.2.8/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DynamoDBBuilder.py
--rw-r--r--   0        0        0     1134 2023-05-09 21:53:23.860126 tomcru-0.2.8/tomcru/services/aws/hosted/ddb/sqlalchemy_b/SqlAlchemyJSONType.py
--rw-r--r--   0        0        0       79 2023-04-20 17:41:37.808233 tomcru-0.2.8/tomcru/services/aws/hosted/ddb/sqlalchemy_b/__init__.py
--rw-r--r--   0        0        0      377 2023-05-09 21:44:42.921751 tomcru-0.2.8/tomcru/services/aws/hosted/ddb/sqlalchemy_b/boto3_proxy.py
--rw-r--r--   0        0        0     5436 2023-05-09 22:04:01.245469 tomcru-0.2.8/tomcru/services/aws/hosted/ddb/sqlalchemy_b/dal_ddb.py
--rw-r--r--   0        0        0     4400 2023-05-07 02:33:48.046038 tomcru-0.2.8/tomcru/services/aws/hosted/lambda_b/LambdaBuilder.py
--rw-r--r--   0        0        0      784 2023-05-01 08:27:27.476570 tomcru-0.2.8/tomcru/services/aws/hosted/lambda_b/LambdaHostedPyContext.py
--rw-r--r--   0        0        0       74 2023-04-17 18:29:36.248599 tomcru-0.2.8/tomcru/services/aws/hosted/lambda_b/__init__.py
--rw-r--r--   0        0        0     5074 2023-05-13 17:44:03.162000 tomcru-0.2.8/tomcru/services/aws/hosted/lambda_b/proxy/Py2NodeLambdaProxy.py
--rw-r--r--   0        0        0     2585 2023-05-12 20:18:40.139204 tomcru-0.2.8/tomcru/services/aws/hosted/s3_b/S3AdapterLocal.py
--rw-r--r--   0        0        0      585 2023-05-09 23:34:07.782900 tomcru-0.2.8/tomcru/services/aws/hosted/s3_b/S3Service.py
--rw-r--r--   0        0        0       61 2023-04-25 22:42:25.629435 tomcru-0.2.8/tomcru/services/aws/hosted/s3_b/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 18:29:36.248599 tomcru-0.2.8/tomcru/services/aws/onpremise/__init__.py
--rw-r--r--   0        0        0     4043 2023-04-29 11:53:00.190328 tomcru-0.2.8/tomcru/services/aws/onpremise/model_checker/SwaggerResponseModelValidator.py
--rw-r--r--   0        0        0      121 2023-04-17 18:29:36.248599 tomcru-0.2.8/tomcru/services/aws/onpremise/model_checker/__init__.py
--rw-r--r--   0        0        0      782 2023-04-29 11:52:34.530450 tomcru-0.2.8/tomcru/services/aws/onpremise/s3_static/S3StaticBuilder.py
--rw-r--r--   0        0        0       78 2023-04-17 18:29:36.248599 tomcru-0.2.8/tomcru/services/aws/onpremise/s3_static/__init__.py
--rw-r--r--   0        0        0     7308 2023-04-17 18:29:36.248599 tomcru-0.2.8/tomcru/services/aws/sam/_junk/SamTplBuilder.py
--rw-r--r--   0        0        0      841 2023-04-17 18:29:36.248599 tomcru-0.2.8/tomcru/services/aws/sam/_junk/core.yaml
--rw-r--r--   0        0        0      855 2023-04-17 18:29:36.248599 tomcru-0.2.8/tomcru/services/aws/sam/_junk/httpapi.yaml
--rw-r--r--   0        0        0      372 2023-04-17 18:29:36.248599 tomcru-0.2.8/tomcru/services/aws/sam/_junk/integ_normal.yaml
--rw-r--r--   0        0        0      638 2023-04-17 18:29:36.248599 tomcru-0.2.8/tomcru/services/aws/sam/_junk/integ_ws.yaml
--rw-r--r--   0        0        0      153 2023-04-17 18:29:36.248599 tomcru-0.2.8/tomcru/services/aws/sam/_junk/lambda.yaml
--rw-r--r--   0        0        0      231 2023-04-17 18:29:36.248599 tomcru-0.2.8/tomcru/services/aws/sam/_junk/layer.yaml
--rw-r--r--   0        0        0     4389 2023-04-17 18:29:36.248599 tomcru-0.2.8/tomcru/services/aws/sam/_junk/template.yaml
--rw-r--r--   0        0        0     1027 2023-04-17 18:29:36.248599 tomcru-0.2.8/tomcru/services/aws/sam/_junk/wsapi.yaml
--rw-r--r--   0        0        0     2101 2023-04-29 11:53:00.174328 tomcru-0.2.8/tomcru/services/aws/sam/lambda_b/LambdaBuilder.py
--rw-r--r--   0        0        0       74 2023-04-17 18:29:36.248599 tomcru-0.2.8/tomcru/services/aws/sam/lambda_b/__init__.py
--rw-r--r--   0        0        0     1344 2023-04-29 11:53:00.154328 tomcru-0.2.8/tomcru/services/aws/sam/params_b/ParametersBuilder.py
--rw-r--r--   0        0        0       85 2023-04-17 18:29:36.248599 tomcru-0.2.8/tomcru/services/aws/sam/params_b/__init__.py
--rw-r--r--   0        0        0     2725 2023-04-29 11:53:00.170328 tomcru-0.2.8/tomcru/services/aws/sam/spec_api_b/SwaggerApiTemplater.py
--rw-r--r--   0        0        0       91 2023-04-17 18:29:36.248599 tomcru-0.2.8/tomcru/services/aws/sam/spec_api_b/__init__.py
--rw-r--r--   0        0        0     1757 2023-04-29 11:52:34.502450 tomcru-0.2.8/tomcru/services/aws/sam/spec_api_b/authorizers/SAMLambdaAuthBuilder.py
--rw-r--r--   0        0        0      774 2023-04-29 11:52:34.470450 tomcru-0.2.8/tomcru/services/aws/sam/spec_api_b/authorizers/SAMOIDCAuthBuilder.py
--rw-r--r--   0        0        0      835 2023-04-29 11:52:43.962414 tomcru-0.2.8/tomcru/services/aws/sam/spec_api_b/integrations/SAMLambdaBuilder.py
--rw-r--r--   0        0        0     2266 2023-04-29 11:52:43.970414 tomcru-0.2.8/tomcru/services/general/eme2swagger/Eme2Swagger.py
--rw-r--r--   0        0        0       67 2023-04-17 18:29:36.252599 tomcru-0.2.8/tomcru/services/general/eme2swagger/__init__.py
--rw-r--r--   0        0        0     1047 1970-01-01 00:00:00.000000 tomcru-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-17 18:29:36.244599 tomcru-0.2.9/LICENSE
+-rw-r--r--   0        0        0      183 2023-04-17 18:29:36.244599 tomcru-0.2.9/README.md
+-rw-r--r--   0        0        0      632 2023-05-20 16:20:48.409970 tomcru-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      474 2023-04-29 11:53:00.162328 tomcru-0.2.9/tomcru/__init__.py
+-rw-r--r--   0        0        0      885 2023-04-20 17:28:59.003207 tomcru-0.2.9/tomcru/appbuilders/envmapping.py
+-rw-r--r--   0        0        0     1615 2023-05-20 15:16:54.612458 tomcru-0.2.9/tomcru/appbuilders/faas/InjectableAppBase.py
+-rw-r--r--   0        0        0     2936 2023-04-29 11:52:43.934414 tomcru-0.2.9/tomcru/appbuilders/faas/sam_app/SamAppBuilder.py
+-rw-r--r--   0        0        0       70 2023-04-17 18:29:36.248599 tomcru-0.2.9/tomcru/appbuilders/faas/sam_app/__init__.py
+-rw-r--r--   0        0        0      848 2023-04-27 10:14:15.980656 tomcru-0.2.9/tomcru/appbuilders/faas/static_app/StaticAppBuilder.py
+-rw-r--r--   0        0        0       79 2023-04-17 18:29:36.248599 tomcru-0.2.9/tomcru/appbuilders/faas/static_app/__init__.py
+-rw-r--r--   0        0        0     9980 2023-04-29 12:03:31.807647 tomcru-0.2.9/tomcru/cfgparsers/BaseCfgParser.py
+-rw-r--r--   0        0        0     3070 2023-04-29 01:53:19.641911 tomcru-0.2.9/tomcru/cfgparsers/EnvParser.py
+-rw-r--r--   0        0        0     1144 2023-04-20 10:17:05.036609 tomcru-0.2.9/tomcru/cfgparsers/MergeCfgParser.py
+-rw-r--r--   0        0        0     5042 2023-05-15 22:40:30.130155 tomcru-0.2.9/tomcru/cfgparsers/SwaggerCfgParser.py
+-rw-r--r--   0        0        0      322 2023-04-23 19:46:42.543716 tomcru-0.2.9/tomcru/cfgparsers/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 19:28:55.917588 tomcru-0.2.9/tomcru/core/__init__.py
+-rw-r--r--   0        0        0     3291 2023-04-29 12:02:24.479889 tomcru-0.2.9/tomcru/core/cfg/api.py
+-rw-r--r--   0        0        0     1164 2023-05-15 22:40:30.130155 tomcru-0.2.9/tomcru/core/cfg/authorizers.py
+-rw-r--r--   0        0        0     3716 2023-04-29 12:01:41.192048 tomcru-0.2.9/tomcru/core/cfg/integrations.py
+-rw-r--r--   0        0        0     2103 2023-05-20 15:10:36.085264 tomcru-0.2.9/tomcru/core/cfg/proj.py
+-rw-r--r--   0        0        0      784 2023-05-20 14:56:16.513268 tomcru-0.2.9/tomcru/core/logger.py
+-rw-r--r--   0        0        0      670 2023-04-29 16:16:10.250867 tomcru-0.2.9/tomcru/core/modloader.py
+-rw-r--r--   0        0        0      833 2023-04-25 19:30:27.561274 tomcru-0.2.9/tomcru/core/obj_store.py
+-rw-r--r--   0        0        0     2091 2023-05-20 15:11:10.028634 tomcru-0.2.9/tomcru/core/project.py
+-rw-r--r--   0        0        0     2227 2023-04-29 16:20:26.534540 tomcru-0.2.9/tomcru/core/servmgr.py
+-rw-r--r--   0        0        0     3802 2023-05-07 01:20:10.626850 tomcru-0.2.9/tomcru/core/utils/MyMetaLoader.py
+-rw-r--r--   0        0        0      104 2023-04-20 13:43:12.977618 tomcru-0.2.9/tomcru/core/utils/__init__.py
+-rw-r--r--   0        0        0     1135 2023-04-20 13:44:18.245442 tomcru-0.2.9/tomcru/core/utils/toml_custom.py
+-rw-r--r--   0        0        0     2462 2023-04-17 18:29:36.252599 tomcru-0.2.9/tomcru/core/utils/yaml_custom.py
+-rw-r--r--   0        0        0       72 2023-05-05 20:11:13.811402 tomcru-0.2.9/tomcru/etc/proxies/aws-sdk/index.js
+-rw-r--r--   0        0        0      261 2023-05-05 20:10:34.172421 tomcru-0.2.9/tomcru/etc/proxies/aws-sdk/package.json
+-rw-r--r--   0        0        0      558 2023-05-05 23:50:53.045569 tomcru-0.2.9/tomcru/etc/proxies/aws-sdk/proxylib.js
+-rw-r--r--   0        0        0      873 2023-05-06 16:59:17.798252 tomcru-0.2.9/tomcru/etc/proxies/aws-sdk/serv/ddb.js
+-rw-r--r--   0        0        0      703 2023-05-06 16:12:42.134096 tomcru-0.2.9/tomcru/etc/proxies/t_proxy.js
+-rw-r--r--   0        0        0      540 2023-04-25 19:12:49.028297 tomcru-0.2.9/tomcru/services/ServiceBase.py
+-rw-r--r--   0        0        0        0 2023-04-17 18:29:36.248599 tomcru-0.2.9/tomcru/services/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 18:29:36.248599 tomcru-0.2.9/tomcru/services/aws/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 00:05:26.709577 tomcru-0.2.9/tomcru/services/aws/hosted/apigw/__init__.py
+-rw-r--r--   0        0        0     7174 2023-05-20 15:54:04.339614 tomcru-0.2.9/tomcru/services/aws/hosted/apigw/api_shared/ApiGWBuilderBase.py
+-rw-r--r--   0        0        0        0 2023-04-29 03:09:12.832374 tomcru-0.2.9/tomcru/services/aws/hosted/apigw/api_shared/__init__.py
+-rw-r--r--   0        0        0      835 2023-04-29 11:52:34.482450 tomcru-0.2.9/tomcru/services/aws/hosted/apigw/api_shared/integration/ExternalLambdaAuthorizerIntegration.py
+-rw-r--r--   0        0        0     1604 2023-05-19 12:51:39.546701 tomcru-0.2.9/tomcru/services/aws/hosted/apigw/api_shared/integration/FlaskCorsAfterRequestHook.py
+-rw-r--r--   0        0        0     2688 2023-05-01 08:08:53.636339 tomcru-0.2.9/tomcru/services/aws/hosted/apigw/api_shared/integration/LambdaAuthorizerIntegration.py
+-rw-r--r--   0        0        0     3306 2023-05-20 15:54:04.359614 tomcru-0.2.9/tomcru/services/aws/hosted/apigw/api_shared/integration/OIDCAuthorizerIntegration.py
+-rw-r--r--   0        0        0      711 2023-04-29 11:52:34.510450 tomcru-0.2.9/tomcru/services/aws/hosted/apigw/api_shared/integration/TomcruApiGWHttpIntegration.py
+-rw-r--r--   0        0        0      322 2023-04-29 03:05:19.325205 tomcru-0.2.9/tomcru/services/aws/hosted/apigw/api_shared/integration/__init__.py
+-rw-r--r--   0        0        0     5236 2023-05-19 12:44:01.661611 tomcru-0.2.9/tomcru/services/aws/hosted/apigw/flask_b/ApiGWFlaskBuilder.py
+-rw-r--r--   0        0        0       85 2023-04-21 15:34:30.512217 tomcru-0.2.9/tomcru/services/aws/hosted/apigw/flask_b/__init__.py
+-rw-r--r--   0        0        0      691 2023-04-17 18:29:36.248599 tomcru-0.2.9/tomcru/services/aws/hosted/apigw/flask_b/controllers/EmeProxyController.py
+-rw-r--r--   0        0        0      213 2023-04-17 18:29:36.248599 tomcru-0.2.9/tomcru/services/aws/hosted/apigw/flask_b/controllers/HomeController.py
+-rw-r--r--   0        0        0      236 2023-04-17 18:29:36.248599 tomcru-0.2.9/tomcru/services/aws/hosted/apigw/flask_b/controllers/SwaggerController.py
+-rw-r--r--   0        0        0     3904 2023-05-18 00:27:37.541718 tomcru-0.2.9/tomcru/services/aws/hosted/apigw/flask_b/integration/LambdaIntegration.py
+-rw-r--r--   0        0        0     1827 2023-05-18 00:24:53.528626 tomcru-0.2.9/tomcru/services/aws/hosted/apigw/flask_b/integration/MockedIntegration.py
+-rw-r--r--   0        0        0     2553 2023-04-29 11:52:43.966414 tomcru-0.2.9/tomcru/services/aws/hosted/apigw/flask_b/integration/SwaggerIntegration.py
+-rw-r--r--   0        0        0      148 2023-04-23 17:59:42.203687 tomcru-0.2.9/tomcru/services/aws/hosted/apigw/flask_b/integration/__init__.py
+-rw-r--r--   0        0        0      352 2023-04-21 15:34:30.504217 tomcru-0.2.9/tomcru/services/aws/hosted/apigw/ws_b/ApiGWWebsocketBuilder.py
+-rw-r--r--   0        0        0       97 2023-04-21 15:34:35.936203 tomcru-0.2.9/tomcru/services/aws/hosted/apigw/ws_b/__init__.py
+-rw-r--r--   0        0        0     2994 2023-04-29 11:52:43.946414 tomcru-0.2.9/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/WsAppBuilder.py
+-rw-r--r--   0        0        0       70 2023-04-17 18:29:36.248599 tomcru-0.2.9/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/__init__.py
+-rw-r--r--   0        0        0     1750 2023-04-29 11:53:00.170328 tomcru-0.2.9/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/_jank.py
+-rw-r--r--   0        0        0     3296 2023-04-29 11:52:34.474450 tomcru-0.2.9/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/apps/EmeWsApp.py
+-rw-r--r--   0        0        0     3510 2023-04-29 11:52:43.962414 tomcru-0.2.9/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/LambdaIntegration.py
+-rw-r--r--   0        0        0      205 2023-05-18 00:24:37.405021 tomcru-0.2.9/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/TomcruApiGWWsIntegration.py
+-rw-r--r--   0        0        0      686 2023-04-17 18:29:36.248599 tomcru-0.2.9/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/WsEnRouteCachedAuthorizer.py
+-rw-r--r--   0        0        0      853 2023-04-25 19:16:13.145908 tomcru-0.2.9/tomcru/services/aws/hosted/apigw_manager_b/ApiGWMgr.py
+-rw-r--r--   0        0        0       58 2023-04-23 13:47:38.385293 tomcru-0.2.9/tomcru/services/aws/hosted/apigw_manager_b/__init__.py
+-rw-r--r--   0        0        0     1477 2023-05-07 02:33:51.682008 tomcru-0.2.9/tomcru/services/aws/hosted/boto3_b/Boto3Builder.py
+-rw-r--r--   0        0        0       70 2023-04-17 18:29:36.248599 tomcru-0.2.9/tomcru/services/aws/hosted/boto3_b/__init__.py
+-rw-r--r--   0        0        0      622 2023-05-03 19:16:05.271285 tomcru-0.2.9/tomcru/services/aws/hosted/boto3_b/boto3.py
+-rw-r--r--   0        0        0     1782 2023-04-29 22:03:41.543858 tomcru-0.2.9/tomcru/services/aws/hosted/cloudfront/flask_b/CloudfrontFlaskBuilder.py
+-rw-r--r--   0        0        0      100 2023-04-29 15:54:06.512215 tomcru-0.2.9/tomcru/services/aws/hosted/cloudfront/flask_b/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 18:57:16.415271 tomcru-0.2.9/tomcru/services/aws/hosted/ddb/__init__.py
+-rw-r--r--   0        0        0      993 2023-05-04 12:19:56.412205 tomcru-0.2.9/tomcru/services/aws/hosted/ddb/proxy.py
+-rw-r--r--   0        0        0     8695 2023-05-13 22:09:34.428940 tomcru-0.2.9/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DDBSqlAlchemyTable.py
+-rw-r--r--   0        0        0      971 2023-05-04 22:52:05.711536 tomcru-0.2.9/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DynamoDBBuilder.py
+-rw-r--r--   0        0        0     1134 2023-05-09 21:53:23.860126 tomcru-0.2.9/tomcru/services/aws/hosted/ddb/sqlalchemy_b/SqlAlchemyJSONType.py
+-rw-r--r--   0        0        0       79 2023-04-20 17:41:37.808233 tomcru-0.2.9/tomcru/services/aws/hosted/ddb/sqlalchemy_b/__init__.py
+-rw-r--r--   0        0        0      377 2023-05-09 21:44:42.921751 tomcru-0.2.9/tomcru/services/aws/hosted/ddb/sqlalchemy_b/boto3_proxy.py
+-rw-r--r--   0        0        0     5436 2023-05-09 22:04:01.245469 tomcru-0.2.9/tomcru/services/aws/hosted/ddb/sqlalchemy_b/dal_ddb.py
+-rw-r--r--   0        0        0     4400 2023-05-07 02:33:48.046038 tomcru-0.2.9/tomcru/services/aws/hosted/lambda_b/LambdaBuilder.py
+-rw-r--r--   0        0        0      784 2023-05-01 08:27:27.476570 tomcru-0.2.9/tomcru/services/aws/hosted/lambda_b/LambdaHostedPyContext.py
+-rw-r--r--   0        0        0       74 2023-04-17 18:29:36.248599 tomcru-0.2.9/tomcru/services/aws/hosted/lambda_b/__init__.py
+-rw-r--r--   0        0        0     5120 2023-05-20 16:14:57.915247 tomcru-0.2.9/tomcru/services/aws/hosted/lambda_b/proxy/Py2NodeLambdaProxy.py
+-rw-r--r--   0        0        0     2646 2023-05-20 16:08:55.310229 tomcru-0.2.9/tomcru/services/aws/hosted/s3_b/S3AdapterLocal.py
+-rw-r--r--   0        0        0      585 2023-05-09 23:34:07.782900 tomcru-0.2.9/tomcru/services/aws/hosted/s3_b/S3Service.py
+-rw-r--r--   0        0        0       61 2023-04-25 22:42:25.629435 tomcru-0.2.9/tomcru/services/aws/hosted/s3_b/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 18:29:36.248599 tomcru-0.2.9/tomcru/services/aws/onpremise/__init__.py
+-rw-r--r--   0        0        0     4018 2023-05-20 16:09:42.289700 tomcru-0.2.9/tomcru/services/aws/onpremise/model_checker/SwaggerResponseModelValidator.py
+-rw-r--r--   0        0        0      121 2023-04-17 18:29:36.248599 tomcru-0.2.9/tomcru/services/aws/onpremise/model_checker/__init__.py
+-rw-r--r--   0        0        0      782 2023-04-29 11:52:34.530450 tomcru-0.2.9/tomcru/services/aws/onpremise/s3_static/S3StaticBuilder.py
+-rw-r--r--   0        0        0       78 2023-04-17 18:29:36.248599 tomcru-0.2.9/tomcru/services/aws/onpremise/s3_static/__init__.py
+-rw-r--r--   0        0        0     7308 2023-04-17 18:29:36.248599 tomcru-0.2.9/tomcru/services/aws/sam/_junk/SamTplBuilder.py
+-rw-r--r--   0        0        0      841 2023-04-17 18:29:36.248599 tomcru-0.2.9/tomcru/services/aws/sam/_junk/core.yaml
+-rw-r--r--   0        0        0      855 2023-04-17 18:29:36.248599 tomcru-0.2.9/tomcru/services/aws/sam/_junk/httpapi.yaml
+-rw-r--r--   0        0        0      372 2023-04-17 18:29:36.248599 tomcru-0.2.9/tomcru/services/aws/sam/_junk/integ_normal.yaml
+-rw-r--r--   0        0        0      638 2023-04-17 18:29:36.248599 tomcru-0.2.9/tomcru/services/aws/sam/_junk/integ_ws.yaml
+-rw-r--r--   0        0        0      153 2023-04-17 18:29:36.248599 tomcru-0.2.9/tomcru/services/aws/sam/_junk/lambda.yaml
+-rw-r--r--   0        0        0      231 2023-04-17 18:29:36.248599 tomcru-0.2.9/tomcru/services/aws/sam/_junk/layer.yaml
+-rw-r--r--   0        0        0     4389 2023-04-17 18:29:36.248599 tomcru-0.2.9/tomcru/services/aws/sam/_junk/template.yaml
+-rw-r--r--   0        0        0     1027 2023-04-17 18:29:36.248599 tomcru-0.2.9/tomcru/services/aws/sam/_junk/wsapi.yaml
+-rw-r--r--   0        0        0     2101 2023-04-29 11:53:00.174328 tomcru-0.2.9/tomcru/services/aws/sam/lambda_b/LambdaBuilder.py
+-rw-r--r--   0        0        0       74 2023-04-17 18:29:36.248599 tomcru-0.2.9/tomcru/services/aws/sam/lambda_b/__init__.py
+-rw-r--r--   0        0        0     1344 2023-04-29 11:53:00.154328 tomcru-0.2.9/tomcru/services/aws/sam/params_b/ParametersBuilder.py
+-rw-r--r--   0        0        0       85 2023-04-17 18:29:36.248599 tomcru-0.2.9/tomcru/services/aws/sam/params_b/__init__.py
+-rw-r--r--   0        0        0     2725 2023-04-29 11:53:00.170328 tomcru-0.2.9/tomcru/services/aws/sam/spec_api_b/SwaggerApiTemplater.py
+-rw-r--r--   0        0        0       91 2023-04-17 18:29:36.248599 tomcru-0.2.9/tomcru/services/aws/sam/spec_api_b/__init__.py
+-rw-r--r--   0        0        0     1757 2023-04-29 11:52:34.502450 tomcru-0.2.9/tomcru/services/aws/sam/spec_api_b/authorizers/SAMLambdaAuthBuilder.py
+-rw-r--r--   0        0        0      774 2023-04-29 11:52:34.470450 tomcru-0.2.9/tomcru/services/aws/sam/spec_api_b/authorizers/SAMOIDCAuthBuilder.py
+-rw-r--r--   0        0        0      835 2023-04-29 11:52:43.962414 tomcru-0.2.9/tomcru/services/aws/sam/spec_api_b/integrations/SAMLambdaBuilder.py
+-rw-r--r--   0        0        0     2266 2023-04-29 11:52:43.970414 tomcru-0.2.9/tomcru/services/general/eme2swagger/Eme2Swagger.py
+-rw-r--r--   0        0        0       67 2023-04-17 18:29:36.252599 tomcru-0.2.9/tomcru/services/general/eme2swagger/__init__.py
+-rw-r--r--   0        0        0     1047 1970-01-01 00:00:00.000000 tomcru-0.2.9/PKG-INFO
```

### Comparing `tomcru-0.2.8/LICENSE` & `tomcru-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/pyproject.toml` & `tomcru-0.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tomcru"
-version = "0.2.8"
+version = "0.2.9"
 description = "Serverless app framework"
 authors = ["Rajmund Csombordi <rajmund.csombordi@hotmail.com>"]
 readme = "README.md"
 packages = [{include = "tomcru"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -15,12 +15,12 @@
 pyjwt = ">=2.6,<3.0"
 requests = ">=2.28,<3.0"
 botocore = ">=1.29,<2.0"
 pyyaml = "^6.0"
 flatten-json = "^0.1.13"
 deepmerge = "^1.1.0"
 tabulate = "^0.9.0"
-tomcru-jerry = "^0.1.2"
+tomcru-jerry = "^0.1.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tomcru-0.2.8/tomcru/appbuilders/envmapping.py` & `tomcru-0.2.9/tomcru/appbuilders/envmapping.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/appbuilders/faas/InjectableAppBase.py` & `tomcru-0.2.9/tomcru/appbuilders/faas/InjectableAppBase.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,13 @@
+import logging
+
 from tomcru.core import utils
 
+logger = logging.getLogger('tomcru')
+
 
 class InjectableAppBase:
 
     def __init__(self, proj: 'TomcruProject', cfg: 'TomcruProjectCfg', env: 'TomcruEnvCfg'):
         self.p = proj
         self.env = env
         self.cfg = cfg
@@ -20,19 +24,18 @@
                 service.inject_dependencies()
 
         if not self.inited:
             self.inited = True
 
             for serv_id, service in sorted(self.p.srvmgr, key=lambda s: s[1].INIT_PRIORITY):
                 if hasattr(service, 'init'):
-                    # todo: debug
-                    print(f"Initializing service {serv_id}[ENV={self.env.env}]")
+                    logger.debug(f"[{serv_id}] initializing (ENV={self.env.env})")
                     service.init()
                 else:
-                    print(f"Skipping init on {serv_id}[ENV={self.env.env}]")
+                    logger.debug(f"[{serv_id}] skipped init (ENV={self.env.env})")
 
         return self
 
     def __exit__(self, exc_type=None, exc_val=None, exc_tb=None):
         for serv_id, service in self.p.srvmgr:
             if hasattr(service, 'deject_dependencies'):
                 service.deject_dependencies()
```

### Comparing `tomcru-0.2.8/tomcru/appbuilders/faas/sam_app/SamAppBuilder.py` & `tomcru-0.2.9/tomcru/appbuilders/faas/sam_app/SamAppBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/appbuilders/faas/static_app/StaticAppBuilder.py` & `tomcru-0.2.9/tomcru/appbuilders/faas/static_app/StaticAppBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/cfgparsers/BaseCfgParser.py` & `tomcru-0.2.9/tomcru/cfgparsers/BaseCfgParser.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/cfgparsers/EnvParser.py` & `tomcru-0.2.9/tomcru/cfgparsers/EnvParser.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/cfgparsers/MergeCfgParser.py` & `tomcru-0.2.9/tomcru/cfgparsers/MergeCfgParser.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/cfgparsers/SwaggerCfgParser.py` & `tomcru-0.2.9/tomcru/cfgparsers/SwaggerCfgParser.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/core/cfg/api.py` & `tomcru-0.2.9/tomcru/core/cfg/api.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/core/cfg/authorizers.py` & `tomcru-0.2.9/tomcru/core/cfg/authorizers.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/core/cfg/integrations.py` & `tomcru-0.2.9/tomcru/core/cfg/integrations.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/core/cfg/proj.py` & `tomcru-0.2.9/tomcru/core/cfg/proj.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     def __init__(self, env_id: str, cfg: dict):
         self.app_path: str | None = None
         self.env_id: str = env_id
         self.env: str = cfg['envcfg']['env']
         self.vendors: list[str] = cfg['envcfg']['vendors']
         self.target: str = cfg['envcfg']['target']
         self.service_type: str = cfg['envcfg'].get('service_type', 'faas')
+        self.logging: dict = cfg.get['envcfg'].get('logging')
 
         # environment variables for various services
         self.global_envvars: dict[str, str] = {}
         self.envvars_lamb: dict[str, dict[str, dict]] = defaultdict(dict)
 
         # service specifications
         self.serv_opts: dict[str, SettingWrapper] = {}
```

### Comparing `tomcru-0.2.8/tomcru/core/modloader.py` & `tomcru-0.2.9/tomcru/core/modloader.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/core/obj_store.py` & `tomcru-0.2.9/tomcru/core/obj_store.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/core/project.py` & `tomcru-0.2.9/tomcru/core/project.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 
+from .logger import init_logging
 from .obj_store import ObjStore
 from .servmgr import ServiceManager
 from ..appbuilders.envmapping import map_env_to_appbuilder
 from ..cfgparsers import BaseCfgParser, _parsers
 from .cfg.proj import TomcruSubProjectCfg, TomcruEnvCfg
 from ..appbuilders.faas.InjectableAppBase import InjectableAppBase
 
@@ -56,39 +57,14 @@
         :return:
         """
         _env = self.envs.get(env_id)
 
         if not _env:
             _cfg = self.cfg if cfg_id is None else self.cfgs[cfg_id]
 
-            # todo: itt: return EnvAppBuilder
-            _env = map_env_to_appbuilder(self, _cfg, self.envcfgs[env_id])
+            envcfg = self.envcfgs[env_id]
+            init_logging(envcfg.logging.get('loglvl', 'DEBUG'), envcfg.logging.get('filepath'))
+
+            _env = map_env_to_appbuilder(self, _cfg, envcfg)
             self.envs[env_id] = _env
 
         return _env
-    #
-    # @deprecated("Don't call services from the project, instead use environment")
-    # def serv(self, name):
-    #     env = self.find_env_from_legacy_name(name)
-    #
-    #     # load service into cache; cfg
-    #     return self.env(env.env_id).serv(name)
-    #
-    # @deprecated("Don't call services from the project, instead use environment")
-    # def find_env_from_legacy_name(self, name) -> TomcruEnvCfg:
-    #     n = name.split(':')
-    #     vendor, target, service_id = n
-    #     if not target:
-    #         target = ''
-    #     if not vendor:
-    #         vendor = 'general'
-    #
-    #     if target == 'onpremise':
-    #         # @note: hosted frameworks were incorrectly labeled as onpremise
-    #         target = 'hosted'
-    #
-    #     env: TomcruEnvCfg = next(filter(lambda env: env.target == target and vendor in env.vendors, self.envcfgs.values()), None)
-    #
-    #     if env is None:
-    #         raise Exception(f"Service not found: {name}")
-    #
-    #     return env
```

### Comparing `tomcru-0.2.8/tomcru/core/servmgr.py` & `tomcru-0.2.9/tomcru/core/servmgr.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/core/utils/MyMetaLoader.py` & `tomcru-0.2.9/tomcru/core/utils/MyMetaLoader.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/core/utils/toml_custom.py` & `tomcru-0.2.9/tomcru/core/utils/toml_custom.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/core/utils/yaml_custom.py` & `tomcru-0.2.9/tomcru/core/utils/yaml_custom.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/etc/proxies/aws-sdk/proxylib.js` & `tomcru-0.2.9/tomcru/etc/proxies/aws-sdk/proxylib.js`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/etc/proxies/aws-sdk/serv/ddb.js` & `tomcru-0.2.9/tomcru/etc/proxies/aws-sdk/serv/ddb.js`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/etc/proxies/t_proxy.js` & `tomcru-0.2.9/tomcru/etc/proxies/t_proxy.js`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/ServiceBase.py` & `tomcru-0.2.9/tomcru/services/ServiceBase.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/hosted/apigw/api_shared/ApiGWBuilderBase.py` & `tomcru-0.2.9/tomcru/services/aws/hosted/apigw/api_shared/ApiGWBuilderBase.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+import logging
 import os.path
 
 from abc import ABCMeta, abstractmethod
 
 from tomcru.services.ServiceBase import ServiceBase
 from tomcru import TomcruApiEP, TomcruEndpoint, TomcruRouteEP, TomcruSwaggerIntegrationEP, TomcruApiLambdaAuthorizerEP, TomcruApiOIDCAuthorizerEP
 from .integration import TomcruApiGWHttpIntegration, TomcruApiGWAuthorizerIntegration, LambdaAuthorizerIntegration, ExternalLambdaAuthorizerIntegration, OIDCAuthorizerIntegration
 
 __dir__ = os.path.dirname(os.path.realpath(__file__))
+logger = logging.getLogger('tomcru')
 
 
 class ApiGWBuilderBase(ServiceBase, metaclass=ABCMeta):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
@@ -107,15 +109,15 @@
             for endpoint in ro.endpoints:
                 auth = self.authorizers[endpoint.auth] if endpoint.auth else None
 
                 # refer to integration (proxy controller refers to self.on_request)
                 _integration: TomcruApiGWHttpIntegration = self.get_integration(api, endpoint, auth)
 
                 if _integration is None:
-                    print(f"Not found integration for {endpoint}")
+                    logger.warning(f"Not found integration for {endpoint}")
                     continue
                 self.integrations[endpoint] = _integration
                 self.add_method(api, ro, endpoint, apiopts, _integration)
 
                 if endpoint.route == '/':
                     _index = endpoint
```

### Comparing `tomcru-0.2.8/tomcru/services/aws/hosted/apigw/api_shared/integration/ExternalLambdaAuthorizerIntegration.py` & `tomcru-0.2.9/tomcru/services/aws/hosted/apigw/api_shared/integration/ExternalLambdaAuthorizerIntegration.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/hosted/apigw/api_shared/integration/FlaskCorsAfterRequestHook.py` & `tomcru-0.2.9/tomcru/services/aws/hosted/apigw/api_shared/integration/FlaskCorsAfterRequestHook.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/hosted/apigw/api_shared/integration/LambdaAuthorizerIntegration.py` & `tomcru-0.2.9/tomcru/services/aws/hosted/apigw/api_shared/integration/LambdaAuthorizerIntegration.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/hosted/apigw/api_shared/integration/OIDCAuthorizerIntegration.py` & `tomcru-0.2.9/tomcru/services/aws/hosted/apigw/api_shared/integration/OIDCAuthorizerIntegration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,17 @@
+import logging
+
 import requests
 from .TomcruApiGWHttpIntegration import TomcruApiGWAuthorizerIntegration
 from tomcru import TomcruApiOIDCAuthorizerEP
 
-from flask import request
+
+logger = logging.getLogger('tomcru')
+
+
 class AWSOIDCException(Exception):
     pass
 
 
 class OIDCAuthorizerIntegration(TomcruApiGWAuthorizerIntegration):
 
     def __init__(self, cfg: TomcruApiOIDCAuthorizerEP, auth_cfg, env=None):
@@ -55,15 +60,16 @@
                         'scopes': scopes
                     }
                 }
 
             return data
         except (jwt.InvalidTokenError, AWSOIDCException) as e:
             # invalidated claims -> authorizer refuses the token
-            print("[OIDC] JWT Authorizer error: ", str(type(e)), e)
+
+            logger.error("[OIDC] JWT Authorizer error: ", str(type(e)), e)
             return None
 
     def verify_claims(self, data: dict):
         _scope = data.get('scp', data.get('scope', None))
 
         # validate: The token must include at least one of the scopes in the route's authorizationScopes
         #self.scope, self.scopes_supported
```

### Comparing `tomcru-0.2.8/tomcru/services/aws/hosted/apigw/api_shared/integration/TomcruApiGWHttpIntegration.py` & `tomcru-0.2.9/tomcru/services/aws/hosted/apigw/api_shared/integration/TomcruApiGWHttpIntegration.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/hosted/apigw/flask_b/ApiGWFlaskBuilder.py` & `tomcru-0.2.9/tomcru/services/aws/hosted/apigw/flask_b/ApiGWFlaskBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/hosted/apigw/flask_b/controllers/EmeProxyController.py` & `tomcru-0.2.9/tomcru/services/aws/hosted/apigw/flask_b/controllers/EmeProxyController.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/hosted/apigw/flask_b/integration/LambdaIntegration.py` & `tomcru-0.2.9/tomcru/services/aws/hosted/apigw/flask_b/integration/LambdaIntegration.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/hosted/apigw/flask_b/integration/MockedIntegration.py` & `tomcru-0.2.9/tomcru/services/aws/hosted/apigw/flask_b/integration/MockedIntegration.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/hosted/apigw/flask_b/integration/SwaggerIntegration.py` & `tomcru-0.2.9/tomcru/services/aws/hosted/apigw/flask_b/integration/SwaggerIntegration.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/WsAppBuilder.py` & `tomcru-0.2.9/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/WsAppBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/_jank.py` & `tomcru-0.2.9/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/_jank.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/apps/EmeWsApp.py` & `tomcru-0.2.9/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/apps/EmeWsApp.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/LambdaIntegration.py` & `tomcru-0.2.9/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/LambdaIntegration.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/WsEnRouteCachedAuthorizer.py` & `tomcru-0.2.9/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/WsEnRouteCachedAuthorizer.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/hosted/apigw_manager_b/ApiGWMgr.py` & `tomcru-0.2.9/tomcru/services/aws/hosted/apigw_manager_b/ApiGWMgr.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/hosted/boto3_b/Boto3Builder.py` & `tomcru-0.2.9/tomcru/services/aws/hosted/boto3_b/Boto3Builder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/hosted/boto3_b/boto3.py` & `tomcru-0.2.9/tomcru/services/aws/hosted/boto3_b/boto3.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/hosted/cloudfront/flask_b/CloudfrontFlaskBuilder.py` & `tomcru-0.2.9/tomcru/services/aws/hosted/cloudfront/flask_b/CloudfrontFlaskBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/hosted/ddb/proxy.py` & `tomcru-0.2.9/tomcru/services/aws/hosted/ddb/proxy.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DDBSqlAlchemyTable.py` & `tomcru-0.2.9/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DDBSqlAlchemyTable.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DynamoDBBuilder.py` & `tomcru-0.2.9/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DynamoDBBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/hosted/ddb/sqlalchemy_b/SqlAlchemyJSONType.py` & `tomcru-0.2.9/tomcru/services/aws/hosted/ddb/sqlalchemy_b/SqlAlchemyJSONType.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/hosted/ddb/sqlalchemy_b/dal_ddb.py` & `tomcru-0.2.9/tomcru/services/aws/hosted/ddb/sqlalchemy_b/dal_ddb.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/hosted/lambda_b/LambdaBuilder.py` & `tomcru-0.2.9/tomcru/services/aws/hosted/lambda_b/LambdaBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/hosted/lambda_b/LambdaHostedPyContext.py` & `tomcru-0.2.9/tomcru/services/aws/hosted/lambda_b/LambdaHostedPyContext.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/hosted/lambda_b/proxy/Py2NodeLambdaProxy.py` & `tomcru-0.2.9/tomcru/services/aws/hosted/lambda_b/proxy/Py2NodeLambdaProxy.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,85 +1,86 @@
 import json
+import logging
 from base64 import b64encode, b64decode
 import os
 import shutil
 import signal
 import subprocess
 
 from ..LambdaHostedPyContext import LambdaHostedPyContext
 from tomcru import TomcruEnvCfg
 
 json_type = dict | list | str
+logger = logging.getLogger('tomcru')
+
 
 def ser(o: json_type) -> str:
     return b64encode(json.dumps(o).encode('utf8')).decode('utf8')
 
 def deser(s: str) -> json_type:
     return json.loads(b64decode(s.encode('utf8')))
 
 
 class Py2NodeLambdaProxy:
     """
     This class forwards AWS lambda requests from python to a node.js executable.
     """
-    def __init__(self, lambda_id: str, lambda_path: str, env: TomcruEnvCfg, pck_path, srvmgr):
+    def __init__(self, lambda_id: str, lambda_path: str, env: TomcruEnvCfg, pck_path, srvmgr, cleanup=False):
         self.lambda_id = lambda_id
         self.lambda_path = lambda_path
         self.env = env
 
         # todo: make option to provide node path in settings
         self.node_path: str | None = None
         self.is_shell = False
         self.timeout = 5
         self.srvmgr = srvmgr
         self.boto3 = None
+        self.cleanup: bool = cleanup
 
         self.proxy_path = os.path.join(pck_path, 'etc', 'proxies')
 
         # todo: verify if 'tomcru_integ' is in packages.json
 
     def init(self):
         # inject AWS sdk object to node_modules
         self.copy_proxy()
 
         if self.node_path is None:
-            print("NODE PATH:", self.node_path)
             try:
                 self.node_path = subprocess.check_output('which node', text=True, shell=True).rstrip()
                 self.is_shell = False
             except:
                 self.node_path = 'node'
                 self.is_shell = True
+        logger.debug(f"[Py2NodeLambdaProxy] NODE PATH: {self.node_path} Is shell? {self.is_shell}")
 
 
     def deject_dependencies(self):
         self.clean_proxy()
 
     def __call__(self, event: dict, context: LambdaHostedPyContext, **kwargs):
         env_dict = os.environ.copy()
         cmd = [self.node_path, 't_proxy.js', ser(event)]
         if self.is_shell:
             cmd = ' '.join(cmd)
 
-        print("calling", cmd)
+        logger.debug(f"[Py2NodeLambdaProxy] calling f{cmd}")
 
         # todo: @later: pass serialzied json as binary instead of base64 between processes
         resp = None
         with subprocess.Popen(cmd, bufsize=1, universal_newlines=True, shell=self.is_shell,
                               cwd=self.lambda_path, env=env_dict,
                               stdin=subprocess.PIPE, stdout=subprocess.PIPE) as p:
             for line in p.stdout:
-                if line.startswith('FOO'):
-                    p.stdin.write('BAR\n')
-                    continue
-
                 t_in = deser(line)
 
                 if 'serv_id' in t_in:
-                    print("  [LUAEXEC]: requesting service", t_in)
+                    logger.debug(f"[Py2NodeLambdaProxy] requesting service f{t_in}")
+
                     if 'boto3' in t_in:
                         import boto3
                         #boto3 = self.srvmgr.service(self.env, 'boto3').boto3
 
                         if t_in['boto3'] == 'resource':
                             srv = boto3.resource(t_in['serv_id'])
 
@@ -88,58 +89,54 @@
                             srv = boto3.client(t_in['serv_id'])
 
                         serv_resp = getattr(srv, t_in['method'])(**t_in['args'])
                         p.stdin.write(ser(serv_resp)+'\n')
                     else:
                         raise NotImplementedError(t_in)
                 elif 'log' in t_in:
-                    print("  [LUAEXEC.LOG]:", t_in['log'])
+                    logger.info(f"[Py2NodeLambdaProxy] log f{t_in['log']}")
                 elif 'err' in t_in:
-                    print("  [LUAEXEC.ERROR]:", t_in['err'])
+                    logger.error(f"[Py2NodeLambdaProxy] error f{t_in['err']}")
                 elif 'resp' in t_in:
                     resp = t_in['resp'].copy()
                 elif 'bye' in t_in:
-                    print("  [LUAEXEC] said GOODBYE")
+                    logger.info(f"[Py2NodeLambdaProxy] said GOODBYE")
                     p.send_signal(signal.SIGINT)
                     break
                 else:
-                    print("  [LUAEXEC] received:", line.rstrip('\n'))
+                    line = line.rstrip('\n')
+                    logger.warning(f"[Py2NodeLambdaProxy] received unknown: {line}")
 
             p.terminate()
 
         if resp:
             return resp
         else:
             raise Exception("no resp from lambda!")
 
     def copy_proxy(self):
         _aws = os.path.join(self.lambda_path, 'node_modules', 'aws-sdk')
 
         if os.path.exists(_aws):
             if os.path.exists(os.path.join(_aws, 'proxylib.js')):
-                print("RM PROXY")
                 shutil.rmtree(_aws)
             else:
-                print("BACKUP AWS")
                 # save aws sdk
                 os.rename(_aws, _aws+'_tmp')
 
         shutil.copy(os.path.join(self.proxy_path, 't_proxy.js'), self.lambda_path)
         shutil.copytree(os.path.join(self.proxy_path, 'aws-sdk'), _aws)
 
     def clean_proxy(self):
         _aws = os.path.join(self.lambda_path, 'node_modules', 'aws-sdk')
 
         if os.path.exists(_aws):
             if os.path.exists(os.path.join(_aws, 'proxylib.js')):
                 # remove AWS sdk & tomcru lambda js proxy from node_modules
-                print("DELETE", _aws)
                 shutil.rmtree(_aws)
-            else:
-                print("NOOP")
 
         try:
             os.remove(os.path.join(self.lambda_path, 't_proxy.js'))
         except:
             pass
 
         # add back aws-sdk
```

### Comparing `tomcru-0.2.8/tomcru/services/aws/hosted/s3_b/S3AdapterLocal.py` & `tomcru-0.2.9/tomcru/services/aws/hosted/s3_b/S3AdapterLocal.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+import logging
 import os.path
 import shutil
 
 from deepmerge import always_merger
 from typing.io import BinaryIO
+logger = logging.getLogger('tomcru')
 
 
 class S3AdapterLocal:
 
     def __init__(self, app_path, cfg, opts):
         """
         Boto3 resource adapter for S3
@@ -15,15 +17,15 @@
         self.buckets = always_merger.merge(cfg.get('buckets'), opts.get('buckets'))
 
         for bucket, bucket_cfg in self.buckets.items():
             path = bucket_cfg.get('path', os.path.join(_default_bucket_path, bucket))
             bucket_cfg['path'] = os.path.join(app_path, path)
 
             if not os.path.exists(bucket_cfg['path']):
-                print("S3AdapterLocal: creating bucket directory:", bucket_cfg['path'])
+                logger.debug(f"S3AdapterLocal: creating bucket directory: {bucket_cfg['path']}")
                 os.makedirs(bucket_cfg['path'])
 
     def _get_path(self, Bucket, Key):
         return os.path.join(self.buckets[Bucket]['path'], Key)
 
     def upload_file(self, Filename, Bucket, Key):
         # with open(Filename, 'b') as fh:
```

### Comparing `tomcru-0.2.8/tomcru/services/aws/hosted/s3_b/S3Service.py` & `tomcru-0.2.9/tomcru/services/aws/hosted/s3_b/S3Service.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/onpremise/model_checker/SwaggerResponseModelValidator.py` & `tomcru-0.2.9/tomcru/services/aws/onpremise/model_checker/SwaggerResponseModelValidator.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
             # ignore all swagger endpoints, no need to validate
             return
 
         content_type = response.headers['content-type']
         _paths = api.spec_resolved_schemas['paths']
 
         if ep.route not in _paths:
-            self.log_warning("Not in paths")
+            logger.warning(f"[{self.__class__.__name__}] Not in paths")
 
         ep_model = _paths[ep.route][ep.method.lower()]
 
         req_model = ep_model['parameters']
         self._validate_request(request, req_model)
 
         resp_model = ep_model['responses'].get(str(response.status_code), 'default')
@@ -99,10 +99,7 @@
                 'properties': {
                     'id': {'type': 'integer', 'format': 'int64'},
                     'name': {'type': 'string'},
                     'tag': {'type': 'string'}
                 }
             }
         }
-
-    def log_warning(self, err):
-        print(err)
```

### Comparing `tomcru-0.2.8/tomcru/services/aws/onpremise/s3_static/S3StaticBuilder.py` & `tomcru-0.2.9/tomcru/services/aws/onpremise/s3_static/S3StaticBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/sam/_junk/SamTplBuilder.py` & `tomcru-0.2.9/tomcru/services/aws/sam/_junk/SamTplBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/sam/_junk/core.yaml` & `tomcru-0.2.9/tomcru/services/aws/sam/_junk/core.yaml`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/sam/_junk/httpapi.yaml` & `tomcru-0.2.9/tomcru/services/aws/sam/_junk/httpapi.yaml`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/sam/_junk/integ_ws.yaml` & `tomcru-0.2.9/tomcru/services/aws/sam/_junk/integ_ws.yaml`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/sam/_junk/template.yaml` & `tomcru-0.2.9/tomcru/services/aws/sam/_junk/template.yaml`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/sam/_junk/wsapi.yaml` & `tomcru-0.2.9/tomcru/services/aws/sam/_junk/wsapi.yaml`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/sam/lambda_b/LambdaBuilder.py` & `tomcru-0.2.9/tomcru/services/aws/sam/lambda_b/LambdaBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/sam/params_b/ParametersBuilder.py` & `tomcru-0.2.9/tomcru/services/aws/sam/params_b/ParametersBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/sam/spec_api_b/SwaggerApiTemplater.py` & `tomcru-0.2.9/tomcru/services/aws/sam/spec_api_b/SwaggerApiTemplater.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/sam/spec_api_b/authorizers/SAMLambdaAuthBuilder.py` & `tomcru-0.2.9/tomcru/services/aws/sam/spec_api_b/authorizers/SAMLambdaAuthBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/sam/spec_api_b/authorizers/SAMOIDCAuthBuilder.py` & `tomcru-0.2.9/tomcru/services/aws/sam/spec_api_b/authorizers/SAMOIDCAuthBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/aws/sam/spec_api_b/integrations/SAMLambdaBuilder.py` & `tomcru-0.2.9/tomcru/services/aws/sam/spec_api_b/integrations/SAMLambdaBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/tomcru/services/general/eme2swagger/Eme2Swagger.py` & `tomcru-0.2.9/tomcru/services/general/eme2swagger/Eme2Swagger.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.2.8/PKG-INFO` & `tomcru-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomcru
-Version: 0.2.8
+Version: 0.2.9
 Summary: Serverless app framework
 Author: Rajmund Csombordi
 Author-email: rajmund.csombordi@hotmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -15,13 +15,13 @@
 Requires-Dist: flatten-json (>=0.1.13,<0.2.0)
 Requires-Dist: openapi-spec-validator (>=0.5,<1.0)
 Requires-Dist: prance (>=0.22,<1.0)
 Requires-Dist: pyjwt (>=2.6,<3.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28,<3.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
-Requires-Dist: tomcru-jerry (>=0.1.2,<0.2.0)
+Requires-Dist: tomcru-jerry (>=0.1.3,<0.2.0)
 Description-Content-Type: text/markdown
 
 # tomcru
 Py &amp; node.js application framework that can target multiple architectures (microservices, FaaS, monolithic) over multiple vendors (AWS, Azure, on premise, single server)
```

