# Comparing `tmp/Surfactant-0.0.0rc4.tar.gz` & `tmp/surfactant-0.0.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Surfactant-0.0.0rc4.tar", last modified: Thu Feb 22 04:59:19 2024, max compression
+gzip compressed data, was "surfactant-0.0.0rc5.tar", last modified: Fri Apr 19 01:26:51 2024, max compression
```

## Comparing `Surfactant-0.0.0rc4.tar` & `surfactant-0.0.0rc5.tar`

### file list

```diff
@@ -1,235 +1,239 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.133871 Surfactant-0.0.0rc4/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.105871 Surfactant-0.0.0rc4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.105871 Surfactant-0.0.0rc4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.105871 Surfactant-0.0.0rc4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)    16160 2024-02-22 04:59:19.133871 Surfactant-0.0.0rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13932 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.133871 Surfactant-0.0.0rc4/Surfactant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16160 2024-02-22 04:59:19.000000 Surfactant-0.0.0rc4/Surfactant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-02-22 04:59:19.000000 Surfactant-0.0.0rc4/Surfactant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 04:59:19.000000 Surfactant-0.0.0rc4/Surfactant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-22 04:59:19.000000 Surfactant-0.0.0rc4/Surfactant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-02-22 04:59:19.000000 Surfactant-0.0.0rc4/Surfactant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-22 04:59:19.000000 Surfactant-0.0.0rc4/Surfactant.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.109871 Surfactant-0.0.0rc4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.109871 Surfactant-0.0.0rc4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/docs/_static/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.109871 Surfactant-0.0.0rc4/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/docs/_templates/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/docs/basic_usage.md
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/docs/configuration_files.md
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/docs/contribution_guide.md
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/docs/getting_started.md
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.109871 Surfactant-0.0.0rc4/docs/logos/
--rw-r--r--   0 runner    (1001) docker     (127)    32676 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/docs/logos/surfactant-logo-dark-250px.png
--rw-r--r--   0 runner    (1001) docker     (127)   117613 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/docs/logos/surfactant-logo-dark.png
--rw-r--r--   0 runner    (1001) docker     (127)    31219 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/docs/logos/surfactant-logo-light-250px.png
--rw-r--r--   0 runner    (1001) docker     (127)   119482 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/docs/logos/surfactant-logo-light.png
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/docs/plugins.md
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.113871 Surfactant-0.0.0rc4/docs/windows_installer_tutorial/
--rwxr-xr-x   0 runner    (1001) docker     (127)     9767 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/docs/windows_installer_tutorial/AutomatedInstallerWorkflowSetup.md
--rw-r--r--   0 runner    (1001) docker     (127)    13436 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/docs/windows_installer_tutorial/execinstaller.py
--rw-r--r--   0 runner    (1001) docker     (127)   111741 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/docs/windows_installer_tutorial/fsfilter.patch
--rw-r--r--   0 runner    (1001) docker     (127)    12567 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/docs/windows_installer_tutorial/setupstepper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.113871 Surfactant-0.0.0rc4/example-configs/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/example-configs/helics-archive-config.json
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/example-configs/helics-installprefix-config.json
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/example-configs/multiple-archives-config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.113871 Surfactant-0.0.0rc4/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/plugins/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.113871 Surfactant-0.0.0rc4/plugins/angrimportfinder/
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/plugins/angrimportfinder/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/plugins/angrimportfinder/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/plugins/angrimportfinder/surfactantplugin_angrimportfinder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.113871 Surfactant-0.0.0rc4/plugins/binary2strings/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/plugins/binary2strings/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/plugins/binary2strings/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/plugins/binary2strings/surfactantplugin_binary2strings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.113871 Surfactant-0.0.0rc4/plugins/checksec.py/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/plugins/checksec.py/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/plugins/checksec.py/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/plugins/checksec.py/surfactantplugin_checksec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.113871 Surfactant-0.0.0rc4/plugins/syft/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/plugins/syft/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/plugins/syft/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/plugins/syft/surfactantplugin_syft.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/requirements-build.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/requirements-dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.113871 Surfactant-0.0.0rc4/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/scripts/README-merge_sbom.md
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/scripts/merge_additional_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/scripts/merge_config.json
--rwxr-xr-x   0 runner    (1001) docker     (127)    21205 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/scripts/merge_sbom.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 04:59:19.133871 Surfactant-0.0.0rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.117871 Surfactant-0.0.0rc4/surfactant/
--rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1458 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-02-22 04:59:18.000000 Surfactant-0.0.0rc4/surfactant/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.117871 Surfactant-0.0.0rc4/surfactant/cmd/
--rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/cmd/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/cmd/createconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    22485 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/cmd/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/cmd/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/cmd/stat.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2183 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/fileinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.117871 Surfactant-0.0.0rc4/surfactant/filetypeid/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/filetypeid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/filetypeid/id_extension.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2282 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/filetypeid/id_hex.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7283 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/filetypeid/id_magic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.117871 Surfactant-0.0.0rc4/surfactant/infoextractors/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/infoextractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/infoextractors/a_out_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/infoextractors/coff_file.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9202 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/infoextractors/elf_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/infoextractors/java_file.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1997 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/infoextractors/ole_file.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    26267 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/infoextractors/pe_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.117871 Surfactant-0.0.0rc4/surfactant/input_readers/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/input_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/input_readers/cytrics_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.121871 Surfactant-0.0.0rc4/surfactant/output/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/output/csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12597 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/output/cyclonedx_writer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      483 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/output/cytrics_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    27142 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/output/spdx_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.121871 Surfactant-0.0.0rc4/surfactant/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/plugin/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/plugin/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.121871 Surfactant-0.0.0rc4/surfactant/relationships/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1405 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/relationships/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.121871 Surfactant-0.0.0rc4/surfactant/relationships/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/relationships/_internal/posix_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/relationships/_internal/windows_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13707 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/relationships/dotnet_relationship.py
--rw-r--r--   0 runner    (1001) docker     (127)    11862 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/relationships/elf_relationship.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/relationships/java_relationship.py
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/relationships/pe_relationship.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.121871 Surfactant-0.0.0rc4/surfactant/sbomtypes/
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/sbomtypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/sbomtypes/_analysisdata.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/sbomtypes/_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/sbomtypes/_hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/sbomtypes/_observation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/sbomtypes/_provenance.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/sbomtypes/_relationship.py
--rw-r--r--   0 runner    (1001) docker     (127)    13419 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/sbomtypes/_sbom.py
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/sbomtypes/_software.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/surfactant/sbomtypes/_system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.101871 Surfactant-0.0.0rc4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.121871 Surfactant-0.0.0rc4/tests/cmd/
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/cmd/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/cmd/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/cmd/test_merge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.101871 Surfactant-0.0.0rc4/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.101871 Surfactant-0.0.0rc4/tests/data/ELF_shared_obj_test_no1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.125871 Surfactant-0.0.0rc4/tests/data/ELF_shared_obj_test_no1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)    16424 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data/ELF_shared_obj_test_no1/bin/hello_world
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.125871 Surfactant-0.0.0rc4/tests/data/ELF_shared_obj_test_no1/lib/
--rw-r--r--   0 runner    (1001) docker     (127)    16184 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data/ELF_shared_obj_test_no1/lib/libtestlib.so
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.125871 Surfactant-0.0.0rc4/tests/data/NET_app_config_test_no1/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data/NET_app_config_test_no1/ConsoleApp2.dll.config
--rw-r--r--   0 runner    (1001) docker     (127)   147968 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data/NET_app_config_test_no1/ConsoleApp2.exe
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.101871 Surfactant-0.0.0rc4/tests/data/NET_app_config_test_no1/bin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.101871 Surfactant-0.0.0rc4/tests/data/NET_app_config_test_no1/bin/Debug/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.125871 Surfactant-0.0.0rc4/tests/data/NET_app_config_test_no1/bin/Debug/net6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data/NET_app_config_test_no1/bin/Debug/net6.0/hello.dll
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.125871 Surfactant-0.0.0rc4/tests/data/Windows_dll_test_no1/
--rw-r--r--   0 runner    (1001) docker     (127)    58880 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data/Windows_dll_test_no1/hello_world.exe
--rw-r--r--   0 runner    (1001) docker     (127)    53248 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data/Windows_dll_test_no1/testlib.dll
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.125871 Surfactant-0.0.0rc4/tests/data/a_out_files/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data/a_out_files/big_m68020.aout
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data/a_out_files/big_netbsd_i386.aout
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data/a_out_files/big_netbsd_sparc.aout
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data/a_out_files/little_386.aout
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data/a_out_files/little_unknown.aout
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.125871 Surfactant-0.0.0rc4/tests/data/coff_files/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data/coff_files/intel_80386_coff
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.125871 Surfactant-0.0.0rc4/tests/data/java_class_no1/
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data/java_class_no1/HelloWorld.class
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.101871 Surfactant-0.0.0rc4/tests/data/mach_o_dylib_test_no1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.125871 Surfactant-0.0.0rc4/tests/data/mach_o_dylib_test_no1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)    55672 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data/mach_o_dylib_test_no1/bin/hello_world
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.125871 Surfactant-0.0.0rc4/tests/data/mach_o_dylib_test_no1/lib/
--rwxr-xr-x   0 runner    (1001) docker     (127)    51128 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data/mach_o_dylib_test_no1/lib/libtestlib.dylib
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.125871 Surfactant-0.0.0rc4/tests/data/msitest_no1/
--rw-r--r--   0 runner    (1001) docker     (127)    12288 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data/msitest_no1/test.msi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.125871 Surfactant-0.0.0rc4/tests/data/sample_sboms/
--rw-r--r--   0 runner    (1001) docker     (127)    15436 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data/sample_sboms/helics_binaries_sbom.json
--rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data/sample_sboms/helics_libs_sbom.json
--rw-r--r--   0 runner    (1001) docker     (127)    21305 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data/sample_sboms/helics_sbom.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.125871 Surfactant-0.0.0rc4/tests/data/srectest_no1/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data/srectest_no1/HexFile.hex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.125871 Surfactant-0.0.0rc4/tests/data_src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.129871 Surfactant-0.0.0rc4/tests/data_src/NET_app_config_test_no1/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data_src/NET_app_config_test_no1/App.config
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data_src/NET_app_config_test_no1/ConsoleApp2.csproj
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data_src/NET_app_config_test_no1/ConsoleApp2.sln
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data_src/NET_app_config_test_no1/Program.cs
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data_src/NET_app_config_test_no1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data_src/NET_app_config_test_no1/hello.cs
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data_src/NET_app_config_test_no1/hello.csproj
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data_src/NET_app_config_test_no1/hello.sln
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data_src/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.129871 Surfactant-0.0.0rc4/tests/data_src/java_class_no1/
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data_src/java_class_no1/HelloWorld.class
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data_src/java_class_no1/HelloWorld.jar
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data_src/java_class_no1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data_src/java_class_no1/helloworld.java
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.129871 Surfactant-0.0.0rc4/tests/data_src/msitest_no1/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data_src/msitest_no1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data_src/msitest_no1/hello.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)    16376 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data_src/msitest_no1/hello.exe
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data_src/msitest_no1/test.wxs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.129871 Surfactant-0.0.0rc4/tests/data_src/native_shared_lib_test_no1/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data_src/native_shared_lib_test_no1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data_src/native_shared_lib_test_no1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data_src/native_shared_lib_test_no1/hello_world.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.129871 Surfactant-0.0.0rc4/tests/data_src/native_shared_lib_test_no1/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data_src/native_shared_lib_test_no1/lib/testlib.cpp
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data_src/native_shared_lib_test_no1/lib/testlib.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.129871 Surfactant-0.0.0rc4/tests/data_src/srectest_no1/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data_src/srectest_no1/BinaryFile.bin
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data_src/srectest_no1/HexFile.hex
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/data_src/srectest_no1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.133871 Surfactant-0.0.0rc4/tests/file_types/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/file_types/test_a_out_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/file_types/test_file_magic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.133871 Surfactant-0.0.0rc4/tests/relationships/
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/relationships/test_dotnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/relationships/test_elf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/relationships/test_java.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/relationships/test_pe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/relationships/test_posix_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 04:59:19.133871 Surfactant-0.0.0rc4/tests/symlink/
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-02-22 04:59:06.000000 Surfactant-0.0.0rc4/tests/symlink/test_resolve_links.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.370040 surfactant-0.0.0rc5/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.338040 surfactant-0.0.0rc5/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.338040 surfactant-0.0.0rc5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.338040 surfactant-0.0.0rc5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)    16160 2024-04-19 01:26:51.370040 surfactant-0.0.0rc5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13932 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.366040 surfactant-0.0.0rc5/Surfactant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16160 2024-04-19 01:26:51.000000 surfactant-0.0.0rc5/Surfactant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-04-19 01:26:51.000000 surfactant-0.0.0rc5/Surfactant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 01:26:51.000000 surfactant-0.0.0rc5/Surfactant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-19 01:26:51.000000 surfactant-0.0.0rc5/Surfactant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-19 01:26:51.000000 surfactant-0.0.0rc5/Surfactant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 01:26:51.000000 surfactant-0.0.0rc5/Surfactant.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.342040 surfactant-0.0.0rc5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.342040 surfactant-0.0.0rc5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/_static/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.342040 surfactant-0.0.0rc5/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/_templates/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/basic_usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/configuration_files.md
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/contribution_guide.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/getting_started.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.342040 surfactant-0.0.0rc5/docs/logos/
+-rw-r--r--   0 runner    (1001) docker     (127)    32676 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/logos/surfactant-logo-dark-250px.png
+-rw-r--r--   0 runner    (1001) docker     (127)   117613 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/logos/surfactant-logo-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31219 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/logos/surfactant-logo-light-250px.png
+-rw-r--r--   0 runner    (1001) docker     (127)   119482 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/logos/surfactant-logo-light.png
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/plugins.md
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.346040 surfactant-0.0.0rc5/docs/windows_installer_tutorial/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9767 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/windows_installer_tutorial/AutomatedInstallerWorkflowSetup.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13434 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/windows_installer_tutorial/execinstaller.py
+-rw-r--r--   0 runner    (1001) docker     (127)   111741 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/windows_installer_tutorial/fsfilter.patch
+-rw-r--r--   0 runner    (1001) docker     (127)    12565 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/windows_installer_tutorial/setupstepper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.346040 surfactant-0.0.0rc5/example-configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/example-configs/helics-archive-config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/example-configs/helics-installprefix-config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/example-configs/multiple-archives-config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.346040 surfactant-0.0.0rc5/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/plugins/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.346040 surfactant-0.0.0rc5/plugins/angrimportfinder/
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/plugins/angrimportfinder/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/plugins/angrimportfinder/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/plugins/angrimportfinder/surfactantplugin_angrimportfinder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.346040 surfactant-0.0.0rc5/plugins/binary2strings/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/plugins/binary2strings/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/plugins/binary2strings/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/plugins/binary2strings/surfactantplugin_binary2strings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.346040 surfactant-0.0.0rc5/plugins/checksec.py/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/plugins/checksec.py/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/plugins/checksec.py/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/plugins/checksec.py/surfactantplugin_checksec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.346040 surfactant-0.0.0rc5/plugins/fuzzyhashes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/plugins/fuzzyhashes/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/plugins/fuzzyhashes/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/plugins/fuzzyhashes/surfactantplugin_fuzzyhashes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.346040 surfactant-0.0.0rc5/plugins/syft/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/plugins/syft/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/plugins/syft/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/plugins/syft/surfactantplugin_syft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/requirements-build.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/requirements-dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.350040 surfactant-0.0.0rc5/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/scripts/README-merge_sbom.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/scripts/merge_additional_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/scripts/merge_config.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21205 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/scripts/merge_sbom.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 01:26:51.370040 surfactant-0.0.0rc5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.350040 surfactant-0.0.0rc5/surfactant/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1583 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-19 01:26:51.000000 surfactant-0.0.0rc5/surfactant/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.350040 surfactant-0.0.0rc5/surfactant/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/cmd/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/cmd/createconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23582 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/cmd/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/cmd/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/cmd/stat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2183 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/fileinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.350040 surfactant-0.0.0rc5/surfactant/filetypeid/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/filetypeid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/filetypeid/id_extension.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2304 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/filetypeid/id_hex.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7283 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/filetypeid/id_magic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.354040 surfactant-0.0.0rc5/surfactant/infoextractors/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/infoextractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/infoextractors/a_out_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/infoextractors/coff_file.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9202 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/infoextractors/elf_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/infoextractors/java_file.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1997 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/infoextractors/ole_file.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26619 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/infoextractors/pe_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.354040 surfactant-0.0.0rc5/surfactant/input_readers/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/input_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/input_readers/cytrics_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.354040 surfactant-0.0.0rc5/surfactant/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/output/csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12782 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/output/cyclonedx_writer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      483 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/output/cytrics_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27142 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/output/spdx_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.354040 surfactant-0.0.0rc5/surfactant/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/plugin/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/plugin/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.354040 surfactant-0.0.0rc5/surfactant/relationships/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1405 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/relationships/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.354040 surfactant-0.0.0rc5/surfactant/relationships/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/relationships/_internal/posix_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/relationships/_internal/windows_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13707 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/relationships/dotnet_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11862 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/relationships/elf_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/relationships/java_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/relationships/pe_relationship.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.358040 surfactant-0.0.0rc5/surfactant/sbomtypes/
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/sbomtypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/sbomtypes/_analysisdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/sbomtypes/_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/sbomtypes/_hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/sbomtypes/_observation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/sbomtypes/_provenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/sbomtypes/_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13639 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/sbomtypes/_sbom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/sbomtypes/_software.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/sbomtypes/_system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.334040 surfactant-0.0.0rc5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.358040 surfactant-0.0.0rc5/tests/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/cmd/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/cmd/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/cmd/test_merge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.334040 surfactant-0.0.0rc5/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.334040 surfactant-0.0.0rc5/tests/data/ELF_shared_obj_test_no1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.358040 surfactant-0.0.0rc5/tests/data/ELF_shared_obj_test_no1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16424 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/ELF_shared_obj_test_no1/bin/hello_world
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.358040 surfactant-0.0.0rc5/tests/data/ELF_shared_obj_test_no1/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)    16184 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/ELF_shared_obj_test_no1/lib/libtestlib.so
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.358040 surfactant-0.0.0rc5/tests/data/NET_app_config_test_no1/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/NET_app_config_test_no1/ConsoleApp2.dll.config
+-rw-r--r--   0 runner    (1001) docker     (127)   147968 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/NET_app_config_test_no1/ConsoleApp2.exe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.334040 surfactant-0.0.0rc5/tests/data/NET_app_config_test_no1/bin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.334040 surfactant-0.0.0rc5/tests/data/NET_app_config_test_no1/bin/Debug/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.358040 surfactant-0.0.0rc5/tests/data/NET_app_config_test_no1/bin/Debug/net6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/NET_app_config_test_no1/bin/Debug/net6.0/hello.dll
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.358040 surfactant-0.0.0rc5/tests/data/Windows_dll_test_no1/
+-rw-r--r--   0 runner    (1001) docker     (127)    58880 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/Windows_dll_test_no1/hello_world.exe
+-rw-r--r--   0 runner    (1001) docker     (127)    53248 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/Windows_dll_test_no1/testlib.dll
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.358040 surfactant-0.0.0rc5/tests/data/a_out_files/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/a_out_files/big_m68020.aout
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/a_out_files/big_netbsd_i386.aout
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/a_out_files/big_netbsd_sparc.aout
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/a_out_files/little_386.aout
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/a_out_files/little_unknown.aout
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.362040 surfactant-0.0.0rc5/tests/data/coff_files/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/coff_files/intel_80386_coff
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.362040 surfactant-0.0.0rc5/tests/data/java_class_no1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/java_class_no1/HelloWorld.class
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.334040 surfactant-0.0.0rc5/tests/data/mach_o_dylib_test_no1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.362040 surfactant-0.0.0rc5/tests/data/mach_o_dylib_test_no1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    55672 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/mach_o_dylib_test_no1/bin/hello_world
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.362040 surfactant-0.0.0rc5/tests/data/mach_o_dylib_test_no1/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    51128 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/mach_o_dylib_test_no1/lib/libtestlib.dylib
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.362040 surfactant-0.0.0rc5/tests/data/msitest_no1/
+-rw-r--r--   0 runner    (1001) docker     (127)    12288 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/msitest_no1/test.msi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.362040 surfactant-0.0.0rc5/tests/data/sample_sboms/
+-rw-r--r--   0 runner    (1001) docker     (127)    15436 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/sample_sboms/helics_binaries_sbom.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/sample_sboms/helics_libs_sbom.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21305 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/sample_sboms/helics_sbom.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.362040 surfactant-0.0.0rc5/tests/data/srectest_no1/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/srectest_no1/HexFile.hex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.362040 surfactant-0.0.0rc5/tests/data_src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.362040 surfactant-0.0.0rc5/tests/data_src/NET_app_config_test_no1/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/NET_app_config_test_no1/App.config
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/NET_app_config_test_no1/ConsoleApp2.csproj
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/NET_app_config_test_no1/ConsoleApp2.sln
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/NET_app_config_test_no1/Program.cs
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/NET_app_config_test_no1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/NET_app_config_test_no1/hello.cs
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/NET_app_config_test_no1/hello.csproj
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/NET_app_config_test_no1/hello.sln
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.362040 surfactant-0.0.0rc5/tests/data_src/java_class_no1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/java_class_no1/HelloWorld.class
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/java_class_no1/HelloWorld.jar
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/java_class_no1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/java_class_no1/helloworld.java
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.366040 surfactant-0.0.0rc5/tests/data_src/msitest_no1/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/msitest_no1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/msitest_no1/hello.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16376 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/msitest_no1/hello.exe
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/msitest_no1/test.wxs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.366040 surfactant-0.0.0rc5/tests/data_src/native_shared_lib_test_no1/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/native_shared_lib_test_no1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/native_shared_lib_test_no1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/native_shared_lib_test_no1/hello_world.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.366040 surfactant-0.0.0rc5/tests/data_src/native_shared_lib_test_no1/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/native_shared_lib_test_no1/lib/testlib.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/native_shared_lib_test_no1/lib/testlib.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.366040 surfactant-0.0.0rc5/tests/data_src/srectest_no1/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/srectest_no1/BinaryFile.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/srectest_no1/HexFile.hex
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/srectest_no1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.366040 surfactant-0.0.0rc5/tests/file_types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/file_types/test_a_out_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/file_types/test_file_magic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.366040 surfactant-0.0.0rc5/tests/relationships/
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/relationships/test_dotnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-19 01:26:41.000000 surfactant-0.0.0rc5/tests/relationships/test_elf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-19 01:26:41.000000 surfactant-0.0.0rc5/tests/relationships/test_java.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-19 01:26:41.000000 surfactant-0.0.0rc5/tests/relationships/test_pe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-19 01:26:41.000000 surfactant-0.0.0rc5/tests/relationships/test_posix_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.366040 surfactant-0.0.0rc5/tests/symlink/
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-19 01:26:41.000000 surfactant-0.0.0rc5/tests/symlink/test_resolve_links.py
```

### Comparing `Surfactant-0.0.0rc4/.github/CODE_OF_CONDUCT.md` & `surfactant-0.0.0rc5/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/.github/ISSUE_TEMPLATE/bug_report.md` & `surfactant-0.0.0rc5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/.github/ISSUE_TEMPLATE/feature_request.md` & `surfactant-0.0.0rc5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/.github/PULL_REQUEST_TEMPLATE.md` & `surfactant-0.0.0rc5/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/.github/workflows/pytest.yml` & `surfactant-0.0.0rc5/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/.github/workflows/release.yml` & `surfactant-0.0.0rc5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/.gitignore` & `surfactant-0.0.0rc5/.gitignore`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/.gitlab-ci.yml` & `surfactant-0.0.0rc5/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/.pre-commit-config.yaml` & `surfactant-0.0.0rc5/.pre-commit-config.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,34 @@
 exclude: ^(.gitignore|generate_sbom.py|extract_file_info.py|pe_info.py)
 repos:
-  - repo: https://github.com/psf/black
-    rev: 24.2.0
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.3.7
     hooks:
-      - id: black
-        args: [--config=pyproject.toml, --line-length=100]
-  - repo: https://github.com/pycqa/isort
-    rev: 5.13.2
-    hooks:
-      - id: isort
-        args: ["--profile", "black", "--filter-files"]
-  - repo: https://github.com/pycqa/flake8
-    rev: 7.0.0
-    hooks:
-      - id: flake8
-        additional_dependencies: [flake8-bugbear]
+      # Run the linter
+      - id: ruff
+        args: [ --fix ]
+      # Run the formatter
+      - id: ruff-format
   - repo: https://github.com/pycqa/pylint
-    rev: v3.0.3
+    rev: v3.1.0
     hooks:
       - id: pylint
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: mixed-line-ending
       - id: end-of-file-fixer
       - id: trailing-whitespace
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-toml
       - id: check-json
       #- id: pretty-format-json
   - repo: https://github.com/shellcheck-py/shellcheck-py
-    rev: v0.9.0.6
+    rev: v0.10.0.1
     hooks:
       - id: shellcheck
         args: [-x]
 
 # Note: codespell will try to spell check file extensions that should not be changed
 #  - repo: https://github.com/codespell-project/codespell
 #    rev: v2.2.2
```

### Comparing `Surfactant-0.0.0rc4/.readthedocs.yaml` & `surfactant-0.0.0rc5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/CONTRIBUTING.md` & `surfactant-0.0.0rc5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/LICENSE` & `surfactant-0.0.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/NOTICE` & `surfactant-0.0.0rc5/NOTICE`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/PKG-INFO` & `surfactant-0.0.0rc5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Surfactant
-Version: 0.0.0rc4
+Version: 0.0.0rc5
 Summary: Modular framework to gather file information, analyze dependencies, and generate an SBOM
 Author-email: Ryan Mast <mast9@llnl.gov>, Levi Lloyd <lloyd27@llnl.gov>, Micaela Gallegos <gallegos31@llnl.gov>, Alexander Armstrong <armstrong48@llnl.gov>, Shayna Kapadia <kapadia2@llnl.gov>
 Maintainer-email: Ryan Mast <mast9@llnl.gov>
 License: MIT License
 Project-URL: Homepage, https://github.com/LLNL/Surfactant
 Project-URL: Discussions, https://github.com/LLNL/Surfactant/discussions
 Project-URL: Documentation, https://surfactant.readthedocs.io/en/latest/
@@ -35,15 +35,15 @@
 Requires-Dist: dataclasses_json
 Requires-Dist: pyelftools
 Requires-Dist: pefile
 Requires-Dist: dnfile
 Requires-Dist: olefile
 Requires-Dist: defusedxml
 Requires-Dist: spdx-tools==0.8.*
-Requires-Dist: cyclonedx-python-lib==6.4.1
+Requires-Dist: cyclonedx-python-lib==6.4.4
 Requires-Dist: pluggy
 Requires-Dist: click
 Requires-Dist: javatools>=1.6.0
 Requires-Dist: loguru
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: dev
```

### Comparing `Surfactant-0.0.0rc4/README.md` & `surfactant-0.0.0rc5/README.md`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/Surfactant.egg-info/PKG-INFO` & `surfactant-0.0.0rc5/Surfactant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Surfactant
-Version: 0.0.0rc4
+Version: 0.0.0rc5
 Summary: Modular framework to gather file information, analyze dependencies, and generate an SBOM
 Author-email: Ryan Mast <mast9@llnl.gov>, Levi Lloyd <lloyd27@llnl.gov>, Micaela Gallegos <gallegos31@llnl.gov>, Alexander Armstrong <armstrong48@llnl.gov>, Shayna Kapadia <kapadia2@llnl.gov>
 Maintainer-email: Ryan Mast <mast9@llnl.gov>
 License: MIT License
 Project-URL: Homepage, https://github.com/LLNL/Surfactant
 Project-URL: Discussions, https://github.com/LLNL/Surfactant/discussions
 Project-URL: Documentation, https://surfactant.readthedocs.io/en/latest/
@@ -35,15 +35,15 @@
 Requires-Dist: dataclasses_json
 Requires-Dist: pyelftools
 Requires-Dist: pefile
 Requires-Dist: dnfile
 Requires-Dist: olefile
 Requires-Dist: defusedxml
 Requires-Dist: spdx-tools==0.8.*
-Requires-Dist: cyclonedx-python-lib==6.4.1
+Requires-Dist: cyclonedx-python-lib==6.4.4
 Requires-Dist: pluggy
 Requires-Dist: click
 Requires-Dist: javatools>=1.6.0
 Requires-Dist: loguru
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: dev
```

### Comparing `Surfactant-0.0.0rc4/Surfactant.egg-info/SOURCES.txt` & `surfactant-0.0.0rc5/Surfactant.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.flake8
+.editorconfig
 .git_archival.txt
 .gitattributes
 .gitignore
 .gitlab-ci.yml
 .gitmodules
 .pre-commit-config.yaml
 .readthedocs.yaml
@@ -58,14 +58,17 @@
 plugins/angrimportfinder/surfactantplugin_angrimportfinder.py
 plugins/binary2strings/README.md
 plugins/binary2strings/pyproject.toml
 plugins/binary2strings/surfactantplugin_binary2strings.py
 plugins/checksec.py/README.md
 plugins/checksec.py/pyproject.toml
 plugins/checksec.py/surfactantplugin_checksec.py
+plugins/fuzzyhashes/README.md
+plugins/fuzzyhashes/pyproject.toml
+plugins/fuzzyhashes/surfactantplugin_fuzzyhashes.py
 plugins/syft/README.md
 plugins/syft/pyproject.toml
 plugins/syft/surfactantplugin_syft.py
 scripts/README-merge_sbom.md
 scripts/merge_additional_metadata.py
 scripts/merge_config.json
 scripts/merge_sbom.py
```

### Comparing `Surfactant-0.0.0rc4/docs/Makefile` & `surfactant-0.0.0rc5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/docs/basic_usage.md` & `surfactant-0.0.0rc5/docs/basic_usage.md`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/docs/conf.py` & `surfactant-0.0.0rc5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/docs/configuration_files.md` & `surfactant-0.0.0rc5/docs/configuration_files.md`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/docs/getting_started.md` & `surfactant-0.0.0rc5/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/docs/index.md` & `surfactant-0.0.0rc5/docs/index.md`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/docs/logos/surfactant-logo-dark-250px.png` & `surfactant-0.0.0rc5/docs/logos/surfactant-logo-dark-250px.png`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/docs/logos/surfactant-logo-dark.png` & `surfactant-0.0.0rc5/docs/logos/surfactant-logo-dark.png`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/docs/logos/surfactant-logo-light-250px.png` & `surfactant-0.0.0rc5/docs/logos/surfactant-logo-light-250px.png`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/docs/logos/surfactant-logo-light.png` & `surfactant-0.0.0rc5/docs/logos/surfactant-logo-light.png`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/docs/make.bat` & `surfactant-0.0.0rc5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/docs/plugins.md` & `surfactant-0.0.0rc5/docs/plugins.md`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/docs/windows_installer_tutorial/AutomatedInstallerWorkflowSetup.md` & `surfactant-0.0.0rc5/docs/windows_installer_tutorial/AutomatedInstallerWorkflowSetup.md`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/docs/windows_installer_tutorial/execinstaller.py` & `surfactant-0.0.0rc5/docs/windows_installer_tutorial/execinstaller.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" execinstaller.py """
+"""execinstaller.py"""
 
 import sys
 from json import dumps
 from logging import DEBUG, basicConfig, exception, info
 from os import getcwd, listdir, makedirs, mkdir, remove
 from os.path import abspath, exists
 from shutil import copy, copy2
```

### Comparing `Surfactant-0.0.0rc4/docs/windows_installer_tutorial/fsfilter.patch` & `surfactant-0.0.0rc5/docs/windows_installer_tutorial/fsfilter.patch`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/docs/windows_installer_tutorial/setupstepper.py` & `surfactant-0.0.0rc5/docs/windows_installer_tutorial/setupstepper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" setupstepper.py """
+"""setupstepper.py"""
 
 from json import loads
 from logging import DEBUG, basicConfig, exception, info
 from ntpath import basename
 from os import listdir, remove, system
 from os.path import exists
 from re import sub
```

### Comparing `Surfactant-0.0.0rc4/plugins/README.md` & `surfactant-0.0.0rc5/plugins/README.md`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/plugins/angrimportfinder/README.md` & `surfactant-0.0.0rc5/plugins/angrimportfinder/README.md`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/plugins/angrimportfinder/pyproject.toml` & `surfactant-0.0.0rc5/plugins/angrimportfinder/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/plugins/angrimportfinder/surfactantplugin_angrimportfinder.py` & `surfactant-0.0.0rc5/plugins/angrimportfinder/surfactantplugin_angrimportfinder.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/plugins/binary2strings/README.md` & `surfactant-0.0.0rc5/plugins/binary2strings/README.md`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/plugins/binary2strings/pyproject.toml` & `surfactant-0.0.0rc5/plugins/binary2strings/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/plugins/binary2strings/surfactantplugin_binary2strings.py` & `surfactant-0.0.0rc5/plugins/binary2strings/surfactantplugin_binary2strings.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/plugins/checksec.py/README.md` & `surfactant-0.0.0rc5/plugins/checksec.py/README.md`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/plugins/checksec.py/pyproject.toml` & `surfactant-0.0.0rc5/plugins/checksec.py/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/plugins/checksec.py/surfactantplugin_checksec.py` & `surfactant-0.0.0rc5/plugins/checksec.py/surfactantplugin_checksec.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/plugins/syft/README.md` & `surfactant-0.0.0rc5/plugins/syft/README.md`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/plugins/syft/pyproject.toml` & `surfactant-0.0.0rc5/plugins/syft/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/plugins/syft/surfactantplugin_syft.py` & `surfactant-0.0.0rc5/plugins/syft/surfactantplugin_syft.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/pyproject.toml` & `surfactant-0.0.0rc5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     "dataclasses_json",
     "pyelftools",
     "pefile",
     "dnfile",
     "olefile",
     "defusedxml",
     "spdx-tools==0.8.*",
-    "cyclonedx-python-lib==6.4.1",
+    "cyclonedx-python-lib==6.4.4",
     "pluggy",
     "click",
     "javatools>=1.6.0",
     "loguru"
 ]
 dynamic = ["version"]
 
@@ -75,14 +75,29 @@
 [tool.setuptools_scm]
 version_file = "surfactant/_version.py"
 
 [tool.pytest.ini_options]
 addopts = ["--import-mode=importlib"]
 pythonpath = "."
 
+[tool.ruff]
+line-length = 100
+indent-width = 4
+
+[tool.ruff.lint]
+# ruff defaults: E4, E7, E9, F
+select = ["E", "F", "B", "I"]
+ignore = ["E501", "F841"]
+# don't fix flake8-bugbear (`B`) violations
+unfixable = ["B"]
+
+# Ignore `E402` import violations in plugin manager
+[tool.ruff.lint.per-file-ignores]
+"surfactant/plugin/manager.py" = ["E402"]
+
 [tool.pylint.messages_control]
 max-line-length = "100"
 good-names-rgxs = "x,y,e,md,sw"
 disable = [
   "line-too-long",
   "missing-module-docstring",
   "missing-class-docstring",
```

### Comparing `Surfactant-0.0.0rc4/scripts/README-merge_sbom.md` & `surfactant-0.0.0rc5/scripts/README-merge_sbom.md`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/scripts/merge_additional_metadata.py` & `surfactant-0.0.0rc5/scripts/merge_additional_metadata.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/scripts/merge_sbom.py` & `surfactant-0.0.0rc5/scripts/merge_sbom.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/surfactant/__main__.py` & `surfactant-0.0.0rc5/surfactant/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,22 +15,29 @@
 from surfactant.cmd.createconfig import create_config
 from surfactant.cmd.generate import sbom as generate
 from surfactant.cmd.merge import merge_command
 from surfactant.cmd.stat import stat
 
 
 @click.group()
+@click.version_option(
+    importlib.metadata.version("surfactant"),
+    "--version",
+    "-v",
+    message="%(version)s",
+)
 @click.option(
     "--log-level",
     type=click.Choice(
-        ["TRACE", "DEBUG", "INFO", "SUCCESS", "WARNING", "ERROR", "CRITICAL"], case_sensitive=False
+        ["TRACE", "DEBUG", "INFO", "SUCCESS", "WARNING", "ERROR", "CRITICAL"],
+        case_sensitive=False,
     ),
     default="INFO",
 )
-def main(log_level):
+def main(log_level="INFO"):
     # Can't change the logging level; need to remove and add a new logger with the desired log level
     logger.remove()
     logger.add(sys.stderr, level=log_level)
 
 
 @click.command("version")
 def version():
@@ -53,8 +60,8 @@
 
 # CLI Subcommands
 cli.add_command(find)
 cli.add_command(edit)
 cli.add_command(add)
 
 if __name__ == "__main__":
-    main(log_level="INFO")
+    main()
```

### Comparing `Surfactant-0.0.0rc4/surfactant/cmd/cli.py` & `surfactant-0.0.0rc5/surfactant/cmd/cli.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/surfactant/cmd/createconfig.py` & `surfactant-0.0.0rc5/surfactant/cmd/createconfig.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/surfactant/cmd/generate.py` & `surfactant-0.0.0rc5/surfactant/cmd/generate.py`

 * *Files 3% similar despite different names*

```diff
@@ -225,15 +225,19 @@
 
     pm = get_plugin_manager()
     output_writer = find_io_plugin(pm, output_format, "write_sbom")
     input_reader = find_io_plugin(pm, input_format, "read_sbom")
 
     if pathlib.Path(config_file).is_file():
         with click.open_file(config_file) as f:
-            config = json.load(f)
+            try:
+                config = json.load(f)
+            except json.decoder.JSONDecodeError as err:
+                logger.exception(f"Invalid JSON in given config file ({config_file})")
+                raise SystemExit(f"Invalid JSON in given config file ({config_file})") from err
             # TODO: what if it isn't a JSON config file, but a single file to generate an SBOM for? perhaps file == "archive"?
     else:
         # Emulate a configuration file with the path
         config = []
         config.append({})
         config[0]["extractPaths"] = [config_file]
         config[0]["installPrefix"] = config_file
@@ -279,18 +283,29 @@
                 else:
                     new_sbom.add_software(parent_entry)
                 parent_uuid = parent_entry.UUID
             else:
                 parent_entry = None
                 parent_uuid = None
 
-            if entry.installPrefix and not entry.installPrefix.endswith(("/", "\\")):
-                # Make sure the installPrefix given ends with a "/" (or Windows backslash path, but users should avoid those)
-                logger.warning("Fixing install path")
-                entry.installPrefix += "/"
+            # If an installPrefix was given, clean it up some
+            if entry.installPrefix:
+                if not entry.installPrefix.endswith(("/", "\\")):
+                    # Make sure the installPrefix given ends with a "/" (or Windows backslash path, but users should avoid those)
+                    logger.warning(
+                        "Fixing installPrefix in config file entry (include the trailing /)"
+                    )
+                    entry.installPrefix += "/"
+                if "\\" in entry.installPrefix:
+                    # Using an install prefix with backslashes can result in a gradual reduction of the number of backslashes... and weirdness
+                    # Ideally even on a Windows "/" should be preferred instead in file paths, but "\" can be a valid character in Linux folder names
+                    logger.warning(
+                        "Fixing installPrefix with Windows-style backslash path separator in config file (ideally use / as path separator instead of \\, even for Windows"
+                    )
+                    entry.installPrefix = entry.installPrefix.replace("\\", "\\\\")
 
             for epath in entry.extractPaths:
                 # extractPath should not end with "/" (Windows-style backslash paths shouldn't be used at all)
                 if epath.endswith("/"):
                     epath = epath[:-1]
                 logger.trace("Extracted Path: " + str(epath))
                 for cdir, dirs, files in os.walk(epath):
```

### Comparing `Surfactant-0.0.0rc4/surfactant/cmd/merge.py` & `surfactant-0.0.0rc5/surfactant/cmd/merge.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,20 +49,31 @@
     """Merge two or more SBOMs."""
     merged_sbom = input_sboms[0]
     for sbom_m in input_sboms[1:]:
         merged_sbom.merge(sbom_m)
 
     rel_graph = construct_relationship_graph(merged_sbom)
     roots = get_roots_check_cycles(rel_graph)
+
+    # Check if provided UUID for a system object already exists to avoid creating a duplicate
+    add_system = True
+    if config and "system" in config:
+        if "UUID" in config["system"]:
+            for s in merged_sbom.systems:
+                if config["system"]["UUID"] == s.UUID:
+                    add_system = False
+                    break
+    # Even if not adding the system, create a dummy/placeholder with the UUID for creating relationships
     system = create_system_object(merged_sbom, config)
-    merged_sbom.systems.append(system)
+    if add_system:
+        merged_sbom.systems.append(system)
 
     # Add a system relationship to each root software/systems entry identified
     for r in roots:
-        merged_sbom.relationships.append(
+        merged_sbom.relationships.add(
             Relationship(xUUID=system["UUID"], yUUID=r, relationship="Includes")
         )
 
     output_writer.write_sbom(merged_sbom, sbom_outfile)
 
 
 def construct_relationship_graph(sbom: SBOM):
@@ -147,15 +158,15 @@
         config: The user specified config json (Optional).
 
     Returns:
         System: The created system object.
     """
 
     system = {}
-    if config:
+    if config and "system" in config:
         system = config["system"]
     # make sure the required fields are present and at least mostly valid
     if ("UUID" not in system) or not sbom.is_valid_uuid4(system["UUID"]):
         system["UUID"] = str(uuid_module.uuid4())
     if "name" not in system:
         system["name"] = ""
     captureStart = -1
@@ -167,8 +178,8 @@
         if captureEnd and sw.captureTime:
             if captureEnd == -1 or sw.captureTime > captureEnd:
                 captureEnd = sw.captureTime
     if "captureStart" not in system or not system["captureStart"]:
         system["captureStart"] = captureStart
     if "captureEnd" not in system or not system["captureEnd"]:
         system["captureEnd"] = captureEnd
-    return system
+    return System(**system)
```

### Comparing `Surfactant-0.0.0rc4/surfactant/cmd/stat.py` & `surfactant-0.0.0rc5/surfactant/cmd/stat.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/surfactant/fileinfo.py` & `surfactant-0.0.0rc5/surfactant/fileinfo.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/surfactant/filetypeid/id_extension.py` & `surfactant-0.0.0rc5/surfactant/filetypeid/id_extension.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/surfactant/filetypeid/id_hex.py` & `surfactant-0.0.0rc5/surfactant/filetypeid/id_hex.py`

 * *Files 7% similar despite different names*

```diff
@@ -88,9 +88,9 @@
                     percent_intel += 1
             if percent_intel > percent_motorola:
                 return "INTEL_HEX"
             if percent_motorola > percent_intel:
                 return "MOTOROLA_SREC"
             return None
 
-    except FileNotFoundError:
+    except (FileNotFoundError, UnicodeDecodeError):
         return None
```

### Comparing `Surfactant-0.0.0rc4/surfactant/filetypeid/id_magic.py` & `surfactant-0.0.0rc5/surfactant/filetypeid/id_magic.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
             # https://www.ibm.com/docs/en/aix/7.3?topic=formats-xcoff-object-file-format
             if magic_bytes[:2] == "\x1d\x00":
                 return "XCOFF32"
             if magic_bytes[:2] == "\xf7\x01":
                 return "XCOFF64"
             # ECOFF:
             # https://web.archive.org/web/20160305114748/http://h41361.www4.hp.com/docs/base_doc/DOCUMENTATION/V50A_ACRO_SUP/OBJSPEC.PDF
-            if magic_bytes[:2] in ("\x83\x01", "\x88\x01", "\x8F\x01"):
+            if magic_bytes[:2] in ("\x83\x01", "\x88\x01", "\x8f\x01"):
                 return "ECOFF"
             # AR:
             # https://www.garykessler.net/library/file_sigs.html
             if magic_bytes[:8] == b"!<arch>\n":
                 return "AR_LIB"
             # OMF:
             # https://github.com/file/file/blob/c8bba134ac1f3c9f5/magic/Magdir/msvc#L22
```

### Comparing `Surfactant-0.0.0rc4/surfactant/infoextractors/a_out_file.py` & `surfactant-0.0.0rc5/surfactant/infoextractors/a_out_file.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/surfactant/infoextractors/coff_file.py` & `surfactant-0.0.0rc5/surfactant/infoextractors/coff_file.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/surfactant/infoextractors/elf_file.py` & `surfactant-0.0.0rc5/surfactant/infoextractors/elf_file.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/surfactant/infoextractors/java_file.py` & `surfactant-0.0.0rc5/surfactant/infoextractors/java_file.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/surfactant/infoextractors/ole_file.py` & `surfactant-0.0.0rc5/surfactant/infoextractors/ole_file.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/surfactant/infoextractors/pe_file.py` & `surfactant-0.0.0rc5/surfactant/infoextractors/pe_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,21 +186,27 @@
     if app_config_info:
         file_details["appConfigFile"] = app_config_info
 
     return file_details
 
 
 def add_core_assembly_info(asm_dict, asm_info):
-    asm_dict["Name"] = asm_info.Name
-    asm_dict["Culture"] = asm_info.Culture
+    asm_dict["Name"] = asm_info.Name.value if hasattr(asm_info.Name, "value") else asm_info.Name
+    asm_dict["Culture"] = (
+        asm_info.Culture.value if hasattr(asm_info.Culture, "value") else asm_info.Culture
+    )
     asm_dict["Version"] = (
         f"{asm_info.MajorVersion}.{asm_info.MinorVersion}.{asm_info.BuildNumber}.{asm_info.RevisionNumber}"
     )
     asm_dict["PublicKey"] = (
-        asm_info.PublicKey.hex() if hasattr(asm_info.PublicKey, "hex") else asm_info.PublicKey
+        asm_info.PublicKey.hex()
+        if hasattr(asm_info.PublicKey, "hex")
+        else (
+            asm_info.PublicKey.value if hasattr(asm_info.PublicKey, "value") else asm_info.PublicKey
+        )
     )
 
 
 def add_assembly_flags_info(asm_dict, asm_info):
     # Info on flags
     # Processor Architecture fields/values: https://learn.microsoft.com/en-us/dotnet/api/system.reflection.processorarchitecture?view=net-6.0
     # PA enum values in dnfile: https://github.com/malwarefrank/dnfile/blob/7441fe326e0cc254ed2944a18773d8b4fe99c4c6/src/dnfile/enums.py#L663-L671
@@ -231,15 +237,19 @@
     add_assembly_flags_info(asm, asm_info)
     return asm
 
 
 def get_assemblyref_info(asmref_info):
     asmref: Dict[str, Any] = {}
     add_core_assembly_info(asmref, asmref_info)
-    asmref["HashValue"] = asmref_info.HashValue.hex()
+    asmref["HashValue"] = (
+        asmref_info.HashValue.hex()
+        if hasattr(asmref_info.HashValue, "hex")
+        else asmref_info.HashValue
+    )
     add_assembly_flags_info(asmref, asmref_info)
     return asmref
 
 
 def insert_implmap_info(im_info, imp_modules):
     dllName = im_info.ImportScope.row.Name
     methodName = im_info.ImportName
```

### Comparing `Surfactant-0.0.0rc4/surfactant/output/csv_writer.py` & `surfactant-0.0.0rc5/surfactant/output/csv_writer.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/surfactant/output/cyclonedx_writer.py` & `surfactant-0.0.0rc5/surfactant/output/cyclonedx_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,16 @@
     # due to being found within multiple different containers
     container_path_relationships: Dict[Tuple[str, str]] = {}
 
     for software in sbom.software:
         # Create CycloneDX Components for every software entry
         # start with software entries that act as containers for other software entries
         if sbom.has_relationship(xUUID=software.UUID, relationship="Contains"):
-            for _, container in convert_software_to_cyclonedx_container_components(software):
+            _, container_list = convert_software_to_cyclonedx_container_components(software)
+            for container in container_list:
                 bom.components.add(container)
         else:
             for parent_uuid, _, file in convert_software_to_cyclonedx_file_components(software):
                 bom.components.add(file)
                 if parent_uuid:
                     container_path_relationships[file.bom_ref.value] = parent_uuid
 
@@ -252,22 +253,28 @@
     if not hashes:
         hashes = None
 
     copyright_text = None
     if cr_text := get_fileinfo_metadata(software, "LegalCopyright"):
         copyright_text = cr_text  # free-form text field extracted from actual file identifying copyright holder and any dates present
 
+    if software.description == "":
+        software.description = None
+
+    if software.version == "":
+        software.version = None
+
     return Component(
         bom_ref=software.UUID,
         name=file_path,
         version=software.version,
         supplier=supplier,
         description=software.description,
         hashes=hashes,
-        copyright=copyright,
+        copyright=copyright_text,
         # components: Optional[Iterable['Component']]
         type=ComponentType.FILE,
     )
 
 
 def get_fileinfo_metadata(software: Software, field: str) -> Optional[str]:
     """Retrieves the value for a field in a 'FileInfo' metadata object in a software entry.
```

### Comparing `Surfactant-0.0.0rc4/surfactant/output/spdx_writer.py` & `surfactant-0.0.0rc5/surfactant/output/spdx_writer.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/surfactant/plugin/hookspecs.py` & `surfactant-0.0.0rc5/surfactant/plugin/hookspecs.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/surfactant/plugin/manager.py` & `surfactant-0.0.0rc5/surfactant/plugin/manager.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/surfactant/relationships/__init__.py` & `surfactant-0.0.0rc5/surfactant/relationships/__init__.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/surfactant/relationships/_internal/posix_utils.py` & `surfactant-0.0.0rc5/surfactant/relationships/_internal/posix_utils.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/surfactant/relationships/_internal/windows_utils.py` & `surfactant-0.0.0rc5/surfactant/relationships/_internal/windows_utils.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/surfactant/relationships/dotnet_relationship.py` & `surfactant-0.0.0rc5/surfactant/relationships/dotnet_relationship.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/surfactant/relationships/elf_relationship.py` & `surfactant-0.0.0rc5/surfactant/relationships/elf_relationship.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/surfactant/relationships/java_relationship.py` & `surfactant-0.0.0rc5/surfactant/relationships/java_relationship.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/surfactant/relationships/pe_relationship.py` & `surfactant-0.0.0rc5/surfactant/relationships/pe_relationship.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/surfactant/sbomtypes/__init__.py` & `surfactant-0.0.0rc5/surfactant/sbomtypes/__init__.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/surfactant/sbomtypes/_analysisdata.py` & `surfactant-0.0.0rc5/surfactant/sbomtypes/_analysisdata.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/surfactant/sbomtypes/_hardware.py` & `surfactant-0.0.0rc5/surfactant/sbomtypes/_hardware.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/surfactant/sbomtypes/_observation.py` & `surfactant-0.0.0rc5/surfactant/sbomtypes/_observation.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/surfactant/sbomtypes/_provenance.py` & `surfactant-0.0.0rc5/surfactant/sbomtypes/_provenance.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/surfactant/sbomtypes/_sbom.py` & `surfactant-0.0.0rc5/surfactant/sbomtypes/_sbom.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,76 +2,85 @@
 # See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 from __future__ import annotations
 
 import uuid as uuid_module
 from dataclasses import dataclass, field
-from typing import List, Optional
+from typing import Dict, List, Optional, Set
 
 from dataclasses_json import dataclass_json
 from loguru import logger
 
 from ._analysisdata import AnalysisData
 from ._file import File
 from ._hardware import Hardware
 from ._observation import Observation
 from ._provenance import SoftwareProvenance
 from ._relationship import Relationship, StarRelationship
 from ._software import Software, SoftwareComponent
 from ._system import System
 
+INTERNAL_FIELDS = {"software_lookup_by_sha256"}
+
 
 @dataclass_json
 @dataclass
 class SBOM:
+    # pylint: disable=R0902
     systems: List[System] = field(default_factory=list)
     hardware: List[Hardware] = field(default_factory=list)
     software: List[Software] = field(default_factory=list)
-    relationships: List[Relationship] = field(default_factory=list)
+    relationships: Set[Relationship] = field(default_factory=set)
     analysisData: List[AnalysisData] = field(default_factory=list)
     observations: List[Observation] = field(default_factory=list)
-    starRelationships: List[StarRelationship] = field(default_factory=list)
+    starRelationships: Set[StarRelationship] = field(default_factory=set)
+    software_lookup_by_sha256: Dict = field(default_factory=dict)
+
+    def __post_init__(self):
+        self.__dataclass_fields__ = {
+            k: v for k, v in self.__dataclass_fields__.items() if k not in INTERNAL_FIELDS
+        }
 
     def add_relationship(self, rel: Relationship) -> None:
-        self.relationships.append(rel)
+        self.relationships.add(rel)
 
     def create_relationship(self, xUUID: str, yUUID: str, relationship: str) -> Relationship:
         rel = Relationship(xUUID, yUUID, relationship)
-        self.relationships.append(rel)
+        self.relationships.add(rel)
         return rel
 
     def find_relationship_object(self, relationship: Relationship) -> bool:
         return relationship in self.relationships
 
     def find_relationship(self, xUUID: str, yUUID: str, relationship: str) -> bool:
         return Relationship(xUUID, yUUID, relationship) in self.relationships
 
     def has_relationship(
         self, xUUID: str = None, yUUID: str = None, relationship: str = None
     ) -> bool:
         for rel in self.relationships:
-            all_match = True
+            # We iterate until we find a relationship that meets all the conditions
             if xUUID and rel.xUUID != xUUID:
-                all_match = False
+                continue
             if yUUID and rel.yUUID != yUUID:
-                all_match = False
+                continue
             if relationship and rel.relationship.upper() != relationship.upper():
-                all_match = False
-            if all_match:
-                return True
+                continue
+            return True
         return False
 
     def find_software(self, sha256: Optional[str]) -> Optional[Software]:
-        for sw in self.software:
-            if sha256 == sw.sha256:
-                return sw
+        if sha256 in self.software_lookup_by_sha256:
+            return self.software_lookup_by_sha256[sha256]
         return None
 
     def add_software(self, sw: Software) -> None:
+        if sw.sha256 is not None:
+            self.software_lookup_by_sha256[sw.sha256] = sw
         self.software.append(sw)
 
     # pylint: disable=too-many-arguments
     def create_software(
         self,
         name: Optional[str] = None,
         size: Optional[int] = None,
@@ -110,14 +119,15 @@
             comments=comments,
             metadata=metadata,
             supplementaryFiles=supplementaryFiles,
             provenance=provenance,
             recordedInstitution=recordedInstitution,
             components=components,
         )
+        self.software_lookup_by_sha256[sw.sha256] = sw
         self.software.append(sw)
         return sw
 
     def merge(self, sbom_m: SBOM) -> SBOM:
         # merged_sbom = SBOM()
         # merged/old to new UUID map
         uuid_updates = {}
@@ -158,15 +168,15 @@
                 if existing_rel := self._find_relationship_entry(
                     xUUID=rel.xUUID,
                     yUUID=rel.yUUID,
                     relationship=rel.relationship,
                 ):
                     logger.info(f"DUPLICATE RELATIONSHIP: {existing_rel}")
                 else:
-                    self.relationships.append(rel)
+                    self.relationships.add(rel)
 
         # rewrite container path UUIDs using rewrite map/list
         for sw in self.software:
             if sw.containerPath:
                 for idx, path in enumerate(sw.containerPath):
                     u = path[:36]
                     # if container path starts with an invalid uuid4, sbom might not be valid
@@ -196,15 +206,15 @@
                 if existing_rel := self._find_star_relationship_entry(
                     xUUID=rel.xUUID,
                     yUUID=rel.yUUID,
                     relationship=rel.relationship,
                 ):
                     logger.info(f"DUPLICATE STAR RELATIONSHIP: {existing_rel}")
                 else:
-                    self.starRelationships.append(rel)
+                    self.starRelationships.add(rel)
 
     def _find_systems_entry(
         self, uuid: Optional[str] = None, name: Optional[str] = None
     ) -> Optional[System]:
         """Merge helper function to find and return
         the matching system entry in the provided sbom.
 
@@ -212,23 +222,21 @@
             uuid (Optional[str]): The uuid of the desired system entry.
             name (Optional[str]): The name of the desired system entry.
 
         Returns:
             Optional[System]: The system found that matches the given criteria, otherwise None.
         """
         for system in self.systems:
-            all_match = True
             if uuid:
                 if system.UUID != uuid:
-                    all_match = False
+                    continue
             if name:
                 if system.name != name:
-                    all_match = False
-            if all_match:
-                return system
+                    continue
+            return system
         return None
 
     def _find_software_entry(
         self,
         uuid: Optional[str] = None,
         sha256: Optional[str] = None,
         md5: Optional[str] = None,
@@ -282,26 +290,24 @@
             yUUID (Optional[str]): The yUUID of the desired relationship entry.
             relationship (Optional[str]): The relationship type of the desired relationship entry.
 
         Returns:
             Optional[Relationship]: The relationship entry found that matches the given criteria, otherwise None.
         """
         for rel in self.relationships:
-            all_match = True
             if xUUID:
                 if rel.xUUID != xUUID:
-                    all_match = False
+                    continue
             if yUUID:
                 if rel.yUUID != yUUID:
-                    all_match = False
+                    continue
             if relationship:
                 if rel.relationship != relationship:
-                    all_match = False
-            if all_match:
-                return rel
+                    continue
+            return rel
         return None
 
     def _find_star_relationship_entry(
         self,
         xUUID: Optional[str] = None,
         yUUID: Optional[str] = None,
         relationship: Optional[str] = None,
@@ -314,26 +320,24 @@
             yUUID (Optional[str]): The yUUID of the desired relationship entry.
             relationship (Optional[str]): The relationship type of the desired relationship entry.
 
         Returns:
             Optional[StarRelationship]: The star relationship found that matches the given criteria, otherwise None.
         """
         for rel in self.starRelationships:
-            all_match = True
             if xUUID:
                 if rel.xUUID != xUUID:
-                    all_match = False
+                    continue
             if yUUID:
                 if rel.yUUID != yUUID:
-                    all_match = False
+                    continue
             if relationship:
                 if rel.relationship != relationship:
-                    all_match = False
-            if all_match:
-                return rel
+                    continue
+            return rel
         return None
 
     def is_valid_uuid4(self, u: str) -> bool:
         """Merge helper function to check if a uuid is valid.
 
         Args:
             u (str):  The UUID to check.
```

### Comparing `Surfactant-0.0.0rc4/surfactant/sbomtypes/_software.py` & `surfactant-0.0.0rc5/surfactant/sbomtypes/_software.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/surfactant/sbomtypes/_system.py` & `surfactant-0.0.0rc5/surfactant/sbomtypes/_system.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/tests/cmd/test_cli.py` & `surfactant-0.0.0rc5/tests/cmd/test_cli.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/tests/cmd/test_generate.py` & `surfactant-0.0.0rc5/tests/cmd/test_generate.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/tests/cmd/test_merge.py` & `surfactant-0.0.0rc5/tests/cmd/test_merge.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,88 +9,125 @@
 import random
 import string
 
 import pytest
 
 from surfactant.cmd.merge import merge
 from surfactant.plugin.manager import get_plugin_manager
-from surfactant.sbomtypes import SBOM, Relationship, Software
+from surfactant.sbomtypes import SBOM, Relationship
 
 # Generate Sample SBOMs
-sbom1 = SBOM(
-    software=[
-        Software(UUID="dd6f7f6b-7c31-4a4a-afef-14678b9942bf", fileName=["helics.tar.gz"]),
-        Software(
-            UUID="08526f02-8f08-485d-bfd1-ea16ce964fd2",
-            fileName=["helics_binary"],
-            installPath=["/bin/helics_binary"],
-            containerPath=["dd6f7f6b-7c31-4a4a-afef-14678b9942bf/bin/helics_binary"],
-        ),
-        Software(
-            UUID="a5db7e12-fe3d-490e-90b8-98a8bfaace09",
-            fileName=["lib1.so"],
-            installPath=["/lib64/lib1.so"],
-            containerPath=["dd6f7f6b-7c31-4a4a-afef-14678b9942bf/lib64/lib1.so"],
-        ),
-    ],
-    relationships=[
-        Relationship(
-            xUUID="08526f02-8f08-485d-bfd1-ea16ce964fd2",
-            yUUID="a5db7e12-fe3d-490e-90b8-98a8bfaace09",
-            relationship="Uses",
-        ),
-        Relationship(
-            xUUID="dd6f7f6b-7c31-4a4a-afef-14678b9942bf",
-            yUUID="08526f02-8f08-485d-bfd1-ea16ce964fd2",
-            relationship="Contains",
-        ),
-        Relationship(
-            xUUID="dd6f7f6b-7c31-4a4a-afef-14678b9942bf",
-            yUUID="a5db7e12-fe3d-490e-90b8-98a8bfaace09",
-            relationship="Contains",
-        ),
-    ],
+sbom1 = SBOM.from_json(
+    """{
+  "software": [
+    {
+      "UUID": "dd6f7f6b-7c31-4a4a-afef-14678b9942bf",
+      "fileName": [
+        "helics.tar.gz"
+      ]
+    },
+    {
+      "UUID": "08526f02-8f08-485d-bfd1-ea16ce964fd2",
+      "fileName": [
+        "helics_binary"
+      ],
+      "installPath": [
+        "/bin/helics_binary"
+      ],
+      "containerPath": [
+        "dd6f7f6b-7c31-4a4a-afef-14678b9942bf/bin/helics_binary"
+      ]
+    },
+    {
+      "UUID": "a5db7e12-fe3d-490e-90b8-98a8bfaace09",
+      "fileName": [
+        "lib1.so"
+      ],
+      "installPath": [
+        "/lib64/lib1.so"
+      ],
+      "containerPath": [
+        "dd6f7f6b-7c31-4a4a-afef-14678b9942bf/lib64/lib1.so"
+      ]
+    }
+  ],
+  "relationships": [
+    {
+      "xUUID": "08526f02-8f08-485d-bfd1-ea16ce964fd2",
+      "yUUID": "a5db7e12-fe3d-490e-90b8-98a8bfaace09",
+      "relationship": "Uses"
+    },
+    {
+      "xUUID": "dd6f7f6b-7c31-4a4a-afef-14678b9942bf",
+      "yUUID": "08526f02-8f08-485d-bfd1-ea16ce964fd2",
+      "relationship": "Contains"
+    },
+    {
+      "xUUID": "dd6f7f6b-7c31-4a4a-afef-14678b9942bf",
+      "yUUID": "a5db7e12-fe3d-490e-90b8-98a8bfaace09",
+      "relationship": "Contains"
+    }
+  ]
+}"""
 )
 
-sbom2 = SBOM(
-    software=[
-        Software(
-            UUID="625a07da-7eed-47b9-a0fa-47dcbf76574a",
-            fileName=["helics_plugin.tar.gz"],
-        ),
-        Software(
-            UUID="820d3ddc-14d7-4ce5-833c-beede8725366",
-            fileName=["helics_plugin"],
-            installPath=["/bin/helics_plugin"],
-            containerPath=["625a07da-7eed-47b9-a0fa-47dcbf76574a/bin/helics_plugin"],
-        ),
-        Software(
-            UUID="df81b6a7-f9df-42f1-85ee-86a8865fa5f1",
-            fileName=["lib_plugin.so"],
-            installPath=["/lib64/lib_plugin.so"],
-            containerPath=["625a07da-7eed-47b9-a0fa-47dcbf76574a/lib64/lib_plugin.so"],
-        ),
-    ],
-    relationships=[
-        Relationship(
-            xUUID="820d3ddc-14d7-4ce5-833c-beede8725366",
-            yUUID="df81b6a7-f9df-42f1-85ee-86a8865fa5f1",
-            relationship="Uses",
-        ),
-        Relationship(
-            xUUID="625a07da-7eed-47b9-a0fa-47dcbf76574a",
-            yUUID="820d3ddc-14d7-4ce5-833c-beede8725366",
-            relationship="Contains",
-        ),
-        Relationship(
-            xUUID="625a07da-7eed-47b9-a0fa-47dcbf76574a",
-            yUUID="df81b6a7-f9df-42f1-85ee-86a8865fa5f1",
-            relationship="Contains",
-        ),
-    ],
+sbom2 = SBOM.from_json(
+    """{
+        "software": [
+            {
+            "UUID": "625a07da-7eed-47b9-a0fa-47dcbf76574a",
+            "name": null,
+            "size": null,
+            "fileName": [
+                "helics_plugin.tar.gz"
+            ]
+            },
+            {
+            "UUID": "820d3ddc-14d7-4ce5-833c-beede8725366",
+            "fileName": [
+                "helics_plugin"
+            ],
+            "installPath": [
+                "/bin/helics_plugin"
+            ],
+            "containerPath": [
+                "625a07da-7eed-47b9-a0fa-47dcbf76574a/bin/helics_plugin"
+            ]
+            },
+            {
+            "UUID": "df81b6a7-f9df-42f1-85ee-86a8865fa5f1",
+            "fileName": [
+                "lib_plugin.so"
+            ],
+            "installPath": [
+                "/lib64/lib_plugin.so"
+            ],
+            "containerPath": [
+                "625a07da-7eed-47b9-a0fa-47dcbf76574a/lib64/lib_plugin.so"
+            ]
+            }
+        ],
+        "relationships": [
+            {
+            "xUUID": "820d3ddc-14d7-4ce5-833c-beede8725366",
+            "yUUID": "df81b6a7-f9df-42f1-85ee-86a8865fa5f1",
+            "relationship": "Uses"
+            },
+            {
+            "xUUID": "625a07da-7eed-47b9-a0fa-47dcbf76574a",
+            "yUUID": "820d3ddc-14d7-4ce5-833c-beede8725366",
+            "relationship": "Contains"
+            },
+            {
+            "xUUID": "625a07da-7eed-47b9-a0fa-47dcbf76574a",
+            "yUUID": "df81b6a7-f9df-42f1-85ee-86a8865fa5f1",
+            "relationship": "Contains"
+            }
+        ]
+        }"""
 )
 
 sbom3 = None
 sbom4 = None
 
 config = {
     "system": {
@@ -99,39 +136,40 @@
         "vendor": None,
         "captureStart": 1689186121,
         "captureEnd": 1689186146,
     }
 }
 
 with open(
-    pathlib.Path(__file__).parent / "../data/sample_sboms/helics_binaries_sbom.json", "r"
+    pathlib.Path(__file__).parent / "../data/sample_sboms/helics_binaries_sbom.json",
+    "r",
 ) as f:
     sbom3 = SBOM.from_json(f.read())
 with open(pathlib.Path(__file__).parent / "../data/sample_sboms/helics_libs_sbom.json", "r") as f:
     sbom4 = SBOM.from_json(f.read())
 
 
 # Test Functions
 def test_simple_merge_method():
     merged_sbom = sbom1
     merged_sbom.merge(sbom2)
     softwares = sbom1.software
     softwares.extend(sbom2.software)
     assert merged_sbom.software.sort(key=lambda x: x.UUID) == softwares.sort(key=lambda x: x.UUID)
     relations = sbom1.relationships
-    relations.extend(sbom2.relationships)
-    assert merged_sbom.relationships.sort(key=lambda x: x.xUUID) == relations.sort(
-        key=lambda x: x.xUUID
+    relations.update(sbom2.relationships)
+    assert sorted(merged_sbom.relationships, key=lambda x: x.xUUID) == sorted(
+        relations, key=lambda x: x.xUUID
     )
 
 
 @pytest.mark.skip(reason="No way of validating this test yet")
 def test_merge_with_circular_dependency():
     circular_dependency_sbom = sbom1
-    circular_dependency_sbom.relationships.append(
+    circular_dependency_sbom.relationships.add(
         Relationship(
             xUUID="a5db7e12-fe3d-490e-90b8-98a8bfaace09",
             yUUID="dd6f7f6b-7c31-4a4a-afef-14678b9942bf",
             relationship="Contains",
         )
     )
```

### Comparing `Surfactant-0.0.0rc4/tests/data/ELF_shared_obj_test_no1/bin/hello_world` & `surfactant-0.0.0rc5/tests/data/ELF_shared_obj_test_no1/bin/hello_world`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/tests/data/ELF_shared_obj_test_no1/lib/libtestlib.so` & `surfactant-0.0.0rc5/tests/data/ELF_shared_obj_test_no1/lib/libtestlib.so`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/tests/data/NET_app_config_test_no1/ConsoleApp2.exe` & `surfactant-0.0.0rc5/tests/data/NET_app_config_test_no1/ConsoleApp2.exe`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/tests/data/NET_app_config_test_no1/bin/Debug/net6.0/hello.dll` & `surfactant-0.0.0rc5/tests/data/NET_app_config_test_no1/bin/Debug/net6.0/hello.dll`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/tests/data/Windows_dll_test_no1/hello_world.exe` & `surfactant-0.0.0rc5/tests/data/Windows_dll_test_no1/hello_world.exe`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/tests/data/Windows_dll_test_no1/testlib.dll` & `surfactant-0.0.0rc5/tests/data/Windows_dll_test_no1/testlib.dll`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/tests/data/java_class_no1/HelloWorld.class` & `surfactant-0.0.0rc5/tests/data/java_class_no1/HelloWorld.class`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/tests/data/mach_o_dylib_test_no1/bin/hello_world` & `surfactant-0.0.0rc5/tests/data/mach_o_dylib_test_no1/bin/hello_world`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/tests/data/mach_o_dylib_test_no1/lib/libtestlib.dylib` & `surfactant-0.0.0rc5/tests/data/mach_o_dylib_test_no1/lib/libtestlib.dylib`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/tests/data/msitest_no1/test.msi` & `surfactant-0.0.0rc5/tests/data/msitest_no1/test.msi`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/tests/data/sample_sboms/helics_binaries_sbom.json` & `surfactant-0.0.0rc5/tests/data/sample_sboms/helics_binaries_sbom.json`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/tests/data/sample_sboms/helics_libs_sbom.json` & `surfactant-0.0.0rc5/tests/data/sample_sboms/helics_libs_sbom.json`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/tests/data/sample_sboms/helics_sbom.json` & `surfactant-0.0.0rc5/tests/data/sample_sboms/helics_sbom.json`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/tests/data_src/NET_app_config_test_no1/ConsoleApp2.sln` & `surfactant-0.0.0rc5/tests/data_src/NET_app_config_test_no1/ConsoleApp2.sln`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/tests/data_src/NET_app_config_test_no1/README.md` & `surfactant-0.0.0rc5/tests/data_src/NET_app_config_test_no1/README.md`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/tests/data_src/NET_app_config_test_no1/hello.sln` & `surfactant-0.0.0rc5/tests/data_src/NET_app_config_test_no1/hello.sln`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/tests/data_src/README.md` & `surfactant-0.0.0rc5/tests/data_src/README.md`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/tests/data_src/java_class_no1/HelloWorld.class` & `surfactant-0.0.0rc5/tests/data_src/java_class_no1/HelloWorld.class`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/tests/data_src/java_class_no1/HelloWorld.jar` & `surfactant-0.0.0rc5/tests/data_src/java_class_no1/HelloWorld.jar`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/tests/data_src/msitest_no1/hello.exe` & `surfactant-0.0.0rc5/tests/data_src/msitest_no1/hello.exe`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/tests/data_src/msitest_no1/test.wxs` & `surfactant-0.0.0rc5/tests/data_src/msitest_no1/test.wxs`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/tests/data_src/native_shared_lib_test_no1/CMakeLists.txt` & `surfactant-0.0.0rc5/tests/data_src/native_shared_lib_test_no1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/tests/data_src/native_shared_lib_test_no1/README.md` & `surfactant-0.0.0rc5/tests/data_src/native_shared_lib_test_no1/README.md`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/tests/file_types/test_a_out_files.py` & `surfactant-0.0.0rc5/tests/file_types/test_a_out_files.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/tests/file_types/test_file_magic.py` & `surfactant-0.0.0rc5/tests/file_types/test_file_magic.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/tests/relationships/test_dotnet.py` & `surfactant-0.0.0rc5/tests/relationships/test_dotnet.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/tests/relationships/test_elf.py` & `surfactant-0.0.0rc5/tests/relationships/test_elf.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/tests/relationships/test_java.py` & `surfactant-0.0.0rc5/tests/relationships/test_java.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/tests/relationships/test_pe.py` & `surfactant-0.0.0rc5/tests/relationships/test_pe.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/tests/relationships/test_posix_utils.py` & `surfactant-0.0.0rc5/tests/relationships/test_posix_utils.py`

 * *Files identical despite different names*

### Comparing `Surfactant-0.0.0rc4/tests/symlink/test_resolve_links.py` & `surfactant-0.0.0rc5/tests/symlink/test_resolve_links.py`

 * *Files identical despite different names*

