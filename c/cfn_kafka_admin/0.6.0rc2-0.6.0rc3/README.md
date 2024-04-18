# Comparing `tmp/cfn_kafka_admin-0.6.0rc2.tar.gz` & `tmp/cfn_kafka_admin-0.6.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfn_kafka_admin-0.6.0rc2.tar", max compression
+gzip compressed data, was "cfn_kafka_admin-0.6.0rc3.tar", max compression
```

## Comparing `cfn_kafka_admin-0.6.0rc2.tar` & `cfn_kafka_admin-0.6.0rc3.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0    16725 2022-03-22 06:17:38.518532 cfn_kafka_admin-0.6.0rc2/LICENSE
--rw-r--r--   0        0        0     2314 2022-05-11 06:55:41.690789 cfn_kafka_admin-0.6.0rc2/README.rst
--rw-r--r--   0        0        0      225 2023-12-04 23:02:38.429865 cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/__init__.py
--rw-r--r--   0        0        0    21939 2023-12-04 22:14:42.038293 cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/cfn_kafka_admin.py
--rw-r--r--   0        0        0      652 2023-04-24 12:49:19.847982 cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/cfn_resources_definitions/__init__.py
--rw-r--r--   0        0        0     1905 2023-04-24 12:49:19.847982 cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/cfn_resources_definitions/custom.py
--rw-r--r--   0        0        0     1793 2023-04-24 12:49:19.847982 cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/cfn_resources_definitions/resource.py
--rw-r--r--   0        0        0     1852 2023-04-24 12:49:19.848981 cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/cli.py
--rw-r--r--   0        0        0     2949 2023-05-05 09:04:48.510208 cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/common.py
--rw-r--r--   0        0        0     1547 2023-12-04 22:56:22.531409 cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/kafka_resources/__init__.py
--rw-r--r--   0        0        0     3309 2023-12-04 22:56:22.531409 cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/kafka_resources/acls.py
--rw-r--r--   0        0        0     1649 2023-12-04 22:56:22.531409 cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/kafka_resources/topics/__init__.py
--rw-r--r--   0        0        0     3333 2023-12-04 22:56:22.531409 cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/kafka_resources/topics/create.py
--rw-r--r--   0        0        0     2063 2023-12-04 22:56:22.531409 cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/kafka_resources/topics/delete.py
--rw-r--r--   0        0        0     4308 2023-12-04 22:56:22.531409 cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/kafka_resources/topics/update.py
--rw-r--r--   0        0        0      136 2023-04-24 12:49:19.849982 cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/lambda_functions/__init__.py
--rw-r--r--   0        0        0     4926 2023-12-04 22:56:22.532409 cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/lambda_functions/acls.py
--rw-r--r--   0        0        0     6357 2023-12-04 22:14:42.058293 cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/lambda_functions/schemas.py
--rw-r--r--   0        0        0     8535 2023-12-04 22:56:22.532409 cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/lambda_functions/topics.py
--rw-r--r--   0        0        0      118 2023-04-24 12:49:19.850982 cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/models/__init__.py
--rw-r--r--   0        0        0    12326 2023-12-04 22:56:22.532409 cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/models/admin.py
--rw-r--r--   0        0        0      118 2023-04-24 12:49:19.850982 cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/specs/__init__.py
--rw-r--r--   0        0        0     2990 2023-12-04 23:02:38.644861 cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/specs/aws-cfn-kafka-admin-provider-schema.json
--rw-r--r--   0        0        0     2466 2023-12-04 23:02:38.644861 cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/specs/ews-kafka-acl.json
--rw-r--r--   0        0        0     2386 2023-12-04 23:02:38.643861 cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/specs/ews-kafka-parameters.json
--rw-r--r--   0        0        0     2130 2023-12-04 23:02:38.643861 cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/specs/ews-kafka-schema.json
--rw-r--r--   0        0        0     7051 2023-12-04 23:02:38.644861 cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/specs/ews-kafka-topic.json
--rw-r--r--   0        0        0     2573 2023-12-04 23:02:38.429865 cfn_kafka_admin-0.6.0rc2/pyproject.toml
--rw-r--r--   0        0        0     3687 1970-01-01 00:00:00.000000 cfn_kafka_admin-0.6.0rc2/PKG-INFO
+-rw-r--r--   0        0        0    16725 2022-03-22 06:17:38.518532 cfn_kafka_admin-0.6.0rc3/LICENSE
+-rw-r--r--   0        0        0     2314 2022-05-11 06:55:41.690789 cfn_kafka_admin-0.6.0rc3/README.rst
+-rw-r--r--   0        0        0      225 2024-04-18 22:54:32.979021 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/__init__.py
+-rw-r--r--   0        0        0    22377 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/cfn_kafka_admin.py
+-rw-r--r--   0        0        0      652 2023-04-24 12:49:19.847982 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/cfn_resources_definitions/__init__.py
+-rw-r--r--   0        0        0     1958 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/cfn_resources_definitions/custom.py
+-rw-r--r--   0        0        0     1793 2023-04-24 12:49:19.847982 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/cfn_resources_definitions/resource.py
+-rw-r--r--   0        0        0     1852 2023-04-24 12:49:19.848981 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/cli.py
+-rw-r--r--   0        0        0     2949 2023-05-05 09:04:48.510208 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/common.py
+-rw-r--r--   0        0        0     1012 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/kafka_resources/__init__.py
+-rw-r--r--   0        0        0     4202 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/kafka_resources/acls.py
+-rw-r--r--   0        0        0     1654 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/kafka_resources/topics/__init__.py
+-rw-r--r--   0        0        0     3082 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/kafka_resources/topics/create.py
+-rw-r--r--   0        0        0     1895 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/kafka_resources/topics/delete.py
+-rw-r--r--   0        0        0     4711 2024-04-18 22:54:19.305230 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/kafka_resources/topics/update.py
+-rw-r--r--   0        0        0      136 2024-04-17 21:17:54.966767 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/lambda_functions/__init__.py
+-rw-r--r--   0        0        0     3764 2024-04-18 22:54:19.306229 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/lambda_functions/acls.py
+-rw-r--r--   0        0        0     6408 2024-04-18 22:54:19.306229 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/lambda_functions/schemas.py
+-rw-r--r--   0        0        0     7956 2024-04-18 22:54:19.306229 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/lambda_functions/topics.py
+-rw-r--r--   0        0        0     2105 2024-04-18 22:54:19.306229 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/lambda_functions/utils.py
+-rw-r--r--   0        0        0      118 2023-04-24 12:49:19.850982 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/models/__init__.py
+-rw-r--r--   0        0        0    13210 2024-04-18 22:54:19.306229 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/models/admin.py
+-rw-r--r--   0        0        0      118 2023-04-24 12:49:19.850982 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/specs/__init__.py
+-rw-r--r--   0        0        0     2998 2024-04-18 22:54:33.235017 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/specs/aws-cfn-kafka-admin-provider-schema.json
+-rw-r--r--   0        0        0     2446 2024-04-18 22:54:33.235017 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/specs/ews-kafka-acl.json
+-rw-r--r--   0        0        0     2560 2024-04-18 22:54:33.235017 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/specs/ews-kafka-parameters.json
+-rw-r--r--   0        0        0     2150 2024-04-18 22:54:33.235017 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/specs/ews-kafka-schema.json
+-rw-r--r--   0        0        0     7182 2024-04-18 22:54:33.235017 cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/specs/ews-kafka-topic.json
+-rw-r--r--   0        0        0     2632 2024-04-18 22:59:23.114604 cfn_kafka_admin-0.6.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 cfn_kafka_admin-0.6.0rc3/PKG-INFO
```

### Comparing `cfn_kafka_admin-0.6.0rc2/LICENSE` & `cfn_kafka_admin-0.6.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.0rc2/README.rst` & `cfn_kafka_admin-0.6.0rc3/README.rst`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/cfn_kafka_admin.py` & `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/cfn_kafka_admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,29 +246,37 @@
         """
         Method to set the global new_settings
         """
         self.globals_config.update(
             {
                 "BootstrapServers": self.model.Globals.BootstrapServers.__root__,
                 "SASLUsername": self.model.Globals.SASLUsername.__root__
-                if self.model.Globals.SASLUsername.__root__
+                if self.model.Globals.SASLUsername
+                and self.model.Globals.SASLUsername.__root__
                 else Ref(AWS_NO_VALUE),
                 "SASLPassword": self.model.Globals.SASLPassword.__root__
-                if self.model.Globals.SASLPassword.__root__
+                if self.model.Globals.SASLPassword
+                and self.model.Globals.SASLPassword.__root__
                 else Ref(AWS_NO_VALUE),
                 "SASLMechanism": SASLMechanism[
                     self.model.Globals.SASLMechanism.name
                 ].value
-                if isinstance(self.model.Globals.SASLMechanism, SASLMechanism)
+                if self.model.Globals.SASLMechanism
+                and isinstance(self.model.Globals.SASLMechanism, SASLMechanism)
                 else self.model.Globals.SASLMechanism,
                 "SecurityProtocol": SecurityProtocol[
                     self.model.Globals.SecurityProtocol.name
                 ].value
-                if isinstance(self.model.Globals.SecurityProtocol, SecurityProtocol)
+                if self.model.Globals.SecurityProtocol
+                and isinstance(self.model.Globals.SecurityProtocol, SecurityProtocol)
                 else self.model.Globals.SecurityProtocol,
+                "ClientConfig": self.model.Globals.ClientConfig
+                if self.model.Globals.ClientConfig
+                and isinstance(self.model.Globals.ClientConfig, dict)
+                else Ref(AWS_NO_VALUE),
             }
         )
 
     def define_schema_definition_path(
         self, topic_name: str, subject_suffix: str, attribute: TopicSchemaDef
     ):
         file_name = None
```

### Comparing `cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/cfn_resources_definitions/__init__.py` & `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/cfn_resources_definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/cfn_resources_definitions/custom.py` & `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/cfn_resources_definitions/resource.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,70 +1,65 @@
 #  -*- coding: utf-8 -*-
 # SPDX-License-Identifier: MPL-2.0
 # Copyright 2020-2021 John Mille <john@ews-network.net>
 
-"""Definition of Custom::KafkaTopic."""
+"""Definition of EWS::Kafka::Topic resource."""
 
-from troposphere.cloudformation import CustomResource
+from troposphere import AWSObject
 from troposphere.validators import positive_integer
 
 from cfn_kafka_admin.cfn_resources_definitions import KafkaAclPolicy
 
 
-class KafkaTopic(CustomResource):
+class KafkaTopic(AWSObject):
     """
     Class to represent EWS::Kafka::Topic
     """
 
-    resource_type = "Custom::KafkaTopic"
-
+    resource_type = "EWS::Kafka::Topic"
     props = {
-        "Name": (str, True),
-        "PartitionsCount": (positive_integer, True),
-        "ReplicationFactor": (positive_integer, False),
         "BootstrapServers": (str, True),
+        "ReplicationFactor": (positive_integer, False),
         "SecurityProtocol": (str, False),
         "SASLMechanism": (str, False),
         "SASLUsername": (str, False),
         "SASLPassword": (str, False),
+        "Name": (str, True),
+        "PartitionsCount": (positive_integer, True),
         "Settings": (dict, False),
-        "ServiceToken": (str, True),
     }
 
 
-class KafkaAcl(CustomResource):
+class KafkaAcl(AWSObject):
     """
-    Class to represent Custom::KafkaACL
+    Class to represent EWS::Kafka::ACL
     """
 
-    resource_type = "Custom::KafkaACL"
-
+    resource_type = "EWS::Kafka::ACL"
     props = {
         "BootstrapServers": (str, True),
         "ReplicationFactor": (positive_integer, False),
         "SecurityProtocol": (str, False),
         "SASLMechanism": (str, False),
         "SASLUsername": (str, False),
         "SASLPassword": (str, False),
-        "ServiceToken": (str, True),
         "Policies": ([KafkaAclPolicy], True),
     }
 
 
-class KafkaTopicSchema(CustomResource):
+class KafkaTopicSchema(AWSObject):
     """
-    Class to represent Custom::EwsKafkaSchema
+    Class to represent EWS::Kafka::Schema
     """
 
-    resource_type = "Custom::KafkaSchema"
-
+    resource_type = "EWS::Kafka::Schema"
     props = {
         "RegistryUrl": (str, True),
         "RegistryUsername": (str, False),
         "RegistryPassword": (str, False),
         "RegistryUserInfo": (str, False),
         "Subject": (str, True),
-        "Serializer": (str, True),
+        "Type": (str, True),
         "Definition": ((str, dict), True),
+        "SerializeAttribute": (str, True),
         "CompatibilityMode": (str, True),
-        "ServiceToken": (str, True),
     }
```

### Comparing `cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/cfn_resources_definitions/resource.py` & `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/cfn_resources_definitions/custom.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,65 +1,71 @@
-#  -*- coding: utf-8 -*-
 # SPDX-License-Identifier: MPL-2.0
 # Copyright 2020-2021 John Mille <john@ews-network.net>
 
-"""Definition of EWS::Kafka::Topic resource."""
+"""Definition of Custom::KafkaTopic."""
 
-from troposphere import AWSObject
+from troposphere.cloudformation import CustomResource
 from troposphere.validators import positive_integer
 
 from cfn_kafka_admin.cfn_resources_definitions import KafkaAclPolicy
 
 
-class KafkaTopic(AWSObject):
+class KafkaTopic(CustomResource):
     """
     Class to represent EWS::Kafka::Topic
     """
 
-    resource_type = "EWS::Kafka::Topic"
+    resource_type = "Custom::KafkaTopic"
+
     props = {
-        "BootstrapServers": (str, True),
+        "Name": (str, True),
+        "PartitionsCount": (positive_integer, True),
         "ReplicationFactor": (positive_integer, False),
+        "BootstrapServers": (str, True),
         "SecurityProtocol": (str, False),
         "SASLMechanism": (str, False),
         "SASLUsername": (str, False),
         "SASLPassword": (str, False),
-        "Name": (str, True),
-        "PartitionsCount": (positive_integer, True),
         "Settings": (dict, False),
+        "ServiceToken": (str, True),
+        "ClientConfig": (dict, False),
     }
 
 
-class KafkaAcl(AWSObject):
+class KafkaAcl(CustomResource):
     """
-    Class to represent EWS::Kafka::ACL
+    Class to represent Custom::KafkaACL
     """
 
-    resource_type = "EWS::Kafka::ACL"
+    resource_type = "Custom::KafkaACL"
+
     props = {
         "BootstrapServers": (str, True),
         "ReplicationFactor": (positive_integer, False),
         "SecurityProtocol": (str, False),
         "SASLMechanism": (str, False),
         "SASLUsername": (str, False),
         "SASLPassword": (str, False),
+        "ServiceToken": (str, True),
         "Policies": ([KafkaAclPolicy], True),
+        "ClientConfig": (dict, False),
     }
 
 
-class KafkaTopicSchema(AWSObject):
+class KafkaTopicSchema(CustomResource):
     """
-    Class to represent EWS::Kafka::Schema
+    Class to represent Custom::EwsKafkaSchema
     """
 
-    resource_type = "EWS::Kafka::Schema"
+    resource_type = "Custom::KafkaSchema"
+
     props = {
         "RegistryUrl": (str, True),
         "RegistryUsername": (str, False),
         "RegistryPassword": (str, False),
         "RegistryUserInfo": (str, False),
         "Subject": (str, True),
-        "Type": (str, True),
+        "Serializer": (str, True),
         "Definition": ((str, dict), True),
-        "SerializeAttribute": (str, True),
         "CompatibilityMode": (str, True),
+        "ServiceToken": (str, True),
     }
```

### Comparing `cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/cli.py` & `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/cli.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/common.py` & `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/common.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/kafka_resources/topics/__init__.py` & `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/kafka_resources/topics/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: MPL-2.0
-# Copyright 2021 John Mille<john@ews-network.net>
+# Copyright 2021-2024 John Mille<john@ews-network.net>
 
 """
 Module to handle Kafka topics management.
 """
 
 from __future__ import annotations
```

### Comparing `cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/kafka_resources/topics/create.py` & `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/kafka_resources/topics/create.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 # SPDX-License-Identifier: MPL-2.0
-# Copyright 2021 John Mille<john@ews-network.net>
+# Copyright 2021-2024 John Mille<john@ews-network.net>
 
 from __future__ import annotations
 
 from os import environ
 
 from confluent_kafka import KafkaError, KafkaException
 from confluent_kafka.admin import ConfigResource, ResourceType
 from confluent_kafka.cimpl import NewTopic
-from kafka import errors
 from retry import retry
 
 from cfn_kafka_admin.kafka_resources import get_admin_client
 from cfn_kafka_admin.kafka_resources.topics import (
     LOG,
     RETRY_ATTEMPTS,
     RETRY_JITTER,
     wait_for_result,
 )
 
 
 @retry(
-    (
-        errors.KafkaError,
-        KafkaException,
-    ),
+    (KafkaException,),
     tries=RETRY_ATTEMPTS,
     jitter=RETRY_JITTER,
     logger=LOG,
 )
 def create_new_kafka_topic(
     topic_name,
     partitions: int,
@@ -64,29 +60,24 @@
         wait_for_result(admin_client.create_topics([new_topic], validate_only=False))
     except KafkaException as create_error:
         LOG.exception(create_error)
         if create_error.args[0] == KafkaError.TOPIC_ALREADY_EXISTS:
             if environ.get("FAIL_IF_ALREADY_EXISTS", None) is None:
                 return topic_name
             else:
-                raise errors.TopicAlreadyExistsError(
-                    f"Topic {topic_name} already exists"
-                )
-        raise errors.KafkaConnectionError(f"Failed to create topic {topic_name}")
+                raise create_error
+        raise create_error
     topic_config_resource = ConfigResource(ResourceType.TOPIC, topic_name)
     created_topic_config = validate_topic_created(admin_client, topic_config_resource)
     LOG.debug(created_topic_config)
     return topic_name
 
 
 @retry(
-    (
-        errors.KafkaError,
-        KafkaError,
-    ),
+    (KafkaError,),
     tries=RETRY_ATTEMPTS,
     jitter=RETRY_JITTER,
     logger=LOG,
 )
 def validate_topic_created(admin_client, topic_config_resource: ConfigResource):
     try:
         desc = wait_for_result(admin_client.describe_configs([topic_config_resource]))
```

### Comparing `cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/kafka_resources/topics/delete.py` & `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/kafka_resources/topics/delete.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,36 @@
 # SPDX-License-Identifier: MPL-2.0
-# Copyright 2021 John Mille<john@ews-network.net>
+# Copyright 2021-2024 John Mille<john@ews-network.net>
 
 from __future__ import annotations
 
 from time import sleep
 
 from confluent_kafka import KafkaError, KafkaException
 from confluent_kafka.admin import ConfigResource, ResourceType
-from kafka import errors
 from retry import retry
 
 from cfn_kafka_admin.kafka_resources import get_admin_client
 from cfn_kafka_admin.kafka_resources.topics import (
     LOG,
     RETRY_ATTEMPTS,
     RETRY_JITTER,
     describe_topic_configs,
     wait_for_result,
 )
 
 
 @retry(
-    (
-        errors.KafkaError,
-        KafkaException,
-    ),
+    (KafkaException,),
     tries=RETRY_ATTEMPTS,
     jitter=RETRY_JITTER,
     logger=LOG,
 )
 def delete_topic(topic_name: str, cluster_info: dict):
-    """
-    Function to delete kafka topic
-
-    :param topic_name: name of the topic to delete
-    :param cluster_info: cluster information
-    """
+    """Function to delete kafka topic"""
     admin_client = get_admin_client(cluster_info, "DELETE", topic_name)
     try:
         configs = describe_topic_configs(admin_client, topic_name, result_only=True)
         LOG.info(f"Deleting topic: {topic_name}")
         LOG.debug(f"{topic_name} => {configs}")
     except KafkaException as error:
         if error.args[0] == KafkaError.UNKNOWN_TOPIC_OR_PART:
```

### Comparing `cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/kafka_resources/topics/update.py` & `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/kafka_resources/topics/update.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: MPL-2.0
-# Copyright 2021 John Mille<john@ews-network.net>
+# Copyright 2021-2024 John Mille<john@ews-network.net>
 
 from __future__ import annotations
 
 from confluent_kafka.admin import (
     AlterConfigOpType,
     ConfigEntry,
     ConfigResource,
@@ -47,15 +47,18 @@
         LOG.debug(
             f"Topic {topic_name} partitions is already set to {topic_current_partitions}. Nothing to update"
         )
         return topic_current_partitions
 
 
 def update_kafka_topic(
-    topic_name: str, partitions: int, cluster_info: dict, settings: dict
+    topic_name: str,
+    partitions: int,
+    cluster_info: dict,
+    settings: dict,
 ):
     """
     Function to update existing Kafka topic
 
     :param topic_name:
     :param partitions:
     :param cluster_info:
@@ -94,25 +97,31 @@
                 )
                 new_config = ConfigEntry(
                     config_name,
                     str(setting_value),
                     incremental_operation=AlterConfigOpType["SET"],
                 )
                 incremental_configs.append(new_config)
-
-    wait_for_result(
-        admin_client.incremental_alter_configs(
-            [
-                ConfigResource(
-                    ResourceType.TOPIC,
-                    topic_name,
-                    incremental_configs=incremental_configs,
+    for _incremental_config in incremental_configs:
+        try:
+            wait_for_result(
+                admin_client.incremental_alter_configs(
+                    [
+                        ConfigResource(
+                            ResourceType.TOPIC,
+                            topic_name,
+                            incremental_configs=[_incremental_config],
+                        )
+                    ]
                 )
-            ]
-        )
-    )
+            )
+        except Exception as error:
+            LOG.error(
+                f"Error updating topic {topic_name} property {_incremental_config.name}={_incremental_config.value}: {error}"
+            )
+            LOG.exception(error)
+    partitions = update_topic_partitions(admin_client, topic_name, partitions)
     new_topic_configs = describe_topic_configs(
         admin_client, topic_name, result_only=True
     )
     LOG.debug(new_topic_configs)
-    partitions = update_topic_partitions(admin_client, topic_name, partitions)
     return partitions, new_topic_configs
```

### Comparing `cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/lambda_functions/acls.py` & `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/lambda_functions/acls.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # SPDX-License-Identifier: MPL-2.0
-# Copyright 2021 John Mille<john@ews-network.net>
+# Copyright 2021-2024 John Mille<john@ews-network.net>
 
 """Main module."""
 
 from __future__ import annotations
 
 import uuid
 
-from aws_cfn_custom_resource_resolve_parser import handle
 from cfn_resource_provider import ResourceProvider
 from compose_x_common.compose_x_common import keyisset, keypresent
 
 from cfn_kafka_admin.common import setup_logging
 from cfn_kafka_admin.kafka_resources.acls import (
     create_new_acls,
     delete_acls,
     differentiate_old_new_acls,
 )
 from cfn_kafka_admin.models.admin import EwsKafkaAcl
 
+from .utils import set_client_info
+
 LOG = setup_logging()
 
 
 class KafkaACL(ResourceProvider):
     def __init__(self):
         """
         Init method
@@ -41,42 +42,21 @@
                 self.properties[prop] = int(self.properties[prop])
         for prop in boolean_props:
             if keypresent(prop, self.properties) and isinstance(
                 self.properties[prop], str
             ):
                 self.properties[prop] = self.properties[prop].lower() == "true"
 
-    def define_cluster_info(self):
-        """
-        Method to define the cluster information into a simple format
-        """
-        try:
-            self.cluster_info["bootstrap_servers"] = self.get("BootstrapServers")
-            self.cluster_info["security_protocol"] = self.get("SecurityProtocol")
-            self.cluster_info["sasl_mechanism"] = self.get("SASLMechanism")
-            self.cluster_info["sasl_plain_username"] = self.get("SASLUsername")
-            self.cluster_info["sasl_plain_password"] = self.get("SASLPassword")
-        except Exception as error:
-            self.fail(f"Failed to get cluster information - {str(error)}")
-
-        for key, value in self.cluster_info.items():
-            if isinstance(value, str) and value.find("resolve:secretsmanager") >= 0:
-                try:
-                    self.cluster_info[key] = handle(value)
-                except Exception as error:
-                    LOG.error("Failed to import secrets from SecretsManager")
-                    self.fail(str(error))
-
     def create(self):
         """
         Method to create a new Kafka topic
         :return:
         """
+        set_client_info(self)
         try:
-            self.define_cluster_info()
             LOG.info(f"Connecting to {self.cluster_info['bootstrap_servers']}")
             LOG.info(f"Attempting to create new ACLs {self.get('Name')}")
             topic_name = create_new_acls(
                 self.get("Policies"),
                 self.cluster_info,
             )
             self.physical_resource_id = str(uuid.uuid4())
@@ -86,18 +66,15 @@
             self.physical_resource_id = "could-not-create"
             self.fail(f"Failed to create the ACLs. {str(error)}")
 
     def update(self):
         """
         :return:
         """
-        try:
-            self.define_cluster_info()
-        except Exception as error:
-            self.fail(str(error))
+        set_client_info(self)
         old_policies = self.get_old("Policies")
         for policy in old_policies:
             if not keyisset("Host", policy):
                 policy.update({"Host": "*"})
         new_policies = self.get("Policies")
         new_acls, to_delete_acls = differentiate_old_new_acls(
             new_policies, old_policies
@@ -119,19 +96,19 @@
         except Exception as error:
             LOG.error(error)
             LOG.error("Failed to create new ACLs")
             self.fail(str(error))
 
     def delete(self):
         """
-        Method to delete the Topic resource
+        Method to delete the ACLs resource
         :return:
         """
+        set_client_info(self)
         try:
-            self.define_cluster_info()
             delete_acls(self.get("Policies"), self.cluster_info)
             self.success("ACLs deleted")
         except Exception as error:
             self.fail(
                 f"Failed to delete topic {self.get_attribute('Name')}. {str(error)}"
             )
```

### Comparing `cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/lambda_functions/schemas.py` & `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/lambda_functions/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: MPL-2.0
-# Copyright 2021 John Mille<john@ews-network.net>
+# Copyright 2021-2024 John Mille<john@ews-network.net>
 
 """Module to handle the custom resource for Schemas"""
 
 from __future__ import annotations
 
 import json
 import logging
@@ -89,39 +89,36 @@
             password = user_info.split(":")[1]
         else:
             username = self.try_replace_from_secret("RegistryUsername")
             password = self.try_replace_from_secret("RegistryPassword")
         registry_url = self.try_replace_from_secret("RegistryUrl")
         LOG.info(registry_url)
         registry = SchemaRegistry(
-            **{
-                "SchemaRegistryUrl": registry_url,
-                "Username": username,
-                "Password": password,
-            }
+            registry_url,
+            **{"basic_auth.username": username, "basic_auth.password": password},
         )
         return registry
 
     def create(self):
         """
         Creates a new Schema / Version in the Schema Registry
         """
         try:
             registry = self.set_registry()
             subject = self.get("Subject")
             serializer = self.get("Serializer")
             compatibility = self.get("CompatibilityMode")
             schema_def = import_definition(self.get("Definition"))
-            schema = registry.post_subject_version(
+            schema = registry.post_subject_schema_version(
                 subject, schema_def, schema_type=serializer
             )
             registry.put_compatibility_subject_config(
                 subject_name=subject, compatibility=compatibility
             )
-            self.set_attribute("Id", schema["id"])
+            self.set_attribute("Id", schema.json()["id"])
             self.physical_resource_id = subject
             self.success("Schema version created")
         except Exception as error:
             LOG.exception(error)
             self.physical_resource_id = "could-not-create"
             self.fail(str(error))
 
@@ -134,24 +131,26 @@
             subject = self.get("Subject")
             serializer = self.get("Serializer")
             schema_def = import_definition(self.get("Definition"))
             compatible = registry.post_compatibility_subjects_versions(
                 subject_name=subject,
                 version_id="latest",
                 definition=schema_def,
-                definition_type=serializer,
-                as_bool=True,
-            )
+                schema_type=serializer,
+            ).json()["is_compatible"]
             if not compatible:
                 print(schema_def)
                 self.fail(
                     f"Schema for {subject} is not compatible with the latest version"
                 )
-            schema = registry.post_subject_version(subject, schema_def)
-            self.set_attribute("Id", schema["id"])
+                return
+            schema = registry.post_subject_schema_version(
+                subject, schema_def, schema_type=serializer
+            )
+            self.set_attribute("Id", schema.json()["id"])
             self.success("New schema version created")
         except Exception as error:
             LOG.exception(error)
             self.fail(str(error))
 
     def delete(self):
         """
```

### Comparing `cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/lambda_functions/topics.py` & `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/lambda_functions/topics.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # SPDX-License-Identifier: MPL-2.0
-# Copyright 2021 John Mille<john@ews-network.net>
+# Copyright 2021-2024 John Mille<john@ews-network.net>
 
 """Main module."""
 
 from __future__ import annotations
 
 import re
 from os import environ
 
 from aws_cfn_custom_resource_resolve_parser import handle
 from cfn_resource_provider import ResourceProvider
 from cfn_resource_provider.resource_provider import is_int
 from compose_x_common.compose_x_common import keypresent
-from kafka import errors
+from confluent_kafka import KafkaError, KafkaException
 
 from cfn_kafka_admin.common import setup_logging
 from cfn_kafka_admin.kafka_resources.topics.create import create_new_kafka_topic
 from cfn_kafka_admin.kafka_resources.topics.delete import delete_topic
 from cfn_kafka_admin.kafka_resources.topics.update import update_kafka_topic
 from cfn_kafka_admin.models.admin import EwsKafkaTopic
 
+from .utils import cfn_resolve_string, define_cluster_info, set_client_info
+
 LOG = setup_logging(__name__)
 
 INT_RE = re.compile(r"(^[1-9]+\d*$|^0$)")
 FLOAT_RE = re.compile(r"(^\d+\.\d+$|^\.\d+$)")
 
 
 def is_float(number: str) -> bool:
@@ -70,68 +72,51 @@
             else:
                 pass
         return properties
 
     def convert_property_types(self):
         self.heuristic_convert_property_types(self.properties)
         int_props = ["PartitionsCount", "ReplicationFactor"]
-        boolean_props = ["IsConfluentKafka"]
         for prop in int_props:
             if keypresent(prop, self.properties) and isinstance(
                 self.properties[prop], str
             ):
                 try:
                     self.properties[prop] = int(self.properties[prop])
                 except Exception as error:
                     self.fail(
                         f"Failed to get cluster information - {prop} - {str(error)}"
                     )
-        for prop in boolean_props:
-            if keypresent(prop, self.properties) and isinstance(
-                self.properties[prop], str
-            ):
-                self.properties[prop] = self.properties[prop].lower() == "true"
-
-    def define_cluster_info(self):
-        """
-        Method to define the cluster information into a simple format
-        """
-        try:
-            self.cluster_info["bootstrap_servers"] = self.get("BootstrapServers")
-            self.cluster_info["security_protocol"] = self.get("SecurityProtocol")
-            self.cluster_info["sasl_mechanism"] = self.get("SASLMechanism")
-            self.cluster_info["sasl_plain_username"] = self.get("SASLUsername")
-            self.cluster_info["sasl_plain_password"] = self.get("SASLPassword")
-        except Exception as error:
-            self.fail(f"Failed to get cluster information - {str(error)}")
 
-        for key, value in self.cluster_info.items():
+    def interpolate_secret_vars(self, config_input: dict) -> None:
+        for key, value in config_input.items():
             if isinstance(value, str) and value.find("resolve:secretsmanager") >= 0:
                 try:
-                    self.cluster_info[key] = handle(value)
+                    config_input[key] = handle(value)
                 except Exception as error:
                     LOG.error("Failed to import secrets from SecretsManager")
                     self.fail(str(error))
 
+    def define_cluster_info(self):
+        """Method to define the cluster information into a simple format"""
+        try:
+            self.cluster_info["bootstrap_servers"] = self.get("BootstrapServers")
+            self.cluster_info["security.protocol"] = self.get("SecurityProtocol")
+            self.cluster_info["sasl.mechanism"] = self.get("SASLMechanism")
+            self.cluster_info["sasl.username"] = self.get("SASLUsername")
+            self.cluster_info["sasl.password"] = self.get("SASLPassword")
+        except Exception as error:
+            self.fail(f"Failed to get cluster information - {str(error)}")
+
     def create(self):
         """
         Method to create a new Kafka topic
         :return:
         """
-        try:
-            LOG.info(f"Attempting to create new topic {self.get('Name')}")
-            self.define_cluster_info()
-            cluster_url = (
-                self.cluster_info["bootstrap.servers"]
-                if self.get("IsConfluentKafka")
-                else self.cluster_info["bootstrap_servers"]
-            )
-            LOG.info(f"Cluster is {cluster_url}")
-        except Exception as error:
-            self.fail(f"Failed to initialize - {str(error)}")
+        set_client_info(self)
         if not self.get("PartitionsCount") >= 1:
             self.fail("The number of partitions must be a strictly positive value >= 1")
         try:
             LOG.info(f'{self.get("Name")} - {self.get("Settings")}')
             topic_name = create_new_kafka_topic(
                 self.get("Name"),
                 self.get("PartitionsCount"),
@@ -140,30 +125,30 @@
                 topic_config=self.get("Settings"),
             )
             self.physical_resource_id = topic_name
             self.set_attribute("Name", self.get("Name"))
             self.set_attribute("Partitions", self.get("PartitionsCount"))
             self.set_attribute("BootstrapServers", self.get("BootstrapServers"))
             self.success(f"Created new topic {topic_name}")
-        except errors.TopicAlreadyExistsError as error:
+        except KafkaException as error:
             self.physical_resource_id = "could-not-create-nor-import"
             self.fail(
                 f"{self.get('Name')} - Topic already exists and import is disabled, {str(error)}"
             )
         except Exception as error:
             LOG.exception(error)
             self.physical_resource_id = "could-not-create"
             self.fail(f"Failed to create the topic {self.get('Name')}, {str(error)}")
 
     def update(self):
         """
         :return:
         """
+        set_client_info(self)
         try:
-            self.define_cluster_info()
             update_kafka_topic(
                 self.get("Name"),
                 self.get("PartitionsCount"),
                 self.cluster_info,
                 settings=self.get("Settings"),
             )
             self.physical_resource_id = self.get("Name")
@@ -177,29 +162,32 @@
             self.fail(str(error))
 
     def delete(self):
         """
         Method to delete the Topic resource
         :return:
         """
-        LOG.info("Delet: topic attribute name: {}".format(self.get("Name")))
+        LOG.info("Delete: topic attribute name: {}".format(self.get("Name")))
         LOG.info(f"DELETE: {self.stack_id} - {self.physical_resource_id}")
         if self.get("Name") and self.get("Name") != self.physical_resource_id:
             self.success("Name does not match physical ID. Skipping.")
             return
         elif self.get("Name") is None or (
             self.physical_resource_id
             and re.match(r"(.*)could-not-create(.*)$", self.physical_resource_id)
         ):
             LOG.warning("Deleting failed create resource.")
             self.success("Deleting non-working resource")
             return
+        set_client_info(self)
         try:
-            self.define_cluster_info()
-            delete_topic(self.get("Name"), self.cluster_info)
+            delete_topic(
+                self.get("Name"),
+                self.cluster_info,
+            )
             self.success(
                 f"Topic {self.get_attribute('Name')} does not exist. Nothing to delete."
             )
         except Exception as error:
             LOG.exception(error)
             if environ.get("DELETE_FAIL_ON_ERROR", None) is None:
                 self.success(
```

### Comparing `cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/specs/aws-cfn-kafka-admin-provider-schema.json` & `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/specs/aws-cfn-kafka-admin-provider-schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9739257812500001%*

 * *Differences: {"'definitions'": "{'SchemasDef': {'$ref': 'ews-kafka-schema.json#/'}, 'AclsModel': {'$ref': "*

 * *                  "'ews-kafka-acl.json#/'}}",*

 * * "'properties'": "{'Globals': {'$ref': 'ews-kafka-parameters.json#/'}, 'Topics': {'properties': "*

 * *                 "{'Topics': {'items': {'$ref': 'ews-kafka-topic.json#/'}}}}}"}*

```diff
@@ -1,15 +1,15 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "definitions": {
         "AclsModel": {
-            "$ref": "ews-kafka-acl.json"
+            "$ref": "ews-kafka-acl.json#/"
         },
         "SchemasDef": {
-            "$ref": "ews-kafka-schema.json"
+            "$ref": "ews-kafka-schema.json#/"
         }
     },
     "properties": {
         "ACLs": {
             "properties": {
                 "FunctionName": {
                     "description": "Name or ARN of the Lambda function to use for Custom::KafkaACL",
@@ -18,15 +18,15 @@
                 "Policies": {
                     "$ref": "ews-kafka-acl.json#/properties/Policies"
                 }
             },
             "type": "object"
         },
         "Globals": {
-            "$ref": "ews-kafka-parameters.json"
+            "$ref": "ews-kafka-parameters.json#/"
         },
         "Schemas": {
             "properties": {
                 "CompatibilityMode": {
                     "$ref": "ews-kafka-schema.json#/definitions/CompatibilityMode"
                 },
                 "DeletionPolicy": {
@@ -95,15 +95,15 @@
                     "type": "boolean"
                 },
                 "ReplicationFactor": {
                     "$ref": "ews-kafka-topic.json#/definitions/ReplicationFactor"
                 },
                 "Topics": {
                     "items": {
-                        "$ref": "ews-kafka-topic.json"
+                        "$ref": "ews-kafka-topic.json#/"
                     },
                     "type": "array"
                 }
             },
             "type": "object"
         }
     },
```

### Comparing `cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/specs/ews-kafka-acl.json` & `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/specs/ews-kafka-acl.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'sourceUrl'": "'https://github.com/compose-x/cfn-kafka-admin'"}*

```diff
@@ -84,10 +84,10 @@
             "items": {
                 "$ref": "#/definitions/PolicyDef"
             },
             "type": "array",
             "uniqueItems": true
         }
     },
-    "sourceUrl": "https://github.com/ews-network/cfn-kafka-topic-resource-provider",
+    "sourceUrl": "https://github.com/compose-x/cfn-kafka-admin",
     "typeName": "EWS::Kafka::ACL"
 }
```

### Comparing `cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/specs/ews-kafka-parameters.json` & `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/specs/ews-kafka-parameters.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9083333333333333%*

 * *Differences: {"'properties'": "{'ClientConfig': OrderedDict([('description', 'Client configuration as per the "*

 * *                 "librdkafka settings. Incompatible with the SASL & SecurityProtocol properties'), "*

 * *                 "('type', 'object')])}",*

 * * "'sourceUrl'": "'https://github.com/compose-x/cfn-kafka-admin'"}*

```diff
@@ -56,14 +56,18 @@
         }
     },
     "description": "Generic properties used to connect to Kafka cluster.",
     "properties": {
         "BootstrapServers": {
             "$ref": "#/definitions/BootstrapServers"
         },
+        "ClientConfig": {
+            "description": "Client configuration as per the librdkafka settings. Incompatible with the SASL & SecurityProtocol properties",
+            "type": "object"
+        },
         "CompatibilityMode": {
             "$ref": "ews-kafka-schema.json#/definitions/CompatibilityMode"
         },
         "RegistryPassword": {
             "$ref": "#/definitions/RegistryPassword"
         },
         "RegistryUrl": {
@@ -81,10 +85,10 @@
         "SASLUsername": {
             "$ref": "#/definitions/SASLUsername"
         },
         "SecurityProtocol": {
             "$ref": "#/definitions/SecurityProtocol"
         }
     },
-    "sourceUrl": "https://github.com/ews-network/aws_cfn_kafka_definitions",
+    "sourceUrl": "https://github.com/compose-x/cfn-kafka-admin",
     "typeName": "EWS::Kafka::Parameters"
 }
```

### Comparing `cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/specs/ews-kafka-schema.json` & `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/specs/ews-kafka-schema.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7857142857142857%*

 * *Differences: {"'sourceUrl'": "'https://github.com/compose-x/cfn-kafka-admin'", "'type'": "'object'"}*

```diff
@@ -82,10 +82,11 @@
             "description": "The Lambda Function ARN",
             "type": "string"
         },
         "Subject": {
             "type": "string"
         }
     },
-    "sourceUrl": "https://github.com/compose-x/cfn_kafka_admin",
+    "sourceUrl": "https://github.com/compose-x/cfn-kafka-admin",
+    "type": "object",
     "typeName": "EWS::Kafka::Schema"
 }
```

### Comparing `cfn_kafka_admin-0.6.0rc2/cfn_kafka_admin/specs/ews-kafka-topic.json` & `cfn_kafka_admin-0.6.0rc3/cfn_kafka_admin/specs/ews-kafka-topic.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8068181818181819%*

 * *Differences: {"'properties'": "{'ClientConfig': OrderedDict([('description', 'Client configuration as per the "*

 * *                 "librdkafka settings.'), ('type', 'object')])}",*

 * * "'sourceUrl'": "'https://github.com/compose-x/cfn-kafka-admin'",*

 * * "'type'": "'object'"}*

```diff
@@ -155,14 +155,18 @@
         }
     },
     "description": "Resource to create Kafka topics in your cluster.",
     "properties": {
         "BootstrapServers": {
             "$ref": "ews-kafka-parameters.json#/definitions/BootstrapServers"
         },
+        "ClientConfig": {
+            "description": "Client configuration as per the librdkafka settings.",
+            "type": "object"
+        },
         "Name": {
             "$ref": "#/definitions/Name"
         },
         "PartitionsCount": {
             "$ref": "#/definitions/PartitionsCount"
         },
         "ReplicationFactor": {
@@ -187,10 +191,11 @@
             "$ref": "#/definitions/TopicsSettings"
         }
     },
     "required": [
         "Name",
         "PartitionsCount"
     ],
-    "sourceUrl": "https://github.com/ews-network/cfn-kafka-acl-resource-provider",
+    "sourceUrl": "https://github.com/compose-x/cfn-kafka-admin",
+    "type": "object",
     "typeName": "EWS::Kafka::Topic"
 }
```

### Comparing `cfn_kafka_admin-0.6.0rc2/pyproject.toml` & `cfn_kafka_admin-0.6.0rc3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,73 +1,76 @@
 [tool.poetry]
 name = "cfn_kafka_admin"
-version = "0.6.0-rc2"
+version = "0.6.0-rc3"
 description = "AWS CloudFormation Resources to manage Kafka"
 authors = ["John Mille <john@compose-x.io>"]
 classifiers = [
   "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
   "Natural Language :: English",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 
 readme = "README.rst"
 license = "MPL-2.0"
 
 [tool.poetry.urls]
 "Source" = "https://github.com/compose-x/cfn-kafka-admin"
 "Bug Tracker" = "https://github.com/compose-x/cfn-kafka-admin/issues"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 compose-x-common = "^1.4"
-jsonschema = "4.17.3"
+jsonschema = "^4.21"
 importlib-resources = "^6.0"
 PyYAML = "^6.0"
 troposphere = "^4.5.1"
-kafka-schema-registry-admin = "^0.2"
+kafka-schema-registry-admin = "^0.5"
 datamodel-code-generator = { extras = ["http"], version = "^0.25" }
 aws-cfn-custom-resource-resolve-parser = "^0.3"
-kafka-python = "^2.0.2"
 cfn-resource-provider = "^1.0.7"
 retry2 = "^0.9.5"
 confluent-kafka = "^2.3"
 
 [tool.poetry.scripts]
 aws-cfn-kafka-admin-provider = "cfn_kafka_admin.cli:main"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.7"
+black = ">=23.7,<25.0"
 isort = "^5.10"
 coverage = "^5.5"
 pytest = "^7.4"
 pre-commit = "^2.19.0"
 tbump = "^6.8.0"
 cleanpy = "^0.3.1"
 Sphinx = "^4.5.0"
 sphinx-material = "^0.0.35"
 sphinx-jsonschema = "^1.19.1"
 pyupgrade = "^3.3.1"
-testcontainers = "^3.7.1"
+testcontainers = "^4.0"
 
 [tool.datamodel-codegen]
 input = "cfn_kafka_admin/specs/aws-cfn-kafka-admin-provider-schema.json"
 input-file-type = "jsonschema"
 output = "cfn_kafka_admin/models/admin.py"
+#output-model-type = "dataclasses.dataclass"
 reuse-model = "true"
-target-python-version = "3.9"
+target-python-version = "3.10"
+use-schema-description = "true"
+use-field-description = "true"
+use-double-quotes = "true"
+disable-timestamp = "true"
+
 
 [tool.tbump]
 github_url = "https://github.com/compose-x/cfn-kafka-admin"
 
 [tool.tbump.version]
-current = "0.6.0-rc2"
+current = "0.6.0-rc3"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
```

### Comparing `cfn_kafka_admin-0.6.0rc2/PKG-INFO` & `cfn_kafka_admin-0.6.0rc3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 Metadata-Version: 2.1
 Name: cfn_kafka_admin
-Version: 0.6.0rc2
+Version: 0.6.0rc3
 Summary: AWS CloudFormation Resources to manage Kafka
 License: MPL-2.0
 Author: John Mille
 Author-email: john@compose-x.io
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: aws-cfn-custom-resource-resolve-parser (>=0.3,<0.4)
 Requires-Dist: cfn-resource-provider (>=1.0.7,<2.0.0)
 Requires-Dist: compose-x-common (>=1.4,<2.0)
 Requires-Dist: confluent-kafka (>=2.3,<3.0)
 Requires-Dist: datamodel-code-generator[http] (>=0.25,<0.26)
 Requires-Dist: importlib-resources (>=6.0,<7.0)
-Requires-Dist: jsonschema (==4.17.3)
-Requires-Dist: kafka-python (>=2.0.2,<3.0.0)
-Requires-Dist: kafka-schema-registry-admin (>=0.2,<0.3)
+Requires-Dist: jsonschema (>=4.21,<5.0)
+Requires-Dist: kafka-schema-registry-admin (>=0.5,<0.6)
 Requires-Dist: retry2 (>=0.9.5,<0.10.0)
 Requires-Dist: troposphere (>=4.5.1,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/compose-x/cfn-kafka-admin/issues
 Project-URL: Source, https://github.com/compose-x/cfn-kafka-admin
 Description-Content-Type: text/x-rst
 
 ===============
```

