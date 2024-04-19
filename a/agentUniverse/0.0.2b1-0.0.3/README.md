# Comparing `tmp/agentuniverse-0.0.2b1.tar.gz` & `tmp/agentUniverse-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentuniverse-0.0.2b1.tar", last modified: Wed Apr 17 10:21:50 2024, max compression
+gzip compressed data, was "agentUniverse-0.0.3.tar", last modified: Fri Apr 19 04:59:49 2024, max compression
```

## Comparing `agentuniverse-0.0.2b1.tar` & `agentUniverse-0.0.3.tar`

### file list

```diff
@@ -1,261 +1,261 @@
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.257498 agentuniverse-0.0.2b1/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)    11335 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/LICENSE
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2723 2024-04-17 10:21:50.257058 agentuniverse-0.0.2b1/PKG-INFO
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1944 2024-04-12 13:32:53.000000 agentuniverse-0.0.2b1/README.md
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.256647 agentuniverse-0.0.2b1/agentUniverse.egg-info/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2723 2024-04-17 10:21:50.000000 agentuniverse-0.0.2b1/agentUniverse.egg-info/PKG-INFO
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     9829 2024-04-17 10:21:50.000000 agentuniverse-0.0.2b1/agentUniverse.egg-info/SOURCES.txt
--rw-r--r--   0 jerry.zzw   (501) staff       (20)        1 2024-04-17 10:21:50.000000 agentuniverse-0.0.2b1/agentUniverse.egg-info/dependency_links.txt
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      362 2024-04-17 10:21:50.000000 agentuniverse-0.0.2b1/agentUniverse.egg-info/requires.txt
--rw-r--r--   0 jerry.zzw   (501) staff       (20)       68 2024-04-17 10:21:50.000000 agentuniverse-0.0.2b1/agentUniverse.egg-info/top_level.txt
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.225573 agentuniverse-0.0.2b1/agentuniverse/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:12:13.000000 agentuniverse-0.0.2b1/agentuniverse/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.226498 agentuniverse-0.0.2b1/agentuniverse/agent/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.226653 agentuniverse-0.0.2b1/agentuniverse/agent/action/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.227144 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.227609 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/embedding/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/embedding/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      959 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/embedding/embedding.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     4460 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/embedding/openai_embedding.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3097 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/knowledge.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      655 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/knowledge_manager.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.227910 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/reader/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/reader/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.228812 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/reader/file/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/reader/file/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1160 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/reader/file/docx_reader.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1638 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/reader/file/file_reader.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1568 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/reader/file/pdf_reader.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1460 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/reader/file/pptx_reader.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1465 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/reader/file/web_pdf_reader.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      552 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/reader/reader.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.229569 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/store/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/store/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     4648 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/store/chroma_store.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1971 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/store/document.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      662 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/store/query.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3190 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/store/store.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.230157 agentuniverse-0.0.2b1/agentuniverse/agent/action/tool/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/tool/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      276 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/tool/enum.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3855 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/tool/tool.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      626 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/tool/tool_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     5371 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      639 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/agent_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      526 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/agent_model.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.231772 agentuniverse-0.0.2b1/agentuniverse/agent/default/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/default/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3034 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/default/executing_agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      365 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/agentuniverse/agent/default/executing_agent.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1937 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/default/expressing_agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      362 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/agentuniverse/agent/default/expressing_agent.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1532 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/default/planning_agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      352 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/agentuniverse/agent/default/planning_agent.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1247 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/default/rag_agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      266 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/agentuniverse/agent/default/rag_agent.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1862 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/default/reviewing_agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      357 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/agentuniverse/agent/default/reviewing_agent.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      657 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/input_object.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.232961 agentuniverse-0.0.2b1/agentuniverse/agent/memory/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-09 07:08:39.000000 agentuniverse-0.0.2b1/agentuniverse/agent/memory/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3675 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/memory/chat_memory.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      402 2024-04-01 06:19:56.000000 agentuniverse-0.0.2b1/agentuniverse/agent/memory/enum.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     7755 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/memory/langchain_instance.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3042 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/memory/memory.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      635 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/memory/memory_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      508 2024-04-09 16:15:17.000000 agentuniverse-0.0.2b1/agentuniverse/agent/memory/message.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1759 2024-04-09 06:57:56.000000 agentuniverse-0.0.2b1/agentuniverse/agent/memory/prompt.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      572 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/output_object.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.233116 agentuniverse-0.0.2b1/agentuniverse/agent/plan/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.233550 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.234170 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/executing_planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/executing_planner/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3103 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/executing_planner/executing_planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      195 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/executing_planner/executing_planner.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1287 2024-04-09 16:15:17.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/executing_planner/prompt.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.234771 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/expressing_planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/expressing_planner/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3040 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      200 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1493 2024-04-09 16:15:17.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/expressing_planner/prompt.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.235220 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/peer_planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      158 2024-04-09 16:15:17.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/peer_planner/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     7621 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/peer_planner/peer_planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      170 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/peer_planner/peer_planner.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     6397 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      659 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/planner_manager.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.235814 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/planning_planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/planning_planner/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2987 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/planning_planner/planning_planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      190 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/planning_planner/planning_planner.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1178 2024-04-09 16:15:17.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/planning_planner/prompt.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.236411 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/rag_planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/rag_planner/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      675 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/rag_planner/prompt.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2784 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/rag_planner/rag_planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/rag_planner/rag_planner.yaml
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.237008 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/reviewing_planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/reviewing_planner/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1212 2024-04-09 16:15:17.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/reviewing_planner/prompt.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3041 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      195 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.yaml
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.237748 agentuniverse-0.0.2b1/agentuniverse/agent_serve/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)        0 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent_serve/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1944 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent_serve/service.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3152 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/agentuniverse/agent_serve/service_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1161 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent_serve/service_instance.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      402 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent_serve/service_manager.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.238660 agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.238970 agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/dal/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/dal/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.239273 agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/dal/entity/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/dal/entity/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1075 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/dal/entity/request_do.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     5231 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/dal/request_library.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     9326 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/request_task.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1146 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/thread_with_result.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2573 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/web_booster.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     5064 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/web_server.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2434 2024-04-09 16:15:17.000000 agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/web_util.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.239569 agentuniverse-0.0.2b1/agentuniverse/base/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     9452 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/agentuniverse.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.239864 agentuniverse-0.0.2b1/agentuniverse/base/annotation/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/annotation/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      515 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/annotation/singleton.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.241006 agentuniverse-0.0.2b1/agentuniverse/base/component/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/component/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1081 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/component/application_component_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1264 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/component/component_base.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     4129 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/component/component_configer_util.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      604 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/component/component_enum.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2576 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/component/component_manager_base.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.241495 agentuniverse-0.0.2b1/agentuniverse/base/config/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.242242 agentuniverse-0.0.2b1/agentuniverse/base/config/application_configer/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/application_configer/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3885 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/application_configer/app_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1006 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/application_configer/application_config_manager.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.242791 agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2557 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/component_configer.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.244172 agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/configers/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/configers/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2599 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/configers/agent_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2053 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/configers/knowledge_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3272 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/configers/llm_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2540 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/configers/memory_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2392 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/configers/planner_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2192 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/configers/tool_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      423 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/config_type_enum.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     4828 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/configer.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.244503 agentuniverse-0.0.2b1/agentuniverse/base/config/custom_configer/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/custom_configer/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      707 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/custom_configer/custom_key_configer.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.245015 agentuniverse-0.0.2b1/agentuniverse/base/context/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/context/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1447 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/context/framework_context.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2768 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/context/framework_context_manager.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.245822 agentuniverse-0.0.2b1/agentuniverse/base/util/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/util/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      307 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/util/env_util.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.246435 agentuniverse-0.0.2b1/agentuniverse/base/util/logging/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/util/logging/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     6600 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/util/logging/general_logger.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     5132 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/util/logging/logging_config.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     6395 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/agentuniverse/base/util/logging/logging_util.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      502 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/util/memory_util.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     6379 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/util/prompt_util.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      715 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/util/system_util.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.247325 agentuniverse-0.0.2b1/agentuniverse/llm/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/llm/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.247769 agentuniverse-0.0.2b1/agentuniverse/llm/default/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/llm/default/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1422 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/llm/default/default_openai_llm.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      223 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/agentuniverse/llm/default/default_openai_llm.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2911 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/llm/langchain_instance.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     4946 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/llm/llm.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      619 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/llm/llm_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      328 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/llm/llm_output.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     4514 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/llm/openai_llm.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.248248 agentuniverse-0.0.2b1/agentuniverse/prompt/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/prompt/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1931 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/prompt/prompt.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      834 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/prompt/prompt_model.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.248409 agentuniverse-0.0.2b1/agentuniverse_connector/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:12:13.000000 agentuniverse-0.0.2b1/agentuniverse_connector/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.248566 agentuniverse-0.0.2b1/agentuniverse_extension/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:13:12.000000 agentuniverse-0.0.2b1/agentuniverse_extension/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.248899 agentuniverse-0.0.2b1/agentuniverse_extension/logger/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse_extension/logger/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     7321 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse_extension/logger/sls_sink.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2160 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/pyproject.toml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)       38 2024-04-17 10:21:50.257551 agentuniverse-0.0.2b1/setup.cfg
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1201 2024-04-17 10:21:46.000000 agentuniverse-0.0.2b1/setup.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.249083 agentuniverse-0.0.2b1/tests/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:13:12.000000 agentuniverse-0.0.2b1/tests/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.249259 agentuniverse-0.0.2b1/tests/test_agentuniverse/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.249417 agentuniverse-0.0.2b1/tests/test_agentuniverse/mock/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/mock/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.250179 agentuniverse-0.0.2b1/tests/test_agentuniverse/mock/agent_serve/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/mock/agent_serve/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      535 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/mock/agent_serve/mock_agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      475 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/mock/agent_serve/mock_application_config_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      896 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/mock/agent_serve/mock_service_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      509 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/mock/agent_serve/mock_simple_service.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.250366 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.251082 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.251330 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/action/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/action/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.251745 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/action/knowledge/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/action/knowledge/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.252242 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/action/knowledge/embedding/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/action/knowledge/embedding/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1097 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/action/knowledge/embedding/test_embedding.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1566 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/action/knowledge/test_knowledge.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.252683 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/memory/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/memory/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3894 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/memory/test_memory.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      776 2024-04-12 13:27:46.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/test_agent.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.253684 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent_serve/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent_serve/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1237 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent_serve/test_service.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      920 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent_serve/test_service_instance.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1613 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent_serve/test_service_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      524 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent_serve/test_web_booster.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.253883 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/base/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/base/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.254266 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/base/context/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/base/context/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1442 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/base/context/test_framework_context.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.254450 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/base/util/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/base/util/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.254799 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/base/util/logging/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/base/util/logging/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1670 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/base/util/logging/test_logging_util.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.255138 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/llm/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/llm/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1264 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/llm/test_llm.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.255285 agentuniverse-0.0.2b1/tests/test_agentuniverse_connector/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse_connector/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.255437 agentuniverse-0.0.2b1/tests/test_agentuniverse_extension/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse_extension/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.255592 agentuniverse-0.0.2b1/tests/test_agentuniverse_extension/mock/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse_extension/mock/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.255951 agentuniverse-0.0.2b1/tests/test_agentuniverse_extension/mock/logger/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse_extension/mock/logger/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      620 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse_extension/mock/logger/mock_log_client.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.256110 agentuniverse-0.0.2b1/tests/test_agentuniverse_extension/unit/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse_extension/unit/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.256428 agentuniverse-0.0.2b1/tests/test_agentuniverse_extension/unit/logger/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse_extension/unit/logger/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1288 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse_extension/unit/logger/test_sls_sink.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.171234 agentUniverse-0.0.3/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)    11335 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/LICENSE
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2701 2024-04-19 04:59:49.170901 agentUniverse-0.0.3/PKG-INFO
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2560 2024-04-19 04:56:45.000000 agentUniverse-0.0.3/README.md
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.170492 agentUniverse-0.0.3/agentUniverse.egg-info/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2701 2024-04-19 04:59:49.000000 agentUniverse-0.0.3/agentUniverse.egg-info/PKG-INFO
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     9829 2024-04-19 04:59:49.000000 agentUniverse-0.0.3/agentUniverse.egg-info/SOURCES.txt
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)        1 2024-04-19 04:59:49.000000 agentUniverse-0.0.3/agentUniverse.egg-info/dependency_links.txt
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      362 2024-04-19 04:59:49.000000 agentUniverse-0.0.3/agentUniverse.egg-info/requires.txt
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)       68 2024-04-19 04:59:49.000000 agentUniverse-0.0.3/agentUniverse.egg-info/top_level.txt
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.134226 agentUniverse-0.0.3/agentuniverse/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:12:13.000000 agentUniverse-0.0.3/agentuniverse/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.135182 agentUniverse-0.0.3/agentuniverse/agent/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.135327 agentUniverse-0.0.3/agentuniverse/agent/action/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/action/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.135960 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.136408 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/embedding/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/embedding/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      957 2024-04-19 04:49:33.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/embedding/embedding.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     4458 2024-04-19 04:49:33.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/embedding/openai_embedding.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3097 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/knowledge.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      655 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/knowledge_manager.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.136699 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/reader/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/reader/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.137573 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/reader/file/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/reader/file/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1160 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/reader/file/docx_reader.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1636 2024-04-19 04:49:33.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/reader/file/file_reader.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1568 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/reader/file/pdf_reader.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1460 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/reader/file/pptx_reader.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1463 2024-04-19 04:49:33.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/reader/file/web_pdf_reader.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      552 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/reader/reader.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.138293 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/store/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/store/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     4644 2024-04-19 04:49:33.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/store/chroma_store.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1967 2024-04-19 04:49:33.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/store/document.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      662 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/store/query.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3190 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/store/store.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.138853 agentUniverse-0.0.3/agentuniverse/agent/action/tool/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/action/tool/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      276 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/action/tool/enum.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3853 2024-04-19 04:49:33.000000 agentUniverse-0.0.3/agentuniverse/agent/action/tool/tool.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      626 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/action/tool/tool_manager.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     5371 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/agent.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      639 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/agent_manager.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      526 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/agent_model.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.140398 agentUniverse-0.0.3/agentuniverse/agent/default/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/default/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3034 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/default/executing_agent.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      365 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/agent/default/executing_agent.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1937 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/default/expressing_agent.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      362 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/agent/default/expressing_agent.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1532 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/default/planning_agent.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      352 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/agent/default/planning_agent.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1247 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/default/rag_agent.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      266 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/agent/default/rag_agent.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1862 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/default/reviewing_agent.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      357 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/agent/default/reviewing_agent.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      657 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/input_object.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.142170 agentUniverse-0.0.3/agentuniverse/agent/memory/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-09 07:08:39.000000 agentUniverse-0.0.3/agentuniverse/agent/memory/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3675 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/memory/chat_memory.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      402 2024-04-01 06:19:56.000000 agentUniverse-0.0.3/agentuniverse/agent/memory/enum.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     7755 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/memory/langchain_instance.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3042 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/memory/memory.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      635 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/memory/memory_manager.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      508 2024-04-09 16:15:17.000000 agentUniverse-0.0.3/agentuniverse/agent/memory/message.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1759 2024-04-09 06:57:56.000000 agentUniverse-0.0.3/agentuniverse/agent/memory/prompt.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      572 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/output_object.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.142319 agentUniverse-0.0.3/agentuniverse/agent/plan/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.142782 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.143400 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/executing_planner/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/executing_planner/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3103 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/executing_planner/executing_planner.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      195 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/executing_planner/executing_planner.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1287 2024-04-09 16:15:17.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/executing_planner/prompt.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.143999 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/expressing_planner/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/expressing_planner/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3040 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      200 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1493 2024-04-09 16:15:17.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/expressing_planner/prompt.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.144444 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/peer_planner/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      158 2024-04-09 16:15:17.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/peer_planner/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     7621 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/peer_planner/peer_planner.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      170 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/peer_planner/peer_planner.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     6441 2024-04-19 04:58:00.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/planner.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      659 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/planner_manager.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.145155 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/planning_planner/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/planning_planner/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2987 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/planning_planner/planning_planner.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      190 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/planning_planner/planning_planner.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1178 2024-04-09 16:15:17.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/planning_planner/prompt.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.146445 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/rag_planner/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/rag_planner/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      675 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/rag_planner/prompt.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2784 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/rag_planner/rag_planner.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/rag_planner/rag_planner.yaml
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.147159 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/reviewing_planner/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/reviewing_planner/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1212 2024-04-09 16:15:17.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/reviewing_planner/prompt.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3041 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      195 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.yaml
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.148112 agentUniverse-0.0.3/agentuniverse/agent_serve/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)        0 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent_serve/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1944 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent_serve/service.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3152 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/agent_serve/service_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1161 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent_serve/service_instance.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      402 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent_serve/service_manager.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.149090 agentUniverse-0.0.3/agentuniverse/agent_serve/web/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent_serve/web/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.149466 agentUniverse-0.0.3/agentuniverse/agent_serve/web/dal/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent_serve/web/dal/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.149833 agentUniverse-0.0.3/agentuniverse/agent_serve/web/dal/entity/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent_serve/web/dal/entity/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1075 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent_serve/web/dal/entity/request_do.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     5231 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent_serve/web/dal/request_library.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     9326 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent_serve/web/request_task.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1146 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/agent_serve/web/thread_with_result.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2573 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/agent_serve/web/web_booster.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     5064 2024-04-19 04:49:33.000000 agentUniverse-0.0.3/agentuniverse/agent_serve/web/web_server.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2434 2024-04-09 16:15:17.000000 agentUniverse-0.0.3/agentuniverse/agent_serve/web/web_util.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.150132 agentUniverse-0.0.3/agentuniverse/base/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     9442 2024-04-19 04:49:33.000000 agentUniverse-0.0.3/agentuniverse/base/agentuniverse.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.150426 agentUniverse-0.0.3/agentuniverse/base/annotation/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/annotation/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      515 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/annotation/singleton.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.151489 agentUniverse-0.0.3/agentuniverse/base/component/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/component/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1081 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/component/application_component_manager.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1264 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/component/component_base.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     4129 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/component/component_configer_util.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      604 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/component/component_enum.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2576 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/component/component_manager_base.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.152327 agentUniverse-0.0.3/agentuniverse/base/config/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/config/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.152859 agentUniverse-0.0.3/agentuniverse/base/config/application_configer/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/config/application_configer/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3885 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/config/application_configer/app_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1006 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/config/application_configer/application_config_manager.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.153219 agentUniverse-0.0.3/agentuniverse/base/config/component_configer/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/config/component_configer/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2557 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/config/component_configer/component_configer.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.154305 agentUniverse-0.0.3/agentuniverse/base/config/component_configer/configers/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/config/component_configer/configers/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2599 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/config/component_configer/configers/agent_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2053 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/config/component_configer/configers/knowledge_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3272 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/config/component_configer/configers/llm_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2540 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/config/component_configer/configers/memory_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2392 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/config/component_configer/configers/planner_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2192 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/config/component_configer/configers/tool_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      423 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/config/config_type_enum.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     4828 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/config/configer.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.154607 agentUniverse-0.0.3/agentuniverse/base/config/custom_configer/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/config/custom_configer/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      707 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/config/custom_configer/custom_key_configer.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.155433 agentUniverse-0.0.3/agentuniverse/base/context/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/context/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1447 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/context/framework_context.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2768 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/context/framework_context_manager.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.156355 agentUniverse-0.0.3/agentuniverse/base/util/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/util/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      307 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/util/env_util.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.156988 agentUniverse-0.0.3/agentuniverse/base/util/logging/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/util/logging/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     6600 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/base/util/logging/general_logger.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     5132 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/util/logging/logging_config.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     6395 2024-04-19 04:49:33.000000 agentUniverse-0.0.3/agentuniverse/base/util/logging/logging_util.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      502 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/base/util/memory_util.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     6379 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/base/util/prompt_util.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      715 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/base/util/system_util.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.158045 agentUniverse-0.0.3/agentuniverse/llm/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/llm/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.158645 agentUniverse-0.0.3/agentuniverse/llm/default/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/llm/default/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1422 2024-04-19 04:40:08.000000 agentUniverse-0.0.3/agentuniverse/llm/default/default_openai_llm.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      223 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/llm/default/default_openai_llm.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2907 2024-04-19 04:49:33.000000 agentUniverse-0.0.3/agentuniverse/llm/langchain_instance.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     4946 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/llm/llm.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      619 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/agentuniverse/llm/llm_manager.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      328 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/llm/llm_output.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     4512 2024-04-19 04:49:33.000000 agentUniverse-0.0.3/agentuniverse/llm/openai_llm.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.159214 agentUniverse-0.0.3/agentuniverse/prompt/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/prompt/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1931 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/agentuniverse/prompt/prompt.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      834 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse/prompt/prompt_model.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.159435 agentUniverse-0.0.3/agentuniverse_connector/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:12:13.000000 agentUniverse-0.0.3/agentuniverse_connector/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.159625 agentUniverse-0.0.3/agentuniverse_extension/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:13:12.000000 agentUniverse-0.0.3/agentuniverse_extension/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.160141 agentUniverse-0.0.3/agentuniverse_extension/logger/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse_extension/logger/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     7321 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/agentuniverse_extension/logger/sls_sink.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2074 2024-04-19 04:49:33.000000 agentUniverse-0.0.3/pyproject.toml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)       38 2024-04-19 04:59:49.171290 agentUniverse-0.0.3/setup.cfg
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1176 2024-04-19 04:56:45.000000 agentUniverse-0.0.3/setup.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.160542 agentUniverse-0.0.3/tests/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:13:12.000000 agentUniverse-0.0.3/tests/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.160724 agentUniverse-0.0.3/tests/test_agentuniverse/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.160885 agentUniverse-0.0.3/tests/test_agentuniverse/mock/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/mock/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.162360 agentUniverse-0.0.3/tests/test_agentuniverse/mock/agent_serve/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/mock/agent_serve/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      535 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/mock/agent_serve/mock_agent.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      475 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/mock/agent_serve/mock_application_config_manager.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      896 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/tests/test_agentuniverse/mock/agent_serve/mock_service_manager.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      509 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/tests/test_agentuniverse/mock/agent_serve/mock_simple_service.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.162595 agentUniverse-0.0.3/tests/test_agentuniverse/unit/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.163017 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.163229 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/action/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/action/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.163877 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/action/knowledge/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/action/knowledge/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.164274 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/action/knowledge/embedding/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/action/knowledge/embedding/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1097 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/action/knowledge/embedding/test_embedding.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1566 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/action/knowledge/test_knowledge.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.164720 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/memory/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/memory/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3894 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/memory/test_memory.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      786 2024-04-19 04:49:33.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/test_agent.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.166178 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent_serve/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent_serve/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1237 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent_serve/test_service.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      920 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent_serve/test_service_instance.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1613 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent_serve/test_service_manager.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      524 2024-04-19 04:49:33.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent_serve/test_web_booster.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.166373 agentUniverse-0.0.3/tests/test_agentuniverse/unit/base/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/base/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.166890 agentUniverse-0.0.3/tests/test_agentuniverse/unit/base/context/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/base/context/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1442 2024-04-19 04:34:47.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/base/context/test_framework_context.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.167095 agentUniverse-0.0.3/tests/test_agentuniverse/unit/base/util/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/base/util/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.167609 agentUniverse-0.0.3/tests/test_agentuniverse/unit/base/util/logging/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/base/util/logging/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1670 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/base/util/logging/test_logging_util.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.168168 agentUniverse-0.0.3/tests/test_agentuniverse/unit/llm/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/llm/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1264 2024-04-19 04:33:11.000000 agentUniverse-0.0.3/tests/test_agentuniverse/unit/llm/test_llm.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.168361 agentUniverse-0.0.3/tests/test_agentuniverse_connector/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse_connector/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.168522 agentUniverse-0.0.3/tests/test_agentuniverse_extension/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse_extension/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.168868 agentUniverse-0.0.3/tests/test_agentuniverse_extension/mock/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse_extension/mock/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.169577 agentUniverse-0.0.3/tests/test_agentuniverse_extension/mock/logger/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse_extension/mock/logger/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      620 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse_extension/mock/logger/mock_log_client.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.169812 agentUniverse-0.0.3/tests/test_agentuniverse_extension/unit/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse_extension/unit/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-19 04:59:49.170222 agentUniverse-0.0.3/tests/test_agentuniverse_extension/unit/logger/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.3/tests/test_agentuniverse_extension/unit/logger/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1288 2024-04-19 04:49:33.000000 agentUniverse-0.0.3/tests/test_agentuniverse_extension/unit/logger/test_sls_sink.py
```

### Comparing `agentuniverse-0.0.2b1/LICENSE` & `agentUniverse-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/PKG-INFO` & `agentUniverse-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: agentUniverse
-Version: 0.0.2b1
+Version: 0.0.3
 Summary: agentUniverse is a framework for developing applications powered by multi-agent base on large language model.
-Home-page: https://gitee.com/ant-fin-agent-framework/ant-fin-agent-framework
+Home-page: https://gitee.com/agentUniverse/agentUniverse
 Author: AntGroup
 Author-email: jerry.zzw@antgroup.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -27,18 +27,18 @@
 Requires-Dist: sphinx>=7.2.6
 Requires-Dist: sphinx-rtd-theme>=2.0.0
 Requires-Dist: aliyun-log-python-sdk>=0.8.8
 Requires-Dist: googleapis-common-protos>=1.63.0
 Requires-Dist: myst-parser>=2.0.0
 Requires-Dist: pdfminer.six
 
-# AgentUniverse
+# agentUniverse
 
 ## Overview
-AgentUniverse is a framework for developing applications powered by multi-agent base on large language model.  It provides all the essential components for building a single agent, and a multi-agent collaboration mechanism which  serves as a pattern factory that allowing developers to buid and customize multi-agent collaboration patterns. With this framework,  developers can easily construct multi-agent applications, and share the pattern practices from different technical  and business fields.
+agentUniverse is a framework for developing applications powered by multi-agent base on large language model.  It provides all the essential components for building a single agent, and a multi-agent collaboration mechanism which  serves as a pattern factory that allowing developers to buid and customize multi-agent collaboration patterns. With this framework,  developers can easily construct multi-agent applications, and share the pattern practices from different technical  and business fields.
 
 The framework will come with serveral pre-install multi-agent collaboration patterns which have been proven effective in real business scenarios, and will continue to be enriched in the future. Patterns that are currently about to be released include:
 
 - PEER pattern：
 This pattern utilizes four distinct agent roles: Plan, Execute, Express, and Review, to achieve a multi-step breakdown and sequential execution of a complex task. It also performs autonomous iteration based on evaluative feedback which enhancing performance in reasoning and analytical tasks.
```

### Comparing `agentuniverse-0.0.2b1/README.md` & `agentUniverse-0.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,44 @@
 # agentUniverse
 ****************************************
 Language version: [English](./README.md) | [中文](./README_zh.md)
 
-![](https://img.shields.io/badge/framework-aU-pink)
+![](https://img.shields.io/badge/framework-agentUniverse-pink)
 ![](https://img.shields.io/badge/python-3.10%2B-blue?logo=Python)
 [![](https://img.shields.io/badge/%20license-Apache--2.0-yellow)](LICENSE)
+[![Static Badge](https://img.shields.io/badge/pypi-v0.0.3-blue?logo=pypi)](https://pypi.org/project/agentUniverse/)
 ****************************************
 
 ## Overview
-AgentUniverse is a framework for developing applications powered by multi-agent base on large language model.  It provides all the essential components for building a single agent, and a multi-agent collaboration mechanism which  serves as a pattern factory that allowing developers to buid and customize multi-agent collaboration patterns. With this framework,  developers can easily construct multi-agent applications, and share the pattern practices from different technical  and business fields.
+agentUniverse is a framework for developing applications powered by multi-agent base on large language model.  It provides all the essential components for building a single agent, and a multi-agent collaboration mechanism which  serves as a pattern factory that allowing developers to buid and customize multi-agent collaboration patterns. With this framework,  developers can easily construct multi-agent applications, and share the pattern practices from different technical  and business fields.
 
 The framework will come with serveral pre-install multi-agent collaboration patterns which have been proven effective in real business scenarios, and will continue to be enriched in the future. Patterns that are currently about to be released include:
 
 - PEER pattern：
 This pattern utilizes four distinct agent roles: Plan, Execute, Express, and Review, to achieve a multi-step breakdown and sequential execution of a complex task. It also performs autonomous iteration based on evaluative feedback which enhancing performance in reasoning and analytical tasks. 
 
 
 - DOE pattern：
 This pattern consists of three agents: Data-fining agent, which is designed to solve data-intensive and high-computational-precision task; Opinion-inject agent, which combines the data results from first agent and the expert opinions which are pre-collected and structured; the third agent, Express agent generates the final result base on given document type and language style.
 
 More patterns are coming soon...
 
+## agentUniverseSample Project
+[agentUniverse Sample Project pending...](pending...)
+
 ## Quick Installation
 Using pip:
 ```shell
-pip install agentUniverse
-```
+pending...
+```
+
+## Quick Start
+We will show you how to:
+* Prepare the environment and application project
+* Build a simple agent
+* Use pattern components to complete multi-agent collaboration
+* Test and optimize the performance of the agent
+* Quickly serve the agent
+For details, please read [Quick Start pending...](pending...).
+
+## Guidebook
+For more detailed information, please refer to the [Guidebook  pending...]( pending...).
```

### Comparing `agentuniverse-0.0.2b1/agentUniverse.egg-info/PKG-INFO` & `agentUniverse-0.0.3/agentUniverse.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: agentUniverse
-Version: 0.0.2b1
+Version: 0.0.3
 Summary: agentUniverse is a framework for developing applications powered by multi-agent base on large language model.
-Home-page: https://gitee.com/ant-fin-agent-framework/ant-fin-agent-framework
+Home-page: https://gitee.com/agentUniverse/agentUniverse
 Author: AntGroup
 Author-email: jerry.zzw@antgroup.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -27,18 +27,18 @@
 Requires-Dist: sphinx>=7.2.6
 Requires-Dist: sphinx-rtd-theme>=2.0.0
 Requires-Dist: aliyun-log-python-sdk>=0.8.8
 Requires-Dist: googleapis-common-protos>=1.63.0
 Requires-Dist: myst-parser>=2.0.0
 Requires-Dist: pdfminer.six
 
-# AgentUniverse
+# agentUniverse
 
 ## Overview
-AgentUniverse is a framework for developing applications powered by multi-agent base on large language model.  It provides all the essential components for building a single agent, and a multi-agent collaboration mechanism which  serves as a pattern factory that allowing developers to buid and customize multi-agent collaboration patterns. With this framework,  developers can easily construct multi-agent applications, and share the pattern practices from different technical  and business fields.
+agentUniverse is a framework for developing applications powered by multi-agent base on large language model.  It provides all the essential components for building a single agent, and a multi-agent collaboration mechanism which  serves as a pattern factory that allowing developers to buid and customize multi-agent collaboration patterns. With this framework,  developers can easily construct multi-agent applications, and share the pattern practices from different technical  and business fields.
 
 The framework will come with serveral pre-install multi-agent collaboration patterns which have been proven effective in real business scenarios, and will continue to be enriched in the future. Patterns that are currently about to be released include:
 
 - PEER pattern：
 This pattern utilizes four distinct agent roles: Plan, Execute, Express, and Review, to achieve a multi-step breakdown and sequential execution of a complex task. It also performs autonomous iteration based on evaluative feedback which enhancing performance in reasoning and analytical tasks.
```

### Comparing `agentuniverse-0.0.2b1/agentUniverse.egg-info/SOURCES.txt` & `agentUniverse-0.0.3/agentUniverse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/embedding/embedding.py` & `agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/embedding/embedding.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,9 +26,9 @@
         """Get embeddings."""
 
     @abstractmethod
     async def async_get_embeddings(self, texts: List[str]) -> List[List[float]]:
         """Asynchronously get embeddings."""
 
     def as_langchain(self) -> LCEmbeddings:
-        """Convert the AFAF embedding class to the langchain embedding class."""
+        """Convert the aU embedding class to the langchain embedding class."""
         pass
```

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/embedding/openai_embedding.py` & `agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/embedding/openai_embedding.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,10 +95,10 @@
 
             # Return the embeddings as a list of lists of floats
             return [embedding.embedding for embedding in data]
         except BadRequestError as e:
             raise ValueError(e.message)
 
     def as_langchain(self) -> OpenAIEmbeddings:
-        """Convert the AFAF openai embedding class to the langchain openai embedding class."""
+        """Convert the aU openai embedding class to the langchain openai embedding class."""
         return OpenAIEmbeddings(openai_api_key=self.openai_api_key,
                                 client=self.client.embeddings, async_client=self.async_client.embeddings)
```

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/knowledge.py` & `agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/knowledge.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/knowledge_manager.py` & `agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/knowledge_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/reader/file/docx_reader.py` & `agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/reader/file/docx_reader.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/reader/file/file_reader.py` & `agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/reader/file/file_reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     ".pdf": PdfReader,
     ".docx": DocxReader,
     ".pptx": PptxReader,
 }
 
 
 class FileReader(Reader):
-    """The AFAF file reader class.
+    """The aU file reader class.
 
     FileReader is used to load data from files based on the provided file paths.
 
     Attributes:
         file_readers (Dict[str, Type[Reader]], optional): The file reader dictionary,
         the key is the suffix of the file, and the value is the specific file reader class.
     """
```

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/reader/file/pdf_reader.py` & `agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/reader/file/pdf_reader.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/reader/file/pptx_reader.py` & `agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/reader/file/pptx_reader.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/reader/file/web_pdf_reader.py` & `agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/reader/file/web_pdf_reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import requests
 
 from agentuniverse.agent.action.knowledge.reader.reader import Reader
 from agentuniverse.agent.action.knowledge.store.document import Document
 
 
 class WebPdfReader(Reader):
-    """The AFAF web pdf reader.
+    """The aU web pdf reader.
 
     The pdf file will be downloaded and then parsed by `pdfminer.six`.
     """
 
     def load_data(self, web_pdf_url: str) -> List[Document]:
         if web_pdf_url is None:
             return []
```

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/reader/reader.py` & `agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/reader/reader.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/store/chroma_store.py` & `agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/store/chroma_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
                 query_embeddings=[embedding]
             )
         else:
             query_result = self.collection.query(
                 n_results=query.similarity_top_k,
                 query_texts=[query.query_str]
             )
-        # convert to the AFAF document format
+        # convert to the aU document format
         return self.to_documents(query_result)
 
     def insert_documents(self, documents: List[Document], **kwargs: Any):
         """Insert documents to the chroma collection.
 
         Args:
             documents (List[Document]): The documents to be inserted.
@@ -97,15 +97,15 @@
                 metadatas=[document.metadata],
                 embeddings=[embedding] if embedding is not None else None,
                 ids=[document.id]
             )
 
     @staticmethod
     def to_documents(query_result: QueryResult) -> List[Document]:
-        """Convert the query results of ChromaDB to the AFAF document format."""
+        """Convert the query results of ChromaDB to the aU document format."""
 
         if query_result is None:
             return []
         documents = []
         for i in range(len(query_result['ids'][0])):
             documents.append(Document(id=query_result['ids'][0][i],
                                       text=query_result['documents'][0][i],
```

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/store/document.py` & `agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/store/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,24 +29,24 @@
     def as_langchain(self) -> LCDocument:
         """Convert to LangChain document format."""
         metadata = self.metadata or {}
         return LCDocument(page_content=self.text, metadata=metadata)
 
     @staticmethod
     def as_langchain_list(document_list) -> List[LCDocument]:
-        """Convert AFAF document list to langchain document list """
+        """Convert aU document list to langchain document list """
         langchain_document_list = []
         if document_list is None:
             return langchain_document_list
         for document in document_list:
             langchain_document_list.append(LCDocument(page_content=document.text, metadata=document.metadata))
         return langchain_document_list
 
     @staticmethod
     def from_langchain_list(lc_document_list: List[LCDocument]):
-        """Convert langchain document list to AFAF document list """
+        """Convert langchain document list to aU document list """
         document_list = []
         if lc_document_list is None:
             return document_list
         for lc_document in lc_document_list:
             document_list.append(Document(text=lc_document.page_content, metadata=lc_document.metadata))
         return document_list
```

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/store/query.py` & `agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/store/query.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/store/store.py` & `agentUniverse-0.0.3/agentuniverse/agent/action/knowledge/store/store.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/action/tool/tool.py` & `agentUniverse-0.0.3/agentuniverse/agent/action/tool/tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
                 raise Exception(f'{self.get_instance_code()} - The input must include key: {key}.')
 
     @abstractmethod
     def execute(self, tool_input: ToolInput):
         raise NotImplementedError
 
     def as_langchain(self) -> LangchainTool:
-        """Convert the AFAF tool class to the langchain tool class."""
+        """Convert the aU tool class to the langchain tool class."""
         return LangchainTool(name=self.name,
                              func=self.run,
                              description=self.description)
 
     def get_instance_code(self) -> str:
         """Return the full name of the tool."""
         appname = ApplicationConfigManager().app_configer.base_info_appname
```

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/action/tool/tool_manager.py` & `agentUniverse-0.0.3/agentuniverse/agent/action/tool/tool_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/agent.py` & `agentUniverse-0.0.3/agentuniverse/agent/agent.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/agent_manager.py` & `agentUniverse-0.0.3/agentuniverse/agent/agent_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/agent_model.py` & `agentUniverse-0.0.3/agentuniverse/agent/agent_model.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/default/executing_agent.py` & `agentUniverse-0.0.3/agentuniverse/agent/default/executing_agent.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/default/expressing_agent.py` & `agentUniverse-0.0.3/agentuniverse/agent/default/expressing_agent.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/default/planning_agent.py` & `agentUniverse-0.0.3/agentuniverse/agent/default/planning_agent.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/default/rag_agent.py` & `agentUniverse-0.0.3/agentuniverse/agent/default/rag_agent.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/default/reviewing_agent.py` & `agentUniverse-0.0.3/agentuniverse/agent/default/reviewing_agent.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/input_object.py` & `agentUniverse-0.0.3/agentuniverse/agent/input_object.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/memory/chat_memory.py` & `agentUniverse-0.0.3/agentuniverse/agent/memory/chat_memory.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/memory/langchain_instance.py` & `agentUniverse-0.0.3/agentuniverse/agent/memory/langchain_instance.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/memory/memory.py` & `agentUniverse-0.0.3/agentuniverse/agent/memory/memory.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/memory/memory_manager.py` & `agentUniverse-0.0.3/agentuniverse/agent/memory/memory_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/memory/prompt.py` & `agentUniverse-0.0.3/agentuniverse/agent/memory/prompt.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/output_object.py` & `agentUniverse-0.0.3/agentuniverse/agent/output_object.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/executing_planner/executing_planner.py` & `agentUniverse-0.0.3/agentuniverse/agent/plan/planner/executing_planner/executing_planner.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/executing_planner/prompt.py` & `agentUniverse-0.0.3/agentuniverse/agent/plan/planner/executing_planner/prompt.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.py` & `agentUniverse-0.0.3/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/expressing_planner/prompt.py` & `agentUniverse-0.0.3/agentuniverse/agent/plan/planner/expressing_planner/prompt.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/peer_planner/peer_planner.py` & `agentUniverse-0.0.3/agentuniverse/agent/plan/planner/peer_planner/peer_planner.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/planner.py` & `agentUniverse-0.0.3/agentuniverse/agent/plan/planner/planner.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,16 @@
         params['messages'] = messages
         params['llm'] = llm
         params['input_key'] = self.input_key
         params['output_key'] = self.output_key
 
         memory: Memory = MemoryManager().get_instance_obj(memory_name)
         if memory is None:
-            LOGGER.warn('memory does not exist.')
+            # todo process memory warning
+            # LOGGER.warn('memory does not exist.')
             return None
         memory.set_by_agent_model(**params)
         langchain_memory: BaseMemory = memory.as_langchain()
 
         planner_input['chat_history'] = langchain_memory.load_memory_str
         return langchain_memory
```

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/planner_manager.py` & `agentUniverse-0.0.3/agentuniverse/agent/plan/planner/planner_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/planning_planner/planning_planner.py` & `agentUniverse-0.0.3/agentuniverse/agent/plan/planner/planning_planner/planning_planner.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/planning_planner/prompt.py` & `agentUniverse-0.0.3/agentuniverse/agent/plan/planner/planning_planner/prompt.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/rag_planner/prompt.py` & `agentUniverse-0.0.3/agentuniverse/agent/plan/planner/rag_planner/prompt.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/rag_planner/rag_planner.py` & `agentUniverse-0.0.3/agentuniverse/agent/plan/planner/rag_planner/rag_planner.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/reviewing_planner/prompt.py` & `agentUniverse-0.0.3/agentuniverse/agent/plan/planner/reviewing_planner/prompt.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.py` & `agentUniverse-0.0.3/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent_serve/service.py` & `agentUniverse-0.0.3/agentuniverse/agent_serve/service.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent_serve/service_configer.py` & `agentUniverse-0.0.3/agentuniverse/agent_serve/service_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent_serve/service_instance.py` & `agentUniverse-0.0.3/agentuniverse/agent_serve/service_instance.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/dal/entity/request_do.py` & `agentUniverse-0.0.3/agentuniverse/agent_serve/web/dal/entity/request_do.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/dal/request_library.py` & `agentUniverse-0.0.3/agentuniverse/agent_serve/web/dal/request_library.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/request_task.py` & `agentUniverse-0.0.3/agentuniverse/agent_serve/web/request_task.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/thread_with_result.py` & `agentUniverse-0.0.3/agentuniverse/agent_serve/web/thread_with_result.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/web_booster.py` & `agentUniverse-0.0.3/agentuniverse/agent_serve/web/web_booster.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/web_server.py` & `agentUniverse-0.0.3/agentuniverse/agent_serve/web/web_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 app = Flask(__name__)
 app.config['JSON_AS_ASCII'] = False
 
 
 @app.route("/echo")
 def echo():
-    return 'Welcome to AgentUniverse!!!'
+    return 'Welcome to agentUniverse!!!'
 
 
 @app.route("/liveness")
 def liveness():
     return make_standard_response(success=True,
                                   result="liveness health check pass!")
```

### Comparing `agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/web_util.py` & `agentUniverse-0.0.3/agentuniverse/agent_serve/web/web_util.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/base/agentuniverse.py` & `agentUniverse-0.0.3/agentuniverse/base/agentuniverse.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,24 +24,24 @@
 from agentuniverse.base.util.logging.logging_util import init_loggers
 from agentuniverse.agent_serve.web.request_task import RequestLibrary
 from agentuniverse.agent_serve.web.web_booster import GunicornApplication
 
 
 @singleton
 class AgentUniverse(object):
-    """AgentUniverse framework object, responsible for the framework initialization,
+    """agentUniverse object, responsible for the framework initialization,
        system variables management, etc."""
 
     def __init__(self):
         self.__application_container = ApplicationComponentManager()
         self.__config_container: ApplicationConfigManager = ApplicationConfigManager()
         self.__system_default_package = ['agentuniverse']
 
     def start(self, config_path: str = None):
-        """Start the AgentUniverse framework."""
+        """Start the agentUniverse framework."""
         # step0: get default config path
         project_root_path = get_project_root_path()
         app_path = project_root_path / 'app'
         if app_path.exists():
             sys.path.append(str(app_path))
         if not config_path:
             config_path = project_root_path / 'config' / 'config.toml'
```

### Comparing `agentuniverse-0.0.2b1/agentuniverse/base/annotation/singleton.py` & `agentUniverse-0.0.3/agentuniverse/base/annotation/singleton.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/base/component/application_component_manager.py` & `agentUniverse-0.0.3/agentuniverse/base/component/application_component_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/base/component/component_base.py` & `agentUniverse-0.0.3/agentuniverse/base/component/component_base.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/base/component/component_configer_util.py` & `agentUniverse-0.0.3/agentuniverse/base/component/component_configer_util.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/base/component/component_enum.py` & `agentUniverse-0.0.3/agentuniverse/base/component/component_enum.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/base/component/component_manager_base.py` & `agentUniverse-0.0.3/agentuniverse/base/component/component_manager_base.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/base/config/application_configer/app_configer.py` & `agentUniverse-0.0.3/agentuniverse/base/config/application_configer/app_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/base/config/application_configer/application_config_manager.py` & `agentUniverse-0.0.3/agentuniverse/base/config/application_configer/application_config_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/component_configer.py` & `agentUniverse-0.0.3/agentuniverse/base/config/component_configer/component_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/configers/agent_configer.py` & `agentUniverse-0.0.3/agentuniverse/base/config/component_configer/configers/agent_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/configers/knowledge_configer.py` & `agentUniverse-0.0.3/agentuniverse/base/config/component_configer/configers/knowledge_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/configers/llm_configer.py` & `agentUniverse-0.0.3/agentuniverse/base/config/component_configer/configers/llm_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/configers/memory_configer.py` & `agentUniverse-0.0.3/agentuniverse/base/config/component_configer/configers/memory_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/configers/planner_configer.py` & `agentUniverse-0.0.3/agentuniverse/base/config/component_configer/configers/planner_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/configers/tool_configer.py` & `agentUniverse-0.0.3/agentuniverse/base/config/component_configer/configers/tool_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/base/config/configer.py` & `agentUniverse-0.0.3/agentuniverse/base/config/configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/base/config/custom_configer/custom_key_configer.py` & `agentUniverse-0.0.3/agentuniverse/base/config/custom_configer/custom_key_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/base/context/framework_context.py` & `agentUniverse-0.0.3/agentuniverse/base/context/framework_context.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/base/context/framework_context_manager.py` & `agentUniverse-0.0.3/agentuniverse/base/context/framework_context_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/base/util/logging/general_logger.py` & `agentUniverse-0.0.3/agentuniverse/base/util/logging/general_logger.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/base/util/logging/logging_config.py` & `agentUniverse-0.0.3/agentuniverse/base/util/logging/logging_config.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/base/util/logging/logging_util.py` & `agentUniverse-0.0.3/agentuniverse/base/util/logging/logging_util.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/base/util/prompt_util.py` & `agentUniverse-0.0.3/agentuniverse/base/util/prompt_util.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/base/util/system_util.py` & `agentUniverse-0.0.3/agentuniverse/base/util/system_util.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/llm/default/default_openai_llm.py` & `agentUniverse-0.0.3/agentuniverse/llm/default/default_openai_llm.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import Any
 
 from agentuniverse.llm.llm_output import LLMOutput
 from agentuniverse.llm.openai_llm import OpenAILLM
 
 
 class DefaultOpenAILLM(OpenAILLM):
-    """The AgentUniverse default openai llm module.
+    """The agentUniverse default openai llm module.
 
     LLM parameters, such as name/description/model_name/max_tokens,
     are injected into this class by the default_openai_llm.yaml configuration.
     """
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
```

### Comparing `agentuniverse-0.0.2b1/agentuniverse/llm/langchain_instance.py` & `agentUniverse-0.0.3/agentuniverse/llm/langchain_instance.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 
 class LangchainOpenAI(ChatOpenAI):
     """Langchain OpenAI LLM wrapper."""
 
     def __init__(self, llm: LLM):
         """The __init__ method.
 
-        The AgentUniverse LLM instance is passed to this class as an argument.
-        Convert the attributes of AFAF LLM instance to the LangchainOpenAI object for initialization
+        The agentUniverse LLM instance is passed to this class as an argument.
+        Convert the attributes of aU LLM instance to the LangchainOpenAI object for initialization
 
         Args:
-            llm (LLM): the AFAF LLM instance.
+            llm (LLM): the aU LLM instance.
         """
         init_params = dict()
         init_params['model_name'] = llm.model_name if llm.model_name is not None else 'gpt-3.5-turbo'
         init_params['temperature'] = llm.temperature if llm.temperature is not None else 0.7
         init_params['request_timeout'] = llm.request_timeout
         init_params['max_tokens'] = llm.max_tokens
         init_params['max_retries'] = llm.max_retries if llm.max_retries is not None else 2
```

### Comparing `agentuniverse-0.0.2b1/agentuniverse/llm/llm.py` & `agentUniverse-0.0.3/agentuniverse/llm/llm.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/llm/llm_manager.py` & `agentUniverse-0.0.3/agentuniverse/llm/llm_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/llm/openai_llm.py` & `agentUniverse-0.0.3/agentuniverse/llm/openai_llm.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
             stream=self.streaming,
             **kwargs,
         )
         text = chat_completion.choices[0].message.content
         return LLMOutput(text=text)
 
     def as_langchain(self) -> BaseLanguageModel:
-        """Convert the AFAF openai llm class to the langchain openai llm class."""
+        """Convert the aU openai llm class to the langchain openai llm class."""
         return LangchainOpenAI(self)
 
     def set_by_agent_model(self, **kwargs) -> None:
         """ Assign values of parameters to the OpenAILLM model in the agent configuration."""
         super().set_by_agent_model(**kwargs)
         if 'openai_api_key' in kwargs and kwargs['openai_api_key']:
             self.openai_api_key = kwargs['openai_api_key']
```

### Comparing `agentuniverse-0.0.2b1/agentuniverse/prompt/prompt.py` & `agentUniverse-0.0.3/agentuniverse/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse/prompt/prompt_model.py` & `agentUniverse-0.0.3/agentuniverse/prompt/prompt_model.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/agentuniverse_extension/logger/sls_sink.py` & `agentUniverse-0.0.3/agentuniverse_extension/logger/sls_sink.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/pyproject.toml` & `agentUniverse-0.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 [tool.poetry]
-name = "AgentUniverse"
-version = "0.0.1"
-description = "AgentUniverse is a framework for developing applications powered by multi-agent base on large language model."
+name = "agentUniverse"
+version = "0.0.2"
+description = "agentUniverse is a framework for developing applications powered by multi-agent base on large language model."
 authors = ["AntGroup <AntGroup>"]
-#repository = ""
-#documentation = ""
 readme = "README.md"
-packages = [
-    { include = "agentuniverse" }
-]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.31.0"
 cffi = "^1.15.1"
 flask = "2.2"
 werkzeug = "2.2.2"
```

### Comparing `agentuniverse-0.0.2b1/setup.py` & `agentUniverse-0.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,26 +18,26 @@
         requirements = content.split('\n')
 
     return requirements
 
 
 setuptools.setup(
     name="agentUniverse",
-    version="0.0.2.beta1",
+    version="0.0.3",
     author="AntGroup",
     author_email="jerry.zzw@antgroup.com",
     description="agentUniverse is a framework for developing applications powered "
                 "by multi-agent base on large language model.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://gitee.com/ant-fin-agent-framework/ant-fin-agent-framework",
+    url="https://gitee.com/agentUniverse/agentUniverse",
     packages=setuptools.find_packages(),
     package_data={
             '': ['*.yaml'],
         },
     install_requires=read_requirements(),
     classifiers=[
         'Programming Language :: Python :: 3.10',
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
-)
+)
```

### Comparing `agentuniverse-0.0.2b1/tests/test_agentuniverse/mock/agent_serve/mock_agent.py` & `agentUniverse-0.0.3/tests/test_agentuniverse/mock/agent_serve/mock_agent.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/tests/test_agentuniverse/mock/agent_serve/mock_service_manager.py` & `agentUniverse-0.0.3/tests/test_agentuniverse/mock/agent_serve/mock_service_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/action/knowledge/embedding/test_embedding.py` & `agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/action/knowledge/embedding/test_embedding.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/action/knowledge/test_knowledge.py` & `agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/action/knowledge/test_knowledge.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/memory/test_memory.py` & `agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/memory/test_memory.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/test_agent.py` & `agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent/test_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,9 +19,8 @@
     def test_rag_agent(self):
         instance: Agent = AgentManager().get_instance_obj('rag_agent')
         output_object: OutputObject = instance.run(input='分析下先锋领航退出中国的原因')
         print(output_object.get_data('output'))
 
 
 if __name__ == '__main__':
-    pass
-
+    unittest.main()
```

### Comparing `agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent_serve/test_service.py` & `agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent_serve/test_service.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent_serve/test_service_instance.py` & `agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent_serve/test_service_instance.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent_serve/test_service_manager.py` & `agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent_serve/test_service_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent_serve/test_web_booster.py` & `agentUniverse-0.0.3/tests/test_agentuniverse/unit/agent_serve/test_web_booster.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/base/context/test_framework_context.py` & `agentUniverse-0.0.3/tests/test_agentuniverse/unit/base/context/test_framework_context.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/base/util/logging/test_logging_util.py` & `agentUniverse-0.0.3/tests/test_agentuniverse/unit/base/util/logging/test_logging_util.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/llm/test_llm.py` & `agentUniverse-0.0.3/tests/test_agentuniverse/unit/llm/test_llm.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/tests/test_agentuniverse_extension/mock/logger/mock_log_client.py` & `agentUniverse-0.0.3/tests/test_agentuniverse_extension/mock/logger/mock_log_client.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.2b1/tests/test_agentuniverse_extension/unit/logger/test_sls_sink.py` & `agentUniverse-0.0.3/tests/test_agentuniverse_extension/unit/logger/test_sls_sink.py`

 * *Files identical despite different names*

