# Comparing `tmp/wtfis-0.8.0.tar.gz` & `tmp/wtfis-0.9.0.tar.gz`

## Comparing `wtfis-0.8.0.tar` & `wtfis-0.9.0.tar`

### file list

```diff
@@ -1,92 +1,100 @@
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 wtfis-0.8.0/.env.wtfis.example
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 wtfis-0.8.0/.flake8
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 wtfis-0.8.0/Dockerfile
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 wtfis-0.8.0/Makefile
--rw-r--r--   0        0        0    80106 2020-02-02 00:00:00.000000 wtfis-0.8.0/imgs/demo-old.gif
--rw-r--r--   0        0        0   132990 2020-02-02 00:00:00.000000 wtfis-0.8.0/imgs/demo.gif
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 wtfis-0.8.0/imgs/example-greynoise.png
--rw-r--r--   0        0        0    93031 2020-02-02 00:00:00.000000 wtfis-0.8.0/imgs/example-ip.png
--rw-r--r--   0        0        0    58474 2020-02-02 00:00:00.000000 wtfis-0.8.0/imgs/example-no-color.png
--rw-r--r--   0        0        0   110694 2020-02-02 00:00:00.000000 wtfis-0.8.0/imgs/example-one-column.png
--rw-r--r--   0        0        0    29089 2020-02-02 00:00:00.000000 wtfis-0.8.0/imgs/example-shodan.png
--rw-r--r--   0        0        0    23045 2020-02-02 00:00:00.000000 wtfis-0.8.0/imgs/example-urlhaus.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/conftest.py
--rw-r--r--   0        0        0    17458 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_cli.py
--rw-r--r--   0        0        0     7346 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_clients.py
--rw-r--r--   0        0        0    23052 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_handlers.py
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_models_vt.py
--rw-r--r--   0        0        0    53110 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_ui_domain_view.py
--rw-r--r--   0        0        0    25453 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_ui_ip_view.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_utils.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_data/greynoise_1.1.1.1.json
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_data/greynoise_1.1.1.1_malicious.json
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_data/greynoise_1.1.1.1_unknown.json
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_data/greynoise_one.json
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_data/ip2whois_whois_bbc.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_data/ip2whois_whois_hotmail.json
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_data/ipwhois_1.1.1.1.json
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_data/ipwhois_gist.json
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_data/ipwhois_raw_10.0.0.1.json
--rw-r--r--   0        0        0     9733 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_data/pt_passive_dns_gist.json
--rw-r--r--   0        0        0    10017 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_data/pt_whois_1.1.1.1.json
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_data/pt_whois_gist.json
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_data/shodan_1.1.1.1.json
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_data/shodan_gist.json
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_data/shodan_gist_2.json
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_data/shodan_one.json
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_data/shodan_wired.json
--rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_data/urlhaus_1.1.1.1.json
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_data/urlhaus_gist.json
--rw-r--r--   0        0        0    18175 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_data/vt_domain_gist.json
--rw-r--r--   0        0        0    20408 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_data/vt_domain_google.json
--rw-r--r--   0        0        0    17624 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_data/vt_domain_tucows.json
--rw-r--r--   0        0        0    17725 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_data/vt_ip_1.1.1.1.json
--rw-r--r--   0        0        0    11171 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_data/vt_ip_142.251.220.110.json
--rw-r--r--   0        0        0     5673 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_data/vt_resolutions_gist.json
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_data/vt_resolutions_one.json
--rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_data/vt_resolutions_wired.json
--rw-r--r--   0        0        0    19472 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_data/vt_whois_1.1.1.1.json
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_data/vt_whois_bbc.json
--rw-r--r--   0        0        0    14040 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_data/vt_whois_example.json
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_data/vt_whois_example_2.json
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_data/vt_whois_foo.json
--rw-r--r--   0        0        0    18644 2020-02-02 00:00:00.000000 wtfis-0.8.0/tests/test_data/vt_whois_gist.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 wtfis-0.8.0/wtfis/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.8.0/wtfis/__init__.py
--rw-r--r--   0        0        0     7512 2020-02-02 00:00:00.000000 wtfis-0.8.0/wtfis/main.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 wtfis-0.8.0/wtfis/types.py
--rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 wtfis-0.8.0/wtfis/utils.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 wtfis-0.8.0/wtfis/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.8.0/wtfis/clients/__init__.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 wtfis-0.8.0/wtfis/clients/base.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 wtfis-0.8.0/wtfis/clients/greynoise.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 wtfis-0.8.0/wtfis/clients/ip2whois.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 wtfis-0.8.0/wtfis/clients/ipwhois.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 wtfis-0.8.0/wtfis/clients/passivetotal.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 wtfis-0.8.0/wtfis/clients/shodan.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 wtfis-0.8.0/wtfis/clients/urlhaus.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 wtfis-0.8.0/wtfis/clients/virustotal.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.8.0/wtfis/handlers/__init__.py
--rw-r--r--   0        0        0     4464 2020-02-02 00:00:00.000000 wtfis-0.8.0/wtfis/handlers/base.py
--rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 wtfis-0.8.0/wtfis/handlers/domain.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 wtfis-0.8.0/wtfis/handlers/ip.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.8.0/wtfis/models/__init__.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 wtfis-0.8.0/wtfis/models/common.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 wtfis-0.8.0/wtfis/models/greynoise.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 wtfis-0.8.0/wtfis/models/ip2whois.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 wtfis-0.8.0/wtfis/models/ipwhois.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 wtfis-0.8.0/wtfis/models/passivetotal.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 wtfis-0.8.0/wtfis/models/shodan.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 wtfis-0.8.0/wtfis/models/urlhaus.py
--rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 wtfis-0.8.0/wtfis/models/virustotal.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.8.0/wtfis/ui/__init__.py
--rw-r--r--   0        0        0    18352 2020-02-02 00:00:00.000000 wtfis-0.8.0/wtfis/ui/base.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 wtfis-0.8.0/wtfis/ui/progress.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 wtfis-0.8.0/wtfis/ui/theme.py
--rw-r--r--   0        0        0     7889 2020-02-02 00:00:00.000000 wtfis-0.8.0/wtfis/ui/view.py
--rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 wtfis-0.8.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 wtfis-0.8.0/LICENSE
--rw-r--r--   0        0        0    10051 2020-02-02 00:00:00.000000 wtfis-0.8.0/README.md
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 wtfis-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    10854 2020-02-02 00:00:00.000000 wtfis-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 wtfis-0.9.0/.env.wtfis.example
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 wtfis-0.9.0/.flake8
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 wtfis-0.9.0/Dockerfile
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 wtfis-0.9.0/Makefile
+-rw-r--r--   0        0        0    80106 2020-02-02 00:00:00.000000 wtfis-0.9.0/imgs/demo-old.gif
+-rw-r--r--   0        0        0   132990 2020-02-02 00:00:00.000000 wtfis-0.9.0/imgs/demo.gif
+-rw-r--r--   0        0        0     5765 2020-02-02 00:00:00.000000 wtfis-0.9.0/imgs/example-abuseipdb.png
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 wtfis-0.9.0/imgs/example-greynoise.png
+-rw-r--r--   0        0        0   100708 2020-02-02 00:00:00.000000 wtfis-0.9.0/imgs/example-ip.png
+-rw-r--r--   0        0        0    58474 2020-02-02 00:00:00.000000 wtfis-0.9.0/imgs/example-no-color.png
+-rw-r--r--   0        0        0   110694 2020-02-02 00:00:00.000000 wtfis-0.9.0/imgs/example-one-column.png
+-rw-r--r--   0        0        0    29089 2020-02-02 00:00:00.000000 wtfis-0.9.0/imgs/example-shodan.png
+-rw-r--r--   0        0        0    23045 2020-02-02 00:00:00.000000 wtfis-0.9.0/imgs/example-urlhaus.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/conftest.py
+-rw-r--r--   0        0        0    19304 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_cli.py
+-rw-r--r--   0        0        0     8351 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_clients.py
+-rw-r--r--   0        0        0    23993 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_handlers.py
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_models_vt.py
+-rw-r--r--   0        0        0    54609 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_ui_domain_view.py
+-rw-r--r--   0        0        0    28862 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_ui_ip_view.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_utils.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/abuseipdb_1.1.1.1_green.json
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/abuseipdb_1.1.1.1_raw.json
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/abuseipdb_1.1.1.1_red.json
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/abuseipdb_1.1.1.1_yellow.json
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/abuseipdb_one.json
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/greynoise_1.1.1.1.json
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/greynoise_1.1.1.1_malicious.json
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/greynoise_1.1.1.1_unknown.json
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/greynoise_one.json
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/ip2whois_whois_bbc.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/ip2whois_whois_hotmail.json
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/ipwhois_1.1.1.1.json
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/ipwhois_gist.json
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/ipwhois_raw_10.0.0.1.json
+-rw-r--r--   0        0        0     9733 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/pt_passive_dns_gist.json
+-rw-r--r--   0        0        0    10017 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/pt_whois_1.1.1.1.json
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/pt_whois_gist.json
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/shodan_1.1.1.1.json
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/shodan_gist.json
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/shodan_gist_2.json
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/shodan_one.json
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/shodan_wired.json
+-rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/urlhaus_1.1.1.1.json
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/urlhaus_gist.json
+-rw-r--r--   0        0        0    18175 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/vt_domain_gist.json
+-rw-r--r--   0        0        0    20408 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/vt_domain_google.json
+-rw-r--r--   0        0        0    17624 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/vt_domain_tucows.json
+-rw-r--r--   0        0        0    17725 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/vt_ip_1.1.1.1.json
+-rw-r--r--   0        0        0    11171 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/vt_ip_142.251.220.110.json
+-rw-r--r--   0        0        0     5673 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/vt_resolutions_gist.json
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/vt_resolutions_one.json
+-rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/vt_resolutions_wired.json
+-rw-r--r--   0        0        0    19472 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/vt_whois_1.1.1.1.json
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/vt_whois_bbc.json
+-rw-r--r--   0        0        0    14040 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/vt_whois_example.json
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/vt_whois_example_2.json
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/vt_whois_foo.json
+-rw-r--r--   0        0        0    18644 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/vt_whois_gist.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/__init__.py
+-rw-r--r--   0        0        0     8239 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/main.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/types.py
+-rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/utils.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/clients/__init__.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/clients/abuseipdb.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/clients/base.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/clients/greynoise.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/clients/ip2whois.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/clients/ipwhois.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/clients/passivetotal.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/clients/shodan.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/clients/urlhaus.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/clients/virustotal.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/handlers/__init__.py
+-rw-r--r--   0        0        0     4931 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/handlers/base.py
+-rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/handlers/domain.py
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/handlers/ip.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/models/__init__.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/models/abuseipdb.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/models/common.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/models/greynoise.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/models/ip2whois.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/models/ipwhois.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/models/passivetotal.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/models/shodan.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/models/urlhaus.py
+-rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/models/virustotal.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/ui/__init__.py
+-rw-r--r--   0        0        0    19498 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/ui/base.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/ui/progress.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/ui/theme.py
+-rw-r--r--   0        0        0     8186 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/ui/view.py
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 wtfis-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 wtfis-0.9.0/LICENSE
+-rw-r--r--   0        0        0    10744 2020-02-02 00:00:00.000000 wtfis-0.9.0/README.md
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 wtfis-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    11547 2020-02-02 00:00:00.000000 wtfis-0.9.0/PKG-INFO
```

### Comparing `wtfis-0.8.0/Dockerfile` & `wtfis-0.9.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/imgs/demo-old.gif` & `wtfis-0.9.0/imgs/demo-old.gif`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/imgs/demo.gif` & `wtfis-0.9.0/imgs/demo.gif`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/imgs/example-greynoise.png` & `wtfis-0.9.0/imgs/example-greynoise.png`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/imgs/example-no-color.png` & `wtfis-0.9.0/imgs/example-no-color.png`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/imgs/example-one-column.png` & `wtfis-0.9.0/imgs/example-one-column.png`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/imgs/example-shodan.png` & `wtfis-0.9.0/imgs/example-shodan.png`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/imgs/example-urlhaus.png` & `wtfis-0.9.0/imgs/example-urlhaus.png`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/tests/conftest.py` & `wtfis-0.9.0/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import pytest
 from pathlib import Path
 from typing import Optional
 
 from rich.console import RenderableType
 from rich.text import Span, Text
 
+from wtfis.models.abuseipdb import AbuseIpDb
 from wtfis.models.greynoise import GreynoiseIp
 from wtfis.models.ipwhois import IpWhois
 from wtfis.models.shodan import ShodanIp
 from wtfis.models.urlhaus import UrlHaus
 
 
 class TestTheme:
     """ Expected theme values for the tests """
-    panel_title_main = "bold yellow"
+    panel_title = "bold yellow"
     heading_h1 = "bold bright_green on dark_green"
     heading_h2 = "bold yellow"
     table_field = "bold bright_magenta"
     table_value = "not bold default"
     nameserver_list = "bright_blue"
     timestamp_date = "not bold default"
     timestamp_t = "dim bright_white"
@@ -41,14 +42,19 @@
 
 def open_test_data(fname: str) -> str:
     path = Path(__file__).parent.resolve() / "test_data" / fname
     with open(path) as f:
         return f.read()
 
 
+def abuseipdb_get_ip(ip, pool) -> AbuseIpDb:
+    """ Mock replacement for AbuseIpDbClient()._get_ip() """
+    return AbuseIpDb.model_validate(pool[ip])
+
+
 def greynoise_get(ip, pool) -> GreynoiseIp:
     """ Mock replacement for GreynoiseClient().get_ip() """
     return GreynoiseIp.model_validate(pool[ip])
 
 
 def ipwhois_get(ip, pool) -> IpWhois:
     """ Mock replacement for IpWhoisClient().get_ipwhois() """
@@ -56,16 +62,16 @@
 
 
 def shodan_get_ip(ip, pool) -> ShodanIp:
     """ Mock replacement for ShodanClient().get_ip() """
     return ShodanIp.model_validate(pool[ip])
 
 
-def urlhaus_get_host(entity, pool) -> ShodanIp:
-    """ Mock replacement for Urlhaus()._get_host() """
+def urlhaus_get_host(entity, pool) -> UrlHaus:
+    """ Mock replacement for UrlHausClient()._get_host() """
     return UrlHaus.model_validate(pool[entity])
 
 
 def timestamp_text(ts) -> Optional[RenderableType]:
     """ Standard timestamp formatting """
     theme = TestTheme()
     return Text(
@@ -85,14 +91,19 @@
 
 @pytest.fixture(scope="module")
 def theme():
     return TestTheme()
 
 
 @pytest.fixture(scope="module")
+def mock_abuseipdb_get():
+    return abuseipdb_get_ip
+
+
+@pytest.fixture(scope="module")
 def mock_greynoise_get():
     return greynoise_get
 
 
 @pytest.fixture(scope="module")
 def mock_ipwhois_get():
     return ipwhois_get
```

### Comparing `wtfis-0.8.0/tests/test_cli.py` & `wtfis-0.9.0/tests/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,41 @@
 import json
 import os
+from pathlib import Path
+from unittest.mock import MagicMock, patch
+
 import pytest
 from dotenv import load_dotenv
-from pathlib import Path
 from rich.console import Console
-from rich.progress import (
-    BarColumn,
-    Progress,
-    SpinnerColumn,
-    TaskProgressColumn,
-    TimeElapsedColumn,
-    TextColumn,
-)
-from unittest.mock import patch, MagicMock
+from rich.progress import (BarColumn, Progress, SpinnerColumn,
+                           TaskProgressColumn, TextColumn, TimeElapsedColumn)
 
+from wtfis.clients.abuseipdb import AbuseIpDbClient
 from wtfis.clients.greynoise import GreynoiseClient
 from wtfis.clients.ip2whois import Ip2WhoisClient
 from wtfis.clients.ipwhois import IpWhoisClient
 from wtfis.clients.passivetotal import PTClient
 from wtfis.clients.shodan import ShodanClient
 from wtfis.clients.urlhaus import UrlHausClient
 from wtfis.clients.virustotal import VTClient
 from wtfis.handlers.domain import DomainHandler
 from wtfis.handlers.ip import IpAddressHandler
-from wtfis.main import (
-    generate_entity_handler,
-    generate_view,
-    main,
-    parse_args,
-    parse_env,
-)
+from wtfis.main import (generate_entity_handler, generate_view, main,
+                        parse_args, parse_env)
 from wtfis.models.virustotal import Domain, IpAddress
 from wtfis.ui.view import DomainView, IpAddressView
 
-
 POSSIBLE_ENV_VARS = [
     "VT_API_KEY",
     "PT_API_KEY",
     "PT_API_USER",
     "IP2WHOIS_API_KEY",
     "SHODAN_API_KEY",
     "GREYNOISE_API_KEY",
+    "ABUSEIPDB_API_KEY",
     "WTFIS_DEFAULTS",
 ]
 
 
 def unset_env_vars():
     for var in POSSIBLE_ENV_VARS:
         try:
@@ -80,14 +71,15 @@
     fake_env_vars = {
         "VT_API_KEY": "foo",
         "PT_API_KEY": "bar",
         "PT_API_USER": "baz@example.com",
         "IP2WHOIS_API_KEY": "alice",
         "SHODAN_API_KEY": "hunter2",
         "GREYNOISE_API_KEY": "upupdowndown",
+        "ABUSEIPDB_API_KEY": "dummy",
     }
     return fake_load_dotenv(tmp_path, fake_env_vars)
 
 
 @pytest.fixture()
 def fake_load_dotenv_2(tmp_path):
     fake_env_vars = {
@@ -108,15 +100,16 @@
 
 
 @pytest.fixture()
 def fake_load_dotenv_4(tmp_path):
     fake_env_vars = {
         "VT_API_KEY": "foo",
         "GREYNOISE_API_KEY": "bar",
-        "WTFIS_DEFAULTS": "-g -u",
+        "ABUSEIPDB_API_KEY": "dummy",
+        "WTFIS_DEFAULTS": "-g -u -a",
     }
     return fake_load_dotenv(tmp_path, fake_env_vars)
 
 
 @pytest.fixture()
 def fake_load_dotenv_vt_whois(tmp_path):
     fake_env_vars = {
@@ -259,25 +252,52 @@
             "main",
             "www.example.com",
             "-u",
         ]):
             args = parse_args()
             assert args.use_urlhaus is True
 
+    def test_abuseipdb_ok(self):
+        os.environ["ABUSEIPDB_API_KEY"] = "foo"
+        with patch("sys.argv", [
+            "main",
+            "1.1.1.1",
+            "-a",
+        ]):
+            args = parse_args()
+            assert args.use_abuseipdb is True
+        del os.environ["ABUSEIPDB_API_KEY"]
+
+    def test_abuseipdb_error(self, capsys):
+        with pytest.raises(SystemExit) as e:
+            with patch("sys.argv", [
+                "main",
+                "1.1.1.1",
+                "-a",
+            ]):
+                parse_args()
+
+        capture = capsys.readouterr()
+
+        assert capture.err == "usage: main [-h]\nmain: error: ABUSEIPDB_API_KEY is not set\n"
+        assert e.type == SystemExit
+        assert e.value.code == 2
+
 
 class TestEnvs:
     def test_env_file(self, fake_load_dotenv_1):
         with patch("wtfis.main.load_dotenv", fake_load_dotenv_1):
             parse_env()
             assert os.environ["VT_API_KEY"] == "foo"
             assert os.environ["PT_API_KEY"] == "bar"
             assert os.environ["PT_API_USER"] == "baz@example.com"
             assert os.environ["IP2WHOIS_API_KEY"] == "alice"
             assert os.environ["SHODAN_API_KEY"] == "hunter2"
             assert os.environ["GREYNOISE_API_KEY"] == "upupdowndown"
+            assert os.environ["ABUSEIPDB_API_KEY"] == "dummy"
         unset_env_vars()
 
     @patch("wtfis.main.load_dotenv", MagicMock())
     def test_required_env_vars(self):
         os.environ["VT_API_KEY"] = "foo"
         parse_env()
         unset_env_vars()
@@ -364,14 +384,15 @@
                 args = parse_args()
                 assert args.entity == "1.1.1.1"
                 assert args.no_color is False
                 assert args.one_column is False
                 assert args.use_shodan is False
                 assert args.use_greynoise is True
                 assert args.use_urlhaus is False
+                assert args.use_abuseipdb is True
         unset_env_vars()
 
 
 class TestGenEntityHandler:
     """ Tests for the generate_entity_handler function """
     @patch("sys.argv", ["main", "www.example[.]com"])
     def test_handler_domain_1(self, fake_load_dotenv_1):
@@ -445,28 +466,44 @@
         assert isinstance(entity._vt, VTClient)
         assert isinstance(entity._enricher, IpWhoisClient)
         assert isinstance(entity._whois, PTClient)
         assert entity._greynoise is None
         assert entity._urlhaus is None
         unset_env_vars()
 
+    @patch("sys.argv", ["main", "1[.]1[.]1[.]1", "-s", "-g", "-u", "-a"])
+    def test_handler_ip_2(self, fake_load_dotenv_1):
+        """ IP with various options """
+        with patch("wtfis.main.load_dotenv", fake_load_dotenv_1):
+            parse_env()
+            console = Console()
+            progress = simulate_progress(console),
+            entity = generate_entity_handler(parse_args(), console, progress)
+        assert isinstance(entity._enricher, ShodanClient)
+        assert isinstance(entity._whois, PTClient)
+        assert isinstance(entity._greynoise, GreynoiseClient)
+        assert isinstance(entity._urlhaus, UrlHausClient)
+        assert isinstance(entity._abuseipdb, AbuseIpDbClient)
+        unset_env_vars()
+
 
 class TestGenView:
     """ Tests for the generate_view function """
     @patch("wtfis.main.DomainView", return_value=MagicMock(spec=DomainView))
     def test_view_domain_1(self, m_domain_view, test_data):
         """ Domain view with default params """
         entity = DomainHandler(
             entity=MagicMock(),
             console=MagicMock(),
             progress=MagicMock(),
             vt_client=MagicMock(),
             ip_enricher_client=MagicMock(),
             whois_client=MagicMock(),
             greynoise_client=MagicMock(),
+            abuseipdb_client=MagicMock(),
             urlhaus_client=MagicMock(),
         )
         entity.vt_info = Domain.model_validate(json.loads(test_data("vt_domain_gist.json")))
         entity.whois = MagicMock()
         entity.ip_enrich = MagicMock()
         view = generate_view(MagicMock(), MagicMock(), entity)
         assert isinstance(view, DomainView)
@@ -478,14 +515,15 @@
             entity=MagicMock(),
             console=MagicMock(),
             progress=MagicMock(),
             vt_client=MagicMock(),
             ip_enricher_client=MagicMock(),
             whois_client=MagicMock(),
             greynoise_client=MagicMock(),
+            abuseipdb_client=MagicMock(),
             urlhaus_client=MagicMock(),
         )
         entity.vt_info = IpAddress.model_validate(json.loads(test_data("vt_ip_1.1.1.1.json")))
         entity.whois = MagicMock()
         entity.ip_enrich = MagicMock()
         view = generate_view(MagicMock(), MagicMock(), entity)
         assert isinstance(view, IpAddressView)
```

### Comparing `wtfis-0.8.0/tests/test_clients.py` & `wtfis-0.9.0/tests/test_clients.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 import json
 import pytest
 from unittest.mock import MagicMock, patch
 
+from wtfis.clients.abuseipdb import AbuseIpDbClient
 from wtfis.clients.base import requests
 from wtfis.clients.greynoise import GreynoiseClient
 from wtfis.clients.ip2whois import Ip2WhoisClient
 from wtfis.clients.ipwhois import IpWhoisClient
 from wtfis.clients.passivetotal import PTClient
 from wtfis.clients.shodan import APIError, Shodan, ShodanClient
 from wtfis.clients.urlhaus import UrlHausClient
 from wtfis.clients.virustotal import VTClient
 from wtfis.models.ipwhois import IpWhoisMap
 
 
 @pytest.fixture()
+def abuseipdb_client():
+    return AbuseIpDbClient("dummykey")
+
+
+@pytest.fixture()
 def greynoise_client():
     return GreynoiseClient("dummykey")
 
 
 @pytest.fixture()
 def ip2whois_client():
     return Ip2WhoisClient("dummykey")
@@ -44,14 +50,35 @@
 
 
 @pytest.fixture()
 def virustotal_client():
     return VTClient("dummykey")
 
 
+class TestAbuseIpDbClient:
+    def test_init(self, abuseipdb_client):
+        assert abuseipdb_client.name == "AbuseIPDB"
+        assert abuseipdb_client.api_key == "dummykey"
+
+    @patch.object(requests.Session, "get")
+    def test_enrich_ips(self, mock_requests_get, test_data, abuseipdb_client):
+        mock_resp = MagicMock()
+        mock_resp.status_code = 200
+        mock_resp.json.return_value = json.loads(test_data("abuseipdb_1.1.1.1_raw.json"))
+        mock_requests_get.return_value = mock_resp
+
+        abuseipdb = abuseipdb_client.enrich_ips("thisdoesntmatter").root["1.1.1.1"]
+
+        assert abuseipdb.ip_address == "1.1.1.1"
+        assert abuseipdb.abuse_confidence_score == 100
+        assert abuseipdb.usage_type == "Data Center/Web Hosting/Transit"
+        assert abuseipdb.total_reports == 567
+        assert abuseipdb.num_distinct_users == 123
+
+
 class TestIp2WhoisClient:
     def test_init(self, ip2whois_client):
         assert ip2whois_client.api_key == "dummykey"
         assert ip2whois_client.name == "IP2Whois"
 
     @patch.object(requests.Session, "get")
     def test_get_whois(self, mock_requests_get, test_data, ip2whois_client):
```

### Comparing `wtfis-0.8.0/tests/test_handlers.py` & `wtfis-0.9.0/tests/test_handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import json
+from unittest.mock import MagicMock, patch
+
 import pytest
 from requests.exceptions import ConnectionError
 from rich.console import Console
-from unittest.mock import MagicMock, patch
 
+from wtfis.clients.abuseipdb import AbuseIpDbClient
 from wtfis.clients.base import requests
 from wtfis.clients.greynoise import GreynoiseClient
 from wtfis.clients.ipwhois import IpWhoisClient
 from wtfis.clients.passivetotal import PTClient
 from wtfis.clients.urlhaus import UrlHausClient
 from wtfis.clients.virustotal import VTClient
 from wtfis.handlers.domain import DomainHandler
@@ -22,28 +24,30 @@
         entity="www.example[.]com",
         console=Console(),
         progress=MagicMock(),
         vt_client=VTClient("dummykey"),
         ip_enricher_client=IpWhoisClient(),
         whois_client=PTClient("dummyuser", "dummykey"),
         greynoise_client=GreynoiseClient("dummykey"),
+        abuseipdb_client=AbuseIpDbClient("dummykey"),
         urlhaus_client=UrlHausClient(),
         max_resolutions=max_resolutions,
     )
 
 
 def generate_ip_handler():
     return IpAddressHandler(
         entity="1[.]1[.]1[.]1",
         console=Console(),
         progress=MagicMock(),
         vt_client=VTClient("dummykey"),
         ip_enricher_client=IpWhoisClient(),
         whois_client=PTClient("dummyuser", "dummykey"),
         greynoise_client=GreynoiseClient("dummykey"),
+        abuseipdb_client=AbuseIpDbClient("dummykey"),
         urlhaus_client=UrlHausClient(),
     )
 
 
 @pytest.fixture
 def domain_handler():
     return generate_domain_handler
@@ -370,21 +374,23 @@
     def test_fetch_data(self, ip_handler):
         handler = ip_handler()
         handler._fetch_vt_ip_address = MagicMock()
         handler._fetch_ip_enrichments = MagicMock()
         handler._fetch_whois = MagicMock()
         handler._fetch_greynoise = MagicMock()
         handler._fetch_urlhaus = MagicMock()
+        handler._fetch_abuseipdb = MagicMock()
 
         handler.fetch_data()
         handler._fetch_vt_ip_address.assert_called_once()
         handler._fetch_ip_enrichments.assert_called_once()
         handler._fetch_whois.assert_called_once()
         handler._fetch_greynoise.assert_called_once()
         handler._fetch_urlhaus.assert_called_once()
+        handler._fetch_abuseipdb.assert_called_once()
 
     @patch.object(requests.Session, "get")
     def test_vt_http_error(self, mock_requests_get, ip_handler, capsys):
         handler = ip_handler()
         mock_resp = requests.models.Response()
 
         mock_resp.status_code = 404
@@ -594,7 +600,25 @@
 
         handler._fetch_urlhaus()
         assert handler.warnings[0] == "Could not fetch URLhaus: Foo bar message"
 
         handler.print_warnings()
         capture = capsys.readouterr()
         assert capture.out.startswith("WARN: Could not fetch URLhaus: Foo bar message")
+
+    @patch.object(requests.Session, "get")
+    def test_abuseipdb_429_error(self, mock_requests_get, ip_handler, capsys):
+        """
+        Test fail open behavior of AbuseIPDB when rate limited
+        """
+        handler = ip_handler()
+        mock_resp = requests.models.Response()
+
+        mock_resp.status_code = 429
+        mock_requests_get.return_value = mock_resp
+
+        handler._fetch_abuseipdb("1.2.3.4")
+        assert handler.warnings[0].startswith("Could not fetch AbuseIPDB: 429 Client Error:")
+
+        handler.print_warnings()
+        capture = capsys.readouterr()
+        assert capture.out.startswith("WARN: Could not fetch AbuseIPDB: 429 Client Error:")
```

### Comparing `wtfis-0.8.0/tests/test_models_vt.py` & `wtfis-0.9.0/tests/test_models_vt.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/tests/test_ui_domain_view.py` & `wtfis-0.9.0/tests/test_ui_domain_view.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-import pytest
 import json
+from unittest.mock import MagicMock
 
+import pytest
 from rich.console import Console
 from rich.panel import Panel
 from rich.table import Table
 from rich.text import Span, Text
-from unittest.mock import MagicMock
 
+from wtfis.clients.abuseipdb import AbuseIpDbClient
 from wtfis.clients.greynoise import GreynoiseClient
 from wtfis.clients.ipwhois import IpWhoisClient
 from wtfis.clients.shodan import ShodanClient
+from wtfis.models.abuseipdb import AbuseIpDbMap
 from wtfis.clients.urlhaus import UrlHausClient
 from wtfis.models.greynoise import GreynoiseIpMap
 from wtfis.models.ip2whois import Whois as Ip2Whois
 from wtfis.models.ipwhois import IpWhoisMap
 from wtfis.models.passivetotal import Whois as PTWhois
 from wtfis.models.urlhaus import UrlHausMap
 from wtfis.models.virustotal import (
@@ -37,14 +39,15 @@
     return DomainView(
         console=Console(),
         entity=Domain.model_validate(json.loads(test_data("vt_domain_gist.json"))),
         resolutions=resolutions,
         whois=PTWhois.model_validate(json.loads(test_data("pt_whois_gist.json"))),
         ip_enrich=ip_enrich,
         greynoise=GreynoiseIpMap.model_validate({}),
+        abuseipdb=AbuseIpDbMap.model_validate({}),
         urlhaus=UrlHausMap.model_validate({}),
     )
 
 
 @pytest.fixture()
 def view02(test_data):
     """
@@ -54,14 +57,15 @@
     return DomainView(
         console=Console(),
         entity=MagicMock(),
         resolutions=Resolutions.model_validate(json.loads(test_data("vt_resolutions_gist.json"))),
         whois=VTWhois.model_validate(json.loads(test_data("vt_whois_gist.json"))),
         ip_enrich=IpWhoisMap.model_validate({}),
         greynoise=GreynoiseIpMap.model_validate({}),
+        abuseipdb=AbuseIpDbMap.model_validate({}),
         urlhaus=MagicMock(),
         max_resolutions=1,
     )
 
 
 @pytest.fixture()
 def view03(test_data):
@@ -69,14 +73,15 @@
     return DomainView(
         console=Console(),
         entity=MagicMock(),
         resolutions=MagicMock(),
         whois=VTWhois.model_validate(json.loads(test_data("vt_whois_bbc.json"))),
         ip_enrich=MagicMock(),
         greynoise=MagicMock(),
+        abuseipdb=MagicMock(),
         urlhaus=MagicMock(),
     )
 
 
 @pytest.fixture()
 def view04(test_data):
     """
@@ -86,42 +91,45 @@
     return DomainView(
         console=Console(),
         entity=Domain.model_validate(json.loads(test_data("vt_domain_google.json"))),
         resolutions=None,
         whois=MagicMock(),
         ip_enrich=MagicMock(),
         greynoise=MagicMock(),
+        abuseipdb=MagicMock(),
         urlhaus=MagicMock(),
     )
 
 
 @pytest.fixture()
 def view05(test_data):
     """ tucows.com domain. Domain test only. Test domain with negative reputation and no popularity."""
     return DomainView(
         console=Console(),
         entity=Domain.model_validate(json.loads(test_data("vt_domain_tucows.json"))),
         resolutions=MagicMock(),
         whois=MagicMock(),
         ip_enrich=MagicMock(),
         greynoise=MagicMock(),
+        abuseipdb=MagicMock(),
         urlhaus=MagicMock(),
     )
 
 
 @pytest.fixture()
 def view06(test_data):
     """ exmple.com VT whois. Whois test only. Test empty whois_map."""
     return DomainView(
         console=Console(),
         entity=MagicMock(),
         resolutions=MagicMock(),
         whois=VTWhois.model_validate(json.loads(test_data("vt_whois_example_2.json"))),
         ip_enrich=MagicMock(),
         greynoise=MagicMock(),
+        abuseipdb=MagicMock(),
         urlhaus=MagicMock(),
     )
 
 
 @pytest.fixture()
 def view07(test_data, mock_shodan_get_ip):
     """ gist.github.com with Shodan. Only test resolution and IP enrich. """
@@ -135,14 +143,15 @@
     return DomainView(
         console=Console(),
         entity=MagicMock(),
         resolutions=resolutions,
         whois=MagicMock(),
         ip_enrich=ip_enrich,
         greynoise=GreynoiseIpMap.model_validate({}),
+        abuseipdb=AbuseIpDbMap.model_validate({}),
         urlhaus=MagicMock(),
     )
 
 
 @pytest.fixture()
 def view08(test_data, mock_shodan_get_ip):
     """ www.wired.com with Shodan. Only test resolution and IP enrich. """
@@ -156,41 +165,48 @@
     return DomainView(
         console=Console(),
         entity=MagicMock(),
         resolutions=resolutions,
         whois=MagicMock(),
         ip_enrich=ip_enrich,
         greynoise=GreynoiseIpMap.model_validate({}),
+        abuseipdb=AbuseIpDbMap.model_validate({}),
         urlhaus=MagicMock(),
         max_resolutions=1,
     )
 
 
 @pytest.fixture()
-def view09(test_data, mock_shodan_get_ip, mock_greynoise_get):
-    """ one.one.one.one with Shodan and Greynoise. Only test resolution and IP enrich. """
+def view09(test_data, mock_shodan_get_ip, mock_greynoise_get, mock_abuseipdb_get):
+    """ one.one.one.one with Shodan, Greynoise and AbuseIPDB. Only test resolution and IP enrich. """
     resolutions = Resolutions.model_validate(json.loads(test_data("vt_resolutions_one.json")))
 
     shodan_pool = json.loads(test_data("shodan_one.json"))
     shodan_client = ShodanClient(MagicMock())
     shodan_client._get_ip = MagicMock(side_effect=lambda ip: mock_shodan_get_ip(ip, shodan_pool))
     ip_enrich = shodan_client.enrich_ips(*resolutions.ip_list(1))
 
     greynoise_pool = json.loads(test_data("greynoise_one.json"))
     greynoise_client = GreynoiseClient("dummykey")
     greynoise_client._get_ip = MagicMock(side_effect=lambda ip: mock_greynoise_get(ip, greynoise_pool))
     greynoise_enrich = greynoise_client.enrich_ips(*resolutions.ip_list(1))
 
+    abuseipdb_pool = json.loads(test_data("abuseipdb_one.json"))
+    abuseipdb_client = AbuseIpDbClient("dummykey")
+    abuseipdb_client._get_ip = MagicMock(side_effect=lambda ip: mock_abuseipdb_get(ip, abuseipdb_pool))
+    abuseipdb_enrich = abuseipdb_client.enrich_ips(*resolutions.ip_list(1))
+
     return DomainView(
         console=Console(),
         entity=MagicMock(),
         resolutions=resolutions,
         whois=MagicMock(),
         ip_enrich=ip_enrich,
         greynoise=greynoise_enrich,
+        abuseipdb=abuseipdb_enrich,
         urlhaus=MagicMock(),
         max_resolutions=1,
     )
 
 
 @pytest.fixture()
 def view10(test_data):
@@ -198,14 +214,15 @@
     return DomainView(
         console=Console(),
         entity=MagicMock(),
         resolutions=MagicMock(),
         whois=VTWhois.model_validate(json.loads(test_data("vt_whois_foo.json"))),
         ip_enrich=MagicMock(),
         greynoise=GreynoiseIpMap.model_validate({}),
+        abuseipdb=AbuseIpDbMap.model_validate({}),
         urlhaus=MagicMock(),
     )
 
 
 @pytest.fixture()
 def view11(test_data, mock_shodan_get_ip):
     """ gist.github.com with Shodan. Only test IP enrich. Test empty open ports. """
@@ -219,42 +236,45 @@
     return DomainView(
         console=Console(),
         entity=MagicMock(),
         resolutions=resolutions,
         whois=MagicMock(),
         ip_enrich=ip_enrich,
         greynoise=GreynoiseIpMap.model_validate({}),
+        abuseipdb=AbuseIpDbMap.model_validate({}),
         urlhaus=MagicMock(),
     )
 
 
 @pytest.fixture()
 def view12(test_data):
     """ Dummy IP2WHOIS whois. Whois panel test only. """
     return DomainView(
         console=Console(),
         entity=MagicMock(),
         resolutions=MagicMock(),
         whois=Ip2Whois.model_validate(json.loads(test_data("ip2whois_whois_hotmail.json"))),
         ip_enrich=MagicMock(),
         greynoise=MagicMock(),
+        abuseipdb=MagicMock(),
         urlhaus=MagicMock(),
     )
 
 
 @pytest.fixture()
 def view13(test_data):
     """ Dummy IP2WHOIS whois. Whois panel test only. Test null registrant. """
     return DomainView(
         console=Console(),
         entity=MagicMock(),
         resolutions=MagicMock(),
         whois=Ip2Whois.model_validate(json.loads(test_data("ip2whois_whois_bbc.json"))),
         ip_enrich=MagicMock(),
         greynoise=MagicMock(),
+        abuseipdb=MagicMock(),
         urlhaus=MagicMock(),
     )
 
 
 @pytest.fixture()
 def view14(test_data, mock_ipwhois_get, mock_urlhaus_get):
     """ Same as view01() but with Urlhaus enrichment. Test URLhaus only. """
@@ -273,24 +293,25 @@
     return DomainView(
         console=Console(),
         entity=Domain.model_validate(json.loads(test_data("vt_domain_gist.json"))),
         resolutions=resolutions,
         whois=PTWhois.model_validate(json.loads(test_data("pt_whois_gist.json"))),
         ip_enrich=ip_enrich,
         greynoise=GreynoiseIpMap.model_validate({}),
+        abuseipdb=AbuseIpDbMap.model_validate({}),
         urlhaus=urlhaus_enrich,
     )
 
 
 class TestView01:
     def test_domain_panel(self, view01, theme, display_timestamp):
         domain = view01.domain_panel()
         assert type(domain) is Panel
         assert domain.title == Text("gist.github.com")
-        assert domain.title.style == theme.panel_title_main
+        assert domain.title.style == theme.panel_title
 
         #
         # VT section
         #
 
         vt_section = domain.renderable.renderables[0]
 
@@ -1255,14 +1276,18 @@
                 spans=[Span(0, 8, "link https://www.shodan.io/host/1.0.0.1")]
             ),
             "Last Scan:",
             Text(
                 "GreyNoise:",
                 spans=[Span(0, 9, "link https://viz.greynoise.io/riot/1.0.0.1")]
             ),
+            Text(
+                "AbuseIPDB:",
+                spans=[Span(0, 9, "link https://www.abuseipdb.com/check/1.0.0.1")]
+            ),
         ]
         assert table.columns[1].style == theme.table_value
         assert table.columns[1].justify == "left"
         assert table.columns[1]._cells == [
             Text("2/94 malicious"),
             display_timestamp("2020-08-01T22:07:20Z"),
             Text(
@@ -1330,14 +1355,22 @@
                     Span(2, 6, theme.tags),
                     Span(8, 9, theme.warn),
                     Span(10, 15, theme.tags),
                     Span(17, 18, theme.info),
                     Span(19, 25, theme.tags_green),
                 ]
             ),
+            Text(
+                "100 confidence score (567 reports)",
+                spans=[
+                    Span(0, 3, theme.error),
+                    Span(3, 20, "red"),
+                    Span(20, 34, theme.table_value),
+                ]
+            ),
         ]
 
         # Old timestamp warning
         # assert group[1].renderables[1] == Text("**Enrichment data may be inaccurate")
 
         # Spacing
         assert res.renderable.renderables[2] == ""
@@ -1548,15 +1581,18 @@
             "Tags:",
         ]
         assert table.columns[1].style == theme.table_value
         assert table.columns[1].justify == "left"
         assert table.columns[1]._cells == [
             Text(
                 "1+ online (3248 total)",
-                spans=[Span(9, 22, theme.table_value)],
+                spans=[
+                    Span(0, 9, theme.error),
+                    Span(9, 22, theme.table_value),
+                ],
             ),
             Text(
                 "abused_legit_malware in spamhaus\nlisted in surbl",
                 spans=[
                     Span(0, 20, theme.urlhaus_bl_med),
                     Span(24, 32, theme.urlhaus_bl_name),
                     Span(33, 48, ""),
```

### Comparing `wtfis-0.8.0/tests/test_ui_ip_view.py` & `wtfis-0.9.0/tests/test_ui_ip_view.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import json
 
 from rich.console import Console
 from rich.panel import Panel
 from rich.table import Table
 from rich.text import Span, Text
 from unittest.mock import MagicMock
+from wtfis.clients.abuseipdb import AbuseIpDbClient
 
 from wtfis.clients.greynoise import GreynoiseClient
 from wtfis.clients.ipwhois import IpWhoisClient
 from wtfis.clients.shodan import ShodanClient
 from wtfis.clients.urlhaus import UrlHausClient
 from wtfis.models.greynoise import GreynoiseIpMap
 from wtfis.models.ipwhois import IpWhoisMap
@@ -19,38 +20,45 @@
     IpAddress,
     Whois as VTWhois,
 )
 from wtfis.ui.view import IpAddressView
 
 
 @pytest.fixture()
-def view01(test_data, mock_ipwhois_get, mock_greynoise_get, mock_urlhaus_get):
+def view01(test_data, mock_abuseipdb_get, mock_ipwhois_get, mock_greynoise_get, mock_urlhaus_get):
     """ 1.1.1.1 with PT whois. Complete test of all panels. Also test print(). """
     ip = "1.1.1.1"
+
+    abuseipdb_pool = json.loads(test_data("abuseipdb_1.1.1.1_red.json"))
+    abuseipdb_client = AbuseIpDbClient("dummykey")
+    abuseipdb_client._get_ip = MagicMock(side_effect=lambda ip: mock_abuseipdb_get(ip, abuseipdb_pool))
+    abuseipdb_enrich = abuseipdb_client.enrich_ips(ip)
+
     ipwhois_pool = json.loads(test_data("ipwhois_1.1.1.1.json"))
     ipwhois_client = IpWhoisClient()
     ipwhois_client._get_ipwhois = MagicMock(side_effect=lambda ip: mock_ipwhois_get(ip, ipwhois_pool))
     ip_enrich = ipwhois_client.enrich_ips(ip)
 
     greynoise_pool = json.loads(test_data("greynoise_1.1.1.1.json"))
     greynoise_client = GreynoiseClient("dummykey")
     greynoise_client._get_ip = MagicMock(side_effect=lambda ip: mock_greynoise_get(ip, greynoise_pool))
     greynoise_enrich = greynoise_client.enrich_ips(ip)
 
     urlhaus_pool = json.loads(test_data("urlhaus_1.1.1.1.json"))
     urlhaus_client = UrlHausClient()
     urlhaus_client._get_host = MagicMock(side_effect=lambda ip: mock_urlhaus_get(ip, urlhaus_pool))
-    urlhaus_enrich = urlhaus_client.enrich_ips("1.1.1.1")
+    urlhaus_enrich = urlhaus_client.enrich_ips(ip)
 
     return IpAddressView(
         console=Console(),
         entity=IpAddress.model_validate(json.loads(test_data("vt_ip_1.1.1.1.json"))),
         whois=PTWhois.model_validate(json.loads(test_data("pt_whois_1.1.1.1.json"))),
         ip_enrich=ip_enrich,
         greynoise=greynoise_enrich,
+        abuseipdb=abuseipdb_enrich,
         urlhaus=urlhaus_enrich,
     )
 
 
 @pytest.fixture()
 def view02(test_data, mock_shodan_get_ip, mock_greynoise_get):
     """ 1.1.1.1 with Shodan and Greynoise. Test the whole IP panel. """
@@ -67,27 +75,29 @@
 
     return IpAddressView(
         console=Console(),
         entity=IpAddress.model_validate(json.loads(test_data("vt_ip_1.1.1.1.json"))),
         whois=MagicMock(),
         ip_enrich=ip_enrich,
         greynoise=greynoise_enrich,
+        abuseipdb=MagicMock(),
         urlhaus=UrlHausMap.model_validate({}),
     )
 
 
 @pytest.fixture()
 def view03(test_data):
     """ 1.1.1.1 VT whois. Whois panel test only."""
     return IpAddressView(
         console=Console(),
         entity=MagicMock(),
         whois=VTWhois.model_validate(json.loads(test_data("vt_whois_1.1.1.1.json"))),
         ip_enrich=MagicMock(),
         greynoise=MagicMock(),
+        abuseipdb=MagicMock(),
         urlhaus=MagicMock(),
     )
 
 
 @pytest.fixture()
 def view04(test_data):
     """
@@ -96,14 +106,15 @@
     """
     return IpAddressView(
         console=Console(),
         entity=IpAddress.model_validate(json.loads(test_data("vt_ip_142.251.220.110.json"))),
         whois=MagicMock(),
         ip_enrich=IpWhoisMap.model_validate({}),
         greynoise=GreynoiseIpMap.model_validate({}),
+        abuseipdb=MagicMock(),
         urlhaus=UrlHausMap.model_validate({}),
     )
 
 
 @pytest.fixture()
 def view05(test_data, mock_greynoise_get):
     """ 1.1.1.1 with alt Greynoise results. Test Greynoise only. """
@@ -115,14 +126,15 @@
 
     return IpAddressView(
         console=Console(),
         entity=IpAddress.model_validate(json.loads(test_data("vt_ip_1.1.1.1.json"))),
         whois=MagicMock(),
         ip_enrich=IpWhoisMap.model_validate({}),
         greynoise=greynoise_enrich,
+        abuseipdb=MagicMock(),
         urlhaus=UrlHausMap.model_validate({}),
     )
 
 
 @pytest.fixture()
 def view06(test_data, mock_greynoise_get):
     """ 1.1.1.1 with another alt Greynoise result (unknown class). Test Greynoise only. """
@@ -134,24 +146,65 @@
 
     return IpAddressView(
         console=Console(),
         entity=IpAddress.model_validate(json.loads(test_data("vt_ip_1.1.1.1.json"))),
         whois=MagicMock(),
         ip_enrich=IpWhoisMap.model_validate({}),
         greynoise=greynoise_enrich,
+        abuseipdb=MagicMock(),
+        urlhaus=MagicMock(),
+    )
+
+
+@pytest.fixture()
+def view07(test_data, mock_abuseipdb_get):
+    """ 1.1.1.1 with green AbuseIPDB score. Test AbuseIPDB only. """
+    ip = "1.1.1.1"
+    abuseipdb_pool = json.loads(test_data("abuseipdb_1.1.1.1_green.json"))
+    abuseipdb_client = AbuseIpDbClient("dummykey")
+    abuseipdb_client._get_ip = MagicMock(side_effect=lambda ip: mock_abuseipdb_get(ip, abuseipdb_pool))
+    abuseipdb_enrich = abuseipdb_client.enrich_ips(ip)
+
+    return IpAddressView(
+        console=Console(),
+        entity=IpAddress.model_validate(json.loads(test_data("vt_ip_1.1.1.1.json"))),
+        whois=MagicMock(),
+        ip_enrich=IpWhoisMap.model_validate({}),
+        greynoise=MagicMock(),
+        abuseipdb=abuseipdb_enrich,
+        urlhaus=MagicMock(),
+    )
+
+
+@pytest.fixture()
+def view08(test_data, mock_abuseipdb_get):
+    """ 1.1.1.1 with yellow AbuseIPDB score. Test AbuseIPDB only. """
+    ip = "1.1.1.1"
+    abuseipdb_pool = json.loads(test_data("abuseipdb_1.1.1.1_yellow.json"))
+    abuseipdb_client = AbuseIpDbClient("dummykey")
+    abuseipdb_client._get_ip = MagicMock(side_effect=lambda ip: mock_abuseipdb_get(ip, abuseipdb_pool))
+    abuseipdb_enrich = abuseipdb_client.enrich_ips(ip)
+
+    return IpAddressView(
+        console=Console(),
+        entity=IpAddress.model_validate(json.loads(test_data("vt_ip_1.1.1.1.json"))),
+        whois=MagicMock(),
+        ip_enrich=IpWhoisMap.model_validate({}),
+        greynoise=MagicMock(),
+        abuseipdb=abuseipdb_enrich,
         urlhaus=MagicMock(),
     )
 
 
 class TestView01:
     def test_ip_panel(self, view01, theme, display_timestamp):
         ip = view01.ip_panel()
         assert type(ip) is Panel
         assert ip.title == Text("1.1.1.1")
-        assert ip.title.style == theme.panel_title_main
+        assert ip.title.style == theme.panel_title
 
         # Sections
         vt_section = ip.renderable.renderables[0]
         enrich_section = ip.renderable.renderables[2]
         urlhaus_section = ip.renderable.renderables[4]
         other_section = ip.renderable.renderables[6]
 
@@ -260,14 +313,15 @@
         assert table.columns[1].style == theme.table_value
         assert table.columns[1].justify == "left"
         print(table.columns[1])
         assert table.columns[1]._cells == [
             Text(
                 "10 online (10 total)",
                 spans=[
+                    Span(0, 9, theme.error),
                     Span(9, 20, theme.table_value),
                 ]
             ),
             Text(
                 "not listed in spamhaus\nnot listed in surbl",
                 spans=[
                     Span(0, 10, theme.urlhaus_bl_low),
@@ -301,14 +355,18 @@
         assert table.columns[0].style == theme.table_field
         assert table.columns[0].justify == "left"
         assert table.columns[0]._cells == [
             Text(
                 "GreyNoise:",
                 spans=[Span(0, 9, "link https://viz.greynoise.io/riot/1.1.1.1")]
             ),
+            Text(
+                "AbuseIPDB:",
+                spans=[Span(0, 9, "link https://www.abuseipdb.com/check/1.1.1.1")]
+            )
         ]
         assert table.columns[1].style == theme.table_value
         assert table.columns[1].justify == "left"
         assert table.columns[1]._cells == [
             Text(
                 "✓ riot  ✗ noise  ✓ benign",
                 spans=[
@@ -316,14 +374,22 @@
                     Span(2, 6, theme.tags),
                     Span(8, 9, theme.warn),
                     Span(10, 15, theme.tags),
                     Span(17, 18, theme.info),
                     Span(19, 25, theme.tags_green),
                 ]
             ),
+            Text(
+                "100 confidence score (567 reports)",
+                spans=[
+                    Span(0, 3, theme.error),
+                    Span(3, 20, "red"),
+                    Span(20, 34, theme.table_value),
+                ]
+            ),
         ]
 
     def test_whois_panel(self, view01, theme):
         whois = view01.whois_panel()
         assert type(whois) is Panel
         assert whois.title is None
 
@@ -722,7 +788,40 @@
                 Span(0, 1, theme.info),
                 Span(2, 6, theme.tags),
                 Span(8, 9, theme.warn),
                 Span(10, 15, theme.tags),
                 Span(19, 26, theme.tags),
             ]
         )
+
+
+class TestAbuseIpDbOnly:
+    def test_abuseipdb_green(self, view07, theme):
+        ip = view07.ip_panel()
+
+        other_section = ip.renderable.renderables[2]
+
+        # Table
+        table = other_section.renderables[1]
+        assert table.columns[1]._cells[-1] == Text(
+            "0 confidence score",
+            spans=[
+                Span(0, 1, theme.info),
+                Span(1, 18, "green"),
+            ]
+        )
+
+    def test_abuseipdb_yellow(self, view08, theme):
+        ip = view08.ip_panel()
+
+        other_section = ip.renderable.renderables[2]
+
+        # Table
+        table = other_section.renderables[1]
+        assert table.columns[1]._cells[-1] == Text(
+            "30 confidence score (567 reports)",
+            spans=[
+                Span(0, 2, theme.warn),
+                Span(2, 19, "yellow"),
+                Span(19, 33, theme.table_value),
+            ]
+        )
```

### Comparing `wtfis-0.8.0/tests/test_utils.py` & `wtfis-0.9.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/tests/test_data/ip2whois_whois_bbc.json` & `wtfis-0.9.0/tests/test_data/ip2whois_whois_bbc.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/tests/test_data/ip2whois_whois_hotmail.json` & `wtfis-0.9.0/tests/test_data/ip2whois_whois_hotmail.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/tests/test_data/ipwhois_1.1.1.1.json` & `wtfis-0.9.0/tests/test_data/ipwhois_1.1.1.1.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/tests/test_data/ipwhois_gist.json` & `wtfis-0.9.0/tests/test_data/ipwhois_gist.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/tests/test_data/pt_passive_dns_gist.json` & `wtfis-0.9.0/tests/test_data/pt_passive_dns_gist.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/tests/test_data/pt_whois_1.1.1.1.json` & `wtfis-0.9.0/tests/test_data/pt_whois_1.1.1.1.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/tests/test_data/pt_whois_gist.json` & `wtfis-0.9.0/tests/test_data/pt_whois_gist.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/tests/test_data/shodan_1.1.1.1.json` & `wtfis-0.9.0/tests/test_data/shodan_1.1.1.1.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/tests/test_data/shodan_gist.json` & `wtfis-0.9.0/tests/test_data/shodan_gist.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/tests/test_data/shodan_gist_2.json` & `wtfis-0.9.0/tests/test_data/shodan_gist_2.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/tests/test_data/shodan_one.json` & `wtfis-0.9.0/tests/test_data/shodan_one.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/tests/test_data/shodan_wired.json` & `wtfis-0.9.0/tests/test_data/shodan_wired.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/tests/test_data/urlhaus_1.1.1.1.json` & `wtfis-0.9.0/tests/test_data/urlhaus_1.1.1.1.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/tests/test_data/urlhaus_gist.json` & `wtfis-0.9.0/tests/test_data/urlhaus_gist.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/tests/test_data/vt_domain_gist.json` & `wtfis-0.9.0/tests/test_data/vt_domain_gist.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/tests/test_data/vt_domain_google.json` & `wtfis-0.9.0/tests/test_data/vt_domain_google.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/tests/test_data/vt_domain_tucows.json` & `wtfis-0.9.0/tests/test_data/vt_domain_tucows.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/tests/test_data/vt_ip_1.1.1.1.json` & `wtfis-0.9.0/tests/test_data/vt_ip_1.1.1.1.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/tests/test_data/vt_ip_142.251.220.110.json` & `wtfis-0.9.0/tests/test_data/vt_ip_142.251.220.110.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/tests/test_data/vt_resolutions_gist.json` & `wtfis-0.9.0/tests/test_data/vt_resolutions_gist.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/tests/test_data/vt_resolutions_one.json` & `wtfis-0.9.0/tests/test_data/vt_resolutions_one.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/tests/test_data/vt_resolutions_wired.json` & `wtfis-0.9.0/tests/test_data/vt_resolutions_wired.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/tests/test_data/vt_whois_1.1.1.1.json` & `wtfis-0.9.0/tests/test_data/vt_whois_1.1.1.1.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/tests/test_data/vt_whois_bbc.json` & `wtfis-0.9.0/tests/test_data/vt_whois_bbc.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/tests/test_data/vt_whois_example.json` & `wtfis-0.9.0/tests/test_data/vt_whois_example.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/tests/test_data/vt_whois_example_2.json` & `wtfis-0.9.0/tests/test_data/vt_whois_example_2.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/tests/test_data/vt_whois_gist.json` & `wtfis-0.9.0/tests/test_data/vt_whois_gist.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/wtfis/main.py` & `wtfis-0.9.0/wtfis/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from argparse import Namespace
 from dotenv import load_dotenv
 from pathlib import Path
 from rich.console import Console
 from rich.progress import Progress
 from typing import Union
+from wtfis.clients.abuseipdb import AbuseIpDbClient
 
 from wtfis.clients.greynoise import GreynoiseClient
 from wtfis.clients.ip2whois import Ip2WhoisClient
 from wtfis.clients.ipwhois import IpWhoisClient
 from wtfis.clients.passivetotal import PTClient
 from wtfis.clients.shodan import ShodanClient
 from wtfis.clients.urlhaus import UrlHausClient
@@ -52,14 +53,15 @@
         "-m", "--max-resolutions", metavar="N",
         help=f"Maximum number of resolutions to show (default: {DEFAULT_MAX_RESOLUTIONS})",
         type=int,
         default=DEFAULT_MAX_RESOLUTIONS
     )
     parser.add_argument("-s", "--use-shodan", help="Use Shodan to enrich IPs", action="store_true")
     parser.add_argument("-g", "--use-greynoise", help="Enable Greynoise for IPs", action="store_true")
+    parser.add_argument("-a", "--use-abuseipdb", help="Enable AbuseIPDB for IPs", action="store_true")
     parser.add_argument("-u", "--use-urlhaus", help="Enable URLhaus for IPs and domains", action="store_true")
     parser.add_argument("-n", "--no-color", help="Show output without colors", action="store_true")
     parser.add_argument("-1", "--one-column", help="Display results in one column", action="store_true")
     parser.add_argument(
         "-V", "--version",
         help="Print version number",
         action="version",
@@ -70,28 +72,32 @@
     # Default overrides
     # If a default is set, then setting the flag as an argument _negates_ the effect
     for option in os.environ.get("WTFIS_DEFAULTS", "").split(" "):
         if option in ("-s", "--use-shodan"):
             parsed.use_shodan = not parsed.use_shodan
         elif option in ("-g", "--use-greynoise"):
             parsed.use_greynoise = not parsed.use_greynoise
+        elif option in ("-a", "--use-abuseipdb"):
+            parsed.use_abuseipdb = not parsed.use_abuseipdb
         elif option in ("-u", "--use-urlhaus"):
             parsed.use_urlhaus = not parsed.use_urlhaus
         elif option in ("-n", "--no-color"):
             parsed.no_color = not parsed.no_color
         elif option in ("-1", "--one-column"):
             parsed.one_column = not parsed.one_column
 
     # Validation
     if parsed.max_resolutions > 10:
         argparse.ArgumentParser().error("Maximum --max-resolutions value is 10")
     if parsed.use_shodan and not os.environ.get("SHODAN_API_KEY"):
         argparse.ArgumentParser().error("SHODAN_API_KEY is not set")
     if parsed.use_greynoise and not os.environ.get("GREYNOISE_API_KEY"):
         argparse.ArgumentParser().error("GREYNOISE_API_KEY is not set")
+    if parsed.use_abuseipdb and not os.environ.get("ABUSEIPDB_API_KEY"):
+        argparse.ArgumentParser().error("ABUSEIPDB_API_KEY is not set")
     if is_ip(parsed.entity) and parsed.max_resolutions != DEFAULT_MAX_RESOLUTIONS:
         argparse.ArgumentParser().error("--max-resolutions is not applicable to IPs")
 
     return parsed
 
 
 def generate_entity_handler(
@@ -126,14 +132,20 @@
     # Greynoise client (optional)
     greynoise_client = (
         GreynoiseClient(os.environ["GREYNOISE_API_KEY"])
         if args.use_greynoise
         else None
     )
 
+    # AbuseIPDB client (optional)
+    abuseipdb_client = (
+        AbuseIpDbClient(os.environ["ABUSEIPDB_API_KEY"])
+        if args.use_abuseipdb else None
+    )
+
     # URLhaus client (optional)
     urlhaus_client = (
         UrlHausClient()
         if args.use_urlhaus
         else None
     )
 
@@ -143,27 +155,29 @@
             entity=args.entity,
             console=console,
             progress=progress,
             vt_client=vt_client,
             ip_enricher_client=enricher_client,
             whois_client=whois_client,
             greynoise_client=greynoise_client,
+            abuseipdb_client=abuseipdb_client,
             urlhaus_client=urlhaus_client,
             max_resolutions=args.max_resolutions,
         )
     # IP address handler
     else:
         entity = IpAddressHandler(
             entity=args.entity,
             console=console,
             progress=progress,
             vt_client=vt_client,
             ip_enricher_client=enricher_client,
             whois_client=whois_client,
             greynoise_client=greynoise_client,
+            abuseipdb_client=abuseipdb_client,
             urlhaus_client=urlhaus_client,
         )
 
     return entity
 
 
 def generate_view(
@@ -176,24 +190,26 @@
         view: BaseView = DomainView(
             console,
             entity.vt_info,
             entity.resolutions,
             entity.whois,
             entity.ip_enrich,
             entity.greynoise,
+            entity.abuseipdb,
             entity.urlhaus,
             max_resolutions=args.max_resolutions,
         )
     elif isinstance(entity, IpAddressHandler) and isinstance(entity.vt_info, IpAddress):
         view = IpAddressView(
             console,
             entity.vt_info,
             entity.whois,
             entity.ip_enrich,
             entity.greynoise,
+            entity.abuseipdb,
             entity.urlhaus,
         )
     else:
         raise Exception("Unsupported entity!")
 
     return view
```

### Comparing `wtfis-0.8.0/wtfis/utils.py` & `wtfis-0.9.0/wtfis/utils.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/wtfis/clients/base.py` & `wtfis-0.9.0/wtfis/clients/base.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/wtfis/clients/greynoise.py` & `wtfis-0.9.0/wtfis/clients/greynoise.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/wtfis/clients/ip2whois.py` & `wtfis-0.9.0/wtfis/clients/ip2whois.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/wtfis/clients/ipwhois.py` & `wtfis-0.9.0/wtfis/clients/ipwhois.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/wtfis/clients/passivetotal.py` & `wtfis-0.9.0/wtfis/clients/passivetotal.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/wtfis/clients/shodan.py` & `wtfis-0.9.0/wtfis/clients/shodan.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/wtfis/clients/urlhaus.py` & `wtfis-0.9.0/wtfis/clients/urlhaus.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/wtfis/clients/virustotal.py` & `wtfis-0.9.0/wtfis/clients/virustotal.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/wtfis/handlers/base.py` & `wtfis-0.9.0/wtfis/handlers/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,21 +9,23 @@
     Timeout,
 )
 from rich.console import Console
 from rich.progress import Progress
 from shodan.exception import APIError
 from typing import Callable, List, Optional, Union
 
+from wtfis.clients.abuseipdb import AbuseIpDbClient
 from wtfis.clients.greynoise import GreynoiseClient
 from wtfis.clients.ip2whois import Ip2WhoisClient
 from wtfis.clients.ipwhois import IpWhoisClient
 from wtfis.clients.passivetotal import PTClient
 from wtfis.clients.shodan import ShodanClient
 from wtfis.clients.urlhaus import UrlHausClient
 from wtfis.clients.virustotal import VTClient
+from wtfis.models.abuseipdb import AbuseIpDbMap
 from wtfis.models.common import WhoisBase
 from wtfis.models.greynoise import GreynoiseIpMap
 from wtfis.models.ipwhois import IpWhoisMap
 from wtfis.models.shodan import ShodanIpMap
 from wtfis.models.urlhaus import UrlHausMap
 from wtfis.models.virustotal import Domain, IpAddress
 from wtfis.ui.theme import Theme
@@ -66,34 +68,37 @@
         entity: str,
         console: Console,
         progress: Progress,
         vt_client: VTClient,
         ip_enricher_client: Union[IpWhoisClient, ShodanClient],
         whois_client: Union[Ip2WhoisClient, PTClient, VTClient],
         greynoise_client: Optional[GreynoiseClient],
+        abuseipdb_client: Optional[AbuseIpDbClient],
         urlhaus_client: Optional[UrlHausClient],
     ):
         # Process-specific
         self.entity = refang(entity)
         self.console = console
         self.progress = progress
 
         # Clients
         self._vt = vt_client
         self._enricher = ip_enricher_client
         self._whois = whois_client
         self._greynoise = greynoise_client
+        self._abuseipdb = abuseipdb_client
         self._urlhaus = urlhaus_client
 
         # Dataset containers
-        self.vt_info:   Union[Domain, IpAddress]
+        self.vt_info: Union[Domain, IpAddress]
         self.ip_enrich: Union[IpWhoisMap, ShodanIpMap] = IpWhoisMap.empty()
-        self.whois:     WhoisBase
+        self.whois: WhoisBase
         self.greynoise: GreynoiseIpMap = GreynoiseIpMap.empty()
-        self.urlhaus:  UrlHausMap = UrlHausMap.empty()
+        self.abuseipdb: AbuseIpDbMap = AbuseIpDbMap.empty()
+        self.urlhaus: UrlHausMap = UrlHausMap.empty()
 
         # Warning messages container
         self.warnings: List[str] = []
 
     @abc.abstractmethod
     def fetch_data(self) -> None:
         """ Main method that controls what get fetched """
@@ -107,14 +112,20 @@
     @common_exception_handler
     @failopen_exception_handler("_greynoise")
     def _fetch_greynoise(self, *ips: str) -> None:
         if self._greynoise:
             self.greynoise = self._greynoise.enrich_ips(*ips)
 
     @common_exception_handler
+    @failopen_exception_handler("_abuseipdb")
+    def _fetch_abuseipdb(self, *ips: str) -> None:
+        if self._abuseipdb:
+            self.abuseipdb = self._abuseipdb.enrich_ips(*ips)
+
+    @common_exception_handler
     def _fetch_whois(self) -> None:
         # Let continue if rate limited
         try:
             self.whois = self._whois.get_whois(self.entity)
         except HTTPError as e:
             if e.response.status_code == 429:
                 self.warnings.append(f"Could not fetch Whois: {e}")
```

### Comparing `wtfis-0.8.0/wtfis/handlers/domain.py` & `wtfis-0.9.0/wtfis/handlers/domain.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 """
 Logic handler for domain and hostname inputs
 """
+from typing import Optional, Union
+
 from requests.exceptions import HTTPError
 from rich.console import Console
 from rich.progress import Progress
-from typing import Optional, Union
 
+from wtfis.clients.abuseipdb import AbuseIpDbClient
 from wtfis.clients.greynoise import GreynoiseClient
 from wtfis.clients.ip2whois import Ip2WhoisClient
 from wtfis.clients.ipwhois import IpWhoisClient
 from wtfis.clients.passivetotal import PTClient
 from wtfis.clients.shodan import ShodanClient
 from wtfis.clients.urlhaus import UrlHausClient
 from wtfis.clients.virustotal import VTClient
+
 from wtfis.handlers.base import (
     BaseHandler,
     common_exception_handler,
     failopen_exception_handler,
 )
+
 from wtfis.models.virustotal import Resolutions
 
 
 class DomainHandler(BaseHandler):
     def __init__(
         self,
         entity: str,
         console: Console,
         progress: Progress,
         vt_client: VTClient,
         ip_enricher_client: Union[IpWhoisClient, ShodanClient],
         whois_client: Union[Ip2WhoisClient, PTClient, VTClient],
         greynoise_client: Optional[GreynoiseClient],
+        abuseipdb_client: Optional[AbuseIpDbClient],
         urlhaus_client: Optional[UrlHausClient],
         max_resolutions: int = 0,
     ):
         super().__init__(entity, console, progress, vt_client, ip_enricher_client,
-                         whois_client, greynoise_client, urlhaus_client)
+                         whois_client, greynoise_client, abuseipdb_client, urlhaus_client)
 
         # Extended attributes
         self.max_resolutions = max_resolutions
         self.resolutions: Optional[Resolutions] = None
 
     @common_exception_handler
     def _fetch_vt_domain(self) -> None:
@@ -79,14 +84,20 @@
 
             if self._greynoise:
                 task_g = self.progress.add_task(f"Fetching IP enrichments from {self._greynoise.name}")
                 self.progress.update(task_g, advance=50)
                 self._fetch_greynoise(*self.resolutions.ip_list(self.max_resolutions))
                 self.progress.update(task_g, completed=100)
 
+            if self._abuseipdb:
+                task_g = self.progress.add_task(f"Fetching IP enrichments from {self._abuseipdb.name}")
+                self.progress.update(task_g, advance=50)
+                self._fetch_abuseipdb(*self.resolutions.ip_list(self.max_resolutions))
+                self.progress.update(task_g, completed=100)
+
         if self._urlhaus:
             task_u = self.progress.add_task(f"Fetching domain enrichments from {self._urlhaus.name}")
             self.progress.update(task_u, advance=50)
             self._fetch_urlhaus()
             self.progress.update(task_u, completed=100)
 
         task_w = self.progress.add_task(f"Fetching domain whois from {self._whois.name}")
```

### Comparing `wtfis-0.8.0/wtfis/handlers/ip.py` & `wtfis-0.9.0/wtfis/handlers/ip.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,11 +38,17 @@
 
         if self._greynoise:
             task_g = self.progress.add_task(f"Fetching IP enrichments from {self._greynoise.name}")
             self.progress.update(task_g, advance=50)
             self._fetch_greynoise(self.entity)
             self.progress.update(task_g, completed=100)
 
+        if self._abuseipdb:
+            task_a = self.progress.add_task(f"Fetching IP enrichments from {self._abuseipdb.name}")
+            self.progress.update(task_a, advance=50)
+            self._fetch_abuseipdb(self.entity)
+            self.progress.update(task_a, completed=100)
+
         task_w = self.progress.add_task(f"Fetching IP whois from {self._whois.name}")
         self.progress.update(task_w, advance=50)
         self._fetch_whois()
         self.progress.update(task_w, completed=100)
```

### Comparing `wtfis-0.8.0/wtfis/models/common.py` & `wtfis-0.9.0/wtfis/models/common.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/wtfis/models/ip2whois.py` & `wtfis-0.9.0/wtfis/models/ip2whois.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/wtfis/models/ipwhois.py` & `wtfis-0.9.0/wtfis/models/ipwhois.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/wtfis/models/passivetotal.py` & `wtfis-0.9.0/wtfis/models/passivetotal.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/wtfis/models/shodan.py` & `wtfis-0.9.0/wtfis/models/shodan.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/wtfis/models/urlhaus.py` & `wtfis-0.9.0/wtfis/models/urlhaus.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/wtfis/models/virustotal.py` & `wtfis-0.9.0/wtfis/models/virustotal.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/wtfis/ui/base.py` & `wtfis-0.9.0/wtfis/ui/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     RenderableType,
     group,
 )
 from rich.panel import Panel
 from rich.table import Table
 from rich.text import Text
 from typing import Any, Generator, List, Optional, Tuple, Union
+from wtfis.models.abuseipdb import AbuseIpDb, AbuseIpDbMap
 
 from wtfis.models.common import WhoisBase
 from wtfis.models.greynoise import GreynoiseIp, GreynoiseIpMap
 from wtfis.models.ipwhois import IpWhois, IpWhoisMap
 from wtfis.models.shodan import ShodanIp, ShodanIpMap
 from wtfis.models.virustotal import (
     LastAnalysisStats,
@@ -36,21 +37,23 @@
     def __init__(
         self,
         console: Console,
         entity: Any,
         whois: Optional[WhoisBase],
         ip_enrich: Union[IpWhoisMap, ShodanIpMap],
         greynoise: GreynoiseIpMap,
+        abuseipdb: AbuseIpDbMap,
         urlhaus: UrlHausMap,
     ) -> None:
         self.console = console
         self.entity = entity
         self.whois = whois
         self.ip_enrich = ip_enrich
         self.greynoise = greynoise
+        self.abuseipdb = abuseipdb
         self.urlhaus = urlhaus
         self.theme = Theme()
 
     def _vendors_who_flagged_malicious(self) -> List[str]:
         vendors = []
         for key, result in self.entity.data.attributes.last_analysis_results.root.items():
             if result.category == "malicious":
@@ -65,15 +68,15 @@
         """
         link_style = f" link {hyperlink}" if hyperlink else ""
         if type == "h1":
             return Text(heading, style=f"{self.theme.heading_h1}{link_style}", justify="center")
         elif type == "h2":
             text = Text(justify="center")
             return text.append(heading, style=f"{self.theme.heading_h2}{link_style}")
-        else:
+        else:  # pragma: no cover
             raise Exception(f"Invalid heading type \"{type}\"")
 
     def _gen_linked_field_name(self, name: str, hyperlink: str) -> Text:
         text = Text(style=self.theme.table_field)
         text.append(name, style=f"link {hyperlink}")
         text.append(":")
         return text
@@ -107,22 +110,17 @@
         """ A section is a subset of a panel, with its own title and content """
         return Group(heading, body) if heading else body
 
     def _gen_panel(
         self,
         renderable: RenderableType,
         title: Optional[str] = None,
-        main_panel: bool = False
     ) -> Panel:
         if title is not None:
-            if main_panel is True:
-                title_style = self.theme.panel_title_main
-            else:  # Note to future self: we might not need two panel title styles anymore
-                title_style = self.theme.panel_title_default
-            panel_title = Text(title, style=title_style)
+            panel_title = Text(title, style=self.theme.panel_title)
             return Panel(renderable, title=panel_title, expand=False)
         return Panel(renderable, expand=False)
 
     def _gen_vt_analysis_stats(
         self,
         stats: LastAnalysisStats,
         vendors: Optional[List[str]] = None
@@ -252,33 +250,66 @@
             else:
                 (text
                  .append("? ")
                  .append(Text(ip.classification, style=text_style)))
 
         return title, text
 
+    def _gen_abuseipdb_tuple(self, ip: AbuseIpDb) -> Tuple[Text, Text]:
+
+        #
+        # Title
+        #
+        title = self._gen_linked_field_name("AbuseIPDB", hyperlink=f"https://www.abuseipdb.com/check/{ip.ip_address}")
+
+        #
+        # Content
+        #
+
+        if ip.abuse_confidence_score == 0:
+            style = self.theme.info
+        elif ip.abuse_confidence_score <= 30:
+            style = self.theme.warn
+        else:
+            style = self.theme.error
+
+        text = Text()
+        (text
+         .append(Text(str(ip.abuse_confidence_score), style=style))
+         .append(" confidence score", style=style.replace("bold ", "")))
+
+        if ip.abuse_confidence_score > 0:
+            text.append(f" ({ip.total_reports} reports)", style=self.theme.table_value)
+
+        return title, text
+
     def _gen_asn_text(
         self,
         asn: Optional[str],
         org: Optional[RenderableType],
     ) -> Optional[RenderableType]:
-        if not asn:
+        if asn == "0" or not asn:
             return None
 
-        text = Text(f"{asn.replace('AS', '')} (")
-        text.append(str(org), style=self.theme.asn_org)
-        text.append(")")
+        text = Text()
+        (text
+         .append(f"{asn.replace('AS', '')} (")
+         .append(str(org), style=self.theme.asn_org)
+         .append(")"))
         return text
 
     def _get_ip_enrichment(self, ip: str) -> Optional[Union[IpWhois, ShodanIp]]:
         return self.ip_enrich.root[ip] if ip in self.ip_enrich.root.keys() else None
 
     def _get_greynoise_enrichment(self, ip: str) -> Optional[GreynoiseIp]:
         return self.greynoise.root[ip] if ip in self.greynoise.root.keys() else None
 
+    def _get_abuseipdb_enrichment(self, ip: str) -> Optional[AbuseIpDb]:
+        return self.abuseipdb.root[ip] if ip in self.abuseipdb.root.keys() else None
+
     def _get_urlhaus_enrichment(self, entity: str) -> Optional[UrlHaus]:
         return self.urlhaus.root[entity] if entity in self.urlhaus.root.keys() else None
 
     def _gen_vt_section(self) -> RenderableType:
         """ Virustotal section. Applies to both domain and IP views """
         attributes = self.entity.data.attributes
         baseurl = self.vt_gui_baseurl_ip if is_ip(self.entity.data.id_) else self.vt_gui_baseurl_domain
@@ -381,40 +412,41 @@
             text = Text()
             if status == "not listed":
                 text.append(status, self.theme.urlhaus_bl_low)
             elif status.startswith("abused_"):
                 text.append(status, self.theme.urlhaus_bl_med)
             elif status.endswith("_domain") or status == "listed":
                 text.append(status, self.theme.urlhaus_bl_high)
-            else:
+            else:  # pragma: no cover
                 raise Exception(f"Invalid URLhaus BL status: {status}")
             text.append(" in ").append(blocklist, style=self.theme.urlhaus_bl_name)
             return text
 
         enrich = self._get_urlhaus_enrichment(self.entity.data.id_)
 
         data: List[Tuple[Union[str, Text], Union[RenderableType, None]]] = []
 
         if enrich:
             malware_urls_field: Union[Text, str] = self._gen_linked_field_name(
                 "Malware URLs",
                 hyperlink=enrich.urlhaus_reference,
             ) if enrich.urlhaus_reference else "Malware URLs:"
 
-            malware_urls_value = Text(
+            malware_urls_value = Text()
+            (malware_urls_value
+             .append(
                 (str(enrich.online_url_count)
-                 if enrich.url_count and enrich.url_count <= 100
-                 else f"{enrich.online_url_count}+") + " online",
+                    if enrich.url_count and enrich.url_count <= 100
+                    else f"{enrich.online_url_count}+") + " online",
                 style=self.theme.error if enrich.online_url_count > 0 else self.theme.warn,
-            )
-
-            malware_urls_value.append(
+             )
+             .append(
                 f" ({enrich.url_count} total)",
                 style=self.theme.table_value,
-            )
+             ))
 
             tags = smart_join(*enrich.tags, style=self.theme.tags) if enrich.tags else None
 
             data += [
                 (malware_urls_field, malware_urls_value),
                 (
                     "Blocklists:",
@@ -436,14 +468,19 @@
         data: List[Tuple[Union[str, Text], Union[RenderableType, None]]] = []
 
         # Greynoise
         greynoise = self._get_greynoise_enrichment(self.entity.data.id_)
         if greynoise:
             data.append(self._gen_greynoise_tuple(greynoise))
 
+        # abuseIPDB
+        abuseipdb = self._get_abuseipdb_enrichment(ip=self.entity.data.id_)
+        if abuseipdb:
+            data.append(self._gen_abuseipdb_tuple(abuseipdb))
+
         if data:
             return self._gen_section(
                 self._gen_table(*data),
                 self._gen_heading_text("Other")
             )
 
         return None  # No other data
```

### Comparing `wtfis-0.8.0/wtfis/ui/theme.py` & `wtfis-0.9.0/wtfis/ui/theme.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 class Theme:
-    panel_title_default = "default"
-    panel_title_main = "bold yellow"
+    panel_title = "bold yellow"
     heading_h1 = "bold bright_green on dark_green"
     heading_h2 = "bold yellow"
     table_field = "bold bright_magenta"
     table_value = "not bold default"
     popularity_source = "bright_cyan"
     inline_stat = "cyan"
     vendor_list = "cyan"
```

### Comparing `wtfis-0.8.0/wtfis/ui/view.py` & `wtfis-0.9.0/wtfis/ui/view.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     Group,
     RenderableType,
 )
 from rich.padding import Padding
 from rich.panel import Panel
 from rich.text import Text
 from typing import List, Optional, Tuple, Union
+from wtfis.models.abuseipdb import AbuseIpDbMap
 
 from wtfis.models.common import WhoisBase
 from wtfis.models.greynoise import GreynoiseIpMap
 from wtfis.models.ipwhois import IpWhois, IpWhoisMap
 from wtfis.models.shodan import ShodanIpMap
 from wtfis.models.urlhaus import UrlHausMap
 from wtfis.models.virustotal import (
@@ -23,39 +24,42 @@
 from wtfis.utils import Timestamp, smart_join
 
 
 class DomainView(BaseView):
     """
     Handler for FQDN and domain lookup output
     """
+
     def __init__(
         self,
         console: Console,
         entity: Domain,
         resolutions: Optional[Resolutions],
         whois: WhoisBase,
         ip_enrich: Union[IpWhoisMap, ShodanIpMap],
         greynoise: GreynoiseIpMap,
+        abuseipdb: AbuseIpDbMap,
         urlhaus: UrlHausMap,
         max_resolutions: int = 3,
     ) -> None:
-        super().__init__(console, entity, whois, ip_enrich, greynoise, urlhaus)
+        super().__init__(console, entity, whois, ip_enrich, greynoise, abuseipdb, urlhaus)
+
         self.resolutions = resolutions
         self.max_resolutions = max_resolutions
 
     def domain_panel(self) -> Panel:
         content = [self._gen_vt_section()]  # VT section
         for section in (
             self._gen_urlhaus_section(),    # URLhaus section
         ):
             if section is not None:
                 content.append("")
                 content.append(section)
 
-        return self._gen_panel(self._gen_group(content), self.entity.data.id_, main_panel=True)
+        return self._gen_panel(self._gen_group(content), self.entity.data.id_)
 
     def resolutions_panel(self) -> Optional[Panel]:
         # Skip if no resolutions data
         if not self.resolutions:
             return None
 
         content: List[RenderableType] = [self._gen_heading_text("Resolutions")]
@@ -116,14 +120,19 @@
 
             # Greynoise
             greynoise = self._get_greynoise_enrichment(attributes.ip_address)
 
             if greynoise:
                 data += [self._gen_greynoise_tuple(greynoise)]
 
+            # AbuseIPDB
+            abuseipdb = self._get_abuseipdb_enrichment(attributes.ip_address)
+            if abuseipdb:
+                data += [self._gen_abuseipdb_tuple(abuseipdb)]
+
             # Include a disclaimer if last seen is older than 1 year
             # Note: Disabled for now because I originally understood that the resolution date was the last time
             # the domain was resolved, but it may actually be he first time the IP itself was seen with the domain.
             # if enrich and older_than(attributes.date, 365):
             #     body = Group(
             #         self._gen_table(*data),
             #         Text("**Enrichment data may be inaccurate", style=self.theme.disclaimer),
@@ -172,37 +181,39 @@
             self.console.print(Padding(Columns(renderables), (1, 0)))
 
 
 class IpAddressView(BaseView):
     """
     Handler for IP Address lookup output
     """
+
     def __init__(
         self,
         console: Console,
         entity: IpAddress,
         whois: WhoisBase,
         ip_enrich: Union[IpWhoisMap, ShodanIpMap],
         greynoise: GreynoiseIpMap,
+        abuseipdb: AbuseIpDbMap,
         urlhaus: UrlHausMap,
     ) -> None:
-        super().__init__(console, entity, whois, ip_enrich, greynoise, urlhaus)
+        super().__init__(console, entity, whois, ip_enrich, greynoise, abuseipdb, urlhaus)
 
     def ip_panel(self) -> Panel:
         content = [self._gen_vt_section()]  # VT section
         for section in (
             self._gen_ip_enrich_section(),  # IP enrich section
             self._gen_urlhaus_section(),    # URLhaus section
             self._gen_ip_other_section(),   # Other section
         ):
             if section is not None:
                 content.append("")
                 content.append(section)
 
-        return self._gen_panel(self._gen_group(content), self.entity.data.id_, main_panel=True)
+        return self._gen_panel(self._gen_group(content), self.entity.data.id_)
 
     def print(self, one_column: bool = False) -> None:
         renderables = [i for i in (
             self.ip_panel(),
             self.whois_panel(),
         ) if i is not None]
```

### Comparing `wtfis-0.8.0/.gitignore` & `wtfis-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/LICENSE` & `wtfis-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/README.md` & `wtfis-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 | [Virustotal](https://virustotal.com) | All | Yes | [Yes](https://www.virustotal.com/gui/join-us) |
 | [Passivetotal](https://community.riskiq.com) | All | No | [Yes](https://community.riskiq.com/registration/)
 | [IP2Whois](https://www.ip2whois.com) | Domain/FQDN | No | [Yes](https://www.ip2location.io/pricing#ip2whois)
 | [IPWhois](https://ipwhois.io) | IP address | No | Yes (no signup) |
 | [Shodan](https://shodan.io) | IP address | No | [No](https://account.shodan.io/billing) |
 | [Greynoise](https://greynoise.io) | IP address | No | [Yes](https://www.greynoise.io/plans/community)
 | [URLhaus](https://urlhaus.abuse.ch/) | All | No | Yes (no signup)
+| [AbuseIPDB](https://www.abuseipdb.com/)| IP address | No | [Yes](https://www.abuseipdb.com/register?plan=free)
 
 ### Virustotal
 
 The primary source of information. Retrieves:
 
 * [Hostname (FQDN), domain or IP](https://developers.virustotal.com/reference/domains-1)
     * Latest analysis stats with vendor detail
@@ -67,32 +68,32 @@
 * [Whois](https://www.ip2location.io/ip2whois-documentation)
     * Various whois data about the domain itself
 
 As above, IP2Whois is recommended over Virustotal if a Passivetotal account cannot be obtained.
 
 ### IPWhois
 
-Default enrichment for IP addresses. Retrieves:
+Default Geolocation and ASN lookup source for IP addresses. Retrieves:
 
 * ASN, Org, ISP and Geolocation
 
 IPWhois should not be confused with IP2Whois, which provides domain Whois data.
 
 ### Shodan
 
-Alternative IP address enrichment source. GETs data from the `/shodan/host/{ip}` endpoint (see [doc](https://developer.shodan.io/api)). For each IP, retrieves:
+GETs data from the `/shodan/host/{ip}` endpoint (see [doc](https://developer.shodan.io/api)). For each IP, retrieves:
 
 * ASN, Org, ISP and Geolocation
 * List of open ports and services
 * Operating system (if available)
 * Tags (assigned by Shodan)
 
 ### Greynoise
 
-Supplementary IP address enrichment source. Using its [community API](https://docs.greynoise.io/docs/using-the-greynoise-community-api), wtfis will show whether an IP is in one of Greynoise's datasets:
+Using Greynoise's [community API](https://docs.greynoise.io/docs/using-the-greynoise-community-api), wtfis will show whether an IP is in one of Greynoise's datasets:
 
 * **Noise**: IP has been seen regularly scanning the Internet
 * **RIOT**: IP belongs to a common business application (e.g. Microsoft O365, Google Workspace, Slack)
 
 More information about the datasets [here](https://docs.greynoise.io/docs/understanding-greynoise-data-sets).
 
 In addition, the API also returns Greynoise's [classification](https://docs.greynoise.io/docs/understanding-greynoise-classifications) of an IP (if available). Possible values are **benign**, **malicious**, and **unknown**.
@@ -101,59 +102,69 @@
 
 [URLhaus](https://urlhaus.abuse.ch/) is a crowd-sourced database of reported malicious URLs. This enrichment provides insight on whether the queried hostname or IP is being or was used for malware distribution via HTTP or HTTPS. Data that is provided include:
 
 * Count of currently online and total malware URLs
 * Whether the hostname or IP is currently in the [DNSBL](https://www.dnsbl.info/) and [SURBL](https://www.surbl.org/) public blocklists
 * All tags that have been assigned to the URL throughout its history in the URLhaus database
 
+### AbuseIPDB
+
+[AbuseIPDB](https://www.abuseipdb.com/) is a crowd-sourced database of reported malicious IP addresses. Through its API wtfis shows:
+
+* Abuse confidence score (0-100)
+* Number of reports
+
 
 ## Install
 
 ```
 $ pip install wtfis
 ```
 
 To install via `conda` (from conda-forge), see [wtfis-feedstock](https://github.com/conda-forge/wtfis-feedstock).
 
 To install via [`brew`](https://brew.sh):
+
 ```
 brew install wtfis
 ```
 
 ## Setup
 
 wtfis uses these environment variables:
 
 * `VT_API_KEY` (required) - Virustotal API key
 * `PT_API_KEY` (optional) - Passivetotal API key
 * `PT_API_USER` (optional) - Passivetotal API user
 * `IP2WHOIS_API_KEY` (optional) - IP2WHOIS API key
 * `SHODAN_API_KEY` (optional) - Shodan API key
 * `GREYNOISE_API_KEY` (optional) - Greynoise API key
+* `ABUSEIPDB_API_KEY` (optional) - AbuseIPDB API key
 * `WTFIS_DEFAULTS` (optional) - Default arguments
 
 Set these using your own method.
 
 Alternatively, create a file in your home directory `~/.env.wtfis` with the above declarations. See [.env.wtfis.example](./.env.wtfis.example) for a template. **NOTE: Don't forget to `chmod 400` the file!**
 
 
 ## Usage
 
 ```
-usage: wtfis [-h] [-m N] [-s] [-g] [-u] [-n] [-1] [-V] entity
+usage: wtfis [-h] [-m N] [-s] [-g] [-a] [-u] [-n] [-1] [-V] entity
 
 positional arguments:
   entity                Hostname, domain or IP
 
-options:
+optional arguments:
   -h, --help            show this help message and exit
   -m N, --max-resolutions N
                         Maximum number of resolutions to show (default: 3)
   -s, --use-shodan      Use Shodan to enrich IPs
   -g, --use-greynoise   Enable Greynoise for IPs
+  -a, --use-abuseipdb   Enable AbuseIPDB for IPs
   -u, --use-urlhaus     Enable URLhaus for IPs and domains
   -n, --no-color        Show output without colors
   -1, --one-column      Display results in one column
   -V, --version         Print version number
 ```
 
 Basically:
@@ -164,38 +175,46 @@
 
 and you will get results organized by panel, similar to the image above.
 
 Defanged input is accepted (e.g. `api[.]google[.]com`).
 
 If supported by the terminal, the `Analysis` field and (if using PT) headings in the whois panel are clickable hyperlinks that point to the appropriate pages on the VT or PT website.
 
-### Shodan enrichment
+### Shodan
 
 Shodan can be used to enrich the IP addresses (instead of IPWhois). Invoke with the `-s` or `--use-shodan` flag.
 
 ![](https://github.com/pirxthepilot/wtfis/blob/main/imgs/example-shodan.png?raw=true)
 
 If supported by the terminal, the `Services` field is a clickable hyperlink that takes you to the Shodan web interface.
 
-### Greynoise enrichment
+### Greynoise
 
 To enable Greynoise, invoke with the `-g` or `--use-greynoise` flag. Because the API quota is quite low (50 requests per week as of March 2023), this lookup is off by default.
 
 ![](https://github.com/pirxthepilot/wtfis/blob/main/imgs/example-greynoise.png?raw=true)
 
 The `GreyNoise` field name is also a hyperlink (if terminal-supported) that points to the IP entry in the Greynoise web interface, where more context is shown.
 
-### URLhaus enrichment
+### URLhaus
 
 Use the `-u` or `--use-urlhaus` flag to enable URLhaus enrichment for hostnames, domains and IPs.
 
 ![](https://github.com/pirxthepilot/wtfis/blob/main/imgs/example-urlhaus.png?raw=true)
 
 The `Malware URLs` field name is a hyperlink (if terminal-supported) that takes you to the specific URLhaus database page for your query.
 
+### AbuseIPDB
+
+Use the `-a` or `--use-abuseipdb` flag to enable AbuseIPDB enrichment for hostnames, domains and IPs.
+
+![](https://github.com/pirxthepilot/wtfis/blob/main/imgs/example-abuseipdb.png?raw=true)
+
+The `AbuseIPDB` field name is a hyperlink (if terminal-supported) that takes you to the specific AbuseIPDB database page for your query.
+
 ### Display options
 
 For FQDN and domain lookups, you can increase or decrease the maximum number of displayed IP resolutions with `-m NUMBER` or `--max-resolutions=NUMBER`. The upper limit is 10. If you don't need resolutions at all, set the number to `0`.
 
 To show all panels in one column, use the `-1` or `--one-column` flag.
 
 ![](https://github.com/pirxthepilot/wtfis/blob/main/imgs/example-one-column.png?raw=true)
```

### Comparing `wtfis-0.8.0/pyproject.toml` & `wtfis-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wtfis-0.8.0/PKG-INFO` & `wtfis-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: wtfis
-Version: 0.8.0
+Version: 0.9.0
 Summary: Passive hostname, domain and IP lookup tool for non-robots
 Project-URL: Homepage, https://github.com/pirxthepilot/wtfis
 Author-email: pirxthepilot <pirxthepilot@users.noreply.github.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: ipinfo,osint,passive lookup,passivetotal,security,shodan,virustotal,whois
 Classifier: Development Status :: 4 - Beta
@@ -48,14 +48,15 @@
 | [Virustotal](https://virustotal.com) | All | Yes | [Yes](https://www.virustotal.com/gui/join-us) |
 | [Passivetotal](https://community.riskiq.com) | All | No | [Yes](https://community.riskiq.com/registration/)
 | [IP2Whois](https://www.ip2whois.com) | Domain/FQDN | No | [Yes](https://www.ip2location.io/pricing#ip2whois)
 | [IPWhois](https://ipwhois.io) | IP address | No | Yes (no signup) |
 | [Shodan](https://shodan.io) | IP address | No | [No](https://account.shodan.io/billing) |
 | [Greynoise](https://greynoise.io) | IP address | No | [Yes](https://www.greynoise.io/plans/community)
 | [URLhaus](https://urlhaus.abuse.ch/) | All | No | Yes (no signup)
+| [AbuseIPDB](https://www.abuseipdb.com/)| IP address | No | [Yes](https://www.abuseipdb.com/register?plan=free)
 
 ### Virustotal
 
 The primary source of information. Retrieves:
 
 * [Hostname (FQDN), domain or IP](https://developers.virustotal.com/reference/domains-1)
     * Latest analysis stats with vendor detail
@@ -89,32 +90,32 @@
 * [Whois](https://www.ip2location.io/ip2whois-documentation)
     * Various whois data about the domain itself
 
 As above, IP2Whois is recommended over Virustotal if a Passivetotal account cannot be obtained.
 
 ### IPWhois
 
-Default enrichment for IP addresses. Retrieves:
+Default Geolocation and ASN lookup source for IP addresses. Retrieves:
 
 * ASN, Org, ISP and Geolocation
 
 IPWhois should not be confused with IP2Whois, which provides domain Whois data.
 
 ### Shodan
 
-Alternative IP address enrichment source. GETs data from the `/shodan/host/{ip}` endpoint (see [doc](https://developer.shodan.io/api)). For each IP, retrieves:
+GETs data from the `/shodan/host/{ip}` endpoint (see [doc](https://developer.shodan.io/api)). For each IP, retrieves:
 
 * ASN, Org, ISP and Geolocation
 * List of open ports and services
 * Operating system (if available)
 * Tags (assigned by Shodan)
 
 ### Greynoise
 
-Supplementary IP address enrichment source. Using its [community API](https://docs.greynoise.io/docs/using-the-greynoise-community-api), wtfis will show whether an IP is in one of Greynoise's datasets:
+Using Greynoise's [community API](https://docs.greynoise.io/docs/using-the-greynoise-community-api), wtfis will show whether an IP is in one of Greynoise's datasets:
 
 * **Noise**: IP has been seen regularly scanning the Internet
 * **RIOT**: IP belongs to a common business application (e.g. Microsoft O365, Google Workspace, Slack)
 
 More information about the datasets [here](https://docs.greynoise.io/docs/understanding-greynoise-data-sets).
 
 In addition, the API also returns Greynoise's [classification](https://docs.greynoise.io/docs/understanding-greynoise-classifications) of an IP (if available). Possible values are **benign**, **malicious**, and **unknown**.
@@ -123,59 +124,69 @@
 
 [URLhaus](https://urlhaus.abuse.ch/) is a crowd-sourced database of reported malicious URLs. This enrichment provides insight on whether the queried hostname or IP is being or was used for malware distribution via HTTP or HTTPS. Data that is provided include:
 
 * Count of currently online and total malware URLs
 * Whether the hostname or IP is currently in the [DNSBL](https://www.dnsbl.info/) and [SURBL](https://www.surbl.org/) public blocklists
 * All tags that have been assigned to the URL throughout its history in the URLhaus database
 
+### AbuseIPDB
+
+[AbuseIPDB](https://www.abuseipdb.com/) is a crowd-sourced database of reported malicious IP addresses. Through its API wtfis shows:
+
+* Abuse confidence score (0-100)
+* Number of reports
+
 
 ## Install
 
 ```
 $ pip install wtfis
 ```
 
 To install via `conda` (from conda-forge), see [wtfis-feedstock](https://github.com/conda-forge/wtfis-feedstock).
 
 To install via [`brew`](https://brew.sh):
+
 ```
 brew install wtfis
 ```
 
 ## Setup
 
 wtfis uses these environment variables:
 
 * `VT_API_KEY` (required) - Virustotal API key
 * `PT_API_KEY` (optional) - Passivetotal API key
 * `PT_API_USER` (optional) - Passivetotal API user
 * `IP2WHOIS_API_KEY` (optional) - IP2WHOIS API key
 * `SHODAN_API_KEY` (optional) - Shodan API key
 * `GREYNOISE_API_KEY` (optional) - Greynoise API key
+* `ABUSEIPDB_API_KEY` (optional) - AbuseIPDB API key
 * `WTFIS_DEFAULTS` (optional) - Default arguments
 
 Set these using your own method.
 
 Alternatively, create a file in your home directory `~/.env.wtfis` with the above declarations. See [.env.wtfis.example](./.env.wtfis.example) for a template. **NOTE: Don't forget to `chmod 400` the file!**
 
 
 ## Usage
 
 ```
-usage: wtfis [-h] [-m N] [-s] [-g] [-u] [-n] [-1] [-V] entity
+usage: wtfis [-h] [-m N] [-s] [-g] [-a] [-u] [-n] [-1] [-V] entity
 
 positional arguments:
   entity                Hostname, domain or IP
 
-options:
+optional arguments:
   -h, --help            show this help message and exit
   -m N, --max-resolutions N
                         Maximum number of resolutions to show (default: 3)
   -s, --use-shodan      Use Shodan to enrich IPs
   -g, --use-greynoise   Enable Greynoise for IPs
+  -a, --use-abuseipdb   Enable AbuseIPDB for IPs
   -u, --use-urlhaus     Enable URLhaus for IPs and domains
   -n, --no-color        Show output without colors
   -1, --one-column      Display results in one column
   -V, --version         Print version number
 ```
 
 Basically:
@@ -186,38 +197,46 @@
 
 and you will get results organized by panel, similar to the image above.
 
 Defanged input is accepted (e.g. `api[.]google[.]com`).
 
 If supported by the terminal, the `Analysis` field and (if using PT) headings in the whois panel are clickable hyperlinks that point to the appropriate pages on the VT or PT website.
 
-### Shodan enrichment
+### Shodan
 
 Shodan can be used to enrich the IP addresses (instead of IPWhois). Invoke with the `-s` or `--use-shodan` flag.
 
 ![](https://github.com/pirxthepilot/wtfis/blob/main/imgs/example-shodan.png?raw=true)
 
 If supported by the terminal, the `Services` field is a clickable hyperlink that takes you to the Shodan web interface.
 
-### Greynoise enrichment
+### Greynoise
 
 To enable Greynoise, invoke with the `-g` or `--use-greynoise` flag. Because the API quota is quite low (50 requests per week as of March 2023), this lookup is off by default.
 
 ![](https://github.com/pirxthepilot/wtfis/blob/main/imgs/example-greynoise.png?raw=true)
 
 The `GreyNoise` field name is also a hyperlink (if terminal-supported) that points to the IP entry in the Greynoise web interface, where more context is shown.
 
-### URLhaus enrichment
+### URLhaus
 
 Use the `-u` or `--use-urlhaus` flag to enable URLhaus enrichment for hostnames, domains and IPs.
 
 ![](https://github.com/pirxthepilot/wtfis/blob/main/imgs/example-urlhaus.png?raw=true)
 
 The `Malware URLs` field name is a hyperlink (if terminal-supported) that takes you to the specific URLhaus database page for your query.
 
+### AbuseIPDB
+
+Use the `-a` or `--use-abuseipdb` flag to enable AbuseIPDB enrichment for hostnames, domains and IPs.
+
+![](https://github.com/pirxthepilot/wtfis/blob/main/imgs/example-abuseipdb.png?raw=true)
+
+The `AbuseIPDB` field name is a hyperlink (if terminal-supported) that takes you to the specific AbuseIPDB database page for your query.
+
 ### Display options
 
 For FQDN and domain lookups, you can increase or decrease the maximum number of displayed IP resolutions with `-m NUMBER` or `--max-resolutions=NUMBER`. The upper limit is 10. If you don't need resolutions at all, set the number to `0`.
 
 To show all panels in one column, use the `-1` or `--one-column` flag.
 
 ![](https://github.com/pirxthepilot/wtfis/blob/main/imgs/example-one-column.png?raw=true)
```

