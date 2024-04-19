# Comparing `tmp/fistminio-1.0.1.tar.gz` & `tmp/fistminio-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fistminio-1.0.1.tar", last modified: Wed Jan 31 06:35:31 2024, max compression
+gzip compressed data, was "fistminio-1.0.2.tar", last modified: Fri Apr 19 07:23:17 2024, max compression
```

## Comparing `fistminio-1.0.1.tar` & `fistminio-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-01-31 06:35:31.490495 fistminio-1.0.1/
--rw-rw-rw-   0        0        0    11358 2024-01-13 17:42:18.000000 fistminio-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     6545 2024-01-31 06:35:31.489494 fistminio-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5589 2024-01-31 03:46:26.000000 fistminio-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-01-31 06:35:31.480494 fistminio-1.0.1/fistminio/
--rw-rw-rw-   0        0        0        0 2024-01-25 11:23:36.000000 fistminio-1.0.1/fistminio/__init__.py
--rw-rw-rw-   0        0        0    15041 2024-01-31 06:17:42.000000 fistminio-1.0.1/fistminio/fistapi.py
-drwxrwxrwx   0        0        0        0 2024-01-31 06:35:31.489494 fistminio-1.0.1/fistminio.egg-info/
--rw-rw-rw-   0        0        0     6545 2024-01-31 06:35:31.000000 fistminio-1.0.1/fistminio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2024-01-31 06:35:31.000000 fistminio-1.0.1/fistminio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-31 06:35:31.000000 fistminio-1.0.1/fistminio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-01-31 06:35:31.000000 fistminio-1.0.1/fistminio.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-01-31 06:35:31.000000 fistminio-1.0.1/fistminio.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-31 06:35:31.490495 fistminio-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1082 2024-01-31 06:30:40.000000 fistminio-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:23:17.506816 fistminio-1.0.2/
+-rw-rw-rw-   0        0        0    11560 2024-04-19 02:51:05.000000 fistminio-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     6650 2024-04-19 07:23:17.504817 fistminio-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5876 2024-04-19 07:23:13.000000 fistminio-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 07:23:17.491817 fistminio-1.0.2/fistminio/
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:05.000000 fistminio-1.0.2/fistminio/__init__.py
+-rw-rw-rw-   0        0        0    15162 2024-04-19 07:01:27.000000 fistminio-1.0.2/fistminio/fistapi.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:23:17.502817 fistminio-1.0.2/fistminio.egg-info/
+-rw-rw-rw-   0        0        0     6650 2024-04-19 07:23:17.000000 fistminio-1.0.2/fistminio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2024-04-19 07:23:17.000000 fistminio-1.0.2/fistminio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 07:23:17.000000 fistminio-1.0.2/fistminio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-04-19 07:23:17.000000 fistminio-1.0.2/fistminio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-19 07:23:17.000000 fistminio-1.0.2/fistminio.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 07:23:17.507820 fistminio-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1082 2024-04-19 07:19:27.000000 fistminio-1.0.2/setup.py
```

### Comparing `fistminio-1.0.1/LICENSE` & `fistminio-1.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,202 +1,202 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "{}"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright {yyyy} {name of copyright owner}
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
-
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "{}"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright {yyyy} {name of copyright owner}
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
+
```

### Comparing `fistminio-1.0.1/PKG-INFO` & `fistminio-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fistminio
-Version: 1.0.1
+Version: 1.0.2
 Summary: FIST MinIO Client SDK for Python
 Author: ccyy
 Author-email: 1805878415@qq.com
 License: Apache-2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -25,14 +25,19 @@
 
 基于MinIO Python Client SDK 构建 FIST 内部 Py-Client 访问 MinIO 云存储服务
 
 本文将介绍如何安装FIST MinIO Client SDK for Python，并基于`fistminio.fistapi`进行fistminio用户注册，运行简单文件上传和下载示例程序。对于更完整的API以及更多使用示例，请参考[Python Client API Reference](https://min.io/docs/minio/linux/developers/python/API.html)。
 
 假设您已经有一个可运行的 [Python](https://www.python.org/downloads/)开发环境。
 
+> Update history：
+> 
+> * 2024-01-31 1.0.1 初始版本
+> * 2024-04-19 1.0.2 新增外网ip访问
+
 ## 最低要求
 
 - Python 3.7或更高版本
 
 ## 使用pip安装
 
 ```sh
```

### Comparing `fistminio-1.0.1/README.md` & `fistminio-1.0.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,183 +1,188 @@
-# FIST MinIO Client SDK for Python
-
-基于MinIO Python Client SDK 构建 FIST 内部 Py-Client 访问 MinIO 云存储服务
-
-本文将介绍如何安装FIST MinIO Client SDK for Python，并基于`fistminio.fistapi`进行fistminio用户注册，运行简单文件上传和下载示例程序。对于更完整的API以及更多使用示例，请参考[Python Client API Reference](https://min.io/docs/minio/linux/developers/python/API.html)。
-
-假设您已经有一个可运行的 [Python](https://www.python.org/downloads/)开发环境。
-
-## 最低要求
-
-- Python 3.7或更高版本
-
-## 使用pip安装
-
-```sh
-pip install fistminio
-```
-
-## 示例-自行注册fistminio用户
-需要根据《fistuser使用手册》手册，创建 `fistmino_autousers_keys.yaml`配置文件，再执行`python auto_register.py`
-
-#### auto_register.py
-
-```py
-from fistminio.fistapi import register_user
-
-# 自动进行fistminio用户注册
-register_user('fistmino_autousers_keys.yaml')
-```
-
-#### Run auto_register
-
-```bash
-python auto_register.py
-```
-
-## 配置 FIST MinIO Client
-
-FIST MinIO client需要以下3个参数来连接 FIST MinIO 对象存储服务。
-
-| 参数     | 描述  |
-| :------- | :---- |
-| bucket_name | 所在FIST存储服务器上的存储桶名（默认为Username） |
-| access_key| Access key是唯一标识你的账户的用户ID  |
-| secret_key| Secret key是你账户的密码  |
-
-## 示例-文件夹上传
-本示例使用测试用户 wangdc 访问 FIST MinIO 对象存储服务，并上传一个文件文件夹到存储桶中。
-
-#### folder_upload.py
-
-```py
-from fistminio.fistapi import init_minio_client, upload_folder
-
-# 替换为自己的access_key和secret_key
-access_key="your_access_key"
-secret_key="your_secret_key"
-client = init_minio_client(access_key, secret_key)
-
-# bucket_name替换为自己的Username
-bucket_name = "wangdc"
-
-# 本地需要上传的文件夹路径
-source_folder = "C:\\Users\\18058\\Desktop\\youtube"
-# FIST存储服务器上的目标文件夹路径，如果没用会自动新建文件夹
-target_folder = "youtube/"
-# 调用upload_folder上传整个文件
-upload_folder(client, bucket_name, source_folder, target_folder)
-```
-
-#### Run folder_upload
-
-```bash
-python folder_upload.py
-
-Uploading files: 100%|████████████████| 99/99 [00:06<00:00, 15.04it/s]
-😀 Upload successful. All contents from the local folder 'C:\Users\18058\Desktop\youtube' have been successfully uploaded to the bucket 'wangdc/youtube/'.
-```
-
-## 其他示例
-
-目前`fistminio.fistapi`实现单文件/文件夹上传、下载、删除，更多api待完善。
-* [API开发文档参考](https://min.io/docs/minio/linux/developers/python/API.html)
-
-#### single_file_upload.py
-```py
-from fistminio.fistapi import init_minio_client, fupload
-
-# 替换为自己的access_key和secret_key
-access_key="your_access_key"
-secret_key="your_secret_key"
-client = init_minio_client(access_key, secret_key)
-
-# bucket_name替换为自己的Username
-bucket_name = "wangdc"
-
-# 本地需要上传的文件路径
-source_file = "tmp/test-file.txt"
-# FIST 存储服务器上的目标文件路径
-dest_file = "/newfolder/rename-test-file.txt"
-# 调用upload上传单个文件
-fupload(client, bucket_name, source_file, dest_file)
-```
-
-
-
-#### single_file_download.py
-```py
-from fistminio.fistapi import init_minio_client, fdownload
-
-# 替换为自己的access_key和secret_key
-access_key="your_access_key"
-secret_key="your_secret_key"
-client = init_minio_client(access_key, secret_key)
-
-# bucket_name替换为自己的Username
-bucket_name = "wangdc"
-
-# FIST存储服务器上需要下载的文件路径
-source_file = "CrawlGoogleScholar_v1.rar"
-# 目标文件本地路径
-dest_file = "tmp/CrawlGoogleScholar_v1.rar"
-# 调用fdownload下载单个文件
-fdownload(client, bucket_name, source_file, dest_file)
-```
-
-#### folder_download.py
-```py
-from fistminio.fistapi import init_minio_client, download_folder
-
-# 替换为自己的access_key和secret_key
-access_key="your_access_key"
-secret_key="your_secret_key"
-client = init_minio_client(access_key, secret_key)
-
-# bucket_name替换为自己的Username
-bucket_name = "wangdc"
-
-# FIST存储服务器上需要下载的文件夹路径
-source_folder_prefix = "hmr-master/"
-# 目标文件夹本地路径
-dest_local_folder_path = "tmp/hmr-master/"
-# 调用download_folder下载整个文件夹
-download_folder(client, bucket_name, source_folder_prefix, dest_local_folder_path)
-```
-
-### single_file_deleted.py
-```py
-from fistminio.fistapi import init_minio_client, delete_object_from_bucket
-
-# 替换为自己的access_key和secret_key
-access_key="your_access_key"
-secret_key="your_secret_key"
-client = init_minio_client(access_key, secret_key)
-
-# bucket_name替换为自己的Username
-bucket_name = "wangdc"
-
-# FIST存储服务器上要删除的目标文件路径
-target_file = "youtube/start.bat"
-# 调用delete_object_from_bucket删除单个文件
-delete_object_from_bucket(client, bucket_name, target_file)
-```
-
-### folder_deleted.py
-```py
-from fistminio.fistapi import init_minio_client, download_folder
-
-# 替换为自己的access_key和secret_key
-access_key="your_access_key"
-secret_key="your_secret_key"
-client = init_minio_client(access_key, secret_key)
-
-# bucket_name替换为自己的Username
-bucket_name = "wangdc"
-
-# FIST存储服务器上需要下载的文件夹路径
-source_folder_prefix = "hmr-master/"
-# 目标文件夹本地路径
-dest_local_folder_path = "tmp/hmr-master/"
-# 调用download_folder下载整个文件夹
-download_folder(client, bucket_name, source_folder_prefix, dest_local_folder_path)
+# FIST MinIO Client SDK for Python
+
+基于MinIO Python Client SDK 构建 FIST 内部 Py-Client 访问 MinIO 云存储服务
+
+本文将介绍如何安装FIST MinIO Client SDK for Python，并基于`fistminio.fistapi`进行fistminio用户注册，运行简单文件上传和下载示例程序。对于更完整的API以及更多使用示例，请参考[Python Client API Reference](https://min.io/docs/minio/linux/developers/python/API.html)。
+
+假设您已经有一个可运行的 [Python](https://www.python.org/downloads/)开发环境。
+
+> Update history：
+> 
+> * 2024-01-31 1.0.1 初始版本
+> * 2024-04-19 1.0.2 新增外网ip访问
+
+## 最低要求
+
+- Python 3.7或更高版本
+
+## 使用pip安装
+
+```sh
+pip install fistminio
+```
+
+## 示例-自行注册fistminio用户
+需要根据《fistuser使用手册》手册，创建 `fistmino_autousers_keys.yaml`配置文件，再执行`python auto_register.py`
+
+#### auto_register.py
+
+```py
+from fistminio.fistapi import register_user
+
+# 自动进行fistminio用户注册
+register_user('fistmino_autousers_keys.yaml')
+```
+
+#### Run auto_register
+
+```bash
+python auto_register.py
+```
+
+## 配置 FIST MinIO Client
+
+FIST MinIO client需要以下3个参数来连接 FIST MinIO 对象存储服务。
+
+| 参数     | 描述  |
+| :------- | :---- |
+| bucket_name | 所在FIST存储服务器上的存储桶名（默认为Username） |
+| access_key| Access key是唯一标识你的账户的用户ID  |
+| secret_key| Secret key是你账户的密码  |
+
+## 示例-文件夹上传
+本示例使用测试用户 wangdc 访问 FIST MinIO 对象存储服务，并上传一个文件文件夹到存储桶中。
+
+#### folder_upload.py
+
+```py
+from fistminio.fistapi import init_minio_client, upload_folder
+
+# 替换为自己的access_key和secret_key
+access_key="your_access_key"
+secret_key="your_secret_key"
+client = init_minio_client(access_key, secret_key)
+
+# bucket_name替换为自己的Username
+bucket_name = "wangdc"
+
+# 本地需要上传的文件夹路径
+source_folder = "C:\\Users\\18058\\Desktop\\youtube"
+# FIST存储服务器上的目标文件夹路径，如果没用会自动新建文件夹
+target_folder = "youtube/"
+# 调用upload_folder上传整个文件
+upload_folder(client, bucket_name, source_folder, target_folder)
+```
+
+#### Run folder_upload
+
+```bash
+python folder_upload.py
+
+Uploading files: 100%|████████████████| 99/99 [00:06<00:00, 15.04it/s]
+😀 Upload successful. All contents from the local folder 'C:\Users\18058\Desktop\youtube' have been successfully uploaded to the bucket 'wangdc/youtube/'.
+```
+
+## 其他示例
+
+目前`fistminio.fistapi`实现单文件/文件夹上传、下载、删除，更多api待完善。
+* [API开发文档参考](https://min.io/docs/minio/linux/developers/python/API.html)
+
+#### single_file_upload.py
+```py
+from fistminio.fistapi import init_minio_client, fupload
+
+# 替换为自己的access_key和secret_key
+access_key="your_access_key"
+secret_key="your_secret_key"
+client = init_minio_client(access_key, secret_key)
+
+# bucket_name替换为自己的Username
+bucket_name = "wangdc"
+
+# 本地需要上传的文件路径
+source_file = "tmp/test-file.txt"
+# FIST 存储服务器上的目标文件路径
+dest_file = "/newfolder/rename-test-file.txt"
+# 调用upload上传单个文件
+fupload(client, bucket_name, source_file, dest_file)
+```
+
+
+
+#### single_file_download.py
+```py
+from fistminio.fistapi import init_minio_client, fdownload
+
+# 替换为自己的access_key和secret_key
+access_key="your_access_key"
+secret_key="your_secret_key"
+client = init_minio_client(access_key, secret_key)
+
+# bucket_name替换为自己的Username
+bucket_name = "wangdc"
+
+# FIST存储服务器上需要下载的文件路径
+source_file = "CrawlGoogleScholar_v1.rar"
+# 目标文件本地路径
+dest_file = "tmp/CrawlGoogleScholar_v1.rar"
+# 调用fdownload下载单个文件
+fdownload(client, bucket_name, source_file, dest_file)
+```
+
+#### folder_download.py
+```py
+from fistminio.fistapi import init_minio_client, download_folder
+
+# 替换为自己的access_key和secret_key
+access_key="your_access_key"
+secret_key="your_secret_key"
+client = init_minio_client(access_key, secret_key)
+
+# bucket_name替换为自己的Username
+bucket_name = "wangdc"
+
+# FIST存储服务器上需要下载的文件夹路径
+source_folder_prefix = "hmr-master/"
+# 目标文件夹本地路径
+dest_local_folder_path = "tmp/hmr-master/"
+# 调用download_folder下载整个文件夹
+download_folder(client, bucket_name, source_folder_prefix, dest_local_folder_path)
+```
+
+### single_file_deleted.py
+```py
+from fistminio.fistapi import init_minio_client, delete_object_from_bucket
+
+# 替换为自己的access_key和secret_key
+access_key="your_access_key"
+secret_key="your_secret_key"
+client = init_minio_client(access_key, secret_key)
+
+# bucket_name替换为自己的Username
+bucket_name = "wangdc"
+
+# FIST存储服务器上要删除的目标文件路径
+target_file = "youtube/start.bat"
+# 调用delete_object_from_bucket删除单个文件
+delete_object_from_bucket(client, bucket_name, target_file)
+```
+
+### folder_deleted.py
+```py
+from fistminio.fistapi import init_minio_client, download_folder
+
+# 替换为自己的access_key和secret_key
+access_key="your_access_key"
+secret_key="your_secret_key"
+client = init_minio_client(access_key, secret_key)
+
+# bucket_name替换为自己的Username
+bucket_name = "wangdc"
+
+# FIST存储服务器上需要下载的文件夹路径
+source_folder_prefix = "hmr-master/"
+# 目标文件夹本地路径
+dest_local_folder_path = "tmp/hmr-master/"
+# 调用download_folder下载整个文件夹
+download_folder(client, bucket_name, source_folder_prefix, dest_local_folder_path)
 ```
```

### Comparing `fistminio-1.0.1/fistminio/fistapi.py` & `fistminio-1.0.2/fistminio/fistapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,20 @@
 from minio.minioadmin import MinioAdmin
 from minio.error import S3Error
 import tempfile
 
 from tqdm import tqdm 
 from cryptography.fernet import Fernet
 
+ip = '58.57.119.57'
+page_port = '10025'
+api_service_port = '10105'
 
 def init_minio_client(access_key, secret_key):
-    return Minio("172.16.60.18:9000",
+    return Minio(ip+':'+api_service_port,
                  access_key=access_key,
                  secret_key=secret_key,
                  secure=False)
 
 
 def check_bucket_exists(client, bucket_name):
     found = client.bucket_exists(bucket_name)
@@ -130,19 +133,19 @@
     :param user_name: The username for the new user.
     :param password: The password for the new user.
     :param group_name: The name of the group to add the new user to.
     """
     minio_admin_client.user_add(user_name, password)
     add_user_to_group(minio_admin_client, user_name, group_name)
     minio_client.make_bucket(user_name)
-    text_content = f"Welcome {user_name}. Please access the console through the browser at http://172.16.60.18:9001, Username: {user_name}, Password: {password}. \
+    text_content = f"Welcome {user_name}. Please access the console through the browser at http:{ip}:{page_port}, Username: {user_name}, Password: {password}. \
                     \nYou can also apply for Access Keys in the console using Minio Client and fistminio SDK"
     destination_file = "access_info.txt"  # The name of the file saved in the bucket
     upload_text_as_file(minio_client, user_name, text_content, destination_file)
-    print(f"User created successfully. Please access the console through the browser at http://172.16.60.18:9001, Username: {user_name}, Password: {password}")
+    print(f"User created successfully. Please access the console through the browser at http:{ip}:{page_port}, Username: {user_name}, Password: {password}")
 
 
 def register_user(yaml_file_path):
     """
     Register a new user in the MinIO server by reading encrypted credentials from a YAML file, decrypting them, and creating a new user and bucket.
 
     :param yaml_file_path: Path to the YAML file containing encrypted MinIO access and secret keys.
@@ -157,23 +160,23 @@
         encrypted_data = yaml.safe_load(yaml_file)
 
     cipher_suite = Fernet(encrypted_data['key'].encode())
     decrypted_access_key = cipher_suite.decrypt(encrypted_data['encoder_access_key'].encode()).decode()
     decrypted_secret_key = cipher_suite.decrypt(encrypted_data['encoder_secret_key'].encode()).decode()
 
     minio_client = init_minio_client(decrypted_access_key, decrypted_secret_key)
-    minio_admin_client = MinioAdmin(endpoint="172.16.60.18:9000",
+    minio_admin_client = MinioAdmin(endpoint=ip+':'+api_service_port,
                                     credentials=StaticProvider(access_key=decrypted_access_key,
                                                                secret_key=decrypted_secret_key),
                                     secure=False)
 
-    username = input("Please enter a username (3-63 characters): ")
-    while not (3 <= len(username) <= 63 and username.isascii() and username.isalnum()):
-        print("The username must be between 3 to 63 ASCII characters, please re-enter.")
-        username = input("Please enter a username (3-63 characters):")
+    username = input("Please enter a username (3-63 Lowercase characters): ")
+    while not (3 <= len(username) <= 63 and username.isascii() and username.isalnum() or "_" in username):
+        print("The username must be between 3 to 63 ASCII Lowercase characters, please re-enter.")
+        username = input("Please enter a username (3-63 Lowercase characters):")
     password = username + '123456'
     auto_create_users(minio_client, minio_admin_client, username, password, "fistgroup")
 
 
 def upload_folder(minio_client, bucket_name, folder_path, target_folder):
     """
     Upload all contents of a local folder to a specified folder in a MinIO bucket.
```

### Comparing `fistminio-1.0.1/fistminio.egg-info/PKG-INFO` & `fistminio-1.0.2/fistminio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fistminio
-Version: 1.0.1
+Version: 1.0.2
 Summary: FIST MinIO Client SDK for Python
 Author: ccyy
 Author-email: 1805878415@qq.com
 License: Apache-2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -25,14 +25,19 @@
 
 基于MinIO Python Client SDK 构建 FIST 内部 Py-Client 访问 MinIO 云存储服务
 
 本文将介绍如何安装FIST MinIO Client SDK for Python，并基于`fistminio.fistapi`进行fistminio用户注册，运行简单文件上传和下载示例程序。对于更完整的API以及更多使用示例，请参考[Python Client API Reference](https://min.io/docs/minio/linux/developers/python/API.html)。
 
 假设您已经有一个可运行的 [Python](https://www.python.org/downloads/)开发环境。
 
+> Update history：
+> 
+> * 2024-01-31 1.0.1 初始版本
+> * 2024-04-19 1.0.2 新增外网ip访问
+
 ## 最低要求
 
 - Python 3.7或更高版本
 
 ## 使用pip安装
 
 ```sh
```

### Comparing `fistminio-1.0.1/setup.py` & `fistminio-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setuptools.setup(
     name="fistminio",
     description="FIST MinIO Client SDK for Python",
     author="ccyy",
     author_email="1805878415@qq.com",
-    version="1.0.1",
+    version="1.0.2",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # package_dir={"fistminio": "fistminio"},
     packages=setuptools.find_packages(),
     license="Apache-2.0",
     classifiers=[
         "Programming Language :: Python",
```

