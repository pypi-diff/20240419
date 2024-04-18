# Comparing `tmp/sbcli_jm-3.0.0.zip` & `tmp/sbcli_jm-4.0.0.zip`

## zipinfo {}

```diff
@@ -1,146 +1,146 @@
-Zip file size: 177896 bytes, number of entries: 144
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 13:59 sbcli_jm-3.0.0/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_cli/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 13:59 sbcli_jm-3.0.0/sbcli_jm.egg-info/
--rw-r--r--  2.0 unx       38 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/setup.cfg
--rw-r--r--  2.0 unx       84 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/pyproject.toml
--rw-r--r--  2.0 unx      730 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/README.md
--rw-r--r--  2.0 unx     2251 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/setup.py
--rw-r--r--  2.0 unx      147 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/env_var
--rw-r--r--  2.0 unx     1128 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/PKG-INFO
--rw-r--r--  2.0 unx    76335 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_cli/cli.py
--rw-r--r--  2.0 unx      357 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_cli/main.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/templates/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/blueprints/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/static/
--rw-r--r--  2.0 unx      725 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/caching_node_app_k8s.py
--rw-r--r--  2.0 unx     1263 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/app.py
--rw-r--r--  2.0 unx     1434 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/node_webapp.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/__init__.py
--rw-r--r--  2.0 unx      717 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/caching_node_app.py
--rw-r--r--  2.0 unx      703 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/snode_app.py
--rw-r--r--  2.0 unx     5098 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/node_utils.py
--rw-r--r--  2.0 unx     2508 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/utils.py
--rw-r--r--  2.0 unx     1638 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/auth_middleware.py
--rw-r--r--  2.0 unx     2876 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/templates/deploy_spdk.yaml.j2
--rw-r--r--  2.0 unx     5274 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_cluster.py
--rw-r--r--  2.0 unx     7846 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/blueprints/caching_node_ops_k8s.py
--rw-r--r--  2.0 unx     8169 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_lvol.py
--rw-r--r--  2.0 unx     6326 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_storage_node.py
--rw-r--r--  2.0 unx     5547 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/blueprints/node_api_caching_docker.py
--rw-r--r--  2.0 unx     3103 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/blueprints/node_api_basic.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/blueprints/__init__.py
--rw-r--r--  2.0 unx     8654 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/blueprints/snode_ops.py
--rw-r--r--  2.0 unx    11244 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/blueprints/csi.py
--rw-r--r--  2.0 unx      975 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_mgmt_node.py
--rw-r--r--  2.0 unx     6206 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_pool.py
--rw-r--r--  2.0 unx    12198 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/blueprints/caching_node_ops.py
--rw-r--r--  2.0 unx     4795 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/blueprints/node_api_caching_ks.py
--rw-r--r--  2.0 unx     2940 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_device.py
--rw-r--r--  2.0 unx     5317 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_caching_node.py
--rw-r--r--  2.0 unx      463 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/static/rpac.yaml
--rw-r--r--  2.0 unx     1466 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/static/deploy_spdk.yaml
--rw-r--r--  2.0 unx      827 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/static/delete.py
--rw-r--r--  2.0 unx      507 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/static/deploy_cnode.yaml
--rw-r--r--  2.0 unx     1302 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/static/deploy.py
--rw-r--r--  2.0 unx      434 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/static/is_up.py
--rw-r--r--  2.0 unx      417 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/static/list_deps.py
--rw-r--r--  2.0 unx      322 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_web/static/tst.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/controllers/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/
--rw-r--r--  2.0 unx     6199 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/distr_controller.py
--rw-r--r--  2.0 unx      938 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/pci_utils.py
--rw-r--r--  2.0 unx      279 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/shell_utils.py
--rw-r--r--  2.0 unx    21410 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/rpc_client.py
--rw-r--r--  2.0 unx     1440 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/constants.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/__init__.py
--rw-r--r--  2.0 unx    64162 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/storage_node_ops.py
--rw-r--r--  2.0 unx     3444 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/cnode_client.py
--rw-r--r--  2.0 unx     5112 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/compute_node_ops.py
--rw-r--r--  2.0 unx    23335 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/cluster_ops.py
--rw-r--r--  2.0 unx     3153 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/mgmt_node_ops.py
--rw-r--r--  2.0 unx     7640 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/utils.py
--rw-r--r--  2.0 unx     8189 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/kv_store.py
--rw-r--r--  2.0 unx     3193 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/snode_client.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/alerting/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/dashboards/
--rw-r--r--  2.0 unx      152 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/set_db_config.sh
--rw-r--r--  2.0 unx     5305 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/stack_deploy_wait.sh
--rw-r--r--  2.0 unx     1420 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/install_deps.sh
--rw-r--r--  2.0 unx       43 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/run_ssh.sh
--rw-r--r--  2.0 unx      453 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/config_docker.sh
--rw-r--r--  2.0 unx     1694 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/__init__.py
--rw-r--r--  2.0 unx      360 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/datasource.yml
--rw-r--r--  2.0 unx     1163 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/haproxy.cfg
--rw-r--r--  2.0 unx       54 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/db_config_single.sh
--rwxr-xr-x  2.0 unx      595 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/apply_dashboard.sh
--rw-r--r--  2.0 unx      187 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/prometheus.yml
--rw-r--r--  2.0 unx     8081 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/docker-compose-swarm.yml
--rw-r--r--  2.0 unx      694 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/deploy_stack.sh
--rw-r--r--  2.0 unx      118 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/db_config_double.sh
--rw-r--r--  2.0 unx      311 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/clean_local_storage_deploy.sh
--rw-r--r--  2.0 unx     5860 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/alerting/alert_rules.yaml
--rw-r--r--  2.0 unx     1853 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/alerting/alert_resources.yaml
--rw-r--r--  2.0 unx    98143 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/dashboards/devices.json
--rw-r--r--  2.0 unx    98031 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/dashboards/lvols.json
--rw-r--r--  2.0 unx    98198 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/dashboards/cluster.json
--rw-r--r--  2.0 unx    98086 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/scripts/dashboards/nodes.json
--rw-r--r--  2.0 unx    22847 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/controllers/caching_node_controller.py
--rw-r--r--  2.0 unx    13535 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/controllers/device_controller.py
--rw-r--r--  2.0 unx     1900 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/controllers/cluster_events.py
--rw-r--r--  2.0 unx     1427 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/controllers/lvol_events.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/controllers/__init__.py
--rw-r--r--  2.0 unx      695 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/controllers/pool_events.py
--rw-r--r--  2.0 unx    10787 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/controllers/snapshot_controller.py
--rw-r--r--  2.0 unx     1122 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/controllers/snapshot_events.py
--rw-r--r--  2.0 unx     1521 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/controllers/storage_events.py
--rw-r--r--  2.0 unx     1120 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/controllers/mgmt_events.py
--rw-r--r--  2.0 unx     1961 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/controllers/events_controller.py
--rw-r--r--  2.0 unx    46637 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/controllers/lvol_controller.py
--rw-r--r--  2.0 unx    10375 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/controllers/pool_controller.py
--rw-r--r--  2.0 unx     1568 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/controllers/device_events.py
--rw-r--r--  2.0 unx    11300 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/controllers/health_controller.py
--rw-r--r--  2.0 unx     3003 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/mgmt_node_monitor.py
--rw-r--r--  2.0 unx     2410 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/log_agg_service.py
--rw-r--r--  2.0 unx     5443 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/capacity_collector.py
--rw-r--r--  2.0 unx     2423 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/port_stat_collector.py
--rw-r--r--  2.0 unx     4118 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/__init__.py
--rw-r--r--  2.0 unx      837 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/install_service.sh
--rw-r--r--  2.0 unx     4817 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/lvol_stat_collector.py
--rw-r--r--  2.0 unx     2490 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/device_monitor.py
--rw-r--r--  2.0 unx     6372 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/storage_node_monitor.py
--rw-r--r--  2.0 unx     2189 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/lvol_monitor.py
--rw-r--r--  2.0 unx     4971 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/distr_event_collector.py
--rw-r--r--  2.0 unx      173 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/remove_service.sh
--rw-r--r--  2.0 unx     5462 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/health_check_service.py
--rw-r--r--  2.0 unx     3203 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/caching_node_monitor.py
--rw-r--r--  2.0 unx     2671 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/cap_monitor.py
--rw-r--r--  2.0 unx      229 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/service_template.service
--rw-r--r--  2.0 unx     7218 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/services/capacity_and_stats_collector.py
--rw-r--r--  2.0 unx     1228 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/global_settings.py
--rw-r--r--  2.0 unx     2565 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/cluster.py
--rw-r--r--  2.0 unx     3766 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/caching_node.py
--rw-r--r--  2.0 unx     1602 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/pool.py
--rw-r--r--  2.0 unx     1500 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/events.py
--rw-r--r--  2.0 unx      806 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/iface.py
--rw-r--r--  2.0 unx     4846 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/base_model.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/__init__.py
--rw-r--r--  2.0 unx     4242 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/stats.py
--rw-r--r--  2.0 unx     2193 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/nvme_device.py
--rw-r--r--  2.0 unx     3222 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/storage_node.py
--rw-r--r--  2.0 unx     1020 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/port_stat.py
--rw-r--r--  2.0 unx     1466 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/mgmt_node.py
--rw-r--r--  2.0 unx      736 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/snapshot.py
--rw-r--r--  2.0 unx      917 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/compute_node.py
--rw-r--r--  2.0 unx     2579 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/simplyblock_core/models/lvol_model.py
--rw-r--r--  2.0 unx       49 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/sbcli_jm.egg-info/top_level.txt
--rw-r--r--  2.0 unx     5067 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/sbcli_jm.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/sbcli_jm.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx       54 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/sbcli_jm.egg-info/entry_points.txt
--rw-r--r--  2.0 unx       66 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/sbcli_jm.egg-info/requires.txt
--rw-r--r--  2.0 unx     1128 b- defN 24-Apr-16 13:59 sbcli_jm-3.0.0/sbcli_jm.egg-info/PKG-INFO
-144 files, 985536 bytes uncompressed, 152062 bytes compressed:  84.6%
+Zip file size: 180070 bytes, number of entries: 144
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 23:00 sbcli_jm-4.0.0/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_cli/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 23:00 sbcli_jm-4.0.0/sbcli_jm.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/
+-rw-r--r--  2.0 unx     2251 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/setup.py
+-rw-r--r--  2.0 unx      740 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/README.md
+-rw-r--r--  2.0 unx      152 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/env_var
+-rw-r--r--  2.0 unx       84 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/pyproject.toml
+-rw-r--r--  2.0 unx       38 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/setup.cfg
+-rw-r--r--  2.0 unx     1138 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/PKG-INFO
+-rw-r--r--  2.0 unx    76791 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_cli/cli.py
+-rw-r--r--  2.0 unx      357 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_cli/main.py
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/sbcli_jm.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx     5067 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/sbcli_jm.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       49 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/sbcli_jm.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     1138 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/sbcli_jm.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       66 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/sbcli_jm.egg-info/requires.txt
+-rw-r--r--  2.0 unx       54 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/sbcli_jm.egg-info/entry_points.txt
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/services/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/scripts/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/controllers/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/models/
+-rw-r--r--  2.0 unx    66153 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/storage_node_ops.py
+-rw-r--r--  2.0 unx     1445 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/constants.py
+-rw-r--r--  2.0 unx     3153 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/mgmt_node_ops.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/cnode_client.py
+-rw-r--r--  2.0 unx      279 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/shell_utils.py
+-rw-r--r--  2.0 unx      938 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/pci_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/__init__.py
+-rw-r--r--  2.0 unx     3416 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/snode_client.py
+-rw-r--r--  2.0 unx     8189 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/kv_store.py
+-rw-r--r--  2.0 unx     7640 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/utils.py
+-rw-r--r--  2.0 unx    23335 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/cluster_ops.py
+-rw-r--r--  2.0 unx     5112 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/compute_node_ops.py
+-rw-r--r--  2.0 unx    21979 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/rpc_client.py
+-rw-r--r--  2.0 unx     7401 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/distr_controller.py
+-rw-r--r--  2.0 unx     2189 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/services/lvol_monitor.py
+-rw-r--r--  2.0 unx     3203 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/services/caching_node_monitor.py
+-rw-r--r--  2.0 unx     5443 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/services/capacity_collector.py
+-rw-r--r--  2.0 unx     5462 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/services/health_check_service.py
+-rw-r--r--  2.0 unx      229 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/services/service_template.service
+-rw-r--r--  2.0 unx     5262 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/services/lvol_stat_collector.py
+-rw-r--r--  2.0 unx      173 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/services/remove_service.sh
+-rw-r--r--  2.0 unx     2410 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/services/log_agg_service.py
+-rw-r--r--  2.0 unx     5123 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/services/distr_event_collector.py
+-rw-r--r--  2.0 unx     7438 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/services/capacity_and_stats_collector.py
+-rw-r--r--  2.0 unx     2423 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/services/port_stat_collector.py
+-rw-r--r--  2.0 unx     2490 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/services/device_monitor.py
+-rw-r--r--  2.0 unx     4118 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/services/__init__.py
+-rw-r--r--  2.0 unx      837 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/services/install_service.sh
+-rw-r--r--  2.0 unx     3003 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/services/mgmt_node_monitor.py
+-rw-r--r--  2.0 unx     2671 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/services/cap_monitor.py
+-rw-r--r--  2.0 unx     6577 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/services/storage_node_monitor.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/scripts/alerting/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/scripts/dashboards/
+-rw-r--r--  2.0 unx      694 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/scripts/deploy_stack.sh
+-rw-r--r--  2.0 unx      152 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/scripts/set_db_config.sh
+-rw-r--r--  2.0 unx     1163 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/scripts/haproxy.cfg
+-rw-r--r--  2.0 unx     8081 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/scripts/docker-compose-swarm.yml
+-rw-r--r--  2.0 unx       54 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/scripts/db_config_single.sh
+-rw-r--r--  2.0 unx     5305 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/scripts/stack_deploy_wait.sh
+-rw-r--r--  2.0 unx      453 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/scripts/config_docker.sh
+-rw-r--r--  2.0 unx     1694 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/scripts/__init__.py
+-rw-r--r--  2.0 unx      311 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/scripts/clean_local_storage_deploy.sh
+-rw-r--r--  2.0 unx      118 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/scripts/db_config_double.sh
+-rw-r--r--  2.0 unx      360 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/scripts/datasource.yml
+-rw-r--r--  2.0 unx       43 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/scripts/run_ssh.sh
+-rw-r--r--  2.0 unx     1438 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/scripts/install_deps.sh
+-rw-r--r--  2.0 unx      187 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/scripts/prometheus.yml
+-rwxr-xr-x  2.0 unx      595 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/scripts/apply_dashboard.sh
+-rw-r--r--  2.0 unx     5860 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/scripts/alerting/alert_rules.yaml
+-rw-r--r--  2.0 unx     1853 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/scripts/alerting/alert_resources.yaml
+-rw-r--r--  2.0 unx    98143 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/scripts/dashboards/devices.json
+-rw-r--r--  2.0 unx    98086 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/scripts/dashboards/nodes.json
+-rw-r--r--  2.0 unx    98031 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/scripts/dashboards/lvols.json
+-rw-r--r--  2.0 unx    98198 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/scripts/dashboards/cluster.json
+-rw-r--r--  2.0 unx    12785 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/controllers/device_controller.py
+-rw-r--r--  2.0 unx     1120 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/controllers/mgmt_events.py
+-rw-r--r--  2.0 unx     1961 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/controllers/events_controller.py
+-rw-r--r--  2.0 unx     1521 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/controllers/storage_events.py
+-rw-r--r--  2.0 unx     1630 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/controllers/lvol_events.py
+-rw-r--r--  2.0 unx    10557 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/controllers/snapshot_controller.py
+-rw-r--r--  2.0 unx     1568 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/controllers/device_events.py
+-rw-r--r--  2.0 unx    10375 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/controllers/pool_controller.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/controllers/__init__.py
+-rw-r--r--  2.0 unx     1900 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/controllers/cluster_events.py
+-rw-r--r--  2.0 unx    22802 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/controllers/caching_node_controller.py
+-rw-r--r--  2.0 unx     1122 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/controllers/snapshot_events.py
+-rw-r--r--  2.0 unx    47314 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/controllers/lvol_controller.py
+-rw-r--r--  2.0 unx    11294 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/controllers/health_controller.py
+-rw-r--r--  2.0 unx      695 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/controllers/pool_events.py
+-rw-r--r--  2.0 unx     1500 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/models/events.py
+-rw-r--r--  2.0 unx      806 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/models/iface.py
+-rw-r--r--  2.0 unx     4846 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/models/base_model.py
+-rw-r--r--  2.0 unx     2579 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/models/lvol_model.py
+-rw-r--r--  2.0 unx      917 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/models/compute_node.py
+-rw-r--r--  2.0 unx      736 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/models/snapshot.py
+-rw-r--r--  2.0 unx     1602 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/models/pool.py
+-rw-r--r--  2.0 unx     1228 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/models/global_settings.py
+-rw-r--r--  2.0 unx     1020 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/models/port_stat.py
+-rw-r--r--  2.0 unx     3471 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/models/storage_node.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/models/__init__.py
+-rw-r--r--  2.0 unx     4242 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/models/stats.py
+-rw-r--r--  2.0 unx     2565 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/models/cluster.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/models/mgmt_node.py
+-rw-r--r--  2.0 unx     3766 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/models/caching_node.py
+-rw-r--r--  2.0 unx     2132 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_core/models/nvme_device.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/static/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/templates/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/blueprints/
+-rw-r--r--  2.0 unx      725 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/caching_node_app_k8s.py
+-rw-r--r--  2.0 unx     5098 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/node_utils.py
+-rw-r--r--  2.0 unx      703 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/snode_app.py
+-rw-r--r--  2.0 unx     1263 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/app.py
+-rw-r--r--  2.0 unx     1638 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/auth_middleware.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/__init__.py
+-rw-r--r--  2.0 unx      717 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/caching_node_app.py
+-rw-r--r--  2.0 unx     2513 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/utils.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/node_webapp.py
+-rw-r--r--  2.0 unx      507 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/static/deploy_cnode.yaml
+-rw-r--r--  2.0 unx      322 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/static/tst.py
+-rw-r--r--  2.0 unx      434 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/static/is_up.py
+-rw-r--r--  2.0 unx      827 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/static/delete.py
+-rw-r--r--  2.0 unx     1302 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/static/deploy.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/static/deploy_spdk.yaml
+-rw-r--r--  2.0 unx      463 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/static/rpac.yaml
+-rw-r--r--  2.0 unx      417 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/static/list_deps.py
+-rw-r--r--  2.0 unx     2876 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/templates/deploy_spdk.yaml.j2
+-rw-r--r--  2.0 unx     5547 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/blueprints/node_api_caching_docker.py
+-rw-r--r--  2.0 unx     4795 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/blueprints/node_api_caching_ks.py
+-rw-r--r--  2.0 unx     5317 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/blueprints/web_api_caching_node.py
+-rw-r--r--  2.0 unx    10230 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/blueprints/snode_ops.py
+-rw-r--r--  2.0 unx     8547 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/blueprints/web_api_lvol.py
+-rw-r--r--  2.0 unx    11244 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/blueprints/csi.py
+-rw-r--r--  2.0 unx    12198 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/blueprints/caching_node_ops.py
+-rw-r--r--  2.0 unx      975 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/blueprints/web_api_mgmt_node.py
+-rw-r--r--  2.0 unx     6326 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/blueprints/web_api_storage_node.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/blueprints/__init__.py
+-rw-r--r--  2.0 unx     7846 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/blueprints/caching_node_ops_k8s.py
+-rw-r--r--  2.0 unx     2940 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/blueprints/web_api_device.py
+-rw-r--r--  2.0 unx     5274 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/blueprints/web_api_cluster.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/blueprints/node_api_basic.py
+-rw-r--r--  2.0 unx     6206 b- defN 24-Apr-18 23:00 sbcli_jm-4.0.0/simplyblock_web/blueprints/web_api_pool.py
+144 files, 993053 bytes uncompressed, 154236 bytes compressed:  84.5%
```

## zipnote {}

```diff
@@ -1,433 +1,433 @@
-Filename: sbcli_jm-3.0.0/
+Filename: sbcli_jm-4.0.0/
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_cli/
+Filename: sbcli_jm-4.0.0/simplyblock_cli/
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/
+Filename: sbcli_jm-4.0.0/sbcli_jm.egg-info/
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/
+Filename: sbcli_jm-4.0.0/simplyblock_core/
 Comment: 
 
-Filename: sbcli_jm-3.0.0/sbcli_jm.egg-info/
+Filename: sbcli_jm-4.0.0/simplyblock_web/
 Comment: 
 
-Filename: sbcli_jm-3.0.0/setup.cfg
+Filename: sbcli_jm-4.0.0/setup.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/pyproject.toml
+Filename: sbcli_jm-4.0.0/README.md
 Comment: 
 
-Filename: sbcli_jm-3.0.0/README.md
+Filename: sbcli_jm-4.0.0/env_var
 Comment: 
 
-Filename: sbcli_jm-3.0.0/setup.py
+Filename: sbcli_jm-4.0.0/pyproject.toml
 Comment: 
 
-Filename: sbcli_jm-3.0.0/env_var
+Filename: sbcli_jm-4.0.0/setup.cfg
 Comment: 
 
-Filename: sbcli_jm-3.0.0/PKG-INFO
+Filename: sbcli_jm-4.0.0/PKG-INFO
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_cli/cli.py
+Filename: sbcli_jm-4.0.0/simplyblock_cli/cli.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_cli/main.py
+Filename: sbcli_jm-4.0.0/simplyblock_cli/main.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/templates/
+Filename: sbcli_jm-4.0.0/sbcli_jm.egg-info/dependency_links.txt
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/blueprints/
+Filename: sbcli_jm-4.0.0/sbcli_jm.egg-info/SOURCES.txt
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/static/
+Filename: sbcli_jm-4.0.0/sbcli_jm.egg-info/top_level.txt
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/caching_node_app_k8s.py
+Filename: sbcli_jm-4.0.0/sbcli_jm.egg-info/PKG-INFO
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/app.py
+Filename: sbcli_jm-4.0.0/sbcli_jm.egg-info/requires.txt
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/node_webapp.py
+Filename: sbcli_jm-4.0.0/sbcli_jm.egg-info/entry_points.txt
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/__init__.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/services/
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/caching_node_app.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/scripts/
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/snode_app.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/controllers/
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/node_utils.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/models/
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/utils.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/storage_node_ops.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/auth_middleware.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/constants.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/templates/deploy_spdk.yaml.j2
+Filename: sbcli_jm-4.0.0/simplyblock_core/mgmt_node_ops.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_cluster.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/cnode_client.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/blueprints/caching_node_ops_k8s.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/shell_utils.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_lvol.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/pci_utils.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_storage_node.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/__init__.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/blueprints/node_api_caching_docker.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/snode_client.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/blueprints/node_api_basic.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/kv_store.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/blueprints/__init__.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/utils.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/blueprints/snode_ops.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/cluster_ops.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/blueprints/csi.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/compute_node_ops.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_mgmt_node.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/rpc_client.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_pool.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/distr_controller.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/blueprints/caching_node_ops.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/services/lvol_monitor.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/blueprints/node_api_caching_ks.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/services/caching_node_monitor.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_device.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/services/capacity_collector.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_caching_node.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/services/health_check_service.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/static/rpac.yaml
+Filename: sbcli_jm-4.0.0/simplyblock_core/services/service_template.service
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/static/deploy_spdk.yaml
+Filename: sbcli_jm-4.0.0/simplyblock_core/services/lvol_stat_collector.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/static/delete.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/services/remove_service.sh
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/static/deploy_cnode.yaml
+Filename: sbcli_jm-4.0.0/simplyblock_core/services/log_agg_service.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/static/deploy.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/services/distr_event_collector.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/static/is_up.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/services/capacity_and_stats_collector.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/static/list_deps.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/services/port_stat_collector.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_web/static/tst.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/services/device_monitor.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/
+Filename: sbcli_jm-4.0.0/simplyblock_core/services/__init__.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/controllers/
+Filename: sbcli_jm-4.0.0/simplyblock_core/services/install_service.sh
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/services/
+Filename: sbcli_jm-4.0.0/simplyblock_core/services/mgmt_node_monitor.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/models/
+Filename: sbcli_jm-4.0.0/simplyblock_core/services/cap_monitor.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/distr_controller.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/services/storage_node_monitor.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/pci_utils.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/scripts/alerting/
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/shell_utils.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/scripts/dashboards/
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/rpc_client.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/scripts/deploy_stack.sh
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/constants.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/scripts/set_db_config.sh
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/__init__.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/scripts/haproxy.cfg
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/storage_node_ops.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/scripts/docker-compose-swarm.yml
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/cnode_client.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/scripts/db_config_single.sh
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/compute_node_ops.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/scripts/stack_deploy_wait.sh
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/cluster_ops.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/scripts/config_docker.sh
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/mgmt_node_ops.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/scripts/__init__.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/utils.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/scripts/clean_local_storage_deploy.sh
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/kv_store.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/scripts/db_config_double.sh
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/snode_client.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/scripts/datasource.yml
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/alerting/
+Filename: sbcli_jm-4.0.0/simplyblock_core/scripts/run_ssh.sh
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/dashboards/
+Filename: sbcli_jm-4.0.0/simplyblock_core/scripts/install_deps.sh
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/set_db_config.sh
+Filename: sbcli_jm-4.0.0/simplyblock_core/scripts/prometheus.yml
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/stack_deploy_wait.sh
+Filename: sbcli_jm-4.0.0/simplyblock_core/scripts/apply_dashboard.sh
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/install_deps.sh
+Filename: sbcli_jm-4.0.0/simplyblock_core/scripts/alerting/alert_rules.yaml
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/run_ssh.sh
+Filename: sbcli_jm-4.0.0/simplyblock_core/scripts/alerting/alert_resources.yaml
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/config_docker.sh
+Filename: sbcli_jm-4.0.0/simplyblock_core/scripts/dashboards/devices.json
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/__init__.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/scripts/dashboards/nodes.json
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/datasource.yml
+Filename: sbcli_jm-4.0.0/simplyblock_core/scripts/dashboards/lvols.json
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/haproxy.cfg
+Filename: sbcli_jm-4.0.0/simplyblock_core/scripts/dashboards/cluster.json
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/db_config_single.sh
+Filename: sbcli_jm-4.0.0/simplyblock_core/controllers/device_controller.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/apply_dashboard.sh
+Filename: sbcli_jm-4.0.0/simplyblock_core/controllers/mgmt_events.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/prometheus.yml
+Filename: sbcli_jm-4.0.0/simplyblock_core/controllers/events_controller.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/docker-compose-swarm.yml
+Filename: sbcli_jm-4.0.0/simplyblock_core/controllers/storage_events.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/deploy_stack.sh
+Filename: sbcli_jm-4.0.0/simplyblock_core/controllers/lvol_events.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/db_config_double.sh
+Filename: sbcli_jm-4.0.0/simplyblock_core/controllers/snapshot_controller.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/clean_local_storage_deploy.sh
+Filename: sbcli_jm-4.0.0/simplyblock_core/controllers/device_events.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/alerting/alert_rules.yaml
+Filename: sbcli_jm-4.0.0/simplyblock_core/controllers/pool_controller.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/alerting/alert_resources.yaml
+Filename: sbcli_jm-4.0.0/simplyblock_core/controllers/__init__.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/dashboards/devices.json
+Filename: sbcli_jm-4.0.0/simplyblock_core/controllers/cluster_events.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/dashboards/lvols.json
+Filename: sbcli_jm-4.0.0/simplyblock_core/controllers/caching_node_controller.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/dashboards/cluster.json
+Filename: sbcli_jm-4.0.0/simplyblock_core/controllers/snapshot_events.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/scripts/dashboards/nodes.json
+Filename: sbcli_jm-4.0.0/simplyblock_core/controllers/lvol_controller.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/controllers/caching_node_controller.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/controllers/health_controller.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/controllers/device_controller.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/controllers/pool_events.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/controllers/cluster_events.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/models/events.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/controllers/lvol_events.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/models/iface.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/controllers/__init__.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/models/base_model.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/controllers/pool_events.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/models/lvol_model.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/controllers/snapshot_controller.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/models/compute_node.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/controllers/snapshot_events.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/models/snapshot.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/controllers/storage_events.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/models/pool.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/controllers/mgmt_events.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/models/global_settings.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/controllers/events_controller.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/models/port_stat.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/controllers/lvol_controller.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/models/storage_node.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/controllers/pool_controller.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/models/__init__.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/controllers/device_events.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/models/stats.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/controllers/health_controller.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/models/cluster.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/services/mgmt_node_monitor.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/models/mgmt_node.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/services/log_agg_service.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/models/caching_node.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/services/capacity_collector.py
+Filename: sbcli_jm-4.0.0/simplyblock_core/models/nvme_device.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/services/port_stat_collector.py
+Filename: sbcli_jm-4.0.0/simplyblock_web/static/
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/services/__init__.py
+Filename: sbcli_jm-4.0.0/simplyblock_web/templates/
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/services/install_service.sh
+Filename: sbcli_jm-4.0.0/simplyblock_web/blueprints/
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/services/lvol_stat_collector.py
+Filename: sbcli_jm-4.0.0/simplyblock_web/caching_node_app_k8s.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/services/device_monitor.py
+Filename: sbcli_jm-4.0.0/simplyblock_web/node_utils.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/services/storage_node_monitor.py
+Filename: sbcli_jm-4.0.0/simplyblock_web/snode_app.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/services/lvol_monitor.py
+Filename: sbcli_jm-4.0.0/simplyblock_web/app.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/services/distr_event_collector.py
+Filename: sbcli_jm-4.0.0/simplyblock_web/auth_middleware.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/services/remove_service.sh
+Filename: sbcli_jm-4.0.0/simplyblock_web/__init__.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/services/health_check_service.py
+Filename: sbcli_jm-4.0.0/simplyblock_web/caching_node_app.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/services/caching_node_monitor.py
+Filename: sbcli_jm-4.0.0/simplyblock_web/utils.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/services/cap_monitor.py
+Filename: sbcli_jm-4.0.0/simplyblock_web/node_webapp.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/services/service_template.service
+Filename: sbcli_jm-4.0.0/simplyblock_web/static/deploy_cnode.yaml
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/services/capacity_and_stats_collector.py
+Filename: sbcli_jm-4.0.0/simplyblock_web/static/tst.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/models/global_settings.py
+Filename: sbcli_jm-4.0.0/simplyblock_web/static/is_up.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/models/cluster.py
+Filename: sbcli_jm-4.0.0/simplyblock_web/static/delete.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/models/caching_node.py
+Filename: sbcli_jm-4.0.0/simplyblock_web/static/deploy.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/models/pool.py
+Filename: sbcli_jm-4.0.0/simplyblock_web/static/deploy_spdk.yaml
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/models/events.py
+Filename: sbcli_jm-4.0.0/simplyblock_web/static/rpac.yaml
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/models/iface.py
+Filename: sbcli_jm-4.0.0/simplyblock_web/static/list_deps.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/models/base_model.py
+Filename: sbcli_jm-4.0.0/simplyblock_web/templates/deploy_spdk.yaml.j2
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/models/__init__.py
+Filename: sbcli_jm-4.0.0/simplyblock_web/blueprints/node_api_caching_docker.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/models/stats.py
+Filename: sbcli_jm-4.0.0/simplyblock_web/blueprints/node_api_caching_ks.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/models/nvme_device.py
+Filename: sbcli_jm-4.0.0/simplyblock_web/blueprints/web_api_caching_node.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/models/storage_node.py
+Filename: sbcli_jm-4.0.0/simplyblock_web/blueprints/snode_ops.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/models/port_stat.py
+Filename: sbcli_jm-4.0.0/simplyblock_web/blueprints/web_api_lvol.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/models/mgmt_node.py
+Filename: sbcli_jm-4.0.0/simplyblock_web/blueprints/csi.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/models/snapshot.py
+Filename: sbcli_jm-4.0.0/simplyblock_web/blueprints/caching_node_ops.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/models/compute_node.py
+Filename: sbcli_jm-4.0.0/simplyblock_web/blueprints/web_api_mgmt_node.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/simplyblock_core/models/lvol_model.py
+Filename: sbcli_jm-4.0.0/simplyblock_web/blueprints/web_api_storage_node.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/sbcli_jm.egg-info/top_level.txt
+Filename: sbcli_jm-4.0.0/simplyblock_web/blueprints/__init__.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/sbcli_jm.egg-info/SOURCES.txt
+Filename: sbcli_jm-4.0.0/simplyblock_web/blueprints/caching_node_ops_k8s.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/sbcli_jm.egg-info/dependency_links.txt
+Filename: sbcli_jm-4.0.0/simplyblock_web/blueprints/web_api_device.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/sbcli_jm.egg-info/entry_points.txt
+Filename: sbcli_jm-4.0.0/simplyblock_web/blueprints/web_api_cluster.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/sbcli_jm.egg-info/requires.txt
+Filename: sbcli_jm-4.0.0/simplyblock_web/blueprints/node_api_basic.py
 Comment: 
 
-Filename: sbcli_jm-3.0.0/sbcli_jm.egg-info/PKG-INFO
+Filename: sbcli_jm-4.0.0/simplyblock_web/blueprints/web_api_pool.py
 Comment: 
 
 Zip file comment:
```

## Comparing `sbcli_jm-3.0.0/README.md` & `sbcli_jm-4.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # Components 
 
 ## Simply Block Core
 Contains core logic and controllers for the simplyblock cluster
 
 ## Simply Block CLI
 Please see this document 
-[README.md](../simplyblock_cli/README.md)
+[README.md](../main/simplyblock_cli/README.md)
 
 
 ## Simply Block Web API
 Please see this document 
-[README.md](../simplyblock_web/README.md)
+[README.md](../main/simplyblock_web/README.md)
```

## Comparing `sbcli_jm-3.0.0/setup.py` & `sbcli_jm-4.0.0/setup.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/PKG-INFO` & `sbcli_jm-4.0.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-jm
-Version: 3.0.0
+Version: 4.0.0
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
@@ -29,16 +29,16 @@
 # Components 
 
 ## Simply Block Core
 Contains core logic and controllers for the simplyblock cluster
 
 ## Simply Block CLI
 Please see this document 
-[README.md](../simplyblock_cli/README.md)
+[README.md](../main/simplyblock_cli/README.md)
 
 
 ## Simply Block Web API
 Please see this document 
-[README.md](../simplyblock_web/README.md)
+[README.md](../main/simplyblock_web/README.md)
```

## Comparing `sbcli_jm-3.0.0/simplyblock_cli/cli.py` & `sbcli_jm-4.0.0/simplyblock_cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -442,14 +442,18 @@
                                  dest='ha_type', choices=["single", "ha", "default"], default='default')
 
         sub_command.add_argument("--compress",
                                  help='Use inline data compression and de-compression on the logical volume',
                                  required=False, action='store_true')
         sub_command.add_argument("--encrypt", help='Use inline data encryption and de-cryption on the logical volume',
                                  required=False, action='store_true')
+        sub_command.add_argument("--crypto-key1", help='the hex value of key1 to be used for lvol encryption',
+                                 dest='crypto_key1', default=None)
+        sub_command.add_argument("--crypto-key2", help='the hex value of key2 to be used for lvol encryption',
+                                 dest='crypto_key2', default=None)
         sub_command.add_argument("--thick", help='Deactivate thin provisioning', required=False, action='store_true')
         sub_command.add_argument("--node-ha",
                                  help='The maximum amount of concurrent node failures accepted without interruption of operations',
                                  required=False, default=1, type=int, choices=[0, 1, 2])
         sub_command.add_argument("--dev-redundancy",
                                  help='{1,2} supported minimal concurrent device failures without data loss',
                                  required=False, action='store_true')
@@ -1069,15 +1073,17 @@
                     args.max_rw_iops,
                     args.max_rw_mbytes,
                     args.max_r_mbytes,
                     args.max_w_mbytes,
                     distr_bs,
                     distr_chunk_bs,
                     with_snapshot=with_snapshot,
-                    max_size=max_size)
+                    max_size=max_size,
+                    crypto_key1=args.crypto_key1,
+                    crypto_key2=args.crypto_key2)
                 if results:
                     ret = results
                 else:
                     ret = error
             elif sub_command == "add-distr":
                 pass
             elif sub_command == "qos-set":
```

## Comparing `sbcli_jm-3.0.0/simplyblock_web/caching_node_app_k8s.py` & `sbcli_jm-4.0.0/simplyblock_web/caching_node_app_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_web/app.py` & `sbcli_jm-4.0.0/simplyblock_web/app.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_web/node_webapp.py` & `sbcli_jm-4.0.0/simplyblock_web/node_webapp.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_web/caching_node_app.py` & `sbcli_jm-4.0.0/simplyblock_web/caching_node_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_web/snode_app.py` & `sbcli_jm-4.0.0/simplyblock_web/snode_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_web/node_utils.py` & `sbcli_jm-4.0.0/simplyblock_web/node_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_web/utils.py` & `sbcli_jm-4.0.0/simplyblock_web/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             elif size_v == "g":
                 multi = 3
             elif size_v == "t":
                 multi = 4
             else:
                 print(f"Error parsing size: {size_string}")
                 return -1
-            return size_number * math.pow(one_k, multi)
+            return int(size_number * math.pow(one_k, multi))
         else:
             return -1
     except:
         print(f"Error parsing size: {size_string}")
         return -1
```

## Comparing `sbcli_jm-3.0.0/simplyblock_web/auth_middleware.py` & `sbcli_jm-4.0.0/simplyblock_web/auth_middleware.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_web/templates/deploy_spdk.yaml.j2` & `sbcli_jm-4.0.0/simplyblock_web/templates/deploy_spdk.yaml.j2`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_cluster.py` & `sbcli_jm-4.0.0/simplyblock_web/blueprints/web_api_cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_web/blueprints/caching_node_ops_k8s.py` & `sbcli_jm-4.0.0/simplyblock_web/blueprints/caching_node_ops_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_lvol.py` & `sbcli_jm-4.0.0/simplyblock_web/blueprints/web_api_lvol.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,15 +90,16 @@
         | max_w_mbytes    | Maximum Write Mega Bytes Per Second
         | ha_type         | LVol HA type, can be (single,ha,default=cluster's ha type), Default=default
         | distr_vuid      | Distr bdev virtual unique ID, Default=0 means random
         | distr_ndcs      | Distr bdev number of data chunks per stripe, Default=0 means auto set
         | distr_npcs      | Distr bdev number of parity chunks per stripe, Default=0 means auto set
         | distr_bs        | Distr bdev block size, Default=4096
         | distr_chunk_bs  | Distr bdev chunk block size, Default=4096
-
+        | crypto_key1     | the hex value of key1 to be used for lvol encryption
+        | crypto_key2     | the hex value of key2 to be used for lvol encryption
     """""
 
     cl_data = request.get_json()
     logger.debug(cl_data)
     if 'size' not in cl_data:
         return utils.get_csi_response(None, "missing required param: size", 400)
     if 'name' not in cl_data:
@@ -134,14 +135,16 @@
     ha_type = utils.get_value_or_default(cl_data, "ha_type", "default")
 
     distr_vuid = utils.get_int_value_or_default(cl_data, "distr_vuid", 0)
     distr_ndcs = utils.get_int_value_or_default(cl_data, "distr_ndcs", 0)
     distr_npcs = utils.get_int_value_or_default(cl_data, "distr_npcs", 0)
     distr_bs = utils.get_int_value_or_default(cl_data, "distr_ps", 4096)
     distr_chunk_bs = utils.get_int_value_or_default(cl_data, "distr_chunk_bs", 4096)
+    crypto_key1 = utils.get_value_or_default(cl_data, "crypto_key1", None)
+    crypto_key2 = utils.get_value_or_default(cl_data, "crypto_key2", None)
 
     ret, error = lvol_controller.add_lvol_ha(
         name=name,
         size=size,
         pool_id_or_name=pool.get_id(),
 
         use_comp=compression,
@@ -154,15 +157,17 @@
 
         host_id_or_name=None,
         ha_type=ha_type,
         distr_vuid=distr_vuid,
         distr_ndcs=distr_ndcs,
         distr_npcs=distr_npcs,
         distr_bs=distr_bs,
-        distr_chunk_bs=distr_chunk_bs
+        distr_chunk_bs=distr_chunk_bs,
+        crypto_key1=crypto_key1,
+        crypto_key2=crypto_key2,
     )
 
     return utils.get_csi_response(ret, error)
 
 
 @bp.route('/lvol/<string:uuid>', methods=['PUT'])
 def update_lvol(uuid):
```

## Comparing `sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_storage_node.py` & `sbcli_jm-4.0.0/simplyblock_web/blueprints/web_api_storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_web/blueprints/node_api_caching_docker.py` & `sbcli_jm-4.0.0/simplyblock_web/blueprints/node_api_caching_docker.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_web/blueprints/node_api_basic.py` & `sbcli_jm-4.0.0/simplyblock_web/blueprints/node_api_basic.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_web/blueprints/snode_ops.py` & `sbcli_jm-4.0.0/simplyblock_web/blueprints/snode_ops.py`

 * *Files 19% similar despite different names*

```diff
@@ -188,14 +188,34 @@
 
 
 def delete_cluster_id():
     out, _, _ = node_utils.run_command(f"rm -f {cluster_id_file}")
     return out
 
 
+def get_ec2_meta():
+    stream = os.popen('curl -X PUT "http://169.254.169.254/latest/api/token" -H "X-aws-ec2-metadata-token-ttl-seconds: 21600"')
+    token = stream.read()
+    stream = os.popen(f"curl -H \"X-aws-ec2-metadata-token: {token}\" http://169.254.169.254/latest/dynamic/instance-identity/document")
+    out = stream.read()
+    try:
+        data = json.loads(out)
+        return data
+    except:
+        return {}
+
+
+def get_ec2_public_ip():
+    stream = os.popen('curl -X PUT "http://169.254.169.254/latest/api/token" -H "X-aws-ec2-metadata-token-ttl-seconds: 21600"')
+    token = stream.read()
+    stream = os.popen(f"curl -H \"X-aws-ec2-metadata-token: {token}\" http://169.254.169.254/latest/meta-data/public-ipv4")
+    out = stream.read()
+    return out
+
+
 @bp.route('/info', methods=['GET'])
 def get_info():
 
     out = {
         "cluster_id": get_cluster_id(),
 
         "hostname": hostname,
@@ -210,15 +230,19 @@
 
         "nvme_devices": node_utils._get_nvme_devices(),
         "nvme_pcie_list": node_utils._get_nvme_pcie_list(),
 
         "spdk_devices": node_utils._get_spdk_devices(),
         "spdk_pcie_list": node_utils._get_spdk_pcie_list(),
 
-        "network_interface": node_utils.get_nics_data()
+        "network_interface": node_utils.get_nics_data(),
+
+        "ec2_metadata": get_ec2_meta(),
+
+        "ec2_public_ip": get_ec2_public_ip(),
     }
     return utils.get_response(out)
 
 
 @bp.route('/join_swarm', methods=['POST'])
 def join_swarm():
     data = request.get_json()
@@ -264,7 +288,29 @@
     delete_cluster_id()
     try:
         node_docker = docker.DockerClient(base_url='unix://var/run/docker.sock')
         node_docker.swarm.leave(force=True)
     except:
         pass
     return utils.get_response(True)
+
+
+@bp.route('/make_gpt_partitions', methods=['POST'])
+def make_gpt_partitions_for_nbd():
+    nbd_device = '/dev/nbd0'
+    jm_percent = '3'
+
+    try:
+        data = request.get_json()
+        nbd_device = data['nbd_device']
+        jm_percent = data['jm_percent']
+    except:
+        pass
+
+    os.popen("modprobe nbd")
+    os.popen(f"parted -s {nbd_device} mklabel gpt")
+    os.popen(f"parted -s {nbd_device} mkpart journal '0%' '{jm_percent}%'")
+    os.popen(f"parted -s {nbd_device} mkpart main '{jm_percent}%' '100%'")
+    os.popen(f"sgdisk -t 1:6527994e-2c5a-4eec-9613-8f5944074e8b {nbd_device}")
+    os.popen(f"sgdisk -t 2:6527994e-2c5a-4eec-9613-8f5944074e8b {nbd_device}")
+
+    return utils.get_response(True)
```

## Comparing `sbcli_jm-3.0.0/simplyblock_web/blueprints/csi.py` & `sbcli_jm-4.0.0/simplyblock_web/blueprints/csi.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_mgmt_node.py` & `sbcli_jm-4.0.0/simplyblock_web/blueprints/web_api_mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_pool.py` & `sbcli_jm-4.0.0/simplyblock_web/blueprints/web_api_pool.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_web/blueprints/caching_node_ops.py` & `sbcli_jm-4.0.0/simplyblock_web/blueprints/caching_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_web/blueprints/node_api_caching_ks.py` & `sbcli_jm-4.0.0/simplyblock_web/blueprints/node_api_caching_ks.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_device.py` & `sbcli_jm-4.0.0/simplyblock_web/blueprints/web_api_device.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_web/blueprints/web_api_caching_node.py` & `sbcli_jm-4.0.0/simplyblock_web/blueprints/web_api_caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_web/static/deploy_spdk.yaml` & `sbcli_jm-4.0.0/simplyblock_web/static/deploy_spdk.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_web/static/delete.py` & `sbcli_jm-4.0.0/simplyblock_web/static/delete.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_web/static/deploy.py` & `sbcli_jm-4.0.0/simplyblock_web/static/deploy.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/distr_controller.py` & `sbcli_jm-4.0.0/simplyblock_core/distr_controller.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # coding=utf-8
 import datetime
 import logging
 import re
 
+from simplyblock_core.models.nvme_device import NVMeDevice
 from simplyblock_core.rpc_client import RPCClient
 from simplyblock_core.kv_store import DBController
 
 logger = logging.getLogger()
 
 
 def send_node_status_event(node_id, node_status):
@@ -65,37 +66,34 @@
         node.write_to_db(db_controller.kv_store)
 
 
 def get_distr_cluster_map(snodes, target_node):
     map_cluster = {}
     map_prob = []
     for snode in snodes:
-        if snode.status not in [snode.STATUS_ONLINE, snode.STATUS_RESTARTING]:
-            logger.debug(f"Node is not online: {snode.get_id()}, status: {snode.status}")
-            continue
         dev_map = {}
         dev_w_map = []
         node_w = 0
-
         for i, dev in enumerate(snode.nvme_devices):
             logger.debug(f"Device: {dev.get_id()}, status: {dev.status}")
-            if dev.status == "JM_DEV":
+            if dev.status == NVMeDevice.STATUS_JM:
                 continue
+
             dev_w = int(dev.size/(1024*1024*1024)) or 1
             node_w += dev_w
             name = None
             if snode.get_id() == target_node.get_id():
                 name = dev.alceml_bdev
             else:
                 for dev2 in target_node.remote_devices:
                     if dev2.get_id() == dev.get_id():
                         name = dev2.remote_bdev
                         break
             if not name:
-                continue
+                name = f"remote_{dev.alceml_bdev}n1"
             dev_map[dev.cluster_device_order] = {
                 "UUID": dev.get_id(),
                 "bdev_name": name,
                 "status": dev.status}
             dev_w_map.append({
                 "weight": dev_w,
                 "id": dev.cluster_device_order})
@@ -166,8 +164,43 @@
                 else:
                     data["Results"] = "failed"
                     passed = False
             else:
                 data["Results"] = "not found"
                 passed = False
             results.append(data)
-    return results, passed
+    return results, passed
+
+
+def send_cluster_map_to_node(node):
+    db_controller = DBController()
+    snodes = db_controller.get_storage_nodes()
+    rpc_client = RPCClient(node.mgmt_ip, node.rpc_port, node.rpc_username, node.rpc_password)
+    cluster_map_data = get_distr_cluster_map(snodes, node)
+    cluster_map_data['UUID_node_target'] = node.get_id()
+    ret = rpc_client.distr_send_cluster_map(cluster_map_data)
+    if not ret:
+        logger.error("Failed to send cluster map")
+        logger.info(cluster_map_data)
+        return False
+    return True
+
+
+def send_cluster_map_add_node(snode):
+    db_controller = DBController()
+    snodes = db_controller.get_storage_nodes()
+    for node in snodes:
+        if node.status != node.STATUS_ONLINE:
+            continue
+        logger.info(f"Sending to: {node.get_id()}")
+        rpc_client = RPCClient(node.mgmt_ip, node.rpc_port, node.rpc_username, node.rpc_password)
+
+        cluster_map_data = get_distr_cluster_map([snode], node)
+        cl_map = {
+            "map_cluster": cluster_map_data['map_cluster'],
+            "map_prob": cluster_map_data['map_prob']}
+        ret = rpc_client.distr_add_nodes(cl_map)
+        if not ret:
+            logger.error("Failed to send cluster map")
+            logger.info(cl_map)
+            return False
+    return True
```

## Comparing `sbcli_jm-3.0.0/simplyblock_core/pci_utils.py` & `sbcli_jm-4.0.0/simplyblock_core/pci_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/rpc_client.py` & `sbcli_jm-4.0.0/simplyblock_core/rpc_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,14 +320,15 @@
             "base_bdev_name": base_name,
             "name": name,
             "key_name": key_name,
         }
         return self._request("bdev_crypto_create", params)
 
     def lvol_crypto_key_create(self, name, key, key2):
+        # todo: mask the keys so that they don't show up in logs
         params = {
             "cipher": "AES_XTS",
             "key": key,
             "key2": key2,
             "name": name
         }
         return self._request("accel_crypto_key_create", params)
@@ -336,17 +337,17 @@
         params = {"name": name}
         return self._request("bdev_crypto_delete", params)
 
     def lvol_compress_delete(self, name):
         params = {"name": name}
         return self._request("bdev_compress_delete", params)
 
-    def ultra21_bdev_pass_create(self, alloc_bdev, vuid, pt_name):
+    def ultra21_bdev_pass_create(self, base_bdev, vuid, pt_name):
         params = {
-            "base_bdev": alloc_bdev,
+            "base_bdev": base_bdev,
             "vuid": vuid,
             "pt_bdev": pt_name
         }
         return self._request2("ultra21_bdev_pass_create", params)
 
     def ultra21_bdev_pass_delete(self, name):
         params = {"name": name}
@@ -641,7 +642,24 @@
     def jm_delete(self):
         params = {"name": 0, "vuid": 0}
         return self._request("jm_delete", params)
 
     def framework_start_init(self):
         return self._request("framework_start_init")
 
+    def bdev_examine(self, name):
+        params = {"name": name}
+        return self._request("bdev_examine", params)
+
+    def nbd_start_disk(self, bdev_name, nbd_device="/dev/nbd0"):
+        params = {
+            "bdev_name": bdev_name,
+            "nbd_device": nbd_device,
+        }
+        return self._request("nbd_start_disk", params)
+
+    def nbd_stop_disk(self, nbd_device):
+        params = {
+            "nbd_device": nbd_device
+        }
+        return self._request("nbd_stop_disk", params)
+
```

## Comparing `sbcli_jm-3.0.0/simplyblock_core/constants.py` & `sbcli_jm-4.0.0/simplyblock_core/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,12 +46,12 @@
 
 # To use 75% of hugepages to calculate ssd size to use for the ocf bdev
 CACHING_NODE_MEMORY_FACTOR = 0.75
 
 HEALTH_CHECK_INTERVAL_SEC = 60
 
 
-SIMPLY_BLOCK_DOCKER_IMAGE = "simplyblock/simplyblock:dev"
+SIMPLY_BLOCK_DOCKER_IMAGE = "simplyblock/simplyblock:jm_4.0.0"
 SIMPLY_BLOCK_SPDK_CORE_IMAGE = "simplyblock/spdk-core:latest"
 SIMPLY_BLOCK_SPDK_ULTRA_IMAGE = "simplyblock/spdk:main-latest"
 
 GELF_PORT = 12201
```

## Comparing `sbcli_jm-3.0.0/simplyblock_core/storage_node_ops.py` & `sbcli_jm-4.0.0/simplyblock_core/storage_node_ops.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,52 +88,61 @@
         ctr_map = {i["ctrlrs"][0]['trid']['traddr']: i["name"] for i in ret}
     else:
         ctr_map = {}
 
     for index, pcie in enumerate(devs):
 
         if pcie in ctr_map:
-            nvme_bdev = ctr_map[pcie] + "n1"
+            nvme_controller = ctr_map[pcie]
         else:
-            name = "nvme_%s" % index
-            ret, err = rpc_client.bdev_nvme_controller_attach(name, pcie)
+            nvme_controller = "nvme_%s" % index
+            ret, err = rpc_client.bdev_nvme_controller_attach(nvme_controller, pcie)
             time.sleep(2)
-            nvme_bdev = f"{name}n1"
 
+        nvme_bdev = f"{nvme_controller}n1"
+        rpc_client.bdev_examine(nvme_bdev)
         ret = rpc_client.get_bdevs(nvme_bdev)
-        if ret:
-            nvme_dict = ret[0]
-            nvme_driver_data = nvme_dict['driver_specific']['nvme'][0]
-            model_number = nvme_driver_data['ctrlr_data']['model_number']
-
-            size = nvme_dict['block_size'] * nvme_dict['num_blocks']
-            device_partitions_count = int(size / (cluster.blk_size * cluster.page_size_in_blocks))
-            devices.append(
-                NVMeDevice({
-                    'uuid': str(uuid.uuid4()),
-                    'device_name': nvme_dict['name'],
-                    'sequential_number': sequential_number,
-                    'partitions_count': device_partitions_count,
-                    'capacity': size,
-                    'size': size,
-                    'pcie_address': nvme_driver_data['pci_address'],
-                    'model_id': model_number,
-                    'serial_number': nvme_driver_data['ctrlr_data']['serial_number'],
-                    'nvme_bdev': nvme_bdev,
-                    'alloc_bdev': nvme_bdev,
-                    'node_id': snode.get_id(),
-                    'cluster_id': snode.cluster_id,
-
-                    # 'nvmf_nqn': subsystem_nqn,
-                    # 'nvmf_ip': IP,
-                    # 'nvmf_port': 4420,
-
-                    'status': 'online'
-                }))
-            sequential_number += device_partitions_count
+        nvme_dict = ret[0]
+        nvme_driver_data = nvme_dict['driver_specific']['nvme'][0]
+        model_number = nvme_driver_data['ctrlr_data']['model_number']
+        size = nvme_dict['block_size'] * nvme_dict['num_blocks']
+        device_partitions_count = int(size / (cluster.blk_size * cluster.page_size_in_blocks))
+        # look for partitions
+        jm_bdev = ""
+        nvme_main_bdev = ""
+        for bdev in rpc_client.get_bdevs():
+            if bdev['name'] == f"{nvme_bdev}p1":
+                jm_bdev = bdev['name']
+            elif bdev['name'] == f"{nvme_bdev}p2":
+                nvme_main_bdev = bdev['name']
+        devices.append(
+            NVMeDevice({
+                'uuid': str(uuid.uuid4()),
+                'device_name': nvme_dict['name'],
+                'sequential_number': sequential_number,
+                'partitions_count': device_partitions_count,
+                'capacity': size,
+                'size': size,
+                'pcie_address': nvme_driver_data['pci_address'],
+                'model_id': model_number,
+                'serial_number': nvme_driver_data['ctrlr_data']['serial_number'],
+                'nvme_bdev': nvme_bdev,
+                'nvme_controller': nvme_controller,
+                'node_id': snode.get_id(),
+                'cluster_id': snode.cluster_id,
+                'jm_bdev': jm_bdev,
+                'nvme_main_bdev': nvme_main_bdev,
+
+                # 'nvmf_nqn': subsystem_nqn,
+                # 'nvmf_ip': IP,
+                # 'nvmf_port': 4420,
+
+                'status': 'online'
+        }))
+        sequential_number += device_partitions_count
     return devices
 
 
 def _get_nvme_list(cluster):
     out, err, _ = shell_utils.run_command("sudo nvme list -v -o json")
     data = json.loads(out)
     logger.debug("nvme list:")
@@ -214,30 +223,53 @@
 
     rpc_client = RPCClient(
         snode.mgmt_ip, snode.rpc_port,
         snode.rpc_username, snode.rpc_password)
 
     jm_nvme_bdevs = []
     for index, nvme in enumerate(snode.nvme_devices):
-        if nvme.status not in [NVMeDevice.STATUS_ONLINE, NVMeDevice.STATUS_UNAVAILABLE]:
-            logger.debug(f"Device is not online or unavailable: {nvme.get_id()}, status: {nvme.status}")
+        if nvme.status not in [NVMeDevice.STATUS_ONLINE, NVMeDevice.STATUS_UNAVAILABLE, NVMeDevice.STATUS_READONLY]:
+            logger.debug(f"Device is skipped: {nvme.get_id()}, status: {nvme.status}")
             continue
 
-        ret = rpc_client.bdev_split(nvme.nvme_bdev, 10)
-        if not ret:
-            logger.error(f"Failed to split nvme bdev: {nvme.nvme_bdev}")
-            return False
-        jm_nvme_bdevs.append(f"{nvme.nvme_bdev}p0")
-        ret = rpc_client.bdev_raid_create(f"raid_{nvme.nvme_bdev}", [f"{nvme.nvme_bdev}p{i}" for i in range(1,10)])
-        if not ret:
-            logger.error(f"Failed to create raid_{nvme.nvme_bdev}")
-            return False
+        if nvme.nvme_main_bdev and nvme.jm_bdev:
+            logger.info(f"Device partitions found, JM: {nvme.jm_bdev}, main: {nvme.nvme_main_bdev}")
+        else:
+            logger.info(f"Creating partitions for {nvme.nvme_bdev}")
+
+            nbd_device = rpc_client.nbd_start_disk(nvme.nvme_bdev)
+            if not nbd_device:
+                logger.error(f"Failed to start nbd dev")
+                return False
+            snode_api = SNodeClient(snode.mgmt_ip)
+            ret = snode_api.make_gpt_partitions(nbd_device, "3")
+            if not ret:
+                logger.error(f"Failed to make partitions")
+                return False
+            rpc_client.nbd_stop_disk(nbd_device)
+            rpc_client.bdev_nvme_detach_controller(nvme.nvme_controller)
+            time.sleep(3)
+            rpc_client.bdev_nvme_controller_attach(nvme.nvme_controller, nvme.pcie_address)
+            rpc_client.bdev_examine(nvme.nvme_bdev)
+            bdevs = rpc_client.get_bdevs()
+            for bdev in bdevs:
+                if bdev['name'] == f"{nvme.nvme_bdev}p1":
+                    nvme.jm_bdev = bdev['name']
+                elif bdev['name'] == f"{nvme.nvme_bdev}p2":
+                    nvme.nvme_main_bdev = bdev['name']
+
+            if nvme.nvme_main_bdev and nvme.jm_bdev:
+                logger.info(f"Device partitions created, JM: {nvme.jm_bdev}, main: {nvme.nvme_main_bdev}")
+            else:
+                logger.error("Failed to create partitions")
+                return False
+
+        jm_nvme_bdevs.append(nvme.jm_bdev)
         test_name = f"{nvme.nvme_bdev}_test"
-        # create testing bdev
-        ret = rpc_client.bdev_passtest_create(test_name, f"raid_{nvme.nvme_bdev}")
+        ret = rpc_client.bdev_passtest_create(test_name, nvme.nvme_main_bdev)
         if not ret:
             logger.error(f"Failed to create passtest bdev {test_name}")
             return False
         alceml_id = nvme.get_id()
         alceml_name = f"alceml_{alceml_id}"
         logger.info(f"adding {alceml_name}")
         pba_init_mode = 3
@@ -283,15 +315,18 @@
         nvme.testing_bdev = test_name
         nvme.alceml_bdev = alceml_name
         nvme.pt_bdev = pt_name
         nvme.nvmf_nqn = subsystem_nqn
         nvme.nvmf_ip = IP
         nvme.nvmf_port = 4420
         nvme.io_error = False
+        old_status = nvme.status
         nvme.status = NVMeDevice.STATUS_ONLINE
+        device_events.device_status_change(nvme, nvme.status, old_status)
+        snode.write_to_db(db_controller.kv_store)
 
     if jm_nvme_bdevs:
         ret = rpc_client.bdev_raid_create(f"raid_jm_{snode.get_id()}", jm_nvme_bdevs)
         if not ret:
             logger.error(f"Failed to create raid_jm_{snode.get_id()}")
             return False
         alceml_name = f"alceml_jm_{snode.get_id()}"
@@ -299,18 +334,20 @@
         if after_restart:
             pba_init_mode = 2
         ret = rpc_client.bdev_alceml_create(alceml_name, f"raid_jm_{snode.get_id()}", str(uuid.uuid4()), pba_init_mode=pba_init_mode)
         if not ret:
             logger.error(f"Failed to create alceml bdev: {alceml_name}")
             return False
 
-        ret = rpc_client.bdev_jm_create(f"jm_{snode.get_id()}", alceml_name)
+        jm_bdev = f"jm_{snode.get_id()}"
+        ret = rpc_client.bdev_jm_create(jm_bdev, alceml_name)
         if not ret:
-            logger.error(f"Failed to create jm_{snode.get_id()}")
+            logger.error(f"Failed to create {jm_bdev}")
             return False
+        snode.jm_bdev = jm_bdev
 
     snode.write_to_db(db_controller.kv_store)
     return True
 
 
 def _connect_to_remote_devs(this_node):
     db_controller = DBController()
@@ -359,14 +396,49 @@
     node_info, _ = snode_api.info()
     logger.info(f"Node found: {node_info['hostname']}")
     if "cluster_id" in node_info and node_info['cluster_id']:
         if node_info['cluster_id'] != cluster_id:
             logger.error(f"This node is part of another cluster: {node_info['cluster_id']}")
             return False
 
+    ec2_metadata = None
+    if "ec2_metadata" in node_info and node_info['ec2_metadata']:
+        ec2_metadata = node_info['ec2_metadata']
+        """"
+         "ec2_metadata": {
+              "accountId": "565979732541",
+              "architecture": "x86_64",
+              "availabilityZone": "eu-west-1a",
+              "billingProducts": [
+                "bp-6fa54006"
+              ],
+              "devpayProductCodes": null,
+              "imageId": "ami-08e592fbb0f535224",
+              "instanceId": "i-0ba9e766df57bc62c",
+              "instanceType": "m6id.large",
+              "kernelId": null,
+              "marketplaceProductCodes": null,
+              "pendingTime": "2024-03-24T19:39:14Z",
+              "privateIp": "172.31.23.236",
+              "ramdiskId": null,
+              "region": "eu-west-1",
+              "version": "2017-09-30"
+        }
+        """""
+        logger.debug(json.dumps(ec2_metadata,indent=2))
+        logger.info(f"EC2 Instance found: {ec2_metadata['instanceId']}")
+        logger.info(f"EC2 Instance type: {ec2_metadata['instanceType']}")
+        logger.info(f"EC2 Instance privateIp: {ec2_metadata['privateIp']}")
+        logger.info(f"EC2 Instance region: {ec2_metadata['region']}")
+
+        for node in db_controller.get_storage_nodes():
+            if node.ec2_instance_id and node.ec2_instance_id == ec2_metadata['instanceId']:
+                logger.error(f"Node already exists, try remove it first: {ec2_metadata['instanceId']}")
+                return False
+
     # check for memory
     if "memory_details" in node_info and node_info['memory_details']:
         memory_details = node_info['memory_details']
         logger.info("Node Memory info")
         logger.info(f"Total: {utils.humanbytes(memory_details['total'])}")
         logger.info(f"Free: {utils.humanbytes(memory_details['free'])}")
         logger.info(f"Hugepages Total: {utils.humanbytes(memory_details['huge_total'])}")
@@ -394,41 +466,44 @@
     logger.info("Deploying SPDK")
     results, err = snode_api.spdk_process_start(spdk_cpu_mask, spdk_mem, spdk_image, spdk_debug, cluster_ip)
     time.sleep(10)
     if not results:
         logger.error(f"Failed to start spdk: {err}")
         return False
 
-    hostname = node_info['hostname']
-    snode = db_controller.get_storage_node_by_hostname(hostname)
-    if snode:
-        logger.error("Node already exists, try remove it first.")
-        return False
-
     data_nics = []
     names = data_nics_list or [iface_name]
     for nic in names:
         device = node_info['network_interface'][nic]
         data_nics.append(
             IFace({
                 'uuid': str(uuid.uuid4()),
                 'if_name': device['name'],
                 'ip4_address': device['ip'],
                 'status': device['status'],
                 'net_type': device['net_type']}))
 
+    hostname = node_info['hostname']
     rpc_user, rpc_pass = utils.generate_rpc_user_and_pass()
     BASE_NQN = cluster.nqn.split(":")[0]
     subsystem_nqn = f"{BASE_NQN}:{hostname}"
     # creating storage node object
     snode = StorageNode()
     snode.uuid = str(uuid.uuid4())
     snode.status = StorageNode.STATUS_IN_CREATION
     snode.baseboard_sn = node_info['system_id']
     snode.system_uuid = node_info['system_id']
+
+    if ec2_metadata:
+        snode.ec2_metadata = ec2_metadata
+        snode.ec2_instance_id = ec2_metadata['instanceId']
+
+    if "ec2_public_ip" in node_info and node_info['ec2_public_ip']:
+        snode.ec2_public_ip = node_info['ec2_public_ip']
+
     snode.hostname = hostname
     snode.host_nqn = subsystem_nqn
     snode.subsystem = subsystem_nqn
     snode.data_nics = data_nics
     snode.mgmt_ip = node_info['network_interface'][iface_name]['ip']
     snode.rpc_port = constants.RPC_HTTP_PROXY_PORT
     snode.rpc_username = rpc_user
@@ -551,31 +626,21 @@
             else:
                 node.remote_devices.append(dev)
             count += 1
         node.write_to_db(kv_store)
         logger.info(f"connected to devices count: {count}")
 
     logger.info("Sending cluster map")
-    snodes = db_controller.get_storage_nodes()
-    for node in snodes:
-        if node.status != node.STATUS_ONLINE:
-            continue
-        logger.info(f"Sending to: {node.get_id()}")
-        rpc_client = RPCClient(node.mgmt_ip, node.rpc_port, node.rpc_username, node.rpc_password)
-        if node.get_id() == snode.get_id():
-            cluster_map_data = distr_controller.get_distr_cluster_map(snodes, node)
-            cluster_map_data['UUID_node_target'] = node.get_id()
-            ret = rpc_client.distr_send_cluster_map(cluster_map_data)
-        else:
-            cluster_map_data = distr_controller.get_distr_cluster_map([snode], node)
-            cl_map = {
-                "map_cluster": cluster_map_data['map_cluster'],
-                "map_prob": cluster_map_data['map_prob']}
-            ret = rpc_client.distr_add_nodes(cl_map)
-        time.sleep(3)
+    ret = distr_controller.send_cluster_map_to_node(snode)
+    if not ret:
+        return False, "Failed to send cluster map"
+    ret = distr_controller.send_cluster_map_add_node(snode)
+    if not ret:
+        return False, "Failed to send cluster map add node"
+    time.sleep(3)
 
     logger.info("Sending cluster event updates")
     distr_controller.send_node_status_event(snode.get_id(), "online")
 
     for dev in snode.nvme_devices:
         distr_controller.send_dev_status_event(dev.cluster_device_order, "online")
 
@@ -696,31 +761,21 @@
             else:
                 node.remote_devices.append(dev)
             count += 1
         node.write_to_db(kv_store)
         logger.info(f"connected to devices count: {count}")
 
     logger.info("Sending cluster map")
-    snodes = db_controller.get_storage_nodes()
-    for node in snodes:
-        if node.status != node.STATUS_ONLINE:
-            continue
-        logger.info(f"Sending to: {node.get_id()}")
-        rpc_client = RPCClient(node.mgmt_ip, node.rpc_port, node.rpc_username, node.rpc_password)
-        if node.get_id() == snode.get_id():
-            cluster_map_data = distr_controller.get_distr_cluster_map(snodes, node)
-            cluster_map_data['UUID_node_target'] = node.get_id()
-            ret = rpc_client.distr_send_cluster_map(cluster_map_data)
-        else:
-            cluster_map_data = distr_controller.get_distr_cluster_map([snode], node)
-            cl_map = {
-                "map_cluster": cluster_map_data['map_cluster'],
-                "map_prob": cluster_map_data['map_prob']}
-            ret = rpc_client.distr_add_nodes(cl_map)
-        time.sleep(3)
+    ret = distr_controller.send_cluster_map_to_node(snode)
+    if not ret:
+        return False, "Failed to send cluster map"
+    ret = distr_controller.send_cluster_map_add_node(snode)
+    if not ret:
+        return False, "Failed to send cluster map add node"
+    time.sleep(3)
 
     logger.info("Sending cluster event updates")
     distr_controller.send_node_status_event(snode.get_id(), "online")
 
     for dev in snode.nvme_devices:
         distr_controller.send_dev_status_event(dev.cluster_device_order, "online")
 
@@ -766,16 +821,19 @@
         else:
             logger.error("Snapshots found on the storage node, use --force-remove or --force-migrate")
             return False
 
     if snode.nvme_devices:
         for dev in snode.nvme_devices:
             if dev.status == 'online':
-                distr_controller.send_dev_status_event(dev.cluster_device_order, "unavailable")
-            distr_controller.disconnect_device(dev)
+                distr_controller.disconnect_device(dev)
+            old_status = dev.status
+            dev.status = NVMeDevice.STATUS_FAILED
+            distr_controller.send_dev_status_event(dev.cluster_device_order, NVMeDevice.STATUS_FAILED)
+            device_events.device_status_change(dev, NVMeDevice.STATUS_FAILED, old_status)
 
     for lvol in db_controller.get_lvols():
         lvol_controller.send_cluster_map(lvol.get_id())
 
     logger.info("Removing storage node")
 
     logger.debug("Leaving swarm...")
@@ -789,15 +847,18 @@
     try:
         snode_api = SNodeClient(snode.api_endpoint)
         snode_api.spdk_process_kill()
         snode_api.leave_swarm()
     except Exception as e:
         logger.warning(f"Failed to remove SPDK process: {e}")
 
-    snode.remove(db_controller.kv_store)
+    snode.status = StorageNode.STATUS_REMOVED
+    snode.write_to_db(db_controller.kv_store)
+    logger.info("Sending node event update")
+    distr_controller.send_node_status_event(snode.get_id(), snode.status)
     storage_events.snode_remove(snode)
     logger.info("done")
 
 
 def restart_storage_node(
         node_id,
         spdk_cpu_mask=None,
@@ -818,20 +879,24 @@
         return False
 
     if snode.status == StorageNode.STATUS_ONLINE:
         logger.error(f"Can not restart online node: {node_id}")
         return False
 
     logger.info("Setting node state to restarting")
+    old_status = snode.status
     snode.status = StorageNode.STATUS_RESTARTING
     snode.write_to_db(kv_store)
+    logger.info("Sending node event update")
+    distr_controller.send_node_status_event(snode.get_id(), snode.status)
+    storage_events.snode_status_change(snode, snode.status, old_status)
 
     logger.info(f"Restarting Storage node: {snode.mgmt_ip}")
-    snode_api = SNodeClient(snode.api_endpoint)
 
+    snode_api = SNodeClient(snode.api_endpoint)
     node_info, _ = snode_api.info()
     logger.info(f"Node info: {node_info}")
 
     logger.info("Restarting SPDK")
     cpu = snode.spdk_cpu_mask
     if spdk_cpu_mask:
         cpu = spdk_cpu_mask
@@ -899,16 +964,14 @@
     known_devices_sn = []
     devices_sn = [d.serial_number for d in nvme_devs]
     for db_dev in snode.nvme_devices:
         known_devices_sn.append(db_dev.serial_number)
         if db_dev.serial_number in devices_sn:
             logger.info(f"Device found: {db_dev.get_id()}")
             active_devices.append(db_dev)
-            if db_dev.status == NVMeDevice.STATUS_UNAVAILABLE:
-                db_dev.status = NVMeDevice.STATUS_ONLINE
         else:
             logger.info(f"Device not found: {db_dev.get_id()}")
             db_dev.status = NVMeDevice.STATUS_REMOVED
             distr_controller.send_dev_status_event(db_dev.cluster_device_order, "offline")
 
     for dev in nvme_devs:
         if dev.serial_number not in known_devices_sn:
@@ -961,41 +1024,28 @@
             else:
                 node.remote_devices.append(dev)
             count += 1
         node.write_to_db(kv_store)
         logger.info(f"connected to devices count: {count}")
 
     logger.info("Sending cluster map")
-    snodes = db_controller.get_storage_nodes()
-    for node in snodes:
-        if node.status != node.STATUS_ONLINE:
-            continue
-        logger.info(f"Sending to: {node.get_id()}")
-        rpc_client = RPCClient(node.mgmt_ip, node.rpc_port, node.rpc_username, node.rpc_password)
-        if node.get_id() == snode.get_id():
-            cluster_map_data = distr_controller.get_distr_cluster_map(snodes, node)
-            cluster_map_data['UUID_node_target'] = node.get_id()
-            ret = rpc_client.distr_send_cluster_map(cluster_map_data)
-        else:
-            cluster_map_data = distr_controller.get_distr_cluster_map([snode], node)
-            cl_map = {
-                "map_cluster": cluster_map_data['map_cluster'],
-                "map_prob": cluster_map_data['map_prob']}
-            ret = rpc_client.distr_add_nodes(cl_map)
-        time.sleep(3)
+    ret = distr_controller.send_cluster_map_to_node(snode)
+    if not ret:
+        return False, "Failed to send cluster map"
+    time.sleep(3)
 
     logger.info("Sending node event update")
     distr_controller.send_node_status_event(snode.get_id(), "online")
 
     logger.info("Sending devices event updates")
     for dev in snode.nvme_devices:
-        if dev.status != "online":
+        if dev.status != NVMeDevice.STATUS_ONLINE:
             logger.debug(f"Device is not online: {dev.get_id()}, status: {dev.status}")
             continue
-        distr_controller.send_dev_status_event(dev.cluster_device_order, "online")
+        distr_controller.send_dev_status_event(dev.cluster_device_order, NVMeDevice.STATUS_ONLINE)
 
     for lvol_id in snode.lvols:
         lvol = lvol_controller.recreate_lvol(lvol_id, snode)
         if not lvol:
             logger.error(f"Failed to create LVol: {lvol_id}")
             return False
         lvol.status = lvol.STATUS_ONLINE
@@ -1027,21 +1077,25 @@
             if dev.status == NVMeDevice.STATUS_ONLINE:
                 online_devices += 1
         data.append({
             "UUID": node.uuid,
             "Hostname": node.hostname,
             "Management IP": node.mgmt_ip,
             "Devices": f"{total_devices}/{online_devices}",
-            "LVOLs": f"{len(node.lvols)}",
-            "Data NICs": "\n".join([d.if_name for d in node.data_nics]),
+            "LVols": f"{len(node.lvols)}",
+            # "Data NICs": "\n".join([d.if_name for d in node.data_nics]),
             "Status": node.status,
             "Health": node.health_check,
 
-            "Updated At": datetime.datetime.strptime(node.updated_at, "%Y-%m-%d %H:%M:%S.%f").strftime(
-                "%H:%M:%S, %d/%m/%Y"),
+            "EC2 ID": node.ec2_instance_id,
+            "EC2 Type": node.ec2_metadata['instanceType'] if node.ec2_metadata else "",
+            "EC2 Ext IP": node.ec2_public_ip,
+
+            # "Updated At": datetime.datetime.strptime(node.updated_at, "%Y-%m-%d %H:%M:%S.%f").strftime(
+            #     "%H:%M:%S, %d/%m/%Y"),
         })
 
     if not data:
         return output
 
     if is_json:
         output = json.dumps(data, indent=2)
```

## Comparing `sbcli_jm-3.0.0/simplyblock_core/cnode_client.py` & `sbcli_jm-4.0.0/simplyblock_core/cnode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/compute_node_ops.py` & `sbcli_jm-4.0.0/simplyblock_core/compute_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/cluster_ops.py` & `sbcli_jm-4.0.0/simplyblock_core/cluster_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/mgmt_node_ops.py` & `sbcli_jm-4.0.0/simplyblock_core/mgmt_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/utils.py` & `sbcli_jm-4.0.0/simplyblock_core/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/kv_store.py` & `sbcli_jm-4.0.0/simplyblock_core/kv_store.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/snode_client.py` & `sbcli_jm-4.0.0/simplyblock_core/snode_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,7 +91,13 @@
         return self._request("POST", "join_swarm", params)
 
     def spdk_process_kill(self):
         return self._request("GET", "spdk_process_kill")
 
     def leave_swarm(self):
         return self._request("GET", "leave_swarm")
+
+    def make_gpt_partitions(self, nbd_device, jm_percent):
+        params = {
+            "nbd_device": nbd_device,
+            "jm_percent": jm_percent}
+        return self._request("POST", "make_gpt_partitions", params)
```

## Comparing `sbcli_jm-3.0.0/simplyblock_core/scripts/stack_deploy_wait.sh` & `sbcli_jm-4.0.0/simplyblock_core/scripts/stack_deploy_wait.sh`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/scripts/install_deps.sh` & `sbcli_jm-4.0.0/simplyblock_core/scripts/install_deps.sh`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 sudo sed -i 's/#X11Forwarding no/X11Forwarding yes/g' /etc/ssh/sshd_config
 sudo sed -i 's/#X11DisplayOffset 10/X11DisplayOffset 10/g' /etc/ssh/sshd_config
 sudo sed -i 's/#X11UseLocalhost yes/X11UseLocalhost no/g' /etc/ssh/sshd_config
 
 sudo service sshd restart
 sudo modprobe nvme-tcp
+sudo modprobe nbd
 
 sudo sysctl -w net.ipv6.conf.all.disable_ipv6=1
 
 # required for graylog
 sudo sysctl -w vm.max_map_count=262144
 
 sudo mkdir -p /etc/simplyblock
```

## Comparing `sbcli_jm-3.0.0/simplyblock_core/scripts/__init__.py` & `sbcli_jm-4.0.0/simplyblock_core/scripts/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/scripts/haproxy.cfg` & `sbcli_jm-4.0.0/simplyblock_core/scripts/haproxy.cfg`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/scripts/apply_dashboard.sh` & `sbcli_jm-4.0.0/simplyblock_core/scripts/apply_dashboard.sh`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/scripts/docker-compose-swarm.yml` & `sbcli_jm-4.0.0/simplyblock_core/scripts/docker-compose-swarm.yml`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/scripts/deploy_stack.sh` & `sbcli_jm-4.0.0/simplyblock_core/scripts/deploy_stack.sh`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/scripts/alerting/alert_rules.yaml` & `sbcli_jm-4.0.0/simplyblock_core/scripts/alerting/alert_rules.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/scripts/alerting/alert_resources.yaml` & `sbcli_jm-4.0.0/simplyblock_core/scripts/alerting/alert_resources.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/scripts/dashboards/devices.json` & `sbcli_jm-4.0.0/simplyblock_core/scripts/dashboards/devices.json`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/scripts/dashboards/lvols.json` & `sbcli_jm-4.0.0/simplyblock_core/scripts/dashboards/lvols.json`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/scripts/dashboards/cluster.json` & `sbcli_jm-4.0.0/simplyblock_core/scripts/dashboards/cluster.json`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/scripts/dashboards/nodes.json` & `sbcli_jm-4.0.0/simplyblock_core/scripts/dashboards/nodes.json`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/controllers/caching_node_controller.py` & `sbcli_jm-4.0.0/simplyblock_core/controllers/caching_node_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,14 @@
                     'partitions_count': device_partitions_count,
                     'capacity': size,
                     'size': size,
                     'pcie_address': nvme_driver_data['pci_address'],
                     'model_id': model_number,
                     'serial_number': nvme_driver_data['ctrlr_data']['serial_number'],
                     'nvme_bdev': nvme_bdev,
-                    'alloc_bdev': nvme_bdev,
                     'node_id': snode.get_id(),
                     'cluster_id': snode.cluster_id,
                     'status': 'online'
                 }))
             sequential_number += device_partitions_count
     return devices
```

## Comparing `sbcli_jm-3.0.0/simplyblock_core/controllers/device_controller.py` & `sbcli_jm-4.0.0/simplyblock_core/controllers/device_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,20 +148,14 @@
             # logger.info("adding listener for %s on IP %s" % (subsystem_nqn, iface.ip4_address))
             ret = rpc_client.listeners_create(subsystem_nqn, tr_type, iface.ip4_address, "4420")
             IP = iface.ip4_address
             break
     logger.info(f"Adding {pt_name} to the subsystem")
     ret = rpc_client.nvmf_subsystem_add_ns(subsystem_nqn, pt_name)
 
-    if device_obj.jm_bdev:
-        ret = rpc_client.bdev_jm_create(device_obj.jm_bdev, device_obj.alceml_bdev)
-        if not ret:
-            logger.error(f"Failed to create bdev: {device_obj.jm_bdev}")
-            return False
-
     device_obj.testing_bdev = test_name
     device_obj.alceml_bdev = alceml_name
     device_obj.pt_bdev = pt_name
     device_obj.nvmf_nqn = subsystem_nqn
     device_obj.nvmf_ip = IP
     device_obj.nvmf_port = 4420
     device_obj.io_error = False
@@ -241,21 +235,14 @@
         return False
 
     for dev in snode.nvme_devices:
         if dev.get_id() == device_id:
             device = dev
             break
 
-    if device.jm_bdev:
-        if snode.lvols:
-            logger.error(f"Failed to remove device: {device.get_id()}, "
-                         f"there are LVols that uses JM from this device, delete LVol to continue")
-            # if not force:
-            return False
-
     logger.info("Sending device event")
     distr_controller.send_dev_status_event(device.cluster_device_order, "removed")
 
     logger.info("Disconnecting device from all nodes")
     distr_controller.disconnect_device(device)
 
     logger.info("Removing device fabric")
@@ -265,21 +252,14 @@
 
     ret = rpc_client.subsystem_delete(device.nvmf_nqn)
     if not ret:
         logger.error(f"Failed to remove subsystem: {device.nvmf_nqn}")
         if not force:
             return False
 
-    if device.jm_bdev:
-        ret = rpc_client.bdev_jm_delete(f"jm_{snode.get_id()}")
-        if not ret:
-            logger.error(f"Failed to remove journal manager: jm_{snode.get_id()}")
-            if not force:
-                return False
-
     logger.info("Removing device bdevs")
     ret = rpc_client.bdev_PT_NoExcl_delete(f"{device.alceml_bdev}_PT")
     if not ret:
         logger.error(f"Failed to remove bdev: {device.alceml_bdev}_PT")
         if not force:
             return False
     ret = rpc_client.bdev_alceml_delete(device.alceml_bdev)
```

## Comparing `sbcli_jm-3.0.0/simplyblock_core/controllers/cluster_events.py` & `sbcli_jm-4.0.0/simplyblock_core/controllers/cluster_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/controllers/lvol_events.py` & `sbcli_jm-4.0.0/simplyblock_core/controllers/lvol_events.py`

 * *Files 15% similar despite different names*

```diff
@@ -35,7 +35,11 @@
 def lvol_migrate(lvol, old_node, new_node, caused_by=ec.CAUSED_BY_CLI):
     _lvol_event(lvol, f"LVol migrated from: {old_node}, \nto {new_node}", caused_by, ec.EVENT_STATUS_CHANGE)
 
 
 def lvol_health_check_change(lvol, new_state, old_status, caused_by=ec.CAUSED_BY_CLI):
     _lvol_event(lvol, f"LVol health check changed from: {old_status} to: {new_state}", caused_by, ec.EVENT_STATUS_CHANGE)
 
+
+def lvol_io_error_change(lvol, new_state, old_status, caused_by=ec.CAUSED_BY_CLI):
+    _lvol_event(lvol, f"LVol IO Error changed from: {old_status} to: {new_state}", caused_by, ec.EVENT_STATUS_CHANGE)
+
```

## Comparing `sbcli_jm-3.0.0/simplyblock_core/controllers/pool_events.py` & `sbcli_jm-4.0.0/simplyblock_core/controllers/pool_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/controllers/snapshot_controller.py` & `sbcli_jm-4.0.0/simplyblock_core/controllers/snapshot_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,18 +50,17 @@
         base_name, new_vuid, lvol.ndcs, lvol.npcs, num_blocks,
         lvol.distr_bs, lvol_controller.get_jm_names(snode), lvol.distr_chunk_bs,
         None, None, lvol.distr_page_size)
     if not ret:
         logger.error("Failed to create Distr bdev")
         return False, "Failed to create Distr bdev"
 
-    snodes = db_controller.get_storage_nodes()
-    cluster_map_data = distr_controller.get_distr_cluster_map(snodes, snode)
-    cluster_map_data['UUID_node_target'] = snode.get_id()
-    rpc_client.distr_send_cluster_map(cluster_map_data)
+    ret = distr_controller.send_cluster_map_to_node(snode)
+    if not ret:
+        return False, "Failed to send cluster map"
 
     ret = rpc_client.ultra21_lvol_bmap_init(
         base_name, num_blocks, lvol.distr_bs, int(lvol.distr_page_size / lvol.distr_bs), num_blocks * 10)
     if not ret:
         return False, "Failed to init distr bdev"
 
     logger.info("Creating Snapshot bdev")
@@ -229,18 +228,17 @@
         logger.error("Failed to create Distr bdev")
         return False, "Failed to create Distr bdev"
     if ret == "?":
         logger.error(f"Failed to create Distr bdev, ret={ret}")
         # return False
 
     logger.info("Sending cluster map to the lvol")
-    snodes = db_controller.get_storage_nodes()
-    cluster_map_data = distr_controller.get_distr_cluster_map(snodes, snode)
-    cluster_map_data['UUID_node_target'] = snode.get_id()
-    ret = rpc_client.distr_send_cluster_map(cluster_map_data)
+    ret = distr_controller.send_cluster_map_to_node(snode)
+    if not ret:
+        return False, "Failed to send cluster map"
 
     logger.info("Creating clone bdev")
     block_len = lvol.distr_bs
     page_len = int(lvol.distr_page_size / lvol.distr_bs)
     max_num_blocks = num_blocks * 10
     ret = rpc_client.ultra21_lvol_bmap_init(name, num_blocks, block_len, page_len, max_num_blocks)
     if not ret:
```

## Comparing `sbcli_jm-3.0.0/simplyblock_core/controllers/snapshot_events.py` & `sbcli_jm-4.0.0/simplyblock_core/controllers/snapshot_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/controllers/storage_events.py` & `sbcli_jm-4.0.0/simplyblock_core/controllers/storage_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/controllers/mgmt_events.py` & `sbcli_jm-4.0.0/simplyblock_core/controllers/mgmt_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/controllers/events_controller.py` & `sbcli_jm-4.0.0/simplyblock_core/controllers/events_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/controllers/lvol_controller.py` & `sbcli_jm-4.0.0/simplyblock_core/controllers/lvol_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,21 +26,20 @@
     def _generate_string(length):
         return ''.join(random.SystemRandom().choice(
             string.ascii_letters + string.digits) for _ in range(length))
 
     return _generate_string(length).encode('utf-8').hex()
 
 
-def _create_crypto_lvol(rpc_client, name, base_name):
+def _create_crypto_lvol(rpc_client, name, base_name, key1, key2):
     key_name = f'key_{name}'
-    key1 = _generate_hex_string(32)
-    key2 = _generate_hex_string(32)
     ret = rpc_client.lvol_crypto_key_create(key_name, key1, key2)
     if not ret:
-        logger.warning("failed to create crypto key")
+        logger.error("failed to create crypto key")
+        return False
     ret = rpc_client.lvol_crypto_create(name, base_name, key_name)
     if not ret:
         logger.error(f"failed to create crypto LVol {name}")
         return False
     return ret
 
 
@@ -290,15 +289,15 @@
 
     lvol_type = 'lvol'
     lvol_bdev = f"LVS_{vuid}/{name}"
     crypto_bdev = ''
     comp_bdev = ''
     top_bdev = lvol_bdev
     if use_crypto is True:
-        crypto_bdev = _create_crypto_lvol(rpc_client, name, lvol_bdev)
+        crypto_bdev = _create_crypto_lvol(rpc_client, name, lvol_bdev, "", "")
         bdev_stack.append({"type": "crypto", "name": crypto_bdev})
         if not crypto_bdev:
             return False, "Error creating crypto bdev"
         lvol_type += ',crypto'
         top_bdev = crypto_bdev
 
     if use_comp is True:
@@ -428,19 +427,48 @@
             node = db_controller.get_storage_node_by_id(node_id)
             print(f"Selected node: {node_id}, {node.hostname}")
             ret.append(node)
         return ret
     else:
         return online_nodes
 
+def is_hex(s: str) -> bool:
+    """
+    given an input checks if the value is hex encoded or not
+    """
+    try:
+        int(s, 16)
+        return True
+    except ValueError:
+        return False
+
+def validate_aes_xts_keys(key1: str, key2: str) -> tuple[bool, str]:
+    """
+    Key Length: each key should be either 128 or 256 bits long.
+    since hex values of the keys are expected, the key lengths should be either 32 or 64
+    """
+
+    if len(key1) != len(key2):
+        return False, "both the keys should be of the same length"
+
+    if len(key1) not in [32, 64] or len(key2) not in [32, 64]:
+        return False, "each key should be either 16 or 32 bytes long"
+
+    if not is_hex(key1):
+        return False, "please provide hex encoded value for crypto_key1"
+
+    if not is_hex(key2):
+        return False, "please provide hex encoded value for crypto_key2"
+
+    return True, ""
 
 def add_lvol_ha(name, size, host_id_or_name, ha_type, pool_id_or_name, use_comp, use_crypto,
                 distr_vuid, distr_ndcs, distr_npcs,
                 max_rw_iops, max_rw_mbytes, max_r_mbytes, max_w_mbytes,
-                distr_bs=None, distr_chunk_bs=None, with_snapshot=False, max_size=0):
+                distr_bs=None, distr_chunk_bs=None, with_snapshot=False, max_size=0, crypto_key1=None, crypto_key2=None):
 
     logger.info(f"Adding LVol: {name}")
     host_node = None
     if host_id_or_name:
         host_node = db_controller.get_storage_node_by_id(host_id_or_name)
         if not host_node:
             host_node = db_controller.get_storage_node_by_hostname(host_id_or_name)
@@ -524,15 +552,14 @@
         vuid = distr_vuid
 
     if distr_ndcs == 0 and distr_npcs == 0:
         if ha_type == "single":
             distr_ndcs = 4
             distr_npcs = 1
         else:
-
             if dev_count == 3:
                 distr_ndcs = 1
             elif dev_count in [4, 5]:
                 distr_ndcs = 2
             elif dev_count >= 6:
                 distr_ndcs = 4
             distr_npcs = 1
@@ -616,22 +643,31 @@
                 "lvol_name": lvol.top_bdev,
                 "base_bdev": lvol.base_bdev,
                 "label": "label",
                 "desc": "desc"
             }
         })
 
-    if use_crypto is True:
+    if use_crypto:
+        if crypto_key1 == None or crypto_key2 == None:
+            return False, "encryption keys for lvol not provided"
+        else:
+            success, err = validate_aes_xts_keys(crypto_key1, crypto_key2)
+            if not success:
+                return False, err
+
         lvol.crypto_bdev = f"crypto_{lvol.lvol_name}"
         lvol.bdev_stack.append({
             "type": "crypto",
             "name": lvol.crypto_bdev,
             "params": {
                 "name": lvol.crypto_bdev,
-                "base_name": lvol.lvol_bdev
+                "base_name": lvol.base_bdev,
+                "key1": crypto_key1,
+                "key2": crypto_key2,
             }
         })
         lvol.lvol_type += ',crypto'
         lvol.top_bdev = lvol.crypto_bdev
 
     if use_comp is True:
         base_bdev = lvol.lvol_bdev
@@ -709,19 +745,18 @@
         ret = None
 
         if type == "bdev_distr":
             params['jm_names'] = get_jm_names(snode)
             params['ha_comm_addrs'] = ha_comm_addrs
             params['ha_inode_self'] = ha_inode_self
             ret = rpc_client.bdev_distrib_create(**params)
-
-            snodes = db_controller.get_storage_nodes()
-            cluster_map_data = distr_controller.get_distr_cluster_map(snodes, snode)
-            cluster_map_data['UUID_node_target'] = snode.get_id()
-            rpc_client.distr_send_cluster_map(cluster_map_data)
+            if ret:
+                ret = distr_controller.send_cluster_map_to_node(snode)
+                if not ret:
+                    return False, "Failed to send cluster map"
 
         elif type == "bmap_init":
             ret = rpc_client.ultra21_lvol_bmap_init(**params)
 
         elif type == "ultra_lvol":
             ret = rpc_client.ultra21_lvol_mount_lvol(**params)
 
@@ -783,18 +818,17 @@
 
     logger.info("Add BDev to subsystem")
     ret = rpc_client.nvmf_subsystem_add_ns(lvol.nqn, lvol.top_bdev, lvol.uuid, lvol.guid)
     if not ret:
         return False, "Failed to add bdev to subsystem"
 
     logger.info("Sending cluster map to LVol")
-    snodes = db_controller.get_storage_nodes()
-    cluster_map_data = distr_controller.get_distr_cluster_map(snodes, snode)
-    cluster_map_data['UUID_node_target'] = snode.get_id()
-    ret = rpc_client.distr_send_cluster_map(cluster_map_data)
+    ret = distr_controller.send_cluster_map_to_node(snode)
+    if not ret:
+        return False, "Failed to send cluster map"
 
     spdk_mem_info_after = rpc_client.ultra21_util_get_malloc_stats()
     logger.debug("ultra21_util_get_malloc_stats:")
     logger.debug(spdk_mem_info_after)
 
     diff = {}
     for key in spdk_mem_info_after.keys():
@@ -1271,21 +1305,15 @@
     lvol = db_controller.get_lvol_by_id(lvol_id)
     if not lvol:
         logger.error(f"LVol not found: {lvol_id}")
         return False
 
     snode = db_controller.get_storage_node_by_id(lvol.node_id)
     logger.info("Sending cluster map")
-    snodes = db_controller.get_storage_nodes()
-    logger.info(f"Sending to: {snode.get_id()}")
-    rpc_client = RPCClient(snode.mgmt_ip, snode.rpc_port, snode.rpc_username, snode.rpc_password)
-    cluster_map_data = distr_controller.get_distr_cluster_map(snodes, snode)
-    cluster_map_data['UUID_node_target'] = snode.get_id()
-    ret = rpc_client.distr_send_cluster_map(cluster_map_data)
-    return ret
+    return distr_controller.send_cluster_map_to_node(snode)
 
 
 def get_cluster_map(lvol_id):
     lvol = db_controller.get_lvol_by_id(lvol_id)
     if not lvol:
         logger.error(f"LVol not found: {lvol_id}")
         return False
```

## Comparing `sbcli_jm-3.0.0/simplyblock_core/controllers/pool_controller.py` & `sbcli_jm-4.0.0/simplyblock_core/controllers/pool_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/controllers/device_events.py` & `sbcli_jm-4.0.0/simplyblock_core/controllers/device_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/controllers/health_controller.py` & `sbcli_jm-4.0.0/simplyblock_core/controllers/health_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         logger.error("node not found")
         return False
 
     if snode.status in [StorageNode.STATUS_OFFLINE, StorageNode.STATUS_REMOVED]:
         logger.info(f"Skipping ,node status is {snode.status}")
         return True
 
-    if device.status in [NVMeDevice.STATUS_REMOVED, NVMeDevice.STATUS_UNRECOGNIZED]:
+    if device.status in [NVMeDevice.STATUS_REMOVED, NVMeDevice.STATUS_FAILED]:
         logger.info(f"Skipping ,device status is {device.status}")
         return True
 
     passed = True
     try:
         rpc_client = RPCClient(
             snode.mgmt_ip, snode.rpc_port,
```

## Comparing `sbcli_jm-3.0.0/simplyblock_core/services/mgmt_node_monitor.py` & `sbcli_jm-4.0.0/simplyblock_core/services/mgmt_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/services/log_agg_service.py` & `sbcli_jm-4.0.0/simplyblock_core/services/log_agg_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/services/capacity_collector.py` & `sbcli_jm-4.0.0/simplyblock_core/services/capacity_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/services/port_stat_collector.py` & `sbcli_jm-4.0.0/simplyblock_core/services/port_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/services/__init__.py` & `sbcli_jm-4.0.0/simplyblock_core/services/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/services/install_service.sh` & `sbcli_jm-4.0.0/simplyblock_core/services/install_service.sh`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/services/lvol_stat_collector.py` & `sbcli_jm-4.0.0/simplyblock_core/services/lvol_stat_collector.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 
 import time
 import sys
 
 
 from simplyblock_core import constants, kv_store, utils
+from simplyblock_core.controllers import lvol_events
 from simplyblock_core.models.stats import LVolStatObject, PoolStatObject
 from simplyblock_core.rpc_client import RPCClient
 
 # Import the GELF logger
 from graypy import GELFUDPHandler
 
 last_object_record = {}
@@ -55,14 +56,21 @@
                 data['write_io_ps'] = int((data['write_io'] - last_record['write_io']) / time_diff)
                 data['write_latency_ps'] = int((data['write_latency_ticks'] - last_record['write_latency_ticks']) / time_diff)
 
                 data['unmap_bytes_ps'] = int((data['unmap_bytes'] - last_record['unmap_bytes']) / time_diff)
                 data['unmap_io_ps'] = int((data['unmap_io'] - last_record['unmap_io']) / time_diff)
                 data['unmap_latency_ps'] = int((data['unmap_latency_ticks'] - last_record['unmap_latency_ticks']) / time_diff)
 
+                if data['read_io_ps'] > 0 and data['write_io_ps'] > 0 and lvol.io_error:
+                    # set lvol io error to false
+                    lvol = db_controller.get_lvol_by_id(lvol.get_id())
+                    lvol.io_error = False
+                    lvol.write_to_db(db_store)
+                    lvol_events.lvol_io_error_change(lvol, False, True, caused_by="monitor")
+
         else:
             logger.warning("last record not found")
     else:
         logger.error("Error getting stats")
 
     stat_obj = LVolStatObject(data=data)
     stat_obj.write_to_db(db_controller.kv_store)
```

## Comparing `sbcli_jm-3.0.0/simplyblock_core/services/device_monitor.py` & `sbcli_jm-4.0.0/simplyblock_core/services/device_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/services/storage_node_monitor.py` & `sbcli_jm-4.0.0/simplyblock_core/services/storage_node_monitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 import time
 import sys
 from datetime import datetime
 
 
-from simplyblock_core import constants, kv_store, cluster_ops, storage_node_ops
+from simplyblock_core import constants, kv_store, cluster_ops, storage_node_ops, distr_controller
 from simplyblock_core.controllers import storage_events, health_controller
 from simplyblock_core.models.cluster import Cluster
 from simplyblock_core.models.nvme_device import NVMeDevice
 from simplyblock_core.models.storage_node import StorageNode
 
 # Import the GELF logger
 from graypy import GELFUDPHandler
@@ -112,14 +112,15 @@
         #         distr_controller.send_dev_status_event(dev.cluster_device_order, "online")
 
         old_status = snode.status
         snode.status = StorageNode.STATUS_ONLINE
         snode.updated_at = str(datetime.now())
         snode.write_to_db(db_store)
         storage_events.snode_status_change(snode, snode.status, old_status, caused_by="monitor")
+        distr_controller.send_node_status_event(snode.get_id(), StorageNode.STATUS_ONLINE)
 
         logger.info("Connecting to remote devices")
         storage_node_ops._connect_to_remote_devs(snode)
 
 
 def set_node_offline(node):
     if node.status == StorageNode.STATUS_ONLINE:
@@ -130,14 +131,15 @@
         #         distr_controller.send_dev_status_event(dev.cluster_device_order, "unavailable")
 
         old_status = snode.status
         snode.status = StorageNode.STATUS_UNREACHABLE
         snode.updated_at = str(datetime.now())
         snode.write_to_db(db_store)
         storage_events.snode_status_change(snode, snode.status, old_status, caused_by="monitor")
+        distr_controller.send_node_status_event(snode.get_id(), StorageNode.STATUS_UNREACHABLE)
 
 
 logger.info("Starting node monitor")
 
 while True:
     # get storage nodes
     nodes = db_controller.get_storage_nodes()
```

## Comparing `sbcli_jm-3.0.0/simplyblock_core/services/lvol_monitor.py` & `sbcli_jm-4.0.0/simplyblock_core/services/lvol_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/services/distr_event_collector.py` & `sbcli_jm-4.0.0/simplyblock_core/services/distr_event_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,20 +57,20 @@
             return
 
         if event.message == 'SPDK_BDEV_EVENT_REMOVE':
             logger.info(f"Removing storage id: {storage_id} from node: {node_id}")
             device_controller.device_remove(device_id)
         elif event.message == 'error_write':
             logger.info(f"Setting device to read-only")
-            device_controller.device_set_read_only(device_id)
             device_controller.device_set_io_error(device_id, True)
+            device_controller.device_set_read_only(device_id)
         else:
             logger.info(f"Setting device to unavailable")
-            device_controller.device_set_unavailable(device_id)
             device_controller.device_set_io_error(device_id, True)
+            device_controller.device_set_unavailable(device_id)
 
         event.status = 'processed'
 
 
 def process_lvol_event(event):
     if event.message in ["error_open", 'error_read', "error_write", "error_unmap"]:
         vuid = event.object_dict['vuid']
@@ -87,15 +87,18 @@
             lvol.io_error = True
             if lvol.status == LVol.STATUS_ONLINE:
                 logger.info("Setting LVol to offline")
                 old_status = lvol.status
                 lvol.status = LVol.STATUS_OFFLINE
                 lvol.write_to_db(db_controller.kv_store)
                 lvol_events.lvol_status_change(lvol, lvol.status, old_status, caused_by="monitor")
-            event.status = 'processed'
+                lvol_events.lvol_io_error_change(lvol, True, False, caused_by="monitor")
+                event.status = 'processed'
+            else:
+                event.status = 'skipped'
     else:
         logger.error(f"Unknown LVol event message: {event.message}")
         event.status = "event_unknown"
 
 
 def process_event(event_id):
     event = db_controller.get_events(event_id)[0]
```

## Comparing `sbcli_jm-3.0.0/simplyblock_core/services/health_check_service.py` & `sbcli_jm-4.0.0/simplyblock_core/services/health_check_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/services/caching_node_monitor.py` & `sbcli_jm-4.0.0/simplyblock_core/services/caching_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/services/cap_monitor.py` & `sbcli_jm-4.0.0/simplyblock_core/services/cap_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/services/capacity_and_stats_collector.py` & `sbcli_jm-4.0.0/simplyblock_core/services/capacity_and_stats_collector.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # coding=utf-8
 import logging
 
 import time
 import sys
 
 from simplyblock_core import constants, kv_store, utils
+from simplyblock_core.models.nvme_device import NVMeDevice
 from simplyblock_core.rpc_client import RPCClient
 from simplyblock_core.models.stats import DeviceStatObject, NodeStatObject, ClusterStatObject
 
 # Import the GELF logger
 from graypy import GELFUDPHandler
 
 last_object_record = {}
@@ -83,42 +84,43 @@
     stat_obj = DeviceStatObject(data=data)
     stat_obj.write_to_db(db_controller.kv_store)
     last_object_record[device.get_id()] = stat_obj
     return stat_obj
 
 
 def add_node_stats(node, records):
-    if not records:
-        return False
-    records_sum = utils.sum_records(records)
-
-    size_total = records_sum.size_total
-    size_used = records_sum.size_used
+    size_used = 0
+    size_total = 0
+    data = {}
+    if records:
+        records_sum = utils.sum_records(records)
+        size_total = records_sum.size_total
+        size_used = records_sum.size_used
+        data.update(records_sum.get_clean_dict())
 
     size_prov = 0
     for lvol_id in node.lvols:
         lvol = db_controller.get_lvol_by_id(lvol_id)
         if lvol:
             size_prov += lvol.size
+
     size_util = 0
     size_prov_util = 0
     if size_total > 0:
         size_util = int((size_used / size_total) * 100)
         size_prov_util = int((size_prov / size_total) * 100)
 
-    data = records_sum.get_clean_dict()
     data.update({
         "cluster_id": cl.get_id(),
         "uuid": node.get_id(),
         "date": int(time.time()),
-
         "size_util": size_util,
         "size_prov": size_prov,
-        "size_prov_util": size_prov_util })
-
+        "size_prov_util": size_prov_util
+    })
     stat_obj = NodeStatObject(data=data)
     stat_obj.write_to_db(db_controller.kv_store)
     return stat_obj
 
 
 def add_cluster_stats(cl, records):
 
@@ -183,21 +185,22 @@
                 node.mgmt_ip, node.rpc_port,
                 node.rpc_username, node.rpc_password,
                 timeout=3, retry=2)
 
             devices_records = []
             for device in node.nvme_devices:
                 logger.info("Getting device stats: %s", device.uuid)
-                if device.status != 'online':
-                    logger.info("Device is not online, skipping")
+                if device.status not in [NVMeDevice.STATUS_ONLINE, NVMeDevice.STATUS_READONLY]:
+                    logger.info(f"Device is skipped: {device.get_id()} status: {device.status}")
                     continue
                 capacity_dict = rpc_client.alceml_get_capacity(device.alceml_bdev)
-                stats_dict = rpc_client.get_device_stats(device.alloc_bdev)
+                stats_dict = rpc_client.get_device_stats(device.nvme_bdev)
                 record = add_device_stats(cl, device, capacity_dict, stats_dict)
-                devices_records.append(record)
+                if record:
+                    devices_records.append(record)
 
             node_record = add_node_stats(node, devices_records)
             node_records.append(node_record)
 
         add_cluster_stats(cl, node_records)
 
     time.sleep(constants.DEV_STAT_COLLECTOR_INTERVAL_SEC)
```

## Comparing `sbcli_jm-3.0.0/simplyblock_core/models/global_settings.py` & `sbcli_jm-4.0.0/simplyblock_core/models/global_settings.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/models/cluster.py` & `sbcli_jm-4.0.0/simplyblock_core/models/cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/models/caching_node.py` & `sbcli_jm-4.0.0/simplyblock_core/models/caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/models/pool.py` & `sbcli_jm-4.0.0/simplyblock_core/models/pool.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/models/events.py` & `sbcli_jm-4.0.0/simplyblock_core/models/events.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/models/iface.py` & `sbcli_jm-4.0.0/simplyblock_core/models/iface.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/models/base_model.py` & `sbcli_jm-4.0.0/simplyblock_core/models/base_model.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/models/stats.py` & `sbcli_jm-4.0.0/simplyblock_core/models/stats.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/models/nvme_device.py` & `sbcli_jm-4.0.0/simplyblock_core/models/nvme_device.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,38 +2,37 @@
 from typing import List
 
 from simplyblock_core.models.base_model import BaseModel
 
 
 class NVMeDevice(BaseModel):
 
+    STATUS_JM = "JM_DEV"
+
     STATUS_ONLINE = 'online'
-    STATUS_AVAILABLE = 'available'
     STATUS_UNAVAILABLE = 'unavailable'
-    STATUS_READONLY = 'read_only'
-    STATUS_OVERLOADED = 'overloaded'
-    STATUS_FAILED = 'failed'
     STATUS_REMOVED = 'removed'
-    STATUS_RESETTING = 'resetting'
-    STATUS_UNRECOGNIZED = 'unrecognized'
+    STATUS_FAILED = 'failed'
+    STATUS_READONLY = 'read_only'
 
     attributes = {
         "uuid": {"type": str, 'default': ""},
         "device_name": {"type": str, 'default': ""},
         "status": {"type": str, 'default': ""},
         "sequential_number": {"type": int, 'default': 0},
         "partitions_count": {"type": int, 'default': 0},
         "capacity": {"type": int, 'default': -1},
         "size": {"type": int, 'default': -1},
         "pcie_address": {"type": str, 'default': ""},
         "model_id": {"type": str, 'default': ""},
         "serial_number": {"type": str, 'default': ""},
         "overload_percentage": {"type": int, 'default': 0},
         "nvme_bdev": {"type": str, 'default': ""},
-        "alloc_bdev": {"type": str, 'default': ""},
+        "nvme_main_bdev": {"type": str, 'default': ""},
+        "nvme_controller": {"type": str, 'default': ""},
         "alceml_bdev": {"type": str, 'default': ""},
         "node_id": {"type": str, 'default': ""},
         "pt_bdev": {"type": str, 'default': ""},
         "nvmf_nqn": {"type": str, 'default': ""},
         "nvmf_ip": {"type": str, 'default': ""},
         "nvmf_port": {"type": int, 'default': 0},
         "remote_bdev": {"type": str, 'default': ""},
```

## Comparing `sbcli_jm-3.0.0/simplyblock_core/models/storage_node.py` & `sbcli_jm-4.0.0/simplyblock_core/models/storage_node.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 
 
 class StorageNode(BaseModel):
 
     STATUS_ONLINE = 'online'
     STATUS_OFFLINE = 'offline'
     STATUS_SUSPENDED = 'suspended'
-    STATUS_IN_CREATION = 'in_creation'
     STATUS_IN_SHUTDOWN = 'in_shutdown'
-    STATUS_RESTARTING = 'restarting'
-    STATUS_UNREACHABLE = 'unreachable'
     STATUS_REMOVED = 'removed'
+    STATUS_RESTARTING = 'in_restart'
+
+    STATUS_IN_CREATION = 'in_restart'  # 'in_creation'
+    STATUS_UNREACHABLE = 'offline'  # 'unreachable'
 
     STATUS_CODE_MAP = {
         STATUS_ONLINE: 0,
         STATUS_OFFLINE: 1,
         STATUS_SUSPENDED: 2,
         STATUS_REMOVED: 3,
 
@@ -68,14 +69,21 @@
         "health_check": {"type": bool, "default": True},
 
         # spdk params
         "spdk_cpu_mask": {"type": str, "default": ""},
         "spdk_mem": {"type": int, "default": 0},
         "spdk_image": {"type": str, "default": ""},
         "spdk_debug": {"type": bool, "default": False},
+
+        "ec2_metadata": {"type": dict, "default": {}},
+        "ec2_instance_id": {"type": str, "default": ""},
+        "ec2_public_ip": {"type": str, "default": ""},
+
+        "jm_bdev": {"type": str, "default": ""},
+
     }
 
     def __init__(self, data=None):
         super(StorageNode, self).__init__()
         self.set_attrs(self.attributes, data)
         self.object_type = "object"
```

## Comparing `sbcli_jm-3.0.0/simplyblock_core/models/port_stat.py` & `sbcli_jm-4.0.0/simplyblock_core/models/port_stat.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/models/mgmt_node.py` & `sbcli_jm-4.0.0/simplyblock_core/models/mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/models/snapshot.py` & `sbcli_jm-4.0.0/simplyblock_core/models/snapshot.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/models/compute_node.py` & `sbcli_jm-4.0.0/simplyblock_core/models/compute_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/simplyblock_core/models/lvol_model.py` & `sbcli_jm-4.0.0/simplyblock_core/models/lvol_model.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/sbcli_jm.egg-info/SOURCES.txt` & `sbcli_jm-4.0.0/sbcli_jm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `sbcli_jm-3.0.0/sbcli_jm.egg-info/PKG-INFO` & `sbcli_jm-4.0.0/sbcli_jm.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-jm
-Version: 3.0.0
+Version: 4.0.0
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
@@ -29,16 +29,16 @@
 # Components 
 
 ## Simply Block Core
 Contains core logic and controllers for the simplyblock cluster
 
 ## Simply Block CLI
 Please see this document 
-[README.md](../simplyblock_cli/README.md)
+[README.md](../main/simplyblock_cli/README.md)
 
 
 ## Simply Block Web API
 Please see this document 
-[README.md](../simplyblock_web/README.md)
+[README.md](../main/simplyblock_web/README.md)
```

