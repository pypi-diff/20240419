# Comparing `tmp/new_python_scrapy-0.1.1.tar.gz` & `tmp/new_python_scrapy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "new_python_scrapy-0.1.1.tar", last modified: Fri Apr 19 09:39:45 2024, max compression
+gzip compressed data, was "new_python_scrapy-0.1.2.tar", last modified: Fri Apr 19 10:11:41 2024, max compression
```

## Comparing `new_python_scrapy-0.1.1.tar` & `new_python_scrapy-0.1.2.tar`

### file list

```diff
@@ -1,535 +1,532 @@
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:45.017659 new_python_scrapy-0.1.1/
--rw-rw-r--   0 test      (1000) test      (1000)     1284 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/AUTHORS
--rw-rw-r--   0 test      (1000) test      (1000)     1517 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/LICENSE
--rw-rw-r--   0 test      (1000) test      (1000)      510 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/MANIFEST.in
--rw-rw-r--   0 test      (1000) test      (1000)       18 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/NEWS
--rw-r--r--   0 test      (1000) test      (1000)     4354 2024-04-19 09:39:45.017659 new_python_scrapy-0.1.1/PKG-INFO
--rw-rw-r--   0 test      (1000) test      (1000)     3117 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/README.rst
--rw-rw-r--   0 test      (1000) test      (1000)       80 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/codecov.yml
--rw-rw-r--   0 test      (1000) test      (1000)     2574 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/conftest.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:44.969659 new_python_scrapy-0.1.1/docs/
--rw-rw-r--   0 test      (1000) test      (1000)     2829 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/Makefile
--rw-rw-r--   0 test      (1000) test      (1000)     1581 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/README.rst
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:44.969659 new_python_scrapy-0.1.1/docs/_ext/
--rw-rw-r--   0 test      (1000) test      (1000)     4516 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/_ext/scrapydocs.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:44.969659 new_python_scrapy-0.1.1/docs/_static/
--rw-rw-r--   0 test      (1000) test      (1000)      360 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/_static/custom.css
--rw-rw-r--   0 test      (1000) test      (1000)      667 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/_static/selectors-sample1.html
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:44.969659 new_python_scrapy-0.1.1/docs/_tests/
--rw-rw-r--   0 test      (1000) test      (1000)    11043 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/_tests/quotes.html
--rw-rw-r--   0 test      (1000) test      (1000)    11043 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/_tests/quotes1.html
--rw-rw-r--   0 test      (1000) test      (1000)    10944 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/conf.py
--rw-rw-r--   0 test      (1000) test      (1000)      921 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/conftest.py
--rw-rw-r--   0 test      (1000) test      (1000)    13224 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/contributing.rst
--rw-rw-r--   0 test      (1000) test      (1000)    16563 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/faq.rst
--rw-rw-r--   0 test      (1000) test      (1000)     6876 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/index.rst
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:44.969659 new_python_scrapy-0.1.1/docs/intro/
--rw-rw-r--   0 test      (1000) test      (1000)      745 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/intro/examples.rst
--rw-rw-r--   0 test      (1000) test      (1000)    10323 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/intro/install.rst
--rw-rw-r--   0 test      (1000) test      (1000)     6671 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/intro/overview.rst
--rw-rw-r--   0 test      (1000) test      (1000)    30811 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/intro/tutorial.rst
--rw-rw-r--   0 test      (1000) test      (1000)   263677 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/news.rst
--rw-rw-r--   0 test      (1000) test      (1000)       90 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/requirements.txt
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:44.973659 new_python_scrapy-0.1.1/docs/topics/
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:44.973659 new_python_scrapy-0.1.1/docs/topics/_images/
--rw-rw-r--   0 test      (1000) test      (1000)    53922 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/_images/inspector_01.png
--rw-rw-r--   0 test      (1000) test      (1000)    10720 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/_images/network_01.png
--rw-rw-r--   0 test      (1000) test      (1000)    82702 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/_images/network_02.png
--rw-rw-r--   0 test      (1000) test      (1000)    45506 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/_images/network_03.png
--rw-rw-r--   0 test      (1000) test      (1000)    19653 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/_images/scrapy_architecture.odg
--rw-rw-r--   0 test      (1000) test      (1000)    92558 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/_images/scrapy_architecture.png
--rw-rw-r--   0 test      (1000) test      (1000)    53978 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/_images/scrapy_architecture_02.png
--rw-rw-r--   0 test      (1000) test      (1000)     6785 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/addons.rst
--rw-rw-r--   0 test      (1000) test      (1000)     8348 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/api.rst
--rw-rw-r--   0 test      (1000) test      (1000)     6114 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/architecture.rst
--rw-rw-r--   0 test      (1000) test      (1000)     4983 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/asyncio.rst
--rw-rw-r--   0 test      (1000) test      (1000)     6277 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/autothrottle.rst
--rw-rw-r--   0 test      (1000) test      (1000)     5257 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/benchmarking.rst
--rw-rw-r--   0 test      (1000) test      (1000)     8436 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/broad-crawls.rst
--rw-rw-r--   0 test      (1000) test      (1000)    17953 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/commands.rst
--rw-rw-r--   0 test      (1000) test      (1000)     2758 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/components.rst
--rw-rw-r--   0 test      (1000) test      (1000)     4976 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/contracts.rst
--rw-rw-r--   0 test      (1000) test      (1000)    10376 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/coroutines.rst
--rw-rw-r--   0 test      (1000) test      (1000)     5233 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/debug.rst
--rw-rw-r--   0 test      (1000) test      (1000)     2263 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/deploy.rst
--rw-rw-r--   0 test      (1000) test      (1000)    13859 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/developer-tools.rst
--rw-rw-r--   0 test      (1000) test      (1000)      194 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/djangoitem.rst
--rw-rw-r--   0 test      (1000) test      (1000)    41078 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/downloader-middleware.rst
--rw-rw-r--   0 test      (1000) test      (1000)    12165 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/dynamic-content.rst
--rw-rw-r--   0 test      (1000) test      (1000)     5110 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/email.rst
--rw-rw-r--   0 test      (1000) test      (1000)     3253 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/exceptions.rst
--rw-rw-r--   0 test      (1000) test      (1000)    15581 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/exporters.rst
--rw-rw-r--   0 test      (1000) test      (1000)    16702 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/extensions.rst
--rw-rw-r--   0 test      (1000) test      (1000)    24592 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/feed-exports.rst
--rw-rw-r--   0 test      (1000) test      (1000)     8751 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/item-pipeline.rst
--rw-rw-r--   0 test      (1000) test      (1000)    11569 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/items.rst
--rw-rw-r--   0 test      (1000) test      (1000)     2904 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/jobs.rst
--rw-rw-r--   0 test      (1000) test      (1000)    11883 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/leaks.rst
--rw-rw-r--   0 test      (1000) test      (1000)     6858 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/link-extractors.rst
--rw-rw-r--   0 test      (1000) test      (1000)    16958 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/loaders.rst
--rw-rw-r--   0 test      (1000) test      (1000)    10990 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/logging.rst
--rw-rw-r--   0 test      (1000) test      (1000)    26720 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/media-pipeline.rst
--rw-rw-r--   0 test      (1000) test      (1000)    10607 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/practices.rst
--rw-rw-r--   0 test      (1000) test      (1000)    48143 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/request-response.rst
--rw-rw-r--   0 test      (1000) test      (1000)      761 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/scheduler.rst
--rw-rw-r--   0 test      (1000) test      (1000)      188 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/scrapyd.rst
--rw-rw-r--   0 test      (1000) test      (1000)    37984 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/selectors.rst
--rw-rw-r--   0 test      (1000) test      (1000)    52593 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/settings.rst
--rw-rw-r--   0 test      (1000) test      (1000)    11101 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/shell.rst
--rw-rw-r--   0 test      (1000) test      (1000)    16976 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/signals.rst
--rw-rw-r--   0 test      (1000) test      (1000)    19050 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/spider-middleware.rst
--rw-rw-r--   0 test      (1000) test      (1000)    35299 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/spiders.rst
--rw-rw-r--   0 test      (1000) test      (1000)     3713 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/stats.rst
--rw-rw-r--   0 test      (1000) test      (1000)     7468 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/topics/telnetconsole.rst
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:44.973659 new_python_scrapy-0.1.1/docs/utils/
--rw-rw-r--   0 test      (1000) test      (1000)     1975 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/utils/linkfix.py
--rw-rw-r--   0 test      (1000) test      (1000)     2161 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/docs/versioning.rst
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:44.977659 new_python_scrapy-0.1.1/extras/
--rwxrwxr-x   0 test      (1000) test      (1000)      259 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/extras/coverage-report.sh
--rwxrwxr-x   0 test      (1000) test      (1000)     1618 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/extras/qps-bench-server.py
--rw-rw-r--   0 test      (1000) test      (1000)     1507 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/extras/qpsclient.py
--rw-rw-r--   0 test      (1000) test      (1000)     2010 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/extras/scrapy.1
--rw-rw-r--   0 test      (1000) test      (1000)      698 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/extras/scrapy_bash_completion
--rw-rw-r--   0 test      (1000) test      (1000)     7008 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/extras/scrapy_zsh_completion
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:45.017659 new_python_scrapy-0.1.1/new_python_scrapy.egg-info/
--rw-r--r--   0 test      (1000) test      (1000)     4354 2024-04-19 09:39:44.000000 new_python_scrapy-0.1.1/new_python_scrapy.egg-info/PKG-INFO
--rw-rw-r--   0 test      (1000) test      (1000)    15580 2024-04-19 09:39:44.000000 new_python_scrapy-0.1.1/new_python_scrapy.egg-info/SOURCES.txt
--rw-rw-r--   0 test      (1000) test      (1000)        1 2024-04-19 09:39:44.000000 new_python_scrapy-0.1.1/new_python_scrapy.egg-info/dependency_links.txt
--rw-rw-r--   0 test      (1000) test      (1000)       52 2024-04-19 09:39:44.000000 new_python_scrapy-0.1.1/new_python_scrapy.egg-info/entry_points.txt
--rw-rw-r--   0 test      (1000) test      (1000)        1 2024-04-19 09:39:44.000000 new_python_scrapy-0.1.1/new_python_scrapy.egg-info/not-zip-safe
--rw-rw-r--   0 test      (1000) test      (1000)      414 2024-04-19 09:39:44.000000 new_python_scrapy-0.1.1/new_python_scrapy.egg-info/requires.txt
--rw-rw-r--   0 test      (1000) test      (1000)        8 2024-04-19 09:39:44.000000 new_python_scrapy-0.1.1/new_python_scrapy.egg-info/top_level.txt
--rw-rw-r--   0 test      (1000) test      (1000)     1000 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/pytest.ini
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:44.977659 new_python_scrapy-0.1.1/scrapyy/
--rw-rw-r--   0 test      (1000) test      (1000)     1071 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/__init__.py
--rw-rw-r--   0 test      (1000) test      (1000)       77 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/__main__.py
--rw-rw-r--   0 test      (1000) test      (1000)     1837 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/addons.py
--rw-rw-r--   0 test      (1000) test      (1000)     5757 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/cmdline.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:44.981659 new_python_scrapy-0.1.1/scrapyy/commands/
--rw-rw-r--   0 test      (1000) test      (1000)     7481 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/commands/__init__.py
--rw-rw-r--   0 test      (1000) test      (1000)     1930 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/commands/bench.py
--rw-rw-r--   0 test      (1000) test      (1000)     3836 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/commands/check.py
--rw-rw-r--   0 test      (1000) test      (1000)     1273 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/commands/crawl.py
--rw-rw-r--   0 test      (1000) test      (1000)     1239 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/commands/edit.py
--rw-rw-r--   0 test      (1000) test      (1000)     3150 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/commands/fetch.py
--rw-rw-r--   0 test      (1000) test      (1000)     7057 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/commands/genspider.py
--rw-rw-r--   0 test      (1000) test      (1000)      459 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/commands/list.py
--rw-rw-r--   0 test      (1000) test      (1000)    13974 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/commands/parse.py
--rw-rw-r--   0 test      (1000) test      (1000)     1943 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/commands/runspider.py
--rw-rw-r--   0 test      (1000) test      (1000)     2046 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/commands/settings.py
--rw-rw-r--   0 test      (1000) test      (1000)     3187 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/commands/shell.py
--rw-rw-r--   0 test      (1000) test      (1000)     4635 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/commands/startproject.py
--rw-rw-r--   0 test      (1000) test      (1000)     1092 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/commands/version.py
--rw-rw-r--   0 test      (1000) test      (1000)      892 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/commands/view.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:44.981659 new_python_scrapy-0.1.1/scrapyy/contracts/
--rw-rw-r--   0 test      (1000) test      (1000)     6724 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/contracts/__init__.py
--rw-rw-r--   0 test      (1000) test      (1000)     2946 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/contracts/default.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:44.981659 new_python_scrapy-0.1.1/scrapyy/core/
--rw-rw-r--   0 test      (1000) test      (1000)       51 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/core/__init__.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:44.981659 new_python_scrapy-0.1.1/scrapyy/core/downloader/
--rw-rw-r--   0 test      (1000) test      (1000)     9107 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/core/downloader/__init__.py
--rw-rw-r--   0 test      (1000) test      (1000)     6768 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/core/downloader/contextfactory.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:44.985659 new_python_scrapy-0.1.1/scrapyy/core/downloader/handlers/
--rw-rw-r--   0 test      (1000) test      (1000)     3351 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/core/downloader/handlers/__init__.py
--rw-rw-r--   0 test      (1000) test      (1000)      795 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/core/downloader/handlers/datauri.py
--rw-rw-r--   0 test      (1000) test      (1000)      479 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/core/downloader/handlers/file.py
--rw-rw-r--   0 test      (1000) test      (1000)     4638 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/core/downloader/handlers/ftp.py
--rw-rw-r--   0 test      (1000) test      (1000)      178 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/core/downloader/handlers/http.py
--rw-rw-r--   0 test      (1000) test      (1000)     1302 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/core/downloader/handlers/http10.py
--rw-rw-r--   0 test      (1000) test      (1000)    24230 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/core/downloader/handlers/http11.py
--rw-rw-r--   0 test      (1000) test      (1000)     4410 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/core/downloader/handlers/http2.py
--rw-rw-r--   0 test      (1000) test      (1000)     2969 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/core/downloader/handlers/s3.py
--rw-rw-r--   0 test      (1000) test      (1000)     4286 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/core/downloader/middleware.py
--rw-rw-r--   0 test      (1000) test      (1000)     3253 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/core/downloader/tls.py
--rw-rw-r--   0 test      (1000) test      (1000)     8460 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/core/downloader/webclient.py
--rw-rw-r--   0 test      (1000) test      (1000)    17068 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/core/engine.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:44.985659 new_python_scrapy-0.1.1/scrapyy/core/http2/
--rw-rw-r--   0 test      (1000) test      (1000)        0 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/core/http2/__init__.py
--rw-rw-r--   0 test      (1000) test      (1000)     6042 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/core/http2/agent.py
--rw-rw-r--   0 test      (1000) test      (1000)    17089 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/core/http2/protocol.py
--rw-rw-r--   0 test      (1000) test      (1000)    19199 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/core/http2/stream.py
--rw-rw-r--   0 test      (1000) test      (1000)    14514 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/core/scheduler.py
--rw-rw-r--   0 test      (1000) test      (1000)    14449 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/core/scraper.py
--rw-rw-r--   0 test      (1000) test      (1000)    14575 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/core/spidermw.py
--rw-rw-r--   0 test      (1000) test      (1000)    17730 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/crawler.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:44.985659 new_python_scrapy-0.1.1/scrapyy/downloadermiddlewares/
--rw-rw-r--   0 test      (1000) test      (1000)        0 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/downloadermiddlewares/__init__.py
--rw-rw-r--   0 test      (1000) test      (1000)     3737 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/downloadermiddlewares/ajaxcrawl.py
--rw-rw-r--   0 test      (1000) test      (1000)     6135 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/downloadermiddlewares/cookies.py
--rw-rw-r--   0 test      (1000) test      (1000)     1009 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/downloadermiddlewares/defaultheaders.py
--rw-rw-r--   0 test      (1000) test      (1000)     1093 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/downloadermiddlewares/downloadtimeout.py
--rw-rw-r--   0 test      (1000) test      (1000)     1484 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/downloadermiddlewares/httpauth.py
--rw-rw-r--   0 test      (1000) test      (1000)     5724 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/downloadermiddlewares/httpcache.py
--rw-rw-r--   0 test      (1000) test      (1000)     6932 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/downloadermiddlewares/httpcompression.py
--rw-rw-r--   0 test      (1000) test      (1000)     3783 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/downloadermiddlewares/httpproxy.py
--rw-rw-r--   0 test      (1000) test      (1000)     6297 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/downloadermiddlewares/redirect.py
--rw-rw-r--   0 test      (1000) test      (1000)     7748 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/downloadermiddlewares/retry.py
--rw-rw-r--   0 test      (1000) test      (1000)     5548 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/downloadermiddlewares/robotstxt.py
--rw-rw-r--   0 test      (1000) test      (1000)     2881 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/downloadermiddlewares/stats.py
--rw-rw-r--   0 test      (1000) test      (1000)     1125 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/downloadermiddlewares/useragent.py
--rw-rw-r--   0 test      (1000) test      (1000)     3627 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/dupefilters.py
--rw-rw-r--   0 test      (1000) test      (1000)     2033 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/exceptions.py
--rw-rw-r--   0 test      (1000) test      (1000)    13928 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/exporters.py
--rw-rw-r--   0 test      (1000) test      (1000)      397 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/extension.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:44.989659 new_python_scrapy-0.1.1/scrapyy/extensions/
--rw-rw-r--   0 test      (1000) test      (1000)        0 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/extensions/__init__.py
--rw-rw-r--   0 test      (1000) test      (1000)     4910 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/extensions/closespider.py
--rw-rw-r--   0 test      (1000) test      (1000)     2394 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/extensions/corestats.py
--rw-rw-r--   0 test      (1000) test      (1000)     2285 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/extensions/debug.py
--rw-rw-r--   0 test      (1000) test      (1000)    24676 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/extensions/feedexport.py
--rw-rw-r--   0 test      (1000) test      (1000)    14805 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/extensions/httpcache.py
--rw-rw-r--   0 test      (1000) test      (1000)     3277 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/extensions/logstats.py
--rw-rw-r--   0 test      (1000) test      (1000)     1326 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/extensions/memdebug.py
--rw-rw-r--   0 test      (1000) test      (1000)     5951 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/extensions/memusage.py
--rw-rw-r--   0 test      (1000) test      (1000)     5570 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/extensions/periodic_log.py
--rw-rw-r--   0 test      (1000) test      (1000)     4933 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/extensions/postprocessing.py
--rw-rw-r--   0 test      (1000) test      (1000)     1641 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/extensions/spiderstate.py
--rw-rw-r--   0 test      (1000) test      (1000)     1726 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/extensions/statsmailer.py
--rw-rw-r--   0 test      (1000) test      (1000)     4493 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/extensions/telnet.py
--rw-rw-r--   0 test      (1000) test      (1000)     4653 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/extensions/throttle.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:44.989659 new_python_scrapy-0.1.1/scrapyy/http/
--rw-rw-r--   0 test      (1000) test      (1000)      651 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/http/__init__.py
--rw-rw-r--   0 test      (1000) test      (1000)     6014 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/http/cookies.py
--rw-rw-r--   0 test      (1000) test      (1000)     4399 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/http/headers.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:44.989659 new_python_scrapy-0.1.1/scrapyy/http/request/
--rw-rw-r--   0 test      (1000) test      (1000)     9708 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/http/request/__init__.py
--rw-rw-r--   0 test      (1000) test      (1000)     8859 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/http/request/form.py
--rw-rw-r--   0 test      (1000) test      (1000)     2026 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/http/request/json_request.py
--rw-rw-r--   0 test      (1000) test      (1000)     1161 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/http/request/rpc.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:44.989659 new_python_scrapy-0.1.1/scrapyy/http/response/
--rw-rw-r--   0 test      (1000) test      (1000)     9025 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/http/response/__init__.py
--rw-rw-r--   0 test      (1000) test      (1000)      300 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/http/response/html.py
--rw-rw-r--   0 test      (1000) test      (1000)      286 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/http/response/json.py
--rw-rw-r--   0 test      (1000) test      (1000)    11510 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/http/response/text.py
--rw-rw-r--   0 test      (1000) test      (1000)      297 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/http/response/xml.py
--rw-rw-r--   0 test      (1000) test      (1000)      557 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/interfaces.py
--rw-rw-r--   0 test      (1000) test      (1000)     3823 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/item.py
--rw-rw-r--   0 test      (1000) test      (1000)     2082 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/link.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:44.989659 new_python_scrapy-0.1.1/scrapyy/linkextractors/
--rw-rw-r--   0 test      (1000) test      (1000)     1647 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/linkextractors/__init__.py
--rw-rw-r--   0 test      (1000) test      (1000)     8463 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/linkextractors/lxmlhtml.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:44.989659 new_python_scrapy-0.1.1/scrapyy/loader/
--rw-rw-r--   0 test      (1000) test      (1000)     3498 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/loader/__init__.py
--rw-rw-r--   0 test      (1000) test      (1000)     6110 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/logformatter.py
--rw-rw-r--   0 test      (1000) test      (1000)     6459 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/mail.py
--rw-rw-r--   0 test      (1000) test      (1000)     3689 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/middleware.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:44.989659 new_python_scrapy-0.1.1/scrapyy/pipelines/
--rw-rw-r--   0 test      (1000) test      (1000)      949 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/pipelines/__init__.py
--rw-rw-r--   0 test      (1000) test      (1000)    21346 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/pipelines/files.py
--rw-rw-r--   0 test      (1000) test      (1000)     9007 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/pipelines/images.py
--rw-rw-r--   0 test      (1000) test      (1000)     8613 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/pipelines/media.py
--rw-rw-r--   0 test      (1000) test      (1000)     7709 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/pqueues.py
--rw-rw-r--   0 test      (1000) test      (1000)        0 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/py.typed
--rw-rw-r--   0 test      (1000) test      (1000)     4205 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/resolver.py
--rw-rw-r--   0 test      (1000) test      (1000)     5576 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/responsetypes.py
--rw-rw-r--   0 test      (1000) test      (1000)     4714 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/robotstxt.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:44.989659 new_python_scrapy-0.1.1/scrapyy/selector/
--rw-rw-r--   0 test      (1000) test      (1000)       98 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/selector/__init__.py
--rw-rw-r--   0 test      (1000) test      (1000)     3116 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/selector/unified.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:44.989659 new_python_scrapy-0.1.1/scrapyy/settings/
--rw-rw-r--   0 test      (1000) test      (1000)    19859 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/settings/__init__.py
--rw-rw-r--   0 test      (1000) test      (1000)    10079 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/settings/default_settings.py
--rw-rw-r--   0 test      (1000) test      (1000)     8537 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/shell.py
--rw-rw-r--   0 test      (1000) test      (1000)     2584 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/signalmanager.py
--rw-rw-r--   0 test      (1000) test      (1000)      875 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/signals.py
--rw-rw-r--   0 test      (1000) test      (1000)     3483 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/spiderloader.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:44.989659 new_python_scrapy-0.1.1/scrapyy/spidermiddlewares/
--rw-rw-r--   0 test      (1000) test      (1000)        0 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/spidermiddlewares/__init__.py
--rw-rw-r--   0 test      (1000) test      (1000)     2788 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/spidermiddlewares/depth.py
--rw-rw-r--   0 test      (1000) test      (1000)     2529 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/spidermiddlewares/httperror.py
--rw-rw-r--   0 test      (1000) test      (1000)     3841 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/spidermiddlewares/offsite.py
--rw-rw-r--   0 test      (1000) test      (1000)    15250 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/spidermiddlewares/referer.py
--rw-rw-r--   0 test      (1000) test      (1000)     1831 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/spidermiddlewares/urllength.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:44.993659 new_python_scrapy-0.1.1/scrapyy/spiders/
--rw-rw-r--   0 test      (1000) test      (1000)     3622 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/spiders/__init__.py
--rw-rw-r--   0 test      (1000) test      (1000)     4722 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/spiders/crawl.py
--rw-rw-r--   0 test      (1000) test      (1000)     5506 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/spiders/feed.py
--rw-rw-r--   0 test      (1000) test      (1000)     1337 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/spiders/init.py
--rw-rw-r--   0 test      (1000) test      (1000)     4867 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/spiders/sitemap.py
--rw-rw-r--   0 test      (1000) test      (1000)     4842 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/squeues.py
--rw-rw-r--   0 test      (1000) test      (1000)     3005 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/statscollectors.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:44.993659 new_python_scrapy-0.1.1/scrapyy/utils/
--rw-rw-r--   0 test      (1000) test      (1000)        0 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/__init__.py
--rw-rw-r--   0 test      (1000) test      (1000)     4291 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/_compression.py
--rw-rw-r--   0 test      (1000) test      (1000)      507 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/asyncgen.py
--rw-rw-r--   0 test      (1000) test      (1000)     1308 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/benchserver.py
--rw-rw-r--   0 test      (1000) test      (1000)      180 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/boto.py
--rw-rw-r--   0 test      (1000) test      (1000)     9064 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/conf.py
--rw-rw-r--   0 test      (1000) test      (1000)     4114 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/console.py
--rw-rw-r--   0 test      (1000) test      (1000)     3587 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/curl.py
--rw-rw-r--   0 test      (1000) test      (1000)     6410 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/datatypes.py
--rw-rw-r--   0 test      (1000) test      (1000)     1528 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/decorators.py
--rw-rw-r--   0 test      (1000) test      (1000)    14775 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/defer.py
--rw-rw-r--   0 test      (1000) test      (1000)     6993 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/deprecate.py
--rw-rw-r--   0 test      (1000) test      (1000)     1455 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/display.py
--rw-rw-r--   0 test      (1000) test      (1000)     1540 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/engine.py
--rw-rw-r--   0 test      (1000) test      (1000)     1355 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/ftp.py
--rw-rw-r--   0 test      (1000) test      (1000)     1384 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/gz.py
--rw-rw-r--   0 test      (1000) test      (1000)      712 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/httpobj.py
--rw-rw-r--   0 test      (1000) test      (1000)     8225 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/iterators.py
--rw-rw-r--   0 test      (1000) test      (1000)      320 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/job.py
--rw-rw-r--   0 test      (1000) test      (1000)     7660 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/log.py
--rw-rw-r--   0 test      (1000) test      (1000)    10547 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/misc.py
--rw-rw-r--   0 test      (1000) test      (1000)     1243 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/ossignal.py
--rw-rw-r--   0 test      (1000) test      (1000)     2640 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/project.py
--rw-rw-r--   0 test      (1000) test      (1000)    10491 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/python.py
--rw-rw-r--   0 test      (1000) test      (1000)     7190 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/reactor.py
--rw-rw-r--   0 test      (1000) test      (1000)     8560 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/request.py
--rw-rw-r--   0 test      (1000) test      (1000)     3383 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/response.py
--rw-rw-r--   0 test      (1000) test      (1000)     1171 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/serialize.py
--rw-rw-r--   0 test      (1000) test      (1000)     3833 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/signal.py
--rw-rw-r--   0 test      (1000) test      (1000)     1713 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/sitemap.py
--rw-rw-r--   0 test      (1000) test      (1000)     3728 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/spider.py
--rw-rw-r--   0 test      (1000) test      (1000)     2441 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/ssl.py
--rw-rw-r--   0 test      (1000) test      (1000)      918 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/template.py
--rw-rw-r--   0 test      (1000) test      (1000)     4307 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/test.py
--rw-rw-r--   0 test      (1000) test      (1000)     2079 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/testproc.py
--rw-rw-r--   0 test      (1000) test      (1000)     1611 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/testsite.py
--rw-rw-r--   0 test      (1000) test      (1000)     2261 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/trackref.py
--rw-rw-r--   0 test      (1000) test      (1000)     6020 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/url.py
--rw-rw-r--   0 test      (1000) test      (1000)      915 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/scrapyy/utils/versions.py
--rw-rw-r--   0 test      (1000) test      (1000)      392 2024-04-19 09:39:45.017659 new_python_scrapy-0.1.1/setup.cfg
--rw-rw-r--   0 test      (1000) test      (1000)     1696 2024-04-19 09:38:56.000000 new_python_scrapy-0.1.1/setup.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:45.009659 new_python_scrapy-0.1.1/tests/
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:45.013659 new_python_scrapy-0.1.1/tests/CrawlerProcess/
--rw-rw-r--   0 test      (1000) test      (1000)      609 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/CrawlerProcess/args_settings.py
--rw-rw-r--   0 test      (1000) test      (1000)      399 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/CrawlerProcess/asyncio_custom_loop.py
--rw-rw-r--   0 test      (1000) test      (1000)     1173 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/CrawlerProcess/asyncio_deferred_signal.py
--rw-rw-r--   0 test      (1000) test      (1000)      354 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/CrawlerProcess/asyncio_enabled_no_reactor.py
--rw-rw-r--   0 test      (1000) test      (1000)      639 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/CrawlerProcess/asyncio_enabled_reactor.py
--rw-rw-r--   0 test      (1000) test      (1000)      741 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/CrawlerProcess/asyncio_enabled_reactor_different_loop.py
--rw-rw-r--   0 test      (1000) test      (1000)      739 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/CrawlerProcess/asyncio_enabled_reactor_same_loop.py
--rw-rw-r--   0 test      (1000) test      (1000)      913 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/CrawlerProcess/caching_hostname_resolver.py
--rw-rw-r--   0 test      (1000) test      (1000)      548 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/CrawlerProcess/caching_hostname_resolver_ipv6.py
--rw-rw-r--   0 test      (1000) test      (1000)      424 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/CrawlerProcess/default_name_resolver.py
--rw-rw-r--   0 test      (1000) test      (1000)      291 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/CrawlerProcess/multi.py
--rw-rw-r--   0 test      (1000) test      (1000)      311 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/CrawlerProcess/reactor_default.py
--rw-rw-r--   0 test      (1000) test      (1000)      454 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/CrawlerProcess/reactor_default_twisted_reactor_select.py
--rw-rw-r--   0 test      (1000) test      (1000)      328 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/CrawlerProcess/reactor_select.py
--rw-rw-r--   0 test      (1000) test      (1000)      624 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/CrawlerProcess/reactor_select_subclass_twisted_reactor_select.py
--rw-rw-r--   0 test      (1000) test      (1000)      414 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/CrawlerProcess/reactor_select_twisted_reactor_select.py
--rw-rw-r--   0 test      (1000) test      (1000)      259 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/CrawlerProcess/simple.py
--rw-rw-r--   0 test      (1000) test      (1000)      545 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/CrawlerProcess/sleeping.py
--rw-rw-r--   0 test      (1000) test      (1000)      318 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/CrawlerProcess/twisted_reactor_asyncio.py
--rw-rw-r--   0 test      (1000) test      (1000)      326 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/CrawlerProcess/twisted_reactor_custom_settings.py
--rw-rw-r--   0 test      (1000) test      (1000)      626 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/CrawlerProcess/twisted_reactor_custom_settings_conflict.py
--rw-rw-r--   0 test      (1000) test      (1000)      557 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/CrawlerProcess/twisted_reactor_custom_settings_same.py
--rw-rw-r--   0 test      (1000) test      (1000)      295 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/CrawlerProcess/twisted_reactor_poll.py
--rw-rw-r--   0 test      (1000) test      (1000)      304 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/CrawlerProcess/twisted_reactor_select.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:45.013659 new_python_scrapy-0.1.1/tests/CrawlerRunner/
--rw-rw-r--   0 test      (1000) test      (1000)     1855 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/CrawlerRunner/ip_address.py
--rw-rw-r--   0 test      (1000) test      (1000)     1287 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/__init__.py
--rw-rw-r--   0 test      (1000) test      (1000)      632 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/ftpserver.py
--rw-rw-r--   0 test      (1000) test      (1000)      103 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/ignores.txt
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:45.013659 new_python_scrapy-0.1.1/tests/keys/
--rw-rw-r--   0 test      (1000) test      (1000)     1867 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/keys/__init__.py
--rw-rw-r--   0 test      (1000) test      (1000)     1562 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/keys/example-com.cert.pem
--rw-rw-r--   0 test      (1000) test      (1000)     3126 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/keys/example-com.conf
--rw-rw-r--   0 test      (1000) test      (1000)      933 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/keys/example-com.gen.README
--rw-rw-r--   0 test      (1000) test      (1000)     1704 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/keys/example-com.key.pem
--rw-rw-r--   0 test      (1000) test      (1000)      945 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/keys/localhost-ip.gen.README
--rw-rw-r--   0 test      (1000) test      (1000)      945 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/keys/localhost.gen.README
--rw-rw-r--   0 test      (1000) test      (1000)     1176 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/keys/localhost.ip.crt
--rw-rw-r--   0 test      (1000) test      (1000)     1704 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/keys/localhost.ip.key
--rw-rw-r--   0 test      (1000) test      (1000)     2847 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/keys/mitmproxy-ca.pem
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:45.013659 new_python_scrapy-0.1.1/tests/mocks/
--rw-rw-r--   0 test      (1000) test      (1000)        0 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/mocks/__init__.py
--rw-rw-r--   0 test      (1000) test      (1000)      507 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/mocks/dummydbm.py
--rw-rw-r--   0 test      (1000) test      (1000)    12662 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/mockserver.py
--rw-rw-r--   0 test      (1000) test      (1000)      289 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/pipelines.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:44.969659 new_python_scrapy-0.1.1/tests/sample_data/
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:45.013659 new_python_scrapy-0.1.1/tests/sample_data/compressed/
--rw-rw-r--   0 test      (1000) test      (1000)       34 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/compressed/bomb-br.bin
--rw-rw-r--   0 test      (1000) test      (1000)    27968 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/compressed/bomb-deflate.bin
--rw-rw-r--   0 test      (1000) test      (1000)    27988 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/compressed/bomb-gzip.bin
--rw-rw-r--   0 test      (1000) test      (1000)     1096 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/compressed/bomb-zstd.bin
--rw-rw-r--   0 test      (1000) test      (1000)    20480 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/compressed/feed-sample1.tar
--rw-rw-r--   0 test      (1000) test      (1000)     9950 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/compressed/feed-sample1.xml
--rw-rw-r--   0 test      (1000) test      (1000)     1430 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/compressed/feed-sample1.xml.bz2
--rw-rw-r--   0 test      (1000) test      (1000)     1131 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/compressed/feed-sample1.xml.gz
--rw-rw-r--   0 test      (1000) test      (1000)     1260 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/compressed/feed-sample1.zip
--rw-rw-r--   0 test      (1000) test      (1000)     4027 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/compressed/html-br.bin
--rw-rw-r--   0 test      (1000) test      (1000)     8014 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/compressed/html-gzip-deflate-gzip.bin
--rw-rw-r--   0 test      (1000) test      (1000)     7991 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/compressed/html-gzip-deflate.bin
--rw-rw-r--   0 test      (1000) test      (1000)     8037 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/compressed/html-gzip.bin
--rw-rw-r--   0 test      (1000) test      (1000)     8021 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/compressed/html-rawdeflate.bin
--rw-rw-r--   0 test      (1000) test      (1000)     8027 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/compressed/html-zlibdeflate.bin
--rw-rw-r--   0 test      (1000) test      (1000)     8066 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/compressed/html-zstd-static-content-size.bin
--rw-rw-r--   0 test      (1000) test      (1000)     8063 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/compressed/html-zstd-static-no-content-size.bin
--rw-rw-r--   0 test      (1000) test      (1000)     8047 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/compressed/html-zstd-streaming-no-content-size.bin
--rw-rw-r--   0 test      (1000) test      (1000)     1930 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/compressed/truncated-crc-error-short.gz
--rw-rw-r--   0 test      (1000) test      (1000)     5766 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/compressed/truncated-crc-error.gz
--rw-rw-r--   0 test      (1000) test      (1000)    16782 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/compressed/unexpected-eof-output.txt
--rw-rw-r--   0 test      (1000) test      (1000)     5134 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/compressed/unexpected-eof.gz
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:45.013659 new_python_scrapy-0.1.1/tests/sample_data/feeds/
--rw-rw-r--   0 test      (1000) test      (1000)     9950 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/feeds/feed-sample1.xml
--rw-rw-r--   0 test      (1000) test      (1000)     6388 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/feeds/feed-sample2.xml
--rw-rw-r--   0 test      (1000) test      (1000)       81 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/feeds/feed-sample3.csv
--rw-rw-r--   0 test      (1000) test      (1000)       45 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/feeds/feed-sample4.csv
--rw-rw-r--   0 test      (1000) test      (1000)       47 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/feeds/feed-sample5.csv
--rw-rw-r--   0 test      (1000) test      (1000)      101 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/feeds/feed-sample6.csv
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:45.017659 new_python_scrapy-0.1.1/tests/sample_data/link_extractor/
--rw-rw-r--   0 test      (1000) test      (1000)      830 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/link_extractor/linkextractor.html
--rw-rw-r--   0 test      (1000) test      (1000)      585 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/link_extractor/linkextractor_latin1.html
--rw-rw-r--   0 test      (1000) test      (1000)      740 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/link_extractor/linkextractor_no_href.html
--rw-rw-r--   0 test      (1000) test      (1000)      390 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/link_extractor/linkextractor_noenc.html
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:45.017659 new_python_scrapy-0.1.1/tests/sample_data/test_site/
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:44.969659 new_python_scrapy-0.1.1/tests/sample_data/test_site/files/
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:45.017659 new_python_scrapy-0.1.1/tests/sample_data/test_site/files/images/
--rw-rw-r--   0 test      (1000) test      (1000)    11155 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/test_site/files/images/python-logo-master-v3-TM-flattened.png
--rw-rw-r--   0 test      (1000) test      (1000)     3243 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/test_site/files/images/python-powered-h-50x65.png
--rw-rw-r--   0 test      (1000) test      (1000)     2710 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/test_site/files/images/scrapy.png
--rw-rw-r--   0 test      (1000) test      (1000)      311 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/test_site/index.html
--rw-rw-r--   0 test      (1000) test      (1000)      225 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/test_site/item1.html
--rw-rw-r--   0 test      (1000) test      (1000)      209 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/sample_data/test_site/item2.html
--rw-rw-r--   0 test      (1000) test      (1000)    15603 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/spiders.py
--rw-rw-r--   0 test      (1000) test      (1000)     7406 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_addons.py
--rw-rw-r--   0 test      (1000) test      (1000)     2843 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_closespider.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:45.017659 new_python_scrapy-0.1.1/tests/test_cmdline/
--rw-rw-r--   0 test      (1000) test      (1000)     2670 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_cmdline/__init__.py
--rw-rw-r--   0 test      (1000) test      (1000)      309 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_cmdline/extensions.py
--rw-rw-r--   0 test      (1000) test      (1000)      223 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_cmdline/settings.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:45.017659 new_python_scrapy-0.1.1/tests/test_cmdline_crawl_with_pipeline/
--rw-rw-r--   0 test      (1000) test      (1000)      632 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_cmdline_crawl_with_pipeline/__init__.py
--rw-rw-r--   0 test      (1000) test      (1000)       42 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_cmdline_crawl_with_pipeline/scrapy.cfg
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:45.017659 new_python_scrapy-0.1.1/tests/test_cmdline_crawl_with_pipeline/test_spider/
--rw-rw-r--   0 test      (1000) test      (1000)        0 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_cmdline_crawl_with_pipeline/test_spider/__init__.py
--rw-rw-r--   0 test      (1000) test      (1000)      309 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_cmdline_crawl_with_pipeline/test_spider/pipelines.py
--rw-rw-r--   0 test      (1000) test      (1000)       66 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_cmdline_crawl_with_pipeline/test_spider/settings.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:45.017659 new_python_scrapy-0.1.1/tests/test_cmdline_crawl_with_pipeline/test_spider/spiders/
--rw-rw-r--   0 test      (1000) test      (1000)        0 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_cmdline_crawl_with_pipeline/test_spider/spiders/__init__.py
--rw-rw-r--   0 test      (1000) test      (1000)      238 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_cmdline_crawl_with_pipeline/test_spider/spiders/exception.py
--rw-rw-r--   0 test      (1000) test      (1000)      223 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_cmdline_crawl_with_pipeline/test_spider/spiders/normal.py
--rw-rw-r--   0 test      (1000) test      (1000)     6871 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_command_check.py
--rw-rw-r--   0 test      (1000) test      (1000)     1242 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_command_fetch.py
--rw-rw-r--   0 test      (1000) test      (1000)    14538 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_command_parse.py
--rw-rw-r--   0 test      (1000) test      (1000)     5954 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_command_shell.py
--rw-rw-r--   0 test      (1000) test      (1000)     1198 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_command_version.py
--rw-rw-r--   0 test      (1000) test      (1000)    39524 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_commands.py
--rw-rw-r--   0 test      (1000) test      (1000)    13668 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_contracts.py
--rw-rw-r--   0 test      (1000) test      (1000)      350 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_core_downloader.py
--rw-rw-r--   0 test      (1000) test      (1000)    27668 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_crawl.py
--rw-rw-r--   0 test      (1000) test      (1000)    32765 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_crawler.py
--rw-rw-r--   0 test      (1000) test      (1000)     1457 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_dependencies.py
--rw-rw-r--   0 test      (1000) test      (1000)    46807 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_downloader_handlers.py
--rw-rw-r--   0 test      (1000) test      (1000)     9270 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_downloader_handlers_http2.py
--rw-rw-r--   0 test      (1000) test      (1000)     9307 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_downloadermiddleware.py
--rw-rw-r--   0 test      (1000) test      (1000)     2541 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_downloadermiddleware_ajaxcrawlable.py
--rw-rw-r--   0 test      (1000) test      (1000)    28199 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_downloadermiddleware_cookies.py
--rw-rw-r--   0 test      (1000) test      (1000)     1397 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_downloadermiddleware_defaultheaders.py
--rw-rw-r--   0 test      (1000) test      (1000)     1701 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_downloadermiddleware_downloadtimeout.py
--rw-rw-r--   0 test      (1000) test      (1000)     2658 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_downloadermiddleware_httpauth.py
--rw-rw-r--   0 test      (1000) test      (1000)    25829 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_downloadermiddleware_httpcache.py
--rw-rw-r--   0 test      (1000) test      (1000)    28941 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_downloadermiddleware_httpcompression.py
--rw-rw-r--   0 test      (1000) test      (1000)    19971 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_downloadermiddleware_httpproxy.py
--rw-rw-r--   0 test      (1000) test      (1000)    16631 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_downloadermiddleware_redirect.py
--rw-rw-r--   0 test      (1000) test      (1000)    23673 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_downloadermiddleware_retry.py
--rw-rw-r--   0 test      (1000) test      (1000)    10222 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_downloadermiddleware_robotstxt.py
--rw-rw-r--   0 test      (1000) test      (1000)     1597 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_downloadermiddleware_stats.py
--rw-rw-r--   0 test      (1000) test      (1000)     2227 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_downloadermiddleware_useragent.py
--rw-rw-r--   0 test      (1000) test      (1000)     3162 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_downloaderslotssettings.py
--rw-rw-r--   0 test      (1000) test      (1000)     9493 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_dupefilters.py
--rw-rw-r--   0 test      (1000) test      (1000)    16283 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_engine.py
--rw-rw-r--   0 test      (1000) test      (1000)     2966 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_engine_stop_download_bytes.py
--rw-rw-r--   0 test      (1000) test      (1000)     2709 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_engine_stop_download_headers.py
--rw-rw-r--   0 test      (1000) test      (1000)    23999 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_exporters.py
--rw-rw-r--   0 test      (1000) test      (1000)     6672 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_extension_periodic_log.py
--rw-rw-r--   0 test      (1000) test      (1000)     1833 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_extension_telnet.py
--rw-rw-r--   0 test      (1000) test      (1000)    10434 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_extension_throttle.py
--rw-rw-r--   0 test      (1000) test      (1000)   103071 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_feedexport.py
--rw-rw-r--   0 test      (1000) test      (1000)    24639 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_http2_client_protocol.py
--rw-rw-r--   0 test      (1000) test      (1000)     2878 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_http_cookies.py
--rw-rw-r--   0 test      (1000) test      (1000)     6251 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_http_headers.py
--rw-rw-r--   0 test      (1000) test      (1000)    68129 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_http_request.py
--rw-rw-r--   0 test      (1000) test      (1000)    39823 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_http_response.py
--rw-rw-r--   0 test      (1000) test      (1000)     9066 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_item.py
--rw-rw-r--   0 test      (1000) test      (1000)     1900 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_link.py
--rw-rw-r--   0 test      (1000) test      (1000)    33344 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_linkextractors.py
--rw-rw-r--   0 test      (1000) test      (1000)    21184 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_loader.py
--rw-rw-r--   0 test      (1000) test      (1000)    25781 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_loader_deprecated.py
--rw-rw-r--   0 test      (1000) test      (1000)     8853 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_logformatter.py
--rw-rw-r--   0 test      (1000) test      (1000)     2530 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_logstats.py
--rw-rw-r--   0 test      (1000) test      (1000)     5768 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_mail.py
--rw-rw-r--   0 test      (1000) test      (1000)     2346 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_middleware.py
--rw-rw-r--   0 test      (1000) test      (1000)     8605 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_pipeline_crawl.py
--rw-rw-r--   0 test      (1000) test      (1000)    25239 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_pipeline_files.py
--rw-rw-r--   0 test      (1000) test      (1000)    25719 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_pipeline_images.py
--rw-rw-r--   0 test      (1000) test      (1000)    18445 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_pipeline_media.py
--rw-rw-r--   0 test      (1000) test      (1000)     3893 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_pipelines.py
--rw-rw-r--   0 test      (1000) test      (1000)     6200 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_pqueues.py
--rw-rw-r--   0 test      (1000) test      (1000)     3864 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_proxy_connect.py
--rw-rw-r--   0 test      (1000) test      (1000)     7644 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_request_attribute_binding.py
--rw-rw-r--   0 test      (1000) test      (1000)     7512 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_request_cb_kwargs.py
--rw-rw-r--   0 test      (1000) test      (1000)     6943 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_request_dict.py
--rw-rw-r--   0 test      (1000) test      (1000)     1931 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_request_left.py
--rw-rw-r--   0 test      (1000) test      (1000)     5122 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_responsetypes.py
--rw-rw-r--   0 test      (1000) test      (1000)     8062 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_robotstxt_interface.py
--rw-rw-r--   0 test      (1000) test      (1000)    10774 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_scheduler.py
--rw-rw-r--   0 test      (1000) test      (1000)     5505 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_scheduler_base.py
--rw-rw-r--   0 test      (1000) test      (1000)     9412 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_selector.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:45.017659 new_python_scrapy-0.1.1/tests/test_settings/
--rw-rw-r--   0 test      (1000) test      (1000)    20083 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_settings/__init__.py
--rw-rw-r--   0 test      (1000) test      (1000)       54 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_settings/default_settings.py
--rw-rw-r--   0 test      (1000) test      (1000)     1339 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_signals.py
--rw-rw-r--   0 test      (1000) test      (1000)    31192 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_spider.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:45.017659 new_python_scrapy-0.1.1/tests/test_spiderloader/
--rw-rw-r--   0 test      (1000) test      (1000)     7774 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_spiderloader/__init__.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:45.017659 new_python_scrapy-0.1.1/tests/test_spiderloader/test_spiders/
--rw-rw-r--   0 test      (1000) test      (1000)        0 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_spiderloader/test_spiders/__init__.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:45.017659 new_python_scrapy-0.1.1/tests/test_spiderloader/test_spiders/nested/
--rw-rw-r--   0 test      (1000) test      (1000)        0 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_spiderloader/test_spiders/nested/__init__.py
--rw-rw-r--   0 test      (1000) test      (1000)      235 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_spiderloader/test_spiders/nested/spider4.py
--rw-rw-r--   0 test      (1000) test      (1000)      112 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_spiderloader/test_spiders/spider0.py
--rw-rw-r--   0 test      (1000) test      (1000)      133 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_spiderloader/test_spiders/spider1.py
--rw-rw-r--   0 test      (1000) test      (1000)      133 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_spiderloader/test_spiders/spider2.py
--rw-rw-r--   0 test      (1000) test      (1000)      235 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_spiderloader/test_spiders/spider3.py
--rw-rw-r--   0 test      (1000) test      (1000)    19879 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_spidermiddleware.py
--rw-rw-r--   0 test      (1000) test      (1000)     1342 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_spidermiddleware_depth.py
--rw-rw-r--   0 test      (1000) test      (1000)     9286 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_spidermiddleware_httperror.py
--rw-rw-r--   0 test      (1000) test      (1000)     3725 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_spidermiddleware_offsite.py
--rw-rw-r--   0 test      (1000) test      (1000)    19049 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_spidermiddleware_output_chain.py
--rw-rw-r--   0 test      (1000) test      (1000)    44049 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_spidermiddleware_referer.py
--rw-rw-r--   0 test      (1000) test      (1000)     1495 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_spidermiddleware_urllength.py
--rw-rw-r--   0 test      (1000) test      (1000)     1433 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_spiderstate.py
--rw-rw-r--   0 test      (1000) test      (1000)     5229 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_squeues.py
--rw-rw-r--   0 test      (1000) test      (1000)     7604 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_squeues_request.py
--rw-rw-r--   0 test      (1000) test      (1000)     3993 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_stats.py
--rw-rw-r--   0 test      (1000) test      (1000)      869 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_toplevel.py
--rw-rw-r--   0 test      (1000) test      (1000)      362 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_urlparse_monkeypatches.py
--rw-rw-r--   0 test      (1000) test      (1000)      663 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_utils_asyncgen.py
--rw-rw-r--   0 test      (1000) test      (1000)     1204 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_utils_asyncio.py
--rw-rw-r--   0 test      (1000) test      (1000)     8822 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_utils_conf.py
--rw-rw-r--   0 test      (1000) test      (1000)     1173 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_utils_console.py
--rw-rw-r--   0 test      (1000) test      (1000)    10221 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_utils_curl.py
--rw-rw-r--   0 test      (1000) test      (1000)    11322 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_utils_datatypes.py
--rw-rw-r--   0 test      (1000) test      (1000)     7611 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_utils_defer.py
--rw-rw-r--   0 test      (1000) test      (1000)    10343 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_utils_deprecate.py
--rw-rw-r--   0 test      (1000) test      (1000)     3204 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_utils_display.py
--rw-rw-r--   0 test      (1000) test      (1000)     1909 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_utils_gz.py
--rw-rw-r--   0 test      (1000) test      (1000)      685 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_utils_httpobj.py
--rw-rw-r--   0 test      (1000) test      (1000)    21676 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_utils_iterators.py
--rw-rw-r--   0 test      (1000) test      (1000)     3576 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_utils_log.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:45.017659 new_python_scrapy-0.1.1/tests/test_utils_misc/
--rw-rw-r--   0 test      (1000) test      (1000)    10121 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_utils_misc/__init__.py
--rw-rw-r--   0 test      (1000) test      (1000)     2231 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_utils_misc/test.egg
--rw-rw-r--   0 test      (1000) test      (1000)     8263 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_utils_misc/test_return_with_argument_inside_generator.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:45.017659 new_python_scrapy-0.1.1/tests/test_utils_misc/test_walk_modules/
--rw-rw-r--   0 test      (1000) test      (1000)        0 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_utils_misc/test_walk_modules/__init__.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 09:39:45.017659 new_python_scrapy-0.1.1/tests/test_utils_misc/test_walk_modules/mod/
--rw-rw-r--   0 test      (1000) test      (1000)        0 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_utils_misc/test_walk_modules/mod/__init__.py
--rw-rw-r--   0 test      (1000) test      (1000)        0 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_utils_misc/test_walk_modules/mod/mod0.py
--rw-rw-r--   0 test      (1000) test      (1000)        0 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_utils_misc/test_walk_modules/mod1.py
--rw-rw-r--   0 test      (1000) test      (1000)     2598 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_utils_project.py
--rw-rw-r--   0 test      (1000) test      (1000)     7970 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_utils_python.py
--rw-rw-r--   0 test      (1000) test      (1000)    17748 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_utils_request.py
--rw-rw-r--   0 test      (1000) test      (1000)     7540 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_utils_response.py
--rw-rw-r--   0 test      (1000) test      (1000)     2488 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_utils_serialize.py
--rw-rw-r--   0 test      (1000) test      (1000)     3376 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_utils_signal.py
--rw-rw-r--   0 test      (1000) test      (1000)     9009 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_utils_sitemap.py
--rw-rw-r--   0 test      (1000) test      (1000)      995 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_utils_spider.py
--rw-rw-r--   0 test      (1000) test      (1000)     1187 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_utils_template.py
--rw-rw-r--   0 test      (1000) test      (1000)     2152 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_utils_trackref.py
--rw-rw-r--   0 test      (1000) test      (1000)    22563 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_utils_url.py
--rw-rw-r--   0 test      (1000) test      (1000)    17220 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/test_webclient.py
--rw-rw-r--   0 test      (1000) test      (1000)      412 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tests/upper-constraints.txt
--rw-rw-r--   0 test      (1000) test      (1000)     6105 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.1/tox.ini
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.166803 new_python_scrapy-0.1.2/
+-rw-rw-r--   0 test      (1000) test      (1000)     1284 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/AUTHORS
+-rw-rw-r--   0 test      (1000) test      (1000)     1517 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/LICENSE
+-rw-rw-r--   0 test      (1000) test      (1000)      510 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/MANIFEST.in
+-rw-rw-r--   0 test      (1000) test      (1000)       18 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/NEWS
+-rw-r--r--   0 test      (1000) test      (1000)      693 2024-04-19 10:11:41.166803 new_python_scrapy-0.1.2/PKG-INFO
+-rw-rw-r--   0 test      (1000) test      (1000)     3117 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/README.rst
+-rw-rw-r--   0 test      (1000) test      (1000)       80 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/codecov.yml
+-rw-rw-r--   0 test      (1000) test      (1000)     2574 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/conftest.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.090799 new_python_scrapy-0.1.2/docs/
+-rw-rw-r--   0 test      (1000) test      (1000)     2829 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/Makefile
+-rw-rw-r--   0 test      (1000) test      (1000)     1581 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/README.rst
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.094800 new_python_scrapy-0.1.2/docs/_ext/
+-rw-rw-r--   0 test      (1000) test      (1000)     4516 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/_ext/scrapydocs.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.098800 new_python_scrapy-0.1.2/docs/_static/
+-rw-rw-r--   0 test      (1000) test      (1000)      360 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/_static/custom.css
+-rw-rw-r--   0 test      (1000) test      (1000)      667 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/_static/selectors-sample1.html
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.102800 new_python_scrapy-0.1.2/docs/_tests/
+-rw-rw-r--   0 test      (1000) test      (1000)    11043 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/_tests/quotes.html
+-rw-rw-r--   0 test      (1000) test      (1000)    11043 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/_tests/quotes1.html
+-rw-rw-r--   0 test      (1000) test      (1000)    10944 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/conf.py
+-rw-rw-r--   0 test      (1000) test      (1000)      921 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/conftest.py
+-rw-rw-r--   0 test      (1000) test      (1000)    13224 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/contributing.rst
+-rw-rw-r--   0 test      (1000) test      (1000)    16563 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/faq.rst
+-rw-rw-r--   0 test      (1000) test      (1000)     6876 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/index.rst
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.102800 new_python_scrapy-0.1.2/docs/intro/
+-rw-rw-r--   0 test      (1000) test      (1000)      745 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/intro/examples.rst
+-rw-rw-r--   0 test      (1000) test      (1000)    10323 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/intro/install.rst
+-rw-rw-r--   0 test      (1000) test      (1000)     6671 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/intro/overview.rst
+-rw-rw-r--   0 test      (1000) test      (1000)    30811 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/intro/tutorial.rst
+-rw-rw-r--   0 test      (1000) test      (1000)   263677 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/news.rst
+-rw-rw-r--   0 test      (1000) test      (1000)       90 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/requirements.txt
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.114800 new_python_scrapy-0.1.2/docs/topics/
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.114800 new_python_scrapy-0.1.2/docs/topics/_images/
+-rw-rw-r--   0 test      (1000) test      (1000)    53922 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/_images/inspector_01.png
+-rw-rw-r--   0 test      (1000) test      (1000)    10720 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/_images/network_01.png
+-rw-rw-r--   0 test      (1000) test      (1000)    82702 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/_images/network_02.png
+-rw-rw-r--   0 test      (1000) test      (1000)    45506 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/_images/network_03.png
+-rw-rw-r--   0 test      (1000) test      (1000)    19653 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/_images/scrapy_architecture.odg
+-rw-rw-r--   0 test      (1000) test      (1000)    92558 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/_images/scrapy_architecture.png
+-rw-rw-r--   0 test      (1000) test      (1000)    53978 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/_images/scrapy_architecture_02.png
+-rw-rw-r--   0 test      (1000) test      (1000)     6785 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/addons.rst
+-rw-rw-r--   0 test      (1000) test      (1000)     8348 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/api.rst
+-rw-rw-r--   0 test      (1000) test      (1000)     6114 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/architecture.rst
+-rw-rw-r--   0 test      (1000) test      (1000)     4983 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/asyncio.rst
+-rw-rw-r--   0 test      (1000) test      (1000)     6277 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/autothrottle.rst
+-rw-rw-r--   0 test      (1000) test      (1000)     5257 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/benchmarking.rst
+-rw-rw-r--   0 test      (1000) test      (1000)     8436 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/broad-crawls.rst
+-rw-rw-r--   0 test      (1000) test      (1000)    17953 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/commands.rst
+-rw-rw-r--   0 test      (1000) test      (1000)     2758 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/components.rst
+-rw-rw-r--   0 test      (1000) test      (1000)     4976 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/contracts.rst
+-rw-rw-r--   0 test      (1000) test      (1000)    10376 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/coroutines.rst
+-rw-rw-r--   0 test      (1000) test      (1000)     5233 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/debug.rst
+-rw-rw-r--   0 test      (1000) test      (1000)     2263 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/deploy.rst
+-rw-rw-r--   0 test      (1000) test      (1000)    13859 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/developer-tools.rst
+-rw-rw-r--   0 test      (1000) test      (1000)      194 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/djangoitem.rst
+-rw-rw-r--   0 test      (1000) test      (1000)    41078 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/downloader-middleware.rst
+-rw-rw-r--   0 test      (1000) test      (1000)    12165 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/dynamic-content.rst
+-rw-rw-r--   0 test      (1000) test      (1000)     5110 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/email.rst
+-rw-rw-r--   0 test      (1000) test      (1000)     3253 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/exceptions.rst
+-rw-rw-r--   0 test      (1000) test      (1000)    15581 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/exporters.rst
+-rw-rw-r--   0 test      (1000) test      (1000)    16702 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/extensions.rst
+-rw-rw-r--   0 test      (1000) test      (1000)    24592 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/feed-exports.rst
+-rw-rw-r--   0 test      (1000) test      (1000)     8751 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/item-pipeline.rst
+-rw-rw-r--   0 test      (1000) test      (1000)    11569 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/items.rst
+-rw-rw-r--   0 test      (1000) test      (1000)     2904 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/jobs.rst
+-rw-rw-r--   0 test      (1000) test      (1000)    11883 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/leaks.rst
+-rw-rw-r--   0 test      (1000) test      (1000)     6858 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/link-extractors.rst
+-rw-rw-r--   0 test      (1000) test      (1000)    16958 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/loaders.rst
+-rw-rw-r--   0 test      (1000) test      (1000)    10990 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/logging.rst
+-rw-rw-r--   0 test      (1000) test      (1000)    26720 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/media-pipeline.rst
+-rw-rw-r--   0 test      (1000) test      (1000)    10607 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/practices.rst
+-rw-rw-r--   0 test      (1000) test      (1000)    48143 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/request-response.rst
+-rw-rw-r--   0 test      (1000) test      (1000)      761 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/scheduler.rst
+-rw-rw-r--   0 test      (1000) test      (1000)      188 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/scrapyd.rst
+-rw-rw-r--   0 test      (1000) test      (1000)    37984 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/selectors.rst
+-rw-rw-r--   0 test      (1000) test      (1000)    52593 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/settings.rst
+-rw-rw-r--   0 test      (1000) test      (1000)    11101 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/shell.rst
+-rw-rw-r--   0 test      (1000) test      (1000)    16976 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/signals.rst
+-rw-rw-r--   0 test      (1000) test      (1000)    19050 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/spider-middleware.rst
+-rw-rw-r--   0 test      (1000) test      (1000)    35299 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/spiders.rst
+-rw-rw-r--   0 test      (1000) test      (1000)     3713 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/stats.rst
+-rw-rw-r--   0 test      (1000) test      (1000)     7468 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/topics/telnetconsole.rst
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.114800 new_python_scrapy-0.1.2/docs/utils/
+-rw-rw-r--   0 test      (1000) test      (1000)     1975 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/utils/linkfix.py
+-rw-rw-r--   0 test      (1000) test      (1000)     2161 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/docs/versioning.rst
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.114800 new_python_scrapy-0.1.2/extras/
+-rwxrwxr-x   0 test      (1000) test      (1000)      259 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/extras/coverage-report.sh
+-rwxrwxr-x   0 test      (1000) test      (1000)     1618 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/extras/qps-bench-server.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1507 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/extras/qpsclient.py
+-rw-rw-r--   0 test      (1000) test      (1000)     2010 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/extras/scrapy.1
+-rw-rw-r--   0 test      (1000) test      (1000)      698 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/extras/scrapy_bash_completion
+-rw-rw-r--   0 test      (1000) test      (1000)     7008 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/extras/scrapy_zsh_completion
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.166803 new_python_scrapy-0.1.2/new_python_scrapy.egg-info/
+-rw-r--r--   0 test      (1000) test      (1000)      693 2024-04-19 10:11:41.000000 new_python_scrapy-0.1.2/new_python_scrapy.egg-info/PKG-INFO
+-rw-rw-r--   0 test      (1000) test      (1000)    15456 2024-04-19 10:11:41.000000 new_python_scrapy-0.1.2/new_python_scrapy.egg-info/SOURCES.txt
+-rw-rw-r--   0 test      (1000) test      (1000)        1 2024-04-19 10:11:41.000000 new_python_scrapy-0.1.2/new_python_scrapy.egg-info/dependency_links.txt
+-rw-rw-r--   0 test      (1000) test      (1000)        8 2024-04-19 10:11:41.000000 new_python_scrapy-0.1.2/new_python_scrapy.egg-info/top_level.txt
+-rw-rw-r--   0 test      (1000) test      (1000)     1000 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/pytest.ini
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.118800 new_python_scrapy-0.1.2/scrapyy/
+-rw-rw-r--   0 test      (1000) test      (1000)     1071 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/__init__.py
+-rw-rw-r--   0 test      (1000) test      (1000)       77 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/__main__.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1837 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/addons.py
+-rw-rw-r--   0 test      (1000) test      (1000)     5757 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/cmdline.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.118800 new_python_scrapy-0.1.2/scrapyy/commands/
+-rw-rw-r--   0 test      (1000) test      (1000)     7481 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/commands/__init__.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1930 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/commands/bench.py
+-rw-rw-r--   0 test      (1000) test      (1000)     3836 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/commands/check.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1273 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/commands/crawl.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1239 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/commands/edit.py
+-rw-rw-r--   0 test      (1000) test      (1000)     3150 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/commands/fetch.py
+-rw-rw-r--   0 test      (1000) test      (1000)     7057 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/commands/genspider.py
+-rw-rw-r--   0 test      (1000) test      (1000)      459 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/commands/list.py
+-rw-rw-r--   0 test      (1000) test      (1000)    13974 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/commands/parse.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1943 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/commands/runspider.py
+-rw-rw-r--   0 test      (1000) test      (1000)     2046 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/commands/settings.py
+-rw-rw-r--   0 test      (1000) test      (1000)     3187 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/commands/shell.py
+-rw-rw-r--   0 test      (1000) test      (1000)     4635 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/commands/startproject.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1092 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/commands/version.py
+-rw-rw-r--   0 test      (1000) test      (1000)      892 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/commands/view.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.118800 new_python_scrapy-0.1.2/scrapyy/contracts/
+-rw-rw-r--   0 test      (1000) test      (1000)     6724 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/contracts/__init__.py
+-rw-rw-r--   0 test      (1000) test      (1000)     2946 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/contracts/default.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.122801 new_python_scrapy-0.1.2/scrapyy/core/
+-rw-rw-r--   0 test      (1000) test      (1000)       51 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/core/__init__.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.122801 new_python_scrapy-0.1.2/scrapyy/core/downloader/
+-rw-rw-r--   0 test      (1000) test      (1000)     9107 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/core/downloader/__init__.py
+-rw-rw-r--   0 test      (1000) test      (1000)     6768 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/core/downloader/contextfactory.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.122801 new_python_scrapy-0.1.2/scrapyy/core/downloader/handlers/
+-rw-rw-r--   0 test      (1000) test      (1000)     3351 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/core/downloader/handlers/__init__.py
+-rw-rw-r--   0 test      (1000) test      (1000)      795 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/core/downloader/handlers/datauri.py
+-rw-rw-r--   0 test      (1000) test      (1000)      479 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/core/downloader/handlers/file.py
+-rw-rw-r--   0 test      (1000) test      (1000)     4638 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/core/downloader/handlers/ftp.py
+-rw-rw-r--   0 test      (1000) test      (1000)      178 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/core/downloader/handlers/http.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1302 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/core/downloader/handlers/http10.py
+-rw-rw-r--   0 test      (1000) test      (1000)    24230 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/core/downloader/handlers/http11.py
+-rw-rw-r--   0 test      (1000) test      (1000)     4410 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/core/downloader/handlers/http2.py
+-rw-rw-r--   0 test      (1000) test      (1000)     2969 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/core/downloader/handlers/s3.py
+-rw-rw-r--   0 test      (1000) test      (1000)     4286 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/core/downloader/middleware.py
+-rw-rw-r--   0 test      (1000) test      (1000)     3253 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/core/downloader/tls.py
+-rw-rw-r--   0 test      (1000) test      (1000)     8460 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/core/downloader/webclient.py
+-rw-rw-r--   0 test      (1000) test      (1000)    17068 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/core/engine.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.122801 new_python_scrapy-0.1.2/scrapyy/core/http2/
+-rw-rw-r--   0 test      (1000) test      (1000)        0 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/core/http2/__init__.py
+-rw-rw-r--   0 test      (1000) test      (1000)     6042 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/core/http2/agent.py
+-rw-rw-r--   0 test      (1000) test      (1000)    17089 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/core/http2/protocol.py
+-rw-rw-r--   0 test      (1000) test      (1000)    19199 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/core/http2/stream.py
+-rw-rw-r--   0 test      (1000) test      (1000)    14514 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/core/scheduler.py
+-rw-rw-r--   0 test      (1000) test      (1000)    14449 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/core/scraper.py
+-rw-rw-r--   0 test      (1000) test      (1000)    14575 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/core/spidermw.py
+-rw-rw-r--   0 test      (1000) test      (1000)    17730 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/crawler.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.122801 new_python_scrapy-0.1.2/scrapyy/downloadermiddlewares/
+-rw-rw-r--   0 test      (1000) test      (1000)        0 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/downloadermiddlewares/__init__.py
+-rw-rw-r--   0 test      (1000) test      (1000)     3737 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/downloadermiddlewares/ajaxcrawl.py
+-rw-rw-r--   0 test      (1000) test      (1000)     6135 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/downloadermiddlewares/cookies.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1009 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/downloadermiddlewares/defaultheaders.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1093 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/downloadermiddlewares/downloadtimeout.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1484 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/downloadermiddlewares/httpauth.py
+-rw-rw-r--   0 test      (1000) test      (1000)     5724 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/downloadermiddlewares/httpcache.py
+-rw-rw-r--   0 test      (1000) test      (1000)     6932 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/downloadermiddlewares/httpcompression.py
+-rw-rw-r--   0 test      (1000) test      (1000)     3783 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/downloadermiddlewares/httpproxy.py
+-rw-rw-r--   0 test      (1000) test      (1000)     6297 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/downloadermiddlewares/redirect.py
+-rw-rw-r--   0 test      (1000) test      (1000)     7748 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/downloadermiddlewares/retry.py
+-rw-rw-r--   0 test      (1000) test      (1000)     5548 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/downloadermiddlewares/robotstxt.py
+-rw-rw-r--   0 test      (1000) test      (1000)     2881 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/downloadermiddlewares/stats.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1125 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/downloadermiddlewares/useragent.py
+-rw-rw-r--   0 test      (1000) test      (1000)     3627 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/dupefilters.py
+-rw-rw-r--   0 test      (1000) test      (1000)     2033 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/exceptions.py
+-rw-rw-r--   0 test      (1000) test      (1000)    13928 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/exporters.py
+-rw-rw-r--   0 test      (1000) test      (1000)      397 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/extension.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.134801 new_python_scrapy-0.1.2/scrapyy/extensions/
+-rw-rw-r--   0 test      (1000) test      (1000)        0 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/extensions/__init__.py
+-rw-rw-r--   0 test      (1000) test      (1000)     4910 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/extensions/closespider.py
+-rw-rw-r--   0 test      (1000) test      (1000)     2394 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/extensions/corestats.py
+-rw-rw-r--   0 test      (1000) test      (1000)     2285 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/extensions/debug.py
+-rw-rw-r--   0 test      (1000) test      (1000)    24676 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/extensions/feedexport.py
+-rw-rw-r--   0 test      (1000) test      (1000)    14805 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/extensions/httpcache.py
+-rw-rw-r--   0 test      (1000) test      (1000)     3277 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/extensions/logstats.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1326 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/extensions/memdebug.py
+-rw-rw-r--   0 test      (1000) test      (1000)     5951 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/extensions/memusage.py
+-rw-rw-r--   0 test      (1000) test      (1000)     5570 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/extensions/periodic_log.py
+-rw-rw-r--   0 test      (1000) test      (1000)     4933 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/extensions/postprocessing.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1641 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/extensions/spiderstate.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1726 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/extensions/statsmailer.py
+-rw-rw-r--   0 test      (1000) test      (1000)     4493 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/extensions/telnet.py
+-rw-rw-r--   0 test      (1000) test      (1000)     4653 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/extensions/throttle.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.134801 new_python_scrapy-0.1.2/scrapyy/http/
+-rw-rw-r--   0 test      (1000) test      (1000)      651 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/http/__init__.py
+-rw-rw-r--   0 test      (1000) test      (1000)     6014 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/http/cookies.py
+-rw-rw-r--   0 test      (1000) test      (1000)     4399 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/http/headers.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.134801 new_python_scrapy-0.1.2/scrapyy/http/request/
+-rw-rw-r--   0 test      (1000) test      (1000)     9708 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/http/request/__init__.py
+-rw-rw-r--   0 test      (1000) test      (1000)     8859 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/http/request/form.py
+-rw-rw-r--   0 test      (1000) test      (1000)     2026 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/http/request/json_request.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1161 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/http/request/rpc.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.134801 new_python_scrapy-0.1.2/scrapyy/http/response/
+-rw-rw-r--   0 test      (1000) test      (1000)     9025 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/http/response/__init__.py
+-rw-rw-r--   0 test      (1000) test      (1000)      300 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/http/response/html.py
+-rw-rw-r--   0 test      (1000) test      (1000)      286 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/http/response/json.py
+-rw-rw-r--   0 test      (1000) test      (1000)    11510 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/http/response/text.py
+-rw-rw-r--   0 test      (1000) test      (1000)      297 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/http/response/xml.py
+-rw-rw-r--   0 test      (1000) test      (1000)      557 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/interfaces.py
+-rw-rw-r--   0 test      (1000) test      (1000)     3823 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/item.py
+-rw-rw-r--   0 test      (1000) test      (1000)     2082 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/link.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.138801 new_python_scrapy-0.1.2/scrapyy/linkextractors/
+-rw-rw-r--   0 test      (1000) test      (1000)     1647 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/linkextractors/__init__.py
+-rw-rw-r--   0 test      (1000) test      (1000)     8463 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/linkextractors/lxmlhtml.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.138801 new_python_scrapy-0.1.2/scrapyy/loader/
+-rw-rw-r--   0 test      (1000) test      (1000)     3498 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/loader/__init__.py
+-rw-rw-r--   0 test      (1000) test      (1000)     6110 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/logformatter.py
+-rw-rw-r--   0 test      (1000) test      (1000)     6459 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/mail.py
+-rw-rw-r--   0 test      (1000) test      (1000)     3689 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/middleware.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.138801 new_python_scrapy-0.1.2/scrapyy/pipelines/
+-rw-rw-r--   0 test      (1000) test      (1000)      949 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/pipelines/__init__.py
+-rw-rw-r--   0 test      (1000) test      (1000)    21346 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/pipelines/files.py
+-rw-rw-r--   0 test      (1000) test      (1000)     9007 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/pipelines/images.py
+-rw-rw-r--   0 test      (1000) test      (1000)     8613 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/pipelines/media.py
+-rw-rw-r--   0 test      (1000) test      (1000)     7709 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/pqueues.py
+-rw-rw-r--   0 test      (1000) test      (1000)        0 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/py.typed
+-rw-rw-r--   0 test      (1000) test      (1000)     4205 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/resolver.py
+-rw-rw-r--   0 test      (1000) test      (1000)     5576 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/responsetypes.py
+-rw-rw-r--   0 test      (1000) test      (1000)     4714 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/robotstxt.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.138801 new_python_scrapy-0.1.2/scrapyy/selector/
+-rw-rw-r--   0 test      (1000) test      (1000)       98 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/selector/__init__.py
+-rw-rw-r--   0 test      (1000) test      (1000)     3116 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/selector/unified.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.138801 new_python_scrapy-0.1.2/scrapyy/settings/
+-rw-rw-r--   0 test      (1000) test      (1000)    19859 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/settings/__init__.py
+-rw-rw-r--   0 test      (1000) test      (1000)    10079 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/settings/default_settings.py
+-rw-rw-r--   0 test      (1000) test      (1000)     8537 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/shell.py
+-rw-rw-r--   0 test      (1000) test      (1000)     2584 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/signalmanager.py
+-rw-rw-r--   0 test      (1000) test      (1000)      875 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/signals.py
+-rw-rw-r--   0 test      (1000) test      (1000)     3483 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/spiderloader.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.138801 new_python_scrapy-0.1.2/scrapyy/spidermiddlewares/
+-rw-rw-r--   0 test      (1000) test      (1000)        0 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/spidermiddlewares/__init__.py
+-rw-rw-r--   0 test      (1000) test      (1000)     2788 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/spidermiddlewares/depth.py
+-rw-rw-r--   0 test      (1000) test      (1000)     2529 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/spidermiddlewares/httperror.py
+-rw-rw-r--   0 test      (1000) test      (1000)     3841 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/spidermiddlewares/offsite.py
+-rw-rw-r--   0 test      (1000) test      (1000)    15250 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/spidermiddlewares/referer.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1831 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/spidermiddlewares/urllength.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.138801 new_python_scrapy-0.1.2/scrapyy/spiders/
+-rw-rw-r--   0 test      (1000) test      (1000)     3622 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/spiders/__init__.py
+-rw-rw-r--   0 test      (1000) test      (1000)     4722 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/spiders/crawl.py
+-rw-rw-r--   0 test      (1000) test      (1000)     5506 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/spiders/feed.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1337 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/spiders/init.py
+-rw-rw-r--   0 test      (1000) test      (1000)     4867 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/spiders/sitemap.py
+-rw-rw-r--   0 test      (1000) test      (1000)     4842 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/squeues.py
+-rw-rw-r--   0 test      (1000) test      (1000)     3005 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/statscollectors.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.142802 new_python_scrapy-0.1.2/scrapyy/utils/
+-rw-rw-r--   0 test      (1000) test      (1000)        0 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/__init__.py
+-rw-rw-r--   0 test      (1000) test      (1000)     4291 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/_compression.py
+-rw-rw-r--   0 test      (1000) test      (1000)      507 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/asyncgen.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1308 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/benchserver.py
+-rw-rw-r--   0 test      (1000) test      (1000)      180 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/boto.py
+-rw-rw-r--   0 test      (1000) test      (1000)     9064 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/conf.py
+-rw-rw-r--   0 test      (1000) test      (1000)     4114 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/console.py
+-rw-rw-r--   0 test      (1000) test      (1000)     3587 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/curl.py
+-rw-rw-r--   0 test      (1000) test      (1000)     6410 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/datatypes.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1528 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/decorators.py
+-rw-rw-r--   0 test      (1000) test      (1000)    14775 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/defer.py
+-rw-rw-r--   0 test      (1000) test      (1000)     6993 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/deprecate.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1455 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/display.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1540 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/engine.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1355 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/ftp.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1384 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/gz.py
+-rw-rw-r--   0 test      (1000) test      (1000)      712 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/httpobj.py
+-rw-rw-r--   0 test      (1000) test      (1000)     8225 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/iterators.py
+-rw-rw-r--   0 test      (1000) test      (1000)      320 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/job.py
+-rw-rw-r--   0 test      (1000) test      (1000)     7660 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/log.py
+-rw-rw-r--   0 test      (1000) test      (1000)    10547 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/misc.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1243 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/ossignal.py
+-rw-rw-r--   0 test      (1000) test      (1000)     2640 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/project.py
+-rw-rw-r--   0 test      (1000) test      (1000)    10491 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/python.py
+-rw-rw-r--   0 test      (1000) test      (1000)     7190 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/reactor.py
+-rw-rw-r--   0 test      (1000) test      (1000)     8560 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/request.py
+-rw-rw-r--   0 test      (1000) test      (1000)     3383 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/response.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1171 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/serialize.py
+-rw-rw-r--   0 test      (1000) test      (1000)     3833 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/signal.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1713 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/sitemap.py
+-rw-rw-r--   0 test      (1000) test      (1000)     3728 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/spider.py
+-rw-rw-r--   0 test      (1000) test      (1000)     2441 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/ssl.py
+-rw-rw-r--   0 test      (1000) test      (1000)      918 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/template.py
+-rw-rw-r--   0 test      (1000) test      (1000)     4307 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/test.py
+-rw-rw-r--   0 test      (1000) test      (1000)     2079 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/testproc.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1611 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/testsite.py
+-rw-rw-r--   0 test      (1000) test      (1000)     2261 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/trackref.py
+-rw-rw-r--   0 test      (1000) test      (1000)     6020 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/url.py
+-rw-rw-r--   0 test      (1000) test      (1000)      915 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/scrapyy/utils/versions.py
+-rw-rw-r--   0 test      (1000) test      (1000)      392 2024-04-19 10:11:41.166803 new_python_scrapy-0.1.2/setup.cfg
+-rw-rw-r--   0 test      (1000) test      (1000)     3844 2024-04-19 10:10:50.000000 new_python_scrapy-0.1.2/setup.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.154802 new_python_scrapy-0.1.2/tests/
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.158802 new_python_scrapy-0.1.2/tests/CrawlerProcess/
+-rw-rw-r--   0 test      (1000) test      (1000)      609 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/CrawlerProcess/args_settings.py
+-rw-rw-r--   0 test      (1000) test      (1000)      399 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/CrawlerProcess/asyncio_custom_loop.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1173 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/CrawlerProcess/asyncio_deferred_signal.py
+-rw-rw-r--   0 test      (1000) test      (1000)      354 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/CrawlerProcess/asyncio_enabled_no_reactor.py
+-rw-rw-r--   0 test      (1000) test      (1000)      639 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/CrawlerProcess/asyncio_enabled_reactor.py
+-rw-rw-r--   0 test      (1000) test      (1000)      741 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/CrawlerProcess/asyncio_enabled_reactor_different_loop.py
+-rw-rw-r--   0 test      (1000) test      (1000)      739 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/CrawlerProcess/asyncio_enabled_reactor_same_loop.py
+-rw-rw-r--   0 test      (1000) test      (1000)      913 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/CrawlerProcess/caching_hostname_resolver.py
+-rw-rw-r--   0 test      (1000) test      (1000)      548 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/CrawlerProcess/caching_hostname_resolver_ipv6.py
+-rw-rw-r--   0 test      (1000) test      (1000)      424 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/CrawlerProcess/default_name_resolver.py
+-rw-rw-r--   0 test      (1000) test      (1000)      291 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/CrawlerProcess/multi.py
+-rw-rw-r--   0 test      (1000) test      (1000)      311 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/CrawlerProcess/reactor_default.py
+-rw-rw-r--   0 test      (1000) test      (1000)      454 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/CrawlerProcess/reactor_default_twisted_reactor_select.py
+-rw-rw-r--   0 test      (1000) test      (1000)      328 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/CrawlerProcess/reactor_select.py
+-rw-rw-r--   0 test      (1000) test      (1000)      624 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/CrawlerProcess/reactor_select_subclass_twisted_reactor_select.py
+-rw-rw-r--   0 test      (1000) test      (1000)      414 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/CrawlerProcess/reactor_select_twisted_reactor_select.py
+-rw-rw-r--   0 test      (1000) test      (1000)      259 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/CrawlerProcess/simple.py
+-rw-rw-r--   0 test      (1000) test      (1000)      545 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/CrawlerProcess/sleeping.py
+-rw-rw-r--   0 test      (1000) test      (1000)      318 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/CrawlerProcess/twisted_reactor_asyncio.py
+-rw-rw-r--   0 test      (1000) test      (1000)      326 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/CrawlerProcess/twisted_reactor_custom_settings.py
+-rw-rw-r--   0 test      (1000) test      (1000)      626 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/CrawlerProcess/twisted_reactor_custom_settings_conflict.py
+-rw-rw-r--   0 test      (1000) test      (1000)      557 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/CrawlerProcess/twisted_reactor_custom_settings_same.py
+-rw-rw-r--   0 test      (1000) test      (1000)      295 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/CrawlerProcess/twisted_reactor_poll.py
+-rw-rw-r--   0 test      (1000) test      (1000)      304 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/CrawlerProcess/twisted_reactor_select.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.158802 new_python_scrapy-0.1.2/tests/CrawlerRunner/
+-rw-rw-r--   0 test      (1000) test      (1000)     1855 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/CrawlerRunner/ip_address.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1287 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/__init__.py
+-rw-rw-r--   0 test      (1000) test      (1000)      632 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/ftpserver.py
+-rw-rw-r--   0 test      (1000) test      (1000)      103 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/ignores.txt
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.158802 new_python_scrapy-0.1.2/tests/keys/
+-rw-rw-r--   0 test      (1000) test      (1000)     1867 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/keys/__init__.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1562 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/keys/example-com.cert.pem
+-rw-rw-r--   0 test      (1000) test      (1000)     3126 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/keys/example-com.conf
+-rw-rw-r--   0 test      (1000) test      (1000)      933 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/keys/example-com.gen.README
+-rw-rw-r--   0 test      (1000) test      (1000)     1704 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/keys/example-com.key.pem
+-rw-rw-r--   0 test      (1000) test      (1000)      945 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/keys/localhost-ip.gen.README
+-rw-rw-r--   0 test      (1000) test      (1000)      945 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/keys/localhost.gen.README
+-rw-rw-r--   0 test      (1000) test      (1000)     1176 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/keys/localhost.ip.crt
+-rw-rw-r--   0 test      (1000) test      (1000)     1704 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/keys/localhost.ip.key
+-rw-rw-r--   0 test      (1000) test      (1000)     2847 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/keys/mitmproxy-ca.pem
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.158802 new_python_scrapy-0.1.2/tests/mocks/
+-rw-rw-r--   0 test      (1000) test      (1000)        0 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/mocks/__init__.py
+-rw-rw-r--   0 test      (1000) test      (1000)      507 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/mocks/dummydbm.py
+-rw-rw-r--   0 test      (1000) test      (1000)    12662 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/mockserver.py
+-rw-rw-r--   0 test      (1000) test      (1000)      289 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/pipelines.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.086799 new_python_scrapy-0.1.2/tests/sample_data/
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.162802 new_python_scrapy-0.1.2/tests/sample_data/compressed/
+-rw-rw-r--   0 test      (1000) test      (1000)       34 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/compressed/bomb-br.bin
+-rw-rw-r--   0 test      (1000) test      (1000)    27968 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/compressed/bomb-deflate.bin
+-rw-rw-r--   0 test      (1000) test      (1000)    27988 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/compressed/bomb-gzip.bin
+-rw-rw-r--   0 test      (1000) test      (1000)     1096 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/compressed/bomb-zstd.bin
+-rw-rw-r--   0 test      (1000) test      (1000)    20480 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/compressed/feed-sample1.tar
+-rw-rw-r--   0 test      (1000) test      (1000)     9950 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/compressed/feed-sample1.xml
+-rw-rw-r--   0 test      (1000) test      (1000)     1430 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/compressed/feed-sample1.xml.bz2
+-rw-rw-r--   0 test      (1000) test      (1000)     1131 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/compressed/feed-sample1.xml.gz
+-rw-rw-r--   0 test      (1000) test      (1000)     1260 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/compressed/feed-sample1.zip
+-rw-rw-r--   0 test      (1000) test      (1000)     4027 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/compressed/html-br.bin
+-rw-rw-r--   0 test      (1000) test      (1000)     8014 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/compressed/html-gzip-deflate-gzip.bin
+-rw-rw-r--   0 test      (1000) test      (1000)     7991 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/compressed/html-gzip-deflate.bin
+-rw-rw-r--   0 test      (1000) test      (1000)     8037 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/compressed/html-gzip.bin
+-rw-rw-r--   0 test      (1000) test      (1000)     8021 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/compressed/html-rawdeflate.bin
+-rw-rw-r--   0 test      (1000) test      (1000)     8027 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/compressed/html-zlibdeflate.bin
+-rw-rw-r--   0 test      (1000) test      (1000)     8066 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/compressed/html-zstd-static-content-size.bin
+-rw-rw-r--   0 test      (1000) test      (1000)     8063 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/compressed/html-zstd-static-no-content-size.bin
+-rw-rw-r--   0 test      (1000) test      (1000)     8047 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/compressed/html-zstd-streaming-no-content-size.bin
+-rw-rw-r--   0 test      (1000) test      (1000)     1930 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/compressed/truncated-crc-error-short.gz
+-rw-rw-r--   0 test      (1000) test      (1000)     5766 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/compressed/truncated-crc-error.gz
+-rw-rw-r--   0 test      (1000) test      (1000)    16782 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/compressed/unexpected-eof-output.txt
+-rw-rw-r--   0 test      (1000) test      (1000)     5134 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/compressed/unexpected-eof.gz
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.162802 new_python_scrapy-0.1.2/tests/sample_data/feeds/
+-rw-rw-r--   0 test      (1000) test      (1000)     9950 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/feeds/feed-sample1.xml
+-rw-rw-r--   0 test      (1000) test      (1000)     6388 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/feeds/feed-sample2.xml
+-rw-rw-r--   0 test      (1000) test      (1000)       81 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/feeds/feed-sample3.csv
+-rw-rw-r--   0 test      (1000) test      (1000)       45 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/feeds/feed-sample4.csv
+-rw-rw-r--   0 test      (1000) test      (1000)       47 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/feeds/feed-sample5.csv
+-rw-rw-r--   0 test      (1000) test      (1000)      101 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/feeds/feed-sample6.csv
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.162802 new_python_scrapy-0.1.2/tests/sample_data/link_extractor/
+-rw-rw-r--   0 test      (1000) test      (1000)      830 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/link_extractor/linkextractor.html
+-rw-rw-r--   0 test      (1000) test      (1000)      585 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/link_extractor/linkextractor_latin1.html
+-rw-rw-r--   0 test      (1000) test      (1000)      740 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/link_extractor/linkextractor_no_href.html
+-rw-rw-r--   0 test      (1000) test      (1000)      390 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/link_extractor/linkextractor_noenc.html
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.162802 new_python_scrapy-0.1.2/tests/sample_data/test_site/
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.086799 new_python_scrapy-0.1.2/tests/sample_data/test_site/files/
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.162802 new_python_scrapy-0.1.2/tests/sample_data/test_site/files/images/
+-rw-rw-r--   0 test      (1000) test      (1000)    11155 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/test_site/files/images/python-logo-master-v3-TM-flattened.png
+-rw-rw-r--   0 test      (1000) test      (1000)     3243 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/test_site/files/images/python-powered-h-50x65.png
+-rw-rw-r--   0 test      (1000) test      (1000)     2710 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/test_site/files/images/scrapy.png
+-rw-rw-r--   0 test      (1000) test      (1000)      311 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/test_site/index.html
+-rw-rw-r--   0 test      (1000) test      (1000)      225 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/test_site/item1.html
+-rw-rw-r--   0 test      (1000) test      (1000)      209 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/sample_data/test_site/item2.html
+-rw-rw-r--   0 test      (1000) test      (1000)    15603 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/spiders.py
+-rw-rw-r--   0 test      (1000) test      (1000)     7406 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_addons.py
+-rw-rw-r--   0 test      (1000) test      (1000)     2843 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_closespider.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.162802 new_python_scrapy-0.1.2/tests/test_cmdline/
+-rw-rw-r--   0 test      (1000) test      (1000)     2670 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_cmdline/__init__.py
+-rw-rw-r--   0 test      (1000) test      (1000)      309 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_cmdline/extensions.py
+-rw-rw-r--   0 test      (1000) test      (1000)      223 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_cmdline/settings.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.162802 new_python_scrapy-0.1.2/tests/test_cmdline_crawl_with_pipeline/
+-rw-rw-r--   0 test      (1000) test      (1000)      632 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_cmdline_crawl_with_pipeline/__init__.py
+-rw-rw-r--   0 test      (1000) test      (1000)       42 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_cmdline_crawl_with_pipeline/scrapy.cfg
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.162802 new_python_scrapy-0.1.2/tests/test_cmdline_crawl_with_pipeline/test_spider/
+-rw-rw-r--   0 test      (1000) test      (1000)        0 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_cmdline_crawl_with_pipeline/test_spider/__init__.py
+-rw-rw-r--   0 test      (1000) test      (1000)      309 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_cmdline_crawl_with_pipeline/test_spider/pipelines.py
+-rw-rw-r--   0 test      (1000) test      (1000)       66 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_cmdline_crawl_with_pipeline/test_spider/settings.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.162802 new_python_scrapy-0.1.2/tests/test_cmdline_crawl_with_pipeline/test_spider/spiders/
+-rw-rw-r--   0 test      (1000) test      (1000)        0 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_cmdline_crawl_with_pipeline/test_spider/spiders/__init__.py
+-rw-rw-r--   0 test      (1000) test      (1000)      238 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_cmdline_crawl_with_pipeline/test_spider/spiders/exception.py
+-rw-rw-r--   0 test      (1000) test      (1000)      223 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_cmdline_crawl_with_pipeline/test_spider/spiders/normal.py
+-rw-rw-r--   0 test      (1000) test      (1000)     6871 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_command_check.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1242 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_command_fetch.py
+-rw-rw-r--   0 test      (1000) test      (1000)    14538 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_command_parse.py
+-rw-rw-r--   0 test      (1000) test      (1000)     5954 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_command_shell.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1198 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_command_version.py
+-rw-rw-r--   0 test      (1000) test      (1000)    39524 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_commands.py
+-rw-rw-r--   0 test      (1000) test      (1000)    13668 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_contracts.py
+-rw-rw-r--   0 test      (1000) test      (1000)      350 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_core_downloader.py
+-rw-rw-r--   0 test      (1000) test      (1000)    27668 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_crawl.py
+-rw-rw-r--   0 test      (1000) test      (1000)    32765 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_crawler.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1457 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_dependencies.py
+-rw-rw-r--   0 test      (1000) test      (1000)    46807 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_downloader_handlers.py
+-rw-rw-r--   0 test      (1000) test      (1000)     9270 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_downloader_handlers_http2.py
+-rw-rw-r--   0 test      (1000) test      (1000)     9307 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_downloadermiddleware.py
+-rw-rw-r--   0 test      (1000) test      (1000)     2541 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_downloadermiddleware_ajaxcrawlable.py
+-rw-rw-r--   0 test      (1000) test      (1000)    28199 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_downloadermiddleware_cookies.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1397 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_downloadermiddleware_defaultheaders.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1701 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_downloadermiddleware_downloadtimeout.py
+-rw-rw-r--   0 test      (1000) test      (1000)     2658 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_downloadermiddleware_httpauth.py
+-rw-rw-r--   0 test      (1000) test      (1000)    25829 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_downloadermiddleware_httpcache.py
+-rw-rw-r--   0 test      (1000) test      (1000)    28941 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_downloadermiddleware_httpcompression.py
+-rw-rw-r--   0 test      (1000) test      (1000)    19971 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_downloadermiddleware_httpproxy.py
+-rw-rw-r--   0 test      (1000) test      (1000)    16631 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_downloadermiddleware_redirect.py
+-rw-rw-r--   0 test      (1000) test      (1000)    23673 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_downloadermiddleware_retry.py
+-rw-rw-r--   0 test      (1000) test      (1000)    10222 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_downloadermiddleware_robotstxt.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1597 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_downloadermiddleware_stats.py
+-rw-rw-r--   0 test      (1000) test      (1000)     2227 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_downloadermiddleware_useragent.py
+-rw-rw-r--   0 test      (1000) test      (1000)     3162 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_downloaderslotssettings.py
+-rw-rw-r--   0 test      (1000) test      (1000)     9493 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_dupefilters.py
+-rw-rw-r--   0 test      (1000) test      (1000)    16283 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_engine.py
+-rw-rw-r--   0 test      (1000) test      (1000)     2966 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_engine_stop_download_bytes.py
+-rw-rw-r--   0 test      (1000) test      (1000)     2709 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_engine_stop_download_headers.py
+-rw-rw-r--   0 test      (1000) test      (1000)    23999 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_exporters.py
+-rw-rw-r--   0 test      (1000) test      (1000)     6672 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_extension_periodic_log.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1833 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_extension_telnet.py
+-rw-rw-r--   0 test      (1000) test      (1000)    10434 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_extension_throttle.py
+-rw-rw-r--   0 test      (1000) test      (1000)   103071 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_feedexport.py
+-rw-rw-r--   0 test      (1000) test      (1000)    24639 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_http2_client_protocol.py
+-rw-rw-r--   0 test      (1000) test      (1000)     2878 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_http_cookies.py
+-rw-rw-r--   0 test      (1000) test      (1000)     6251 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_http_headers.py
+-rw-rw-r--   0 test      (1000) test      (1000)    68129 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_http_request.py
+-rw-rw-r--   0 test      (1000) test      (1000)    39823 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_http_response.py
+-rw-rw-r--   0 test      (1000) test      (1000)     9066 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_item.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1900 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_link.py
+-rw-rw-r--   0 test      (1000) test      (1000)    33344 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_linkextractors.py
+-rw-rw-r--   0 test      (1000) test      (1000)    21184 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_loader.py
+-rw-rw-r--   0 test      (1000) test      (1000)    25781 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_loader_deprecated.py
+-rw-rw-r--   0 test      (1000) test      (1000)     8853 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_logformatter.py
+-rw-rw-r--   0 test      (1000) test      (1000)     2530 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_logstats.py
+-rw-rw-r--   0 test      (1000) test      (1000)     5768 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_mail.py
+-rw-rw-r--   0 test      (1000) test      (1000)     2346 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_middleware.py
+-rw-rw-r--   0 test      (1000) test      (1000)     8605 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_pipeline_crawl.py
+-rw-rw-r--   0 test      (1000) test      (1000)    25239 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_pipeline_files.py
+-rw-rw-r--   0 test      (1000) test      (1000)    25719 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_pipeline_images.py
+-rw-rw-r--   0 test      (1000) test      (1000)    18445 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_pipeline_media.py
+-rw-rw-r--   0 test      (1000) test      (1000)     3893 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_pipelines.py
+-rw-rw-r--   0 test      (1000) test      (1000)     6200 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_pqueues.py
+-rw-rw-r--   0 test      (1000) test      (1000)     3864 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_proxy_connect.py
+-rw-rw-r--   0 test      (1000) test      (1000)     7644 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_request_attribute_binding.py
+-rw-rw-r--   0 test      (1000) test      (1000)     7512 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_request_cb_kwargs.py
+-rw-rw-r--   0 test      (1000) test      (1000)     6943 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_request_dict.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1931 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_request_left.py
+-rw-rw-r--   0 test      (1000) test      (1000)     5122 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_responsetypes.py
+-rw-rw-r--   0 test      (1000) test      (1000)     8062 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_robotstxt_interface.py
+-rw-rw-r--   0 test      (1000) test      (1000)    10774 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_scheduler.py
+-rw-rw-r--   0 test      (1000) test      (1000)     5505 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_scheduler_base.py
+-rw-rw-r--   0 test      (1000) test      (1000)     9412 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_selector.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.162802 new_python_scrapy-0.1.2/tests/test_settings/
+-rw-rw-r--   0 test      (1000) test      (1000)    20083 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_settings/__init__.py
+-rw-rw-r--   0 test      (1000) test      (1000)       54 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_settings/default_settings.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1339 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_signals.py
+-rw-rw-r--   0 test      (1000) test      (1000)    31192 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_spider.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.162802 new_python_scrapy-0.1.2/tests/test_spiderloader/
+-rw-rw-r--   0 test      (1000) test      (1000)     7774 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_spiderloader/__init__.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.162802 new_python_scrapy-0.1.2/tests/test_spiderloader/test_spiders/
+-rw-rw-r--   0 test      (1000) test      (1000)        0 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_spiderloader/test_spiders/__init__.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.162802 new_python_scrapy-0.1.2/tests/test_spiderloader/test_spiders/nested/
+-rw-rw-r--   0 test      (1000) test      (1000)        0 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_spiderloader/test_spiders/nested/__init__.py
+-rw-rw-r--   0 test      (1000) test      (1000)      235 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_spiderloader/test_spiders/nested/spider4.py
+-rw-rw-r--   0 test      (1000) test      (1000)      112 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_spiderloader/test_spiders/spider0.py
+-rw-rw-r--   0 test      (1000) test      (1000)      133 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_spiderloader/test_spiders/spider1.py
+-rw-rw-r--   0 test      (1000) test      (1000)      133 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_spiderloader/test_spiders/spider2.py
+-rw-rw-r--   0 test      (1000) test      (1000)      235 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_spiderloader/test_spiders/spider3.py
+-rw-rw-r--   0 test      (1000) test      (1000)    19879 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_spidermiddleware.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1342 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_spidermiddleware_depth.py
+-rw-rw-r--   0 test      (1000) test      (1000)     9286 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_spidermiddleware_httperror.py
+-rw-rw-r--   0 test      (1000) test      (1000)     3725 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_spidermiddleware_offsite.py
+-rw-rw-r--   0 test      (1000) test      (1000)    19049 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_spidermiddleware_output_chain.py
+-rw-rw-r--   0 test      (1000) test      (1000)    44049 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_spidermiddleware_referer.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1495 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_spidermiddleware_urllength.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1433 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_spiderstate.py
+-rw-rw-r--   0 test      (1000) test      (1000)     5229 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_squeues.py
+-rw-rw-r--   0 test      (1000) test      (1000)     7604 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_squeues_request.py
+-rw-rw-r--   0 test      (1000) test      (1000)     3993 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_stats.py
+-rw-rw-r--   0 test      (1000) test      (1000)      869 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_toplevel.py
+-rw-rw-r--   0 test      (1000) test      (1000)      362 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_urlparse_monkeypatches.py
+-rw-rw-r--   0 test      (1000) test      (1000)      663 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_utils_asyncgen.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1204 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_utils_asyncio.py
+-rw-rw-r--   0 test      (1000) test      (1000)     8822 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_utils_conf.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1173 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_utils_console.py
+-rw-rw-r--   0 test      (1000) test      (1000)    10221 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_utils_curl.py
+-rw-rw-r--   0 test      (1000) test      (1000)    11322 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_utils_datatypes.py
+-rw-rw-r--   0 test      (1000) test      (1000)     7611 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_utils_defer.py
+-rw-rw-r--   0 test      (1000) test      (1000)    10343 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_utils_deprecate.py
+-rw-rw-r--   0 test      (1000) test      (1000)     3204 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_utils_display.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1909 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_utils_gz.py
+-rw-rw-r--   0 test      (1000) test      (1000)      685 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_utils_httpobj.py
+-rw-rw-r--   0 test      (1000) test      (1000)    21676 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_utils_iterators.py
+-rw-rw-r--   0 test      (1000) test      (1000)     3576 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_utils_log.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.162802 new_python_scrapy-0.1.2/tests/test_utils_misc/
+-rw-rw-r--   0 test      (1000) test      (1000)    10121 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_utils_misc/__init__.py
+-rw-rw-r--   0 test      (1000) test      (1000)     2231 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_utils_misc/test.egg
+-rw-rw-r--   0 test      (1000) test      (1000)     8263 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_utils_misc/test_return_with_argument_inside_generator.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.162802 new_python_scrapy-0.1.2/tests/test_utils_misc/test_walk_modules/
+-rw-rw-r--   0 test      (1000) test      (1000)        0 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_utils_misc/test_walk_modules/__init__.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-04-19 10:11:41.166803 new_python_scrapy-0.1.2/tests/test_utils_misc/test_walk_modules/mod/
+-rw-rw-r--   0 test      (1000) test      (1000)        0 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_utils_misc/test_walk_modules/mod/__init__.py
+-rw-rw-r--   0 test      (1000) test      (1000)        0 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_utils_misc/test_walk_modules/mod/mod0.py
+-rw-rw-r--   0 test      (1000) test      (1000)        0 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_utils_misc/test_walk_modules/mod1.py
+-rw-rw-r--   0 test      (1000) test      (1000)     2598 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_utils_project.py
+-rw-rw-r--   0 test      (1000) test      (1000)     7970 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_utils_python.py
+-rw-rw-r--   0 test      (1000) test      (1000)    17748 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_utils_request.py
+-rw-rw-r--   0 test      (1000) test      (1000)     7540 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_utils_response.py
+-rw-rw-r--   0 test      (1000) test      (1000)     2488 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_utils_serialize.py
+-rw-rw-r--   0 test      (1000) test      (1000)     3376 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_utils_signal.py
+-rw-rw-r--   0 test      (1000) test      (1000)     9009 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_utils_sitemap.py
+-rw-rw-r--   0 test      (1000) test      (1000)      995 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_utils_spider.py
+-rw-rw-r--   0 test      (1000) test      (1000)     1187 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_utils_template.py
+-rw-rw-r--   0 test      (1000) test      (1000)     2152 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_utils_trackref.py
+-rw-rw-r--   0 test      (1000) test      (1000)    22563 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_utils_url.py
+-rw-rw-r--   0 test      (1000) test      (1000)    17220 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/test_webclient.py
+-rw-rw-r--   0 test      (1000) test      (1000)      412 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tests/upper-constraints.txt
+-rw-rw-r--   0 test      (1000) test      (1000)     6105 2024-04-19 08:53:16.000000 new_python_scrapy-0.1.2/tox.ini
```

### Comparing `new_python_scrapy-0.1.1/AUTHORS` & `new_python_scrapy-0.1.2/AUTHORS`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/LICENSE` & `new_python_scrapy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/README.rst` & `new_python_scrapy-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/conftest.py` & `new_python_scrapy-0.1.2/conftest.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/Makefile` & `new_python_scrapy-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/README.rst` & `new_python_scrapy-0.1.2/docs/README.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/_ext/scrapydocs.py` & `new_python_scrapy-0.1.2/docs/_ext/scrapydocs.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/_static/selectors-sample1.html` & `new_python_scrapy-0.1.2/docs/_static/selectors-sample1.html`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/_tests/quotes.html` & `new_python_scrapy-0.1.2/docs/_tests/quotes.html`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/_tests/quotes1.html` & `new_python_scrapy-0.1.2/docs/_tests/quotes1.html`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/conf.py` & `new_python_scrapy-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/conftest.py` & `new_python_scrapy-0.1.2/docs/conftest.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/contributing.rst` & `new_python_scrapy-0.1.2/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/faq.rst` & `new_python_scrapy-0.1.2/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/index.rst` & `new_python_scrapy-0.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/intro/examples.rst` & `new_python_scrapy-0.1.2/docs/intro/examples.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/intro/install.rst` & `new_python_scrapy-0.1.2/docs/intro/install.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/intro/overview.rst` & `new_python_scrapy-0.1.2/docs/intro/overview.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/intro/tutorial.rst` & `new_python_scrapy-0.1.2/docs/intro/tutorial.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/news.rst` & `new_python_scrapy-0.1.2/docs/news.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/_images/inspector_01.png` & `new_python_scrapy-0.1.2/docs/topics/_images/inspector_01.png`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/_images/network_01.png` & `new_python_scrapy-0.1.2/docs/topics/_images/network_01.png`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/_images/network_02.png` & `new_python_scrapy-0.1.2/docs/topics/_images/network_02.png`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/_images/network_03.png` & `new_python_scrapy-0.1.2/docs/topics/_images/network_03.png`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/_images/scrapy_architecture.odg` & `new_python_scrapy-0.1.2/docs/topics/_images/scrapy_architecture.odg`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/_images/scrapy_architecture.png` & `new_python_scrapy-0.1.2/docs/topics/_images/scrapy_architecture.png`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/_images/scrapy_architecture_02.png` & `new_python_scrapy-0.1.2/docs/topics/_images/scrapy_architecture_02.png`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/addons.rst` & `new_python_scrapy-0.1.2/docs/topics/addons.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/api.rst` & `new_python_scrapy-0.1.2/docs/topics/api.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/architecture.rst` & `new_python_scrapy-0.1.2/docs/topics/architecture.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/asyncio.rst` & `new_python_scrapy-0.1.2/docs/topics/asyncio.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/autothrottle.rst` & `new_python_scrapy-0.1.2/docs/topics/autothrottle.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/benchmarking.rst` & `new_python_scrapy-0.1.2/docs/topics/benchmarking.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/broad-crawls.rst` & `new_python_scrapy-0.1.2/docs/topics/broad-crawls.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/commands.rst` & `new_python_scrapy-0.1.2/docs/topics/commands.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/components.rst` & `new_python_scrapy-0.1.2/docs/topics/components.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/contracts.rst` & `new_python_scrapy-0.1.2/docs/topics/contracts.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/coroutines.rst` & `new_python_scrapy-0.1.2/docs/topics/coroutines.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/debug.rst` & `new_python_scrapy-0.1.2/docs/topics/debug.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/deploy.rst` & `new_python_scrapy-0.1.2/docs/topics/deploy.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/developer-tools.rst` & `new_python_scrapy-0.1.2/docs/topics/developer-tools.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/downloader-middleware.rst` & `new_python_scrapy-0.1.2/docs/topics/downloader-middleware.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/dynamic-content.rst` & `new_python_scrapy-0.1.2/docs/topics/dynamic-content.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/email.rst` & `new_python_scrapy-0.1.2/docs/topics/email.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/exceptions.rst` & `new_python_scrapy-0.1.2/docs/topics/exceptions.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/exporters.rst` & `new_python_scrapy-0.1.2/docs/topics/exporters.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/extensions.rst` & `new_python_scrapy-0.1.2/docs/topics/extensions.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/feed-exports.rst` & `new_python_scrapy-0.1.2/docs/topics/feed-exports.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/item-pipeline.rst` & `new_python_scrapy-0.1.2/docs/topics/item-pipeline.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/items.rst` & `new_python_scrapy-0.1.2/docs/topics/items.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/jobs.rst` & `new_python_scrapy-0.1.2/docs/topics/jobs.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/leaks.rst` & `new_python_scrapy-0.1.2/docs/topics/leaks.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/link-extractors.rst` & `new_python_scrapy-0.1.2/docs/topics/link-extractors.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/loaders.rst` & `new_python_scrapy-0.1.2/docs/topics/loaders.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/logging.rst` & `new_python_scrapy-0.1.2/docs/topics/logging.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/media-pipeline.rst` & `new_python_scrapy-0.1.2/docs/topics/media-pipeline.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/practices.rst` & `new_python_scrapy-0.1.2/docs/topics/practices.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/request-response.rst` & `new_python_scrapy-0.1.2/docs/topics/request-response.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/scheduler.rst` & `new_python_scrapy-0.1.2/docs/topics/scheduler.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/selectors.rst` & `new_python_scrapy-0.1.2/docs/topics/selectors.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/settings.rst` & `new_python_scrapy-0.1.2/docs/topics/settings.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/shell.rst` & `new_python_scrapy-0.1.2/docs/topics/shell.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/signals.rst` & `new_python_scrapy-0.1.2/docs/topics/signals.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/spider-middleware.rst` & `new_python_scrapy-0.1.2/docs/topics/spider-middleware.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/spiders.rst` & `new_python_scrapy-0.1.2/docs/topics/spiders.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/stats.rst` & `new_python_scrapy-0.1.2/docs/topics/stats.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/topics/telnetconsole.rst` & `new_python_scrapy-0.1.2/docs/topics/telnetconsole.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/utils/linkfix.py` & `new_python_scrapy-0.1.2/docs/utils/linkfix.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/docs/versioning.rst` & `new_python_scrapy-0.1.2/docs/versioning.rst`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/extras/qps-bench-server.py` & `new_python_scrapy-0.1.2/extras/qps-bench-server.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/extras/qpsclient.py` & `new_python_scrapy-0.1.2/extras/qpsclient.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/extras/scrapy.1` & `new_python_scrapy-0.1.2/extras/scrapy.1`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/extras/scrapy_bash_completion` & `new_python_scrapy-0.1.2/extras/scrapy_bash_completion`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/extras/scrapy_zsh_completion` & `new_python_scrapy-0.1.2/extras/scrapy_zsh_completion`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/new_python_scrapy.egg-info/SOURCES.txt` & `new_python_scrapy-0.1.2/new_python_scrapy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -83,17 +83,14 @@
 extras/qpsclient.py
 extras/scrapy.1
 extras/scrapy_bash_completion
 extras/scrapy_zsh_completion
 new_python_scrapy.egg-info/PKG-INFO
 new_python_scrapy.egg-info/SOURCES.txt
 new_python_scrapy.egg-info/dependency_links.txt
-new_python_scrapy.egg-info/entry_points.txt
-new_python_scrapy.egg-info/not-zip-safe
-new_python_scrapy.egg-info/requires.txt
 new_python_scrapy.egg-info/top_level.txt
 scrapyy/__init__.py
 scrapyy/__main__.py
 scrapyy/addons.py
 scrapyy/cmdline.py
 scrapyy/crawler.py
 scrapyy/dupefilters.py
```

### Comparing `new_python_scrapy-0.1.1/pytest.ini` & `new_python_scrapy-0.1.2/pytest.ini`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/__init__.py` & `new_python_scrapy-0.1.2/scrapyy/__init__.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/addons.py` & `new_python_scrapy-0.1.2/scrapyy/addons.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/cmdline.py` & `new_python_scrapy-0.1.2/scrapyy/cmdline.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/commands/__init__.py` & `new_python_scrapy-0.1.2/scrapyy/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/commands/bench.py` & `new_python_scrapy-0.1.2/scrapyy/commands/bench.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/commands/check.py` & `new_python_scrapy-0.1.2/scrapyy/commands/check.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/commands/crawl.py` & `new_python_scrapy-0.1.2/scrapyy/commands/crawl.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/commands/edit.py` & `new_python_scrapy-0.1.2/scrapyy/commands/edit.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/commands/fetch.py` & `new_python_scrapy-0.1.2/scrapyy/commands/fetch.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/commands/genspider.py` & `new_python_scrapy-0.1.2/scrapyy/commands/genspider.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/commands/parse.py` & `new_python_scrapy-0.1.2/scrapyy/commands/parse.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/commands/runspider.py` & `new_python_scrapy-0.1.2/scrapyy/commands/runspider.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/commands/settings.py` & `new_python_scrapy-0.1.2/scrapyy/commands/settings.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/commands/shell.py` & `new_python_scrapy-0.1.2/scrapyy/commands/shell.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/commands/startproject.py` & `new_python_scrapy-0.1.2/scrapyy/commands/startproject.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/commands/version.py` & `new_python_scrapy-0.1.2/scrapyy/commands/version.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/commands/view.py` & `new_python_scrapy-0.1.2/scrapyy/commands/view.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/contracts/__init__.py` & `new_python_scrapy-0.1.2/scrapyy/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/contracts/default.py` & `new_python_scrapy-0.1.2/scrapyy/contracts/default.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/core/downloader/__init__.py` & `new_python_scrapy-0.1.2/scrapyy/core/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/core/downloader/contextfactory.py` & `new_python_scrapy-0.1.2/scrapyy/core/downloader/contextfactory.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/core/downloader/handlers/__init__.py` & `new_python_scrapy-0.1.2/scrapyy/core/downloader/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/core/downloader/handlers/datauri.py` & `new_python_scrapy-0.1.2/scrapyy/core/downloader/handlers/datauri.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/core/downloader/handlers/ftp.py` & `new_python_scrapy-0.1.2/scrapyy/core/downloader/handlers/ftp.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/core/downloader/handlers/http10.py` & `new_python_scrapy-0.1.2/scrapyy/core/downloader/handlers/http10.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/core/downloader/handlers/http11.py` & `new_python_scrapy-0.1.2/scrapyy/core/downloader/handlers/http11.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/core/downloader/handlers/http2.py` & `new_python_scrapy-0.1.2/scrapyy/core/downloader/handlers/http2.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/core/downloader/handlers/s3.py` & `new_python_scrapy-0.1.2/scrapyy/core/downloader/handlers/s3.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/core/downloader/middleware.py` & `new_python_scrapy-0.1.2/scrapyy/core/downloader/middleware.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/core/downloader/tls.py` & `new_python_scrapy-0.1.2/scrapyy/core/downloader/tls.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/core/downloader/webclient.py` & `new_python_scrapy-0.1.2/scrapyy/core/downloader/webclient.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/core/engine.py` & `new_python_scrapy-0.1.2/scrapyy/core/engine.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/core/http2/agent.py` & `new_python_scrapy-0.1.2/scrapyy/core/http2/agent.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/core/http2/protocol.py` & `new_python_scrapy-0.1.2/scrapyy/core/http2/protocol.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/core/http2/stream.py` & `new_python_scrapy-0.1.2/scrapyy/core/http2/stream.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/core/scheduler.py` & `new_python_scrapy-0.1.2/scrapyy/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/core/scraper.py` & `new_python_scrapy-0.1.2/scrapyy/core/scraper.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/core/spidermw.py` & `new_python_scrapy-0.1.2/scrapyy/core/spidermw.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/crawler.py` & `new_python_scrapy-0.1.2/scrapyy/crawler.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/downloadermiddlewares/ajaxcrawl.py` & `new_python_scrapy-0.1.2/scrapyy/downloadermiddlewares/ajaxcrawl.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/downloadermiddlewares/cookies.py` & `new_python_scrapy-0.1.2/scrapyy/downloadermiddlewares/cookies.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/downloadermiddlewares/defaultheaders.py` & `new_python_scrapy-0.1.2/scrapyy/downloadermiddlewares/defaultheaders.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/downloadermiddlewares/downloadtimeout.py` & `new_python_scrapy-0.1.2/scrapyy/downloadermiddlewares/downloadtimeout.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/downloadermiddlewares/httpauth.py` & `new_python_scrapy-0.1.2/scrapyy/downloadermiddlewares/httpauth.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/downloadermiddlewares/httpcache.py` & `new_python_scrapy-0.1.2/scrapyy/downloadermiddlewares/httpcache.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/downloadermiddlewares/httpcompression.py` & `new_python_scrapy-0.1.2/scrapyy/downloadermiddlewares/httpcompression.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/downloadermiddlewares/httpproxy.py` & `new_python_scrapy-0.1.2/scrapyy/downloadermiddlewares/httpproxy.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/downloadermiddlewares/redirect.py` & `new_python_scrapy-0.1.2/scrapyy/downloadermiddlewares/redirect.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/downloadermiddlewares/retry.py` & `new_python_scrapy-0.1.2/scrapyy/downloadermiddlewares/retry.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/downloadermiddlewares/robotstxt.py` & `new_python_scrapy-0.1.2/scrapyy/downloadermiddlewares/robotstxt.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/downloadermiddlewares/stats.py` & `new_python_scrapy-0.1.2/scrapyy/downloadermiddlewares/stats.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/downloadermiddlewares/useragent.py` & `new_python_scrapy-0.1.2/scrapyy/downloadermiddlewares/useragent.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/dupefilters.py` & `new_python_scrapy-0.1.2/scrapyy/dupefilters.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/exceptions.py` & `new_python_scrapy-0.1.2/scrapyy/exceptions.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/exporters.py` & `new_python_scrapy-0.1.2/scrapyy/exporters.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/extensions/closespider.py` & `new_python_scrapy-0.1.2/scrapyy/extensions/closespider.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/extensions/corestats.py` & `new_python_scrapy-0.1.2/scrapyy/extensions/corestats.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/extensions/debug.py` & `new_python_scrapy-0.1.2/scrapyy/extensions/debug.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/extensions/feedexport.py` & `new_python_scrapy-0.1.2/scrapyy/extensions/feedexport.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/extensions/httpcache.py` & `new_python_scrapy-0.1.2/scrapyy/extensions/httpcache.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/extensions/logstats.py` & `new_python_scrapy-0.1.2/scrapyy/extensions/logstats.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/extensions/memdebug.py` & `new_python_scrapy-0.1.2/scrapyy/extensions/memdebug.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/extensions/memusage.py` & `new_python_scrapy-0.1.2/scrapyy/extensions/memusage.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/extensions/periodic_log.py` & `new_python_scrapy-0.1.2/scrapyy/extensions/periodic_log.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/extensions/postprocessing.py` & `new_python_scrapy-0.1.2/scrapyy/extensions/postprocessing.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/extensions/spiderstate.py` & `new_python_scrapy-0.1.2/scrapyy/extensions/spiderstate.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/extensions/statsmailer.py` & `new_python_scrapy-0.1.2/scrapyy/extensions/statsmailer.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/extensions/telnet.py` & `new_python_scrapy-0.1.2/scrapyy/extensions/telnet.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/extensions/throttle.py` & `new_python_scrapy-0.1.2/scrapyy/extensions/throttle.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/http/__init__.py` & `new_python_scrapy-0.1.2/scrapyy/http/__init__.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/http/cookies.py` & `new_python_scrapy-0.1.2/scrapyy/http/cookies.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/http/headers.py` & `new_python_scrapy-0.1.2/scrapyy/http/headers.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/http/request/__init__.py` & `new_python_scrapy-0.1.2/scrapyy/http/request/__init__.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/http/request/form.py` & `new_python_scrapy-0.1.2/scrapyy/http/request/form.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/http/request/json_request.py` & `new_python_scrapy-0.1.2/scrapyy/http/request/json_request.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/http/request/rpc.py` & `new_python_scrapy-0.1.2/scrapyy/http/request/rpc.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/http/response/__init__.py` & `new_python_scrapy-0.1.2/scrapyy/http/response/__init__.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/http/response/text.py` & `new_python_scrapy-0.1.2/scrapyy/http/response/text.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/interfaces.py` & `new_python_scrapy-0.1.2/scrapyy/interfaces.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/item.py` & `new_python_scrapy-0.1.2/scrapyy/item.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/link.py` & `new_python_scrapy-0.1.2/scrapyy/link.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/linkextractors/__init__.py` & `new_python_scrapy-0.1.2/scrapyy/linkextractors/__init__.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/linkextractors/lxmlhtml.py` & `new_python_scrapy-0.1.2/scrapyy/linkextractors/lxmlhtml.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/loader/__init__.py` & `new_python_scrapy-0.1.2/scrapyy/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/logformatter.py` & `new_python_scrapy-0.1.2/scrapyy/logformatter.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/mail.py` & `new_python_scrapy-0.1.2/scrapyy/mail.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/middleware.py` & `new_python_scrapy-0.1.2/scrapyy/middleware.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/pipelines/__init__.py` & `new_python_scrapy-0.1.2/scrapyy/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/pipelines/files.py` & `new_python_scrapy-0.1.2/scrapyy/pipelines/files.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/pipelines/images.py` & `new_python_scrapy-0.1.2/scrapyy/pipelines/images.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/pipelines/media.py` & `new_python_scrapy-0.1.2/scrapyy/pipelines/media.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/pqueues.py` & `new_python_scrapy-0.1.2/scrapyy/pqueues.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/resolver.py` & `new_python_scrapy-0.1.2/scrapyy/resolver.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/responsetypes.py` & `new_python_scrapy-0.1.2/scrapyy/responsetypes.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/robotstxt.py` & `new_python_scrapy-0.1.2/scrapyy/robotstxt.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/selector/unified.py` & `new_python_scrapy-0.1.2/scrapyy/selector/unified.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/settings/__init__.py` & `new_python_scrapy-0.1.2/scrapyy/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/settings/default_settings.py` & `new_python_scrapy-0.1.2/scrapyy/settings/default_settings.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/shell.py` & `new_python_scrapy-0.1.2/scrapyy/shell.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/signalmanager.py` & `new_python_scrapy-0.1.2/scrapyy/signalmanager.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/signals.py` & `new_python_scrapy-0.1.2/scrapyy/signals.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/spiderloader.py` & `new_python_scrapy-0.1.2/scrapyy/spiderloader.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/spidermiddlewares/depth.py` & `new_python_scrapy-0.1.2/scrapyy/spidermiddlewares/depth.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/spidermiddlewares/httperror.py` & `new_python_scrapy-0.1.2/scrapyy/spidermiddlewares/httperror.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/spidermiddlewares/offsite.py` & `new_python_scrapy-0.1.2/scrapyy/spidermiddlewares/offsite.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/spidermiddlewares/referer.py` & `new_python_scrapy-0.1.2/scrapyy/spidermiddlewares/referer.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/spidermiddlewares/urllength.py` & `new_python_scrapy-0.1.2/scrapyy/spidermiddlewares/urllength.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/spiders/__init__.py` & `new_python_scrapy-0.1.2/scrapyy/spiders/__init__.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/spiders/crawl.py` & `new_python_scrapy-0.1.2/scrapyy/spiders/crawl.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/spiders/feed.py` & `new_python_scrapy-0.1.2/scrapyy/spiders/feed.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/spiders/init.py` & `new_python_scrapy-0.1.2/scrapyy/spiders/init.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/spiders/sitemap.py` & `new_python_scrapy-0.1.2/scrapyy/spiders/sitemap.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/squeues.py` & `new_python_scrapy-0.1.2/scrapyy/squeues.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/statscollectors.py` & `new_python_scrapy-0.1.2/scrapyy/statscollectors.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/_compression.py` & `new_python_scrapy-0.1.2/scrapyy/utils/_compression.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/benchserver.py` & `new_python_scrapy-0.1.2/scrapyy/utils/benchserver.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/conf.py` & `new_python_scrapy-0.1.2/scrapyy/utils/conf.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/console.py` & `new_python_scrapy-0.1.2/scrapyy/utils/console.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/curl.py` & `new_python_scrapy-0.1.2/scrapyy/utils/curl.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/datatypes.py` & `new_python_scrapy-0.1.2/scrapyy/utils/datatypes.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/decorators.py` & `new_python_scrapy-0.1.2/scrapyy/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/defer.py` & `new_python_scrapy-0.1.2/scrapyy/utils/defer.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/deprecate.py` & `new_python_scrapy-0.1.2/scrapyy/utils/deprecate.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/display.py` & `new_python_scrapy-0.1.2/scrapyy/utils/display.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/engine.py` & `new_python_scrapy-0.1.2/scrapyy/utils/engine.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/ftp.py` & `new_python_scrapy-0.1.2/scrapyy/utils/ftp.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/gz.py` & `new_python_scrapy-0.1.2/scrapyy/utils/gz.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/httpobj.py` & `new_python_scrapy-0.1.2/scrapyy/utils/httpobj.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/iterators.py` & `new_python_scrapy-0.1.2/scrapyy/utils/iterators.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/log.py` & `new_python_scrapy-0.1.2/scrapyy/utils/log.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/misc.py` & `new_python_scrapy-0.1.2/scrapyy/utils/misc.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/ossignal.py` & `new_python_scrapy-0.1.2/scrapyy/utils/ossignal.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/project.py` & `new_python_scrapy-0.1.2/scrapyy/utils/project.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/python.py` & `new_python_scrapy-0.1.2/scrapyy/utils/python.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/reactor.py` & `new_python_scrapy-0.1.2/scrapyy/utils/reactor.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/request.py` & `new_python_scrapy-0.1.2/scrapyy/utils/request.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/response.py` & `new_python_scrapy-0.1.2/scrapyy/utils/response.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/serialize.py` & `new_python_scrapy-0.1.2/scrapyy/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/signal.py` & `new_python_scrapy-0.1.2/scrapyy/utils/signal.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/sitemap.py` & `new_python_scrapy-0.1.2/scrapyy/utils/sitemap.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/spider.py` & `new_python_scrapy-0.1.2/scrapyy/utils/spider.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/ssl.py` & `new_python_scrapy-0.1.2/scrapyy/utils/ssl.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/template.py` & `new_python_scrapy-0.1.2/scrapyy/utils/template.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/test.py` & `new_python_scrapy-0.1.2/scrapyy/utils/test.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/testproc.py` & `new_python_scrapy-0.1.2/scrapyy/utils/testproc.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/testsite.py` & `new_python_scrapy-0.1.2/scrapyy/utils/testsite.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/trackref.py` & `new_python_scrapy-0.1.2/scrapyy/utils/trackref.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/url.py` & `new_python_scrapy-0.1.2/scrapyy/utils/url.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/scrapyy/utils/versions.py` & `new_python_scrapy-0.1.2/scrapyy/utils/versions.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/CrawlerProcess/args_settings.py` & `new_python_scrapy-0.1.2/tests/CrawlerProcess/args_settings.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/CrawlerProcess/asyncio_deferred_signal.py` & `new_python_scrapy-0.1.2/tests/CrawlerProcess/asyncio_deferred_signal.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/CrawlerProcess/asyncio_enabled_reactor.py` & `new_python_scrapy-0.1.2/tests/CrawlerProcess/asyncio_enabled_reactor.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/CrawlerProcess/asyncio_enabled_reactor_different_loop.py` & `new_python_scrapy-0.1.2/tests/CrawlerProcess/asyncio_enabled_reactor_different_loop.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/CrawlerProcess/asyncio_enabled_reactor_same_loop.py` & `new_python_scrapy-0.1.2/tests/CrawlerProcess/asyncio_enabled_reactor_same_loop.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/CrawlerProcess/caching_hostname_resolver.py` & `new_python_scrapy-0.1.2/tests/CrawlerProcess/caching_hostname_resolver.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/CrawlerProcess/caching_hostname_resolver_ipv6.py` & `new_python_scrapy-0.1.2/tests/CrawlerProcess/caching_hostname_resolver_ipv6.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/CrawlerProcess/reactor_select_subclass_twisted_reactor_select.py` & `new_python_scrapy-0.1.2/tests/CrawlerProcess/reactor_select_subclass_twisted_reactor_select.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/CrawlerProcess/sleeping.py` & `new_python_scrapy-0.1.2/tests/CrawlerProcess/sleeping.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/CrawlerProcess/twisted_reactor_custom_settings_conflict.py` & `new_python_scrapy-0.1.2/tests/CrawlerProcess/twisted_reactor_custom_settings_conflict.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/CrawlerProcess/twisted_reactor_custom_settings_same.py` & `new_python_scrapy-0.1.2/tests/CrawlerProcess/twisted_reactor_custom_settings_same.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/CrawlerRunner/ip_address.py` & `new_python_scrapy-0.1.2/tests/CrawlerRunner/ip_address.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/__init__.py` & `new_python_scrapy-0.1.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/ftpserver.py` & `new_python_scrapy-0.1.2/tests/ftpserver.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/keys/__init__.py` & `new_python_scrapy-0.1.2/tests/keys/__init__.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/keys/example-com.cert.pem` & `new_python_scrapy-0.1.2/tests/keys/example-com.cert.pem`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/keys/example-com.conf` & `new_python_scrapy-0.1.2/tests/keys/example-com.conf`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/keys/example-com.gen.README` & `new_python_scrapy-0.1.2/tests/keys/example-com.gen.README`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/keys/example-com.key.pem` & `new_python_scrapy-0.1.2/tests/keys/example-com.key.pem`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/keys/localhost-ip.gen.README` & `new_python_scrapy-0.1.2/tests/keys/localhost-ip.gen.README`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/keys/localhost.gen.README` & `new_python_scrapy-0.1.2/tests/keys/localhost.gen.README`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/keys/localhost.ip.crt` & `new_python_scrapy-0.1.2/tests/keys/localhost.ip.crt`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/keys/localhost.ip.key` & `new_python_scrapy-0.1.2/tests/keys/localhost.ip.key`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/keys/mitmproxy-ca.pem` & `new_python_scrapy-0.1.2/tests/keys/mitmproxy-ca.pem`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/mockserver.py` & `new_python_scrapy-0.1.2/tests/mockserver.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/sample_data/compressed/bomb-deflate.bin` & `new_python_scrapy-0.1.2/tests/sample_data/compressed/bomb-deflate.bin`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/sample_data/compressed/bomb-gzip.bin` & `new_python_scrapy-0.1.2/tests/sample_data/compressed/bomb-gzip.bin`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/sample_data/compressed/bomb-zstd.bin` & `new_python_scrapy-0.1.2/tests/sample_data/compressed/bomb-zstd.bin`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/sample_data/compressed/feed-sample1.tar` & `new_python_scrapy-0.1.2/tests/sample_data/compressed/feed-sample1.tar`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/sample_data/compressed/feed-sample1.xml` & `new_python_scrapy-0.1.2/tests/sample_data/compressed/feed-sample1.xml`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/sample_data/compressed/feed-sample1.xml.bz2` & `new_python_scrapy-0.1.2/tests/sample_data/compressed/feed-sample1.xml.bz2`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/sample_data/compressed/feed-sample1.xml.gz` & `new_python_scrapy-0.1.2/tests/sample_data/compressed/feed-sample1.xml.gz`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/sample_data/compressed/feed-sample1.zip` & `new_python_scrapy-0.1.2/tests/sample_data/compressed/feed-sample1.zip`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/sample_data/compressed/html-br.bin` & `new_python_scrapy-0.1.2/tests/sample_data/compressed/html-br.bin`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/sample_data/compressed/html-gzip-deflate-gzip.bin` & `new_python_scrapy-0.1.2/tests/sample_data/compressed/html-gzip-deflate-gzip.bin`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/sample_data/compressed/html-gzip-deflate.bin` & `new_python_scrapy-0.1.2/tests/sample_data/compressed/html-gzip-deflate.bin`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/sample_data/compressed/html-gzip.bin` & `new_python_scrapy-0.1.2/tests/sample_data/compressed/html-gzip.bin`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/sample_data/compressed/html-rawdeflate.bin` & `new_python_scrapy-0.1.2/tests/sample_data/compressed/html-rawdeflate.bin`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/sample_data/compressed/html-zlibdeflate.bin` & `new_python_scrapy-0.1.2/tests/sample_data/compressed/html-zlibdeflate.bin`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/sample_data/compressed/html-zstd-static-content-size.bin` & `new_python_scrapy-0.1.2/tests/sample_data/compressed/html-zstd-static-content-size.bin`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/sample_data/compressed/html-zstd-static-no-content-size.bin` & `new_python_scrapy-0.1.2/tests/sample_data/compressed/html-zstd-static-no-content-size.bin`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/sample_data/compressed/html-zstd-streaming-no-content-size.bin` & `new_python_scrapy-0.1.2/tests/sample_data/compressed/html-zstd-streaming-no-content-size.bin`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/sample_data/compressed/truncated-crc-error-short.gz` & `new_python_scrapy-0.1.2/tests/sample_data/compressed/truncated-crc-error-short.gz`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/sample_data/compressed/truncated-crc-error.gz` & `new_python_scrapy-0.1.2/tests/sample_data/compressed/truncated-crc-error.gz`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/sample_data/compressed/unexpected-eof-output.txt` & `new_python_scrapy-0.1.2/tests/sample_data/compressed/unexpected-eof-output.txt`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/sample_data/compressed/unexpected-eof.gz` & `new_python_scrapy-0.1.2/tests/sample_data/compressed/unexpected-eof.gz`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/sample_data/feeds/feed-sample1.xml` & `new_python_scrapy-0.1.2/tests/sample_data/feeds/feed-sample1.xml`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/sample_data/feeds/feed-sample2.xml` & `new_python_scrapy-0.1.2/tests/sample_data/feeds/feed-sample2.xml`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/sample_data/link_extractor/linkextractor.html` & `new_python_scrapy-0.1.2/tests/sample_data/link_extractor/linkextractor.html`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/sample_data/link_extractor/linkextractor_latin1.html` & `new_python_scrapy-0.1.2/tests/sample_data/link_extractor/linkextractor_latin1.html`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/sample_data/link_extractor/linkextractor_no_href.html` & `new_python_scrapy-0.1.2/tests/sample_data/link_extractor/linkextractor_no_href.html`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/sample_data/test_site/files/images/python-logo-master-v3-TM-flattened.png` & `new_python_scrapy-0.1.2/tests/sample_data/test_site/files/images/python-logo-master-v3-TM-flattened.png`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/sample_data/test_site/files/images/python-powered-h-50x65.png` & `new_python_scrapy-0.1.2/tests/sample_data/test_site/files/images/python-powered-h-50x65.png`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/sample_data/test_site/files/images/scrapy.png` & `new_python_scrapy-0.1.2/tests/sample_data/test_site/files/images/scrapy.png`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/spiders.py` & `new_python_scrapy-0.1.2/tests/spiders.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_addons.py` & `new_python_scrapy-0.1.2/tests/test_addons.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_closespider.py` & `new_python_scrapy-0.1.2/tests/test_closespider.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_cmdline/__init__.py` & `new_python_scrapy-0.1.2/tests/test_cmdline/__init__.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_cmdline_crawl_with_pipeline/__init__.py` & `new_python_scrapy-0.1.2/tests/test_cmdline_crawl_with_pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_command_check.py` & `new_python_scrapy-0.1.2/tests/test_command_check.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_command_fetch.py` & `new_python_scrapy-0.1.2/tests/test_command_fetch.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_command_parse.py` & `new_python_scrapy-0.1.2/tests/test_command_parse.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_command_shell.py` & `new_python_scrapy-0.1.2/tests/test_command_shell.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_command_version.py` & `new_python_scrapy-0.1.2/tests/test_command_version.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_commands.py` & `new_python_scrapy-0.1.2/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_contracts.py` & `new_python_scrapy-0.1.2/tests/test_contracts.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_crawl.py` & `new_python_scrapy-0.1.2/tests/test_crawl.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_crawler.py` & `new_python_scrapy-0.1.2/tests/test_crawler.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_dependencies.py` & `new_python_scrapy-0.1.2/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_downloader_handlers.py` & `new_python_scrapy-0.1.2/tests/test_downloader_handlers.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_downloader_handlers_http2.py` & `new_python_scrapy-0.1.2/tests/test_downloader_handlers_http2.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_downloadermiddleware.py` & `new_python_scrapy-0.1.2/tests/test_downloadermiddleware.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_downloadermiddleware_ajaxcrawlable.py` & `new_python_scrapy-0.1.2/tests/test_downloadermiddleware_ajaxcrawlable.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_downloadermiddleware_cookies.py` & `new_python_scrapy-0.1.2/tests/test_downloadermiddleware_cookies.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_downloadermiddleware_defaultheaders.py` & `new_python_scrapy-0.1.2/tests/test_downloadermiddleware_defaultheaders.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_downloadermiddleware_downloadtimeout.py` & `new_python_scrapy-0.1.2/tests/test_downloadermiddleware_downloadtimeout.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_downloadermiddleware_httpauth.py` & `new_python_scrapy-0.1.2/tests/test_downloadermiddleware_httpauth.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_downloadermiddleware_httpcache.py` & `new_python_scrapy-0.1.2/tests/test_downloadermiddleware_httpcache.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_downloadermiddleware_httpcompression.py` & `new_python_scrapy-0.1.2/tests/test_downloadermiddleware_httpcompression.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_downloadermiddleware_httpproxy.py` & `new_python_scrapy-0.1.2/tests/test_downloadermiddleware_httpproxy.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_downloadermiddleware_redirect.py` & `new_python_scrapy-0.1.2/tests/test_downloadermiddleware_redirect.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_downloadermiddleware_retry.py` & `new_python_scrapy-0.1.2/tests/test_downloadermiddleware_retry.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_downloadermiddleware_robotstxt.py` & `new_python_scrapy-0.1.2/tests/test_downloadermiddleware_robotstxt.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_downloadermiddleware_stats.py` & `new_python_scrapy-0.1.2/tests/test_downloadermiddleware_stats.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_downloadermiddleware_useragent.py` & `new_python_scrapy-0.1.2/tests/test_downloadermiddleware_useragent.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_downloaderslotssettings.py` & `new_python_scrapy-0.1.2/tests/test_downloaderslotssettings.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_dupefilters.py` & `new_python_scrapy-0.1.2/tests/test_dupefilters.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_engine.py` & `new_python_scrapy-0.1.2/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_engine_stop_download_bytes.py` & `new_python_scrapy-0.1.2/tests/test_engine_stop_download_bytes.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_engine_stop_download_headers.py` & `new_python_scrapy-0.1.2/tests/test_engine_stop_download_headers.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_exporters.py` & `new_python_scrapy-0.1.2/tests/test_exporters.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_extension_periodic_log.py` & `new_python_scrapy-0.1.2/tests/test_extension_periodic_log.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_extension_telnet.py` & `new_python_scrapy-0.1.2/tests/test_extension_telnet.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_extension_throttle.py` & `new_python_scrapy-0.1.2/tests/test_extension_throttle.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_feedexport.py` & `new_python_scrapy-0.1.2/tests/test_feedexport.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_http2_client_protocol.py` & `new_python_scrapy-0.1.2/tests/test_http2_client_protocol.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_http_cookies.py` & `new_python_scrapy-0.1.2/tests/test_http_cookies.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_http_headers.py` & `new_python_scrapy-0.1.2/tests/test_http_headers.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_http_request.py` & `new_python_scrapy-0.1.2/tests/test_http_request.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_http_response.py` & `new_python_scrapy-0.1.2/tests/test_http_response.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_item.py` & `new_python_scrapy-0.1.2/tests/test_item.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_link.py` & `new_python_scrapy-0.1.2/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_linkextractors.py` & `new_python_scrapy-0.1.2/tests/test_linkextractors.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_loader.py` & `new_python_scrapy-0.1.2/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_loader_deprecated.py` & `new_python_scrapy-0.1.2/tests/test_loader_deprecated.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_logformatter.py` & `new_python_scrapy-0.1.2/tests/test_logformatter.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_logstats.py` & `new_python_scrapy-0.1.2/tests/test_logstats.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_mail.py` & `new_python_scrapy-0.1.2/tests/test_mail.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_middleware.py` & `new_python_scrapy-0.1.2/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_pipeline_crawl.py` & `new_python_scrapy-0.1.2/tests/test_pipeline_crawl.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_pipeline_files.py` & `new_python_scrapy-0.1.2/tests/test_pipeline_files.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_pipeline_images.py` & `new_python_scrapy-0.1.2/tests/test_pipeline_images.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_pipeline_media.py` & `new_python_scrapy-0.1.2/tests/test_pipeline_media.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_pipelines.py` & `new_python_scrapy-0.1.2/tests/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_pqueues.py` & `new_python_scrapy-0.1.2/tests/test_pqueues.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_proxy_connect.py` & `new_python_scrapy-0.1.2/tests/test_proxy_connect.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_request_attribute_binding.py` & `new_python_scrapy-0.1.2/tests/test_request_attribute_binding.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_request_cb_kwargs.py` & `new_python_scrapy-0.1.2/tests/test_request_cb_kwargs.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_request_dict.py` & `new_python_scrapy-0.1.2/tests/test_request_dict.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_request_left.py` & `new_python_scrapy-0.1.2/tests/test_request_left.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_responsetypes.py` & `new_python_scrapy-0.1.2/tests/test_responsetypes.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_robotstxt_interface.py` & `new_python_scrapy-0.1.2/tests/test_robotstxt_interface.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_scheduler.py` & `new_python_scrapy-0.1.2/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_scheduler_base.py` & `new_python_scrapy-0.1.2/tests/test_scheduler_base.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_selector.py` & `new_python_scrapy-0.1.2/tests/test_selector.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_settings/__init__.py` & `new_python_scrapy-0.1.2/tests/test_settings/__init__.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_signals.py` & `new_python_scrapy-0.1.2/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_spider.py` & `new_python_scrapy-0.1.2/tests/test_spider.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_spiderloader/__init__.py` & `new_python_scrapy-0.1.2/tests/test_spiderloader/__init__.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_spidermiddleware.py` & `new_python_scrapy-0.1.2/tests/test_spidermiddleware.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_spidermiddleware_depth.py` & `new_python_scrapy-0.1.2/tests/test_spidermiddleware_depth.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_spidermiddleware_httperror.py` & `new_python_scrapy-0.1.2/tests/test_spidermiddleware_httperror.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_spidermiddleware_offsite.py` & `new_python_scrapy-0.1.2/tests/test_spidermiddleware_offsite.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_spidermiddleware_output_chain.py` & `new_python_scrapy-0.1.2/tests/test_spidermiddleware_output_chain.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_spidermiddleware_referer.py` & `new_python_scrapy-0.1.2/tests/test_spidermiddleware_referer.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_spidermiddleware_urllength.py` & `new_python_scrapy-0.1.2/tests/test_spidermiddleware_urllength.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_spiderstate.py` & `new_python_scrapy-0.1.2/tests/test_spiderstate.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_squeues.py` & `new_python_scrapy-0.1.2/tests/test_squeues.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_squeues_request.py` & `new_python_scrapy-0.1.2/tests/test_squeues_request.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_stats.py` & `new_python_scrapy-0.1.2/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_toplevel.py` & `new_python_scrapy-0.1.2/tests/test_toplevel.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_utils_asyncgen.py` & `new_python_scrapy-0.1.2/tests/test_utils_asyncgen.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_utils_asyncio.py` & `new_python_scrapy-0.1.2/tests/test_utils_asyncio.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_utils_conf.py` & `new_python_scrapy-0.1.2/tests/test_utils_conf.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_utils_console.py` & `new_python_scrapy-0.1.2/tests/test_utils_console.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_utils_curl.py` & `new_python_scrapy-0.1.2/tests/test_utils_curl.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_utils_datatypes.py` & `new_python_scrapy-0.1.2/tests/test_utils_datatypes.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_utils_defer.py` & `new_python_scrapy-0.1.2/tests/test_utils_defer.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_utils_deprecate.py` & `new_python_scrapy-0.1.2/tests/test_utils_deprecate.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_utils_display.py` & `new_python_scrapy-0.1.2/tests/test_utils_display.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_utils_gz.py` & `new_python_scrapy-0.1.2/tests/test_utils_gz.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_utils_httpobj.py` & `new_python_scrapy-0.1.2/tests/test_utils_httpobj.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_utils_iterators.py` & `new_python_scrapy-0.1.2/tests/test_utils_iterators.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_utils_log.py` & `new_python_scrapy-0.1.2/tests/test_utils_log.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_utils_misc/__init__.py` & `new_python_scrapy-0.1.2/tests/test_utils_misc/__init__.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_utils_misc/test.egg` & `new_python_scrapy-0.1.2/tests/test_utils_misc/test.egg`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_utils_misc/test_return_with_argument_inside_generator.py` & `new_python_scrapy-0.1.2/tests/test_utils_misc/test_return_with_argument_inside_generator.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_utils_project.py` & `new_python_scrapy-0.1.2/tests/test_utils_project.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_utils_python.py` & `new_python_scrapy-0.1.2/tests/test_utils_python.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_utils_request.py` & `new_python_scrapy-0.1.2/tests/test_utils_request.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_utils_response.py` & `new_python_scrapy-0.1.2/tests/test_utils_response.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_utils_serialize.py` & `new_python_scrapy-0.1.2/tests/test_utils_serialize.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_utils_signal.py` & `new_python_scrapy-0.1.2/tests/test_utils_signal.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_utils_sitemap.py` & `new_python_scrapy-0.1.2/tests/test_utils_sitemap.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_utils_spider.py` & `new_python_scrapy-0.1.2/tests/test_utils_spider.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_utils_template.py` & `new_python_scrapy-0.1.2/tests/test_utils_template.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_utils_trackref.py` & `new_python_scrapy-0.1.2/tests/test_utils_trackref.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_utils_url.py` & `new_python_scrapy-0.1.2/tests/test_utils_url.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tests/test_webclient.py` & `new_python_scrapy-0.1.2/tests/test_webclient.py`

 * *Files identical despite different names*

### Comparing `new_python_scrapy-0.1.1/tox.ini` & `new_python_scrapy-0.1.2/tox.ini`

 * *Files identical despite different names*

