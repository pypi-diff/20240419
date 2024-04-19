# Comparing `tmp/batou-2.4rc2.tar.gz` & `tmp/batou-2.5.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batou-2.4rc2.tar", last modified: Wed Nov 29 10:06:25 2023, max compression
+gzip compressed data, was "batou-2.5.0b1.tar", last modified: Fri Apr 19 05:17:23 2024, max compression
```

## Comparing `batou-2.4rc2.tar` & `batou-2.5.0b1.tar`

### file list

```diff
@@ -1,264 +1,268 @@
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.674394 batou-2.4rc2/
--rw-r--r--   0 ctheune    (501) staff       (20)    31241 2023-11-29 10:06:22.000000 batou-2.4rc2/CHANGES.history.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     1608 2023-11-29 10:06:22.000000 batou-2.4rc2/LICENSE.txt
--rw-r--r--   0 ctheune    (501) staff       (20)      212 2023-11-29 10:06:22.000000 batou-2.4rc2/MANIFEST.in
--rw-r--r--   0 ctheune    (501) staff       (20)     3446 2023-11-29 10:06:25.674625 batou-2.4rc2/PKG-INFO
--rw-r--r--   0 ctheune    (501) staff       (20)     2636 2023-11-29 10:06:22.000000 batou-2.4rc2/README.md
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.527175 batou-2.4rc2/doc/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.567322 batou-2.4rc2/doc/source/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.569491 batou-2.4rc2/doc/source/api/
--rw-r--r--   0 ctheune    (501) staff       (20)      886 2023-11-29 10:06:22.000000 batou-2.4rc2/doc/source/api/component.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     2299 2023-11-29 10:06:22.000000 batou-2.4rc2/doc/source/api/environment.txt
--rw-r--r--   0 ctheune    (501) staff       (20)       48 2023-11-29 10:06:22.000000 batou-2.4rc2/doc/source/api/templates.txt
--rw-r--r--   0 ctheune    (501) staff       (20)       63 2023-11-29 10:06:22.000000 batou-2.4rc2/doc/source/api/utilities.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.569952 batou-2.4rc2/doc/source/cli/
--rw-r--r--   0 ctheune    (501) staff       (20)     4211 2023-11-29 10:06:22.000000 batou-2.4rc2/doc/source/cli/index.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.572791 batou-2.4rc2/doc/source/components/
--rw-r--r--   0 ctheune    (501) staff       (20)     1025 2023-11-29 10:06:22.000000 batou-2.4rc2/doc/source/components/cmmi.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     2941 2023-11-29 10:06:22.000000 batou-2.4rc2/doc/source/components/downloads-vcs.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     5657 2023-11-29 10:06:22.000000 batou-2.4rc2/doc/source/components/files.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     4820 2023-11-29 10:06:22.000000 batou-2.4rc2/doc/source/components/python.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     3050 2023-11-29 10:06:22.000000 batou-2.4rc2/doc/source/components/services.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.574941 batou-2.4rc2/doc/source/dev/
--rw-r--r--   0 ctheune    (501) staff       (20)      718 2023-11-29 10:06:22.000000 batou-2.4rc2/doc/source/dev/authors.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     8555 2023-11-29 10:06:22.000000 batou-2.4rc2/doc/source/dev/contributing.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     1711 2023-11-29 10:06:22.000000 batou-2.4rc2/doc/source/dev/testing.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     2809 2023-11-29 10:06:22.000000 batou-2.4rc2/doc/source/dev/todo.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     8498 2023-11-29 10:06:22.000000 batou-2.4rc2/doc/source/index.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     4799 2023-11-29 10:06:22.000000 batou-2.4rc2/doc/source/upgrading.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.579595 batou-2.4rc2/doc/source/user/
--rw-r--r--   0 ctheune    (501) staff       (20)    10870 2023-11-29 10:06:22.000000 batou-2.4rc2/doc/source/user/advanced.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     2565 2023-11-29 10:06:22.000000 batou-2.4rc2/doc/source/user/install.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     3848 2023-11-29 10:06:22.000000 batou-2.4rc2/doc/source/user/installation-deb.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     3798 2023-11-29 10:06:22.000000 batou-2.4rc2/doc/source/user/installation-rpm.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     2907 2023-11-29 10:06:22.000000 batou-2.4rc2/doc/source/user/intro.txt
--rw-r--r--   0 ctheune    (501) staff       (20)    47505 2023-11-29 10:06:22.000000 batou-2.4rc2/doc/source/user/quickstart.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.536791 batou-2.4rc2/examples/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.580546 batou-2.4rc2/examples/api/
--rw-r--r--   0 ctheune    (501) staff       (20)      349 2023-11-29 10:06:22.000000 batou-2.4rc2/examples/api/index.txt
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2023-11-29 10:06:22.000000 batou-2.4rc2/examples/api/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.580907 batou-2.4rc2/examples/django/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2023-11-29 10:06:22.000000 batou-2.4rc2/examples/django/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.581499 batou-2.4rc2/examples/durations/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2023-11-29 10:06:22.000000 batou-2.4rc2/examples/durations/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.582399 batou-2.4rc2/examples/errors/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2023-11-29 10:06:22.000000 batou-2.4rc2/examples/errors/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.583073 batou-2.4rc2/examples/errors2/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2023-11-29 10:06:22.000000 batou-2.4rc2/examples/errors2/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.583519 batou-2.4rc2/examples/ignores/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2023-11-29 10:06:22.000000 batou-2.4rc2/examples/ignores/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.583898 batou-2.4rc2/examples/largetempl/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2023-11-29 10:06:22.000000 batou-2.4rc2/examples/largetempl/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.584345 batou-2.4rc2/examples/package/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2023-11-29 10:06:22.000000 batou-2.4rc2/examples/package/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.584756 batou-2.4rc2/examples/sync_async/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2023-11-29 10:06:22.000000 batou-2.4rc2/examples/sync_async/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.585139 batou-2.4rc2/examples/tutorial-buildout/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2023-11-29 10:06:22.000000 batou-2.4rc2/examples/tutorial-buildout/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.585684 batou-2.4rc2/examples/tutorial-component/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2023-11-29 10:06:22.000000 batou-2.4rc2/examples/tutorial-component/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.586057 batou-2.4rc2/examples/tutorial-helloworld/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2023-11-29 10:06:22.000000 batou-2.4rc2/examples/tutorial-helloworld/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.586417 batou-2.4rc2/examples/tutorial-parallelize/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2023-11-29 10:06:22.000000 batou-2.4rc2/examples/tutorial-parallelize/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.586976 batou-2.4rc2/examples/tutorial-provision-container/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2023-11-29 10:06:22.000000 batou-2.4rc2/examples/tutorial-provision-container/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.587816 batou-2.4rc2/examples/tutorial-secrets/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.536108 batou-2.4rc2/examples/tutorial-secrets/environments/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.588282 batou-2.4rc2/examples/tutorial-secrets/environments/age/
--rw-r--r--   0 ctheune    (501) staff       (20)     2431 2023-11-29 10:06:22.000000 batou-2.4rc2/examples/tutorial-secrets/environments/age/age_keys.txt
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2023-11-29 10:06:22.000000 batou-2.4rc2/examples/tutorial-secrets/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.588693 batou-2.4rc2/examples/vagrant/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2023-11-29 10:06:22.000000 batou-2.4rc2/examples/vagrant/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.589077 batou-2.4rc2/examples/vagrant-multi/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2023-11-29 10:06:22.000000 batou-2.4rc2/examples/vagrant-multi/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.589453 batou-2.4rc2/examples/venvs/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.589820 batou-2.4rc2/examples/venvs/environments/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2023-11-29 10:06:22.000000 batou-2.4rc2/examples/venvs/environments/requirements.txt
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2023-11-29 10:06:22.000000 batou-2.4rc2/examples/venvs/requirements.txt
--rw-r--r--   0 ctheune    (501) staff       (20)      129 2023-11-29 10:06:22.000000 batou-2.4rc2/pyproject.toml
--rw-r--r--   0 ctheune    (501) staff       (20)      277 2023-11-29 10:06:22.000000 batou-2.4rc2/requirements-dev.txt
--rw-r--r--   0 ctheune    (501) staff       (20)      139 2023-11-29 10:06:25.675303 batou-2.4rc2/setup.cfg
--rw-r--r--   0 ctheune    (501) staff       (20)     2248 2023-11-29 10:06:22.000000 batou-2.4rc2/setup.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.537622 batou-2.4rc2/src/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.601189 batou-2.4rc2/src/batou/
--rw-r--r--   0 ctheune    (501) staff       (20)    22450 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/__init__.py
--rw-r--r--   0 ctheune    (501) staff       (20)      997 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/_output.py
--rw-r--r--   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/agent.py
--rw-r--r--   0 ctheune    (501) staff       (20)      163 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/c.py
--rw-r--r--   0 ctheune    (501) staff       (20)    40979 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/component.py
--rw-r--r--   0 ctheune    (501) staff       (20)      795 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/conftest.py
--rw-r--r--   0 ctheune    (501) staff       (20)    14630 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/deploy.py
--rw-r--r--   0 ctheune    (501) staff       (20)    21013 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/environment.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1507 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/fixtures.py
--rw-r--r--   0 ctheune    (501) staff       (20)    12064 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/host.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.604977 batou-2.4rc2/src/batou/init-template/
--rw-r--r--   0 ctheune    (501) staff       (20)       44 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/init-template/.hgignore
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.538452 batou-2.4rc2/src/batou/init-template/components/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.605443 batou-2.4rc2/src/batou/init-template/components/example/
--rw-r--r--   0 ctheune    (501) staff       (20)      177 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/init-template/components/example/component.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.605912 batou-2.4rc2/src/batou/init-template/environments/
--rw-r--r--   0 ctheune    (501) staff       (20)       66 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/init-template/environments/dev.cfg
--rw-r--r--   0 ctheune    (501) staff       (20)      411 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/insecure-private.key
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.621007 batou-2.4rc2/src/batou/lib/
--rw-r--r--   0 ctheune    (501) staff       (20)       29 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/__init__.py
--rw-r--r--   0 ctheune    (501) staff       (20)     3983 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/appenv.py
--rw-r--r--   0 ctheune    (501) staff       (20)     6457 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/archive.py
--rw-r--r--   0 ctheune    (501) staff       (20)     3297 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/buildout.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2211 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/cmmi.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2524 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/cron.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1224 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/debian.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2286 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/download.py
--rw-r--r--   0 ctheune    (501) staff       (20)    22067 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/file.py
--rw-r--r--   0 ctheune    (501) staff       (20)     6368 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/git.py
--rw-r--r--   0 ctheune    (501) staff       (20)      854 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/goceptnet.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1388 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/logrotate.py
--rw-r--r--   0 ctheune    (501) staff       (20)     4541 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/mercurial.py
--rw-r--r--   0 ctheune    (501) staff       (20)     3647 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/mysql.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2814 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/nagios.py
--rw-r--r--   0 ctheune    (501) staff       (20)      707 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/package.py
--rw-r--r--   0 ctheune    (501) staff       (20)     8150 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/python.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.624999 batou-2.4rc2/src/batou/lib/resources/
--rw-r--r--   0 ctheune    (501) staff       (20)     2120 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/resources/check_supervisor.py.in
--rw-r--r--   0 ctheune    (501) staff       (20)      244 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/resources/crontab
--rw-r--r--   0 ctheune    (501) staff       (20)      548 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/resources/init.sh
--rw-r--r--   0 ctheune    (501) staff       (20)      299 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/resources/logrotate.in
--rw-r--r--   0 ctheune    (501) staff       (20)      840 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/resources/nagios.cfg
--rw-r--r--   0 ctheune    (501) staff       (20)      153 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/resources/nrpe.cfg
--rw-r--r--   0 ctheune    (501) staff       (20)      380 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/resources/supervisor.buildout.cfg
--rw-r--r--   0 ctheune    (501) staff       (20)      609 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/resources/supervisor.conf
--rw-r--r--   0 ctheune    (501) staff       (20)      932 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/service.py
--rw-r--r--   0 ctheune    (501) staff       (20)    10273 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/supervisor.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1172 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/svn.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.635033 batou-2.4rc2/src/batou/lib/tests/
--rw-r--r--   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/tests/__init__.py
--rw-r--r--   0 ctheune    (501) staff       (20)     3083 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/tests/test_appenv.py
--rw-r--r--   0 ctheune    (501) staff       (20)     3858 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/tests/test_archive.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2449 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/tests/test_buildout.py
--rw-r--r--   0 ctheune    (501) staff       (20)     3261 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/tests/test_cmmi.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2110 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/tests/test_cron.py
--rw-r--r--   0 ctheune    (501) staff       (20)      639 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/tests/test_debian.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2158 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/tests/test_download.py
--rw-r--r--   0 ctheune    (501) staff       (20)    31505 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/tests/test_file.py
--rw-r--r--   0 ctheune    (501) staff       (20)    10383 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/tests/test_git.py
--rw-r--r--   0 ctheune    (501) staff       (20)     6165 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/tests/test_mercurial.py
--rw-r--r--   0 ctheune    (501) staff       (20)      121 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/tests/test_mysql.py
--rw-r--r--   0 ctheune    (501) staff       (20)      847 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/tests/test_nagios.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1430 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/tests/test_python.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1693 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/tests/test_service.py
--rw-r--r--   0 ctheune    (501) staff       (20)     3106 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/tests/test_supervisor.py
--rw-r--r--   0 ctheune    (501) staff       (20)      707 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/lib/tests/test_svn.py
--rw-r--r--   0 ctheune    (501) staff       (20)     6247 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/main.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.635656 batou-2.4rc2/src/batou/migrate/
--rw-r--r--   0 ctheune    (501) staff       (20)     3377 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/migrate/__init__.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.638501 batou-2.4rc2/src/batou/migrate/migrations/
--rw-r--r--   0 ctheune    (501) staff       (20)      389 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/migrate/migrations/2300.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1775 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/migrate/migrations/2301.py
--rw-r--r--   0 ctheune    (501) staff       (20)      874 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/migrate/migrations/2302.py
--rw-r--r--   0 ctheune    (501) staff       (20)      790 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/migrate/migrations/2303.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1282 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/migrate/migrations/2400.py
--rw-r--r--   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/migrate/migrations/__init__.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.639303 batou-2.4rc2/src/batou/migrate/tests/
--rw-r--r--   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/migrate/tests/__init__.py
--rw-r--r--   0 ctheune    (501) staff       (20)     4532 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/migrate/tests/test_migrate.py
--rw-r--r--   0 ctheune    (501) staff       (20)    15653 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/provision.py
--rw-r--r--   0 ctheune    (501) staff       (20)    11728 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/remote_core.py
--rw-r--r--   0 ctheune    (501) staff       (20)    13393 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/repository.py
--rw-r--r--   0 ctheune    (501) staff       (20)     6424 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/resources.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.642209 batou-2.4rc2/src/batou/secrets/
--rw-r--r--   0 ctheune    (501) staff       (20)    22918 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/secrets/__init__.py
--rw-r--r--   0 ctheune    (501) staff       (20)     3935 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/secrets/edit.py
--rw-r--r--   0 ctheune    (501) staff       (20)    13507 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/secrets/encryption.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2434 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/secrets/manage.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.649867 batou-2.4rc2/src/batou/secrets/tests/
--rw-r--r--   0 ctheune    (501) staff       (20)       23 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/secrets/tests/__init__.py
--rw-r--r--   0 ctheune    (501) staff       (20)     3706 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/secrets/tests/test_editor.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2307 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/secrets/tests/test_manage.py
--rw-r--r--   0 ctheune    (501) staff       (20)     4379 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/secrets/tests/test_secrets.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2429 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/template.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.662095 batou-2.4rc2/src/batou/tests/
--rw-r--r--   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/__init__.py
--rw-r--r--   0 ctheune    (501) staff       (20)      666 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/conftest.py
--rw-r--r--   0 ctheune    (501) staff       (20)     3012 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/ellipsis.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.559121 batou-2.4rc2/src/batou/tests/fixture/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.662734 batou-2.4rc2/src/batou/tests/fixture/basic_service/
--rw-r--r--   0 ctheune    (501) staff       (20)       33 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/fixture/basic_service/.batou.json
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.551360 batou-2.4rc2/src/batou/tests/fixture/basic_service/components/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.663915 batou-2.4rc2/src/batou/tests/fixture/basic_service/components/zeo/
--rw-r--r--   0 ctheune    (501) staff       (20)      178 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/fixture/basic_service/components/zeo/component.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.664733 batou-2.4rc2/src/batou/tests/fixture/basic_service/components/zope/
--rw-r--r--   0 ctheune    (501) staff       (20)       72 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/fixture/basic_service/components/zope/component.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.552650 batou-2.4rc2/src/batou/tests/fixture/basic_service/environments/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.665932 batou-2.4rc2/src/batou/tests/fixture/basic_service/environments/dev/
--rw-r--r--   0 ctheune    (501) staff       (20)       79 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/fixture/basic_service/environments/dev/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.666385 batou-2.4rc2/src/batou/tests/fixture/basic_service/environments/production/
--rw-r--r--   0 ctheune    (501) staff       (20)      128 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/fixture/basic_service/environments/production/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.666758 batou-2.4rc2/src/batou/tests/fixture/component/
--rw-r--r--   0 ctheune    (501) staff       (20)       40 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/fixture/component/haproxy.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.667248 batou-2.4rc2/src/batou/tests/fixture/sample_service/
--rw-r--r--   0 ctheune    (501) staff       (20)       33 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/fixture/sample_service/.batou.json
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.553755 batou-2.4rc2/src/batou/tests/fixture/sample_service/components/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.667776 batou-2.4rc2/src/batou/tests/fixture/sample_service/components/hello/
--rw-r--r--   0 ctheune    (501) staff       (20)      973 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/fixture/sample_service/components/hello/component.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.557003 batou-2.4rc2/src/batou/tests/fixture/sample_service/environments/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.668206 batou-2.4rc2/src/batou/tests/fixture/sample_service/environments/test-multiple-components/
--rw-r--r--   0 ctheune    (501) staff       (20)      144 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/fixture/sample_service/environments/test-multiple-components/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.668592 batou-2.4rc2/src/batou/tests/fixture/sample_service/environments/test-multiple-hosts/
--rw-r--r--   0 ctheune    (501) staff       (20)       88 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/fixture/sample_service/environments/test-multiple-hosts/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.668971 batou-2.4rc2/src/batou/tests/fixture/sample_service/environments/test-overlapping-components/
--rw-r--r--   0 ctheune    (501) staff       (20)      110 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/fixture/sample_service/environments/test-overlapping-components/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.669344 batou-2.4rc2/src/batou/tests/fixture/sample_service/environments/test-resolver/
--rw-r--r--   0 ctheune    (501) staff       (20)       72 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/fixture/sample_service/environments/test-resolver/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.669769 batou-2.4rc2/src/batou/tests/fixture/sample_service/environments/test-resolver-invalid/
--rw-r--r--   0 ctheune    (501) staff       (20)       90 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/fixture/sample_service/environments/test-resolver-invalid/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.670142 batou-2.4rc2/src/batou/tests/fixture/sample_service/environments/test-with-env-config/
--rw-r--r--   0 ctheune    (501) staff       (20)      191 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/fixture/sample_service/environments/test-with-env-config/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.670497 batou-2.4rc2/src/batou/tests/fixture/sample_service/environments/test-with-overrides/
--rw-r--r--   0 ctheune    (501) staff       (20)       94 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/fixture/sample_service/environments/test-with-overrides/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.670859 batou-2.4rc2/src/batou/tests/fixture/sample_service/environments/test-with-provide-require/
--rw-r--r--   0 ctheune    (501) staff       (20)       85 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/fixture/sample_service/environments/test-with-provide-require/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.671205 batou-2.4rc2/src/batou/tests/fixture/sample_service/environments/test-with-vfs-sandbox/
--rw-r--r--   0 ctheune    (501) staff       (20)       64 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/fixture/sample_service/environments/test-with-vfs-sandbox/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.671551 batou-2.4rc2/src/batou/tests/fixture/sample_service/environments/test-without-env-config/
--rw-r--r--   0 ctheune    (501) staff       (20)       26 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/fixture/sample_service/environments/test-without-env-config/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.671920 batou-2.4rc2/src/batou/tests/fixture/service_early_resource/
--rw-r--r--   0 ctheune    (501) staff       (20)       33 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/fixture/service_early_resource/.batou.json
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.558108 batou-2.4rc2/src/batou/tests/fixture/service_early_resource/components/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.672353 batou-2.4rc2/src/batou/tests/fixture/service_early_resource/components/zeo/
--rw-r--r--   0 ctheune    (501) staff       (20)      346 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/fixture/service_early_resource/components/zeo/component.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.672917 batou-2.4rc2/src/batou/tests/fixture/service_early_resource/components/zope/
--rw-r--r--   0 ctheune    (501) staff       (20)      116 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/fixture/service_early_resource/components/zope/component.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.558736 batou-2.4rc2/src/batou/tests/fixture/service_early_resource/environments/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.673297 batou-2.4rc2/src/batou/tests/fixture/service_early_resource/environments/dev/
--rw-r--r--   0 ctheune    (501) staff       (20)       62 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/fixture/service_early_resource/environments/dev/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.674061 batou-2.4rc2/src/batou/tests/fixture/template/
--rw-r--r--   0 ctheune    (501) staff       (20)       84 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/fixture/template/haproxy.cfg
--rw-r--r--   0 ctheune    (501) staff       (20)      119 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/fixture/template/haproxy.cfg.jinja2
--rw-r--r--   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/test_bootstrap.py
--rw-r--r--   0 ctheune    (501) staff       (20)    18565 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/test_component.py
--rw-r--r--   0 ctheune    (501) staff       (20)     4776 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/test_config.py
--rw-r--r--   0 ctheune    (501) staff       (20)     5707 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/test_dependencies.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1725 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/test_deploy.py
--rw-r--r--   0 ctheune    (501) staff       (20)    10621 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/test_endtoend.py
--rw-r--r--   0 ctheune    (501) staff       (20)     8674 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/test_environment.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2305 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/test_exceptions.py
--rw-r--r--   0 ctheune    (501) staff       (20)      606 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/test_host.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1488 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/test_main.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1326 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/test_remote.py
--rw-r--r--   0 ctheune    (501) staff       (20)     9398 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/test_remote_core.py
--rw-r--r--   0 ctheune    (501) staff       (20)     3648 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/test_repository.py
--rw-r--r--   0 ctheune    (501) staff       (20)      743 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/test_resources.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2602 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/test_template.py
--rw-r--r--   0 ctheune    (501) staff       (20)    16346 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/test_utils.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1169 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/tests/test_vfs.py
--rw-r--r--   0 ctheune    (501) staff       (20)    19046 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/utils.py
--rw-r--r--   0 ctheune    (501) staff       (20)        7 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/version.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     1009 2023-11-29 10:06:22.000000 batou-2.4rc2/src/batou/vfs.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2023-11-29 10:06:25.604528 batou-2.4rc2/src/batou.egg-info/
--rw-r--r--   0 ctheune    (501) staff       (20)     3446 2023-11-29 10:06:23.000000 batou-2.4rc2/src/batou.egg-info/PKG-INFO
--rw-r--r--   0 ctheune    (501) staff       (20)     6796 2023-11-29 10:06:25.000000 batou-2.4rc2/src/batou.egg-info/SOURCES.txt
--rw-r--r--   0 ctheune    (501) staff       (20)        1 2023-11-29 10:06:23.000000 batou-2.4rc2/src/batou.egg-info/dependency_links.txt
--rw-r--r--   0 ctheune    (501) staff       (20)      220 2023-11-29 10:06:23.000000 batou-2.4rc2/src/batou.egg-info/entry_points.txt
--rw-r--r--   0 ctheune    (501) staff       (20)        1 2023-11-29 10:06:23.000000 batou-2.4rc2/src/batou.egg-info/not-zip-safe
--rw-r--r--   0 ctheune    (501) staff       (20)      184 2023-11-29 10:06:23.000000 batou-2.4rc2/src/batou.egg-info/requires.txt
--rw-r--r--   0 ctheune    (501) staff       (20)        6 2023-11-29 10:06:23.000000 batou-2.4rc2/src/batou.egg-info/top_level.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.102186 batou-2.5.0b1/
+-rw-r--r--   0 zagy       (501) staff       (20)    31241 2024-04-19 05:17:22.000000 batou-2.5.0b1/CHANGES.history.txt
+-rw-r--r--   0 zagy       (501) staff       (20)     1608 2024-04-19 05:17:22.000000 batou-2.5.0b1/LICENSE.txt
+-rw-r--r--   0 zagy       (501) staff       (20)      212 2024-04-19 05:17:22.000000 batou-2.5.0b1/MANIFEST.in
+-rw-r--r--   0 zagy       (501) staff       (20)     3973 2024-04-19 05:17:23.102099 batou-2.5.0b1/PKG-INFO
+-rw-r--r--   0 zagy       (501) staff       (20)     2691 2024-04-19 05:17:22.000000 batou-2.5.0b1/README.md
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.073315 batou-2.5.0b1/doc/
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.080193 batou-2.5.0b1/doc/source/
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.080741 batou-2.5.0b1/doc/source/api/
+-rw-r--r--   0 zagy       (501) staff       (20)      886 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/api/component.txt
+-rw-r--r--   0 zagy       (501) staff       (20)     2299 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/api/environment.txt
+-rw-r--r--   0 zagy       (501) staff       (20)       48 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/api/templates.txt
+-rw-r--r--   0 zagy       (501) staff       (20)       63 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/api/utilities.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.080861 batou-2.5.0b1/doc/source/cli/
+-rw-r--r--   0 zagy       (501) staff       (20)     4731 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/cli/index.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.081564 batou-2.5.0b1/doc/source/components/
+-rw-r--r--   0 zagy       (501) staff       (20)     1025 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/components/cmmi.txt
+-rw-r--r--   0 zagy       (501) staff       (20)     2941 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/components/downloads-vcs.txt
+-rw-r--r--   0 zagy       (501) staff       (20)     5657 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/components/files.txt
+-rw-r--r--   0 zagy       (501) staff       (20)     4820 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/components/python.txt
+-rw-r--r--   0 zagy       (501) staff       (20)     3050 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/components/services.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.082032 batou-2.5.0b1/doc/source/dev/
+-rw-r--r--   0 zagy       (501) staff       (20)      718 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/dev/authors.txt
+-rw-r--r--   0 zagy       (501) staff       (20)     8555 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/dev/contributing.txt
+-rw-r--r--   0 zagy       (501) staff       (20)     1711 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/dev/testing.txt
+-rw-r--r--   0 zagy       (501) staff       (20)     2809 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/dev/todo.txt
+-rw-r--r--   0 zagy       (501) staff       (20)     8498 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/index.txt
+-rw-r--r--   0 zagy       (501) staff       (20)     4799 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/upgrading.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.082699 batou-2.5.0b1/doc/source/user/
+-rw-r--r--   0 zagy       (501) staff       (20)    10870 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/user/advanced.txt
+-rw-r--r--   0 zagy       (501) staff       (20)     2565 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/user/install.txt
+-rw-r--r--   0 zagy       (501) staff       (20)     3848 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/user/installation-deb.txt
+-rw-r--r--   0 zagy       (501) staff       (20)     3798 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/user/installation-rpm.txt
+-rw-r--r--   0 zagy       (501) staff       (20)     2907 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/user/intro.txt
+-rw-r--r--   0 zagy       (501) staff       (20)    47505 2024-04-19 05:17:22.000000 batou-2.5.0b1/doc/source/user/quickstart.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.075183 batou-2.5.0b1/examples/
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.082957 batou-2.5.0b1/examples/api/
+-rw-r--r--   0 zagy       (501) staff       (20)      349 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/api/index.txt
+-rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/api/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.083060 batou-2.5.0b1/examples/django/
+-rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/django/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.083169 batou-2.5.0b1/examples/durations/
+-rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/durations/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.083272 batou-2.5.0b1/examples/errors/
+-rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/errors/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.083378 batou-2.5.0b1/examples/errors2/
+-rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/errors2/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.083486 batou-2.5.0b1/examples/errorsnohost/
+-rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/errorsnohost/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.083593 batou-2.5.0b1/examples/ignores/
+-rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/ignores/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.083704 batou-2.5.0b1/examples/largetempl/
+-rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/largetempl/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.083811 batou-2.5.0b1/examples/package/
+-rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/package/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.083913 batou-2.5.0b1/examples/sync_async/
+-rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/sync_async/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.084018 batou-2.5.0b1/examples/tutorial-buildout/
+-rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/tutorial-buildout/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.084123 batou-2.5.0b1/examples/tutorial-component/
+-rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/tutorial-component/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.084237 batou-2.5.0b1/examples/tutorial-helloworld/
+-rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/tutorial-helloworld/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.084345 batou-2.5.0b1/examples/tutorial-parallelize/
+-rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/tutorial-parallelize/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.084454 batou-2.5.0b1/examples/tutorial-provision-container/
+-rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/tutorial-provision-container/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.084561 batou-2.5.0b1/examples/tutorial-secrets/
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.074943 batou-2.5.0b1/examples/tutorial-secrets/environments/
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.084670 batou-2.5.0b1/examples/tutorial-secrets/environments/age/
+-rw-r--r--   0 zagy       (501) staff       (20)     2269 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/tutorial-secrets/environments/age/age_keys.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.084787 batou-2.5.0b1/examples/tutorial-secrets/environments/age-diffable/
+-rw-r--r--   0 zagy       (501) staff       (20)     2269 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/tutorial-secrets/environments/age-diffable/age_keys.txt
+-rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/tutorial-secrets/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.084897 batou-2.5.0b1/examples/vagrant/
+-rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/vagrant/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.085005 batou-2.5.0b1/examples/vagrant-multi/
+-rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/vagrant-multi/requirements.txt
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.085111 batou-2.5.0b1/examples/venvs/
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.085217 batou-2.5.0b1/examples/venvs/environments/
+-rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/venvs/environments/requirements.txt
+-rw-r--r--   0 zagy       (501) staff       (20)       54 2024-04-19 05:17:22.000000 batou-2.5.0b1/examples/venvs/requirements.txt
+-rw-r--r--   0 zagy       (501) staff       (20)      129 2024-04-19 05:17:22.000000 batou-2.5.0b1/pyproject.toml
+-rw-r--r--   0 zagy       (501) staff       (20)      277 2024-04-19 05:17:22.000000 batou-2.5.0b1/requirements-dev.txt
+-rw-r--r--   0 zagy       (501) staff       (20)      139 2024-04-19 05:17:23.102414 batou-2.5.0b1/setup.cfg
+-rw-r--r--   0 zagy       (501) staff       (20)     2248 2024-04-19 05:17:22.000000 batou-2.5.0b1/setup.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.075484 batou-2.5.0b1/src/
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.087773 batou-2.5.0b1/src/batou/
+-rw-r--r--   0 zagy       (501) staff       (20)    25625 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/__init__.py
+-rw-r--r--   0 zagy       (501) staff       (20)      997 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/_output.py
+-rw-r--r--   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/agent.py
+-rw-r--r--   0 zagy       (501) staff       (20)      163 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/c.py
+-rw-r--r--   0 zagy       (501) staff       (20)    41055 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/component.py
+-rw-r--r--   0 zagy       (501) staff       (20)      795 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/conftest.py
+-rw-r--r--   0 zagy       (501) staff       (20)    14886 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/deploy.py
+-rw-r--r--   0 zagy       (501) staff       (20)    21045 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/environment.py
+-rw-r--r--   0 zagy       (501) staff       (20)     1507 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/fixtures.py
+-rw-r--r--   0 zagy       (501) staff       (20)    12064 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/host.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.088633 batou-2.5.0b1/src/batou/init-template/
+-rw-r--r--   0 zagy       (501) staff       (20)       44 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/init-template/.hgignore
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.075706 batou-2.5.0b1/src/batou/init-template/components/
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.088746 batou-2.5.0b1/src/batou/init-template/components/example/
+-rw-r--r--   0 zagy       (501) staff       (20)      177 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/init-template/components/example/component.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.088853 batou-2.5.0b1/src/batou/init-template/environments/
+-rw-r--r--   0 zagy       (501) staff       (20)       66 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/init-template/environments/dev.cfg
+-rw-r--r--   0 zagy       (501) staff       (20)      411 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/insecure-private.key
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.091106 batou-2.5.0b1/src/batou/lib/
+-rw-r--r--   0 zagy       (501) staff       (20)       29 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/__init__.py
+-rw-r--r--   0 zagy       (501) staff       (20)     3983 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/appenv.py
+-rw-r--r--   0 zagy       (501) staff       (20)     6457 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/archive.py
+-rw-r--r--   0 zagy       (501) staff       (20)     3297 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/buildout.py
+-rw-r--r--   0 zagy       (501) staff       (20)     2211 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/cmmi.py
+-rw-r--r--   0 zagy       (501) staff       (20)     2524 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/cron.py
+-rw-r--r--   0 zagy       (501) staff       (20)     1224 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/debian.py
+-rw-r--r--   0 zagy       (501) staff       (20)     2286 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/download.py
+-rw-r--r--   0 zagy       (501) staff       (20)    23943 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/file.py
+-rw-r--r--   0 zagy       (501) staff       (20)     6872 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/git.py
+-rw-r--r--   0 zagy       (501) staff       (20)      854 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/goceptnet.py
+-rw-r--r--   0 zagy       (501) staff       (20)     1388 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/logrotate.py
+-rw-r--r--   0 zagy       (501) staff       (20)     4541 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/mercurial.py
+-rw-r--r--   0 zagy       (501) staff       (20)     3647 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/mysql.py
+-rw-r--r--   0 zagy       (501) staff       (20)     2814 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/nagios.py
+-rw-r--r--   0 zagy       (501) staff       (20)      707 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/package.py
+-rw-r--r--   0 zagy       (501) staff       (20)     8150 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/python.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.092117 batou-2.5.0b1/src/batou/lib/resources/
+-rw-r--r--   0 zagy       (501) staff       (20)     2120 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/resources/check_supervisor.py.in
+-rw-r--r--   0 zagy       (501) staff       (20)      244 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/resources/crontab
+-rw-r--r--   0 zagy       (501) staff       (20)      548 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/resources/init.sh
+-rw-r--r--   0 zagy       (501) staff       (20)      299 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/resources/logrotate.in
+-rw-r--r--   0 zagy       (501) staff       (20)      840 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/resources/nagios.cfg
+-rw-r--r--   0 zagy       (501) staff       (20)      153 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/resources/nrpe.cfg
+-rw-r--r--   0 zagy       (501) staff       (20)      380 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/resources/supervisor.buildout.cfg
+-rw-r--r--   0 zagy       (501) staff       (20)      609 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/resources/supervisor.conf
+-rw-r--r--   0 zagy       (501) staff       (20)      932 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/service.py
+-rw-r--r--   0 zagy       (501) staff       (20)    10273 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/supervisor.py
+-rw-r--r--   0 zagy       (501) staff       (20)     1172 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/svn.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.094264 batou-2.5.0b1/src/batou/lib/tests/
+-rw-r--r--   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/__init__.py
+-rw-r--r--   0 zagy       (501) staff       (20)     3083 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/test_appenv.py
+-rw-r--r--   0 zagy       (501) staff       (20)     3858 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/test_archive.py
+-rw-r--r--   0 zagy       (501) staff       (20)     2449 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/test_buildout.py
+-rw-r--r--   0 zagy       (501) staff       (20)     3261 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/test_cmmi.py
+-rw-r--r--   0 zagy       (501) staff       (20)     2110 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/test_cron.py
+-rw-r--r--   0 zagy       (501) staff       (20)      639 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/test_debian.py
+-rw-r--r--   0 zagy       (501) staff       (20)     2158 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/test_download.py
+-rw-r--r--   0 zagy       (501) staff       (20)    32144 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/test_file.py
+-rw-r--r--   0 zagy       (501) staff       (20)    11092 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/test_git.py
+-rw-r--r--   0 zagy       (501) staff       (20)     6165 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/test_mercurial.py
+-rw-r--r--   0 zagy       (501) staff       (20)      121 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/test_mysql.py
+-rw-r--r--   0 zagy       (501) staff       (20)      847 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/test_nagios.py
+-rw-r--r--   0 zagy       (501) staff       (20)     1430 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/test_python.py
+-rw-r--r--   0 zagy       (501) staff       (20)     1693 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/test_service.py
+-rw-r--r--   0 zagy       (501) staff       (20)     3106 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/test_supervisor.py
+-rw-r--r--   0 zagy       (501) staff       (20)      707 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/lib/tests/test_svn.py
+-rw-r--r--   0 zagy       (501) staff       (20)     6608 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/main.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.094388 batou-2.5.0b1/src/batou/migrate/
+-rw-r--r--   0 zagy       (501) staff       (20)     3377 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/migrate/__init__.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.095044 batou-2.5.0b1/src/batou/migrate/migrations/
+-rw-r--r--   0 zagy       (501) staff       (20)      389 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/migrate/migrations/2300.py
+-rw-r--r--   0 zagy       (501) staff       (20)     1775 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/migrate/migrations/2301.py
+-rw-r--r--   0 zagy       (501) staff       (20)      874 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/migrate/migrations/2302.py
+-rw-r--r--   0 zagy       (501) staff       (20)      790 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/migrate/migrations/2303.py
+-rw-r--r--   0 zagy       (501) staff       (20)     1282 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/migrate/migrations/2400.py
+-rw-r--r--   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/migrate/migrations/__init__.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.095221 batou-2.5.0b1/src/batou/migrate/tests/
+-rw-r--r--   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/migrate/tests/__init__.py
+-rw-r--r--   0 zagy       (501) staff       (20)     4532 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/migrate/tests/test_migrate.py
+-rw-r--r--   0 zagy       (501) staff       (20)    15653 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/provision.py
+-rw-r--r--   0 zagy       (501) staff       (20)    11728 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/remote_core.py
+-rw-r--r--   0 zagy       (501) staff       (20)    13588 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/repository.py
+-rw-r--r--   0 zagy       (501) staff       (20)     6424 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/resources.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.095709 batou-2.5.0b1/src/batou/secrets/
+-rw-r--r--   0 zagy       (501) staff       (20)    24397 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/secrets/__init__.py
+-rw-r--r--   0 zagy       (501) staff       (20)     4372 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/secrets/edit.py
+-rw-r--r--   0 zagy       (501) staff       (20)    17282 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/secrets/encryption.py
+-rw-r--r--   0 zagy       (501) staff       (20)     2800 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/secrets/manage.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.096147 batou-2.5.0b1/src/batou/secrets/tests/
+-rw-r--r--   0 zagy       (501) staff       (20)       23 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/secrets/tests/__init__.py
+-rw-r--r--   0 zagy       (501) staff       (20)     5126 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/secrets/tests/test_editor.py
+-rw-r--r--   0 zagy       (501) staff       (20)     3994 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/secrets/tests/test_manage.py
+-rw-r--r--   0 zagy       (501) staff       (20)     4379 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/secrets/tests/test_secrets.py
+-rw-r--r--   0 zagy       (501) staff       (20)     2696 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/template.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.098355 batou-2.5.0b1/src/batou/tests/
+-rw-r--r--   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/__init__.py
+-rw-r--r--   0 zagy       (501) staff       (20)      666 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/conftest.py
+-rw-r--r--   0 zagy       (501) staff       (20)     3012 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/ellipsis.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.078747 batou-2.5.0b1/src/batou/tests/fixture/
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.098462 batou-2.5.0b1/src/batou/tests/fixture/basic_service/
+-rw-r--r--   0 zagy       (501) staff       (20)       33 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/basic_service/.batou.json
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.076847 batou-2.5.0b1/src/batou/tests/fixture/basic_service/components/
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.098577 batou-2.5.0b1/src/batou/tests/fixture/basic_service/components/zeo/
+-rw-r--r--   0 zagy       (501) staff       (20)      178 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/basic_service/components/zeo/component.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.098684 batou-2.5.0b1/src/batou/tests/fixture/basic_service/components/zope/
+-rw-r--r--   0 zagy       (501) staff       (20)       72 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/basic_service/components/zope/component.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.077065 batou-2.5.0b1/src/batou/tests/fixture/basic_service/environments/
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.098796 batou-2.5.0b1/src/batou/tests/fixture/basic_service/environments/dev/
+-rw-r--r--   0 zagy       (501) staff       (20)       79 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/basic_service/environments/dev/environment.cfg
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.098907 batou-2.5.0b1/src/batou/tests/fixture/basic_service/environments/production/
+-rw-r--r--   0 zagy       (501) staff       (20)      128 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/basic_service/environments/production/environment.cfg
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.099014 batou-2.5.0b1/src/batou/tests/fixture/component/
+-rw-r--r--   0 zagy       (501) staff       (20)       40 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/component/haproxy.cfg
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.099126 batou-2.5.0b1/src/batou/tests/fixture/sample_service/
+-rw-r--r--   0 zagy       (501) staff       (20)       33 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/sample_service/.batou.json
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.077357 batou-2.5.0b1/src/batou/tests/fixture/sample_service/components/
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.099233 batou-2.5.0b1/src/batou/tests/fixture/sample_service/components/hello/
+-rw-r--r--   0 zagy       (501) staff       (20)      973 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/sample_service/components/hello/component.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.078227 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.099349 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-multiple-components/
+-rw-r--r--   0 zagy       (501) staff       (20)      144 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-multiple-components/environment.cfg
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.099462 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-multiple-hosts/
+-rw-r--r--   0 zagy       (501) staff       (20)       88 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-multiple-hosts/environment.cfg
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.099573 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-overlapping-components/
+-rw-r--r--   0 zagy       (501) staff       (20)      110 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-overlapping-components/environment.cfg
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.099681 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-resolver/
+-rw-r--r--   0 zagy       (501) staff       (20)       72 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-resolver/environment.cfg
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.099801 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-resolver-invalid/
+-rw-r--r--   0 zagy       (501) staff       (20)       90 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-resolver-invalid/environment.cfg
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.099932 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-with-env-config/
+-rw-r--r--   0 zagy       (501) staff       (20)      191 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-with-env-config/environment.cfg
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.100053 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-with-overrides/
+-rw-r--r--   0 zagy       (501) staff       (20)       94 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-with-overrides/environment.cfg
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.100178 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-with-provide-require/
+-rw-r--r--   0 zagy       (501) staff       (20)       85 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-with-provide-require/environment.cfg
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.100309 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-with-vfs-sandbox/
+-rw-r--r--   0 zagy       (501) staff       (20)       64 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-with-vfs-sandbox/environment.cfg
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.100437 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-without-env-config/
+-rw-r--r--   0 zagy       (501) staff       (20)       26 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/sample_service/environments/test-without-env-config/environment.cfg
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.100563 batou-2.5.0b1/src/batou/tests/fixture/service_early_resource/
+-rw-r--r--   0 zagy       (501) staff       (20)       33 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/service_early_resource/.batou.json
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.078523 batou-2.5.0b1/src/batou/tests/fixture/service_early_resource/components/
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.100697 batou-2.5.0b1/src/batou/tests/fixture/service_early_resource/components/zeo/
+-rw-r--r--   0 zagy       (501) staff       (20)      346 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/service_early_resource/components/zeo/component.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.100825 batou-2.5.0b1/src/batou/tests/fixture/service_early_resource/components/zope/
+-rw-r--r--   0 zagy       (501) staff       (20)      116 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/service_early_resource/components/zope/component.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.078667 batou-2.5.0b1/src/batou/tests/fixture/service_early_resource/environments/
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.100952 batou-2.5.0b1/src/batou/tests/fixture/service_early_resource/environments/dev/
+-rw-r--r--   0 zagy       (501) staff       (20)       62 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/service_early_resource/environments/dev/environment.cfg
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.101196 batou-2.5.0b1/src/batou/tests/fixture/template/
+-rw-r--r--   0 zagy       (501) staff       (20)       84 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/template/haproxy.cfg
+-rw-r--r--   0 zagy       (501) staff       (20)      119 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/fixture/template/haproxy.cfg.jinja2
+-rw-r--r--   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_bootstrap.py
+-rw-r--r--   0 zagy       (501) staff       (20)    18565 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_component.py
+-rw-r--r--   0 zagy       (501) staff       (20)     4776 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_config.py
+-rw-r--r--   0 zagy       (501) staff       (20)     5707 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_dependencies.py
+-rw-r--r--   0 zagy       (501) staff       (20)     3012 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_deploy.py
+-rw-r--r--   0 zagy       (501) staff       (20)    11409 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_endtoend.py
+-rw-r--r--   0 zagy       (501) staff       (20)     8674 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_environment.py
+-rw-r--r--   0 zagy       (501) staff       (20)     2311 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_exceptions.py
+-rw-r--r--   0 zagy       (501) staff       (20)      606 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_host.py
+-rw-r--r--   0 zagy       (501) staff       (20)     1488 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_main.py
+-rw-r--r--   0 zagy       (501) staff       (20)     2144 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_remote.py
+-rw-r--r--   0 zagy       (501) staff       (20)     9398 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_remote_core.py
+-rw-r--r--   0 zagy       (501) staff       (20)     3648 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_repository.py
+-rw-r--r--   0 zagy       (501) staff       (20)      743 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_resources.py
+-rw-r--r--   0 zagy       (501) staff       (20)     2630 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_template.py
+-rw-r--r--   0 zagy       (501) staff       (20)    16458 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_utils.py
+-rw-r--r--   0 zagy       (501) staff       (20)     1169 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/tests/test_vfs.py
+-rw-r--r--   0 zagy       (501) staff       (20)    19590 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/utils.py
+-rw-r--r--   0 zagy       (501) staff       (20)        8 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/version.txt
+-rw-r--r--   0 zagy       (501) staff       (20)     1009 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou/vfs.py
+drwxr-xr-x   0 zagy       (501) staff       (20)        0 2024-04-19 05:17:23.101489 batou-2.5.0b1/src/batou.egg-info/
+-rw-r--r--   0 zagy       (501) staff       (20)     3973 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou.egg-info/PKG-INFO
+-rw-r--r--   0 zagy       (501) staff       (20)     6900 2024-04-19 05:17:23.000000 batou-2.5.0b1/src/batou.egg-info/SOURCES.txt
+-rw-r--r--   0 zagy       (501) staff       (20)        1 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou.egg-info/dependency_links.txt
+-rw-r--r--   0 zagy       (501) staff       (20)      220 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou.egg-info/entry_points.txt
+-rw-r--r--   0 zagy       (501) staff       (20)        1 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou.egg-info/not-zip-safe
+-rw-r--r--   0 zagy       (501) staff       (20)      184 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou.egg-info/requires.txt
+-rw-r--r--   0 zagy       (501) staff       (20)        6 2024-04-19 05:17:22.000000 batou-2.5.0b1/src/batou.egg-info/top_level.txt
```

### Comparing `batou-2.4rc2/CHANGES.history.txt` & `batou-2.5.0b1/CHANGES.history.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/LICENSE.txt` & `batou-2.5.0b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/PKG-INFO` & `batou-2.5.0b1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: batou
-Version: 2.4rc2
-Summary: A utility for automating multi-host, multi-environment software builds and deployments.
-Home-page: https://batou.readthedocs.io/en/latest/
-Author: Christian Theune
-Author-email: ct@flyingcircus.io
-License: BSD (2-clause)
-Keywords: deployment
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE.txt
-
 <img width="150" src="https://batou.readthedocs.io/en/latest/_static/batou.png">
 
 batou helps you to automate your application deployments:
 
 * You create a model of your deployment using a simple but powerful Python API.
 * You configure how the model applies to hosts in different environments.
 * You verify and run the deployment with the batou utility.
@@ -96,15 +74,16 @@
 ## License
 
 The project is licensed under the 2-clause BSD license.
 
 ## Hacking
 
 * Make sure `mercurial` and `subversion` are installed and in `$PATH`.
-* `python27` also needs to be installed and in `$PATH`.
 * Run `./develop.sh` to create a local virtualenv with everything set up.
 * Run the test suite using: `bin/tox`
 * Build the documentation using: `cd doc; make`
 * Set up GPG for the examples with `export GNUPGHOME=<DIRECTORY OF BATOU HERE>/src/batou/secrets/tests/fixture/gnupg`
+* Make sure [age](https://github.com/FiloSottile/age) is installed and in `$PATH` for age encryption support.
+
 ## Changelog
 
 See [CHANGES.md](./CHANGES.md).
```

### Comparing `batou-2.4rc2/doc/source/api/component.txt` & `batou-2.5.0b1/doc/source/api/component.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/doc/source/api/environment.txt` & `batou-2.5.0b1/doc/source/api/environment.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/doc/source/cli/index.txt` & `batou-2.5.0b1/doc/source/cli/index.txt`

 * *Files 3% similar despite different names*

```diff
@@ -131,7 +131,23 @@
       keyid                 The user's key ID or email address
 
     optional arguments:
       -h, --help            show this help message and exit
       --environments ENVIRONMENTS
                             The environments to update. Update all if not
                             specified.
+
+batou secrets reencrypt
+-----------------------
+
+Re-encrypt all secrets with the current set of keys. This is useful when
+you want to update the set of public keys fetched from a key server.
+
+.. code-block:: console
+
+    usage: batou secrets reencrypt [-h] [--environments ENVIRONMENTS]
+
+    optional arguments:
+      -h, --help            show this help message and exit
+      --environments ENVIRONMENTS
+                            The environments to update. Update all if not
+                            specified.
```

### Comparing `batou-2.4rc2/doc/source/components/cmmi.txt` & `batou-2.5.0b1/doc/source/components/cmmi.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/doc/source/components/downloads-vcs.txt` & `batou-2.5.0b1/doc/source/components/downloads-vcs.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/doc/source/components/files.txt` & `batou-2.5.0b1/doc/source/components/files.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/doc/source/components/python.txt` & `batou-2.5.0b1/doc/source/components/python.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/doc/source/components/services.txt` & `batou-2.5.0b1/doc/source/components/services.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/doc/source/dev/authors.txt` & `batou-2.5.0b1/doc/source/dev/authors.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/doc/source/dev/contributing.txt` & `batou-2.5.0b1/doc/source/dev/contributing.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/doc/source/dev/testing.txt` & `batou-2.5.0b1/doc/source/dev/testing.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/doc/source/dev/todo.txt` & `batou-2.5.0b1/doc/source/dev/todo.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/doc/source/index.txt` & `batou-2.5.0b1/doc/source/index.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/doc/source/upgrading.txt` & `batou-2.5.0b1/doc/source/upgrading.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/doc/source/user/advanced.txt` & `batou-2.5.0b1/doc/source/user/advanced.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/doc/source/user/install.txt` & `batou-2.5.0b1/doc/source/user/install.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/doc/source/user/installation-deb.txt` & `batou-2.5.0b1/doc/source/user/installation-deb.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/doc/source/user/installation-rpm.txt` & `batou-2.5.0b1/doc/source/user/installation-rpm.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/doc/source/user/intro.txt` & `batou-2.5.0b1/doc/source/user/intro.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/doc/source/user/quickstart.txt` & `batou-2.5.0b1/doc/source/user/quickstart.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/examples/tutorial-secrets/environments/age/age_keys.txt` & `batou-2.5.0b1/examples/tutorial-secrets/environments/age/age_keys.txt`

 * *Files 15% similar despite different names*

```diff
@@ -6,20 +6,18 @@
 # encrypted (after a change).             #
 ###########################################
 # ssh key file from https://github.com/ctheune.keys
 ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIPYrVHEfF/DJzGyabfH/Bm9aJnKiTU827z5FPCQ7+utj
 # ssh key file from https://github.com/zagy.keys
 ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAII/V2m6ZLeYirvLbc5qGYbtBlRGLVbTUimUXIvfVdpvP
 # ssh key file from https://github.com/frlan.keys
-ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAACtwZOhqKCRHvdk8szRkjr79tTOjw2mIwwzz7mTDoexNUHWjDBqSXIXQbTEaBr9MWcCvVvzqB6Mk/IHlKXy5C2Qc0ycH7oMvcG/jg766jNS396J2j1OLEc3UM53YDQ/GrJWBWAOceb5o3rc/qz6+rl7Oqrnq+273iM8EmZF63esU5uY53SrL+3Hm1lgbnpO8DAA5HInindUyJMpnj/W640D+60qY76QoGMwnhU9aWWdgp2EkFEyYPbvMZYZnC18iiSk9qIAOkhNX1yXvhLJfXLX6eSz7YTTxAl7xelp0Ysuuzy2uejVYNEl1S14a8+aM04dN4gFh8K+lI9U8DdFuLENvtnyQ+3+s0P6aV6dRHjQAwF7q9kIOUZ2IVO9bBXoVimqQT8hL0/qMPaF4/Bmc8ffcmXEJkN7RhGUW8Xay4SPkbES73Lupc+WPSDOlAdRbEMI6gIHmXgYwuAlk8lT+CuBB4ljjiZUMwBfS3I8gCmfNHZN+Ip9fdO5QSiZoaflZ51P8wNgcMXID7/1aZpREOQnDqQpqzUoY82lZ3GMfWaZS8f8CGr9tayXz/vK3/W0TIirE6Gnq1ccUAzYcPXFhaWJtpudLzCkwCeVLqrQB8MGoaDEXVKjYMuSzMy70xlUGmI8ryJhXqMNHJjpfjgsGzlzzBZEZMwrO6SgDpX5BtzBDJC4gJw+QRBcomD2JT1VE/QCO9MOKgWuuhkA7DJ3Raq+b1e7enoXqyvrUB/8pO79MfDDJmgu2IcHswhx6Cp6mxsTTORi74x3IE7fz9ctZUJjQCeKqa9hYf7YF01nOzlRxWU7MaPjIrf4vdYaStZtSwVg2g9L2/TqQr9RUsPcDp9MACM8KEn4mz0uHAXxNsw0WwyqzM7MryL7U7mYLLmykGsgqd2tFlQQ8WmX9CgQbVOjf+imEXR6fwh
 ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIFFa6yqU0JuPZ3mtN1EVDUvaf9/IYBQQC2GJFuX5+ucO
+ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAACtwZOhqKCRHvdk8szRkjr79tTOjw2mIwwzz7mTDoexNUHWjDBqSXIXQbTEaBr9MWcCvVvzqB6Mk/IHlKXy5C2Qc0ycH7oMvcG/jg766jNS396J2j1OLEc3UM53YDQ/GrJWBWAOceb5o3rc/qz6+rl7Oqrnq+273iM8EmZF63esU5uY53SrL+3Hm1lgbnpO8DAA5HInindUyJMpnj/W640D+60qY76QoGMwnhU9aWWdgp2EkFEyYPbvMZYZnC18iiSk9qIAOkhNX1yXvhLJfXLX6eSz7YTTxAl7xelp0Ysuuzy2uejVYNEl1S14a8+aM04dN4gFh8K+lI9U8DdFuLENvtnyQ+3+s0P6aV6dRHjQAwF7q9kIOUZ2IVO9bBXoVimqQT8hL0/qMPaF4/Bmc8ffcmXEJkN7RhGUW8Xay4SPkbES73Lupc+WPSDOlAdRbEMI6gIHmXgYwuAlk8lT+CuBB4ljjiZUMwBfS3I8gCmfNHZN+Ip9fdO5QSiZoaflZ51P8wNgcMXID7/1aZpREOQnDqQpqzUoY82lZ3GMfWaZS8f8CGr9tayXz/vK3/W0TIirE6Gnq1ccUAzYcPXFhaWJtpudLzCkwCeVLqrQB8MGoaDEXVKjYMuSzMy70xlUGmI8ryJhXqMNHJjpfjgsGzlzzBZEZMwrO6SgDpX5BtzBDJC4gJw+QRBcomD2JT1VE/QCO9MOKgWuuhkA7DJ3Raq+b1e7enoXqyvrUB/8pO79MfDDJmgu2IcHswhx6Cp6mxsTTORi74x3IE7fz9ctZUJjQCeKqa9hYf7YF01nOzlRxWU7MaPjIrf4vdYaStZtSwVg2g9L2/TqQr9RUsPcDp9MACM8KEn4mz0uHAXxNsw0WwyqzM7MryL7U7mYLLmykGsgqd2tFlQQ8WmX9CgQbVOjf+imEXR6fwh
 # ssh key file from https://github.com/chrschm.keys
-ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIFbIH7V91cNn6vBTVWrTkyMP9pmYVF0eJsWWy0lEOWJD
+ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAILxEP3GtxYFY5vQkY7qYf7J8BKLg2sTwV4oy97mJb2Qf
 # ssh key file from https://github.com/nichmoe.keys
 ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIN73G31DK8s8C/Z7UNFiGg5+05mYfdexhjFafl7z33yH
 # ssh key file from https://github.com/elikoga.keys
-ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIEO9rt2tmkMNPVhhKNrwSHSrZH632rbqrEzRVfCQO0gn
 ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIKhg8pee2fZwv6ADydB9Lxa2xjmJlbwUESFIILyh9PZ+
-ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIEF+8v7VDSypngMnG/wPSQKl8jg3WBnSZpRfiHJh7ce0
 ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAINp4T6ndjaJKZfGnvl+xNoNMsZ7hXmsblRulj8ILLI5e
 # plain ssh public key
 ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIACZ8++sQADp8fztgumfw2i+WSgzMHB7MgSpkM2y5pHi batou-ci-test-key
```

### Comparing `batou-2.4rc2/setup.py` & `batou-2.5.0b1/setup.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/__init__.py` & `batou-2.5.0b1/src/batou/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,54 @@
 # This code must not cause non-stdlib imports to support self-bootstrapping.
 import os
 import os.path
+import socket
 import traceback
 from typing import List, Optional
 
+import jinja2
+
 from ._output import output
 
 with open(os.path.dirname(__file__) + "/version.txt") as f:
     __version__ = f.read().strip()
 
 # Configure `remote-pdb` to be used with `breakpoint()` in Python 3.7+:
 os.environ["PYTHONBREAKPOINT"] = "remote_pdb.set_trace"
 if not os.environ.get("REMOTE_PDB_HOST", None):
     os.environ["REMOTE_PDB_HOST"] = "127.0.0.1"
 if not os.environ.get("REMOTE_PDB_PORT", None):
     os.environ["REMOTE_PDB_PORT"] = "4444"
 
 
+def prepare_error(error):
+    return f"{error.__class__.__name__}: {error}"
+
+
+def prepare_traceback(tb):
+    from batou import component, environment
+
+    stack = traceback.extract_tb(tb)
+    while stack:
+        # Delete remoting-internal stack frames.'
+        line = stack.pop(0)
+        if line[0] in [
+            "<string>",
+            "<remote exec>",
+            environment.__file__.rstrip("c"),
+            component.__file__.rstrip("c"),
+        ]:
+            continue
+        stack.insert(0, line)
+        break
+    if not stack:
+        return "<no-non-remote-internal-traceback-lines-found>"
+    return "".join(traceback.format_list(stack))
+
+
 class ReportingException(Exception):
     """Exceptions that support user-readable reporting."""
 
     affected_hostname: Optional[str]
 
     def __str__(self):
         raise NotImplementedError()
@@ -134,14 +162,36 @@
     def report(self):
         output.error("Error while calling age")
         output.tabular("command", self.command, red=True)
         output.tabular("exit code", self.exitcode)
         output.tabular("message", self.output, separator=":\n")
 
 
+class GetAddressInfoError(ReportingException, socket.gaierror):
+    """There was an error calling getaddrinfo."""
+
+    hostname: str
+    error: str
+
+    @classmethod
+    def from_context(cls, hostname, error):
+        self = cls()
+        self.hostname = hostname
+        self.error = error
+        return self
+
+    def __str__(self):
+        return f"Error while resolving {self.hostname}: {self.error}"
+
+    def report(self):
+        output.error("Error while resolving hostname")
+        output.tabular("hostname", self.hostname, red=True)
+        output.tabular("message", self.error, separator=":\n")
+
+
 class UpdateNeeded(AssertionError):
     """A component requires an update."""
 
 
 class ConfigurationError(ReportingException):
     """Indicates that an environment could not be configured successfully."""
 
@@ -171,14 +221,58 @@
             message = "{}: {}".format(
                 self.component_root_name,
                 message,
             )
         output.error(message)
 
 
+class AttributeExpansionError(ConfigurationError):
+    """An override attribute could not be expanded properly."""
+
+    component_breadcrumbs: str
+    value_repr: str
+    error_str: str
+    key: str
+
+    @property
+    def sort_key(self):
+        return (
+            1,
+            self.affected_hostname,
+            self.component_breadcrumbs,
+            self.key,
+        )
+
+    @classmethod
+    def from_context(cls, component, key, value, error):
+        self = cls()
+        self.affected_hostname = component.root.host.name
+        self.component_breadcrumbs = component._breadcrumbs
+        self.value_repr = repr(value)
+        self.error = prepare_error(error)
+        self.key = key
+        return self
+
+    def __str__(self):
+        return "Error while expanding attribute: " + self.error
+
+    def report(self):
+        output.error("Error while expanding attribute:")
+        output.tabular(
+            "Message",
+            self.error,
+            red=True,
+        )
+        output.tabular(
+            "Attribute",
+            "{}.{}".format(self.component_breadcrumbs, self.key),
+            red=True,
+        )
+
+
 class ConversionError(ConfigurationError):
     """An override attribute could not be converted properly."""
 
     component_breadcrumbs: str
     conversion_name: str
     value_repr: str
     error_str: str
@@ -230,15 +324,14 @@
     They basically only influence control flow during configuration and
     are manually placed to avoid double reporting.
 
     """
 
 
 class MissingOverrideAttributes(ConfigurationError):
-
     component_breadcrumbs: str
     attributes: List[str]
 
     @property
     def sort_key(self):
         return (3, self.affected_hostname, self.component_breadcrumbs)
 
@@ -324,31 +417,19 @@
         return (4, self.root_host_name, 2)
 
     @classmethod
     def from_context(cls, root, exception, tb):
         self = cls()
         self.root_name = root.name
         self.root_host_name = root.host.name
-        self.exception_repr = repr(exception)
+        self.exception_repr = prepare_error(exception)
         stack = traceback.extract_tb(tb)
         from batou import component, environment
 
-        while True:
-            # Delete remoting-internal stack frames.'
-            line = stack.pop(0)
-            if line[0] in [
-                "<string>",
-                "<remote exec>",
-                environment.__file__.rstrip("c"),
-                component.__file__.rstrip("c"),
-            ]:
-                continue
-            stack.insert(0, line)
-            break
-        self.traceback = "".join(traceback.format_list(stack))
+        self.traceback = prepare_traceback(tb)
         return self
 
     def __str__(self):
         return self.exception_repr
 
     def report(self):
         output.error(self.exception_repr)
@@ -442,27 +523,34 @@
 
 class ComponentLoadingError(ConfigurationError):
     """The specified component file failed to load."""
 
     sort_key = (0,)
 
     @classmethod
-    def from_context(cls, filename, exception):
+    def from_context(cls, filename, exception, tb):
         self = cls()
         self.filename = filename
         self.exception_str = str(exception)
+
+        self.traceback = prepare_traceback(tb)
         return self
 
     def __str__(self):
         return "Failed loading component file " + self.filename
 
     def report(self):
         output.error("Failed loading component file")
         output.tabular("File", self.filename, red=True)
         output.tabular("Exception", self.exception_str, red=True)
+        output.annotate(
+            "Traceback (simplified, most recent call last):", red=True
+        )
+        output.annotate(self.traceback, red=True)
+
         # TODO provide traceback in debug output
         # see: https://github.com/flyingcircusio/batou/issues/316
 
 
 class MissingComponent(ConfigurationError):
     """The specified environment does not exist."""
 
@@ -728,15 +816,14 @@
     def report(self):
         output.error(
             "Duplicate definition of host: {}".format(self.affected_hostname)
         )
 
 
 class InvalidIPAddressError(ConfigurationError):
-
     sort_key = (0,)
 
     @classmethod
     def from_context(cls, address):
         self = cls()
         self.address = address
         return self
@@ -774,7 +861,33 @@
             f"Use `require_v{self.kind}=True` when instantiating the Address"
             " object.",
             red=True,
         )
 
         # TODO provide traceback/line numbers/excerpt
         # see: https://github.com/flyingcircusio/batou/issues/316
+
+
+class TemplatingError(ReportingException):
+    """An error occured while rendering a template."""
+
+    sort_key = (0,)
+
+    @classmethod
+    def from_context(cls, exception, template_identifier):
+        self = cls()
+        self.exception_str = prepare_error(exception)
+        self.template_identifier = template_identifier
+        # if exception is instance of jinja2.TemplateSyntaxError
+        # there is some magic in jinja2 that makes the __str__ method
+        # less capable, if exception.translated is set to True
+        if isinstance(exception, jinja2.TemplateSyntaxError):
+            exception.translated = False
+            self.exception_str = str(exception)
+            exception.translated = True
+        return self
+
+    def __str__(self):
+        return f"An error occured while rendering a template ({self.template_identifier}): {self.exception_str}"
+
+    def report(self):
+        output.error(str(self))
```

### Comparing `batou-2.4rc2/src/batou/_output.py` & `batou-2.5.0b1/src/batou/_output.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/component.py` & `batou-2.5.0b1/src/batou/component.py`

 * *Files 2% similar despite different names*

```diff
@@ -1146,27 +1146,28 @@
         # be applied, use the following pattern:
         #
         # attribute = getattr(self.__class__, key, None)
         # if isinstance(attribute, Attribute):
         #     value = attribute.from_config_string(self, value)
         # setattr(self, key, value)
         #
-        if self.expand:
-            value = obj.expand(value)
+        try:
+            if self.expand:
+                value = obj.expand(value)
+        except Exception as e:
+            name = self.names.get(obj.__class__, "<unknown>")
+            raise batou.AttributeExpansionError.from_context(
+                obj, name, value, e
+            ) from e
         if self.map:
             value = obj.map(value)
         try:
             value = self.conversion(value)
         except Exception as e:
-            # Try to detect our own name.
-            name = "<unknown>"
-            for k in dir(obj):
-                if getattr(obj.__class__, k, None) is self:
-                    name = k
-                    break
+            name = self.names.get(obj.__class__, "<unknown>")
             raise batou.ConversionError.from_context(
                 obj, name, value, self.conversion, e
             )
         return value
 
     def __set__(self, obj, value):
         self.instances[obj] = value
```

### Comparing `batou-2.4rc2/src/batou/conftest.py` & `batou-2.5.0b1/src/batou/conftest.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/deploy.py` & `batou-2.5.0b1/src/batou/deploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 import random
 import sys
 import threading
 import time
 import traceback
 from concurrent.futures import ThreadPoolExecutor
 
-from batou import ReportingException, SilentConfigurationError
+from batou import (
+    ConfigurationError,
+    ReportingException,
+    SilentConfigurationError,
+)
 from batou._output import TerminalBackend, output
 
 from .environment import Environment
 from .utils import Timer, locked, notify, self_id
 
 
 class Connector(threading.Thread):
@@ -94,28 +98,26 @@
     def __str__(self):
         return "{} DeploymentError(s): {}".format(
             len(self.errors), ", ".join(str(e) for e in self.errors)
         )
 
 
 class Deployment(object):
-
     _upstream = None
 
     def __init__(
         self,
         environment,
         platform,
         timeout,
         dirty,
         jobs,
         predict_only=False,
         provision_rebuild=False,
     ):
-
         self.environment = Environment(
             environment, timeout, platform, provision_rebuild=provision_rebuild
         )
         self.environment.deployment = self
 
         self.dirty = dirty
         self.predict_only = predict_only
@@ -201,14 +203,19 @@
         all_reporting_hostnames = set()
         for c in self.connections:
             errors = pickle.loads(c.errors)
             reporting_hostname = c.host.name
             all_reporting_hostnames.add(reporting_hostname)
             all_errors.extend([(reporting_hostname, e) for e in errors])
             # collects all errors into (reporting_hostname, error) tuples
+        # if there are no connections, then we append a ConfigurationError
+        if not self.connections:
+            raise ConfigurationError.from_context(
+                "No host found in environment."
+            )
         # if there are no errors, we're done
         if not all_errors:
             return
         # collect with .should_merge
         errors_by_equivalence_class = []
         for hostname, error in all_errors:
             # check wether it fits into an existing equivalence class
```

### Comparing `batou-2.4rc2/src/batou/environment.py` & `batou-2.5.0b1/src/batou/environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,23 +158,22 @@
     @classmethod
     def all(cls):
         for path in pathlib.Path("environments").glob("*/environment.cfg"):
             yield cls(path.parent.name)
 
     @classmethod
     def filter(cls, filter):
-        if filter:
-            filter = filter.split(",")
+        if not filter:
+            return list(cls.all())
+        filter = filter.split(",")
         environments = []
         for e in cls.all():
-            if filter:
-                if e.name in filter:
-                    filter.remove(e.name)
-                else:
-                    continue
+            if e.name not in filter:
+                continue
+            filter.remove(e.name)
             environments.append(e)
         if filter:
             raise UnknownEnvironmentError(filter)
         return environments
 
     def _environment_path(self, path="."):
         return os.path.abspath(
@@ -211,16 +210,17 @@
         # Scan all components
         for filename in sorted(
             glob.glob(os.path.join(self.base_dir, "components/*/component.py"))
         ):
             try:
                 self.components.update(load_components_from_file(filename))
             except Exception as e:
+                exc_type, ex, tb = sys.exc_info()
                 self.exceptions.append(
-                    ComponentLoadingError.from_context(filename, e)
+                    ComponentLoadingError.from_context(filename, e, tb)
                 )
 
         config = Config(config_file)
 
         self.load_environment(config)
         self.load_provisioners(config)
         self.load_hosts(config)
```

### Comparing `batou-2.4rc2/src/batou/fixtures.py` & `batou-2.5.0b1/src/batou/fixtures.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/host.py` & `batou-2.5.0b1/src/batou/host.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/appenv.py` & `batou-2.5.0b1/src/batou/lib/appenv.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/archive.py` & `batou-2.5.0b1/src/batou/lib/archive.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/buildout.py` & `batou-2.5.0b1/src/batou/lib/buildout.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/cmmi.py` & `batou-2.5.0b1/src/batou/lib/cmmi.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/cron.py` & `batou-2.5.0b1/src/batou/lib/cron.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/debian.py` & `batou-2.5.0b1/src/batou/lib/debian.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/download.py` & `batou-2.5.0b1/src/batou/lib/download.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/file.py` & `batou-2.5.0b1/src/batou/lib/file.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,24 +13,48 @@
 import yaml
 
 import batou
 from batou import output
 from batou.component import Attribute, Component
 from batou.utils import dict_merge
 
+# Explain the logic that in a multi-user and concurrent system there isn't really a coarse grained guarantee around files not existing.
+
+# What this can guarantee, however, is that during the lifetime of this function call, there will have been an atomic moment where the file did not exist, or, if it existed and can not be removed, it will raise an error.
+
+# This means: if the file wasn't there in the first place, we're fine. If the file existed and we removed it, we are fine, we don't care whether someone else might have recreated it immediately after. If the file existed and was removed by someone else, we don't care either. If the file existed and we can't remove it, we need to fail.
+
+
+def ensure_path_nonexistent(path: str) -> None:
+    """Ensure that the given path does not exist.
+
+    In a multi-user/concurrent environment, it is possible that a path is created
+    at any time. This function will ensure that the path does not exist at some
+    point in time during the execution of this function.
+
+    During the lifetime of this function call, there will have been an atomic
+    moment where the file did not exist, or, if it existed and can not be
+    removed, it will raise an error.
+
+    This function will not guarantee that the path does not exist after this
+    function has returned.
+    """
 
-def ensure_path_nonexistent(path):
     if not os.path.lexists(path):
         return
-    if os.path.islink(path):
-        os.unlink(path)
-    elif os.path.isdir(path):
-        shutil.rmtree(path)
-    else:
-        os.unlink(path)
+
+    parent_dir = os.path.dirname(os.path.abspath(path))
+    path_basename = os.path.basename(os.path.normpath(path))
+
+    with tempfile.TemporaryDirectory(dir=parent_dir) as temp_dir:
+        try:
+            os.rename(path, os.path.join(temp_dir, path_basename))
+        except FileNotFoundError as e:
+            # The file was not there in the first place, we're done.
+            pass
 
 
 class File(Component):
 
     namevar = "path"
 
     ensure = "file"  # or: directory, symlink
@@ -200,14 +224,17 @@
     @property
     def exclude_arg(self):
         if not self.exclude:
             return ""
         return " ".join("--exclude '{}'".format(x) for x in self.exclude) + " "
 
     def verify(self):
+        if not os.path.isdir(self.path):
+            raise batou.UpdateNeeded()
+
         stdout, stderr = self.cmd(
             "rsync {} {}{}/ {}".format(
                 self.verify_opts, self.exclude_arg, self.source, self.path
             )
         )
 
         # In case of we see non-convergent rsync runs
@@ -237,21 +264,30 @@
 class Directory(Component):
 
     namevar = "path"
     leading = False
     source = None
     exclude = ()
 
+    verify_opts = None
+    sync_opts = None
+
     def configure(self):
         self.path = self.map(self.path)
         if self.source:
             # XXX The ordering is wrong. SyncDirectory should run *after*.
-            self += SyncDirectory(
-                self.path, source=self.source, exclude=self.exclude
-            )
+            args = {
+                "source": self.source,
+                "exclude": self.exclude,
+            }
+            if self.verify_opts:
+                args["verify_opts"] = self.verify_opts
+            if self.sync_opts:
+                args["sync_opts"] = self.sync_opts
+            self += SyncDirectory(self.path, **args)
 
     def verify(self):
         assert os.path.isdir(self.path)
 
     def update(self):
         ensure_path_nonexistent(self.path)
         if self.leading:
```

### Comparing `batou-2.4rc2/src/batou/lib/git.py` & `batou-2.5.0b1/src/batou/lib/git.py`

 * *Files 15% similar despite different names*

```diff
@@ -172,15 +172,28 @@
             self.cmd("git submodule update --init --recursive")
 
     def untracked_files(self):
         stdout, stderr = self.cmd(
             "git status --porcelain --untracked-files=all"
         )
         items = (line.split(None, 1) for line in stdout.splitlines())
-        return [filepath for status, filepath in items if status == "??"]
+        untracked_items = [
+            filepath for status, filepath in items if status == "??"
+        ]
+
+        # from the manpage of git-status: If a filename contains whitespace
+        # or other nonprintable characters, that field will be quoted
+        # in the manner of a C string literal
+        # so we need to unquote the filenames
+        def unquote_git(s):
+            if s.startswith('"') and s.endswith('"'):
+                return s[1:-1].encode().decode("unicode-escape")
+            return s
+
+        return [unquote_git(item) for item in untracked_items]
 
     def last_updated(self):
         with self.chdir(self.target):
             if not os.path.exists(".git"):
                 return None
             stdout, stderr = self.cmd("git show -s --format=%ct")
             timestamp = stdout.strip()
```

### Comparing `batou-2.4rc2/src/batou/lib/goceptnet.py` & `batou-2.5.0b1/src/batou/lib/goceptnet.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/logrotate.py` & `batou-2.5.0b1/src/batou/lib/logrotate.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/mercurial.py` & `batou-2.5.0b1/src/batou/lib/mercurial.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/mysql.py` & `batou-2.5.0b1/src/batou/lib/mysql.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/nagios.py` & `batou-2.5.0b1/src/batou/lib/nagios.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/package.py` & `batou-2.5.0b1/src/batou/lib/package.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/python.py` & `batou-2.5.0b1/src/batou/lib/python.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/resources/check_supervisor.py.in` & `batou-2.5.0b1/src/batou/lib/resources/check_supervisor.py.in`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/resources/init.sh` & `batou-2.5.0b1/src/batou/lib/resources/init.sh`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/resources/nagios.cfg` & `batou-2.5.0b1/src/batou/lib/resources/nagios.cfg`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/resources/supervisor.conf` & `batou-2.5.0b1/src/batou/lib/resources/supervisor.conf`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/service.py` & `batou-2.5.0b1/src/batou/lib/service.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/supervisor.py` & `batou-2.5.0b1/src/batou/lib/supervisor.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/svn.py` & `batou-2.5.0b1/src/batou/lib/svn.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/tests/test_appenv.py` & `batou-2.5.0b1/src/batou/lib/tests/test_appenv.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/tests/test_archive.py` & `batou-2.5.0b1/src/batou/lib/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/tests/test_buildout.py` & `batou-2.5.0b1/src/batou/lib/tests/test_buildout.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/tests/test_cmmi.py` & `batou-2.5.0b1/src/batou/lib/tests/test_cmmi.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/tests/test_cron.py` & `batou-2.5.0b1/src/batou/lib/tests/test_cron.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/tests/test_debian.py` & `batou-2.5.0b1/src/batou/lib/tests/test_debian.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/tests/test_download.py` & `batou-2.5.0b1/src/batou/lib/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/tests/test_file.py` & `batou-2.5.0b1/src/batou/lib/tests/test_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     File,
     FileComponent,
     JSONContent,
     Mode,
     Presence,
     Purge,
     Symlink,
+    SyncDirectory,
     YAMLContent,
     ensure_path_nonexistent,
 )
 from batou.tests.ellipsis import Ellipsis
 
 
 def test_ensure_path_nonexistent_removes_normal_file(tmpdir):
@@ -1140,7 +1141,26 @@
 
 def test_purge_globs_and_deletes_files(root):
     os.mkdir("work/mycomponent/source-one")
     open("work/mycomponent/source-two", "w").close()
     root.component += Purge("sourc*")
     root.component.deploy()
     assert sorted(os.listdir("work/mycomponent")) == []
+
+
+def test_syncdirectory_needs_update_on_nonexisting_target(root):
+    os.mkdir("work/mycomponent/existing_dir")
+    open("work/mycomponent/existing_dir/test_file", "w").close()
+    with pytest.raises(batou.UpdateNeeded):
+        sd = SyncDirectory("non_existing_dir", source="existing_dir")
+        sd.verify()
+
+
+def test_directory_passes_args_to_syncdirectory(root):
+    d = Directory(
+        "target", source="source", verify_opts="-abc", sync_opts="-xyz"
+    )
+    d.prepare(root.component)
+    sd = d._
+    assert isinstance(sd, SyncDirectory)
+    assert sd.verify_opts == "-abc"
+    assert sd.sync_opts == "-xyz"
```

### Comparing `batou-2.4rc2/src/batou/lib/tests/test_git.py` & `batou-2.5.0b1/src/batou/lib/tests/test_git.py`

 * *Files 3% similar despite different names*

```diff
@@ -321,7 +321,28 @@
 def test_clone_into_workdir_works(root, repos_path, repos_path2):
     git = batou.lib.git.Clone(repos_path, branch="master")
     with open(root.component.map("asdf"), "w") as f:
         f.write("foo")
     root.component += git
     root.component.deploy()
     assert not os.path.exists(root.component.map("asdf"))
+
+
+@pytest.mark.slow
+def test_can_read_untracked_files_correctly(root, repos_path):
+    fun_strings = [
+        "this string has spaces in it",
+        "this string has a ' in it",
+        'this string has a " in it',
+        '"this string has a \' and a " in it"',
+        "this string has a \\ in it",
+        "this string has a \\ and a ' in it",
+        "this string has a \\ and a & in it",
+    ]
+    git = batou.lib.git.Clone(repos_path, branch="master")
+    root.component += git
+    root.component.deploy()
+    for s in fun_strings:
+        with open(root.component.map(s), "w") as f:
+            f.write(s)
+    with git.chdir(git.target):
+        assert set(git.untracked_files()) == set(fun_strings)
```

### Comparing `batou-2.4rc2/src/batou/lib/tests/test_mercurial.py` & `batou-2.5.0b1/src/batou/lib/tests/test_mercurial.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/tests/test_nagios.py` & `batou-2.5.0b1/src/batou/lib/tests/test_nagios.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/tests/test_python.py` & `batou-2.5.0b1/src/batou/lib/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/tests/test_service.py` & `batou-2.5.0b1/src/batou/lib/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/tests/test_supervisor.py` & `batou-2.5.0b1/src/batou/lib/tests/test_supervisor.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/lib/tests/test_svn.py` & `batou-2.5.0b1/src/batou/lib/tests/test_svn.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/main.py` & `batou-2.5.0b1/src/batou/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,14 +162,26 @@
     p.add_argument(
         "--environments",
         default="",
         help="The environments to update. Update all if not specified.",
     )
     p.set_defaults(func=batou.secrets.manage.remove_user)
 
+    p = sp.add_parser(
+        "reencrypt",
+        help="Re-encrypt all secret files with the current members.",
+    )
+    p.set_defaults(func=p.print_usage)
+    p.add_argument(
+        "--environments",
+        default="",
+        help="The environments to update. Update all if not specified.",
+    )
+    p.set_defaults(func=batou.secrets.manage.reencrypt)
+
     # migrate
     migrate = subparsers.add_parser(
         "migrate",
         help=textwrap.dedent(
             """
             Migrate the configuration to be compatible with the batou version
             used. Requires to commit the changes afterwards. Might show some
```

### Comparing `batou-2.4rc2/src/batou/migrate/__init__.py` & `batou-2.5.0b1/src/batou/migrate/__init__.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/migrate/migrations/2301.py` & `batou-2.5.0b1/src/batou/migrate/migrations/2301.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/migrate/migrations/2302.py` & `batou-2.5.0b1/src/batou/migrate/migrations/2302.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/migrate/migrations/2303.py` & `batou-2.5.0b1/src/batou/migrate/migrations/2303.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/migrate/migrations/2400.py` & `batou-2.5.0b1/src/batou/migrate/migrations/2400.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/migrate/tests/test_migrate.py` & `batou-2.5.0b1/src/batou/migrate/tests/test_migrate.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/provision.py` & `batou-2.5.0b1/src/batou/provision.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/remote_core.py` & `batou-2.5.0b1/src/batou/remote_core.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/repository.py` & `batou-2.5.0b1/src/batou/repository.py`

 * *Files 3% similar despite different names*

```diff
@@ -391,22 +391,29 @@
         else:
             head = head.decode("ascii")
             bundle_range = "{head}..{branch}".format(
                 head=head, branch=self.branch
             )
         fd, bundle_file = tempfile.mkstemp()
         os.close(fd)
-        out, err = cmd(
-            "git bundle create {file} {range}".format(
-                file=bundle_file, range=bundle_range
-            ),
-            acceptable_returncodes=[0, 128],
-        )
-        if "create empty bundle" in err:
-            return
+        try:
+            out, err = cmd(
+                "git bundle create {file} {range}".format(
+                    file=bundle_file, range=bundle_range
+                ),
+                acceptable_returncodes=[0],
+            )
+        except CmdExecutionError as e:
+            if (
+                e.returncode == 128
+                and "fatal: Refusing to create empty bundle." in e.stderr
+            ):
+                return
+            raise
+
         change_size = os.stat(bundle_file).st_size
         if change_size == 0:
             output.error("Created invalid bundle (0 bytes):")
             output.annotate(err, red=True)
             raise DeploymentError()
         output.annotate(
             "Sending {} bytes of changes".format(change_size), debug=True
```

### Comparing `batou-2.4rc2/src/batou/resources.py` & `batou-2.5.0b1/src/batou/resources.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/secrets/__init__.py` & `batou-2.5.0b1/src/batou/secrets/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     SuperfluousSecretsSection,
     UnknownHostSecretsSection,
 )
 from batou._output import output
 
 from .encryption import (
     AGEEncryptedFile,
+    DiffableAGEEncryptedFile,
     EncryptedFile,
     GPGEncryptedFile,
     NoBackingEncryptedFile,
     debug,
 )
 
 if TYPE_CHECKING:
@@ -77,14 +78,22 @@
             secret_provider_candidates.append(AGESecretProvider(environment))
         elif extension == ".gpg":
             output.annotate(
                 f"Found gpg secrets for environment {environment.name}.",
                 debug=True,
             )
             secret_provider_candidates.append(GPGSecretProvider(environment))
+        elif extension == ".age-diffable":
+            output.annotate(
+                f"Found age-diffable secrets for environment {environment.name}.",
+                debug=True,
+            )
+            secret_provider_candidates.append(
+                DiffableAGESecretProvider(environment)
+            )
         else:
             raise ValueError(
                 f"Invalid secret provider {extension}.",
             )
 
         return secret_provider_candidates[0]
 
@@ -173,15 +182,15 @@
         Edit the secrets.
         """
         raise NotImplementedError("edit() not implemented.")
 
     def write_file(self, file: EncryptedFile, content: bytes):
         raise NotImplementedError("write_file() not implemented.")
 
-    def write_config(self, content: bytes):
+    def write_config(self, content: bytes, force_reencrypt: bool = False):
         raise NotImplementedError("write_config() not implemented.")
 
     def write_config_new(self, content: bytes):
         raise NotImplementedError("write_config_new() not implemented.")
 
     def change_secret_provider(
         self,
@@ -189,40 +198,39 @@
         old_secret_provider: "SecretProvider",
     ):
         new_secret_provider_str = config.get("batou", "secret_provider").value
         if new_secret_provider_str == "age":
             new_secret_provider = AGESecretProvider(self.environment)
         elif new_secret_provider_str == "gpg":
             new_secret_provider = GPGSecretProvider(self.environment)
+        elif new_secret_provider_str == "age-diffable":
+            new_secret_provider = DiffableAGESecretProvider(self.environment)
         else:
             raise ValueError(
                 f"Invalid secret provider {new_secret_provider_str}.",
             )
         output.annotate(
-            f"Changing secret provider from {old_secret_provider.secret_provider_str()} to {new_secret_provider.secret_provider_str()}."
+            f"Changing secret provider from {old_secret_provider.secret_provider_str} to {new_secret_provider.secret_provider_str}."
         )
         new_secret_provider.write_config_new(str(config).encode("utf-8"))
         new_secret_provider.write_secret_files(
             old_secret_provider.read_secret_files()
         )
         self.environment.secret_provider = new_secret_provider
-        old_secret_provider.purge()
+        old_secret_provider.purge(new_secret_provider.iter_secret_files())
         output.annotate(
-            f"Secret provider changed from {old_secret_provider.secret_provider_str()} to {new_secret_provider.secret_provider_str()}."
+            f"Secret provider changed from {old_secret_provider.secret_provider_str} to {new_secret_provider.secret_provider_str}."
         )
 
-    def purge(self):
+    def purge(self, except_files: Dict[str, EncryptedFile] = {}):
         raise NotImplementedError("purge() not implemented.")
 
     def _get_recipients(self) -> List[str]:
         raise NotImplementedError("_get_recipients() not implemented.")
 
-    def secret_provider_str(self) -> str:
-        raise NotImplementedError("secret_provider_str() not implemented.")
-
 
 class SecretBlob:
     def __init__(
         self,
         host_data: Dict[str, Dict[str, str]],
         component_overrides: Dict[str, Dict[str, str]],
         secret_data: Set[str],
@@ -234,14 +242,16 @@
         self.host_data = host_data
         self.component_overrides = component_overrides
         self.secret_data = secret_data
         self.secret_files = secret_files
 
 
 class NoSecretProvider(SecretProvider):
+    secret_provider_str = "none"
+
     def __init__(self, environment: "Environment"):
         super().__init__(environment)
 
     def read(self):
         return SecretBlob({}, {}, set(), {})
 
     def summary(self):
@@ -254,32 +264,29 @@
         )
         if edit_file is not None:
             raise ValueError(
                 "Cannot edit secret files for environment without secret configuration.",
             )
         return NoBackingEncryptedFile()
 
-    def write_config(self, content: bytes):
+    def write_config(self, content: bytes, force_reencrypt: bool = False):
         output.annotate(
             f"Writing secrets configuration for environment {self.environment.name} without secret configuration.",
             debug=True,
         )
         self.change_secret_provider(
             ConfigUpdater().read_string(content.decode("utf-8")), self
         )
 
     def read_secret_files(self) -> Dict[str, bytes]:
         return {}
 
-    def purge(self):
+    def purge(self, except_files: Dict[str, EncryptedFile] = {}):
         pass
 
-    def secret_provider_str(self) -> str:
-        return "none"
-
 
 class ConfigFileSecretProvider(SecretProvider):
     config_file: EncryptedFile
 
     @property
     def config(self):
         return ConfigUpdater().read_string(self.config_file.cleartext)
@@ -329,17 +336,18 @@
         return secret_files
 
     def write_secret_files(self, secret_files: Dict[str, bytes]):
         for name, content in secret_files.items():
             with self._get_file(name, writeable=True) as file:
                 self.write_file(file, content)
 
-    def purge(self):
-        for file in self.iter_secret_files(writeable=True).values():
-            file.delete()
+    def purge(self, except_files: Dict[str, EncryptedFile] = {}):
+        for name, file in self.iter_secret_files(writeable=True).items():
+            if name not in except_files:
+                file.delete()
         self.config_file.delete()
 
     def summary(self):
         print("\t members")
         with self.config_file:
             members = self.config.get("batou", "members")
             if members.value is not None:
@@ -368,29 +376,40 @@
         else:
             return self._get_file(edit_file, writeable=True)
 
     def _get_file(self, name: str, writeable: bool) -> EncryptedFile:
         raise NotImplementedError("_get_file() not implemented.")
 
     def write_file(self, file: EncryptedFile, content: bytes):
-        recipients = self._get_recipients()
+        recipients = self._get_recipients_for_encryption()
         if not recipients:
             raise ValueError(
                 "No recipients found for environment. "
                 "Please add a 'batou.members' section to the secrets file."
             )
         file.write(content, recipients)
 
     def write_config_new(self, content: bytes):
         self.config_file.writeable = True
         with self.config_file:
             self.write_config(content)
 
+    def _get_recipients(self) -> List[str]:
+        recipients = self.config.get("batou", "members")
+
+        if recipients.value is None:
+            return []
+        recipients = re.split(r"(\n|,)+", recipients.value)
+        recipients = [r.strip() for r in recipients if r.strip()]
+        return recipients
+
 
 class GPGSecretProvider(ConfigFileSecretProvider):
+    secret_provider_str = "gpg"
+
     def __init__(self, environment: "Environment"):
         super().__init__(environment)
         # load encrypted file
         self.config_file = GPGEncryptedFile(
             pathlib.Path(environment.base_dir)
             / "environments"
             / environment.name
@@ -417,23 +436,18 @@
             pathlib.Path(self.environment.base_dir)
             / "environments"
             / self.environment.name
             / f"secret-{name}.gpg",
             writeable,
         )
 
-    def _get_recipients(self) -> List[str]:
-        recipients = self.config.get("batou", "members")
-        if recipients.value is None:
-            return []
-        recipients = re.split(r"(\n|,)+", recipients.value)
-        recipients = [r.strip() for r in recipients if r.strip()]
-        return recipients
+    def _get_recipients_for_encryption(self) -> List[str]:
+        return self._get_recipients()
 
-    def write_config(self, content: bytes):
+    def write_config(self, content: bytes, force_reencrypt: bool = False):
         config = ConfigUpdater().read_string(content.decode("utf-8"))
         secret_provider = config.get("batou", "secret_provider", fallback=None)
         if secret_provider is None or secret_provider.value is None:
             config.set("batou", "secret_provider", "gpg")
             print("Setting secret provider to gpg.")
         secret_provider = config.get("batou", "secret_provider")
         if secret_provider.value != "gpg":
@@ -449,20 +463,18 @@
         if not recipients or len(recipients) == 0 or recipients[0] == "":
             raise ValueError(
                 "Please add at least one recipient to the secrets file."
             )
         self.config_file.write(
             str(config).encode("utf-8"),
             recipients,
+            reencrypt=force_reencrypt,
         )
         self.write_secret_files(self.read_secret_files())
 
-    def secret_provider_str(self) -> str:
-        return "gpg"
-
 
 def process_age_recipients(members, environment_path):
     """Process the recipients list."""
     key_meta_file_path = os.path.join(
         environment_path,
         "age_keys.txt",
     )
@@ -494,48 +506,60 @@
                     "Downloading public keys over http is insecure!"
                 )
             key_meta_file_content += f"# ssh key file from {key}\n"
             if debug:
                 print(f"Downloading key file from `{key}`")
             key_file = urllib.request.urlopen(key)
             key_file_content = key_file.read().decode("utf-8")
-            for line in key_file_content.splitlines():
-                if line.startswith("ssh-"):
-                    new_members.append(line)
-                    key_meta_file_content += f"{line}\n"
+            remote_keys = sorted(
+                [
+                    line
+                    for line in key_file_content.splitlines()
+                    if line.startswith("ssh-")
+                ]
+            )
+            for line in remote_keys:
+                new_members.append(line)
+                key_meta_file_content += f"{line}\n"
         else:
             # unknown key type
             print(f"WARNING: Unknown key type for {key}\nWill be ignored!")
     # compare key_meta_file_content and the old one
     # if they differ, we will warn
+    keys_changed = False
     if os.path.exists(key_meta_file_path):
         with open(key_meta_file_path, "r") as f:
             old_key_meta_file_content = f.read()
         if old_key_meta_file_content != key_meta_file_content:
+            keys_changed = True
             print(
                 "WARNING: The age encryption public-key metadata file has changed!\n"
                 "This means that some secrets are now encrypted with a different set of keys.\n"
                 "Please make sure that the new keys are correct and check the file in once you are done."
             )
     else:
+        keys_changed = True
         print(
             "WARNING: The age encryption public-key metadata file does not exist!\n"
             "This is not a problem if you are setting up the environment for the first time.\n"
             "Please make sure that the new keys are correct and check the file in once you are done."
         )
     # write the new key meta file
     with open(key_meta_file_path, "w") as f:
         f.write(key_meta_file_content)
-    return new_members
+    return new_members, keys_changed
 
 
 class AGESecretProvider(ConfigFileSecretProvider):
+    FileFactory = AGEEncryptedFile
+    secret_provider_str = "age"
+
     def __init__(self, environment: "Environment"):
         super().__init__(environment)
-        self.config_file = AGEEncryptedFile(
+        self.config_file = self.FileFactory(
             pathlib.Path(environment.base_dir)
             / "environments"
             / environment.name
             / "secrets.cfg.age"
         )
 
     def iter_secret_files(self, writeable=False) -> Dict[str, EncryptedFile]:
@@ -558,55 +582,64 @@
             pathlib.Path(self.environment.base_dir)
             / "environments"
             / self.environment.name
             / f"secret-{name}.age",
             writeable,
         )
 
-    def _get_recipients(self) -> List[str]:
-        recipients = self.config.get("batou", "members")
-        if recipients.value is None:
-            return []
-        recipients = re.split(r"(\n|,)+", recipients.value)
-        recipients = [r.strip() for r in recipients if r.strip()]
+    def _get_recipients_for_encryption(self) -> List[str]:
+        recipients = self._get_recipients()
         return process_age_recipients(
             recipients,
             pathlib.Path(self.environment.base_dir)
             / pathlib.Path("environments")
             / self.environment.name,
-        )
+        )[0]
 
-    def write_config(self, content: bytes):
+    def write_config(self, content: bytes, force_reencrypt: bool = False):
         config = ConfigUpdater().read_string(content.decode("utf-8"))
         secret_provider = config.get("batou", "secret_provider", fallback=None)
         if secret_provider is None or secret_provider.value is None:
-            config.set("batou", "secret_provider", "age")
-            print("Setting secret provider to age.")
+            config.set("batou", "secret_provider", self.secret_provider_str)
+            print(f"Setting secret provider to {self.secret_provider_str}.")
         secret_provider = config.get("batou", "secret_provider")
-        if secret_provider.value != "age":
+        if secret_provider.value != self.secret_provider_str:
             self.change_secret_provider(config, self)
             return
         recipients_opt = config.get("batou", "members")
         if recipients_opt is None or recipients_opt.value is None:
             raise ValueError(
                 "Please add a 'batou.members' section to the secrets file."
             )
         recipients = re.split(r"(\n|,)+", recipients_opt.value)
         recipients = [r.strip() for r in recipients if r.strip()]
         if not recipients or len(recipients) == 0 or recipients[0] == "":
             raise ValueError(
                 "Please add at least one recipient to the secrets file."
             )
-        recipients = process_age_recipients(
+        recipients, keys_changed = process_age_recipients(
             recipients,
             pathlib.Path(self.environment.base_dir)
             / pathlib.Path("environments")
             / self.environment.name,
         )
         self.config_file.write(
             str(config).encode("utf-8"),
             recipients,
+            reencrypt=keys_changed or force_reencrypt,
         )
-        self.write_secret_files(self.read_secret_files())
+        if keys_changed or force_reencrypt:
+            self.write_secret_files(self.read_secret_files())
 
-    def secret_provider_str(self) -> str:
-        return "age"
+
+class DiffableAGESecretProvider(AGESecretProvider):
+    FileFactory = DiffableAGEEncryptedFile
+    secret_provider_str = "age-diffable"
+
+    def __init__(self, environment: "Environment"):
+        super().__init__(environment)
+        self.config_file = DiffableAGEEncryptedFile(
+            pathlib.Path(environment.base_dir)
+            / "environments"
+            / environment.name
+            / "secrets.cfg.age-diffable"
+        )
```

### Comparing `batou-2.4rc2/src/batou/secrets/edit.py` & `batou-2.5.0b1/src/batou/secrets/edit.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,24 @@
         while cmd != "quit":
             try:
                 self.process_cmd(cmd)
             except Exception as e:
                 print()
                 print()
                 print(f"An error occurred: {e}")
+                print("Traceback:")
+                tb = traceback.format_exc()
+                tb_lines = tb.splitlines()
+                # if tb is too long, only have first and last 10 lines
+                if len(tb_lines) > 20 and not debug:
+                    print("\n".join(tb_lines[:10]))
+                    print("...")
+                    print("\n".join(tb_lines[-10:]))
+                else:
+                    print(tb)
                 print()
                 print("Your changes are still available. You can try:")
                 print("\tedit       -- opens editor with current data again")
                 print("\tencrypt    -- tries to encrypt current data again")
                 print("\tquit       -- quits and loses your changes")
                 cmd = self._input()
             else:
```

### Comparing `batou-2.4rc2/src/batou/secrets/encryption.py` & `batou-2.5.0b1/src/batou/secrets/encryption.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+import base64
 import errno
 import fcntl
 import os
 import pathlib
 import pty
 import subprocess
 import sys
 import tempfile
 from typing import Dict, List, Optional
 
+from configupdater import ConfigUpdater
+
 from batou import AgeCallError, FileLockedError, GPGCallError
 from batou._output import output
 
 debug = False
 
 
 class EncryptedFile:
@@ -41,20 +44,29 @@
     def cleartext(self) -> str:
         return self.decrypted.decode("utf-8")
 
     @property
     def locked(self) -> bool:
         return self.fd is not None
 
-    def write(self, content: bytes, recipients: List[str]):
+    def write(
+        self, content: bytes, recipients: List[str], reencrypt: bool = False
+    ):
+        if debug:
+            print(
+                f"EncryptedFile({self.path}).write({content}, {recipients}, {reencrypt})",
+                file=sys.stderr,
+            )
         self._decrypted = None
-        self._write(content, recipients)
+        self._write(content, recipients, reencrypt)
         self._decrypted = content
 
-    def _write(self, content: bytes, recipients: List[str]):
+    def _write(
+        self, content: bytes, recipients: List[str], reencrypt: bool = False
+    ):
         raise NotImplementedError("_write() not implemented")
 
     def __enter__(self):
         self._lock()
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
@@ -136,15 +148,17 @@
             )
         except subprocess.CalledProcessError as e:
             raise GPGCallError.from_context(
                 e.cmd, e.returncode, e.stderr
             ) from e
         return p.stdout
 
-    def _write(self, content: bytes, recipients: List[str]):
+    def _write(
+        self, content: bytes, recipients: List[str], reencrypt: bool = False
+    ):
         if not self.locked:
             raise RuntimeError("File not locked")
         if not self.writeable:
             raise RuntimeError("File not writeable")
         self.path.rename(str(self.path) + ".old")
         old_path = pathlib.Path(str(self.path) + ".old")
         # starting with python 3.8, pathlib.Path's rename() method
@@ -379,15 +393,17 @@
                     return result
         for e in exceptions:
             print(e)
         raise Exception(
             f"Could not decrypt {self.path} with any of the identities {identities}"
         )
 
-    def _write(self, content: bytes, recipients: List[str]):
+    def _write(
+        self, content: bytes, recipients: List[str], reencrypt: bool = False
+    ):
         if not self.locked:
             raise ValueError("File is not locked")
         if not self.writeable:
             raise ValueError("File is not writeable")
         args = [self.age(), "-e"]
         for recipient in recipients:
             args.extend(["-r", recipient])
@@ -429,7 +445,99 @@
                     return cls._age
         raise RuntimeError(
             "Could not find age binary."
             " Is age installed? I tried looking for: {}".format(
                 ", ".join("`{}`".format(x) for x in cls.AGE_BINARY_CANDIDATES)
             )
         )
+
+
+class DiffableAGEEncryptedFile(EncryptedFile):
+    def __init__(self, path: "pathlib.Path", writeable: bool = False):
+        super().__init__(path, writeable)
+        self._decrypted_content = None
+        self._encrypted_content = None
+
+    def decrypt_age_string(self, content: str) -> str:
+        # base64 -> tmpfile -> AGEEncryptedFile -> decrypt -> read
+        with tempfile.NamedTemporaryFile() as temp_file:
+            temp_file.write(base64.b64decode(content))
+            temp_file.flush()
+            with AGEEncryptedFile(pathlib.Path(temp_file.name)) as ef:
+                return ef.cleartext
+
+    def encrypt_age_string(self, content: str, recipients: List[str]) -> str:
+        # tmpfile -> AGEEncryptedFile -> write plaintext -> read ciphertext -> base64
+        with tempfile.NamedTemporaryFile() as temp_file:
+            with AGEEncryptedFile(pathlib.Path(temp_file.name), True) as ef:
+                ef.write(content.encode("utf-8"), recipients)
+            with open(temp_file.name, "rb") as f:
+                return base64.b64encode(f.read()).decode("utf-8")
+
+    def decrypt(self):
+        # read the entire file, parse as ConfigUpdater
+
+        if not self.locked:
+            raise ValueError("File is not locked")
+
+        config_encrypted = ConfigUpdater().read(self.path)
+        config = ConfigUpdater().read(self.path)
+
+        # for each section
+        for section in config.sections():
+            # if section is called batou, skip
+            if section == "batou":
+                continue
+            # for each option
+            for option in config[section]:
+                # decrypt the value
+                config[section][option].value = self.decrypt_age_string(
+                    config[section][option].value
+                )
+
+        # cache the decrypted content
+        self._decrypted_content = config
+        self._encrypted_content = config_encrypted
+
+        # return the decrypted content as bytes
+        return str(config).encode("utf-8")
+
+    def _write(
+        self, content: bytes, recipients: List[str], reencrypt: bool = False
+    ):
+        # parse the content as ConfigUpdater
+        config = ConfigUpdater()
+        config.read_string(content.decode("utf-8"))
+
+        # for each section
+        for section in config.sections():
+            # if section is called batou, skip
+            if section == "batou":
+                continue
+            # for each option
+            for option in config[section]:
+                new_value = config[section][option].value
+                assert new_value is not None
+
+                try:
+                    old_value = self._decrypted_content[section][option].value
+                except Exception:
+                    old_value = None
+
+                value_has_changed = new_value != old_value
+
+                if reencrypt or value_has_changed:
+                    new_encrypted_value = self.encrypt_age_string(
+                        new_value, recipients
+                    )
+                else:
+                    new_encrypted_value = self._encrypted_content[section][
+                        option
+                    ].value
+
+                config[section][option].value = new_encrypted_value
+
+        # write the config to the file
+        with open(self.path, "w") as f:
+            f.write(str(config))
+
+        self.is_new = False
```

### Comparing `batou-2.4rc2/src/batou/secrets/manage.py` & `batou-2.5.0b1/src/batou/secrets/manage.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 
 from configupdater import ConfigUpdater
 
 from batou import AgeCallError, GPGCallError
-from batou.environment import Environment
+from batou.environment import Environment, UnknownEnvironmentError
 
 
 def summary():
     return_code = 0
     environments = Environment.all()
     for environment in environments:
         print(environment.name)
@@ -40,18 +40,14 @@
             members = environment.secret_provider._get_recipients()
             if keyid not in members:
                 members.append(keyid)
             config.set("batou", "members", ",\n".join(members).split("\n"))
             environment.secret_provider.write_config(
                 str(config).encode("utf-8")
             )
-    if not environments_:
-        raise UnknownEnvironmentError(
-            [e.strip() for e in environments.split(",")]
-        )
 
 
 def remove_user(keyid, environments, **kw):
     """Remove a user from a given environment.
 
     If environments is not given, the user is removed
     from all environments.
@@ -65,11 +61,24 @@
             members = environment.secret_provider._get_recipients()
             if keyid in members:
                 members.remove(keyid)
             config.set("batou", "members", ",\n".join(members).split("\n"))
             environment.secret_provider.write_config(
                 str(config).encode("utf-8")
             )
-    if not environments:
-        raise UnknownEnvironmentError(
-            [e.strip() for e in environments.split(",")]
-        )
+
+
+def reencrypt(environments, **kw):
+    """Re-encrypt all secrets in given environments.
+
+    If environments is not given, all secrets are re-encrypted.
+
+    """
+    environments_ = Environment.filter(environments)
+    print(f"Re-encrypting environments {[e.name for e in environments_]}")
+    for environment in environments_:
+        environment.load_secrets()
+        with environment.secret_provider.edit():
+            config = environment.secret_provider.config
+            environment.secret_provider.write_config(
+                str(config).encode("utf-8"), force_reencrypt=True
+            )
```

### Comparing `batou-2.4rc2/src/batou/secrets/tests/test_editor.py` & `batou-2.5.0b1/src/batou/secrets/tests/test_editor.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import pathlib
 import sys
 
 import pytest
 
 from batou.environment import Environment
 from batou.secrets.edit import Editor
+from batou.tests.ellipsis import Ellipsis
 
 from .test_secrets import encrypted_file
 
 
 def test_edit_gpg(tmpdir):
     editor = Editor(
         "true",
@@ -62,44 +63,81 @@
         return cmds.pop(0)
 
     editor._input = _input
     editor.interact()
 
     out, err = capsys.readouterr()
     assert err == ""
-    assert (
-        out
-        == """\
+    assert out == Ellipsis(
+        """\
 
 
 An error occurred: gpg is broken
+Traceback:
+Traceback (most recent call last):
+  File ".../src/batou/secrets/edit.py", line ..., in interact
+    self.process_cmd(cmd)
+  File ".../src/batou/secrets/edit.py", line ..., in process_cmd
+    self.edit()
+  File ".../src/batou/secrets/tests/test_editor.py", line ..., in broken_cmd
+    raise RuntimeError("gpg is broken")
+RuntimeError: gpg is broken
+
 
 Your changes are still available. You can try:
 \tedit       -- opens editor with current data again
 \tencrypt    -- tries to encrypt current data again
 \tquit       -- quits and loses your changes
 
 
 An error occurred: gpg is broken
+Traceback:
+Traceback (most recent call last):
+  File ".../src/batou/secrets/edit.py", line ..., in interact
+    self.process_cmd(cmd)
+  File ".../src/batou/secrets/edit.py", line ..., in process_cmd
+    self.edit()
+  File ".../src/batou/secrets/tests/test_editor.py", line ..., in broken_cmd
+    raise RuntimeError("gpg is broken")
+RuntimeError: gpg is broken
+
 
 Your changes are still available. You can try:
 \tedit       -- opens editor with current data again
 \tencrypt    -- tries to encrypt current data again
 \tquit       -- quits and loses your changes
 
 
 An error occurred: unknown command `asdf`
+Traceback:
+Traceback (most recent call last):
+  File ".../src/batou/secrets/edit.py", line ..., in interact
+    self.process_cmd(cmd)
+  File ".../src/batou/secrets/edit.py", line ..., in process_cmd
+    raise ValueError("unknown command `{}`".format(cmd))
+ValueError: unknown command `asdf`
+
 
 Your changes are still available. You can try:
 \tedit       -- opens editor with current data again
 \tencrypt    -- tries to encrypt current data again
 \tquit       -- quits and loses your changes
 
 
 An error occurred: gpg is broken
+Traceback:
+Traceback (most recent call last):
+  File ".../src/batou/secrets/edit.py", line ..., in interact
+    self.process_cmd(cmd)
+  File ".../src/batou/secrets/edit.py", line ..., in process_cmd
+    self.encrypt()
+  File ".../src/batou/secrets/tests/test_editor.py", line ..., in broken_cmd
+    raise RuntimeError("gpg is broken")
+RuntimeError: gpg is broken
+
 
 Your changes are still available. You can try:
 \tedit       -- opens editor with current data again
 \tencrypt    -- tries to encrypt current data again
 \tquit       -- quits and loses your changes
 """
     )
```

### Comparing `batou-2.4rc2/src/batou/secrets/tests/test_secrets.py` & `batou-2.5.0b1/src/batou/secrets/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/template.py` & `batou-2.5.0b1/src/batou/template.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # There is a weird bug going on with Jinja2 on Python3.6 where this
 # test fails if Jinja tries to import ctypes itself ... o_O
 import ctypes
 import io
 
 import jinja2
 
-from batou import output
+from batou import TemplatingError, output
 
 
 class TemplateEngine(object):
     """Abstract templating wrapper class.
 
     Use a subclass that connects to a specific template engine.
     """
@@ -30,15 +30,18 @@
         """Return TemplateEngine instance for `enginename`."""
         if enginename.lower() == "jinja2":
             return Jinja2Engine()
         raise NotImplementedError("template engine not known", enginename)
 
     def template(self, sourcefile, args):
         """Render template from `sourcefile` and return the value."""
-        return self._render_template_file(sourcefile, args).getvalue()
+        try:
+            return self._render_template_file(sourcefile, args).getvalue()
+        except jinja2.exceptions.TemplateError as e:
+            raise TemplatingError.from_context(e, sourcefile)
 
     def _render_template_file(self, sourcefile, args):
         """Expand template found in `sourcefile` and return it as StringIO."""
         raise NotImplementedError
 
     def expand(self, templatestr, args):
         """Expand template in `templatestr` and return it as string."""
@@ -67,10 +70,13 @@
             output.error(
                 "You are trying to render a template that is bigger than "
                 "100KiB we've seen that Jinja can crash at large templates "
                 "and suggest you find alternatives for this. The affected "
                 "template starts with:"
             )
             output.annotate(templatestr[:100])
-        tmpl = self.env.from_string(templatestr)
-        tmpl.filename = identifier
-        return tmpl.render(**args)
+        try:
+            tmpl = self.env.from_string(templatestr)
+            tmpl.filename = identifier
+            return tmpl.render(**args)
+        except Exception as e:
+            raise TemplatingError.from_context(e, identifier)
```

### Comparing `batou-2.4rc2/src/batou/tests/conftest.py` & `batou-2.5.0b1/src/batou/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/tests/ellipsis.py` & `batou-2.5.0b1/src/batou/tests/ellipsis.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/tests/fixture/sample_service/components/hello/component.py` & `batou-2.5.0b1/src/batou/tests/fixture/sample_service/components/hello/component.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/tests/test_component.py` & `batou-2.5.0b1/src/batou/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/tests/test_config.py` & `batou-2.5.0b1/src/batou/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/tests/test_dependencies.py` & `batou-2.5.0b1/src/batou/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/tests/test_endtoend.py` & `batou-2.5.0b1/src/batou/tests/test_endtoend.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,18 +27,24 @@
 main: Loading environment `errors`...
 main: Verifying repository ...
 main: Loading secrets ...
 
 ERROR: Failed loading component file
            File: .../examples/errors/components/component5/component.py
       Exception: invalid syntax (component.py, line 1)
+Traceback (simplified, most recent call last):
+<no-non-remote-internal-traceback-lines-found>
 
 ERROR: Failed loading component file
            File: .../examples/errors/components/component6/component.py
       Exception: No module named 'asdf'
+Traceback (simplified, most recent call last):
+  File ".../errors/components/component6/component.py", line 1, in <module>
+    import asdf  # noqa: F401 import unused
+
 
 ERROR: Missing component
       Component: missingcomponent
 
 ERROR: Superfluous section in environment configuration
         Section: superfluoussection
 
@@ -73,18 +79,24 @@
       exit code: 2
         message:
 gpg: ...
 ...
 ERROR: Failed loading component file
            File: .../examples/errors/components/component5/component.py
       Exception: invalid syntax (component.py, line 1)
+Traceback (simplified, most recent call last):
+<no-non-remote-internal-traceback-lines-found>
 
 ERROR: Failed loading component file
            File: .../examples/errors/components/component6/component.py
       Exception: No module named 'asdf'
+Traceback (simplified, most recent call last):
+  File ".../examples/errors/components/component6/component.py", line 1, in <module>
+    import asdf  # noqa: F401 import unused
+
 
 ERROR: Missing component
       Component: missingcomponent
 
 ERROR: Superfluous section in environment configuration
         Section: superfluoussection
 
@@ -116,14 +128,19 @@
  Affected hosts: localhost
 
 ERROR: malformed node or string: <...Name object at 0x...>
       Attribute: Component1.do_what_is_needed
      Conversion: convert_literal('false')
  Affected hosts: localhost
 
+ERROR: Error while expanding attribute:
+        Message: TemplatingError: An error occured while rendering a template (Component5): KeyError: 'doesnotexist'
+      Attribute: Component5.attribute_cannot_be_expanded
+ Affected hosts: localhost
+
 ERROR: Need port for service address.
       Attribute: DNSProblem.attribute_with_problem
      Conversion: Address('localhost')
  Affected hosts: localhost
 
 ERROR: Mode-string should be between `---------` and `rwxrwxrwx`.
       Attribute: FileMode > File('work/filemode/new-file.txt') > Mode('new-file.txt').mode
@@ -145,16 +162,16 @@
 
 ERROR: Found dependency cycle
 cycle1 depends on
         cycle2
 cycle2 depends on
         cycle1
 
-ERROR: 9 remaining unconfigured component(s): component1, component2, component4, crontab, cycle1, cycle2, dnsproblem, dnsproblem2, filemode
-======================= 10 ERRORS - CONFIGURATION FAILED =======================
+ERROR: 10 remaining unconfigured component(s): component1, component2, component4, component5, crontab, cycle1, cycle2, dnsproblem, dnsproblem2, filemode
+======================= 11 ERRORS - CONFIGURATION FAILED =======================
 ====================== DEPLOYMENT FAILED (during connect) ======================
 """
     )  # noqa: E501 line too long
 
 
 def test_example_errors_missing_environment():
     os.chdir("examples/errors")
```

### Comparing `batou-2.4rc2/src/batou/tests/test_environment.py` & `batou-2.5.0b1/src/batou/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/tests/test_exceptions.py` & `batou-2.5.0b1/src/batou/tests/test_exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     errors.append(UnusedResources.from_context({"asdf": {root: 1}}))
 
     errors.append(UnsatisfiedResources.from_context({"asdf": [root]}))
 
     errors.append(MissingEnvironment.from_context(root.environment))
 
     errors.append(
-        ComponentLoadingError.from_context("asdf.py", ValueError("asdf"))
+        ComponentLoadingError.from_context("asdf.py", ValueError("asdf"), None)
     )
 
     errors.append(MissingComponent.from_context("component", "hostname"))
 
     errors.append(SuperfluousSection.from_context("asdf"))
 
     errors.append(SuperfluousComponentSection.from_context("asdf"))
```

### Comparing `batou-2.4rc2/src/batou/tests/test_host.py` & `batou-2.5.0b1/src/batou/tests/test_host.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/tests/test_main.py` & `batou-2.5.0b1/src/batou/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/tests/test_remote.py` & `batou-2.5.0b1/src/batou/tests/test_remote.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import os
+
 import mock
 import pytest
 
 from batou.deploy import Deployment
 from batou.environment import Environment
 from batou.host import RemoteHost
-from batou.utils import cmd
+from batou.utils import CmdExecutionError, cmd
 
 
 @pytest.mark.slow
 def test_remote_deployment_initializable(sample_service):
     cmd("hg init")
     with open(".hg/hgrc", "w") as f:
         f.write("[paths]\ndefault=https://example.com")
@@ -32,14 +34,38 @@
         repository.update(h)
     assert e.value.args == (
         "Remote repository did not find any heads. "
         "Can not continue creating a bundle.",
     )
 
 
+def test_git_remote_bundle_fails_if_needed(tmp_path):
+    env = mock.Mock()
+    env.base_dir = tmp_path
+    env.branch = "master"
+    host = mock.Mock()
+    host.rpc.git_current_head.return_value.decode.return_value = "HEAD"
+    from batou.repository import GitBundleRepository
+
+    os.chdir(tmp_path)
+    cmd("git init")
+    cmd("touch foo")
+    cmd("git add foo")
+    cmd("git commit -m 'initial commit'")
+    repository = GitBundleRepository(env)
+    assert repository._ship(host) is None
+
+    # now destroy the repository state
+    head_commit = cmd("git rev-parse HEAD")[0].strip()
+    cmd(f"rm -rf .git/objects/{head_commit[:2]}/{head_commit[2:]}")
+    with pytest.raises(CmdExecutionError) as e:
+        repository._ship(host)
+    assert "Invalid revision range" in str(e.value)
+
+
 def test_remotehost_start(sample_service):
     env = Environment("test-with-env-config")
     env.load()
     env.configure()
     h = RemoteHost("asdf", env)
     h.connect = mock.Mock()
     h.rpc = mock.Mock()
```

### Comparing `batou-2.4rc2/src/batou/tests/test_remote_core.py` & `batou-2.5.0b1/src/batou/tests/test_remote_core.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/tests/test_repository.py` & `batou-2.5.0b1/src/batou/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/tests/test_resources.py` & `batou-2.5.0b1/src/batou/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/tests/test_template.py` & `batou-2.5.0b1/src/batou/tests/test_template.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import collections
 import os.path
 
 import jinja2
 import mock
 import pytest
 
+from batou import TemplatingError
 from batou.template import TemplateEngine
 
 Server = collections.namedtuple("Server", ["name", "address"])
 
 sample_dict = dict(
     host=mock.Mock(),
     config=dict(),
@@ -77,14 +78,14 @@
 {{hello}}hello {{hello}}hello {{he"""
         == log
     )
 
 
 def test_jinja2_unknown_variable_should_fail():
     tmpl = TemplateEngine.get("jinja2")
-    with pytest.raises(jinja2.UndefinedError):
+    with pytest.raises(TemplatingError):
         tmpl.expand("unknown variable {{foo}}", {})
 
 
 def test_jinja2_umlaut_variables():
     tmpl = TemplateEngine.get("jinja2")
     assert "hello wörld" == tmpl.expand("hello {{hello2}}", sample_dict)
```

### Comparing `batou-2.4rc2/src/batou/tests/test_utils.py` & `batou-2.5.0b1/src/batou/tests/test_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -168,49 +168,49 @@
 def test_address_v6_only(monkeypatch):
     hostname = "v6only.example.com"
 
     from batou.utils import resolve_v6_override
 
     monkeypatch.setitem(resolve_v6_override, hostname, "::346")
 
-    with pytest.raises(socket.gaierror) as f:
+    with pytest.raises(batou.GetAddressInfoError) as f:
         a = Address(hostname, 1234)
         a.listen
 
-    assert str(f.value) in RESOLVER_ERRORS
+    assert any(x in str(f.value) for x in RESOLVER_ERRORS)
 
     address = Address(hostname, 1234, require_v4=False, require_v6=True)
     assert address.listen_v6.host == "::346"
     assert address.require_v6
 
 
 def test_address_fails_when_name_cannot_be_looked_up_at_all():
-    with pytest.raises(socket.gaierror) as f:
+    with pytest.raises(batou.GetAddressInfoError) as f:
         a = Address("does-not-exist.example.com:1234")
         a.listen
-    assert str(f.value) in RESOLVER_ERRORS
+    assert any(x in str(f.value) for x in RESOLVER_ERRORS)
 
-    with pytest.raises(socket.gaierror) as f:
+    with pytest.raises(batou.GetAddressInfoError) as f:
         a = Address(
             "does-not-exist.example.com:1234", require_v4=False, require_v6=True
         )
         a.listen_v6
-    assert str(f.value) in RESOLVER_ERRORS
+    assert any(x in str(f.value) for x in RESOLVER_ERRORS)
 
-    with pytest.raises(socket.gaierror) as f:
+    with pytest.raises(batou.GetAddressInfoError) as f:
         a = Address(
             "does-not-exist.example.com:1234", require_v4=True, require_v6=True
         )
         a.listen
-    with pytest.raises(socket.gaierror) as f:
+    with pytest.raises(batou.GetAddressInfoError) as f:
         a = Address(
             "does-not-exist.example.com:1234", require_v4=True, require_v6=True
         )
         a.listen_v6
-    assert str(f.value) in RESOLVER_ERRORS
+    assert any(x in str(f.value) for x in RESOLVER_ERRORS)
 
 
 def test_address_optional_when_name_cannot_be_looked_up_at_all():
     a = Address(
         "does-not-exist.example.com:1234",
         require_v4="optional",
         require_v6="optional",
@@ -337,15 +337,14 @@
         lockfile = self.tempfile()
         with locked(lockfile):
             locked2 = locked(lockfile)
             self.assertRaises(RuntimeError, locked2.__enter__)
 
 
 class NotifyTests(unittest.TestCase):
-
     # XXX: What this actually should test is:
     # if notify-send is there, use it. It does not need to exit on all
     # non-darwin machines.
     # @pytest.mark.skipif("sys.platform == 'darwin'")
     # @mock.patch('subprocess.check_call')
     # def test_notify_calls_notify_send(self, call):
     #     notify('foo', 'bar')
@@ -390,15 +389,14 @@
 def test_graph_remove_leafs():
     graph = {1: [1], 2: []}
     remove_nodes_without_outgoing_edges(graph)
     assert graph == {1: [1]}
 
 
 class Checksum(unittest.TestCase):
-
     fixture = os.path.join(
         os.path.dirname(__file__), "fixture", "component", "haproxy.cfg"
     )
 
     def test_hash_md5(self):
         self.assertEqual(
             "ce0324fa445475e76182c0d114615c7b", hash(self.fixture, "md5")
```

### Comparing `batou-2.4rc2/src/batou/tests/test_vfs.py` & `batou-2.5.0b1/src/batou/tests/test_vfs.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou/utils.py` & `batou-2.5.0b1/src/batou/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,20 @@
 import sys
 import time
 from collections import defaultdict
 from typing import Optional
 
 import pkg_resources
 
-from batou import DeploymentError, IPAddressConfigurationError, output
+from batou import (
+    DeploymentError,
+    GetAddressInfoError,
+    IPAddressConfigurationError,
+    output,
+)
 
 
 class BagOfAttributes(dict):
     """Provide a dict-like object that can also
     be accessed using attributes.
 
     It's sometimes more convenient to write
@@ -255,19 +260,24 @@
             raise IPAddressConfigurationError.from_context(self, 4)
 
         assert self.connect.port is not None
         if not hasattr(self, "_listen_v4"):
             try:
                 address = resolve(self.connect.host, self.connect.port)
                 self.listen = NetLoc(address, self.connect.port)
-            except Exception:
+            except Exception as e:
                 if self.require_v4 == "optional":
                     self.listen = None
                 else:
-                    raise
+                    if isinstance(e, OSError):
+                        raise GetAddressInfoError.from_context(
+                            f"{self.connect.host}:{self.connect.port}", str(e)
+                        )
+                    else:
+                        raise
 
         return self._listen_v4
 
     @listen.setter
     def listen(self, value):
         self._listen_v4 = value
 
@@ -282,19 +292,24 @@
             raise IPAddressConfigurationError.from_context(self, 6)
 
         assert self.connect.port is not None
         if not hasattr(self, "_listen_v6"):
             try:
                 address = resolve_v6(self.connect.host, self.connect.port)
                 self.listen_v6 = NetLoc(address, self.connect.port)
-            except Exception:
+            except Exception as e:
                 if self.require_v6 == "optional":
                     self.listen_v6 = None
                 else:
-                    raise
+                    if isinstance(e, OSError):
+                        raise GetAddressInfoError.from_context(
+                            f"{self.connect.host}:{self.connect.port}", str(e)
+                        )
+                    else:
+                        raise
 
         return self._listen_v6
 
     @listen_v6.setter
     def listen_v6(self, value):
         self._listen_v6 = value
```

### Comparing `batou-2.4rc2/src/batou/vfs.py` & `batou-2.5.0b1/src/batou/vfs.py`

 * *Files identical despite different names*

### Comparing `batou-2.4rc2/src/batou.egg-info/SOURCES.txt` & `batou-2.5.0b1/src/batou.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -30,25 +30,27 @@
 doc/source/user/quickstart.txt
 examples/api/index.txt
 examples/api/requirements.txt
 examples/django/requirements.txt
 examples/durations/requirements.txt
 examples/errors/requirements.txt
 examples/errors2/requirements.txt
+examples/errorsnohost/requirements.txt
 examples/ignores/requirements.txt
 examples/largetempl/requirements.txt
 examples/package/requirements.txt
 examples/sync_async/requirements.txt
 examples/tutorial-buildout/requirements.txt
 examples/tutorial-component/requirements.txt
 examples/tutorial-helloworld/requirements.txt
 examples/tutorial-parallelize/requirements.txt
 examples/tutorial-provision-container/requirements.txt
 examples/tutorial-secrets/requirements.txt
 examples/tutorial-secrets/environments/age/age_keys.txt
+examples/tutorial-secrets/environments/age-diffable/age_keys.txt
 examples/vagrant/requirements.txt
 examples/vagrant-multi/requirements.txt
 examples/venvs/requirements.txt
 examples/venvs/environments/requirements.txt
 src/batou/__init__.py
 src/batou/_output.py
 src/batou/agent.py
```

