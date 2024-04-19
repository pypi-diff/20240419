# Comparing `tmp/plex-api-client-0.6.2.tar.gz` & `tmp/plex-api-client-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plex-api-client-0.6.2.tar", last modified: Tue Apr  9 01:14:59 2024, max compression
+gzip compressed data, was "plex-api-client-0.6.3.tar", last modified: Fri Apr 19 01:15:37 2024, max compression
```

## Comparing `plex-api-client-0.6.2.tar` & `plex-api-client-0.6.3.tar`

### file list

```diff
@@ -1,169 +1,172 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:14:59.313967 plex-api-client-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    21032 2024-04-09 01:14:59.313967 plex-api-client-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14178 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 01:14:59.313967 plex-api-client-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:14:59.289967 plex-api-client-0.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:14:59.293967 plex-api-client-0.6.2/src/plex_api/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:14:59.293967 plex-api-client-0.6.2/src/plex_api/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/activities.py
--rw-r--r--   0 runner    (1001) docker     (127)     7827 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)    18207 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/butler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8526 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/hubs.py
--rw-r--r--   0 runner    (1001) docker     (127)    42834 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/library.py
--rw-r--r--   0 runner    (1001) docker     (127)    11991 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    10434 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/media.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:14:59.293967 plex-api-client-0.6.2/src/plex_api/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:14:59.293967 plex-api-client-0.6.2/src/plex_api/models/components/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/components/security.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:14:59.301967 plex-api-client-0.6.2/src/plex_api/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/addplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/applyupdates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/cancelserveractivities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/checkforupdates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/clearplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/createplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/deletelibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/deleteplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/enablepapertrail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getavailableclients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getbutlertasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getdevices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getfilehash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getglobalhubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getlibraries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getlibraryhubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getmetadatachildren.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getmyplexaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getondeck.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getpin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getplaylists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getrecentlyadded.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getresizedphoto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getsearchresults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getserveractivities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getservercapabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getserveridentity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getserverlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getserverpreferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getsessionhistory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getsessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getsourceconnectioninformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getstatistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/gettimeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/gettoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/gettranscodesessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/gettransienttoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getupdatestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/logline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/logmultiline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/markplayed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/markunplayed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/performsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/performvoicesearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/refreshlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/sdkerror.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/startalltasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/starttask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/startuniversaltranscode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/stopalltasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/stoptask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/stoptranscodesession.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/updateplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/updateplayprogress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/uploadplaylist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:14:59.313967 plex-api-client-0.6.2/src/plex_api/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/addplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/applyupdates.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/cancelserveractivities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/checkforupdates.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/clearplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/createplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/deletelibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/deleteplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/enablepapertrail.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getavailableclients.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getbutlertasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getdevices.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getfilehash.py
--rw-r--r--   0 runner    (1001) docker     (127)     7952 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getglobalhubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getlibraries.py
--rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)    18873 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getlibraryhubs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21445 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getlibraryitems.py
--rw-r--r--   0 runner    (1001) docker     (127)    26862 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getmetadatachildren.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getmyplexaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)    18560 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getondeck.py
--rw-r--r--   0 runner    (1001) docker     (127)     6235 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getpin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)    16058 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getplaylists.py
--rw-r--r--   0 runner    (1001) docker     (127)    14896 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getrecentlyadded.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getresizedphoto.py
--rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getsearchresults.py
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getserveractivities.py
--rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getservercapabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getserveridentity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getserverlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getserverpreferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getsessionhistory.py
--rw-r--r--   0 runner    (1001) docker     (127)    19635 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getsessions.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getsourceconnectioninformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getstatistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/gettimeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/gettoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/gettranscodesessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/gettransienttoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getupdatestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/logline.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/logmultiline.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/markplayed.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/markunplayed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/performsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/performvoicesearch.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/refreshlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/searchlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/startalltasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/starttask.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/startuniversaltranscode.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/stopalltasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/stoptask.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/stoptranscodesession.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/updateplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/updateplayprogress.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/uploadplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)    34763 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/playlists.py
--rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/plex.py
--rw-r--r--   0 runner    (1001) docker     (127)     8014 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    13517 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    28067 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    14387 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    10953 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:14:59.313967 plex-api-client-0.6.2/src/plex_api/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    30026 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:14:59.313967 plex-api-client-0.6.2/src/plex_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21032 2024-04-09 01:14:59.000000 plex-api-client-0.6.2/src/plex_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-04-09 01:14:59.000000 plex-api-client-0.6.2/src/plex_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 01:14:59.000000 plex-api-client-0.6.2/src/plex_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-09 01:14:59.000000 plex-api-client-0.6.2/src/plex_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 01:14:59.000000 plex-api-client-0.6.2/src/plex_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:15:37.852731 plex-api-client-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    21032 2024-04-19 01:15:37.852731 plex-api-client-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14178 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 01:15:37.852731 plex-api-client-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:15:37.828730 plex-api-client-0.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:15:37.832731 plex-api-client-0.6.3/src/plex_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:15:37.832731 plex-api-client-0.6.3/src/plex_api/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18086 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/hubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42185 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11932 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10238 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/media.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:15:37.832731 plex-api-client-0.6.3/src/plex_api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:15:37.832731 plex-api-client-0.6.3/src/plex_api/models/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/components/security.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:15:37.840731 plex-api-client-0.6.3/src/plex_api/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/addplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/applyupdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/cancelserveractivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/checkforupdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/clearplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/createplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/deletelibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/deleteplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/enablepapertrail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/getavailableclients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/getbutlertasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/getdevices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/getfilehash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/getglobalhubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/getlibraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/getlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/getlibraryhubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/getmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/getmetadatachildren.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/getmyplexaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/getondeck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/getpin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/getplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/getplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/getplaylists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/getrecentlyadded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/getresizedphoto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/getsearchresults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/getserveractivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/getservercapabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/getserveridentity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/getserverlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/getserverpreferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/getsessionhistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/getsessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/getsourceconnectioninformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/getstatistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/gettimeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/gettoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/gettranscodesessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/gettransienttoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/getupdatestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/logline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/logmultiline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/markplayed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/markunplayed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/performsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/performvoicesearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/refreshlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/sdkerror.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/startalltasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/starttask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/startuniversaltranscode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/stopalltasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/stoptask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/stoptranscodesession.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/updateplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/updateplayprogress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/errors/uploadplaylist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:15:37.840731 plex-api-client-0.6.3/src/plex_api/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/internal/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:15:37.852731 plex-api-client-0.6.3/src/plex_api/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/addplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/applyupdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/cancelserveractivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/checkforupdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/clearplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/createplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/deletelibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/deleteplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/enablepapertrail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/getavailableclients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/getbutlertasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/getdevices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/getfilehash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7952 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/getglobalhubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/getlibraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/getlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18873 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/getlibraryhubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21445 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/getlibraryitems.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26862 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/getmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/getmetadatachildren.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/getmyplexaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18560 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/getondeck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/getpin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/getplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16058 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/getplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/getplaylists.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14896 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/getrecentlyadded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/getresizedphoto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/getsearchresults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/getserveractivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/getservercapabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/getserveridentity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/getserverlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/getserverpreferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/getsessionhistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19635 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/getsessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/getsourceconnectioninformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/getstatistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/gettimeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/gettoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/gettranscodesessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/gettransienttoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/getupdatestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/logline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/logmultiline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/markplayed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/markunplayed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/performsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/performvoicesearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/refreshlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/searchlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/startalltasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/starttask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/startuniversaltranscode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/stopalltasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/stoptask.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/stoptranscodesession.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/updateplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/updateplayprogress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/models/operations/uploadplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33949 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/playlists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7880 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/plex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13314 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28000 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14315 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10822 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:15:37.852731 plex-api-client-0.6.3/src/plex_api/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32093 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-04-19 01:15:25.000000 plex-api-client-0.6.3/src/plex_api/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:15:37.852731 plex-api-client-0.6.3/src/plex_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21032 2024-04-19 01:15:37.000000 plex-api-client-0.6.3/src/plex_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-04-19 01:15:37.000000 plex-api-client-0.6.3/src/plex_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 01:15:37.000000 plex-api-client-0.6.3/src/plex_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-19 01:15:37.000000 plex-api-client-0.6.3/src/plex_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 01:15:37.000000 plex-api-client-0.6.3/src/plex_api_client.egg-info/top_level.txt
```

### Comparing `plex-api-client-0.6.2/LICENSE.md` & `plex-api-client-0.6.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/PKG-INFO` & `plex-api-client-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-api-client
-Version: 0.6.2
+Version: 0.6.3
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/LukeHagar/plexpy.git
 Author: LukeHagar
 License: UNKNOWN
 Description: # plexpy
         
         <div align="left">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plex-api-client Version: 0.6.2 Summary: Python
+Metadata-Version: 2.1 Name: plex-api-client Version: 0.6.3 Summary: Python
 Client SDK Generated by Speakeasy Home-page: https://github.com/LukeHagar/
 plexpy.git Author: LukeHagar License: UNKNOWN Description: # plexpy
 _[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
 _2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]
 ## SDK Installation ```bash pip install plex-api-client ``` ## SDK Example
 Usage ### Example ```python import plex_api s = plex_api.PlexAPI
```

### Comparing `plex-api-client-0.6.2/README.md` & `plex-api-client-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/setup.py` & `plex-api-client-0.6.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='plex-api-client',
-    version='0.6.2',
+    version='0.6.3',
     author='LukeHagar',
     description='Python Client SDK Generated by Speakeasy',
     url='https://github.com/LukeHagar/plexpy.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `plex-api-client-0.6.2/src/plex_api/_hooks/registration.py` & `plex-api-client-0.6.3/src/plex_api/_hooks/registration.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/_hooks/sdkhooks.py` & `plex-api-client-0.6.3/src/plex_api/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/_hooks/types.py` & `plex-api-client-0.6.3/src/plex_api/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/activities.py` & `plex-api-client-0.6.3/src/plex_api/activities.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         hook_ctx = HookContext(operation_id='cancelServerActivities', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.CancelServerActivitiesRequest(
             activity_uuid=activity_uuid,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CancelServerActivitiesRequest, base_url, '/activities/{activityUUID}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/activities/{activityUUID}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
```

### Comparing `plex-api-client-0.6.2/src/plex_api/authentication.py` & `plex-api-client-0.6.3/src/plex_api/authentication.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         url = base_url + '/security/token'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetTransientTokenRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -95,15 +95,15 @@
         url = base_url + '/security/resources'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetSourceConnectionInformationRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `plex-api-client-0.6.2/src/plex_api/butler.py` & `plex-api-client-0.6.3/src/plex_api/butler.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,15 @@
         hook_ctx = HookContext(operation_id='startTask', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.StartTaskRequest(
             task_name=task_name,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.StartTaskRequest, base_url, '/butler/{taskName}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/butler/{taskName}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -276,15 +276,15 @@
         hook_ctx = HookContext(operation_id='stopTask', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.StopTaskRequest(
             task_name=task_name,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.StopTaskRequest, base_url, '/butler/{taskName}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/butler/{taskName}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
```

### Comparing `plex-api-client-0.6.2/src/plex_api/hubs.py` & `plex-api-client-0.6.3/src/plex_api/hubs.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         url = base_url + '/hubs'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetGlobalHubsRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -95,22 +95,22 @@
             section_id=section_id,
             count=count,
             only_transient=only_transient,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetLibraryHubsRequest, base_url, '/hubs/sections/{sectionId}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/hubs/sections/{sectionId}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetLibraryHubsRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `plex-api-client-0.6.2/src/plex_api/library.py` & `plex-api-client-0.6.3/src/plex_api/library.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         url = base_url + '/library/hashes'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetFileHashRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -260,22 +260,22 @@
         request = operations.GetLibraryRequest(
             section_id=section_id,
             include_details=include_details,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetLibraryRequest, base_url, '/library/sections/{sectionId}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/library/sections/{sectionId}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetLibraryRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -329,15 +329,15 @@
         hook_ctx = HookContext(operation_id='deleteLibrary', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.DeleteLibraryRequest(
             section_id=section_id,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.DeleteLibraryRequest, base_url, '/library/sections/{sectionId}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/library/sections/{sectionId}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -412,15 +412,15 @@
         request = operations.GetLibraryItemsRequest(
             section_id=section_id,
             tag=tag,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetLibraryItemsRequest, base_url, '/library/sections/{sectionId}/{tag}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/library/sections/{sectionId}/{tag}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -472,15 +472,15 @@
         hook_ctx = HookContext(operation_id='refreshLibrary', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.RefreshLibraryRequest(
             section_id=section_id,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RefreshLibraryRequest, base_url, '/library/sections/{sectionId}/refresh', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/library/sections/{sectionId}/refresh', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -553,22 +553,22 @@
         request = operations.SearchLibraryRequest(
             section_id=section_id,
             type=type_,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.SearchLibraryRequest, base_url, '/library/sections/{sectionId}/search', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/library/sections/{sectionId}/search', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.SearchLibraryRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -614,15 +614,15 @@
         hook_ctx = HookContext(operation_id='getMetadata', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.GetMetadataRequest(
             rating_key=rating_key,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetMetadataRequest, base_url, '/library/metadata/{ratingKey}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/library/metadata/{ratingKey}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -682,15 +682,15 @@
         hook_ctx = HookContext(operation_id='getMetadataChildren', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.GetMetadataChildrenRequest(
             rating_key=rating_key,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetMetadataChildrenRequest, base_url, '/library/metadata/{ratingKey}/children', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/library/metadata/{ratingKey}/children', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
```

### Comparing `plex-api-client-0.6.2/src/plex_api/log.py` & `plex-api-client-0.6.3/src/plex_api/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         url = base_url + '/log'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.LogLineRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `plex-api-client-0.6.2/src/plex_api/media.py` & `plex-api-client-0.6.3/src/plex_api/media.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         url = base_url + '/:/scrobble'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.MarkPlayedRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -93,15 +93,15 @@
         url = base_url + '/:/unscrobble'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.MarkUnplayedRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -159,15 +159,15 @@
         url = base_url + '/:/progress'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.UpdatePlayProgressRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/__init__.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/addplaylistcontents.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/addplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/applyupdates.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/applyupdates.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/cancelserveractivities.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/cancelserveractivities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/checkforupdates.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/checkforupdates.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/clearplaylistcontents.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/clearplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/createplaylist.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/createplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/deletelibrary.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/deletelibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/deleteplaylist.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/deleteplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/enablepapertrail.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/enablepapertrail.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/getavailableclients.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/getavailableclients.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/getbutlertasks.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/getbutlertasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/getdevices.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/getdevices.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/getfilehash.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/getfilehash.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/getglobalhubs.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/getglobalhubs.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/getlibraries.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/getlibraries.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/getlibrary.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/getlibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/getlibraryhubs.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/getlibraryhubs.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/getmetadata.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/getmetadata.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/getmetadatachildren.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/getmetadatachildren.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/getmyplexaccount.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/getmyplexaccount.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/getondeck.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/getondeck.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/getpin.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/getpin.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/getplaylist.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/getplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/getplaylistcontents.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/getplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/getplaylists.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/getplaylists.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/getrecentlyadded.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/getrecentlyadded.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/getresizedphoto.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/getresizedphoto.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/getsearchresults.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/getsearchresults.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/getserveractivities.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/getserveractivities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/getservercapabilities.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/getservercapabilities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/getserveridentity.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/getserveridentity.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/getserverlist.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/getserverlist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/getserverpreferences.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/getserverpreferences.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/getsessionhistory.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/getsessionhistory.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/getsessions.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/getsessions.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/getsourceconnectioninformation.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/getsourceconnectioninformation.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/getstatistics.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/getstatistics.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/gettimeline.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/gettimeline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/gettoken.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/gettoken.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/gettranscodesessions.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/gettranscodesessions.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/gettransienttoken.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/gettransienttoken.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/getupdatestatus.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/getupdatestatus.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/logline.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/logline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/logmultiline.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/logmultiline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/markplayed.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/markplayed.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/markunplayed.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/markunplayed.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/performsearch.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/performsearch.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/performvoicesearch.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/performvoicesearch.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/refreshlibrary.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/refreshlibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/sdkerror.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/startalltasks.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/startalltasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/starttask.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/starttask.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/startuniversaltranscode.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/startuniversaltranscode.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/stopalltasks.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/stopalltasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/stoptask.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/stoptask.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/stoptranscodesession.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/stoptranscodesession.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/updateplaylist.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/updateplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/updateplayprogress.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/updateplayprogress.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/errors/uploadplaylist.py` & `plex-api-client-0.6.3/src/plex_api/models/errors/uploadplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/__init__.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,8 +57,8 @@
 from .stopalltasks import *
 from .stoptask import *
 from .stoptranscodesession import *
 from .updateplaylist import *
 from .updateplayprogress import *
 from .uploadplaylist import *
 
-__all__ = ["Account","Activity","AddPlaylistContentsMediaContainer","AddPlaylistContentsMetadata","AddPlaylistContentsRequest","AddPlaylistContentsResponse","AddPlaylistContentsResponseBody","ApplyUpdatesRequest","ApplyUpdatesResponse","ButlerTask","ButlerTasks","CancelServerActivitiesRequest","CancelServerActivitiesResponse","CheckForUpdatesRequest","CheckForUpdatesResponse","ClearPlaylistContentsRequest","ClearPlaylistContentsResponse","Context","Country","CreatePlaylistMediaContainer","CreatePlaylistMetadata","CreatePlaylistRequest","CreatePlaylistResponse","CreatePlaylistResponseBody","DeleteLibraryRequest","DeleteLibraryResponse","DeletePlaylistRequest","DeletePlaylistResponse","Device","Director","Directory","Download","EnablePaperTrailResponse","Field","FieldType","Filter","Force","GET_PIN_SERVERS","GET_TOKEN_SERVERS","Genre","GetAvailableClientsMediaContainer","GetAvailableClientsResponse","GetAvailableClientsResponseBody","GetButlerTasksResponse","GetButlerTasksResponseBody","GetDevicesMediaContainer","GetDevicesResponse","GetDevicesResponseBody","GetFileHashRequest","GetFileHashResponse","GetGlobalHubsMediaContainer","GetGlobalHubsMetadata","GetGlobalHubsRequest","GetGlobalHubsResponse","GetGlobalHubsResponseBody","GetLibrariesDirectory","GetLibrariesLocation","GetLibrariesMediaContainer","GetLibrariesResponse","GetLibrariesResponseBody","GetLibraryDirectory","GetLibraryHubsCountry","GetLibraryHubsDirector","GetLibraryHubsGenre","GetLibraryHubsHub","GetLibraryHubsMedia","GetLibraryHubsMediaContainer","GetLibraryHubsMetadata","GetLibraryHubsPart","GetLibraryHubsRequest","GetLibraryHubsResponse","GetLibraryHubsResponseBody","GetLibraryHubsRole","GetLibraryHubsWriter","GetLibraryItemsCountry","GetLibraryItemsDirector","GetLibraryItemsGenre","GetLibraryItemsMedia","GetLibraryItemsMediaContainer","GetLibraryItemsMetadata","GetLibraryItemsPart","GetLibraryItemsRequest","GetLibraryItemsResponse","GetLibraryItemsResponseBody","GetLibraryItemsRole","GetLibraryItemsWriter","GetLibraryMediaContainer","GetLibraryRequest","GetLibraryResponse","GetLibraryResponseBody","GetLibraryType","GetMetadataChildrenDirectory","GetMetadataChildrenMediaContainer","GetMetadataChildrenMetadata","GetMetadataChildrenRequest","GetMetadataChildrenResponse","GetMetadataChildrenResponseBody","GetMetadataCountry","GetMetadataDirector","GetMetadataGenre","GetMetadataMedia","GetMetadataMediaContainer","GetMetadataMetadata","GetMetadataPart","GetMetadataRequest","GetMetadataResponse","GetMetadataResponseBody","GetMetadataRole","GetMetadataWriter","GetMyPlexAccountResponse","GetMyPlexAccountResponseBody","GetOnDeckGuids","GetOnDeckMedia","GetOnDeckMediaContainer","GetOnDeckMetadata","GetOnDeckPart","GetOnDeckResponse","GetOnDeckResponseBody","GetOnDeckStream","GetPinRequest","GetPinResponse","GetPinResponseBody","GetPlaylistContentsCountry","GetPlaylistContentsDirector","GetPlaylistContentsGenre","GetPlaylistContentsMedia","GetPlaylistContentsMediaContainer","GetPlaylistContentsMetadata","GetPlaylistContentsPart","GetPlaylistContentsRequest","GetPlaylistContentsResponse","GetPlaylistContentsResponseBody","GetPlaylistContentsRole","GetPlaylistContentsWriter","GetPlaylistMediaContainer","GetPlaylistMetadata","GetPlaylistRequest","GetPlaylistResponse","GetPlaylistResponseBody","GetPlaylistsMediaContainer","GetPlaylistsMetadata","GetPlaylistsRequest","GetPlaylistsResponse","GetPlaylistsResponseBody","GetRecentlyAddedMediaContainer","GetRecentlyAddedResponse","GetRecentlyAddedResponseBody","GetResizedPhotoRequest","GetResizedPhotoResponse","GetSearchResultsCountry","GetSearchResultsDirector","GetSearchResultsGenre","GetSearchResultsMedia","GetSearchResultsMediaContainer","GetSearchResultsMetadata","GetSearchResultsPart","GetSearchResultsRequest","GetSearchResultsResponse","GetSearchResultsResponseBody","GetSearchResultsRole","GetSearchResultsWriter","GetServerActivitiesMediaContainer","GetServerActivitiesResponse","GetServerActivitiesResponseBody","GetServerCapabilitiesResponse","GetServerCapabilitiesResponseBody","GetServerIdentityMediaContainer","GetServerIdentityResponse","GetServerIdentityResponseBody","GetServerListMediaContainer","GetServerListResponse","GetServerListResponseBody","GetServerListServer","GetServerPreferencesMediaContainer","GetServerPreferencesResponse","GetServerPreferencesResponseBody","GetSessionHistoryMediaContainer","GetSessionHistoryMetadata","GetSessionHistoryResponse","GetSessionHistoryResponseBody","GetSessionsMedia","GetSessionsMediaContainer","GetSessionsMetadata","GetSessionsPart","GetSessionsResponse","GetSessionsResponseBody","GetSessionsStream","GetSourceConnectionInformationRequest","GetSourceConnectionInformationResponse","GetStatisticsDevice","GetStatisticsMediaContainer","GetStatisticsRequest","GetStatisticsResponse","GetStatisticsResponseBody","GetTimelineRequest","GetTimelineResponse","GetTokenRequest","GetTokenResponse","GetTranscodeSessionsMediaContainer","GetTranscodeSessionsResponse","GetTranscodeSessionsResponseBody","GetTransientTokenQueryParamType","GetTransientTokenRequest","GetTransientTokenResponse","GetUpdateStatusMediaContainer","GetUpdateStatusResponse","GetUpdateStatusResponseBody","Guids","Hub","IncludeDetails","Level","Location","LogLineRequest","LogLineResponse","LogMultiLineResponse","MarkPlayedRequest","MarkPlayedResponse","MarkUnplayedRequest","MarkUnplayedResponse","Media","MediaContainer","Metadata","MinSize","MyPlex","OnlyTransient","Operator","Part","PathParamTaskName","PerformSearchRequest","PerformSearchResponse","PerformVoiceSearchRequest","PerformVoiceSearchResponse","Player","PlaylistType","Producer","Provider","QueryParamOnlyTransient","QueryParamSmart","QueryParamType","Ratings","RefreshLibraryRequest","RefreshLibraryResponse","Release","Role","Scope","SearchLibraryMediaContainer","SearchLibraryMetadata","SearchLibraryRequest","SearchLibraryResponse","SearchLibraryResponseBody","Server","Session","Setting","Skip","Smart","Sort","StartAllTasksResponse","StartTaskRequest","StartTaskResponse","StartUniversalTranscodeRequest","StartUniversalTranscodeResponse","State","StatisticsMedia","StopAllTasksResponse","StopTaskRequest","StopTaskResponse","StopTranscodeSessionRequest","StopTranscodeSessionResponse","Stream","Tag","TaskName","Tonight","TranscodeSession","Type","UpdatePlayProgressRequest","UpdatePlayProgressResponse","UpdatePlaylistRequest","UpdatePlaylistResponse","UploadPlaylistRequest","UploadPlaylistResponse","Upscale","User","Writer"]
+__all__ = ["Account","Activity","AddPlaylistContentsMediaContainer","AddPlaylistContentsMetadata","AddPlaylistContentsRequest","AddPlaylistContentsResponse","AddPlaylistContentsResponseBody","ApplyUpdatesRequest","ApplyUpdatesResponse","ButlerTask","ButlerTasks","CancelServerActivitiesRequest","CancelServerActivitiesResponse","CheckForUpdatesRequest","CheckForUpdatesResponse","ClearPlaylistContentsRequest","ClearPlaylistContentsResponse","Context","Country","CreatePlaylistMediaContainer","CreatePlaylistMetadata","CreatePlaylistRequest","CreatePlaylistResponse","CreatePlaylistResponseBody","DeleteLibraryRequest","DeleteLibraryResponse","DeletePlaylistRequest","DeletePlaylistResponse","Device","Director","Directory","Download","EnablePaperTrailResponse","Field","FieldType","Filter","Force","GET_PIN_SERVERS","GET_TOKEN_SERVERS","Genre","GetAvailableClientsMediaContainer","GetAvailableClientsResponse","GetAvailableClientsResponseBody","GetButlerTasksResponse","GetButlerTasksResponseBody","GetDevicesMediaContainer","GetDevicesResponse","GetDevicesResponseBody","GetFileHashRequest","GetFileHashResponse","GetGlobalHubsMediaContainer","GetGlobalHubsMetadata","GetGlobalHubsRequest","GetGlobalHubsResponse","GetGlobalHubsResponseBody","GetLibrariesDirectory","GetLibrariesLocation","GetLibrariesMediaContainer","GetLibrariesResponse","GetLibrariesResponseBody","GetLibraryDirectory","GetLibraryHubsCountry","GetLibraryHubsDirector","GetLibraryHubsGenre","GetLibraryHubsHub","GetLibraryHubsMedia","GetLibraryHubsMediaContainer","GetLibraryHubsMetadata","GetLibraryHubsPart","GetLibraryHubsRequest","GetLibraryHubsResponse","GetLibraryHubsResponseBody","GetLibraryHubsRole","GetLibraryHubsWriter","GetLibraryItemsCountry","GetLibraryItemsDirector","GetLibraryItemsGenre","GetLibraryItemsMedia","GetLibraryItemsMediaContainer","GetLibraryItemsMetadata","GetLibraryItemsPart","GetLibraryItemsRequest","GetLibraryItemsResponse","GetLibraryItemsResponseBody","GetLibraryItemsRole","GetLibraryItemsWriter","GetLibraryMediaContainer","GetLibraryRequest","GetLibraryResponse","GetLibraryResponseBody","GetLibraryType","GetMetadataChildrenDirectory","GetMetadataChildrenMediaContainer","GetMetadataChildrenMetadata","GetMetadataChildrenRequest","GetMetadataChildrenResponse","GetMetadataChildrenResponseBody","GetMetadataCountry","GetMetadataDirector","GetMetadataGenre","GetMetadataMedia","GetMetadataMediaContainer","GetMetadataMetadata","GetMetadataPart","GetMetadataRequest","GetMetadataResponse","GetMetadataResponseBody","GetMetadataRole","GetMetadataWriter","GetMyPlexAccountResponse","GetMyPlexAccountResponseBody","GetOnDeckGuids","GetOnDeckMedia","GetOnDeckMediaContainer","GetOnDeckMetadata","GetOnDeckPart","GetOnDeckResponse","GetOnDeckResponseBody","GetOnDeckStream","GetPinGlobals","GetPinRequest","GetPinResponse","GetPinResponseBody","GetPlaylistContentsCountry","GetPlaylistContentsDirector","GetPlaylistContentsGenre","GetPlaylistContentsMedia","GetPlaylistContentsMediaContainer","GetPlaylistContentsMetadata","GetPlaylistContentsPart","GetPlaylistContentsRequest","GetPlaylistContentsResponse","GetPlaylistContentsResponseBody","GetPlaylistContentsRole","GetPlaylistContentsWriter","GetPlaylistMediaContainer","GetPlaylistMetadata","GetPlaylistRequest","GetPlaylistResponse","GetPlaylistResponseBody","GetPlaylistsMediaContainer","GetPlaylistsMetadata","GetPlaylistsRequest","GetPlaylistsResponse","GetPlaylistsResponseBody","GetRecentlyAddedMediaContainer","GetRecentlyAddedResponse","GetRecentlyAddedResponseBody","GetResizedPhotoRequest","GetResizedPhotoResponse","GetSearchResultsCountry","GetSearchResultsDirector","GetSearchResultsGenre","GetSearchResultsMedia","GetSearchResultsMediaContainer","GetSearchResultsMetadata","GetSearchResultsPart","GetSearchResultsRequest","GetSearchResultsResponse","GetSearchResultsResponseBody","GetSearchResultsRole","GetSearchResultsWriter","GetServerActivitiesMediaContainer","GetServerActivitiesResponse","GetServerActivitiesResponseBody","GetServerCapabilitiesResponse","GetServerCapabilitiesResponseBody","GetServerIdentityMediaContainer","GetServerIdentityResponse","GetServerIdentityResponseBody","GetServerListMediaContainer","GetServerListResponse","GetServerListResponseBody","GetServerListServer","GetServerPreferencesMediaContainer","GetServerPreferencesResponse","GetServerPreferencesResponseBody","GetSessionHistoryMediaContainer","GetSessionHistoryMetadata","GetSessionHistoryResponse","GetSessionHistoryResponseBody","GetSessionsMedia","GetSessionsMediaContainer","GetSessionsMetadata","GetSessionsPart","GetSessionsResponse","GetSessionsResponseBody","GetSessionsStream","GetSourceConnectionInformationRequest","GetSourceConnectionInformationResponse","GetStatisticsDevice","GetStatisticsMediaContainer","GetStatisticsRequest","GetStatisticsResponse","GetStatisticsResponseBody","GetTimelineRequest","GetTimelineResponse","GetTokenGlobals","GetTokenRequest","GetTokenResponse","GetTranscodeSessionsMediaContainer","GetTranscodeSessionsResponse","GetTranscodeSessionsResponseBody","GetTransientTokenQueryParamType","GetTransientTokenRequest","GetTransientTokenResponse","GetUpdateStatusMediaContainer","GetUpdateStatusResponse","GetUpdateStatusResponseBody","Guids","Hub","IncludeDetails","Level","Location","LogLineRequest","LogLineResponse","LogMultiLineResponse","MarkPlayedRequest","MarkPlayedResponse","MarkUnplayedRequest","MarkUnplayedResponse","Media","MediaContainer","Metadata","MinSize","MyPlex","OnlyTransient","Operator","Part","PathParamTaskName","PerformSearchRequest","PerformSearchResponse","PerformVoiceSearchRequest","PerformVoiceSearchResponse","Player","PlaylistType","Producer","Provider","QueryParamOnlyTransient","QueryParamSmart","QueryParamType","Ratings","RefreshLibraryRequest","RefreshLibraryResponse","Release","Role","Scope","SearchLibraryMediaContainer","SearchLibraryMetadata","SearchLibraryRequest","SearchLibraryResponse","SearchLibraryResponseBody","Server","Session","Setting","Skip","Smart","Sort","StartAllTasksResponse","StartTaskRequest","StartTaskResponse","StartUniversalTranscodeRequest","StartUniversalTranscodeResponse","State","StatisticsMedia","StopAllTasksResponse","StopTaskRequest","StopTaskResponse","StopTranscodeSessionRequest","StopTranscodeSessionResponse","Stream","Tag","TaskName","Tonight","TranscodeSession","Type","UpdatePlayProgressRequest","UpdatePlayProgressResponse","UpdatePlaylistRequest","UpdatePlaylistResponse","UploadPlaylistRequest","UploadPlaylistResponse","Upscale","User","Writer"]
```

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/addplaylistcontents.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/addplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/applyupdates.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/applyupdates.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/cancelserveractivities.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/cancelserveractivities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/checkforupdates.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/checkforupdates.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/clearplaylistcontents.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/clearplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/createplaylist.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/createplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/deletelibrary.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/deletelibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/deleteplaylist.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/deleteplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/enablepapertrail.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/enablepapertrail.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/getavailableclients.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/getavailableclients.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/getbutlertasks.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/getbutlertasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/getdevices.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/getdevices.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/getfilehash.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/getfilehash.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/getglobalhubs.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/getglobalhubs.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/getlibraries.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/getlibraries.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/getlibrary.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/getlibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/getlibraryhubs.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/getlibraryhubs.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/getlibraryitems.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/getlibraryitems.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/getmetadata.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/getmetadata.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/getmetadatachildren.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/getmetadatachildren.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/getmyplexaccount.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/getmyplexaccount.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/getondeck.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/getondeck.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/getpin.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/getpin.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,25 @@
 
 GET_PIN_SERVERS = [
 	"https://plex.tv/api/v2",
 ]
 
 
 @dataclasses.dataclass
+class GetPinGlobals:
+    x_plex_client_identifier: str = dataclasses.field(metadata={'header': { 'field_name': 'X-Plex-Client-Identifier', 'style': 'simple', 'explode': False }})
+    r"""The unique identifier for the client application
+    This is used to track the client application and its usage
+    (UUID, serial number, or other number unique per device)
+    """
+    
+
+
+
+@dataclasses.dataclass
 class GetPinRequest:
     strong: Optional[bool] = dataclasses.field(default=False, metadata={'query_param': { 'field_name': 'strong', 'style': 'form', 'explode': True }})
     r"""Determines the kind of code returned by the API call
     Strong codes are used for Pin authentication flows
     Non-Strong codes are used for `Plex.tv/link`
     """
     x_plex_client_identifier: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'X-Plex-Client-Identifier', 'style': 'simple', 'explode': False }})
```

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/getplaylist.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/getplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/getplaylistcontents.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/getplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/getplaylists.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/getplaylists.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/getrecentlyadded.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/getrecentlyadded.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/getresizedphoto.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/getresizedphoto.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/getsearchresults.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/getsearchresults.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/getserveractivities.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/getserveractivities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/getservercapabilities.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/getservercapabilities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/getserveridentity.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/getserveridentity.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/getserverlist.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/getserverlist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/getserverpreferences.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/getserverpreferences.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/getsessionhistory.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/getsessionhistory.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/getsessions.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/getsessions.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/getsourceconnectioninformation.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/getsourceconnectioninformation.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/getstatistics.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/getstatistics.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/gettimeline.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/gettimeline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/gettoken.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/gettoken.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,25 @@
 
 GET_TOKEN_SERVERS = [
 	"https://plex.tv/api/v2",
 ]
 
 
 @dataclasses.dataclass
+class GetTokenGlobals:
+    x_plex_client_identifier: str = dataclasses.field(metadata={'header': { 'field_name': 'X-Plex-Client-Identifier', 'style': 'simple', 'explode': False }})
+    r"""The unique identifier for the client application
+    This is used to track the client application and its usage
+    (UUID, serial number, or other number unique per device)
+    """
+    
+
+
+
+@dataclasses.dataclass
 class GetTokenRequest:
     pin_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'pinID', 'style': 'simple', 'explode': False }})
     r"""The PinID to retrieve an access token for"""
     x_plex_client_identifier: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'X-Plex-Client-Identifier', 'style': 'simple', 'explode': False }})
     r"""The unique identifier for the client application
     This is used to track the client application and its usage
     (UUID, serial number, or other number unique per device)
```

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/gettranscodesessions.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/gettranscodesessions.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/gettransienttoken.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/gettransienttoken.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/getupdatestatus.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/getupdatestatus.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/logline.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/logline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/logmultiline.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/logmultiline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/markplayed.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/markplayed.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/markunplayed.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/markunplayed.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/performsearch.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/performsearch.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/performvoicesearch.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/performvoicesearch.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/refreshlibrary.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/refreshlibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/searchlibrary.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/searchlibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/startalltasks.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/startalltasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/starttask.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/starttask.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/startuniversaltranscode.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/startuniversaltranscode.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/stopalltasks.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/stopalltasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/stoptask.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/stoptask.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/stoptranscodesession.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/stoptranscodesession.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/updateplaylist.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/updateplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/updateplayprogress.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/updateplayprogress.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/models/operations/uploadplaylist.py` & `plex-api-client-0.6.3/src/plex_api/models/operations/uploadplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/playlists.py` & `plex-api-client-0.6.3/src/plex_api/playlists.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         url = base_url + '/playlists'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.CreatePlaylistRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -102,15 +102,15 @@
         url = base_url + '/playlists'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetPlaylistsRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -165,15 +165,15 @@
         hook_ctx = HookContext(operation_id='getPlaylist', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.GetPlaylistRequest(
             playlist_id=playlist_id,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetPlaylistRequest, base_url, '/playlists/{playlistID}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/playlists/{playlistID}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -233,15 +233,15 @@
         hook_ctx = HookContext(operation_id='deletePlaylist', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.DeletePlaylistRequest(
             playlist_id=playlist_id,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.DeletePlaylistRequest, base_url, '/playlists/{playlistID}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/playlists/{playlistID}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -298,22 +298,22 @@
             playlist_id=playlist_id,
             title=title,
             summary=summary,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdatePlaylistRequest, base_url, '/playlists/{playlistID}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/playlists/{playlistID}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.UpdatePlaylistRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -366,22 +366,22 @@
         request = operations.GetPlaylistContentsRequest(
             playlist_id=playlist_id,
             type=type_,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetPlaylistContentsRequest, base_url, '/playlists/{playlistID}/items', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/playlists/{playlistID}/items', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetPlaylistContentsRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -435,15 +435,15 @@
         hook_ctx = HookContext(operation_id='clearPlaylistContents', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.ClearPlaylistContentsRequest(
             playlist_id=playlist_id,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ClearPlaylistContentsRequest, base_url, '/playlists/{playlistID}/items', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/playlists/{playlistID}/items', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -501,22 +501,22 @@
             playlist_id=playlist_id,
             uri=uri,
             play_queue_id=play_queue_id,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.AddPlaylistContentsRequest, base_url, '/playlists/{playlistID}/items', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/playlists/{playlistID}/items', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.AddPlaylistContentsRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -578,15 +578,15 @@
         url = base_url + '/playlists/upload'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.UploadPlaylistRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `plex-api-client-0.6.2/src/plex_api/plex.py` & `plex-api-client-0.6.3/src/plex_api/plex.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,26 +22,30 @@
         """
         hook_ctx = HookContext(operation_id='getPin', oauth2_scopes=[], security_source=None)
         request = operations.GetPinRequest(
             strong=strong,
             x_plex_client_identifier=x_plex_client_identifier,
         )
         
+        _globals = operations.GetPinGlobals(
+            x_plex_client_identifier=self.sdk_configuration.globals.x_plex_client_identifier,
+        )
+        
         base_url = utils.template_url(operations.GET_PIN_SERVERS[0], {
         })
         if server_url is not None:
             base_url = server_url
         
-        url = base_url + '/pins'
+        url = utils.generate_url(base_url, '/pins', request, _globals)
         
         headers = {}
         query_params = {}
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
-        query_params = { **utils.get_query_params(operations.GetPinRequest, request, self.sdk_configuration.globals), **query_params }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -94,30 +98,36 @@
         """
         hook_ctx = HookContext(operation_id='getToken', oauth2_scopes=[], security_source=None)
         request = operations.GetTokenRequest(
             pin_id=pin_id,
             x_plex_client_identifier=x_plex_client_identifier,
         )
         
+        _globals = operations.GetTokenGlobals(
+            x_plex_client_identifier=self.sdk_configuration.globals.x_plex_client_identifier,
+        )
+        
         base_url = utils.template_url(operations.GET_TOKEN_SERVERS[0], {
         })
         if server_url is not None:
             base_url = server_url
         
-        url = utils.generate_url(operations.GetTokenRequest, base_url, '/pins/{pinID}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/pins/{pinID}', request, _globals)
         
         headers = {}
+        query_params = {}
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('GET', url, headers=headers))
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
```

### Comparing `plex-api-client-0.6.2/src/plex_api/sdk.py` & `plex-api-client-0.6.3/src/plex_api/sdk.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from .sessions import Sessions
 from .statistics import Statistics
 from .updater import Updater
 from .utils.retries import RetryConfig
 from .video import Video
 from plex_api import utils
 from plex_api._hooks import SDKHooks
-from plex_api.models import components
+from plex_api.models import components, internal
 from typing import Callable, Dict, Optional, Union
 
 class PlexAPI:
     r"""Plex-API: A Plex Media Server API Map
     An Open API Spec for interacting with Plex.tv and Plex Servers
     """
     server: Server
@@ -123,45 +123,38 @@
         server_defaults = [
             {
                 'protocol': protocol or 'http',
                 'ip': ip or '10.10.10.47',
                 'port': port or '32400',
             },
         ]
-        global_params = {
-            'parameters': {
-                'queryParam': {
-                },
-                'pathParam': {
-                },
-                'header': {
-                    'x_plex_client_identifier': x_plex_client_identifier,
-                },
-            },
-        }
+    
+        _globals = internal.Globals(
+            x_plex_client_identifier=x_plex_client_identifier,
+        )
 
         self.sdk_configuration = SDKConfiguration(
             client,
+            _globals,
             security,
             server_url,
             server_idx,
             server_defaults,
-            global_params,
             retry_config=retry_config
         )
 
         hooks = SDKHooks()
 
         current_server_url, *_ = self.sdk_configuration.get_server_details()
         server_url, self.sdk_configuration.client = hooks.sdk_init(current_server_url, self.sdk_configuration.client)
         if current_server_url != server_url:
             self.sdk_configuration.server_url = server_url
 
         # pylint: disable=protected-access
-        self.sdk_configuration._hooks = hooks
+        self.sdk_configuration.__dict__['_hooks'] = hooks
 
         self._init_sdks()
 
 
     def _init_sdks(self):
         self.server = Server(self.sdk_configuration)
         self.media = Media(self.sdk_configuration)
```

### Comparing `plex-api-client-0.6.2/src/plex_api/sdkconfiguration.py` & `plex-api-client-0.6.3/src/plex_api/sdkconfiguration.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 import requests as requests_http
 from ._hooks import SDKHooks
 from .utils import utils
 from .utils.retries import RetryConfig
 from dataclasses import dataclass, field
 from enum import Enum
-from plex_api.models import components
-from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+from plex_api.models import components, internal
+from typing import Callable, Dict, List, Optional, Tuple, Union
 
 
 SERVERS = [
     '{protocol}://{ip}:{port}',
     # The full address of your Plex Server
 ]
 """Contains the list of servers available to the SDK"""
@@ -22,26 +22,28 @@
     HTTP = 'http'
     HTTPS = 'https'
 
 
 @dataclass
 class SDKConfiguration:
     client: requests_http.Session
+    globals: internal.Globals
     security: Union[components.Security,Callable[[], components.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     server_defaults: List[Dict[str, str]] = field(default_factory=List)
-    globals: Dict[str, Dict[str, Dict[str, Any]]] = field(default_factory=Dict)
     language: str = 'python'
     openapi_doc_version: str = '0.0.3'
-    sdk_version: str = '0.6.2'
-    gen_version: str = '2.300.0'
-    user_agent: str = 'speakeasy-sdk/python 0.6.2 2.300.0 0.0.3 plex-api-client'
+    sdk_version: str = '0.6.3'
+    gen_version: str = '2.301.0'
+    user_agent: str = 'speakeasy-sdk/python 0.6.3 2.301.0 0.0.3 plex-api-client'
     retry_config: Optional[RetryConfig] = None
-    _hooks: Optional[SDKHooks] = None
+
+    def __post_init__(self):
+        self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
             return utils.remove_suffix(self.server_url, '/'), {}
         if self.server_idx is None:
             self.server_idx = 0
```

### Comparing `plex-api-client-0.6.2/src/plex_api/search.py` & `plex-api-client-0.6.3/src/plex_api/search.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         url = base_url + '/hubs/search'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.PerformSearchRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -112,15 +112,15 @@
         url = base_url + '/hubs/search/voice'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.PerformVoiceSearchRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -176,15 +176,15 @@
         url = base_url + '/search'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetSearchResultsRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `plex-api-client-0.6.2/src/plex_api/server.py` & `plex-api-client-0.6.3/src/plex_api/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -410,15 +410,15 @@
         url = base_url + '/photo/:/transcode'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetResizedPhotoRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `plex-api-client-0.6.2/src/plex_api/sessions.py` & `plex-api-client-0.6.3/src/plex_api/sessions.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
         hook_ctx = HookContext(operation_id='stopTranscodeSession', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.StopTranscodeSessionRequest(
             session_key=session_key,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.StopTranscodeSessionRequest, base_url, '/transcode/sessions/{sessionKey}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/transcode/sessions/{sessionKey}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
```

### Comparing `plex-api-client-0.6.2/src/plex_api/statistics.py` & `plex-api-client-0.6.3/src/plex_api/statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         url = base_url + '/statistics/media'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetStatisticsRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `plex-api-client-0.6.2/src/plex_api/updater.py` & `plex-api-client-0.6.3/src/plex_api/updater.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         url = base_url + '/updater/check'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.CheckForUpdatesRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -161,15 +161,15 @@
         url = base_url + '/updater/apply'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ApplyUpdatesRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `plex-api-client-0.6.2/src/plex_api/utils/retries.py` & `plex-api-client-0.6.3/src/plex_api/utils/retries.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.2/src/plex_api/utils/utils.py` & `plex-api-client-0.6.3/src/plex_api/utils/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,16 +5,25 @@
 import re
 import sys
 from dataclasses import Field, fields, is_dataclass, make_dataclass
 from datetime import date, datetime
 from decimal import Decimal
 from email.message import Message
 from enum import Enum
-from typing import (Any, Callable, Dict, List, Optional, Tuple, Union,
-                    get_args, get_origin)
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Tuple,
+    Union,
+    get_args,
+    get_origin,
+)
 from xmlrpc.client import boolean
 from typing_inspect import is_optional_type
 import dateutil.parser
 from dataclasses_json import DataClassJsonMixin
 
 
 def get_security(security: Any) -> Tuple[Dict[str, str], Dict[str, str]]:
@@ -26,470 +35,600 @@
 
     sec_fields: Tuple[Field, ...] = fields(security)
     for sec_field in sec_fields:
         value = getattr(security, sec_field.name)
         if value is None:
             continue
 
-        metadata = sec_field.metadata.get('security')
+        metadata = sec_field.metadata.get("security")
         if metadata is None:
             continue
-        if metadata.get('option'):
+        if metadata.get("option"):
             _parse_security_option(headers, query_params, value)
             return headers, query_params
-        if metadata.get('scheme'):
+        if metadata.get("scheme"):
             # Special case for basic auth which could be a flattened struct
             if metadata.get("sub_type") == "basic" and not is_dataclass(value):
                 _parse_security_scheme(headers, query_params, metadata, security)
             else:
                 _parse_security_scheme(headers, query_params, metadata, value)
 
     return headers, query_params
 
 
-def _parse_security_option(headers: Dict[str, str], query_params: Dict[str, str], option: Any):
+def _parse_security_option(
+    headers: Dict[str, str], query_params: Dict[str, str], option: Any
+):
     opt_fields: Tuple[Field, ...] = fields(option)
     for opt_field in opt_fields:
-        metadata = opt_field.metadata.get('security')
-        if metadata is None or metadata.get('scheme') is None:
+        metadata = opt_field.metadata.get("security")
+        if metadata is None or metadata.get("scheme") is None:
             continue
         _parse_security_scheme(
-            headers, query_params, metadata, getattr(option, opt_field.name))
+            headers, query_params, metadata, getattr(option, opt_field.name)
+        )
 
 
-def _parse_security_scheme(headers: Dict[str, str], query_params: Dict[str, str], scheme_metadata: Dict, scheme: Any):
-    scheme_type = scheme_metadata.get('type')
-    sub_type = scheme_metadata.get('sub_type')
+def _parse_security_scheme(
+    headers: Dict[str, str],
+    query_params: Dict[str, str],
+    scheme_metadata: Dict,
+    scheme: Any,
+):
+    scheme_type = scheme_metadata.get("type")
+    sub_type = scheme_metadata.get("sub_type")
 
     if is_dataclass(scheme):
-        if scheme_type == 'http' and sub_type == 'basic':
+        if scheme_type == "http" and sub_type == "basic":
             _parse_basic_auth_scheme(headers, scheme)
             return
 
         scheme_fields: Tuple[Field, ...] = fields(scheme)
         for scheme_field in scheme_fields:
-            metadata = scheme_field.metadata.get('security')
-            if metadata is None or metadata.get('field_name') is None:
+            metadata = scheme_field.metadata.get("security")
+            if metadata is None or metadata.get("field_name") is None:
                 continue
 
             value = getattr(scheme, scheme_field.name)
 
             _parse_security_scheme_value(
-                headers, query_params, scheme_metadata, metadata, value)
+                headers, query_params, scheme_metadata, metadata, value
+            )
     else:
         _parse_security_scheme_value(
-            headers, query_params, scheme_metadata, scheme_metadata, scheme)
+            headers, query_params, scheme_metadata, scheme_metadata, scheme
+        )
 
 
-def _parse_security_scheme_value(headers: Dict[str, str], query_params: Dict[str, str], scheme_metadata: Dict, security_metadata: Dict, value: Any):
-    scheme_type = scheme_metadata.get('type')
-    sub_type = scheme_metadata.get('sub_type')
+def _parse_security_scheme_value(
+    headers: Dict[str, str],
+    query_params: Dict[str, str],
+    scheme_metadata: Dict,
+    security_metadata: Dict,
+    value: Any,
+):
+    scheme_type = scheme_metadata.get("type")
+    sub_type = scheme_metadata.get("sub_type")
 
-    header_name = str(security_metadata.get('field_name'))
+    header_name = str(security_metadata.get("field_name"))
 
     if scheme_type == "apiKey":
-        if sub_type == 'header':
+        if sub_type == "header":
             headers[header_name] = value
-        elif sub_type == 'query':
+        elif sub_type == "query":
             query_params[header_name] = value
         else:
-            raise Exception('not supported')
+            raise Exception("not supported")
     elif scheme_type == "openIdConnect":
         headers[header_name] = _apply_bearer(value)
-    elif scheme_type == 'oauth2':
-        if sub_type != 'client_credentials':
+    elif scheme_type == "oauth2":
+        if sub_type != "client_credentials":
             headers[header_name] = _apply_bearer(value)
-    elif scheme_type == 'http':
-        if sub_type == 'bearer':
+    elif scheme_type == "http":
+        if sub_type == "bearer":
             headers[header_name] = _apply_bearer(value)
         else:
-            raise Exception('not supported')
+            raise Exception("not supported")
     else:
-        raise Exception('not supported')
+        raise Exception("not supported")
 
 
 def _apply_bearer(token: str) -> str:
-    return token.lower().startswith('bearer ') and token or f'Bearer {token}'
+    return token.lower().startswith("bearer ") and token or f"Bearer {token}"
 
 
 def _parse_basic_auth_scheme(headers: Dict[str, str], scheme: Any):
     username = ""
     password = ""
 
     scheme_fields: Tuple[Field, ...] = fields(scheme)
     for scheme_field in scheme_fields:
-        metadata = scheme_field.metadata.get('security')
-        if metadata is None or metadata.get('field_name') is None:
+        metadata = scheme_field.metadata.get("security")
+        if metadata is None or metadata.get("field_name") is None:
             continue
 
-        field_name = metadata.get('field_name')
+        field_name = metadata.get("field_name")
         value = getattr(scheme, scheme_field.name)
 
-        if field_name == 'username':
+        if field_name == "username":
             username = value
-        if field_name == 'password':
+        if field_name == "password":
             password = value
 
-    data = f'{username}:{password}'.encode()
-    headers['Authorization'] = f'Basic {base64.b64encode(data).decode()}'
+    data = f"{username}:{password}".encode()
+    headers["Authorization"] = f"Basic {base64.b64encode(data).decode()}"
 
 
-def generate_url(clazz: type, server_url: str, path: str, path_params: Any,
-                 gbls: Optional[Dict[str, Dict[str, Dict[str, Any]]]] = None) -> str:
-    path_param_fields: Tuple[Field, ...] = fields(clazz)
+def generate_url(
+    server_url: str,
+    path: str,
+    path_params: Any,
+    gbls: Optional[Any] = None,
+) -> str:
+    path_param_values: Dict[str, str] = {}
+
+    globals_already_populated = _populate_path_params(
+        path_params, gbls, path_param_values, []
+    )
+    if gbls is not None:
+        _populate_path_params(gbls, None, path_param_values, globals_already_populated)
+
+    for key, value in path_param_values.items():
+        path = path.replace("{" + key + "}", value, 1)
+
+    return remove_suffix(server_url, "/") + path
+
+
+def _populate_path_params(
+    path_params: Any,
+    gbls: Any,
+    path_param_values: Dict[str, str],
+    skip_fields: List[str],
+) -> List[str]:
+    globals_already_populated: List[str] = []
+
+    path_param_fields: Tuple[Field, ...] = fields(path_params)
     for field in path_param_fields:
-        request_metadata = field.metadata.get('request')
-        if request_metadata is not None:
+        if field.name in skip_fields:
             continue
 
-        param_metadata = field.metadata.get('path_param')
+        param_metadata = field.metadata.get("path_param")
         if param_metadata is None:
             continue
 
-        param = getattr(
-            path_params, field.name) if path_params is not None else None
-        param = _populate_from_globals(
-            field.name, param, 'pathParam', gbls)
+        param = getattr(path_params, field.name) if path_params is not None else None
+        param, global_found = _populate_from_globals(
+            field.name, param, "path_param", gbls
+        )
+        if global_found:
+            globals_already_populated.append(field.name)
 
         if param is None:
             continue
 
         f_name = param_metadata.get("field_name", field.name)
-        serialization = param_metadata.get('serialization', '')
-        if serialization != '':
+        serialization = param_metadata.get("serialization", "")
+        if serialization != "":
             serialized_params = _get_serialized_params(
-                param_metadata, field.type, f_name, param)
+                param_metadata, field.type, f_name, param
+            )
             for key, value in serialized_params.items():
-                path = path.replace(
-                    '{' + key + '}', value, 1)
+                path_param_values[key] = value
         else:
-            if param_metadata.get('style', 'simple') == 'simple':
+            if param_metadata.get("style", "simple") == "simple":
                 if isinstance(param, List):
                     pp_vals: List[str] = []
                     for pp_val in param:
                         if pp_val is None:
                             continue
                         pp_vals.append(_val_to_string(pp_val))
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        ",".join(pp_vals)
+                    )
                 elif isinstance(param, Dict):
                     pp_vals: List[str] = []
                     for pp_key in param:
                         if param[pp_key] is None:
                             continue
-                        if param_metadata.get('explode'):
-                            pp_vals.append(
-                                f"{pp_key}={_val_to_string(param[pp_key])}")
+                        if param_metadata.get("explode"):
+                            pp_vals.append(f"{pp_key}={_val_to_string(param[pp_key])}")
                         else:
-                            pp_vals.append(
-                                f"{pp_key},{_val_to_string(param[pp_key])}")
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                            pp_vals.append(f"{pp_key},{_val_to_string(param[pp_key])}")
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        ",".join(pp_vals)
+                    )
                 elif not isinstance(param, (str, int, float, complex, bool, Decimal)):
                     pp_vals: List[str] = []
                     param_fields: Tuple[Field, ...] = fields(param)
                     for param_field in param_fields:
-                        param_value_metadata = param_field.metadata.get(
-                            'path_param')
+                        param_value_metadata = param_field.metadata.get("path_param")
                         if not param_value_metadata:
                             continue
 
-                        parm_name = param_value_metadata.get(
-                            'field_name', field.name)
+                        param_name = param_value_metadata.get("field_name", field.name)
 
                         param_field_val = getattr(param, param_field.name)
                         if param_field_val is None:
                             continue
-                        if param_metadata.get('explode'):
+                        if param_metadata.get("explode"):
                             pp_vals.append(
-                                f"{parm_name}={_val_to_string(param_field_val)}")
+                                f"{param_name}={_val_to_string(param_field_val)}"
+                            )
                         else:
                             pp_vals.append(
-                                f"{parm_name},{_val_to_string(param_field_val)}")
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                                f"{param_name},{_val_to_string(param_field_val)}"
+                            )
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        ",".join(pp_vals)
+                    )
                 else:
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', _val_to_string(param), 1)
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        _val_to_string(param)
+                    )
 
-    return remove_suffix(server_url, '/') + path
+    return globals_already_populated
 
 
 def is_optional(field):
     return get_origin(field) is Union and type(None) in get_args(field)
 
 
 def template_url(url_with_params: str, params: Dict[str, str]) -> str:
     for key, value in params.items():
-        url_with_params = url_with_params.replace(
-            '{' + key + '}', value)
+        url_with_params = url_with_params.replace("{" + key + "}", value)
 
     return url_with_params
 
 
-def get_query_params(clazz: type, query_params: Any, gbls: Optional[Dict[str, Dict[str, Dict[str, Any]]]] = None) -> Dict[
-        str, List[str]]:
+def get_query_params(
+    query_params: Any,
+    gbls: Optional[Any] = None,
+) -> Dict[str, List[str]]:
     params: Dict[str, List[str]] = {}
 
-    param_fields: Tuple[Field, ...] = fields(clazz)
+    globals_already_populated = _populate_query_params(query_params, gbls, params, [])
+    if gbls is not None:
+        _populate_query_params(gbls, None, params, globals_already_populated)
+
+    return params
+
+
+def _populate_query_params(
+    query_params: Any,
+    gbls: Any,
+    query_param_values: Dict[str, List[str]],
+    skip_fields: List[str],
+) -> List[str]:
+    globals_already_populated: List[str] = []
+
+    param_fields: Tuple[Field, ...] = fields(query_params)
     for field in param_fields:
-        request_metadata = field.metadata.get('request')
-        if request_metadata is not None:
+        if field.name in skip_fields:
             continue
 
-        metadata = field.metadata.get('query_param')
+        metadata = field.metadata.get("query_param")
         if not metadata:
             continue
 
         param_name = field.name
-        value = getattr(
-            query_params, param_name) if query_params is not None else None
+        value = getattr(query_params, param_name) if query_params is not None else None
 
-        value = _populate_from_globals(param_name, value, 'queryParam', gbls)
+        value, global_found = _populate_from_globals(
+            param_name, value, "query_param", gbls
+        )
+        if global_found:
+            globals_already_populated.append(param_name)
 
         f_name = metadata.get("field_name")
-        serialization = metadata.get('serialization', '')
-        if serialization != '':
+        serialization = metadata.get("serialization", "")
+        if serialization != "":
             serialized_parms = _get_serialized_params(
-                metadata, field.type, f_name, value)
+                metadata, field.type, f_name, value
+            )
             for key, value in serialized_parms.items():
-                if key in params:
-                    params[key].extend(value)
+                if key in query_param_values:
+                    query_param_values[key].extend(value)
                 else:
-                    params[key] = [value]
+                    query_param_values[key] = [value]
         else:
-            style = metadata.get('style', 'form')
-            if style == 'deepObject':
-                params = {**params, **_get_deep_object_query_params(
-                    metadata, f_name, value)}
-            elif style == 'form':
-                params = {**params, **_get_delimited_query_params(
-                    metadata, f_name, value, ",")}
-            elif style == 'pipeDelimited':
-                params = {**params, **_get_delimited_query_params(
-                    metadata, f_name, value, "|")}
+            style = metadata.get("style", "form")
+            if style == "deepObject":
+                _populate_deep_object_query_params(
+                    metadata, f_name, value, query_param_values
+                )
+            elif style == "form":
+                _populate_delimited_query_params(
+                    metadata, f_name, value, ",", query_param_values
+                )
+            elif style == "pipeDelimited":
+                _populate_delimited_query_params(
+                    metadata, f_name, value, "|", query_param_values
+                )
             else:
-                raise Exception('not yet implemented')
-    return params
+                raise Exception("not yet implemented")
 
+    return globals_already_populated
 
-def get_headers(headers_params: Any, gbls: Optional[Dict[str, Dict[str, Dict[str, Any]]]] = None) -> Dict[str, str]:
-    if headers_params is None:
-        return {}
 
+def get_headers(headers_params: Any, gbls: Optional[Any] = None) -> Dict[str, str]:
     headers: Dict[str, str] = {}
 
-    param_fields: Tuple[Field, ...] = fields(headers_params)
-    for field in param_fields:
-        metadata = field.metadata.get('header')
-        if not metadata:
-            continue
+    globals_already_populated = []
+    if headers_params is not None:
+        globals_already_populated = _populate_headers(headers_params, gbls, headers, [])
+    if gbls is not None:
+        _populate_headers(gbls, None, headers, globals_already_populated)
 
-        value = _populate_from_globals(field.name, getattr(headers_params, field.name), 'header', gbls)
-        value = _serialize_header(metadata.get('explode', False), value)
+    return headers
 
-        if value != '':
-            headers[metadata.get('field_name', field.name)] = value
 
-    return headers
+def _populate_headers(
+    headers_params: Any,
+    gbls: Any,
+    header_values: Dict[str, str],
+    skip_fields: List[str],
+) -> List[str]:
+    globals_already_populated: List[str] = []
+
+    param_fields: Tuple[Field, ...] = fields(headers_params)
+    for field in param_fields:
+        if field.name in skip_fields:
+            continue
 
+        metadata = field.metadata.get("header")
+        if not metadata:
+            continue
 
-def _get_serialized_params(metadata: Dict, field_type: type, field_name: str, obj: Any) -> Dict[str, str]:
+        value, global_found = _populate_from_globals(
+            field.name, getattr(headers_params, field.name), "header", gbls
+        )
+        if global_found:
+            globals_already_populated.append(field.name)
+        value = _serialize_header(metadata.get("explode", False), value)
+
+        if value != "":
+            header_values[metadata.get("field_name", field.name)] = value
+
+    return globals_already_populated
+
+
+def _get_serialized_params(
+    metadata: Dict, field_type: type, field_name: str, obj: Any
+) -> Dict[str, str]:
     params: Dict[str, str] = {}
 
-    serialization = metadata.get('serialization', '')
-    if serialization == 'json':
-        params[metadata.get("field_name", field_name)
-               ] = marshal_json(obj, field_type)
+    serialization = metadata.get("serialization", "")
+    if serialization == "json":
+        params[metadata.get("field_name", field_name)] = marshal_json(obj, field_type)
 
     return params
 
 
-def _get_deep_object_query_params(metadata: Dict, field_name: str, obj: Any) -> Dict[str, List[str]]:
-    params: Dict[str, List[str]] = {}
-
+def _populate_deep_object_query_params(
+    metadata: Dict, field_name: str, obj: Any, params: Dict[str, List[str]]
+):
     if obj is None:
-        return params
+        return
 
     if is_dataclass(obj):
         obj_fields: Tuple[Field, ...] = fields(obj)
         for obj_field in obj_fields:
-            obj_param_metadata = obj_field.metadata.get('query_param')
+            obj_param_metadata = obj_field.metadata.get("query_param")
             if not obj_param_metadata:
                 continue
 
             obj_val = getattr(obj, obj_field.name)
             if obj_val is None:
                 continue
 
             if isinstance(obj_val, List):
                 for val in obj_val:
                     if val is None:
                         continue
 
-                    if params.get(
-                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]') is None:
+                    if (
+                        params.get(
+                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                        )
+                        is None
+                    ):
                         params[
-                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
-                        ]
+                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                        ] = []
 
                     params[
-                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'].append(
-                        _val_to_string(val))
+                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                    ].append(_val_to_string(val))
             else:
                 params[
-                    f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
-                    _val_to_string(obj_val)]
+                    f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                ] = [_val_to_string(obj_val)]
     elif isinstance(obj, Dict):
         for key, value in obj.items():
             if value is None:
                 continue
 
             if isinstance(value, List):
                 for val in value:
                     if val is None:
                         continue
 
-                    if params.get(f'{metadata.get("field_name", field_name)}[{key}]') is None:
-                        params[f'{metadata.get("field_name", field_name)}[{key}]'] = [
-                        ]
-
-                    params[
-                        f'{metadata.get("field_name", field_name)}[{key}]'].append(_val_to_string(val))
+                    if (
+                        params.get(f'{metadata.get("field_name", field_name)}[{key}]')
+                        is None
+                    ):
+                        params[f'{metadata.get("field_name", field_name)}[{key}]'] = []
+
+                    params[f'{metadata.get("field_name", field_name)}[{key}]'].append(
+                        _val_to_string(val)
+                    )
             else:
                 params[f'{metadata.get("field_name", field_name)}[{key}]'] = [
-                    _val_to_string(value)]
-    return params
+                    _val_to_string(value)
+                ]
 
 
 def _get_query_param_field_name(obj_field: Field) -> str:
-    obj_param_metadata = obj_field.metadata.get('query_param')
+    obj_param_metadata = obj_field.metadata.get("query_param")
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _get_delimited_query_params(metadata: Dict, field_name: str, obj: Any, delimiter: str) -> Dict[
-        str, List[str]]:
-    return _populate_form(field_name, metadata.get("explode", True), obj, _get_query_param_field_name, delimiter)
+def _populate_delimited_query_params(
+    metadata: Dict,
+    field_name: str,
+    obj: Any,
+    delimiter: str,
+    query_param_values: Dict[str, List[str]],
+):
+    _populate_form(
+        field_name,
+        metadata.get("explode", True),
+        obj,
+        _get_query_param_field_name,
+        delimiter,
+        query_param_values,
+    )
 
 
 SERIALIZATION_METHOD_TO_CONTENT_TYPE = {
-    'json': 'application/json',
-    'form': 'application/x-www-form-urlencoded',
-    'multipart': 'multipart/form-data',
-    'raw': 'application/octet-stream',
-    'string': 'text/plain',
+    "json": "application/json",
+    "form": "application/x-www-form-urlencoded",
+    "multipart": "multipart/form-data",
+    "raw": "application/octet-stream",
+    "string": "text/plain",
 }
 
 
-def serialize_request_body(request: Any, request_type: type, request_field_name: str, nullable: bool, optional: bool, serialization_method: str, encoder=None) -> Tuple[
-        Optional[str], Optional[Any], Optional[Any]]:
+def serialize_request_body(
+    request: Any,
+    request_type: type,
+    request_field_name: str,
+    nullable: bool,
+    optional: bool,
+    serialization_method: str,
+    encoder=None,
+) -> Tuple[Optional[str], Optional[Any], Optional[Any]]:
     if request is None:
         if not nullable and optional:
             return None, None, None
 
     if not is_dataclass(request) or not hasattr(request, request_field_name):
-        return serialize_content_type(request_field_name, request_type, SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method],
-                                      request, encoder)
+        return serialize_content_type(
+            request_field_name,
+            request_type,
+            SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method],
+            request,
+            encoder,
+        )
 
     request_val = getattr(request, request_field_name)
 
     if request_val is None:
         if not nullable and optional:
             return None, None, None
 
     request_fields: Tuple[Field, ...] = fields(request)
     request_metadata = None
 
     for field in request_fields:
         if field.name == request_field_name:
-            request_metadata = field.metadata.get('request')
+            request_metadata = field.metadata.get("request")
             break
 
     if request_metadata is None:
-        raise Exception('invalid request type')
+        raise Exception("invalid request type")
 
-    return serialize_content_type(request_field_name, request_type, request_metadata.get('media_type', 'application/octet-stream'),
-                                  request_val)
+    return serialize_content_type(
+        request_field_name,
+        request_type,
+        request_metadata.get("media_type", "application/octet-stream"),
+        request_val,
+    )
 
 
-def serialize_content_type(field_name: str, request_type: Any, media_type: str, request: Any, encoder=None) -> Tuple[Optional[str], Optional[Any], Optional[List[List[Any]]]]:
-    if re.match(r'(application|text)\/.*?\+*json.*', media_type) is not None:
+def serialize_content_type(
+    field_name: str, request_type: Any, media_type: str, request: Any, encoder=None
+) -> Tuple[Optional[str], Optional[Any], Optional[List[List[Any]]]]:
+    if re.match(r"(application|text)\/.*?\+*json.*", media_type) is not None:
         return media_type, marshal_json(request, request_type, encoder), None
-    if re.match(r'multipart\/.*', media_type) is not None:
+    if re.match(r"multipart\/.*", media_type) is not None:
         return serialize_multipart_form(media_type, request)
-    if re.match(r'application\/x-www-form-urlencoded.*', media_type) is not None:
+    if re.match(r"application\/x-www-form-urlencoded.*", media_type) is not None:
         return media_type, serialize_form_data(field_name, request), None
     if isinstance(request, (bytes, bytearray)):
         return media_type, request, None
     if isinstance(request, str):
         return media_type, request, None
 
     raise Exception(
-        f"invalid request body type {type(request)} for mediaType {media_type}")
+        f"invalid request body type {type(request)} for mediaType {media_type}"
+    )
 
 
-def serialize_multipart_form(media_type: str, request: Any) -> Tuple[str, Any, List[List[Any]]]:
+def serialize_multipart_form(
+    media_type: str, request: Any
+) -> Tuple[str, Any, List[List[Any]]]:
     form: List[List[Any]] = []
     request_fields = fields(request)
 
     for field in request_fields:
         val = getattr(request, field.name)
         if val is None:
             continue
 
-        field_metadata = field.metadata.get('multipart_form')
+        field_metadata = field.metadata.get("multipart_form")
         if not field_metadata:
             continue
 
         if field_metadata.get("file") is True:
             file_fields = fields(val)
 
             file_name = ""
             field_name = ""
             content = bytes()
 
             for file_field in file_fields:
-                file_metadata = file_field.metadata.get('multipart_form')
+                file_metadata = file_field.metadata.get("multipart_form")
                 if file_metadata is None:
                     continue
 
                 if file_metadata.get("content") is True:
                     content = getattr(val, file_field.name)
                 else:
-                    field_name = file_metadata.get(
-                        "field_name", file_field.name)
+                    field_name = file_metadata.get("field_name", file_field.name)
                     file_name = getattr(val, file_field.name)
             if field_name == "" or file_name == "" or content == bytes():
-                raise Exception('invalid multipart/form-data file')
+                raise Exception("invalid multipart/form-data file")
 
             form.append([field_name, [file_name, content]])
         elif field_metadata.get("json") is True:
-            to_append = [field_metadata.get("field_name", field.name), [
-                None, marshal_json(val, field.type), "application/json"]]
+            to_append = [
+                field_metadata.get("field_name", field.name),
+                [None, marshal_json(val, field.type), "application/json"],
+            ]
             form.append(to_append)
         else:
-            field_name = field_metadata.get(
-                "field_name", field.name)
+            field_name = field_metadata.get("field_name", field.name)
             if isinstance(val, List):
                 for value in val:
                     if value is None:
                         continue
-                    form.append(
-                        [field_name + "[]", [None, _val_to_string(value)]])
+                    form.append([field_name + "[]", [None, _val_to_string(value)]])
             else:
                 form.append([field_name, [None, _val_to_string(val)]])
     return media_type, None, form
 
 
-def serialize_dict(original: Dict, explode: bool, field_name, existing: Optional[Dict[str, List[str]]]) -> Dict[
-        str, List[str]]:
+def serialize_dict(
+    original: Dict, explode: bool, field_name, existing: Optional[Dict[str, List[str]]]
+) -> Dict[str, List[str]]:
     if existing is None:
         existing = {}
 
     if explode is True:
         for key, val in original.items():
             if key not in existing:
                 existing[key] = []
@@ -510,215 +649,218 @@
 
     if is_dataclass(data):
         for field in fields(data):
             val = getattr(data, field.name)
             if val is None:
                 continue
 
-            metadata = field.metadata.get('form')
+            metadata = field.metadata.get("form")
             if metadata is None:
                 continue
 
-            field_name = metadata.get('field_name', field.name)
+            field_name = metadata.get("field_name", field.name)
 
-            if metadata.get('json'):
+            if metadata.get("json"):
                 form[field_name] = [marshal_json(val, field.type)]
             else:
-                if metadata.get('style', 'form') == 'form':
-                    form = {**form, **_populate_form(
-                        field_name, metadata.get('explode', True), val, _get_form_field_name, ",")}
+                if metadata.get("style", "form") == "form":
+                    _populate_form(
+                        field_name,
+                        metadata.get("explode", True),
+                        val,
+                        _get_form_field_name,
+                        ",",
+                        form,
+                    )
                 else:
-                    raise Exception(
-                        f'Invalid form style for field {field.name}')
+                    raise Exception(f"Invalid form style for field {field.name}")
     elif isinstance(data, Dict):
         for key, value in data.items():
             form[key] = [_val_to_string(value)]
     else:
-        raise Exception(f'Invalid request body type for field {field_name}')
+        raise Exception(f"Invalid request body type for field {field_name}")
 
     return form
 
 
 def _get_form_field_name(obj_field: Field) -> str:
-    obj_param_metadata = obj_field.metadata.get('form')
+    obj_param_metadata = obj_field.metadata.get("form")
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _populate_form(field_name: str, explode: boolean, obj: Any, get_field_name_func: Callable, delimiter: str) -> \
-        Dict[str, List[str]]:
-    params: Dict[str, List[str]] = {}
-
+def _populate_form(
+    field_name: str,
+    explode: boolean,
+    obj: Any,
+    get_field_name_func: Callable,
+    delimiter: str,
+    form: Dict[str, List[str]],
+):
     if obj is None:
-        return params
+        return form
 
     if is_dataclass(obj):
         items = []
 
         obj_fields: Tuple[Field, ...] = fields(obj)
         for obj_field in obj_fields:
             obj_field_name = get_field_name_func(obj_field)
-            if obj_field_name == '':
+            if obj_field_name == "":
                 continue
 
             val = getattr(obj, obj_field.name)
             if val is None:
                 continue
 
             if explode:
-                params[obj_field_name] = [_val_to_string(val)]
+                form[obj_field_name] = [_val_to_string(val)]
             else:
-                items.append(
-                    f'{obj_field_name}{delimiter}{_val_to_string(val)}')
+                items.append(f"{obj_field_name}{delimiter}{_val_to_string(val)}")
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join(items)]
+            form[field_name] = [delimiter.join(items)]
     elif isinstance(obj, Dict):
         items = []
         for key, value in obj.items():
             if value is None:
                 continue
 
             if explode:
-                params[key] = [_val_to_string(value)]
+                form[key] = [_val_to_string(value)]
             else:
-                items.append(f'{key}{delimiter}{_val_to_string(value)}')
+                items.append(f"{key}{delimiter}{_val_to_string(value)}")
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join(items)]
+            form[field_name] = [delimiter.join(items)]
     elif isinstance(obj, List):
         items = []
 
         for value in obj:
             if value is None:
                 continue
 
             if explode:
-                if not field_name in params:
-                    params[field_name] = []
-                params[field_name].append(_val_to_string(value))
+                if not field_name in form:
+                    form[field_name] = []
+                form[field_name].append(_val_to_string(value))
             else:
                 items.append(_val_to_string(value))
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join(
-                [str(item) for item in items])]
+            form[field_name] = [delimiter.join([str(item) for item in items])]
     else:
-        params[field_name] = [_val_to_string(obj)]
+        form[field_name] = [_val_to_string(obj)]
 
-    return params
+    return form
 
 
 def _serialize_header(explode: bool, obj: Any) -> str:
     if obj is None:
-        return ''
+        return ""
 
     if is_dataclass(obj):
         items = []
         obj_fields: Tuple[Field, ...] = fields(obj)
         for obj_field in obj_fields:
-            obj_param_metadata = obj_field.metadata.get('header')
+            obj_param_metadata = obj_field.metadata.get("header")
 
             if not obj_param_metadata:
                 continue
 
-            obj_field_name = obj_param_metadata.get(
-                'field_name', obj_field.name)
-            if obj_field_name == '':
+            obj_field_name = obj_param_metadata.get("field_name", obj_field.name)
+            if obj_field_name == "":
                 continue
 
             val = getattr(obj, obj_field.name)
             if val is None:
                 continue
 
             if explode:
-                items.append(
-                    f'{obj_field_name}={_val_to_string(val)}')
+                items.append(f"{obj_field_name}={_val_to_string(val)}")
             else:
                 items.append(obj_field_name)
                 items.append(_val_to_string(val))
 
         if len(items) > 0:
-            return ','.join(items)
+            return ",".join(items)
     elif isinstance(obj, Dict):
         items = []
 
         for key, value in obj.items():
             if value is None:
                 continue
 
             if explode:
-                items.append(f'{key}={_val_to_string(value)}')
+                items.append(f"{key}={_val_to_string(value)}")
             else:
                 items.append(key)
                 items.append(_val_to_string(value))
 
         if len(items) > 0:
-            return ','.join([str(item) for item in items])
+            return ",".join([str(item) for item in items])
     elif isinstance(obj, List):
         items = []
 
         for value in obj:
             if value is None:
                 continue
 
             items.append(_val_to_string(value))
 
         if len(items) > 0:
-            return ','.join(items)
+            return ",".join(items)
     else:
-        return f'{_val_to_string(obj)}'
+        return f"{_val_to_string(obj)}"
 
-    return ''
+    return ""
 
 
 def unmarshal_json(data, typ, decoder=None):
-    unmarshal = make_dataclass('Unmarshal', [('res', typ)],
-                               bases=(DataClassJsonMixin,))
+    unmarshal = make_dataclass("Unmarshal", [("res", typ)], bases=(DataClassJsonMixin,))
     json_dict = json.loads(data)
     try:
         out = unmarshal.from_dict({"res": json_dict})
     except AttributeError as attr_err:
         raise AttributeError(
-            f'unable to unmarshal {data} as {typ} - {attr_err}') from attr_err
+            f"unable to unmarshal {data} as {typ} - {attr_err}"
+        ) from attr_err
 
     return out.res if decoder is None else decoder(out.res)
 
 
 def marshal_json(val, typ, encoder=None):
     if not is_optional_type(typ) and val is None:
-        raise ValueError(
-            f"Could not marshal None into non-optional type: {typ}")
+        raise ValueError(f"Could not marshal None into non-optional type: {typ}")
 
-    marshal = make_dataclass('Marshal', [('res', typ)],
-                             bases=(DataClassJsonMixin,))
+    marshal = make_dataclass("Marshal", [("res", typ)], bases=(DataClassJsonMixin,))
     marshaller = marshal(res=val)
     json_dict = marshaller.to_dict()
     val = json_dict["res"] if encoder is None else encoder(json_dict["res"])
 
-    return json.dumps(val, separators=(',', ':'), sort_keys=True)
+    return json.dumps(val, separators=(",", ":"), sort_keys=True)
 
 
 def match_content_type(content_type: str, pattern: str) -> boolean:
     if pattern in (content_type, "*", "*/*"):
         return True
 
     msg = Message()
-    msg['content-type'] = content_type
+    msg["content-type"] = content_type
     media_type = msg.get_content_type()
 
     if media_type == pattern:
         return True
 
     parts = media_type.split("/")
     if len(parts) == 2:
-        if pattern in (f'{parts[0]}/*', f'*/{parts[1]}'):
+        if pattern in (f"{parts[0]}/*", f"*/{parts[1]}"):
             return True
 
     return False
 
 
 def match_status_codes(status_codes: List[str], status_code: int) -> bool:
     for code in status_codes:
@@ -835,64 +977,84 @@
 
 
 def union_encoder(all_encoders: Dict[str, Callable]):
     def selective_encoder(val: Any):
         if type(val) in all_encoders:
             return all_encoders[type(val)](val)
         return val
+
     return selective_encoder
 
 
 def union_decoder(all_decoders: List[Callable]):
     def selective_decoder(val: Any):
         decoded = val
         for decoder in all_decoders:
             try:
                 decoded = decoder(val)
                 break
             except (TypeError, ValueError):
                 continue
         return decoded
+
     return selective_decoder
 
 
 def get_field_name(name):
     def override(_, _field_name=name):
         return _field_name
 
     return override
 
 
 def _val_to_string(val) -> str:
     if isinstance(val, bool):
         return str(val).lower()
     if isinstance(val, datetime):
-        return str(val.isoformat().replace('+00:00', 'Z'))
+        return str(val.isoformat().replace("+00:00", "Z"))
     if isinstance(val, Enum):
         return str(val.value)
 
     return str(val)
 
 
-def _populate_from_globals(param_name: str, value: Any, param_type: str, gbls: Optional[Dict[str, Dict[str, Dict[str, Any]]]]):
-    if value is None and gbls is not None:
-        if 'parameters' in gbls:
-            if param_type in gbls['parameters']:
-                if param_name in gbls['parameters'][param_type]:
-                    global_value = gbls['parameters'][param_type][param_name]
-                    if global_value is not None:
-                        value = global_value
+def _populate_from_globals(
+    param_name: str, value: Any, param_type: str, gbls: Any
+) -> Tuple[Any, bool]:
+    if gbls is None:
+        return value, False
+
+    global_fields = fields(gbls)
+
+    found = False
+    for field in global_fields:
+        if field.name is not param_name:
+            continue
+
+        found = True
+
+        if value is not None:
+            return value, True
 
-    return value
+        global_value = getattr(gbls, field.name)
+
+        param_metadata = field.metadata.get(param_type)
+        if param_metadata is None:
+            return value, True
+
+        return global_value, True
+
+    return value, found
 
 
 def decoder_with_discriminator(field_name):
     def decode_fx(obj):
-        kls = getattr(sys.modules['sdk.models.components'], obj[field_name])
+        kls = getattr(sys.modules["sdk.models.components"], obj[field_name])
         return unmarshal_json(json.dumps(obj), kls)
+
     return decode_fx
 
 
 def remove_suffix(input_string, suffix):
     if suffix and input_string.endswith(suffix):
-        return input_string[:-len(suffix)]
+        return input_string[: -len(suffix)]
     return input_string
```

### Comparing `plex-api-client-0.6.2/src/plex_api/video.py` & `plex-api-client-0.6.3/src/plex_api/video.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         url = base_url + '/:/timeline'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetTimelineRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -85,15 +85,15 @@
         url = base_url + '/video/:/transcode/universal/start.mpd'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.StartUniversalTranscodeRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `plex-api-client-0.6.2/src/plex_api_client.egg-info/PKG-INFO` & `plex-api-client-0.6.3/src/plex_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-api-client
-Version: 0.6.2
+Version: 0.6.3
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/LukeHagar/plexpy.git
 Author: LukeHagar
 License: UNKNOWN
 Description: # plexpy
         
         <div align="left">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plex-api-client Version: 0.6.2 Summary: Python
+Metadata-Version: 2.1 Name: plex-api-client Version: 0.6.3 Summary: Python
 Client SDK Generated by Speakeasy Home-page: https://github.com/LukeHagar/
 plexpy.git Author: LukeHagar License: UNKNOWN Description: # plexpy
 _[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
 _2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]
 ## SDK Installation ```bash pip install plex-api-client ``` ## SDK Example
 Usage ### Example ```python import plex_api s = plex_api.PlexAPI
```

### Comparing `plex-api-client-0.6.2/src/plex_api_client.egg-info/SOURCES.txt` & `plex-api-client-0.6.3/src/plex_api_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,16 @@
 src/plex_api/models/errors/startuniversaltranscode.py
 src/plex_api/models/errors/stopalltasks.py
 src/plex_api/models/errors/stoptask.py
 src/plex_api/models/errors/stoptranscodesession.py
 src/plex_api/models/errors/updateplaylist.py
 src/plex_api/models/errors/updateplayprogress.py
 src/plex_api/models/errors/uploadplaylist.py
+src/plex_api/models/internal/__init__.py
+src/plex_api/models/internal/globals.py
 src/plex_api/models/operations/__init__.py
 src/plex_api/models/operations/addplaylistcontents.py
 src/plex_api/models/operations/applyupdates.py
 src/plex_api/models/operations/cancelserveractivities.py
 src/plex_api/models/operations/checkforupdates.py
 src/plex_api/models/operations/clearplaylistcontents.py
 src/plex_api/models/operations/createplaylist.py
```

