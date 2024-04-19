# Comparing `tmp/netbox_topology_views-3.9.1.tar.gz` & `tmp/netbox-topology-views-3.9b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_topology_views-3.9.1.tar", last modified: Fri Apr 19 13:56:14 2024, max compression
+gzip compressed data, was "netbox-topology-views-3.9b1.tar", last modified: Tue Jan  2 11:24:09 2024, max compression
```

## Comparing `netbox_topology_views-3.9.1.tar` & `netbox-topology-views-3.9b1.tar`

### file list

```diff
@@ -1,127 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:56:14.960331 netbox_topology_views-3.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12645 2024-04-19 13:56:14.960331 netbox_topology_views-3.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12107 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:56:14.940331 netbox_topology_views-3.9.1/netbox_topology_views/
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:56:14.944331 netbox_topology_views-3.9.1/netbox_topology_views/api/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    11410 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    19831 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:56:14.944331 netbox_topology_views-3.9.1/netbox_topology_views/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/migrations/0002_individualoptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/migrations/0003_individualoptions_show_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/migrations/0004_coordinategroup_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/migrations/0005_individualoptions_save_coords.py
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/migrations/0006_powerpanelcoordinate_powerfeedcoordinate_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/migrations/0007_individualoptions_group_locations_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13704 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/navigation.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/search.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:56:14.940331 netbox_topology_views-3.9.1/netbox_topology_views/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:56:14.940331 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:56:14.944331 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/css/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/css/app.css
--rw-r--r--   0 runner    (1001) docker     (127)   220074 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/css/vendor.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:56:14.956331 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/
--rw-r--r--   0 runner    (1001) docker     (127)    20139 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/access-switch.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/backhaul.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/backup.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/cable-doubler.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/camera-server.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/camera.svg
--rw-r--r--   0 runner    (1001) docker     (127)    10537 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/circuit.svg
--rw-r--r--   0 runner    (1001) docker     (127)    10590 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/console-server.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/core-router.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6603 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/core-switch.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/database-server.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/database.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7899 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/dect-station.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/desktop.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9148 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/distribution-switch.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/docking-station.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/environment-monitor.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9309 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/fire-alarm-control-panel.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/firewall.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/fo-patch-panel.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/intrusion-alarm-system.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/kvm-over-ip.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/kvm.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/load-balancer.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/mobile-phone.svg
--rw-r--r--   0 runner    (1001) docker     (127)    17466 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/modem.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/network-socket.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/notebook.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9374 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/pabx.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/patch-panel.svg
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/pdu.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/phone.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/power-panel.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/power-units.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/printer.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/provider-networks.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/proxy.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/role-unknown.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/router.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/server.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/siem.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/storage.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/switch.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7764 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/time-recording-terminal.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/ups.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7585 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/usb-lan-adapter.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/wan-network.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/wireless-ap.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:56:14.956331 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/js/
--rw-r--r--   0 runner    (1001) docker     (127)   346518 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/js/app.js
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/js/images.js
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/js/images.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:56:14.940331 netbox_topology_views-3.9.1/netbox_topology_views/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:56:14.960331 netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/circuitcoordinate.html
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/circuitcoordinate_add.html
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/circuitcoordinate_edit.html
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/circuitcoordinate_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/coordinate.html
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/coordinate_add.html
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/coordinate_edit.html
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/coordinate_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/coordinategroup.html
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/coordinategroup_add.html
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/coordinategroup_edit.html
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/coordinategroup_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/htmx_topology.html
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/images.html
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/individual_options.html
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/location_button.html
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/powerfeedcoordinate.html
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/powerfeedcoordinate_add.html
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/powerfeedcoordinate_edit.html
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/powerfeedcoordinate_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/powerpanelcoordinate.html
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/powerpanelcoordinate_add.html
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/powerpanelcoordinate_edit.html
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/powerpanelcoordinate_list.html
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/site_button.html
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/toasts.html
--rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    11274 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    46994 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/netbox_topology_views/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:56:14.960331 netbox_topology_views-3.9.1/netbox_topology_views.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12645 2024-04-19 13:56:14.000000 netbox_topology_views-3.9.1/netbox_topology_views.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-04-19 13:56:14.000000 netbox_topology_views-3.9.1/netbox_topology_views.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:56:14.000000 netbox_topology_views-3.9.1/netbox_topology_views.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 13:56:14.000000 netbox_topology_views-3.9.1/netbox_topology_views.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 13:56:14.960331 netbox_topology_views-3.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-19 13:56:10.000000 netbox_topology_views-3.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 11:24:09.058412 netbox-topology-views-3.9b1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12645 2024-01-02 11:24:09.058412 netbox-topology-views-3.9b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12107 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 11:24:09.042412 netbox-topology-views-3.9b1/netbox_topology_views/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 11:24:09.042412 netbox-topology-views-3.9b1/netbox_topology_views/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9012 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18563 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 11:24:09.042412 netbox-topology-views-3.9b1/netbox_topology_views/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/migrations/0002_individualoptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/migrations/0003_individualoptions_show_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/migrations/0004_coordinategroup_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/migrations/0005_individualoptions_save_coords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/migrations/0006_powerpanelcoordinate_powerfeedcoordinate_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13303 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 11:24:09.038412 netbox-topology-views-3.9b1/netbox_topology_views/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 11:24:09.038412 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 11:24:09.042412 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/css/app.css
+-rw-r--r--   0 runner    (1001) docker     (127)   220074 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/css/vendor.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 11:24:09.050412 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    20139 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/access-switch.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/backhaul.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/backup.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/cable-doubler.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/camera-server.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/camera.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    10537 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/circuit.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    10590 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/console-server.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/core-router.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6603 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/core-switch.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/database-server.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/database.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7899 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/dect-station.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/desktop.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9148 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/distribution-switch.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/docking-station.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/environment-monitor.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9309 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/fire-alarm-control-panel.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/firewall.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/fo-patch-panel.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/intrusion-alarm-system.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/kvm-over-ip.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/kvm.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/load-balancer.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/mobile-phone.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    17466 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/modem.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/network-socket.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/notebook.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9374 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/pabx.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/patch-panel.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/pdu.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/phone.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/power-panel.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/power-units.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/printer.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/provider-networks.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/proxy.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/role-unknown.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/router.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/server.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/siem.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/storage.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/switch.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7764 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/time-recording-terminal.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/ups.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7585 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/usb-lan-adapter.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/wan-network.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/wireless-ap.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 11:24:09.054412 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   344153 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/js/app.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/js/images.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/js/images.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 11:24:09.038412 netbox-topology-views-3.9b1/netbox_topology_views/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 11:24:09.058412 netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/circuitcoordinate.html
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/circuitcoordinate_add.html
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/circuitcoordinate_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/circuitcoordinate_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/coordinate.html
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/coordinate_add.html
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/coordinate_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/coordinate_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/coordinategroup.html
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/coordinategroup_add.html
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/coordinategroup_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/coordinategroup_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/htmx_topology.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/images.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/individual_options.html
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/location_button.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/powerfeedcoordinate.html
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/powerfeedcoordinate_add.html
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/powerfeedcoordinate_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/powerfeedcoordinate_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/powerpanelcoordinate.html
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/powerpanelcoordinate_add.html
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/powerpanelcoordinate_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/powerpanelcoordinate_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/site_button.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/toasts.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10681 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43522 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/netbox_topology_views/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 11:24:09.058412 netbox-topology-views-3.9b1/netbox_topology_views.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12645 2024-01-02 11:24:09.000000 netbox-topology-views-3.9b1/netbox_topology_views.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7082 2024-01-02 11:24:09.000000 netbox-topology-views-3.9b1/netbox_topology_views.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-02 11:24:09.000000 netbox-topology-views-3.9b1/netbox_topology_views.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-02 11:24:09.000000 netbox-topology-views-3.9b1/netbox_topology_views.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-02 11:24:09.058412 netbox-topology-views-3.9b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-01-02 11:24:01.000000 netbox-topology-views-3.9b1/setup.py
```

### Comparing `netbox_topology_views-3.9.1/LICENSE` & `netbox-topology-views-3.9b1/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/PKG-INFO` & `netbox-topology-views-3.9b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-topology-views
-Version: 3.9.1
+Version: 3.9b1
 Summary: An NetBox plugin to create Topology maps
 Home-page: https://github.com/mattieserver/netbox-topology-views
 Author: Mattijs Vanhaverbeke
 License: Apache 2.0
 Project-URL: Source, https://github.com/mattieserver/netbox-topology-views
 Keywords: netbox-plugin
 Classifier: Programming Language :: Python
```

### Comparing `netbox_topology_views-3.9.1/README.md` & `netbox-topology-views-3.9b1/README.md`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/__init__.py` & `netbox-topology-views-3.9b1/netbox_topology_views/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from extras.plugins import PluginConfig
 
 
 class TopologyViewsConfig(PluginConfig):
     name = "netbox_topology_views"
     verbose_name = "Topology views"
     description = "An plugin to render topology maps"
-    version = "3.9.1"
+    version = "3.9-beta1"
     author = "Mattijs Vanhaverbeke"
     author_email = "author@example.com"
     base_url = "netbox_topology_views"
     required_settings = []
     default_settings = {
         "static_image_directory": "netbox_topology_views/img",
         "allow_coordinates_saving": False,
```

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/api/serializers.py` & `netbox-topology-views-3.9b1/netbox_topology_views/api/serializers.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,8 +46,8 @@
     class Meta:
         model = PowerFeedCoordinate
         fields = ("x", "y")
 
 class IndividualOptionsSerializer(NetBoxModelSerializer):
     class Meta:
         model = IndividualOptions
-        fields = ("ignore_cable_type", "save_coords", "show_unconnected", "show_cables", "show_logical_connections", "show_single_cable_logical_conns", "show_neighbors", "show_circuit", "show_power", "show_wireless", "group_sites", "group_locations", "group_racks", "draw_default_layout")
+        fields = ("ignore_cable_type", "save_coords", "show_unconnected", "show_cables", "show_logical_connections", "show_single_cable_logical_conns", "show_neighbors", "show_circuit", "show_power", "show_wireless", "draw_default_layout")
```

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/api/views.py` & `netbox-topology-views-3.9b1/netbox_topology_views/api/views.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Dict
 import sys
 
 from circuits.models import Circuit
 from dcim.models import Device, DeviceRole, PowerFeed, PowerPanel
-from extras.models import SavedFilter
 from django.conf import settings
 from django.contrib.auth.mixins import PermissionRequiredMixin
 from django.contrib.contenttypes.models import ContentType
 from django.http import HttpResponse, JsonResponse
 from rest_framework.decorators import action
 from rest_framework.response import Response
 from rest_framework.viewsets import ReadOnlyModelViewSet, ViewSet
@@ -105,38 +104,15 @@
 
         individualOptions, created = IndividualOptions.objects.get_or_create(
             user_id=request.user.id,
         )
 
         if request.GET:
 
-            filter_id, save_coords, show_unconnected, show_power, show_circuit, show_logical_connections, show_single_cable_logical_conns, show_cables, show_wireless, group_sites, group_locations, group_racks,show_neighbors = get_query_settings(request)
-
-            # Read options from saved filters as NetBox does not handle custom plugin filters
-            if "filter_id" in request.GET and request.GET["filter_id"] != '':
-                try:
-                    saved_filter = SavedFilter.objects.get(pk=filter_id)
-                    saved_filter_params = getattr(saved_filter, 'parameters')
-
-                    if save_coords == False and 'save_coords' in saved_filter_params: save_coords = saved_filter_params['save_coords']
-                    if show_power == False and 'show_power' in saved_filter_params: show_power = saved_filter_params['show_power']
-                    if show_circuit == False and 'show_circuit' in saved_filter_params: show_circuit = saved_filter_params['show_circuit']
-                    if show_logical_connections == False and 'show_logical_connections' in saved_filter_params: show_logical_connections = saved_filter_params['show_logical_connections']
-                    if show_single_cable_logical_conns == False and 'show_single_cable_logical_conns' in saved_filter_params: show_single_cable_logical_conns = saved_filter_params['show_single_cable_logical_conns']
-                    if show_cables == False and 'show_cables' in saved_filter_params: show_cables = saved_filter_params['show_cables']
-                    if show_wireless == False and 'show_wireless' in saved_filter_params: show_wireless = saved_filter_params['show_wireless']
-                    if group_sites == False and 'group_sites' in saved_filter_params: group_sites = saved_filter_params['group_sites']
-                    if group_locations == False and 'group_locations' in saved_filter_params: group_locations = saved_filter_params['group_locations']
-                    if group_racks == False and 'group_racks' in saved_filter_params: group_racks = saved_filter_params['group_racks']
-                    if show_neighbors == False and 'show_neighbors' in saved_filter_params: show_neighbors = saved_filter_params['show_neighbors']
-                except SavedFilter.DoesNotExist: # filter_id not found
-                    pass
-                except Exception as inst:
-                    print(type(inst))
-
+            save_coords, show_unconnected, show_power, show_circuit, show_logical_connections, show_single_cable_logical_conns, show_cables, show_wireless, show_neighbors = get_query_settings(request)
             if 'group' not in request.query_params:
                 group_id = "default"
             else:
                 group_id = request.query_params["group"]
             topo_data = get_topology_data(
                 queryset=self.queryset,
                 individualOptions=individualOptions,
@@ -145,17 +121,14 @@
                 show_cables=show_cables,
                 show_logical_connections=show_logical_connections,
                 show_single_cable_logical_conns=show_single_cable_logical_conns,
                 show_neighbors=show_neighbors,
                 show_circuit=show_circuit,
                 show_power=show_power,
                 show_wireless=show_wireless,
-                group_sites=group_sites,
-                group_locations=group_locations,
-                group_racks=group_racks,
                 group_id=group_id,
             )
             xml_data = export_data_to_xml(topo_data).decode('utf-8')
 
             return HttpResponse(xml_data, content_type="application/xml; charset=utf-8")
         else:
             return JsonResponse(
```

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/filters.py` & `netbox-topology-views-3.9b1/netbox_topology_views/filters.py`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/forms.py` & `netbox-topology-views-3.9b1/netbox_topology_views/forms.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,16 +31,15 @@
 ):
     default_renderer = forms.renderers.DjangoTemplates()
     model = Device
     fieldsets = (
         (None, ('q', 'filter_id', 'tag')),
         (_('Options'), (
             'group', 'save_coords', 'show_unconnected', 'show_cables', 'show_logical_connections',
-            'show_single_cable_logical_conns', 'show_neighbors', 'show_circuit', 'show_power', 'show_wireless', 
-            'group_sites', 'group_locations', 'group_racks'
+            'show_single_cable_logical_conns', 'show_neighbors', 'show_circuit', 'show_power', 'show_wireless',
         )),
         (_('Device'), ('id',)),        
         (_('Location'), ('region_id', 'site_group_id', 'site_id', 'location_id', 'rack_id')),
         (_('Operation'), ('status', 'role_id', 'airflow', 'serial', 'asset_tag', 'mac_address')),
         (_('Hardware'), ('manufacturer_id', 'device_type_id', 'platform_id')),
         (_('Tenant'), ('tenant_group_id', 'tenant_id')),
         (_('Contacts'), ('contact', 'contact_role', 'contact_group')),
@@ -255,23 +254,14 @@
     )
     show_power = forms.BooleanField(
         label=_('Show Power Feeds'), required=False, initial=False
     )
     show_wireless = forms.BooleanField(
         label =_('Show Wireless Links'), required=False, initial=False
     )
-    group_sites = forms.BooleanField(
-        label =_('Group Sites'), required=False, initial=False
-    )
-    group_locations = forms.BooleanField(
-        label =_('Group Locations'), required=False, initial=False
-    )
-    group_racks = forms.BooleanField(
-        label =_('Group Racks'), required=False, initial=False
-    )
 
 class CoordinateGroupsForm(NetBoxModelForm):
     fieldsets = (
         ('Group Details', ('name', 'description')),
     )
 
     class Meta:
@@ -453,17 +443,14 @@
                 'show_cables',
                 'show_logical_connections',
                 'show_single_cable_logical_conns',
                 'show_neighbors',
                 'show_circuit',
                 'show_power',
                 'show_wireless',
-                'group_sites',
-                'group_locations',
-                'group_racks',
                 'draw_default_layout',
             ),
         ),
     )
 
     user_id = forms.CharField(widget=forms.HiddenInput())
 
@@ -557,44 +544,20 @@
     show_wireless = forms.BooleanField(
         label =_('Show Wireless Links'), 
         required=False, 
         initial=False,
         help_text=_('Displays wireless connections. These connections are '
             'displayed as blue dotted lines.')
     )
-    group_sites = forms.BooleanField(
-        label =_('Group Sites'), 
-        required=False, 
-        initial=False,
-        help_text=_('Draws a rectangle around Devices that belong to the '
-            'same site.')
-    )
-    group_locations = forms.BooleanField(
-        label =_('Group Locations'), 
-        required=False, 
-        initial=False,
-        help_text=_('Draws a rectangle around Devices that belong to the '
-            'same location.')
-    )
-    group_racks = forms.BooleanField(
-        label =_('Group Racks'), 
-        required=False, 
-        initial=False,
-        help_text=_('Draws a rectangle around Devices that belong to the '
-            'same rack.')
-    )
     draw_default_layout = forms.BooleanField(
         label = ('Draw Default Layout'),
         required=False,
         initial=False,
         help_text=_('Enable this option if you want to draw the topology on '
             'the initial load (when you go to the topology plugin page).')
     )
 
     class Meta:
         model = IndividualOptions
         fields = [
-            'user_id', 'ignore_cable_type', 'preselected_device_roles', 'preselected_tags', 
-            'save_coords', 'show_unconnected', 'show_cables', 'show_logical_connections', 
-            'show_single_cable_logical_conns', 'show_neighbors', 'show_circuit', 'show_power', 
-            'show_wireless', 'group_sites', 'group_locations', 'group_racks', 'draw_default_layout'
+            'user_id', 'ignore_cable_type', 'preselected_device_roles', 'preselected_tags', 'save_coords', 'show_unconnected', 'show_cables', 'show_logical_connections', 'show_single_cable_logical_conns', 'show_neighbors', 'show_circuit', 'show_power', 'show_wireless', 'draw_default_layout'
         ]
```

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/migrations/0001_initial.py` & `netbox-topology-views-3.9b1/netbox_topology_views/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/migrations/0002_individualoptions.py` & `netbox-topology-views-3.9b1/netbox_topology_views/migrations/0002_individualoptions.py`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/migrations/0004_coordinategroup_coordinate.py` & `netbox-topology-views-3.9b1/netbox_topology_views/migrations/0004_coordinategroup_coordinate.py`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/migrations/0006_powerpanelcoordinate_powerfeedcoordinate_and_more.py` & `netbox-topology-views-3.9b1/netbox_topology_views/migrations/0006_powerpanelcoordinate_powerfeedcoordinate_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/models.py` & `netbox-topology-views-3.9b1/netbox_topology_views/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,16 +37,14 @@
     image = models.CharField("Path within the netbox static directory", max_length=255)
 
     content_type = models.ForeignKey(ContentType, on_delete=models.CASCADE)
     object_id = models.PositiveIntegerField(null=True, blank=True)
 
     __role: Optional[Role] = None
 
-    _netbox_private = True
-
     @property
     def role(self) -> Role:
         if self.__role:
             return self.__role
 
         model_class = self.content_type.model_class()
 
@@ -109,16 +107,14 @@
     )
 
     description = models.CharField(
         max_length=255,
         blank = True,
     )
 
-    _netbox_private = True
-
     class Meta:
         ordering = ['name']
 
     def __str__(self):
         return self.name
 
     def get_absolute_url(self):
@@ -138,16 +134,14 @@
             'Smaller values correspond to a position further to the left on the monitor.',
     )
     y = models.IntegerField(
         help_text='Y-coordinate of the device (vertical) on the canvas. '
             'Smaller values correspond to a position further up on the monitor.',
     )
 
-    _netbox_private = True
-
     def get_or_create_default_group(group_id):
         # Default group named "default" must always exist in order to make sure
         # that coordinate values can be stored even if no coordinate group has been
         # selected. The default group will be added automatically if it does not exist.
         try:
             if CoordinateGroup.objects.filter(name="default"):
                 group = CoordinateGroup.objects.get(name="default")
@@ -189,16 +183,14 @@
             'Smaller values correspond to a position further to the left on the monitor.',
     )
     y = models.IntegerField(
         help_text='Y-coordinate of the device (vertical) on the canvas. '
             'Smaller values correspond to a position further up on the monitor.',
     )
 
-    _netbox_private = True
-
     def get_or_create_default_group(group_id):
         # Default group named "default" must always exist in order to make sure
         # that coordinate values can be stored even if no coordinate group has been
         # selected. The default group will be added automatically if it does not exist.
         try:
             if CoordinateGroup.objects.filter(name="default"):
                 group = CoordinateGroup.objects.get(name="default")
@@ -240,16 +232,14 @@
             'Smaller values correspond to a position further to the left on the monitor.',
     )
     y = models.IntegerField(
         help_text='Y-coordinate of the device (vertical) on the canvas. '
             'Smaller values correspond to a position further up on the monitor.',
     )
 
-    _netbox_private = True
-
     def get_or_create_default_group(group_id):
         # Default group named "default" must always exist in order to make sure
         # that coordinate values can be stored even if no coordinate group has been
         # selected. The default group will be added automatically if it does not exist.
         try:
             if CoordinateGroup.objects.filter(name="default"):
                 group = CoordinateGroup.objects.get(name="default")
@@ -291,16 +281,14 @@
             'Smaller values correspond to a position further to the left on the monitor.',
     )
     y = models.IntegerField(
         help_text='Y-coordinate of the device (vertical) on the canvas. '
             'Smaller values correspond to a position further up on the monitor.',
     )
 
-    _netbox_private = True
-
     def get_or_create_default_group(group_id):
         # Default group named "default" must always exist in order to make sure
         # that coordinate values can be stored even if no coordinate group has been
         # selected. The default group will be added automatically if it does not exist.
         try:
             if CoordinateGroup.objects.filter(name="default"):
                 group = CoordinateGroup.objects.get(name="default")
@@ -382,24 +370,13 @@
     )
     show_power = models.BooleanField(
         default=False
     )
     show_wireless = models.BooleanField(
         default=False
     )
-    group_sites = models.BooleanField(
-        default=False
-    )
-    group_locations = models.BooleanField(
-        default=False
-    )
-    group_racks = models.BooleanField(
-        default=False
-    )
     draw_default_layout = models.BooleanField(
         default=False
     )
 
-    _netbox_private = True
-
     def __str___(self):
         return f"{self.user_id}"
```

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/navigation.py` & `netbox-topology-views-3.9b1/netbox_topology_views/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/signals.py` & `netbox-topology-views-3.9b1/netbox_topology_views/signals.py`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/css/vendor.css` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/css/vendor.css`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/LICENSE` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/access-switch.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/access-switch.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/backhaul.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/backhaul.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/backup.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/backup.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/cable-doubler.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/cable-doubler.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/camera-server.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/camera-server.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/camera.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/camera.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/circuit.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/circuit.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/console-server.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/console-server.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/core-router.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/core-router.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/core-switch.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/core-switch.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/database-server.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/database-server.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/database.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/database.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/dect-station.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/dect-station.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/desktop.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/desktop.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/distribution-switch.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/distribution-switch.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/docking-station.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/docking-station.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/environment-monitor.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/environment-monitor.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/fire-alarm-control-panel.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/fire-alarm-control-panel.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/firewall.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/firewall.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/fo-patch-panel.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/fo-patch-panel.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/intrusion-alarm-system.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/intrusion-alarm-system.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/kvm-over-ip.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/kvm-over-ip.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/kvm.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/kvm.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/load-balancer.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/load-balancer.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/mobile-phone.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/mobile-phone.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/modem.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/modem.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/network-socket.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/network-socket.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/notebook.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/notebook.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/pabx.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/pabx.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/patch-panel.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/patch-panel.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/pdu.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/pdu.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/phone.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/phone.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/power-panel.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/power-panel.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/power-units.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/power-units.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/printer.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/printer.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/provider-networks.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/provider-networks.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/proxy.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/proxy.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/role-unknown.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/role-unknown.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/router.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/router.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/server.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/server.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/siem.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/siem.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/storage.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/storage.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/switch.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/switch.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/time-recording-terminal.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/time-recording-terminal.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/ups.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/ups.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/usb-lan-adapter.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/usb-lan-adapter.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/wan-network.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/wan-network.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/img/wireless-ap.svg` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/img/wireless-ap.svg`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/js/app.js` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/js/app.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -11,21 +11,21 @@
         Cn = Object.prototype.propertyIsEnumerable;
     var Zt = (n, e, t) => e in n ? Tt(n, e, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: t
         }) : n[e] = t,
-        le = (n, e) => {
+        de = (n, e) => {
             for (var t in e || (e = {})) Wi.call(e, t) && Zt(n, t, e[t]);
             if (ji)
                 for (var t of ji(e)) Cn.call(e, t) && Zt(n, t, e[t]);
             return n
         },
-        Be = (n, e) => vn(n, _n(e)),
+        Me = (n, e) => vn(n, _n(e)),
         Tn = n => Tt(n, "__esModule", {
             value: !0
         });
     var kn = (n, e) => () => (e || n((e = {
         exports: {}
     }).exports, e), e.exports);
     var On = (n, e, t) => {
@@ -39,15 +39,15 @@
         Vi = n => On(Tn(Tt(n != null ? bn(xn(n)) : {}, "default", n && n.__esModule && "default" in n ? {
             get: () => n.default,
             enumerable: !0
         } : {
             value: n,
             enumerable: !0
         })), n);
-    var X = (n, e, t) => (Zt(n, typeof e != "symbol" ? e + "" : e, t), t);
+    var Y = (n, e, t) => (Zt(n, typeof e != "symbol" ? e + "" : e, t), t);
     var qi = (n, e, t) => new Promise((i, s) => {
         var o = d => {
                 try {
                     a(t.next(d))
                 } catch (h) {
                     s(h)
                 }
@@ -107,25 +107,25 @@
         };
         te.prototype.hasListeners = function(n) {
             return !!this.listeners(n).length
         }
     });
     var Os = Vi(Jt());
 
-    function ce() {
-        return ce = Object.assign || function(n) {
+    function he() {
+        return he = Object.assign || function(n) {
             for (var e = 1; e < arguments.length; e++) {
                 var t = arguments[e];
                 for (var i in t) Object.prototype.hasOwnProperty.call(t, i) && (n[i] = t[i])
             }
             return n
-        }, ce.apply(this, arguments)
+        }, he.apply(this, arguments)
     }
 
-    function ne(n, e) {
+    function oe(n, e) {
         n.prototype = Object.create(e.prototype), n.prototype.constructor = n, n.__proto__ = e
     }
 
     function kt(n) {
         if (n === void 0) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
         return n
     }
@@ -135,130 +135,130 @@
         for (var t = Object(e), i = 1; i < arguments.length; i++) {
             var s = arguments[i];
             if (s != null)
                 for (var o in s) s.hasOwnProperty(o) && (t[o] = s[o])
         }
         return t
     } : ei = Object.assign;
-    var Ae = ei,
+    var Fe = ei,
         Ui = ["", "webkit", "Moz", "MS", "ms", "o"],
         In = typeof document == "undefined" ? {
             style: {}
         } : document.createElement("div"),
         Pn = "function",
-        $e = Math.round,
-        ze = Math.abs,
+        Ke = Math.round,
+        Ne = Math.abs,
         ti = Date.now;
 
     function Ot(n, e) {
         for (var t, i, s = e[0].toUpperCase() + e.slice(1), o = 0; o < Ui.length;) {
             if (t = Ui[o], i = t ? t + s : e, i in n) return i;
             o++
         }
     }
-    var me;
-    typeof window == "undefined" ? me = {} : me = window;
+    var pe;
+    typeof window == "undefined" ? pe = {} : pe = window;
     var Yi = Ot(In.style, "touchAction"),
         Xi = Yi !== void 0;
 
-    function Mn() {
+    function Dn() {
         if (!Xi) return !1;
         var n = {},
-            e = me.CSS && me.CSS.supports;
+            e = pe.CSS && pe.CSS.supports;
         return ["auto", "manipulation", "pan-y", "pan-x", "pan-x pan-y", "none"].forEach(function(t) {
-            return n[t] = e ? me.CSS.supports("touch-action", t) : !0
+            return n[t] = e ? pe.CSS.supports("touch-action", t) : !0
         }), n
     }
     var Gi = "compute",
         Ki = "auto",
         ii = "manipulation",
-        Re = "none",
-        nt = "pan-x",
-        rt = "pan-y",
-        St = Mn(),
-        Dn = /mobile|tablet|ip(ad|hone|od)|android/i,
-        $i = "ontouchstart" in me,
-        Fn = Ot(me, "PointerEvent") !== void 0,
-        Nn = $i && Dn.test(navigator.userAgent),
-        at = "touch",
+        Be = "none",
+        ot = "pan-x",
+        nt = "pan-y",
+        St = Dn(),
+        Mn = /mobile|tablet|ip(ad|hone|od)|android/i,
+        $i = "ontouchstart" in pe,
+        Fn = Ot(pe, "PointerEvent") !== void 0,
+        Nn = $i && Mn.test(navigator.userAgent),
+        rt = "touch",
         Bn = "pen",
         si = "mouse",
         An = "kinect",
         zn = 25,
         $ = 1,
-        Le = 2,
+        Ae = 2,
         j = 4,
         J = 8,
         It = 1,
-        dt = 2,
-        ht = 4,
-        lt = 8,
-        Ze = 16,
-        ue = dt | ht,
-        He = lt | Ze,
-        Zi = ue | He,
+        at = 2,
+        dt = 4,
+        ht = 8,
+        $e = 16,
+        ce = at | dt,
+        ze = ht | $e,
+        Zi = ce | ze,
         Qi = ["x", "y"],
         Pt = ["clientX", "clientY"];
 
-    function ye(n, e, t) {
+    function ge(n, e, t) {
         var i;
         if (!!n)
             if (n.forEach) n.forEach(e, t);
             else if (n.length !== void 0)
             for (i = 0; i < n.length;) e.call(t, n[i], i, n), i++;
         else
             for (i in n) n.hasOwnProperty(i) && e.call(t, n[i], i, n)
     }
 
-    function Mt(n, e) {
+    function Dt(n, e) {
         return typeof n === Pn ? n.apply(e && e[0] || void 0, e) : n
     }
 
-    function je(n, e) {
+    function Re(n, e) {
         return n.indexOf(e) > -1
     }
 
     function Rn(n) {
-        if (je(n, Re)) return Re;
-        var e = je(n, nt),
-            t = je(n, rt);
-        return e && t ? Re : e || t ? e ? nt : rt : je(n, ii) ? ii : Ki
+        if (Re(n, Be)) return Be;
+        var e = Re(n, ot),
+            t = Re(n, nt);
+        return e && t ? Be : e || t ? e ? ot : nt : Re(n, ii) ? ii : Ki
     }
     var Ji = function() {
         function n(t, i) {
             this.manager = t, this.set(i)
         }
         var e = n.prototype;
         return e.set = function(i) {
             i === Gi && (i = this.compute()), Xi && this.manager.element.style && St[i] && (this.manager.element.style[Yi] = i), this.actions = i.toLowerCase().trim()
         }, e.update = function() {
             this.set(this.manager.options.touchAction)
         }, e.compute = function() {
             var i = [];
-            return ye(this.manager.recognizers, function(s) {
-                Mt(s.options.enable, [s]) && (i = i.concat(s.getTouchAction()))
+            return ge(this.manager.recognizers, function(s) {
+                Dt(s.options.enable, [s]) && (i = i.concat(s.getTouchAction()))
             }), Rn(i.join(" "))
         }, e.preventDefaults = function(i) {
             var s = i.srcEvent,
                 o = i.offsetDirection;
             if (this.manager.session.prevented) {
                 s.preventDefault();
                 return
             }
             var r = this.actions,
-                a = je(r, Re) && !St[Re],
-                d = je(r, rt) && !St[rt],
-                h = je(r, nt) && !St[nt];
+                a = Re(r, Be) && !St[Be],
+                d = Re(r, nt) && !St[nt],
+                h = Re(r, ot) && !St[ot];
             if (a) {
                 var l = i.pointers.length === 1,
                     c = i.distance < 2,
                     u = i.deltaTime < 250;
                 if (l && c && u) return
             }
-            if (!(h && d) && (a || d && o & ue || h && o & He)) return this.preventSrc(s)
+            if (!(h && d) && (a || d && o & ce || h && o & ze)) return this.preventSrc(s)
         }, e.preventSrc = function(i) {
             this.manager.session.prevented = !0, i.preventDefault()
         }, n
     }();
 
     function oi(n, e) {
         for (; n;) {
@@ -267,54 +267,54 @@
         }
         return !1
     }
 
     function es(n) {
         var e = n.length;
         if (e === 1) return {
-            x: $e(n[0].clientX),
-            y: $e(n[0].clientY)
+            x: Ke(n[0].clientX),
+            y: Ke(n[0].clientY)
         };
         for (var t = 0, i = 0, s = 0; s < e;) t += n[s].clientX, i += n[s].clientY, s++;
         return {
-            x: $e(t / e),
-            y: $e(i / e)
+            x: Ke(t / e),
+            y: Ke(i / e)
         }
     }
 
     function ts(n) {
         for (var e = [], t = 0; t < n.pointers.length;) e[t] = {
-            clientX: $e(n.pointers[t].clientX),
-            clientY: $e(n.pointers[t].clientY)
+            clientX: Ke(n.pointers[t].clientX),
+            clientY: Ke(n.pointers[t].clientY)
         }, t++;
         return {
             timeStamp: ti(),
             pointers: e,
             center: es(e),
             deltaX: n.deltaX,
             deltaY: n.deltaY
         }
     }
 
-    function Dt(n, e, t) {
+    function Mt(n, e, t) {
         t || (t = Qi);
         var i = e[t[0]] - n[t[0]],
             s = e[t[1]] - n[t[1]];
         return Math.sqrt(i * i + s * s)
     }
 
     function ni(n, e, t) {
         t || (t = Qi);
         var i = e[t[0]] - n[t[0]],
             s = e[t[1]] - n[t[1]];
         return Math.atan2(s, i) * 180 / Math.PI
     }
 
     function is(n, e) {
-        return n === e ? It : ze(n) >= ze(e) ? n < 0 ? dt : ht : e < 0 ? lt : Ze
+        return n === e ? It : Ne(n) >= Ne(e) ? n < 0 ? at : dt : e < 0 ? ht : $e
     }
 
     function Ln(n, e) {
         var t = e.center,
             i = n.offsetDelta || {},
             s = n.prevDelta || {},
             o = n.prevInput || {};
@@ -331,223 +331,223 @@
         return {
             x: e / n || 0,
             y: t / n || 0
         }
     }
 
     function Hn(n, e) {
-        return Dt(e[0], e[1], Pt) / Dt(n[0], n[1], Pt)
+        return Mt(e[0], e[1], Pt) / Mt(n[0], n[1], Pt)
     }
 
     function jn(n, e) {
         return ni(e[1], e[0], Pt) + ni(n[1], n[0], Pt)
     }
 
     function Wn(n, e) {
         var t = n.lastInterval || e,
             i = e.timeStamp - t.timeStamp,
             s, o, r, a;
         if (e.eventType !== J && (i > zn || t.velocity === void 0)) {
             var d = e.deltaX - t.deltaX,
                 h = e.deltaY - t.deltaY,
                 l = ss(i, d, h);
-            o = l.x, r = l.y, s = ze(l.x) > ze(l.y) ? l.x : l.y, a = is(d, h), n.lastInterval = e
+            o = l.x, r = l.y, s = Ne(l.x) > Ne(l.y) ? l.x : l.y, a = is(d, h), n.lastInterval = e
         } else s = t.velocity, o = t.velocityX, r = t.velocityY, a = t.direction;
         e.velocity = s, e.velocityX = o, e.velocityY = r, e.direction = a
     }
 
     function Vn(n, e) {
         var t = n.session,
             i = e.pointers,
             s = i.length;
         t.firstInput || (t.firstInput = ts(e)), s > 1 && !t.firstMultiple ? t.firstMultiple = ts(e) : s === 1 && (t.firstMultiple = !1);
         var o = t.firstInput,
             r = t.firstMultiple,
             a = r ? r.center : o.center,
             d = e.center = es(i);
-        e.timeStamp = ti(), e.deltaTime = e.timeStamp - o.timeStamp, e.angle = ni(a, d), e.distance = Dt(a, d), Ln(t, e), e.offsetDirection = is(e.deltaX, e.deltaY);
+        e.timeStamp = ti(), e.deltaTime = e.timeStamp - o.timeStamp, e.angle = ni(a, d), e.distance = Mt(a, d), Ln(t, e), e.offsetDirection = is(e.deltaX, e.deltaY);
         var h = ss(e.deltaTime, e.deltaX, e.deltaY);
-        e.overallVelocityX = h.x, e.overallVelocityY = h.y, e.overallVelocity = ze(h.x) > ze(h.y) ? h.x : h.y, e.scale = r ? Hn(r.pointers, i) : 1, e.rotation = r ? jn(r.pointers, i) : 0, e.maxPointers = t.prevInput ? e.pointers.length > t.prevInput.maxPointers ? e.pointers.length : t.prevInput.maxPointers : e.pointers.length, Wn(t, e);
+        e.overallVelocityX = h.x, e.overallVelocityY = h.y, e.overallVelocity = Ne(h.x) > Ne(h.y) ? h.x : h.y, e.scale = r ? Hn(r.pointers, i) : 1, e.rotation = r ? jn(r.pointers, i) : 0, e.maxPointers = t.prevInput ? e.pointers.length > t.prevInput.maxPointers ? e.pointers.length : t.prevInput.maxPointers : e.pointers.length, Wn(t, e);
         var l = n.element,
             c = e.srcEvent,
             u;
         c.composedPath ? u = c.composedPath()[0] : c.path ? u = c.path[0] : u = c.target, oi(u, l) && (l = u), e.target = l
     }
 
     function qn(n, e, t) {
         var i = t.pointers.length,
             s = t.changedPointers.length,
             o = e & $ && i - s == 0,
             r = e & (j | J) && i - s == 0;
         t.isFirst = !!o, t.isFinal = !!r, o && (n.session = {}), t.eventType = e, Vn(n, t), n.emit("hammer.input", t), n.recognize(t), n.session.prevInput = t
     }
 
-    function ct(n) {
+    function lt(n) {
         return n.trim().split(/\s+/g)
     }
 
-    function ut(n, e, t) {
-        ye(ct(e), function(i) {
+    function ct(n, e, t) {
+        ge(lt(e), function(i) {
             n.addEventListener(i, t, !1)
         })
     }
 
-    function ft(n, e, t) {
-        ye(ct(e), function(i) {
+    function ut(n, e, t) {
+        ge(lt(e), function(i) {
             n.removeEventListener(i, t, !1)
         })
     }
 
     function os(n) {
         var e = n.ownerDocument || n;
         return e.defaultView || e.parentWindow || window
     }
-    var Qe = function() {
+    var Ze = function() {
         function n(t, i) {
             var s = this;
             this.manager = t, this.callback = i, this.element = t.element, this.target = t.options.inputTarget, this.domHandler = function(o) {
-                Mt(t.options.enable, [t]) && s.handler(o)
+                Dt(t.options.enable, [t]) && s.handler(o)
             }, this.init()
         }
         var e = n.prototype;
         return e.handler = function() {}, e.init = function() {
-            this.evEl && ut(this.element, this.evEl, this.domHandler), this.evTarget && ut(this.target, this.evTarget, this.domHandler), this.evWin && ut(os(this.element), this.evWin, this.domHandler)
+            this.evEl && ct(this.element, this.evEl, this.domHandler), this.evTarget && ct(this.target, this.evTarget, this.domHandler), this.evWin && ct(os(this.element), this.evWin, this.domHandler)
         }, e.destroy = function() {
-            this.evEl && ft(this.element, this.evEl, this.domHandler), this.evTarget && ft(this.target, this.evTarget, this.domHandler), this.evWin && ft(os(this.element), this.evWin, this.domHandler)
+            this.evEl && ut(this.element, this.evEl, this.domHandler), this.evTarget && ut(this.target, this.evTarget, this.domHandler), this.evWin && ut(os(this.element), this.evWin, this.domHandler)
         }, n
     }();
 
-    function We(n, e, t) {
+    function Le(n, e, t) {
         if (n.indexOf && !t) return n.indexOf(e);
         for (var i = 0; i < n.length;) {
             if (t && n[i][t] == e || !t && n[i] === e) return i;
             i++
         }
         return -1
     }
     var Un = {
             pointerdown: $,
-            pointermove: Le,
+            pointermove: Ae,
             pointerup: j,
             pointercancel: J,
             pointerout: J
         },
         Yn = {
-            2: at,
+            2: rt,
             3: Bn,
             4: si,
             5: An
         },
         ns = "pointerdown",
         rs = "pointermove pointerup pointercancel";
-    me.MSPointerEvent && !me.PointerEvent && (ns = "MSPointerDown", rs = "MSPointerMove MSPointerUp MSPointerCancel");
+    pe.MSPointerEvent && !pe.PointerEvent && (ns = "MSPointerDown", rs = "MSPointerMove MSPointerUp MSPointerCancel");
     var as = function(n) {
-        ne(e, n);
+        oe(e, n);
 
         function e() {
             var i, s = e.prototype;
             return s.evEl = ns, s.evWin = rs, i = n.apply(this, arguments) || this, i.store = i.manager.session.pointerEvents = [], i
         }
         var t = e.prototype;
         return t.handler = function(s) {
             var o = this.store,
                 r = !1,
                 a = s.type.toLowerCase().replace("ms", ""),
                 d = Un[a],
                 h = Yn[s.pointerType] || s.pointerType,
-                l = h === at,
-                c = We(o, s.pointerId, "pointerId");
+                l = h === rt,
+                c = Le(o, s.pointerId, "pointerId");
             d & $ && (s.button === 0 || l) ? c < 0 && (o.push(s), c = o.length - 1) : d & (j | J) && (r = !0), !(c < 0) && (o[c] = s, this.callback(this.manager, d, {
                 pointers: o,
                 changedPointers: [s],
                 pointerType: h,
                 srcEvent: s
             }), r && o.splice(c, 1))
         }, e
-    }(Qe);
+    }(Ze);
 
-    function pt(n) {
+    function ft(n) {
         return Array.prototype.slice.call(n, 0)
     }
 
     function ri(n, e, t) {
         for (var i = [], s = [], o = 0; o < n.length;) {
             var r = e ? n[o][e] : n[o];
-            We(s, r) < 0 && i.push(n[o]), s[o] = r, o++
+            Le(s, r) < 0 && i.push(n[o]), s[o] = r, o++
         }
         return t && (e ? i = i.sort(function(a, d) {
             return a[e] > d[e]
         }) : i = i.sort()), i
     }
     var Xn = {
             touchstart: $,
-            touchmove: Le,
+            touchmove: Ae,
             touchend: j,
             touchcancel: J
         },
         Gn = "touchstart touchmove touchend touchcancel",
         ai = function(n) {
-            ne(e, n);
+            oe(e, n);
 
             function e() {
                 var i;
                 return e.prototype.evTarget = Gn, i = n.apply(this, arguments) || this, i.targetIds = {}, i
             }
             var t = e.prototype;
             return t.handler = function(s) {
                 var o = Xn[s.type],
                     r = Kn.call(this, s, o);
                 !r || this.callback(this.manager, o, {
                     pointers: r[0],
                     changedPointers: r[1],
-                    pointerType: at,
+                    pointerType: rt,
                     srcEvent: s
                 })
             }, e
-        }(Qe);
+        }(Ze);
 
     function Kn(n, e) {
-        var t = pt(n.touches),
+        var t = ft(n.touches),
             i = this.targetIds;
-        if (e & ($ | Le) && t.length === 1) return i[t[0].identifier] = !0, [t, t];
-        var s, o, r = pt(n.changedTouches),
+        if (e & ($ | Ae) && t.length === 1) return i[t[0].identifier] = !0, [t, t];
+        var s, o, r = ft(n.changedTouches),
             a = [],
             d = this.target;
         if (o = t.filter(function(h) {
                 return oi(h.target, d)
             }), e === $)
             for (s = 0; s < o.length;) i[o[s].identifier] = !0, s++;
         for (s = 0; s < r.length;) i[r[s].identifier] && a.push(r[s]), e & (j | J) && delete i[r[s].identifier], s++;
         if (!!a.length) return [ri(o.concat(a), "identifier", !0), a]
     }
     var $n = {
             mousedown: $,
-            mousemove: Le,
+            mousemove: Ae,
             mouseup: j
         },
         Zn = "mousedown",
         Qn = "mousemove mouseup",
         di = function(n) {
-            ne(e, n);
+            oe(e, n);
 
             function e() {
                 var i, s = e.prototype;
                 return s.evEl = Zn, s.evWin = Qn, i = n.apply(this, arguments) || this, i.pressed = !1, i
             }
             var t = e.prototype;
             return t.handler = function(s) {
                 var o = $n[s.type];
-                o & $ && s.button === 0 && (this.pressed = !0), o & Le && s.which !== 1 && (o = j), !!this.pressed && (o & j && (this.pressed = !1), this.callback(this.manager, o, {
+                o & $ && s.button === 0 && (this.pressed = !0), o & Ae && s.which !== 1 && (o = j), !!this.pressed && (o & j && (this.pressed = !1), this.callback(this.manager, o, {
                     pointers: [s],
                     changedPointers: [s],
                     pointerType: si,
                     srcEvent: s
                 }))
             }, e
-        }(Qe),
+        }(Ze),
         Jn = 2500,
         ds = 25;
 
     function hs(n) {
         var e = n.changedPointers,
             t = e[0];
         if (t.identifier === this.primaryTouch) {
@@ -576,125 +576,125 @@
                 r = Math.abs(t - s.y);
             if (o <= ds && r <= ds) return !0
         }
         return !1
     }
     var ls = function() {
         var n = function(e) {
-            ne(t, e);
+            oe(t, e);
 
             function t(s, o) {
                 var r;
                 return r = e.call(this, s, o) || this, r.handler = function(a, d, h) {
-                    var l = h.pointerType === at,
+                    var l = h.pointerType === rt,
                         c = h.pointerType === si;
                     if (!(c && h.sourceCapabilities && h.sourceCapabilities.firesTouchEvents)) {
                         if (l) er.call(kt(kt(r)), d, h);
                         else if (c && tr.call(kt(kt(r)), h)) return;
                         r.callback(a, d, h)
                     }
                 }, r.touch = new ai(r.manager, r.handler), r.mouse = new di(r.manager, r.handler), r.primaryTouch = null, r.lastTouches = [], r
             }
             var i = t.prototype;
             return i.destroy = function() {
                 this.touch.destroy(), this.mouse.destroy()
             }, t
-        }(Qe);
+        }(Ze);
         return n
     }();
 
     function ir(n) {
         var e, t = n.options.inputClass;
         return t ? e = t : Fn ? e = as : Nn ? e = ai : $i ? e = ls : e = di, new e(n, qn)
     }
 
-    function Je(n, e, t) {
-        return Array.isArray(n) ? (ye(n, t[e], t), !0) : !1
+    function Qe(n, e, t) {
+        return Array.isArray(n) ? (ge(n, t[e], t), !0) : !1
     }
     var Ft = 1,
-        re = 2,
-        et = 4,
-        Se = 8,
-        be = Se,
-        gt = 16,
-        fe = 32,
+        ne = 2,
+        Je = 4,
+        Te = 8,
+        me = Te,
+        pt = 16,
+        ue = 32,
         sr = 1;
 
     function or() {
         return sr++
     }
 
     function Nt(n, e) {
         var t = e.manager;
         return t ? t.get(n) : n
     }
 
     function cs(n) {
-        return n & gt ? "cancel" : n & Se ? "end" : n & et ? "move" : n & re ? "start" : ""
+        return n & pt ? "cancel" : n & Te ? "end" : n & Je ? "move" : n & ne ? "start" : ""
     }
-    var mt = function() {
+    var gt = function() {
             function n(t) {
-                t === void 0 && (t = {}), this.options = ce({
+                t === void 0 && (t = {}), this.options = he({
                     enable: !0
                 }, t), this.id = or(), this.manager = null, this.state = Ft, this.simultaneous = {}, this.requireFail = []
             }
             var e = n.prototype;
             return e.set = function(i) {
-                return Ae(this.options, i), this.manager && this.manager.touchAction.update(), this
+                return Fe(this.options, i), this.manager && this.manager.touchAction.update(), this
             }, e.recognizeWith = function(i) {
-                if (Je(i, "recognizeWith", this)) return this;
+                if (Qe(i, "recognizeWith", this)) return this;
                 var s = this.simultaneous;
                 return i = Nt(i, this), s[i.id] || (s[i.id] = i, i.recognizeWith(this)), this
             }, e.dropRecognizeWith = function(i) {
-                return Je(i, "dropRecognizeWith", this) ? this : (i = Nt(i, this), delete this.simultaneous[i.id], this)
+                return Qe(i, "dropRecognizeWith", this) ? this : (i = Nt(i, this), delete this.simultaneous[i.id], this)
             }, e.requireFailure = function(i) {
-                if (Je(i, "requireFailure", this)) return this;
+                if (Qe(i, "requireFailure", this)) return this;
                 var s = this.requireFail;
-                return i = Nt(i, this), We(s, i) === -1 && (s.push(i), i.requireFailure(this)), this
+                return i = Nt(i, this), Le(s, i) === -1 && (s.push(i), i.requireFailure(this)), this
             }, e.dropRequireFailure = function(i) {
-                if (Je(i, "dropRequireFailure", this)) return this;
+                if (Qe(i, "dropRequireFailure", this)) return this;
                 i = Nt(i, this);
-                var s = We(this.requireFail, i);
+                var s = Le(this.requireFail, i);
                 return s > -1 && this.requireFail.splice(s, 1), this
             }, e.hasRequireFailures = function() {
                 return this.requireFail.length > 0
             }, e.canRecognizeWith = function(i) {
                 return !!this.simultaneous[i.id]
             }, e.emit = function(i) {
                 var s = this,
                     o = this.state;
 
                 function r(a) {
                     s.manager.emit(a, i)
                 }
-                o < Se && r(s.options.event + cs(o)), r(s.options.event), i.additionalEvent && r(i.additionalEvent), o >= Se && r(s.options.event + cs(o))
+                o < Te && r(s.options.event + cs(o)), r(s.options.event), i.additionalEvent && r(i.additionalEvent), o >= Te && r(s.options.event + cs(o))
             }, e.tryEmit = function(i) {
                 if (this.canEmit()) return this.emit(i);
-                this.state = fe
+                this.state = ue
             }, e.canEmit = function() {
                 for (var i = 0; i < this.requireFail.length;) {
-                    if (!(this.requireFail[i].state & (fe | Ft))) return !1;
+                    if (!(this.requireFail[i].state & (ue | Ft))) return !1;
                     i++
                 }
                 return !0
             }, e.recognize = function(i) {
-                var s = Ae({}, i);
-                if (!Mt(this.options.enable, [this, s])) {
-                    this.reset(), this.state = fe;
+                var s = Fe({}, i);
+                if (!Dt(this.options.enable, [this, s])) {
+                    this.reset(), this.state = ue;
                     return
                 }
-                this.state & (be | gt | fe) && (this.state = Ft), this.state = this.process(s), this.state & (re | et | Se | gt) && this.tryEmit(s)
+                this.state & (me | pt | ue) && (this.state = Ft), this.state = this.process(s), this.state & (ne | Je | Te | pt) && this.tryEmit(s)
             }, e.process = function(i) {}, e.getTouchAction = function() {}, e.reset = function() {}, n
         }(),
         hi = function(n) {
-            ne(e, n);
+            oe(e, n);
 
             function e(i) {
                 var s;
-                return i === void 0 && (i = {}), s = n.call(this, ce({
+                return i === void 0 && (i = {}), s = n.call(this, he({
                     event: "tap",
                     pointers: 1,
                     taps: 1,
                     interval: 300,
                     time: 250,
                     threshold: 9,
                     posThreshold: 10
@@ -709,160 +709,160 @@
                     a = s.pointers.length === r.pointers,
                     d = s.distance < r.threshold,
                     h = s.deltaTime < r.time;
                 if (this.reset(), s.eventType & $ && this.count === 0) return this.failTimeout();
                 if (d && h && a) {
                     if (s.eventType !== j) return this.failTimeout();
                     var l = this.pTime ? s.timeStamp - this.pTime < r.interval : !0,
-                        c = !this.pCenter || Dt(this.pCenter, s.center) < r.posThreshold;
+                        c = !this.pCenter || Mt(this.pCenter, s.center) < r.posThreshold;
                     this.pTime = s.timeStamp, this.pCenter = s.center, !c || !l ? this.count = 1 : this.count += 1, this._input = s;
                     var u = this.count % r.taps;
                     if (u === 0) return this.hasRequireFailures() ? (this._timer = setTimeout(function() {
-                        o.state = be, o.tryEmit()
-                    }, r.interval), re) : be
+                        o.state = me, o.tryEmit()
+                    }, r.interval), ne) : me
                 }
-                return fe
+                return ue
             }, t.failTimeout = function() {
                 var s = this;
                 return this._timer = setTimeout(function() {
-                    s.state = fe
-                }, this.options.interval), fe
+                    s.state = ue
+                }, this.options.interval), ue
             }, t.reset = function() {
                 clearTimeout(this._timer)
             }, t.emit = function() {
-                this.state === be && (this._input.tapCount = this.count, this.manager.emit(this.options.event, this._input))
+                this.state === me && (this._input.tapCount = this.count, this.manager.emit(this.options.event, this._input))
             }, e
-        }(mt),
-        tt = function(n) {
-            ne(e, n);
+        }(gt),
+        et = function(n) {
+            oe(e, n);
 
             function e(i) {
-                return i === void 0 && (i = {}), n.call(this, ce({
+                return i === void 0 && (i = {}), n.call(this, he({
                     pointers: 1
                 }, i)) || this
             }
             var t = e.prototype;
             return t.attrTest = function(s) {
                 var o = this.options.pointers;
                 return o === 0 || s.pointers.length === o
             }, t.process = function(s) {
                 var o = this.state,
                     r = s.eventType,
-                    a = o & (re | et),
+                    a = o & (ne | Je),
                     d = this.attrTest(s);
-                return a && (r & J || !d) ? o | gt : a || d ? r & j ? o | Se : o & re ? o | et : re : fe
+                return a && (r & J || !d) ? o | pt : a || d ? r & j ? o | Te : o & ne ? o | Je : ne : ue
             }, e
-        }(mt);
+        }(gt);
 
     function us(n) {
-        return n === Ze ? "down" : n === lt ? "up" : n === dt ? "left" : n === ht ? "right" : ""
+        return n === $e ? "down" : n === ht ? "up" : n === at ? "left" : n === dt ? "right" : ""
     }
     var li = function(n) {
-            ne(e, n);
+            oe(e, n);
 
             function e(i) {
                 var s;
-                return i === void 0 && (i = {}), s = n.call(this, ce({
+                return i === void 0 && (i = {}), s = n.call(this, he({
                     event: "pan",
                     threshold: 10,
                     pointers: 1,
                     direction: Zi
                 }, i)) || this, s.pX = null, s.pY = null, s
             }
             var t = e.prototype;
             return t.getTouchAction = function() {
                 var s = this.options.direction,
                     o = [];
-                return s & ue && o.push(rt), s & He && o.push(nt), o
+                return s & ce && o.push(nt), s & ze && o.push(ot), o
             }, t.directionTest = function(s) {
                 var o = this.options,
                     r = !0,
                     a = s.distance,
                     d = s.direction,
                     h = s.deltaX,
                     l = s.deltaY;
-                return d & o.direction || (o.direction & ue ? (d = h === 0 ? It : h < 0 ? dt : ht, r = h !== this.pX, a = Math.abs(s.deltaX)) : (d = l === 0 ? It : l < 0 ? lt : Ze, r = l !== this.pY, a = Math.abs(s.deltaY))), s.direction = d, r && a > o.threshold && d & o.direction
+                return d & o.direction || (o.direction & ce ? (d = h === 0 ? It : h < 0 ? at : dt, r = h !== this.pX, a = Math.abs(s.deltaX)) : (d = l === 0 ? It : l < 0 ? ht : $e, r = l !== this.pY, a = Math.abs(s.deltaY))), s.direction = d, r && a > o.threshold && d & o.direction
             }, t.attrTest = function(s) {
-                return tt.prototype.attrTest.call(this, s) && (this.state & re || !(this.state & re) && this.directionTest(s))
+                return et.prototype.attrTest.call(this, s) && (this.state & ne || !(this.state & ne) && this.directionTest(s))
             }, t.emit = function(s) {
                 this.pX = s.deltaX, this.pY = s.deltaY;
                 var o = us(s.direction);
                 o && (s.additionalEvent = this.options.event + o), n.prototype.emit.call(this, s)
             }, e
-        }(tt),
+        }(et),
         fs = function(n) {
-            ne(e, n);
+            oe(e, n);
 
             function e(i) {
-                return i === void 0 && (i = {}), n.call(this, ce({
+                return i === void 0 && (i = {}), n.call(this, he({
                     event: "swipe",
                     threshold: 10,
                     velocity: .3,
-                    direction: ue | He,
+                    direction: ce | ze,
                     pointers: 1
                 }, i)) || this
             }
             var t = e.prototype;
             return t.getTouchAction = function() {
                 return li.prototype.getTouchAction.call(this)
             }, t.attrTest = function(s) {
                 var o = this.options.direction,
                     r;
-                return o & (ue | He) ? r = s.overallVelocity : o & ue ? r = s.overallVelocityX : o & He && (r = s.overallVelocityY), n.prototype.attrTest.call(this, s) && o & s.offsetDirection && s.distance > this.options.threshold && s.maxPointers === this.options.pointers && ze(r) > this.options.velocity && s.eventType & j
+                return o & (ce | ze) ? r = s.overallVelocity : o & ce ? r = s.overallVelocityX : o & ze && (r = s.overallVelocityY), n.prototype.attrTest.call(this, s) && o & s.offsetDirection && s.distance > this.options.threshold && s.maxPointers === this.options.pointers && Ne(r) > this.options.velocity && s.eventType & j
             }, t.emit = function(s) {
                 var o = us(s.offsetDirection);
                 o && this.manager.emit(this.options.event + o, s), this.manager.emit(this.options.event, s)
             }, e
-        }(tt),
+        }(et),
         ps = function(n) {
-            ne(e, n);
+            oe(e, n);
 
             function e(i) {
-                return i === void 0 && (i = {}), n.call(this, ce({
+                return i === void 0 && (i = {}), n.call(this, he({
                     event: "pinch",
                     threshold: 0,
                     pointers: 2
                 }, i)) || this
             }
             var t = e.prototype;
             return t.getTouchAction = function() {
-                return [Re]
+                return [Be]
             }, t.attrTest = function(s) {
-                return n.prototype.attrTest.call(this, s) && (Math.abs(s.scale - 1) > this.options.threshold || this.state & re)
+                return n.prototype.attrTest.call(this, s) && (Math.abs(s.scale - 1) > this.options.threshold || this.state & ne)
             }, t.emit = function(s) {
                 if (s.scale !== 1) {
                     var o = s.scale < 1 ? "in" : "out";
                     s.additionalEvent = this.options.event + o
                 }
                 n.prototype.emit.call(this, s)
             }, e
-        }(tt),
+        }(et),
         gs = function(n) {
-            ne(e, n);
+            oe(e, n);
 
             function e(i) {
-                return i === void 0 && (i = {}), n.call(this, ce({
+                return i === void 0 && (i = {}), n.call(this, he({
                     event: "rotate",
                     threshold: 0,
                     pointers: 2
                 }, i)) || this
             }
             var t = e.prototype;
             return t.getTouchAction = function() {
-                return [Re]
+                return [Be]
             }, t.attrTest = function(s) {
-                return n.prototype.attrTest.call(this, s) && (Math.abs(s.rotation) > this.options.threshold || this.state & re)
+                return n.prototype.attrTest.call(this, s) && (Math.abs(s.rotation) > this.options.threshold || this.state & ne)
             }, e
-        }(tt),
+        }(et),
         ms = function(n) {
-            ne(e, n);
+            oe(e, n);
 
             function e(i) {
                 var s;
-                return i === void 0 && (i = {}), s = n.call(this, ce({
+                return i === void 0 && (i = {}), s = n.call(this, he({
                     event: "press",
                     pointers: 1,
                     time: 251,
                     threshold: 9
                 }, i)) || this, s._timer = null, s._input = null, s
             }
             var t = e.prototype;
@@ -872,24 +872,24 @@
                 var o = this,
                     r = this.options,
                     a = s.pointers.length === r.pointers,
                     d = s.distance < r.threshold,
                     h = s.deltaTime > r.time;
                 if (this._input = s, !d || !a || s.eventType & (j | J) && !h) this.reset();
                 else if (s.eventType & $) this.reset(), this._timer = setTimeout(function() {
-                    o.state = be, o.tryEmit()
+                    o.state = me, o.tryEmit()
                 }, r.time);
-                else if (s.eventType & j) return be;
-                return fe
+                else if (s.eventType & j) return me;
+                return ue
             }, t.reset = function() {
                 clearTimeout(this._timer)
             }, t.emit = function(s) {
-                this.state === be && (s && s.eventType & j ? this.manager.emit(this.options.event + "up", s) : (this._input.timeStamp = ti(), this.manager.emit(this.options.event, this._input)))
+                this.state === me && (s && s.eventType & j ? this.manager.emit(this.options.event + "up", s) : (this._input.timeStamp = ti(), this.manager.emit(this.options.event, this._input)))
             }, e
-        }(mt),
+        }(gt),
         ys = {
             domEvents: !1,
             touchAction: Gi,
             enable: !0,
             inputTarget: null,
             inputClass: null,
             cssProps: {
@@ -907,18 +907,18 @@
             }],
             [ps, {
                     enable: !1
                 },
                 ["rotate"]
             ],
             [fs, {
-                direction: ue
+                direction: ce
             }],
             [li, {
-                    direction: ue
+                    direction: ce
                 },
                 ["swipe"]
             ],
             [hi],
             [hi, {
                     event: "doubletap",
                     taps: 2
@@ -930,75 +930,75 @@
         nr = 1,
         vs = 2;
 
     function ws(n, e) {
         var t = n.element;
         if (!!t.style) {
             var i;
-            ye(n.options.cssProps, function(s, o) {
+            ge(n.options.cssProps, function(s, o) {
                 i = Ot(t.style, o), e ? (n.oldCssProps[i] = t.style[i], t.style[i] = s) : t.style[i] = n.oldCssProps[i] || ""
             }), e || (n.oldCssProps = {})
         }
     }
 
     function rr(n, e) {
         var t = document.createEvent("Event");
         t.initEvent(n, !0, !0), t.gesture = e, e.target.dispatchEvent(t)
     }
     var _s = function() {
             function n(t, i) {
                 var s = this;
-                this.options = Ae({}, ys, i || {}), this.options.inputTarget = this.options.inputTarget || t, this.handlers = {}, this.session = {}, this.recognizers = [], this.oldCssProps = {}, this.element = t, this.input = ir(this), this.touchAction = new Ji(this, this.options.touchAction), ws(this, !0), ye(this.options.recognizers, function(o) {
+                this.options = Fe({}, ys, i || {}), this.options.inputTarget = this.options.inputTarget || t, this.handlers = {}, this.session = {}, this.recognizers = [], this.oldCssProps = {}, this.element = t, this.input = ir(this), this.touchAction = new Ji(this, this.options.touchAction), ws(this, !0), ge(this.options.recognizers, function(o) {
                     var r = s.add(new o[0](o[1]));
                     o[2] && r.recognizeWith(o[2]), o[3] && r.requireFailure(o[3])
                 }, this)
             }
             var e = n.prototype;
             return e.set = function(i) {
-                return Ae(this.options, i), i.touchAction && this.touchAction.update(), i.inputTarget && (this.input.destroy(), this.input.target = i.inputTarget, this.input.init()), this
+                return Fe(this.options, i), i.touchAction && this.touchAction.update(), i.inputTarget && (this.input.destroy(), this.input.target = i.inputTarget, this.input.init()), this
             }, e.stop = function(i) {
                 this.session.stopped = i ? vs : nr
             }, e.recognize = function(i) {
                 var s = this.session;
                 if (!s.stopped) {
                     this.touchAction.preventDefaults(i);
                     var o, r = this.recognizers,
                         a = s.curRecognizer;
-                    (!a || a && a.state & be) && (s.curRecognizer = null, a = null);
-                    for (var d = 0; d < r.length;) o = r[d], s.stopped !== vs && (!a || o === a || o.canRecognizeWith(a)) ? o.recognize(i) : o.reset(), !a && o.state & (re | et | Se) && (s.curRecognizer = o, a = o), d++
+                    (!a || a && a.state & me) && (s.curRecognizer = null, a = null);
+                    for (var d = 0; d < r.length;) o = r[d], s.stopped !== vs && (!a || o === a || o.canRecognizeWith(a)) ? o.recognize(i) : o.reset(), !a && o.state & (ne | Je | Te) && (s.curRecognizer = o, a = o), d++
                 }
             }, e.get = function(i) {
-                if (i instanceof mt) return i;
+                if (i instanceof gt) return i;
                 for (var s = this.recognizers, o = 0; o < s.length; o++)
                     if (s[o].options.event === i) return s[o];
                 return null
             }, e.add = function(i) {
-                if (Je(i, "add", this)) return this;
+                if (Qe(i, "add", this)) return this;
                 var s = this.get(i.options.event);
                 return s && this.remove(s), this.recognizers.push(i), i.manager = this, this.touchAction.update(), i
             }, e.remove = function(i) {
-                if (Je(i, "remove", this)) return this;
+                if (Qe(i, "remove", this)) return this;
                 var s = this.get(i);
                 if (i) {
                     var o = this.recognizers,
-                        r = We(o, s);
+                        r = Le(o, s);
                     r !== -1 && (o.splice(r, 1), this.touchAction.update())
                 }
                 return this
             }, e.on = function(i, s) {
                 if (i === void 0 || s === void 0) return this;
                 var o = this.handlers;
-                return ye(ct(i), function(r) {
+                return ge(lt(i), function(r) {
                     o[r] = o[r] || [], o[r].push(s)
                 }), this
             }, e.off = function(i, s) {
                 if (i === void 0) return this;
                 var o = this.handlers;
-                return ye(ct(i), function(r) {
-                    s ? o[r] && o[r].splice(We(o[r], s), 1) : delete o[r]
+                return ge(lt(i), function(r) {
+                    s ? o[r] && o[r].splice(Le(o[r], s), 1) : delete o[r]
                 }), this
             }, e.emit = function(i, s) {
                 this.options.domEvents && rr(i, s);
                 var o = this.handlers[i] && this.handlers[i].slice();
                 if (!(!o || !o.length)) {
                     s.type = i, s.preventDefault = function() {
                         s.srcEvent.preventDefault()
@@ -1007,45 +1007,45 @@
                 }
             }, e.destroy = function() {
                 this.element && ws(this, !1), this.handlers = {}, this.session = {}, this.input.destroy(), this.element = null
             }, n
         }(),
         ar = {
             touchstart: $,
-            touchmove: Le,
+            touchmove: Ae,
             touchend: j,
             touchcancel: J
         },
         dr = "touchstart",
         hr = "touchstart touchmove touchend touchcancel",
         lr = function(n) {
-            ne(e, n);
+            oe(e, n);
 
             function e() {
                 var i, s = e.prototype;
                 return s.evTarget = dr, s.evWin = hr, i = n.apply(this, arguments) || this, i.started = !1, i
             }
             var t = e.prototype;
             return t.handler = function(s) {
                 var o = ar[s.type];
                 if (o === $ && (this.started = !0), !!this.started) {
                     var r = cr.call(this, s, o);
                     o & (j | J) && r[0].length - r[1].length == 0 && (this.started = !1), this.callback(this.manager, o, {
                         pointers: r[0],
                         changedPointers: r[1],
-                        pointerType: at,
+                        pointerType: rt,
                         srcEvent: s
                     })
                 }
             }, e
-        }(Qe);
+        }(Ze);
 
     function cr(n, e) {
-        var t = pt(n.touches),
-            i = pt(n.changedTouches);
+        var t = ft(n.touches),
+            i = ft(n.changedTouches);
         return e & (j | J) && (t = ri(t.concat(i), "identifier", !0)), [t, i]
     }
 
     function Es(n, e, t) {
         var i = "DEPRECATED METHOD: " + e + `
 ` + t + ` AT 
 `;
@@ -1063,43 +1063,43 @@
         ur = Es(function(n, e) {
             return xs(n, e, !0)
         }, "merge", "Use `assign`.");
 
     function fr(n, e, t) {
         var i = e.prototype,
             s;
-        s = n.prototype = Object.create(i), s.constructor = n, s._super = i, t && Ae(s, t)
+        s = n.prototype = Object.create(i), s.constructor = n, s._super = i, t && Fe(s, t)
     }
 
     function Cs(n, e) {
         return function() {
             return n.apply(e, arguments)
         }
     }
     var Ts = function() {
             var n = function(t, i) {
-                return i === void 0 && (i = {}), new _s(t, ce({
+                return i === void 0 && (i = {}), new _s(t, he({
                     recognizers: bs.concat()
                 }, i))
             };
-            return n.VERSION = "2.0.17-rc", n.DIRECTION_ALL = Zi, n.DIRECTION_DOWN = Ze, n.DIRECTION_LEFT = dt, n.DIRECTION_RIGHT = ht, n.DIRECTION_UP = lt, n.DIRECTION_HORIZONTAL = ue, n.DIRECTION_VERTICAL = He, n.DIRECTION_NONE = It, n.DIRECTION_DOWN = Ze, n.INPUT_START = $, n.INPUT_MOVE = Le, n.INPUT_END = j, n.INPUT_CANCEL = J, n.STATE_POSSIBLE = Ft, n.STATE_BEGAN = re, n.STATE_CHANGED = et, n.STATE_ENDED = Se, n.STATE_RECOGNIZED = be, n.STATE_CANCELLED = gt, n.STATE_FAILED = fe, n.Manager = _s, n.Input = Qe, n.TouchAction = Ji, n.TouchInput = ai, n.MouseInput = di, n.PointerEventInput = as, n.TouchMouseInput = ls, n.SingleTouchInput = lr, n.Recognizer = mt, n.AttrRecognizer = tt, n.Tap = hi, n.Pan = li, n.Swipe = fs, n.Pinch = ps, n.Rotate = gs, n.Press = ms, n.on = ut, n.off = ft, n.each = ye, n.merge = ur, n.extend = xs, n.bindFn = Cs, n.assign = Ae, n.inherit = fr, n.bindFn = Cs, n.prefixed = Ot, n.toArray = pt, n.inArray = We, n.uniqueArray = ri, n.splitStr = ct, n.boolOrFn = Mt, n.hasParent = oi, n.addEventListeners = ut, n.removeEventListeners = ft, n.defaults = Ae({}, ys, {
+            return n.VERSION = "2.0.17-rc", n.DIRECTION_ALL = Zi, n.DIRECTION_DOWN = $e, n.DIRECTION_LEFT = at, n.DIRECTION_RIGHT = dt, n.DIRECTION_UP = ht, n.DIRECTION_HORIZONTAL = ce, n.DIRECTION_VERTICAL = ze, n.DIRECTION_NONE = It, n.DIRECTION_DOWN = $e, n.INPUT_START = $, n.INPUT_MOVE = Ae, n.INPUT_END = j, n.INPUT_CANCEL = J, n.STATE_POSSIBLE = Ft, n.STATE_BEGAN = ne, n.STATE_CHANGED = Je, n.STATE_ENDED = Te, n.STATE_RECOGNIZED = me, n.STATE_CANCELLED = pt, n.STATE_FAILED = ue, n.Manager = _s, n.Input = Ze, n.TouchAction = Ji, n.TouchInput = ai, n.MouseInput = di, n.PointerEventInput = as, n.TouchMouseInput = ls, n.SingleTouchInput = lr, n.Recognizer = gt, n.AttrRecognizer = et, n.Tap = hi, n.Pan = li, n.Swipe = fs, n.Pinch = ps, n.Rotate = gs, n.Press = ms, n.on = ct, n.off = ut, n.each = ge, n.merge = ur, n.extend = xs, n.bindFn = Cs, n.assign = Fe, n.inherit = fr, n.bindFn = Cs, n.prefixed = Ot, n.toArray = ft, n.inArray = Le, n.uniqueArray = ri, n.splitStr = lt, n.boolOrFn = Dt, n.hasParent = oi, n.addEventListeners = ct, n.removeEventListeners = ut, n.defaults = Fe({}, ys, {
                 preset: bs
             }), n
         }(),
         Ra = Ts.defaults,
         ks = Ts;
     var ci = Symbol("DELETE");
 
     function Ss(n, ...e) {
         return Is({}, n, ...e)
     }
 
     function Is(...n) {
         let e = Bt(...n);
-        return Ms(e), e
+        return Ds(e), e
     }
 
     function Bt(...n) {
         if (n.length < 2) return n[0];
         if (n.length > 2) return Bt(Is(n[0], n[1]), ...n.slice(2));
         let e = n[0],
             t = n[1];
@@ -1108,19 +1108,19 @@
         return e
     }
 
     function Ps(n) {
         return Array.isArray(n) ? n.map(e => Ps(e)) : typeof n == "object" && n !== null ? n instanceof Date ? new Date(n.getTime()) : Bt({}, n) : n
     }
 
-    function Ms(n) {
-        for (let e of Object.keys(n)) n[e] === ci ? delete n[e] : typeof n[e] == "object" && n[e] !== null && Ms(n[e])
+    function Ds(n) {
+        for (let e of Object.keys(n)) n[e] === ci ? delete n[e] : typeof n[e] == "object" && n[e] !== null && Ds(n[e])
     }
 
-    function yt(...n) {
+    function mt(...n) {
         return pr(n.length ? n : [Date.now()])
     }
 
     function pr(n) {
         let [e, t, i] = gr(n), s = 1, o = () => {
             let r = 2091639 * e + s * 23283064365386963e-26;
             return e = t, t = i, i = r - (s = r | 0)
@@ -1164,15 +1164,15 @@
             }
         }
     }
     var ui = typeof window != "undefined" ? window.Hammer || ks : function() {
         return yr()
     };
 
-    function pe(n) {
+    function fe(n) {
         this._cleanupQueue = [], this.active = !1, this._dom = {
             container: n,
             overlay: document.createElement("div")
         }, this._dom.overlay.classList.add("vis-overlay"), this._dom.container.appendChild(this._dom.overlay), this._cleanupQueue.push(() => {
             this._dom.overlay.parentNode.removeChild(this._dom.overlay)
         });
         let e = ui(this._dom.overlay);
@@ -1185,27 +1185,27 @@
         }), document && document.body && (this._onClick = i => {
             br(i.target, n) || this.deactivate()
         }, document.body.addEventListener("click", this._onClick), this._cleanupQueue.push(() => {
             document.body.removeEventListener("click", this._onClick)
         })), this._escListener = i => {
             ("key" in i ? i.key === "Escape" : i.keyCode === 27) && this.deactivate()
         }
-    }(0, Os.default)(pe.prototype);
-    pe.current = null;
-    pe.prototype.destroy = function() {
+    }(0, Os.default)(fe.prototype);
+    fe.current = null;
+    fe.prototype.destroy = function() {
         this.deactivate();
         for (let n of this._cleanupQueue.splice(0).reverse()) n()
     };
-    pe.prototype.activate = function() {
-        pe.current && pe.current.deactivate(), pe.current = this, this.active = !0, this._dom.overlay.style.display = "none", this._dom.container.classList.add("vis-active"), this.emit("change"), this.emit("activate"), document.body.addEventListener("keydown", this._escListener)
+    fe.prototype.activate = function() {
+        fe.current && fe.current.deactivate(), fe.current = this, this.active = !0, this._dom.overlay.style.display = "none", this._dom.container.classList.add("vis-active"), this.emit("change"), this.emit("activate"), document.body.addEventListener("keydown", this._escListener)
     };
-    pe.prototype.deactivate = function() {
+    fe.prototype.deactivate = function() {
         this.active = !1, this._dom.overlay.style.display = "block", this._dom.container.classList.remove("vis-active"), document.body.removeEventListener("keydown", this._escListener), this.emit("change"), this.emit("deactivate")
     };
-    pe.prototype._onTapOverlay = function(n) {
+    fe.prototype._onTapOverlay = function(n) {
         this.activate(), n.srcEvent.stopPropagation()
     };
 
     function br(n, e) {
         for (; n;) {
             if (n === e) return !0;
             n = n.parentNode
@@ -1213,74 +1213,74 @@
         return !1
     }
     var vr = /^#?([a-f\d]{2})([a-f\d]{2})([a-f\d]{2})$/i,
         wr = /^#?([a-f\d])([a-f\d])([a-f\d])$/i,
         _r = /^rgb\( *(1?\d{1,2}|2[0-4]\d|25[0-5]) *, *(1?\d{1,2}|2[0-4]\d|25[0-5]) *, *(1?\d{1,2}|2[0-4]\d|25[0-5]) *\)$/i,
         Er = /^rgba\( *(1?\d{1,2}|2[0-4]\d|25[0-5]) *, *(1?\d{1,2}|2[0-4]\d|25[0-5]) *, *(1?\d{1,2}|2[0-4]\d|25[0-5]) *, *([01]|0?\.\d+) *\)$/i;
 
-    function ve(n) {
+    function ye(n) {
         if (n)
             for (; n.hasChildNodes() === !0;) {
                 let e = n.firstChild;
-                e && (ve(e), n.removeChild(e))
+                e && (ye(e), n.removeChild(e))
             }
     }
 
-    function we(n) {
+    function be(n) {
         return n instanceof String || typeof n == "string"
     }
 
-    function Ds(n) {
+    function Ms(n) {
         return typeof n == "object" && n !== null
     }
 
-    function Ve(n, e, t, i) {
+    function He(n, e, t, i) {
         let s = !1;
         i === !0 && (s = e[t] === null && n[t] !== void 0), s ? delete n[t] : n[t] = e[t]
     }
 
     function fi(n, e, t = !1) {
         for (let i in n)
             if (e[i] !== void 0)
-                if (e[i] === null || typeof e[i] != "object") Ve(n, e, i, t);
+                if (e[i] === null || typeof e[i] != "object") He(n, e, i, t);
                 else {
                     let s = n[i],
                         o = e[i];
-                    Ds(s) && Ds(o) && fi(s, o, t)
+                    Ms(s) && Ms(o) && fi(s, o, t)
                 }
     }
 
-    function qe(n, e, t, i = !1) {
+    function je(n, e, t, i = !1) {
         if (Array.isArray(t)) throw new TypeError("Arrays are not supported by deepExtend");
         for (let s = 0; s < n.length; s++) {
             let o = n[s];
             if (Object.prototype.hasOwnProperty.call(t, o))
-                if (t[o] && t[o].constructor === Object) e[o] === void 0 && (e[o] = {}), e[o].constructor === Object ? D(e[o], t[o], !1, i) : Ve(e, t, o, i);
+                if (t[o] && t[o].constructor === Object) e[o] === void 0 && (e[o] = {}), e[o].constructor === Object ? D(e[o], t[o], !1, i) : He(e, t, o, i);
                 else {
                     if (Array.isArray(t[o])) throw new TypeError("Arrays are not supported by deepExtend");
-                    Ve(e, t, o, i)
+                    He(e, t, o, i)
                 }
         }
         return e
     }
 
-    function bt(n, e, t, i = !1) {
+    function yt(n, e, t, i = !1) {
         if (Array.isArray(t)) throw new TypeError("Arrays are not supported by deepExtend");
         for (let s in t)
             if (!!Object.prototype.hasOwnProperty.call(t, s) && !n.includes(s))
-                if (t[s] && t[s].constructor === Object) e[s] === void 0 && (e[s] = {}), e[s].constructor === Object ? D(e[s], t[s]) : Ve(e, t, s, i);
+                if (t[s] && t[s].constructor === Object) e[s] === void 0 && (e[s] = {}), e[s].constructor === Object ? D(e[s], t[s]) : He(e, t, s, i);
                 else if (Array.isArray(t[s])) {
             e[s] = [];
             for (let o = 0; o < t[s].length; o++) e[s].push(t[s][o])
-        } else Ve(e, t, s, i);
+        } else He(e, t, s, i);
         return e
     }
 
     function D(n, e, t = !1, i = !1) {
-        for (let s in e)(Object.prototype.hasOwnProperty.call(e, s) || t === !0) && (typeof e[s] == "object" && e[s] !== null && Object.getPrototypeOf(e[s]) === Object.prototype ? n[s] === void 0 ? n[s] = D({}, e[s], t) : typeof n[s] == "object" && n[s] !== null && Object.getPrototypeOf(n[s]) === Object.prototype ? D(n[s], e[s], t) : Ve(n, e, s, i) : Array.isArray(e[s]) ? n[s] = e[s].slice() : Ve(n, e, s, i));
+        for (let s in e)(Object.prototype.hasOwnProperty.call(e, s) || t === !0) && (typeof e[s] == "object" && e[s] !== null && Object.getPrototypeOf(e[s]) === Object.prototype ? n[s] === void 0 ? n[s] = D({}, e[s], t) : typeof n[s] == "object" && n[s] !== null && Object.getPrototypeOf(n[s]) === Object.prototype ? D(n[s], e[s], t) : He(n, e, s, i) : Array.isArray(e[s]) ? n[s] = e[s].slice() : He(n, e, s, i));
         return n
     }
 
     function At(n, e) {
         return [...n, e]
     }
 
@@ -1338,15 +1338,15 @@
     }
 
     function Bs(n, e, t) {
         return "#" + ((1 << 24) + (n << 16) + (e << 8) + t).toString(16).slice(1)
     }
 
     function zt(n, e) {
-        if (we(n)) {
+        if (be(n)) {
             let t = n;
             if (zs(t)) {
                 let i = t.substr(4).substr(0, t.length - 5).split(",").map(function(s) {
                     return parseInt(s)
                 });
                 t = Bs(i[0], i[1], i[2])
             }
@@ -1387,49 +1387,49 @@
                     background: t,
                     border: t
                 }
             }
         } else return e ? {
             background: n.background || e.background,
             border: n.border || e.border,
-            highlight: we(n.highlight) ? {
+            highlight: be(n.highlight) ? {
                 border: n.highlight,
                 background: n.highlight
             } : {
                 background: n.highlight && n.highlight.background || e.highlight.background,
                 border: n.highlight && n.highlight.border || e.highlight.border
             },
-            hover: we(n.hover) ? {
+            hover: be(n.hover) ? {
                 border: n.hover,
                 background: n.hover
             } : {
                 border: n.hover && n.hover.border || e.hover.border,
                 background: n.hover && n.hover.background || e.hover.background
             }
         } : {
             background: n.background || void 0,
             border: n.border || void 0,
-            highlight: we(n.highlight) ? {
+            highlight: be(n.highlight) ? {
                 border: n.highlight,
                 background: n.highlight
             } : {
                 background: n.highlight && n.highlight.background || void 0,
                 border: n.highlight && n.highlight.border || void 0
             },
-            hover: we(n.hover) ? {
+            hover: be(n.hover) ? {
                 border: n.hover,
                 background: n.hover
             } : {
                 border: n.hover && n.hover.border || void 0,
                 background: n.hover && n.hover.background || void 0
             }
         }
     }
 
-    function vt(n, e, t) {
+    function bt(n, e, t) {
         n = n / 255, e = e / 255, t = t / 255;
         let i = Math.min(n, Math.min(e, t)),
             s = Math.max(n, Math.max(e, t));
         if (i === s) return {
             h: 0,
             s: 0,
             v: i
@@ -1481,58 +1481,58 @@
         let i = Rt(n, e, t);
         return Bs(i.r, i.g, i.b)
     }
 
     function Cr(n) {
         let e = pi(n);
         if (!e) throw new TypeError(`'${n}' is not a valid color.`);
-        return vt(e.r, e.g, e.b)
+        return bt(e.r, e.g, e.b)
     }
 
     function As(n) {
         return /(^#[0-9A-F]{6}$)|(^#[0-9A-F]{3}$)/i.test(n)
     }
 
     function zs(n) {
         return _r.test(n)
     }
 
     function Tr(n) {
         return Er.test(n)
     }
 
-    function _e(n) {
+    function ve(n) {
         if (n === null || typeof n != "object") return null;
         if (n instanceof Element) return n;
         let e = Object.create(n);
-        for (let t in n) Object.prototype.hasOwnProperty.call(n, t) && typeof n[t] == "object" && (e[t] = _e(n[t]));
+        for (let t in n) Object.prototype.hasOwnProperty.call(n, t) && typeof n[t] == "object" && (e[t] = ve(n[t]));
         return e
     }
 
     function se(n, e, t, i = {}) {
         let s = function(f) {
                 return f != null
             },
             o = function(f) {
                 return f !== null && typeof f == "object"
             },
             r = function(f) {
-                for (let y in f)
-                    if (Object.prototype.hasOwnProperty.call(f, y)) return !1;
+                for (let m in f)
+                    if (Object.prototype.hasOwnProperty.call(f, m)) return !1;
                 return !0
             };
         if (!o(n)) throw new Error("Parameter mergeTarget must be an object");
         if (!o(e)) throw new Error("Parameter options must be an object");
         if (!s(t)) throw new Error("Parameter option must have a value");
         if (!o(i)) throw new Error("Parameter globalOptions must be an object");
-        let a = function(f, y, v) {
-                o(f[v]) || (f[v] = {});
-                let g = y[v],
-                    p = f[v];
-                for (let b in g) Object.prototype.hasOwnProperty.call(g, b) && (p[b] = g[b])
+        let a = function(f, m, b) {
+                o(f[b]) || (f[b] = {});
+                let p = m[b],
+                    y = f[b];
+                for (let _ in p) Object.prototype.hasOwnProperty.call(p, _) && (y[_] = p[_])
             },
             d = e[t],
             l = o(i) && !r(i) ? i[t] : void 0,
             c = l ? l.enabled : void 0;
         if (d === void 0) return;
         if (typeof d == "boolean") {
             o(n[t]) || (n[t] = {}), n[t].enabled = d;
@@ -1583,15 +1583,15 @@
             return 1 + --n * n * n * n * n
         },
         easeInOutQuint(n) {
             return n < .5 ? 16 * n * n * n * n * n : 1 + 16 * --n * n * n * n * n
         }
     };
 
-    function Ee(n, e) {
+    function we(n, e) {
         let t;
         Array.isArray(e) || (e = [e]);
         for (let i of n)
             if (i) {
                 t = i[e[0]];
                 for (let s = 1; s < e.length; s++) t && (t = t[e[s]]);
                 if (typeof t != "undefined") break
@@ -1769,15 +1769,15 @@
             }
             _isColorString(e) {
                 if (typeof e == "string") return kr[e]
             }
             setColor(e, t = !0) {
                 if (e === "none") return;
                 let i, s = this._isColorString(e);
-                if (s !== void 0 && (e = s), we(e) === !0) {
+                if (s !== void 0 && (e = s), be(e) === !0) {
                     if (zs(e) === !0) {
                         let o = e.substr(4).substr(0, e.length - 5).split(",");
                         i = {
                             r: o[0],
                             g: o[1],
                             b: o[2],
                             a: 1
@@ -1826,32 +1826,32 @@
                 this.applied = !0, this.updateCallback(this.color), this._updatePicker(this.color)
             }
             _loadLast() {
                 this.previousColor !== void 0 ? this.setColor(this.previousColor, !1) : alert("There is no last color to load...")
             }
             _setColor(e, t = !0) {
                 t === !0 && (this.initialColor = Object.assign({}, e)), this.color = e;
-                let i = vt(e.r, e.g, e.b),
+                let i = bt(e.r, e.g, e.b),
                     s = 2 * Math.PI,
                     o = this.r * i.s,
                     r = this.centerCoordinates.x + o * Math.sin(s * i.h),
                     a = this.centerCoordinates.y + o * Math.cos(s * i.h);
                 this.colorPickerSelector.style.left = r - .5 * this.colorPickerSelector.clientWidth + "px", this.colorPickerSelector.style.top = a - .5 * this.colorPickerSelector.clientHeight + "px", this._updatePicker(e)
             }
             _setOpacity(e) {
                 this.color.a = e / 100, this._updatePicker(this.color)
             }
             _setBrightness(e) {
-                let t = vt(this.color.r, this.color.g, this.color.b);
+                let t = bt(this.color.r, this.color.g, this.color.b);
                 t.v = e / 100;
                 let i = Rt(t.h, t.s, t.v);
                 i.a = this.color.a, this.color = i, this._updatePicker()
             }
             _updatePicker(e = this.color) {
-                let t = vt(e.r, e.g, e.b),
+                let t = bt(e.r, e.g, e.b),
                     i = this.colorPickerCanvas.getContext("2d");
                 this.pixelRation === void 0 && (this.pixelRatio = (window.devicePixelRatio || 1) / (i.webkitBackingStorePixelRatio || i.mozBackingStorePixelRatio || i.msBackingStorePixelRatio || i.oBackingStorePixelRatio || i.backingStorePixelRatio || 1)), i.setTransform(this.pixelRatio, 0, 0, this.pixelRatio, 0, 0);
                 let s = this.colorPickerCanvas.clientWidth,
                     o = this.colorPickerCanvas.clientHeight;
                 i.clearRect(0, 0, s, o), i.putImageData(this.hueCircle, 0, 0), i.fillStyle = "rgba(0,0,0," + (1 - t.v) + ")", i.circle(this.centerCoordinates.x, this.centerCoordinates.y, this.r), i.fill(), this.brightnessRange.value = 100 * t.v, this.opacityRange.value = 100 * e.a, this.initialColorDiv.style.backgroundColor = "rgba(" + this.initialColor.r + "," + this.initialColor.g + "," + this.initialColor.b + "," + this.initialColor.a + ")", this.newColorDiv.style.backgroundColor = "rgba(" + this.color.r + "," + this.color.g + "," + this.color.b + "," + this.color.a + ")"
             }
             _setSize() {
@@ -1933,19 +1933,19 @@
                     h = Math.atan2(a, d),
                     l = .98 * Math.min(Math.sqrt(a * a + d * d), r),
                     c = Math.cos(h) * l + o,
                     u = Math.sin(h) * l + r;
                 this.colorPickerSelector.style.top = c - .5 * this.colorPickerSelector.clientHeight + "px", this.colorPickerSelector.style.left = u - .5 * this.colorPickerSelector.clientWidth + "px";
                 let f = h / (2 * Math.PI);
                 f = f < 0 ? f + 1 : f;
-                let y = l / this.r,
-                    v = vt(this.color.r, this.color.g, this.color.b);
-                v.h = f, v.s = y;
-                let g = Rt(v.h, v.s, v.v);
-                g.a = this.color.a, this.color = g, this.initialColorDiv.style.backgroundColor = "rgba(" + this.initialColor.r + "," + this.initialColor.g + "," + this.initialColor.b + "," + this.initialColor.a + ")", this.newColorDiv.style.backgroundColor = "rgba(" + this.color.r + "," + this.color.g + "," + this.color.b + "," + this.color.a + ")"
+                let m = l / this.r,
+                    b = bt(this.color.r, this.color.g, this.color.b);
+                b.h = f, b.s = m;
+                let p = Rt(b.h, b.s, b.v);
+                p.a = this.color.a, this.color = p, this.initialColorDiv.style.backgroundColor = "rgba(" + this.initialColor.r + "," + this.initialColor.g + "," + this.initialColor.b + "," + this.initialColor.a + ")", this.newColorDiv.style.backgroundColor = "rgba(" + this.color.r + "," + this.color.g + "," + this.color.b + "," + this.color.a + ")"
             }
         };
 
     function gi(...n) {
         if (n.length < 1) throw new TypeError("Invalid arguments.");
         if (n.length === 1) return document.createTextNode(n[0]);
         {
@@ -2047,33 +2047,33 @@
                     o = e[1],
                     r = e[2],
                     a = e[3],
                     d = document.createElement("input");
                 d.className = "vis-configuration vis-config-range";
                 try {
                     d.type = "range", d.min = o, d.max = r
-                } catch (v) {}
+                } catch (b) {}
                 d.step = a;
                 let h = "",
                     l = 0;
                 if (t !== void 0) {
-                    let v = 1.2;
-                    t < 0 && t * v < o ? (d.min = Math.ceil(t * v), l = d.min, h = "range increased") : t / v < o && (d.min = Math.ceil(t / v), l = d.min, h = "range increased"), t * v > r && r !== 1 && (d.max = Math.ceil(t * v), l = d.max, h = "range increased"), d.value = t
+                    let b = 1.2;
+                    t < 0 && t * b < o ? (d.min = Math.ceil(t * b), l = d.min, h = "range increased") : t / b < o && (d.min = Math.ceil(t / b), l = d.min, h = "range increased"), t * b > r && r !== 1 && (d.max = Math.ceil(t * b), l = d.max, h = "range increased"), d.value = t
                 } else d.value = s;
                 let c = document.createElement("input");
                 c.className = "vis-configuration vis-config-rangeinput", c.value = d.value;
                 let u = this;
                 d.onchange = function() {
                     c.value = this.value, u._update(Number(this.value), i)
                 }, d.oninput = function() {
                     c.value = this.value
                 };
                 let f = this._makeLabel(i[i.length - 1], i),
-                    y = this._makeItem(i, f, d, c);
-                h !== "" && this.popupHistory[y] !== l && (this.popupHistory[y] = l, this._setupPopup(h, y))
+                    m = this._makeItem(i, f, d, c);
+                h !== "" && this.popupHistory[m] !== l && (this.popupHistory[m] = l, this._setupPopup(h, m))
             }
             _makeButton() {
                 if (this.options.showButton === !0) {
                     let e = document.createElement("div");
                     e.className = "vis-configuration vis-config-button", e.innerText = "generate options", e.onclick = () => {
                         this._printOptions()
                     }, e.onmouseover = () => {
@@ -2252,70 +2252,70 @@
             hide() {
                 this.hidden = !0, this.frame.style.left = "0", this.frame.style.top = "0", this.frame.style.visibility = "hidden"
             }
             destroy() {
                 this.frame.parentNode.removeChild(this.frame)
             }
         },
-        wt = !1,
+        vt = !1,
         Ls, mi = "background: #FFeeee; color: #dd0000",
-        Pr = class L {
+        Pr = class R {
             static validate(e, t, i) {
-                wt = !1, Ls = t;
+                vt = !1, Ls = t;
                 let s = t;
-                return i !== void 0 && (s = t[i]), L.parse(e, s, []), wt
+                return i !== void 0 && (s = t[i]), R.parse(e, s, []), vt
             }
             static parse(e, t, i) {
-                for (let s in e) Object.prototype.hasOwnProperty.call(e, s) && L.check(s, e, t, i)
+                for (let s in e) Object.prototype.hasOwnProperty.call(e, s) && R.check(s, e, t, i)
             }
             static check(e, t, i, s) {
                 if (i[e] === void 0 && i.__any__ === void 0) {
-                    L.getSuggestion(e, i, s);
+                    R.getSuggestion(e, i, s);
                     return
                 }
                 let o = e,
                     r = !0;
-                i[e] === void 0 && i.__any__ !== void 0 && (o = "__any__", r = L.getType(t[e]) === "object");
+                i[e] === void 0 && i.__any__ !== void 0 && (o = "__any__", r = R.getType(t[e]) === "object");
                 let a = i[o];
-                r && a.__type__ !== void 0 && (a = a.__type__), L.checkFields(e, t, i, o, a, s)
+                r && a.__type__ !== void 0 && (a = a.__type__), R.checkFields(e, t, i, o, a, s)
             }
             static checkFields(e, t, i, s, o, r) {
                 let a = function(l) {
-                        console.error("%c" + l + L.printLocation(r, e), mi)
+                        console.error("%c" + l + R.printLocation(r, e), mi)
                     },
-                    d = L.getType(t[e]),
+                    d = R.getType(t[e]),
                     h = o[d];
-                h !== void 0 ? L.getType(h) === "array" && h.indexOf(t[e]) === -1 ? (a('Invalid option detected in "' + e + '". Allowed values are:' + L.print(h) + ' not "' + t[e] + '". '), wt = !0) : d === "object" && s !== "__any__" && (r = At(r, e), L.parse(t[e], i[s], r)) : o.any === void 0 && (a('Invalid type received for "' + e + '". Expected: ' + L.print(Object.keys(o)) + ". Received [" + d + '] "' + t[e] + '"'), wt = !0)
+                h !== void 0 ? R.getType(h) === "array" && h.indexOf(t[e]) === -1 ? (a('Invalid option detected in "' + e + '". Allowed values are:' + R.print(h) + ' not "' + t[e] + '". '), vt = !0) : d === "object" && s !== "__any__" && (r = At(r, e), R.parse(t[e], i[s], r)) : o.any === void 0 && (a('Invalid type received for "' + e + '". Expected: ' + R.print(Object.keys(o)) + ". Received [" + d + '] "' + t[e] + '"'), vt = !0)
             }
             static getType(e) {
                 let t = typeof e;
                 return t === "object" ? e === null ? "null" : e instanceof Boolean ? "boolean" : e instanceof Number ? "number" : e instanceof String ? "string" : Array.isArray(e) ? "array" : e instanceof Date ? "date" : e.nodeType !== void 0 ? "dom" : e._isAMomentObject === !0 ? "moment" : "object" : t === "number" ? "number" : t === "boolean" ? "boolean" : t === "string" ? "string" : t === void 0 ? "undefined" : t
             }
             static getSuggestion(e, t, i) {
-                let s = L.findInOptions(e, t, i, !1),
-                    o = L.findInOptions(e, Ls, [], !0),
+                let s = R.findInOptions(e, t, i, !1),
+                    o = R.findInOptions(e, Ls, [], !0),
                     r = 8,
                     a = 4,
                     d;
-                s.indexMatch !== void 0 ? d = " in " + L.printLocation(s.path, e, "") + 'Perhaps it was incomplete? Did you mean: "' + s.indexMatch + `"?
+                s.indexMatch !== void 0 ? d = " in " + R.printLocation(s.path, e, "") + 'Perhaps it was incomplete? Did you mean: "' + s.indexMatch + `"?
 
-` : o.distance <= a && s.distance > o.distance ? d = " in " + L.printLocation(s.path, e, "") + "Perhaps it was misplaced? Matching option found at: " + L.printLocation(o.path, o.closestMatch, "") : s.distance <= r ? d = '. Did you mean "' + s.closestMatch + '"?' + L.printLocation(s.path, e) : d = ". Did you mean one of these: " + L.print(Object.keys(t)) + L.printLocation(i, e), console.error('%cUnknown option detected: "' + e + '"' + d, mi), wt = !0
+` : o.distance <= a && s.distance > o.distance ? d = " in " + R.printLocation(s.path, e, "") + "Perhaps it was misplaced? Matching option found at: " + R.printLocation(o.path, o.closestMatch, "") : s.distance <= r ? d = '. Did you mean "' + s.closestMatch + '"?' + R.printLocation(s.path, e) : d = ". Did you mean one of these: " + R.print(Object.keys(t)) + R.printLocation(i, e), console.error('%cUnknown option detected: "' + e + '"' + d, mi), vt = !0
             }
             static findInOptions(e, t, i, s = !1) {
                 let o = 1e9,
                     r = "",
                     a = [],
                     d = e.toLowerCase(),
                     h;
                 for (let l in t) {
                     let c;
                     if (t[l].__type__ !== void 0 && s === !0) {
-                        let u = L.findInOptions(e, t[l], At(i, l));
+                        let u = R.findInOptions(e, t[l], At(i, l));
                         o > u.distance && (r = u.closestMatch, a = u.path, o = u.distance, h = u.indexMatch)
-                    } else l.toLowerCase().indexOf(d) !== -1 && (h = l), c = L.levenshteinDistance(e, l), o > c && (r = l, a = xr(i), o = c)
+                    } else l.toLowerCase().indexOf(d) !== -1 && (h = l), c = R.levenshteinDistance(e, l), o > c && (r = l, a = xr(i), o = c)
                 }
                 return {
                     closestMatch: r,
                     path: a,
                     distance: o,
                     indexMatch: h
                 }
@@ -2355,39 +2355,39 @@
                 let o;
                 for (o = 0; o <= e.length; o++) i[0][o] = o;
                 for (s = 1; s <= t.length; s++)
                     for (o = 1; o <= e.length; o++) t.charAt(s - 1) == e.charAt(o - 1) ? i[s][o] = i[s - 1][o - 1] : i[s][o] = Math.min(i[s - 1][o - 1] + 1, Math.min(i[s][o - 1] + 1, i[s - 1][o] + 1));
                 return i[t.length][e.length]
             }
         },
-        Hs = pe;
+        Hs = fe;
     var js = Sr,
-        Ue = ui,
+        We = ui,
         Ws = Ir,
         yi = mi,
         Vs = Pr;
-    var Ht, Mr = new Uint8Array(16);
+    var Ht, Dr = new Uint8Array(16);
 
     function bi() {
         if (!Ht && (Ht = typeof crypto != "undefined" && crypto.getRandomValues && crypto.getRandomValues.bind(crypto) || typeof msCrypto != "undefined" && typeof msCrypto.getRandomValues == "function" && msCrypto.getRandomValues.bind(msCrypto), !Ht)) throw new Error("crypto.getRandomValues() not supported. See https://github.com/uuidjs/uuid#getrandomvalues-not-supported");
-        return Ht(Mr)
+        return Ht(Dr)
     }
     var qs = /^(?:[0-9a-f]{8}-[0-9a-f]{4}-[1-5][0-9a-f]{3}-[89ab][0-9a-f]{3}-[0-9a-f]{12}|00000000-0000-0000-0000-000000000000)$/i;
 
-    function Dr(n) {
+    function Mr(n) {
         return typeof n == "string" && qs.test(n)
     }
-    var Us = Dr;
-    var U = [];
-    for (jt = 0; jt < 256; ++jt) U.push((jt + 256).toString(16).substr(1));
+    var Us = Mr;
+    var q = [];
+    for (jt = 0; jt < 256; ++jt) q.push((jt + 256).toString(16).substr(1));
     var jt;
 
     function Fr(n) {
         var e = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : 0,
-            t = (U[n[e + 0]] + U[n[e + 1]] + U[n[e + 2]] + U[n[e + 3]] + "-" + U[n[e + 4]] + U[n[e + 5]] + "-" + U[n[e + 6]] + U[n[e + 7]] + "-" + U[n[e + 8]] + U[n[e + 9]] + "-" + U[n[e + 10]] + U[n[e + 11]] + U[n[e + 12]] + U[n[e + 13]] + U[n[e + 14]] + U[n[e + 15]]).toLowerCase();
+            t = (q[n[e + 0]] + q[n[e + 1]] + q[n[e + 2]] + q[n[e + 3]] + "-" + q[n[e + 4]] + q[n[e + 5]] + "-" + q[n[e + 6]] + q[n[e + 7]] + "-" + q[n[e + 8]] + q[n[e + 9]] + "-" + q[n[e + 10]] + q[n[e + 11]] + q[n[e + 12]] + q[n[e + 13]] + q[n[e + 14]] + q[n[e + 15]]).toLowerCase();
         if (!Us(t)) throw TypeError("Stringified UUID is invalid");
         return t
     }
     var Ys = Fr;
 
     function Nr(n, e, t) {
         n = n || {};
@@ -2395,26 +2395,26 @@
         if (i[6] = i[6] & 15 | 64, i[8] = i[8] & 63 | 128, e) {
             t = t || 0;
             for (var s = 0; s < 16; ++s) e[t + s] = i[s];
             return e
         }
         return Ys(i)
     }
-    var xe = Nr;
+    var _e = Nr;
 
     function Xs(n) {
         return typeof n == "string" || typeof n == "number"
     }
     var Wt = class {
             constructor(e) {
-                X(this, "delay");
-                X(this, "max");
-                X(this, "_queue", []);
-                X(this, "_timeout", null);
-                X(this, "_extended", null);
+                Y(this, "delay");
+                Y(this, "max");
+                Y(this, "_queue", []);
+                Y(this, "_timeout", null);
+                Y(this, "_extended", null);
                 this.delay = null, this.max = 1 / 0, this.setOptions(e)
             }
             setOptions(e) {
                 e && typeof e.delay != "undefined" && (this.delay = e.delay), e && typeof e.max != "undefined" && (this.max = e.max), this._flushIfNeeded()
             }
             static extend(e, t) {
                 let i = new Wt(t);
@@ -2474,41 +2474,41 @@
             }
             flush() {
                 this._queue.splice(0).forEach(e => {
                     e.fn.apply(e.context || e.fn, e.args || [])
                 })
             }
         },
-        _t = class {
+        wt = class {
             constructor() {
-                X(this, "_subscribers", {
+                Y(this, "_subscribers", {
                     "*": [],
                     add: [],
                     remove: [],
                     update: []
                 });
-                X(this, "subscribe", _t.prototype.on);
-                X(this, "unsubscribe", _t.prototype.off)
+                Y(this, "subscribe", wt.prototype.on);
+                Y(this, "unsubscribe", wt.prototype.off)
             }
             _trigger(e, t, i) {
                 if (e === "*") throw new Error("Cannot trigger event *");
                 [...this._subscribers[e], ...this._subscribers["*"]].forEach(s => {
                     s(e, t, i != null ? i : null)
                 })
             }
             on(e, t) {
                 typeof t == "function" && this._subscribers[e].push(t)
             }
             off(e, t) {
                 this._subscribers[e] = this._subscribers[e].filter(i => i !== t)
             }
         },
-        Ie = class {
+        ke = class {
             constructor(e) {
-                X(this, "_pairs");
+                Y(this, "_pairs");
                 this._pairs = e
             }*[Symbol.iterator]() {
                 for (let [e, t] of this._pairs) yield [e, t]
             }* entries() {
                 for (let [e, t] of this._pairs) yield [e, t]
             }* keys() {
                 for (let [e] of this._pairs) yield e
@@ -2535,35 +2535,35 @@
             toIdSet() {
                 return new Set(this.toIdArray())
             }
             toItemSet() {
                 return new Set(this.toItemArray())
             }
             cache() {
-                return new Ie([...this._pairs])
+                return new ke([...this._pairs])
             }
             distinct(e) {
                 let t = new Set;
                 for (let [i, s] of this._pairs) t.add(e(s, i));
                 return t
             }
             filter(e) {
                 let t = this._pairs;
-                return new Ie({
+                return new ke({
                     *[Symbol.iterator]() {
                         for (let [i, s] of t) e(s, i) && (yield [i, s])
                     }
                 })
             }
             forEach(e) {
                 for (let [t, i] of this._pairs) e(i, t)
             }
             map(e) {
                 let t = this._pairs;
-                return new Ie({
+                return new ke({
                     *[Symbol.iterator]() {
                         for (let [i, s] of t) yield [i, e(s, i)]
                     }
                 })
             }
             max(e) {
                 let t = this._pairs[Symbol.iterator](),
@@ -2590,32 +2590,32 @@
                 return s
             }
             reduce(e, t) {
                 for (let [i, s] of this._pairs) t = e(t, s, i);
                 return t
             }
             sort(e) {
-                return new Ie({
+                return new ke({
                     [Symbol.iterator]: () => [...this._pairs].sort(([t, i], [s, o]) => e(i, o, t, s))[Symbol.iterator]()
                 })
             }
         };
 
     function Br(n, e) {
-        return n[e] == null && (n[e] = xe()), n
+        return n[e] == null && (n[e] = _e()), n
     }
-    var Ce = class extends _t {
+    var Ee = class extends wt {
         constructor(e, t) {
             super();
-            X(this, "flush");
-            X(this, "length");
-            X(this, "_options");
-            X(this, "_data");
-            X(this, "_idProp");
-            X(this, "_queue", null);
+            Y(this, "flush");
+            Y(this, "length");
+            Y(this, "_options");
+            Y(this, "_data");
+            Y(this, "_idProp");
+            Y(this, "_queue", null);
             e && !Array.isArray(e) && (t = e, e = []), this._options = t || {}, this._data = new Map, this.length = 0, this._idProp = this._options.fieldId || "id", e && e.length && this.add(e), this.setOptions(t)
         }
         get idProp() {
             return this._idProp
         }
         setOptions(e) {
             e && e.queue !== void 0 && (e.queue === !1 ? this._queue && (this._queue.destroy(), this._queue = null) : (this._queue || (this._queue = Wt.extend(this, {
@@ -2712,22 +2712,22 @@
                 l = [...this._data.keys()];
                 for (let u = 0, f = l.length; u < f; u++) c = l[u], h = this._data.get(c), h != null && (!a || a(h)) && d.push(h)
             }
             if (o && o.order && i == null && this._sort(d, o.order), o && o.fields) {
                 let u = o.fields;
                 if (i != null && h != null) h = this._filterFields(h, u);
                 else
-                    for (let f = 0, y = d.length; f < y; f++) d[f] = this._filterFields(d[f], u)
+                    for (let f = 0, m = d.length; f < m; f++) d[f] = this._filterFields(d[f], u)
             }
             if (r == "Object") {
                 let u = {};
-                for (let f = 0, y = d.length; f < y; f++) {
-                    let v = d[f],
-                        g = v[this._idProp];
-                    u[g] = v
+                for (let f = 0, m = d.length; f < m; f++) {
+                    let b = d[f],
+                        p = b[this._idProp];
+                    u[p] = b
                 }
                 return u
             } else return i != null ? h != null ? h : null : d
         }
         getIds(e) {
             let t = this._data,
                 i = e && e.filter,
@@ -2885,28 +2885,28 @@
             return this._data.set(i, t), ++this.length, i
         }
         _updateItem(e) {
             let t = e[this._idProp];
             if (t == null) throw new Error("Cannot update item: item has no id (item: " + JSON.stringify(e) + ")");
             let i = this._data.get(t);
             if (!i) throw new Error("Cannot update item: no item with id " + t + " found");
-            return this._data.set(t, le(le({}, i), e)), t
+            return this._data.set(t, de(de({}, i), e)), t
         }
         stream(e) {
             if (e) {
                 let t = this._data;
-                return new Ie({
+                return new ke({
                     *[Symbol.iterator]() {
                         for (let i of e) {
                             let s = t.get(i);
                             s != null && (yield [i, s])
                         }
                     }
                 })
-            } else return new Ie({
+            } else return new ke({
                 [Symbol.iterator]: this._data.entries.bind(this._data)
             })
         }
     };
 
     function Ar(n, e) {
         return typeof e == "object" && e !== null && n === e.idProp && typeof e.add == "function" && typeof e.clear == "function" && typeof e.distinct == "function" && typeof e.forEach == "function" && typeof e.get == "function" && typeof e.getDataSet == "function" && typeof e.getIds == "function" && typeof e.length == "number" && typeof e.map == "function" && typeof e.max == "function" && typeof e.min == "function" && typeof e.off == "function" && typeof e.on == "function" && typeof e.remove == "function" && typeof e.setOptions == "function" && typeof e.stream == "function" && typeof e.update == "function" && typeof e.updateOnly == "function"
@@ -3048,17 +3048,17 @@
                     if (l.shiftKey == !1 && o[c].shift == !1 && l.keyCode == o[c].code) return c;
                     if (l.keyCode == o[c].code && c == "shift") return c
                 } return "unknown key, currently not supported"
         }, i.unbind = function(l, c, u) {
             if (u === void 0 && (u = "keydown"), o[l] === void 0) throw new Error("unsupported key: " + l);
             if (c !== void 0) {
                 var f = [],
-                    y = s[u][o[l].code];
-                if (y !== void 0)
-                    for (var v = 0; v < y.length; v++) y[v].fn == c && y[v].shift == o[l].shift || f.push(s[u][o[l].code][v]);
+                    m = s[u][o[l].code];
+                if (m !== void 0)
+                    for (var b = 0; b < m.length; b++) m[b].fn == c && m[b].shift == o[l].shift || f.push(s[u][o[l].code][b]);
                 s[u][o[l].code] = f
             } else s[u][o[l].code] = []
         }, i.reset = function() {
             s = {
                 keydown: {},
                 keyup: {}
             }
@@ -3131,32 +3131,32 @@
             a = s * o,
             d = .5522848,
             h = r / 2 * d,
             l = a / 2 * d,
             c = e + r,
             u = t + a,
             f = e + r / 2,
-            y = t + a / 2,
-            v = t + (s - a / 2),
-            g = t + s;
-        n.beginPath(), n.moveTo(c, y), n.bezierCurveTo(c, y + l, f + h, u, f, u), n.bezierCurveTo(f - h, u, e, y + l, e, y), n.bezierCurveTo(e, y - l, f - h, t, f, t), n.bezierCurveTo(f + h, t, c, y - l, c, y), n.lineTo(c, v), n.bezierCurveTo(c, v + l, f + h, g, f, g), n.bezierCurveTo(f - h, g, e, v + l, e, v), n.lineTo(e, y)
+            m = t + a / 2,
+            b = t + (s - a / 2),
+            p = t + s;
+        n.beginPath(), n.moveTo(c, m), n.bezierCurveTo(c, m + l, f + h, u, f, u), n.bezierCurveTo(f - h, u, e, m + l, e, m), n.bezierCurveTo(e, m - l, f - h, t, f, t), n.bezierCurveTo(f + h, t, c, m - l, c, m), n.lineTo(c, b), n.bezierCurveTo(c, b + l, f + h, p, f, p), n.bezierCurveTo(f - h, p, e, b + l, e, b), n.lineTo(e, m)
     }
 
     function Zs(n, e, t, i, s, o) {
         n.beginPath(), n.moveTo(e, t);
         let r = o.length,
             a = i - e,
             d = s - t,
             h = d / a,
             l = Math.sqrt(a * a + d * d),
             c = 0,
             u = !0,
             f = 0,
-            y = +o[0];
-        for (; l >= .1;) y = +o[c++ % r], y > l && (y = l), f = Math.sqrt(y * y / (1 + h * h)), f = a < 0 ? -f : f, e += f, t += h * f, u === !0 ? n.lineTo(e, t) : n.moveTo(e, t), l -= y, u = !u
+            m = +o[0];
+        for (; l >= .1;) m = +o[c++ % r], m > l && (m = l), f = Math.sqrt(m * m / (1 + h * h)), f = a < 0 ? -f : f, e += f, t += h * f, u === !0 ? n.lineTo(e, t) : n.moveTo(e, t), l -= m, u = !u
     }
 
     function Wr(n, e, t, i) {
         n.beginPath();
         let s = 6,
             o = Math.PI * 2 / s;
         n.moveTo(e + i, t);
@@ -3181,15 +3181,15 @@
     function Vr(n) {
         return Object.prototype.hasOwnProperty.call(Qs, n) ? Qs[n] : function(e, ...t) {
             CanvasRenderingContext2D.prototype[n].call(e, t)
         }
     }
 
     function qr(n) {
-        return Pe = n, Gr()
+        return Oe = n, Gr()
     }
     var Js = {
             fontsize: "font.size",
             fontcolor: "font.color",
             labelfontcolor: "font.color",
             fontname: "font.face",
             color: ["color.border", "color.background"],
@@ -3213,38 +3213,38 @@
             "]": !0,
             ";": !0,
             "=": !0,
             ",": !0,
             "->": !0,
             "--": !0
         },
-        Pe = "",
-        it = 0,
+        Oe = "",
+        tt = 0,
         P = "",
-        S = "",
+        k = "",
         ee = Z.NULL;
 
     function Ur() {
-        it = 0, P = Pe.charAt(0)
+        tt = 0, P = Oe.charAt(0)
     }
 
     function V() {
-        it++, P = Pe.charAt(it)
+        tt++, P = Oe.charAt(tt)
     }
 
-    function st() {
-        return Pe.charAt(it + 1)
+    function it() {
+        return Oe.charAt(tt + 1)
     }
 
     function to(n) {
         var e = n.charCodeAt(0);
         return e < 47 ? e === 35 || e === 46 : e < 59 ? e > 47 : e < 91 ? e > 64 : e < 96 ? e === 95 : e < 123 ? e > 96 : !1
     }
 
-    function Me(n, e) {
+    function Se(n, e) {
         if (n || (n = {}), e)
             for (var t in e) e.hasOwnProperty(t) && (n[t] = e[t]);
         return n
     }
 
     function Yr(n, e, t) {
         for (var i = e.split("."), s = n; i.length;) {
@@ -3260,170 +3260,170 @@
                 if (e.id === r.nodes[t].id) {
                     s = r.nodes[t];
                     break
                 }
         }
         for (s || (s = {
                 id: e.id
-            }, n.node && (s.attr = Me(s.attr, n.node))), t = o.length - 1; t >= 0; t--) {
+            }, n.node && (s.attr = Se(s.attr, n.node))), t = o.length - 1; t >= 0; t--) {
             var a = o[t];
             a.nodes || (a.nodes = []), a.nodes.indexOf(s) === -1 && a.nodes.push(s)
         }
-        e.attr && (s.attr = Me(s.attr, e.attr))
+        e.attr && (s.attr = Se(s.attr, e.attr))
     }
 
     function Xr(n, e) {
         if (n.edges || (n.edges = []), n.edges.push(e), n.edge) {
-            var t = Me({}, n.edge);
-            e.attr = Me(t, e.attr)
+            var t = Se({}, n.edge);
+            e.attr = Se(t, e.attr)
         }
     }
 
     function so(n, e, t, i, s) {
         var o = {
             from: e,
             to: t,
             type: i
         };
-        return n.edge && (o.attr = Me({}, n.edge)), o.attr = Me(o.attr || {}, s), s != null && s.hasOwnProperty("arrows") && s.arrows != null && (o.arrows = {
+        return n.edge && (o.attr = Se({}, n.edge)), o.attr = Se(o.attr || {}, s), s != null && s.hasOwnProperty("arrows") && s.arrows != null && (o.arrows = {
             to: {
                 enabled: !0,
                 type: s.arrows.type
             }
         }, s.arrows = null), o
     }
 
-    function B() {
-        for (ee = Z.NULL, S = ""; P === " " || P === "	" || P === `
+    function N() {
+        for (ee = Z.NULL, k = ""; P === " " || P === "	" || P === `
 ` || P === "\r";) V();
         do {
             var n = !1;
             if (P === "#") {
-                for (var e = it - 1; Pe.charAt(e) === " " || Pe.charAt(e) === "	";) e--;
-                if (Pe.charAt(e) === `
-` || Pe.charAt(e) === "") {
+                for (var e = tt - 1; Oe.charAt(e) === " " || Oe.charAt(e) === "	";) e--;
+                if (Oe.charAt(e) === `
+` || Oe.charAt(e) === "") {
                     for (; P != "" && P != `
 `;) V();
                     n = !0
                 }
             }
-            if (P === "/" && st() === "/") {
+            if (P === "/" && it() === "/") {
                 for (; P != "" && P != `
 `;) V();
                 n = !0
             }
-            if (P === "/" && st() === "*") {
+            if (P === "/" && it() === "*") {
                 for (; P != "";)
-                    if (P === "*" && st() === "/") {
+                    if (P === "*" && it() === "/") {
                         V(), V();
                         break
                     } else V();
                 n = !0
             }
             for (; P === " " || P === "	" || P === `
 ` || P === "\r";) V()
         } while (n);
         if (P === "") {
             ee = Z.DELIMITER;
             return
         }
-        var t = P + st();
+        var t = P + it();
         if (eo[t]) {
-            ee = Z.DELIMITER, S = t, V(), V();
+            ee = Z.DELIMITER, k = t, V(), V();
             return
         }
         if (eo[P]) {
-            ee = Z.DELIMITER, S = P, V();
+            ee = Z.DELIMITER, k = P, V();
             return
         }
         if (to(P) || P === "-") {
-            for (S += P, V(); to(P);) S += P, V();
-            S === "false" ? S = !1 : S === "true" ? S = !0 : isNaN(Number(S)) || (S = Number(S)), ee = Z.IDENTIFIER;
+            for (k += P, V(); to(P);) k += P, V();
+            k === "false" ? k = !1 : k === "true" ? k = !0 : isNaN(Number(k)) || (k = Number(k)), ee = Z.IDENTIFIER;
             return
         }
         if (P === '"') {
-            for (V(); P != "" && (P != '"' || P === '"' && st() === '"');) P === '"' ? (S += P, V()) : P === "\\" && st() === "n" ? (S += `
-`, V()) : S += P, V();
+            for (V(); P != "" && (P != '"' || P === '"' && it() === '"');) P === '"' ? (k += P, V()) : P === "\\" && it() === "n" ? (k += `
+`, V()) : k += P, V();
             if (P != '"') throw Q('End of string " expected');
             V(), ee = Z.IDENTIFIER;
             return
         }
-        for (ee = Z.UNKNOWN; P != "";) S += P, V();
-        throw new SyntaxError('Syntax error in part "' + ao(S, 30) + '"')
+        for (ee = Z.UNKNOWN; P != "";) k += P, V();
+        throw new SyntaxError('Syntax error in part "' + ao(k, 30) + '"')
     }
 
     function Gr() {
         var n = {};
-        if (Ur(), B(), S === "strict" && (n.strict = !0, B()), (S === "graph" || S === "digraph") && (n.type = S, B()), ee === Z.IDENTIFIER && (n.id = S, B()), S != "{") throw Q("Angle bracket { expected");
-        if (B(), oo(n), S != "}") throw Q("Angle bracket } expected");
-        if (B(), S !== "") throw Q("End of file expected");
-        return B(), delete n.node, delete n.edge, delete n.graph, n
+        if (Ur(), N(), k === "strict" && (n.strict = !0, N()), (k === "graph" || k === "digraph") && (n.type = k, N()), ee === Z.IDENTIFIER && (n.id = k, N()), k != "{") throw Q("Angle bracket { expected");
+        if (N(), oo(n), k != "}") throw Q("Angle bracket } expected");
+        if (N(), k !== "") throw Q("End of file expected");
+        return N(), delete n.node, delete n.edge, delete n.graph, n
     }
 
     function oo(n) {
-        for (; S !== "" && S != "}";) Kr(n), S === ";" && B()
+        for (; k !== "" && k != "}";) Kr(n), k === ";" && N()
     }
 
     function Kr(n) {
         var e = no(n);
         if (e) {
             ro(n, e);
             return
         }
         var t = $r(n);
         if (!t) {
             if (ee != Z.IDENTIFIER) throw Q("Identifier expected");
-            var i = S;
-            if (B(), S === "=") {
-                if (B(), ee != Z.IDENTIFIER) throw Q("Identifier expected");
-                n[i] = S, B()
+            var i = k;
+            if (N(), k === "=") {
+                if (N(), ee != Z.IDENTIFIER) throw Q("Identifier expected");
+                n[i] = k, N()
             } else Zr(n, i)
         }
     }
 
     function no(n) {
         var e = null;
-        if (S === "subgraph" && (e = {}, e.type = "subgraph", B(), ee === Z.IDENTIFIER && (e.id = S, B())), S === "{") {
-            if (B(), e || (e = {}), e.parent = n, e.node = n.node, e.edge = n.edge, e.graph = n.graph, oo(e), S != "}") throw Q("Angle bracket } expected");
-            B(), delete e.node, delete e.edge, delete e.graph, delete e.parent, n.subgraphs || (n.subgraphs = []), n.subgraphs.push(e)
+        if (k === "subgraph" && (e = {}, e.type = "subgraph", N(), ee === Z.IDENTIFIER && (e.id = k, N())), k === "{") {
+            if (N(), e || (e = {}), e.parent = n, e.node = n.node, e.edge = n.edge, e.graph = n.graph, oo(e), k != "}") throw Q("Angle bracket } expected");
+            N(), delete e.node, delete e.edge, delete e.graph, delete e.parent, n.subgraphs || (n.subgraphs = []), n.subgraphs.push(e)
         }
         return e
     }
 
     function $r(n) {
-        return S === "node" ? (B(), n.node = Et(), "node") : S === "edge" ? (B(), n.edge = Et(), "edge") : S === "graph" ? (B(), n.graph = Et(), "graph") : null
+        return k === "node" ? (N(), n.node = _t(), "node") : k === "edge" ? (N(), n.edge = _t(), "edge") : k === "graph" ? (N(), n.graph = _t(), "graph") : null
     }
 
     function Zr(n, e) {
         var t = {
                 id: e
             },
-            i = Et();
+            i = _t();
         i && (t.attr = i), io(n, t), ro(n, e)
     }
 
     function ro(n, e) {
-        for (; S === "->" || S === "--";) {
-            var t, i = S;
-            B();
+        for (; k === "->" || k === "--";) {
+            var t, i = k;
+            N();
             var s = no(n);
             if (s) t = s;
             else {
                 if (ee != Z.IDENTIFIER) throw Q("Identifier or subgraph expected");
-                t = S, io(n, {
+                t = k, io(n, {
                     id: t
-                }), B()
+                }), N()
             }
-            var o = Et(),
+            var o = _t(),
                 r = so(n, e, t, i, o);
             Xr(n, r), e = t
         }
     }
 
-    function Et() {
+    function _t() {
         for (var n, e = null, t = {
                 dashed: !0,
                 solid: !1,
                 dotted: [1, 5]
             }, i = {
                 dot: "circle",
                 box: "box",
@@ -3431,21 +3431,21 @@
                 curve: "curve",
                 icurve: "inv_curve",
                 normal: "triangle",
                 inv: "inv_triangle",
                 diamond: "diamond",
                 tee: "bar",
                 vee: "vee"
-            }, s = new Array, o = new Array; S === "[";) {
-            for (B(), e = {}; S !== "" && S != "]";) {
+            }, s = new Array, o = new Array; k === "[";) {
+            for (N(), e = {}; k !== "" && k != "]";) {
                 if (ee != Z.IDENTIFIER) throw Q("Attribute name expected");
-                var r = S;
-                if (B(), S != "=") throw Q("Equal sign = expected");
-                if (B(), ee != Z.IDENTIFIER) throw Q("Attribute value expected");
-                var a = S;
+                var r = k;
+                if (N(), k != "=") throw Q("Equal sign = expected");
+                if (N(), ee != Z.IDENTIFIER) throw Q("Attribute value expected");
+                var a = k;
                 r === "style" && (a = t[a]);
                 var d;
                 r === "arrowhead" && (d = i[a], r = "arrows", a = {
                     to: {
                         enabled: !0,
                         type: d
                     }
@@ -3454,18 +3454,18 @@
                         enabled: !0,
                         type: d
                     }
                 }), s.push({
                     attr: e,
                     name: r,
                     value: a
-                }), o.push(r), B(), S == "," && B()
+                }), o.push(r), N(), k == "," && N()
             }
-            if (S != "]") throw Q("Bracket ] expected");
-            B()
+            if (k != "]") throw Q("Bracket ] expected");
+            N()
         }
         if (o.includes("dir")) {
             var h = {};
             for (h.arrows = {}, n = 0; n < s.length; n++)
                 if (s[n].name === "arrows")
                     if (s[n].value.to != null) h.arrows.to = n;
                     else if (s[n].value.from != null) h.arrows.from = n;
@@ -3659,26 +3659,26 @@
                         type: s[h.arrows.to].value.to.type
                     }
                 }
             };
             else throw Q('Invalid dir type "' + l + '"');
             s.splice(h.dir, 1)
         }
-        var y;
+        var m;
         if (o.includes("penwidth")) {
-            var v = [];
-            for (y = s.length, n = 0; n < y; n++) s[n].name !== "width" && (s[n].name === "penwidth" && (s[n].name = "width"), v.push(s[n]));
-            s = v
+            var b = [];
+            for (m = s.length, n = 0; n < m; n++) s[n].name !== "width" && (s[n].name === "penwidth" && (s[n].name = "width"), b.push(s[n]));
+            s = b
         }
-        for (y = s.length, n = 0; n < y; n++) Yr(s[n].attr, s[n].name, s[n].value);
+        for (m = s.length, n = 0; n < m; n++) Yr(s[n].attr, s[n].name, s[n].value);
         return e
     }
 
     function Q(n) {
-        return new SyntaxError(n + ', got "' + ao(S, 30) + '" (char ' + it + ")")
+        return new SyntaxError(n + ', got "' + ao(k, 30) + '" (char ' + tt + ")")
     }
 
     function ao(n, e) {
         return n.length <= e ? n : n.substr(0, 27) + "..."
     }
 
     function Qr(n, e, t) {
@@ -3718,22 +3718,22 @@
                 options: {}
             };
         if (e.nodes && e.nodes.forEach(function(s) {
                 var o = {
                     id: s.id,
                     label: String(s.label || s.id)
                 };
-                Me(o, ho(s.attr, Js)), o.image && (o.shape = "image"), t.nodes.push(o)
+                Se(o, ho(s.attr, Js)), o.image && (o.shape = "image"), t.nodes.push(o)
             }), e.edges) {
             var i = function(s) {
                 var o = {
                     from: s.from,
                     to: s.to
                 };
-                return Me(o, ho(s.attr, Ei)), o.arrows == null && s.type === "->" && (o.arrows = "to"), o
+                return Se(o, ho(s.attr, Ei)), o.arrows == null && s.type === "->" && (o.arrows = "to"), o
             };
             e.edges.forEach(function(s) {
                 var o, r;
                 s.from instanceof Object ? o = s.from.nodes : o = {
                     id: s.from
                 }, s.to instanceof Object ? r = s.to.nodes : r = {
                     id: s.to
@@ -4339,19 +4339,19 @@
                 return this._groups.has(e) || this._groupNames.push(e), this._groups.set(e, t), t
             }
         };
 
     function Ci(n, e) {
         let t = ["node", "edge", "label"],
             i = !0,
-            s = Ee(e, "chosen");
+            s = we(e, "chosen");
         if (typeof s == "boolean") i = s;
         else if (typeof s == "object") {
             if (t.indexOf(n) === -1) throw new Error("choosify: subOption '" + n + "' should be one of '" + t.join("', '") + "'");
-            let o = Ee(e, ["chosen", n]);
+            let o = we(e, ["chosen", n]);
             (typeof o == "boolean" || typeof o == "function") && (i = o)
         }
         return i
     }
 
     function Ti(n, e, t) {
         if (n.width <= 0 || n.height <= 0) return !1;
@@ -4650,15 +4650,15 @@
                         let a = s.slice(0, o).join("");
                         o == s.length && i ? this.lines.append(a, t) : this.lines.newLine(a, t), s = s.slice(r)
                     }
                 }
             }
         },
         Ut = ["bold", "ital", "boldital", "mono"],
-        Ye = class {
+        Ve = class {
             constructor(e, t, i = !1) {
                 this.body = e, this.pointToSelf = !1, this.baseSize = void 0, this.fontOptions = {}, this.setOptions(t), this.size = {
                     top: 0,
                     left: 0,
                     width: 0,
                     height: 0,
                     yLine: 0
@@ -4672,15 +4672,15 @@
                         t !== void 0 && (this.baseSize = t)
                     }
                 }
             }
             initFontOptions(e) {
                 if (I(Ut, t => {
                         this.fontOptions[t] = {}
-                    }), Ye.parseFontString(this.fontOptions, e)) {
+                    }), Ve.parseFontString(this.fontOptions, e)) {
                     this.fontOptions.vadjust = 0;
                     return
                 }
                 I(e, (t, i) => {
                     t != null && typeof t != "object" && (this.fontOptions[i] = t)
                 })
             }
@@ -4694,28 +4694,28 @@
                         constrainWidth: !1,
                         maxWdt: -1,
                         minWdt: -1,
                         constrainHeight: !1,
                         minHgt: -1,
                         valign: "middle"
                     },
-                    i = Ee(e, "widthConstraint");
+                    i = we(e, "widthConstraint");
                 if (typeof i == "number") t.maxWdt = Number(i), t.minWdt = Number(i);
                 else if (typeof i == "object") {
-                    let o = Ee(e, ["widthConstraint", "maximum"]);
+                    let o = we(e, ["widthConstraint", "maximum"]);
                     typeof o == "number" && (t.maxWdt = Number(o));
-                    let r = Ee(e, ["widthConstraint", "minimum"]);
+                    let r = we(e, ["widthConstraint", "minimum"]);
                     typeof r == "number" && (t.minWdt = Number(r))
                 }
-                let s = Ee(e, "heightConstraint");
+                let s = we(e, "heightConstraint");
                 if (typeof s == "number") t.minHgt = Number(s);
                 else if (typeof s == "object") {
-                    let o = Ee(e, ["heightConstraint", "minimum"]);
+                    let o = we(e, ["heightConstraint", "minimum"]);
                     typeof o == "number" && (t.minHgt = Number(o));
-                    let r = Ee(e, ["heightConstraint", "valign"]);
+                    let r = we(e, ["heightConstraint", "valign"]);
                     typeof r == "string" && (r === "top" || r === "bottom") && (t.valign = r)
                 }
                 return t
             }
             update(e, t) {
                 this.setOptions(e, !0), this.propagateFonts(t), D(this.fontOptions, this.constrain(t)), this.fontOptions.chooser = Ci("label", t)
             }
@@ -4734,28 +4734,28 @@
                 e.push(i)
             }
             getBasicOptions(e) {
                 let t = {};
                 for (let i = 0; i < e.length; ++i) {
                     let s = e[i],
                         o = {};
-                    Ye.parseFontString(o, s) && (s = o), I(s, (r, a) => {
+                    Ve.parseFontString(o, s) && (s = o), I(s, (r, a) => {
                         r !== void 0 && (Object.prototype.hasOwnProperty.call(t, a) || (Ut.indexOf(a) !== -1 ? t[a] = {} : t[a] = r))
                     })
                 }
                 return t
             }
             getFontOption(e, t, i) {
                 let s;
                 for (let o = 0; o < e.length; ++o) {
                     let r = e[o];
                     if (Object.prototype.hasOwnProperty.call(r, t)) {
                         if (s = r[t], s == null) continue;
                         let a = {};
-                        if (Ye.parseFontString(a, s) && (s = a), Object.prototype.hasOwnProperty.call(s, i)) return s[i]
+                        if (Ve.parseFontString(a, s) && (s = a), Object.prototype.hasOwnProperty.call(s, i)) return s[i]
                     }
                 }
                 if (Object.prototype.hasOwnProperty.call(this.fontOptions, i)) return this.fontOptions[i];
                 throw new Error("Did not find value for multi-font for property: '" + i + "'")
             }
             getFontOptions(e, t) {
                 let i = {},
@@ -4887,15 +4887,15 @@
                 let s = this._processLabelText(e, t, i, this.elementOptions.label);
                 this.fontOptions.minWdt > 0 && s.width < this.fontOptions.minWdt && (s.width = this.fontOptions.minWdt), this.size.labelHeight = s.height, this.fontOptions.minHgt > 0 && s.height < this.fontOptions.minHgt && (s.height = this.fontOptions.minHgt), this.lines = s.lines, this.lineCount = s.lines.length, this.size.width = s.width, this.size.height = s.height, this.selectedState = t, this.hoverState = i, this.labelDirty = !1
             }
             visible() {
                 return !(this.size.width === 0 || this.size.height === 0 || this.elementOptions.label === void 0 || this.fontOptions.size * this.body.view.scale < this.elementOptions.scaling.label.drawThreshold - 1)
             }
         },
-        De = class {
+        Ie = class {
             constructor(e, t, i) {
                 this.body = t, this.labelModule = i, this.setOptions(e), this.top = void 0, this.left = void 0, this.height = void 0, this.width = void 0, this.radius = void 0, this.margin = void 0, this.refreshNeeded = !0, this.boundingBox = {
                     top: 0,
                     left: 0,
                     right: 0,
                     bottom: 0
                 }
@@ -4956,15 +4956,15 @@
                     r = 14;
                 return s === 0 && (s = r, o = r), {
                     width: s,
                     height: o
                 }
             }
         },
-        ga = class extends De {
+        ga = class extends Ie {
             constructor(e, t, i) {
                 super(e, t, i);
                 this._setMargins(i)
             }
             resize(e, t = this.selected, i = this.hover) {
                 if (this.needsRefresh(t, i)) {
                     let s = this.getDimensionsFromLabel(e, t, i);
@@ -4981,15 +4981,15 @@
             }
             distanceToBorder(e, t) {
                 e && this.resize(e);
                 let i = this.options.borderWidth;
                 return Math.min(Math.abs(this.width / 2 / Math.cos(t)), Math.abs(this.height / 2 / Math.sin(t))) + i
             }
         },
-        Yt = class extends De {
+        Yt = class extends Ie {
             constructor(e, t, i) {
                 super(e, t, i);
                 this.labelOffset = 0, this.selected = !1
             }
             setOptions(e, t, i) {
                 this.options = e, t === void 0 && i === void 0 || this.setImages(t, i)
             }
@@ -5099,15 +5099,15 @@
             updateBoundingBox(e, t) {
                 this.options.shapeProperties.coordinateOrigin === "top-left" ? (this.boundingBox.top = t, this.boundingBox.left = e, this.boundingBox.right = e + this.options.size * 2, this.boundingBox.bottom = t + this.options.size * 2) : (this.boundingBox.top = t - this.options.size, this.boundingBox.left = e - this.options.size, this.boundingBox.right = e + this.options.size, this.boundingBox.bottom = t + this.options.size), this.boundingBox.left = Math.min(this.boundingBox.left, this.labelModule.size.left), this.boundingBox.right = Math.max(this.boundingBox.right, this.labelModule.size.left + this.labelModule.size.width), this.boundingBox.bottom = Math.max(this.boundingBox.bottom, this.boundingBox.bottom + this.labelOffset)
             }
             distanceToBorder(e) {
                 return e && this.resize(e), this.width * .5
             }
         },
-        Te = class extends De {
+        xe = class extends Ie {
             constructor(e, t, i) {
                 super(e, t, i)
             }
             resize(e, t = this.selected, i = this.hover, s = {
                 size: this.options.size
             }) {
                 var o, r;
@@ -5129,15 +5129,15 @@
                     }
                 }
             }
             updateBoundingBox(e, t) {
                 this.boundingBox.top = t - this.options.size, this.boundingBox.left = e - this.options.size, this.boundingBox.right = e + this.options.size, this.boundingBox.bottom = t + this.options.size, this.options.label !== void 0 && this.labelModule.size.width > 0 && (this.boundingBox.left = Math.min(this.boundingBox.left, this.labelModule.size.left), this.boundingBox.right = Math.max(this.boundingBox.right, this.labelModule.size.left + this.labelModule.size.width), this.boundingBox.bottom = Math.max(this.boundingBox.bottom, this.boundingBox.bottom + this.labelModule.size.height))
             }
         },
-        yo = class extends Te {
+        yo = class extends xe {
             constructor(e, t, i, s) {
                 super(e, t, i, s);
                 this.ctxRenderer = s
             }
             draw(e, t, i, s, o, r) {
                 this.resize(e, s, o, r), this.left = t - this.width / 2, this.top = i - this.height / 2, e.save();
                 let a = this.ctxRenderer({
@@ -5145,30 +5145,30 @@
                     id: this.options.id,
                     x: t,
                     y: i,
                     state: {
                         selected: s,
                         hover: o
                     },
-                    style: le({}, r),
+                    style: de({}, r),
                     label: this.options.label
                 });
                 if (a.drawNode != null && a.drawNode(), e.restore(), a.drawExternalLabel) {
                     let d = a.drawExternalLabel;
                     a.drawExternalLabel = () => {
                         e.save(), d(), e.restore()
                     }
                 }
                 return a.nodeDimensions && (this.customSizeWidth = a.nodeDimensions.width, this.customSizeHeight = a.nodeDimensions.height), a
             }
             distanceToBorder(e, t) {
                 return this._distanceToBorder(e, t)
             }
         },
-        bo = class extends De {
+        bo = class extends Ie {
             constructor(e, t, i) {
                 super(e, t, i);
                 this._setMargins(i)
             }
             resize(e, t, i) {
                 if (this.needsRefresh(t, i)) {
                     let o = this.getDimensionsFromLabel(e, t, i).width + this.margin.right + this.margin.left;
@@ -5178,37 +5178,37 @@
             draw(e, t, i, s, o, r) {
                 this.resize(e, s, o), this.left = t - this.width / 2, this.top = i - this.height / 2, this.initContextForDraw(e, r), $s(e, t - this.width / 2, i - this.height / 2, this.width, this.height), this.performFill(e, r), this.updateBoundingBox(t, i, e, s, o), this.labelModule.draw(e, this.left + this.textSize.width / 2 + this.margin.left, this.top + this.textSize.height / 2 + this.margin.top, s, o)
             }
             distanceToBorder(e, t) {
                 return this._distanceToBorder(e, t)
             }
         },
-        ya = class extends Te {
+        ya = class extends xe {
             constructor(e, t, i) {
                 super(e, t, i)
             }
             draw(e, t, i, s, o, r) {
                 return this._drawShape(e, "diamond", 4, t, i, s, o, r)
             }
             distanceToBorder(e, t) {
                 return this._distanceToBorder(e, t)
             }
         },
-        vo = class extends Te {
+        vo = class extends xe {
             constructor(e, t, i) {
                 super(e, t, i)
             }
             draw(e, t, i, s, o, r) {
                 return this._drawShape(e, "circle", 2, t, i, s, o, r)
             }
             distanceToBorder(e) {
                 return e && this.resize(e), this.options.size
             }
         },
-        Oi = class extends De {
+        Oi = class extends Ie {
             constructor(e, t, i) {
                 super(e, t, i)
             }
             resize(e, t = this.selected, i = this.hover) {
                 if (this.needsRefresh(t, i)) {
                     let s = this.getDimensionsFromLabel(e, t, i);
                     this.height = s.height * 2, this.width = s.width + s.height, this.radius = .5 * this.width
@@ -5222,15 +5222,15 @@
                 let i = this.width * .5,
                     s = this.height * .5,
                     o = Math.sin(t) * i,
                     r = Math.cos(t) * s;
                 return i * s / Math.sqrt(o * o + r * r)
             }
         },
-        wo = class extends De {
+        wo = class extends Ie {
             constructor(e, t, i) {
                 super(e, t, i);
                 this._setMargins(i)
             }
             resize(e, t, i) {
                 this.needsRefresh(t, i) && (this.iconSize = {
                     width: Number(this.options.icon.size),
@@ -5293,87 +5293,87 @@
             updateBoundingBox(e, t) {
                 this.resize(), this.options.shapeProperties.coordinateOrigin === "top-left" ? (this.left = e, this.top = t) : (this.left = e - this.width / 2, this.top = t - this.height / 2), this.boundingBox.left = this.left, this.boundingBox.top = this.top, this.boundingBox.bottom = this.top + this.height, this.boundingBox.right = this.left + this.width, this.options.label !== void 0 && this.labelModule.size.width > 0 && (this.boundingBox.left = Math.min(this.boundingBox.left, this.labelModule.size.left), this.boundingBox.right = Math.max(this.boundingBox.right, this.labelModule.size.left + this.labelModule.size.width), this.boundingBox.bottom = Math.max(this.boundingBox.bottom, this.boundingBox.bottom + this.labelOffset))
             }
             distanceToBorder(e, t) {
                 return this._distanceToBorder(e, t)
             }
         },
-        _o = class extends Te {
+        _o = class extends xe {
             constructor(e, t, i) {
                 super(e, t, i)
             }
             draw(e, t, i, s, o, r) {
                 return this._drawShape(e, "square", 2, t, i, s, o, r)
             }
             distanceToBorder(e, t) {
                 return this._distanceToBorder(e, t)
             }
         },
-        Eo = class extends Te {
+        Eo = class extends xe {
             constructor(e, t, i) {
                 super(e, t, i)
             }
             draw(e, t, i, s, o, r) {
                 return this._drawShape(e, "hexagon", 4, t, i, s, o, r)
             }
             distanceToBorder(e, t) {
                 return this._distanceToBorder(e, t)
             }
         },
-        xo = class extends Te {
+        xo = class extends xe {
             constructor(e, t, i) {
                 super(e, t, i)
             }
             draw(e, t, i, s, o, r) {
                 return this._drawShape(e, "star", 4, t, i, s, o, r)
             }
             distanceToBorder(e, t) {
                 return this._distanceToBorder(e, t)
             }
         },
-        Co = class extends De {
+        Co = class extends Ie {
             constructor(e, t, i) {
                 super(e, t, i);
                 this._setMargins(i)
             }
             resize(e, t, i) {
                 this.needsRefresh(t, i) && (this.textSize = this.labelModule.getTextSize(e, t, i), this.width = this.textSize.width + this.margin.right + this.margin.left, this.height = this.textSize.height + this.margin.top + this.margin.bottom, this.radius = .5 * this.width)
             }
             draw(e, t, i, s, o, r) {
                 this.resize(e, s, o), this.left = t - this.width / 2, this.top = i - this.height / 2, this.enableShadow(e, r), this.labelModule.draw(e, this.left + this.textSize.width / 2 + this.margin.left, this.top + this.textSize.height / 2 + this.margin.top, s, o), this.disableShadow(e, r), this.updateBoundingBox(t, i, e, s, o)
             }
             distanceToBorder(e, t) {
                 return this._distanceToBorder(e, t)
             }
         },
-        va = class extends Te {
+        va = class extends xe {
             constructor(e, t, i) {
                 super(e, t, i)
             }
             draw(e, t, i, s, o, r) {
                 return this._drawShape(e, "triangle", 3, t, i, s, o, r)
             }
             distanceToBorder(e, t) {
                 return this._distanceToBorder(e, t)
             }
         },
-        To = class extends Te {
+        To = class extends xe {
             constructor(e, t, i) {
                 super(e, t, i)
             }
             draw(e, t, i, s, o, r) {
                 return this._drawShape(e, "triangleDown", 3, t, i, s, o, r)
             }
             distanceToBorder(e, t) {
                 return this._distanceToBorder(e, t)
             }
         },
         z = class {
             constructor(e, t, i, s, o, r) {
-                this.options = _e(o), this.globalOptions = o, this.defaultOptions = r, this.body = t, this.edges = [], this.id = void 0, this.imagelist = i, this.grouplist = s, this.x = void 0, this.y = void 0, this.baseSize = this.options.size, this.baseFontSize = this.options.font.size, this.predefinedPosition = !1, this.selected = !1, this.hover = !1, this.labelModule = new Ye(this.body, this.options, !1), this.setOptions(e)
+                this.options = ve(o), this.globalOptions = o, this.defaultOptions = r, this.body = t, this.edges = [], this.id = void 0, this.imagelist = i, this.grouplist = s, this.x = void 0, this.y = void 0, this.baseSize = this.options.size, this.baseFontSize = this.options.font.size, this.predefinedPosition = !1, this.selected = !1, this.hover = !1, this.labelModule = new Ve(this.body, this.options, !1), this.setOptions(e)
             }
             attachEdge(e) {
                 this.edges.indexOf(e) === -1 && this.edges.push(e)
             }
             detachEdge(e) {
                 let t = this.edges.indexOf(e);
                 t != -1 && this.edges.splice(t, 1)
@@ -5407,22 +5407,22 @@
                 if (i === void 0) return;
                 let s = e.group;
                 if (t !== void 0 && t.group !== void 0 && s !== t.group) throw new Error("updateGroupOptions: group values in options don't match.");
                 if (!(typeof s == "number" || typeof s == "string" && s != "")) return;
                 let r = i.get(s);
                 r.opacity !== void 0 && t.opacity === void 0 && (z.checkOpacity(r.opacity) || (console.error("Invalid option for node opacity. Value must be between 0 and 1, found: " + r.opacity), r.opacity = void 0));
                 let a = Object.getOwnPropertyNames(t).filter(d => t[d] != null);
-                a.push("font"), bt(a, e, r), e.color = zt(e.color)
+                a.push("font"), yt(a, e, r), e.color = zt(e.color)
             }
             static parseOptions(e, t, i = !1, s = {}, o) {
-                if (bt(["color", "fixed", "shadow"], e, t, i), z.checkMass(t), e.opacity !== void 0 && (z.checkOpacity(e.opacity) || (console.error("Invalid option for node opacity. Value must be between 0 and 1, found: " + e.opacity), e.opacity = void 0)), t.opacity !== void 0 && (z.checkOpacity(t.opacity) || (console.error("Invalid option for node opacity. Value must be between 0 and 1, found: " + t.opacity), t.opacity = void 0)), t.shapeProperties && !z.checkCoordinateOrigin(t.shapeProperties.coordinateOrigin) && console.error("Invalid option for node coordinateOrigin, found: " + t.shapeProperties.coordinateOrigin), se(e, t, "shadow", s), t.color !== void 0 && t.color !== null) {
+                if (yt(["color", "fixed", "shadow"], e, t, i), z.checkMass(t), e.opacity !== void 0 && (z.checkOpacity(e.opacity) || (console.error("Invalid option for node opacity. Value must be between 0 and 1, found: " + e.opacity), e.opacity = void 0)), t.opacity !== void 0 && (z.checkOpacity(t.opacity) || (console.error("Invalid option for node opacity. Value must be between 0 and 1, found: " + t.opacity), t.opacity = void 0)), t.shapeProperties && !z.checkCoordinateOrigin(t.shapeProperties.coordinateOrigin) && console.error("Invalid option for node coordinateOrigin, found: " + t.shapeProperties.coordinateOrigin), se(e, t, "shadow", s), t.color !== void 0 && t.color !== null) {
                     let a = zt(t.color);
                     fi(e.color, a)
-                } else i === !0 && t.color === null && (e.color = _e(s.color));
-                t.fixed !== void 0 && t.fixed !== null && (typeof t.fixed == "boolean" ? (e.fixed.x = t.fixed, e.fixed.y = t.fixed) : (t.fixed.x !== void 0 && typeof t.fixed.x == "boolean" && (e.fixed.x = t.fixed.x), t.fixed.y !== void 0 && typeof t.fixed.y == "boolean" && (e.fixed.y = t.fixed.y))), i === !0 && t.font === null && (e.font = _e(s.font)), z.updateGroupOptions(e, t, o), t.scaling !== void 0 && se(e.scaling, t.scaling, "label", s.scaling)
+                } else i === !0 && t.color === null && (e.color = ve(s.color));
+                t.fixed !== void 0 && t.fixed !== null && (typeof t.fixed == "boolean" ? (e.fixed.x = t.fixed, e.fixed.y = t.fixed) : (t.fixed.x !== void 0 && typeof t.fixed.x == "boolean" && (e.fixed.x = t.fixed.x), t.fixed.y !== void 0 && typeof t.fixed.y == "boolean" && (e.fixed.y = t.fixed.y))), i === !0 && t.font === null && (e.font = ve(s.font)), z.updateGroupOptions(e, t, o), t.scaling !== void 0 && se(e.scaling, t.scaling, "label", s.scaling)
             }
             getFormattingValues() {
                 let e = {
                     color: this.options.color.background,
                     opacity: this.options.opacity,
                     borderWidth: this.options.borderWidth,
                     borderColor: this.options.color.border,
@@ -5438,15 +5438,15 @@
                 if (this.selected || this.hover ? this.chooser === !0 ? this.selected ? (this.options.borderWidthSelected != null ? e.borderWidth = this.options.borderWidthSelected : e.borderWidth *= 2, e.color = this.options.color.highlight.background, e.borderColor = this.options.color.highlight.border, e.shadow = this.options.shadow.enabled) : this.hover && (e.color = this.options.color.hover.background, e.borderColor = this.options.color.hover.border, e.shadow = this.options.shadow.enabled) : typeof this.chooser == "function" && (this.chooser(e, this.options.id, this.selected, this.hover), e.shadow === !1 && (e.shadowColor !== this.options.shadow.color || e.shadowSize !== this.options.shadow.size || e.shadowX !== this.options.shadow.x || e.shadowY !== this.options.shadow.y) && (e.shadow = !0)) : e.shadow = this.options.shadow.enabled, this.options.opacity !== void 0) {
                     let t = this.options.opacity;
                     e.borderColor = ie(e.borderColor, t), e.color = ie(e.color, t), e.shadowColor = ie(e.shadowColor, t)
                 }
                 return e
             }
             updateLabelModule(e) {
-                (this.options.label === void 0 || this.options.label === null) && (this.options.label = ""), z.updateGroupOptions(this.options, Be(le({}, e), {
+                (this.options.label === void 0 || this.options.label === null) && (this.options.label = ""), z.updateGroupOptions(this.options, Me(de({}, e), {
                     color: e && e.color || this._localColor || void 0
                 }), this.grouplist);
                 let t = this.grouplist.get(this.options.group, !1),
                     i = [e, this.options, t, this.globalOptions, this.defaultOptions];
                 this.labelModule.update(this.options, i), this.labelModule.baseSize !== void 0 && (this.baseFontSize = this.labelModule.baseSize)
             }
             updateShape(e) {
@@ -5699,15 +5699,15 @@
                         },
                         size: 25,
                         title: void 0,
                         value: void 0,
                         x: void 0,
                         y: void 0
                     }, this.defaultOptions.mass <= 0) throw "Internal error: mass in defaultOptions of NodesHandler may not be zero or negative";
-                this.options = _e(this.defaultOptions), this.bindEventListeners()
+                this.options = ve(this.defaultOptions), this.bindEventListeners()
             }
             bindEventListeners() {
                 this.body.emitter.on("refreshNodes", this.refresh.bind(this)), this.body.emitter.on("refresh", this.refresh.bind(this)), this.body.emitter.on("destroy", () => {
                     I(this.nodesListeners, (e, t) => {
                         this.body.data.nodes && this.body.data.nodes.off(t, e)
                     }), delete this.body.functions.createNode, delete this.nodesListeners.add, delete this.nodesListeners.update, delete this.nodesListeners.remove, delete this.nodesListeners
                 })
@@ -5722,16 +5722,16 @@
                         for (let t in this.body.nodes) Object.prototype.hasOwnProperty.call(this.body.nodes, t) && this.body.nodes[t].needsRefresh();
                     (e.hidden !== void 0 || e.physics !== void 0) && this.body.emitter.emit("_dataChanged")
                 }
             }
             setData(e, t = !1) {
                 let i = this.body.data.nodes;
                 if (vi("id", e)) this.body.data.nodes = e;
-                else if (Array.isArray(e)) this.body.data.nodes = new Ce, this.body.data.nodes.add(e);
-                else if (!e) this.body.data.nodes = new Ce;
+                else if (Array.isArray(e)) this.body.data.nodes = new Ee, this.body.data.nodes.add(e);
+                else if (!e) this.body.data.nodes = new Ee;
                 else throw new TypeError("Array or DataSet expected");
                 if (i && I(this.nodesListeners, function(s, o) {
                         i.off(o, s)
                     }), this.body.nodes = {}, this.body.data.nodes) {
                     let s = this;
                     I(this.nodesListeners, function(r, a) {
                         s.body.data.nodes.on(a, r)
@@ -5864,15 +5864,15 @@
             }
             moveNode(e, t, i) {
                 this.body.nodes[e] !== void 0 ? (this.body.nodes[e].x = Number(t), this.body.nodes[e].y = Number(i), setTimeout(() => {
                     this.body.emitter.emit("startSimulation")
                 }, 0)) : console.error("Node id supplied to moveNode does not exist. Provided: ", e)
             }
         },
-        H = class {
+        L = class {
             static transform(e, t) {
                 Array.isArray(e) || (e = [e]);
                 let i = t.point.x,
                     s = t.point.y,
                     o = t.angle,
                     r = t.length;
                 for (let a = 0; a < e.length; ++a) {
@@ -5884,41 +5884,41 @@
             }
             static drawPath(e, t) {
                 e.beginPath(), e.moveTo(t[0].x, t[0].y);
                 for (let i = 1; i < t.length; ++i) e.lineTo(t[i].x, t[i].y);
                 e.closePath()
             }
         },
-        wa = class extends H {
+        wa = class extends L {
             static draw(e, t) {
                 if (t.image) {
                     e.save(), e.translate(t.point.x, t.point.y), e.rotate(Math.PI / 2 + t.angle);
                     let i = t.imageWidth != null ? t.imageWidth : t.image.width,
                         s = t.imageHeight != null ? t.imageHeight : t.image.height;
                     t.image.drawImageAtPosition(e, 1, -i / 2, 0, i, s), e.restore()
                 }
                 return !1
             }
         },
-        Oo = class extends H {
+        Oo = class extends L {
             static draw(e, t) {
                 let i = [{
                     x: 0,
                     y: 0
                 }, {
                     x: -1,
                     y: .3
                 }, {
                     x: -.9,
                     y: 0
                 }, {
                     x: -1,
                     y: -.3
                 }];
-                return H.transform(i, t), H.drawPath(e, i), !0
+                return L.transform(i, t), L.drawPath(e, i), !0
             }
         },
         So = class {
             static draw(e, t) {
                 let i = [{
                     x: -1,
                     y: 0
@@ -5928,80 +5928,80 @@
                 }, {
                     x: -.4,
                     y: 0
                 }, {
                     x: 0,
                     y: -.3
                 }];
-                return H.transform(i, t), H.drawPath(e, i), !0
+                return L.transform(i, t), L.drawPath(e, i), !0
             }
         },
         Io = class {
             static draw(e, t) {
                 let i = {
                     x: -.4,
                     y: 0
                 };
-                H.transform(i, t), e.strokeStyle = e.fillStyle, e.fillStyle = "rgba(0, 0, 0, 0)";
+                L.transform(i, t), e.strokeStyle = e.fillStyle, e.fillStyle = "rgba(0, 0, 0, 0)";
                 let s = Math.PI,
                     o = t.angle - s / 2,
                     r = t.angle + s / 2;
                 return e.beginPath(), e.arc(i.x, i.y, t.length * .4, o, r, !1), e.stroke(), !0
             }
         },
         Po = class {
             static draw(e, t) {
                 let i = {
                     x: -.3,
                     y: 0
                 };
-                H.transform(i, t), e.strokeStyle = e.fillStyle, e.fillStyle = "rgba(0, 0, 0, 0)";
+                L.transform(i, t), e.strokeStyle = e.fillStyle, e.fillStyle = "rgba(0, 0, 0, 0)";
                 let s = Math.PI,
                     o = t.angle + s / 2,
                     r = t.angle + 3 * s / 2;
                 return e.beginPath(), e.arc(i.x, i.y, t.length * .4, o, r, !1), e.stroke(), !0
             }
         },
-        Mo = class {
+        Do = class {
             static draw(e, t) {
                 let i = [{
                     x: .02,
                     y: 0
                 }, {
                     x: -1,
                     y: .3
                 }, {
                     x: -1,
                     y: -.3
                 }];
-                return H.transform(i, t), H.drawPath(e, i), !0
+                return L.transform(i, t), L.drawPath(e, i), !0
             }
         },
-        Do = class {
+        Mo = class {
             static draw(e, t) {
                 let i = [{
                     x: 0,
                     y: .3
                 }, {
                     x: 0,
                     y: -.3
                 }, {
                     x: -1,
                     y: 0
                 }];
-                return H.transform(i, t), H.drawPath(e, i), !0
+                return L.transform(i, t), L.drawPath(e, i), !0
             }
         },
         Fo = class {
             static draw(e, t) {
                 let i = {
                     x: -.4,
                     y: 0
                 };
-                return H.transform(i, t), wi(e, i.x, i.y, t.length * .4), !0
+                return L.transform(i, t), wi(e, i.x, i.y, t.length * .4), !0
             }
         },
         No = class {
             static draw(e, t) {
                 let i = [{
                     x: 0,
                     y: .5
@@ -6011,15 +6011,15 @@
                 }, {
                     x: -.15,
                     y: -.5
                 }, {
                     x: -.15,
                     y: .5
                 }];
-                return H.transform(i, t), H.drawPath(e, i), !0
+                return L.transform(i, t), L.drawPath(e, i), !0
             }
         },
         Bo = class {
             static draw(e, t) {
                 let i = [{
                     x: 0,
                     y: .3
@@ -6029,15 +6029,15 @@
                 }, {
                     x: -.6,
                     y: -.3
                 }, {
                     x: -.6,
                     y: .3
                 }];
-                return H.transform(i, t), H.drawPath(e, i), !0
+                return L.transform(i, t), L.drawPath(e, i), !0
             }
         },
         Ao = class {
             static draw(e, t) {
                 let i = [{
                     x: 0,
                     y: 0
@@ -6047,15 +6047,15 @@
                 }, {
                     x: -1,
                     y: 0
                 }, {
                     x: -.5,
                     y: .3
                 }];
-                return H.transform(i, t), H.drawPath(e, i), !0
+                return L.transform(i, t), L.drawPath(e, i), !0
             }
         },
         zo = class {
             static draw(e, t) {
                 let i = [{
                     x: -1,
                     y: .3
@@ -6065,15 +6065,15 @@
                 }, {
                     x: -1,
                     y: -.3
                 }, {
                     x: 0,
                     y: 0
                 }];
-                return H.transform(i, t), H.drawPath(e, i), !0
+                return L.transform(i, t), L.drawPath(e, i), !0
             }
         },
         Si = class {
             static draw(e, t) {
                 let i;
                 switch (t.type && (i = t.type.toLowerCase()), i) {
                     case "image":
@@ -6087,17 +6087,17 @@
                     case "curve":
                         return Io.draw(e, t);
                     case "diamond":
                         return Ao.draw(e, t);
                     case "inv_curve":
                         return Po.draw(e, t);
                     case "triangle":
-                        return Mo.draw(e, t);
-                    case "inv_triangle":
                         return Do.draw(e, t);
+                    case "inv_triangle":
+                        return Mo.draw(e, t);
                     case "bar":
                         return No.draw(e, t);
                     case "vee":
                         return zo.draw(e, t);
                     case "arrow":
                     default:
                         return Oo.draw(e, t)
@@ -6193,27 +6193,27 @@
                     r = i.low,
                     a = i.high,
                     d = i.direction,
                     h = 10,
                     l = this.options.selfReference.size,
                     c = .05,
                     u, f = (r + a) * .5,
-                    y = 0;
-                this.options.arrowStrikethrough === !0 && (d === -1 ? y = this.options.endPointOffset.from : d === 1 && (y = this.options.endPointOffset.to));
-                let v = 0;
+                    m = 0;
+                this.options.arrowStrikethrough === !0 && (d === -1 ? m = this.options.endPointOffset.from : d === 1 && (m = this.options.endPointOffset.to));
+                let b = 0;
                 do {
                     f = (r + a) * .5, u = this._pointOnCircle(s, o, l, f);
-                    let g = Math.atan2(e.y - u.y, e.x - u.x),
-                        p = e.distanceToBorder(t, g) + y,
-                        b = Math.sqrt(Math.pow(u.x - e.x, 2) + Math.pow(u.y - e.y, 2)),
-                        _ = p - b;
-                    if (Math.abs(_) < c) break;
-                    _ > 0 ? d > 0 ? r = f : a = f : d > 0 ? a = f : r = f, ++v
-                } while (r <= a && v < h);
-                return Be(le({}, u), {
+                    let p = Math.atan2(e.y - u.y, e.x - u.x),
+                        y = e.distanceToBorder(t, p) + m,
+                        _ = Math.sqrt(Math.pow(u.x - e.x, 2) + Math.pow(u.y - e.y, 2)),
+                        x = y - _;
+                    if (Math.abs(x) < c) break;
+                    x > 0 ? d > 0 ? r = f : a = f : d > 0 ? a = f : r = f, ++b
+                } while (r <= a && b < h);
+                return Me(de({}, u), {
                     t: f
                 })
             }
             getLineWidth(e, t) {
                 return e === !0 ? Math.max(this.selectionWidth, .3 / this._body.view.scale) : t === !0 ? Math.max(this.hoverWidth, .3 / this._body.view.scale) : Math.max(this.options.width, .3 / this._body.view.scale)
             }
             getColor(e, t) {
@@ -6264,77 +6264,77 @@
                     d = s - t,
                     h = a * a + d * d,
                     l = ((o - e) * a + (r - t) * d) / h;
                 l > 1 ? l = 1 : l < 0 && (l = 0);
                 let c = e + l * a,
                     u = t + l * d,
                     f = c - o,
-                    y = u - r;
-                return Math.sqrt(f * f + y * y)
+                    m = u - r;
+                return Math.sqrt(f * f + m * m)
             }
             getArrowData(e, t, i, s, o, r) {
-                let a, d, h, l, c, u, f, y = r.width;
+                let a, d, h, l, c, u, f, m = r.width;
                 t === "from" ? (h = this.from, l = this.to, c = r.fromArrowScale < 0, u = Math.abs(r.fromArrowScale), f = r.fromArrowType) : t === "to" ? (h = this.to, l = this.from, c = r.toArrowScale < 0, u = Math.abs(r.toArrowScale), f = r.toArrowType) : (h = this.to, l = this.from, c = r.middleArrowScale < 0, u = Math.abs(r.middleArrowScale), f = r.middleArrowType);
-                let v = 15 * u + 3 * y;
+                let b = 15 * u + 3 * m;
                 if (h != l) {
-                    let _ = Math.hypot(h.x - l.x, h.y - l.y),
-                        C = v / _;
+                    let x = Math.hypot(h.x - l.x, h.y - l.y),
+                        T = b / x;
                     if (t !== "middle")
                         if (this.options.smooth.enabled === !0) {
-                            let x = this._findBorderPosition(h, e, {
+                            let O = this._findBorderPosition(h, e, {
                                     via: i
                                 }),
-                                O = this.getPoint(x.t + C * (t === "from" ? 1 : -1), i);
-                            a = Math.atan2(x.y - O.y, x.x - O.x), d = x
+                                S = this.getPoint(O.t + T * (t === "from" ? 1 : -1), i);
+                            a = Math.atan2(O.y - S.y, O.x - S.x), d = O
                         } else a = Math.atan2(h.y - l.y, h.x - l.x), d = this._findBorderPosition(h, e);
                     else {
-                        let x = (c ? -C : C) / 2,
-                            O = this.getPoint(.5 + x, i),
-                            M = this.getPoint(.5 - x, i);
-                        a = Math.atan2(O.y - M.y, O.x - M.x), d = this.getPoint(.5, i)
+                        let O = (c ? -T : T) / 2,
+                            S = this.getPoint(.5 + O, i),
+                            A = this.getPoint(.5 - O, i);
+                        a = Math.atan2(S.y - A.y, S.x - A.x), d = this.getPoint(.5, i)
                     }
                 } else {
-                    let [_, C, x] = this._getCircleData(e);
+                    let [x, T, O] = this._getCircleData(e);
                     if (t === "from") {
-                        let O = this.options.selfReference.angle,
-                            M = this.options.selfReference.angle + Math.PI,
-                            R = this._findBorderPositionCircle(this.from, e, {
-                                x: _,
-                                y: C,
-                                low: O,
-                                high: M,
+                        let S = this.options.selfReference.angle,
+                            A = this.options.selfReference.angle + Math.PI,
+                            H = this._findBorderPositionCircle(this.from, e, {
+                                x,
+                                y: T,
+                                low: S,
+                                high: A,
                                 direction: -1
                             });
-                        a = R.t * -2 * Math.PI + 1.5 * Math.PI + .1 * Math.PI, d = R
+                        a = H.t * -2 * Math.PI + 1.5 * Math.PI + .1 * Math.PI, d = H
                     } else if (t === "to") {
-                        let O = this.options.selfReference.angle,
-                            M = this.options.selfReference.angle + Math.PI,
-                            R = this._findBorderPositionCircle(this.from, e, {
-                                x: _,
-                                y: C,
-                                low: O,
-                                high: M,
+                        let S = this.options.selfReference.angle,
+                            A = this.options.selfReference.angle + Math.PI,
+                            H = this._findBorderPositionCircle(this.from, e, {
+                                x,
+                                y: T,
+                                low: S,
+                                high: A,
                                 direction: 1
                             });
-                        a = R.t * -2 * Math.PI + 1.5 * Math.PI - 1.1 * Math.PI, d = R
+                        a = H.t * -2 * Math.PI + 1.5 * Math.PI - 1.1 * Math.PI, d = H
                     } else {
-                        let O = this.options.selfReference.angle / (2 * Math.PI);
-                        d = this._pointOnCircle(_, C, x, O), a = O * -2 * Math.PI + 1.5 * Math.PI + .1 * Math.PI
+                        let S = this.options.selfReference.angle / (2 * Math.PI);
+                        d = this._pointOnCircle(x, T, O, S), a = S * -2 * Math.PI + 1.5 * Math.PI + .1 * Math.PI
                     }
                 }
-                let g = d.x - v * .9 * Math.cos(a),
-                    p = d.y - v * .9 * Math.sin(a);
+                let p = d.x - b * .9 * Math.cos(a),
+                    y = d.y - b * .9 * Math.sin(a);
                 return {
                     point: d,
                     core: {
-                        x: g,
-                        y: p
+                        x: p,
+                        y
                     },
                     angle: a,
-                    length: v,
+                    length: b,
                     type: f
                 }
             }
             drawArrowHead(e, t, i, s, o) {
                 e.strokeStyle = this.getColor(e, t), e.fillStyle = e.strokeStyle, e.lineWidth = t.width, Si.draw(e, o) && (this.enableShadow(e, t), e.fill(), this.disableShadow(e, t))
             }
             enableShadow(e, t) {
@@ -6374,30 +6374,30 @@
                     d = 0,
                     h = this.to,
                     l, c, u = this.options.endPointOffset ? this.options.endPointOffset.to : 0;
                 e.id === this.from.id && (h = this.from, r = !0, u = this.options.endPointOffset ? this.options.endPointOffset.from : 0), this.options.arrowStrikethrough === !1 && (u = 0);
                 let f = 0;
                 do {
                     c = (d + a) * .5, l = this.getPoint(c, i);
-                    let y = Math.atan2(h.y - l.y, h.x - l.x),
-                        v = h.distanceToBorder(t, y) + u,
-                        g = Math.sqrt(Math.pow(l.x - h.x, 2) + Math.pow(l.y - h.y, 2)),
-                        p = v - g;
-                    if (Math.abs(p) < o) break;
-                    p < 0 ? r === !1 ? d = c : a = c : r === !1 ? a = c : d = c, ++f
+                    let m = Math.atan2(h.y - l.y, h.x - l.x),
+                        b = h.distanceToBorder(t, m) + u,
+                        p = Math.sqrt(Math.pow(l.x - h.x, 2) + Math.pow(l.y - h.y, 2)),
+                        y = b - p;
+                    if (Math.abs(y) < o) break;
+                    y < 0 ? r === !1 ? d = c : a = c : r === !1 ? a = c : d = c, ++f
                 } while (d <= a && f < s);
-                return Be(le({}, l), {
+                return Me(de({}, l), {
                     t: c
                 })
             }
             _getDistanceToBezierEdge(e, t, i, s, o, r, a) {
                 let d = 1e9,
-                    h, l, c, u, f, y = e,
-                    v = t;
-                for (l = 1; l < 10; l++) c = .1 * l, u = Math.pow(1 - c, 2) * e + 2 * c * (1 - c) * a.x + Math.pow(c, 2) * i, f = Math.pow(1 - c, 2) * t + 2 * c * (1 - c) * a.y + Math.pow(c, 2) * s, l > 0 && (h = this._getDistanceToLine(y, v, u, f, o, r), d = h < d ? h : d), y = u, v = f;
+                    h, l, c, u, f, m = e,
+                    b = t;
+                for (l = 1; l < 10; l++) c = .1 * l, u = Math.pow(1 - c, 2) * e + 2 * c * (1 - c) * a.x + Math.pow(c, 2) * i, f = Math.pow(1 - c, 2) * t + 2 * c * (1 - c) * a.y + Math.pow(c, 2) * s, l > 0 && (h = this._getDistanceToLine(m, b, u, f, o, r), d = h < d ? h : d), m = u, b = f;
                 return d
             }
             _bezierCurve(e, t, i, s) {
                 e.beginPath(), e.moveTo(this.fromPoint.x, this.fromPoint.y), i != null && i.x != null ? s != null && s.x != null ? e.bezierCurveTo(i.x, i.y, s.x, s.y, this.toPoint.x, this.toPoint.y) : e.quadraticCurveTo(i.x, i.y, this.toPoint.x, this.toPoint.y) : e.lineTo(this.toPoint.x, this.toPoint.y), this.drawBackground(e, t), this.enableShadow(e, t), e.stroke(), this.disableShadow(e, t)
             }
             getViaNode() {
                 return this._getViaCoordinates()
@@ -6468,15 +6468,15 @@
             _findBorderPosition(e, t) {
                 return this._findBorderPositionBezier(e, t, this.via)
             }
             _getDistanceToEdge(e, t, i, s, o, r) {
                 return this._getDistanceToBezierEdge(e, t, i, s, o, r, this.via)
             }
         },
-        Mi = class extends Xt {
+        Di = class extends Xt {
             constructor(e, t, i) {
                 super(e, t, i)
             }
             _line(e, t, i) {
                 this._bezierCurve(e, t, i)
             }
             getViaNode() {
@@ -6566,28 +6566,28 @@
             }
             _getDistanceToBezierEdge2(e, t, i, s, o, r, a, d) {
                 let h = 1e9,
                     l = e,
                     c = t,
                     u = [0, 0, 0, 0];
                 for (let f = 1; f < 10; f++) {
-                    let y = .1 * f;
-                    u[0] = Math.pow(1 - y, 3), u[1] = 3 * y * Math.pow(1 - y, 2), u[2] = 3 * Math.pow(y, 2) * (1 - y), u[3] = Math.pow(y, 3);
-                    let v = u[0] * e + u[1] * a.x + u[2] * d.x + u[3] * i,
-                        g = u[0] * t + u[1] * a.y + u[2] * d.y + u[3] * s;
+                    let m = .1 * f;
+                    u[0] = Math.pow(1 - m, 3), u[1] = 3 * m * Math.pow(1 - m, 2), u[2] = 3 * Math.pow(m, 2) * (1 - m), u[3] = Math.pow(m, 3);
+                    let b = u[0] * e + u[1] * a.x + u[2] * d.x + u[3] * i,
+                        p = u[0] * t + u[1] * a.y + u[2] * d.y + u[3] * s;
                     if (f > 0) {
-                        let p = this._getDistanceToLine(l, c, v, g, o, r);
-                        h = p < h ? p : h
+                        let y = this._getDistanceToLine(l, c, b, p, o, r);
+                        h = y < h ? y : h
                     }
-                    l = v, c = g
+                    l = b, c = p
                 }
                 return h
             }
         },
-        Di = class extends Ro {
+        Mi = class extends Ro {
             constructor(e, t, i) {
                 super(e, t, i)
             }
             _line(e, t, i) {
                 let s = i[0],
                     o = i[1];
                 this._bezierCurve(e, t, s, o)
@@ -6654,53 +6654,53 @@
                     t: 0
                 }
             }
             _getDistanceToEdge(e, t, i, s, o, r) {
                 return this._getDistanceToLine(e, t, i, s, o, r)
             }
         },
-        ke = class {
+        Ce = class {
             constructor(e, t, i, s, o) {
                 if (t === void 0) throw new Error("No body provided");
-                this.options = _e(s), this.globalOptions = s, this.defaultOptions = o, this.body = t, this.imagelist = i, this.id = void 0, this.fromId = void 0, this.toId = void 0, this.selected = !1, this.hover = !1, this.labelDirty = !0, this.baseWidth = this.options.width, this.baseFontSize = this.options.font.size, this.from = void 0, this.to = void 0, this.edgeType = void 0, this.connected = !1, this.labelModule = new Ye(this.body, this.options, !0), this.setOptions(e)
+                this.options = ve(s), this.globalOptions = s, this.defaultOptions = o, this.body = t, this.imagelist = i, this.id = void 0, this.fromId = void 0, this.toId = void 0, this.selected = !1, this.hover = !1, this.labelDirty = !0, this.baseWidth = this.options.width, this.baseFontSize = this.options.font.size, this.from = void 0, this.to = void 0, this.edgeType = void 0, this.connected = !1, this.labelModule = new Ve(this.body, this.options, !0), this.setOptions(e)
             }
             setOptions(e) {
                 if (!e) return;
                 let t = typeof e.physics != "undefined" && this.options.physics !== e.physics || typeof e.hidden != "undefined" && (this.options.hidden || !1) !== (e.hidden || !1) || typeof e.from != "undefined" && this.options.from !== e.from || typeof e.to != "undefined" && this.options.to !== e.to;
-                ke.parseOptions(this.options, e, !0, this.globalOptions), e.id !== void 0 && (this.id = e.id), e.from !== void 0 && (this.fromId = e.from), e.to !== void 0 && (this.toId = e.to), e.title !== void 0 && (this.title = e.title), e.value !== void 0 && (e.value = parseFloat(e.value));
+                Ce.parseOptions(this.options, e, !0, this.globalOptions), e.id !== void 0 && (this.id = e.id), e.from !== void 0 && (this.fromId = e.from), e.to !== void 0 && (this.toId = e.to), e.title !== void 0 && (this.title = e.title), e.value !== void 0 && (e.value = parseFloat(e.value));
                 let i = [e, this.options, this.defaultOptions];
                 return this.chooser = Ci("edge", i), this.updateLabelModule(e), t = this.updateEdgeType() || t, this._setInteractionWidths(), this.connect(), t
             }
             static parseOptions(e, t, i = !1, s = {}, o = !1) {
-                if (qe(["endPointOffset", "arrowStrikethrough", "id", "from", "hidden", "hoverWidth", "labelHighlightBold", "length", "line", "opacity", "physics", "scaling", "selectionWidth", "selfReferenceSize", "selfReference", "to", "title", "value", "width", "font", "chosen", "widthConstraint"], e, t, i), t.endPointOffset !== void 0 && t.endPointOffset.from !== void 0 && (Number.isFinite(t.endPointOffset.from) ? e.endPointOffset.from = t.endPointOffset.from : (e.endPointOffset.from = s.endPointOffset.from !== void 0 ? s.endPointOffset.from : 0, console.error("endPointOffset.from is not a valid number"))), t.endPointOffset !== void 0 && t.endPointOffset.to !== void 0 && (Number.isFinite(t.endPointOffset.to) ? e.endPointOffset.to = t.endPointOffset.to : (e.endPointOffset.to = s.endPointOffset.to !== void 0 ? s.endPointOffset.to : 0, console.error("endPointOffset.to is not a valid number"))), qt(t.label) ? e.label = t.label : qt(e.label) || (e.label = void 0), se(e, t, "smooth", s), se(e, t, "shadow", s), se(e, t, "background", s), t.dashes !== void 0 && t.dashes !== null ? e.dashes = t.dashes : i === !0 && t.dashes === null && (e.dashes = Object.create(s.dashes)), t.scaling !== void 0 && t.scaling !== null ? (t.scaling.min !== void 0 && (e.scaling.min = t.scaling.min), t.scaling.max !== void 0 && (e.scaling.max = t.scaling.max), se(e.scaling, t.scaling, "label", s.scaling)) : i === !0 && t.scaling === null && (e.scaling = Object.create(s.scaling)), t.arrows !== void 0 && t.arrows !== null)
+                if (je(["endPointOffset", "arrowStrikethrough", "id", "from", "hidden", "hoverWidth", "labelHighlightBold", "length", "line", "opacity", "physics", "scaling", "selectionWidth", "selfReferenceSize", "selfReference", "to", "title", "value", "width", "font", "chosen", "widthConstraint"], e, t, i), t.endPointOffset !== void 0 && t.endPointOffset.from !== void 0 && (Number.isFinite(t.endPointOffset.from) ? e.endPointOffset.from = t.endPointOffset.from : (e.endPointOffset.from = s.endPointOffset.from !== void 0 ? s.endPointOffset.from : 0, console.error("endPointOffset.from is not a valid number"))), t.endPointOffset !== void 0 && t.endPointOffset.to !== void 0 && (Number.isFinite(t.endPointOffset.to) ? e.endPointOffset.to = t.endPointOffset.to : (e.endPointOffset.to = s.endPointOffset.to !== void 0 ? s.endPointOffset.to : 0, console.error("endPointOffset.to is not a valid number"))), qt(t.label) ? e.label = t.label : qt(e.label) || (e.label = void 0), se(e, t, "smooth", s), se(e, t, "shadow", s), se(e, t, "background", s), t.dashes !== void 0 && t.dashes !== null ? e.dashes = t.dashes : i === !0 && t.dashes === null && (e.dashes = Object.create(s.dashes)), t.scaling !== void 0 && t.scaling !== null ? (t.scaling.min !== void 0 && (e.scaling.min = t.scaling.min), t.scaling.max !== void 0 && (e.scaling.max = t.scaling.max), se(e.scaling, t.scaling, "label", s.scaling)) : i === !0 && t.scaling === null && (e.scaling = Object.create(s.scaling)), t.arrows !== void 0 && t.arrows !== null)
                     if (typeof t.arrows == "string") {
                         let a = t.arrows.toLowerCase();
                         e.arrows.to.enabled = a.indexOf("to") != -1, e.arrows.middle.enabled = a.indexOf("middle") != -1, e.arrows.from.enabled = a.indexOf("from") != -1
                     } else if (typeof t.arrows == "object") se(e.arrows, t.arrows, "to", s.arrows), se(e.arrows, t.arrows, "middle", s.arrows), se(e.arrows, t.arrows, "from", s.arrows);
                 else throw new Error("The arrow newOptions can only be an object or a string. Refer to the documentation. You used:" + JSON.stringify(t.arrows));
                 else i === !0 && t.arrows === null && (e.arrows = Object.create(s.arrows));
                 if (t.color !== void 0 && t.color !== null) {
-                    let a = we(t.color) ? {
+                    let a = be(t.color) ? {
                             color: t.color,
                             highlight: t.color,
                             hover: t.color,
                             inherit: !1,
                             opacity: 1
                         } : t.color,
                         d = e.color;
                     if (o) D(d, s.color, !1, i);
                     else
                         for (let h in d) Object.prototype.hasOwnProperty.call(d, h) && delete d[h];
-                    if (we(d)) d.color = d, d.highlight = d, d.hover = d, d.inherit = !1, a.opacity === void 0 && (d.opacity = 1);
+                    if (be(d)) d.color = d, d.highlight = d, d.hover = d, d.inherit = !1, a.opacity === void 0 && (d.opacity = 1);
                     else {
                         let h = !1;
                         a.color !== void 0 && (d.color = a.color, h = !0), a.highlight !== void 0 && (d.highlight = a.highlight, h = !0), a.hover !== void 0 && (d.hover = a.hover, h = !0), a.inherit !== void 0 && (d.inherit = a.inherit), a.opacity !== void 0 && (d.opacity = Math.min(1, Math.max(0, a.opacity))), h === !0 ? d.inherit = !1 : d.inherit === void 0 && (d.inherit = "from")
                     }
-                } else i === !0 && t.color === null && (e.color = _e(s.color));
-                i === !0 && t.font === null && (e.font = _e(s.font)), Object.prototype.hasOwnProperty.call(t, "selfReferenceSize") && (console.warn("The selfReferenceSize property has been deprecated. Please use selfReference property instead. The selfReference can be set like thise selfReference:{size:30, angle:Math.PI / 4}"), e.selfReference.size = t.selfReferenceSize)
+                } else i === !0 && t.color === null && (e.color = ve(s.color));
+                i === !0 && t.font === null && (e.font = ve(s.font)), Object.prototype.hasOwnProperty.call(t, "selfReferenceSize") && (console.warn("The selfReferenceSize property has been deprecated. Please use selfReference property instead. The selfReference can be set like thise selfReference:{size:30, angle:Math.PI / 4}"), e.selfReference.size = t.selfReferenceSize)
             }
             getFormattingValues() {
                 let e = this.options.arrows.to === !0 || this.options.arrows.to.enabled === !0,
                     t = this.options.arrows.from === !0 || this.options.arrows.from.enabled === !0,
                     i = this.options.arrows.middle === !0 || this.options.arrows.middle.enabled === !0,
                     s = this.options.color.inherit,
                     o = {
@@ -6757,15 +6757,15 @@
                 let t = [e, this.options, this.globalOptions, this.defaultOptions];
                 this.labelModule.update(this.options, t), this.labelModule.baseSize !== void 0 && (this.baseFontSize = this.labelModule.baseSize)
             }
             updateEdgeType() {
                 let e = this.options.smooth,
                     t = !1,
                     i = !0;
-                return this.edgeType !== void 0 && ((this.edgeType instanceof Pi && e.enabled === !0 && e.type === "dynamic" || this.edgeType instanceof Di && e.enabled === !0 && e.type === "cubicBezier" || this.edgeType instanceof Mi && e.enabled === !0 && e.type !== "dynamic" && e.type !== "cubicBezier" || this.edgeType instanceof Fi && e.type.enabled === !1) && (i = !1), i === !0 && (t = this.cleanup())), i === !0 ? e.enabled === !0 ? e.type === "dynamic" ? (t = !0, this.edgeType = new Pi(this.options, this.body, this.labelModule)) : e.type === "cubicBezier" ? this.edgeType = new Di(this.options, this.body, this.labelModule) : this.edgeType = new Mi(this.options, this.body, this.labelModule) : this.edgeType = new Fi(this.options, this.body, this.labelModule) : this.edgeType.setOptions(this.options), t
+                return this.edgeType !== void 0 && ((this.edgeType instanceof Pi && e.enabled === !0 && e.type === "dynamic" || this.edgeType instanceof Mi && e.enabled === !0 && e.type === "cubicBezier" || this.edgeType instanceof Di && e.enabled === !0 && e.type !== "dynamic" && e.type !== "cubicBezier" || this.edgeType instanceof Fi && e.type.enabled === !1) && (i = !1), i === !0 && (t = this.cleanup())), i === !0 ? e.enabled === !0 ? e.type === "dynamic" ? (t = !0, this.edgeType = new Pi(this.options, this.body, this.labelModule)) : e.type === "cubicBezier" ? this.edgeType = new Mi(this.options, this.body, this.labelModule) : this.edgeType = new Di(this.options, this.body, this.labelModule) : this.edgeType = new Fi(this.options, this.body, this.labelModule) : this.edgeType.setOptions(this.options), t
             }
             connect() {
                 this.disconnect(), this.from = this.body.nodes[this.fromId] || void 0, this.to = this.body.nodes[this.toId] || void 0, this.connected = this.from !== void 0 && this.to !== void 0, this.connected === !0 ? (this.from.attachEdge(this), this.to.attachEdge(this)) : (this.from && this.from.detachEdge(this), this.to && this.to.detachEdge(this)), this.edgeType.connect()
             }
             disconnect() {
                 this.from && (this.from.detachEdge(this), this.from = void 0), this.to && (this.to.detachEdge(this), this.to = void 0), this.connected = !1
             }
@@ -7037,28 +7037,28 @@
                     I(this.edgesListeners, (e, t) => {
                         this.body.data.edges && this.body.data.edges.off(t, e)
                     }), delete this.body.functions.createEdge, delete this.edgesListeners.add, delete this.edgesListeners.update, delete this.edgesListeners.remove, delete this.edgesListeners
                 })
             }
             setOptions(e) {
                 if (e !== void 0) {
-                    ke.parseOptions(this.options, e, !0, this.defaultOptions, !0);
+                    Ce.parseOptions(this.options, e, !0, this.defaultOptions, !0);
                     let t = !1;
                     if (e.smooth !== void 0)
                         for (let i in this.body.edges) Object.prototype.hasOwnProperty.call(this.body.edges, i) && (t = this.body.edges[i].updateEdgeType() || t);
                     if (e.font !== void 0)
                         for (let i in this.body.edges) Object.prototype.hasOwnProperty.call(this.body.edges, i) && this.body.edges[i].updateLabelModule();
                     (e.hidden !== void 0 || e.physics !== void 0 || t === !0) && this.body.emitter.emit("_dataChanged")
                 }
             }
             setData(e, t = !1) {
                 let i = this.body.data.edges;
                 if (vi("id", e)) this.body.data.edges = e;
-                else if (Array.isArray(e)) this.body.data.edges = new Ce, this.body.data.edges.add(e);
-                else if (!e) this.body.data.edges = new Ce;
+                else if (Array.isArray(e)) this.body.data.edges = new Ee, this.body.data.edges.add(e);
+                else if (!e) this.body.data.edges = new Ee;
                 else throw new TypeError("Array or DataSet expected");
                 if (i && I(this.edgesListeners, (s, o) => {
                         i.off(o, s)
                     }), this.body.edges = {}, this.body.data.edges) {
                     I(this.edgesListeners, (o, r) => {
                         this.body.data.edges.on(r, o)
                     });
@@ -7104,15 +7104,15 @@
             refresh() {
                 I(this.body.edges, (e, t) => {
                     let i = this.body.data.edges.get(t);
                     i !== void 0 && e.setOptions(i)
                 })
             }
             create(e) {
-                return new ke(e, this.body, this.images, this.options, this.defaultOptions)
+                return new Ce(e, this.body, this.images, this.options, this.defaultOptions)
             }
             reconnectEdges() {
                 let e, t = this.body.nodes,
                     i = this.body.edges;
                 for (e in t) Object.prototype.hasOwnProperty.call(t, e) && (t[e].edges = []);
                 for (e in i)
                     if (Object.prototype.hasOwnProperty.call(i, e)) {
@@ -7147,15 +7147,15 @@
                 e.forEach((s, o) => {
                     t[o] === void 0 && i.push(o)
                 }), this.add(i, !0)
             }
         },
         Ni = class {
             constructor(e, t, i) {
-                this.body = e, this.physicsBody = t, this.barnesHutTree, this.setOptions(i), this._rng = yt("BARNES HUT SOLVER")
+                this.body = e, this.physicsBody = t, this.barnesHutTree, this.setOptions(i), this._rng = mt("BARNES HUT SOLVER")
             }
             setOptions(e) {
                 this.options = e, this.thetaInversed = 1 / this.options.theta, this.overlapAvoidanceFactor = 1 - Math.max(0, Math.min(1, this.options.avoidOverlap))
             }
             solve() {
                 if (this.options.gravitationalConstant !== 0 && this.physicsBody.physicsNodeIndices.length > 0) {
                     let e, t = this.body.nodes,
@@ -7186,52 +7186,52 @@
             }
             _formBarnesHutTree(e, t) {
                 let i, s = t.length,
                     o = e[t[0]].x,
                     r = e[t[0]].y,
                     a = e[t[0]].x,
                     d = e[t[0]].y;
-                for (let g = 1; g < s; g++) {
-                    let p = e[t[g]],
-                        b = p.x,
-                        _ = p.y;
-                    p.options.mass > 0 && (b < o && (o = b), b > a && (a = b), _ < r && (r = _), _ > d && (d = _))
+                for (let p = 1; p < s; p++) {
+                    let y = e[t[p]],
+                        _ = y.x,
+                        x = y.y;
+                    y.options.mass > 0 && (_ < o && (o = _), _ > a && (a = _), x < r && (r = x), x > d && (d = x))
                 }
                 let h = Math.abs(a - o) - Math.abs(d - r);
                 h > 0 ? (r -= .5 * h, d += .5 * h) : (o += .5 * h, a -= .5 * h);
                 let c = Math.max(1e-5, Math.abs(a - o)),
                     u = .5 * c,
                     f = .5 * (o + a),
-                    y = .5 * (r + d),
-                    v = {
+                    m = .5 * (r + d),
+                    b = {
                         root: {
                             centerOfMass: {
                                 x: 0,
                                 y: 0
                             },
                             mass: 0,
                             range: {
                                 minX: f - u,
                                 maxX: f + u,
-                                minY: y - u,
-                                maxY: y + u
+                                minY: m - u,
+                                maxY: m + u
                             },
                             size: c,
                             calcSize: 1 / c,
                             children: {
                                 data: null
                             },
                             maxWidth: 0,
                             level: 0,
                             childrenCount: 4
                         }
                     };
-                this._splitBranch(v.root);
-                for (let g = 0; g < s; g++) i = e[t[g]], i.options.mass > 0 && this._placeInTree(v.root, i);
-                return v
+                this._splitBranch(b.root);
+                for (let p = 0; p < s; p++) i = e[t[p]], i.options.mass > 0 && this._placeInTree(b.root, i);
+                return b
             }
             _updateBranchMass(e, t) {
                 let i = e.centerOfMass,
                     s = e.mass + t.options.mass,
                     o = 1 / s;
                 i.x = i.x * e.mass + t.x * t.options.mass, i.x *= o, i.y = i.y * e.mass + t.y * t.options.mass, i.y *= o, e.mass = s;
                 let r = Math.max(Math.max(t.height, t.radius), t.width);
@@ -7304,29 +7304,29 @@
             }
             _drawBranch(e, t, i) {
                 i === void 0 && (i = "#FF0000"), e.childrenCount === 4 && (this._drawBranch(e.children.NW, t), this._drawBranch(e.children.NE, t), this._drawBranch(e.children.SE, t), this._drawBranch(e.children.SW, t)), t.strokeStyle = i, t.beginPath(), t.moveTo(e.range.minX, e.range.minY), t.lineTo(e.range.maxX, e.range.minY), t.stroke(), t.beginPath(), t.moveTo(e.range.maxX, e.range.minY), t.lineTo(e.range.maxX, e.range.maxY), t.stroke(), t.beginPath(), t.moveTo(e.range.maxX, e.range.maxY), t.lineTo(e.range.minX, e.range.maxY), t.stroke(), t.beginPath(), t.moveTo(e.range.minX, e.range.maxY), t.lineTo(e.range.minX, e.range.minY), t.stroke()
             }
         },
         Ho = class {
             constructor(e, t, i) {
-                this._rng = yt("REPULSION SOLVER"), this.body = e, this.physicsBody = t, this.setOptions(i)
+                this._rng = mt("REPULSION SOLVER"), this.body = e, this.physicsBody = t, this.setOptions(i)
             }
             setOptions(e) {
                 this.options = e
             }
             solve() {
                 let e, t, i, s, o, r, a, d, h = this.body.nodes,
                     l = this.physicsBody.physicsNodeIndices,
                     c = this.physicsBody.forces,
                     u = this.options.nodeDistance,
                     f = -2 / 3 / u,
-                    y = 4 / 3;
-                for (let v = 0; v < l.length - 1; v++) {
-                    a = h[l[v]];
-                    for (let g = v + 1; g < l.length; g++) d = h[l[g]], e = d.x - a.x, t = d.y - a.y, i = Math.sqrt(e * e + t * t), i === 0 && (i = .1 * this._rng(), e = i), i < 2 * u && (i < .5 * u ? r = 1 : r = f * i + y, r = r / i, s = e * r, o = t * r, c[a.id].x -= s, c[a.id].y -= o, c[d.id].x += s, c[d.id].y += o)
+                    m = 4 / 3;
+                for (let b = 0; b < l.length - 1; b++) {
+                    a = h[l[b]];
+                    for (let p = b + 1; p < l.length; p++) d = h[l[p]], e = d.x - a.x, t = d.y - a.y, i = Math.sqrt(e * e + t * t), i === 0 && (i = .1 * this._rng(), e = i), i < 2 * u && (i < .5 * u ? r = 1 : r = f * i + m, r = r / i, s = e * r, o = t * r, c[a.id].x -= s, c[a.id].y -= o, c[d.id].x += s, c[d.id].y += o)
                 }
             }
         },
         jo = class {
             constructor(e, t, i) {
                 this.body = e, this.physicsBody = t, this.setOptions(i)
             }
@@ -7344,19 +7344,19 @@
                         let d = e[t[a]];
                         if (r.level === d.level) {
                             let h = s + this.overlapAvoidanceFactor * ((r.shape.radius || 0) / 2 + (d.shape.radius || 0) / 2),
                                 l = d.x - r.x,
                                 c = d.y - r.y,
                                 u = Math.sqrt(l * l + c * c),
                                 f = .05,
-                                y;
-                            u < h ? y = -Math.pow(f * u, 2) + Math.pow(f * h, 2) : y = 0, u !== 0 && (y = y / u);
-                            let v = l * y,
-                                g = c * y;
-                            i[r.id].x -= v, i[r.id].y -= g, i[d.id].x += v, i[d.id].y += g
+                                m;
+                            u < h ? m = -Math.pow(f * u, 2) + Math.pow(f * h, 2) : m = 0, u !== 0 && (m = m / u);
+                            let b = l * m,
+                                p = c * m;
+                            i[r.id].x -= b, i[r.id].y -= p, i[d.id].x += b, i[d.id].y += p
                         }
                     }
                 }
             }
         },
         Gt = class {
             constructor(e, t, i) {
@@ -7390,40 +7390,40 @@
             }
             solve() {
                 let e, t, i, s, o, r, a, d, h = this.body.edges,
                     l = .5,
                     c = this.physicsBody.physicsEdgeIndices,
                     u = this.physicsBody.physicsNodeIndices,
                     f = this.physicsBody.forces;
-                for (let C = 0; C < u.length; C++) {
-                    let x = u[C];
-                    f[x].springFx = 0, f[x].springFy = 0
+                for (let T = 0; T < u.length; T++) {
+                    let O = u[T];
+                    f[O].springFx = 0, f[O].springFy = 0
                 }
-                for (let C = 0; C < c.length; C++) t = h[c[C]], t.connected === !0 && (e = t.options.length === void 0 ? this.options.springLength : t.options.length, i = t.from.x - t.to.x, s = t.from.y - t.to.y, d = Math.sqrt(i * i + s * s), d = d === 0 ? .01 : d, a = this.options.springConstant * (e - d) / d, o = i * a, r = s * a, t.to.level != t.from.level ? (f[t.toId] !== void 0 && (f[t.toId].springFx -= o, f[t.toId].springFy -= r), f[t.fromId] !== void 0 && (f[t.fromId].springFx += o, f[t.fromId].springFy += r)) : (f[t.toId] !== void 0 && (f[t.toId].x -= l * o, f[t.toId].y -= l * r), f[t.fromId] !== void 0 && (f[t.fromId].x += l * o, f[t.fromId].y += l * r)));
+                for (let T = 0; T < c.length; T++) t = h[c[T]], t.connected === !0 && (e = t.options.length === void 0 ? this.options.springLength : t.options.length, i = t.from.x - t.to.x, s = t.from.y - t.to.y, d = Math.sqrt(i * i + s * s), d = d === 0 ? .01 : d, a = this.options.springConstant * (e - d) / d, o = i * a, r = s * a, t.to.level != t.from.level ? (f[t.toId] !== void 0 && (f[t.toId].springFx -= o, f[t.toId].springFy -= r), f[t.fromId] !== void 0 && (f[t.fromId].springFx += o, f[t.fromId].springFy += r)) : (f[t.toId] !== void 0 && (f[t.toId].x -= l * o, f[t.toId].y -= l * r), f[t.fromId] !== void 0 && (f[t.fromId].x += l * o, f[t.fromId].y += l * r)));
                 a = 1;
-                let y, v;
-                for (let C = 0; C < u.length; C++) {
-                    let x = u[C];
-                    y = Math.min(a, Math.max(-a, f[x].springFx)), v = Math.min(a, Math.max(-a, f[x].springFy)), f[x].x += y, f[x].y += v
-                }
-                let g = 0,
-                    p = 0;
-                for (let C = 0; C < u.length; C++) {
-                    let x = u[C];
-                    g += f[x].x, p += f[x].y
-                }
-                let b = g / u.length,
-                    _ = p / u.length;
-                for (let C = 0; C < u.length; C++) {
-                    let x = u[C];
-                    f[x].x -= b, f[x].y -= _
+                let m, b;
+                for (let T = 0; T < u.length; T++) {
+                    let O = u[T];
+                    m = Math.min(a, Math.max(-a, f[O].springFx)), b = Math.min(a, Math.max(-a, f[O].springFy)), f[O].x += m, f[O].y += b
+                }
+                let p = 0,
+                    y = 0;
+                for (let T = 0; T < u.length; T++) {
+                    let O = u[T];
+                    p += f[O].x, y += f[O].y
+                }
+                let _ = p / u.length,
+                    x = y / u.length;
+                for (let T = 0; T < u.length; T++) {
+                    let O = u[T];
+                    f[O].x -= _, f[O].y -= x
                 }
             }
         },
-        xt = class {
+        Et = class {
             constructor(e, t, i) {
                 this.body = e, this.physicsBody = t, this.setOptions(i)
             }
             setOptions(e) {
                 this.options = e
             }
             solve() {
@@ -7439,26 +7439,26 @@
                 let r = e === 0 ? 0 : this.options.centralGravity / e;
                 s[o.id].x = t * r, s[o.id].y = i * r
             }
         },
         Vo = class extends Ni {
             constructor(e, t, i) {
                 super(e, t, i);
-                this._rng = yt("FORCE ATLAS 2 BASED REPULSION SOLVER")
+                this._rng = mt("FORCE ATLAS 2 BASED REPULSION SOLVER")
             }
             _calculateForces(e, t, i, s, o) {
                 e === 0 && (e = .1 * this._rng(), t = e), this.overlapAvoidanceFactor < 1 && s.shape.radius && (e = Math.max(.1 + this.overlapAvoidanceFactor * s.shape.radius, e - s.shape.radius));
                 let r = s.edges.length + 1,
                     a = this.options.gravitationalConstant * o.mass * s.options.mass * r / Math.pow(e, 2),
                     d = t * a,
                     h = i * a;
                 this.physicsBody.forces[s.id].x += d, this.physicsBody.forces[s.id].y += h
             }
         },
-        qo = class extends xt {
+        qo = class extends Et {
             constructor(e, t, i) {
                 super(e, t, i)
             }
             _calculateForces(e, t, i, s, o) {
                 if (e > 0) {
                     let r = o.edges.length + 1,
                         a = this.options.centralGravity * r * o.options.mass;
@@ -7548,23 +7548,23 @@
                 })
             }
             setOptions(e) {
                 if (e !== void 0)
                     if (e === !1) this.options.enabled = !1, this.physicsEnabled = !1, this.stopSimulation();
                     else if (e === !0) this.options.enabled = !0, this.physicsEnabled = !0, this.startSimulation();
                 else {
-                    this.physicsEnabled = !0, bt(["stabilization"], this.options, e), se(this.options, e, "stabilization"), e.enabled === void 0 && (this.options.enabled = !0), this.options.enabled === !1 && (this.physicsEnabled = !1, this.stopSimulation());
+                    this.physicsEnabled = !0, yt(["stabilization"], this.options, e), se(this.options, e, "stabilization"), e.enabled === void 0 && (this.options.enabled = !0), this.options.enabled === !1 && (this.physicsEnabled = !1, this.stopSimulation());
                     let t = this.options.wind;
                     t && ((typeof t.x != "number" || Number.isNaN(t.x)) && (t.x = 0), (typeof t.y != "number" || Number.isNaN(t.y)) && (t.y = 0)), this.timestep = this.options.timestep
                 }
                 this.init()
             }
             init() {
                 let e;
-                this.options.solver === "forceAtlas2Based" ? (e = this.options.forceAtlas2Based, this.nodesSolver = new Vo(this.body, this.physicsBody, e), this.edgesSolver = new Gt(this.body, this.physicsBody, e), this.gravitySolver = new qo(this.body, this.physicsBody, e)) : this.options.solver === "repulsion" ? (e = this.options.repulsion, this.nodesSolver = new Ho(this.body, this.physicsBody, e), this.edgesSolver = new Gt(this.body, this.physicsBody, e), this.gravitySolver = new xt(this.body, this.physicsBody, e)) : this.options.solver === "hierarchicalRepulsion" ? (e = this.options.hierarchicalRepulsion, this.nodesSolver = new jo(this.body, this.physicsBody, e), this.edgesSolver = new Wo(this.body, this.physicsBody, e), this.gravitySolver = new xt(this.body, this.physicsBody, e)) : (e = this.options.barnesHut, this.nodesSolver = new Ni(this.body, this.physicsBody, e), this.edgesSolver = new Gt(this.body, this.physicsBody, e), this.gravitySolver = new xt(this.body, this.physicsBody, e)), this.modelOptions = e
+                this.options.solver === "forceAtlas2Based" ? (e = this.options.forceAtlas2Based, this.nodesSolver = new Vo(this.body, this.physicsBody, e), this.edgesSolver = new Gt(this.body, this.physicsBody, e), this.gravitySolver = new qo(this.body, this.physicsBody, e)) : this.options.solver === "repulsion" ? (e = this.options.repulsion, this.nodesSolver = new Ho(this.body, this.physicsBody, e), this.edgesSolver = new Gt(this.body, this.physicsBody, e), this.gravitySolver = new Et(this.body, this.physicsBody, e)) : this.options.solver === "hierarchicalRepulsion" ? (e = this.options.hierarchicalRepulsion, this.nodesSolver = new jo(this.body, this.physicsBody, e), this.edgesSolver = new Wo(this.body, this.physicsBody, e), this.gravitySolver = new Et(this.body, this.physicsBody, e)) : (e = this.options.barnesHut, this.nodesSolver = new Ni(this.body, this.physicsBody, e), this.edgesSolver = new Gt(this.body, this.physicsBody, e), this.gravitySolver = new Et(this.body, this.physicsBody, e)), this.modelOptions = e
             }
             initPhysics() {
                 this.physicsEnabled === !0 && this.options.enabled === !0 ? this.options.stabilization.enabled === !0 ? this.stabilize() : (this.stabilized = !1, this.ready = !0, this.body.emitter.emit("fit", {}, this.layoutFailed), this.startSimulation()) : (this.ready = !0, this.body.emitter.emit("fit"))
             }
             startSimulation() {
                 this.physicsEnabled === !0 && this.options.enabled === !0 ? (this.stabilized = !1, this.adaptiveTimestep = !1, this.body.emitter.emit("_resizeNodes"), this.viewFunction === void 0 && (this.viewFunction = this.simulationStep.bind(this), this.body.emitter.on("initRedraw", this.viewFunction), this.body.emitter.emit("_startRendering"))) : this.body.emitter.emit("_redraw")
             }
@@ -7727,15 +7727,15 @@
                         point: u,
                         angle: f,
                         length: l
                     }), e.fill()
                 }
             }
         },
-        G = class {
+        X = class {
             constructor() {}
             static getRange(e, t = []) {
                 let i = 1e9,
                     s = -1e9,
                     o = 1e9,
                     r = -1e9,
                     a;
@@ -7834,40 +7834,40 @@
                 for (let h = 0; h < this.body.nodeIndices.length; h++) {
                     let l = {},
                         c = {},
                         u = this.body.nodeIndices[h],
                         f = this.body.nodes[u];
                     if (o[u] === void 0) {
                         d = 0, a = [];
-                        for (let y = 0; y < f.edges.length; y++) r = f.edges[y], this.clusteredEdges[r.id] === void 0 && (r.toId !== r.fromId && d++, a.push(r));
+                        for (let m = 0; m < f.edges.length; m++) r = f.edges[m], this.clusteredEdges[r.id] === void 0 && (r.toId !== r.fromId && d++, a.push(r));
                         if (d === e) {
-                            let y = function(g) {
+                            let m = function(p) {
                                     if (t.joinCondition === void 0 || t.joinCondition === null) return !0;
-                                    let p = G.cloneOptions(g);
-                                    return t.joinCondition(p)
+                                    let y = X.cloneOptions(p);
+                                    return t.joinCondition(y)
                                 },
-                                v = !0;
-                            for (let g = 0; g < a.length; g++) {
-                                r = a[g];
-                                let p = this._getConnectedId(r, u);
-                                if (y(f)) c[r.id] = r, l[u] = f, l[p] = this.body.nodes[p], o[u] = !0;
+                                b = !0;
+                            for (let p = 0; p < a.length; p++) {
+                                r = a[p];
+                                let y = this._getConnectedId(r, u);
+                                if (m(f)) c[r.id] = r, l[u] = f, l[y] = this.body.nodes[y], o[u] = !0;
                                 else {
-                                    v = !1;
+                                    b = !1;
                                     break
                                 }
                             }
-                            if (Object.keys(l).length > 0 && Object.keys(c).length > 0 && v === !0) {
-                                let p = function() {
-                                    for (let b = 0; b < s.length; ++b)
-                                        for (let _ in l)
-                                            if (s[b].nodes[_] !== void 0) return s[b]
+                            if (Object.keys(l).length > 0 && Object.keys(c).length > 0 && b === !0) {
+                                let y = function() {
+                                    for (let _ = 0; _ < s.length; ++_)
+                                        for (let x in l)
+                                            if (s[_].nodes[x] !== void 0) return s[_]
                                 }();
-                                if (p !== void 0) {
-                                    for (let b in l) p.nodes[b] === void 0 && (p.nodes[b] = l[b]);
-                                    for (let b in c) p.edges[b] === void 0 && (p.edges[b] = c[b])
+                                if (y !== void 0) {
+                                    for (let _ in l) y.nodes[_] === void 0 && (y.nodes[_] = l[_]);
+                                    for (let _ in c) y.edges[_] === void 0 && (y.edges[_] = c[_])
                                 } else s.push({
                                     nodes: l,
                                     edges: c
                                 })
                             }
                         }
                     }
@@ -7885,25 +7885,25 @@
                 if (e === void 0) throw new Error("No nodeId supplied to clusterByConnection!");
                 if (this.body.nodes[e] === void 0) throw new Error("The nodeId given to clusterByConnection does not exist!");
                 let s = this.body.nodes[e];
                 t = this._checkOptions(t, s), t.clusterNodeProperties.x === void 0 && (t.clusterNodeProperties.x = s.x), t.clusterNodeProperties.y === void 0 && (t.clusterNodeProperties.y = s.y), t.clusterNodeProperties.fixed === void 0 && (t.clusterNodeProperties.fixed = {}, t.clusterNodeProperties.fixed.x = s.options.fixed.x, t.clusterNodeProperties.fixed.y = s.options.fixed.y);
                 let o = {},
                     r = {},
                     a = s.id,
-                    d = G.cloneOptions(s);
+                    d = X.cloneOptions(s);
                 o[a] = s;
                 for (let l = 0; l < s.edges.length; l++) {
                     let c = s.edges[l];
                     if (this.clusteredEdges[c.id] === void 0) {
                         let u = this._getConnectedId(c, a);
                         if (this.clusteredNodes[u] === void 0)
                             if (u !== a)
                                 if (t.joinCondition === void 0) r[c.id] = c, o[u] = this.body.nodes[u];
                                 else {
-                                    let f = G.cloneOptions(this.body.nodes[u]);
+                                    let f = X.cloneOptions(this.body.nodes[u]);
                                     t.joinCondition(d, f) === !0 && (r[c.id] = c, o[u] = this.body.nodes[u])
                                 }
                         else r[c.id] = c
                     }
                 }
                 let h = Object.keys(o).map(function(l) {
                     return o[l].id
@@ -7917,37 +7917,37 @@
                     }
                 }
                 this._cluster(o, r, t, i)
             }
             _createClusterEdges(e, t, i, s) {
                 let o, r, a, d, h, l, c = Object.keys(e),
                     u = [];
-                for (let v = 0; v < c.length; v++) {
-                    r = c[v], a = e[r];
-                    for (let g = 0; g < a.edges.length; g++) o = a.edges[g], this.clusteredEdges[o.id] === void 0 && (o.toId == o.fromId ? t[o.id] = o : o.toId == r ? (d = i.id, h = o.fromId, l = h) : (d = o.toId, h = i.id, l = d), e[l] === void 0 && u.push({
+                for (let b = 0; b < c.length; b++) {
+                    r = c[b], a = e[r];
+                    for (let p = 0; p < a.edges.length; p++) o = a.edges[p], this.clusteredEdges[o.id] === void 0 && (o.toId == o.fromId ? t[o.id] = o : o.toId == r ? (d = i.id, h = o.fromId, l = h) : (d = o.toId, h = i.id, l = d), e[l] === void 0 && u.push({
                         edge: o,
                         fromId: h,
                         toId: d
                     }))
                 }
                 let f = [],
-                    y = function(v) {
-                        for (let g = 0; g < f.length; g++) {
-                            let p = f[g],
-                                b = v.fromId === p.fromId && v.toId === p.toId,
-                                _ = v.fromId === p.toId && v.toId === p.fromId;
-                            if (b || _) return p
+                    m = function(b) {
+                        for (let p = 0; p < f.length; p++) {
+                            let y = f[p],
+                                _ = b.fromId === y.fromId && b.toId === y.toId,
+                                x = b.fromId === y.toId && b.toId === y.fromId;
+                            if (_ || x) return y
                         }
                         return null
                     };
-                for (let v = 0; v < u.length; v++) {
-                    let g = u[v],
-                        p = g.edge,
-                        b = y(g);
-                    b === null ? (b = this._createClusteredEdge(g.fromId, g.toId, p, s), f.push(b)) : b.clusteringEdgeReplacingIds.push(p.id), this.body.edges[p.id].edgeReplacedById = b.id, this._backupEdgeOptions(p), p.setOptions({
+                for (let b = 0; b < u.length; b++) {
+                    let p = u[b],
+                        y = p.edge,
+                        _ = m(p);
+                    _ === null ? (_ = this._createClusteredEdge(p.fromId, p.toId, y, s), f.push(_)) : _.clusteringEdgeReplacingIds.push(y.id), this.body.edges[y.id].edgeReplacedById = _.id, this._backupEdgeOptions(y), y.setOptions({
                         physics: !1
                     })
                 }
             }
             _checkOptions(e = {}) {
                 return e.clusterEdgeProperties === void 0 && (e.clusterEdgeProperties = {}), e.clusterNodeProperties === void 0 && (e.clusterNodeProperties = {}), e
             }
@@ -7957,24 +7957,24 @@
                 for (let l = 0; l < o.length; ++l) delete e[o[l]];
                 if (Object.keys(e).length == 0 || Object.keys(e).length == 1 && i.clusterNodeProperties.allowSingleNodeCluster != !0) return;
                 let r = D({}, i.clusterNodeProperties);
                 if (i.processProperties !== void 0) {
                     let l = [];
                     for (let u in e)
                         if (Object.prototype.hasOwnProperty.call(e, u)) {
-                            let f = G.cloneOptions(e[u]);
+                            let f = X.cloneOptions(e[u]);
                             l.push(f)
                         } let c = [];
                     for (let u in t)
                         if (Object.prototype.hasOwnProperty.call(t, u) && u.substr(0, 12) !== "clusterEdge:") {
-                            let f = G.cloneOptions(t[u], "edge");
+                            let f = X.cloneOptions(t[u], "edge");
                             c.push(f)
                         } if (r = i.processProperties(r, l, c), !r) throw new Error("The processProperties function does not return properties!")
                 }
-                r.id === void 0 && (r.id = "cluster:" + xe());
+                r.id === void 0 && (r.id = "cluster:" + _e());
                 let a = r.id;
                 r.label === void 0 && (r.label = "cluster");
                 let d;
                 r.x === void 0 && (d = this._getClusterPosition(e), r.x = d.x), r.y === void 0 && (d === void 0 && (d = this._getClusterPosition(e)), r.y = d.y), r.id = a;
                 let h = this.body.functions.createNode(r, Yo);
                 h.containedNodes = e, h.containedEdges = t, h.clusterEdgeProperties = i.clusterEdgeProperties, this.body.nodes[r.id] = h, this._clusterEdges(e, t, r, i.clusterEdgeProperties), r.id = void 0, s === !0 && this.body.emitter.emit("_dataChanged")
             }
@@ -8023,24 +8023,24 @@
                     let l = {},
                         c = {
                             x: s.x,
                             y: s.y
                         };
                     for (let f in a)
                         if (Object.prototype.hasOwnProperty.call(a, f)) {
-                            let y = this.body.nodes[f];
+                            let m = this.body.nodes[f];
                             l[f] = {
-                                x: y.x,
-                                y: y.y
+                                x: m.x,
+                                y: m.y
                             }
                         } let u = t.releaseFunction(c, l);
                     for (let f in a)
                         if (Object.prototype.hasOwnProperty.call(a, f)) {
-                            let y = this.body.nodes[f];
-                            u[f] !== void 0 && (y.x = u[f].x === void 0 ? s.x : u[f].x, y.y = u[f].y === void 0 ? s.y : u[f].y)
+                            let m = this.body.nodes[f];
+                            u[f] !== void 0 && (m.x = u[f].x === void 0 ? s.x : u[f].x, m.y = u[f].y === void 0 ? s.y : u[f].y)
                         }
                 } else I(a, function(l) {
                     l.options.fixed.x === !1 && (l.x = s.x), l.options.fixed.y === !1 && (l.y = s.y)
                 });
                 for (let l in a)
                     if (Object.prototype.hasOwnProperty.call(a, l)) {
                         let c = this.body.nodes[l];
@@ -8049,28 +8049,28 @@
                         }), delete this.clusteredNodes[l]
                     } let h = [];
                 for (let l = 0; l < s.edges.length; l++) h.push(s.edges[l]);
                 for (let l = 0; l < h.length; l++) {
                     let c = h[l],
                         u = this._getConnectedId(c, e),
                         f = this.clusteredNodes[u];
-                    for (let y = 0; y < c.clusteringEdgeReplacingIds.length; y++) {
-                        let v = c.clusteringEdgeReplacingIds[y],
-                            g = this.body.edges[v];
-                        if (g !== void 0)
+                    for (let m = 0; m < c.clusteringEdgeReplacingIds.length; m++) {
+                        let b = c.clusteringEdgeReplacingIds[m],
+                            p = this.body.edges[b];
+                        if (p !== void 0)
                             if (f !== void 0) {
-                                let p = this.body.nodes[f.clusterId];
-                                p.containedEdges[g.id] = g, delete d[g.id];
-                                let b = g.fromId,
-                                    _ = g.toId;
-                                g.toId == u ? _ = f.clusterId : b = f.clusterId, this._createClusteredEdge(b, _, g, p.clusterEdgeProperties, {
+                                let y = this.body.nodes[f.clusterId];
+                                y.containedEdges[p.id] = p, delete d[p.id];
+                                let _ = p.fromId,
+                                    x = p.toId;
+                                p.toId == u ? x = f.clusterId : _ = f.clusterId, this._createClusteredEdge(_, x, p, y.clusterEdgeProperties, {
                                     hidden: !1,
                                     physics: !0
                                 })
-                            } else this._restoreEdge(g)
+                            } else this._restoreEdge(p)
                     }
                     c.remove()
                 }
                 for (let l in d) Object.prototype.hasOwnProperty.call(d, l) && this._restoreEdge(d[l]);
                 delete this.body.nodes[e], i === !0 && this.body.emitter.emit("_dataChanged")
             }
             getNodesInCluster(e) {
@@ -8154,21 +8154,21 @@
                 e = e / i, t = t / i;
                 let o = t - Math.pow(e, 2),
                     r = Math.sqrt(o),
                     a = Math.floor(e + 2 * r);
                 return a > s && (a = s), a
             }
             _createClusteredEdge(e, t, i, s, o) {
-                let r = G.cloneOptions(i, "edge");
-                D(r, s), r.from = e, r.to = t, r.id = "clusterEdge:" + xe(), o !== void 0 && D(r, o);
+                let r = X.cloneOptions(i, "edge");
+                D(r, s), r.from = e, r.to = t, r.id = "clusterEdge:" + _e(), o !== void 0 && D(r, o);
                 let a = this.body.functions.createEdge(r);
                 return a.clusteringEdgeReplacingIds = [i.id], a.connect(), this.body.edges[a.id] = a, a
             }
             _clusterEdges(e, t, i, s) {
-                if (t instanceof ke) {
+                if (t instanceof Ce) {
                     let o = t,
                         r = {};
                     r[o.id] = o, t = r
                 }
                 if (e instanceof z) {
                     let o = e,
                         r = {};
@@ -8227,16 +8227,16 @@
                     })
                 }), I(this.body.edges, (d, h) => {
                     let l = !0,
                         c = d.clusteringEdgeReplacingIds;
                     if (c !== void 0) {
                         let u = 0;
                         I(c, f => {
-                            let y = this.body.edges[f];
-                            y !== void 0 && y.endPointsValid() && (u += 1)
+                            let m = this.body.edges[f];
+                            m !== void 0 && m.endPointsValid() && (u += 1)
                         }), l = u > 0
                     }(!d.endPointsValid() || !l) && (i[h] = h)
                 }), s(d => {
                     I(i, h => {
                         delete d.containedEdges[h], I(d.edges, (l, c) => {
                             if (l.id === h) {
                                 d.edges[c] = null;
@@ -8324,15 +8324,15 @@
             }), this.body.emitter.on("_stopRendering", () => {
                 this.renderRequests -= 1, this.renderingActive = this.renderRequests > 0, this.renderTimer = void 0
             }), this.body.emitter.on("destroy", () => {
                 this.renderRequests = 0, this.allowRedraw = !1, this.renderingActive = !1, this.requiresTimeout === !0 ? clearTimeout(this.renderTimer) : window.cancelAnimationFrame(this.renderTimer), this.body.emitter.off()
             })
         }
         setOptions(e) {
-            e !== void 0 && qe(["hideEdgesOnDrag", "hideEdgesOnZoom", "hideNodesOnDrag"], this.options, e)
+            e !== void 0 && je(["hideEdgesOnDrag", "hideEdgesOnZoom", "hideNodesOnDrag"], this.options, e)
         }
         _requestNextFrame(e, t) {
             if (typeof window == "undefined") return;
             let i, s = window;
             return this.requiresTimeout === !0 ? i = s.setTimeout(e, t) : s.requestAnimationFrame && (i = s.requestAnimationFrame(e)), i
         }
         _startRendering() {
@@ -8395,39 +8395,39 @@
                 c = {
                     top: h.y,
                     left: h.x,
                     bottom: l.y,
                     right: l.x
                 },
                 u = [];
-            for (let g = 0; g < s.length; g++)
-                if (o = i[s[g]], o.hover) a.push(s[g]);
-                else if (o.isSelected()) r.push(s[g]);
+            for (let p = 0; p < s.length; p++)
+                if (o = i[s[p]], o.hover) a.push(s[p]);
+                else if (o.isSelected()) r.push(s[p]);
             else if (t === !0) {
-                let p = o.draw(e);
-                p.drawExternalLabel != null && u.push(p.drawExternalLabel)
+                let y = o.draw(e);
+                y.drawExternalLabel != null && u.push(y.drawExternalLabel)
             } else if (o.isBoundingBoxOverlappingWith(c) === !0) {
-                let p = o.draw(e);
-                p.drawExternalLabel != null && u.push(p.drawExternalLabel)
+                let y = o.draw(e);
+                y.drawExternalLabel != null && u.push(y.drawExternalLabel)
             } else o.updateBoundingBox(e, o.selected);
-            let f, y = r.length,
-                v = a.length;
-            for (f = 0; f < y; f++) {
+            let f, m = r.length,
+                b = a.length;
+            for (f = 0; f < m; f++) {
                 o = i[r[f]];
-                let g = o.draw(e);
-                g.drawExternalLabel != null && u.push(g.drawExternalLabel)
+                let p = o.draw(e);
+                p.drawExternalLabel != null && u.push(p.drawExternalLabel)
             }
-            for (f = 0; f < v; f++) {
+            for (f = 0; f < b; f++) {
                 o = i[a[f]];
-                let g = o.draw(e);
-                g.drawExternalLabel != null && u.push(g.drawExternalLabel)
+                let p = o.draw(e);
+                p.drawExternalLabel != null && u.push(p.drawExternalLabel)
             }
             return {
                 drawExternalLabels: () => {
-                    for (let g of u) g()
+                    for (let p of u) p()
                 }
             }
         }
         _drawEdges(e) {
             let t = this.body.edges,
                 i = this.body.edgeIndices;
             for (let s = 0; s < i.length; s++) {
@@ -8482,15 +8482,15 @@
             this.body.emitter.once("resize", e => {
                 e.width !== 0 && (this.body.view.translation.x = e.width * .5), e.height !== 0 && (this.body.view.translation.y = e.height * .5)
             }), this.body.emitter.on("setSize", this.setSize.bind(this)), this.body.emitter.on("destroy", () => {
                 this.hammerFrame.destroy(), this.hammer.destroy(), this._cleanUp()
             })
         }
         setOptions(e) {
-            if (e !== void 0 && qe(["width", "height", "autoResize"], this.options, e), this._cleanUp(), this.options.autoResize === !0) {
+            if (e !== void 0 && je(["width", "height", "autoResize"], this.options, e), this._cleanUp(), this.options.autoResize === !0) {
                 if (window.ResizeObserver) {
                     let i = new ResizeObserver(() => {
                             this.setSize() === !0 && this.body.emitter.emit("_requestRedraw")
                         }),
                         {
                             frame: s
                         } = this;
@@ -8563,19 +8563,19 @@
             }
             this.body.container.appendChild(this.frame), this.body.view.scale = 1, this.body.view.translation = {
                 x: .5 * this.frame.canvas.clientWidth,
                 y: .5 * this.frame.canvas.clientHeight
             }, this._bindHammer()
         }
         _bindHammer() {
-            this.hammer !== void 0 && this.hammer.destroy(), this.drag = {}, this.pinch = {}, this.hammer = new Ue(this.frame.canvas), this.hammer.get("pinch").set({
+            this.hammer !== void 0 && this.hammer.destroy(), this.drag = {}, this.pinch = {}, this.hammer = new We(this.frame.canvas), this.hammer.get("pinch").set({
                 enable: !0
             }), this.hammer.get("pan").set({
                 threshold: 5,
-                direction: Ue.DIRECTION_ALL
+                direction: We.DIRECTION_ALL
             }), Kt(this.hammer, e => {
                 this.body.eventListeners.onTouch(e)
             }), this.hammer.on("tap", e => {
                 this.body.eventListeners.onTap(e)
             }), this.hammer.on("doubletap", e => {
                 this.body.eventListeners.onDoubleTap(e)
             }), this.hammer.on("press", e => {
@@ -8590,15 +8590,15 @@
                 this.body.eventListeners.onPinch(e)
             }), this.frame.canvas.addEventListener("wheel", e => {
                 this.body.eventListeners.onMouseWheel(e)
             }), this.frame.canvas.addEventListener("mousemove", e => {
                 this.body.eventListeners.onMouseMove(e)
             }), this.frame.canvas.addEventListener("contextmenu", e => {
                 this.body.eventListeners.onContext(e)
-            }), this.hammerFrame = new Ue(this.frame), Ko(this.hammerFrame, e => {
+            }), this.hammerFrame = new We(this.frame), Ko(this.hammerFrame, e => {
                 this.body.eventListeners.onRelease(e)
             })
         }
         setSize(e = this.options.width, t = this.options.height) {
             e = this._prepareValue(e), t = this._prepareValue(t);
             let i = !1,
                 s = this.frame.canvas.width,
@@ -8686,36 +8686,36 @@
                 this.options = e
             }
             fit(e, t = !1) {
                 e = Ea(e, this.body.nodeIndices);
                 let i = this.canvas.frame.canvas.clientWidth,
                     s = this.canvas.frame.canvas.clientHeight,
                     o, r;
-                if (i === 0 || s === 0) r = 1, o = G.getRange(this.body.nodes, e.nodes);
+                if (i === 0 || s === 0) r = 1, o = X.getRange(this.body.nodes, e.nodes);
                 else if (t === !0) {
                     let h = 0;
                     for (let u in this.body.nodes) Object.prototype.hasOwnProperty.call(this.body.nodes, u) && this.body.nodes[u].predefinedPosition === !0 && (h += 1);
                     if (h > .5 * this.body.nodeIndices.length) {
                         this.fit(e, !1);
                         return
                     }
-                    o = G.getRange(this.body.nodes, e.nodes);
+                    o = X.getRange(this.body.nodes, e.nodes);
                     let l = this.body.nodeIndices.length;
                     r = 12.662 / (l + 7.4147) + .0964822, r *= Math.min(i / 600, s / 600)
                 } else {
-                    this.body.emitter.emit("_resizeNodes"), o = G.getRange(this.body.nodes, e.nodes);
+                    this.body.emitter.emit("_resizeNodes"), o = X.getRange(this.body.nodes, e.nodes);
                     let h = Math.abs(o.maxX - o.minX) * 1.1,
                         l = Math.abs(o.maxY - o.minY) * 1.1,
                         c = i / h,
                         u = s / l;
                     r = c <= u ? c : u
                 }
                 r > e.maxZoomLevel ? r = e.maxZoomLevel : r < e.minZoomLevel && (r = e.minZoomLevel);
                 let d = {
-                    position: G.findCenter(o),
+                    position: X.findCenter(o),
                     scale: r,
                     animation: e.animation
                 };
                 this.moveTo(d)
             }
             focus(e, t = {}) {
                 if (this.body.nodes[e] !== void 0) {
@@ -8842,18 +8842,18 @@
             loadNavigationElements() {
                 this.cleanNavigation(), this.navigationDOM = {};
                 let e = ["up", "down", "left", "right", "zoomIn", "zoomOut", "zoomExtends"],
                     t = ["_moveUp", "_moveDown", "_moveLeft", "_moveRight", "_zoomIn", "_zoomOut", "_fit"];
                 this.navigationDOM.wrapper = document.createElement("div"), this.navigationDOM.wrapper.className = "vis-navigation", this.canvas.frame.appendChild(this.navigationDOM.wrapper);
                 for (let s = 0; s < e.length; s++) {
                     this.navigationDOM[e[s]] = document.createElement("div"), this.navigationDOM[e[s]].className = "vis-button vis-" + e[s], this.navigationDOM.wrapper.appendChild(this.navigationDOM[e[s]]);
-                    let o = new Ue(this.navigationDOM[e[s]]);
+                    let o = new We(this.navigationDOM[e[s]]);
                     t[s] === "_fit" ? Kt(o, this._fit.bind(this)) : Kt(o, this.bindToRedraw.bind(this, t[s])), this.navigationHammers.push(o)
                 }
-                let i = new Ue(this.canvas.frame);
+                let i = new We(this.canvas.frame);
                 Ko(i, () => {
                     this._stopMovement()
                 }), this.navigationHammers.push(i), this.iconsCreated = !0
             }
             bindToRedraw(e) {
                 this.boundFunctions[e] === void 0 && (this.boundFunctions[e] = this[e].bind(this), this.body.emitter.on("initRedraw", this.boundFunctions[e]), this.body.emitter.emit("_startRendering"))
             }
@@ -8995,15 +8995,15 @@
             }
             bindEventListeners() {
                 this.body.emitter.on("destroy", () => {
                     clearTimeout(this.popupTimer), delete this.body.functions.getPointer
                 })
             }
             setOptions(e) {
-                e !== void 0 && (bt(["hideEdgesOnDrag", "hideEdgesOnZoom", "hideNodesOnDrag", "keyboard", "multiselect", "selectable", "selectConnectedEdges"], this.options, e), se(this.options, e, "keyboard"), e.tooltip && (Object.assign(this.options.tooltip, e.tooltip), e.tooltip.color && (this.options.tooltip.color = zt(e.tooltip.color)))), this.navigationHandler.setOptions(this.options)
+                e !== void 0 && (yt(["hideEdgesOnDrag", "hideEdgesOnZoom", "hideNodesOnDrag", "keyboard", "multiselect", "selectable", "selectConnectedEdges"], this.options, e), se(this.options, e, "keyboard"), e.tooltip && (Object.assign(this.options.tooltip, e.tooltip), e.tooltip.color && (this.options.tooltip.color = zt(e.tooltip.color)))), this.navigationHandler.setOptions(this.options)
             }
             getPointer(e) {
                 return {
                     x: e.x - Fs(this.canvas.frame.canvas),
                     y: e.y - Ns(this.canvas.frame.canvas)
                 }
             }
@@ -9239,110 +9239,110 @@
                         i = s === void 0 ? !1 : s.id === this.popup.popupTargetId
                     }
                 } else this.selectionHandler.getNodeAt(e) === void 0 && this.body.edges[this.popup.popupTargetId] !== void 0 && (i = this.body.edges[this.popup.popupTargetId].isOverlappingWith(t));
                 i === !1 && (this.popupObj = void 0, this.popup.hide(), this.body.emitter.emit("hidePopup"))
             }
         };
 
-    function A(n, e, t, i) {
+    function B(n, e, t, i) {
         if (t === "a" && !i) throw new TypeError("Private accessor was defined without a getter");
         if (typeof e == "function" ? n !== e || !i : !e.has(n)) throw new TypeError("Cannot read private member from an object whose class did not declare it");
         return t === "m" ? i : t === "a" ? i.call(n) : i ? i.value : e.get(n)
     }
 
     function Bi(n, e, t, i, s) {
         if (i === "m") throw new TypeError("Private method is not writable");
         if (i === "a" && !s) throw new TypeError("Private accessor was defined without a setter");
         if (typeof e == "function" ? n !== e || !s : !e.has(n)) throw new TypeError("Cannot write private member to an object whose class did not declare it");
         return i === "a" ? s.call(n, t) : s ? s.value = t : e.set(n, t), t
     }
     typeof SuppressedError == "function" && SuppressedError;
-    var Xe, ae, Fe, Ne, $t;
+    var qe, re, Pe, De, $t;
 
     function en(n, e) {
         let t = new Set;
         for (let i of e) n.has(i) || t.add(i);
         return t
     }
     var Ai = class {
         constructor() {
-            Xe.set(this, new Set), ae.set(this, new Set)
+            qe.set(this, new Set), re.set(this, new Set)
         }
         get size() {
-            return A(this, ae, "f").size
+            return B(this, re, "f").size
         }
         add(...e) {
-            for (let t of e) A(this, ae, "f").add(t)
+            for (let t of e) B(this, re, "f").add(t)
         }
         delete(...e) {
-            for (let t of e) A(this, ae, "f").delete(t)
+            for (let t of e) B(this, re, "f").delete(t)
         }
         clear() {
-            A(this, ae, "f").clear()
+            B(this, re, "f").clear()
         }
         getSelection() {
-            return [...A(this, ae, "f")]
+            return [...B(this, re, "f")]
         }
         getChanges() {
             return {
-                added: [...en(A(this, Xe, "f"), A(this, ae, "f"))],
-                deleted: [...en(A(this, ae, "f"), A(this, Xe, "f"))],
-                previous: [...new Set(A(this, Xe, "f"))],
-                current: [...new Set(A(this, ae, "f"))]
+                added: [...en(B(this, qe, "f"), B(this, re, "f"))],
+                deleted: [...en(B(this, re, "f"), B(this, qe, "f"))],
+                previous: [...new Set(B(this, qe, "f"))],
+                current: [...new Set(B(this, re, "f"))]
             }
         }
         commit() {
             let e = this.getChanges();
-            Bi(this, Xe, A(this, ae, "f"), "f"), Bi(this, ae, new Set(A(this, Xe, "f")), "f");
+            Bi(this, qe, B(this, re, "f"), "f"), Bi(this, re, new Set(B(this, qe, "f")), "f");
             for (let t of e.added) t.select();
             for (let t of e.deleted) t.unselect();
             return e
         }
     };
-    Xe = new WeakMap, ae = new WeakMap;
+    qe = new WeakMap, re = new WeakMap;
     var tn = class {
         constructor(e = () => {}) {
-            Fe.set(this, new Ai), Ne.set(this, new Ai), $t.set(this, void 0), Bi(this, $t, e, "f")
+            Pe.set(this, new Ai), De.set(this, new Ai), $t.set(this, void 0), Bi(this, $t, e, "f")
         }
         get sizeNodes() {
-            return A(this, Fe, "f").size
+            return B(this, Pe, "f").size
         }
         get sizeEdges() {
-            return A(this, Ne, "f").size
+            return B(this, De, "f").size
         }
         getNodes() {
-            return A(this, Fe, "f").getSelection()
+            return B(this, Pe, "f").getSelection()
         }
         getEdges() {
-            return A(this, Ne, "f").getSelection()
+            return B(this, De, "f").getSelection()
         }
         addNodes(...e) {
-            A(this, Fe, "f").add(...e)
+            B(this, Pe, "f").add(...e)
         }
         addEdges(...e) {
-            A(this, Ne, "f").add(...e)
+            B(this, De, "f").add(...e)
         }
         deleteNodes(e) {
-            A(this, Fe, "f").delete(e)
+            B(this, Pe, "f").delete(e)
         }
         deleteEdges(e) {
-            A(this, Ne, "f").delete(e)
+            B(this, De, "f").delete(e)
         }
         clear() {
-            A(this, Fe, "f").clear(), A(this, Ne, "f").clear()
+            B(this, Pe, "f").clear(), B(this, De, "f").clear()
         }
         commit(...e) {
             let t = {
-                nodes: A(this, Fe, "f").commit(),
-                edges: A(this, Ne, "f").commit()
+                nodes: B(this, Pe, "f").commit(),
+                edges: B(this, De, "f").commit()
             };
-            return A(this, $t, "f").call(this, t, ...e), t
+            return B(this, $t, "f").call(this, t, ...e), t
         }
     };
-    Fe = new WeakMap, Ne = new WeakMap, $t = new WeakMap;
+    Pe = new WeakMap, De = new WeakMap, $t = new WeakMap;
     var sn = class {
             constructor(e, t) {
                 this.body = e, this.canvas = t, this._selectionAccumulator = new tn, this.hoverObj = {
                     nodes: {},
                     edges: {}
                 }, this.options = {}, this.defaultOptions = {
                     multiselect: !1,
@@ -9350,15 +9350,15 @@
                     selectConnectedEdges: !0,
                     hoverConnectedEdges: !0
                 }, Object.assign(this.options, this.defaultOptions), this.body.emitter.on("_dataChanged", () => {
                     this.updateSelection()
                 })
             }
             setOptions(e) {
-                e !== void 0 && qe(["multiselect", "hoverConnectedEdges", "selectable", "selectConnectedEdges"], this.options, e)
+                e !== void 0 && je(["multiselect", "hoverConnectedEdges", "selectable", "selectConnectedEdges"], this.options, e)
             }
             selectOnPoint(e) {
                 let t = !1;
                 if (this.options.selectable === !0) {
                     let i = this.getNodeAt(e) || this.getEdgeAt(e);
                     this.unselectAll(), i !== void 0 && (t = this.selectObject(i)), this.body.emitter.emit("_requestRedraw")
                 }
@@ -9440,16 +9440,16 @@
                     let d = this.body.edgeIndices[a],
                         h = r[d];
                     if (h.connected) {
                         let l = h.from.x,
                             c = h.from.y,
                             u = h.to.x,
                             f = h.to.y,
-                            y = h.edgeType.getDistanceToEdge(l, c, u, f, i.x, i.y);
-                        y < s && (o = d, s = y)
+                            m = h.edgeType.getDistanceToEdge(l, c, u, f, i.x, i.y);
+                        m < s && (o = d, s = m)
                     }
                 }
                 if (o !== null) return t === !0 ? this.body.edges[o] : o
             }
             _addToHover(e) {
                 e instanceof z ? this.hoverObj.nodes[e.id] = e : this.hoverObj.edges[e.id] = e
             }
@@ -9480,20 +9480,20 @@
                     o = !1;
                 return i.hover === !1 && (i.hover = !0, this._addToHover(i), o = !0, i instanceof z ? (s.node = i.id, this.body.emitter.emit("hoverNode", s)) : (s.edge = i.id, this.body.emitter.emit("hoverEdge", s))), o
             }
             hoverObject(e, t) {
                 let i = this.getNodeAt(t);
                 i === void 0 && (i = this.getEdgeAt(t));
                 let s = !1;
-                for (let o in this.hoverObj.nodes) Object.prototype.hasOwnProperty.call(this.hoverObj.nodes, o) && (i === void 0 || i instanceof z && i.id != o || i instanceof ke) && (this.emitBlurEvent(e, t, this.hoverObj.nodes[o]), delete this.hoverObj.nodes[o], s = !0);
-                for (let o in this.hoverObj.edges) Object.prototype.hasOwnProperty.call(this.hoverObj.edges, o) && (s === !0 ? (this.hoverObj.edges[o].hover = !1, delete this.hoverObj.edges[o]) : (i === void 0 || i instanceof ke && i.id != o || i instanceof z && !i.hover) && (this.emitBlurEvent(e, t, this.hoverObj.edges[o]), delete this.hoverObj.edges[o], s = !0));
+                for (let o in this.hoverObj.nodes) Object.prototype.hasOwnProperty.call(this.hoverObj.nodes, o) && (i === void 0 || i instanceof z && i.id != o || i instanceof Ce) && (this.emitBlurEvent(e, t, this.hoverObj.nodes[o]), delete this.hoverObj.nodes[o], s = !0);
+                for (let o in this.hoverObj.edges) Object.prototype.hasOwnProperty.call(this.hoverObj.edges, o) && (s === !0 ? (this.hoverObj.edges[o].hover = !1, delete this.hoverObj.edges[o]) : (i === void 0 || i instanceof Ce && i.id != o || i instanceof z && !i.hover) && (this.emitBlurEvent(e, t, this.hoverObj.edges[o]), delete this.hoverObj.edges[o], s = !0));
                 if (i !== void 0) {
                     let o = Object.keys(this.hoverObj.edges).length,
                         r = Object.keys(this.hoverObj.nodes).length,
-                        a = i instanceof ke && o === 0 && r === 0,
+                        a = i instanceof Ce && o === 0 && r === 0,
                         d = i instanceof z && o === 0 && r === 0;
                     (s || a || d) && (s = this.emitHoverEvent(e, t, i)), i instanceof z && this.options.hoverConnectedEdges === !0 && this._hoverConnectedEdges(i)
                 }
                 s === !0 && this.body.emitter.emit("_requestRedraw")
             }
             commitWithoutEmitting() {
                 this._selectionAccumulator.commit()
@@ -9702,18 +9702,18 @@
             s[d] = 0;
             let l = [h],
                 c = 0,
                 u;
             for (; u = l.pop();) {
                 if (!i.has(d)) continue;
                 let f = s[u.id] + a;
-                if (u.edges.filter(y => y.connected && y.to !== y.from && y[t] !== u && i.has(y.toId) && i.has(y.fromId)).forEach(y => {
-                        let v = y[r],
-                            g = s[v];
-                        (g == null || e(f, g)) && (s[v] = f, l.push(y[t]))
+                if (u.edges.filter(m => m.connected && m.to !== m.from && m[t] !== u && i.has(m.toId) && i.has(m.fromId)).forEach(m => {
+                        let b = m[r],
+                            p = s[b];
+                        (p == null || e(f, p)) && (s[b] = f, l.push(m[t]))
                     }), c > o) return xa(i, s);
                 ++c
             }
         }
         return s
     }
     var an = class {
@@ -9837,21 +9837,21 @@
                     this.body.emitter.emit("_forceDisableDynamicCurves", e, !1)
                 })
             }
             setOptions(e, t) {
                 if (e !== void 0) {
                     let i = this.options.hierarchical,
                         s = i.enabled;
-                    if (qe(["randomSeed", "improvedLayout", "clusterThreshold"], this.options, e), se(this.options, e, "hierarchical"), e.randomSeed !== void 0 && this._resetRNG(e.randomSeed), i.enabled === !0) return s === !0 && this.body.emitter.emit("refresh", !0), i.direction === "RL" || i.direction === "DU" ? i.levelSeparation > 0 && (i.levelSeparation *= -1) : i.levelSeparation < 0 && (i.levelSeparation *= -1), this.setDirectionStrategy(), this.body.emitter.emit("_resetHierarchicalLayout"), this.adaptAllOptionsForHierarchicalLayout(t);
+                    if (je(["randomSeed", "improvedLayout", "clusterThreshold"], this.options, e), se(this.options, e, "hierarchical"), e.randomSeed !== void 0 && this._resetRNG(e.randomSeed), i.enabled === !0) return s === !0 && this.body.emitter.emit("refresh", !0), i.direction === "RL" || i.direction === "DU" ? i.levelSeparation > 0 && (i.levelSeparation *= -1) : i.levelSeparation < 0 && (i.levelSeparation *= -1), this.setDirectionStrategy(), this.body.emitter.emit("_resetHierarchicalLayout"), this.adaptAllOptionsForHierarchicalLayout(t);
                     if (s === !0) return this.body.emitter.emit("refresh"), D(t, this.optionsBackup)
                 }
                 return t
             }
             _resetRNG(e) {
-                this.initialRandomSeed = e, this._rng = yt(this.initialRandomSeed)
+                this.initialRandomSeed = e, this._rng = mt(this.initialRandomSeed)
             }
             adaptAllOptionsForHierarchicalLayout(e) {
                 if (this.options.hierarchical.enabled === !0) {
                     let t = this.optionsBackup.physics;
                     e.physics === void 0 || e.physics === !0 ? (e.physics = {
                         enabled: t.enabled === void 0 ? !0 : t.enabled,
                         solver: "hierarchicalRepulsion"
@@ -9961,16 +9961,16 @@
                             h.predefinedPosition === !1 && (h.x += (.5 - this._rng()) * a, h.y += (.5 - this._rng()) * a)
                         }
                         this._declusterAll(), this.body.emitter.emit("_repositionBezierNodes")
                     }
                 }
             }
             _shiftToCenter() {
-                let e = G.getRangeCore(this.body.nodes, this.body.nodeIndices),
-                    t = G.findCenter(e);
+                let e = X.getRangeCore(this.body.nodes, this.body.nodeIndices),
+                    t = X.findCenter(e);
                 for (let i = 0; i < this.body.nodeIndices.length; i++) {
                     let s = this.body.nodes[this.body.nodeIndices[i]];
                     s.x -= t.x, s.y -= t.y
                 }
             }
             _declusterAll() {
                 let e = !0;
@@ -10001,184 +10001,184 @@
                     }
                 }
             }
             _condenseHierarchy() {
                 let e = !1,
                     t = {},
                     i = () => {
-                        let g = o(),
-                            p = 0;
-                        for (let b = 0; b < g.length - 1; b++) p += g[b].max - g[b + 1].min + this.options.hierarchical.treeSpacing, s(b + 1, p)
-                    },
-                    s = (g, p) => {
-                        let b = this.hierarchical.trees;
-                        for (let _ in b) Object.prototype.hasOwnProperty.call(b, _) && b[_] === g && this.direction.shift(_, p)
+                        let p = o(),
+                            y = 0;
+                        for (let _ = 0; _ < p.length - 1; _++) y += p[_].max - p[_ + 1].min + this.options.hierarchical.treeSpacing, s(_ + 1, y)
+                    },
+                    s = (p, y) => {
+                        let _ = this.hierarchical.trees;
+                        for (let x in _) Object.prototype.hasOwnProperty.call(_, x) && _[x] === p && this.direction.shift(x, y)
                     },
                     o = () => {
-                        let g = [];
-                        for (let p = 0; p < this.hierarchical.numTrees(); p++) g.push(this.direction.getTreeSize(p));
-                        return g
-                    },
-                    r = (g, p) => {
-                        if (!p[g.id] && (p[g.id] = !0, this.hierarchical.childrenReference[g.id])) {
-                            let b = this.hierarchical.childrenReference[g.id];
-                            if (b.length > 0)
-                                for (let _ = 0; _ < b.length; _++) r(this.body.nodes[b[_]], p)
-                        }
-                    },
-                    a = (g, p = 1e9) => {
-                        let b = 1e9,
-                            _ = 1e9,
-                            C = 1e9,
-                            x = -1e9;
-                        for (let O in g)
-                            if (Object.prototype.hasOwnProperty.call(g, O)) {
-                                let M = this.body.nodes[O],
-                                    R = this.hierarchical.levels[M.id],
-                                    q = this.direction.getPosition(M),
-                                    [oe, Oe] = this._getSpaceAroundNode(M, g);
-                                b = Math.min(oe, b), _ = Math.min(Oe, _), R <= p && (C = Math.min(q, C), x = Math.max(q, x))
-                            } return [C, x, b, _]
-                    },
-                    d = (g, p) => {
-                        let b = this.hierarchical.getMaxLevel(g.id),
-                            _ = this.hierarchical.getMaxLevel(p.id);
-                        return Math.min(b, _)
-                    },
-                    h = (g, p, b) => {
-                        let _ = this.hierarchical;
-                        for (let C = 0; C < p.length; C++) {
-                            let x = p[C],
-                                O = _.distributionOrdering[x];
-                            if (O.length > 1)
-                                for (let M = 0; M < O.length - 1; M++) {
-                                    let R = O[M],
-                                        q = O[M + 1];
-                                    _.hasSameParent(R, q) && _.inSameSubNetwork(R, q) && g(R, q, b)
+                        let p = [];
+                        for (let y = 0; y < this.hierarchical.numTrees(); y++) p.push(this.direction.getTreeSize(y));
+                        return p
+                    },
+                    r = (p, y) => {
+                        if (!y[p.id] && (y[p.id] = !0, this.hierarchical.childrenReference[p.id])) {
+                            let _ = this.hierarchical.childrenReference[p.id];
+                            if (_.length > 0)
+                                for (let x = 0; x < _.length; x++) r(this.body.nodes[_[x]], y)
+                        }
+                    },
+                    a = (p, y = 1e9) => {
+                        let _ = 1e9,
+                            x = 1e9,
+                            T = 1e9,
+                            O = -1e9;
+                        for (let S in p)
+                            if (Object.prototype.hasOwnProperty.call(p, S)) {
+                                let A = this.body.nodes[S],
+                                    H = this.hierarchical.levels[A.id],
+                                    G = this.direction.getPosition(A),
+                                    [le, Ye] = this._getSpaceAroundNode(A, p);
+                                _ = Math.min(le, _), x = Math.min(Ye, x), H <= y && (T = Math.min(G, T), O = Math.max(G, O))
+                            } return [T, O, _, x]
+                    },
+                    d = (p, y) => {
+                        let _ = this.hierarchical.getMaxLevel(p.id),
+                            x = this.hierarchical.getMaxLevel(y.id);
+                        return Math.min(_, x)
+                    },
+                    h = (p, y, _) => {
+                        let x = this.hierarchical;
+                        for (let T = 0; T < y.length; T++) {
+                            let O = y[T],
+                                S = x.distributionOrdering[O];
+                            if (S.length > 1)
+                                for (let A = 0; A < S.length - 1; A++) {
+                                    let H = S[A],
+                                        G = S[A + 1];
+                                    x.hasSameParent(H, G) && x.inSameSubNetwork(H, G) && p(H, G, _)
                                 }
                         }
                     },
-                    l = (g, p, b = !1) => {
-                        let _ = this.direction.getPosition(g),
-                            C = this.direction.getPosition(p),
-                            x = Math.abs(C - _),
-                            O = this.options.hierarchical.nodeSpacing;
-                        if (x > O) {
-                            let M = {},
-                                R = {};
-                            r(g, M), r(p, R);
-                            let q = d(g, p),
-                                oe = a(M, q),
-                                Oe = a(R, q),
-                                ge = oe[1],
-                                Ge = Oe[0],
-                                W = Oe[2];
-                            if (Math.abs(ge - Ge) > O) {
-                                let N = ge - Ge + O;
-                                N < -W + O && (N = -W + O), N < 0 && (this._shiftBlock(p.id, N), e = !0, b === !0 && this._centerParent(p))
+                    l = (p, y, _ = !1) => {
+                        let x = this.direction.getPosition(p),
+                            T = this.direction.getPosition(y),
+                            O = Math.abs(T - x),
+                            S = this.options.hierarchical.nodeSpacing;
+                        if (O > S) {
+                            let A = {},
+                                H = {};
+                            r(p, A), r(y, H);
+                            let G = d(p, y),
+                                le = a(A, G),
+                                Ye = a(H, G),
+                                Ct = le[1],
+                                Xe = Ye[0],
+                                W = Ye[2];
+                            if (Math.abs(Ct - Xe) > S) {
+                                let F = Ct - Xe + S;
+                                F < -W + S && (F = -W + S), F < 0 && (this._shiftBlock(y.id, F), e = !0, _ === !0 && this._centerParent(y))
                             }
                         }
                     },
-                    c = (g, p) => {
-                        let b = p.id,
-                            _ = p.edges,
-                            C = this.hierarchical.levels[p.id],
-                            x = this.options.hierarchical.levelSeparation * this.options.hierarchical.levelSeparation,
-                            O = {},
-                            M = [];
-                        for (let W = 0; W < _.length; W++) {
-                            let F = _[W];
-                            if (F.toId != F.fromId) {
-                                let N = F.toId == b ? F.from : F.to;
-                                O[_[W].id] = N, this.hierarchical.levels[N.id] < C && M.push(F)
+                    c = (p, y) => {
+                        let _ = y.id,
+                            x = y.edges,
+                            T = this.hierarchical.levels[y.id],
+                            O = this.options.hierarchical.levelSeparation * this.options.hierarchical.levelSeparation,
+                            S = {},
+                            A = [];
+                        for (let W = 0; W < x.length; W++) {
+                            let M = x[W];
+                            if (M.toId != M.fromId) {
+                                let F = M.toId == _ ? M.from : M.to;
+                                S[x[W].id] = F, this.hierarchical.levels[F.id] < T && A.push(M)
                             }
                         }
-                        let R = (W, F) => {
-                                let N = 0;
-                                for (let Y = 0; Y < F.length; Y++)
-                                    if (O[F[Y].id] !== void 0) {
-                                        let K = this.direction.getPosition(O[F[Y].id]) - W;
-                                        N += K / Math.sqrt(K * K + x)
-                                    } return N
+                        let H = (W, M) => {
+                                let F = 0;
+                                for (let U = 0; U < M.length; U++)
+                                    if (S[M[U].id] !== void 0) {
+                                        let K = this.direction.getPosition(S[M[U].id]) - W;
+                                        F += K / Math.sqrt(K * K + O)
+                                    } return F
                             },
-                            q = (W, F) => {
-                                let N = 0;
-                                for (let Y = 0; Y < F.length; Y++)
-                                    if (O[F[Y].id] !== void 0) {
-                                        let K = this.direction.getPosition(O[F[Y].id]) - W;
-                                        N -= x * Math.pow(K * K + x, -1.5)
-                                    } return N
+                            G = (W, M) => {
+                                let F = 0;
+                                for (let U = 0; U < M.length; U++)
+                                    if (S[M[U].id] !== void 0) {
+                                        let K = this.direction.getPosition(S[M[U].id]) - W;
+                                        F -= O * Math.pow(K * K + O, -1.5)
+                                    } return F
                             },
-                            oe = (W, F) => {
-                                let N = this.direction.getPosition(p),
-                                    Y = {};
+                            le = (W, M) => {
+                                let F = this.direction.getPosition(y),
+                                    U = {};
                                 for (let K = 0; K < W; K++) {
-                                    let he = R(N, F),
-                                        Ke = q(N, F),
-                                        ot = 40,
-                                        yn = Math.max(-ot, Math.min(ot, Math.round(he / Ke)));
-                                    if (N = N - yn, Y[N] !== void 0) break;
-                                    Y[N] = K
+                                    let ae = H(F, M),
+                                        Ge = G(F, M),
+                                        st = 40,
+                                        yn = Math.max(-st, Math.min(st, Math.round(ae / Ge)));
+                                    if (F = F - yn, U[F] !== void 0) break;
+                                    U[F] = K
                                 }
-                                return N
+                                return F
                             },
-                            Oe = W => {
-                                let F = this.direction.getPosition(p);
-                                if (t[p.id] === void 0) {
-                                    let ot = {};
-                                    r(p, ot), t[p.id] = ot
+                            Ye = W => {
+                                let M = this.direction.getPosition(y);
+                                if (t[y.id] === void 0) {
+                                    let st = {};
+                                    r(y, st), t[y.id] = st
                                 }
-                                let N = a(t[p.id]),
-                                    Y = N[2],
-                                    K = N[3],
-                                    he = W - F,
-                                    Ke = 0;
-                                he > 0 ? Ke = Math.min(he, K - this.options.hierarchical.nodeSpacing) : he < 0 && (Ke = -Math.min(-he, Y - this.options.hierarchical.nodeSpacing)), Ke != 0 && (this._shiftBlock(p.id, Ke), e = !0)
+                                let F = a(t[y.id]),
+                                    U = F[2],
+                                    K = F[3],
+                                    ae = W - M,
+                                    Ge = 0;
+                                ae > 0 ? Ge = Math.min(ae, K - this.options.hierarchical.nodeSpacing) : ae < 0 && (Ge = -Math.min(-ae, U - this.options.hierarchical.nodeSpacing)), Ge != 0 && (this._shiftBlock(y.id, Ge), e = !0)
                             },
-                            ge = W => {
-                                let F = this.direction.getPosition(p),
-                                    [N, Y] = this._getSpaceAroundNode(p),
-                                    K = W - F,
-                                    he = F;
-                                K > 0 ? he = Math.min(F + (Y - this.options.hierarchical.nodeSpacing), W) : K < 0 && (he = Math.max(F - (N - this.options.hierarchical.nodeSpacing), W)), he !== F && (this.direction.setPosition(p, he), e = !0)
+                            Ct = W => {
+                                let M = this.direction.getPosition(y),
+                                    [F, U] = this._getSpaceAroundNode(y),
+                                    K = W - M,
+                                    ae = M;
+                                K > 0 ? ae = Math.min(M + (U - this.options.hierarchical.nodeSpacing), W) : K < 0 && (ae = Math.max(M - (F - this.options.hierarchical.nodeSpacing), W)), ae !== M && (this.direction.setPosition(y, ae), e = !0)
                             },
-                            Ge = oe(g, M);
-                        Oe(Ge), Ge = oe(g, _), ge(Ge)
+                            Xe = le(p, A);
+                        Ye(Xe), Xe = le(p, x), Ct(Xe)
                     },
-                    u = g => {
-                        let p = this.hierarchical.getLevels();
-                        p = p.reverse();
-                        for (let b = 0; b < g; b++) {
+                    u = p => {
+                        let y = this.hierarchical.getLevels();
+                        y = y.reverse();
+                        for (let _ = 0; _ < p; _++) {
                             e = !1;
-                            for (let _ = 0; _ < p.length; _++) {
-                                let C = p[_],
-                                    x = this.hierarchical.distributionOrdering[C];
-                                for (let O = 0; O < x.length; O++) c(1e3, x[O])
+                            for (let x = 0; x < y.length; x++) {
+                                let T = y[x],
+                                    O = this.hierarchical.distributionOrdering[T];
+                                for (let S = 0; S < O.length; S++) c(1e3, O[S])
                             }
                             if (e !== !0) break
                         }
                     },
-                    f = g => {
-                        let p = this.hierarchical.getLevels();
-                        p = p.reverse();
-                        for (let b = 0; b < g && (e = !1, h(l, p, !0), e === !0); b++);
+                    f = p => {
+                        let y = this.hierarchical.getLevels();
+                        y = y.reverse();
+                        for (let _ = 0; _ < p && (e = !1, h(l, y, !0), e === !0); _++);
                     },
-                    y = () => {
-                        for (let g in this.body.nodes) Object.prototype.hasOwnProperty.call(this.body.nodes, g) && this._centerParent(this.body.nodes[g])
+                    m = () => {
+                        for (let p in this.body.nodes) Object.prototype.hasOwnProperty.call(this.body.nodes, p) && this._centerParent(this.body.nodes[p])
                     },
-                    v = () => {
-                        let g = this.hierarchical.getLevels();
-                        g = g.reverse();
-                        for (let p = 0; p < g.length; p++) {
-                            let b = g[p],
-                                _ = this.hierarchical.distributionOrdering[b];
-                            for (let C = 0; C < _.length; C++) this._centerParent(_[C])
+                    b = () => {
+                        let p = this.hierarchical.getLevels();
+                        p = p.reverse();
+                        for (let y = 0; y < p.length; y++) {
+                            let _ = p[y],
+                                x = this.hierarchical.distributionOrdering[_];
+                            for (let T = 0; T < x.length; T++) this._centerParent(x[T])
                         }
                     };
-                this.options.hierarchical.blockShifting === !0 && (f(5), y()), this.options.hierarchical.edgeMinimization === !0 && u(20), this.options.hierarchical.parentCentralization === !0 && v(), i()
+                this.options.hierarchical.blockShifting === !0 && (f(5), m()), this.options.hierarchical.edgeMinimization === !0 && u(20), this.options.hierarchical.parentCentralization === !0 && b(), i()
             }
             _getSpaceAroundNode(e, t) {
                 let i = !0;
                 t === void 0 && (i = !1);
                 let s = this.hierarchical.levels[e.id];
                 if (s !== void 0) {
                     let o = this.hierarchical.distributionIndex[e.id],
@@ -10320,15 +10320,15 @@
             }
             _determineLevelsCustomCallback() {
                 let e = 1e5,
                     t = function(s, o, r) {},
                     i = (s, o, r) => {
                         let a = this.hierarchical.levels[s.id];
                         a === void 0 && (a = this.hierarchical.levels[s.id] = e);
-                        let d = t(G.cloneOptions(s, "node"), G.cloneOptions(o, "node"), G.cloneOptions(r, "edge"));
+                        let d = t(X.cloneOptions(s, "node"), X.cloneOptions(o, "node"), X.cloneOptions(r, "edge"));
                         this.hierarchical.levels[o.id] = a + d
                     };
                 this._crawlNetwork(i), this.hierarchical.setMinLevelToZero(this.body.nodes)
             }
             _determineLevelsDirected() {
                 let e = this.body.nodeIndices.reduce((t, i) => (t.set(i, this.body.nodes[i]), t), new Map);
                 this.options.hierarchical.shakeTowards === "roots" ? this.hierarchical.levels = Ta(e) : this.hierarchical.levels = Ca(e), this.hierarchical.setMinLevelToZero(this.body.nodes)
@@ -10564,37 +10564,37 @@
             }
             _createWrappers() {
                 var e, t;
                 this.manipulationDiv === void 0 && (this.manipulationDiv = document.createElement("div"), this.manipulationDiv.className = "vis-manipulation", this.editMode === !0 ? this.manipulationDiv.style.display = "block" : this.manipulationDiv.style.display = "none", this.canvas.frame.appendChild(this.manipulationDiv)), this.editModeDiv === void 0 && (this.editModeDiv = document.createElement("div"), this.editModeDiv.className = "vis-edit-mode", this.editMode === !0 ? this.editModeDiv.style.display = "none" : this.editModeDiv.style.display = "block", this.canvas.frame.appendChild(this.editModeDiv)), this.closeDiv === void 0 && (this.closeDiv = document.createElement("button"), this.closeDiv.className = "vis-close", this.closeDiv.setAttribute("aria-label", (t = (e = this.options.locales[this.options.locale]) == null ? void 0 : e.close) != null ? t : this.options.locales.en.close), this.closeDiv.style.display = this.manipulationDiv.style.display, this.canvas.frame.appendChild(this.closeDiv))
             }
             _getNewTargetNode(e, t) {
                 let i = D({}, this.options.controlNodeStyle);
-                i.id = "targetNode" + xe(), i.hidden = !1, i.physics = !1, i.x = e, i.y = t;
+                i.id = "targetNode" + _e(), i.hidden = !1, i.physics = !1, i.x = e, i.y = t;
                 let s = this.body.functions.createNode(i);
                 return s.shape.boundingBox = {
                     left: e,
                     right: e,
                     top: t,
                     bottom: t
                 }, s
             }
             _createEditButton() {
-                this._clean(), this.manipulationDOM = {}, ve(this.editModeDiv);
+                this._clean(), this.manipulationDOM = {}, ye(this.editModeDiv);
                 let e = this.options.locales[this.options.locale],
                     t = this._createButton("editMode", "vis-edit vis-edit-mode", e.edit || this.options.locales.en.edit);
                 this.editModeDiv.appendChild(t), this._bindElementEvents(t, this.toggleEditMode.bind(this))
             }
             _clean() {
-                this.inMode = !1, this.guiEnabled === !0 && (ve(this.editModeDiv), ve(this.manipulationDiv), this._cleanupDOMEventListeners()), this._cleanupTemporaryNodesAndEdges(), this._unbindTemporaryUIs(), this._unbindTemporaryEvents(), this.body.emitter.emit("restorePhysics")
+                this.inMode = !1, this.guiEnabled === !0 && (ye(this.editModeDiv), ye(this.manipulationDiv), this._cleanupDOMEventListeners()), this._cleanupTemporaryNodesAndEdges(), this._unbindTemporaryUIs(), this._unbindTemporaryEvents(), this.body.emitter.emit("restorePhysics")
             }
             _cleanupDOMEventListeners() {
                 for (let e of this._domEventListenerCleanupQueue.splice(0)) e()
             }
             _removeManipulationDOM() {
-                this._clean(), ve(this.manipulationDiv), ve(this.editModeDiv), ve(this.closeDiv), this.manipulationDiv && this.canvas.frame.removeChild(this.manipulationDiv), this.editModeDiv && this.canvas.frame.removeChild(this.editModeDiv), this.closeDiv && this.canvas.frame.removeChild(this.closeDiv), this.manipulationDiv = void 0, this.editModeDiv = void 0, this.closeDiv = void 0
+                this._clean(), ye(this.manipulationDiv), ye(this.editModeDiv), ye(this.closeDiv), this.manipulationDiv && this.canvas.frame.removeChild(this.manipulationDiv), this.editModeDiv && this.canvas.frame.removeChild(this.editModeDiv), this.closeDiv && this.canvas.frame.removeChild(this.closeDiv), this.manipulationDiv = void 0, this.editModeDiv = void 0, this.closeDiv = void 0
             }
             _createSeperator(e = 1) {
                 this.manipulationDOM["seperatorLineDiv" + e] = document.createElement("div"), this.manipulationDOM["seperatorLineDiv" + e].className = "vis-separator-line", this.manipulationDiv.appendChild(this.manipulationDOM["seperatorLineDiv" + e])
             }
             _createAddNodeButton(e) {
                 let t = this._createButton("addNode", "vis-add", e.addNode || this.options.locales.en.addNode);
                 this.manipulationDiv.appendChild(t), this._bindElementEvents(t, this.addNodeMode.bind(this))
@@ -10646,15 +10646,15 @@
                     let t = this.temporaryEventFunctions[e].event,
                         i = this.temporaryEventFunctions[e].boundFunction;
                     this.body.emitter.off(t, i)
                 }
                 this.temporaryEventFunctions = []
             }
             _bindElementEvents(e, t) {
-                let i = new Ue(e, {});
+                let i = new We(e, {});
                 Kt(i, t), this._domEventListenerCleanupQueue.push(() => {
                     i.destroy()
                 });
                 let s = ({
                     keyCode: o,
                     key: r
                 }) => {
@@ -10728,15 +10728,15 @@
                         i = this.selectionHandler.getNodeAt(t);
                     if (i !== void 0)
                         if (i.isCluster === !0) alert(this.options.locales[this.options.locale].createEdgeError || this.options.locales.en.createEdgeError);
                         else {
                             let s = this._getNewTargetNode(i.x, i.y);
                             this.body.nodes[s.id] = s, this.body.nodeIndices.push(s.id);
                             let o = this.body.functions.createEdge({
-                                id: "connectionEdge" + xe(),
+                                id: "connectionEdge" + _e(),
                                 from: i.id,
                                 to: s.id,
                                 physics: !1,
                                 smooth: {
                                     enabled: !0,
                                     type: "continuous",
                                     roundness: .5
@@ -10783,15 +10783,15 @@
             }
             _dragStartEdge(e) {
                 let t = this.lastTouch;
                 this.selectionHandler.generateClickEvent("dragStart", e, t, void 0, !0)
             }
             _performAddNode(e) {
                 let t = {
-                    id: xe(),
+                    id: _e(),
                     x: e.pointer.canvas.x,
                     y: e.pointer.canvas.y,
                     label: "new"
                 };
                 if (typeof this.options.addNode == "function")
                     if (this.options.addNode.length === 2) this.options.addNode(t, i => {
                         i != null && this.inMode === "addNode" && this.body.data.nodes.getDataSet().add(i), this.showManipulatorToolbar()
@@ -10823,1246 +10823,1246 @@
                     if (s.length === 2) s(i, o => {
                         o == null || this.inMode !== "editEdge" ? (this.body.edges[i.id].updateEdgeType(), this.body.emitter.emit("_redraw"), this.showManipulatorToolbar()) : (this.body.data.edges.getDataSet().update(o), this.selectionHandler.unselectAll(), this.showManipulatorToolbar())
                     });
                     else throw new Error("The function for edit does not support two arguments (data, callback)");
                 else this.body.data.edges.getDataSet().update(i), this.selectionHandler.unselectAll(), this.showManipulatorToolbar()
             }
         },
-        E = "string",
-        w = "boolean",
-        m = "number",
-        Ct = "array",
-        k = "object",
+        w = "string",
+        v = "boolean",
+        g = "number",
+        xt = "array",
+        C = "object",
         ln = "dom",
         ka = "any",
         Ri = ["arrow", "bar", "box", "circle", "crow", "curve", "diamond", "image", "inv_curve", "inv_triangle", "triangle", "vee"],
         Li = {
             borderWidth: {
-                number: m
+                number: g
             },
             borderWidthSelected: {
-                number: m,
+                number: g,
                 undefined: "undefined"
             },
             brokenImage: {
-                string: E,
+                string: w,
                 undefined: "undefined"
             },
             chosen: {
                 label: {
-                    boolean: w,
+                    boolean: v,
                     function: "function"
                 },
                 node: {
-                    boolean: w,
+                    boolean: v,
                     function: "function"
                 },
                 __type__: {
-                    object: k,
-                    boolean: w
+                    object: C,
+                    boolean: v
                 }
             },
             color: {
                 border: {
-                    string: E
+                    string: w
                 },
                 background: {
-                    string: E
+                    string: w
                 },
                 highlight: {
                     border: {
-                        string: E
+                        string: w
                     },
                     background: {
-                        string: E
+                        string: w
                     },
                     __type__: {
-                        object: k,
-                        string: E
+                        object: C,
+                        string: w
                     }
                 },
                 hover: {
                     border: {
-                        string: E
+                        string: w
                     },
                     background: {
-                        string: E
+                        string: w
                     },
                     __type__: {
-                        object: k,
-                        string: E
+                        object: C,
+                        string: w
                     }
                 },
                 __type__: {
-                    object: k,
-                    string: E
+                    object: C,
+                    string: w
                 }
             },
             opacity: {
-                number: m,
+                number: g,
                 undefined: "undefined"
             },
             fixed: {
                 x: {
-                    boolean: w
+                    boolean: v
                 },
                 y: {
-                    boolean: w
+                    boolean: v
                 },
                 __type__: {
-                    object: k,
-                    boolean: w
+                    object: C,
+                    boolean: v
                 }
             },
             font: {
                 align: {
-                    string: E
+                    string: w
                 },
                 color: {
-                    string: E
+                    string: w
                 },
                 size: {
-                    number: m
+                    number: g
                 },
                 face: {
-                    string: E
+                    string: w
                 },
                 background: {
-                    string: E
+                    string: w
                 },
                 strokeWidth: {
-                    number: m
+                    number: g
                 },
                 strokeColor: {
-                    string: E
+                    string: w
                 },
                 vadjust: {
-                    number: m
+                    number: g
                 },
                 multi: {
-                    boolean: w,
-                    string: E
+                    boolean: v,
+                    string: w
                 },
                 bold: {
                     color: {
-                        string: E
+                        string: w
                     },
                     size: {
-                        number: m
+                        number: g
                     },
                     face: {
-                        string: E
+                        string: w
                     },
                     mod: {
-                        string: E
+                        string: w
                     },
                     vadjust: {
-                        number: m
+                        number: g
                     },
                     __type__: {
-                        object: k,
-                        string: E
+                        object: C,
+                        string: w
                     }
                 },
                 boldital: {
                     color: {
-                        string: E
+                        string: w
                     },
                     size: {
-                        number: m
+                        number: g
                     },
                     face: {
-                        string: E
+                        string: w
                     },
                     mod: {
-                        string: E
+                        string: w
                     },
                     vadjust: {
-                        number: m
+                        number: g
                     },
                     __type__: {
-                        object: k,
-                        string: E
+                        object: C,
+                        string: w
                     }
                 },
                 ital: {
                     color: {
-                        string: E
+                        string: w
                     },
                     size: {
-                        number: m
+                        number: g
                     },
                     face: {
-                        string: E
+                        string: w
                     },
                     mod: {
-                        string: E
+                        string: w
                     },
                     vadjust: {
-                        number: m
+                        number: g
                     },
                     __type__: {
-                        object: k,
-                        string: E
+                        object: C,
+                        string: w
                     }
                 },
                 mono: {
                     color: {
-                        string: E
+                        string: w
                     },
                     size: {
-                        number: m
+                        number: g
                     },
                     face: {
-                        string: E
+                        string: w
                     },
                     mod: {
-                        string: E
+                        string: w
                     },
                     vadjust: {
-                        number: m
+                        number: g
                     },
                     __type__: {
-                        object: k,
-                        string: E
+                        object: C,
+                        string: w
                     }
                 },
                 __type__: {
-                    object: k,
-                    string: E
+                    object: C,
+                    string: w
                 }
             },
             group: {
-                string: E,
-                number: m,
+                string: w,
+                number: g,
                 undefined: "undefined"
             },
             heightConstraint: {
                 minimum: {
-                    number: m
+                    number: g
                 },
                 valign: {
-                    string: E
+                    string: w
                 },
                 __type__: {
-                    object: k,
-                    boolean: w,
-                    number: m
+                    object: C,
+                    boolean: v,
+                    number: g
                 }
             },
             hidden: {
-                boolean: w
+                boolean: v
             },
             icon: {
                 face: {
-                    string: E
+                    string: w
                 },
                 code: {
-                    string: E
+                    string: w
                 },
                 size: {
-                    number: m
+                    number: g
                 },
                 color: {
-                    string: E
+                    string: w
                 },
                 weight: {
-                    string: E,
-                    number: m
+                    string: w,
+                    number: g
                 },
                 __type__: {
-                    object: k
+                    object: C
                 }
             },
             id: {
-                string: E,
-                number: m
+                string: w,
+                number: g
             },
             image: {
                 selected: {
-                    string: E,
+                    string: w,
                     undefined: "undefined"
                 },
                 unselected: {
-                    string: E,
+                    string: w,
                     undefined: "undefined"
                 },
                 __type__: {
-                    object: k,
-                    string: E
+                    object: C,
+                    string: w
                 }
             },
             imagePadding: {
                 top: {
-                    number: m
+                    number: g
                 },
                 right: {
-                    number: m
+                    number: g
                 },
                 bottom: {
-                    number: m
+                    number: g
                 },
                 left: {
-                    number: m
+                    number: g
                 },
                 __type__: {
-                    object: k,
-                    number: m
+                    object: C,
+                    number: g
                 }
             },
             label: {
-                string: E,
+                string: w,
                 undefined: "undefined"
             },
             labelHighlightBold: {
-                boolean: w
+                boolean: v
             },
             level: {
-                number: m,
+                number: g,
                 undefined: "undefined"
             },
             margin: {
                 top: {
-                    number: m
+                    number: g
                 },
                 right: {
-                    number: m
+                    number: g
                 },
                 bottom: {
-                    number: m
+                    number: g
                 },
                 left: {
-                    number: m
+                    number: g
                 },
                 __type__: {
-                    object: k,
-                    number: m
+                    object: C,
+                    number: g
                 }
             },
             mass: {
-                number: m
+                number: g
             },
             physics: {
-                boolean: w
+                boolean: v
             },
             scaling: {
                 min: {
-                    number: m
+                    number: g
                 },
                 max: {
-                    number: m
+                    number: g
                 },
                 label: {
                     enabled: {
-                        boolean: w
+                        boolean: v
                     },
                     min: {
-                        number: m
+                        number: g
                     },
                     max: {
-                        number: m
+                        number: g
                     },
                     maxVisible: {
-                        number: m
+                        number: g
                     },
                     drawThreshold: {
-                        number: m
+                        number: g
                     },
                     __type__: {
-                        object: k,
-                        boolean: w
+                        object: C,
+                        boolean: v
                     }
                 },
                 customScalingFunction: {
                     function: "function"
                 },
                 __type__: {
-                    object: k
+                    object: C
                 }
             },
             shadow: {
                 enabled: {
-                    boolean: w
+                    boolean: v
                 },
                 color: {
-                    string: E
+                    string: w
                 },
                 size: {
-                    number: m
+                    number: g
                 },
                 x: {
-                    number: m
+                    number: g
                 },
                 y: {
-                    number: m
+                    number: g
                 },
                 __type__: {
-                    object: k,
-                    boolean: w
+                    object: C,
+                    boolean: v
                 }
             },
             shape: {
                 string: ["custom", "ellipse", "circle", "database", "box", "text", "image", "circularImage", "diamond", "dot", "star", "triangle", "triangleDown", "square", "icon", "hexagon"]
             },
             ctxRenderer: {
                 function: "function"
             },
             shapeProperties: {
                 borderDashes: {
-                    boolean: w,
-                    array: Ct
+                    boolean: v,
+                    array: xt
                 },
                 borderRadius: {
-                    number: m
+                    number: g
                 },
                 interpolation: {
-                    boolean: w
+                    boolean: v
                 },
                 useImageSize: {
-                    boolean: w
+                    boolean: v
                 },
                 useBorderWithImage: {
-                    boolean: w
+                    boolean: v
                 },
                 coordinateOrigin: {
                     string: ["center", "top-left"]
                 },
                 __type__: {
-                    object: k
+                    object: C
                 }
             },
             size: {
-                number: m
+                number: g
             },
             title: {
-                string: E,
+                string: w,
                 dom: ln,
                 undefined: "undefined"
             },
             value: {
-                number: m,
+                number: g,
                 undefined: "undefined"
             },
             widthConstraint: {
                 minimum: {
-                    number: m
+                    number: g
                 },
                 maximum: {
-                    number: m
+                    number: g
                 },
                 __type__: {
-                    object: k,
-                    boolean: w,
-                    number: m
+                    object: C,
+                    boolean: v,
+                    number: g
                 }
             },
             x: {
-                number: m
+                number: g
             },
             y: {
-                number: m
+                number: g
             },
             __type__: {
-                object: k
+                object: C
             }
         },
         Oa = {
             configure: {
                 enabled: {
-                    boolean: w
+                    boolean: v
                 },
                 filter: {
-                    boolean: w,
-                    string: E,
-                    array: Ct,
+                    boolean: v,
+                    string: w,
+                    array: xt,
                     function: "function"
                 },
                 container: {
                     dom: ln
                 },
                 showButton: {
-                    boolean: w
+                    boolean: v
                 },
                 __type__: {
-                    object: k,
-                    boolean: w,
-                    string: E,
-                    array: Ct,
+                    object: C,
+                    boolean: v,
+                    string: w,
+                    array: xt,
                     function: "function"
                 }
             },
             edges: {
                 arrows: {
                     to: {
                         enabled: {
-                            boolean: w
+                            boolean: v
                         },
                         scaleFactor: {
-                            number: m
+                            number: g
                         },
                         type: {
                             string: Ri
                         },
                         imageHeight: {
-                            number: m
+                            number: g
                         },
                         imageWidth: {
-                            number: m
+                            number: g
                         },
                         src: {
-                            string: E
+                            string: w
                         },
                         __type__: {
-                            object: k,
-                            boolean: w
+                            object: C,
+                            boolean: v
                         }
                     },
                     middle: {
                         enabled: {
-                            boolean: w
+                            boolean: v
                         },
                         scaleFactor: {
-                            number: m
+                            number: g
                         },
                         type: {
                             string: Ri
                         },
                         imageWidth: {
-                            number: m
+                            number: g
                         },
                         imageHeight: {
-                            number: m
+                            number: g
                         },
                         src: {
-                            string: E
+                            string: w
                         },
                         __type__: {
-                            object: k,
-                            boolean: w
+                            object: C,
+                            boolean: v
                         }
                     },
                     from: {
                         enabled: {
-                            boolean: w
+                            boolean: v
                         },
                         scaleFactor: {
-                            number: m
+                            number: g
                         },
                         type: {
                             string: Ri
                         },
                         imageWidth: {
-                            number: m
+                            number: g
                         },
                         imageHeight: {
-                            number: m
+                            number: g
                         },
                         src: {
-                            string: E
+                            string: w
                         },
                         __type__: {
-                            object: k,
-                            boolean: w
+                            object: C,
+                            boolean: v
                         }
                     },
                     __type__: {
                         string: ["from", "to", "middle"],
-                        object: k
+                        object: C
                     }
                 },
                 endPointOffset: {
                     from: {
-                        number: m
+                        number: g
                     },
                     to: {
-                        number: m
+                        number: g
                     },
                     __type__: {
-                        object: k,
-                        number: m
+                        object: C,
+                        number: g
                     }
                 },
                 arrowStrikethrough: {
-                    boolean: w
+                    boolean: v
                 },
                 background: {
                     enabled: {
-                        boolean: w
+                        boolean: v
                     },
                     color: {
-                        string: E
+                        string: w
                     },
                     size: {
-                        number: m
+                        number: g
                     },
                     dashes: {
-                        boolean: w,
-                        array: Ct
+                        boolean: v,
+                        array: xt
                     },
                     __type__: {
-                        object: k,
-                        boolean: w
+                        object: C,
+                        boolean: v
                     }
                 },
                 chosen: {
                     label: {
-                        boolean: w,
+                        boolean: v,
                         function: "function"
                     },
                     edge: {
-                        boolean: w,
+                        boolean: v,
                         function: "function"
                     },
                     __type__: {
-                        object: k,
-                        boolean: w
+                        object: C,
+                        boolean: v
                     }
                 },
                 color: {
                     color: {
-                        string: E
+                        string: w
                     },
                     highlight: {
-                        string: E
+                        string: w
                     },
                     hover: {
-                        string: E
+                        string: w
                     },
                     inherit: {
                         string: ["from", "to", "both"],
-                        boolean: w
+                        boolean: v
                     },
                     opacity: {
-                        number: m
+                        number: g
                     },
                     __type__: {
-                        object: k,
-                        string: E
+                        object: C,
+                        string: w
                     }
                 },
                 dashes: {
-                    boolean: w,
-                    array: Ct
+                    boolean: v,
+                    array: xt
                 },
                 font: {
                     color: {
-                        string: E
+                        string: w
                     },
                     size: {
-                        number: m
+                        number: g
                     },
                     face: {
-                        string: E
+                        string: w
                     },
                     background: {
-                        string: E
+                        string: w
                     },
                     strokeWidth: {
-                        number: m
+                        number: g
                     },
                     strokeColor: {
-                        string: E
+                        string: w
                     },
                     align: {
                         string: ["horizontal", "top", "middle", "bottom"]
                     },
                     vadjust: {
-                        number: m
+                        number: g
                     },
                     multi: {
-                        boolean: w,
-                        string: E
+                        boolean: v,
+                        string: w
                     },
                     bold: {
                         color: {
-                            string: E
+                            string: w
                         },
                         size: {
-                            number: m
+                            number: g
                         },
                         face: {
-                            string: E
+                            string: w
                         },
                         mod: {
-                            string: E
+                            string: w
                         },
                         vadjust: {
-                            number: m
+                            number: g
                         },
                         __type__: {
-                            object: k,
-                            string: E
+                            object: C,
+                            string: w
                         }
                     },
                     boldital: {
                         color: {
-                            string: E
+                            string: w
                         },
                         size: {
-                            number: m
+                            number: g
                         },
                         face: {
-                            string: E
+                            string: w
                         },
                         mod: {
-                            string: E
+                            string: w
                         },
                         vadjust: {
-                            number: m
+                            number: g
                         },
                         __type__: {
-                            object: k,
-                            string: E
+                            object: C,
+                            string: w
                         }
                     },
                     ital: {
                         color: {
-                            string: E
+                            string: w
                         },
                         size: {
-                            number: m
+                            number: g
                         },
                         face: {
-                            string: E
+                            string: w
                         },
                         mod: {
-                            string: E
+                            string: w
                         },
                         vadjust: {
-                            number: m
+                            number: g
                         },
                         __type__: {
-                            object: k,
-                            string: E
+                            object: C,
+                            string: w
                         }
                     },
                     mono: {
                         color: {
-                            string: E
+                            string: w
                         },
                         size: {
-                            number: m
+                            number: g
                         },
                         face: {
-                            string: E
+                            string: w
                         },
                         mod: {
-                            string: E
+                            string: w
                         },
                         vadjust: {
-                            number: m
+                            number: g
                         },
                         __type__: {
-                            object: k,
-                            string: E
+                            object: C,
+                            string: w
                         }
                     },
                     __type__: {
-                        object: k,
-                        string: E
+                        object: C,
+                        string: w
                     }
                 },
                 hidden: {
-                    boolean: w
+                    boolean: v
                 },
                 hoverWidth: {
                     function: "function",
-                    number: m
+                    number: g
                 },
                 label: {
-                    string: E,
+                    string: w,
                     undefined: "undefined"
                 },
                 labelHighlightBold: {
-                    boolean: w
+                    boolean: v
                 },
                 length: {
-                    number: m,
+                    number: g,
                     undefined: "undefined"
                 },
                 physics: {
-                    boolean: w
+                    boolean: v
                 },
                 scaling: {
                     min: {
-                        number: m
+                        number: g
                     },
                     max: {
-                        number: m
+                        number: g
                     },
                     label: {
                         enabled: {
-                            boolean: w
+                            boolean: v
                         },
                         min: {
-                            number: m
+                            number: g
                         },
                         max: {
-                            number: m
+                            number: g
                         },
                         maxVisible: {
-                            number: m
+                            number: g
                         },
                         drawThreshold: {
-                            number: m
+                            number: g
                         },
                         __type__: {
-                            object: k,
-                            boolean: w
+                            object: C,
+                            boolean: v
                         }
                     },
                     customScalingFunction: {
                         function: "function"
                     },
                     __type__: {
-                        object: k
+                        object: C
                     }
                 },
                 selectionWidth: {
                     function: "function",
-                    number: m
+                    number: g
                 },
                 selfReferenceSize: {
-                    number: m
+                    number: g
                 },
                 selfReference: {
                     size: {
-                        number: m
+                        number: g
                     },
                     angle: {
-                        number: m
+                        number: g
                     },
                     renderBehindTheNode: {
-                        boolean: w
+                        boolean: v
                     },
                     __type__: {
-                        object: k
+                        object: C
                     }
                 },
                 shadow: {
                     enabled: {
-                        boolean: w
+                        boolean: v
                     },
                     color: {
-                        string: E
+                        string: w
                     },
                     size: {
-                        number: m
+                        number: g
                     },
                     x: {
-                        number: m
+                        number: g
                     },
                     y: {
-                        number: m
+                        number: g
                     },
                     __type__: {
-                        object: k,
-                        boolean: w
+                        object: C,
+                        boolean: v
                     }
                 },
                 smooth: {
                     enabled: {
-                        boolean: w
+                        boolean: v
                     },
                     type: {
                         string: ["dynamic", "continuous", "discrete", "diagonalCross", "straightCross", "horizontal", "vertical", "curvedCW", "curvedCCW", "cubicBezier"]
                     },
                     roundness: {
-                        number: m
+                        number: g
                     },
                     forceDirection: {
                         string: ["horizontal", "vertical", "none"],
-                        boolean: w
+                        boolean: v
                     },
                     __type__: {
-                        object: k,
-                        boolean: w
+                        object: C,
+                        boolean: v
                     }
                 },
                 title: {
-                    string: E,
+                    string: w,
                     undefined: "undefined"
                 },
                 width: {
-                    number: m
+                    number: g
                 },
                 widthConstraint: {
                     maximum: {
-                        number: m
+                        number: g
                     },
                     __type__: {
-                        object: k,
-                        boolean: w,
-                        number: m
+                        object: C,
+                        boolean: v,
+                        number: g
                     }
                 },
                 value: {
-                    number: m,
+                    number: g,
                     undefined: "undefined"
                 },
                 __type__: {
-                    object: k
+                    object: C
                 }
             },
             groups: {
                 useDefaultGroups: {
-                    boolean: w
+                    boolean: v
                 },
                 __any__: Li,
                 __type__: {
-                    object: k
+                    object: C
                 }
             },
             interaction: {
                 dragNodes: {
-                    boolean: w
+                    boolean: v
                 },
                 dragView: {
-                    boolean: w
+                    boolean: v
                 },
                 hideEdgesOnDrag: {
-                    boolean: w
+                    boolean: v
                 },
                 hideEdgesOnZoom: {
-                    boolean: w
+                    boolean: v
                 },
                 hideNodesOnDrag: {
-                    boolean: w
+                    boolean: v
                 },
                 hover: {
-                    boolean: w
+                    boolean: v
                 },
                 keyboard: {
                     enabled: {
-                        boolean: w
+                        boolean: v
                     },
                     speed: {
                         x: {
-                            number: m
+                            number: g
                         },
                         y: {
-                            number: m
+                            number: g
                         },
                         zoom: {
-                            number: m
+                            number: g
                         },
                         __type__: {
-                            object: k
+                            object: C
                         }
                     },
                     bindToWindow: {
-                        boolean: w
+                        boolean: v
                     },
                     autoFocus: {
-                        boolean: w
+                        boolean: v
                     },
                     __type__: {
-                        object: k,
-                        boolean: w
+                        object: C,
+                        boolean: v
                     }
                 },
                 multiselect: {
-                    boolean: w
+                    boolean: v
                 },
                 navigationButtons: {
-                    boolean: w
+                    boolean: v
                 },
                 selectable: {
-                    boolean: w
+                    boolean: v
                 },
                 selectConnectedEdges: {
-                    boolean: w
+                    boolean: v
                 },
                 hoverConnectedEdges: {
-                    boolean: w
+                    boolean: v
                 },
                 tooltipDelay: {
-                    number: m
+                    number: g
                 },
                 zoomView: {
-                    boolean: w
+                    boolean: v
                 },
                 zoomSpeed: {
-                    number: m
+                    number: g
                 },
                 __type__: {
-                    object: k
+                    object: C
                 }
             },
             layout: {
                 randomSeed: {
                     undefined: "undefined",
-                    number: m,
-                    string: E
+                    number: g,
+                    string: w
                 },
                 improvedLayout: {
-                    boolean: w
+                    boolean: v
                 },
                 clusterThreshold: {
-                    number: m
+                    number: g
                 },
                 hierarchical: {
                     enabled: {
-                        boolean: w
+                        boolean: v
                     },
                     levelSeparation: {
-                        number: m
+                        number: g
                     },
                     nodeSpacing: {
-                        number: m
+                        number: g
                     },
                     treeSpacing: {
-                        number: m
+                        number: g
                     },
                     blockShifting: {
-                        boolean: w
+                        boolean: v
                     },
                     edgeMinimization: {
-                        boolean: w
+                        boolean: v
                     },
                     parentCentralization: {
-                        boolean: w
+                        boolean: v
                     },
                     direction: {
                         string: ["UD", "DU", "LR", "RL"]
                     },
                     sortMethod: {
                         string: ["hubsize", "directed"]
                     },
                     shakeTowards: {
                         string: ["leaves", "roots"]
                     },
                     __type__: {
-                        object: k,
-                        boolean: w
+                        object: C,
+                        boolean: v
                     }
                 },
                 __type__: {
-                    object: k
+                    object: C
                 }
             },
             manipulation: {
                 enabled: {
-                    boolean: w
+                    boolean: v
                 },
                 initiallyActive: {
-                    boolean: w
+                    boolean: v
                 },
                 addNode: {
-                    boolean: w,
+                    boolean: v,
                     function: "function"
                 },
                 addEdge: {
-                    boolean: w,
+                    boolean: v,
                     function: "function"
                 },
                 editNode: {
                     function: "function"
                 },
                 editEdge: {
                     editWithoutDrag: {
                         function: "function"
                     },
                     __type__: {
-                        object: k,
-                        boolean: w,
+                        object: C,
+                        boolean: v,
                         function: "function"
                     }
                 },
                 deleteNode: {
-                    boolean: w,
+                    boolean: v,
                     function: "function"
                 },
                 deleteEdge: {
-                    boolean: w,
+                    boolean: v,
                     function: "function"
                 },
                 controlNodeStyle: Li,
                 __type__: {
-                    object: k,
-                    boolean: w
+                    object: C,
+                    boolean: v
                 }
             },
             nodes: Li,
             physics: {
                 enabled: {
-                    boolean: w
+                    boolean: v
                 },
                 barnesHut: {
                     theta: {
-                        number: m
+                        number: g
                     },
                     gravitationalConstant: {
-                        number: m
+                        number: g
                     },
                     centralGravity: {
-                        number: m
+                        number: g
                     },
                     springLength: {
-                        number: m
+                        number: g
                     },
                     springConstant: {
-                        number: m
+                        number: g
                     },
                     damping: {
-                        number: m
+                        number: g
                     },
                     avoidOverlap: {
-                        number: m
+                        number: g
                     },
                     __type__: {
-                        object: k
+                        object: C
                     }
                 },
                 forceAtlas2Based: {
                     theta: {
-                        number: m
+                        number: g
                     },
                     gravitationalConstant: {
-                        number: m
+                        number: g
                     },
                     centralGravity: {
-                        number: m
+                        number: g
                     },
                     springLength: {
-                        number: m
+                        number: g
                     },
                     springConstant: {
-                        number: m
+                        number: g
                     },
                     damping: {
-                        number: m
+                        number: g
                     },
                     avoidOverlap: {
-                        number: m
+                        number: g
                     },
                     __type__: {
-                        object: k
+                        object: C
                     }
                 },
                 repulsion: {
                     centralGravity: {
-                        number: m
+                        number: g
                     },
                     springLength: {
-                        number: m
+                        number: g
                     },
                     springConstant: {
-                        number: m
+                        number: g
                     },
                     nodeDistance: {
-                        number: m
+                        number: g
                     },
                     damping: {
-                        number: m
+                        number: g
                     },
                     __type__: {
-                        object: k
+                        object: C
                     }
                 },
                 hierarchicalRepulsion: {
                     centralGravity: {
-                        number: m
+                        number: g
                     },
                     springLength: {
-                        number: m
+                        number: g
                     },
                     springConstant: {
-                        number: m
+                        number: g
                     },
                     nodeDistance: {
-                        number: m
+                        number: g
                     },
                     damping: {
-                        number: m
+                        number: g
                     },
                     avoidOverlap: {
-                        number: m
+                        number: g
                     },
                     __type__: {
-                        object: k
+                        object: C
                     }
                 },
                 maxVelocity: {
-                    number: m
+                    number: g
                 },
                 minVelocity: {
-                    number: m
+                    number: g
                 },
                 solver: {
                     string: ["barnesHut", "repulsion", "hierarchicalRepulsion", "forceAtlas2Based"]
                 },
                 stabilization: {
                     enabled: {
-                        boolean: w
+                        boolean: v
                     },
                     iterations: {
-                        number: m
+                        number: g
                     },
                     updateInterval: {
-                        number: m
+                        number: g
                     },
                     onlyDynamicEdges: {
-                        boolean: w
+                        boolean: v
                     },
                     fit: {
-                        boolean: w
+                        boolean: v
                     },
                     __type__: {
-                        object: k,
-                        boolean: w
+                        object: C,
+                        boolean: v
                     }
                 },
                 timestep: {
-                    number: m
+                    number: g
                 },
                 adaptiveTimestep: {
-                    boolean: w
+                    boolean: v
                 },
                 wind: {
                     x: {
-                        number: m
+                        number: g
                     },
                     y: {
-                        number: m
+                        number: g
                     },
                     __type__: {
-                        object: k
+                        object: C
                     }
                 },
                 __type__: {
-                    object: k,
-                    boolean: w
+                    object: C,
+                    boolean: v
                 }
             },
             autoResize: {
-                boolean: w
+                boolean: v
             },
             clickToUse: {
-                boolean: w
+                boolean: v
             },
             locale: {
-                string: E
+                string: w
             },
             locales: {
                 __any__: {
                     any: ka
                 },
                 __type__: {
-                    object: k
+                    object: C
                 }
             },
             height: {
-                string: E
+                string: w
             },
             width: {
-                string: E
+                string: w
             },
             __type__: {
-                object: k
+                object: C
             }
         },
         cn = {
             nodes: {
                 borderWidth: [1, 0, 10, 1],
                 borderWidthSelected: [2, 0, 10, 1],
                 color: {
@@ -12306,18 +12306,18 @@
                 for (let a = 0; a < r; a++) {
                     let d = t[a],
                         h = s[d];
                     for (let l = 0; l < r - 1; l++) {
                         let c = t[l],
                             u = s[c];
                         for (let f = l + 1; f < r; f++) {
-                            let y = t[f],
-                                v = s[y],
-                                g = Math.min(u[y], u[d] + h[y]);
-                            u[y] = g, v[c] = g
+                            let m = t[f],
+                                b = s[m],
+                                p = Math.min(u[m], u[d] + h[m]);
+                            u[m] = p, b[c] = p
                         }
                     }
                 }
                 return s
             }
         },
         fn = class {
@@ -12335,18 +12335,18 @@
                     a = 0,
                     d = Math.max(1e3, Math.min(10 * this.body.nodeIndices.length, 6e3)),
                     h = 5,
                     l = 1e9,
                     c = 0,
                     u = 0,
                     f = 0,
-                    y = 0,
-                    v = 0;
+                    m = 0,
+                    b = 0;
                 for (; l > o && a < d;)
-                    for (a += 1, [c, l, u, f] = this._getHighestEnergyNode(i), y = l, v = 0; y > r && v < h;) v += 1, this._moveNode(c, u, f), [y, u, f] = this._getEnergy(c)
+                    for (a += 1, [c, l, u, f] = this._getHighestEnergyNode(i), m = l, b = 0; m > r && b < h;) b += 1, this._moveNode(c, u, f), [m, u, f] = this._getEnergy(c)
             }
             _getHighestEnergyNode(e) {
                 let t = this.body.nodeIndices,
                     i = this.body.nodes,
                     s = 0,
                     o = t[0],
                     r = 0,
@@ -12370,33 +12370,33 @@
                     r = 0,
                     a = 0,
                     d = 0,
                     h = o[e].x,
                     l = o[e].y,
                     c = this.K_matrix[e],
                     u = this.L_matrix[e];
-                for (let C = 0; C < s.length; C++) {
-                    let x = s[C];
-                    if (x !== e) {
-                        let O = o[x].x,
-                            M = o[x].y,
-                            R = c[x],
-                            q = u[x],
-                            oe = 1 / ((h - O) ** 2 + (l - M) ** 2) ** 1.5;
-                        r += R * (1 - q * (l - M) ** 2 * oe), a += R * (q * (h - O) * (l - M) * oe), d += R * (1 - q * (h - O) ** 2 * oe)
+                for (let T = 0; T < s.length; T++) {
+                    let O = s[T];
+                    if (O !== e) {
+                        let S = o[O].x,
+                            A = o[O].y,
+                            H = c[O],
+                            G = u[O],
+                            le = 1 / ((h - S) ** 2 + (l - A) ** 2) ** 1.5;
+                        r += H * (1 - G * (l - A) ** 2 * le), a += H * (G * (h - S) * (l - A) * le), d += H * (1 - G * (h - S) ** 2 * le)
                     }
                 }
                 let f = r,
-                    y = a,
-                    v = t,
-                    g = d,
-                    p = i,
-                    b = (v / f + p / y) / (y / f - g / y),
-                    _ = -(y * b + v) / f;
-                o[e].x += _, o[e].y += b, this._updateE_matrix(e)
+                    m = a,
+                    b = t,
+                    p = d,
+                    y = i,
+                    _ = (b / f + y / m) / (m / f - p / m),
+                    x = -(m * _ + b) / f;
+                o[e].x += x, o[e].y += _, this._updateE_matrix(e)
             }
             _createL_matrix(e) {
                 let t = this.body.nodeIndices,
                     i = this.springLength;
                 this.L_matrix = [];
                 for (let s = 0; s < t.length; s++) {
                     this.L_matrix[t[s]] = {};
@@ -12445,32 +12445,32 @@
                     d = i[e].y,
                     h = 0,
                     l = 0;
                 for (let c = 0; c < t.length; c++) {
                     let u = t[c];
                     if (u !== e) {
                         let f = s[c],
-                            y = f[0],
-                            v = f[1],
-                            g = i[u].x,
-                            p = i[u].y,
-                            b = 1 / Math.sqrt((a - g) ** 2 + (d - p) ** 2),
-                            _ = o[u] * (a - g - r[u] * (a - g) * b),
-                            C = o[u] * (d - p - r[u] * (d - p) * b);
-                        s[c] = [_, C], h += _, l += C;
-                        let x = this.E_sums[u];
-                        x[0] += _ - y, x[1] += C - v
+                            m = f[0],
+                            b = f[1],
+                            p = i[u].x,
+                            y = i[u].y,
+                            _ = 1 / Math.sqrt((a - p) ** 2 + (d - y) ** 2),
+                            x = o[u] * (a - p - r[u] * (a - p) * _),
+                            T = o[u] * (d - y - r[u] * (d - y) * _);
+                        s[c] = [x, T], h += x, l += T;
+                        let O = this.E_sums[u];
+                        O[0] += x - m, O[1] += T - b
                     }
                 }
                 this.E_sums[e] = [h, l]
             }
         };
 
-    function T(n, e, t) {
-        if (!(this instanceof T)) throw new SyntaxError("Constructor must be called with the new operator");
+    function E(n, e, t) {
+        if (!(this instanceof E)) throw new SyntaxError("Constructor must be called with the new operator");
         this.options = {}, this.defaultOptions = {
             locale: "en",
             locales: ua,
             clickToUse: !1
         }, Object.assign(this.options, this.defaultOptions), this.body = {
             container: n,
             nodes: {},
@@ -12524,18 +12524,18 @@
                     end: {
                         x: 0,
                         y: 0
                     }
                 }
             }
         }, this.bindEventListeners(), this.images = new co(() => this.body.emitter.emit("_requestRedraw")), this.groups = new uo, this.canvas = new $o(this.body), this.selectionHandler = new sn(this.body, this.canvas), this.interactionHandler = new Jo(this.body, this.canvas, this.selectionHandler), this.view = new Zo(this.body, this.canvas), this.renderer = new Go(this.body, this.canvas), this.physics = new Uo(this.body), this.layoutEngine = new dn(this.body), this.clustering = new Xo(this.body), this.manipulation = new hn(this.body, this.canvas, this.selectionHandler, this.interactionHandler), this.nodesHandler = new ko(this.body, this.images, this.groups, this.layoutEngine), this.edgesHandler = new Lo(this.body, this.images, this.groups), this.body.modules.kamadaKawai = new fn(this.body, 150, .05), this.body.modules.clustering = this.clustering, this.canvas._create(), this.setOptions(t), this.setData(e)
-    }(0, Gs.default)(T.prototype);
-    T.prototype.setOptions = function(n) {
+    }(0, Gs.default)(E.prototype);
+    E.prototype.setOptions = function(n) {
         if (n === null && (n = void 0), n !== void 0) {
-            if (Vs.validate(n, Oa) === !0 && console.error("%cErrors have been found in the supplied options object.", yi), qe(["locale", "locales", "clickToUse"], this.options, n), n.locale !== void 0 && (n.locale = fa(n.locales || this.options.locales, n.locale)), n = this.layoutEngine.setOptions(n.layout, n), this.canvas.setOptions(n), this.groups.setOptions(n.groups), this.nodesHandler.setOptions(n.nodes), this.edgesHandler.setOptions(n.edges), this.physics.setOptions(n.physics), this.manipulation.setOptions(n.manipulation, n, this.options), this.interactionHandler.setOptions(n.interaction), this.renderer.setOptions(n.interaction), this.selectionHandler.setOptions(n.interaction), n.groups !== void 0 && this.body.emitter.emit("refreshNodes"), "configure" in n && (this.configurator || (this.configurator = new js(this, this.body.container, cn, this.canvas.pixelRatio, Sa)), this.configurator.setOptions(n.configure)), this.configurator && this.configurator.options.enabled === !0) {
+            if (Vs.validate(n, Oa) === !0 && console.error("%cErrors have been found in the supplied options object.", yi), je(["locale", "locales", "clickToUse"], this.options, n), n.locale !== void 0 && (n.locale = fa(n.locales || this.options.locales, n.locale)), n = this.layoutEngine.setOptions(n.layout, n), this.canvas.setOptions(n), this.groups.setOptions(n.groups), this.nodesHandler.setOptions(n.nodes), this.edgesHandler.setOptions(n.edges), this.physics.setOptions(n.physics), this.manipulation.setOptions(n.manipulation, n, this.options), this.interactionHandler.setOptions(n.interaction), this.renderer.setOptions(n.interaction), this.selectionHandler.setOptions(n.interaction), n.groups !== void 0 && this.body.emitter.emit("refreshNodes"), "configure" in n && (this.configurator || (this.configurator = new js(this, this.body.container, cn, this.canvas.pixelRatio, Sa)), this.configurator.setOptions(n.configure)), this.configurator && this.configurator.options.enabled === !0) {
                 let i = {
                     nodes: {},
                     edges: {},
                     layout: {},
                     interaction: {},
                     manipulation: {},
                     physics: {},
@@ -12544,224 +12544,224 @@
                 D(i.nodes, this.nodesHandler.options), D(i.edges, this.edgesHandler.options), D(i.layout, this.layoutEngine.options), D(i.interaction, this.selectionHandler.options), D(i.interaction, this.renderer.options), D(i.interaction, this.interactionHandler.options), D(i.manipulation, this.manipulation.options), D(i.physics, this.physics.options), D(i.global, this.canvas.options), D(i.global, this.options), this.configurator.setModuleOptions(i)
             }
             n.clickToUse !== void 0 ? n.clickToUse === !0 ? this.activator === void 0 && (this.activator = new Hs(this.canvas.frame), this.activator.on("change", () => {
                 this.body.emitter.emit("activate")
             })) : (this.activator !== void 0 && (this.activator.destroy(), delete this.activator), this.body.emitter.emit("activate")) : this.body.emitter.emit("activate"), this.canvas.setSize(), this.body.emitter.emit("startSimulation")
         }
     };
-    T.prototype._updateVisibleIndices = function() {
+    E.prototype._updateVisibleIndices = function() {
         let n = this.body.nodes,
             e = this.body.edges;
         this.body.nodeIndices = [], this.body.edgeIndices = [];
         for (let t in n) Object.prototype.hasOwnProperty.call(n, t) && !this.clustering._isClusteredNode(t) && n[t].options.hidden === !1 && this.body.nodeIndices.push(n[t].id);
         for (let t in e)
             if (Object.prototype.hasOwnProperty.call(e, t)) {
                 let i = e[t],
                     s = n[i.fromId],
                     o = n[i.toId],
                     r = s !== void 0 && o !== void 0;
                 !this.clustering._isClusteredEdge(t) && i.options.hidden === !1 && r && s.options.hidden === !1 && o.options.hidden === !1 && this.body.edgeIndices.push(i.id)
             }
     };
-    T.prototype.bindEventListeners = function() {
+    E.prototype.bindEventListeners = function() {
         this.body.emitter.on("_dataChanged", () => {
             this.edgesHandler._updateState(), this.body.emitter.emit("_dataUpdated")
         }), this.body.emitter.on("_dataUpdated", () => {
             this.clustering._updateState(), this._updateVisibleIndices(), this._updateValueRange(this.body.nodes), this._updateValueRange(this.body.edges), this.body.emitter.emit("startSimulation"), this.body.emitter.emit("_requestRedraw")
         })
     };
-    T.prototype.setData = function(n) {
+    E.prototype.setData = function(n) {
         if (this.body.emitter.emit("resetPhysics"), this.body.emitter.emit("_resetData"), this.selectionHandler.unselectAll(), n && n.dot && (n.nodes || n.edges)) throw new SyntaxError('Data must contain either parameter "dot" or  parameter pair "nodes" and "edges", but not both.');
         if (this.setOptions(n && n.options), n && n.dot) {
             console.warn("The dot property has been deprecated. Please use the static convertDot method to convert DOT into vis.network format and use the normal data format with nodes and edges. This converter is used like this: var data = vis.network.convertDot(dotString);");
             let e = Jr(n.dot);
             this.setData(e);
             return
         } else if (n && n.gephi) {
             console.warn("The gephi property has been deprecated. Please use the static convertGephi method to convert gephi into vis.network format and use the normal data format with nodes and edges. This converter is used like this: var data = vis.network.convertGephi(gephiJson);");
             let e = ea(n.gephi);
             this.setData(e);
             return
         } else this.nodesHandler.setData(n && n.nodes, !0), this.edgesHandler.setData(n && n.edges, !0);
         this.body.emitter.emit("_dataChanged"), this.body.emitter.emit("_dataLoaded"), this.body.emitter.emit("initPhysics")
     };
-    T.prototype.destroy = function() {
+    E.prototype.destroy = function() {
         this.body.emitter.emit("destroy"), this.body.emitter.off(), this.off(), delete this.groups, delete this.canvas, delete this.selectionHandler, delete this.interactionHandler, delete this.view, delete this.renderer, delete this.physics, delete this.layoutEngine, delete this.clustering, delete this.manipulation, delete this.nodesHandler, delete this.edgesHandler, delete this.configurator, delete this.images;
         for (let n in this.body.nodes) !Object.prototype.hasOwnProperty.call(this.body.nodes, n) || delete this.body.nodes[n];
         for (let n in this.body.edges) !Object.prototype.hasOwnProperty.call(this.body.edges, n) || delete this.body.edges[n];
-        ve(this.body.container)
+        ye(this.body.container)
     };
-    T.prototype._updateValueRange = function(n) {
+    E.prototype._updateValueRange = function(n) {
         let e, t, i, s = 0;
         for (e in n)
             if (Object.prototype.hasOwnProperty.call(n, e)) {
                 let o = n[e].getValue();
                 o !== void 0 && (t = t === void 0 ? o : Math.min(o, t), i = i === void 0 ? o : Math.max(o, i), s += o)
             } if (t !== void 0 && i !== void 0)
             for (e in n) Object.prototype.hasOwnProperty.call(n, e) && n[e].setValueRange(t, i, s)
     };
-    T.prototype.isActive = function() {
+    E.prototype.isActive = function() {
         return !this.activator || this.activator.active
     };
-    T.prototype.setSize = function() {
+    E.prototype.setSize = function() {
         return this.canvas.setSize.apply(this.canvas, arguments)
     };
-    T.prototype.canvasToDOM = function() {
+    E.prototype.canvasToDOM = function() {
         return this.canvas.canvasToDOM.apply(this.canvas, arguments)
     };
-    T.prototype.DOMtoCanvas = function() {
+    E.prototype.DOMtoCanvas = function() {
         return this.canvas.DOMtoCanvas.apply(this.canvas, arguments)
     };
-    T.prototype.findNode = function() {
+    E.prototype.findNode = function() {
         return this.clustering.findNode.apply(this.clustering, arguments)
     };
-    T.prototype.isCluster = function() {
+    E.prototype.isCluster = function() {
         return this.clustering.isCluster.apply(this.clustering, arguments)
     };
-    T.prototype.openCluster = function() {
+    E.prototype.openCluster = function() {
         return this.clustering.openCluster.apply(this.clustering, arguments)
     };
-    T.prototype.cluster = function() {
+    E.prototype.cluster = function() {
         return this.clustering.cluster.apply(this.clustering, arguments)
     };
-    T.prototype.getNodesInCluster = function() {
+    E.prototype.getNodesInCluster = function() {
         return this.clustering.getNodesInCluster.apply(this.clustering, arguments)
     };
-    T.prototype.clusterByConnection = function() {
+    E.prototype.clusterByConnection = function() {
         return this.clustering.clusterByConnection.apply(this.clustering, arguments)
     };
-    T.prototype.clusterByHubsize = function() {
+    E.prototype.clusterByHubsize = function() {
         return this.clustering.clusterByHubsize.apply(this.clustering, arguments)
     };
-    T.prototype.updateClusteredNode = function() {
+    E.prototype.updateClusteredNode = function() {
         return this.clustering.updateClusteredNode.apply(this.clustering, arguments)
     };
-    T.prototype.getClusteredEdges = function() {
+    E.prototype.getClusteredEdges = function() {
         return this.clustering.getClusteredEdges.apply(this.clustering, arguments)
     };
-    T.prototype.getBaseEdge = function() {
+    E.prototype.getBaseEdge = function() {
         return this.clustering.getBaseEdge.apply(this.clustering, arguments)
     };
-    T.prototype.getBaseEdges = function() {
+    E.prototype.getBaseEdges = function() {
         return this.clustering.getBaseEdges.apply(this.clustering, arguments)
     };
-    T.prototype.updateEdge = function() {
+    E.prototype.updateEdge = function() {
         return this.clustering.updateEdge.apply(this.clustering, arguments)
     };
-    T.prototype.clusterOutliers = function() {
+    E.prototype.clusterOutliers = function() {
         return this.clustering.clusterOutliers.apply(this.clustering, arguments)
     };
-    T.prototype.getSeed = function() {
+    E.prototype.getSeed = function() {
         return this.layoutEngine.getSeed.apply(this.layoutEngine, arguments)
     };
-    T.prototype.enableEditMode = function() {
+    E.prototype.enableEditMode = function() {
         return this.manipulation.enableEditMode.apply(this.manipulation, arguments)
     };
-    T.prototype.disableEditMode = function() {
+    E.prototype.disableEditMode = function() {
         return this.manipulation.disableEditMode.apply(this.manipulation, arguments)
     };
-    T.prototype.addNodeMode = function() {
+    E.prototype.addNodeMode = function() {
         return this.manipulation.addNodeMode.apply(this.manipulation, arguments)
     };
-    T.prototype.editNode = function() {
+    E.prototype.editNode = function() {
         return this.manipulation.editNode.apply(this.manipulation, arguments)
     };
-    T.prototype.editNodeMode = function() {
+    E.prototype.editNodeMode = function() {
         return console.warn("Deprecated: Please use editNode instead of editNodeMode."), this.manipulation.editNode.apply(this.manipulation, arguments)
     };
-    T.prototype.addEdgeMode = function() {
+    E.prototype.addEdgeMode = function() {
         return this.manipulation.addEdgeMode.apply(this.manipulation, arguments)
     };
-    T.prototype.editEdgeMode = function() {
+    E.prototype.editEdgeMode = function() {
         return this.manipulation.editEdgeMode.apply(this.manipulation, arguments)
     };
-    T.prototype.deleteSelected = function() {
+    E.prototype.deleteSelected = function() {
         return this.manipulation.deleteSelected.apply(this.manipulation, arguments)
     };
-    T.prototype.getPositions = function() {
+    E.prototype.getPositions = function() {
         return this.nodesHandler.getPositions.apply(this.nodesHandler, arguments)
     };
-    T.prototype.getPosition = function() {
+    E.prototype.getPosition = function() {
         return this.nodesHandler.getPosition.apply(this.nodesHandler, arguments)
     };
-    T.prototype.storePositions = function() {
+    E.prototype.storePositions = function() {
         return this.nodesHandler.storePositions.apply(this.nodesHandler, arguments)
     };
-    T.prototype.moveNode = function() {
+    E.prototype.moveNode = function() {
         return this.nodesHandler.moveNode.apply(this.nodesHandler, arguments)
     };
-    T.prototype.getBoundingBox = function() {
+    E.prototype.getBoundingBox = function() {
         return this.nodesHandler.getBoundingBox.apply(this.nodesHandler, arguments)
     };
-    T.prototype.getConnectedNodes = function(n) {
+    E.prototype.getConnectedNodes = function(n) {
         return this.body.nodes[n] !== void 0 ? this.nodesHandler.getConnectedNodes.apply(this.nodesHandler, arguments) : this.edgesHandler.getConnectedNodes.apply(this.edgesHandler, arguments)
     };
-    T.prototype.getConnectedEdges = function() {
+    E.prototype.getConnectedEdges = function() {
         return this.nodesHandler.getConnectedEdges.apply(this.nodesHandler, arguments)
     };
-    T.prototype.startSimulation = function() {
+    E.prototype.startSimulation = function() {
         return this.physics.startSimulation.apply(this.physics, arguments)
     };
-    T.prototype.stopSimulation = function() {
+    E.prototype.stopSimulation = function() {
         return this.physics.stopSimulation.apply(this.physics, arguments)
     };
-    T.prototype.stabilize = function() {
+    E.prototype.stabilize = function() {
         return this.physics.stabilize.apply(this.physics, arguments)
     };
-    T.prototype.getSelection = function() {
+    E.prototype.getSelection = function() {
         return this.selectionHandler.getSelection.apply(this.selectionHandler, arguments)
     };
-    T.prototype.setSelection = function() {
+    E.prototype.setSelection = function() {
         return this.selectionHandler.setSelection.apply(this.selectionHandler, arguments)
     };
-    T.prototype.getSelectedNodes = function() {
+    E.prototype.getSelectedNodes = function() {
         return this.selectionHandler.getSelectedNodeIds.apply(this.selectionHandler, arguments)
     };
-    T.prototype.getSelectedEdges = function() {
+    E.prototype.getSelectedEdges = function() {
         return this.selectionHandler.getSelectedEdgeIds.apply(this.selectionHandler, arguments)
     };
-    T.prototype.getNodeAt = function() {
+    E.prototype.getNodeAt = function() {
         let n = this.selectionHandler.getNodeAt.apply(this.selectionHandler, arguments);
         return n !== void 0 && n.id !== void 0 ? n.id : n
     };
-    T.prototype.getEdgeAt = function() {
+    E.prototype.getEdgeAt = function() {
         let n = this.selectionHandler.getEdgeAt.apply(this.selectionHandler, arguments);
         return n !== void 0 && n.id !== void 0 ? n.id : n
     };
-    T.prototype.selectNodes = function() {
+    E.prototype.selectNodes = function() {
         return this.selectionHandler.selectNodes.apply(this.selectionHandler, arguments)
     };
-    T.prototype.selectEdges = function() {
+    E.prototype.selectEdges = function() {
         return this.selectionHandler.selectEdges.apply(this.selectionHandler, arguments)
     };
-    T.prototype.unselectAll = function() {
+    E.prototype.unselectAll = function() {
         this.selectionHandler.unselectAll.apply(this.selectionHandler, arguments), this.selectionHandler.commitWithoutEmitting.apply(this.selectionHandler), this.redraw()
     };
-    T.prototype.redraw = function() {
+    E.prototype.redraw = function() {
         return this.renderer.redraw.apply(this.renderer, arguments)
     };
-    T.prototype.getScale = function() {
+    E.prototype.getScale = function() {
         return this.view.getScale.apply(this.view, arguments)
     };
-    T.prototype.getViewPosition = function() {
+    E.prototype.getViewPosition = function() {
         return this.view.getViewPosition.apply(this.view, arguments)
     };
-    T.prototype.fit = function() {
+    E.prototype.fit = function() {
         return this.view.fit.apply(this.view, arguments)
     };
-    T.prototype.moveTo = function() {
+    E.prototype.moveTo = function() {
         return this.view.moveTo.apply(this.view, arguments)
     };
-    T.prototype.focus = function() {
+    E.prototype.focus = function() {
         return this.view.focus.apply(this.view, arguments)
     };
-    T.prototype.releaseNode = function() {
+    E.prototype.releaseNode = function() {
         return this.view.releaseNode.apply(this.view, arguments)
     };
-    T.prototype.getOptionsFromConfigurator = function() {
+    E.prototype.getOptionsFromConfigurator = function() {
         let n = {};
         return this.configurator && (n = this.configurator.getOptions.apply(this.configurator)), n
     };
     var pn = n => {
         if (!document.cookie) return;
         let e = null,
             t = document.cookie.split(";");
@@ -12801,187 +12801,77 @@
                 }
             },
             physics: {
                 solver: "forceAtlas2Based"
             }
         },
         Ia = pn("csrftoken"),
-        de = null,
+        Ue = null,
         gn = document.querySelector("#visgraph"),
         mn = document.querySelector("#id_save_coords");
     (function() {
         if (!topologyData) return;
 
-        function e(p) {
-            let b = document.createElement("div");
-            return b.innerHTML = p, b
+        function e(s) {
+            let o = document.createElement("div");
+            return o.innerHTML = s, o
         }
-        let t = new Ce(topologyData.nodes.map(p => Be(le({}, p), {
-            title: e(p.title)
+        let t = new Ee(topologyData.nodes.map(s => Me(de({}, s), {
+            title: e(s.title)
         })));
         window.nodes = t;
-        let i = new Ce(topologyData.edges.map(p => Be(le({}, p), {
-                title: e(p.title)
-            }))),
-            s = topologyData.options.group_sites,
-            o = topologyData.options.group_locations,
-            r = topologyData.options.group_racks;
-        de = new T(gn, {
+        let i = new Ee(topologyData.edges.map(s => Me(de({}, s), {
+            title: e(s.title)
+        })));
+        Ue = new E(gn, {
             nodes: t,
             edges: i
-        }, Hi), de.fit(), de.on("dragEnd", p => {
-            mn != null && (!mn.checked || Promise.allSettled(Object.entries(de.getPositions(p.nodes)).map(C => qi(this, [C], function*([b, _]) {
-                isNaN(parseInt(b)) ? nodeKey = b : nodeKey = parseInt(b);
+        }, Hi), Ue.fit(), Ue.on("dragEnd", s => {
+            mn != null && (!mn.checked || Promise.allSettled(Object.entries(Ue.getPositions(s.nodes)).map(a => qi(this, [a], function*([o, r]) {
+                isNaN(parseInt(o)) ? nodeKey = o : nodeKey = parseInt(o);
                 try {
                     window.nodes.update({
                         id: nodeKey,
                         physics: !1,
-                        x: _.x,
-                        y: _.y
+                        x: r.x,
+                        y: r.y
                     })
-                } catch (O) {
-                    console.log(["Error while executing window.nodes.update()", "nodeId: " + b, "nodeKey: " + nodeKey, "x: " + _.x, "y: " + _.y]), console.log(O)
+                } catch (h) {
+                    console.log(["Error while executing window.nodes.update()", "nodeId: " + o, "nodeKey: " + nodeKey, "x: " + r.x, "y: " + r.y]), console.log(h)
                 }
-                let x = yield fetch("/" + basePath + "api/plugins/netbox_topology_views/save-coords/save_coords/", {
+                let d = yield fetch("/" + basePath + "api/plugins/netbox_topology_views/save-coords/save_coords/", {
                     method: "PATCH",
                     headers: {
                         "X-CSRFToken": Ia,
                         Accept: "application/json",
                         "Content-Type": "application/json"
                     },
                     body: JSON.stringify({
-                        node_id: b,
-                        x: _.x,
-                        y: _.y,
+                        node_id: o,
+                        x: r.x,
+                        y: r.y,
                         group: topologyData.group
                     })
                 })
             }))))
-        }), de.on("doubleClick", p => {
-            p.nodes.length > 0 ? p.nodes.forEach(b => {
-                window.open(t.get(b).href, "_blank")
-            }) : p.edges.forEach(b => {
-                window.open(i.get(b).href, "_blank")
-            })
-        }), de.on("afterDrawing", p => {
-            d = [], s != null && s == "on" && l(p, c, u), o != null && o == "on" && l(p, f, y), r != null && r == "on" && l(p, v, g)
-        }), de.on("click", p => {
-            d.forEach(b => {
-                if (p.pointer.canvas.x > b.x1 - b.border / 2 - 1 && p.pointer.canvas.x < b.x2 + b.border / 2 + 1 && p.pointer.canvas.y > b.y1 - b.border / 2 - 1 && p.pointer.canvas.y < b.y2 + b.border / 2 + 1 && (p.pointer.canvas.x < b.x1 + b.border / 2 + 1 || p.pointer.canvas.x > b.x2 - b.border / 2 - 1 || p.pointer.canvas.y < b.y1 + b.border / 2 + 1 || p.pointer.canvas.y > b.y2 - b.border / 2 - 1)) {
-                    let _ = [];
-                    b.category == "Site" && c.forEach(C => {
-                        C.forEach(x => {
-                            x[1] == b.id && _.push(x[0])
-                        })
-                    }), b.category == "Location" && f.forEach(C => {
-                        C.forEach(x => {
-                            x[1] === b.id && _.push(x[0])
-                        })
-                    }), b.category == "Rack" && v.forEach(C => {
-                        C.forEach(x => {
-                            x[1] === b.id && _.push(x[0])
-                        })
-                    }), de.selectNodes(_)
-                }
-            })
-        });
-
-        function a(p, b) {
-            let _ = [];
-            for (let [x, O] of t._data) O[p] != null && _.push([O.id, O[p], O[b]]);
-            let C = _.reduce((x, O) => {
-                let M = O[1];
-                return x[M] = x[M] || [], x[M].push(O), x
-            }, {});
-            return Object.values(C)
-        }
-        var d = [];
-
-        function h(p) {
-            p.ctx.beginPath(), p.ctx.lineWidth = p.lineWidth, p.ctx.strokeStyle = p.color, p.ctx.rect(p.x, p.y, p.width, p.height), p.ctx.stroke(), p.ctx.font = p.font, p.ctx.fillStyle = p.color, p.ctx.fillText(p.text, p.x + p.textPaddingX, p.y + p.textPaddingY), d.push({
-                category: p.category,
-                id: p.id,
-                x1: p.x,
-                y1: p.y,
-                x2: p.x + p.width,
-                y2: p.y + p.height,
-                border: p.lineWidth
+        }), Ue.on("doubleClick", s => {
+            s.nodes.length > 0 ? s.nodes.forEach(o => {
+                window.open(t.get(o).href, "_blank")
+            }) : s.edges.forEach(o => {
+                window.open(i.get(o).href, "_blank")
             })
-        }
-
-        function l(p, b, _) {
-            for (let C of Object.entries(b)) {
-                let x = [],
-                    O = [],
-                    M = [];
-                for (let ge of C[1]) O.push(de.getPosition(ge[0]).x), M.push(de.getPosition(ge[0]).y);
-                let R = Math.min(...O) - _.paddingX,
-                    q = Math.min(...M) - _.paddingY,
-                    oe = Math.max(...O) - Math.min(...O) + 2 * _.paddingX,
-                    Oe = Math.max(...M) - Math.min(...M) + 2 * _.paddingY;
-                x.push({
-                    ctx: p,
-                    x: R,
-                    y: q,
-                    width: oe,
-                    height: Oe,
-                    lineWidth: _.lineWidth,
-                    color: _.color,
-                    text: C[1][0][2],
-                    textPaddingX: _.textPaddingX,
-                    textPaddingY: _.textPaddingY,
-                    font: _.font,
-                    id: C[1][0][1],
-                    category: _.category
-                }), x.forEach(function(ge) {
-                    h(ge)
-                })
-            }
-        }
-        let c = a("site_id", "site"),
-            u = {
-                lineWidth: "5",
-                color: "red",
-                paddingX: 84,
-                paddingY: 84,
-                textPaddingX: 8,
-                textPaddingY: -8,
-                font: "14px helvetica",
-                category: "Site"
-            },
-            f = a("location_id", "location"),
-            y = {
-                lineWidth: "5",
-                color: "#337ab7",
-                paddingX: 77,
-                paddingY: 77,
-                textPaddingX: 12,
-                textPaddingY: 22,
-                font: "14px helvetica",
-                category: "Location"
-            },
-            v = a("rack_id", "rack"),
-            g = {
-                lineWidth: "5",
-                color: "green",
-                paddingX: 70,
-                paddingY: 70,
-                textPaddingX: 8,
-                textPaddingY: 30,
-                font: "14px helvetica",
-                category: "Rack"
-            }
+        })
     })();
     var Pa = "image/png",
-        Ma = document.querySelector("#btnDownloadImage");
-    Ma.addEventListener("click", n => {
-        Da()
+        Da = document.querySelector("#btnDownloadImage");
+    Da.addEventListener("click", n => {
+        Ma()
     });
 
-    function Da() {
+    function Ma() {
         let n = gn.querySelector("canvas"),
             e = document.createElement("a"),
             t = n.toDataURL(Pa);
         e.href = t, e.download = "topology", document.body.appendChild(e), e.click(), document.body.removeChild(e)
     }
     var Fa = document.querySelector("#btnDownloadXml");
     Fa.addEventListener("click", n => {
@@ -13007,19 +12897,19 @@
             var r = new Blob([o], {
                 type: "text/plain"
             });
             n.setAttribute("href", window.URL.createObjectURL(r)), n.setAttribute("download", "topology.xml"), n.dataset.downloadurl = ["text/plain", n.download, n.href].join(":"), n.click()
         })
     }
     var Ba = new MutationObserver(n => n.forEach(e => {
-        if (!de || e.type !== "attributes" || e.attributeName !== "data-netbox-color-mode" || !(e.target instanceof HTMLElement)) return;
+        if (!Ue || e.type !== "attributes" || e.attributeName !== "data-netbox-color-mode" || !(e.target instanceof HTMLElement)) return;
         let {
             netboxColorMode: t
         } = e.target.dataset;
-        Hi.nodes.font.color = t === "dark" ? "#fff" : "#000", de.setOptions(Hi)
+        Hi.nodes.font.color = t === "dark" ? "#fff" : "#000", Ue.setOptions(Hi)
     }));
     Ba.observe(document.documentElement, {
         attributes: !0,
         attributeFilter: ["data-netbox-color-mode"]
     });
 })();
 /*! Hammer.JS - v2.0.17-rc - 2019-12-16
```

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/js/images.js` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/js/images.js`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/static/netbox_topology_views/js/images.js.map` & `netbox-topology-views-3.9b1/netbox_topology_views/static/netbox_topology_views/js/images.js.map`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/tables.py` & `netbox-topology-views-3.9b1/netbox_topology_views/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/template_content.py` & `netbox-topology-views-3.9b1/netbox_topology_views/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/circuitcoordinate.html` & `netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/circuitcoordinate.html`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/coordinate.html` & `netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/coordinate.html`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/coordinategroup.html` & `netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/coordinategroup.html`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/htmx_topology.html` & `netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/htmx_topology.html`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/images.html` & `netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/images.html`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/powerfeedcoordinate.html` & `netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/powerfeedcoordinate.html`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/powerpanelcoordinate.html` & `netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/powerpanelcoordinate.html`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/templates/netbox_topology_views/toasts.html` & `netbox-topology-views-3.9b1/netbox_topology_views/templates/netbox_topology_views/toasts.html`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/urls.py` & `netbox-topology-views-3.9b1/netbox_topology_views/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/utils.py` & `netbox-topology-views-3.9b1/netbox_topology_views/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,18 +103,14 @@
 def get_model_role(model: Type[Model]) -> Role:
     return Role(
         slug=get_model_slug(model),
         name=re_camel_case.sub(r" \1", model.__name__),
     )
 
 def get_query_settings(request):
-    filter_id = ''
-    if "filter_id" in request.GET:
-        filter_id = request.GET["filter_id"]
-
     save_coords = False
     if "save_coords" in request.GET:
         if request.GET["save_coords"] == "on":
             save_coords = True
     # General options overrides
     if save_coords == True and settings.PLUGINS_CONFIG["netbox_topology_views"]["allow_coordinates_saving"] == False:
         save_coords = False
@@ -154,35 +150,20 @@
             show_cables = True
 
     show_wireless = False
     if "show_wireless" in request.GET:
         if request.GET["show_wireless"] == "on" :
             show_wireless = True
 
-    group_sites = False
-    if "group_sites" in request.GET:
-        if request.GET["group_sites"] == "on" :
-            group_sites = True
-
-    group_locations = False
-    if "group_locations" in request.GET:
-        if request.GET["group_locations"] == "on" :
-            group_locations = True
-
-    group_racks = False
-    if "group_racks" in request.GET:
-        if request.GET["group_racks"] == "on" :
-            group_racks = True
-
     show_neighbors = False
     if "show_neighbors" in request.GET:
         if request.GET["show_neighbors"] == "on" :
             show_neighbors = True
     
-    return filter_id, save_coords, show_unconnected, show_power, show_circuit, show_logical_connections, show_single_cable_logical_conns, show_cables, show_wireless, group_sites, group_locations, group_racks, show_neighbors
+    return save_coords, show_unconnected, show_power, show_circuit, show_logical_connections, show_single_cable_logical_conns, show_cables, show_wireless, show_neighbors
 
 class LinePattern():
     wireless = [2, 10, 2, 10]
     power = [5, 5, 3, 3]
     logical = [1, 10, 1, 10]
```

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views/views.py` & `netbox-topology-views-3.9b1/netbox_topology_views/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from django.contrib.auth.mixins import PermissionRequiredMixin
 from django.contrib.contenttypes.models import ContentType
 from django.db.models import Q, QuerySet, Count
 from django.db.models.functions import Lower
 from django.http import HttpRequest, HttpResponseRedirect, QueryDict
 from django.shortcuts import render, get_object_or_404
 from django.views.generic import View
-from extras.models import Tag, SavedFilter
+from extras.models import Tag
 from wireless.models import WirelessLink
 from netbox.views.generic import (
     ObjectView, 
     ObjectListView, 
     ObjectEditView, 
     ObjectDeleteView, 
     ObjectChangeLogView, 
@@ -176,24 +176,14 @@
             else:
                 node_content += (
                     f"<tr><th>Position: </th><td>{device.position}</td></tr>"
                 )
 
         node["id"] = device.pk
 
-        if device.site is not None:
-            node["site"] = device.site.name
-            node["site_id"] = device.site_id
-        if device.location is not None:
-            node["location"] = device.location.name
-            node["location_id"] = device.location_id
-        if device.rack is not None:
-            node["rack"] = device.rack.name
-            node["rack_id"] = device.rack_id
-
         if device.device_role.color != "":
             node["color.border"] = "#" + device.device_role.color
 
     model_class = getattr(netbox_topology_views.models, model_name)
 
     if group_id is None or group_id == "default":
         group_id = model_class.get_or_create_default_group(group_id)
@@ -331,31 +321,27 @@
     show_cables: bool,
     show_circuit: bool,
     show_logical_connections: bool,
     show_single_cable_logical_conns: bool,
     show_neighbors: bool,
     show_power: bool,
     show_wireless: bool,
-    group_sites: bool,
-    group_locations: bool,
-    group_racks: bool,
     group_id,
 ):
     
     supported_termination_types = []
     for t in IndividualOptions.CHOICES:
         supported_termination_types.append(t[1])
 
     if not queryset:
         return None
 
     nodes_devices = {}
     edges = []
     nodes = []
-    options = {}
     edge_ids = 0
     nodes_circuits: Dict[int, Circuit] = {}
     nodes_powerpanel: Dict[int, PowerPanel] = {}
     nodes_powerfeed: Dict[int, PowerFeed] = {}
     nodes_provider_networks = {}
     cable_ids = DefaultDict(dict)
     interface_ids = DefaultDict(dict)
@@ -661,34 +647,26 @@
                     cable=wlan_link,
                     termination_a=termination_a,
                     termination_b=termination_b,
                     wireless=wireless,
                 )
             )
 
-    if group_locations:
-        options['group_locations'] = 'on'
-    if group_racks:
-        options['group_racks'] = 'on'
-    if group_sites:
-        options['group_sites'] = 'on'
-
     for qs_device in queryset:
         if qs_device.pk not in nodes_devices and show_unconnected:
             nodes_devices[qs_device.pk] = qs_device
 
     results = {}
 
     for d in nodes_devices.values():
         nodes.append(create_node(d, save_coords, group_id))
 
     results["nodes"] = nodes
     results["edges"] = edges
     results["group"] = group_id
-    results["options"] = options
     return results
 
 
 class TopologyHomeView(PermissionRequiredMixin, View):
     permission_required = ("dcim.view_site", "dcim.view_device")
 
     """
@@ -706,38 +684,16 @@
 
         individualOptions, created = IndividualOptions.objects.get_or_create(
             user_id=request.user.id,
         )
 
         if request.GET:
 
-            filter_id, save_coords, show_unconnected, show_power, show_circuit, show_logical_connections, show_single_cable_logical_conns, show_cables, show_wireless, group_sites, group_locations, group_racks, show_neighbors = get_query_settings(request)
+            save_coords, show_unconnected, show_power, show_circuit, show_logical_connections, show_single_cable_logical_conns, show_cables, show_wireless, show_neighbors = get_query_settings(request)
             
-            # Read options from saved filters as NetBox does not handle custom plugin filters
-            if "filter_id" in request.GET and request.GET["filter_id"] != '':
-                try:
-                    saved_filter = SavedFilter.objects.get(pk=filter_id)
-                    saved_filter_params = getattr(saved_filter, 'parameters')
-
-                    if save_coords == False and 'save_coords' in saved_filter_params: save_coords = saved_filter_params['save_coords']
-                    if show_power == False and 'show_power' in saved_filter_params: show_power = saved_filter_params['show_power']
-                    if show_circuit == False and 'show_circuit' in saved_filter_params: show_circuit = saved_filter_params['show_circuit']
-                    if show_logical_connections == False and 'show_logical_connections' in saved_filter_params: show_logical_connections = saved_filter_params['show_logical_connections']
-                    if show_single_cable_logical_conns == False and 'show_single_cable_logical_conns' in saved_filter_params: show_single_cable_logical_conns = saved_filter_params['show_single_cable_logical_conns']
-                    if show_cables == False and 'show_cables' in saved_filter_params: show_cables = saved_filter_params['show_cables']
-                    if show_wireless == False and 'show_wireless' in saved_filter_params: show_wireless = saved_filter_params['show_wireless']
-                    if group_sites == False and 'group_sites' in saved_filter_params: group_sites = saved_filter_params['group_sites']
-                    if group_locations == False and 'group_locations' in saved_filter_params: group_locations = saved_filter_params['group_locations']
-                    if group_racks == False and 'group_racks' in saved_filter_params: group_racks = saved_filter_params['group_racks']
-                    if show_neighbors == False and 'show_neighbors' in saved_filter_params: show_neighbors = saved_filter_params['show_neighbors']
-                except SavedFilter.DoesNotExist: # filter_id not found
-                    pass
-                except Exception as inst:
-                    print(type(inst))
-
             if "group" not in request.GET:
                 group_id = "default"
             else:
                 group_id = request.GET["group"]
 
             if not "draw_init" in request.GET or "draw_init" in request.GET and request.GET["draw_init"].lower() == "true":
                 topo_data = get_topology_data(
@@ -748,17 +704,14 @@
                     show_cables=show_cables,
                     show_logical_connections=show_logical_connections,
                     show_single_cable_logical_conns=show_single_cable_logical_conns,
                     show_neighbors=show_neighbors,
                     show_circuit=show_circuit,
                     show_power=show_power,
                     show_wireless=show_wireless,
-                    group_sites=group_sites,
-                    group_locations=group_locations,
-                    group_racks=group_racks,
                     group_id=group_id,
                 )
             
         else:
             # No GET-Request in URL. We most likely came here from the navigation menu.
             preselected_device_roles = IndividualOptions.objects.get(id=individualOptions.id).preselected_device_roles.all().values_list('id', flat=True)
             preselected_tags = IndividualOptions.objects.get(id=individualOptions.id).preselected_tags.all().values_list(Lower('name'), flat=True)
@@ -772,17 +725,14 @@
             if individualOptions.show_cables: q['show_cables'] = "on"
             if individualOptions.show_logical_connections: q['show_logical_connections'] = "on"
             if individualOptions.show_single_cable_logical_conns: q['show_single_cable_logical_conns'] = "on"
             if individualOptions.show_neighbors: q['show_neighbors'] = "on"
             if individualOptions.show_circuit: q['show_circuit'] = "on"
             if individualOptions.show_power: q['show_power'] = "on"
             if individualOptions.show_wireless: q['show_wireless'] = "on"
-            if individualOptions.group_sites: q['group_sites'] = "on"
-            if individualOptions.group_locations: q['group_locations'] = "on"
-            if individualOptions.group_racks: q['group_racks'] = "on"
             if individualOptions.draw_default_layout: 
                 q['draw_init'] = "true"
             else:
                 q['draw_init'] = "false"
 
             query_string = q.urlencode()
             return HttpResponseRedirect(f"{request.path}?{query_string}")
@@ -1129,17 +1079,14 @@
                 'show_cables': queryset.show_cables, 
                 'show_logical_connections': queryset.show_logical_connections,
                 'show_single_cable_logical_conns': queryset.show_single_cable_logical_conns,
                 'show_neighbors': queryset.show_neighbors,
                 'show_circuit': queryset.show_circuit,
                 'show_power': queryset.show_power,
                 'show_wireless': queryset.show_wireless,
-                'group_sites': queryset.group_sites,
-                'group_locations': queryset.group_locations,
-                'group_racks': queryset.group_racks,
                 'draw_default_layout': queryset.draw_default_layout,
             },
         )
 
         return render(
             request,
             "netbox_topology_views/individual_options.html",
```

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views.egg-info/PKG-INFO` & `netbox-topology-views-3.9b1/netbox_topology_views.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-topology-views
-Version: 3.9.1
+Version: 3.9b1
 Summary: An NetBox plugin to create Topology maps
 Home-page: https://github.com/mattieserver/netbox-topology-views
 Author: Mattijs Vanhaverbeke
 License: Apache 2.0
 Project-URL: Source, https://github.com/mattieserver/netbox-topology-views
 Keywords: netbox-plugin
 Classifier: Programming Language :: Python
```

### Comparing `netbox_topology_views-3.9.1/netbox_topology_views.egg-info/SOURCES.txt` & `netbox-topology-views-3.9b1/netbox_topology_views.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 netbox_topology_views/api/views.py
 netbox_topology_views/migrations/0001_initial.py
 netbox_topology_views/migrations/0002_individualoptions.py
 netbox_topology_views/migrations/0003_individualoptions_show_neighbors.py
 netbox_topology_views/migrations/0004_coordinategroup_coordinate.py
 netbox_topology_views/migrations/0005_individualoptions_save_coords.py
 netbox_topology_views/migrations/0006_powerpanelcoordinate_powerfeedcoordinate_and_more.py
-netbox_topology_views/migrations/0007_individualoptions_group_locations_and_more.py
 netbox_topology_views/migrations/__init__.py
 netbox_topology_views/static/netbox_topology_views/css/app.css
 netbox_topology_views/static/netbox_topology_views/css/vendor.css
 netbox_topology_views/static/netbox_topology_views/img/LICENSE
 netbox_topology_views/static/netbox_topology_views/img/access-switch.svg
 netbox_topology_views/static/netbox_topology_views/img/backhaul.svg
 netbox_topology_views/static/netbox_topology_views/img/backup.svg
```

### Comparing `netbox_topology_views-3.9.1/setup.py` & `netbox-topology-views-3.9b1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 readme = Path(__file__).parent / "README.md"
 long_description = readme.read_text()
 
 setup(
     name="netbox-topology-views",
-    version="3.9.1",
+    version="3.9-beta1",
     description="An NetBox plugin to create Topology maps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mattieserver/netbox-topology-views",
     author="Mattijs Vanhaverbeke",
     license="Apache 2.0",
     install_requires=[],
```

