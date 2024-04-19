# Comparing `tmp/dmk_packages-0.6.2.tar.gz` & `tmp/dmk_packages-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmk_packages-0.6.2.tar", last modified: Mon Apr 15 05:51:13 2024, max compression
+gzip compressed data, was "dmk_packages-0.6.3.tar", last modified: Fri Apr 19 03:10:36 2024, max compression
```

## Comparing `dmk_packages-0.6.2.tar` & `dmk_packages-0.6.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-04-15 05:51:13.695471 dmk_packages-0.6.2/
--rw-r--r--   0 layla      (501) staff       (20)    11347 2024-03-25 06:00:17.000000 dmk_packages-0.6.2/LICENSE
--rw-r--r--   0 layla      (501) staff       (20)     1854 2024-04-15 05:51:13.695086 dmk_packages-0.6.2/PKG-INFO
--rw-r--r--   0 layla      (501) staff       (20)     1365 2024-03-25 06:00:17.000000 dmk_packages-0.6.2/README.md
--rw-r--r--   0 layla      (501) staff       (20)      584 2024-04-15 05:48:43.000000 dmk_packages-0.6.2/pyproject.toml
--rw-r--r--   0 layla      (501) staff       (20)       38 2024-04-15 05:51:13.695564 dmk_packages-0.6.2/setup.cfg
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-04-15 05:51:13.682505 dmk_packages-0.6.2/src/
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-04-15 05:51:13.685380 dmk_packages-0.6.2/src/dmk_packages/
--rw-r--r--   0 layla      (501) staff       (20)        0 2024-03-25 06:00:17.000000 dmk_packages-0.6.2/src/dmk_packages/__init__.py
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-04-15 05:51:13.692862 dmk_packages-0.6.2/src/dmk_packages/crawler/
--rw-r--r--   0 layla      (501) staff       (20)        0 2024-03-25 06:00:17.000000 dmk_packages-0.6.2/src/dmk_packages/crawler/__init__.py
--rw-r--r--   0 layla      (501) staff       (20)     6713 2024-04-15 02:00:53.000000 dmk_packages-0.6.2/src/dmk_packages/crawler/bigkinds.py
--rw-r--r--   0 layla      (501) staff       (20)     7812 2024-04-15 02:00:53.000000 dmk_packages-0.6.2/src/dmk_packages/crawler/clien.py
--rw-r--r--   0 layla      (501) staff       (20)     6418 2024-04-15 02:00:53.000000 dmk_packages-0.6.2/src/dmk_packages/crawler/fnguide.py
--rw-r--r--   0 layla      (501) staff       (20)     2743 2024-04-15 02:00:53.000000 dmk_packages-0.6.2/src/dmk_packages/crawler/fnguide_pdf_update.py
--rw-r--r--   0 layla      (501) staff       (20)     2321 2024-04-03 06:07:52.000000 dmk_packages-0.6.2/src/dmk_packages/crawler/naver_blog.py
--rw-r--r--   0 layla      (501) staff       (20)    15349 2024-04-15 02:00:30.000000 dmk_packages-0.6.2/src/dmk_packages/crawler/naver_search_volume.py
--rw-r--r--   0 layla      (501) staff       (20)    13392 2024-04-15 05:34:36.000000 dmk_packages-0.6.2/src/dmk_packages/crawler/youtube.py
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-04-15 05:51:13.693928 dmk_packages-0.6.2/src/dmk_packages/database/
--rw-r--r--   0 layla      (501) staff       (20)        0 2024-03-25 06:00:17.000000 dmk_packages-0.6.2/src/dmk_packages/database/__init__.py
--rw-r--r--   0 layla      (501) staff       (20)     3057 2024-04-15 03:09:28.000000 dmk_packages-0.6.2/src/dmk_packages/database/database.py
--rw-r--r--   0 layla      (501) staff       (20)     1895 2024-03-25 06:00:17.000000 dmk_packages-0.6.2/src/dmk_packages/naver_datalab.py
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-04-15 05:51:13.694646 dmk_packages-0.6.2/src/dmk_packages.egg-info/
--rw-r--r--   0 layla      (501) staff       (20)     1854 2024-04-15 05:51:13.000000 dmk_packages-0.6.2/src/dmk_packages.egg-info/PKG-INFO
--rw-r--r--   0 layla      (501) staff       (20)      684 2024-04-15 05:51:13.000000 dmk_packages-0.6.2/src/dmk_packages.egg-info/SOURCES.txt
--rw-r--r--   0 layla      (501) staff       (20)        1 2024-04-15 05:51:13.000000 dmk_packages-0.6.2/src/dmk_packages.egg-info/dependency_links.txt
--rw-r--r--   0 layla      (501) staff       (20)       41 2024-04-15 05:51:13.000000 dmk_packages-0.6.2/src/dmk_packages.egg-info/requires.txt
--rw-r--r--   0 layla      (501) staff       (20)       13 2024-04-15 05:51:13.000000 dmk_packages-0.6.2/src/dmk_packages.egg-info/top_level.txt
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-19 03:10:36.699931 dmk_packages-0.6.3/
+-rw-r--r--   0 tommie     (501) staff       (20)    11347 2024-04-04 04:45:57.000000 dmk_packages-0.6.3/LICENSE
+-rw-r--r--   0 tommie     (501) staff       (20)     1854 2024-04-19 03:10:36.699661 dmk_packages-0.6.3/PKG-INFO
+-rw-r--r--   0 tommie     (501) staff       (20)     1365 2024-04-04 04:45:57.000000 dmk_packages-0.6.3/README.md
+-rw-r--r--   0 tommie     (501) staff       (20)      584 2024-04-19 03:08:25.000000 dmk_packages-0.6.3/pyproject.toml
+-rw-r--r--   0 tommie     (501) staff       (20)       38 2024-04-19 03:10:36.699988 dmk_packages-0.6.3/setup.cfg
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-19 03:10:36.693376 dmk_packages-0.6.3/src/
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-19 03:10:36.694705 dmk_packages-0.6.3/src/dmk_packages/
+-rw-r--r--   0 tommie     (501) staff       (20)        0 2024-04-04 04:45:57.000000 dmk_packages-0.6.3/src/dmk_packages/__init__.py
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-19 03:10:36.698393 dmk_packages-0.6.3/src/dmk_packages/crawler/
+-rw-r--r--   0 tommie     (501) staff       (20)        0 2024-04-04 04:45:57.000000 dmk_packages-0.6.3/src/dmk_packages/crawler/__init__.py
+-rw-r--r--   0 tommie     (501) staff       (20)     6713 2024-04-19 01:31:11.000000 dmk_packages-0.6.3/src/dmk_packages/crawler/bigkinds.py
+-rw-r--r--   0 tommie     (501) staff       (20)     6383 2024-04-19 03:06:14.000000 dmk_packages-0.6.3/src/dmk_packages/crawler/clien.py
+-rw-r--r--   0 tommie     (501) staff       (20)     6418 2024-04-19 01:29:55.000000 dmk_packages-0.6.3/src/dmk_packages/crawler/fnguide.py
+-rw-r--r--   0 tommie     (501) staff       (20)     2743 2024-04-19 01:29:55.000000 dmk_packages-0.6.3/src/dmk_packages/crawler/fnguide_pdf_update.py
+-rw-r--r--   0 tommie     (501) staff       (20)     2321 2024-04-04 04:45:57.000000 dmk_packages-0.6.3/src/dmk_packages/crawler/naver_blog.py
+-rw-r--r--   0 tommie     (501) staff       (20)    15349 2024-04-04 04:45:57.000000 dmk_packages-0.6.3/src/dmk_packages/crawler/naver_search_volume.py
+-rw-r--r--   0 tommie     (501) staff       (20)    12855 2024-04-17 07:27:18.000000 dmk_packages-0.6.3/src/dmk_packages/crawler/youtube.py
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-19 03:10:36.699026 dmk_packages-0.6.3/src/dmk_packages/database/
+-rw-r--r--   0 tommie     (501) staff       (20)        0 2024-04-04 04:45:57.000000 dmk_packages-0.6.3/src/dmk_packages/database/__init__.py
+-rw-r--r--   0 tommie     (501) staff       (20)     3057 2024-04-04 04:45:57.000000 dmk_packages-0.6.3/src/dmk_packages/database/database.py
+-rw-r--r--   0 tommie     (501) staff       (20)     1895 2024-04-04 04:45:57.000000 dmk_packages-0.6.3/src/dmk_packages/naver_datalab.py
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-19 03:10:36.699390 dmk_packages-0.6.3/src/dmk_packages.egg-info/
+-rw-r--r--   0 tommie     (501) staff       (20)     1854 2024-04-19 03:10:36.000000 dmk_packages-0.6.3/src/dmk_packages.egg-info/PKG-INFO
+-rw-r--r--   0 tommie     (501) staff       (20)      684 2024-04-19 03:10:36.000000 dmk_packages-0.6.3/src/dmk_packages.egg-info/SOURCES.txt
+-rw-r--r--   0 tommie     (501) staff       (20)        1 2024-04-19 03:10:36.000000 dmk_packages-0.6.3/src/dmk_packages.egg-info/dependency_links.txt
+-rw-r--r--   0 tommie     (501) staff       (20)       41 2024-04-19 03:10:36.000000 dmk_packages-0.6.3/src/dmk_packages.egg-info/requires.txt
+-rw-r--r--   0 tommie     (501) staff       (20)       13 2024-04-19 03:10:36.000000 dmk_packages-0.6.3/src/dmk_packages.egg-info/top_level.txt
```

### Comparing `dmk_packages-0.6.2/LICENSE` & `dmk_packages-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.2/PKG-INFO` & `dmk_packages-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmk_packages
-Version: 0.6.2
+Version: 0.6.3
 Summary: Common packages for DataMKTKorea
 Author-email: DataMarketingKorea <infra@datamarketing.co.kr>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `dmk_packages-0.6.2/README.md` & `dmk_packages-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.2/pyproject.toml` & `dmk_packages-0.6.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dmk_packages"
-version = "0.6.2"
+version = "0.6.3"
 authors = [{ name = "DataMarketingKorea", email = "infra@datamarketing.co.kr" }]
 description = "Common packages for DataMKTKorea"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = ["SQLAlchemy", "python-dotenv", "psycopg2-binary"]
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `dmk_packages-0.6.2/src/dmk_packages/crawler/bigkinds.py` & `dmk_packages-0.6.3/src/dmk_packages/crawler/bigkinds.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.2/src/dmk_packages/crawler/clien.py` & `dmk_packages-0.6.3/src/dmk_packages/crawler/clien.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,160 +2,158 @@
 import time
 import pendulum
 import requests
 from bs4 import BeautifulSoup
 from fake_useragent import UserAgent
 from loguru import logger
 import random
-from dmk_packages.database import database as dbs
 from sqlalchemy import MetaData, Table, select, func
 
+"""
+## Clien 크롤러 ##
+- 사용 유의사항
+카테고리와 검색할 키워드를 묶어서 매개변수로 전달해줘야함
+ex. targets = [
+                (keyword, category)
+                for category in self._cat_list
+                for keyword in keywords
+            ]
+            for target in targets:
+                keyword, category = target
+
+- 사용 순서
+check_borad_sn > start_beautifulsoup > crawling_posts > check_next_page > crawling_post_detail_list
+> 디비 적재 > 페이지가 더 있다면 처음부터 다시 시작(페이지 추가)
+
+"""
+tz = pendulum.timezone("Asia/Seoul")
+
 
 class ClienCrawler:
-    def __init__(self, start_date=None, end_date=None, engine=None, table=None):
-        # 크롤러
+    def __init__(self, date_from, date_until):
+        DEFAULT_DT = pendulum.yesterday(tz=tz)
+
         self._user_agent = UserAgent(min_percentage=1.1, os=["windows", "macos"])
         self._session = requests.session()
         self._max_board_sn = 0
         self._min_board_sn = 0
-        self.BASE_URL = "https://www.clien.net"
+        self._base_url = "https://www.clien.net"
 
-        # 날짜설정
-        self.start_date = start_date
-        self.end_date = end_date
+        self._date_from = pendulum.parse(date_from) if date_from else DEFAULT_DT
+        _date_until = pendulum.parse(date_until) if date_until else DEFAULT_DT
+        self._date_until = _date_until.strftime("%Y-%m-%d 23:59:59")
 
-        # 데이터베이스
-        self.get_engine = engine
-        self.DATA_TABLE = table
-
-
-    def _check_data_table(self, keyword, category, table):
+    def check_board_sn(self, keyword, category, table, engine):
         """
         keyword 및 category에 해당하는 board_sn컬럼의 max, min 값을 가져오는 컬럼
         """
+
         metadata = MetaData()
-        metadata.bind = self.get_engine
-        table = Table(table, metadata, autoload_with=self.get_engine)
+        metadata.bind = engine
+        table = Table(table, metadata, autoload_with=engine)
 
         stmt = select(func.max(table.c.board_sn), func.min(table.c.board_sn)).where(
             (table.c.category_name == category) & (table.c.keyword == keyword)
         )
 
-        with self.get_engine.begin() as connection:
+        with engine.begin() as connection:
             result = connection.execute(stmt)
             a = result.fetchall()
             max_board_sn = a[0][0] or 0
             min_board_sn = a[0][1] or 0
 
         return max_board_sn, min_board_sn
 
-    def _run_list_crawl(self, keyword: str, category: str, page: int):
-        """
-        해당되는 데이터 가져오기
-        """
-        try:
-            headers = {"User-agent": self._user_agent.random}
-            target_url = self.BASE_URL + "/service/search"
-            params = {
-                "q": keyword,
-                "p": page,
-                "sort": "recency",
-                "boardCd": category,
-                "isBoard": True,
-            }
-
-            response = self._session.get(
-                target_url, headers=headers, params=params, timeout=3
-            )
-            time.sleep(random.uniform(1, 10))
-
-            soup = BeautifulSoup(response.text, "html.parser")
-
-            keyword_posts = self._retrieve_posts(soup, keyword, category)
-            next_page = self._retrieve_next_page(soup)
-            return keyword_posts, next_page
-        except Exception as error:
-            logger.error(error)
-
-    def _retrieve_posts(self, soup: BeautifulSoup, keyword: str, category: str):
-        """
-        데이터 수집
-        """
-        try:
-            items = soup.select(".list_item.symph_row.jirum")
-            results = []
-            start_date = pendulum.parse(self.start_date)
-            end_date = pendulum.parse(self.end_date)
-
-            for item in items:
-                board_sn = int(item["data-board-sn"])
-                regist_date = pendulum.parse(item.select_one(".timestamp").text)
-
-                if self._min_board_sn <= board_sn <= self._max_board_sn:
-                    continue
-
-                if start_date < regist_date < end_date:
-                    comment = int(item["data-comment-count"])
-                    url = self.BASE_URL + item.select_one(".subject_fixed")["href"]
-
-                    data = {
-                        "category_name": category,
-                        "regist_date": regist_date,
-                        "comment": comment,
-                        "url": url,
-                        "keyword": keyword,
-                        "board_sn": board_sn,
-                    }
-                    results.append(data)
-            return results
-        except Exception as error:
-            logger.error(error)
+    def start_beautifulsoup(self, keyword: str, category: str, page: int):
+        headers = {"User-agent": self._user_agent.random}
+        target_url = self._base_url + "/service/search"
+        keyword_r = keyword.replace("&", "%26").replace("(", "").replace(")", "")
+        params = {
+            "q": keyword_r,
+            "p": page,
+            "sort": "recency",
+            "boardCd": category,
+            "isBoard": True,
+        }
+
+        response = self._session.get(
+            target_url, headers=headers, params=params, timeout=3
+        )
+        time.sleep(random.uniform(1, 10))
 
-    def _retrieve_next_page(self, soup: BeautifulSoup):
+        soup = BeautifulSoup(response.text, "html.parser")
+        return soup
+
+    def crawling_posts(self, soup: BeautifulSoup, keyword: str, category: str):
         """
-        다음 페이지 가져오기 없으면 패스
+        게시물들의 기본적인 내용 크롤링
         """
+        items = soup.select(".list_item.symph_row.jirum")
+        results = []
+
+        for item in items:
+            board_sn = int(item["data-board-sn"])
+            regist_date = pendulum.parse(item.select_one(".timestamp").text)
+
+            title = item.select_one(".subject_fixed").text
+            if "헤드라인 모음" in title:
+                continue
+
+            if self._min_board_sn <= board_sn <= self._max_board_sn:
+                continue
+
+            if self._date_from < regist_date < pendulum.parse(self._date_until):
+                comment = int(item["data-comment-count"])
+                url = self._base_url + item.select_one(".subject_fixed")["href"]
+
+                data = {
+                    "category_name": category,
+                    "regist_date": regist_date,
+                    "comment": comment,
+                    "url": url,
+                    "keyword": keyword,
+                    "board_sn": board_sn,
+                }
+                results.append(data)
+        return results
+
+    def check_next_page(self, soup: BeautifulSoup):
         pages = soup.select(".board-nav-page")
         if len(pages) <= 1:
             return None
         next_btn_exists = bool(soup.select_one(".board-nav-next"))
 
         last_item = soup.select(".list_item")[-1]
         last_item_timestamp = last_item.select_one(".timestamp").text
 
-        if pendulum.parse(self.start_date) > pendulum.parse(last_item_timestamp):
+        if self._date_from > pendulum.parse(last_item_timestamp):
             return None
 
         for idx, page in enumerate(pages):
             if "active" in page.get("class", []):
                 if next_btn_exists or idx + 1 < len(pages):
                     return idx + 1
                 break
-
         return None
 
-    def _run_item_crawl(self, posts):
+    def crawling_post_detail_list(self, posts):
         """
-        해당 게시물의 내용 가져오는 전반적인 내용
+        해당 게시물의 디테일한 내용 가져와서 리스트에 저장
         """
-        try:
-            results = []
-            for post in posts:
-                logger.info(f"[적재하는 url: {post['url']}")
-
-                details = self._retrieve_post_detail(post.get("url"))
-                results.append({**post, **details})
+        results = []
+        for post in posts:
+            logger.info(f"[적재하는 url: {post['url']}")
 
-            return results
-        except Exception as error:
-            logger.error(error)
+            details = self._crawling_post_detail(post.get("url"))
+            results.append({**post, **details})
+        return results
 
-    def _retrieve_post_detail(self, post_url):
+    def _crawling_post_detail(self, post_url):
         """
-        해당 게시물의 내용 정제해서 가져오기
+        해당 게시물의 디테일한 내용 정제하기
         """
         headers = {"User-agent": self._user_agent.random}
         response = self._session.get(post_url, headers=headers)
         time.sleep(random.uniform(1, 10))
 
         soup = BeautifulSoup(response.text, "html.parser")
 
@@ -178,45 +176,7 @@
         contents = re.sub(r"\n", " ", contents)
         # \xa0, \xad, \ufeff 문자 제거
         contents = re.sub(r"[\xa0\xad\ufeff]+", "", contents)
         # 두 개 이상의 공백을 단일 공백으로 치환
         contents = re.sub(r" {2,}", " ", contents)
 
         return {"view": int(view), "title": title, "contents": contents}
-
-    def _process_target(self, target, page=0):
-        """
-        크롤러 전반적인 운영
-        """
-        keyword, category = target
-        logger.info(f"[{category}][{keyword}] 크롤링 시작")
-        self._max_board_sn, self._min_board_sn = self._check_data_table(
-            keyword=keyword, category=category, table=self.DATA_TABLE
-        )
-
-        keyword_posts, next_page = self._run_list_crawl(keyword, category, page)
-        keyword_results = self._run_item_crawl(keyword_posts)
-
-        # =========================================
-        # NOTE: 데이터베이스 저장
-        try:
-            if len(keyword_results) > 0:
-                dbs.insert_to_postgres(
-                    engine=self.get_engine,
-                    name=self.DATA_TABLE,
-                    values=keyword_results,
-                    index_elements=[
-                        "category_name",
-                        "keyword",
-                        "regist_date",
-                        "board_sn",
-                    ],
-                )
-                logger.info("데이터 적재 완료")
-            else:
-                logger.info("적재할 데이터 없음")
-        except Exception as e:
-            logger.error(f"데이터 적재 실패 | error_comment : {e}")
-        # =========================================
-        if next_page:
-            self._process_target(target, next_page)
-            logger.info("다음 페이지 적재 시작")
```

### Comparing `dmk_packages-0.6.2/src/dmk_packages/crawler/fnguide.py` & `dmk_packages-0.6.3/src/dmk_packages/crawler/fnguide.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.2/src/dmk_packages/crawler/fnguide_pdf_update.py` & `dmk_packages-0.6.3/src/dmk_packages/crawler/fnguide_pdf_update.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.2/src/dmk_packages/crawler/naver_blog.py` & `dmk_packages-0.6.3/src/dmk_packages/crawler/naver_blog.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.2/src/dmk_packages/crawler/naver_search_volume.py` & `dmk_packages-0.6.3/src/dmk_packages/crawler/naver_search_volume.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.2/src/dmk_packages/crawler/youtube.py` & `dmk_packages-0.6.3/src/dmk_packages/crawler/youtube.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,51 +1,39 @@
 import time
 from typing import List
-from datetime import datetime
 
 import pendulum
 from loguru import logger
-from sqlalchemy.sql import func
-from sqlalchemy import text, Column, Integer, String, Date, DateTime, UniqueConstraint
+from sqlalchemy import text
 from googleapiclient.discovery import build
 from googleapiclient.errors import HttpError
 
 from dmk_packages.database import database as db
 
 
 class YoutubeDBHandler:
     # ==============================================================================
     # NOTE : 한투(postgres)로 데이터베이스 설정
-    def __init__(self, target="KOREAINVESTMENT_DMK", meta_table_name="t_metadata_youtube"):
-        self._db_engine = db.get_engine(target)
-        self._meta_table = meta_table_name
-        db.create_to_postgres(
-            self._db_engine,
-            self._meta_table,
-            Column("id", Integer, primary_key=True, autoincrement=True),
-            Column("keyword", String),
-            Column("next_page_token", String),
-            Column("target_date", Date),
-            Column("created_at", DateTime, nullable=False, server_default=func.now()),
-            UniqueConstraint("id", name="t_metadata_youtube_pk")
-        )
-        if not self._db_engine:
+    def __init__(self, target="KOREAINVESTMENT_DMK"):
+        self._krinv_engine = db.get_engine(target)
+        self._meta_table = "t_metadata_youtube"
+        if not self._krinv_engine:
             raise ValueError("데이터베이스 엔진 설정에 실패했습니다.")
     # ==============================================================================
 
     # ==============================================================================
     # NOTE : json 응답에 있는 "next_page_token" 키에 해당하는 값을 metadata 테이블에 저장
     def _save_page_token(self, keyword, target_date, next_page_token):
         query = f"""
         INSERT INTO {self._meta_table} (keyword, next_page_token, target_date)
         VALUES ('{keyword}', '{next_page_token}', '{target_date}');
         """
 
         try:
-            with self._db_engine.begin() as connection:
+            with self._krinv_engine.begin() as connection:
                 connection.execute(text(query))
             logger.info(
                 f"[{keyword}][{target_date}]: Metadata insertion completed."
             )
         except Exception as err:
             logger.error(err)
     # ==============================================================================
@@ -57,15 +45,15 @@
         SELECT next_page_token
         FROM {self._meta_table}
         WHERE keyword = '{keyword}'
             AND target_date = '{target_date}';
         """
 
         try:
-            with self._db_engine.begin() as connection:
+            with self._krinv_engine.begin() as connection:
                 result = connection.execute(text(query)).fetchone()
                 return result[0] if result else False
         except Exception as err:
             logger.error(err)
     # ==============================================================================
 
     # ==============================================================================
@@ -75,15 +63,15 @@
         UPDATE {self._meta_table}
         SET next_page_token = '{next_page_token}'
         WHERE keyword = '{keyword}'
             AND target_date = '{target_date}'
         """
 
         try:
-            with self._db_engine.begin() as connection:
+            with self._krinv_engine.begin() as connection:
                 connection.execute(text(query))
             logger.info(f"[{keyword}][{target_date}]: Metadata update completed.")
         except Exception as err:
             logger.error(err)
     # ==============================================================================
 
 
@@ -288,15 +276,16 @@
 
         except Exception as err:
             logger.error(err)
     # ==============================================================================
 
     # ==============================================================================
     # NOTE : _results 값 반환
-    def get_videos_info(self, keyword, target_date):
+    def get_videos_info(self, keywords_target_dates):
+        keyword, target_date = keywords_target_dates
         next_page_token = self._get_page_token(keyword, target_date)
 
         if next_page_token == 'None':
             logger.info(f"[{keyword}][{target_date}]: 이미 수집 완료")
         elif not next_page_token:
             # logger.info(f"[{keyword}][{target_date}]: 수집 필요")
             self._stack_videos_info(keyword, target_date)
```

### Comparing `dmk_packages-0.6.2/src/dmk_packages/database/database.py` & `dmk_packages-0.6.3/src/dmk_packages/database/database.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.2/src/dmk_packages/naver_datalab.py` & `dmk_packages-0.6.3/src/dmk_packages/naver_datalab.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.2/src/dmk_packages.egg-info/PKG-INFO` & `dmk_packages-0.6.3/src/dmk_packages.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmk_packages
-Version: 0.6.2
+Version: 0.6.3
 Summary: Common packages for DataMKTKorea
 Author-email: DataMarketingKorea <infra@datamarketing.co.kr>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `dmk_packages-0.6.2/src/dmk_packages.egg-info/SOURCES.txt` & `dmk_packages-0.6.3/src/dmk_packages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

