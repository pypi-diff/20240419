# Comparing `tmp/nonebot-plugin-hx-yinying-0.0.6.tar.gz` & `tmp/nonebot-plugin-hx-yinying-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-hx-yinying-0.0.6.tar", last modified: Thu Apr 18 08:18:04 2024, max compression
+gzip compressed data, was "nonebot-plugin-hx-yinying-0.0.7.tar", last modified: Fri Apr 19 20:07:33 2024, max compression
```

## Comparing `nonebot-plugin-hx-yinying-0.0.6.tar` & `nonebot-plugin-hx-yinying-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 08:18:04.192583 nonebot-plugin-hx-yinying-0.0.6/
--rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     3519 2024-04-18 08:18:04.194585 nonebot-plugin-hx-yinying-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3079 2024-04-18 08:16:30.000000 nonebot-plugin-hx-yinying-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 08:18:04.084598 nonebot-plugin-hx-yinying-0.0.6/nonebot_plugin_hx_yinying/
--rw-rw-rw-   0        0        0     1288 2024-04-17 18:38:10.000000 nonebot-plugin-hx-yinying-0.0.6/nonebot_plugin_hx_yinying/__init__.py
--rw-rw-rw-   0        0        0    11708 2024-04-18 08:10:50.000000 nonebot-plugin-hx-yinying-0.0.6/nonebot_plugin_hx_yinying/chat.py
--rw-rw-rw-   0        0        0      749 2024-04-18 04:08:44.000000 nonebot-plugin-hx-yinying-0.0.6/nonebot_plugin_hx_yinying/config.py
-drwxrwxrwx   0        0        0        0 2024-04-18 08:18:04.187191 nonebot-plugin-hx-yinying-0.0.6/nonebot_plugin_hx_yinying.egg-info/
--rw-rw-rw-   0        0        0     3519 2024-04-18 08:18:03.000000 nonebot-plugin-hx-yinying-0.0.6/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2024-04-18 08:18:03.000000 nonebot-plugin-hx-yinying-0.0.6/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 08:18:03.000000 nonebot-plugin-hx-yinying-0.0.6/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      124 2024-04-18 08:18:03.000000 nonebot-plugin-hx-yinying-0.0.6/nonebot_plugin_hx_yinying.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-18 08:18:03.000000 nonebot-plugin-hx-yinying-0.0.6/nonebot_plugin_hx_yinying.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-04-18 08:18:04.196738 nonebot-plugin-hx-yinying-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      840 2024-04-18 08:16:42.000000 nonebot-plugin-hx-yinying-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 20:07:33.716940 nonebot-plugin-hx-yinying-0.0.7/
+-rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     3889 2024-04-19 20:07:33.716940 nonebot-plugin-hx-yinying-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3449 2024-04-19 20:07:15.000000 nonebot-plugin-hx-yinying-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 20:07:33.585275 nonebot-plugin-hx-yinying-0.0.7/nonebot_plugin_hx_yinying/
+-rw-rw-rw-   0        0        0     1968 2024-04-19 20:05:40.000000 nonebot-plugin-hx-yinying-0.0.7/nonebot_plugin_hx_yinying/__init__.py
+-rw-rw-rw-   0        0        0    13088 2024-04-19 20:01:47.000000 nonebot-plugin-hx-yinying-0.0.7/nonebot_plugin_hx_yinying/chat.py
+-rw-rw-rw-   0        0        0      749 2024-04-18 04:08:44.000000 nonebot-plugin-hx-yinying-0.0.7/nonebot_plugin_hx_yinying/config.py
+drwxrwxrwx   0        0        0        0 2024-04-19 20:07:33.716940 nonebot-plugin-hx-yinying-0.0.7/nonebot_plugin_hx_yinying.egg-info/
+-rw-rw-rw-   0        0        0     3889 2024-04-19 20:07:33.000000 nonebot-plugin-hx-yinying-0.0.7/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2024-04-19 20:07:33.000000 nonebot-plugin-hx-yinying-0.0.7/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 20:07:33.000000 nonebot-plugin-hx-yinying-0.0.7/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      124 2024-04-19 20:07:33.000000 nonebot-plugin-hx-yinying-0.0.7/nonebot_plugin_hx_yinying.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-19 20:07:33.000000 nonebot-plugin-hx-yinying-0.0.7/nonebot_plugin_hx_yinying.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-04-19 20:07:33.740244 nonebot-plugin-hx-yinying-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      840 2024-04-19 20:07:25.000000 nonebot-plugin-hx-yinying-0.0.7/setup.py
```

### Comparing `nonebot-plugin-hx-yinying-0.0.6/LICENSE` & `nonebot-plugin-hx-yinying-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-0.0.6/PKG-INFO` & `nonebot-plugin-hx-yinying-0.0.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,16 @@
-Metadata-Version: 2.1
-Name: nonebot-plugin-hx-yinying
-Version: 0.0.6
-Summary: chat with yinying
-Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
-Author: Huan Xin
-Author-email: mc.xiaolang@foxmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <!--
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
  * @Author         : huanxin996
  * @Date           : 2024-4-17
  * @LastEditors    : huanxin996
- * @LastEditTime   : 2024-4-18
+ * @LastEditTime   : 2024-4-19
  * @Description    : None
  * @GitHub         : https://github.com/huanxin996
 -->
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
 
 <p align="center">
@@ -39,15 +26,15 @@
 </div>
 
 <p align="center">
   <a href="https://raw.githubusercontent.com/cscs181/QQ-Github-Bot/master/LICENSE">
     <img src="https://img.shields.io/github/license/cscs181/QQ-Github-Bot.svg" alt="license">
   </a>
   <a href="https://pypi.python.org/pypi/nonebot-plugin-hx-yinying">
-    <img src="https://img.shields.io/pypi/v/nonebot-plugin-status.svg" alt="pypi">
+    <img src="https://skin.huanxinbot.com/api/pypi.svg" alt="pypi">
   </a>
   <img src="https://img.shields.io/badge/python-3.10+-blue.svg" alt="python">
 </p>
 
 ## 使用方式
 
 通用:
@@ -58,15 +45,21 @@
 
 - @Bot
 - 回复Bot
 
 ## 配置项
 
 > [!WARNING]
-> GitHub 仓库中的文档为最新 DEV 版本，配置方式请参考 [PyPI](https://pypi.org/project/nonebot-plugin-status/) 上的文档。
+> GitHub 仓库中的文档为最新 DEV 版本，配置方式请参考 [PyPI](https://pypi.python.org/pypi/nonebot-plugin-hx-yinying) 上的文档。
+
+> [!WARNING]
+> 秩乱(乱乱)的联系方式如下，QQ:1660466270，官方qq群聊:175334224 [官网链接](https://chat.wingmark.cn/) .
+
+> [!WARNING]
+> 请注意，该项目是接入了乱乱的项目，你需要遵守api使用的 [规范](https://wingmark.feishu.cn/docx/NFgJddgQAotygKxXiu6cpyg5nqr)。
 
 配置方式：直接在 NoneBot 全局配置文件中添加以下配置项即可。
 
 ### yinying_appid
 
 - 类型：`str`
 - 默认值：`None`
@@ -89,14 +82,15 @@
 - 重要：必填
 
 ### yinying_model
 
 - 类型：`str`
 - 默认值：`None`
 - 说明：选择使用银影的模型
+- 注意 该配置项即将移除（转为插件内配置！）
 
 ## hx_path
 - 类型：`str`
 - 默认值：`None`
 - 说明：银影对话的用户数据存储路径(不写将使用默认配置)
 
 ## hx_reply
```

#### html2text {}

```diff
@@ -1,33 +1,33 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 0.0.6 Summary:
-chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
-yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Description-Content-
-Type: text/markdown License-File: LICENSE [![All Contributors](https://
-img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
-(#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
-huanxin996 * @LastEditTime : 2024-4-18 * @Description : None * @GitHub : https:
-//github.com/huanxin996 -->
+[![All Contributors](https://img.shields.io/badge/all_contributors-2-
+orange.svg?style=flat-square)](#contributors-) * @Author : huanxin996 * @Date :
+2024-4-17 * @LastEditors : huanxin996 * @LastEditTime : 2024-4-19 *
+@Description : None * @GitHub : https://github.com/huanxin996 -->
                                    _[_n_o_n_e_b_o_t_]
                 # nonebot_plugin_hx-yinying _â¨ Hx vs YinYing
                   (å¨çº¿ä¸é¶å½±è¿è¡å¯¹è¯çæä»¶) â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## ä½¿ç¨æ¹å¼ éç¨: - @Bot æèåå¤å³å¯ OneBot: - @Bot - åå¤Bot ##
 éç½®é¡¹ > [!WARNING] > GitHub ä»åºä¸­çææ¡£ä¸ºææ° DEV
-çæ¬ï¼éç½®æ¹å¼è¯·åè [PyPI](https://pypi.org/project/nonebot-plugin-
-status/) ä¸çææ¡£ã éç½®æ¹å¼ï¼ç´æ¥å¨ NoneBot
+çæ¬ï¼éç½®æ¹å¼è¯·åè [PyPI](https://pypi.python.org/pypi/nonebot-
+plugin-hx-yinying) ä¸çææ¡£ã > [!WARNING] > ç§©ä¹±
+(ä¹±ä¹±)çèç³»æ¹å¼å¦ä¸ï¼QQ:1660466270ï¼å®æ¹qqç¾¤è:175334224
+[å®ç½é¾æ¥](https://chat.wingmark.cn/) . > [!WARNING] >
+è¯·æ³¨æï¼è¯¥é¡¹ç®æ¯æ¥å¥äºä¹±ä¹±çé¡¹ç®ï¼ä½ éè¦éµå®apiä½¿ç¨ç
+[è§è](https://wingmark.feishu.cn/docx/NFgJddgQAotygKxXiu6cpyg5nqr)ã
+éç½®æ¹å¼ï¼ç´æ¥å¨ NoneBot
 å¨å±éç½®æä»¶ä¸­æ·»å ä»¥ä¸éç½®é¡¹å³å¯ã ### yinying_appid -
 ç±»åï¼`str` - é»è®¤å¼ï¼`None` - è¯´æï¼ä½ çappid - éè¦ï¼å¿å¡«
 ### yinying_token - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
 è¯´æï¼è¿éåä½ æ¾ç§©ä¹±è·åå°çapi_key - éè¦ï¼å¿å¡« ###
 hx_api_yinying - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
 è¯´æï¼yinyingçapiå°å - éè¦ï¼å¿å¡« ### yinying_model -
-ç±»åï¼`str` - é»è®¤å¼ï¼`None` - è¯´æï¼éæ©ä½¿ç¨é¶å½±çæ¨¡å ##
-hx_path - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
+ç±»åï¼`str` - é»è®¤å¼ï¼`None` - è¯´æï¼éæ©ä½¿ç¨é¶å½±çæ¨¡å -
+æ³¨æ è¯¥éç½®é¡¹å³å°ç§»é¤ï¼è½¬ä¸ºæä»¶åéç½®ï¼ï¼ ## hx_path -
+ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
 è¯´æï¼é¶å½±å¯¹è¯çç¨æ·æ°æ®å­å¨è·¯å¾(ä¸åå°ä½¿ç¨é»è®¤éç½®)
 ## hx_reply - ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
 è¯´æï¼botåéchatæ¶æ¯æ¶æ¯å¦åå¤ -
 æ³¨æï¼è¯¥é¡¹å¯ç¨æ¶hx_reply_atå°è¢«å¿½ç¥ ## hx_reply_at -
 ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
 è¯´æï¼botåéchatæ¶æ¯æ¶ä¸åå¤æ¶æ¯å¦è¾ç¹ ## yinying_limit -
 ç±»åï¼`int` - é»è®¤å¼ï¼`12` - è¯´æï¼å¯¹äºé¶å½±å¯¹è¯éå¶çæ¬¡æ°
```

### Comparing `nonebot-plugin-hx-yinying-0.0.6/README.md` & `nonebot-plugin-hx-yinying-0.0.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,29 @@
+Metadata-Version: 2.1
+Name: nonebot-plugin-hx-yinying
+Version: 0.0.7
+Summary: chat with yinying
+Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
+Author: Huan Xin
+Author-email: mc.xiaolang@foxmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <!--
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
  * @Author         : huanxin996
  * @Date           : 2024-4-17
  * @LastEditors    : huanxin996
- * @LastEditTime   : 2024-4-18
+ * @LastEditTime   : 2024-4-19
  * @Description    : None
  * @GitHub         : https://github.com/huanxin996
 -->
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
 
 <p align="center">
@@ -26,15 +39,15 @@
 </div>
 
 <p align="center">
   <a href="https://raw.githubusercontent.com/cscs181/QQ-Github-Bot/master/LICENSE">
     <img src="https://img.shields.io/github/license/cscs181/QQ-Github-Bot.svg" alt="license">
   </a>
   <a href="https://pypi.python.org/pypi/nonebot-plugin-hx-yinying">
-    <img src="https://img.shields.io/pypi/v/nonebot-plugin-status.svg" alt="pypi">
+    <img src="https://skin.huanxinbot.com/api/pypi.svg" alt="pypi">
   </a>
   <img src="https://img.shields.io/badge/python-3.10+-blue.svg" alt="python">
 </p>
 
 ## 使用方式
 
 通用:
@@ -45,15 +58,21 @@
 
 - @Bot
 - 回复Bot
 
 ## 配置项
 
 > [!WARNING]
-> GitHub 仓库中的文档为最新 DEV 版本，配置方式请参考 [PyPI](https://pypi.org/project/nonebot-plugin-status/) 上的文档。
+> GitHub 仓库中的文档为最新 DEV 版本，配置方式请参考 [PyPI](https://pypi.python.org/pypi/nonebot-plugin-hx-yinying) 上的文档。
+
+> [!WARNING]
+> 秩乱(乱乱)的联系方式如下，QQ:1660466270，官方qq群聊:175334224 [官网链接](https://chat.wingmark.cn/) .
+
+> [!WARNING]
+> 请注意，该项目是接入了乱乱的项目，你需要遵守api使用的 [规范](https://wingmark.feishu.cn/docx/NFgJddgQAotygKxXiu6cpyg5nqr)。
 
 配置方式：直接在 NoneBot 全局配置文件中添加以下配置项即可。
 
 ### yinying_appid
 
 - 类型：`str`
 - 默认值：`None`
@@ -76,14 +95,15 @@
 - 重要：必填
 
 ### yinying_model
 
 - 类型：`str`
 - 默认值：`None`
 - 说明：选择使用银影的模型
+- 注意 该配置项即将移除（转为插件内配置！）
 
 ## hx_path
 - 类型：`str`
 - 默认值：`None`
 - 说明：银影对话的用户数据存储路径(不写将使用默认配置)
 
 ## hx_reply
```

#### html2text {}

```diff
@@ -1,27 +1,39 @@
-[![All Contributors](https://img.shields.io/badge/all_contributors-2-
-orange.svg?style=flat-square)](#contributors-) * @Author : huanxin996 * @Date :
-2024-4-17 * @LastEditors : huanxin996 * @LastEditTime : 2024-4-18 *
-@Description : None * @GitHub : https://github.com/huanxin996 -->
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 0.0.7 Summary:
+chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
+yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Description-Content-
+Type: text/markdown License-File: LICENSE [![All Contributors](https://
+img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
+(#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
+huanxin996 * @LastEditTime : 2024-4-19 * @Description : None * @GitHub : https:
+//github.com/huanxin996 -->
                                    _[_n_o_n_e_b_o_t_]
                 # nonebot_plugin_hx-yinying _â¨ Hx vs YinYing
                   (å¨çº¿ä¸é¶å½±è¿è¡å¯¹è¯çæä»¶) â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## ä½¿ç¨æ¹å¼ éç¨: - @Bot æèåå¤å³å¯ OneBot: - @Bot - åå¤Bot ##
 éç½®é¡¹ > [!WARNING] > GitHub ä»åºä¸­çææ¡£ä¸ºææ° DEV
-çæ¬ï¼éç½®æ¹å¼è¯·åè [PyPI](https://pypi.org/project/nonebot-plugin-
-status/) ä¸çææ¡£ã éç½®æ¹å¼ï¼ç´æ¥å¨ NoneBot
+çæ¬ï¼éç½®æ¹å¼è¯·åè [PyPI](https://pypi.python.org/pypi/nonebot-
+plugin-hx-yinying) ä¸çææ¡£ã > [!WARNING] > ç§©ä¹±
+(ä¹±ä¹±)çèç³»æ¹å¼å¦ä¸ï¼QQ:1660466270ï¼å®æ¹qqç¾¤è:175334224
+[å®ç½é¾æ¥](https://chat.wingmark.cn/) . > [!WARNING] >
+è¯·æ³¨æï¼è¯¥é¡¹ç®æ¯æ¥å¥äºä¹±ä¹±çé¡¹ç®ï¼ä½ éè¦éµå®apiä½¿ç¨ç
+[è§è](https://wingmark.feishu.cn/docx/NFgJddgQAotygKxXiu6cpyg5nqr)ã
+éç½®æ¹å¼ï¼ç´æ¥å¨ NoneBot
 å¨å±éç½®æä»¶ä¸­æ·»å ä»¥ä¸éç½®é¡¹å³å¯ã ### yinying_appid -
 ç±»åï¼`str` - é»è®¤å¼ï¼`None` - è¯´æï¼ä½ çappid - éè¦ï¼å¿å¡«
 ### yinying_token - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
 è¯´æï¼è¿éåä½ æ¾ç§©ä¹±è·åå°çapi_key - éè¦ï¼å¿å¡« ###
 hx_api_yinying - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
 è¯´æï¼yinyingçapiå°å - éè¦ï¼å¿å¡« ### yinying_model -
-ç±»åï¼`str` - é»è®¤å¼ï¼`None` - è¯´æï¼éæ©ä½¿ç¨é¶å½±çæ¨¡å ##
-hx_path - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
+ç±»åï¼`str` - é»è®¤å¼ï¼`None` - è¯´æï¼éæ©ä½¿ç¨é¶å½±çæ¨¡å -
+æ³¨æ è¯¥éç½®é¡¹å³å°ç§»é¤ï¼è½¬ä¸ºæä»¶åéç½®ï¼ï¼ ## hx_path -
+ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
 è¯´æï¼é¶å½±å¯¹è¯çç¨æ·æ°æ®å­å¨è·¯å¾(ä¸åå°ä½¿ç¨é»è®¤éç½®)
 ## hx_reply - ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
 è¯´æï¼botåéchatæ¶æ¯æ¶æ¯å¦åå¤ -
 æ³¨æï¼è¯¥é¡¹å¯ç¨æ¶hx_reply_atå°è¢«å¿½ç¥ ## hx_reply_at -
 ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
 è¯´æï¼botåéchatæ¶æ¯æ¶ä¸åå¤æ¶æ¯å¦è¾ç¹ ## yinying_limit -
 ç±»åï¼`int` - é»è®¤å¼ï¼`12` - è¯´æï¼å¯¹äºé¶å½±å¯¹è¯éå¶çæ¬¡æ°
```

### Comparing `nonebot-plugin-hx-yinying-0.0.6/nonebot_plugin_hx_yinying/chat.py` & `nonebot-plugin-hx-yinying-0.0.7/nonebot_plugin_hx_yinying/chat.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,82 +19,109 @@
     log_dir.mkdir(parents=True, exist_ok=True)
 else:
     logger.success("找到配置里的路径，载入成功")
     history_dir = store.get_data_dir(f"{hx_config.hx_path}")
     log_dir = Path(f"{history_dir}\yinying_chat").absolute()
     log_dir.mkdir(parents=True, exist_ok=True)
 
+#初始化log记录
+def log_in()-> str:
+    if os.path.exists(f"{log_dir}/chat/all_log.json"):
+        with open(f'{log_dir}/chat/all_log.json','r',encoding='utf-8') as file:
+            json_data = json.load(file)
+            return json_data
+    else:
+        with open(f'{log_dir}/chat/all_log.json','w',encoding='utf-8') as file:
+            json_data = {}
+            package = {}
+            history_package = []
+            package['rule'] = '幻歆'
+            package['msg'] = '初始化log记录'
+            history_package.append(package)
+            json_data['114514'] = history_package
+            json.dump(json_data,file)
+            return json_data
 
 #创建用户文件夹
 def create_dir_usr(path):
     if not os.path.exists(path):
         os.mkdir(path)
 
 #用户输入
 def user_in(id, text):
-    if os.path.exists(f"{log_dir}\chat\{id}\content.json"):
-        with open(f"{log_dir}\chat\{id}\content.json",'a',encoding='utf-8') as file:
-            file.write(',\n{"role": "user", "content": "' + text + '"}')
-    else:
-        create_dir_usr(f"{log_dir}\chat\{id}")
-        with open(f"{log_dir}\chat\{id}\content.json",'w',encoding='utf-8') as file:
-            file.write('{"role": "user", "content": "' + text + '"}')
+    data = log_in()
+    if f'{id}' in data: 
+        id_log = data[f'{id}']['log']
+        package = {}
+        package['rule'] = 'user'
+        package['msg'] = f'{text}'
+        id_log.append(package)
+        data[f'{id}']['log'] = id_log
+        with open(f'{log_dir}/chat/all_log.json','w',encoding='utf-8') as file:
+            json.dump(data,file)
+    else : 
+        package = {}
+        log = {}
+        history_package = []
+        package['rule'] = 'user'
+        package['msg'] = f'{text}'
+        history_package.append(package)
+        log['log'] = history_package
+        dt = time.time()
+        t = int(dt)
+        log['time'] = t
+        data[f'{id}'] = log
+        with open(f'{log_dir}/chat/all_log.json','w',encoding='utf-8') as file:
+            json.dump(data,file)
 
 #AI输出
 def ai_out(id, text):
-    if os.path.exists(f"{log_dir}\chat\{id}\content.json"):
-        with open(f'{log_dir}\chat\{id}\content.json','a',encoding='utf-8') as file:
-            file.write(',\n{"role": "assistant", "content": "' + text + '"}')
+    data = log_in()
+    if f'{id}' in data: 
+        id_log = data[f'{id}']['log']
+        package = {}
+        package['rule'] = 'ai'
+        package['msg'] = f'{text}'
+        id_log.append(package)
+        data[f'{id}']['log'] = id_log
+        with open(f'{log_dir}/chat/all_log.json','w',encoding='utf-8') as file:
+            json.dump(data,file)
+    else : 
+        package = {}
+        log = {}
+        history_package = []
+        package['rule'] = 'ai'
+        package['msg'] = f'{text}'
+        history_package.append(package)
+        log['log'] = history_package
+        dt = time.time()
+        t = int(dt)
+        log['time'] = t
+        data[f'{id}'] = log
+        with open(f'{log_dir}/chat/all_log.json','w',encoding='utf-8') as file:
+            json.dump(data,file)
+
+#检测对话次数
+def chat_times(id) -> str:
+    data = log_in()
+    history = data[f"{id}"]['log']
+    times = len(history)/2 +0.5
+    if times >= hx_config.yinying_limit:
+        dt = time.time()
+        t = int(dt)
+        data[f'{id}']['time'] = t
+        data[f"{id}"]['log'] = []
+        with open(f'{log_dir}/chat/all_log.json','w',encoding='utf-8') as file:
+            json.dump(data,file)
+            return 0
     else:
-        create_dir_usr(f"{log_dir}\chat\{id}")
-        with open(f'{log_dir}\chat\{id}\content.json','w',encoding='utf-8') as file:
-            file.write('{"role": "assistant", "content": "' + text + '"}')
-
-#存储对话次数
-def chat_times(id):
-    if os.path.exists(f'{log_dir}/chat/{id}/times.json'):
-        with open(f"{log_dir}/chat/{id}/times.json",'a',encoding='utf-8') as file:
-                with open(f'{log_dir}/chat/{id}/times.json','r',encoding='utf-8') as file:
-                    data = json.load(file)
-                    data["times"] = data["times"] + 1
-                    data.update(file)
-                with open(f'{log_dir}/chat/{id}/times.json','w',encoding='utf-8') as file:
-                    json.dump(data, file)
-    else:
-        create_dir_usr(f"{log_dir}\chat\{id}")
-        with open(f'{log_dir}/chat/{id}/times.json','w',encoding='utf-8') as file:
-                with open(f'{log_dir}/chat/{id}/times.json','w',encoding='utf-8') as file:
-                    old_data = {}
-                    dt = time.time()
-                    t = int(dt)
-                    data = {"times":0,"time":t,"character":"是一只猫猫龙哦"}
-                    old_data.update(data)
-                with open(f'{log_dir}/chat/{id}/times.json','w',encoding='utf-8') as file:
-                    json.dump(data, file)
-                    return 0
-
+        return times
 
-
-#清楚对话id
-def chat_clear(id):
-    with open(f"{log_dir}/chat/{id}/times.json",'a',encoding='utf-8') as file:
-        with open(f'{log_dir}/chat/{id}/times.json','r',encoding='utf-8') as file:
-            data = json.load(file)
-            dt = time.time()
-            t = int(dt)
-            data["times"] = 0
-            data["time"] = t
-            data.update(file)
-        with open(f'{log_dir}/chat/{id}/times.json','w',encoding='utf-8') as file:
-            json.dump(data, file)
-            return True
-     
-
-
-async def gen_chat_text(event: MessageEvent, bot: Bot) -> str:
+#获取纯文本
+async def gen_chat_text(event, bot: Bot) -> str:
     msg = ""
     for seg in event.message:
         if seg.is_text():
             msg += seg.data.get("text", "")
 
         elif seg.type == "at":
             qq = seg.data.get("qq", None)
@@ -111,36 +138,51 @@
                     user_name = user_info.get("card", None) or user_info.get(
                         "nickname", None
                     )
                     if user_name:
                         msg
     return msg
 
+#手动刷新对话
+def clear_id(id) -> str:
+    data = log_in()
+    dt = time.time()
+    t = int(dt)
+    data[f'{id}']['time'] = t
+    data[f'{id}']['log'] = []
+    try:
+        with open(f'{log_dir}/chat/all_log.json','w',encoding='utf-8') as file:
+            json.dump(data,file)
+            zt = True
+    except Exception as e:
+            zt = False
+    return zt
 
-def get_id(event: MessageEvent) -> str:
+#获取用户id
+def get_id(event) -> str:
     """获取会话id"""
     if isinstance(event, GroupMessageEvent):
             id = f"{event.user_id}"
     else:
         id = f"{event.user_id}"
     return id
 
-async def get_nick(bot:Bot,event: MessageEvent) -> str:
+#获取用户昵称
+async def get_nick(bot,event) -> str:
     """获取昵称"""
     qq = event.user_id
     info = await bot.get_stranger_info(user_id=int(qq))
     nick = info["nickname"]
     if nick is None:
         nick = None
     else:
         nick = nick
     return nick
 
-
-
+#初始化传参（整理data）
 def data_in(id,text,nick) -> str:
     """构建data"""
     with open(f'{log_dir}/chat/{id}/times.json','r',encoding='utf-8') as user,\
          open(f'{log_dir}/global.json','w',encoding='utf-8') as globa:
         data = {}
         packages_data = json.loads(json.dumps(data))
         allvariables = {}
@@ -208,68 +250,84 @@
                 packages_data['variables'] = allvariables
                 packages_data['message'] = f'{text}'
         except Exception as e:
                 logger.error("严重错误，构建data失败！")
                 json_data = False
         return packages_data
 
-            
-
-
-
-
-async def send_msg(matcher: Matcher, event: MessageEvent, content):
+#全局发送消息函数，发送消息直接await就行
+async def send_msg(matcher, event, content):
     if hx_config.hx_reply == True:
         await matcher.send(MessageSegment.reply(event.message_id) + content)
     else:
         await matcher.send(content, at_sender=hx_config.hx_reply_at)
 
+#主要构建
 async def yinying(id,text,nick):
-    chat_times(id)
-    with open(f'{log_dir}/chat/{id}/times.json','r',encoding='utf-8') as file:
-        data = json.load(file)
-        times_yinying = data["times"]
-        headers = {
+    headers = {
         'Content-type': 'application/json',
         'Authorization': f'Bearer {hx_config.yinying_token}'
     }
-        osu = data_in(id,text,nick)
-        async with httpx.AsyncClient(timeout=httpx.Timeout(connect=10, read=60, write=20, pool=30)) as client:
-                back = await client.post(hx_config.hx_api_yinying, headers=headers, json=osu)
-        try:
-                back = back.json()
-        except json.decoder.JSONDecodeError as e:
-                back_msg = f"json解析报错！\n返回结果：{e}"
-                return back_msg
-        try:
-            if times_yinying>=hx_config.yinying_limit:
-                msg = back['choices'][0]['message']['content']
-                back_msg = f"[对话次数达到上限，即将清空缓存.]\n{msg}"
-                user_in(id,text)
-                ai_out(id,msg)
-                chat_clear(id)
-            else:
-                msg = back['choices'][0]['message']['content']
-                back_msg = f"[{times_yinying}|{hx_config.yinying_limit}]\n{msg}"
-                user_in(id,text)
-                ai_out(id,msg)
-        except Exception as e:
-                back_msg = f"{back} \n\n\n{osu}"
-        return back_msg
-    
+    osu = data_in(id,text,nick)
+    async with httpx.AsyncClient(timeout=httpx.Timeout(connect=10, read=60, write=20, pool=30)) as client:
+            back = await client.post(hx_config.hx_api_yinying, headers=headers, json=osu)
+    try:
+            back = back.json()
+    except json.decoder.JSONDecodeError as e:
+            back_msg = f"json解析报错！\n返回结果：{e}"
+            return back_msg
+    try:
+        times = chat_times(id)
+        if times >= hx_config.yinying_limit or times == 0:
+            msg = back['choices'][0]['message']['content']
+            text0 = msg.replace("\n","\\n")
+            text1 = text0.replace("'","\\'")
+            text = text1.replace('"','')
+            ai_out(id,text)
+            back_msg = f"{msg}\n[对话次数达到上限，即将清空缓存.]"
+        else:
+            msg = back['choices'][0]['message']['content']
+            text0 = msg.replace("\n","\\n")
+            text1 = text0.replace("'","\\'")
+            text = text1.replace('"','')
+            ai_out(id,text)
+            back_msg = f"{msg}\n[{times}|{hx_config.yinying_limit}]"
+    except Exception as e:
+            back_msg = f"{back} \n\n\n{osu}\n\n\n未知错误，错误定位于#主要构建函数。"
+    return back_msg
 
-
-async def get_answer(matcher: Matcher, event: MessageEvent, bot: Bot):
+#获取回复（被艾特）
+async def get_answer_at(matcher, event, bot):
     text = unescape(await gen_chat_text(event, bot))
-    id = get_id(event)
-    nick = await get_nick(bot,event)
     if  text == "" or text is None or text == "/hx" or text == "/chat":
         msg = "诶唔，你叫我是有什么事嘛？"
         await send_msg(matcher,event,msg)
     else:
         try:
+            id = get_id(event)
+            nick = await get_nick(bot,event)
+            user_in(id,text)
+            back_msg = str(await yinying(id,text,nick))
+            msg = back_msg.replace("\\n","\n")
+            await send_msg(matcher,event,msg)
+        except httpx.HTTPError as e:
+            back_msg = f"请求接口报错！\n返回结果：{e}"
+            await send_msg(matcher, event, back_msg)
+
+#获取回复（指令触发）
+async def get_answer_ml(matcher, event ,bot ,msg):
+    text = msg.extract_plain_text()
+    if not text == "" or text == None:
+        try:
+            id = get_id(event)
+            nick = await get_nick(bot,event)
+            user_in(id,text)
             back_msg = str(await yinying(id,text,nick))
             msg = back_msg.replace("\\n","\n")
             await send_msg(matcher,event,msg)
         except httpx.HTTPError as e:
             back_msg = f"请求接口报错！\n返回结果：{e}"
-            await send_msg(matcher, back_msg)
+            await send_msg(matcher, event, back_msg)
+    else:
+        msg = "诶唔，你叫我是有什么事嘛？"
+        await send_msg(matcher,event,msg)
+
```

### Comparing `nonebot-plugin-hx-yinying-0.0.6/nonebot_plugin_hx_yinying/config.py` & `nonebot-plugin-hx-yinying-0.0.7/nonebot_plugin_hx_yinying/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-0.0.6/nonebot_plugin_hx_yinying.egg-info/PKG-INFO` & `nonebot-plugin-hx-yinying-0.0.7/nonebot_plugin_hx_yinying.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 0.0.6
+Version: 0.0.7
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
  * @Author         : huanxin996
  * @Date           : 2024-4-17
  * @LastEditors    : huanxin996
- * @LastEditTime   : 2024-4-18
+ * @LastEditTime   : 2024-4-19
  * @Description    : None
  * @GitHub         : https://github.com/huanxin996
 -->
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
 
 <p align="center">
@@ -39,15 +39,15 @@
 </div>
 
 <p align="center">
   <a href="https://raw.githubusercontent.com/cscs181/QQ-Github-Bot/master/LICENSE">
     <img src="https://img.shields.io/github/license/cscs181/QQ-Github-Bot.svg" alt="license">
   </a>
   <a href="https://pypi.python.org/pypi/nonebot-plugin-hx-yinying">
-    <img src="https://img.shields.io/pypi/v/nonebot-plugin-status.svg" alt="pypi">
+    <img src="https://skin.huanxinbot.com/api/pypi.svg" alt="pypi">
   </a>
   <img src="https://img.shields.io/badge/python-3.10+-blue.svg" alt="python">
 </p>
 
 ## 使用方式
 
 通用:
@@ -58,15 +58,21 @@
 
 - @Bot
 - 回复Bot
 
 ## 配置项
 
 > [!WARNING]
-> GitHub 仓库中的文档为最新 DEV 版本，配置方式请参考 [PyPI](https://pypi.org/project/nonebot-plugin-status/) 上的文档。
+> GitHub 仓库中的文档为最新 DEV 版本，配置方式请参考 [PyPI](https://pypi.python.org/pypi/nonebot-plugin-hx-yinying) 上的文档。
+
+> [!WARNING]
+> 秩乱(乱乱)的联系方式如下，QQ:1660466270，官方qq群聊:175334224 [官网链接](https://chat.wingmark.cn/) .
+
+> [!WARNING]
+> 请注意，该项目是接入了乱乱的项目，你需要遵守api使用的 [规范](https://wingmark.feishu.cn/docx/NFgJddgQAotygKxXiu6cpyg5nqr)。
 
 配置方式：直接在 NoneBot 全局配置文件中添加以下配置项即可。
 
 ### yinying_appid
 
 - 类型：`str`
 - 默认值：`None`
@@ -89,14 +95,15 @@
 - 重要：必填
 
 ### yinying_model
 
 - 类型：`str`
 - 默认值：`None`
 - 说明：选择使用银影的模型
+- 注意 该配置项即将移除（转为插件内配置！）
 
 ## hx_path
 - 类型：`str`
 - 默认值：`None`
 - 说明：银影对话的用户数据存储路径(不写将使用默认配置)
 
 ## hx_reply
```

#### html2text {}

```diff
@@ -1,33 +1,39 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 0.0.6 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 0.0.7 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
 img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
-huanxin996 * @LastEditTime : 2024-4-18 * @Description : None * @GitHub : https:
+huanxin996 * @LastEditTime : 2024-4-19 * @Description : None * @GitHub : https:
 //github.com/huanxin996 -->
                                    _[_n_o_n_e_b_o_t_]
                 # nonebot_plugin_hx-yinying _â¨ Hx vs YinYing
                   (å¨çº¿ä¸é¶å½±è¿è¡å¯¹è¯çæä»¶) â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## ä½¿ç¨æ¹å¼ éç¨: - @Bot æèåå¤å³å¯ OneBot: - @Bot - åå¤Bot ##
 éç½®é¡¹ > [!WARNING] > GitHub ä»åºä¸­çææ¡£ä¸ºææ° DEV
-çæ¬ï¼éç½®æ¹å¼è¯·åè [PyPI](https://pypi.org/project/nonebot-plugin-
-status/) ä¸çææ¡£ã éç½®æ¹å¼ï¼ç´æ¥å¨ NoneBot
+çæ¬ï¼éç½®æ¹å¼è¯·åè [PyPI](https://pypi.python.org/pypi/nonebot-
+plugin-hx-yinying) ä¸çææ¡£ã > [!WARNING] > ç§©ä¹±
+(ä¹±ä¹±)çèç³»æ¹å¼å¦ä¸ï¼QQ:1660466270ï¼å®æ¹qqç¾¤è:175334224
+[å®ç½é¾æ¥](https://chat.wingmark.cn/) . > [!WARNING] >
+è¯·æ³¨æï¼è¯¥é¡¹ç®æ¯æ¥å¥äºä¹±ä¹±çé¡¹ç®ï¼ä½ éè¦éµå®apiä½¿ç¨ç
+[è§è](https://wingmark.feishu.cn/docx/NFgJddgQAotygKxXiu6cpyg5nqr)ã
+éç½®æ¹å¼ï¼ç´æ¥å¨ NoneBot
 å¨å±éç½®æä»¶ä¸­æ·»å ä»¥ä¸éç½®é¡¹å³å¯ã ### yinying_appid -
 ç±»åï¼`str` - é»è®¤å¼ï¼`None` - è¯´æï¼ä½ çappid - éè¦ï¼å¿å¡«
 ### yinying_token - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
 è¯´æï¼è¿éåä½ æ¾ç§©ä¹±è·åå°çapi_key - éè¦ï¼å¿å¡« ###
 hx_api_yinying - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
 è¯´æï¼yinyingçapiå°å - éè¦ï¼å¿å¡« ### yinying_model -
-ç±»åï¼`str` - é»è®¤å¼ï¼`None` - è¯´æï¼éæ©ä½¿ç¨é¶å½±çæ¨¡å ##
-hx_path - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
+ç±»åï¼`str` - é»è®¤å¼ï¼`None` - è¯´æï¼éæ©ä½¿ç¨é¶å½±çæ¨¡å -
+æ³¨æ è¯¥éç½®é¡¹å³å°ç§»é¤ï¼è½¬ä¸ºæä»¶åéç½®ï¼ï¼ ## hx_path -
+ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
 è¯´æï¼é¶å½±å¯¹è¯çç¨æ·æ°æ®å­å¨è·¯å¾(ä¸åå°ä½¿ç¨é»è®¤éç½®)
 ## hx_reply - ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
 è¯´æï¼botåéchatæ¶æ¯æ¶æ¯å¦åå¤ -
 æ³¨æï¼è¯¥é¡¹å¯ç¨æ¶hx_reply_atå°è¢«å¿½ç¥ ## hx_reply_at -
 ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
 è¯´æï¼botåéchatæ¶æ¯æ¶ä¸åå¤æ¶æ¯å¦è¾ç¹ ## yinying_limit -
 ç±»åï¼`int` - é»è®¤å¼ï¼`12` - è¯´æï¼å¯¹äºé¶å½±å¯¹è¯éå¶çæ¬¡æ°
```

### Comparing `nonebot-plugin-hx-yinying-0.0.6/setup.py` & `nonebot-plugin-hx-yinying-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot-plugin-hx-yinying",
-    version="0.0.6",
+    version="0.0.7",
     author="Huan Xin",
     author_email="mc.xiaolang@foxmail.com",
     description="chat with yinying",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/huanxin996/nonebot_plugin_hx-yinying",
     packages=setuptools.find_packages(),
```

