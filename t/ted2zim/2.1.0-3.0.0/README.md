# Comparing `tmp/ted2zim-2.1.0.tar.gz` & `tmp/ted2zim-3.0.0.tar.gz`

## Comparing `ted2zim-2.1.0.tar` & `ted2zim-3.0.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 ted2zim-2.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 ted2zim-2.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 ted2zim-2.1.0/Dockerfile
--rwxr-xr-x   0        0        0     2417 2020-02-02 00:00:00.000000 ted2zim-2.1.0/get_js_deps.sh
--rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 ted2zim-2.1.0/tasks.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 ted2zim-2.1.0/src/ted2zim/VERSION
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ted2zim-2.1.0/src/ted2zim/__about__.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ted2zim-2.1.0/src/ted2zim/__init__.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 ted2zim-2.1.0/src/ted2zim/constants.py
--rwxr-xr-x   0        0        0     5695 2020-02-02 00:00:00.000000 ted2zim-2.1.0/src/ted2zim/entrypoint.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 ted2zim-2.1.0/src/ted2zim/processing.py
--rw-r--r--   0        0        0    43424 2020-02-02 00:00:00.000000 ted2zim-2.1.0/src/ted2zim/scraper.py
--rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 ted2zim-2.1.0/src/ted2zim/utils.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 ted2zim-2.1.0/src/ted2zim/locale/hi/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ted2zim-2.1.0/src/ted2zim/multi/__init__.py
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 ted2zim-2.1.0/src/ted2zim/multi/entrypoint.py
--rw-r--r--   0        0        0    12667 2020-02-02 00:00:00.000000 ted2zim-2.1.0/src/ted2zim/multi/scraper.py
--rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 ted2zim-2.1.0/src/ted2zim/templates/article.html
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 ted2zim-2.1.0/src/ted2zim/templates/favicon.png
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 ted2zim-2.1.0/src/ted2zim/templates/home.html
--rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 ted2zim-2.1.0/src/ted2zim/templates/assets/app.js
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 ted2zim-2.1.0/src/ted2zim/templates/assets/article.css
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 ted2zim-2.1.0/src/ted2zim/templates/assets/article.js
--rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 ted2zim-2.1.0/src/ted2zim/templates/assets/db.js
--rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 ted2zim-2.1.0/src/ted2zim/templates/assets/home.css
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 ted2zim-2.1.0/src/ted2zim/templates/assets/webp-trigger.js
--rwxr-xr-x   0        0        0   142472 2020-02-02 00:00:00.000000 ted2zim-2.1.0/src/ted2zim/templates/assets/font/Roboto-Black.ttf
--rwxr-xr-x   0        0        0   135820 2020-02-02 00:00:00.000000 ted2zim-2.1.0/src/ted2zim/templates/assets/font/Roboto-Bold.ttf
--rwxr-xr-x   0        0        0   140276 2020-02-02 00:00:00.000000 ted2zim-2.1.0/src/ted2zim/templates/assets/font/Roboto-Light.ttf
--rwxr-xr-x   0        0        0   145932 2020-02-02 00:00:00.000000 ted2zim-2.1.0/src/ted2zim/templates/assets/font/Roboto-LightItalic.ttf
--rwxr-xr-x   0        0        0   145348 2020-02-02 00:00:00.000000 ted2zim-2.1.0/src/ted2zim/templates/assets/font/Roboto-Regular.ttf
--rw-r--r--   0        0        0    16277 2020-02-02 00:00:00.000000 ted2zim-2.1.0/src/ted2zim/templates/assets/img/TED.png
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 ted2zim-2.1.0/src/ted2zim/templates/assets/img/TED_small.png
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 ted2zim-2.1.0/tests/test_dummy.py
--rw-r--r--   0        0        0     7776 2020-02-02 00:00:00.000000 ted2zim-2.1.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 ted2zim-2.1.0/LICENSE
--rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 ted2zim-2.1.0/README.md
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 ted2zim-2.1.0/hatch_build.py
--rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 ted2zim-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     5995 2020-02-02 00:00:00.000000 ted2zim-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 ted2zim-3.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 ted2zim-3.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 ted2zim-3.0.0/Dockerfile
+-rwxr-xr-x   0        0        0       84 2020-02-02 00:00:00.000000 ted2zim-3.0.0/entrypoint.sh
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 ted2zim-3.0.0/openzim.toml
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 ted2zim-3.0.0/tasks.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/__about__.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/__init__.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/constants.py
+-rwxr-xr-x   0        0        0     6019 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/entrypoint.py
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/languages.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/processing.py
+-rw-r--r--   0        0        0    54583 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/scraper.py
+-rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/utils.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/locale/hi/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/multi/__init__.py
+-rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/multi/entrypoint.py
+-rw-r--r--   0        0        0    12893 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/multi/scraper.py
+-rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/templates/article.html
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/templates/favicon.png
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/templates/home.html
+-rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/templates/assets/app.js
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/templates/assets/article.css
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/templates/assets/article.js
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/templates/assets/db.js
+-rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/templates/assets/home.css
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/templates/assets/webp-trigger.js
+-rwxr-xr-x   0        0        0   142472 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/templates/assets/font/Roboto-Black.ttf
+-rwxr-xr-x   0        0        0   135820 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/templates/assets/font/Roboto-Bold.ttf
+-rwxr-xr-x   0        0        0   140276 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/templates/assets/font/Roboto-Light.ttf
+-rwxr-xr-x   0        0        0   145932 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/templates/assets/font/Roboto-LightItalic.ttf
+-rwxr-xr-x   0        0        0   145348 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/templates/assets/font/Roboto-Regular.ttf
+-rw-r--r--   0        0        0    16277 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/templates/assets/img/TED.png
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/templates/assets/img/TED_small.png
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 ted2zim-3.0.0/tests/test_dummy.py
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 ted2zim-3.0.0/tests/test_languages.py
+-rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 ted2zim-3.0.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 ted2zim-3.0.0/LICENSE
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 ted2zim-3.0.0/README.md
+-rw-r--r--   0        0        0     5574 2020-02-02 00:00:00.000000 ted2zim-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6239 2020-02-02 00:00:00.000000 ted2zim-3.0.0/PKG-INFO
```

### Comparing `ted2zim-2.1.0/.pre-commit-config.yaml` & `ted2zim-3.0.0/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
   rev: v4.5.0
   hooks:
   -   id: trailing-whitespace
   -   id: end-of-file-fixer
 - repo: https://github.com/psf/black
-  rev: "23.12.0"
+  rev: "24.4.0"
   hooks:
   -   id: black
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: v0.1.8
+  rev: v0.4.0
   hooks:
   - id: ruff
 - repo: https://github.com/RobertCraigie/pyright-python
-  rev: v1.1.341
+  rev: v1.1.359
   hooks:
   - id: pyright
     name: pyright (system)
     description: 'pyright static type checker'
     entry: pyright
     language: system
     'types_or': [python, pyi]
```

### Comparing `ted2zim-2.1.0/CHANGELOG.md` & `ted2zim-3.0.0/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,39 @@
 ## Changelog
 
 All notable changes to this project are documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html) (as of version 2.0.11).
 
+## [3.0.0] - 2024-04-19
+
+### Added
+
+- New `long_description` CLI argument to set the ZIM long description
+- New `disable_metadata_check` CLI argument to disable the metadata checks which are automated since zimscraperlib 3.x
+- When `--languages` CLI arugment is not passed, no filtering by language is done (#171)
+
+### Changed
+
+- Changed default publisher metadata from 'Kiwix' to 'openZIM'
+- Validate ZIM metadata as early as possible
+- Migrate to zimscraperlib 3.3.2 (including **new VideoLowWebm encoder preset version 2**)
+- Upgrade Python dependencies, including migration to Python 3.12
+
+## Fixed
+
+- Fix language metadata computation (#172)
+- Fix computation of automatic description and long description
+- Fix subtitles time offset (#177)
+- Fix rare bug in display of videos title and description on video page
+- Fix support for Youtube fallback when download video from TED CDN is not working (#164 + #182)
+- Do not include videos which failed to be fetched / processed in the final list of videos on main page (#167, #169)
+- Fix video not working on Safari iOS / iPad (#145)
+
 ## [2.1.0] - 2024-01-08
 
 ### Changed
 
 - fixed search by topic to use new search API instead of broken web page scraping (#149)
 - download_link is renamed request_url and can also perform POST requests (in addition to previous GET requests)
 - upgrade to Python 3.11 from 3.8
```

### Comparing `ted2zim-2.1.0/Dockerfile` & `ted2zim-3.0.0/Dockerfile`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,24 @@
-FROM python:3.11-slim-bookworm
+FROM python:3.12-slim-bookworm
 LABEL org.opencontainers.image.source https://github.com/openzim/ted
 
 # Install necessary packages
 RUN apt-get update \
  && apt-get install -y --no-install-recommends \
       locales-all wget unzip ffmpeg curl libmagic1 \
  && rm -rf /var/lib/apt/lists/* \
  && python -m pip install --no-cache-dir -U \
       pip
 
+# Custom entrypoint
+COPY entrypoint.sh /usr/local/bin/entrypoint.sh
+ENTRYPOINT ["entrypoint.sh"]
+
 # Copy pyproject.toml and its dependencies
-COPY pyproject.toml README.md hatch_build.py get_js_deps.sh /src/
+COPY pyproject.toml openzim.toml README.md /src/
 COPY src/ted2zim/__about__.py /src/src/ted2zim/__about__.py
 
 # Install Python dependencies
 RUN pip install --no-cache-dir /src
 
 # Copy code + associated artifacts
 COPY src /src/src
```

### Comparing `ted2zim-2.1.0/tasks.py` & `ted2zim-3.0.0/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     ctx.run(f"black {args}", pty=use_pty)
 
 
 @task(optional=["args"], help={"args": "ruff additional arguments"})
 def fix_ruff(ctx: Context, args: str = "."):
     """fix all ruff rules"""
     args = args or "."  # needed for hatch script
-    ctx.run(f"ruff --fix {args}", pty=use_pty)
+    ctx.run(f"ruff check --fix {args}", pty=use_pty)
 
 
 @task(
     optional=["args"],
     help={
         "args": "linting tools (black, ruff) additional arguments, typically a path",
     },
```

### Comparing `ted2zim-2.1.0/src/ted2zim/constants.py` & `ted2zim-3.0.0/src/ted2zim/constants.py`

 * *Files identical despite different names*

### Comparing `ted2zim-2.1.0/src/ted2zim/entrypoint.py` & `ted2zim-3.0.0/src/ted2zim/entrypoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,18 +82,23 @@
     )
 
     parser.add_argument(
         "--description",
         help="Custom description for your ZIM. Based on selection otherwise.",
     )
 
+    parser.add_argument(
+        "--long-description",
+        help="Custom long description for your ZIM.",
+    )
+
     parser.add_argument("--creator", help="Name of content creator", default="TED")
 
     parser.add_argument(
-        "--publisher", help="Custom publisher name (ZIM metadata)", default="Kiwix"
+        "--publisher", help="Custom publisher name (ZIM metadata)", default="openZIM"
     )
 
     parser.add_argument(
         "--tags",
         help="List of comma-separated Tags for the ZIM file. category:ted, ted, and "
         "_videos:yes added automatically",
     )
@@ -159,14 +164,21 @@
     parser.add_argument(
         "--version",
         help="Display scraper version and exit",
         action="version",
         version=SCRAPER,
     )
 
+    parser.add_argument(
+        "--disable-metadata-checks",
+        help="Disable validity checks of metadata according to openZIM conventions",
+        action="store_true",
+        default=False,
+    )
+
     args = parser.parse_args()
     set_debug(args.debug)
     logger = get_logger()
 
     from ted2zim.scraper import Ted2Zim
 
     try:
```

### Comparing `ted2zim-2.1.0/src/ted2zim/processing.py` & `ted2zim-3.0.0/src/ted2zim/processing.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,10 +29,19 @@
 
     # don't reencode if not requesting low-quality and received wanted format
     if not low_quality and src_path.suffix[1:] == video_format:
         return
 
     dst_path = src_path.parent.joinpath(f"video.{video_format}")
     logger.debug(f"Converting video {video_id}")
-    reencode(
-        src_path, dst_path, preset.to_ffmpeg_args(), delete_src=True, failsafe=False
-    )
+    success, process = reencode(
+        src_path,
+        dst_path,
+        preset.to_ffmpeg_args(),
+        delete_src=True,
+        with_process=True,
+        failsafe=True,
+    )  # pyright: ignore[reportGeneralTypeIssues]
+    if not success:
+        if process:
+            logger.error(process.stdout)
+        raise Exception(f"Exception while re-encoding {src_path} for {video_id}")
```

### Comparing `ted2zim-2.1.0/src/ted2zim/scraper.py` & `ted2zim-3.0.0/src/ted2zim/scraper.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,38 +3,48 @@
 import json
 import locale
 import pathlib
 import shutil
 import tempfile
 import time
 import urllib.parse
+from itertools import groupby
 
 import dateutil.parser
 import jinja2
+import yt_dlp
 from bs4 import BeautifulSoup
 from kiwixstorage import KiwixStorage
 from pif import get_public_ip
 from slugify import slugify
 from zimscraperlib.download import BestMp4, BestWebm, YoutubeDownloader, save_large_file
-from zimscraperlib.i18n import _, get_language_details, setlocale
+from zimscraperlib.i18n import _, setlocale
 from zimscraperlib.image.optimization import optimize_image
 from zimscraperlib.image.presets import WebpMedium
 from zimscraperlib.image.transformation import resize_image
+from zimscraperlib.inputs import compute_descriptions
 from zimscraperlib.video.presets import VideoMp4Low, VideoWebmLow
 from zimscraperlib.zim import make_zim_file
+from zimscraperlib.zim.metadata import (
+    validate_description,
+    validate_language,
+    validate_longdescription,
+    validate_tags,
+    validate_title,
+)
 
+from ted2zim import languages as tedlang
 from ted2zim.constants import (
     ALL,
     BASE_URL,
     MATCHING,
     NONE,
     ROOT_DIR,
     SCRAPER,
     SEARCH_URL,
-    TEDLANGS,
     get_logger,
 )
 from ted2zim.processing import post_process_video
 from ted2zim.utils import WebVTT, get_main_title, request_url, update_subtitles_list
 
 logger = get_logger()
 
@@ -50,42 +60,61 @@
         output_dir,
         no_zim,
         fname,
         languages,
         locale_name,
         title,
         description,
+        long_description,
         creator,
         publisher,
         tags,
         keep_build_dir,
         autoplay,
         use_any_optimized_version,
         s3_url_with_credentials,
         playlist,
         subtitles_enough,
         subtitles_setting,
         tmp_dir,
         threads,
+        disable_metadata_checks,
     ):
         # video-encoding info
         self.video_format = video_format
         self.low_quality = low_quality
 
         # zim params
         self.fname = fname
         self.languages = (
             [] if languages is None else [lang.strip() for lang in languages.split(",")]
         )
+
         self.tags = [] if tags is None else [tag.strip() for tag in tags.split(",")]
+        self.tags = [*self.tags, "_category:ted", "ted", "_videos:yes"]
         self.title = title
         self.description = description
+        self.long_description = long_description
         self.creator = creator
         self.publisher = publisher
         self.name = name
+        self.disable_metadata_checks = disable_metadata_checks
+
+        if not self.disable_metadata_checks:
+            # Validate ZIM metadata early so that we do not waste time doing operations
+            # for a scraper which will fail anyway in the end ; language is not
+            # validated here since it is dynamically built based on languages found in
+            # videos that will be added to the ZIM
+            validate_tags("Tags", self.tags)
+            if self.title:
+                validate_title("Title", self.title)
+            if self.description:
+                validate_description("Description", self.description)
+            if self.long_description:
+                validate_longdescription("LongDescription", self.long_description)
 
         # directory setup
         self.output_dir = pathlib.Path(output_dir).expanduser().resolve()
         if tmp_dir:
             pathlib.Path(tmp_dir).mkdir(parents=True, exist_ok=True)
         self.build_dir = pathlib.Path(tempfile.mkdtemp(dir=tmp_dir))
 
@@ -93,15 +122,15 @@
         self.topics = [] if not topics else topics.split(",")
         self.autoplay = autoplay
         self.playlist = playlist
         self.subtitles_enough = subtitles_enough
         self.subtitles_setting = (
             subtitles_setting
             if subtitles_setting in (ALL, MATCHING, NONE)
-            else self.to_ted_langcodes(
+            else tedlang.to_ted_langcodes(
                 [lang.strip() for lang in subtitles_setting.split(",")]
             )
         )
         self.threads = threads
         self.yt_downloader = None
 
         # optimization cache
@@ -116,33 +145,32 @@
         self.debug = debug
 
         # class members
         self.videos = []
         self.playlist_title = None
         self.playlist_description = None
         self.source_languages = (
-            [] if not self.languages else self.to_ted_langcodes(self.languages)
+            [] if not self.languages else tedlang.to_ted_langcodes(self.languages)
         )
-        self.zim_lang = None
-        self.already_visited = []
+        self.already_visited = set()
 
         # set and record locale for translations
-        locale_details = get_language_details(locale_name)
+        locale_details = tedlang.get_language_details(locale_name)
         if locale_details["querytype"] != "locale":
             locale_name = locale_details["iso-639-1"]
         try:
             self.locale = setlocale(ROOT_DIR, locale_name)
         except locale.Error:
             logger.error(
                 f"No locale for {locale_name}. Use --locale to specify it. "
                 "defaulting to en_US"
             )
             self.locale = setlocale(ROOT_DIR, "en")
         # locale's language code
-        self.locale_name = self.to_ted_langcodes(locale_name)
+        self.locale_ted_codes = tedlang.to_ted_langcodes(locale_name)
 
     @property
     def templates_dir(self):
         return ROOT_DIR.joinpath("templates")
 
     @property
     def videos_dir(self):
@@ -160,61 +188,14 @@
     def talks_base_url(self):
         return BASE_URL + "talks/"
 
     @property
     def playlists_base_url(self):
         return BASE_URL + "playlists"
 
-    def append_part1_or_part3(self, lang_code_list, lang_info):
-        """Fills missing ISO languages codes for all in list
-
-        lang_code_list: list og lang codes
-        lang_info: see zimscraperlib.i18n"""
-
-        # ignore extra language mappings if supplied query was an iso-639-1 code
-        if "part1" in lang_info["iso_types"]:
-            lang_code_list.append(lang_info["iso-639-1"])
-
-        # supplied query was not iso-639-1
-        elif lang_info["iso-639-1"]:
-            lang_code_list.append(lang_info["iso-639-1"])
-            # check for extra language codes to include
-            if lang_info["iso-639-1"] in TEDLANGS["mappings"]:
-                for code in TEDLANGS["mappings"][lang_info["iso-639-1"]]:
-                    lang_code_list.append(code)
-        elif lang_info["iso-639-3"]:
-            lang_code_list.append(lang_info["iso-639-3"])
-        else:
-            supplied_lang = lang_info["query"]
-            logger.error(f"Language {supplied_lang} is not supported by TED")
-
-    def to_ted_langcodes(self, languages):
-        """Converts languages queries into TED language codes
-
-        Examples:
-            ["English", "fr", "hin"] => ["en", "fr", "hi"]
-            ["chi", "fake"] => ["zh", "zh-cn", "zh-tw"]
-        """
-
-        lang_code_list = []
-        for lang in languages:
-            lang_info = get_language_details(lang, failsafe=True)
-            if lang_info:
-                if lang_info["querytype"] == "purecode":
-                    self.append_part1_or_part3(lang_code_list, lang_info)
-                elif lang_info["querytype"] == "locale":
-                    query = lang_info["query"].replace("_", "-")
-                    if query in TEDLANGS["locales"]:
-                        lang_code_list.append(query)
-                    else:
-                        self.append_part1_or_part3(lang_code_list, lang_info)
-                else:
-                    self.append_part1_or_part3(lang_code_list, lang_info)
-        return list(set(lang_code_list))
-
     def extract_videos_from_playlist(self, playlist):
         """extracts metadata for all videos in the given playlist
 
         calls extract_video_info on all links to get this data
         """
 
         playlist_url = f"{self.playlists_base_url}/{playlist}"
@@ -225,24 +206,59 @@
         self.playlist_description = soup.find(
             "p", attrs={"class": "text-base"}
         ).string  # pyright: ignore
 
         for element in video_elements:
             relative_path = element.get("href")
             url = urllib.parse.urljoin(self.talks_base_url, relative_path)
-            if self.extract_info_from_video_page(url):
-                if self.source_languages and len(self.source_languages) > 1:
-                    other_lang_urls = self.generate_urls_for_other_languages(url)
-                    logger.debug(
-                        f"Searching info for the video in other {len(other_lang_urls)} "
-                        "language(s)"
-                    )
-                    for lang_url in other_lang_urls:
-                        self.extract_info_from_video_page(lang_url)
-                    self.already_visited.append(urllib.parse.urlparse(url).path)
+            json_data = self.extract_info_from_video_page(url)
+
+            if json_data is not None:
+                player_data = json_data["playerData"]
+                lang_code = json_data["language"]
+                if self.source_languages:
+                    # If the first video which was fetched is in source_languages,
+                    # save it.
+                    if lang_code in self.source_languages:
+                        self.update_videos_list_from_info(json_data)
+                    # Determine the next languages to fetch from source_languages
+                    other_languages = [
+                        code for code in self.source_languages if code != lang_code
+                    ]
+                else:
+                    # No languages were specified. Save the first video
+                    self.update_videos_list_from_info(json_data)
+                    # We use the the languages returned from the first
+                    # video to generate other language urls.
+                    other_languages = [
+                        language["languageCode"]
+                        for language in player_data["languages"]
+                        if language["languageCode"] != lang_code
+                    ]
+
+                if not other_languages:
+                    # No need to generate urls for other languages as the list
+                    # is empty
+                    self.already_visited.add(urllib.parse.urlparse(url).path)
+                    continue
+
+                other_lang_urls = self.generate_urls_for_other_languages(
+                    url, other_languages
+                )
+
+                logger.debug(
+                    f"Searching info for the video in other {len(other_lang_urls)} "
+                    "other language(s)"
+                )
+                for lang_url in other_lang_urls:
+                    data = self.extract_info_from_video_page(lang_url)
+                    if data is not None:
+                        self.update_videos_list_from_info(data)
+
+                self.already_visited.add(urllib.parse.urlparse(url).path)
             logger.debug(f"Seen {relative_path}")
         logger.debug(f"Total videos found on playlist: {len(video_elements)}")
         if not video_elements:
             raise ValueError("Wrong playlist ID supplied. No videos found")
 
     def generate_search_results(self, topic):
         """generates a search results and returns the total number of videos scraped"""
@@ -291,62 +307,111 @@
         total_videos_scraped = self.generate_search_results(topic)
         logger.info(f"Total video links found in {topic}: {total_videos_scraped}")
         if total_videos_scraped == 0:
             return False
         return True
 
     def update_zim_metadata(self):
-        if not self.languages:
-            self.zim_lang = "eng"
-        elif len(self.source_languages) > 1:
-            self.zim_lang = "mul"
-        else:
-            lang_info = get_language_details(self.source_languages[0], failsafe=True)
-            if lang_info:
-                self.zim_lang = lang_info["iso-639-3"]
-            else:
-                self.zim_lang = "eng"
-
         if self.playlist:
             if not self.title:
                 self.title = self.playlist_title.strip()  # pyright: ignore
-            if not self.description:
-                self.description = self.playlist_description.strip()  # pyright: ignore
+            default_description = self.playlist_description.strip()  # pyright: ignore
         elif len(self.topics) > 1:
             if not self.title:
                 self.title = "TED Collection"
-            if not self.description:
-                self.description = "A selection of TED videos from several topics"
+            default_description = "A selection of TED videos from several topics"
         else:
             topic_str = self.topics[0].replace("+", " ")
             if not self.title:
                 self.title = f"{topic_str.capitalize()} from TED"
-            if not self.description:
-                self.description = f"A selection of {topic_str} videos from TED"
+            default_description = f"A selection of {topic_str} videos from TED"
+
+        # update description and long_description if not already set by user input,
+        # based on default_description potentially retrieved from playlist / topics
+        # compute_descriptions always returns valid description and long description
+        # when based on default_description
+        self.description, self.long_description = compute_descriptions(
+            default_description=default_description,
+            user_description=self.description,
+            user_long_description=self.long_description,
+        )
+
+        # Compute ZIM language (first call, approximation since few videos might
+        # fail to download and finally not be added to the ZIM ; this however helps to
+        # ensure that ZIM metadata is OK)
+        self.compute_zim_languages()
+
+    def compute_zim_languages(self):
+        """Compute the ZIM language metadata based on expected videos"""
+
+        # count the number of videos per audio language
+        audio_lang_counts = {
+            lang: len(list(group))
+            for lang, group in groupby(
+                [video["native_talk_language"] for video in self.videos]
+            )
+        }
 
-    def get_display_name(self, lang_code, lang_name):
-        """Display name for language"""
+        # count the number of videos per subtitle language
+        subtitle_lang_counts = {
+            lang: len(list(group))
+            for lang, group in groupby(
+                [
+                    subtitle["languageCode"]
+                    for video in self.videos
+                    for subtitle in video["subtitles"]
+                ]
+            )
+        }
 
-        lang_info = get_language_details(lang_code, failsafe=True)
-        if lang_code != "en" and lang_info:
-            return lang_info["native"] + " - " + lang_name
-        return lang_name
+        # Attribute 10 "points" score to language in video audio and 1 "point" score
+        # to language in video subtitle
+        scored_languages = {
+            k: 10 * audio_lang_counts.get(k, 0) + subtitle_lang_counts.get(k, 0)
+            for k in list(audio_lang_counts.keys()) + list(subtitle_lang_counts.keys())
+        }
+
+        sorted_ted_languages = [
+            lang_code
+            for lang_code, _ in sorted(
+                scored_languages.items(), key=lambda item: -item[1]
+            )
+        ]
+
+        # compute the mappings from TED to ISO639-3 code and set ZIM language
+        mapping = tedlang.ted_to_iso639_3_langcodes(sorted_ted_languages)
+        self.zim_languages = ",".join(
+            [mapping[code] for code in sorted_ted_languages if mapping[code]]
+        )
+
+        # Display a clear warning on languages which have been ignored due to missing
+        # ISO639-3 codes
+        ignored_ted_codes = [code for code in sorted_ted_languages if not mapping[code]]
+        if len(ignored_ted_codes):
+            logger.warning(
+                "Some languages have not been added to ZIM metadata due to missing "
+                f"ISO639-3 code: {ignored_ted_codes}"
+            )
+
+        if not self.disable_metadata_checks:
+            # Validate ZIM languages
+            validate_language("Language", self.zim_languages)
 
     def get_subtitle_dict(self, lang):
         """dict of language name and code from a larger dict lang
 
         Example:
         {
             'languageCode': 'en',
             'languageName': 'English'
         }
         """
 
         return {
-            "languageName": self.get_display_name(
+            "languageName": tedlang.get_display_name(
                 lang["languageCode"], lang["languageName"]
             ),
             "languageCode": lang["languageCode"],
         }
 
     def generate_subtitle_list(self, video_id, langs, page_lang, audio_lang):
         """List of all subtitle languages with link to their pages"""
@@ -379,41 +444,130 @@
                     for lang in langs
                     if lang["languageCode"] in self.subtitles_setting
                     or lang["languageCode"] in self.source_languages
                 ]
 
         return update_subtitles_list(video_id, subtitles)
 
-    def generate_urls_for_other_languages(self, url):
+    def generate_urls_for_other_languages(self, url, languages):
         """Possible URLs for other requested languages based on a video url"""
 
         urls = []
         page_lang, query = self.get_lang_code_from_url(
             url, with_full_query=True
         )  # pyright: ignore[reportGeneralTypeIssues]
         url_parts = list(urllib.parse.urlparse(url))
 
         # update the language query field value with other languages and form URLs
-        for language in self.source_languages:
+        for language in languages:
             if language != page_lang:
                 query.update({"language": language})
                 url_parts[4] = urllib.parse.urlencode(query)
                 urls.append(urllib.parse.urlunparse(url_parts))
         return urls
 
     def extract_videos_in_search_results(self, result_json):
         hits = result_json["results"][0]["hits"]
         nb_extracted = 0
         nb_listed = len(hits)
         logger.debug(f"{nb_listed} video(s) found on current page")
         for hit in hits:
             url = urllib.parse.urljoin(self.talks_base_url, hit["slug"])
-            if self.extract_info_from_video_page(url):
-                nb_extracted += 1
+            json_data = self.extract_info_from_video_page(url)
+
+            if json_data is None:
+                continue
+
+            lang_code = json_data["language"]
+            player_data = json_data["playerData"]
+            # we need to filter videos since this has not been done
+            # before for topics with the "new" search page (2023)
+            if self.source_languages:
+                # If the first video which was fetched is in self.source_languages
+                # save it and increment the counter.
+                if (
+                    lang_code in self.source_languages
+                    and self.update_videos_list_from_info(json_data)
+                ):
+                    nb_extracted += 1
+
+                # Determine the next languages to fetch from source_languages
+                other_languages = [
+                    code for code in self.source_languages if code != lang_code
+                ]
+
+                # If there are any valid language codes which can be fetched, fetch them
+                # and save accordingly
+                if other_languages:
+                    other_lang_urls = self.generate_urls_for_other_languages(
+                        url, other_languages
+                    )
+                    logger.debug(
+                        f"Searching info for the video in {len(other_lang_urls)} "
+                        "other language(s)"
+                    )
+                    for lang_url in other_lang_urls:
+                        data = self.extract_info_from_video_page(lang_url)
+                        if data is not None and self.update_videos_list_from_info(data):
+                            # It is possible that this is the first time we
+                            # are saving this video as the first video might
+                            # not necessarily be in the source_languages.
+                            # We increment the counter relying on the fact that
+                            # update_videos_list returns True only if this
+                            # is the first time we are saving the video.
+                            nb_extracted += 1
+
+                if lang_code not in self.source_languages:
+                    # Video language fetched is not among the selected ones, we have to
+                    # check subtitles if they are enough
+                    if not self.subtitles_enough:
+                        logger.debug(
+                            f"Ignoring video in non-selected language {lang_code}"
+                        )
+                    else:
+                        matching_languages = [
+                            lang
+                            for lang in player_data["languages"]
+                            if lang["languageCode"] in self.source_languages
+                        ]
+                        if len(matching_languages) == 0:
+                            logger.debug(
+                                "Ignoring video without a selected language"
+                                "in audio or subtitles"
+                            )
+            else:
+                # Since we are searching for all languages, first update the
+                # videos list with the data we just scraped.
+                if self.update_videos_list_from_info(json_data):
+                    nb_extracted += 1
+
+                # We use the the languages returned from the json_data of
+                # this video to generate other language urls
+                other_languages = []
+                for language in player_data["languages"]:
+                    #  Do not include the language of the video that was just scraped
+                    if language["languageCode"] == lang_code:
+                        continue
+                    other_languages.append(language["languageCode"])
+
+                if other_languages:
+                    other_lang_urls = self.generate_urls_for_other_languages(
+                        url, other_languages
+                    )
+                    logger.debug(
+                        f"Searching info for the video in {len(other_lang_urls)} "
+                        "other language(s)"
+                    )
+                    for lang_url in other_lang_urls:
+                        data = self.extract_info_from_video_page(lang_url)
+                        if data is not None:
+                            self.update_videos_list_from_info(data)
+
             logger.debug(f"Seen {hit['slug']}")
+            self.already_visited.add(urllib.parse.urlparse(url).path)
         return nb_extracted, nb_listed
 
     def get_lang_code_from_url(self, url, *, with_full_query=False):
         """gets the queried language code from a ted talk url"""
 
         # sample - https://www.ted.com/talks/alex_rosenthal_the_gauntlet_think_like_a_coder_ep_8?language=ja
         url_parts = list(urllib.parse.urlparse(url))
@@ -423,28 +577,38 @@
         current_lang = query.get("language")
         if with_full_query:
             return current_lang, query
         return current_lang
 
     def extract_download_link(self, talk_data):
         """Returns download link / youtube video ID for a TED video"""
-
         if (
             isinstance(talk_data.get("resources", {}).get("h264"), list)
             and len(talk_data["resources"]["h264"])
             and talk_data["resources"]["h264"][0].get("file")
         ):
             logger.debug(
                 "Using h264 resource link for bitrate="
                 f"{talk_data['resources']['h264'][0].get('bitrate')}"
             )
-            return talk_data["resources"]["h264"][0]["file"]
+            download_link = talk_data["resources"]["h264"][0]["file"]
+        else:
+            download_link = None
 
-        logger.error("No download link found for the video")
-        return None
+        if (
+            talk_data.get("external", {}).get("service")
+            and talk_data["external"]["service"] == "YouTube"
+            and talk_data["external"].get("code")
+        ):
+            logger.debug(f"Found Youtube ID {talk_data['external']['code']}")
+            youtube_id = talk_data["external"]["code"]
+        else:
+            youtube_id = None
+
+        return download_link, youtube_id
 
     def update_videos_list(
         self,
         video_id,
         lang_code,
         lang_name,
         title,
@@ -452,102 +616,112 @@
         speaker,
         speaker_profession,
         speaker_bio,
         speaker_picture,
         date,
         thumbnail,
         video_link,
+        youtube_id,
         length,
         subtitles,
+        metadata_link,
+        native_talk_language,
     ):
         # append to self.videos and return if not present
         if not [video for video in self.videos if video.get("id", None) == video_id]:
+
+            # Fetch metadata and compute subtitles offset (sum up all domains durations
+            # up till the primary domain) - we do it only once per video since this
+            # information is same for all languages
+            subtitles_offset = 0
+            if metadata_link:
+                metadatas = request_url(metadata_link).json()
+                if "domains" in metadatas:
+                    for domain in metadatas["domains"]:
+                        if domain["primaryDomain"]:
+                            break
+                        subtitles_offset += int(domain["duration"] * 1000)
+
             self.videos.append(
                 {
                     "id": video_id,
                     "languages": [
                         {
                             "languageCode": lang_code,
-                            "languageName": self.get_display_name(lang_code, lang_name),
+                            "languageName": tedlang.get_display_name(
+                                lang_code, lang_name
+                            ),
                         }
                     ],
                     "title": [{"lang": lang_code, "text": title}],
                     "description": [{"lang": lang_code, "text": description}],
                     "speaker": speaker,
                     "speaker_profession": speaker_profession,
                     "speaker_bio": speaker_bio,
                     "speaker_picture": speaker_picture,
                     "date": date,
                     "thumbnail": thumbnail,
                     "video_link": video_link,
+                    "youtube_id": youtube_id,
                     "length": length,
                     "subtitles": subtitles,
+                    "subtitles_offset": subtitles_offset,
+                    "native_talk_language": native_talk_language,
                 }
             )
             logger.debug(f"Successfully inserted video {video_id} into video list")
             return True
 
         # update localized meta for video if already in self.videos
         # based on --subtitles=matching
         logger.debug(f"Video {video_id} already present in video list")
         for index, video in enumerate(self.videos):
+            if video.get("failed", False):
+                continue
             if video.get("id", None) == video_id:
                 if {"lang": lang_code, "text": title} not in video["title"]:
                     self.videos[index]["title"].append(
                         {"lang": lang_code, "text": title}
                     )
                     self.videos[index]["description"].append(
                         {"lang": lang_code, "text": description}
                     )
                     self.videos[index]["languages"].append(
                         {
                             "languageCode": lang_code,
-                            "languageName": self.get_display_name(lang_code, lang_name),
+                            "languageName": tedlang.get_display_name(
+                                lang_code, lang_name
+                            ),
                         }
                     )
-                if self.subtitles_setting in (MATCHING, NONE):
+
+                if self.subtitles_setting in (MATCHING, NONE) and len(subtitles) == 1:
                     self.videos[index]["subtitles"] += subtitles
         return False
 
-    def extract_video_info_from_json(self, json_data):
-        player_data = json.loads(json_data["playerData"])
+    def get_lang_code_and_name(self, json_data):
+        player_data = json_data["playerData"]
         lang_code = json_data["language"]
         try:
             lang_name = [
                 lang["languageName"]
                 for lang in player_data["languages"]
                 if lang["languageCode"] == lang_code
             ][-1]
         except Exception as exc:
             logger.warning(f"player data has no entry for {lang_code}: {exc}")
             lang_name = lang_code
-        if self.topics:
-            # we need to filter videos since this has not been done before for topics
-            # with the "new" search page (2023)
-            if lang_code not in self.source_languages:
-                # video language is not among the selected ones, we have to check
-                # subtitles if they are enough
-                if not self.subtitles_enough:
-                    logger.debug(f"Ignoring video in non-selected language {lang_code}")
-                    return False
-                else:
-                    matching_languages = [
-                        lang
-                        for lang in player_data["languages"]
-                        if lang["languageCode"] in self.source_languages
-                    ]
-                    if len(matching_languages) == 0:
-                        logger.debug(
-                            "Ignoring video without a selected language in audio or "
-                            "subtitles"
-                        )
-                        return False
 
-        native_talk_language = player_data["nativeLanguage"]
+        return lang_code, lang_name
 
+    def update_videos_list_from_info(self, json_data):
+        player_data = json_data["playerData"]
+        lang_code, lang_name = self.get_lang_code_and_name(json_data)
+
+        native_talk_language = player_data["nativeLanguage"]
         # Extract the speaker of the TED talk
         if len(json_data["speakers"]):
             if isinstance(json_data["speakers"], dict):
                 speaker_info = (
                     json_data["speakers"]["nodes"][0]
                     if json_data["speakers"].get("nodes", [])
                     else {}
@@ -577,23 +751,30 @@
         # Extract the ted talk details from json
         video_id = json_data["id"]
         speaker_profession = speaker_info.get("description")
         speaker_bio = speaker_info.get("whoTheyAre", "-")
         speaker_picture = speaker_info.get("photoUrl", "-")
         title = json_data.get("title", "n/a")
         description = json_data.get("description", "n/a")
-        date = dateutil.parser.parse(json_data["recordedOn"]).strftime("%d %B %Y")
+        date = (
+            dateutil.parser.parse(json_data["recordedOn"]).strftime("%d %B %Y")
+            if json_data.get("recordedOn")
+            else "Unknown"
+        )
         length = int(json_data["duration"]) // 60
         thumbnail = player_data["thumb"]
-        video_link = self.extract_download_link(player_data)
-        if not video_link:
-            logger.error("No suitable download link found. Skipping video")
+        video_link, youtube_id = self.extract_download_link(player_data)
+        if not video_link and not youtube_id:
+            logger.error(
+                "No suitable download link or Youtube ID found. Skipping video"
+            )
             return False
 
         langs = player_data["languages"]
+        metadata_link = player_data["resources"]["hls"]["metadata"]
         subtitles = self.generate_subtitle_list(
             video_id, langs, lang_code, native_talk_language
         )
         return self.update_videos_list(
             video_id=video_id,
             lang_code=lang_code,
             lang_name=lang_name,
@@ -602,54 +783,77 @@
             speaker=speaker,
             speaker_profession=speaker_profession,
             speaker_bio=speaker_bio,
             speaker_picture=speaker_picture,
             date=date,
             thumbnail=thumbnail,
             video_link=video_link,
+            youtube_id=youtube_id,
             length=length,
             subtitles=subtitles,
+            metadata_link=metadata_link,
+            native_talk_language=native_talk_language,
         )
 
-    def extract_info_from_video_page(self, url, retry_count=0):
-        """extract all info from a TED video page url and update self.videos"""
+    def extract_info_from_video_page(
+        self, url: str, retry_count: int = 0
+    ) -> dict | None:
+        """extract all info from a TED video page url.
+        Returns a dict containign the video information if search was
+        successful, else None.
+        """
 
         # Every TED video page has a <script>-tag with a Javascript
         # object with JSON in it. We will just stip away the object
         # signature and load the json to extract meta-data out of it.
         # returns True if successfully scraped new video
 
         # don't scrape if URL already visited
         if urllib.parse.urlparse(url).path in self.already_visited:
-            return False
+            return None
 
         # don't scrape if maximum retry count is reached
         if retry_count > 5:  # noqa: PLR2004
             logger.error("Max retries exceeded. Skipping video")
-            return False
+            return None
 
         logger.debug(f"extract_info_from_video_page: {url}")
-        soup = BeautifulSoup(request_url(url).text, features="html.parser")
+        html_content = request_url(url).text
+        try:
+            soup = BeautifulSoup(html_content, features="html.parser")
 
-        json_data = json.loads(
-            soup.find("script", attrs={"id": "__NEXT_DATA__"}).string  # pyright: ignore
-        )["props"]["pageProps"]["videoData"]
+            json_data = json.loads(
+                soup.find(
+                    "script", attrs={"id": "__NEXT_DATA__"}
+                ).string  # pyright: ignore
+            )["props"]["pageProps"]["videoData"]
 
-        requested_lang_code = self.get_lang_code_from_url(url)
-        if requested_lang_code and json_data["language"] != requested_lang_code:
+            requested_lang_code = self.get_lang_code_from_url(url)
+            if requested_lang_code and json_data["language"] != requested_lang_code:
+                logger.error(
+                    f"Video has not yet been translated into {requested_lang_code}"
+                )
+                return None
+            # Desrialize the data at json_data["playerData"] into a dict
+            # and overwrite it accordingly
+            json_data["playerData"] = json.loads(json_data["playerData"])
+            return json_data
+        except Exception:
             logger.error(
-                f"Video has not yet been translated into {requested_lang_code}"
+                f"Problem occured while parsing {url}. HTML content was:\n"
+                f"{html_content}"
             )
-            return False
-        return self.extract_video_info_from_json(json_data)
+            raise
 
     def add_default_language(self):
         """add metatada in default language (english or first avail) on all videos"""
 
         for video in self.videos:
+            if video.get("failed", False):
+                continue
             en_found = False
             for index, lang in enumerate(video["languages"]):
                 if lang["languageCode"] == "en":
                     en_found = True
                     video["title"] = [
                         {"lang": "default", "text": video["title"][index]["text"]}
                     ] + video["title"]
@@ -671,26 +875,28 @@
     def render_video_pages(self):
         # Render static html pages from the scraped video data and
         # save the pages in build_dir/<video-id>/index.html
         env = jinja2.Environment(
             loader=jinja2.FileSystemLoader(str(self.templates_dir)), autoescape=True
         )
         for video in self.videos:
+            if video.get("failed", False):
+                continue
             titles = video["title"]
             html = env.get_template("article.html").render(
                 speaker=video["speaker"],
                 languages=video["subtitles"],
                 speaker_bio=video["speaker_bio"].replace("Full bio", ""),
                 speaker_img=video["speaker_picture"],
                 date=video["date"],
                 profession=video["speaker_profession"],
                 video_format=self.video_format,
                 autoplay=self.autoplay,
                 video_id=str(video["id"]),
-                title=get_main_title(titles, self.locale_name),
+                title=get_main_title(titles, self.locale_ted_codes),
                 titles=titles,
                 descriptions=video["description"],
                 back_to_list=_("Back to the list"),
             )
             html_path = self.build_dir.joinpath(video["slug"])
             with open(html_path, "w", encoding="utf-8") as html_page:
                 html_page.write(html)  # pyright: ignore[reportGeneralTypeIssues]
@@ -699,14 +905,15 @@
         # Render the homepage
         env = jinja2.Environment(
             loader=jinja2.FileSystemLoader(str(self.templates_dir)), autoescape=True
         )
         all_langs = {
             language["languageCode"]: language["languageName"]
             for video in self.videos
+            if not video.get("failed", False)
             for language in video["subtitles"] + video["languages"]
         }
         languages = [
             {"languageName": value, "languageCode": key}
             for key, value in all_langs.items()
         ]
         languages = sorted(languages, key=lambda x: x["languageName"])
@@ -734,14 +941,16 @@
         )
 
     def generate_datafile(self):
         """Generate data.js inside assets folder"""
 
         video_list = []
         for video in self.videos:
+            if video.get("failed", False):
+                continue
             lang_codes = [lang["languageCode"] for lang in video["subtitles"]] + [
                 lang["languageCode"] for lang in video["languages"]
             ]
             json_data = {
                 "languages": list(set(lang_codes)),
                 "id": video["id"],
                 "description": video["description"],
@@ -848,14 +1057,15 @@
             raise Exception("yt_downloader is not setup")
 
         # set up variables
         video_id = str(video["id"])
         # Take the english version of title or else whatever language it's available in
         video_title = video["title"][0]["text"]
         video_link = video["video_link"]
+        youtube_id = video["youtube_id"]
         video_speaker = video["speaker_picture"]
         video_thumbnail = video["thumbnail"]
         video_dir = self.videos_dir.joinpath(video_id)
         org_video_file_path = video_dir.joinpath("video.mp4")
         req_video_file_path = video_dir.joinpath(f"video.{self.video_format}")
         speaker_path = video_dir.joinpath("speaker.webp")
         thumbnail_path = video_dir.joinpath("thumbnail.webp")
@@ -876,26 +1086,49 @@
             else None
         )
         if self.s3_storage:
             downloaded_from_cache = self.download_from_cache(
                 s3_key, req_video_file_path, preset.VERSION
             )
         if not downloaded_from_cache:
-            try:
-                if "https://" not in video_link:
+            downloaded = False
+            # First try to download from video link
+            if video_link:
+                try:
+                    save_large_file(video_link, org_video_file_path)
+                    downloaded = True
+                except Exception as exc:
+                    logger.error(
+                        f"Could not download from {video_link} for "
+                        f"{org_video_file_path}",
+                    )
+                    logger.debug("", exc_info=exc)
+                    org_video_file_path.unlink(missing_ok=True)
+            # Second try to download from youtube ID (used both when no video link AND
+            # when video link download failed - we experience sometimes 403 errors on
+            # video link, see #167)
+            if not downloaded and youtube_id:
+                try:
                     options = (
                         BestWebm if self.video_format == "webm" else BestMp4
                     ).get_options(
                         target_dir=video_dir, filepath=pathlib.Path("video.%(ext)s")
                     )
-                    self.yt_downloader.download(video_link, options)
-                else:
-                    save_large_file(video_link, org_video_file_path)
-            except Exception:
-                logger.error(f"Could not download {org_video_file_path}")
+                    with yt_dlp.YoutubeDL(options) as ydl:
+                        ydl.download([youtube_id])
+                    downloaded = True
+                except Exception as exc:
+                    logger.error(
+                        f"Could not download from {youtube_id} for "
+                        f"{org_video_file_path}",
+                    )
+                    logger.debug("", exc_info=exc)
+            if not downloaded:
+                video["failed"] = True
+                return
 
         # download speaker and thumbnail images
         self.download_speaker_image(video_id, video_title, video_speaker, speaker_path)
         self.download_thumbnail(video_id, video_title, video_thumbnail, thumbnail_path)
 
         # recompress if necessary
         try:
@@ -905,15 +1138,17 @@
                     video_id,
                     preset,
                     self.video_format,
                     self.low_quality,
                 )
         except Exception as e:
             logger.error(f"Failed to post process video {video_id}")
-            logger.debug(e)
+            logger.debug("", exc_info=e)
+            video["failed"] = True
+            return
         else:
             # upload to cache only if recompress was successful
             if self.s3_storage and not downloaded_from_cache:
                 self.upload_to_cache(s3_key, req_video_file_path, preset.VERSION)
 
     def download_video_files_parallel(self):
         """download videos and images parallely"""
@@ -921,14 +1156,15 @@
         self.yt_downloader = YoutubeDownloader(threads=1)
         with concurrent.futures.ThreadPoolExecutor(
             max_workers=self.threads
         ) as executor:
             fs = [
                 executor.submit(self.download_video_files, video)
                 for video in self.videos
+                if not video.get("failed", False)
             ]
             concurrent.futures.wait(fs, return_when=concurrent.futures.ALL_COMPLETED)
         self.yt_downloader.shutdown()
 
     def download_subtitles(self, index, video):
         """download, converts and writes VTT subtitles
 
@@ -945,18 +1181,22 @@
         if not subs_dir.exists():
             subs_dir.mkdir(parents=True)
         else:
             logger.debug("Subs dir exists already")
 
         # download subtitles
         logger.debug(f"Downloading subtitles for {video['title'][0]['text']}")
+        if video["subtitles_offset"]:
+            logger.debug(f"Subtitles will be offset by {video['subtitles_offset']} ms")
         valid_subs = []
         for subtitle in video["subtitles"]:
             time.sleep(0.5)  # throttling
-            vtt_subtitle = WebVTT(subtitle["link"]).convert()
+            vtt_subtitle = WebVTT(subtitle["link"]).convert(
+                offset=video["subtitles_offset"]
+            )
             if not vtt_subtitle:
                 logger.error(
                     f"Subtitle file for {subtitle['languageCode']} could not be created"
                 )
                 continue
             valid_subs.append(subtitle)
             vtt_path = subs_dir.joinpath(f"subs_{subtitle['languageCode']}.vtt")
@@ -969,14 +1209,15 @@
 
         with concurrent.futures.ThreadPoolExecutor(
             max_workers=self.threads
         ) as executor:
             fs = [
                 executor.submit(self.download_subtitles, index, video)
                 for index, video in enumerate(self.videos)
+                if not video.get("failed", False)
             ]
             concurrent.futures.wait(fs, return_when=concurrent.futures.ALL_COMPLETED)
 
     def s3_credentials_ok(self):
         logger.info("Testing S3 Optimization Cache credentials")
         self.s3_storage = KiwixStorage(self.s3_url_with_credentials)
         if not self.s3_storage.check_credentials(
@@ -1069,17 +1310,27 @@
 
         self.add_default_language()
         self.update_zim_metadata()
         self.download_video_files_parallel()
         self.download_subtitles_parallel()
         self.render_home_page()
         self.render_video_pages()
+        self.compute_zim_languages()  # Compute ZIM language (second/final call)
         self.copy_files_to_build_directory()
         self.generate_datafile()
 
+        # display final stats and abort processing if no videos are left
+        nb_success = sum(
+            0 if video.get("failed", False) else 1 for video in self.videos
+        )
+        nb_failed = sum(1 if video.get("failed", False) else 0 for video in self.videos)
+        logger.debug(f"Stats: {nb_success} videos ok, {nb_failed} videos failed")
+        if nb_success == 0:
+            raise Exception("No successfull video, aborting ZIM creation")
+
         # zim creation and cleanup
         if not self.no_zim:
             self.fname = (
                 self.fname or f"{self.name.replace(' ', '-')}_{{period}}.zim"
             ).format(
                 period=datetime.datetime.now().strftime("%Y-%m")  # noqa: DTZ005
             )
@@ -1087,21 +1338,23 @@
             if not self.output_dir.exists():
                 self.output_dir.mkdir(parents=True)
             make_zim_file(
                 build_dir=self.build_dir,
                 fpath=self.output_dir.joinpath(self.fname),
                 name=self.name,
                 main_page="index",
-                favicon="favicon.png",
+                illustration="favicon.png",
                 title=self.title,
                 description=self.description,
-                language=self.zim_lang,  # pyright: ignore[reportGeneralTypeIssues]
+                language=self.zim_languages,  # pyright: ignore[reportArgumentType]
+                long_description=self.long_description,  # pyright: ignore[reportArgumentType]
                 creator=self.creator,
                 publisher=self.publisher,
-                tags=[*self.tags, "_category:ted", "ted", "_videos:yes"],
+                tags=self.tags,
                 scraper=SCRAPER,
+                disable_metadata_checks=self.disable_metadata_checks,
             )
             if not self.keep_build_dir:
                 logger.info("removing temp folder")
                 shutil.rmtree(self.build_dir, ignore_errors=True)
 
         logger.info("Done Everything")
```

### Comparing `ted2zim-2.1.0/src/ted2zim/utils.py` & `ted2zim-3.0.0/src/ted2zim/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     return list(filter(lambda x: x.startswith(f"--{arg_name}"), all_args))
 
 
 def update_subtitles_list(video_id, language_list):
     """adds `link` to each language dict containing the subtitle url"""
 
     for language in language_list:
-        language[
-            "link"
-        ] = f"https://www.ted.com/talks/subtitles/id/{video_id}/lang/{language['languageCode']}"
+        language["link"] = (
+            f"https://www.ted.com/talks/subtitles/id/{video_id}/lang/{language['languageCode']}"
+        )
 
     return language_list
 
 
 def request_url(url, json_data=None):
     """performs an HTTP request and returns the response, either GET or POST
 
@@ -71,46 +71,45 @@
             raise ConnectionRefusedError(
                 f"Failed to download {url} after {attempt} attempts "
                 f"(HTTP {req.status_code})"
             )
 
 
 class WebVTT:
-
     """TED JSON subtitles to WebVTT"""
 
     def __init__(self, url):
         self.url = url
 
-    def convert(self):
+    def convert(self, offset):
         """download and convert its URL to WebVTT text"""
         req = request_url(self.url)
 
         if req.status_code == HTTPStatus.NOT_FOUND:
             return None
         try:
             source_subtitles = req.json()
         except json.JSONDecodeError:
             return None
 
-        return self.json_to_vtt(source_subtitles)
+        return self.json_to_vtt(source_subtitles, offset)
 
     @staticmethod
     def miliseconds_to_human(miliseconds):
         """Human/VTT formatted time code from miliseconds
 
         ex: 00:00:00.000"""
 
         hours, remainder = divmod(miliseconds, 3600000)
         minutes, remainder = divmod(remainder, 60000)
         seconds, miliseconds = divmod(remainder, 1000)
         return f"{hours:02}:{minutes:02}:{seconds:02}.{miliseconds:03}"
 
     @staticmethod
-    def json_to_vtt(json_subtitles, offset=11820):
+    def json_to_vtt(json_subtitles, offset):
         """WebVTT string from TED JSON subtitles list
 
         TED format: {"captions": [
             {'duration': 1726,
              'content': 'And more concretely,',
              'startOfParagraph': False,
              'startTime': 382083
@@ -145,19 +144,24 @@
         fh.close()
         yield fpath
     finally:
         if fpath:
             fpath.unlink()
 
 
-def get_main_title(titles, prefered_lang):
+def get_main_title(titles, locale_ted_codes: list[str]):
     """main title from list of titles dict based on language pref with fallback"""
     missing = "n/a"
     if not titles:
         return missing
 
-    def get_for(lang):
+    def get_for(lang: str):
         filtered = [title["text"] for title in titles if title["lang"] == lang]
         if filtered:
             return filtered[0]
 
-    return get_for(prefered_lang) or get_for("default") or get_for("en") or missing
+    for code in [*locale_ted_codes, "default", "en"]:
+        title = get_for(code)
+        if title:
+            return title
+
+    return missing
```

### Comparing `ted2zim-2.1.0/src/ted2zim/locale/hi/LC_MESSAGES/messages.po` & `ted2zim-3.0.0/src/ted2zim/locale/hi/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `ted2zim-2.1.0/src/ted2zim/multi/entrypoint.py` & `ted2zim-3.0.0/src/ted2zim/multi/entrypoint.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         "--topics",
         help="Comma seperated list of topics to scrape. Should be same as on "
         "ted.com/talks. Pass all to scrape all",
     )
 
     parser.add_argument(
         "--playlists",
-        help="Comma seperated list of playlist IDs to scrape. Pass all to scrape all",
+        help="Comma separated list of playlist IDs to scrape. Pass all to scrape all",
     )
 
     parser.add_argument(
         "--indiv-zims",
         help="Make individual ZIMs for topics. Multiple ZIMs are always created for "
         "multiple playlists",
         action="store_true",
@@ -69,14 +69,21 @@
     parser.add_argument(
         "--version",
         help="Display scraper version and exit",
         action="version",
         version=SCRAPER,
     )
 
+    parser.add_argument(
+        "--disable-metadata-checks",
+        help="Disable validity checks of metadata according to openZIM conventions",
+        action="store_true",
+        default=False,
+    )
+
     args, extra_args = parser.parse_known_args()
 
     # prevent launching without any topic(s)/playlist(s)
     if (
         not args.playlists
         and not args.topics
         and not has_argument("playlist", extra_args)
```

### Comparing `ted2zim-2.1.0/src/ted2zim/multi/scraper.py` & `ted2zim-3.0.0/src/ted2zim/multi/scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 class TedHandler:
     def __init__(
         self,
         options,
         extra_args,
     ):
         self.debug = False
+        self.disable_metadata_checks = False
         # save options as properties
         for key, value in options.items():
             if key not in ["topics", "playlists"]:
                 setattr(self, key, value)
             else:
                 value_list = (
                     [] if not value else [val.strip() for val in value.split(",")]
@@ -279,14 +280,17 @@
 
         # append regular ted2zim args
         args += self.extra_args
 
         if self.debug:
             args += ["--debug"]
 
+        if self.disable_metadata_checks:
+            args += ["--disable-metadatachecks"]
+
         logger.debug(nicer_args_join(args))
         process = subprocess.run(
             args,
             stdout=subprocess.PIPE,
             stderr=subprocess.STDOUT,
             text=True,
             check=False,
@@ -308,14 +312,16 @@
                 self.playlists[0],
             ]
         else:
             raise ValueError(f"Unsupported mode {mode}")
         args += self.extra_args
         if self.debug:
             args += ["--debug"]
+        if self.disable_metadata_checks:
+            args += ["--disable-metadatachecks"]
         return subprocess.run(args, check=False).returncode
 
     def fetch_metadata(self):
         """retrieves and loads metadata from --metadata-from"""
 
         if not self.metadata_from:
             return
```

### Comparing `ted2zim-2.1.0/src/ted2zim/templates/article.html` & `ted2zim-3.0.0/src/ted2zim/templates/article.html`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             <img id="backtolist" src="assets/img/TED_small.png" title="{{ back_to_list }}"/>
             <p id="speaker">{{ speaker }}</p>
             {% for title in titles %}
             <p class="title lang-{{ title.lang }}">{{ title.text }}</p>
             {% endfor %}
             <div id="video-wrapper">
                 <video class="video-js vjs-default-skin vjs-fill"
-                    controls preload="auto"
+                    controls preload="auto" playsinline
                     poster="videos/{{ video_id }}/thumbnail.webp"
                     data-setup='{"techOrder": ["html5", "ogvjs"], "ogvjs": {"base": "assets/ogvjs"}, "autoplay": {% if autoplay %}true{% else %}false{% endif %}, "preload": true, "controls": true, "controlBar": {"pictureInPictureToggle":false}}'>
                     <source src="videos/{{ video_id }}/video.{{ video_format }}" type="video/{{ video_format }}" />
                         {% for language in languages %}
                         <track kind="subtitles" src="videos/{{ video_id }}/subs/subs_{{ language.languageCode }}.vtt" srclang="{{ language.languageCode }}" label="{{ language.languageName }}" />
                         {% endfor %}
                 </video>
```

### Comparing `ted2zim-2.1.0/src/ted2zim/templates/favicon.png` & `ted2zim-3.0.0/src/ted2zim/templates/favicon.png`

 * *Files identical despite different names*

### Comparing `ted2zim-2.1.0/src/ted2zim/templates/home.html` & `ted2zim-3.0.0/src/ted2zim/templates/home.html`

 * *Files identical despite different names*

### Comparing `ted2zim-2.1.0/src/ted2zim/templates/assets/app.js` & `ted2zim-3.0.0/src/ted2zim/templates/assets/app.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.1.0/src/ted2zim/templates/assets/article.css` & `ted2zim-3.0.0/src/ted2zim/templates/assets/article.css`

 * *Files identical despite different names*

### Comparing `ted2zim-2.1.0/src/ted2zim/templates/assets/article.js` & `ted2zim-3.0.0/src/ted2zim/templates/assets/article.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -4,15 +4,15 @@
         return null;
     }
     return decodeURI(results[1]) || 0;
 };
 
 window.onload = function() {
     var lang = $.urlParam('lang');
-    if (lang !== "undefined") {
+    if (lang && lang !== "undefined") {
         document.getElementById("title-head").innerHTML = $("p.title.lang-" + lang).text();
         $(".lang-default").css("display", "none");
         $(".lang-" + lang).css("display", "block");
     }
 };
 
 $(document).ready(function() {
```

### Comparing `ted2zim-2.1.0/src/ted2zim/templates/assets/db.js` & `ted2zim-3.0.0/src/ted2zim/templates/assets/db.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.1.0/src/ted2zim/templates/assets/home.css` & `ted2zim-3.0.0/src/ted2zim/templates/assets/home.css`

 * *Files identical despite different names*

### Comparing `ted2zim-2.1.0/src/ted2zim/templates/assets/webp-trigger.js` & `ted2zim-3.0.0/src/ted2zim/templates/assets/webp-trigger.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.1.0/src/ted2zim/templates/assets/font/Roboto-Black.ttf` & `ted2zim-3.0.0/src/ted2zim/templates/assets/font/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `ted2zim-2.1.0/src/ted2zim/templates/assets/font/Roboto-Bold.ttf` & `ted2zim-3.0.0/src/ted2zim/templates/assets/font/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `ted2zim-2.1.0/src/ted2zim/templates/assets/font/Roboto-Light.ttf` & `ted2zim-3.0.0/src/ted2zim/templates/assets/font/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `ted2zim-2.1.0/src/ted2zim/templates/assets/font/Roboto-LightItalic.ttf` & `ted2zim-3.0.0/src/ted2zim/templates/assets/font/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `ted2zim-2.1.0/src/ted2zim/templates/assets/font/Roboto-Regular.ttf` & `ted2zim-3.0.0/src/ted2zim/templates/assets/font/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ted2zim-2.1.0/src/ted2zim/templates/assets/img/TED.png` & `ted2zim-3.0.0/src/ted2zim/templates/assets/img/TED.png`

 * *Files identical despite different names*

### Comparing `ted2zim-2.1.0/src/ted2zim/templates/assets/img/TED_small.png` & `ted2zim-3.0.0/src/ted2zim/templates/assets/img/TED_small.png`

 * *Files identical despite different names*

### Comparing `ted2zim-2.1.0/.gitignore` & `ted2zim-3.0.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -371,12 +371,13 @@
 src/ted2zim/templates/assets/chosen/
 src/ted2zim/templates/assets/jquery.min.js
 src/ted2zim/templates/assets/ogvjs/
 src/ted2zim/templates/assets/videojs-ogvjs.js
 src/ted2zim/templates/assets/polyfills.js
 src/ted2zim/templates/assets/webp-hero.bundle.js
 
-# output dir
+# output and tmp dir
 output
+tmp
 
 # ignore all vscode, this is not standard configuration in this place
-.vscode
+.vscode
```

### Comparing `ted2zim-2.1.0/LICENSE` & `ted2zim-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ted2zim-2.1.0/README.md` & `ted2zim-3.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -9,22 +9,25 @@
 [![PyPI version shields.io](https://img.shields.io/pypi/v/ted2zim.svg)](https://pypi.org/project/ted2zim/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ted2zim.svg)](https://pypi.org/project/ted2zim)
 
 TED (Technology, Entertainment, Design) is a global set of conferences under the slogan "ideas worth spreading". They address a wide range of topics within the research and practice of science and culture, often through storytelling. The speakers are given a maximum of 18 minutes to present their ideas in the most innovative and engaging ways they can. One can eaisly find all the TED videos [here](https://ted.com/talks).
 
 This project is aimed at creating a sustainable solution to make TED accessible offline by creating ZIM files providing these videos in a similar manner like online.
 
+`ted2zim` adheres to openZIM's [Contribution Guidelines](https://github.com/openzim/overview/wiki/Contributing).
+
+`ted2zim` has implemented openZIM's [Python bootstrap, conventions and policies](https://github.com/openzim/_python-bootstrap/docs/Policy.md) **v1.0.1**.
 
 ## Getting started :rocket:
 
 #### Install the dependencies
 Make sure that you have `python3`, `unzip`, `ffmpeg`, `wget` and `curl` installed on your system before running the scraper (otherwise you'll get a warning to install them).
 
 #### Setup the package
-One can easily install the PyPI version but let's setup the source version. 
+One can easily install the PyPI version but let's setup the source version.
 
 First, clone this repository.
 
 If you do not already have it on your system, install hatch to build the software and manage virtual environments (you might be interested by our detailed [Developer Setup](https://github.com/openzim/_python-bootstrap/wiki/Developer-Setup) as well).
 
 ```bash
 pip3 install hatch
```

### Comparing `ted2zim-2.1.0/pyproject.toml` & `ted2zim-3.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,72 +1,78 @@
 [build-system]
-requires = ["hatchling"]
+requires = ["hatchling", "hatch-openzim==0.2.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ted2zim"
-authors = [{ name = "Kiwix", email = "dev@kiwix.org" }]
-keywords = ["kiwix", "zim", "ted", "openzim", "offline"]
-requires-python = ">=3.11,<3.12"
+requires-python = ">=3.12,<3.13"
 description = "Make ZIM file from TED Talks"
 readme = "README.md"
-license = { text = "GPL-3.0-or-later" }
-classifiers = [
-  "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.11",
-  "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
-]
 dependencies = [
-  "python-dateutil==2.8.2",
-  # cannot use 3.x for now, see https://github.com/openzim/ted/issues/152
-  "zimscraperlib==2.1.0",
+  "python-dateutil==2.9.0.post0",
+  "zimscraperlib==3.3.2",
   "requests==2.31.0",
-  "beautifulsoup4==4.9.3",
-  "Jinja2==3.1.2",
+  "beautifulsoup4==4.12.3",
+  "Jinja2==3.1.3",
   "kiwixstorage==0.8.3",
   "pif==0.8.2",
-  "python-slugify==8.0.1",
+  "python-slugify==8.0.4",
+  "yt-dlp", # yt-dlp should be updated as frequently as possible
 ]
-dynamic = ["version"]
+dynamic = ["authors", "classifiers", "keywords", "license", "version", "urls"]
+
+[tool.hatch.metadata]
+allow-direct-references = true
+
+[tool.hatch.metadata.hooks.openzim-metadata]
+kind = "scraper"
+additional-keywords = ["ted"]
+
+[tool.hatch.build.hooks.openzim-build]
+dependencies = [ "zimscraperlib==3.3.2"] # required for fix_ogv_dist
 
 [project.optional-dependencies]
-scripts = ["invoke==2.2.0"]
-lint = ["black==23.12.0", "ruff==0.1.8"]
-check = ["pyright==1.1.341"]
-test = ["pytest==7.4.3", "coverage==7.3.3"]
+scripts = [
+  "invoke==2.2.0",
+]
+lint = [
+  "black==24.4.0",
+  "ruff==0.4.0",
+]
+check = [
+  "pyright==1.1.359",
+]
+test = [
+  "pytest==8.1.1",
+  "coverage==7.4.4",
+]
 dev = [
-  "pre-commit==3.6.0",
-  "debugpy==1.8.0",
+  "pre-commit==3.7.0",
+  "debugpy==1.8.1",
   "ted2zim[scripts]",
   "ted2zim[lint]",
   "ted2zim[test]",
   "ted2zim[check]",
-  # hatchling is a dev dependency only needed for hook development on developer machine
-  "hatchling==1.18.0",
 ]
 
-[project.urls]
-Homepage = "https://github.com/openzim/ted"
-Donate = "https://www.kiwix.org/en/support-us/"
-
 [project.scripts]
 ted2zim = "ted2zim.entrypoint:main"
 ted2zim-multi = "ted2zim.multi.entrypoint:main"
 
 [tool.hatch.version]
 path = "src/ted2zim/__about__.py"
 
 [tool.hatch.build]
 exclude = ["/.github"]
 
-[tool.hatch.build.hooks.custom]
-path = "hatch_build.py"
-
 [tool.hatch.build.targets.wheel]
 packages = ["src/ted2zim"]
+artifacts = [
+  "src/ted2zim/templates/assets/**",
+]
 
 [tool.hatch.envs.default]
 features = ["dev"]
 
 [tool.hatch.envs.test]
 features = ["scripts", "test"]
 
@@ -75,14 +81,15 @@
 run-cov = "inv test-cov --args '{args}'"
 report-cov = "inv report-cov"
 coverage = "inv coverage --args '{args}'"
 html = "inv coverage --html --args '{args}'"
 
 [tool.hatch.envs.lint]
 template = "lint"
+python = "py312"
 skip-install = false
 features = ["scripts", "lint"]
 
 [tool.hatch.envs.lint.scripts]
 black = "inv lint-black --args '{args}'"
 ruff = "inv lint-ruff --args '{args}'"
 all = "inv lintall --args '{args}'"
@@ -95,20 +102,22 @@
 
 [tool.hatch.envs.check.scripts]
 pyright = "inv check-pyright --args '{args}'"
 all = "inv checkall --args '{args}'"
 
 [tool.black]
 line-length = 88
-target-version = ['py311']
+target-version = ['py312']
 
 [tool.ruff]
-target-version = "py311"
+target-version = "py312"
 line-length = 88
 src = ["src"]
+
+[tool.ruff.lint]
 select = [
   "A", # flake8-builtins
   # "ANN",  # flake8-annotations
   "ARG", # flake8-unused-arguments
   # "ASYNC",  # flake8-async
   "B", # flake8-bugbear
   # "BLE",  # flake8-blind-except
@@ -183,25 +192,25 @@
   "PLR0915",
 ]
 unfixable = [
   # Don't touch unused imports
   "F401",
 ]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["ted2zim"]
 
-[tool.ruff.flake8-bugbear]
+[tool.ruff.lint.flake8-bugbear]
 # add exceptions to B008 for fastapi.
 extend-immutable-calls = ["fastapi.Depends", "fastapi.Query"]
 
-[tool.ruff.flake8-tidy-imports]
+[tool.ruff.lint.flake8-tidy-imports]
 ban-relative-imports = "all"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 
 [tool.pytest.ini_options]
 minversion = "7.3"
 testpaths = ["tests"]
 pythonpath = [".", "src"]
@@ -219,9 +228,10 @@
 [tool.coverage.report]
 exclude_lines = ["no cov", "if __name__ == .__main__.:", "if TYPE_CHECKING:"]
 
 [tool.pyright]
 include = ["src", "tests", "tasks.py"]
 exclude = [".env/**", ".venv/**"]
 extraPaths = ["src"]
-pythonVersion = "3.11"
+pythonVersion = "3.12"
 typeCheckingMode = "basic"
+disableBytesTypePromotions = true
```

### Comparing `ted2zim-2.1.0/PKG-INFO` & `ted2zim-3.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 Metadata-Version: 2.1
 Name: ted2zim
-Version: 2.1.0
+Version: 3.0.0
 Summary: Make ZIM file from TED Talks
-Project-URL: Homepage, https://github.com/openzim/ted
 Project-URL: Donate, https://www.kiwix.org/en/support-us/
-Author-email: Kiwix <dev@kiwix.org>
+Project-URL: Homepage, https://github.com/openzim/ted
+Author-email: openZIM <dev@openzim.org>
 License: GPL-3.0-or-later
 License-File: LICENSE
-Keywords: kiwix,offline,openzim,ted,zim
+Keywords: offline,openzim,ted,zim
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: <3.12,>=3.11
-Requires-Dist: beautifulsoup4==4.9.3
-Requires-Dist: jinja2==3.1.2
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: <3.13,>=3.12
+Requires-Dist: beautifulsoup4==4.12.3
+Requires-Dist: jinja2==3.1.3
 Requires-Dist: kiwixstorage==0.8.3
 Requires-Dist: pif==0.8.2
-Requires-Dist: python-dateutil==2.8.2
-Requires-Dist: python-slugify==8.0.1
+Requires-Dist: python-dateutil==2.9.0.post0
+Requires-Dist: python-slugify==8.0.4
 Requires-Dist: requests==2.31.0
-Requires-Dist: zimscraperlib==2.1.0
+Requires-Dist: yt-dlp
+Requires-Dist: zimscraperlib==3.3.2
 Provides-Extra: check
-Requires-Dist: pyright==1.1.341; extra == 'check'
+Requires-Dist: pyright==1.1.359; extra == 'check'
 Provides-Extra: dev
-Requires-Dist: debugpy==1.8.0; extra == 'dev'
-Requires-Dist: hatchling==1.18.0; extra == 'dev'
-Requires-Dist: pre-commit==3.6.0; extra == 'dev'
+Requires-Dist: debugpy==1.8.1; extra == 'dev'
+Requires-Dist: pre-commit==3.7.0; extra == 'dev'
 Requires-Dist: ted2zim[check]; extra == 'dev'
 Requires-Dist: ted2zim[lint]; extra == 'dev'
 Requires-Dist: ted2zim[scripts]; extra == 'dev'
 Requires-Dist: ted2zim[test]; extra == 'dev'
 Provides-Extra: lint
-Requires-Dist: black==23.12.0; extra == 'lint'
-Requires-Dist: ruff==0.1.8; extra == 'lint'
+Requires-Dist: black==24.4.0; extra == 'lint'
+Requires-Dist: ruff==0.4.0; extra == 'lint'
 Provides-Extra: scripts
 Requires-Dist: invoke==2.2.0; extra == 'scripts'
 Provides-Extra: test
-Requires-Dist: coverage==7.3.3; extra == 'test'
-Requires-Dist: pytest==7.4.3; extra == 'test'
+Requires-Dist: coverage==7.4.4; extra == 'test'
+Requires-Dist: pytest==8.1.1; extra == 'test'
 Description-Content-Type: text/markdown
 
 # ted2zim
 
 ##### Get the best :bulb: TED videos offline :arrow_down:
 An offliner to create ZIM :package: files from TED talks
 
@@ -51,22 +51,25 @@
 [![PyPI version shields.io](https://img.shields.io/pypi/v/ted2zim.svg)](https://pypi.org/project/ted2zim/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ted2zim.svg)](https://pypi.org/project/ted2zim)
 
 TED (Technology, Entertainment, Design) is a global set of conferences under the slogan "ideas worth spreading". They address a wide range of topics within the research and practice of science and culture, often through storytelling. The speakers are given a maximum of 18 minutes to present their ideas in the most innovative and engaging ways they can. One can eaisly find all the TED videos [here](https://ted.com/talks).
 
 This project is aimed at creating a sustainable solution to make TED accessible offline by creating ZIM files providing these videos in a similar manner like online.
 
+`ted2zim` adheres to openZIM's [Contribution Guidelines](https://github.com/openzim/overview/wiki/Contributing).
+
+`ted2zim` has implemented openZIM's [Python bootstrap, conventions and policies](https://github.com/openzim/_python-bootstrap/docs/Policy.md) **v1.0.1**.
 
 ## Getting started :rocket:
 
 #### Install the dependencies
 Make sure that you have `python3`, `unzip`, `ffmpeg`, `wget` and `curl` installed on your system before running the scraper (otherwise you'll get a warning to install them).
 
 #### Setup the package
-One can easily install the PyPI version but let's setup the source version. 
+One can easily install the PyPI version but let's setup the source version.
 
 First, clone this repository.
 
 If you do not already have it on your system, install hatch to build the software and manage virtual environments (you might be interested by our detailed [Developer Setup](https://github.com/openzim/_python-bootstrap/wiki/Developer-Setup) as well).
 
 ```bash
 pip3 install hatch
```

