# Comparing `tmp/eirStru-0.2.99.tar.gz` & `tmp/eirStru-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eirStru-0.2.99.tar", last modified: Mon Apr 15 09:38:10 2024, max compression
+gzip compressed data, was "eirStru-0.3.0.tar", last modified: Fri Apr 19 09:06:14 2024, max compression
```

## Comparing `eirStru-0.2.99.tar` & `eirStru-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-15 09:38:10.604345 eirStru-0.2.99/
--rw-r--r--   0 wangwh     (501) staff       (20)     1060 2024-01-25 06:27:18.000000 eirStru-0.2.99/LICENSE
--rw-r--r--   0 wangwh     (501) staff       (20)       26 2024-01-25 06:27:18.000000 eirStru-0.2.99/MANIFEST.in
--rw-r--r--   0 wangwh     (501) staff       (20)     2964 2024-04-15 09:38:10.604060 eirStru-0.2.99/PKG-INFO
--rw-r--r--   0 wangwh     (501) staff       (20)     2338 2024-01-25 06:27:18.000000 eirStru-0.2.99/README.md
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-15 09:38:10.603037 eirStru-0.2.99/eirStru/
--rw-r--r--   0 wangwh     (501) staff       (20)       43 2024-03-14 03:14:41.000000 eirStru-0.2.99/eirStru/__init__.py
--rw-r--r--   0 wangwh     (501) staff       (20)      352 2024-01-25 06:27:18.000000 eirStru-0.2.99/eirStru/__version__.py
--rwxr--r--   0 wangwh     (501) staff       (20)     5220 2024-03-14 03:14:41.000000 eirStru-0.2.99/eirStru/aiomysql_helper.py
--rwxr--r--   0 wangwh     (501) staff       (20)    18149 2024-04-15 09:07:32.000000 eirStru-0.2.99/eirStru/common.py
--rw-r--r--   0 wangwh     (501) staff       (20)     3584 2024-02-29 12:42:57.000000 eirStru-0.2.99/eirStru/eirjob_intf.py
--rw-r--r--   0 wangwh     (501) staff       (20)     5936 2024-04-15 08:37:49.000000 eirStru-0.2.99/eirStru/eirlogin_intf.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1190 2024-02-29 02:15:20.000000 eirStru-0.2.99/eirStru/redis_utils.py
--rw-r--r--   0 wangwh     (501) staff       (20)      421 2024-03-15 21:24:26.000000 eirStru-0.2.99/eirStru/test.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1428 2024-03-14 03:14:41.000000 eirStru-0.2.99/eirStru/utils.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1670 2024-03-15 21:25:26.000000 eirStru-0.2.99/eirStru/wx_push.py
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-15 09:38:10.603749 eirStru-0.2.99/eirStru.egg-info/
--rw-r--r--   0 wangwh     (501) staff       (20)     2964 2024-04-15 09:38:10.000000 eirStru-0.2.99/eirStru.egg-info/PKG-INFO
--rw-r--r--   0 wangwh     (501) staff       (20)      373 2024-04-15 09:38:10.000000 eirStru-0.2.99/eirStru.egg-info/SOURCES.txt
--rw-r--r--   0 wangwh     (501) staff       (20)        1 2024-04-15 09:38:10.000000 eirStru-0.2.99/eirStru.egg-info/dependency_links.txt
--rw-r--r--   0 wangwh     (501) staff       (20)        8 2024-04-15 09:38:10.000000 eirStru-0.2.99/eirStru.egg-info/top_level.txt
--rw-r--r--   0 wangwh     (501) staff       (20)       38 2024-04-15 09:38:10.604392 eirStru-0.2.99/setup.cfg
--rw-r--r--   0 wangwh     (501) staff       (20)     3777 2024-04-15 09:38:08.000000 eirStru-0.2.99/setup.py
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-19 09:06:14.768273 eirStru-0.3.0/
+-rw-r--r--   0 wangwh     (501) staff       (20)     1060 2024-01-25 06:27:18.000000 eirStru-0.3.0/LICENSE
+-rw-r--r--   0 wangwh     (501) staff       (20)       26 2024-01-25 06:27:18.000000 eirStru-0.3.0/MANIFEST.in
+-rw-r--r--   0 wangwh     (501) staff       (20)     2963 2024-04-19 09:06:14.768050 eirStru-0.3.0/PKG-INFO
+-rw-r--r--   0 wangwh     (501) staff       (20)     2338 2024-01-25 06:27:18.000000 eirStru-0.3.0/README.md
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-19 09:06:14.767344 eirStru-0.3.0/eirStru/
+-rw-r--r--   0 wangwh     (501) staff       (20)       43 2024-03-14 03:14:41.000000 eirStru-0.3.0/eirStru/__init__.py
+-rw-r--r--   0 wangwh     (501) staff       (20)      352 2024-01-25 06:27:18.000000 eirStru-0.3.0/eirStru/__version__.py
+-rwxr--r--   0 wangwh     (501) staff       (20)     5220 2024-03-14 03:14:41.000000 eirStru-0.3.0/eirStru/aiomysql_helper.py
+-rwxr--r--   0 wangwh     (501) staff       (20)    18256 2024-04-18 16:43:10.000000 eirStru-0.3.0/eirStru/common.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     4341 2024-04-19 09:06:12.000000 eirStru-0.3.0/eirStru/eirjob_intf.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     6488 2024-04-19 09:06:12.000000 eirStru-0.3.0/eirStru/eirlogin_intf.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1190 2024-02-29 02:15:20.000000 eirStru-0.3.0/eirStru/redis_utils.py
+-rw-r--r--   0 wangwh     (501) staff       (20)      421 2024-03-15 21:24:26.000000 eirStru-0.3.0/eirStru/test.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1389 2024-04-18 23:20:17.000000 eirStru-0.3.0/eirStru/utils.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1670 2024-03-15 21:25:26.000000 eirStru-0.3.0/eirStru/wx_push.py
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-19 09:06:14.767861 eirStru-0.3.0/eirStru.egg-info/
+-rw-r--r--   0 wangwh     (501) staff       (20)     2963 2024-04-19 09:06:14.000000 eirStru-0.3.0/eirStru.egg-info/PKG-INFO
+-rw-r--r--   0 wangwh     (501) staff       (20)      373 2024-04-19 09:06:14.000000 eirStru-0.3.0/eirStru.egg-info/SOURCES.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)        1 2024-04-19 09:06:14.000000 eirStru-0.3.0/eirStru.egg-info/dependency_links.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)        8 2024-04-19 09:06:14.000000 eirStru-0.3.0/eirStru.egg-info/top_level.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)       38 2024-04-19 09:06:14.768322 eirStru-0.3.0/setup.cfg
+-rw-r--r--   0 wangwh     (501) staff       (20)     3776 2024-04-19 09:06:12.000000 eirStru-0.3.0/setup.py
```

### Comparing `eirStru-0.2.99/LICENSE` & `eirStru-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.99/PKG-INFO` & `eirStru-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eirStru
-Version: 0.2.99
+Version: 0.3.0
 Summary: My short description for my project.
 Home-page: https://github.com/me/myproject
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `eirStru-0.2.99/README.md` & `eirStru-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.99/eirStru/aiomysql_helper.py` & `eirStru-0.3.0/eirStru/aiomysql_helper.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.99/eirStru/common.py` & `eirStru-0.3.0/eirStru/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import re
-import time
 import uuid
 from datetime import datetime, timedelta, date
 from enum import Enum
 from typing import Optional, Any, List, Dict
 
 from loguru import logger
 from pydantic import BaseModel
@@ -11,17 +10,17 @@
 
 # 调用返回类型
 class RespType(Enum):
     """
     调用返回类型
     """
     task_success = 1  # 任务成功执行，并有结果
-    task_normal = 0  # 任务成功执行，但无结果
+    task_normal = 0  # 任务成功执行
     task_failed = -1  # 任务失败/取消
-    task_delay = -2  # 任务延迟执行
+    task_delay = -2  # 任务延迟执行，比如下一次执行时间5min后
     task_stock_limit = -3  # 无库存
     session_expired = -11  # session过期
     session_invalid_token = -12  # 无效token
     session_invalid_user = -13  # 无效用户名
     session_invalid_password = -14  # 无效密码
     session_user_blocked = -15  # 用户被冻结
     session_request_limit = -16  # 访问次数受限
@@ -61,21 +60,27 @@
 
 class ResponseData(BaseModel):
     """
     响应类
     """
     code: Optional[RespType] = None
     msg: Optional[str] = ''
-    data: Optional[Any] = None
-    log: Optional[bool] = False
+    data: Optional[Any] = None  # 转换后的数据
+    response: Optional[Any] = None  # 原始响应
+    log: Optional[bool] = False  # 是否打印日志
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        if (self.msg or self.data) and self.log:
-            logger.info(f'{self.code.name} {self.msg} {self.data if self.data else ""}')
+        if (self.msg or self.data):
+            if self.code == RespType.task_success:
+                logger.warning(f'{self.msg} {self.data if self.data else ""}')
+            elif self.code == RespType.task_failed:
+                logger.error(f'{self.msg} {self.data if self.data else ""}')
+            else:
+                logger.info(f'{self.msg} {self.data if self.data else ""}')
 
     def __str__(self):
         return f'{self.code.name} {self.msg} {self.data if self.data else ""}'
 
 
 class SessionData(BaseModel):
     """
@@ -94,14 +99,17 @@
     last_access_resp_type: Optional[RespType] = RespType.task_normal
 
     def __init__(self, **data: Any):
         super().__init__(**data)
         if not data.get('session_guid'):
             self.session_guid = uuid.uuid4().hex
 
+    def __str__(self):
+        return f'{self.carrier_id}-{self.session_guid}'
+
     @property
     def redis_session_key(self):
         return f'{self.carrier_id}:{self.account}:{self.session_guid}'
 
 
 class EirTaskInfo(BaseModel):
     """
@@ -111,15 +119,15 @@
     carrier_id: Optional[str] = ''  # 船公司
     bookingagent_id: Optional[str] = ''  # 一代
     account: Optional[str] = ''  # 账号
     password: Optional[str] = ''  # 密码
     bill_no: Optional[str] = ''  # 提单号
     valid_code: Optional[str] = ''  # 校验码
 
-    apply_ctntypedigit: Optional[str] = ''  # 申请箱型箱量 todo cma？
+    apply_ctntypedigit: Optional[str] = ''  # 需一次性申请的箱型箱量
     ctntype_id: Optional[str] = ''  # 箱型
     ctn_digit: Optional[int] = 0  # 箱量
     client_user: Optional[str] = ''  # 客户用户名
     client_user_openid: Optional[str] = ''  # 客户用户Openid用于推送
 
     callback_url: Optional[str] = ''  # 回调url
     notify_email: Optional[str] = ''
@@ -127,15 +135,15 @@
     begin_time: Optional[datetime] = datetime.strptime(datetime.strftime(datetime.now(), '%Y-%m-%d %H:%M:%S'),
                                                        '%Y-%m-%d %H:%M:%S')  # 刷箱开始时间
     end_time: Optional[datetime] = datetime.strptime(
         datetime.strftime(datetime.now() + timedelta(hours=4), '%Y-%m-%d %H:%M:%S'),
         '%Y-%m-%d %H:%M:%S')  # 刷箱结束时间
     plan_amount: Optional[int] = 0  # 计划数 todo
     memo: Optional[str] = None  # 备注
-    cyname: Optional[str] = None
+    cyname: Optional[str] = None  # 推荐堆场
     account_list: Optional[List[dict]] = []
     vessel: Optional[str] = None
     voyage: Optional[str] = None
 
     def log(self, msg: str) -> str:
         logger.info(f'{self} {msg}')
         return msg
@@ -153,14 +161,15 @@
     ctntype_id: Optional[str] = None  # 箱型
     is_applied: Optional[bool] = None  # 是否已申请
     is_printed: Optional[bool] = None  # 是否已打印
     is_taken: Optional[bool] = None  # 是否已提箱
     order_guid: Optional[str] = None  # 完成的订单号
     ctn_data: Optional[dict] = {}  # 服务器返回的集装箱数据
     barcode_data: Optional[dict] = {}  # 条码信息
+    barcode: Optional[str] = None
     desc: Optional[str] = ''
 
 
 class CtnListData(BaseModel):
     data: Optional[List[CtnInfo]] = []
 
 
@@ -170,37 +179,26 @@
     """
     ctntype_id: Optional[str] = None  # 箱型
     ctn_digit: Optional[int] = 0  # 箱量
     ctn_digit_applied: Optional[int] = 0  # 已申请量
     ctn_digit_printed: Optional[int] = 0  # 已打印量
     ctn_digit_for_apply: Optional[int] = 0  # 可申请量，未申请
     ctn_digit_for_print: Optional[int] = 0  # 可打印量，已申请未打印
-    ctn_digit_need_apply: Optional[int] = 0  # 需申请量,订单传过来的
-    is_over_apply: bool = False  # 已超出申请量，不可再申请
-
-    # is_valid = False  #
+    ctn_digit_need_apply: Optional[int] = 0  # 总申请量,订单传过来的，
+    yard_info: Optional[Dict] = {}  # 用于msk，指定堆场
 
+    # 总申请量>0 本次需申请量=总申请量-已申请量, 总申请量=0 本次申请量=箱量-可打印量
+    # 本次打印量=min(可打印量,箱量)
     def __str__(self):
         return f'{self.ctn_digit}x{self.ctntype_id.upper()}'
 
 
-class BillCtntypeDigit(BaseModel):
-    """
-    提单箱型箱量
-    """
-    ctntype_id: Optional[str] = None  # 箱型
-    ctn_digit_total: int = 0  # 总箱量
-    ctn_digit_applied: int = 0  # 已申请量
-    cnt_digit_printed: int = 0  # 已打印量
-    is_over_apply: bool = False  # 已超出申请量，不可再申请
-
-
 def convert_ctntype_tolist(ctntype_id, ctn_digit=1):
     """
-    转换箱型箱量
+    将箱型箱量字符串1x20gp;2x40gp，转化为箱型箱量列表
     @return:
     """
     ctntypedigit_list = []
     if not ctntype_id:
         return ctntypedigit_list
 
     ctntype_id = ctntype_id.upper()
@@ -225,126 +223,142 @@
         ctntypedigit = CtnTypeDigit()
         ctntypedigit.ctntype_id = ctntype_id
         ctntypedigit.ctn_digit = ctn_digit
         ctntypedigit_list.append(ctntypedigit)
     return ctntypedigit_list
 
 
-class TaskResult(BaseModel):
+# 检查箱型箱量是否和集装箱列表匹配
+
+
+class EirOrder(BaseModel):
     order_guid: Optional[str] = None
-    status: Optional[BillStatus] = None
-    memo: Optional[str] = None
-    vessel: Optional[str] = None  # 船名
-    voyage: Optional[str] = None  # 航次
-    ctns: List[CtnInfo] = []  # 申请的集装箱列表
-    time_stamp: int = time.time_ns()
+    task_info: Optional[EirTaskInfo] = None
+    carrier_id: Optional[Any] = None  # 船公司
+    bill_no: Optional[Any] = None  # 提单号
+    booking_no: Optional[Any] = None  # 订舱号
+    cyname: Optional[str] = None  # 推荐堆场
 
+    ctntype_id: Optional[str] = ''  # 箱型
+    ctn_digit: Optional[int] = 0  # 箱量
+    apply_ctntypedigit: Optional[str] = ''  # 需一次性申请的箱型箱量
 
-class BillInfo(BaseModel):
-    """
-    提单信息
-    """
-    carrier_id: Optional[str] = None  # 船公司
-    bookingagent_id: Optional[str] = None  # 代理
-    bill_no: Optional[str] = None  # 提单
-    booking_no: Optional[str] = None  # 订舱号
-    vessel: Optional[str] = None  # 船名
-    voyage: Optional[str] = None  # 航次
-    rel_vessel: Optional[str] = None
-    rel_voyage: Optional[str] = None
-    vessel_id: Optional[str] = None
-    status: BillStatus = BillStatus.unknown
-    info: dict = {}
+    begin_time: Optional[datetime] = datetime.strptime(datetime.strftime(datetime.now(), '%Y-%m-%d %H:%M:%S'),
+                                                       '%Y-%m-%d %H:%M:%S')  # 刷箱开始时间
+    end_time: Optional[datetime] = datetime.strptime(
+        datetime.strftime(datetime.now() + timedelta(hours=4), '%Y-%m-%d %H:%M:%S'),
+        '%Y-%m-%d %H:%M:%S')  # 刷箱结束时间
 
+    bookingagent_id: Optional[Any] = None  # 账号对应的订舱代理
+    vessel: Optional[Any] = None  # 船名
+    voyage: Optional[Any] = None  # 航次
 
-class EirOrder(EirTaskInfo):
-    booking_no: Optional[str] = None  # 提单号
-    bill_info: Optional[BillInfo] = BillInfo()  # 提单信息
-    ctns: List[CtnInfo] = []  # 集装箱列表
-    apply_ctns: List[CtnInfo] = []  # 申请的集装箱列表
-    print_ctns: List[CtnInfo] = []
     ctntypedigit_list: List[CtnTypeDigit] = []  # eir订单箱型箱量
-    bill_ctntypedigit_dict: Dict[str, BillCtntypeDigit] = {}  # 提单箱型箱量
     is_canceled: bool = False
     is_disabled: bool = False
     is_completed: bool = False
 
+    internal_ctns: List[CtnInfo] = []  # 集装箱列表
+
+    def check_ctntype_id(self, ctntype_id, ctn_list):
+        set1 = set(map(lambda ctn: ctn.ctntype_id, ctn_list))
+        ctntypedigit_list = convert_ctntype_tolist(ctntype_id)
+        set2 = set(map(lambda ctntypedigit: ctntypedigit.ctntype_id, ctntypedigit_list))
+
+        if set2 - set1 and len(set1) == 1 and len(set2) == 1:
+            ctntype_id = ctntype_id.replace(list(set2)[0], list(set1)[0])
+            return ResponseData(code=RespType.task_success, msg=f'{self} 箱型成功转化', data=ctntype_id)
+        elif set2 - set1:
+            return ResponseData(code=RespType.task_failed, msg=f'{self} 放舱列表中未找到对应箱型，请联系一代')
+        else:
+            return ResponseData(code=RespType.task_success, msg=f'{self} 箱型匹配', data=ctntype_id)
+
+    def __str__(self):
+        return f'{self.carrier_id} {self.bill_no} {self.order_guid if self.order_guid else ""}'
+
+    @property
+    def ctns(self) -> List[CtnInfo]:
+        return self.internal_ctns
+
+    @ctns.setter
+    def ctns(self, value: List[CtnInfo]):
+        self.internal_ctns = value
+        ctntypedigit_dict = {}
+
+        # 指定箱型箱量模式
+        if self.ctntype_id:
+            ctntypedigit_list = convert_ctntype_tolist(self.ctntype_id, self.ctn_digit)
+            ctntypedigit_dict = {x.ctntype_id: x for x in ctntypedigit_list}
+
+            # cma统一申请模式,更新各箱型 ctn_digit_need_apply
+            if self.apply_ctntypedigit:
+                apply_ctntypedigit_list = convert_ctntype_tolist(self.apply_ctntypedigit)
+                for item in apply_ctntypedigit_list:
+                    ctntypedigit = ctntypedigit_dict.get(item.ctntype_id)
+                    if ctntypedigit:
+                        ctntypedigit.ctn_digit_need_apply = item.ctn_digit
+                    else:
+                        ctntypedigit_dict.update({item.ctntype_id: item})
+
+        # 更新各箱型已申请量、已打印量
+        for ctn in value:
+            ctntypedigit = ctntypedigit_dict.get(ctn.ctntype_id)
+            if not ctntypedigit:
+                ctntypedigit = CtnTypeDigit()
+                ctntypedigit.ctntype_id = ctn.ctntype_id
+                ctntypedigit_dict.update({ctn.ctntype_id: ctntypedigit})
+            if ctn.is_applied:
+                ctntypedigit.ctn_digit_applied += 1
+            if ctn.is_printed:
+                ctntypedigit.ctn_digit_printed += 1
+
+        for item in ctntypedigit_dict.values():
+
+            # 整单模式,不需要申请
+            if not self.ctntype_id:
+                item.ctn_digit_for_print = item.ctn_digit_applied - item.ctn_digit_printed
+                item.ctn_digit_need_apply = 0
+            # 指定箱型箱量模式
+            else:
+                # 本次打印量=min(已申请量-已打印量,箱量)
+                item.ctn_digit_for_print = min(item.ctn_digit_applied - item.ctn_digit_printed, item.ctn_digit)
+
+                # 总申请量=0 本次申请量=箱量-可打印量
+                if item.ctn_digit_need_apply == 0 and item.ctn_digit > item.ctn_digit_applied - item.ctn_digit_printed:
+                    item.ctn_digit_for_apply = item.ctn_digit - item.ctn_digit_applied + item.ctn_digit_printed
+                # 总申请量>0 本次需申请量=总申请量-已申请量
+                elif item.ctn_digit_need_apply > item.ctn_digit_applied:
+                    item.ctn_digit_for_apply = item.ctn_digit_need_apply - item.ctn_digit_applied
+
+        self.ctntypedigit_list = list(ctntypedigit_dict.values())
+
     @property
     def status(self) -> BillStatus:
         if self.is_canceled or self.is_canceled:
             return BillStatus.canceled
         elif not self.bill_info or not self.bill_info.voyage:
             return BillStatus.unknown
         elif self.ctns and self.ctns_for_print():
             return BillStatus.printed
         elif self.ctns and self.ctns_for_apply():
             return BillStatus.applied
         else:
             return BillStatus.inited
 
-    def __init__(self, **data: Any):
-        super().__init__(**data)
-        self.convert_ctntypedigit()
-
     def check_completed(self):
         """
-        @todo 看看还需要吗？
-        检查是否已完成，订单量 < 已打印量
-        @return:
-        """
-        if self.ctntypedigit_list:
-            for item in self.ctntypedigit_list:
-                if item.ctn_digit_need_apply > item.ctn_digit_printed or item.ctn_digit > item.ctn_digit_printed or 0:
-                    return False
-            return True
-        else:
-            ctns = list(filter(lambda x: not x.is_printed, self.ctns))
-            return not ctns
-
-    def bill_summary(self):
-        """
-        获得集装箱列表后，箱型箱量统计
-        @return:
-        """
-        self.ctns.sort(key=lambda x: x.ctntype_id)
-        cur = None
-        for ctn in self.ctns:
-            if not cur or cur.ctntype_id != ctn.ctntype_id:
-                cur = self.bill_ctntypedigit_dict.get(ctn.ctntype_id)
-                if not cur:
-                    cur = BillCtntypeDigit()
-                    cur.ctntype_id = ctn.ctntype_id
-                    self.bill_ctntypedigit_dict.update({cur.ctntype_id: cur})
-                else:
-                    cur.ctn_digit_total = cur.ctn_digit_applied = cur.cnt_digit_printed = 0
-            cur.ctn_digit_total += 1
-            cur.ctn_digit_applied += 1 if ctn.is_applied else 0
-            cur.cnt_digit_printed += 1 if ctn.is_printed else 0
-
-    def convert_ctntypedigit(self):
-        """
-        转换箱型箱量
-        @return:
+        不需要申请，不需要打印
         """
-        self.ctntypedigit_list = convert_ctntype_tolist(self.ctntype_id, self.ctn_digit)
-        # 统一申请模式
-        if self.apply_ctntypedigit:
-            apply_ctntypedigit_list = convert_ctntype_tolist(self.apply_ctntypedigit)
-            for item in apply_ctntypedigit_list:
-                lst = list(filter(lambda x: x.ctntype_id == item.ctntype_id, self.ctntypedigit_list))
-                if lst:
-                    ctntypedigit = lst[0]
-                    ctntypedigit.ctn_digit_need_apply = item.ctn_digit
+        return not (self.need_apply or self.need_print)
 
     def ctns_for_apply(self):
         """
         获得待申请集装箱清单，整单则返回所有，按箱型则返回该箱型实际需求量
         @return:
         """
-        self.summary()
         if self.ctntypedigit_list:
             ctns = []
             for ctntypedigit in self.ctntypedigit_list:
                 if ctntypedigit.ctn_digit_for_apply:
                     ctn_list = list(
                         filter(lambda x: x.ctntype_id == ctntypedigit.ctntype_id and not x.is_applied,
                                self.ctns))
@@ -354,15 +368,14 @@
             return list(filter(lambda x: not x.is_applied, self.ctns))
 
     def ctns_for_print(self) -> List[CtnInfo]:
         """
         获得待打印集装箱清单，整单则返回所有，按箱型则返回该箱型实际需求量
         @return:
         """
-        self.summary()
         if self.ctntypedigit_list:
             ctns = []
             for ctntypedigit in self.ctntypedigit_list:
                 if ctntypedigit.ctn_digit_for_print:
                     ctn_list = list(
                         filter(lambda x: x.ctntype_id == ctntypedigit.ctntype_id and x.is_applied and not x.is_printed,
                                self.ctns))
@@ -373,84 +386,49 @@
 
     @property
     def need_apply(self):
         """
         判断本单是否需要申请
         @return:
         """
-        self.summary()
         if self.ctntypedigit_list:
-            for item in self.ctntypedigit_list:
-                if item.ctn_digit_for_apply > 0:
-                    return True
-            return False
+            return bool(list(filter(lambda x: x.ctn_digit_for_apply, self.ctntypedigit_list)))
         else:
             return bool(list(filter(lambda x: not x.is_applied, self.ctns)))
 
     @property
     def need_print(self):
         """
         判断本单是否需要打印,未打印的 大于 未申请的 大于 0
         @return:
         """
-        self.summary()
         if self.ctntypedigit_list:
-            for item in self.ctntypedigit_list:
-                if item.ctn_digit_for_print > 0:
-                    return True
+            return bool(list(filter(lambda x: x.ctn_digit_for_print, self.ctntypedigit_list)))
         else:
             return bool(list(filter(lambda x: x.is_applied and not x.is_printed, self.ctns)))
 
     @property
     def order_ctntype_digit_describe(self):
         """
         订单箱型箱量描述
         @return:
         """
         return self.ctntypedigit
 
-    def summary(self):
-        """
-        获得集装箱列表后，计算各箱型需申请、打印量
-        @return:
-        """
-        # 除了cma,msk,hpl，需要申请后才能获得集装箱列表，其他船公司都可以获取集装箱列表
-        # msk 以申请为准
-        # 其他船公司，ctntypedigit_list中的值，必须在集装箱列表中，否则就清空ctntypedigit_list，整票刷
-        self.bill_summary()
-
-        if self.carrier_id.upper() not in ['CMA-EIR', 'MSK-EIR', 'HPL-EIR'] and self.ctntypedigit_list:
-            order_ctntype_set = set(map(lambda x: x.ctntype_id, self.ctntypedigit_list))
-            bill_ctntype_set = set(map(lambda x: x.ctntype_id, self.ctns))
-            if not bill_ctntype_set >= order_ctntype_set:
-                self.ctntypedigit_list = []
-
-        for item in self.ctntypedigit_list:
-            bill_ctntypedigit = self.bill_ctntypedigit_dict.get(item.ctntype_id)
-            # item.is_valid = bill_ctntypedigit is not None
-            # if item.is_valid:
-            item.ctn_digit_applied = 0 if not bill_ctntypedigit else bill_ctntypedigit.ctn_digit_applied
-            item.ctn_digit_printed = 0 if not bill_ctntypedigit else bill_ctntypedigit.cnt_digit_printed
-            # 可申请量=订单量-已申请量
-            # 可打印量=min（订单量，已申请量-已打印量)
-            item.ctn_digit_for_print = min(item.ctn_digit_applied - item.ctn_digit_printed, item.ctn_digit)
-
-            if item.ctn_digit_need_apply:
-                item.ctn_digit_for_apply = item.ctn_digit_need_apply - item.ctn_digit_applied if item.ctn_digit_need_apply > item.ctn_digit_applied else 0
-            else:
-                item.ctn_digit_for_apply = item.ctn_digit - item.ctn_digit_for_print if item.ctn_digit > item.ctn_digit_for_print else 0
-
 
 class AccountInfo(BaseModel):
     carrier_id: Optional[str] = None  # 船公司
     account: Optional[str] = None
     password: Optional[str] = None
     bookingagent_id: Optional[str] = None
     info: dict = {}
 
+    def __str__(self):
+        return f'{self.carrier_id} {self.account}'
+
 
 class SpotParams(BaseModel):
     session_data: Optional[SessionData] = None
     carrier_id: Optional[str] = None
     from_port_id: Optional[str] = None  # 起运港
     to_port_id: Optional[str] = None  # 目的港
     ctntype_id: Optional[str] = None  # 箱型
@@ -492,21 +470,27 @@
 
 
 class ParamsCheckAccount(BaseModel):
     carrier_id: str = ''  # 船公司
     account: str = ''  # 账号
     password: str = ''  # 密码
 
+    def __str__(self):
+        return f'{self.carrier_id}/{self.account}'
+
 
 class LoginParams(BaseModel):
     carrier_id: str = ''  # 船公司
     account: str = ''  # 账号
     password: str = ''  # 密码
     proxy_id: Optional[str] = None
 
+    def __str__(self):
+        return f'{self.carrier_id}/{self.account} {self.proxy_id if self.proxy_id else ""}'
+
 
 class RespSessionException(Exception):
     def __init__(self, code, msg, detail=None):
         self.code = code
         self.msg = msg
         self.detail = detail
```

### Comparing `eirStru-0.2.99/eirStru/eirjob_intf.py` & `eirStru-0.3.0/eirStru/eirjob_intf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,77 @@
-import requests
 from aiohttp import ClientSession
+
 from eirStru import *
 
 
-class EirParams(BaseModel):
-    session: Optional[SessionData] = None
+class EirTaskInfoParams(BaseModel):
+    session_data: Optional[SessionData] = None
+    task_info: Optional[EirTaskInfo] = None
+
+
+class EirOrderParams(BaseModel):
+    session_data: Optional[SessionData] = None
     order: Optional[EirOrder] = None
 
 
 class JobIntf:
     def __init__(self, host):
         self.host = host
 
     async def do_eir(self, session_data: SessionData, order: EirOrder) -> ResponseData:
         return await self.call_eir_job('do_eir', session_data, order)
 
-    async def get_bill_info(self, session_data: SessionData, order: EirOrder) -> ResponseData:
-        resp = await self.call_eir_job('get_bill_info', session_data, order)
-        if resp.code == RespType.task_success:
-            bill_info = BillInfo(**resp.data)
-            bill_info.bookingagent_id = session_data.bookingagent_id
-            resp.data = bill_info
-            return resp
-        return resp
+    async def get_bill_info(self, session_data: SessionData, task_info: EirTaskInfo) -> ResponseData:
+        url = f'{self.host}/get_bill_info/'
+        data = EirTaskInfoParams(session_data=session_data, task_info=task_info)
+
+        headers = {
+            'accept': 'application/json',
+            'Content-Type': 'application/json',
+        }
+        try:
+            async with ClientSession() as cs:
+                async with cs.post(url, headers=headers, data=data.model_dump_json(), verify_ssl=False) as resp:
+                    r_json = await resp.json()
+                    if r_json.get('data'):
+                        r_json['data'] = EirOrder(**r_json['data'])
+                    return ResponseData(**r_json)
+        except Exception as e:
+            return ResponseData(code=RespType.task_failed, message=f'{task_info}:{e}')
 
     async def get_ctn_list(self, session_data: SessionData, order: EirOrder) -> ResponseData:
         if not order.booking_no:
             logger.error(f'{order} 没有 bookingno')
             return ResponseData(code=RespType.task_failed, msg=f'{order} 没有 bookingno')
         resp = await self.call_eir_job('get_ctn_list', session_data, order)
         if resp.code == RespType.task_success:
             resp.data = list(map(lambda x: CtnInfo(**x), resp.data))
         return resp
 
+    async def get_apply_cy(self, session_data: SessionData, order: EirOrder) -> ResponseData:
+        if not order.booking_no:
+            logger.error(f'{order} 没有 bookingno')
+            return ResponseData(code=RespType.task_failed, msg=f'{order} 没有 bookingno')
+        return await self.call_eir_job('get_apply_cy', session_data, order)
+
     async def apply_eir(self, session_data: SessionData, order: EirOrder) -> ResponseData:
         if not order.booking_no:
             logger.error(f'{order} 没有 bookingno')
             return ResponseData(code=RespType.task_failed, msg=f'{order} 没有 bookingno')
         return await self.call_eir_job('apply_eir', session_data, order)
 
     async def print_eir(self, session_data: SessionData, order: EirOrder) -> ResponseData:
         if not order.booking_no:
             logger.error(f'{order} 没有 bookingno')
             return ResponseData(code=RespType.task_failed, msg=f'{order} 没有 bookingno')
         return await self.call_eir_job('print_eir', session_data, order)
 
     async def call_eir_job(self, job_type, session_data: SessionData, order: EirOrder) -> ResponseData:
         url = f'{self.host}/{job_type}/'
-        data = EirParams(session=session_data, order=order)
+        data = EirOrderParams(session_data=session_data, order=order)
         # data = {
         #     'session': session_data.model_dump(),
         #     'order': order.model_dump()
         # }
         headers = {
             'accept': 'application/json',
             'Content-Type': 'application/json',
@@ -66,16 +86,14 @@
 
     async def quote_spot(self, params: SpotParams):
         url = f'{self.host}/quote_spot'
         headers = {
             'accept': 'application/json',
             'Content-Type': 'application/json',
         }
-        response = requests.post(url, headers=headers, data=params.model_dump_json(), verify=False)
-        return ResponseData(**response.json())
-        # try:
-        #     async with ClientSession() as cs:
-        #         async with cs.post(url, headers=headers, data=params.model_dump_json(), verify_ssl=False) as resp:
-        #             r_json = await resp.json()
-        #             return ResponseData(**r_json)
-        # except Exception as e:
-        #     return ResponseData(code=RespType.task_failed, message=f'{e}')
+        try:
+            async with ClientSession() as cs:
+                async with cs.post(url, headers=headers, data=params.model_dump_json(), verify_ssl=False) as resp:
+                    r_json = await resp.json()
+                    return ResponseData(**r_json)
+        except Exception as e:
+            return ResponseData(code=RespType.task_failed, message=f'{e}')
```

### Comparing `eirStru-0.2.99/eirStru/eirlogin_intf.py` & `eirStru-0.3.0/eirStru/eirlogin_intf.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import aiohttp
 from aiohttp import ClientSession
 
 from eirStru import *
 
 
 class LoginIntf:
     def __init__(self, host):
@@ -16,18 +15,28 @@
         headers = {
             'accept': 'application/json',
             'Content-Type': 'application/json',
         }
 
         data = params.model_dump_json()
 
+        # try:
+        #     resp = httpx.post(url, params=data, headers=headers, verify=False)
+        #     r_json = resp.json()
+        #     if r_json.get('data'):
+        #         r_json['data'] = AccountInfo(**r_json['data'])
+        #     return ResponseData(**r_json)
+        # except Exception as e:
+        #     logger.info(e)
         try:
             async with ClientSession() as cs:
                 async with cs.post(url, headers=headers, data=data, verify_ssl=False) as resp:
                     r_json = await resp.json()
+                    if r_json.get('data'):
+                        r_json['data'] = AccountInfo(**r_json['data'])
                     return ResponseData(**r_json)
         except Exception as e:
             return ResponseData(code=RespType.task_failed, message=f'{e}')
 
     async def login(self, params: LoginParams) -> ResponseData:
         """
         检查账号
@@ -62,14 +71,16 @@
         params.bookingagent_id = bookingagent_id
         params.sub_code = sub_code
 
         try:
             async with ClientSession() as cs:
                 async with cs.post(url, headers=headers, data=params.model_dump_json(), verify_ssl=False) as resp:
                     r_json = await resp.json()
+                    if r_json.get('data'):
+                        r_json['data'] = SessionData(**r_json['data'])
                     return ResponseData(**r_json)
         except Exception as e:
             return ResponseData(code=RespType.task_failed, message=f'{e}')
 
     async def return_session(self, resp_type: RespType, session_data: SessionData) -> ResponseData:
         url = f'{self.host}/return_session/'
         headers = {
```

### Comparing `eirStru-0.2.99/eirStru/redis_utils.py` & `eirStru-0.3.0/eirStru/redis_utils.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.99/eirStru/utils.py` & `eirStru-0.3.0/eirStru/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,16 +31,15 @@
 
 def is_json(ss):
     """
     判断是否json
     """
     try:
         return json.loads(ss)
-    except Exception as e:
-        logger.error(e)
+    except:
         return
 
 
 def get_guid():
     return uuid.uuid4().hex
```

### Comparing `eirStru-0.2.99/eirStru/wx_push.py` & `eirStru-0.3.0/eirStru/wx_push.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.99/eirStru.egg-info/PKG-INFO` & `eirStru-0.3.0/eirStru.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eirStru
-Version: 0.2.99
+Version: 0.3.0
 Summary: My short description for my project.
 Home-page: https://github.com/me/myproject
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `eirStru-0.2.99/setup.py` & `eirStru-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'eirStru'
 DESCRIPTION = 'My short description for my project.'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'me@example.com'
 AUTHOR = 'Awesome Soul'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.2.99'
+VERSION = '0.3.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

