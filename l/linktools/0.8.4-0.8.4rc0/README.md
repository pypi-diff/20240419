# Comparing `tmp/linktools-0.8.4.tar.gz` & `tmp/linktools-0.8.4rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktools-0.8.4.tar", last modified: Fri Apr 19 01:23:59 2024, max compression
+gzip compressed data, was "linktools-0.8.4rc0.tar", last modified: Tue Apr 16 08:50:18 2024, max compression
```

## Comparing `linktools-0.8.4.tar` & `linktools-0.8.4rc0.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:59.555400 linktools-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11895 2024-04-19 01:21:14.000000 linktools-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 01:21:14.000000 linktools-0.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    35044 2024-04-19 01:23:59.555400 linktools-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    32997 2024-04-19 01:21:14.000000 linktools-0.8.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-19 01:21:14.000000 linktools-0.8.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 01:23:59.555400 linktools-0.8.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     4278 2024-04-19 01:21:14.000000 linktools-0.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:59.531400 linktools-0.8.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:59.535400 linktools-0.8.4/src/linktools/
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21680 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12574 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/_environ.py
--rw-r--r--   0 runner    (1001) docker     (127)    17823 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/_url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:59.539400 linktools-0.8.4/src/linktools/android/
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/android/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23929 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/android/adb.py
--rw-r--r--   0 runner    (1001) docker     (127)    12142 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/android/struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:59.539400 linktools-0.8.4/src/linktools/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    82987 2024-04-19 01:23:50.000000 linktools-0.8.4/src/linktools/assets/android-tools.apk
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-19 01:23:50.000000 linktools-0.8.4/src/linktools/assets/android-tools.json
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/assets/chrome-driver.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:59.531400 linktools-0.8.4/src/linktools/assets/containers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:59.539400 linktools-0.8.4/src/linktools/assets/containers/100-nginx/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/assets/containers/100-nginx/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/assets/containers/100-nginx/compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/assets/containers/100-nginx/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    47272 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/assets/containers/100-nginx/dnsapi.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/assets/containers/100-nginx/http.conf
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/assets/containers/100-nginx/https.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:59.539400 linktools-0.8.4/src/linktools/assets/containers/110-portainer/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/assets/containers/110-portainer/compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/assets/containers/110-portainer/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/assets/containers/110-portainer/nginx.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:59.543400 linktools-0.8.4/src/linktools/assets/containers/120-flare/
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/assets/containers/120-flare/compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/assets/containers/120-flare/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/assets/containers/120-flare/nginx.conf
--rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/assets/fake_useragent.json
--rw-r--r--   0 runner    (1001) docker     (127)    44744 2024-04-19 01:21:24.000000 linktools-0.8.4/src/linktools/assets/frida.js
--rw-r--r--   0 runner    (1001) docker     (127)    24005 2024-04-19 01:21:24.000000 linktools-0.8.4/src/linktools/assets/frida.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:59.531400 linktools-0.8.4/src/linktools/assets/objection/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:59.543400 linktools-0.8.4/src/linktools/assets/objection/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/assets/objection/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12275 2024-04-19 01:23:59.000000 linktools-0.8.4/src/linktools/assets/tools.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:59.543400 linktools-0.8.4/src/linktools/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/cli/argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    31589 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/cli/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:59.543400 linktools-0.8.4/src/linktools/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/cli/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:59.543400 linktools-0.8.4/src/linktools/cli/commands/android/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/cli/commands/android/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2494 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/cli/commands/android/adb.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2140 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/cli/commands/android/agent.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15337 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/cli/commands/android/app.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2614 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/cli/commands/android/debug.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6205 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/cli/commands/android/frida.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/cli/commands/android/info.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4914 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/cli/commands/android/intent.py
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/cli/commands/android/objection.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15517 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/cli/commands/android/pidcat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4595 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/cli/commands/android/top.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:59.547400 linktools-0.8.4/src/linktools/cli/commands/common/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/cli/commands/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/cli/commands/common/cert.py
--rw-r--r--   0 runner    (1001) docker     (127)    15194 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/cli/commands/common/cntr.py
--rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/cli/commands/common/env.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/cli/commands/common/grep.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4134 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/cli/commands/common/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:59.547400 linktools-0.8.4/src/linktools/cli/commands/ios/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/cli/commands/ios/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5332 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/cli/commands/ios/frida.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/cli/commands/ios/ipa.py
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/cli/commands/ios/objection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/cli/commands/ios/scp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/cli/commands/ios/sib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/cli/commands/ios/ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)    17530 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/cli/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:59.547400 linktools-0.8.4/src/linktools/container/
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16189 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/container/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    21050 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/container/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/container/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:59.547400 linktools-0.8.4/src/linktools/frida/
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/frida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/frida/android.py
--rw-r--r--   0 runner    (1001) docker     (127)    29987 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/frida/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/frida/ios.py
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/frida/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/frida/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:59.551400 linktools-0.8.4/src/linktools/ida/
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/ida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/ida/ida.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:59.551400 linktools-0.8.4/src/linktools/ios/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/ios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/ios/ipa.py
--rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/ios/sib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-19 01:23:59.000000 linktools-0.8.4/src/linktools/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/reactor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:59.551400 linktools-0.8.4/src/linktools/references/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/references/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:59.551400 linktools-0.8.4/src/linktools/references/fake_useragent/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/references/fake_useragent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/references/fake_useragent/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/references/fake_useragent/fake.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/references/fake_useragent/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/references/fake_useragent/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/references/fake_useragent/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/rich.py
--rw-r--r--   0 runner    (1001) docker     (127)    13556 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:59.551400 linktools-0.8.4/src/linktools/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/utils/_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/utils/_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6557 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/utils/_subprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19460 2024-04-19 01:21:14.000000 linktools-0.8.4/src/linktools/utils/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:23:59.551400 linktools-0.8.4/src/linktools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    35044 2024-04-19 01:23:59.000000 linktools-0.8.4/src/linktools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-19 01:23:59.000000 linktools-0.8.4/src/linktools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 01:23:59.000000 linktools-0.8.4/src/linktools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-19 01:23:59.000000 linktools-0.8.4/src/linktools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-19 01:23:59.000000 linktools-0.8.4/src/linktools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-19 01:23:59.000000 linktools-0.8.4/src/linktools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.993133 linktools-0.8.4rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11895 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    35047 2024-04-16 08:50:18.993133 linktools-0.8.4rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    32997 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 08:50:18.993133 linktools-0.8.4rc0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4278 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.969134 linktools-0.8.4rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.973134 linktools-0.8.4rc0/src/linktools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21680 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12574 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/_environ.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17823 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/_url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.977134 linktools-0.8.4rc0/src/linktools/android/
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/android/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23929 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/android/adb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12142 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/android/struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.977134 linktools-0.8.4rc0/src/linktools/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    82987 2024-04-16 08:50:09.000000 linktools-0.8.4rc0/src/linktools/assets/android-tools.apk
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-16 08:50:09.000000 linktools-0.8.4rc0/src/linktools/assets/android-tools.json
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/chrome-driver.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.969134 linktools-0.8.4rc0/src/linktools/assets/containers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.977134 linktools-0.8.4rc0/src/linktools/assets/containers/100-nginx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/100-nginx/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/100-nginx/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/100-nginx/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47272 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/100-nginx/dnsapi.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/100-nginx/http.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/100-nginx/https.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.977134 linktools-0.8.4rc0/src/linktools/assets/containers/110-portainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/110-portainer/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/110-portainer/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/110-portainer/nginx.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.981134 linktools-0.8.4rc0/src/linktools/assets/containers/120-flare/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/120-flare/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/120-flare/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/120-flare/nginx.conf
+-rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/fake_useragent.json
+-rw-r--r--   0 runner    (1001) docker     (127)    44744 2024-04-16 08:48:13.000000 linktools-0.8.4rc0/src/linktools/assets/frida.js
+-rw-r--r--   0 runner    (1001) docker     (127)    24005 2024-04-16 08:48:13.000000 linktools-0.8.4rc0/src/linktools/assets/frida.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.969134 linktools-0.8.4rc0/src/linktools/assets/objection/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.981134 linktools-0.8.4rc0/src/linktools/assets/objection/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/objection/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12275 2024-04-16 08:50:18.000000 linktools-0.8.4rc0/src/linktools/assets/tools.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.981134 linktools-0.8.4rc0/src/linktools/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31589 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.981134 linktools-0.8.4rc0/src/linktools/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.981134 linktools-0.8.4rc0/src/linktools/cli/commands/android/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/android/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2494 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/android/adb.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2140 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/android/agent.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15337 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/android/app.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2614 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/android/debug.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6205 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/android/frida.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/android/info.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4914 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/android/intent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/android/objection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15517 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/android/pidcat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4595 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/android/top.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.981134 linktools-0.8.4rc0/src/linktools/cli/commands/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/common/cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15194 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/common/cntr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/common/env.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/common/grep.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4134 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/common/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.985134 linktools-0.8.4rc0/src/linktools/cli/commands/ios/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/ios/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5332 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/ios/frida.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/ios/ipa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/ios/objection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/ios/scp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/ios/sib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/ios/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17530 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.985134 linktools-0.8.4rc0/src/linktools/container/
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16189 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/container/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21050 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/container/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/container/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.985134 linktools-0.8.4rc0/src/linktools/frida/
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/frida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/frida/android.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29987 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/frida/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/frida/ios.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/frida/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/frida/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.985134 linktools-0.8.4rc0/src/linktools/ida/
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/ida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/ida/ida.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.985134 linktools-0.8.4rc0/src/linktools/ios/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/ios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/ios/ipa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/ios/sib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-16 08:50:18.000000 linktools-0.8.4rc0/src/linktools/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/reactor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.985134 linktools-0.8.4rc0/src/linktools/references/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/references/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.989133 linktools-0.8.4rc0/src/linktools/references/fake_useragent/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/references/fake_useragent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/references/fake_useragent/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/references/fake_useragent/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/references/fake_useragent/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/references/fake_useragent/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/references/fake_useragent/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/rich.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13556 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.989133 linktools-0.8.4rc0/src/linktools/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/utils/_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/utils/_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6557 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/utils/_subprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19460 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/utils/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.989133 linktools-0.8.4rc0/src/linktools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    35047 2024-04-16 08:50:18.000000 linktools-0.8.4rc0/src/linktools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-16 08:50:18.000000 linktools-0.8.4rc0/src/linktools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:50:18.000000 linktools-0.8.4rc0/src/linktools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-16 08:50:18.000000 linktools-0.8.4rc0/src/linktools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-16 08:50:18.000000 linktools-0.8.4rc0/src/linktools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 08:50:18.000000 linktools-0.8.4rc0/src/linktools.egg-info/top_level.txt
```

### Comparing `linktools-0.8.4/LICENSE` & `linktools-0.8.4rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/PKG-INFO` & `linktools-0.8.4rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linktools
-Version: 0.8.4
+Version: 0.8.4rc0
 Summary: linktools toolkit
 Author-email: Hu Ji <669898595@qq.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/ice-black-tea/linktools
 Project-URL: Repository, https://github.com/ice-black-tea/linktools.git
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `linktools-0.8.4/README.md` & `linktools-0.8.4rc0/README.md`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/pyproject.toml` & `linktools-0.8.4rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/setup.py` & `linktools-0.8.4rc0/setup.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/__init__.py` & `linktools-0.8.4rc0/src/linktools/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/__main__.py` & `linktools-0.8.4rc0/src/linktools/__main__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/_config.py` & `linktools-0.8.4rc0/src/linktools/_config.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/_environ.py` & `linktools-0.8.4rc0/src/linktools/_environ.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/_tools.py` & `linktools-0.8.4rc0/src/linktools/_tools.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/_url.py` & `linktools-0.8.4rc0/src/linktools/_url.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/android/__init__.py` & `linktools-0.8.4rc0/src/linktools/android/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/android/adb.py` & `linktools-0.8.4rc0/src/linktools/android/adb.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/android/struct.py` & `linktools-0.8.4rc0/src/linktools/android/struct.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/assets/android-tools.json` & `linktools-0.8.4rc0/src/linktools/assets/android-tools.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'ANDROID_TOOL_BRIDGE_APK'": "{'md5': '3097e19b66070036181860877768b952', 'time': '2024-04-16 "*

 * *                              "16:50:09'}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "ANDROID_TOOL_BRIDGE_APK": {
         "main": "android.tools.Main",
-        "md5": "c419cb85594b69ee31bae8730718c425",
+        "md5": "3097e19b66070036181860877768b952",
         "name": "android-tools.apk",
         "size": 82987,
-        "time": "2024-04-19 09:23:50"
+        "time": "2024-04-16 16:50:09"
     },
     "ANDROID_TOOL_FRIDA_SERVER": [
         {
             "min_version": "15.1.8",
             "name": "strong-frida-server-{version}-android-{abi}",
             "url": "https://github.com/hzzheyang/strongR-frida-android/releases/download/{version}/hluda-server-{version}-android-{abi}.xz"
         },
```

### Comparing `linktools-0.8.4/src/linktools/assets/chrome-driver.json` & `linktools-0.8.4rc0/src/linktools/assets/chrome-driver.json`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/assets/containers/100-nginx/Dockerfile` & `linktools-0.8.4rc0/src/linktools/assets/containers/100-nginx/Dockerfile`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/assets/containers/100-nginx/container.py` & `linktools-0.8.4rc0/src/linktools/assets/containers/100-nginx/container.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/assets/containers/100-nginx/dnsapi.txt` & `linktools-0.8.4rc0/src/linktools/assets/containers/100-nginx/dnsapi.txt`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/assets/containers/110-portainer/container.py` & `linktools-0.8.4rc0/src/linktools/assets/containers/110-portainer/container.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/assets/containers/120-flare/compose.yml` & `linktools-0.8.4rc0/src/linktools/assets/containers/120-flare/compose.yml`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/assets/containers/120-flare/container.py` & `linktools-0.8.4rc0/src/linktools/assets/containers/120-flare/container.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/assets/containers/120-flare/nginx.conf` & `linktools-0.8.4rc0/src/linktools/assets/containers/120-flare/nginx.conf`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/assets/fake_useragent.json` & `linktools-0.8.4rc0/src/linktools/assets/fake_useragent.json`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/assets/frida.js` & `linktools-0.8.4rc0/src/linktools/assets/frida.js`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/assets/frida.min.js` & `linktools-0.8.4rc0/src/linktools/assets/frida.min.js`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/assets/objection/plugins/__init__.py` & `linktools-0.8.4rc0/src/linktools/assets/objection/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/assets/tools.json` & `linktools-0.8.4rc0/src/linktools/assets/tools.json`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/cli/__init__.py` & `linktools-0.8.4rc0/src/linktools/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/cli/argparse.py` & `linktools-0.8.4rc0/src/linktools/cli/argparse.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/cli/command.py` & `linktools-0.8.4rc0/src/linktools/cli/command.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/cli/commands/android/adb.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/android/adb.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/cli/commands/android/agent.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/android/agent.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/cli/commands/android/app.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/android/app.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/cli/commands/android/debug.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/android/debug.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/cli/commands/android/frida.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/android/frida.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/cli/commands/android/info.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/android/info.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/cli/commands/android/intent.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/android/intent.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/cli/commands/android/objection.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/android/objection.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/cli/commands/android/pidcat.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/android/pidcat.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/cli/commands/android/top.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/android/top.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/cli/commands/common/cert.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/common/cert.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/cli/commands/common/cntr.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/common/cntr.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/cli/commands/common/env.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/common/env.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/cli/commands/common/grep.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/common/grep.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/cli/commands/common/tools.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/common/tools.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/cli/commands/ios/frida.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/ios/frida.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/cli/commands/ios/ipa.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/ios/ipa.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/cli/commands/ios/objection.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/ios/objection.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/cli/commands/ios/scp.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/ios/scp.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/cli/commands/ios/sib.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/ios/sib.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/cli/commands/ios/ssh.py` & `linktools-0.8.4rc0/src/linktools/cli/commands/ios/ssh.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/cli/device.py` & `linktools-0.8.4rc0/src/linktools/cli/device.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/container/__init__.py` & `linktools-0.8.4rc0/src/linktools/container/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/container/container.py` & `linktools-0.8.4rc0/src/linktools/container/container.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/container/manager.py` & `linktools-0.8.4rc0/src/linktools/container/manager.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/container/repository.py` & `linktools-0.8.4rc0/src/linktools/container/repository.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/decorator.py` & `linktools-0.8.4rc0/src/linktools/decorator.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/device.py` & `linktools-0.8.4rc0/src/linktools/device.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/frida/__init__.py` & `linktools-0.8.4rc0/src/linktools/frida/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/frida/android.py` & `linktools-0.8.4rc0/src/linktools/frida/android.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/frida/app.py` & `linktools-0.8.4rc0/src/linktools/frida/app.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/frida/ios.py` & `linktools-0.8.4rc0/src/linktools/frida/ios.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/frida/script.py` & `linktools-0.8.4rc0/src/linktools/frida/script.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/frida/server.py` & `linktools-0.8.4rc0/src/linktools/frida/server.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/ida/__init__.py` & `linktools-0.8.4rc0/src/linktools/ida/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/ida/ida.py` & `linktools-0.8.4rc0/src/linktools/ida/ida.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/ios/ipa.py` & `linktools-0.8.4rc0/src/linktools/ios/ipa.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/ios/sib.py` & `linktools-0.8.4rc0/src/linktools/ios/sib.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/metadata.py` & `linktools-0.8.4rc0/src/linktools/metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 class __MissingType:
     __eq__ = lambda l, r: \
         l is r or type(l) is type(r)
 
 
 __name__ = "linktools"
 __release__ = True
-__version__ = "0.8.4"
+__version__ = "0.8.4rc0"
 __missing__ = __MissingType()
 __description__ = f"""\
     ___       __   __              __
    / (_)___  / /__/ /_____  ____  / /____
-  / / / __ \\/ //_/ __/ __ \\/ __ \\/ / ___/  linktools toolkit (v0.8.4)
+  / / / __ \\/ //_/ __/ __ \\/ __ \\/ / ___/  linktools toolkit (v0.8.4rc0)
  / / / / / / ,< / /_/ /_/ / /_/ / (__  )   by: Hu Ji <669898595@qq.com>
 /_/_/_/ /_/_/|_|\\__/\\____/\\____/_/____/
 """
```

### Comparing `linktools-0.8.4/src/linktools/reactor.py` & `linktools-0.8.4rc0/src/linktools/reactor.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/references/fake_useragent/fake.py` & `linktools-0.8.4rc0/src/linktools/references/fake_useragent/fake.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/references/fake_useragent/utils.py` & `linktools-0.8.4rc0/src/linktools/references/fake_useragent/utils.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/rich.py` & `linktools-0.8.4rc0/src/linktools/rich.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/ssh.py` & `linktools-0.8.4rc0/src/linktools/ssh.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/utils/__init__.py` & `linktools-0.8.4rc0/src/linktools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/utils/_port.py` & `linktools-0.8.4rc0/src/linktools/utils/_port.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/utils/_proxy.py` & `linktools-0.8.4rc0/src/linktools/utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/utils/_subprocess.py` & `linktools-0.8.4rc0/src/linktools/utils/_subprocess.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools/utils/_utils.py` & `linktools-0.8.4rc0/src/linktools/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools.egg-info/PKG-INFO` & `linktools-0.8.4rc0/src/linktools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linktools
-Version: 0.8.4
+Version: 0.8.4rc0
 Summary: linktools toolkit
 Author-email: Hu Ji <669898595@qq.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/ice-black-tea/linktools
 Project-URL: Repository, https://github.com/ice-black-tea/linktools.git
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `linktools-0.8.4/src/linktools.egg-info/SOURCES.txt` & `linktools-0.8.4rc0/src/linktools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools.egg-info/entry_points.txt` & `linktools-0.8.4rc0/src/linktools.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4/src/linktools.egg-info/requires.txt` & `linktools-0.8.4rc0/src/linktools.egg-info/requires.txt`

 * *Files identical despite different names*

