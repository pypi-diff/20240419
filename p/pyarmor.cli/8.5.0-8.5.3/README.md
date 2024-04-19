# Comparing `tmp/pyarmor.cli-8.5.0-py3-none-any.whl.zip` & `tmp/pyarmor.cli-8.5.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,27 +1,28 @@
-Zip file size: 451125 bytes, number of entries: 25
--rw-r--r--  2.0 unx     1153 b- defN 24-Jan-26 23:50 pyarmor/cli/__init__.py
--rw-r--r--  2.0 unx    26397 b- defN 24-Feb-03 02:51 pyarmor/cli/__main__.py
+Zip file size: 452703 bytes, number of entries: 26
+-rw-r--r--  2.0 unx     1153 b- defN 24-Mar-29 02:25 pyarmor/cli/__init__.py
+-rw-r--r--  2.0 unx    25363 b- defN 24-Apr-13 01:17 pyarmor/cli/__main__.py
 -rw-r--r--  2.0 unx     7189 b- defN 23-Jul-31 09:19 pyarmor/cli/bootstrap.py
+-rw-r--r--  2.0 unx     4073 b- defN 24-Mar-12 23:11 pyarmor/cli/bug.py
 -rw-r--r--  2.0 unx    10726 b- defN 23-May-31 00:18 pyarmor/cli/config.py
--rw-r--r--  2.0 unx    21209 b- defN 24-Jan-26 23:03 pyarmor/cli/context.py
--rw-r--r--  2.0 unx   206158 b- defN 24-Feb-23 01:09 pyarmor/cli/core.data.1
--rw-r--r--  2.0 unx   134208 b- defN 24-Feb-23 01:09 pyarmor/cli/core.data.2
--rw-r--r--  2.0 unx    58049 b- defN 24-Feb-23 01:09 pyarmor/cli/core.data.3
--rw-r--r--  2.0 unx    10202 b- defN 24-Feb-02 01:50 pyarmor/cli/default.cfg
+-rw-r--r--  2.0 unx    21794 b- defN 24-Apr-19 08:21 pyarmor/cli/context.py
+-rw-r--r--  2.0 unx   206158 b- defN 24-Apr-13 02:13 pyarmor/cli/core.data.1
+-rw-r--r--  2.0 unx   134208 b- defN 24-Apr-13 02:13 pyarmor/cli/core.data.2
+-rw-r--r--  2.0 unx    58049 b- defN 24-Apr-13 02:13 pyarmor/cli/core.data.3
+-rw-r--r--  2.0 unx    10699 b- defN 24-Apr-13 02:14 pyarmor/cli/default.cfg
 -rw-r--r--  2.0 unx     6383 b- defN 23-Dec-15 01:31 pyarmor/cli/docker.py
 -rw-r--r--  2.0 unx     6195 b- defN 24-Jan-26 09:18 pyarmor/cli/generate.py
 -rw-r--r--  2.0 unx     2167 b- defN 24-Feb-22 23:04 pyarmor/cli/hdinfo.py
 -rw-r--r--  2.0 unx     7282 b- defN 23-Oct-26 01:05 pyarmor/cli/merge.py
 -rw-r--r--  2.0 unx     3956 b- defN 23-Apr-20 07:02 pyarmor/cli/mixer.py
 -rw-r--r--  2.0 unx    10877 b- defN 24-Jan-26 09:14 pyarmor/cli/plugin.py
 -rw-r--r--  2.0 unx     2487 b- defN 23-Mar-25 22:51 pyarmor/cli/public_capsule.zip
 -rw-r--r--  2.0 unx    22885 b- defN 23-Dec-30 08:29 pyarmor/cli/register.py
 -rw-r--r--  2.0 unx    16911 b- defN 23-Oct-07 23:37 pyarmor/cli/repack.py
 -rw-r--r--  2.0 unx     8283 b- defN 23-Dec-05 02:26 pyarmor/cli/resource.py
 -rw-r--r--  2.0 unx     2193 b- defN 23-Feb-22 14:43 pyarmor/cli/shell.py
--rw-r--r--  2.0 unx     2398 b- defN 24-Feb-29 02:11 pyarmor.cli-8.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-29 02:11 pyarmor.cli-8.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       94 b- defN 24-Feb-29 02:11 pyarmor.cli-8.5.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 24-Feb-29 02:11 pyarmor.cli-8.5.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2012 b- defN 24-Feb-29 02:11 pyarmor.cli-8.5.0.dist-info/RECORD
-25 files, 569514 bytes uncompressed, 447931 bytes compressed:  21.3%
+-rw-r--r--  2.0 unx     2398 b- defN 24-Apr-19 11:23 pyarmor.cli-8.5.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-19 11:23 pyarmor.cli-8.5.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       94 b- defN 24-Apr-19 11:23 pyarmor.cli-8.5.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-19 11:23 pyarmor.cli-8.5.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2087 b- defN 24-Apr-19 11:23 pyarmor.cli-8.5.3.dist-info/RECORD
+26 files, 573710 bytes uncompressed, 449397 bytes compressed:  21.7%
```

## zipnote {}

```diff
@@ -3,14 +3,17 @@
 
 Filename: pyarmor/cli/__main__.py
 Comment: 
 
 Filename: pyarmor/cli/bootstrap.py
 Comment: 
 
+Filename: pyarmor/cli/bug.py
+Comment: 
+
 Filename: pyarmor/cli/config.py
 Comment: 
 
 Filename: pyarmor/cli/context.py
 Comment: 
 
 Filename: pyarmor/cli/core.data.1
@@ -54,23 +57,23 @@
 
 Filename: pyarmor/cli/resource.py
 Comment: 
 
 Filename: pyarmor/cli/shell.py
 Comment: 
 
-Filename: pyarmor.cli-8.5.0.dist-info/METADATA
+Filename: pyarmor.cli-8.5.3.dist-info/METADATA
 Comment: 
 
-Filename: pyarmor.cli-8.5.0.dist-info/WHEEL
+Filename: pyarmor.cli-8.5.3.dist-info/WHEEL
 Comment: 
 
-Filename: pyarmor.cli-8.5.0.dist-info/entry_points.txt
+Filename: pyarmor.cli-8.5.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: pyarmor.cli-8.5.0.dist-info/top_level.txt
+Filename: pyarmor.cli-8.5.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pyarmor.cli-8.5.0.dist-info/RECORD
+Filename: pyarmor.cli-8.5.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyarmor/cli/__init__.py

```diff
@@ -1,10 +1,10 @@
 import logging
 
-__VERSION__ = '8.5.0'
+__VERSION__ = '8.5.3'
 
 logger = logging.getLogger('cli')
 
 
 class CliError(Exception):
     pass
```

## pyarmor/cli/__main__.py

```diff
@@ -28,14 +28,15 @@
 from .context import Context
 from .register import Register, WebRegister
 from .config import Configer
 from .shell import PyarmorShell
 from .plugin import Plugin
 from .generate import Builder
 from .bootstrap import check_prebuilt_runtime_library
+from .bug import find_solutions
 
 
 def _cmd_gen_key(builder, options):
     n = len(options['inputs'])
     if n > 1:
         logger.error('please check online documentation to learn')
         logger.error('how to use command "pyarmor gen key"')
@@ -102,14 +103,18 @@
     if args.inputs:
         options['inputs'] = [os.path.normpath(x) for x in args.inputs]
 
     if args.use_runtime:
         options['no_runtime'] = True
         options['use_runtime'] = args.use_runtime
 
+    if (options.get('restrict_module', 0) == 2
+        and ctx.cfg['builder'].get('private_module_as_restrict', 0)):
+        options['restrict_module'] = 3
+
     if options.get('assert_call') or options.get('assert_import'):
         if options.get('restrict_module', 0) < 2:
             logger.debug('implicitly set restrict_module = 2')
             options['restrict_module'] = 2
 
     if args.enables:
         for x in args.enables:
@@ -323,15 +328,15 @@
             regsvr.upgrade_to_pro(regfile, args.product)
         else:
             group = info['lictype'] == 'GROUP'
             regsvr.register(regfile, args.product, group=group)
 
 
 def cmd_man(ctx, args):
-    pkgpath = os.path.normpath(os.path.dirname(__file__), '..', 'man')
+    pkgpath = os.path.join(os.path.dirname(__file__), '..', 'man')
     if not os.path.exists(pkgpath):
         from subprocess import check_output
         check_output([
             sys.executable, '-m', 'pip', 'install',
             '--disable-pip-version-check', 'pyarmor.man'
         ])
 
@@ -742,44 +747,14 @@
 
     if hasattr(args, 'func'):
         return args.func(ctx, args)
     else:
         parser.print_help()
 
 
-def find_solutions(e):
-    '''Print quick solutions according to exception
-
-    If not enable debug, tell user try `pyarmor -d cmd...`
-
-    If it raises CliError, print possible solutions
-
-    For unknown error, print FAQ page link and `pyarmor man`
-
-    Pyarmor Man is designed to help Pyarmor users to learn
-    and use Pyarmor by web-ui, to find solution quickly when
-    something is wrong, to report bugs and ask questions in
-    standard form in order to save both Pyarmor team's and
-    Pyarmor users' time.
-    '''
-    # debug = logging.getLogger().getEffectiveLevel()
-    # clierr = isinstance(e, CliError)
-    logger.error('''somthing is wrong
-*===========================================================*
-*  Please check                                             *
-*    https://pyarmor.readthedocs.io/en/latest/questions.html*
-*  or run `pyarmor man` to find solutions quickly           *
-*                                                           *
-*  It's recommand to report issue by `pyarmor man` in order *
-*  to provide necessary information, and avoid dupcliated   *
-*  issues or unclear question.                              *
-*===========================================================*
-''')
-
-
 def main():
     logging.basicConfig(
         level=logging.INFO,
         format='%(levelname)-8s %(message)s',
     )
 
     try:
```

## pyarmor/cli/context.py

```diff
@@ -54,15 +54,15 @@
                 elif cname == 'libc':
                     plat = 'android'
         return plat
 
     def format_machine():
         mach = platform.machine().lower()
         arch_table = (
-            ('x86', ('i386', 'i486', 'i586', 'i686')),
+            ('x86', ('i386', 'i486', 'i586', 'i686', 'x86')),
             ('x86_64', ('x64', 'x86_64', 'amd64', 'intel')),
             ('arm', ('armv5',)),
             ('armv6', ('armv6l',)),
             ('armv7', ('armv7l',)),
             ('aarch32', ('aarch32',)),
             ('aarch64', ('aarch64', 'arm64'))
         )
@@ -100,15 +100,15 @@
         ('windows', ('windows', 'cygwin*')),
         ('darwin', ('darwin',)),
         ('linux', ('linux*',)),
         ('freebsd', ('freebsd*', 'openbsd*', 'isilon onefs')),
     )
 
     arch_table = (
-        ('x86', ('i?86', )),
+        ('x86', ('i?86', 'x86')),
         ('x86_64', ('x64', 'x86_64', 'amd64', 'intel')),
         ('arm', ('armv5',)),
         ('armv6', ('armv6l',)),
         ('armv7', ('armv7l',)),
         ('aarch32', ('aarch32',)),
         ('aarch64', ('aarch64', 'arm64'))
     )
@@ -697,7 +697,23 @@
             host = http_proxy[i:]
             port = b'80'
         else:
             host = http_proxy[i:j]
             port = http_proxy[j+1:]
         url = b'http://pyarmor.dashingsoft.com'
         return b'\x00'.join([host, port, url, header, b'\x00'])
+
+    def request_token(self, url, timeout=6.0):
+        from urllib.request import urlopen
+
+        def get_response(host):
+            try:
+                from ssl import _create_unverified_context
+                context = _create_unverified_context()
+                req = 'https://%s%s' % (host, url)
+            except Exception:
+                context = None
+                req = 'http://%s%s' % (host, url)
+            return urlopen(req, None, timeout, context=context)
+
+        with get_response('pyarmor.dashingsoft.com') as res:
+            return res.read()
```

## pyarmor/cli/default.cfg

```diff
@@ -1,16 +1,16 @@
 [pyarmor]
 
 ;; Pyarmor version
 major = 8
 minor = 5
-patch = 0
+patch = 3
 
 ;; Compatible core version
-cli.core = 6.5.0
+cli.core = 6.5.1
 
 ;; Deprecated since Pyarmor 8.2.5
 ; cli.runtime = 3.2.5
 
 ;; Default timeout when send request to remote server for
 ;;     check Pyarmor license
 ;;     register Pyarmor license
@@ -188,14 +188,31 @@
 
 ;; Model level to exclude names
 ; rft_excludes =
 
 ;; Whether encrypt name in statement import
 rft_mix_import_name = 0
 
+;;
+;; Compatiable options
+;;
+
+;; Since pyarmor 8.5.3, pyarmor.core 6.5.1
+;;
+;; If private_module_same_as_restrict is set to 1, --private is same as --restrict, it's default behaviours in previous version. Both --private and --restrict don't allow plain scripts to import the obfsucated modules
+;;
+;; But the right way should be
+;;
+;;    --private allow
+;;    --restrict not allow
+;;
+;; When need this behaviours, set private_module_same_as_restrict is to 0
+;;
+private_module_same_as_restrict = 0
+
 [runtime]
 
 ;; Generate extension for all Python3.7+
 universal = 0
 
 ;; Default runtime package name
 package_name_format = pyarmor_runtime_{suffix}
```

## Comparing `pyarmor.cli-8.5.0.dist-info/METADATA` & `pyarmor.cli-8.5.3.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarmor.cli
-Version: 8.5.0
+Version: 8.5.3
 Summary: A comand line tool to obfuscate python scripts
 Home-page: https://github.com/dashingsoft/pyarmor
 Author: Jondy Zhao
 Author-email: pyarmor@163.com
 License: Free To Use But Restricted
 Keywords: protect obfuscate encrypt obfuscation distribute
 Platform: UNKNOWN
@@ -14,15 +14,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Utilities
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Software Distribution
-Requires-Dist: pyarmor.cli.core (~=6.5.0)
+Requires-Dist: pyarmor.cli.core (~=6.5.1)
 
 Protect Python Scripts By Pyarmor
 =================================
 
 Pyarmor is a command line tool used to obfuscate python scripts, bind obfuscated scripts to fixed machine or expire obfuscated scripts.
 
 Key Features
```

## Comparing `pyarmor.cli-8.5.0.dist-info/RECORD` & `pyarmor.cli-8.5.3.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-pyarmor/cli/__init__.py,sha256=wkyHBwse5rmb6SBrm-KWTd-hFzoVNs9qih-7kmibHwo,1153
-pyarmor/cli/__main__.py,sha256=c_LSWQ-gsnAInJjslWgy3IWZk7waL4S8lZM7IQHGHEI,26397
+pyarmor/cli/__init__.py,sha256=QulKC79u_hW3a_amuDqfs_ZeYBk7vDurz_T6ZW4Mo0A,1153
+pyarmor/cli/__main__.py,sha256=PzCKMiUrCUHrjG594aga4pizTfe7TL7o-HLVFl2JUaw,25363
 pyarmor/cli/bootstrap.py,sha256=yQIfXrNHUNX5M_I1bas0IOgKtBIBcKReaFyNGkbZ6UY,7189
+pyarmor/cli/bug.py,sha256=mM-3K7NQ3hfsqWMZhPMphQmyuSwBdQXuppGJEna3tVU,4073
 pyarmor/cli/config.py,sha256=wma83BdjuUlSTf-_VnPfu3Qi6lEA-TyUyDKBXALtOwQ,10726
-pyarmor/cli/context.py,sha256=lu-NBsjUayM87CrGKTm_T_Cf_ss1EsXaiX1v_8Evhg4,21209
+pyarmor/cli/context.py,sha256=y5-3DTa-g-_-ZxF5fDt5QLZGceNMgwDC9v1tNZ2BsTg,21794
 pyarmor/cli/core.data.1,sha256=PbHMmRO_8rsnjWobICfSWoO_q7VuDE83R0fnYuMWZOA,206158
 pyarmor/cli/core.data.2,sha256=5XMV9dPklosJORUWjvMEbagMjjW6HFQZeAbdF0uLyKo,134208
 pyarmor/cli/core.data.3,sha256=g91hqvwhHF4zpg6UeXn5QD5eB6XoM0ACo5oXTPT6sGk,58049
-pyarmor/cli/default.cfg,sha256=s-oxHhUkA9FP8_titHOsFYRJiezhEkeUFTR7PyFxbjk,10202
+pyarmor/cli/default.cfg,sha256=exd56jimI7gl1RUYj9AzhVPQWMnIFRps4wQ3f0fLKoo,10699
 pyarmor/cli/docker.py,sha256=hfjfeP2LAPf6KkVpldDvJlHVKvifcAR-yq2_QLV2LLQ,6383
 pyarmor/cli/generate.py,sha256=SmTvR9K_8hS6S3PcVRTZMGzzxyH9bZaX3W8WM_Y1L58,6195
 pyarmor/cli/hdinfo.py,sha256=g4F_KdM-6-dp_Qn2ehGGdoOY_UHZ0gpgRTHtSe9Pi9o,2167
 pyarmor/cli/merge.py,sha256=0QqQ8idac5OVvzw6tOtdx5qWlSdD1NzvmWeCiLkvLns,7282
 pyarmor/cli/mixer.py,sha256=i4IrXukoG5L3V3Wv5BgDSTkNU5NB03-Q4bgsWwug6LY,3956
 pyarmor/cli/plugin.py,sha256=besVlBjBjpn-Cq6KYLr9xoiqvhl40BBGN789aYI665Y,10877
 pyarmor/cli/public_capsule.zip,sha256=1r4u42ixfocGPMQc0OklpoHF3nvVW6GA1f4SwcEJWVI,2487
 pyarmor/cli/register.py,sha256=rzX6X4qHtW_AqmLKH0f4bVU1kYF4QxOgs0tCcUTp1Hg,22885
 pyarmor/cli/repack.py,sha256=uF2rqdGucbEn3R6-l2nfTYm1of8PNcrdO9tAsCUrxsA,16911
 pyarmor/cli/resource.py,sha256=LT6BfiQiZvEomgXEZhZUUdwO87KIGhtKWcdIzCZI9Lo,8283
 pyarmor/cli/shell.py,sha256=S1yJ5RQZhTIysQgXk3H4E_cJsV2Lymh-w-_GdnHFngU,2193
-pyarmor.cli-8.5.0.dist-info/METADATA,sha256=OOcxkcQYkA5dTrcPKe973R_3NVx7dToW96uJLYc228s,2398
-pyarmor.cli-8.5.0.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-pyarmor.cli-8.5.0.dist-info/entry_points.txt,sha256=rv9Gd29gFGXLyToOYw7BvYmVl6Y3g_tUXq1nRYxu0Js,94
-pyarmor.cli-8.5.0.dist-info/top_level.txt,sha256=UE1ovZ_90YzwF_lZ3LV7o8HKLe-RgzUaUUvdH5UTUus,8
-pyarmor.cli-8.5.0.dist-info/RECORD,,
+pyarmor.cli-8.5.3.dist-info/METADATA,sha256=TE3KR1e769_MqDaTUJP0J29Pk-cNU2gygFQpy4QZybs,2398
+pyarmor.cli-8.5.3.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+pyarmor.cli-8.5.3.dist-info/entry_points.txt,sha256=rv9Gd29gFGXLyToOYw7BvYmVl6Y3g_tUXq1nRYxu0Js,94
+pyarmor.cli-8.5.3.dist-info/top_level.txt,sha256=UE1ovZ_90YzwF_lZ3LV7o8HKLe-RgzUaUUvdH5UTUus,8
+pyarmor.cli-8.5.3.dist-info/RECORD,,
```

