# Comparing `tmp/zenoh_cli-0.5.0-py3-none-any.whl.zip` & `tmp/zenoh_cli-0.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 10265 bytes, number of entries: 7
--rw-r--r--  2.0 unx    13713 b- defN 24-Apr-09 06:03 zenoh_cli.py
--rw-r--r--  2.0 unx    11357 b- defN 24-Apr-09 06:03 zenoh_cli-0.5.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2255 b- defN 24-Apr-09 06:03 zenoh_cli-0.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-09 06:03 zenoh_cli-0.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       41 b- defN 24-Apr-09 06:03 zenoh_cli-0.5.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 24-Apr-09 06:03 zenoh_cli-0.5.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      564 b- defN 24-Apr-09 06:03 zenoh_cli-0.5.0.dist-info/RECORD
-7 files, 28032 bytes uncompressed, 9265 bytes compressed:  66.9%
+Zip file size: 10281 bytes, number of entries: 7
+-rw-r--r--  2.0 unx    13731 b- defN 24-Apr-19 19:31 zenoh_cli.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-Apr-19 19:31 zenoh_cli-0.5.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2282 b- defN 24-Apr-19 19:31 zenoh_cli-0.5.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-19 19:31 zenoh_cli-0.5.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       41 b- defN 24-Apr-19 19:31 zenoh_cli-0.5.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 24-Apr-19 19:31 zenoh_cli-0.5.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      564 b- defN 24-Apr-19 19:31 zenoh_cli-0.5.1.dist-info/RECORD
+7 files, 28077 bytes uncompressed, 9281 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: zenoh_cli.py
 Comment: 
 
-Filename: zenoh_cli-0.5.0.dist-info/LICENSE
+Filename: zenoh_cli-0.5.1.dist-info/LICENSE
 Comment: 
 
-Filename: zenoh_cli-0.5.0.dist-info/METADATA
+Filename: zenoh_cli-0.5.1.dist-info/METADATA
 Comment: 
 
-Filename: zenoh_cli-0.5.0.dist-info/WHEEL
+Filename: zenoh_cli-0.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: zenoh_cli-0.5.0.dist-info/entry_points.txt
+Filename: zenoh_cli-0.5.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: zenoh_cli-0.5.0.dist-info/top_level.txt
+Filename: zenoh_cli-0.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: zenoh_cli-0.5.0.dist-info/RECORD
+Filename: zenoh_cli-0.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zenoh_cli.py

```diff
@@ -109,22 +109,21 @@
     sys.stdout.write(f"{fmt.format(key=key, value=value)}\n")
     sys.stdout.flush()
 
 
 def get(
     session: zenoh.Session, parser: argparse.ArgumentParser, args: argparse.Namespace
 ):
-    for reply in session.get(args.selector, zenoh.Queue(), value=args.value):
-        if reply.is_ok:
-            response = reply.ok
-            _print_sample_to_stdout(response, args.line, args.decoder)
+    for response in session.get(args.selector, zenoh.Queue(), value=args.value):
+        if response.is_ok:
+            _print_sample_to_stdout(response.ok, args.line, args.decoder)
         else:
             logger.error(
                 "Received error (%s) on get(%s)",
-                reply.err.payload.decode(),
+                response.err.payload.decode(),
                 args.selector,
             )
 
 
 def subscribe(
     session: zenoh.Session, parser: argparse.ArgumentParser, args: argparse.Namespace
 ):
@@ -140,25 +139,29 @@
         except KeyboardInterrupt:
             sys.exit(0)
 
 
 def network(
     session: zenoh.Session, parser: argparse.ArgumentParser, args: argparse.Namespace
 ):
+    import matplotlib.pyplot as plt
+
+    plt.style.use("dark_background")
+    from jsonpointer import resolve_pointer
+
     graph = nx.Graph()
 
     # Scout the nearby network
     for answer in zenoh.scout(what="peer|client", timeout=1.0).receiver():
         graph.add_node(str(answer.zid), whatami=str(answer.whatami))
 
     # Query routers for more information
     for response in session.get("@/router/*", zenoh.Queue()):
         if response.is_ok:
-            reply = response.ok
-            data = json.loads(reply.payload)
+            data = json.loads(response.ok.payload)
 
             # Start adding edges and nodes
             zid = data["zid"]
             metadata = data["metadata"]
             graph.add_node(zid, whatami="router", metadata=metadata)
             for sess in data["sessions"]:
                 peer = sess["peer"]
@@ -167,74 +170,85 @@
                     [link.split("/")[0] for link in sess["links"]]
                 )
                 graph.add_node(peer, whatami=whatami)
                 graph.add_edge(zid, peer, protocol=link_protocols)
 
         else:
             logger.error(
-                "Received error (%s) on get(%s)",
-                reply.err.payload.decode(),
-                args.selector,
+                "Received error (%s)",
+                response.err.payload.decode(),
             )
+            pass
 
     pos = nx.spring_layout(graph, seed=3113794652)
 
     # Nodes
     routers = [
         node for node, attrs in graph.nodes.items() if attrs["whatami"] == "router"
     ]
-    peers = [node for node, attrs in graph.nodes.items() if attrs["whatami"] == "peer"]
-    clients = [
-        node for node, attrs in graph.nodes.items() if attrs["whatami"] == "client"
+    peers_clients = [
+        node
+        for node, attrs in graph.nodes.items()
+        if attrs["whatami"] in ("peer", "client")
     ]
-
     me = str(session.info().zid())
 
+    # Node labels
+    labels = {
+        zid: resolve_pointer(attributes, f"/metadata{args.metadata_field}", zid[:5])
+        for zid, attributes in graph.nodes(data=True)
+    }
+    labels[me] = "Me!"
+
     nx.draw_networkx(
         graph,
         pos,
         nodelist=routers,
-        node_color="#1f77b4",
+        edgelist=[],
+        node_color="steelblue",
         node_size=500,
         with_labels=False,
     )
     nx.draw_networkx(
-        graph, pos, nodelist=peers, node_color="#ff7f0e", with_labels=False
+        graph,
+        pos,
+        nodelist=peers_clients,
+        edgelist=[],
+        node_color="aliceblue",
+        with_labels=False,
     )
+
     nx.draw_networkx(
-        graph, pos, nodelist=clients, node_color="#17becf", with_labels=False
+        graph,
+        pos,
+        nodelist=[me],
+        edgelist=[],
+        node_color="lightcoral",
+        with_labels=False,
     )
-    nx.draw_networkx(graph, pos, nodelist=[me], node_color="#d62728", with_labels=False)
 
-    # Node labels
-    labels = {zid: zid[:5] for zid in nx.nodes(graph)}
-    nx.draw_networkx_labels(graph, pos, labels, font_color="y")
+    nx.draw_networkx_labels(
+        graph, pos, labels, font_color="darkgrey", font_weight="bold"
+    )
 
     # Edges
-    nx.draw_networkx_edge_labels(
-        graph, pos, edge_labels=nx.get_edge_attributes(graph, "protocol"), rotate=False
+    nx.draw_networkx(
+        graph,
+        pos,
+        nodelist=[],
+        edge_color="white",
+        with_labels=False,
     )
-
-    # Rendering of legend
-    import matplotlib.pyplot as plt
-    import matplotlib.patches as mpatches
-
-    orange_legend_entry = mpatches.Patch(color="#1f77b4", label="Routers")
-    blue_legend_entry = mpatches.Patch(color="#ff7f0e", label="Peers")
-    white_legend_entry = mpatches.Patch(color="#17becf", label="Clients")
-    red_legend_entry = mpatches.Patch(color="#d62728", label="Me")
-    plt.legend(
-        handles=[
-            orange_legend_entry,
-            blue_legend_entry,
-            white_legend_entry,
-            red_legend_entry,
-        ]
+    nx.draw_networkx_edge_labels(
+        graph,
+        pos,
+        edge_labels=nx.get_edge_attributes(graph, "protocol"),
+        rotate=False,
+        font_color="black",
     )
-
     plt.tight_layout()
     plt.axis("off")
     plt.show()
 
 
 ## Bundled codecs
 
@@ -363,14 +377,20 @@
     ## Info subcommand
     info_parser = subparsers.add_parser("info")
     info_parser.set_defaults(func=info)
 
     ## Network subcommand
     network_parser = subparsers.add_parser("network")
     network_parser.set_defaults(func=network)
+    network_parser.add_argument(
+        "--metadata-field",
+        type=str,
+        default="/name",
+        help="JSON pointer to a field in a routers metadata configuration",
+    )
 
     ## Scout subcommand
     scout_parser = subparsers.add_parser("scout")
     scout_parser.add_argument("-w", "--what", type=str, default="peer|router")
     scout_parser.add_argument("-t", "--timeout", type=float, default=1.0)
     scout_parser.set_defaults(func=scout)
```

## Comparing `zenoh_cli-0.5.0.dist-info/LICENSE` & `zenoh_cli-0.5.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `zenoh_cli-0.5.0.dist-info/METADATA` & `zenoh_cli-0.5.1.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: zenoh-cli
-Version: 0.5.0
+Version: 0.5.1
 Summary: CLI for Zenoh
 Home-page: https://github.com/MO-RISE/zenoh-cli
 Author: Fredrik Olsson
 Author-email: fredrik.x.olsson@ri.se
 Maintainer: Fredrik Olsson
 Maintainer-email: fredrik.x.olsson@ri.se
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: eclipse-zenoh ==0.10.1-rc
 Requires-Dist: parse
 Requires-Dist: networkx
 Requires-Dist: matplotlib
+Requires-Dist: jsonpointer
 Requires-Dist: importlib-metadata ; python_version < "3.10"
 
 # zenoh-cli
 A command line tool for interacting with a Zenoh session
 
 Typical use cases include:
 * Tests
```

## Comparing `zenoh_cli-0.5.0.dist-info/RECORD` & `zenoh_cli-0.5.1.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-zenoh_cli.py,sha256=st7KMBL2vSNw2OvZZhceKMBAkasi_Rm8mM8SebhEyeM,13713
-zenoh_cli-0.5.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-zenoh_cli-0.5.0.dist-info/METADATA,sha256=nzO7Po8TBHrTuIaAmqnso7DLfpPGEOBqovBU_ieEkD0,2255
-zenoh_cli-0.5.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-zenoh_cli-0.5.0.dist-info/entry_points.txt,sha256=aJfwoOb7Ak5fcAMmsVTFUKD3NTKV7NqeeTubpzDJ_9U,41
-zenoh_cli-0.5.0.dist-info/top_level.txt,sha256=PGGVngbuVqtbHeVek9BhAjXH9RX1zpSsTAzxcxR9jS0,10
-zenoh_cli-0.5.0.dist-info/RECORD,,
+zenoh_cli.py,sha256=u0i9Q7ryu-6oRFjx_mgzkQ0xiQcGVRpGndT0o94Ezvs,13731
+zenoh_cli-0.5.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+zenoh_cli-0.5.1.dist-info/METADATA,sha256=lSr4fJ_ABNlQReRrbdeFQ_2zH5xFmoxxGAoPDKe7dcw,2282
+zenoh_cli-0.5.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+zenoh_cli-0.5.1.dist-info/entry_points.txt,sha256=aJfwoOb7Ak5fcAMmsVTFUKD3NTKV7NqeeTubpzDJ_9U,41
+zenoh_cli-0.5.1.dist-info/top_level.txt,sha256=PGGVngbuVqtbHeVek9BhAjXH9RX1zpSsTAzxcxR9jS0,10
+zenoh_cli-0.5.1.dist-info/RECORD,,
```

