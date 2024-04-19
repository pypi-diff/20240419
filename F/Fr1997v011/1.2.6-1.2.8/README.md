# Comparing `tmp/Fr1997v011-1.2.6.tar.gz` & `tmp/Fr1997v011-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fr1997v011-1.2.6.tar", last modified: Thu Apr 18 02:38:06 2024, max compression
+gzip compressed data, was "Fr1997v011-1.2.8.tar", last modified: Fri Apr 19 12:37:53 2024, max compression
```

## Comparing `Fr1997v011-1.2.6.tar` & `Fr1997v011-1.2.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 02:38:06.719171 Fr1997v011-1.2.6/
-drwxrwxrwx   0        0        0        0 2024-04-18 02:38:06.712171 Fr1997v011-1.2.6/Fr1997v011.egg-info/
--rw-rw-rw-   0        0        0      182 2024-04-18 02:38:06.000000 Fr1997v011-1.2.6/Fr1997v011.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-04-18 02:38:06.000000 Fr1997v011-1.2.6/Fr1997v011.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 02:38:06.000000 Fr1997v011-1.2.6/Fr1997v011.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-18 02:38:06.000000 Fr1997v011-1.2.6/Fr1997v011.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-04-18 02:38:06.000000 Fr1997v011-1.2.6/Fr1997v011.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.2.6/LICENSE
--rw-rw-rw-   0        0        0      182 2024-04-18 02:38:06.718171 Fr1997v011-1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0      773 2024-04-17 10:09:41.000000 Fr1997v011-1.2.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 02:38:06.714170 Fr1997v011-1.2.6/fr1997_mode/
--rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.2.6/fr1997_mode/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:38:06.716171 Fr1997v011-1.2.6/fr1997_mode/mode_func/
--rw-rw-rw-   0        0        0       29 2023-10-09 02:29:18.000000 Fr1997v011-1.2.6/fr1997_mode/mode_func/__init__.py
--rw-rw-rw-   0        0        0   130107 2024-04-17 11:21:03.000000 Fr1997v011-1.2.6/fr1997_mode/mode_func/all_func.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:38:06.717171 Fr1997v011-1.2.6/fr1997_mode/mode_static/
--rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.2.6/fr1997_mode/mode_static/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-18 02:38:06.719171 Fr1997v011-1.2.6/setup.cfg
--rw-rw-rw-   0        0        0      322 2024-04-17 10:09:41.000000 Fr1997v011-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 12:37:53.243040 Fr1997v011-1.2.8/
+drwxrwxrwx   0        0        0        0 2024-04-19 12:37:53.237040 Fr1997v011-1.2.8/Fr1997v011.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-04-19 12:37:53.000000 Fr1997v011-1.2.8/Fr1997v011.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-04-19 12:37:53.000000 Fr1997v011-1.2.8/Fr1997v011.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 12:37:53.000000 Fr1997v011-1.2.8/Fr1997v011.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-19 12:37:53.000000 Fr1997v011-1.2.8/Fr1997v011.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-04-19 12:37:53.000000 Fr1997v011-1.2.8/Fr1997v011.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.2.8/LICENSE
+-rw-rw-rw-   0        0        0      182 2024-04-19 12:37:53.242040 Fr1997v011-1.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2024-04-19 12:37:52.000000 Fr1997v011-1.2.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 12:37:53.238040 Fr1997v011-1.2.8/fr1997_mode/
+-rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.2.8/fr1997_mode/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 12:37:53.240040 Fr1997v011-1.2.8/fr1997_mode/mode_func/
+-rw-rw-rw-   0        0        0       29 2023-10-09 02:29:18.000000 Fr1997v011-1.2.8/fr1997_mode/mode_func/__init__.py
+-rw-rw-rw-   0        0        0   145627 2024-04-19 12:37:49.000000 Fr1997v011-1.2.8/fr1997_mode/mode_func/all_func.py
+drwxrwxrwx   0        0        0        0 2024-04-19 12:37:53.241040 Fr1997v011-1.2.8/fr1997_mode/mode_static/
+-rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.2.8/fr1997_mode/mode_static/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-19 12:37:53.243040 Fr1997v011-1.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      322 2024-04-19 12:37:49.000000 Fr1997v011-1.2.8/setup.py
```

### Comparing `Fr1997v011-1.2.6/LICENSE` & `Fr1997v011-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `Fr1997v011-1.2.6/README.md` & `Fr1997v011-1.2.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ```sh
 python setup.py sdist
 ```
 
 ### （本地）安装包
 
 ```sh
-pip install dist/Fr1997v011-1.2.6.tar.gz
+pip install dist/Fr1997v011-1.2.8.tar.gz
 ```
 
 ### 下载包
 
 ```sh
 pip install Fr1997v011
 ```
```

### Comparing `Fr1997v011-1.2.6/fr1997_mode/mode_func/all_func.py` & `Fr1997v011-1.2.8/fr1997_mode/mode_func/all_func.py`

 * *Files 4% similar despite different names*

```diff
@@ -505,19 +505,350 @@
             'http': ip
         }
         return proxies
 
 
 # 飞书
 class Feishu:
+    """
+        组成：                             app_token        table_id        views
+        https://bchje44bsl.feishu.cn/base/XXXXXXXXXXXXXXXX?table=XXXXXXXXX&view=XXXXXXXX
+    """
+
     def __init__(self):
         # 飞书
         self.feishu_base_url = config_dict['feishu']['fs_base_url']
         self.feishu_bot_url = config_dict['feishu']['fs_bot_url']  # 飞书机器人
         self.feishu_token_url = config_dict['feishu']['fs_token_url']  # 飞书token
+        self.feishu_app_url = config_dict['feishu']['fs_app_url']  # 飞书app
+
+        # 翻页返回
+        self.ret_data_all = []
+
+    # 获取应用token token的过期时间为2小时
+    def get_token(self, app_name):
+        key = f'feishu_token_{app_name}_v3'
+        tenant_access_token = cache_get(key)
+        if not tenant_access_token:
+            r = requests.post(self.feishu_token_url, data=config_dict['feishu']['apps'][app_name])
+            tenant_access_token = r.json()["tenant_access_token"]
+            cache_set(key, tenant_access_token, 1800)  # 缓存半小时
+        return tenant_access_token
+
+    # 基础请求头
+    def base_headers(self, app_name):
+        return {
+            'Authorization': f"Bearer {self.get_token(app_name)}",
+        }
+
+    # 获取 app_token下 所有 table
+    def get_all_table(self, app_name, app_token):
+        url = f'{mode_feishu.feishu_app_url}{app_token}/tables'
+        res = requests.get(url=url, headers=self.base_headers(app_name))
+        if res.status_code == 200:
+            data_data = res.json()
+            code = data_data.get('code')
+            msg = data_data.get('msg')
+            data = data_data.get('data')
+            if code == 0 and msg == "success" and data:
+                items = data['items']
+                return items
+            else:
+                print("内容获取失败")
+        else:
+            print("状态码 错误")
+
+    # 创建 表 table
+    def create_new_table(self, app_name, app_token, table_name):
+        url = f"{mode_feishu.feishu_app_url}{app_token}/tables"
+        data = {
+            "table": {
+                "name": table_name
+            }
+        }
+        res = requests.post(url=url, headers=self.base_headers(app_name), data=json.dumps(data))
+        if res.status_code == 200:
+            data_data = res.json()
+            code = data_data.get('code')
+            msg = data_data.get('msg')
+            data = data_data.get('data')
+            if code == 0 and msg == "success" and data:
+                return 1
+
+    # 删除 表
+    def del_table(self, app_name, app_token, table_id):
+        url = f"{mode_feishu.feishu_app_url}{app_token}/tables/{table_id}"
+        res = requests.delete(url=url, headers=self.base_headers(app_name))
+        if res.status_code == 200:
+            data_data = res.json()
+            code = data_data.get('code')
+            msg = data_data.get('msg')
+            data = data_data.get('data')
+            if code == 0 and msg == "success" and data:
+                return 1
+
+    # 表 增加字段
+    def create_table_fields_test(self, app_name, app_token, table_id, field_update):
+        """
+        table管理
+            1：多行文本
+            2：数字
+                整数	"0"
+                保留1位小数	"0.0"
+                保留2位小数	"0.00"
+                保留3位小数	"0.000"
+                保留4位小数	"0.0000"
+                千分位	"1,000"
+                千分位（小数点）	"1,000.00"
+                百分比	"%"
+                百分比（小数点）	"0.00%"
+                人民币	"¥"
+                人民币（小数点）	"¥0.00"
+                美元	"$"
+                美元（小数点）	"$0.00"
+            3：单选
+            4：多选
+            5：日期
+                2021/01/30	"yyyy/MM/dd"
+                2021/01/30 14:00	"yyyy/MM/dd HH:mm"
+                2021-01-30	"yyyy-MM-dd"
+                2021-01-30 14:00	"yyyy-MM-dd HH:mm"
+                01-30	"MM-dd"
+                01/30/2021	"MM/dd/yyyy"
+                30/01/2021	"dd/MM/yyyy"
+            7：复选框
+            11：人员
+            15：超链接
+            17：附件
+            18：关联
+            20：公式
+            21：双向关联
+            1001：创建时间
+            1002：最后更新时间
+            1003：创建人
+            1004：修改人
+            1005：自动编号
+            13：电话号码
+            22：地理位置
+
+            -- 示例
+            field_update = [
+                # {"field_name": '普通文本', "type": 1},  # 添加普通文本
+                # {"field_name": '数字-整数', "type": 2, "property": {"formatter": "0"}},  # 添加数字 整形
+                # {"field_name": '数字-浮点', "type": 2, "property": {"formatter": "0.00"}},  # 添加数字 浮点数
+                {"field_name": '日期', "type": 5},  # 日期
+            ]
+            mode_feishu.create_table_fields_test(fapp_name, fapp_token, 'tblJyCmlB0Ly6yvr', field_update)
+
+        """
+        url = f'{mode_feishu.feishu_app_url}{app_token}/tables/{table_id}/fields'
+        for i in field_update:
+            res = requests.post(url=url, headers=self.base_headers(app_name), data=json.dumps(i))
+            if res.status_code == 200:
+                ret_data = res.json()
+                code = ret_data.get("code")
+                msg = ret_data.get("msg")
+                if code == 0 and msg == 'success':
+                    print(app_token, "添加字段 成功")
+                else:
+                    print(app_token, "添加字段 添加失败")
+            else:
+                print(app_token, "添加字段 状态码错误")
+
+            time.sleep(1)
+
+    # 表 修改字段
+    def update_table_field(self, app_name, app_token, table_id, field_id, field_dict):
+        url = f"{mode_feishu.feishu_app_url}{app_token}/tables/{table_id}/fields/{field_id}"
+        requests.put(url=url, headers=self.base_headers(app_name), data=json.dumps(field_dict))
+
+    # 表 修改字段 批量
+    def update_table_fields_test(self, app_name, app_token, table_id, field_update):
+        """
+            field_update = [
+                # {"old_field_name": '多行文本', "field_name": '多行文本1', "type": 1},  # 添加普通文本
+                {"old_field_name": '多行文本1', "field_name": '测试数据', "type": 2, "property": {"formatter": "0"}},  # 添加数字 整形
+            ]
+            mode_feishu.update_table_fields_test(app_name, app_token, 'tblJyCmlB0Ly6yvr', field_update)
+        """
+        # 获取table所有字段
+        fields = self.get_table_fields(app_name, app_token, table_id)
+        if fields:
+            # 整理数据
+            fields_dict = {}
+            for f in fields:
+                fields_dict[f['field_name']] = f['field_id']
+
+            # 获取字段对应的 field_id 并更新
+            for i in field_update:
+                old_field_name = i['old_field_name']
+                field_id = fields_dict.get(old_field_name)
+                url = f"{mode_feishu.feishu_app_url}{app_token}/tables/{table_id}/fields/{field_id}"
+                del i['old_field_name']
+                res = requests.put(url=url, headers=self.base_headers(app_name), data=json.dumps(i))
+                if res.status_code == 200:
+                    ret_data = res.json()
+                    code = ret_data.get("code")
+                    msg = ret_data.get("msg")
+                    if code == 0 and msg == 'success':
+                        print(app_token, "修改字段 成功")
+                    elif msg == 'DataNotChange':
+                        print(app_token, "修改字段 无需修改")
+                    else:
+                        print(app_token, "修改字段 修改失败")
+                else:
+                    print(app_token, "修改字段 状态码错误")
+                time.sleep(1)
+
+    # 表 创建+修改字段
+    def create_table_and_fields(self, app_name, app_token, table_name, dct=0, fields_create=None):
+        """
+            fields_create = [
+            {"field_name": '普1', "type": 1},  # 添加普通文本
+            {"field_name": '数字-整数', "type": 2, "property": {"formatter": "0"}},  # 添加数字 整形
+            {"field_name": '日期', "type": 5},  # 日期
+        ]
+        mode_feishu.create_table_and_fields(fapp_name, fapp_token, 'sada', dct=1, fields_create=fields_create)
+        """
+        # 获取当前应用存在相同表
+        all_table = self.get_all_table(app_name, app_token)
+        for at in all_table:
+            if at['name'] == table_name:
+                if dct == 0:
+                    print("存在相同表 不创建")
+                    return
+                else:
+                    self.del_table(app_name, app_token, at['table_id'])
+                    time.sleep(1)
+        # 创建表
+        self.create_new_table(app_name, app_token, table_name)
+
+        # 获取字段
+        all_table = self.get_all_table(app_name, app_token)
+        for at in all_table:
+            if at['name'] == table_name:
+                table_id = at['table_id']
+                fields = self.get_table_fields(app_name, app_token, table_id)
+                if fields_create:
+                    # 要对第一个字段进行修改
+                    self.update_table_field(app_name, app_token, table_id, fields[0]['field_id'], fields_create[0])
+                    if fields_create[1:]:
+                        self.create_table_fields_test(app_name, app_token, table_id, fields_create[1:])
+
+    # 获取 table 字段 【table有字段，视图没有】
+    def get_table_fields(self, app_name, app_token, table_id):
+        url = f'{mode_feishu.feishu_app_url}{app_token}/tables/{table_id}/fields'
+        res = requests.get(url=url, headers=self.base_headers(app_name))
+        print(res.text)
+        if res.status_code == 200:
+            data_data = res.json()
+            code = data_data.get('code')
+            msg = data_data.get('msg')
+            data = data_data.get('data')
+            if code == 0 and msg == "success" and data:
+                items = data['items']
+                return items
+            else:
+                print("内容获取失败")
+        else:
+            print("状态码 错误")
+
+    # 获取 table 视图
+    def get_table_views(self, app_name, app_token, table_id):
+        url = f'{mode_feishu.feishu_app_url}{app_token}/tables/{table_id}/views'
+        res = requests.get(url=url, headers=self.base_headers(app_name))
+        if res.status_code == 200:
+            data_data = res.json()
+            code = data_data.get('code')
+            msg = data_data.get('msg')
+            data = data_data.get('data')
+            if code == 0 and msg == "success" and data:
+                items = data['items']
+                return items
+            else:
+                print("内容获取失败")
+        else:
+            print("状态码 错误")
+
+    # 获取view数据
+    def get_table_view_info(self, app_name, app_token, table_id, view_id, page_toke=None, ret_all=None):
+        """
+        每次最多返回500个
+        :param app_token:
+        :param table_id:
+        :return:
+        """
+        if page_toke:
+            url = f'{mode_feishu.feishu_app_url}{app_token}/tables/{table_id}/records?view_id={view_id}&page_token={page_toke}'
+        else:
+            url = f'{mode_feishu.feishu_app_url}{app_token}/tables/{table_id}/records?view_id={view_id}'
+        ret_data = {
+            'code': 0,
+            'total': 0,
+            'has_more': False,
+            'page_token': "",
+            'items': []
+        }
+        res = requests.get(url=url, headers=self.base_headers(app_name))
+        if res.status_code == 200:
+            data_data = res.json()
+            code = data_data.get('code')
+            msg = data_data.get('msg')
+            data = data_data.get('data')
+            if code == 0 and msg == "success" and data:
+                page_token = data.get('page_token')
+                has_more = data.get('has_more')
+                total = data.get('total')
+                items = data.get('items')
+                if ret_all == 1:
+                    if items:
+                        self.ret_data_all += items
+                    if has_more:
+                        time.sleep(1)
+                        print("请求下一页")
+                        self.get_table_view_info(app_token, table_id, view_id, page_toke=page_token)
+                else:
+                    if items:
+                        for index, it in enumerate(items):
+                            id_id = it.get("id")
+                            record_id = it.get("record_id")
+                            fields = it.get("fields")
+                            print(index, id_id, record_id, fields)
+
+                    return {
+                        'code': 1,
+                        'total': total,
+                        'has_more': has_more,
+                        'page_token': page_token,
+                        'items': items
+                    }
+            else:
+                print("内容获取失败")
+        else:
+            print("状态码 错误")
+
+    # 新增数据 需外部限制500条
+    def add_more_view(self, app_name, app_token, table_id, add_data, ret=0):
+        records = []
+        for i in add_data:
+            records.append({'fields': i})
+        url = mode_feishu.fs_url(app_token, 'add_more', table_id=table_id)
+        data = {
+            "records": records
+        }
+        res = requests.post(url=url, headers=self.base_headers(app_name), data=json.dumps(data))
+        if res.status_code == 200:
+            data_data = res.json()
+            code = data_data.get('code')
+            msg = data_data.get('msg')
+            data = data_data.get('data')
+            if code == 0 and msg == "success" and data:
+                if ret == 1:
+                    return data
+                return 1
 
     # 飞书 机器人推送
     def feishu_send_message(self, text, WEBHOOK_URL=''):
         if WEBHOOK_URL == '':
             WEBHOOK_URL = config_dict['feishu']['fs_url']
 
         data = {
@@ -557,19 +888,21 @@
             code = data_data.get('code')
             msg = data_data.get('msg')
             data = data_data.get('data')
             if code == 0 and msg == "success" and data:
                 return 1
 
     # 飞书各种url统一
-    def fs_url(self, app_token, mode, **kwargs):
+    def fs_url(self, app_token, mode="", **kwargs):
         base_url = f'{config_dict["feishu"]["fs_app_url"]}{app_token}/'
         if mode == 'add_more':
             table_id = kwargs['table_id']
             return f'{base_url}tables/{table_id}/records/batch_create'
+        elif mode == 'tables':
+            return f'{base_url}tables'
 
 
 # 时间
 class TimeJike:
     @staticmethod
     def zero_clock(day=0):
         t2 = time.time()
@@ -3318,7 +3651,40 @@
 mode_douyin = DouyinJike()  # douyin配置
 mode_pros = ModeStatic()  # 其它函数
 mode_cos = Cos()  # cos
 mode_fr_cos = Cos(server_select='personal')  # cos 高阳
 mode_myself = MyGy()
 
 mode_pro = ModeFunc()  # main
+
+# fapp_name = 'jike_app'
+# fapp_token = 'ZOO2bktVDa1OOSsRGvCcJkXLn0b'
+# ftable_id = 'tblCevQUyQAvY4nv'
+# fview_id = 'vewe2KRJqs'
+# fields = mode_feishu.create_new_table(fapp_name, fapp_token, '群响-每日统计')
+
+
+# mode_feishu.create_table_and_fields(fapp_name, fapp_token, '群响-每日统计', dct=1)
+
+# fields_create = [
+#     {"field_name": '日期', "type": 5},  # 日期
+#     {"field_name": '手机', "type": 1},  # 添加普通文本
+#     {"field_name": '添加时间', "type": 5, "property": {"date_formatter": "yyyy/MM/dd HH:mm", "auto_fill": False}},  # 日期
+#     {"field_name": '备注', "type": 1},  # 添加普通文本
+#     {"field_name": '微信姓名', "type": 1},  # 添加普通文本
+#     {"field_name": '添加者', "type": 1},  # 添加普通文本
+#     {"field_name": '通过状态', "type": 1},  # 添加普通文本
+#     {"field_name": '加好友备注', "type": 1},  # 添加普通文本
+# ]
+# mode_feishu.create_table_and_fields(fapp_name, fapp_token, '群响-用户列表', dct=1, fields_create=fields_create)
+
+# add_data = [
+#     {
+#         "日期": int(time.time()) * 1000,
+#         "加好友次数": 1,
+#     }, {
+#         "日期": int(time.time()) * 1000,
+#         "加好友次数": 2,
+#     }
+# ]
+#
+# mode_feishu.add_more_view(fapp_name, fapp_token, 'tbloDwXrLC4Jz0be', add_data)
```

