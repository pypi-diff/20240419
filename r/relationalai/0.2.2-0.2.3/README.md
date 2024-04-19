# Comparing `tmp/relationalai-0.2.2.tar.gz` & `tmp/relationalai-0.2.3.tar.gz`

## Comparing `relationalai-0.2.2.tar` & `relationalai-0.2.3.tar`

### file list

```diff
@@ -1,361 +1,429 @@
--rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 relationalai-0.2.2/README.md
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 relationalai-0.2.2/.github/actions/end-to-end/action.yml
--rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 relationalai-0.2.2/.github/workflows/end-to-end.yml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 relationalai-0.2.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 relationalai-0.2.2/.github/workflows/ruff.yml
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/README.md
--rw-r--r--   0        0        0    17337 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/getting_started.md
--rw-r--r--   0        0        0     9875 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/_old/OLD_pyrel_quickstart.md
--rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/_old/metamodel.md
--rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/_old/python_dsl.md
--rw-r--r--   0        0        0     9371 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/_old/quickstart.md
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/README.md
--rw-r--r--   0        0        0    13377 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/cli/README.md
--rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/configuration/README.md
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Expression.md
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Property.md
--rw-r--r--   0        0        0     6050 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/README.md
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Context/README.md
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Context/enter__.md
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Context/exit__.md
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Context/iter__.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Context/model.md
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Context/results.md
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/ContextSelect/README.md
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/ContextSelect/add.md
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/ContextSelect/call__.md
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/ContextSelect/getattribute__.md
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Instance/README.md
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Instance/persist.md
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Instance/set.md
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Instance/unpersist.md
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/InstanceProperty/README.md
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/InstanceProperty/or_.md
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Model/README.md
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Model/Type.md
--rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Model/found.md
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Model/name.md
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Model/not_found.md
--rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Model/ordered_choice.md
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Model/query.md
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Model/read.md
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Model/rule.md
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Model/scope.md
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Model/union.md
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/README.md
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/add__.md
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/enter__.md
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/eq__.md
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/exit__.md
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/ge__.md
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/getattribute__.md
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/gt__.md
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/le__.md
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/lt__.md
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/mul__.md
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/ne__.md
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/pow__.md
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/radd__.md
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/rmul__.md
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/rpow__.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/rsub__.md
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/rtruediv__.md
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/sub__.md
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/truediv__.md
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Type/README.md
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Type/add.md
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Type/call__.md
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Type/model.md
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Type/name.md
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Type/or__.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/clients/README.md
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/clients/snowflake/PrimaryKey.md
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/clients/snowflake/README.md
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/clients/snowflake/Snowflake.md
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/README.md
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/Vars.md
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/alias.md
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/aggregates/README.md
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/aggregates/avg.md
--rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/aggregates/count.md
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/aggregates/max.md
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/aggregates/min.md
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/aggregates/rank_asc.md
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/aggregates/rank_desc.md
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/aggregates/sum.md
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/README.md
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/README.md
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md
--rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/degree.md
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/degree_centrality.md
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/indegree.md
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/infomap.md
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/label_propagation.md
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/louvain.md
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/outdegree.md
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/pagerank.md
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Edges/README.md
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Edges/add.md
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Edges/extend.md
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/README.md
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/compute.md
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/edges.md
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/fetch.md
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/id.md
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/model.md
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/nodes.md
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/undirected.md
--rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/visualize.md
--rw-r--r--   0        0        0    20679 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png
--rw-r--r--   0        0        0    15558 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png
--rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Nodes/README.md
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Nodes/add.md
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Nodes/extend.md
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/sql/README.md
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/README.md
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/cdc.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/emit_playground.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/found.py
--rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/fraud.ipynb
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/fraud.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/graph_algos.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/load_raw.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/nested.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/or_types.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/remote_load_csv.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/requirements.txt
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/simple.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/simple_recursion.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/simple_streamlit.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/solver.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/weighted_graph_algos.py
--rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/data/people.csv
--rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/data/transactions.csv
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/ev_penetration/ev_penetration.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/ev_penetration/ev_penetration_csv.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/ev_penetration/state_stats.csv
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/imdb/README.md
--rw-r--r--   0        0        0   787694 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/imdb/imdb.csv
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/imdb/imdb.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/rel/bar.rel
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/rel/foo.rel
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/rel/solver.rel
--rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/social-money-network/SF_pagerank.ipynb
--rw-r--r--   0        0        0  2419367 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/social-money-network/Simulation-and-SF-Upload.ipynb
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/social-money-network/snowflake_pagerank.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/.gitignore
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/README.md
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/index.html
--rw-r--r--   0        0        0   454881 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/package-lock.json
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/package.json
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/tsconfig.json
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/vite.config.ts
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/.storybook/main.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/.storybook/preview-body.html
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/.storybook/preview-head.html
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/.storybook/preview.ts
--rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/App.tsx
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/app.styl
--rw-r--r--   0        0        0     5496 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/debugger_client.ts
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/index.css
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/index.tsx
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/logo.svg
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/util.styl
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/ws.ts
--rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/assets/favicon.ico
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Button.styl
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Button.tsx
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Field.stories.tsx
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Field.styl
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Field.tsx
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Modal.stories.tsx
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Modal.styl
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Modal.tsx
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Sidebar.styl
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Sidebar.tsx
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Tooltip.stories.tsx
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Tooltip.styl
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Tooltip.tsx
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx
--rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/ScopeProvider.tsx
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/index.stories.tsx
--rw-r--r--   0        0        0     4724 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/index.styl
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/index.tsx
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/ComputeNode.tsx
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/FilterNode.tsx
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/UnknownNode.tsx
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/base.styl
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/base.tsx
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/index.tsx
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/fixtures/branch-improved.json
--rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/fixtures/branch.json
--rw-r--r--   0        0        0    67308 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/fixtures/fraud.json
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/fixtures/index.ts
--rw-r--r--   0        0        0     9536 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/fixtures/not_found.json
--rw-r--r--   0        0        0     6685 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/fixtures/simple.json
--rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/fixtures/union.json
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/types/json.d.ts
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/types/jsx.d.ts
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/types/mech.d.ts
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/__init__.py
--rw-r--r--   0        0        0    12329 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/emit.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/exec.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/fixtures.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/patch.py
--rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/util.py
--rwxr-xr-x   0        0        0     3521 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/cli/__main__.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/cli/collect_failures.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/cli/collect_tests.py
--rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/cli/repro.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/cli/run_tests.py
--rw-r--r--   0        0        0    15710 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/cli/watch.py
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/gen/action.py
--rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/gen/context.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/gen/document.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/gen/error.py
--rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/gen/group_limited.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/gen/ir.py
--rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/gen/scope.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/gen/staged.py
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/gen/task.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/gen/test.py
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/harness/database.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/harness/vendor_types.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/validate/diff.py
--rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/validate/errors.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/validate/mapping.py
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/validate/roundtrip.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/__init__.py
--rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/compiler.py
--rw-r--r--   0        0        0     9991 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/debugging.py
--rw-r--r--   0        0        0    44677 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/dsl.py
--rw-r--r--   0        0        0    12279 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/errors.py
--rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/metagen.py
--rw-r--r--   0        0        0    27821 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/metamodel.py
--rw-r--r--   0        0        0    18690 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/rel.py
--rw-r--r--   0        0        0    20453 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/rel2.py
--rw-r--r--   0        0        0    12998 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/rel_emitter.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/rel_utils.py
--rw-r--r--   0        0        0     8570 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/analysis/mechanistic.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/analysis/whynot.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/clients/__init__.py
--rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/clients/azure.py
--rw-r--r--   0        0        0    10135 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/clients/client.py
--rw-r--r--   0        0        0    17646 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/clients/config.py
--rw-r--r--   0        0        0    32470 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/clients/snowflake.py
--rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/clients/test.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/clients/types.py
--rw-r--r--   0        0        0     7366 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/loaders/csv.py
--rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/loaders/loader.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/loaders/types.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/std/__init__.py
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/std/aggregates.py
--rw-r--r--   0        0        0    13750 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/std/graphs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/tools/__init__.py
--rw-r--r--   0        0        0    51381 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/tools/cli.py
--rw-r--r--   0        0        0    10318 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/tools/cli_controls.py
--rw-r--r--   0        0        0     6804 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/tools/debugger.py
--rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/tools/debugger_server.py
--rw-r--r--   0        0        0     9121 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/tools/dev.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/tools/notes
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/conftest.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/README.md
--rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/conftest.py
--rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_graph_visualize.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_snapshots.py
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/agg_ordering/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query0.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query1.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/bottom/query0.txt
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/cosine_similarity/query0.txt
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/eigenvector_centrality/query0.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/first/query0.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/indegree/query0.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/indegree/query1.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/infomap/query0.txt
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/jaccard_similarity/query0.txt
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/jaccard_similarity/query1.txt
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/louvain/query0.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query0.txt
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query1.txt
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query3.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query4.txt
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query0.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query1.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/outdegree/query0.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/outdegree/query1.txt
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/page_rank/query0.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query0.txt
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query1.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query2.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query3.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query0.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query1.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/top/query0.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query0.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query1.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query2.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query3.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query4.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query5.txt
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/agg_ordering.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/bool.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/bottom.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/cosine_similarity.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/eigenvector_centrality.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/export.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/first.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/indegree.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/infomap.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/jaccard_similarity.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/louvain.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/multi_valued.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/not_found.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/outdegree.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/page_rank.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/persist.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/smoke.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/top.py
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/weighted_graphs.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/execution/test_core.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/execution/test_examples.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/execution/basic/smoketest.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/execution/snapshots/test_core/test_basic/smoketest/query0.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/execution/snapshots/test_examples/test_example/emit_playground/query0.txt
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/execution/snapshots/test_examples/test_example/found/query0.txt
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/execution/snapshots/test_examples/test_example/graph/query0.txt
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/execution/snapshots/test_examples/test_example/graph/query1.txt
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/execution/snapshots/test_examples/test_example/load_raw/query0.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/execution/snapshots/test_examples/test_example/or_types/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/execution/snapshots/test_examples/test_example/simple/query0.txt
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/execution/snapshots/test_examples/test_example/simple_recursion/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/execution/snapshots/test_examples/test_example/simple_streamlit/query0.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/execution/snapshots/test_examples/test_example/test/query0.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/init-cli/__init__.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/init-cli/azure_basic.py
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/init-cli/common.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/roundtrip/test_document.py
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/roundtrip/test_task.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 relationalai-0.2.2/.gitignore
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 relationalai-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/pypi/README.md
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 relationalai-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 relationalai-0.2.3/README.md
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 relationalai-0.2.3/.github/actions/end-to-end/action.yml
+-rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 relationalai-0.2.3/.github/workflows/end-to-end.yml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 relationalai-0.2.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 relationalai-0.2.3/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/README.md
+-rw-r--r--   0        0        0    17337 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/getting_started.md
+-rw-r--r--   0        0        0     9875 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/_old/OLD_pyrel_quickstart.md
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/_old/metamodel.md
+-rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/_old/python_dsl.md
+-rw-r--r--   0        0        0     9371 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/_old/quickstart.md
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/README.md
+-rw-r--r--   0        0        0    13377 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/cli/README.md
+-rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/configuration/README.md
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Expression.md
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Property.md
+-rw-r--r--   0        0        0     6788 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/README.md
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Context/README.md
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Context/enter__.md
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Context/exit__.md
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Context/iter__.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Context/model.md
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Context/results.md
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/ContextSelect/README.md
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/ContextSelect/add.md
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/ContextSelect/call__.md
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/ContextSelect/getattribute__.md
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Instance/README.md
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Instance/persist.md
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Instance/set.md
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Instance/unpersist.md
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/InstanceProperty/README.md
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/InstanceProperty/or_.md
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Model/README.md
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Model/Type.md
+-rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Model/found.md
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Model/name.md
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Model/not_found.md
+-rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Model/ordered_choice.md
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Model/query.md
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Model/read.md
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Model/rule.md
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Model/scope.md
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Model/union.md
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/README.md
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/add__.md
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/enter__.md
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/eq__.md
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/exit__.md
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/ge__.md
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/getattribute__.md
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/gt__.md
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/le__.md
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/lt__.md
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/mul__.md
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/ne__.md
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/pow__.md
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/radd__.md
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/rmul__.md
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/rpow__.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/rsub__.md
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/rtruediv__.md
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/sub__.md
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/truediv__.md
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Type/README.md
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Type/add.md
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Type/call__.md
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Type/extend.md
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Type/model.md
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Type/name.md
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Type/or__.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/clients/README.md
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/clients/snowflake/PrimaryKey.md
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/clients/snowflake/README.md
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/clients/snowflake/Snowflake.md
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md
+-rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/README.md
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/Vars.md
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/alias.md
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/aggregates/README.md
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/aggregates/avg.md
+-rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/aggregates/count.md
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/aggregates/max.md
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/aggregates/min.md
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/aggregates/rank_asc.md
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/aggregates/rank_desc.md
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/aggregates/sum.md
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/README.md
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/README.md
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/avg_degree.md
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/avg_indegree.md
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/avg_outdegree.md
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md
+-rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/degree.md
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/degree_centrality.md
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/indegree.md
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/infomap.md
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/label_propagation.md
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/louvain.md
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/max_degree.md
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/max_indegree.md
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/max_outdegree.md
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/min_degree.md
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/min_indegree.md
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/min_outdegree.md
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/num_edges.md
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/num_nodes.md
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/outdegree.md
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/pagerank.md
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Edge/README.md
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Edge/add.md
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Edge/call__.md
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Edge/extend.md
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/EdgeInstance/README.md
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/EdgeInstance/from_.md
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/EdgeInstance/set.md
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/EdgeInstance/to.md
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/Edge.md
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/Node.md
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/README.md
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/compute.md
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/fetch.md
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/id.md
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/model.md
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/undirected.md
+-rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/visualize.md
+-rw-r--r--   0        0        0    20679 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png
+-rw-r--r--   0        0        0    15558 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png
+-rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/strings/README.md
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/strings/concat.md
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/strings/contains.md
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/strings/ends_with.md
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/strings/join.md
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/strings/length.md
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/strings/lowercase.md
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/strings/replace.md
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/strings/uppercase.md
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/sql/README.md
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/README.md
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/cdc.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/custom_snowflake_connection.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/emit_playground.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/found.py
+-rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/fraud.ipynb
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/fraud.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/graph_algos.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/load_raw.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/nested.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/or_types.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/remote_load_csv.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/requirements.txt
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/simple.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/simple_recursion.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/simple_streamlit.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/solver.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/weighted_graph_algos.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/articles_graph/README.md
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/articles_graph/articles_graph.py
+-rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/articles_graph/articles_graph_with_nlp.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/articles_graph/pyproject.toml
+-rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/articles_graph/utils.py
+-rw-r--r--   0        0        0  1274296 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/articles_graph/daily_articles/04_04_2024.json
+-rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/data/people.csv
+-rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/data/transactions.csv
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/ev_penetration/ev_penetration.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/ev_penetration/ev_penetration_csv.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/ev_penetration/state_stats.csv
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/imdb/README.md
+-rw-r--r--   0        0        0   787694 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/imdb/imdb.csv
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/imdb/imdb.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/rel/bar.rel
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/rel/foo.rel
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/rel/solver.rel
+-rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/social-money-network/SF_pagerank.ipynb
+-rw-r--r--   0        0        0  2419367 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/social-money-network/Simulation-and-SF-Upload.ipynb
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/social-money-network/snowflake_pagerank.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/.gitignore
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/README.md
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/index.html
+-rw-r--r--   0        0        0   463836 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/package-lock.json
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/package.json
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/tsconfig.json
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/vite.config.ts
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/.storybook/main.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/.storybook/preview-body.html
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/.storybook/preview-head.html
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/.storybook/preview.ts
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/App.styl
+-rw-r--r--   0        0        0     4211 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/App.tsx
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/Selection.tsx
+-rw-r--r--   0        0        0    10577 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/debugger_client.ts
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/index.css
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/index.tsx
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/logo.svg
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/util.styl
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/util.ts
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/ws.ts
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/assets/favicon.png
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/EventList.styl
+-rw-r--r--   0        0        0     6781 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/EventList.tsx
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/EventViewer.styl
+-rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/EventViewer.tsx
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Sidebar.styl
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Sidebar.tsx
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx
+-rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/ScopeProvider.tsx
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/index.stories.tsx
+-rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/index.styl
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/index.tsx
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/ComputeNode.tsx
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/FilterNode.tsx
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/UnknownNode.tsx
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/base.styl
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/base.tsx
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/index.tsx
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Accordion.stories.tsx
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Accordion.styl
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Accordion.tsx
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Button.styl
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Button.tsx
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Code.styl
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Code.tsx
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Collapsible.stories.tsx
+-rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Collapsible.styl
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Collapsible.tsx
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Field.stories.tsx
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Field.styl
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Field.tsx
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Icon.styl
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Icon.tsx
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Modal.stories.tsx
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Modal.styl
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Modal.tsx
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Tooltip.stories.tsx
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Tooltip.styl
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Tooltip.tsx
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/fixtures/branch-improved.json
+-rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/fixtures/branch.json
+-rw-r--r--   0        0        0    67308 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/fixtures/fraud.json
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/fixtures/index.ts
+-rw-r--r--   0        0        0     9536 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/fixtures/not_found.json
+-rw-r--r--   0        0        0     6685 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/fixtures/simple.json
+-rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/fixtures/union.json
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/types/json.d.ts
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/types/jsx.d.ts
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/types/mech.d.ts
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/__init__.py
+-rw-r--r--   0        0        0    12329 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/emit.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/exec.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/fixtures.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/patch.py
+-rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/util.py
+-rwxr-xr-x   0        0        0     3521 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/cli/__main__.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/cli/collect_failures.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/cli/collect_tests.py
+-rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/cli/repro.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/cli/run_tests.py
+-rw-r--r--   0        0        0    15710 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/cli/watch.py
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/gen/action.py
+-rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/gen/context.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/gen/document.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/gen/error.py
+-rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/gen/group_limited.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/gen/ir.py
+-rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/gen/scope.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/gen/staged.py
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/gen/task.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/gen/test.py
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/harness/database.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/harness/vendor_types.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/validate/diff.py
+-rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/validate/errors.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/validate/mapping.py
+-rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/validate/roundtrip.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/__init__.py
+-rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/compiler.py
+-rw-r--r--   0        0        0     9999 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/debugging.py
+-rw-r--r--   0        0        0    44804 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/dsl.py
+-rw-r--r--   0        0        0    12279 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/errors.py
+-rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/metagen.py
+-rw-r--r--   0        0        0    27821 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/metamodel.py
+-rw-r--r--   0        0        0    19780 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/rel.py
+-rw-r--r--   0        0        0    20453 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/rel2.py
+-rw-r--r--   0        0        0    13261 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/rel_emitter.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/rel_utils.py
+-rw-r--r--   0        0        0     8570 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/analysis/mechanistic.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/analysis/whynot.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/clients/__init__.py
+-rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/clients/azure.py
+-rw-r--r--   0        0        0    10327 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/clients/client.py
+-rw-r--r--   0        0        0    17958 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/clients/config.py
+-rw-r--r--   0        0        0    34436 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/clients/snowflake.py
+-rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/clients/test.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/clients/types.py
+-rw-r--r--   0        0        0     7366 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/loaders/csv.py
+-rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/loaders/loader.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/loaders/types.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/std/__init__.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/std/aggregates.py
+-rw-r--r--   0        0        0    14639 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/std/graphs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/std/strings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/tools/__init__.py
+-rw-r--r--   0        0        0    52000 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/tools/cli.py
+-rw-r--r--   0        0        0    10318 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/tools/cli_controls.py
+-rw-r--r--   0        0        0     6792 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/tools/debugger.py
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/tools/debugger_server.py
+-rw-r--r--   0        0        0     9121 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/tools/dev.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/tools/notes
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/__init__.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/conftest.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/README.md
+-rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/conftest.py
+-rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_graph_visualize.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_snapshots.py
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/agg_ordering/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query0.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query1.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/bottom/query0.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/first/query0.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query0.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query1.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query1.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query2.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query3.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query0.txt
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query1.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query2.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query3.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query4.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query0.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query1.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query10.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query11.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query2.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query3.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query4.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query5.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query6.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query7.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query8.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query9.txt
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query0.txt
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query1.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query0.txt
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query1.txt
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query3.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query4.txt
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query0.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query1.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query0.txt
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query1.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query2.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query3.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query0.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query1.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query0.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query1.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query2.txt
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query3.txt
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query4.txt
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query5.txt
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query6.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/top/query0.txt
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/union/query0.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query0.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query1.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query2.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query3.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query4.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query5.txt
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/agg_ordering.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/bool.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/bottom.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/export.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/first.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/multi_valued.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/not_found.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/persist.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/smoke.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/strings.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/top.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/union.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/weighted_graphs.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/graphs/basics.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/graphs/centrality.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/graphs/community.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/graphs/degree.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/graphs/similarity.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/execution/test_core.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/execution/test_examples.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/execution/basic/smoketest.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/execution/snapshots/test_core/test_basic/smoketest/query0.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/execution/snapshots/test_examples/test_example/emit_playground/query0.txt
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/execution/snapshots/test_examples/test_example/found/query0.txt
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/execution/snapshots/test_examples/test_example/graph/query0.txt
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/execution/snapshots/test_examples/test_example/graph/query1.txt
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/execution/snapshots/test_examples/test_example/load_raw/query0.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/execution/snapshots/test_examples/test_example/or_types/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/execution/snapshots/test_examples/test_example/simple/query0.txt
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/execution/snapshots/test_examples/test_example/simple_recursion/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/execution/snapshots/test_examples/test_example/simple_streamlit/query0.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/execution/snapshots/test_examples/test_example/test/query0.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/init-cli/__init__.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/init-cli/azure_basic.py
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/init-cli/common.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/roundtrip/test_document.py
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/roundtrip/test_task.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 relationalai-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 relationalai-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/pypi/README.md
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 relationalai-0.2.3/PKG-INFO
```

### Comparing `relationalai-0.2.2/README.md` & `relationalai-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/.github/actions/end-to-end/action.yml` & `relationalai-0.2.3/.github/actions/end-to-end/action.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/.github/workflows/end-to-end.yml` & `relationalai-0.2.3/.github/workflows/end-to-end.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/.github/workflows/publish-to-pypi.yml` & `relationalai-0.2.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/.github/workflows/ruff.yml` & `relationalai-0.2.3/.github/workflows/ruff.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/getting_started.md` & `relationalai-0.2.3/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/_old/OLD_pyrel_quickstart.md` & `relationalai-0.2.3/docs/_old/OLD_pyrel_quickstart.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/_old/metamodel.md` & `relationalai-0.2.3/docs/_old/metamodel.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/_old/python_dsl.md` & `relationalai-0.2.3/docs/_old/python_dsl.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/_old/quickstart.md` & `relationalai-0.2.3/docs/_old/quickstart.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/cli/README.md` & `relationalai-0.2.3/docs/api_reference/cli/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/configuration/README.md` & `relationalai-0.2.3/docs/api_reference/configuration/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Expression.md` & `relationalai-0.2.3/docs/api_reference/python/Expression.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Property.md` & `relationalai-0.2.3/docs/api_reference/python/Property.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/README.md` & `relationalai-0.2.3/docs/api_reference/python/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -55,14 +55,15 @@
   - [`Producer.__sub__()`](./Producer/sub__.md)
   - [`Producer.__truediv__()`](./Producer/truediv__.md)
 - [`Property`](./Property.md)
 - [`Type`](./Type/README.md)
   - [`Type.__call__()`](./Type/call__.md)
   - [`Type.__or__()`](./Type/or__.md)
   - [`Type.add()`](./Type/add.md)
+  - [`Type.extend()`](./Type/extend.md)
   - [`Type.model`](./Type/model.md)
   - [`Type.name`](./Type/name.md)
 
 ## [`relationalai.std`](./std/README.md)
 
 The `relationalai.std` namespace contains the RelationalAI Query Builder Standard Library.
 This includes functions for performing [aggregations](./std/aggregates/)
@@ -85,35 +86,49 @@
 
 - [`graphs.Compute`](./std/graphs/Compute/README.md)
   - [`graphs.Compute.betweenness_centrality()`](./std/graphs/Compute/betweeness_centrality.md)
   - [`graphs.Compute.cosine_similarity()`](./std/graphs/Compute/cosine_similarity.md)
   - [`graphs.Compute.degree()`](./std/graphs/Compute/degree.md)
   - [`graphs.Compute.degree_centrality()`](./std/graphs/Compute/degree_centrality.md)
   - [`graphs.Compute.eigenvector_centrality()`](./std/graphs/Compute/eigenvector_centrality.md)
+  - [`graphs.Compute.num_edges()`](./std/graphs//Compute/num_edges.md)
   - [`graphs.Compute.indegree()`](./std/graphs/Compute/indegree.md)
   - [`graphs.Compute.label_propagation()`](./std/graphs/Compute/label_propagation.md)
   - [`graphs.Compute.louvain()`](./std/graphs/Compute/louvain.md)
+  - [`graphs.Compute.num_nodes()`](./std//graphs//Compute/num_nodes.md)
   - [`graphs.Compute.outdegree()`](./std/graphs/Compute/outdegree.md)
   - [`graphs.Compute.pagerank()`](./std/graphs/Compute/pagerank.md)
   - [`graphs.Compute.weakly_connected_component()`](./std/graphs/Compute/weakly_connected_component.md)
-- [`graphs.Edges`](./std/graphs/Edges/README.md)
-  - [`graphs.Edges.add()`](./std/graphs/Edges/add.md)
-  - [`graphs.Edges.extend()`](./std/graphs/Edges/extend.md)
+- [`graphs.Edge`](./std/graphs/Edge/README.md)
+  - [`graphs.Edge.add()`](./std/graphs/Edge/add.md)
+  - [`graphs.Edge.extend()`](./std/graphs/Edge/extend.md)
+- [`graphs.EdgeInstance`](./std/graphs/EdgeInstance/README.md)
+  - [`graphs.EdgeInstance.from_`](./std/graphs/EdgeInstance/from_.md)
+  - [`graphs.EdgeInstance.to`](./std/graphs/EdgeInstance/to.md)
+  - [`graphs.EdgeInstance.set()`](./std/graphs/EdgeInstance/set.md)
 - [`graphs.Graph`](./std/graphs/Graph/README.md)
   - [`graphs.Graph.compute`](./std/graphs/Graph/compute.md)
-  - [`graphs.Graph.edges`](./std/graphs/Graph/edges.md)
+  - [`graphs.Graph.Edge`](./std/graphs/Graph/Edge.md)
   - [`graphs.Graph.fetch()`](./std/graphs/Graph/fetch.md)
   - [`graphs.Graph.id`](./std/graphs/Graph/id.md)
   - [`graphs.Graph.model`](./std/graphs/Graph/model.md)
-  - [`graphs.Graph.nodes`](./std/graphs/Graph/nodes.md)
+  - [`graphs.Graph.Node`](./std/graphs/Graph/Node.md)
   - [`graphs.Graph.undirected`](./std/graphs/Graph/undirected.md)
   - [`graphs.Graph.visualize()`](./std/graphs/Graph/visualize.md)
-- [`graphs.Nodes`](./std/graphs/Nodes/README.md)
-  - [`graphs.Nodes.add()`](./std/graphs/Nodes/add.md)
-  - [`graphs.Nodes.extend()`](./std/graphs/Nodes/extend.md)
+
+## [`relationalai.std.strings`](./std/strings/README.md)
+
+- [`strings.concat()`](./std/strings/concat.md)
+- [`strings.contains()`](./std/strings/contains.md)
+- [`strings.ends_with()`](./std/strings/ends_with.md)
+- [`strings.join()`](./std/strings/join.md)
+- [`strings.length()`](./std/strings/length.md)
+- [`strings.lowercase()`](./std/strings/lowercase.md)
+- [`strings.replace()`](./std/strings/replace.md)
+- [`strings.uppercase()`](./std/strings/uppercase.md)
 
 ## [`relationalai.clients`](./clients/README.md)
 
 - [`clients.snowflake`](./clients/snowflake/README.md)
   - [`clients.snowflake.PrimaryKey`](./clients/snowflake/PrimaryKey.md)
   - [`clients.snowflake.Snowflake`](./clients/snowflake/Snowflake.md)
   - [`clients.snowflake.SnowflakeTable`](./clients/snowflake/SnowflakeTable/README.md)
```

### Comparing `relationalai-0.2.2/docs/api_reference/python/Context/README.md` & `relationalai-0.2.3/docs/api_reference/python/Context/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Context/enter__.md` & `relationalai-0.2.3/docs/api_reference/python/Context/enter__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Context/exit__.md` & `relationalai-0.2.3/docs/api_reference/python/Context/exit__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Context/iter__.md` & `relationalai-0.2.3/docs/api_reference/python/Context/iter__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Context/model.md` & `relationalai-0.2.3/docs/api_reference/python/Context/model.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Context/results.md` & `relationalai-0.2.3/docs/api_reference/python/Context/results.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/ContextSelect/README.md` & `relationalai-0.2.3/docs/api_reference/python/ContextSelect/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/ContextSelect/add.md` & `relationalai-0.2.3/docs/api_reference/python/ContextSelect/add.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/ContextSelect/call__.md` & `relationalai-0.2.3/docs/api_reference/python/ContextSelect/call__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/ContextSelect/getattribute__.md` & `relationalai-0.2.3/docs/api_reference/python/ContextSelect/getattribute__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Instance/README.md` & `relationalai-0.2.3/docs/api_reference/python/Instance/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Instance/persist.md` & `relationalai-0.2.3/docs/api_reference/python/Instance/persist.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Instance/set.md` & `relationalai-0.2.3/docs/api_reference/python/Instance/set.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Instance/unpersist.md` & `relationalai-0.2.3/docs/api_reference/python/Instance/unpersist.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/InstanceProperty/README.md` & `relationalai-0.2.3/docs/api_reference/python/InstanceProperty/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/InstanceProperty/or_.md` & `relationalai-0.2.3/docs/api_reference/python/InstanceProperty/or_.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Model/README.md` & `relationalai-0.2.3/docs/api_reference/python/Model/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Model/Type.md` & `relationalai-0.2.3/docs/api_reference/python/Model/Type.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Model/found.md` & `relationalai-0.2.3/docs/api_reference/python/Model/found.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Model/not_found.md` & `relationalai-0.2.3/docs/api_reference/python/Model/not_found.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Model/ordered_choice.md` & `relationalai-0.2.3/docs/api_reference/python/Model/ordered_choice.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Model/query.md` & `relationalai-0.2.3/docs/api_reference/python/Model/query.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Model/read.md` & `relationalai-0.2.3/docs/api_reference/python/Model/read.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Model/rule.md` & `relationalai-0.2.3/docs/api_reference/python/Model/rule.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Model/scope.md` & `relationalai-0.2.3/docs/api_reference/python/Model/scope.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Model/union.md` & `relationalai-0.2.3/docs/api_reference/python/Model/union.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Producer/README.md` & `relationalai-0.2.3/docs/api_reference/python/Producer/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Producer/add__.md` & `relationalai-0.2.3/docs/api_reference/python/Producer/add__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Producer/enter__.md` & `relationalai-0.2.3/docs/api_reference/python/Producer/enter__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Producer/eq__.md` & `relationalai-0.2.3/docs/api_reference/python/Producer/eq__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Producer/exit__.md` & `relationalai-0.2.3/docs/api_reference/python/Producer/exit__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Producer/ge__.md` & `relationalai-0.2.3/docs/api_reference/python/Producer/ge__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Producer/getattribute__.md` & `relationalai-0.2.3/docs/api_reference/python/Producer/getattribute__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Producer/gt__.md` & `relationalai-0.2.3/docs/api_reference/python/Producer/gt__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Producer/le__.md` & `relationalai-0.2.3/docs/api_reference/python/Producer/le__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Producer/lt__.md` & `relationalai-0.2.3/docs/api_reference/python/Producer/lt__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Producer/mul__.md` & `relationalai-0.2.3/docs/api_reference/python/Producer/mul__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Producer/ne__.md` & `relationalai-0.2.3/docs/api_reference/python/Producer/ne__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Producer/pow__.md` & `relationalai-0.2.3/docs/api_reference/python/Producer/pow__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Producer/sub__.md` & `relationalai-0.2.3/docs/api_reference/python/Producer/sub__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Producer/truediv__.md` & `relationalai-0.2.3/docs/api_reference/python/Producer/truediv__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Type/README.md` & `relationalai-0.2.3/docs/api_reference/python/Type/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 ## Attributes
 
 - [`Type.model`](./model.md)
 - [`Type.name`](./name.md)
 
 ## Methods
 
+- [`Type.add()`](./add.md)
 - [`Type.__call__()`](./call__.md)
+- [`Type.extend()`](./extend.md)
 - [`Type.__or__()`](./or__.md)
 
 ## Example
 
 Use [`Model.Type()`](../Model/Type.md) to create a `Type` object rather than constructing one directly:
 
 ```python
```

### Comparing `relationalai-0.2.2/docs/api_reference/python/Type/add.md` & `relationalai-0.2.3/docs/api_reference/python/Type/add.md`

 * *Files 5% similar despite different names*

```diff
@@ -57,8 +57,8 @@
 # Output:
 #                      book
 # 0  iikm1rGdR3jWQtS2XVUZDg
 ```
 
 ## See Also
 
-[`Instanse.set()`](../Instance/set.md)
+[`Instance.set()`](../Instance/set.md)
```

### Comparing `relationalai-0.2.2/docs/api_reference/python/Type/call__.md` & `relationalai-0.2.3/docs/api_reference/python/Type/call__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/Type/or__.md` & `relationalai-0.2.3/docs/api_reference/python/Type/or__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/clients/README.md` & `relationalai-0.2.3/docs/api_reference/python/clients/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/clients/snowflake/PrimaryKey.md` & `relationalai-0.2.3/docs/api_reference/python/clients/snowflake/PrimaryKey.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/clients/snowflake/README.md` & `relationalai-0.2.3/docs/api_reference/python/clients/snowflake/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/clients/snowflake/Snowflake.md` & `relationalai-0.2.3/docs/api_reference/python/clients/snowflake/Snowflake.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md` & `relationalai-0.2.3/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md` & `relationalai-0.2.3/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md` & `relationalai-0.2.3/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md` & `relationalai-0.2.3/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/README.md` & `relationalai-0.2.3/docs/api_reference/python/std/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # `relationalai.std`
 
 The `relationalai.std` namespace contains the RelationalAI Query Builder Standard Library.
-This includes functions for performing [aggregations](./aggregates/)
-as well as classes for creating and working with [graphs](./graphs.md).
 
 - [`alias()`](./alias.md)
 - [`Vars`](./Vars.md)
 
 ## [`relationalai.std.aggregates`](./aggregates/README.md)
 
 - [`aggregates.avg()`](./aggregates/avg.md)
@@ -16,33 +14,57 @@
 - [`aggregates.rank_asc()`](./aggregates/rank_asc.md)
 - [`aggregates.rank_desc()`](./aggregates/rank_desc.md)
 - [`aggregates.sum()`](./aggregates/sum.md)
 
 ## [`relationalai.std.graphs`](./graphs/README.md)
 
 - [`graphs.Compute`](./graphs/Compute/README.md)
+  - [`graphs.Compute.avg_degree()`](./graphs/Compute/avg_degree.md)
+  - [`graphs.Compute.avg_indegree()`](./graphs/Compute/avg_indegree.md)
+  - [`graphs.Compute.avg_outdegree()`](./graphs/Compute/avg_outdegree.md)
   - [`graphs.Compute.betweenness_centrality()`](./graphs/Compute/betweeness_centrality.md)
   - [`graphs.Compute.cosine_similarity()`](./graphs/Compute/cosine_similarity.md)
   - [`graphs.Compute.degree()`](./graphs/Compute/degree.md)
   - [`graphs.Compute.degree_centrality()`](./graphs/Compute/degree_centrality.md)
   - [`graphs.Compute.eigenvector_centrality()`](./graphs/Compute/eigenvector_centrality.md)
+  - [`graphs.Compute.num_edges()`](./graphs/Compute/num_edges.md)
   - [`graphs.Compute.indegree()`](./graphs/Compute/indegree.md)
   - [`graphs.Compute.label_propagation()`](./graphs/Compute/label_propagation.md)
   - [`graphs.Compute.louvain()`](./graphs/Compute/louvain.md)
+  - [`graphs.Compute.max_degree()`](./graphs/Compute/max_degree.md)
+  - [`graphs.Compute.max_indegree()`](./graphs/Compute/max_indegree.md)
+  - [`graphs.Compute.max_outdegree()`](./graphs/Compute/max_outdegree.md)
+  - [`graphs.Compute.min_degree()`](./graphs/Compute/min_degree.md)
+  - [`graphs.Compute.min_indegree()`](./graphs/Compute/min_indegree.md)
+  - [`graphs.Compute.min_outdegree()`](./graphs/Compute/min_outdegree.md)
+  - [`graphs.Compute.num_nodes()`](./graphs/Compute/num_nodes.md)
   - [`graphs.Compute.outdegree()`](./graphs/Compute/outdegree.md)
   - [`graphs.Compute.pagerank()`](./graphs/Compute/pagerank.md)
   - [`graphs.Compute.weakly_connected_component()`](./graphs/Compute/weakly_connected_component.md)
-- [`graphs.Edges`](./graphs/Edges/README.md)
-  - [`graphs.Edges.add()`](./graphs/Edges/add.md)
-  - [`graphs.Edges.extend()`](./graphs/Edges/extend.md)
+- [`graphs.Edge`](./graphs/Edge/README.md)
+  - [`graphs.Edge.__call__()`](./graphs/Edge/call__.md)
+  - [`graphs.Edge.add()`](./graphs/Edge/add.md)
+  - [`graphs.Edge.extend()`](./graphs/Edge/extend.md)
+- [`graphs.EdgeInstance`](./graphs/EdgeInstance/README.md)
+  - [`graphs.EdgeInstance.from_`](./graphs/EdgeInstance/from_.md)
+  - [`graphs.EdgeInstance.to`](./graphs/EdgeInstance/to.md)
+  - [`graphs.EdgeInstance.set()`](./graphs/EdgeInstance/set.md)
 - [`graphs.Graph`](./graphs/Graph/README.md)
   - [`graphs.Graph.compute`](./graphs/Graph/compute.md)
-  - [`graphs.Graph.edges`](./graphs/Graph/edges.md)
+  - [`graphs.Graph.Edge`](./graphs/Graph/Edge.md)
   - [`graphs.Graph.fetch()`](./graphs/Graph/fetch.md)
   - [`graphs.Graph.id`](./graphs/Graph/id.md)
   - [`graphs.Graph.model`](./graphs/Graph/model.md)
-  - [`graphs.Graph.nodes`](./graphs/Graph/nodes.md)
+  - [`graphs.Graph.Node`](./graphs/Graph/Node.md)
   - [`graphs.Graph.undirected`](./graphs/Graph/undirected.md)
   - [`graphs.Graph.visualize()`](./graphs/Graph/visualize.md)
-- [`graphs.Nodes`](./graphs/Nodes/README.md)
-  - [`graphs.Nodes.add()`](./graphs/Nodes/add.md)
-  - [`graphs.Nodes.extend()`](./graphs/Nodes/extend.md)
+
+## [`relationalai.std.strings`](./strings/README.md)
+
+- [`strings.concat()`](./strings/concat.md)
+- [`strings.contains()`](./strings/contains.md)
+- [`strings.ends_with()`](./strings/ends_with.md)
+- [`strings.join()`](./strings/join.md)
+- [`strings.length()`](./strings/length.md)
+- [`strings.lowercase()`](./strings/lowercase.md)
+- [`strings.replace()`](./strings/replace.md)
+- [`strings.uppercase()`](./strings/uppercase.md)
```

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/Vars.md` & `relationalai-0.2.3/docs/api_reference/python/std/Vars.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/alias.md` & `relationalai-0.2.3/docs/api_reference/python/std/alias.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/aggregates/README.md` & `relationalai-0.2.3/docs/api_reference/python/std/aggregates/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/aggregates/avg.md` & `relationalai-0.2.3/docs/api_reference/python/std/aggregates/avg.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/aggregates/count.md` & `relationalai-0.2.3/docs/api_reference/python/std/aggregates/count.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/aggregates/max.md` & `relationalai-0.2.3/docs/api_reference/python/std/aggregates/max.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/aggregates/min.md` & `relationalai-0.2.3/docs/api_reference/python/std/aggregates/min.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/aggregates/rank_asc.md` & `relationalai-0.2.3/docs/api_reference/python/std/aggregates/rank_asc.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/aggregates/rank_desc.md` & `relationalai-0.2.3/docs/api_reference/python/std/aggregates/rank_desc.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/aggregates/sum.md` & `relationalai-0.2.3/docs/api_reference/python/std/aggregates/sum.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/graphs/README.md` & `relationalai-0.2.3/docs/api_reference/python/std/graphs/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,43 @@
 # `relationalai.std.graphs`
 
 The `relationalai.std.graphs` namespace contains functions and classes for building
 [graphs](./Graph/README.md) from objects in a [model](../../Model/README.md) and doing graph analytics.
 
 - [`graphs.Compute`](./Compute/README.md)
+  - [`graphs.Compute.avg_degree()`](./Compute/avg_degree.md)
+  - [`graphs.Compute.avg_indegree()`](./Compute/avg_indegree.md)
+  - [`graphs.Compute.avg_outdegree()`](./Compute/avg_outdegree.md)
   - [`graphs.Compute.betweenness_centrality()`](./Compute/betweeness_centrality.md)
   - [`graphs.Compute.cosine_similarity()`](./Compute/cosine_similarity.md)
   - [`graphs.Compute.degree()`](./Compute/degree.md)
   - [`graphs.Compute.degree_centrality()`](./Compute/degree_centrality.md)
   - [`graphs.Compute.eigenvector_centrality()`](./Compute/eigenvector_centrality.md)
   - [`graph.Compute.indegree()`](./Compute/indegree.md)
   - [`graphs.Compute.label_propagation()`](./Compute/label_propagation.md)
   - [`graphs.Compute.louvain()`](./Compute/louvain.md)
+  - [`graphs.Compute.max_degree()`](./Compute/max_degree.md)
+  - [`graphs.Compute.max_indegree()`](./Compute/max_indegree.md)
+  - [`graphs.Compute.max_outdegree()`](./Compute/max_outdegree.md)
+  - [`graphs.Compute.min_degree()`](./Compute/min_degree.md)
+  - [`graphs.Compute.min_indegree()`](./Compute/min_indegree.md)
+  - [`graphs.Compute.min_outdegree()`](./Compute/min_outdegree.md)
   - [`graphs.Compute.outdegree()`](./Compute/outdegree.md)
   - [`graphs.Compute.pagerank()`](./Compute/pagerank.md)
   - [`graphs.Compute.weakly_connected_component()`](./Compute/weakly_connected_component.md)
-- [`graphs.Edges`](./Edges/README.md)
-  - [`graphs.Edges.add()`](./Edges/add.md)
-  - [`graphs.Edges.extend()`](./Edges/extend.md)
+- [`graphs.Edge`](./Edge/README.md)
+  - [`graphs.Edge.__call__()`](./Edge/call__.md)
+  - [`graphs.Edge.add()`](./Edge/add.md)
+  - [`graphs.Edge.extend()`](./Edge/extend.md)
+- [`graphs.EdgeInstance`](./EdgeInstance/README.md)
+  - [`graphs.EdgeInstance.from_`](./EdgeInstance/from_.md)
+  - [`graphs.EdgeInstance.to`](./EdgeInstance/to.md)
+  - [`graphs.EdgeInstance.set()`](./EdgeInstance/set.md)
 - [`graphs.Graph`](./Graph/README.md)
   - [`graphs.Graph.compute`](./Graph/compute.md)
-  - [`graphs.Graph.edges`](./Graph/edges.md)
+  - [`graphs.Graph.Edge`](./Graph/Edge.md)
   - [`graphs.Graph.fetch()`](./Graph/fetch.md)
   - [`graphs.Graph.id`](./Graph/id.md)
   - [`graphs.Graph.model`](./Graph/model.md)
-  - [`graphs.Graph.nodes`](./Graph/nodes.md)
+  - [`graphs.Graph.Node`](./Graph/Node.md)
   - [`graphs.Graph.undirected`](./Graph/undirected.md)
   - [`graphs.Graph.visualize()`](./Graph/visualize.md)
-- [`graphs.Nodes`](./Nodes/README.md)
-  - [`graphs.Nodes.add()`](./Nodes/add.md)
-  - [`graphs.Nodes.extend()`](./Nodes/extend.md)
```

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/README.md` & `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,33 @@
-# `relationalai.std.graphs.Compute`
-
-The `Compute` class serves as a namespace for graph functions.
-You do not create `Compute` objects directly.
-A `Compute` instance is automatically instantiated when you create a [`Graph`](../Graph/README.md) object.
-You access a graph's `Compute` instance via the [`Graph.compute`](../Graph/compute.md) attribute.
+# `relationalai.std.graphs.Compute.weakly_connected_component()`
 
 ```python
-class relationalai.std.graphs.Compute(graph: Graph)
+relationalai.std.graphs.Compute.weakly_connected_component(node: Producer) -> Expression
 ```
 
+Returns an [`Expression`](../../../Expression.md) that produces the component IDs of the
+[weakly connected components](https://en.wikipedia.org/wiki/Weak_component)
+to which the nodes produced by the `node` producer belong.
+
+## Supported Graph Types
+
+| Graph Type | Supported | Notes |
+| :--- | :--- | :------ |
+| Directed | Yes |   |
+| Undirected | Yes |   |
+
 ## Parameters
 
 | Name | Type | Description |
 | :--- | :--- | :------ |
-| `graph` | [`Graph`](../Graph/README.md) | The graph on which the `Compute` namespace is instantiated. |
+| `node` | [`Producer`](../../../Producer/README.md) | A producer that produces object IDs of nodes. |
 
-## Methods
+## Returns
 
-- [`Compute.betweeness_centrality()`](./betweeness_centrality.md)
-- [`Compute.cosine_similarity()`](./cosine_similarity.md)
-- [`Compute.degree()`](./degree.md)
-- [`Compute.degree_centrality()`](./degree_centrality.md)
-- [`Compute.eigenvector_centrality()`](./eigenvector_centrality.md)
-- [`Compute.indegree()`](./indegree.md)
-- [`Compute.label_propagation()`](./label_propagation.md)
-- [`Compute.louvain()`](./louvain.md)
-- [`Compute.outdegree()`](./outdegree.md)
-- [`Compute.pagerank()`](./pagerank.md)
-- [`Compute.weakly_connected_component()`](./weakly_connected_component.md)
+An [`Expression`](../../../Expression.md) object that produces `string` values.
 
 ## Example
 
 ```python
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
@@ -44,25 +40,33 @@
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
     carol = Person.add(name="Carol")
     alice.set(follows=carol)
     bob.set(follows=alice)
     carol.set(follows=alice).set(follows=bob)
 
-# Create a graph and add the `Person.follows` property to the set of edges.
+# Create a graph and add all Person objects to the set of nodes
+# and the Person.follows property to the set of edges.
 graph = Graph(model)
+graph.Node.extend(Person)
 graph.Edge.extend(Person.follows)
 
-# Compute the PageRank of each person in the graph.
+# Compute the weakly connected component for each person in the graph.
 with model.query() as select:
     person = Person()
-    # The `pagerank` function is in the `graph.compute` namespace.
-    pagerank = graph.compute.pagerank(person)
-    response = select(person.name, pagerank)
+    component = graph.compute.weakly_connected_component(person)
+    response = select(person.name, component)
 
 print(response.results)
 # Output:
-#     name         v
-# 0  Alice  0.397402
-# 1    Bob  0.214806
-# 2  Carol  0.387792
+#     name                       v
+# 0  Alice  JCOgZI0tb1qNRTyXYhDFOw
+# 1    Bob  JCOgZI0tb1qNRTyXYhDFOw
+# 2  Carol  JCOgZI0tb1qNRTyXYhDFOw
 ```
+
+Component IDs are the object IDs of the objects chosen to represent the components.
+In the preceding example, all three nodes are in the same component.
+
+## See Also
+
+[`Compute.label_propagation`](./label_propagation.md)
```

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md` & `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md` & `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/degree.md` & `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/degree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/degree_centrality.md` & `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/degree_centrality.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md` & `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/indegree.md` & `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/indegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/infomap.md` & `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/infomap.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md` & `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/label_propagation.md` & `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/label_propagation.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/louvain.md` & `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/louvain.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/outdegree.md` & `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/outdegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/pagerank.md` & `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/pagerank.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md` & `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/num_edges.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,59 @@
-# `relationalai.std.graphs.Compute.weakly_connected_component()`
+# `relationalai.std.graphs.Compute.num_edges()`
 
 ```python
-relationalai.std.graphs.Compute.weakly_connected_component(node: Producer) -> Expression
+relationalai.std.graphs.Compute.num_edges() -> Expression
 ```
 
-Returns an [`Expression`](../../../Expression.md) that produces the component IDs of the
-[weakly connected components](https://en.wikipedia.org/wiki/Weak_component)
-to which the nodes produced by the `node` producer belong.
+An [Expression](docs/api_reference/python/Expression.md) object that produces the number of edges in the graph.
 
 ## Supported Graph Types
 
 | Graph Type | Supported | Notes |
 | :--- | :--- | :------ |
 | Directed | Yes |   |
 | Undirected | Yes |   |
+| Weighted | Yes | Weights are ignored. |
+
 
 ## Parameters
 
-| Name | Type | Description |
-| :--- | :--- | :------ |
-| `node` | [`Producer`](../../../Producer/README.md) | A producer that produces object IDs of nodes. |
+No parameters are needed.
 
 ## Returns
 
-An [`Expression`](../../../Expression.md) object that produces `string` values.
+Returns an [Expression](docs/api_reference/python/Expression.md) that produces the number of edges in the graph.
 
 ## Example
 
 ```python
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
-# Create a model named "socialNetwork" with a Person type.
+# Create a model named "socialNetwork" with a Person type
 model = rai.Model("socialNetwork")
 Person = model.Type("Person")
 
-# Add some people to the model and connect them with a `follows` property.
+# Add some people to the graph and connect them with a `follows` property
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
-    carol = Person.add(name="Carol")
-    alice.set(follows=carol)
-    bob.set(follows=alice)
-    carol.set(follows=alice).set(follows=bob)
-
-# Create a graph and add all Person objects to the set of nodes
-# and the Person.follows property to the set of edges.
-graph = Graph(model)
-graph.Node.extend(Person)
+    charlie = Person.add(name="Charlie")
+    alice.set(follows=bob)
+    bob.set(follows=charlie)
+    charlie.set(follows=alice).set(follows=bob)
+    
+# Create an undirected graph and add all Person objects to the set of nodes
+graph = Graph(model, undirected=True)
+graph.Node.extend(Person, label=Person.name)
 graph.Edge.extend(Person.follows)
 
-# Compute the weakly connected component for each person in the graph.
+# Compute the number of edges in the graph
 with model.query() as select:
-    person = Person()
-    component = graph.compute.weakly_connected_component(person)
-    response = select(person.name, component)
-
+    num_edges = graph.compute.num_edges()
+    response = select(num_edges)
+    
 print(response.results)
 # Output:
-#     name                       v
-# 0  Alice  JCOgZI0tb1qNRTyXYhDFOw
-# 1    Bob  JCOgZI0tb1qNRTyXYhDFOw
-# 2  Carol  JCOgZI0tb1qNRTyXYhDFOw
-```
-
-Component IDs are the object IDs of the objects chosen to represent the components.
-In the preceding example, all three nodes are in the same component.
-
-## See Also
-
-[`Compute.label_propagation`](./label_propagation.md)
+#    v
+# 0  3
+```
```

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/graphs/Edges/README.md` & `relationalai-0.2.3/docs/api_reference/python/std/graphs/EdgeInstance/from_.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,49 +1,39 @@
-# `relationalai.std.graphs.Edges`
+# `relationalai.std.graphs.EdgeInstance.from_`
 
-The `Edges` class represents the collection of edges in a graph.
-You do not create `Edges` objects directly.
-An `Edges` instance is automatically instantiated when you create a [`Graph`](../Graph/README.md).
-You access a graph's `Edges` instance via the [`Graph.edges`](../Graph/edges.md) attribute.
-
-```python
-class relationalai.std.graphs.Edges(graph: Graph)
-```
-
-## Parameters
-
-| Name | Type | Description |
-| :--- | :--- | :------ |
-| `graph` | [`Graph`](../Graph/README.md) | The graph on which the `Edges` object is instantiated. |
-
-## Methods
-
-- [`Edges.add()`](./add.md)
-- [`Edges.extend()`](./extend.md)
+Returns a `Producer` object that produces the source node(s) of the [`EdgeInstance`](./README.md).
 
 ## Example
 
 ```python
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
-# Create a model named `socialNetwork` with a `Person` type.
+# Create a model with a `Person` type.
 model = rai.Model("socialNetwork")
 Person = model.Type("Person")
 
-# Add some people to the model and connect them with a `follows` property.
+# Add some people to the model and connect them with a 'follows' property.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
-    carol = Person.add(name="Carol")
-    alice.set(follows=carol)
-    bob.set(follows=alice)
-    carol.set(follows=alice).set(follows=bob)
+    alice.set(follows=bob)
 
-# Create a graph and get the set of edges.
+# Create a graph and add edges to it.
 graph = Graph(model)
-Edge = graph.Edge
+graph.Edge.extend(Person.follows)
 
-# Add the `Person.follows` property to the set of edges.
-# The nodes in each edge are automatically added to the graph.
-Edge.extend(Person.follows)
+# Display the source nodes of the edges.
+with model.query() as select:
+    edge = graph.Edge()
+    source_node = edge.from_
+    response = select(source_node.name)
+
+print(response.results)
+# Output:
+#     name
+# 0  Alice
 ```
+
+## See Also
+
+- [`EdgeInstance.to`](./to.md)
```

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/graphs/Edges/add.md` & `relationalai-0.2.3/docs/api_reference/python/std/graphs/Edge/add.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# `relationalai.std.graphs.Edges.add()`
+# `relationalai.std.graphs.Edge.add()`
 
 ```python
 relationalai.std.graph.Edge.add(from_: Producer, to: Producer, **kwargs: Any) -> None
 ```
 
 Adds edges to the graph from objects produced by the `from_` producer to objects produced by the `to` Producer.
 Edge properties may be passed as keyword arguments to `**kwargs`.
```

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/graphs/Edges/extend.md` & `relationalai-0.2.3/docs/api_reference/python/std/graphs/Edge/extend.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# `relationalai.std.graphs.Edges.extend()`
+# `relationalai.std.graphs.Edge.extend()`
 
 ```python
 relationalai.std.graph.Edge.extend(prop: Property, **kwargs: Any) -> None
 ```
 
 Add pairs of objects from a [`Property`](../../../Property.md) to a graph's edges.
 Edge properties may be passed as keyword arguments to `**kwargs`.
@@ -40,8 +40,8 @@
 graph = Graph(model)
 graph.Node.extend(Person)
 graph.Edge.extend(Person.follows)
 ```
 
 ## See Also
 
-[`Edges.add()`](./add.md) and [`Graph.edges`](../Graph/edges.md).
+[`Edges.add()`](./add.md)
```

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/README.md` & `relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/fetch.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,52 @@
-# `relationalai.std.graphs.Graph`
-
-The `Graph` class is used to create graphs representing relationships between objects in a model.
-You can use `Graph` objects to perform graph analytics on data in your model.
+# `relationalai.std.graphs.Graph.fetch()`
 
 ```python
-class relationalai.std.graphs.Graph(model: Model)
+relationalai.std.graphs.Graph.fetch() ->
 ```
 
+Returns a dictionary with two keys, `"nodes"` and `"edges"`, that represents the entire graph.
+
 ## Parameters
 
-| Name | Type | Description |
-| :--- | :--- | :------ |
-| `model` | [`Model`](../../../Model/README.md) | The model on which the `Graph` is instantiated. |
-
-## Attributes
-
-- [`Graph.compute`](./compute.md)
-- [`Graph.edges`](./edges.md)
-- [`Graph.id`](./id.md)
-- [`Graph.model`](./model.md)
-- [`Graph.nodes`](./nodes.md)
-- [`Graph.undirected`](./undirected.md)
+None
 
-## Methods
+## Returns
 
-- [`Graph.fetch()`](./fetch.md)
-- [`Graph.visualize()`](./visualize.md)
+A `dict` object.
 
 ## Example
 
 ```python
+from pprint import pprint
+
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
 # Create a model with a `Person` type.
 model = rai.Model("socialNetwork")
 Person = model.Type("Person")
 
 # Add some people to the model and connect them with a `follows` property.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
     alice.set(follows=bob)
 
-# Create a graph from the model and visualize it.
+# Create a graph with edges from the `Person.follows` property.
 graph = Graph(model)
 graph.Node.extend(Person, label=Person.name)
 graph.Edge.extend(Person.follows)
-graph.visualize()
+
+# Fetch the graph.
+pprint(graph.fetch())
+# Output:
+# {'edges': defaultdict(<class 'dict'>,
+#                       {('JCOgZI0tb1qNRTyXYhDFOw', 'v3PMBEmnWi5E2MxI4bGfzQ'): {}}),
+#  'nodes': defaultdict(<class 'dict'>,
+#                       {'JCOgZI0tb1qNRTyXYhDFOw': {'label': 'Alice'},
+#                        'v3PMBEmnWi5E2MxI4bGfzQ': {'label': 'Bob'}})}
 ```
 
-![A graph with two nodes labeled Alice and Bob and an edge pointing from Alice to Bob.](./img/simple-social-network.png)
+## See Also
+
+[`Graph.visualize()`](./visualize.md)
```

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/compute.md` & `relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/compute.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/edges.md` & `relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/Edge.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-# `relationalai.std.graphs.Graph.edges`
+# `relationalai.std.graphs.Graph.Edge`
 
-An attribute assigned to the graph's [`Edges`](../Edges/README.md) object.
+Returns an [`Edge`](../Edge/README.md) object that can be used to add and query edges in a graph.
 
 ## Returns
 
-A [`Edges`](../Edges/README.md) object.
+A [`Edge`](../Edge/README.md) object.
 
 ## Example
 
-A graph's `.edges` object represents its set of edges:
-
 ```python
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
 # Create a model with a `Person` type.
 model = rai.Model("socialNetwork")
 Person = model.Type("Person")
@@ -26,8 +24,10 @@
 
 # Create a graph from the model add edges from the `Person.follows` property.
 # The nodes from each edge are automatically added to the graph.
 graph = Graph(model)
 graph.Edge.extend(Person.follows)
 ```
 
-See [`Edges`](../Edges/README.md) for more information.
+## See Also
+
+[`Edge`](../Edge/README.md)
```

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/fetch.md` & `relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/Node.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,50 @@
-# `relationalai.std.graphs.Graph.fetch()`
+# `relationalai.std.graphs.Graph.Node`
 
-```python
-relationalai.std.graphs.Graph.fetch() ->
-```
-
-Returns a dictionary with two keys, `"nodes"` and `"edges"`, that represents the entire graph.
-
-## Parameters
-
-None
+A [`Type`](../../../Type/README.md) object representing the set of nodes in a graph.
 
 ## Returns
 
-A `dict` object.
+A [`Type`](../../../Type/README.md) object.
 
 ## Example
 
 ```python
-from pprint import pprint
-
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
 # Create a model with a `Person` type.
 model = rai.Model("socialNetwork")
 Person = model.Type("Person")
 
 # Add some people to the model and connect them with a `follows` property.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
     alice.set(follows=bob)
 
-# Create a graph with edges from the `Person.follows` property.
+# Create a graph.
 graph = Graph(model)
+
+# Add all of the people in the model to the graph's nodes using `Node.extend()`.
 graph.Node.extend(Person, label=Person.name)
-graph.Edge.extend(Person.follows)
 
-# Fetch the graph.
-pprint(graph.fetch())
+# Alternatively, you can add specific nodes in a rule using `Node.add()`.
+with model.rule():
+    p = Person(name="Alice")
+    graph.Node.add(p, label=p.name)
+
+# You can query the nodes the same way you query any other `Type` object.
+with model.query() as select:
+    node = graph.Node()
+    response = select(node.label)
+
+print(response.results)
 # Output:
-# {'edges': defaultdict(<class 'dict'>,
-#                       {('JCOgZI0tb1qNRTyXYhDFOw', 'v3PMBEmnWi5E2MxI4bGfzQ'): {}}),
-#  'nodes': defaultdict(<class 'dict'>,
-#                       {'JCOgZI0tb1qNRTyXYhDFOw': {'label': 'Alice'},
-#                        'v3PMBEmnWi5E2MxI4bGfzQ': {'label': 'Bob'}})}
+#    label
+# 0  Alice
+# 1    Bob
 ```
 
 ## See Also
 
-[`Graph.visualize()`](./visualize.md)
+[`Type`](../../../Type/README.md)
```

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/id.md` & `relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/id.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/model.md` & `relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/model.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/undirected.md` & `relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/undirected.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/visualize.md` & `relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/visualize.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png` & `relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png` & `relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png` & `relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/docs/api_reference/python/std/graphs/Nodes/extend.md` & `relationalai-0.2.3/docs/api_reference/python/std/graphs/EdgeInstance/to.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,39 @@
-# `relationalai.std.graphs.Nodes.extend()`
+# `relationalai.std.graphs.EdgeInstance.to`
 
-```python
-relationalai.std.graph.Node.extend(type: Type, **kwargs: Any) -> None
-```
-
-Add all objects in a [`Type`](../../../Type/README.md) to the graph's nodes.
-Node properties may be passed as keyword arguments to `**kwargs`.
-You can use and display these properties in graph visualizations.
-
-## Parameters
-
-| Name | Type | Description |
-| :--- | :--- | :------ |
-| `type` | [`Type`](../../../Type/README.md) | The `Type` containing the objects to add to the graph's nodes. |
-| `**kwargs` | `Any` | Keyword arguments representing property name and value pairs. Values may be literals or `Producer` objects. |
-
-## Returns
-
-`None`.
+Returns a `Producer` object that produces the target node(s) of the [`EdgeInstance`](./README.md).
 
 ## Example
 
 ```python
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
 # Create a model with a `Person` type.
-model = rai.Model("socialNetwork")
+model = rai.Model("socialNetwork3")
 Person = model.Type("Person")
 
-# Add some people to the model and connect them with a `follows` property.
+# Add some people to the model and connect them with a 'follows' property.
 with model.rule():
-    Person.add(name="Alice")
-    Person.add(name="Bob")
+    alice = Person.add(name="Alice")
+    bob = Person.add(name="Bob")
+    alice.set(follows=bob)
 
-# Create a graph and extend the nodes with the `Person` type.
+# Create a graph and add edges to it.
 graph = Graph(model)
-graph.Node.extend(Person)
+graph.Edge.extend(Person.follows)
+
+# Display the source nodes of the edges.
+with model.query() as select:
+    edge = graph.Edge()
+    target_node = edge.to
+    response = select(target_node.name)
+
+print(response.results)
+# Output:
+#   name
+# 0  Bob
 ```
 
 ## See Also
 
-[`Edges.add()`](./add.md) and [`Graph.nodes`](../Graph/nodes.md).
+- [`EdgeInstance.from_`](./from_.md)
```

### Comparing `relationalai-0.2.2/examples/README.md` & `relationalai-0.2.3/examples/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/examples/cdc.py` & `relationalai-0.2.3/examples/cdc.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/examples/emit_playground.py` & `relationalai-0.2.3/examples/emit_playground.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/examples/found.py` & `relationalai-0.2.3/examples/found.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/examples/fraud.ipynb` & `relationalai-0.2.3/examples/fraud.ipynb`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/examples/fraud.py` & `relationalai-0.2.3/examples/fraud.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/examples/graph_algos.py` & `relationalai-0.2.3/examples/graph_algos.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/examples/nested.py` & `relationalai-0.2.3/examples/nested.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/examples/or_types.py` & `relationalai-0.2.3/examples/or_types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/examples/remote_load_csv.py` & `relationalai-0.2.3/examples/remote_load_csv.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/examples/simple_recursion.py` & `relationalai-0.2.3/examples/simple_recursion.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/examples/simple_streamlit.py` & `relationalai-0.2.3/examples/simple_streamlit.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/examples/solver.py` & `relationalai-0.2.3/examples/solver.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/examples/weighted_graph_algos.py` & `relationalai-0.2.3/examples/weighted_graph_algos.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/examples/data/people.csv` & `relationalai-0.2.3/examples/data/people.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/examples/data/transactions.csv` & `relationalai-0.2.3/examples/data/transactions.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/examples/ev_penetration/ev_penetration.py` & `relationalai-0.2.3/examples/ev_penetration/ev_penetration.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/examples/ev_penetration/ev_penetration_csv.py` & `relationalai-0.2.3/examples/ev_penetration/ev_penetration_csv.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/examples/ev_penetration/state_stats.csv` & `relationalai-0.2.3/examples/ev_penetration/state_stats.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/examples/imdb/README.md` & `relationalai-0.2.3/examples/imdb/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/examples/imdb/imdb.csv` & `relationalai-0.2.3/examples/imdb/imdb.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/examples/imdb/imdb.py` & `relationalai-0.2.3/examples/imdb/imdb.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/examples/rel/solver.rel` & `relationalai-0.2.3/examples/rel/solver.rel`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/examples/social-money-network/SF_pagerank.ipynb` & `relationalai-0.2.3/examples/social-money-network/SF_pagerank.ipynb`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/examples/social-money-network/Simulation-and-SF-Upload.ipynb` & `relationalai-0.2.3/examples/social-money-network/Simulation-and-SF-Upload.ipynb`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/examples/social-money-network/snowflake_pagerank.py` & `relationalai-0.2.3/examples/social-money-network/snowflake_pagerank.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/frontend/debugger/package-lock.json` & `relationalai-0.2.3/frontend/debugger/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9976468253968254%*

 * *Differences: {"'packages'": "{'': {'dependencies': {'@tabler/icons': '^3.1.0', 'prismjs': '^1.29.0', delete: "*

 * *               "['@tabler/icons-solidjs']}, 'devDependencies': {'@types/prismjs': '^1.26.3', "*

 * *               "'vite-plugin-prismjs': '^0.0.11', 'vite-plugin-solid-svg': '^0.8.1'}}, "*

 * *               "'node_modules/@tabler/icons': {'version': '3.1.0', 'resolved': "*

 * *               "'https://registry.npmjs.org/@tabler/icons/-/icons-3.1.0.tgz', 'integrity': "*

 * *               "'sha512-CpZGyS1IVJKFcv88yZ2sYZIpWWhQ6oy7 […]*

```diff
@@ -1,33 +1,37 @@
 {
     "lockfileVersion": 3,
     "name": "relationalai-debugger-ui",
     "packages": {
         "": {
             "dependencies": {
                 "@kobalte/core": "^0.12.6",
-                "@tabler/icons-solidjs": "2.47.0",
+                "@tabler/icons": "^3.1.0",
+                "prismjs": "^1.29.0",
                 "solid-js": "^1.8.11"
             },
             "devDependencies": {
                 "@chromatic-com/storybook": "^1.2.25",
                 "@storybook/addon-essentials": "^8.0.4",
                 "@storybook/addon-interactions": "^8.0.4",
                 "@storybook/addon-links": "^8.0.4",
                 "@storybook/blocks": "^8.0.4",
                 "@storybook/preview-api": "^8.0.4",
                 "@storybook/testing-library": "^0.2.2",
+                "@types/prismjs": "^1.26.3",
                 "solid-devtools": "^0.29.2",
                 "storybook": "^8.0.4",
                 "storybook-solidjs": "^1.0.0-beta.2",
                 "storybook-solidjs-vite": "^1.0.0-beta.2",
                 "stylus": "^0.63.0",
                 "typescript": "^5.3.3",
                 "vite": "^5.0.11",
-                "vite-plugin-solid": "^2.8.2"
+                "vite-plugin-prismjs": "^0.0.11",
+                "vite-plugin-solid": "^2.8.2",
+                "vite-plugin-solid-svg": "^0.8.1"
             },
             "license": "UNLICENSED",
             "name": "relationalai-debugger-ui",
             "version": "0.0.0"
         },
         "node_modules/@adobe/css-tools": {
             "dev": true,
@@ -4791,32 +4795,17 @@
             "version": "2.6.2"
         },
         "node_modules/@tabler/icons": {
             "funding": {
                 "type": "github",
                 "url": "https://github.com/sponsors/codecalm"
             },
-            "integrity": "sha512-4w5evLh+7FUUiA1GucvGj2ReX2TvOjEr4ejXdwL/bsjoSkof6r1gQmzqI+VHrE2CpJpB3al7bCTulOkFa/RcyA==",
-            "resolved": "https://registry.npmjs.org/@tabler/icons/-/icons-2.47.0.tgz",
-            "version": "2.47.0"
-        },
-        "node_modules/@tabler/icons-solidjs": {
-            "dependencies": {
-                "@tabler/icons": "2.47.0"
-            },
-            "funding": {
-                "type": "github",
-                "url": "https://github.com/sponsors/codecalm"
-            },
-            "integrity": "sha512-qyQau0ViXrYy0ut8ZkLTTvLlbCZi92P5YIlEV7t6f1a5sAN9CMuTcsjrZM60Vf7+6o7tloUgW+VFgc9kwsIBcg==",
-            "peerDependencies": {
-                "solid-js": "^1.4.7"
-            },
-            "resolved": "https://registry.npmjs.org/@tabler/icons-solidjs/-/icons-solidjs-2.47.0.tgz",
-            "version": "2.47.0"
+            "integrity": "sha512-CpZGyS1IVJKFcv88yZ2sYZIpWWhQ6oy76BQKQ5SF0fGgOqgyqKdBGG/YGyyMW632on37MX7VqQIMTzN/uQqmFg==",
+            "resolved": "https://registry.npmjs.org/@tabler/icons/-/icons-3.1.0.tgz",
+            "version": "3.1.0"
         },
         "node_modules/@testing-library/dom": {
             "dependencies": {
                 "@babel/code-frame": "^7.10.4",
                 "@babel/runtime": "^7.12.5",
                 "@types/aria-query": "^5.0.1",
                 "aria-query": "5.1.3",
@@ -5030,14 +5019,23 @@
             "integrity": "sha512-YAh82Wh4TIrxYLmfGcixwD18oIjyC1pFQC2Y01F2lzV2HTMiYrI0nze0FD0ocB//CKS/7jIUgae+adPqxK5yCQ==",
             "peerDependencies": {
                 "@testing-library/dom": ">=7.21.4"
             },
             "resolved": "https://registry.npmjs.org/@testing-library/user-event/-/user-event-14.5.2.tgz",
             "version": "14.5.2"
         },
+        "node_modules/@trysound/sax": {
+            "dev": true,
+            "engines": {
+                "node": ">=10.13.0"
+            },
+            "integrity": "sha512-L7z9BgrNEcYyUYtF+HaEfiS5ebkh9jXqbszz7pC0hRBPaatV0XjSD3+eHrpqFemQfgwiFF0QPIarnIihIDn7OA==",
+            "resolved": "https://registry.npmjs.org/@trysound/sax/-/sax-0.2.0.tgz",
+            "version": "0.2.0"
+        },
         "node_modules/@types/aria-query": {
             "dev": true,
             "integrity": "sha512-rfT93uj5s0PRL7EzccGMs3brplhcrghnDoV26NqKhCAS1hVo+WdNsPvE/yb6ilfr5hi2MEk6d5EWJTKdxg8jVw==",
             "resolved": "https://registry.npmjs.org/@types/aria-query/-/aria-query-5.0.4.tgz",
             "version": "5.0.4"
         },
         "node_modules/@types/babel__core": {
@@ -5219,14 +5217,20 @@
         },
         "node_modules/@types/pretty-hrtime": {
             "dev": true,
             "integrity": "sha512-nj39q0wAIdhwn7DGUyT9irmsKK1tV0bd5WFEhgpqNTMFZ8cE+jieuTphCW0tfdm47S2zVT5mr09B28b1chmQMA==",
             "resolved": "https://registry.npmjs.org/@types/pretty-hrtime/-/pretty-hrtime-1.0.3.tgz",
             "version": "1.0.3"
         },
+        "node_modules/@types/prismjs": {
+            "dev": true,
+            "integrity": "sha512-A0D0aTXvjlqJ5ZILMz3rNfDBOx9hHxLZYv2by47Sm/pqW35zzjusrZTryatjN/Rf8Us2gZrJD+KeHbUSTux1Cw==",
+            "resolved": "https://registry.npmjs.org/@types/prismjs/-/prismjs-1.26.3.tgz",
+            "version": "1.26.3"
+        },
         "node_modules/@types/prop-types": {
             "dev": true,
             "integrity": "sha512-5zvhXYtRNRluoE/jAp4GVsSduVUzNWKkOZrCDBWYtE7biZywwdC2AcEzg+cSMLFRfVgeAFqpfNabiPjxFddV1Q==",
             "resolved": "https://registry.npmjs.org/@types/prop-types/-/prop-types-15.7.12.tgz",
             "version": "15.7.12"
         },
         "node_modules/@types/qs": {
@@ -5735,14 +5739,23 @@
             "integrity": "sha512-JfTApdE++cgcTWjsiCQlLyFBMbTUft9ja17saCc93lgV33h4tuCVj7tlvu//qpLwaG+3yEz7/KhahGrUMkVq9g==",
             "peerDependencies": {
                 "@babel/core": "^7.4.0 || ^8.0.0-0 <8.0.0"
             },
             "resolved": "https://registry.npmjs.org/babel-plugin-polyfill-regenerator/-/babel-plugin-polyfill-regenerator-0.6.1.tgz",
             "version": "0.6.1"
         },
+        "node_modules/babel-plugin-prismjs": {
+            "dev": true,
+            "integrity": "sha512-ehzSKYfeAz4U78zi/sfwsjDPlq0LvDKxNefcZTJ/iKBu+plsHsLqZhUeGf1+82LAcA35UZGbU6ksEx2Utphc/g==",
+            "peerDependencies": {
+                "prismjs": "^1.18.0"
+            },
+            "resolved": "https://registry.npmjs.org/babel-plugin-prismjs/-/babel-plugin-prismjs-2.1.0.tgz",
+            "version": "2.1.0"
+        },
         "node_modules/babel-preset-solid": {
             "dependencies": {
                 "babel-plugin-jsx-dom-expressions": "^0.37.19"
             },
             "dev": true,
             "integrity": "sha512-b4HFg/xaKM+H3Tu5iUlZ/43TJOZnhi85xrm3JrXDQ0s4cmtmU37bXXYzb2m55G4QKiFjxLAjvb7sUorPrAMs5w==",
             "peerDependencies": {
@@ -5880,14 +5893,20 @@
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
             "integrity": "sha512-MvjoMCJwEarSbUYk5O+nmoSzSutSsTwF85zcHPQ9OrlFoZOYIjaqBAJIqIXjptyD5vThxGq52Xu/MaJzRkIk4Q==",
             "resolved": "https://registry.npmjs.org/qs/-/qs-6.11.0.tgz",
             "version": "6.11.0"
         },
+        "node_modules/boolbase": {
+            "dev": true,
+            "integrity": "sha512-JZOSA7Mo9sNGB8+UjSgzdLtokWAky1zbztM3WRLCbZ70/3cTANmQmOdR7y2g+J0e2WXywy1yS468tY+IruqEww==",
+            "resolved": "https://registry.npmjs.org/boolbase/-/boolbase-1.0.0.tgz",
+            "version": "1.0.0"
+        },
         "node_modules/bplist-parser": {
             "dependencies": {
                 "big-integer": "^1.6.44"
             },
             "dev": true,
             "engines": {
                 "node": ">= 5.10.0"
@@ -6413,20 +6432,94 @@
             "engines": {
                 "node": ">=8"
             },
             "integrity": "sha512-v1plID3y9r/lPhviJ1wrXpLeyUIGAZ2SHNYTEapm7/8A9nLPoyvVp3RK/EPFqn5kEznyWgYZNsRtYYIWbuG8KA==",
             "resolved": "https://registry.npmjs.org/crypto-random-string/-/crypto-random-string-2.0.0.tgz",
             "version": "2.0.0"
         },
+        "node_modules/css-select": {
+            "dependencies": {
+                "boolbase": "^1.0.0",
+                "css-what": "^6.1.0",
+                "domhandler": "^5.0.2",
+                "domutils": "^3.0.1",
+                "nth-check": "^2.0.1"
+            },
+            "dev": true,
+            "funding": {
+                "url": "https://github.com/sponsors/fb55"
+            },
+            "integrity": "sha512-nwoRF1rvRRnnCqqY7updORDsuqKzqYJ28+oSMaJMMgOauh3fvwHqMS7EZpIPqK8GL+g9mKxF1vP/ZjSeNjEVHg==",
+            "resolved": "https://registry.npmjs.org/css-select/-/css-select-5.1.0.tgz",
+            "version": "5.1.0"
+        },
+        "node_modules/css-tree": {
+            "dependencies": {
+                "mdn-data": "2.0.30",
+                "source-map-js": "^1.0.1"
+            },
+            "dev": true,
+            "engines": {
+                "node": "^10 || ^12.20.0 || ^14.13.0 || >=15.0.0"
+            },
+            "integrity": "sha512-6Fv1DV/TYw//QF5IzQdqsNDjx/wc8TrMBZsqjL9eW01tWb7R7k/mq+/VXfJCl7SoD5emsJop9cOByJZfs8hYIw==",
+            "resolved": "https://registry.npmjs.org/css-tree/-/css-tree-2.3.1.tgz",
+            "version": "2.3.1"
+        },
+        "node_modules/css-what": {
+            "dev": true,
+            "engines": {
+                "node": ">= 6"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/fb55"
+            },
+            "integrity": "sha512-HTUrgRJ7r4dsZKU6GjmpfRK1O76h97Z8MfS1G0FozR+oF2kG6Vfe8JE6zwrkbxigziPHinCJ+gCPjA9EaBDtRw==",
+            "resolved": "https://registry.npmjs.org/css-what/-/css-what-6.1.0.tgz",
+            "version": "6.1.0"
+        },
         "node_modules/css.escape": {
             "dev": true,
             "integrity": "sha512-YUifsXXuknHlUsmlgyY0PKzgPOr7/FjCePfHNt0jxm83wHZi44VDMQ7/fGNkjY3/jV1MC+1CmZbaHzugyeRtpg==",
             "resolved": "https://registry.npmjs.org/css.escape/-/css.escape-1.5.1.tgz",
             "version": "1.5.1"
         },
+        "node_modules/csso": {
+            "dependencies": {
+                "css-tree": "~2.2.0"
+            },
+            "dev": true,
+            "engines": {
+                "node": "^10 || ^12.20.0 || ^14.13.0 || >=15.0.0",
+                "npm": ">=7.0.0"
+            },
+            "integrity": "sha512-0LrrStPOdJj+SPCCrGhzryycLjwcgUSHBtxNA8aIDxf0GLsRh1cKYhB00Gd1lDOS4yGH69+SNn13+TWbVHETFQ==",
+            "resolved": "https://registry.npmjs.org/csso/-/csso-5.0.5.tgz",
+            "version": "5.0.5"
+        },
+        "node_modules/csso/node_modules/css-tree": {
+            "dependencies": {
+                "mdn-data": "2.0.28",
+                "source-map-js": "^1.0.1"
+            },
+            "dev": true,
+            "engines": {
+                "node": "^10 || ^12.20.0 || ^14.13.0 || >=15.0.0",
+                "npm": ">=7.0.0"
+            },
+            "integrity": "sha512-OA0mILzGc1kCOCSJerOeqDxDQ4HOh+G8NbOJFOTgOCzpw7fCBubk0fEyxp8AgOL/jvLgYA/uV0cMbe43ElF1JA==",
+            "resolved": "https://registry.npmjs.org/css-tree/-/css-tree-2.2.1.tgz",
+            "version": "2.2.1"
+        },
+        "node_modules/csso/node_modules/mdn-data": {
+            "dev": true,
+            "integrity": "sha512-aylIc7Z9y4yzHYAJNuESG3hfhC+0Ibp/MAMiaOZgNv4pmEdFyfZhhhny4MNiAfWdBQ1RQ2mfDWmM1x8SvGyp8g==",
+            "resolved": "https://registry.npmjs.org/mdn-data/-/mdn-data-2.0.28.tgz",
+            "version": "2.0.28"
+        },
         "node_modules/csstype": {
             "integrity": "sha512-M1uQkMl8rQK/szD0LNhtqxIPLpimGm8sOBwU7lLnCpSbTyY3yeU1Vc7l4KT5zT4s/yOxHH5O7tIuuLOCnLADRw==",
             "resolved": "https://registry.npmjs.org/csstype/-/csstype-3.1.3.tgz",
             "version": "3.1.3"
         },
         "node_modules/debug": {
             "dependencies": {
@@ -6701,14 +6794,69 @@
         },
         "node_modules/dom-accessibility-api": {
             "dev": true,
             "integrity": "sha512-X7BJ2yElsnOJ30pZF4uIIDfBEVgF4XEBxL9Bxhy6dnrm5hkzqmsWHGTiHqRiITNhMyFLyAiWndIJP7Z1NTteDg==",
             "resolved": "https://registry.npmjs.org/dom-accessibility-api/-/dom-accessibility-api-0.5.16.tgz",
             "version": "0.5.16"
         },
+        "node_modules/dom-serializer": {
+            "dependencies": {
+                "domelementtype": "^2.3.0",
+                "domhandler": "^5.0.2",
+                "entities": "^4.2.0"
+            },
+            "dev": true,
+            "funding": {
+                "url": "https://github.com/cheeriojs/dom-serializer?sponsor=1"
+            },
+            "integrity": "sha512-wIkAryiqt/nV5EQKqQpo3SToSOV9J0DnbJqwK7Wv/Trc92zIAYZ4FlMu+JPFW1DfGFt81ZTCGgDEabffXeLyJg==",
+            "resolved": "https://registry.npmjs.org/dom-serializer/-/dom-serializer-2.0.0.tgz",
+            "version": "2.0.0"
+        },
+        "node_modules/domelementtype": {
+            "dev": true,
+            "funding": [
+                {
+                    "type": "github",
+                    "url": "https://github.com/sponsors/fb55"
+                }
+            ],
+            "integrity": "sha512-OLETBj6w0OsagBwdXnPdN0cnMfF9opN69co+7ZrbfPGrdpPVNBUj02spi6B1N7wChLQiPn4CSH/zJvXw56gmHw==",
+            "resolved": "https://registry.npmjs.org/domelementtype/-/domelementtype-2.3.0.tgz",
+            "version": "2.3.0"
+        },
+        "node_modules/domhandler": {
+            "dependencies": {
+                "domelementtype": "^2.3.0"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">= 4"
+            },
+            "funding": {
+                "url": "https://github.com/fb55/domhandler?sponsor=1"
+            },
+            "integrity": "sha512-cgwlv/1iFQiFnU96XXgROh8xTeetsnJiDsTc7TYCLFd9+/WNkIqPTxiM/8pSd8VIrhXGTf1Ny1q1hquVqDJB5w==",
+            "resolved": "https://registry.npmjs.org/domhandler/-/domhandler-5.0.3.tgz",
+            "version": "5.0.3"
+        },
+        "node_modules/domutils": {
+            "dependencies": {
+                "dom-serializer": "^2.0.0",
+                "domelementtype": "^2.3.0",
+                "domhandler": "^5.0.3"
+            },
+            "dev": true,
+            "funding": {
+                "url": "https://github.com/fb55/domutils?sponsor=1"
+            },
+            "integrity": "sha512-H78uMmQtI2AhgDJjWeQmHwJJ2bLPD3GMmO7Zja/ZZh84wkm+4ut+IUnUdRa8uCGX88DiVx1j6FRe1XfxEgjEZA==",
+            "resolved": "https://registry.npmjs.org/domutils/-/domutils-3.1.0.tgz",
+            "version": "3.1.0"
+        },
         "node_modules/dotenv": {
             "dev": true,
             "engines": {
                 "node": ">=12"
             },
             "funding": {
                 "url": "https://dotenvx.com"
@@ -6821,14 +6969,26 @@
                 "once": "^1.4.0"
             },
             "dev": true,
             "integrity": "sha512-+uw1inIHVPQoaVuHzRyXd21icM+cnt4CzD5rW+NC1wjOUSTOs+Te7FOv7AhN7vS9x/oIyhLP5PR1H+phQAHu5Q==",
             "resolved": "https://registry.npmjs.org/end-of-stream/-/end-of-stream-1.4.4.tgz",
             "version": "1.4.4"
         },
+        "node_modules/entities": {
+            "dev": true,
+            "engines": {
+                "node": ">=0.12"
+            },
+            "funding": {
+                "url": "https://github.com/fb55/entities?sponsor=1"
+            },
+            "integrity": "sha512-V0hjH4dGPh9Ao5p0MoRY6BVqtwCjhz6vI5LT8AJ55H+4g9/4vbHx1I54fS0XuclLhDHArPQCiMjDxjaL8fPxhw==",
+            "resolved": "https://registry.npmjs.org/entities/-/entities-4.5.0.tgz",
+            "version": "4.5.0"
+        },
         "node_modules/envinfo": {
             "bin": {
                 "envinfo": "dist/cli.js"
             },
             "dev": true,
             "engines": {
                 "node": ">=4"
@@ -8975,14 +9135,20 @@
             "integrity": "sha512-B+28F5ucp83aQm+OxNrPkS8z0tMKaeHiy0lHJs3LqCyDQFtWuenaIrkaVTgAm1pf1AU85LXltva86hlaT17i8Q==",
             "peerDependencies": {
                 "react": ">= 0.14.0"
             },
             "resolved": "https://registry.npmjs.org/markdown-to-jsx/-/markdown-to-jsx-7.3.2.tgz",
             "version": "7.3.2"
         },
+        "node_modules/mdn-data": {
+            "dev": true,
+            "integrity": "sha512-GaqWWShW4kv/G9IEucWScBx9G1/vsFZZJUO+tD26M8J8z3Kw5RDQjaoZe03YAClgeS/SWPOcb4nkFBTEi5DUEA==",
+            "resolved": "https://registry.npmjs.org/mdn-data/-/mdn-data-2.0.30.tgz",
+            "version": "2.0.30"
+        },
         "node_modules/media-typer": {
             "dev": true,
             "engines": {
                 "node": ">= 0.6"
             },
             "integrity": "sha512-dq+qelQ9akHpcOl/gUVRTxVIOkAJ1wR3QAvb4RsVjS8oVoFjDGTc679wJYmUmknUF5HwMLOgb5O+a3KxfWapPQ==",
             "resolved": "https://registry.npmjs.org/media-typer/-/media-typer-0.3.0.tgz",
@@ -9306,14 +9472,26 @@
             "engines": {
                 "node": ">=8"
             },
             "integrity": "sha512-S48WzZW777zhNIrn7gxOlISNAqi9ZC/uQFnRdbeIHhZhCA6UqpkOT8T1G7BvfdgP4Er8gF4sUbaS0i7QvIfCWw==",
             "resolved": "https://registry.npmjs.org/npm-run-path/-/npm-run-path-4.0.1.tgz",
             "version": "4.0.1"
         },
+        "node_modules/nth-check": {
+            "dependencies": {
+                "boolbase": "^1.0.0"
+            },
+            "dev": true,
+            "funding": {
+                "url": "https://github.com/fb55/nth-check?sponsor=1"
+            },
+            "integrity": "sha512-lqjrjmaOoAnWfMmBPL+XNnynZh2+swxiX3WUE0s4yEHI6m+AwrK2UZOimIRl3X/4QctVqS8AiZjFqyOGrMXb/w==",
+            "resolved": "https://registry.npmjs.org/nth-check/-/nth-check-2.1.1.tgz",
+            "version": "2.1.1"
+        },
         "node_modules/nypm": {
             "bin": {
                 "nypm": "dist/cli.mjs"
             },
             "dependencies": {
                 "citty": "^0.1.6",
                 "consola": "^3.2.3",
@@ -10017,14 +10195,22 @@
             "engines": {
                 "node": ">= 0.8"
             },
             "integrity": "sha512-66hKPCr+72mlfiSjlEB1+45IjXSqvVAIy6mocupoww4tBFE9R9IhwwUGoI4G++Tc9Aq+2rxOt0RFU6gPcrte0A==",
             "resolved": "https://registry.npmjs.org/pretty-hrtime/-/pretty-hrtime-1.0.3.tgz",
             "version": "1.0.3"
         },
+        "node_modules/prismjs": {
+            "engines": {
+                "node": ">=6"
+            },
+            "integrity": "sha512-Kx/1w86q/epKcmte75LNrEoT+lX8pBpavuAbvJWRXar7Hz8jrtF+e3vY751p0R8H9HdArwaCTNDDzHg/ScJK1Q==",
+            "resolved": "https://registry.npmjs.org/prismjs/-/prismjs-1.29.0.tgz",
+            "version": "1.29.0"
+        },
         "node_modules/process": {
             "dev": true,
             "engines": {
                 "node": ">= 0.6.0"
             },
             "integrity": "sha512-cdGef/drWFoydD1JsMzuFf8100nZl+GT+yacc2bEced5f9Rjk4z+WtFUTBu9PhOi9j/jfmBPu0mMEY4wIdAF8A==",
             "resolved": "https://registry.npmjs.org/process/-/process-0.11.10.tgz",
@@ -11284,14 +11470,48 @@
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
             "integrity": "sha512-ot0WnXS9fgdkgIcePe6RHNk1WA8+muPa6cSjeR3V8K27q9BB1rTE3R1p7Hv0z1ZyAc8s6Vvv8DIyWf681MAt0w==",
             "resolved": "https://registry.npmjs.org/supports-preserve-symlinks-flag/-/supports-preserve-symlinks-flag-1.0.0.tgz",
             "version": "1.0.0"
         },
+        "node_modules/svgo": {
+            "bin": {
+                "svgo": "bin/svgo"
+            },
+            "dependencies": {
+                "@trysound/sax": "0.2.0",
+                "commander": "^7.2.0",
+                "css-select": "^5.1.0",
+                "css-tree": "^2.3.1",
+                "css-what": "^6.1.0",
+                "csso": "^5.0.5",
+                "picocolors": "^1.0.0"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">=14.0.0"
+            },
+            "funding": {
+                "type": "opencollective",
+                "url": "https://opencollective.com/svgo"
+            },
+            "integrity": "sha512-4PP6CMW/V7l/GmKRKzsLR8xxjdHTV4IMvhTnpuHwwBazSIlw5W/5SmPjN8Dwyt7lKbSJrRDgp4t9ph0HgChFBQ==",
+            "resolved": "https://registry.npmjs.org/svgo/-/svgo-3.2.0.tgz",
+            "version": "3.2.0"
+        },
+        "node_modules/svgo/node_modules/commander": {
+            "dev": true,
+            "engines": {
+                "node": ">= 10"
+            },
+            "integrity": "sha512-QrWXB+ZQSVPmIWIhtEO9H+gwHaMGYiF5ChvoJ+K9ZGHG/sVsa6yiesAD1GC/x46sET00Xlwo1u49RVVVzvcSkw==",
+            "resolved": "https://registry.npmjs.org/commander/-/commander-7.2.0.tgz",
+            "version": "7.2.0"
+        },
         "node_modules/tar": {
             "dependencies": {
                 "chownr": "^2.0.0",
                 "fs-minipass": "^2.0.0",
                 "minipass": "^5.0.0",
                 "minizlib": "^2.1.1",
                 "mkdirp": "^1.0.3",
@@ -11879,14 +12099,27 @@
                 "terser": {
                     "optional": true
                 }
             },
             "resolved": "https://registry.npmjs.org/vite/-/vite-5.2.6.tgz",
             "version": "5.2.6"
         },
+        "node_modules/vite-plugin-prismjs": {
+            "dependencies": {
+                "@babel/core": "^7.15.5",
+                "babel-plugin-prismjs": "^2.1.0"
+            },
+            "dev": true,
+            "engines": {
+                "node": ">=12.0.0"
+            },
+            "integrity": "sha512-20NBQxg/zH+3FTrlU6BQTob720xkuXNYtrx7psAQ4E6pMcRDeLEK77QU9kXURU587+f2To7ASH1JVTGbXVV/vQ==",
+            "resolved": "https://registry.npmjs.org/vite-plugin-prismjs/-/vite-plugin-prismjs-0.0.11.tgz",
+            "version": "0.0.11"
+        },
         "node_modules/vite-plugin-solid": {
             "dependencies": {
                 "@babel/core": "^7.23.3",
                 "@types/babel__core": "^7.20.4",
                 "babel-preset-solid": "^1.8.4",
                 "merge-anything": "^5.1.7",
                 "solid-refresh": "^0.6.3",
@@ -11903,14 +12136,27 @@
                 "@testing-library/jest-dom": {
                     "optional": true
                 }
             },
             "resolved": "https://registry.npmjs.org/vite-plugin-solid/-/vite-plugin-solid-2.10.2.tgz",
             "version": "2.10.2"
         },
+        "node_modules/vite-plugin-solid-svg": {
+            "dependencies": {
+                "svgo": "^3.1.0"
+            },
+            "dev": true,
+            "integrity": "sha512-ROGC2ae1eYUCMd+zfJtsbUtuZwsb6DZS0+Sy5/ZXDokOunGi0Ez/cL7OPdsixN3I0/rNYd/3hilo3kpRMAS+IA==",
+            "peerDependencies": {
+                "solid-js": "^1",
+                "vite": ">=4"
+            },
+            "resolved": "https://registry.npmjs.org/vite-plugin-solid-svg/-/vite-plugin-solid-svg-0.8.1.tgz",
+            "version": "0.8.1"
+        },
         "node_modules/vitefu": {
             "dev": true,
             "integrity": "sha512-SgHtMLoqaeeGnd2evZ849ZbACbnwQCIwRH57t18FxcXoZop0uQu0uzlIhJBlF/eWVzuce0sHeqPcDo+evVcg8Q==",
             "peerDependencies": {
                 "vite": "^3.0.0 || ^4.0.0 || ^5.0.0"
             },
             "peerDependenciesMeta": {
```

### Comparing `relationalai-0.2.2/frontend/debugger/package.json` & `relationalai-0.2.3/frontend/debugger/package.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9452380952380953%*

 * *Differences: {"'dependencies'": "{'@tabler/icons': '^3.1.0', 'prismjs': '^1.29.0', delete: "*

 * *                   "['@tabler/icons-solidjs']}",*

 * * "'devDependencies'": "{'@types/prismjs': '^1.26.3', 'vite-plugin-prismjs': '^0.0.11', "*

 * *                      "'vite-plugin-solid-svg': '^0.8.1'}"}*

```diff
@@ -1,30 +1,34 @@
 {
     "dependencies": {
         "@kobalte/core": "^0.12.6",
-        "@tabler/icons-solidjs": "2.47.0",
+        "@tabler/icons": "^3.1.0",
+        "prismjs": "^1.29.0",
         "solid-js": "^1.8.11"
     },
     "description": "",
     "devDependencies": {
         "@chromatic-com/storybook": "^1.2.25",
         "@storybook/addon-essentials": "^8.0.4",
         "@storybook/addon-interactions": "^8.0.4",
         "@storybook/addon-links": "^8.0.4",
         "@storybook/blocks": "^8.0.4",
         "@storybook/preview-api": "^8.0.4",
         "@storybook/testing-library": "^0.2.2",
+        "@types/prismjs": "^1.26.3",
         "solid-devtools": "^0.29.2",
         "storybook": "^8.0.4",
         "storybook-solidjs": "^1.0.0-beta.2",
         "storybook-solidjs-vite": "^1.0.0-beta.2",
         "stylus": "^0.63.0",
         "typescript": "^5.3.3",
         "vite": "^5.0.11",
-        "vite-plugin-solid": "^2.8.2"
+        "vite-plugin-prismjs": "^0.0.11",
+        "vite-plugin-solid": "^2.8.2",
+        "vite-plugin-solid-svg": "^0.8.1"
     },
     "license": "UNLICENSED",
     "name": "relationalai-debugger-ui",
     "scripts": {
         "build": "vite build",
         "build-storybook": "storybook build",
         "dev": "vite",
```

### Comparing `relationalai-0.2.2/frontend/debugger/src/App.tsx` & `relationalai-0.2.3/frontend/debugger/src/App.tsx`

 * *Files 20% similar despite different names*

```diff
@@ -1,113 +1,109 @@
-import { Component, For, Setter, Show, createSignal } from "solid-js";
-import { IconAntennaBars5, IconAntennaBarsOff, IconBan, IconSettings, IconX } from "@tabler/icons-solidjs";
-import { blocks, clear_messages, connection, is_compilation } from "./debugger_client";
-import type { Block } from "./debugger_client";
-import { Machine } from "./components/Schematic";
+import { Show, createEffect, createSignal } from "solid-js";
+import { EventListSelection, Selection } from "./Selection";
+import { EventList } from "./components/EventList";
+import { EventViewer } from "./components/EventViewer";
 import { Sidebar } from "./components/Sidebar";
-import { Button } from "./components/Button";
-import { Tooltip } from "./components/Tooltip";
-import "./app.styl";
-import { Modal } from "./components/Modal";
-import { Format, Field } from "./components/Field";
+import { Button } from "./components/ui/Button";
+import { Field, Format } from "./components/ui/Field";
+import { Icon } from "./components/ui/Icon";
+import { Modal } from "./components/ui/Modal";
+import { Tooltip } from "./components/ui/Tooltip";
+import { client, get_in, type Subject } from "./debugger_client";
+import "./App.styl";
 
+function App() {
+    const event_list_selection = new Selection<Subject>("EventList");
 
-const App: Component = () => {
-    const [block, set_block] = createSignal<Block>()
     const clear = () => {
-        set_block(undefined);
-        clear_messages();
+        client.connection.disconnect();
+        event_list_selection.clear()
+        client.clear();
     };
+
+    const [pinned, set_pinned] = createSignal<boolean>(true);
+
+    createEffect((prev_len: number|undefined) => {
+        const cur_len = client.spans().length;
+        const cur = event_list_selection.primary();
+        if (pinned() && cur_len !== prev_len && cur) {
+            event_list_selection.select({ event: "placeholder", selection_path: [cur_len - 1, ...cur.selection_path.slice(1)] })
+        }
+        return cur_len;
+    });
+
+    createEffect(() => {
+        let selected = event_list_selection.primary();
+        if (selected?.event === "placeholder") {
+            let available = get_in(client.root, selected.selection_path);
+            if(available) {
+                event_list_selection.select(available);
+            }
+        }
+    });
+
     return (
-        <app-chrome>
-            <Sidebar class="left" defaultOpen>
-                <header>
-                    <Modal title="Settings" content={<Settings />}>
-                      <Modal.Trigger as={Button} class="icon" tooltip="settings">
-                        <IconSettings />
-                      </Modal.Trigger>
-                    </Modal>
-                    <span style="flex: 1">
-                        {blocks().length} events
-                    </span>
-                    <Tooltip content={connection.connected() ? "Connected to program" : "Disconnected from program"}>
-                        <Tooltip.Trigger as="span">
-                            <Show when={connection.connected()} fallback={<IconAntennaBarsOff />}>
-                                <IconAntennaBars5 />
-                            </Show>
-                        </Tooltip.Trigger>
-                    </Tooltip>
-                    <Button class="icon" onclick={clear} tooltip="clear events">
-                        <IconBan />
-                    </Button>
-                </header>
-                <search-bar>
-                    {/* @TODO: Combine list + fuzzy searcher into component for selection (?) */}
-                    <input placeholder="search..." />
-                </search-bar>
-                <event-list>
-                    <For each={blocks()}>
-                        {(block) => <BlockItem block={block} select={set_block} />}
-                    </For>
-                </event-list>
-            </Sidebar>
-            <main>
-                <app-scroller>
-                    <Show when={block()}>
-                        <Machine machine={block()!.mech} />
+        <EventListSelection.Provider value={event_list_selection}>
+            <app-chrome>
+                <Sidebar side="left" defaultOpen>
+                    <header>
+                        <Button class="icon" onclick={clear} tooltip="clear events">
+                            <Icon name="ban" />
+                        </Button>
+                        <Button class="icon" tooltip="Follow last run" onclick={() => set_pinned(v => !v)}>
+                            <Icon name="pin" type={pinned() ? "filled" : "outline"} />
+                        </Button>
+                        <span style="flex: 1" />
+                        <Modal title="Settings" content={<Settings />}>
+                            <Modal.Trigger as={Button} class="icon" tooltip="settings">
+                                <Icon name="settings" />
+                            </Modal.Trigger>
+                        </Modal>
+                    </header>
+                    <EventList events={client.spans()} />
+                </Sidebar>
+                <main>
+                    <Show when={event_list_selection.primary()}>
+                        <EventViewer subject={event_list_selection.primary()!} />
+                    </Show>
+                    <Show when={event_list_selection.primary()?.event === "placeholder"}>
+                        <app-scroller>
+
+                        </app-scroller>
                     </Show>
-                </app-scroller>
-            </main>
-            <Show when={block()}>
-              <Sidebar class="right">
-                details
-              </Sidebar>
-            </Show>
-        </app-chrome>
+                </main>
+                <Status />
+            </app-chrome>
+        </EventListSelection.Provider>
     );
 };
 
 export default App;
 
-export function Settings() {
-    /* const [poll_interval, _set_poll_interval] = createSignal(connection.reconnectInterval);
-  * const set_poll_interval = (value: number) => {
-  *   let v = (!isNaN(value) && value >= 1) ? value : 1;
-  *   connection.reconnectInterval = v * 1000;
-  *   _set_poll_interval(v * 1000);
-  * }; */
+function Status() {
+    return (
+        <Tooltip content={client.connected() ? "Connected to program" : "Disconnected from program"}>
+            <Tooltip.Trigger as="status-icon">
+                <Show when={client.connected()} fallback={<Icon name="antenna-bars-off" />}>
+                    <Icon name="antenna-bars-5" />
+                </Show>
+            </Tooltip.Trigger>
+        </Tooltip>
+    )
+}
 
 
-  return (
+export function Settings() {
+    return (
         <>
             <section>
                 <h3>Connection</h3>
                 <Field.Number label="Polling Interval" formatOptions={Format.seconds} minValue={1}
-                              defaultValue={connection.reconnectInterval / 1000}
-                              onRawValueChange={(v) => connection.reconnectInterval = v * 1000} />
+                    defaultValue={client.connection.reconnectInterval / 1000}
+                    onRawValueChange={(v) => client.connection.reconnectInterval = v * 1000} />
                 <Field.Text label={"Debug URL"} placeholder={"ws://localhost:1234"}
-                            defaultValue={connection.ws_url} onChange={(v) => connection.ws_url = v} />
+                    defaultValue={client.connection.ws_url} onChange={(v) => client.connection.ws_url = v} />
             </section>
 
         </>
     )
 }
-
-export interface BlockProps {
-    block: Block,
-    select: Setter<Block | undefined>
-}
-export function BlockItem(props: BlockProps) {
-    let compilation = () => props.block.events.find(is_compilation);
-    let source = () => compilation()?.source;
-    return (
-        <block-item onclick={() => props.select(props.block)}>
-            <header>
-                <span class="file">{source()?.file}</span>
-                <span class="line">L{source()?.line}</span>
-            </header>
-            <code>
-                {source()?.block}
-            </code>
-        </block-item>
-    )
-}
```

### Comparing `relationalai-0.2.2/frontend/debugger/src/logo.svg` & `relationalai-0.2.3/frontend/debugger/src/logo.svg`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/frontend/debugger/src/util.styl` & `relationalai-0.2.3/frontend/debugger/src/util.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/frontend/debugger/src/components/Button.tsx` & `relationalai-0.2.3/frontend/debugger/src/components/ui/Button.tsx`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import {Button as KButton} from "@kobalte/core";
-import type { ButtonRootProps } from "@kobalte/core/dist/types/button";
 import { JSXElement, Match, Switch, splitProps } from "solid-js";
 import {Tooltip} from "./Tooltip";
 import "./Button.styl";
 
-export interface ButtonProps extends ButtonRootProps {
+export interface ButtonProps extends KButton.ButtonRootProps {
     tooltip?: JSXElement
 }
 export function Button(props: ButtonProps) {
-    const [local, remote] = splitProps(props, ["tooltip"]);
+    const [local, remote] = splitProps(props, ["class", "tooltip"]);
     return (
         <Switch>
             <Match when={local.tooltip}>
                 <Tooltip content={local.tooltip}>
-                    <Tooltip.Trigger as={KButton.Root} {...remote} />
+                    <Tooltip.Trigger as={KButton.Root} class={`ui-button ${local.class || ""}`} {...remote} />
                 </Tooltip>
             </Match>
             <Match when={true}>
-                <KButton.Root {...remote} />
+                <KButton.Root class={`ui-button ${local.class || ""}`} {...remote} />
             </Match>
         </Switch>
     )
 }
```

### Comparing `relationalai-0.2.2/frontend/debugger/src/components/Field.stories.tsx` & `relationalai-0.2.3/frontend/debugger/src/components/ui/Field.stories.tsx`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import type {Meta, StoryObj} from "storybook-solidjs";
 import {NumberField, TextField} from "./Field";
-import "../app.styl";
 import { createSignal } from "solid-js";
 
 const meta: Meta<typeof NumberField> = {
     component: NumberField,
 }
 
 export default meta;
```

### Comparing `relationalai-0.2.2/frontend/debugger/src/components/Field.tsx` & `relationalai-0.2.3/frontend/debugger/src/components/ui/Field.tsx`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import { NumberField as KNumberField, TextField as KTextField } from "@kobalte/core";
-import type { NumberFieldRootProps, } from "@kobalte/core/dist/types/number-field";
-import type { TextFieldRootProps } from "@kobalte/core/dist/types/text-field";
-import { IconCaretDownFilled, IconCaretUpFilled } from "@tabler/icons-solidjs";
 import { JSXElement, Show, splitProps } from "solid-js";
 import "./Field.styl";
+import { Icon } from "./Icon";
+import { Button } from "./Button";
 
 //------------------------------------------------------------------------------
 // Common Formats
 //------------------------------------------------------------------------------
 
 function coerce<const T extends Record<string, Intl.NumberFormatOptions>>(v: T) {
     return v;
@@ -23,61 +22,61 @@
     }
 })
 
 //------------------------------------------------------------------------------
 // NumberField
 //------------------------------------------------------------------------------
 
-export interface NumberFieldProps extends NumberFieldRootProps {
+export interface NumberFieldProps extends KNumberField.NumberFieldRootProps {
     label: JSXElement,
     placeholder?: string
 }
 export function NumberField(props: NumberFieldProps) {
     let [local, remote] = splitProps(props, ["label", "class", "placeholder"]);
     return (
-        <KNumberField.Root {...remote} class={`field number ${local.class ?? ""}`}>
+        <KNumberField.Root {...remote} class={`ui-field number ${local.class ?? ""}`}>
             <KNumberField.Label>{local.label}</KNumberField.Label>
             <KNumberField.HiddenInput />
-            <span class="field-input">
-                <KNumberField.Input class="field-input-value" placeholder={local.placeholder} />
-                <div class="field-controls">
-                    <KNumberField.IncrementTrigger class="icon field-input-increment">
-                        <IconCaretUpFilled size="0.66em" />
+            <span class="ui-field-input">
+                <KNumberField.Input class="ui-field-value" placeholder={local.placeholder} />
+                <div class="ui-field-controls">
+                    <KNumberField.IncrementTrigger as={Button} class="icon ui-field-input-increment">
+                        <Icon name="chevron-up" size="0.9em" />
                     </KNumberField.IncrementTrigger>
-                    <KNumberField.DecrementTrigger class="icon field-input-decrement">
-                        <IconCaretDownFilled size="0.66em" />
+                    <KNumberField.DecrementTrigger as={Button} class="icon ui-field-input-decrement">
+                        <Icon name="chevron-down" size="0.9em" />
                     </KNumberField.DecrementTrigger>
                 </div>
             </span>
         </KNumberField.Root>
     )
 }
 
 //------------------------------------------------------------------------------
 // TextField
 //------------------------------------------------------------------------------
 
-export interface TextFieldProps extends TextFieldRootProps {
+export interface TextFieldProps extends KTextField.TextFieldRootProps {
     label: JSXElement,
     type?: string,
     placeholder?: string,
     multiline?: boolean,
     children?: JSXElement,
 }
 export function TextField(props: TextFieldProps) {
     let [local, remote] = splitProps(props, ["label", "type", "class", "placeholder", "multiline", "children"]);
     return (
-        <KTextField.Root {...remote} class={`field ${local.type ?? "text"} ${local.class ?? ""}`}>
+        <KTextField.Root {...remote} class={`ui-field ${local.type ?? "text"} ${local.class ?? ""}`}>
             <KTextField.Label>{local.label}</KTextField.Label>
-            <span class="field-input">
+            <span class="ui-field-input">
                 <Show when={!local.multiline}>
-                    <KTextField.Input class="field-input-value" placeholder={local.placeholder} />
+                    <KTextField.Input class="ui-field-value" placeholder={local.placeholder} />
                 </Show>
                 <Show when={local.multiline}>
-                    <KTextField.TextArea class="field-input-value multiline" placeholder={local.placeholder} />
+                    <KTextField.TextArea class="ui-field-value multiline" placeholder={local.placeholder} />
                 </Show>
             </span>
             {local.children}
         </KTextField.Root>
     )
 }
 TextField.Description = KTextField.Description;
```

### Comparing `relationalai-0.2.2/frontend/debugger/src/components/Modal.stories.tsx` & `relationalai-0.2.3/frontend/debugger/src/components/ui/Modal.stories.tsx`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 import type {Meta, StoryObj} from "storybook-solidjs";
 import {Modal} from "./Modal";
-import { Button } from "./Button";
-import "../app.styl";
-import { IconX } from "@tabler/icons-solidjs";
 
 const meta: Meta<typeof Modal> = {
     component: Modal,
 }
 
 export default meta;
```

### Comparing `relationalai-0.2.2/frontend/debugger/src/components/Modal.styl` & `relationalai-0.2.3/frontend/debugger/src/components/ui/Modal.styl`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,45 @@
-.modal {
-  --modal-bg: #f9f9f9;
-  --modal-overlay-bg: #00091011;
-  --modal-border: oklch(from var(--modal-bg) calc(l * 0.75) c h);
-  --modal-anim-open-duration: 0.1s;
-  --modal-anim-close-duration: 0.2s;
+:root {
+  --modal-bg: var(--section-bg);
+  --modal-border: var(--section-border);
+  --modal-shadow: var(--shadow);
+  --modal-overlay-bg: var(--shadow);
 
+  --modal-anim-open-duration: var(--anim-duration-normal);
+  --modal-anim-close-duration: var(--anim-duration-slow);
+}
+
+.ui-modal {
   display: flex;
   flex-direction: column;
   align-items: center;
   justify-content: center;
 
-  &, .modal-overlay {
+  &, .ui-modal-overlay {
     position: absolute;
     top: 0; left: 0; right: 0; bottom: 0;
   }
 
-  .modal-overlay {
+  .ui-modal-overlay {
     background: var(--modal-overlay-bg);
   }
 
-  .modal-content {
+  .ui-modal-content {
     position: relative;
     padding: 12px;
     max-width: min(calc(100vw - 16px), 380px);
 
     background: var(--modal-bg);
     border-radius: 4px;
     border: 1px solid var(--modal-border);
-    box-shadow: 1px 4px 11px #00091033;
+    box-shadow: 1px 4px 11px var(--modal-shadow);
     z-index: 40;
   }
 
-  .modal-header {
+  .ui-modal-header {
     margin-bottom: 20px;
   }
 
-  .modal-title {
+  .ui-modal-title {
     flex: 1;
   }
 }
```

### Comparing `relationalai-0.2.2/frontend/debugger/src/components/Modal.tsx` & `relationalai-0.2.3/frontend/debugger/src/components/ui/Modal.tsx`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 import { Dialog as KDialog } from "@kobalte/core";
-import type { DialogRootProps } from "@kobalte/core/dist/types/dialog";
-import { IconX } from "@tabler/icons-solidjs";
 import { JSXElement, splitProps } from "solid-js";
 import { Button } from "./Button";
 import "./Modal.styl";
+import { Icon } from "./Icon";
 
-export interface ModalProps extends DialogRootProps {
+export interface ModalProps extends KDialog.DialogRootProps {
     title?: string,
     class?: string,
     content?: JSXElement,
 }
 export function Modal(props: ModalProps) {
     const [local, remote] = splitProps(props, ["title", "content", "children", "class"]);
     return (
         <KDialog.Root modal {...remote}>
             {local.children}
             <KDialog.Portal>
-                <div class="modal">
-                    <KDialog.Overlay class="modal-overlay" />
-                    <KDialog.Content class={`modal-content ${local.class || ""}`}>
-                        <header class="modal-header">
-                            <Modal.Title class="modal-title">{local.title}</Modal.Title>
-                            <Modal.CloseButton as={Button} class="modal-close icon">
-                                <IconX />
+                <div class="ui-modal">
+                    <KDialog.Overlay class="ui-modal-overlay" />
+                    <KDialog.Content class={`ui-modal-content ${local.class || ""}`}>
+                        <header class="ui-modal-header">
+                            <Modal.Title class="ui-modal-title">{local.title}</Modal.Title>
+                            <Modal.CloseButton as={Button} class="ui-modal-close icon">
+                                <Icon name="x" />
                             </Modal.CloseButton>
                         </header>
                         {local.content}
                     </KDialog.Content>
                 </div>
             </KDialog.Portal>
         </KDialog.Root>
```

### Comparing `relationalai-0.2.2/frontend/debugger/src/components/Sidebar.styl` & `relationalai-0.2.3/frontend/debugger/src/components/Sidebar.styl`

 * *Files 10% similar despite different names*

```diff
@@ -1,111 +1,109 @@
 .sidebar {
   box-sizing: border-box;
-  height: 100vh;
   position: relative;
 
-  --sidebar-width: 250px;
   --sidebar-pad: 12px;
   --sidebar-anim-duration: 0.3s;
-  --sidebar-trigger-direction: 1;
 
   .sidebar-trigger {
     position: absolute;
-    top: 0;
     padding: var(--sidebar-pad);
 
-    .tabler-icon {
-      transform: scaleX(var(--sidebar-trigger-direction));
-      transition: transform var(--sidebar-anim-duration) ease-out;
-    }
-
-    &[data-closed] .tabler-icon {
-      transform: scaleX(calc(var(--sidebar-trigger-direction) * -1));
-    }
-
     &:focus {
       outline: none;
     }
   }
 
   .sidebar-content {
     box-sizing: border-box;
-    height: 100%;
     overflow: hidden;
 
     display: flex;
     flex-direction: column;
+    align-items: stretch;
 
     animation-duration: var(--sidebar-anim-duration);
     animation-easing-function: ease-out;
 
-    &[data-closed] {
-      // width: 0;
-      animation-name: sidebar_close;
-
-      .sidebar-inner {
-        width: var(--kb-collapsible-content-width);        
-      }
+    & > .ui-collapsible-inner {
+      box-sizing: border-box;
+      height: 100%;
+      width: 100%;
+      padding: 0;
+      display: flex;
+      flex-direction: column;
     }
+  }
 
-    &[data-expanded] {
-      animation-name: sidebar_open;
+  &.left, &.right {
+    height: 100vh;
 
-      .sidebar-inner {
-        animation: sidebar_inner_open var(--sidebar-anim-duration) ease-out;
-      }
+    .sidebar-trigger {
+      top: 0;
     }
 
-    .sidebar-inner {
-      box-sizing: border-box;
-      min-width: auto;      
+    .sidebar-content {
       height: 100%;
-      padding: var(--sidebar-pad);
-      display: flex;
-      flex-direction: column;
+
+      &[data-closed] {
+        width: var(--kb-collapsible-content-width);
+        min-width: 0 !important;
+
+        & > .ui-collapsible-inner {
+          width: var(--kb-collapsible-content-width);
+        }
+      }
+
+      &[data-expanded] {
+      }
     }
   }
 
   &.left {
-    box-shadow: 3px 0 10px #00091033;
+    box-shadow: 3px 0 15px -5px #00091066;
+
     .sidebar-trigger {
       left: 100%;
     }
+
     .sidebar-content {
       align-items: flex-end;
     }
   }
+
   &.right {
-    box-shadow: 3px 0 10px #00091033;
-    --sidebar-trigger-direction: -1;
+    box-shadow: 3px 0 15px -5px #00091066;
+
     .sidebar-trigger {
       right: 100%;
     }
   }
-}
 
-@keyframes sidebar_close {
-  from {
-    width: var(--kb-collapsible-content-width);
-  }
-  to {
-    width: 0;
-  }
-}
+  &.top, &.bottom {
+    width: 100%;
 
-@keyframes sidebar_open {
-  from {
-    width: 0;
-  }
-  to {
-    width: var(--kb-collapsible-content-width);
-  }
-}
+    .sidebar-trigger {
+      left: 50%;
+      transform: translateX(-50%);
+    }
+
+    .sidebar-content {
+      width: 100%;
 
-@keyframes sidebar_inner_open {
-  from {
-    width: var(--kb-collapsible-content-width);
+      &[data-closed] {
+        height: var(--kb-collapsible-content-height);
+      }
+
+      &[data-expanded] {
+      }
+    }
   }
-  to {
-    width: var(--kb-collapsible-content-width);
+
+  &.bottom {
+    box-shadow: 0 -3px 15px -5px #00091066;
+
+    .sidebar-trigger {
+      bottom: 100%;
+    }
   }
 }
```

### Comparing `relationalai-0.2.2/frontend/debugger/src/components/Tooltip.stories.tsx` & `relationalai-0.2.3/frontend/debugger/src/components/ui/Tooltip.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/frontend/debugger/src/components/Tooltip.styl` & `relationalai-0.2.3/frontend/debugger/src/components/ui/Tooltip.styl`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-.tooltip {
-  --tooltip-bg: #f9f9f9;
-  --tooltip-border: oklch(from var(--tooltip-bg) calc(l * 0.75) c h);
-  --tooltip-anim-open-duration: 0.1s;
-  --tooltip-anim-close-duration: 0.2s;
+:root {
+  --tooltip-bg: var(--section-bg);
+  --tooltip-border: var(--section-border);
+  --tooltip-shadow: var(--shadow);
+  --tooltip-anim-open-duration: var(--anim-duration-quick);
+  --tooltip-anim-close-duration: var(--anim-duration-normal);
+}
 
+.ui-tooltip {
   z-index: 50;
 
-  .tooltip-arrow {
+  .ui-tooltip-arrow {
     margin-bottom: -1px;
     svg {
       fill: var(--tooltip-bg);
       stroke: var(--tooltip-border);
       stroke-width: 1.8px;
     }
     * {
@@ -22,15 +25,15 @@
     padding: 4px 8px;
     max-width: min(calc(100vw - 16px), 380px);
     font-size: 0.8em;
 
     background: var(--tooltip-bg);
     border-radius: 4px;
     border: 1px solid var(--tooltip-border);
-    box-shadow: 1px 4px 11px #00091033;
+    box-shadow: 1px 4px 11px var(--tooltip-shadow);
     transform-origin: var(--kb-tooltip-content-transform-origin);
   }
 
   &[data-expanded] {
     animation: tooltip_show var(--tooltip-anim-open-duration) ease-out;
   }
```

### Comparing `relationalai-0.2.2/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx` & `relationalai-0.2.3/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/frontend/debugger/src/components/Schematic/ScopeProvider.tsx` & `relationalai-0.2.3/frontend/debugger/src/components/Schematic/ScopeProvider.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/frontend/debugger/src/components/Schematic/index.stories.tsx` & `relationalai-0.2.3/frontend/debugger/src/components/Schematic/index.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/frontend/debugger/src/components/Schematic/index.styl` & `relationalai-0.2.3/frontend/debugger/src/components/Schematic/index.styl`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-@require "../../util.styl";
+@require "util.styl";
 
 :root {
-  --schematic-bg-color: white;
-  --schematic-rail-color: #3D5A80;
+  --schematic-bg-color: #121212; // white;
+  --schematic-rail-color: #4D8CC0  // #3D5A80;
   --schematic-rail-width: 4px;
   --schematic-rail-gap: 16px;
 
   --schematic-node-icon-size: 20px;
   --schematic-node-icon-thickness: var(--schematic-rail-width);
   --schematic-node-icon-cutout: var(--schematic-rail-width);
   --schematic-node-icon-padding: 8px;
```

### Comparing `relationalai-0.2.2/frontend/debugger/src/components/Schematic/index.tsx` & `relationalai-0.2.3/frontend/debugger/src/components/Schematic/index.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx` & `relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx` & `relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx` & `relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx` & `relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx` & `relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx` & `relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx` & `relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/base.styl` & `relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/base.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/base.tsx` & `relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/base.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/index.tsx` & `relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/index.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/frontend/debugger/src/fixtures/branch-improved.json` & `relationalai-0.2.3/frontend/debugger/src/fixtures/branch-improved.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/frontend/debugger/src/fixtures/branch.json` & `relationalai-0.2.3/frontend/debugger/src/fixtures/branch.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/frontend/debugger/src/fixtures/fraud.json` & `relationalai-0.2.3/frontend/debugger/src/fixtures/fraud.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/frontend/debugger/src/fixtures/not_found.json` & `relationalai-0.2.3/frontend/debugger/src/fixtures/not_found.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/frontend/debugger/src/fixtures/simple.json` & `relationalai-0.2.3/frontend/debugger/src/fixtures/simple.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/frontend/debugger/src/fixtures/union.json` & `relationalai-0.2.3/frontend/debugger/src/fixtures/union.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/frontend/debugger/src/types/mech.d.ts` & `relationalai-0.2.3/frontend/debugger/src/types/mech.d.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/gentest/README.md` & `relationalai-0.2.3/src/gentest/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/gentest/emit.py` & `relationalai-0.2.3/src/gentest/emit.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/gentest/exec.py` & `relationalai-0.2.3/src/gentest/exec.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/gentest/fixtures.py` & `relationalai-0.2.3/src/gentest/fixtures.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/gentest/patch.py` & `relationalai-0.2.3/src/gentest/patch.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/gentest/util.py` & `relationalai-0.2.3/src/gentest/util.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/gentest/cli/__main__.py` & `relationalai-0.2.3/src/gentest/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/gentest/cli/collect_failures.py` & `relationalai-0.2.3/src/gentest/cli/collect_failures.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/gentest/cli/collect_tests.py` & `relationalai-0.2.3/src/gentest/cli/collect_tests.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/gentest/cli/repro.py` & `relationalai-0.2.3/src/gentest/cli/repro.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/gentest/cli/watch.py` & `relationalai-0.2.3/src/gentest/cli/watch.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/gentest/gen/action.py` & `relationalai-0.2.3/src/gentest/gen/action.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/gentest/gen/context.py` & `relationalai-0.2.3/src/gentest/gen/context.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/gentest/gen/document.py` & `relationalai-0.2.3/src/gentest/gen/document.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/gentest/gen/group_limited.py` & `relationalai-0.2.3/src/gentest/gen/group_limited.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/gentest/gen/ir.py` & `relationalai-0.2.3/src/gentest/gen/ir.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/gentest/gen/scope.py` & `relationalai-0.2.3/src/gentest/gen/scope.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/gentest/gen/task.py` & `relationalai-0.2.3/src/gentest/gen/task.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/gentest/gen/test.py` & `relationalai-0.2.3/src/gentest/gen/test.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/gentest/harness/database.py` & `relationalai-0.2.3/src/gentest/harness/database.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/gentest/validate/diff.py` & `relationalai-0.2.3/src/gentest/validate/diff.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/gentest/validate/errors.py` & `relationalai-0.2.3/src/gentest/validate/errors.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/gentest/validate/mapping.py` & `relationalai-0.2.3/src/gentest/validate/mapping.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/gentest/validate/roundtrip.py` & `relationalai-0.2.3/src/gentest/validate/roundtrip.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/relationalai/__init__.py` & `relationalai-0.2.3/src/relationalai/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,59 @@
 from typing import cast
-from relationalai.tools.debugger_server import start_debugger_session
 from .clients import config as cfg
 from . import clients
 from . import dsl
 from . import debugging
 from . import metamodel
 from . import rel
 from .loaders import csv
 from . import analysis
 from . import tools
 import importlib.metadata
+from snowflake.connector import SnowflakeConnection
 
 __version__ = importlib.metadata.version(__package__ or __name__)
 
-def Model(name:str, *, profile:str|None=None, config:cfg.Config|None=None, dry_run:bool=False, debug=None):
+def Model(
+    name: str,
+    *,
+    profile: str | None = None,
+    config: cfg.Config | None = None,
+    dry_run: bool = False,
+    debug=None,
+    connection: SnowflakeConnection | None = None,
+):
     config = config or cfg.Config(profile=profile)
     if debug is None:
         debug = config.get("debug", False)
     if debug:
+        from relationalai.tools.debugger_server import start_debugger_session
         start_debugger_session(True)
     if not config.file_path:
         if cfg.legacy_config_exists():
             message = (
                 "Use `rai init` to migrate your configuration file "
                 "to the new format (raiconfig.toml)"
             )
         else:
             message = "No configuration file found. Please run `rai init` to create one."
         raise Exception(message)
     if config.get("platform") is None:
         config.set("platform", "snowflake")
     platform = config.get("platform")
+    if platform != "snowflake" and connection is not None:
+        raise ValueError("The `connection` parameter is only supported with the Snowflake platform")
     dry_run = cast(bool, dry_run or config.get("compiler.dry_run", False))
     if platform == "azure":
         return clients.azure.Graph(
             name, profile=profile, config=config, dry_run=dry_run
         )
     elif platform == "snowflake":
         return clients.snowflake.Graph(
-            name, profile=profile, config=config, dry_run=dry_run
+            name, profile=profile, config=config, dry_run=dry_run, connection=connection
         )
     else:
         raise Exception(f"Unknown platform: {platform}")
 
 def Resources(profile:str|None=None, config:cfg.Config|None=None):
     config = config or cfg.Config(profile)
     platform = config.get("platform", "snowflake")
```

### Comparing `relationalai-0.2.2/src/relationalai/compiler.py` & `relationalai-0.2.3/src/relationalai/compiler.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/relationalai/debugging.py` & `relationalai-0.2.3/src/relationalai/debugging.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from textwrap import dedent
 import os
 from typing import Dict
 import logging
 import time as _time
 
 from pandas import DataFrame
-from .errors import Errors
 from .metamodel import Action, Task
 
 DEBUG = True
 
 #--------------------------------------------------
 # Log Formatters
 #--------------------------------------------------
@@ -94,15 +93,15 @@
     end_time = _time.perf_counter()
     logger.debug({**span, "event": "span_end", "end_time": end_time, "elapsed": end_time - span["start_time"]})
 
 @contextlib.contextmanager
 def span(type: str, **kwargs):
     cur = span_start(type, **kwargs)
     try:
-        yield
+        yield cur
     except Exception as err:
         error(err)
         raise
     finally:
         span_end(cur)
 
 #--------------------------------------------------
@@ -288,14 +287,15 @@
 
     lines = source_code.splitlines()
     if caller_line > len(lines):
         return SourceInfo(relative_filename, caller_line)
     return SourceInfo(relative_filename, caller_line, lines[caller_line - 1])
 
 def check_errors(task:Task|Action):
+    from .errors import Errors
     class ErrorFinder(ast.NodeVisitor):
         def __init__(self, start_line):
             self.errors = []
             self.start_line = start_line
 
         def to_line_numbers(self, node):
             return (node.lineno, node.end_lineno)
```

### Comparing `relationalai-0.2.2/src/relationalai/dsl.py` & `relationalai-0.2.3/src/relationalai/dsl.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,14 +250,15 @@
             raise Exception("Add must be provided the same arguments in each branch")
         self._select_len = arg_len
         self._assign_vars()
         if len(self._props) and set(self._props.keys()) != set(kwargs.keys()):
             raise Exception("Add must be provided the same properties in each branch")
         elif len(self._props) == 0:
             for k, v in zip(kwargs.keys(), self._vars[1:]):
+                v.name = k
                 self._props[k] = v
 
         graph = self._context.graph
         graph._action(build.return_([item, *[kwargs[k] for k in self._props.keys()]]))
 
 class Context():
     def __init__(self, graph:'Graph', *args, behavior=Behavior.Query, op=None,
@@ -292,16 +293,16 @@
                 self.graph._pop(self)
             except KeyboardInterrupt as e:
                 print("Canceling transactions...")
                 self.graph.resources.cancel_pending_transactions()
                 raise e
             except RAIException as e:
                 raise RAIException(e.message) from None
-            except RelQueryError:
-                raise RAIException("An error occured translating Python into RelationalAI") from None
+            except RelQueryError as e:
+                raise RelQueryError(e.problems) from None
         else:
             self.graph._pop(self, exec=False)
         return False
 
     def _ensure_rel(self, vs:List[Var]):
         if self._rel is None:
             self._rel = build.relation_action(ActionType.Get, self._task, vs)
@@ -433,15 +434,15 @@
 
 #--------------------------------------------------
 # Property
 #--------------------------------------------------
 
 class Property(Producer):
     def __init__(self, graph:'Graph', name:str, types:List[mType], provider:Type|TypeUnion, scope:str=""):
-        super().__init__(graph, ["to_property", "has_many"])
+        super().__init__(graph, ["to_property", "has_many", "is_multi_valued"])
         self._name = name
         self._type = types[0]
         self._scope = scope
         self._provider = provider
         self._prop = build.property_named(scope+name, types)
 
     def __call__(self, key:Any, value:Any):
@@ -456,14 +457,18 @@
 
     def to_property(self):
         return self._prop
 
     def has_many(self):
         self._graph._check_property(self._prop, multi_valued=True)
 
+    @property
+    def is_multi_valued(self):
+        return self._graph._prop_is_multi.get(self._name)
+
 #--------------------------------------------------
 # Instance
 #--------------------------------------------------
 
 class Instance(Producer):
     def __init__(self, graph:'Graph', action_type:ActionType, positionals:List[Any], named:Dict[str,Any], var:Var|None=None, name=None, is_add=False, scope:str=""):
         super().__init__(graph, RESERVED_PROPS)
@@ -1056,15 +1061,15 @@
         self.name = name
         self._stack = RuleStack(self)
         self._temp_rule = Context(self)
         self._executed = []
         self._client = client
         self._config = client.resources.config
         self.resources = client.resources
-        self._prop_is_multi = {}
+        self._prop_is_multi:Dict[str, bool] = {}
 
         _ensure_stack().append(self)
         self._stack.push(self._temp_rule)
 
     #--------------------------------------------------
     # Rule stack
     #--------------------------------------------------
```

### Comparing `relationalai-0.2.2/src/relationalai/errors.py` & `relationalai-0.2.3/src/relationalai/errors.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/relationalai/metagen.py` & `relationalai-0.2.3/src/relationalai/metagen.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/relationalai/metamodel.py` & `relationalai-0.2.3/src/relationalai/metamodel.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/relationalai/rel.py` & `relationalai-0.2.3/src/relationalai/rel.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,15 @@
     def finalize(self):
         final_tasks = []
         for neue in self.tasks:
             for dep in self.task_deps[neue]:
                 if dep in self.tasks:
                     neue.items.insert(0, build.relation_action(ActionType.Get, dep, self.mapped_bindings(neue, dep)))
             if self.task_bindings[neue]:
+                neue.parents.append(Builtins.InlineAnnotation)
                 neue.items.append(build.relation_action(ActionType.Bind, neue, self.task_bindings[neue]))
             if neue not in self.inlines:
                 final_tasks.append(neue)
         return final_tasks
 
     def reset(self):
         self.tasks.clear()
@@ -168,31 +169,47 @@
 
     #--------------------------------------------------
     # Union
     #--------------------------------------------------
 
     def union_call(self, call:Action, parent:Task):
         has_dep = False
+        result_refs = []
+        # add the final get that will be in the new continued task
+        result_refs.append(build.relation_action(ActionType.Get, cast(Task, call.entity.value), call.bindings.values()))
         # run through the subtasks and add them to the flow
         for item in cast(Task, call.entity.value).items:
             neue = self.query_flow(cast(Task, item.entity.value))
             has_dep = has_dep or (parent in self.flow.task_deps[neue])
             rets = [i for i in neue.items if i.entity.value == Builtins.Return]
             if len(rets):
                 rets[0].entity.value = call.entity.value
                 rets[0].action = ActionType.Bind
+                result_refs.append(rets[0])
 
         # if one of the subtasks depends on the parent, we need to cut the
         # current task to prevent cycles and carry on in a new one
         if has_dep:
             orig = parent
             self.flow.pop_context(orig)
             self.flow.assoc(gather_vars(orig.items), orig)
             parent = self.flow.push_context()
-        parent.items.append(build.relation_action(ActionType.Get, cast(Task, call.entity.value), call.bindings.values()))
+
+            # Update the bindings for the result refs to include the vars we depend on
+            for bind in result_refs:
+                neue_bindings = {}
+                for i, var in enumerate(self.flow.task_bindings[orig]):
+                    neue_bindings[Builtins.Relation.properties[i]] = var
+                prop_len = len(neue_bindings)
+                for v in bind.bindings.values():
+                    neue_bindings[Builtins.Relation.properties[prop_len]] = v
+                    prop_len += 1
+                bind.bindings = neue_bindings
+
+        parent.items.append(result_refs[0])
         return parent
 
     #--------------------------------------------------
     # Ordered choice
     #--------------------------------------------------
 
     def ordered_choice_call(self, call:Action, parent:Task):
@@ -249,17 +266,22 @@
             # We also need to make sure that branches that don't currently depend on
             # the parent now do, since they also need to join correctly with the original
             # rows
             for branch in branches:
                 self.flow.task_deps[branch].add(orig)
             # Update the bindings for the result refs to include the vars we depend on
             for bind in result_refs:
-                prop_len = len(bind.bindings)
+                neue_bindings = {}
                 for i, var in enumerate(self.flow.task_bindings[orig]):
-                    bind.bindings[Builtins.Relation.properties[prop_len+i]] = var
+                    neue_bindings[Builtins.Relation.properties[i]] = var
+                prop_len = len(neue_bindings)
+                for v in bind.bindings.values():
+                    neue_bindings[Builtins.Relation.properties[prop_len]] = v
+                    prop_len += 1
+                bind.bindings = neue_bindings
             parent = self.flow.push_context()
 
         parent.items.append(result_refs[0]) # result_refs[0] is the Get for the ordered_choice
         return parent
 
     #--------------------------------------------------
     # Quantifiers
@@ -396,14 +418,15 @@
 
     #--------------------------------------------------
     # Subtask creation
     #--------------------------------------------------
 
     def create_fetch(self, non_effects: List[Action], effects_vars: Iterable[Var]):
         fetch = Task()
+        fetch.parents.append(Builtins.InlineAnnotation)
         non_effects.append(build.relation_action(ActionType.Bind, fetch, effects_vars))
         fetch.items = non_effects
         return build.call(fetch, [])
 
     def create_effect_query(self, effects: List[Action], effects_vars: Iterable[Var], fetch: Any):
         neue = Task()
         if fetch:
```

### Comparing `relationalai-0.2.2/src/relationalai/rel2.py` & `relationalai-0.2.3/src/relationalai/rel2.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/relationalai/rel_emitter.py` & `relationalai-0.2.3/src/relationalai/rel_emitter.py`

 * *Files 5% similar despite different names*

```diff
@@ -260,14 +260,16 @@
                     (item,) = i.bindings.values()
                     supporting_rules.append(f"declare {self.emit_var(item)}")
                     if isinstance(item.value, Type) and item.value.isa(Builtins.ValueType):
                         vtype = self.sanitize(item.value.name).capitalize() + "Type"
                         supporting_rules.append(f"value type {vtype} {{ UInt128 }}")
                         for op in ["<", ">"]:
                             supporting_rules.append(f"def ::std::common::({op})[x in {vtype}, y in {vtype}]: exists((a, b) | ^{vtype}(a, x) and ^{vtype}(b, y) and a {op} b)")
+                        for op in ["minimum", "maximum"]:
+                            supporting_rules.append(f"def ::std::common::{op}(x in {vtype}, y in {vtype}, z in {vtype}): exists((a, b) | ^{vtype}(minimum[a, b], z) and ^{vtype}(a, x) and ^{vtype}(b, y))")
                 else:
                     body.append(self.to_relation(i, body_vars, body))
             elif i.action == ActionType.Bind and i.entity.value == Builtins.Return:
                 head_rel = self.to_return(i, head_vars, body)
                 head = f"def {head_rel}:\n    "
             elif i.action in [ActionType.Bind, ActionType.Persist, ActionType.Unpersist]:
                 if not inline:
```

### Comparing `relationalai-0.2.2/src/relationalai/rel_utils.py` & `relationalai-0.2.3/src/relationalai/rel_utils.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/relationalai/analysis/mechanistic.py` & `relationalai-0.2.3/src/relationalai/analysis/mechanistic.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/relationalai/analysis/whynot.py` & `relationalai-0.2.3/src/relationalai/analysis/whynot.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/relationalai/clients/azure.py` & `relationalai-0.2.3/src/relationalai/clients/azure.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/relationalai/clients/client.py` & `relationalai-0.2.3/src/relationalai/clients/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,17 @@
 
     @abstractmethod
     def resume_engine(self, name: str):
         pass
 
     def get_default_engine_name(self) -> str:
         return self.config.get("engine")
+    
+    def get_app_name(self):
+        return self.config.get("rai_app_name", "relationalai")
 
     #--------------------------------------------------
     # Transactions
     #--------------------------------------------------
 
     @abstractmethod
     def list_transactions(self, limit:int, only_active=False) -> List[dict]:
@@ -259,24 +262,26 @@
         self.compiler.compile(dsl.build.raw_task(code))
         self._install_batch.append(name, code)
 
     def query(self, task:m.Task, rentrant=False, readonly=True, raw_results=False, inputs={}) -> DataFrame|Any:
         if self._install_batch.is_dirty():
             self._install_batch_flush()
 
-        with debugging.span("query", model=self._database, task=task):
+        with debugging.span("query", model=self._database, task=task) as end_span:
             code = self.compiler.compile(task)
             if task.has_persist():
                 readonly = False
             if self.dry_run:
                 return DataFrame()
 
             start = time.perf_counter()
             results = self.resources.exec_raw(self._database, self.get_engine_name(), code, readonly=readonly, inputs=inputs)
             dataframe, errors = self.resources.format_results(results, task)
+            end_span["results"] = dataframe
+            end_span["errors"] = errors
             if raw_results:
                 debugging.time("query", time.perf_counter() - start, DataFrame())
                 self.report_errors(errors, abort_on_error=False)
                 return results
             self.report_errors(errors)
             debugging.time("query", time.perf_counter() - start, dataframe)
             return dataframe
```

### Comparing `relationalai-0.2.2/src/relationalai/clients/config.py` & `relationalai-0.2.3/src/relationalai/clients/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from copy import deepcopy
 import os
 from typing import Dict, Any, cast
 from railib import config
 import configparser
 import toml
 import tomlkit
 from tomlkit.items import Table
@@ -118,15 +119,16 @@
                         **props,
                     }
             return props
         return self.map(fill)
 
     def merge(self, other):
         """
-        Merge the profiles from `other` into this ConfigFile object
+        Merge the profiles from `other` into this ConfigFile object.
+        For common keys, the values from `self` take precedence.
         """
         combined_profiles = self.get_combined_profiles()
         other_combined_profiles = other.get_combined_profiles()
 
         all_profile_names = set(combined_profiles) | set(other_combined_profiles)
 
         for profile in all_profile_names:
@@ -217,16 +219,16 @@
     root_file = config_files[0]
     if profile:
         root_file.config["active_profile"] = profile
     if ("active_profile" in root_file.config and
         root_file.config["active_profile"] in root_file.profiles):
         active_profile = root_file.config["active_profile"]
         config = {
-            **root_file.profiles[active_profile],
             **root_file.config,
+            **root_file.profiles[active_profile],
         }
     else:
         config = root_file.config
     return config, file_path
 
 def has_platform(cfg, platform):
     return any(profile.get("platform") == platform for profile in cfg.get_combined_profiles().values())
@@ -321,14 +323,17 @@
                 except toml.TomlDecodeError as e:
                     raise Exception(f"Error parsing {self.file_path}: {e}")
             return
 
     def clone_profile(self):
         self.props = {k: v for k,v in self.props.items()}
 
+    def clone(self):
+        return deepcopy(self)
+
     def get(self, name:str, default:Any=_no_default, strict:bool=True):
         parts = name.split(".")
         props = self.props
 
         for part in parts[:-1]:
             props = props.get(part)
             if props is None:
@@ -369,20 +374,23 @@
     def print(self):
         for k, v in self.items():
             print(f"{k}: {v}")
 
     def to_rai_config(self) -> Dict[str, Any]:
         return to_rai_config(self.props)
 
-    def save(self):
+    def save(self, update_active_profile=True):
         new_document = tomlkit.document()
 
         # handle the active_profile key that appears at the top:
         if self.profile != "__top_level__":
-            active_profile = self.profile
+            if update_active_profile:
+                active_profile = self.profile
+            else:
+                active_profile = self.original_toml.get("active_profile", None)
         else:
             active_profile = self.get("active_profile", None)
         if active_profile is not None:
             new_document["active_profile"] = active_profile
 
         # add key-value pairs at the top level if this is the top-level profile:
         if self.profile == "__top_level__":
```

### Comparing `relationalai-0.2.2/src/relationalai/clients/snowflake.py` & `relationalai-0.2.3/src/relationalai/clients/snowflake.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import textwrap
 from railib.api import TransactionAsyncResponse, poll_with_specified_overhead, _parse_metadata_proto
 import requests
 import snowflake.connector
 import pyarrow as pa
 import pandas as pd
 import time
+from snowflake.connector import SnowflakeConnection
 
 from .. import debugging
 
 from typing import Any, Dict, Iterable, Tuple, List, cast
 import base64
 
 from pandas import DataFrame
@@ -24,15 +25,33 @@
 from ..clients.config import Config
 from ..clients.client import Client, ResourceProvider
 from .. import dsl, rel, metamodel as m
 from ..errors import Errors, RAIException
 from .. import std
 import re
 
+#--------------------------------------------------
+# Constants
+#--------------------------------------------------
+
 USE_EXEC_ASYNC = True
+VALID_POOL_STATUS = ["ACTIVE", "IDLE", "SUSPENDED"]
+COMPUTE_POOL_MAP = {
+    "STANDARD_1": "XS",
+    "CPU_X64_XS": "XS",
+    "CPU_X64_S": "XS",
+    "CPU_X64_M": "S",
+    "HIGHMEM_X64_S": "M",
+    "HIGH_MEMORY_4": "L",
+    "HIGHMEM_X64_M": "XL",
+    "HIGHMEM_S": "M",
+    "HIGHMEM_M": "L",
+    "HighMem|S": "M",
+    "HighMem|M": "L",
+}
 
 #--------------------------------------------------
 # Helpers
 #--------------------------------------------------
 
 def type_to_sql(type) -> str:
     if type is str:
@@ -75,36 +94,40 @@
 #--------------------------------------------------
 # Resources
 #--------------------------------------------------
 
 APP_NAME = "___RAI_APP___"
 
 class Resources(ResourceProvider):
-    def __init__(self, profile:str|None=None, config:Config|None=None):
+    def __init__(
+        self,
+        profile: str | None = None,
+        config: Config | None = None,
+        connection: SnowflakeConnection | None = None,
+    ):
         super().__init__(profile, config=config)
-        self._conn = None
-        self._app_name = "relationalai"
+        self._conn = connection
         self._pending_transactions: list[str] = []
 
     def _exec(self, code:str, params:List[Any]|None = None):
         if not self._conn:
             self._conn = snowflake.connector.connect(
                 user=self.config.get('user'),
                 password=self.config.get('password'),
                 account=self.config.get('account'),
                 warehouse=self.config.get('warehouse', ""),
-                # database=self.config.get('database', ""),
-                # schema=self.config.get('schema', ""),
                 role=self.config.get('role', ""),
                 client_store_temporary_credential=True,
                 client_request_mfa_token=True,
             )
-            self._app_name = self.config.get('rai_app_name', "relationalai")
         try:
-            return self._conn.cursor().execute(code.replace(APP_NAME, self._app_name), params)
+            return self._conn.cursor().execute(
+                code.replace(APP_NAME, self.get_app_name()),
+                params
+            )
         except Exception as e:
             orig_message = str(e).lower()
             rai_app = self.config.get("rai_app_name", "")
             if re.search(f"database '{rai_app}' does not exist or not authorized.".lower(), orig_message):
                 print("\n")
                 Errors.snowflake_app_missing(rai_app)
             elif re.search(r"JavaScript execution error", orig_message):
@@ -221,15 +244,15 @@
         py_inputs = ", ".join([name for (name, *rest) in inputs])
         safe_rel = code.replace("'", "\\'").replace("{", "{{").replace("}", "}}").strip()
         for (name, var, type) in inputs:
             if type is str:
                 safe_rel = safe_rel.replace(var, f"'{{{name}.replace(\"'\", \"\\'\")}}'")
             else:
                 safe_rel = safe_rel.replace(var, f"{{{name}}}")
-        safe_rel = safe_rel.replace("\n", "\\n")
+        safe_rel = safe_rel.replace("\n", "\\n").replace("\"", "\\\"")
         if py_inputs:
             py_inputs = f", {py_inputs}"
         sql_code = textwrap.dedent(f"""
                 CREATE OR REPLACE PROCEDURE {func_name}({sql_inputs})
                 RETURNS TABLE({sql_out})
                 LANGUAGE PYTHON
                 RUNTIME_VERSION = '3.8'
@@ -552,16 +575,25 @@
         return [{"name":name}
                 for (name, *rest) in results.fetchall()]
 
     def list_compute_pools(self):
         results = self._exec("SHOW COMPUTE POOLS")
         if not results:
             return []
-        return [{"name":name}
-                for (name, *rest) in results.fetchall()]
+        return [{"name":name, "status":status, "min_nodes":min_nodes, "max_nodes":max_nodes, "instance_family":instance_family}
+                for (name, status, min_nodes, max_nodes, instance_family, *rest) in results.fetchall()]
+
+    def list_valid_compute_pools_by_engine_size(self, engine_size:str):
+        valid_pools = self.list_compute_pools()
+        if not valid_pools:
+            return []
+        engine_pools = [item['name'] for item in valid_pools if item['status'] in VALID_POOL_STATUS and COMPUTE_POOL_MAP.get(item['instance_family']) == engine_size]
+        if not engine_pools:
+            return []
+        return engine_pools
 
     def list_roles(self):
         results = self._exec("SELECT CURRENT_AVAILABLE_ROLES()")
         if not results:
             return []
         # the response is a single row with a single column containing
         # a stringified JSON array of role names:
@@ -646,15 +678,15 @@
         for item in imports:
             database_name, schema_name, table_name = item["name"].lower().split('.')
             database = getattr(self, database_name)
             schema = getattr(database, schema_name)
             schemas.add(schema)
             schema._add(table_name, is_imported=True)
         for schema in schemas:
-            schema._finalize()
+            schema._fetch_info()
         return tree
 
     def __getattribute__(self, __name: str) -> 'SnowflakeDB':
         if __name.startswith("_"):
             return super().__getattribute__(__name)
         __name = __name.lower()
         if __name in self._dbs:
@@ -680,51 +712,67 @@
 
 class SnowflakeSchema:
     def __init__(self, parent, name):
         self._name = name
         self._parent = parent
         self._model = parent._model
         self._tables = {}
+        self._imported = set()
 
-    def _finalize(self):
-        self._table_info = self._model._client.resources.schema_info(self._parent._name, self._name, self._tables.keys())
-        for table in self._tables.values():
-            table._finalize()
+    def _fetch_info(self):
+        self._table_info = self._model._client.resources.schema_info(self._parent._name, self._name, self._imported)
 
     def _add(self, name, is_imported=False):
         name = name.lower()
         if name in self._tables:
             return self._tables[name]
-        self._tables[name] = SnowflakeTable(self, name, is_imported=is_imported)
+        self._tables[name] = SnowflakeTable(self, name)
+        if is_imported:
+            self._imported.add(name)
         return self._tables[name]
 
     def __getattribute__(self, __name: str) -> 'SnowflakeTable':
         if __name.startswith("_"):
             return super().__getattribute__(__name)
-        return self._add(__name)
+        table = self._add(__name)
+        table._lazy_init()
+        return table
 
 class SnowflakeTable(dsl.Type):
-    def __init__(self, parent, name, is_imported=False):
+    def __init__(self, parent, name):
         super().__init__(parent._model, f"sf_{name}", ["namespace", "fqname", "describe"])
         self._name = name
         self._model = parent._model
         self._parent = parent
         self._aliases = {}
         self._finalzed = False
-        if not is_imported and self._parent._parent._parent._auto_import:
-            with Spinner(f"Creating stream for {self.fqname()}", f"Stream created for {self.fqname()}"):
-                db_name = parent._parent._name
-                schema_name = parent._name
-                self._model._client.resources.create_import_stream(ImportSourceTable(db_name, schema_name, name), self._model.name)
-            print("")
-            parent._tables[name] = self
-            parent._finalize()
-        elif not is_imported:
-            Errors.snowflake_import_missing(debugging.capture_code_info(4), self.fqname(), self._model.name)
 
+    def _lazy_init(self):
+        parent = self._parent
+        name = self._name
+        if name not in parent._imported:
+            if self._parent._parent._parent._auto_import:
+                with Spinner(f"Creating stream for {self.fqname()}", f"Stream created for {self.fqname()}"):
+                    db_name = parent._parent._name
+                    schema_name = parent._name
+                    self._model._client.resources.create_import_stream(ImportSourceTable(db_name, schema_name, name), self._model.name)
+                print("")
+                parent._imported.add(name)
+            else:
+                imports = self._model._client.resources.list_imports(self._model.name)
+                for item in imports:
+                    cur_name = item["name"].lower().split(".")[-1]
+                    parent._imported.add(cur_name)
+            if name not in parent._imported:
+                Errors.snowflake_import_missing(debugging.capture_code_info(), self.fqname(), self._model.name)
+
+        if name not in parent._table_info:
+            parent._fetch_info()
+
+        self._finalize()
 
     def _finalize(self):
         if self._finalzed:
             return
 
         self._finalzed = True
         self._schema = self._parent._table_info[self._name]
@@ -737,18 +785,22 @@
             if self._schema["pks"]:
                 getattr(getattr(std.rel, relation_name), self._schema["pks"][0].upper())(id, val)
             else:
                 getattr(std.rel, relation_name)(prop, id, val)
             self.add(snowflake_id=id)
 
         for prop, prop_type in self._schema["columns"].items():
-            with model.rule():
+            with model.rule(dynamic=True):
                 id, val = std.Vars(2)
                 getattr(getattr(std.rel, relation_name), prop.upper())(id, val)
-                self(snowflake_id=id).set(**{prop.lower(): val})
+                if getattr(self, prop.lower()).is_multi_valued:
+                    inst = self(snowflake_id=id)
+                    getattr(inst, prop.lower()).add(val)
+                else:
+                    self(snowflake_id=id).set(**{prop.lower(): val})
 
     def namespace(self):
         return f"{self._parent._parent._name}.{self._parent._name}"
 
     def fqname(self):
         return f"{self.namespace()}.{self._name}"
 
@@ -762,27 +814,37 @@
                 if isinstance(table, SnowflakeTable):
                     fk_table = table
                     pk = fk_table._schema["pks"]
                     with model.rule():
                         inst = fk_table()
                         me = self()
                         getattr(inst, pk[0]) == getattr(me, k)
-                        me.set(**{name: inst})
+                        if getattr(self, name).is_multi_valued:
+                            getattr(me, name).add(inst)
+                        else:
+                            me.set(**{name: inst})
                 else:
                     raise ValueError(f"Invalid foreign key {v}")
             else:
                 raise ValueError(f"Invalid column {k}={v}")
         return self
 
 #--------------------------------------------------
 # Graph
 #--------------------------------------------------
 
-def Graph(name, *, profile:str|None=None, config:Config, dry_run:bool=False):
-    client = Client(Resources(profile, config), rel.Compiler(config), name, dry_run=dry_run)
+def Graph(
+    name,
+    *,
+    profile: str | None = None,
+    config: Config,
+    dry_run: bool = False,
+    connection: SnowflakeConnection | None = None,
+):
+    client = Client(Resources(profile, config, connection), rel.Compiler(config), name, dry_run=dry_run)
     client.install("pyrel_base", dsl.build.raw_task("""
         @inline
         def make_identity(x..., z):
             exists((u) | hash128({x...}, x..., u) and
             hash_value_uint128_convert(u, z))
 
         @inline
```

### Comparing `relationalai-0.2.2/src/relationalai/clients/test.py` & `relationalai-0.2.3/src/relationalai/clients/test.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/relationalai/clients/types.py` & `relationalai-0.2.3/src/relationalai/clients/types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/relationalai/loaders/csv.py` & `relationalai-0.2.3/src/relationalai/loaders/csv.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/relationalai/loaders/loader.py` & `relationalai-0.2.3/src/relationalai/loaders/loader.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/relationalai/loaders/types.py` & `relationalai-0.2.3/src/relationalai/loaders/types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/relationalai/std/aggregates.py` & `relationalai-0.2.3/src/relationalai/std/aggregates.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/relationalai/std/graphs.py` & `relationalai-0.2.3/src/relationalai/std/graphs.py`

 * *Files 18% similar despite different names*

```diff
@@ -36,49 +36,82 @@
 # Algos
 #--------------------------------------------------
 
 class Compute:
     def __init__(self, graph:'Graph'):
         self._graph = graph
         self._lib = dsl.global_ns.graphlib
-        self._module_lib = rel.rel.graph
-        self._old_lib = getattr(rel, self._graph._lib_ref())
 
     def _config(self, **kwargs):
         return dsl.InlineRelation(self._graph.model, [
             *[(dsl.Symbol(k), v) for k, v in kwargs.items()],
         ])
 
     # --------------------------------------------------
     # Degree
     # --------------------------------------------------
 
-    # TODO: these are still in the old style graph lib
     def degree(self, node, weight=None):
         if not weight:
-            return self._old_lib.degree(node)
-        return self._old_lib.weighted_degree(node)
+            return self._lib.degree(self._graph, node)
+        return self._lib.weighted_degree(self._graph, node)
+
+    def min_degree(self):
+        return self._lib.min_degree(self._graph)
+
+    def max_degree(self):
+        return self._lib.max_degree(self._graph)
+
+    def avg_degree(self):
+        return self._lib.average_degree(self._graph)
 
     def indegree(self, node):
         return self._lib.indegree(self._graph, node)
 
+    def min_indegree(self):
+        return self._lib.min_indegree(self._graph)
+
+    def max_indegree(self):
+        return self._lib.max_indegree(self._graph)
+
+    def avg_indegree(self):
+        return self._lib.average_indegree(self._graph)
+
     def outdegree(self, node):
         return self._lib.outdegree(self._graph, node)
 
+    def min_outdegree(self):
+        return self._lib.min_outdegree(self._graph)
+
+    def max_outdegree(self):
+        return self._lib.max_outdegree(self._graph)
+
+    def avg_outdegree(self):
+        return self._lib.average_outdegree(self._graph)
+
+    # --------------------------------------------------
+    # Basics
+    # --------------------------------------------------
+    def num_nodes(self):
+        return self._lib.num_nodes(self._graph)
+
+    def num_edges(self):
+        return self._lib.num_edges(self._graph)
+
     # --------------------------------------------------
     # Similarity
     # --------------------------------------------------
 
     def cosine_similarity(self, node1, node2):
         if not self._graph.undirected:
             invalid_param("graph", "must be undirected")
-        return self._module_lib.similarity.cosine_similarity(self._graph, node1, node2)
+        return self._lib.cosine_similarity(self._graph, node1, node2)
 
     def jaccard_similarity(self, node1, node2):
-        return self._module_lib.similarity.jaccard_similarity(self._graph, node1, node2)
+        return self._lib.jaccard_similarity(self._graph, node1, node2)
 
     # --------------------------------------------------
     # Centrality
     # --------------------------------------------------
 
     def pagerank(self, node, damping_factor=0.85, tolerance=1e-6, max_iter=20):
         between("damping_factor", damping_factor, 0, 1)
@@ -89,47 +122,47 @@
             graph=self._graph,
             damping_factor=damping_factor,
             tolerance=tolerance,
             max_iter=max_iter,
         )
         return self._lib.pagerank(config, node)
 
-    # TODO: these are still in the old style graph lib
     def betweenness_centrality(self, node):
-        return self._old_lib.betweenness_centrality(node)
+        return self._lib.betweenness_centrality(self._graph, node)
 
     def degree_centrality(self, node):
-        return self._old_lib.degree_centrality(node)
+        return self._lib.degree_centrality(self._graph, node)
 
     def eigenvector_centrality(self, node):
         if not self._graph.undirected:
             invalid_param("graph", "must be undirected")
-        return self._old_lib.eigenvector_centrality(node)
+        return self._lib.eigenvector_centrality(self._graph, node)
 
     # --------------------------------------------------
     # Community Detection
     # --------------------------------------------------
 
-    def label_propagation(self, node):
-        return self._old_lib.label_propagation(node)
-
     def weakly_connected_component(self, node):
-        return self._old_lib.weakly_connected_component(node)
+        return self._lib.weakly_connected_component(self._graph, node)
 
     def triangle_community(self, node):
-        return self._old_lib.triangle_community(node)
+        return self._lib.triangle_community(self._graph, node)
 
     def infomap(self, node):
         config = self._config(graph=self._graph)
         return self._lib.infomap(config, node)
 
     def louvain(self, node):
         config = self._config(graph=self._graph)
         return self._lib.louvain(config, node)
 
+    def label_propagation(self, node):
+        config = self._config(graph=self._graph)
+        return self._lib.label_propagation(config, node)
+
 #--------------------------------------------------
 # Edge
 #--------------------------------------------------
 
 class EdgeInstance:
     def __init__(self, edge:'Edge', from_:Any, to:Any, kwargs:dict={}):
         self._edge = edge
@@ -143,14 +176,15 @@
         v = Vars(1)
         self._edge._prop(name)(self.from_, self.to, v)
         return v
 
     def set(self, **kwargs):
         for k, v in kwargs.items():
             self._edge._prop(k).add(self.from_, self.to, v)
+        return self
 
     def _to_var(self):
         raise Exception("Edges can't be returned directly, you can return the from_ and to properties individually")
 
 class Edge:
     def __init__(self, graph:'Graph'):
         self._graph = graph
```

### Comparing `relationalai-0.2.2/src/relationalai/tools/cli.py` & `relationalai-0.2.3/src/relationalai/tools/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -443,23 +443,24 @@
     if engine == "Create a new engine":
         engine = controls.text("Engine name:")
         engine_size = controls.fuzzy("Engine size:", choices=ENGINE_SIZES)
         engine_pool = ""
         if cfg.get("platform") == "snowflake":
             provider = cast(snowflake.Resources, provider)
             rich.print("")
-            with Spinner("Fetching compute pools", "Fetched compute pools"):
+            with Spinner(f"Fetching compute pools for engine size '{engine_size}'", f"Fetched compute pools for engine size '{engine_size}'"):
                 try:
-                    pools = [v["name"] for v in provider.list_compute_pools()]
+                    valid_pools = provider.list_valid_compute_pools_by_engine_size(engine_size)
                 except Exception as e:
                     raise Exception(f"Error fetching compute pools: {e}")
-            if len(pools) == 0:
-                raise Exception("No compute pools found")
+            if len(valid_pools) == 0:
+                rich.print(f"\n[yellow]No valid compute pools found for engine size '{engine_size}'\n")
+                exit(1)
             rich.print("")
-            engine_pool = controls.fuzzy("Compute pool:", pools, mandatory=False)
+            engine_pool = controls.fuzzy("Compute pool:", valid_pools, mandatory=False)
         rich.print("")
         with Spinner(f"Creating '{engine}' engine... (this may take several minutes)", f"Engine '{engine}' created"):
             try:
                 provider.create_engine(engine, engine_size, engine_pool)
             except Exception as e:
                 raise Exception(f"Error creating engine: {e}")
         rich.print("")
@@ -481,24 +482,24 @@
                     if add_to_gitignore:
                         with open(gitignore_path, 'a') as gitignore_file:
                             gitignore_file.write("\nraiconfig.toml")
                     return
         prev_dir = current_dir
         current_dir = current_dir.parent
 
-def save_flow(cfg:config.Config, confirmed:bool=False):
-    if cfg.profile in cfg.get_profiles():
+def save_flow(cfg:config.Config, check_for_profile_overwrite:bool=True, update_active_profile:bool=True):
+    if cfg.profile in cfg.get_profiles() and check_for_profile_overwrite:
         if not controls.confirm(f"Overwrite existing {cfg.profile} profile"):
             profile_name = controls.text("Profile name:")
             if profile_name:
                 cfg.profile = profile_name
             else:
-                save_flow(cfg)
+                save_flow(cfg, update_active_profile=update_active_profile)
                 return
-    cfg.save()
+    cfg.save(update_active_profile=update_active_profile)
 
 def init_flow():
     cfg = config.Config(fetch=False)
     try:
         cfg.clone_profile()
         rich.print("\n[dim]---------------------------------------------------\n")
         rich.print("[bold]Welcome to [green]RelationalAI!\n")
@@ -536,17 +537,19 @@
         rich.print("[yellow bold]Initialization aborted!")
         rich.print(f"[yellow]{e}")
         print(e.with_traceback(None))
         rich.print("")
 
         save = controls.confirm("Save partial config?")
         if save:
+            if cfg.profile == "__top_level__":
+                cfg.profile = "partial"
             rich.print("")
             cfg.fill_in_with_defaults()
-            save_flow(cfg)
+            save_flow(cfg, check_for_profile_overwrite=False, update_active_profile=False)
             gitignore_flow()
             rich.print(f"[yellow bold]✓ Saved partial raiconfig.toml ({os.path.abspath('raiconfig.toml')})")
 
         divider()
 
 #--------------------------------------------------
 # Profile switcher
@@ -591,15 +594,15 @@
     help="Profile to inspect",
 )
 @click.option(
     "--all-profiles",
     help="Whether to show all profiles in config file",
     is_flag=True,
 )
-def config_explain(profile:str="default", all_profiles:bool=False):
+def config_explain(profile:str|None=None, all_profiles:bool=False):
     divider()
     cfg = ensure_config(profile)
 
     rich.print(f"[bold green]{cfg.file_path}")
     if os.getenv("RAI_PROFILE"):
         rich.print(f"[yellow]Environment variable [bold]RAI_PROFILE = {os.getenv('RAI_PROFILE')}[/bold]")
     rich.print("")
@@ -756,24 +759,25 @@
         size = controls.fuzzy("Engine size:", choices=ENGINE_SIZES)
         rich.print("")
     provider = get_resource_provider()
 
     if provider.config.get("platform") == "snowflake":
         provider = cast(snowflake.Resources, provider)
         rich.print("")
-        with Spinner("Fetching compute pools", "Fetched compute pools"):
+        with Spinner(f"Fetching compute pools for engine size '{size}'", f"Fetched compute pools for engine size '{size}'"):
             try:
-                pools = [v["name"] for v in provider.list_compute_pools()]
+                valid_pools = provider.list_valid_compute_pools_by_engine_size(size)
             except Exception as e:
                 rich.print(f"\n\n[yellow]Error fetching compute pools: {e}")
                 exit(1)
-        if len(pools) == 0:
-            raise Exception("No compute pools found")
+        if len(valid_pools) == 0:
+            rich.print(f"\n[yellow]No valid compute pools found for engine size '{size}'\n")
+            exit(1)
         rich.print("")
-        pool = controls.fuzzy("Compute pool:", pools)
+        pool = controls.fuzzy("Compute pool:", valid_pools)
         rich.print("")
     else:
         pool = ""
 
     with Spinner(f"Creating '{name}' engine... (this may take several minutes)", f"Engine '{name}' created!"):
         try:
             provider.create_engine(name, size, pool)
```

### Comparing `relationalai-0.2.2/src/relationalai/tools/cli_controls.py` & `relationalai-0.2.3/src/relationalai/tools/cli_controls.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/src/relationalai/tools/debugger.py` & `relationalai-0.2.3/src/relationalai/tools/debugger.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
                 with ui.column().classes("w-full"):
                     with ui.row():
                         ui.label(p['name'])
                         ui.label(f"({p['elapsed']*1000000:.0f} us)")
                     code(p['task'])
         elif active_item['event'] == "time":
             ui.label(f"{active_item['type']} | {format_time(active_item['elapsed'])} | {active_item['results']['count']}")
-            vals = json.loads(active_item['results']['values'])
+            vals = active_item['results']['values']
             if len(vals):
                 keys = [k for k in vals[0].keys()]
                 columns = [{'name': k, 'label': k, 'field': k, "align": "left"} for k in keys]
                 ui.table(columns=columns, rows=vals)
             if "code" in active_item:
                 header("Code")
                 code(active_item["code"])
```

### Comparing `relationalai-0.2.2/src/relationalai/tools/debugger_server.py` & `relationalai-0.2.3/src/relationalai/tools/debugger_server.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,55 @@
 import asyncio
-import json
 import logging
+import os
 import threading
 import websockets
 
-from relationalai.debugging import logger, JsonFormatter
+from relationalai import debugging
+import __main__ # to get the users root file path
 
 connected_clients = set()
 has_connected_client = threading.Event()
+buffered_broadcasts = []
 
 async def broadcast(message):
+    buffered_broadcasts.append(message)
     if connected_clients:
         tasks = [asyncio.create_task(client.send(message)) for client in connected_clients]
         await asyncio.wait(tasks)
 
 async def handle_connection(websocket, path):
     connected_clients.add(websocket)
     if not has_connected_client.is_set():
         has_connected_client.set()
 
     try:
+        for message in buffered_broadcasts:
+            await websocket.send(message)
         async for message in websocket:
             print("GOT", message)
     except websockets.exceptions.ConnectionClosed as e:
         print(f"Client disconnected with reason: {e}")
     finally:
         connected_clients.remove(websocket)
 
-def _start_server(host: str, port: int):
+def _start_server(host: str, port: int, program_span: dict):
     loop = asyncio.new_event_loop()
     asyncio.set_event_loop(loop)
 
     start_server_coro = websockets.serve(handle_connection, host, port)
     server = loop.run_until_complete(start_server_coro)
 
     try:
         while True:
             if not threading.main_thread().is_alive():
                 break
             loop.run_until_complete(asyncio.sleep(1))
     finally:
-        loop.run_until_complete(broadcast(json.dumps({"event": "program_complete"})))
+        debugging.span_end(program_span)
         server.close()
         loop.run_until_complete(server.wait_closed())
         loop.close()
 
 
 class WebSocketLoggingHandler(logging.Handler):
     def __init__(self, *args, **kwargs):
@@ -56,25 +61,27 @@
         d = record.msg
         if isinstance(d, dict) and d["event"] == "span_start" and "task" in d and "mech" not in d:
             d["mech"] = self.Mechanism(d["task"])
         log_entry = self.format(record)
         asyncio.run(broadcast(log_entry))
 
 already_debugging = False
-def start_debugger_session(wait_for_connection = False, host = "localhost", port = 5678):
+def start_debugger_session(wait_for_connection = False, host = "0.0.0.0", port = 5678):
     global already_debugging
     if already_debugging:
         return
 
     already_debugging = True
     ws_handler = WebSocketLoggingHandler()
-    ws_handler.setFormatter(JsonFormatter())
-    logger.addHandler(ws_handler)
+    ws_handler.setFormatter(debugging.JsonFormatter())
+    debugging.logger.addHandler(ws_handler)
+
+    program_span = debugging.span_start("program",  main=os.path.relpath(__main__.__file__))
 
     # daemon so the make program exiting will kill the thread
-    server_thread = threading.Thread(target=_start_server, args=(host, port)) # , daemon=True
+    server_thread = threading.Thread(target=_start_server, args=(host, port, program_span)) # , daemon=True
     server_thread.start()
 
     if wait_for_connection:
         print(f"Waiting for debugger client to connect at ws://{host}:{port} ...")
         has_connected_client.wait()
         print("Connected.")
```

### Comparing `relationalai-0.2.2/src/relationalai/tools/dev.py` & `relationalai-0.2.3/src/relationalai/tools/dev.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/tests/conftest.py` & `relationalai-0.2.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/tests/end2end/README.md` & `relationalai-0.2.3/tests/end2end/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/tests/end2end/conftest.py` & `relationalai-0.2.3/tests/end2end/conftest.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/tests/end2end/test_graph_visualize.py` & `relationalai-0.2.3/tests/end2end/test_graph_visualize.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/tests/end2end/test_snapshots.py` & `relationalai-0.2.3/tests/end2end/test_snapshots.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,37 +3,40 @@
 
 import pytest
 import random
 from gentest.exec import path_to_slug, validate_query_results
 from relationalai.clients import config as cfg
 
 test_case_dir = Path(__file__).parent / "test_cases"
-test_case_files = [path for path in test_case_dir.iterdir() if path.suffix == ".py"]
+test_case_files = [path for path in test_case_dir.rglob("*.py")]
 
 # This test absorbs the latency of the engine being created
 def test_engine_creation_dummy(engine_config: cfg.Config):
     pass
 
 def randomize(name: str) -> str:
     return f"{name}_{random.randint(1000000000, 9999999999)}"
 
 
 @pytest.mark.parametrize(
     "file_path", test_case_files, ids=lambda path: path_to_slug(path, test_case_dir)
 )
 def test_snapshots(file_path: Path, snapshot, engine_config: cfg.Config):
+    # Clone the engine_config to ensure a fresh configuration for each test case
+    local_config = engine_config.clone()
+
     test_name = file_path.stem
     db_name = randomize(test_name)
     validate_query_results(
         file_path,
         snapshot,
         {
             "name": db_name,
-            "config": engine_config,
+            "config": local_config,
         }
     )
     try:
-        provider = rai.Resources(config=engine_config)
+        provider = rai.Resources(config=local_config)
         provider.delete_graph(db_name)
     except Exception as e:
         print(f"Failed to delete graph {db_name}: {e}")
         pass
```

### Comparing `relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt` & `relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/tests/end2end/test_cases/bool.py` & `relationalai-0.2.3/tests/end2end/test_cases/bool.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/tests/end2end/test_cases/bottom.py` & `relationalai-0.2.3/tests/end2end/test_cases/bottom.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/tests/end2end/test_cases/export.py` & `relationalai-0.2.3/tests/end2end/test_cases/export.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/tests/end2end/test_cases/multi_valued.py` & `relationalai-0.2.3/tests/end2end/test_cases/multi_valued.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/tests/end2end/test_cases/not_found.py` & `relationalai-0.2.3/tests/end2end/test_cases/not_found.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/tests/end2end/test_cases/persist.py` & `relationalai-0.2.3/tests/end2end/test_cases/persist.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/tests/end2end/test_cases/smoke.py` & `relationalai-0.2.3/tests/end2end/test_cases/smoke.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # pyright: reportUnusedExpression=false
 import relationalai as rai
 
-
 model = rai.Model(name=globals().get("name", ""), config=globals().get("config"))
 Person = model.Type("Person")
 Adult = model.Type("Adult")
 
 with model.rule():
     Person.add(name="Joe", age=74)
     Person.add(name="Bob", age=40)
```

### Comparing `relationalai-0.2.2/tests/end2end/test_cases/top.py` & `relationalai-0.2.3/tests/end2end/test_cases/top.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/tests/end2end/test_cases/weighted_graphs.py` & `relationalai-0.2.3/tests/end2end/test_cases/weighted_graphs.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/tests/init-cli/azure_basic.py` & `relationalai-0.2.3/tests/init-cli/azure_basic.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/tests/init-cli/common.py` & `relationalai-0.2.3/tests/init-cli/common.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/tests/roundtrip/test_document.py` & `relationalai-0.2.3/tests/roundtrip/test_document.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/tests/roundtrip/test_task.py` & `relationalai-0.2.3/tests/roundtrip/test_task.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.2/pyproject.toml` & `relationalai-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = 'relationalai'
-version = '0.2.2'
+version = '0.2.3'
 description = 'RelationalAI Library and CLI'
 readme="docs/pypi/README.md"
 authors = [
     { name="RelationalAI", email="support@relational.ai" },
 ]
 requires-python = ">= 3.10"
 dependencies = [
```

### Comparing `relationalai-0.2.2/PKG-INFO` & `relationalai-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: relationalai
-Version: 0.2.2
+Version: 0.2.3
 Summary: RelationalAI Library and CLI
 Author-email: RelationalAI <support@relational.ai>
 Requires-Python: >=3.10
 Requires-Dist: bytecode
 Requires-Dist: click
 Requires-Dist: colorama
 Requires-Dist: gravis
```

