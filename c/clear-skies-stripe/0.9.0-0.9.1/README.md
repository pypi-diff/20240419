# Comparing `tmp/clear_skies_stripe-0.9.0.tar.gz` & `tmp/clear_skies_stripe-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clear_skies_stripe-0.9.0.tar", max compression
+gzip compressed data, was "clear_skies_stripe-0.9.1.tar", max compression
```

## Comparing `clear_skies_stripe-0.9.0.tar` & `clear_skies_stripe-0.9.1.tar`

### file list

```diff
@@ -1,10 +1,16 @@
--rw-r--r--   0        0        0     1065 2024-04-12 11:44:22.990759 clear_skies_stripe-0.9.0/LICENSE
--rw-r--r--   0        0        0     7708 2024-04-19 07:23:00.654964 clear_skies_stripe-0.9.0/README.md
--rw-r--r--   0        0        0      728 2024-04-12 12:02:19.831188 clear_skies_stripe-0.9.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-12 12:00:56.850897 clear_skies_stripe-0.9.0/src/clearskies_stripe/__init__.py
--rw-r--r--   0        0        0      267 2024-04-19 06:51:54.068916 clear_skies_stripe-0.9.0/src/clearskies_stripe/di/__init__.py
--rw-r--r--   0        0        0     3225 2024-04-15 15:53:17.830798 clear_skies_stripe-0.9.0/src/clearskies_stripe/di/stripe.py
--rw-r--r--   0        0        0       91 2024-04-14 19:53:52.183390 clear_skies_stripe-0.9.0/src/clearskies_stripe/handlers/__init__.py
--rw-r--r--   0        0        0     3950 2024-04-19 06:57:54.561778 clear_skies_stripe-0.9.0/src/clearskies_stripe/handlers/create_setup_intent.py
--rw-r--r--   0        0        0     3545 2024-04-19 06:45:32.468903 clear_skies_stripe-0.9.0/src/clearskies_stripe/handlers/create_setup_intent_test.py
--rw-r--r--   0        0        0     8377 1970-01-01 00:00:00.000000 clear_skies_stripe-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-12 11:44:22.990759 clear_skies_stripe-0.9.1/LICENSE
+-rw-r--r--   0        0        0     8996 2024-04-19 12:02:46.816724 clear_skies_stripe-0.9.1/README.md
+-rw-r--r--   0        0        0      728 2024-04-19 18:18:57.575927 clear_skies_stripe-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0       45 2024-04-19 18:15:31.887302 clear_skies_stripe-0.9.1/src/clearskies_stripe/__init__.py
+-rw-r--r--   0        0        0       88 2024-04-19 11:45:03.248687 clear_skies_stripe-0.9.1/src/clearskies_stripe/backends/__init__.py
+-rw-r--r--   0        0        0     2848 2024-04-19 18:17:49.367726 clear_skies_stripe-0.9.1/src/clearskies_stripe/backends/stripe_sdk_backend.py
+-rw-r--r--   0        0        0      267 2024-04-19 06:51:54.068916 clear_skies_stripe-0.9.1/src/clearskies_stripe/di/__init__.py
+-rw-r--r--   0        0        0     3211 2024-04-19 18:18:07.515780 clear_skies_stripe-0.9.1/src/clearskies_stripe/di/stripe.py
+-rw-r--r--   0        0        0       91 2024-04-14 19:53:52.183390 clear_skies_stripe-0.9.1/src/clearskies_stripe/handlers/__init__.py
+-rw-r--r--   0        0        0     3950 2024-04-19 06:57:54.561778 clear_skies_stripe-0.9.1/src/clearskies_stripe/handlers/create_setup_intent.py
+-rw-r--r--   0        0        0     3545 2024-04-19 06:45:32.468903 clear_skies_stripe-0.9.1/src/clearskies_stripe/handlers/create_setup_intent_test.py
+-rw-r--r--   0        0        0       81 2024-04-19 12:12:27.528744 clear_skies_stripe-0.9.1/src/clearskies_stripe/models/__init__.py
+-rw-r--r--   0        0        0     1268 2024-04-19 18:18:47.575898 clear_skies_stripe-0.9.1/src/clearskies_stripe/models/stripe_customer.py
+-rw-r--r--   0        0        0        0 2024-04-19 12:03:26.288725 clear_skies_stripe-0.9.1/src/clearskies_stripe/models/stripe_payment.py
+-rw-r--r--   0        0        0        0 2024-04-19 12:03:29.652725 clear_skies_stripe-0.9.1/src/clearskies_stripe/models/stripe_payment_method.py
+-rw-r--r--   0        0        0     9665 1970-01-01 00:00:00.000000 clear_skies_stripe-0.9.1/PKG-INFO
```

### Comparing `clear_skies_stripe-0.9.0/LICENSE` & `clear_skies_stripe-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clear_skies_stripe-0.9.0/README.md` & `clear_skies_stripe-0.9.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -8,70 +8,109 @@
 
 ```
 pip install clear-skies-stripe
 ```
 
 # Usage
 
+## Authentication
+
 This module has a variety of actions and handlers which take care of the stripe integration.  However, before you can use any of them, you must setup the stripe module with clearskies and tell it how to authenticate to Stripe.  The module assumes that your Stripe API key is stored in your secret manager, so you just have to tell it the path to the API key in your secret manager.
 
 **IMPORTANT**: This module is designed to fetch your Stripe API key only when needed and will automatically re-fetch the key from the secrets manager in the event of an authentication failure.  As a result, you can rotate your Stripe API key at anytime: just drop the new API key in your secret manager and your running processes will automatically find it and use it without needing to restart/rebuild/relaunch the application.
 
-In the following example, we configure a clearskies application to use AWS Secrets Manager for the storage of secrets, and then we tell the Stripe integration to fetch its api key from `/path/to/stripe/api/key` in AWS Secrets Manager.
+In the following example, we configure a clearskies application to use AWS Secrets Manager for the storage of secrets, and then we tell the Stripe integration to fetch its api key from `/path/to/stripe/(api|publishable)/key` in AWS Secrets Manager.  Of course, you can use any secrets manager you want: just swap out `secrets` in the dependency injection configuration.
+
+```
+import clearskies
+import clearskies_stripe
+import clearskies_aws
+
+application = clearskies.Application(
+    SomeHandler,
+    {
+        "your": "application config",
+    },
+    bindings={
+        "stripe": clearskies_stripe.di.stripe(
+            "/path/to/stripe/api/key",
+            "/path/to/stripe/publishable/key",
+        ),
+        "secrets": clearskies_aws.secrets.SecretsManager,
+    },
+)
+```
+
+## Models
+
+To use any of the models you must import the `clearskies_stripe` module into your application (you still have to configure authentication per the above):
 
 ```
 import clearskies
 import clearskies_stripe
 import clearskies_aws
 
 application = clearskies.Application(
     SomeHandler,
     {
         "your": "application config",
     },
+    binding_modules=[
+        clearskies_stripe,
+    ],
     bindings={
         "stripe": clearskies_stripe.di.stripe(
-            "/path/to/stripe/api/key/in/secrets/manager",
-            "/path/to/stripe/publishable/key/in/secrets/manager",
+            "/path/to/stripe/api/key",
+            "/path/to/stripe/publishable/key",
         ),
         "secrets": clearskies_aws.secrets.SecretsManager,
     },
 )
 ```
 
-## SetupInents
+## Models
+
+This module comes with a limited selection of models.  The columns available in each model match those published via the Stripe API.
+
+| Model               | DI name               | Stripe Docs |
+|---------------------|-----------------------|-------------|
+| StripeCustomer      | stripe_customer       | TBD |
+| StripePayment       | stripe_payment        | TBD |
+| StripePaymentMethod | stripe_payment_method | TBD |
+
+## SetupIntent Handler
 
 This handler creates a SetupIntent and returns the details of it, as well as the publishable key.  You can specify any of the parameters for the [create call].  In addition, you can provide `parameters_callable` which can change all the parameters that will be passed to the create call, and you can also provide `output_callable` which changes the response from the handler.  By default, the handler returns the full details of the response from the create call, as well as your publishable key.
 
 ### Configuration Options
 
 Here are the list of allowed configurations for this handler (on top of the standard handler configs).  All configs are optional.  With the exception of the callables (described below), all configuration options will be passed along as-is in the call to `stripe.setup_intents.create()`.  See [the stripe docs](https://docs.stripe.com/api/setup_intents/create) for more details:
 
-| Name                           | Type |
-|--------------------------------|------|
-| `automatic_payment_methods`    | `dict` |
-| `confirm`                      | `bool` |
-| `description`                  | `str` |
-| `metadata`                     | `dict` |
-| `payment_method`               | `str` |
-| `usage`                        | `str` |
-| `attach_to_self`               | `bool` |
-| `confirmation_token`           | `str` |
+| Name                           | Type        |
+|--------------------------------|-------------|
+| `automatic_payment_methods`    | `dict`      |
+| `confirm`                      | `bool`      |
+| `description`                  | `str`       |
+| `metadata`                     | `dict`      |
+| `payment_method`               | `str`       |
+| `usage`                        | `str`       |
+| `attach_to_self`               | `bool`      |
+| `confirmation_token`           | `str`       |
 | `flow_directions`              | `list[str]` |
-| `mandate_data`                 | `dict` |
-| `on_behalf_of`                 | `str` |
-| `payment_method_configuration` | `str` |
-| `payment_method_data,`         | `dict` |
-| `payment_method_options`       | `dict` |
+| `mandate_data`                 | `dict`      |
+| `on_behalf_of`                 | `str`       |
+| `payment_method_configuration` | `str`       |
+| `payment_method_data,`         | `dict`      |
+| `payment_method_options`       | `dict`      |
 | `payment_method_types`         | `list[str]` |
-| `return_url`                   | `str` |
-| `single_use`                   | `dict` |
-| `use_stripe_sdk`               | `bool` |
-| `parameters_callable`          | `Callable` |
-| `output_callable`              | `Callable` |
+| `return_url`                   | `str`       |
+| `single_use`                   | `dict`      |
+| `use_stripe_sdk`               | `bool`      |
+| `parameters_callable`          | `Callable`  |
+| `output_callable`              | `Callable`  |
 
 ### parameters_callable
 
 The `parameters_callable` is provided with the following kwargs:
 
 | Name                 | Type                                   | Value |
 |----------------------|----------------------------------------|-------|
```

### Comparing `clear_skies_stripe-0.9.0/pyproject.toml` & `clear_skies_stripe-0.9.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 [tool.poetry]
 name = "clear-skies-stripe"
-version = "0.9.0"
+version = "0.9.1"
 description = "clearskies bindings for working with Stripe"
 authors = [
     "Conor Mancone <cmancone@gmail.com>",
 ]
 repository = "https://github.com/cmancone/clearskies-stripe"
 license = "MIT"
 readme = "./README.md"
```

### Comparing `clear_skies_stripe-0.9.0/src/clearskies_stripe/di/stripe.py` & `clear_skies_stripe-0.9.1/src/clearskies_stripe/di/stripe.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,18 +68,15 @@
             chain = getattr(chain, name, None)
             if chain is None:
                 raise ValueError("Requested non-existent function from stripe: stripe." + ".".join(self.name))
 
         try:
             response = chain(*args, **kwargs)
         except stripe.error.AuthenticationError as e:
-            # try again without the
-
-
-            cache (e.g. fetch a new api key)
+            # try again without the cache (e.g. fetch a new api key)
             if cache:
                 return self.__call__(*args, **kwargs, cache=False)
             else:
                 # otherwise re-throw.  Don't keep trying forever.
                 raise e
 
         return response
```

### Comparing `clear_skies_stripe-0.9.0/src/clearskies_stripe/handlers/create_setup_intent.py` & `clear_skies_stripe-0.9.1/src/clearskies_stripe/handlers/create_setup_intent.py`

 * *Files identical despite different names*

### Comparing `clear_skies_stripe-0.9.0/src/clearskies_stripe/handlers/create_setup_intent_test.py` & `clear_skies_stripe-0.9.1/src/clearskies_stripe/handlers/create_setup_intent_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_stripe-0.9.0/PKG-INFO` & `clear_skies_stripe-0.9.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clear-skies-stripe
-Version: 0.9.0
+Version: 0.9.1
 Summary: clearskies bindings for working with Stripe
 Home-page: https://github.com/cmancone/clearskies-stripe
 License: MIT
 Author: Conor Mancone
 Author-email: cmancone@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -26,70 +26,109 @@
 
 ```
 pip install clear-skies-stripe
 ```
 
 # Usage
 
+## Authentication
+
 This module has a variety of actions and handlers which take care of the stripe integration.  However, before you can use any of them, you must setup the stripe module with clearskies and tell it how to authenticate to Stripe.  The module assumes that your Stripe API key is stored in your secret manager, so you just have to tell it the path to the API key in your secret manager.
 
 **IMPORTANT**: This module is designed to fetch your Stripe API key only when needed and will automatically re-fetch the key from the secrets manager in the event of an authentication failure.  As a result, you can rotate your Stripe API key at anytime: just drop the new API key in your secret manager and your running processes will automatically find it and use it without needing to restart/rebuild/relaunch the application.
 
-In the following example, we configure a clearskies application to use AWS Secrets Manager for the storage of secrets, and then we tell the Stripe integration to fetch its api key from `/path/to/stripe/api/key` in AWS Secrets Manager.
+In the following example, we configure a clearskies application to use AWS Secrets Manager for the storage of secrets, and then we tell the Stripe integration to fetch its api key from `/path/to/stripe/(api|publishable)/key` in AWS Secrets Manager.  Of course, you can use any secrets manager you want: just swap out `secrets` in the dependency injection configuration.
+
+```
+import clearskies
+import clearskies_stripe
+import clearskies_aws
+
+application = clearskies.Application(
+    SomeHandler,
+    {
+        "your": "application config",
+    },
+    bindings={
+        "stripe": clearskies_stripe.di.stripe(
+            "/path/to/stripe/api/key",
+            "/path/to/stripe/publishable/key",
+        ),
+        "secrets": clearskies_aws.secrets.SecretsManager,
+    },
+)
+```
+
+## Models
+
+To use any of the models you must import the `clearskies_stripe` module into your application (you still have to configure authentication per the above):
 
 ```
 import clearskies
 import clearskies_stripe
 import clearskies_aws
 
 application = clearskies.Application(
     SomeHandler,
     {
         "your": "application config",
     },
+    binding_modules=[
+        clearskies_stripe,
+    ],
     bindings={
         "stripe": clearskies_stripe.di.stripe(
-            "/path/to/stripe/api/key/in/secrets/manager",
-            "/path/to/stripe/publishable/key/in/secrets/manager",
+            "/path/to/stripe/api/key",
+            "/path/to/stripe/publishable/key",
         ),
         "secrets": clearskies_aws.secrets.SecretsManager,
     },
 )
 ```
 
-## SetupInents
+## Models
+
+This module comes with a limited selection of models.  The columns available in each model match those published via the Stripe API.
+
+| Model               | DI name               | Stripe Docs |
+|---------------------|-----------------------|-------------|
+| StripeCustomer      | stripe_customer       | TBD |
+| StripePayment       | stripe_payment        | TBD |
+| StripePaymentMethod | stripe_payment_method | TBD |
+
+## SetupIntent Handler
 
 This handler creates a SetupIntent and returns the details of it, as well as the publishable key.  You can specify any of the parameters for the [create call].  In addition, you can provide `parameters_callable` which can change all the parameters that will be passed to the create call, and you can also provide `output_callable` which changes the response from the handler.  By default, the handler returns the full details of the response from the create call, as well as your publishable key.
 
 ### Configuration Options
 
 Here are the list of allowed configurations for this handler (on top of the standard handler configs).  All configs are optional.  With the exception of the callables (described below), all configuration options will be passed along as-is in the call to `stripe.setup_intents.create()`.  See [the stripe docs](https://docs.stripe.com/api/setup_intents/create) for more details:
 
-| Name                           | Type |
-|--------------------------------|------|
-| `automatic_payment_methods`    | `dict` |
-| `confirm`                      | `bool` |
-| `description`                  | `str` |
-| `metadata`                     | `dict` |
-| `payment_method`               | `str` |
-| `usage`                        | `str` |
-| `attach_to_self`               | `bool` |
-| `confirmation_token`           | `str` |
+| Name                           | Type        |
+|--------------------------------|-------------|
+| `automatic_payment_methods`    | `dict`      |
+| `confirm`                      | `bool`      |
+| `description`                  | `str`       |
+| `metadata`                     | `dict`      |
+| `payment_method`               | `str`       |
+| `usage`                        | `str`       |
+| `attach_to_self`               | `bool`      |
+| `confirmation_token`           | `str`       |
 | `flow_directions`              | `list[str]` |
-| `mandate_data`                 | `dict` |
-| `on_behalf_of`                 | `str` |
-| `payment_method_configuration` | `str` |
-| `payment_method_data,`         | `dict` |
-| `payment_method_options`       | `dict` |
+| `mandate_data`                 | `dict`      |
+| `on_behalf_of`                 | `str`       |
+| `payment_method_configuration` | `str`       |
+| `payment_method_data,`         | `dict`      |
+| `payment_method_options`       | `dict`      |
 | `payment_method_types`         | `list[str]` |
-| `return_url`                   | `str` |
-| `single_use`                   | `dict` |
-| `use_stripe_sdk`               | `bool` |
-| `parameters_callable`          | `Callable` |
-| `output_callable`              | `Callable` |
+| `return_url`                   | `str`       |
+| `single_use`                   | `dict`      |
+| `use_stripe_sdk`               | `bool`      |
+| `parameters_callable`          | `Callable`  |
+| `output_callable`              | `Callable`  |
 
 ### parameters_callable
 
 The `parameters_callable` is provided with the following kwargs:
 
 | Name                 | Type                                   | Value |
 |----------------------|----------------------------------------|-------|
```

