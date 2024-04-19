# Comparing `tmp/airbyte_source_zendesk_support-2.3.1.dev202404101450.tar.gz` & `tmp/airbyte_source_zendesk_support-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_zendesk_support-2.3.1.dev202404101450.tar", max compression
+gzip compressed data, was "airbyte_source_zendesk_support-2.4.0.tar", max compression
```

## Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450.tar` & `airbyte_source_zendesk_support-2.4.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     4663 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/README.md
--rw-r--r--   0        0        0      848 2024-04-10 14:50:39.470050 airbyte_source_zendesk_support-2.3.1.dev202404101450/pyproject.toml
--rw-r--r--   0        0        0     1212 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/__init__.py
--rw-r--r--   0        0        0      255 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/run.py
--rw-r--r--   0        0        0      392 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/account_attributes.json
--rw-r--r--   0        0        0     1064 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/article_comments.json
--rw-r--r--   0        0        0     1714 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/articles.json
--rw-r--r--   0        0        0     1625 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/attribute_definitions.json
--rw-r--r--   0        0        0      877 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/audit_logs.json
--rw-r--r--   0        0        0     1068 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/brands.json
--rw-r--r--   0        0        0     5246 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/custom_roles.json
--rw-r--r--   0        0        0      682 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/deleted_tickets.json
--rw-r--r--   0        0        0      514 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/group_memberships.json
--rw-r--r--   0        0        0      630 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/groups.json
--rw-r--r--   0        0        0     1423 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/macros.json
--rw-r--r--   0        0        0     1284 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/organization_fields.json
--rw-r--r--   0        0        0      651 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/organization_memberships.json
--rw-r--r--   0        0        0     1210 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/organizations.json
--rw-r--r--   0        0        0     1004 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/post_comments.json
--rw-r--r--   0        0        0     1595 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/posts.json
--rw-r--r--   0        0        0      801 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/satisfaction_ratings.json
--rw-r--r--   0        0        0      708 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/schedules.json
--rw-r--r--   0        0        0     1958 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/shared/attachments.json
--rw-r--r--   0        0        0     1835 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/shared/metadata.json
--rw-r--r--   0        0        0     4244 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/shared/tickets.json
--rw-r--r--   0        0        0     1617 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/shared/via.json
--rw-r--r--   0        0        0     2707 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/shared/via_channel.json
--rw-r--r--   0        0        0     1929 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/sla_policies.json
--rw-r--r--   0        0        0      165 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/tags.json
--rw-r--r--   0        0        0    17835 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/ticket_audits.json
--rw-r--r--   0        0        0     1151 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/ticket_comments.json
--rw-r--r--   0        0        0     2335 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/ticket_fields.json
--rw-r--r--   0        0        0     1359 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/ticket_forms.json
--rw-r--r--   0        0        0      394 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/ticket_metric_events.json
--rw-r--r--   0        0        0     3616 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/ticket_metrics.json
--rw-r--r--   0        0        0      512 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/ticket_skips.json
--rw-r--r--   0        0        0       27 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/tickets.json
--rw-r--r--   0        0        0      902 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/topics.json
--rw-r--r--   0        0        0     1054 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/user_fields.json
--rw-r--r--   0        0        0     4496 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/users.json
--rw-r--r--   0        0        0      647 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/votes.json
--rw-r--r--   0        0        0     7528 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/source.py
--rw-r--r--   0        0        0     5975 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/spec.json
--rw-r--r--   0        0        0    36901 2024-04-10 13:53:21.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/streams.py
--rw-r--r--   0        0        0     5438 1970-01-01 00:00:00.000000 airbyte_source_zendesk_support-2.3.1.dev202404101450/PKG-INFO
+-rw-r--r--   0        0        0     4663 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/README.md
+-rw-r--r--   0        0        0      832 2024-04-19 13:51:04.605049 airbyte_source_zendesk_support-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1212 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/__init__.py
+-rw-r--r--   0        0        0      255 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/run.py
+-rw-r--r--   0        0        0      392 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/account_attributes.json
+-rw-r--r--   0        0        0     1064 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/article_comments.json
+-rw-r--r--   0        0        0     1714 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/articles.json
+-rw-r--r--   0        0        0     1625 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/attribute_definitions.json
+-rw-r--r--   0        0        0      877 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/audit_logs.json
+-rw-r--r--   0        0        0     1068 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/brands.json
+-rw-r--r--   0        0        0     5246 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/custom_roles.json
+-rw-r--r--   0        0        0      682 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/deleted_tickets.json
+-rw-r--r--   0        0        0      514 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/group_memberships.json
+-rw-r--r--   0        0        0      630 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/groups.json
+-rw-r--r--   0        0        0     1423 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/macros.json
+-rw-r--r--   0        0        0     1284 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/organization_fields.json
+-rw-r--r--   0        0        0      651 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/organization_memberships.json
+-rw-r--r--   0        0        0     1210 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/organizations.json
+-rw-r--r--   0        0        0     1004 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/post_comments.json
+-rw-r--r--   0        0        0     1595 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/posts.json
+-rw-r--r--   0        0        0      801 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/satisfaction_ratings.json
+-rw-r--r--   0        0        0      708 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/schedules.json
+-rw-r--r--   0        0        0     1958 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/shared/attachments.json
+-rw-r--r--   0        0        0     1835 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/shared/metadata.json
+-rw-r--r--   0        0        0     4244 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/shared/tickets.json
+-rw-r--r--   0        0        0     1617 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/shared/via.json
+-rw-r--r--   0        0        0     2707 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/shared/via_channel.json
+-rw-r--r--   0        0        0     1929 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/sla_policies.json
+-rw-r--r--   0        0        0      165 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/tags.json
+-rw-r--r--   0        0        0    17835 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/ticket_audits.json
+-rw-r--r--   0        0        0     1151 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/ticket_comments.json
+-rw-r--r--   0        0        0     2335 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/ticket_fields.json
+-rw-r--r--   0        0        0     1359 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/ticket_forms.json
+-rw-r--r--   0        0        0      394 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/ticket_metric_events.json
+-rw-r--r--   0        0        0     3616 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/ticket_metrics.json
+-rw-r--r--   0        0        0      512 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/ticket_skips.json
+-rw-r--r--   0        0        0       27 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/tickets.json
+-rw-r--r--   0        0        0      902 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/topics.json
+-rw-r--r--   0        0        0     1054 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/user_fields.json
+-rw-r--r--   0        0        0     4496 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/users.json
+-rw-r--r--   0        0        0      647 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/votes.json
+-rw-r--r--   0        0        0     7572 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/source.py
+-rw-r--r--   0        0        0     5975 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/spec.json
+-rw-r--r--   0        0        0    38860 2024-04-19 12:42:49.000000 airbyte_source_zendesk_support-2.4.0/source_zendesk_support/streams.py
+-rw-r--r--   0        0        0     5422 1970-01-01 00:00:00.000000 airbyte_source_zendesk_support-2.4.0/PKG-INFO
```

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/README.md` & `airbyte_source_zendesk_support-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/pyproject.toml` & `airbyte_source_zendesk_support-2.4.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.3.1.dev202404101450"
+version = "2.4.0"
 name = "airbyte-source-zendesk-support"
 description = "Source implementation for Zendesk Support."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "ELv2"
 readme = "README.md"
```

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/__init__.py` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/article_comments.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/article_comments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/articles.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/articles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/attribute_definitions.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/attribute_definitions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/audit_logs.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/audit_logs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/brands.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/brands.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/custom_roles.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/custom_roles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/deleted_tickets.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/deleted_tickets.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/group_memberships.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/group_memberships.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/groups.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/groups.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/macros.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/macros.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/organization_fields.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/organization_fields.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/organization_memberships.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/organization_memberships.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/organizations.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/organizations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/post_comments.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/post_comments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/posts.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/posts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/satisfaction_ratings.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/satisfaction_ratings.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/schedules.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/schedules.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/shared/attachments.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/shared/attachments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/shared/metadata.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/shared/metadata.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/shared/tickets.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/shared/tickets.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/shared/via.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/shared/via.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/shared/via_channel.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/shared/via_channel.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/sla_policies.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/sla_policies.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/ticket_audits.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/ticket_audits.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/ticket_comments.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/ticket_comments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/ticket_fields.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/ticket_fields.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/ticket_forms.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/ticket_forms.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/ticket_metrics.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/ticket_metrics.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/ticket_skips.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/ticket_skips.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/topics.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/topics.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/user_fields.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/user_fields.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/users.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/users.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/schemas/votes.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/schemas/votes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/source.py` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/source.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,14 +138,17 @@
         }
 
     def streams(self, config: Mapping[str, Any]) -> List[Stream]:
         """Returns relevant a list of available streams
         :param config: A Mapping of the user input configuration as defined in the connector spec.
         """
         args = self.convert_config2stream_args(config)
+
+        tickets = Tickets(**args)
+
         streams = [
             Articles(**args),
             ArticleComments(**args),
             ArticleCommentVotes(**args),
             ArticleVotes(**args),
             AuditLogs(**args),
             GroupMemberships(**args),
@@ -160,18 +163,18 @@
             PostVotes(**args),
             SatisfactionRatings(**args),
             SlaPolicies(**args),
             Tags(**args),
             TicketAudits(**args),
             TicketComments(**args),
             TicketFields(**args),
-            TicketMetrics(**args),
+            TicketMetrics(parent=tickets, **args),
             TicketMetricEvents(**args),
             TicketSkips(**args),
-            Tickets(**args),
+            tickets,
             Topics(**args),
             Users(**args),
             Brands(**args),
             CustomRoles(**args),
             Schedules(**args),
             UserFields(**args),
         ]
```

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/spec.json` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/source_zendesk_support/streams.py` & `airbyte_source_zendesk_support-2.4.0/source_zendesk_support/streams.py`

 * *Files 5% similar despite different names*

```diff
@@ -489,14 +489,39 @@
         """
         The stream returns 400 Bad Request StartTimeTooRecent when requesting tasks 1 second before now.
         Figured out during experiments that the most recent time needed for request to be successful is 3 seconds before now.
         """
         return super().validate_start_time(requested_start_time, value=3)
 
 
+class TicketSubstream(HttpSubStream, IncrementalZendeskSupportStream):
+    def request_params(
+        self,
+        stream_state: Mapping[str, Any],
+        stream_slice: Mapping[str, Any] = None,
+        next_page_token: Mapping[str, Any] = None,
+    ) -> MutableMapping[str, Any]:
+        return {}
+
+    def stream_slices(
+        self, sync_mode: SyncMode, cursor_field: Optional[List[str]] = None, stream_state: Optional[Mapping[str, Any]] = None
+    ) -> Iterable[Optional[Mapping[str, Any]]]:
+        parent_stream_state = None
+        if stream_state:
+            cursor_value = pendulum.parse(stream_state.get(self.cursor_field)).int_timestamp
+            parent_stream_state = {self.parent.cursor_field: cursor_value}
+
+        parent_records = self.parent.read_records(
+            sync_mode=SyncMode.incremental, cursor_field=cursor_field, stream_slice=None, stream_state=parent_stream_state
+        )
+
+        for record in parent_records:
+            yield {"ticket_id": record["id"]}
+
+
 class TicketComments(SourceZendeskSupportTicketEventsExportStream):
     """
     Fetch the TicketComments incrementaly from TicketEvents Export stream
     """
 
     list_entities_from_event = ["via_reference_id", "ticket_id", "timestamp"]
     sideload_param = "comment_events"
@@ -553,16 +578,43 @@
     """TicketFields stream: https://developer.zendesk.com/api-reference/ticketing/tickets/ticket_fields/"""
 
 
 class TicketForms(TimeBasedPaginationZendeskSupportStream):
     """TicketForms stream: https://developer.zendesk.com/api-reference/ticketing/tickets/ticket_forms"""
 
 
-class TicketMetrics(CursorPaginationZendeskSupportStream):
-    """TicketMetric stream: https://developer.zendesk.com/api-reference/ticketing/tickets/ticket_metrics/"""
+class TicketMetrics(TicketSubstream):
+    """TicketMetric stream: https://developer.zendesk.com/api-reference/ticketing/tickets/ticket_metrics/#show-ticket-metrics"""
+
+    response_list_name = "ticket_metric"
+
+    def path(
+        self,
+        *,
+        stream_state: Optional[Mapping[str, Any]] = None,
+        stream_slice: Optional[Mapping[str, Any]] = None,
+        next_page_token: Optional[Mapping[str, Any]] = None,
+    ) -> str:
+        return f"tickets/{stream_slice['ticket_id']}/metrics"
+
+    def parse_response(self, response: requests.Response, stream_state: Mapping[str, Any], **kwargs) -> Iterable[Mapping]:
+        """try to select relevant data only"""
+
+        try:
+            data = response.json().get(self.response_list_name or self.name) or {}
+        except requests.exceptions.JSONDecodeError:
+            data = {}
+
+        if not self.cursor_field:
+            yield data
+        else:
+            cursor_date = (stream_state or {}).get(self.cursor_field)
+            updated = data[self.cursor_field]
+            if not cursor_date or updated >= cursor_date:
+                yield data
 
 
 class TicketSkips(CursorPaginationZendeskSupportStream):
     """TicketSkips stream: https://developer.zendesk.com/api-reference/ticketing/tickets/ticket_skips/"""
 
     response_list_name = "skips"
 
@@ -650,16 +702,16 @@
 
     def _validate_response(self, response: requests.Response, stream_state: Mapping[str, Any]) -> bool:
         """
         Ticket Audits endpoint doesn't allow filtering by date, but all data sorted by descending.
         This method used to stop making requests once we receive a response with cursor value greater than actual cursor.
         This action decreases sync time as we don't filter extra records in parse response.
         """
-        data = response.json().get(self.response_list_name)
-        created_at = data[0].get(self.cursor_field)
+        data = response.json().get(self.response_list_name, [{}])
+        created_at = data[0].get(self.cursor_field, "")
         cursor_date = (stream_state or {}).get(self.cursor_field) or self._start_date
         return created_at >= cursor_date
 
     def _read_pages(
         self,
         records_generator_fn: Callable[
             [requests.PreparedRequest, requests.Response, Mapping[str, Any], Optional[Mapping[str, Any]]], Iterable[StreamData]
```

### Comparing `airbyte_source_zendesk_support-2.3.1.dev202404101450/PKG-INFO` & `airbyte_source_zendesk_support-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-zendesk-support
-Version: 2.3.1.dev202404101450
+Version: 2.4.0
 Summary: Source implementation for Zendesk Support.
 Home-page: https://airbyte.com
 License: ELv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
```

