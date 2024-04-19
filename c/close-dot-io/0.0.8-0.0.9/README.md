# Comparing `tmp/close_dot_io-0.0.8.tar.gz` & `tmp/close_dot_io-0.0.9.tar.gz`

## Comparing `close_dot_io-0.0.8.tar` & `close_dot_io-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/requirements-dev.txt
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/src/close_dot_io/__about__.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/src/close_dot_io/__init__.py
--rw-r--r--   0        0        0    11989 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/src/close_dot_io/client.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/src/close_dot_io/dict_util.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/src/close_dot_io/enums.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/src/close_dot_io/resources/__init__.py
--rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/src/close_dot_io/resources/activity.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/src/close_dot_io/resources/base.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/src/close_dot_io/resources/connected_account.py
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/src/close_dot_io/resources/contact.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/src/close_dot_io/resources/lead.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/src/close_dot_io/resources/sequence.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/src/close_dot_io/resources/smart_view.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/LICENSE.txt
--rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/README.md
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     8476 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 close_dot_io-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 close_dot_io-0.0.9/requirements-dev.txt
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 close_dot_io-0.0.9/src/close_dot_io/__about__.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 close_dot_io-0.0.9/src/close_dot_io/__init__.py
+-rw-r--r--   0        0        0    13491 2020-02-02 00:00:00.000000 close_dot_io-0.0.9/src/close_dot_io/client.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 close_dot_io-0.0.9/src/close_dot_io/dict_util.py
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 close_dot_io-0.0.9/src/close_dot_io/enums.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 close_dot_io-0.0.9/src/close_dot_io/resources/__init__.py
+-rw-r--r--   0        0        0     4507 2020-02-02 00:00:00.000000 close_dot_io-0.0.9/src/close_dot_io/resources/activity.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 close_dot_io-0.0.9/src/close_dot_io/resources/base.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 close_dot_io-0.0.9/src/close_dot_io/resources/connected_account.py
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 close_dot_io-0.0.9/src/close_dot_io/resources/contact.py
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 close_dot_io-0.0.9/src/close_dot_io/resources/lead.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 close_dot_io-0.0.9/src/close_dot_io/resources/opportunity.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 close_dot_io-0.0.9/src/close_dot_io/resources/sequence.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 close_dot_io-0.0.9/src/close_dot_io/resources/smart_view.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 close_dot_io-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 close_dot_io-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 close_dot_io-0.0.9/LICENSE.txt
+-rw-r--r--   0        0        0    10404 2020-02-02 00:00:00.000000 close_dot_io-0.0.9/README.md
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 close_dot_io-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    11483 2020-02-02 00:00:00.000000 close_dot_io-0.0.9/PKG-INFO
```

### Comparing `close_dot_io-0.0.8/.pre-commit-config.yaml` & `close_dot_io-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.8/src/close_dot_io/client.py` & `close_dot_io-0.0.9/src/close_dot_io/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import time
 from typing import Type, TypeVar
 from urllib.parse import urlencode
 
 import requests
 from pydantic import ValidationError, create_model
 
-from .resources import BaseResourceModel, Contact, Lead, SmartView
+from .resources import BaseResourceModel, Contact, Lead, Opportunity, SmartView
 from .resources.activity import BaseActivity
 
 MAX_RETRY = 5
 
 CAMEL_CASE_PATTERN = re.compile(r"(?<!^)(?=[A-Z])")
 
 
@@ -26,14 +26,15 @@
         self.base_url = "https://api.close.com/api/v1/"
         if not api_key:
             raise ValueError("No API key provided!")
         self.api_key = api_key
         self.model_depth = model_depth
 
         self.lead_statuses: dict = {}
+        self.opportunity_statuses: dict = {}
 
     @staticmethod
     def get_model_fields_for_query(
         lead_resource: Type[R] = None, contact_resource: Type[R] = None
     ) -> dict:
         q = {"_fields": {}}
         if lead_resource:
@@ -54,19 +55,33 @@
             if "error" in response.json():
                 return int(float(response.json()["error"]["rate_reset"]))
         except (AttributeError, KeyError, ValueError, Exception):
             return 60
 
     def get_resource_or_none(self, resource: Type[R], data: dict) -> R | None:
         try:
-            return resource(**data | {"lead_statuses": self.lead_statuses})
+            return resource(
+                **data
+                | {
+                    "lead_statuses": self.lead_statuses,
+                    "opportunity_statuses": self.opportunity_statuses,
+                }
+            )
         except ValidationError:
             # todo log?
             return None
 
+    def set_opportunity_statuses(self):
+        if self.opportunity_statuses:
+            return
+        res = self.dispatch(endpoint="/status/opportunity/").get("data")
+        self.opportunity_statuses = {
+            status.get("label"): status.get("id") for status in res
+        }
+
     def set_lead_statuses(self):
         if self.lead_statuses:
             return
         res = self.dispatch(endpoint="/status/lead/").get("data")
         self.lead_statuses = {status.get("label"): status.get("id") for status in res}
 
     def get_base_model(self, model: Type[R] | R):
@@ -77,14 +92,16 @@
 
         This allows for deep inheritance of Lead/Contact/Oppertunity models.
         :param model:
         :param max_depth:
         :return:
         """
         # fetch the status IDs once.
+        if not self.opportunity_statuses:
+            self.set_opportunity_statuses()
         if not self.lead_statuses:
             self.set_lead_statuses()
         class_found = False
         recur_count = 0
         while not class_found:
             try:
                 last_class = model.__bases__
@@ -297,14 +314,30 @@
             )
             swapped_to_lead = True
             resource = dynamic_lead_model.create_from_contact(contact=resource)
         endpoint = self.resource_to_endpoint(resource=resource, resource_id=resource.id)
         method = "PUT" if resource.id else "POST"
         if base_resource == Lead:
             resource.lead_statuses = self.lead_statuses
+            # if Lead we also need to save the opps if they have changed or are new.
+            # Any ids remaining in the list should be deleted since they are no longer on the lead.
+            current_opps = resource._opp_ids_on_init
+            for opp in resource.opportunities:
+                if opp.id and opp.id in current_opps:
+                    current_opps.remove(opp.id)
+                # if no ID we can save since we know its new.
+                # if initial content hash is not the same model has changed so we can save as well.
+                if not opp.id or opp.resource_hash != opp._initial_hash:
+                    self.save(resource=opp)
+
+            for opp_to_delete in current_opps:
+                self.dispatch(endpoint=f"/opportunity/{opp_to_delete}", method="DELETE")
+
+        if base_resource == Opportunity:
+            resource.opportunity_statuses = self.opportunity_statuses
         data = resource.to_close_object()
         if lead_id:
             data["lead_id"] = lead_id
         res = self.dispatch(endpoint=endpoint, method=method, json_data=data)
         resource = resource.__class__(**res)
         # If target resource was a contact, grab it instead of lead.
         if base_resource == Contact and swapped_to_lead:
```

### Comparing `close_dot_io-0.0.8/src/close_dot_io/resources/base.py` & `close_dot_io-0.0.9/src/close_dot_io/resources/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,34 @@
+import hashlib
 from datetime import datetime
 
 from pydantic import BaseModel, ConfigDict
 
+EXPORT_CONFIG = {
+    "exclude_none": True,
+    "by_alias": True,
+    # Exclude status label since we always set the preferred ID.
+    "exclude": {"date_updated", "date_created", "status_label"},
+}
+
 
 class BaseResourceModel(BaseModel):
     id: str | None = None
     organization_id: str | None = None
     date_updated: datetime | None = None
     date_created: datetime | None = None
 
     model_config = ConfigDict(populate_by_name=True)
 
+    @property
+    def resource_hash(self):
+        return (
+            hashlib.md5(self.model_dump_json(**EXPORT_CONFIG).encode("utf-8"))
+            .digest()
+            .hex()
+        )
+
     def to_close_object(self, fields_to_exclude: set = None):
-        # Exclude status label since we always set the preferred ID.
-        default_exclude = {"date_updated", "date_created", "status_label"}
+        config = EXPORT_CONFIG
         if fields_to_exclude:
-            default_exclude.update(fields_to_exclude)
-        return self.model_dump(
-            mode="json", by_alias=True, exclude_none=True, exclude=default_exclude
-        )
+            config["exclude"].update(fields_to_exclude)
+        return self.model_dump(mode="json", **config)
```

### Comparing `close_dot_io-0.0.8/src/close_dot_io/resources/contact.py` & `close_dot_io-0.0.9/src/close_dot_io/resources/contact.py`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.8/src/close_dot_io/resources/lead.py` & `close_dot_io-0.0.9/src/close_dot_io/resources/lead.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,42 @@
-from typing import TypeVar
+from typing import Any, TypeVar
 
 from pydantic import AnyUrl, Field, computed_field
 
 from .base import BaseResourceModel
 from .contact import Contact
+from .opportunity import Opportunity
 
 T = TypeVar("T", bound=Contact)
+Opp = TypeVar("Opp", bound=Opportunity)
 
 
 class Lead(BaseResourceModel):
     name: str | None = None
     status_label: str | None = None
+
     contacts: list[T] = []
+    opportunities: list[Opp] = []
+
     description: str | None = None
     html_url: AnyUrl | None = None
 
     lead_statuses: dict = Field(exclude=True, default={}, repr=False)
+    _opp_ids_on_init: set[str] | None = None
 
     @classmethod
     def create_from_contact(cls, contact: T, **other_lead_data):
         other_lead_data.pop("contacts", None)
         return cls(contacts=[contact], **other_lead_data)
 
+    def model_post_init(self, __context: Any) -> None:
+        if not self.opportunities:
+            return
+        self._opp_ids_on_init = {opp.id for opp in self.opportunities if opp.id}
+
     @computed_field
     @property
     def display_name(self) -> str | None:
         return self.name
 
     @computed_field
     @property
```

### Comparing `close_dot_io-0.0.8/src/close_dot_io/resources/smart_view.py` & `close_dot_io-0.0.9/src/close_dot_io/resources/smart_view.py`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.8/LICENSE.txt` & `close_dot_io-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.8/README.md` & `close_dot_io-0.0.9/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -22,29 +22,33 @@
 
 pip install close-dot-io
 
 ```
 
 ## Basic Usage
 
+All methods will ask for which resource you are looking to interact with.
+
+The `Lead` and `Contact` resource can be subclassed to add your own custom fields and logic.
+
+Further down is an example of how to do that.
+
 #### Getting a list of a resource
 
 ```python
 from close_dot_io import CloseClient, Lead
 
 CLOSE_API_KEY = "MY-KEY-HERE"
 
 # Create a connection to Close.
-client = CloseClient(
-    api_key=CLOSE_API_KEY
-)
+client = CloseClient(api_key=CLOSE_API_KEY)
 
 # Get 200 leads.
 # You get a list of 'Lead' object with the expected Python data types.
-leads:list[Lead] = client.list(resource=Lead, max_results=200)
+leads = client.list(resource=Lead, max_results=200)
 
 print(leads)
 # > [
 #   Lead(
 #       id='lead_xxx',
 #       status_label='Cold',
 #       description='A sales automation ...',
@@ -56,14 +60,15 @@
 #       contacts=[
 #           Contact(id='cont_xxx',
 #           organization_id='orga_xxx',
 #           date_updated=datetime.datetime(2024, 4, 10, 19, 1, 30, 512000, tzinfo=TzInfo(UTC)),
 #           date_created=datetime.datetime(2024, 2, 29, 11, 3, 12, 557000, tzinfo=TzInfo(UTC)),
 #           name='Eric Morris',
 #           title='co-founder',
+#           opportunities=[],
 #           phones=[
 #               ContactPhoneNumber(
 #                   country='CA',
 #                   phone='+16xxx',
 #                   type=<ContactEmailOrPhoneTypeEnum.OFFICE: 'office'>
 #               )
 #           ],
@@ -75,14 +80,15 @@
 #              )
 #          ]
 #      )
 #  ])] ...
 
 
 # Get the first leads ID.
+# All `Lead` fields will autocomplete in your IDE.
 first_lead = leads[0].id
 
 # Iterate over leads and contacts
 for lead in leads:
     for contact in lead.contacts:
         ...
 
@@ -90,59 +96,56 @@
 
 Currently supported resources are:
 
 ```python
 from close_dot_io import (
     Lead,
     Contact,
+    Opportunity,
     ConnectedAccount,
     Sequence,
     CallActivity,
     CreatedActivity,
     EmailActivity,
     EmailThreadActivity,
     LeadStatusChangeActivity,
     MeetingActivity,
     NoteActivity,
     OpportunityStatusChangeActivity,
     SMSActivity,
     TaskCompletedActivity,
-    SmartView
+    SmartView,
 )
 ```
 #### Getting a list of leads based on a smartview.
 
 ```python
-from close_dot_io import CloseClient
+from close_dot_io import CloseClient,Lead
 
 CLOSE_API_KEY = "MY-KEY-HERE"
 
 # Create a connection to Close.
-client = CloseClient(
-    api_key=CLOSE_API_KEY
-)
+client = CloseClient(api_key=CLOSE_API_KEY)
 # By id
-leads = client.get_from_smartview(smartview_id="save_xxx", max_results=10)
+leads = client.get_from_smartview(resource=Lead, smartview_id="save_xxx", max_results=10)
 
 # Or search by name (slower since we need to fetch the smartviews to grab the ID)
-leads = client.get_from_smartview(smartview_name="People to follow up with", max_results=10)
+leads = client.get_from_smartview(resource=Lead, smartview_name="People to follow up with", max_results=1000)
 
 ```
 
 #### Creating/Updating/Cloning a new contact/lead
 
 ```python
 from close_dot_io import CloseClient, Contact, Lead
 
 CLOSE_API_KEY = "MY-KEY-HERE"
 
 # Create a connection to Close.
-client = CloseClient(
-    api_key=CLOSE_API_KEY
-)
+client = CloseClient(api_key=CLOSE_API_KEY)
 
 # Create using only an Email.
 new_contact = Contact.create_from_email(email="j@acme.com", title='CEO')
 
 # Assign contact to lead.
 new_lead = Lead.create_from_contact(new_contact, name="Acme Corp")
 
@@ -175,27 +178,30 @@
 
 You likely have some custom fields that you want to use for your Contacts and Leads.
 
 Here is how to do that.
 
 Under the hood [Pydantic](https://docs.pydantic.dev/) is used to validate models and type annotations.
 
+
 ```python
 from close_dot_io import Contact, Lead, CloseClient
 from pydantic import Field
 from enum import Enum
 
 # Subclass the base Contact object
 class MyCustomContact(Contact):
-    # The name can be anything you want.
+    # The field name can be anything you want.
     # The only required steps are to (1) set the 'alias' parameter with the custom field ID.
     # and (2) set a type annotation to the field.
     # You can copy the ID in the Close custom field settings.
     # **Important** you must prefix the custom field ID with 'custom.{my-id}'
     # Its recommended to set the default to None since your field is likely optional.
+    # If you don't set a default and ask for a Contact that doesn't have that field the model will not be created
+    # since it would be deemed invalid.
     some_custom_field: str | None = Field(
         alias="custom.cf_xxx",
         default=None,
         description="My awesome custom field.",
     )
 
     # Number fields are also fine. Set a default if its applicable.
@@ -226,14 +232,17 @@
         default=CustomerServiceRep.ALICE,
         description="The ID of the CS rep asigned to this contact.",
     )
 
 # Same exact logic applies to a Lead.
 class CustomLead(Lead):
     lead_score: int | None = Field(alias="custom.cf_xxx", default=None)
+    # Set the type of contacts you want
+    # to have a full Lead representation.
+    contacts: list[PostCustomerContactModel] = []
 
 # Now you just create these as you would any other object.
 new_contact = PostCustomerContactModel.create_from_email(
     email="j@customer.com",
     title='CEO',
     customer_rep=CustomerServiceRep.CAM
 )
@@ -242,27 +251,123 @@
     status_label='Customer',
     name="Acme Corp",
     lead_score=1
 )
 
 CLOSE_API_KEY = "MY-KEY-HERE"
 
-# To save you need to bind your custom Contact and Lead models to the client.
-# Now whenever you ask for Leads or Contacts
-# you will get the bound object returned with all the custom fields automatically transposed.
-client = CloseClient(
-    api_key=CLOSE_API_KEY,
-    contact_model=PostCustomerContactModel,
-    lead_model=CustomLead
-)
+client = CloseClient(api_key=CLOSE_API_KEY)
 
+# Save the new lead with our custom fields
 client.save(new_lead)
 
+# Fetch Leads from a smartview using the custom Resource.
+leads = client.get_from_smartview(
+    resource=CustomLead,
+    smartview_name="People to follow up with",
+    max_results=10
+)
+# We now have lead score!
+print(leads[0].lead_score)
+
+
+```
+
+#### Working with Opportunities
+
+Opportunities behave like any other resource and also has support for custom fields.
+
+```python
+from close_dot_io import Opportunity
+from pydantic import Field
+
+
+class CustomOpportunity(Opportunity):
+    my_custom_opp_field:str | None = Field(default=None, alias="custom.cf_xxx")
+
+```
+
+Extending the custom lead example from earlier we can set our CustomOpportunity class
+so that whenever we fetch or interact with the Close API this is the model we are working with.
+
+```python
+from close_dot_io import Opportunity, Lead, CloseClient
+from pydantic import Field
+
+class CustomLead(Lead):
+    lead_score: int | None = Field(alias="custom.cf_xxx", default=None)
+    # Set the type of opportunities you want
+    # to have a full Lead representation.
+    opportunities: list[CustomOpportunity] = []
+
+```
+Just like contacts, opportunities are automatically saved when updating a Lead in the Close API.
+
+Adding and updating a new opportunity to a lead.
+```python
+CLOSE_API_KEY = "MY-KEY-HERE"
+
+client = CloseClient(api_key=CLOSE_API_KEY)
+
+# First get an instance of a Lead
+lead = client.get(resource=CustomLead, resource_id="lead_xxx")
+
+# Update the note of the first opportunity
+lead.opportunities[0].note = "Updated note from the API"
+
+# Now create your opportunity
+my_opp_data = {
+    "note": "i hope this deal closes...",
+    "confidence": 90,
+    "lead_id": lead.id,
+    "value_period": "monthly",
+    "status": "Active",
+    "value": 500,
+    "my_custom_opp_field": "My custom value"
+}
+new_opp = CustomOpportunity(**my_opp_data)
+
+# Add the opportunity to the lead
+lead.opportunities.append(new_opp)
+
+# Save it
+client.save(lead)
 ```
 
+Deleting all opportunities on a lead.
+```python
+CLOSE_API_KEY = "MY-KEY-HERE"
+
+client = CloseClient(api_key=CLOSE_API_KEY)
+
+# First get an instance of a Lead
+lead = client.get(resource=CustomLead, resource_id="lead_xxx")
+
+# Set the opportunities to an empty list.
+lead.opportunities = []
+
+# Save it
+client.save(lead)
+```
+
+Deleting all opportunities on a lead that are closed-lost
+```python
+CLOSE_API_KEY = "MY-KEY-HERE"
+
+client = CloseClient(api_key=CLOSE_API_KEY)
+
+# First get an instance of a Lead
+lead = client.get(resource=CustomLead, resource_id="lead_xxx")
+
+# Set the opportunities to only ones that are not closed lost.
+lead.opportunities = [opp for opp in lead.opportunities if not opp.is_lost]
+
+# Save it
+client.save(lead)
+```
 
 > Huge thank you to the Close team for creating a best-in-class product and API!
 
 Close API documentation: https://developer.close.com/
 
 
 ## License
```

### Comparing `close_dot_io-0.0.8/pyproject.toml` & `close_dot_io-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.8/PKG-INFO` & `close_dot_io-0.0.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: close-dot-io
-Version: 0.0.8
+Version: 0.0.9
 Summary: Easy interface to work with the Close.io API.
 Project-URL: Documentation, https://github.com/unknown/close_dot_io#readme
 Project-URL: Issues, https://github.com/unknown/close_dot_io/issues
 Project-URL: Source, https://github.com/unknown/close_dot_io
 Author-email: Copyfactory <dev@copyfactory.io>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -48,29 +48,33 @@
 
 pip install close-dot-io
 
 ```
 
 ## Basic Usage
 
+All methods will ask for which resource you are looking to interact with.
+
+The `Lead` and `Contact` resource can be subclassed to add your own custom fields and logic.
+
+Further down is an example of how to do that.
+
 #### Getting a list of a resource
 
 ```python
 from close_dot_io import CloseClient, Lead
 
 CLOSE_API_KEY = "MY-KEY-HERE"
 
 # Create a connection to Close.
-client = CloseClient(
-    api_key=CLOSE_API_KEY
-)
+client = CloseClient(api_key=CLOSE_API_KEY)
 
 # Get 200 leads.
 # You get a list of 'Lead' object with the expected Python data types.
-leads:list[Lead] = client.list(resource=Lead, max_results=200)
+leads = client.list(resource=Lead, max_results=200)
 
 print(leads)
 # > [
 #   Lead(
 #       id='lead_xxx',
 #       status_label='Cold',
 #       description='A sales automation ...',
@@ -82,14 +86,15 @@
 #       contacts=[
 #           Contact(id='cont_xxx',
 #           organization_id='orga_xxx',
 #           date_updated=datetime.datetime(2024, 4, 10, 19, 1, 30, 512000, tzinfo=TzInfo(UTC)),
 #           date_created=datetime.datetime(2024, 2, 29, 11, 3, 12, 557000, tzinfo=TzInfo(UTC)),
 #           name='Eric Morris',
 #           title='co-founder',
+#           opportunities=[],
 #           phones=[
 #               ContactPhoneNumber(
 #                   country='CA',
 #                   phone='+16xxx',
 #                   type=<ContactEmailOrPhoneTypeEnum.OFFICE: 'office'>
 #               )
 #           ],
@@ -101,14 +106,15 @@
 #              )
 #          ]
 #      )
 #  ])] ...
 
 
 # Get the first leads ID.
+# All `Lead` fields will autocomplete in your IDE.
 first_lead = leads[0].id
 
 # Iterate over leads and contacts
 for lead in leads:
     for contact in lead.contacts:
         ...
 
@@ -116,59 +122,56 @@
 
 Currently supported resources are:
 
 ```python
 from close_dot_io import (
     Lead,
     Contact,
+    Opportunity,
     ConnectedAccount,
     Sequence,
     CallActivity,
     CreatedActivity,
     EmailActivity,
     EmailThreadActivity,
     LeadStatusChangeActivity,
     MeetingActivity,
     NoteActivity,
     OpportunityStatusChangeActivity,
     SMSActivity,
     TaskCompletedActivity,
-    SmartView
+    SmartView,
 )
 ```
 #### Getting a list of leads based on a smartview.
 
 ```python
-from close_dot_io import CloseClient
+from close_dot_io import CloseClient,Lead
 
 CLOSE_API_KEY = "MY-KEY-HERE"
 
 # Create a connection to Close.
-client = CloseClient(
-    api_key=CLOSE_API_KEY
-)
+client = CloseClient(api_key=CLOSE_API_KEY)
 # By id
-leads = client.get_from_smartview(smartview_id="save_xxx", max_results=10)
+leads = client.get_from_smartview(resource=Lead, smartview_id="save_xxx", max_results=10)
 
 # Or search by name (slower since we need to fetch the smartviews to grab the ID)
-leads = client.get_from_smartview(smartview_name="People to follow up with", max_results=10)
+leads = client.get_from_smartview(resource=Lead, smartview_name="People to follow up with", max_results=1000)
 
 ```
 
 #### Creating/Updating/Cloning a new contact/lead
 
 ```python
 from close_dot_io import CloseClient, Contact, Lead
 
 CLOSE_API_KEY = "MY-KEY-HERE"
 
 # Create a connection to Close.
-client = CloseClient(
-    api_key=CLOSE_API_KEY
-)
+client = CloseClient(api_key=CLOSE_API_KEY)
 
 # Create using only an Email.
 new_contact = Contact.create_from_email(email="j@acme.com", title='CEO')
 
 # Assign contact to lead.
 new_lead = Lead.create_from_contact(new_contact, name="Acme Corp")
 
@@ -201,27 +204,30 @@
 
 You likely have some custom fields that you want to use for your Contacts and Leads.
 
 Here is how to do that.
 
 Under the hood [Pydantic](https://docs.pydantic.dev/) is used to validate models and type annotations.
 
+
 ```python
 from close_dot_io import Contact, Lead, CloseClient
 from pydantic import Field
 from enum import Enum
 
 # Subclass the base Contact object
 class MyCustomContact(Contact):
-    # The name can be anything you want.
+    # The field name can be anything you want.
     # The only required steps are to (1) set the 'alias' parameter with the custom field ID.
     # and (2) set a type annotation to the field.
     # You can copy the ID in the Close custom field settings.
     # **Important** you must prefix the custom field ID with 'custom.{my-id}'
     # Its recommended to set the default to None since your field is likely optional.
+    # If you don't set a default and ask for a Contact that doesn't have that field the model will not be created
+    # since it would be deemed invalid.
     some_custom_field: str | None = Field(
         alias="custom.cf_xxx",
         default=None,
         description="My awesome custom field.",
     )
 
     # Number fields are also fine. Set a default if its applicable.
@@ -252,14 +258,17 @@
         default=CustomerServiceRep.ALICE,
         description="The ID of the CS rep asigned to this contact.",
     )
 
 # Same exact logic applies to a Lead.
 class CustomLead(Lead):
     lead_score: int | None = Field(alias="custom.cf_xxx", default=None)
+    # Set the type of contacts you want
+    # to have a full Lead representation.
+    contacts: list[PostCustomerContactModel] = []
 
 # Now you just create these as you would any other object.
 new_contact = PostCustomerContactModel.create_from_email(
     email="j@customer.com",
     title='CEO',
     customer_rep=CustomerServiceRep.CAM
 )
@@ -268,27 +277,123 @@
     status_label='Customer',
     name="Acme Corp",
     lead_score=1
 )
 
 CLOSE_API_KEY = "MY-KEY-HERE"
 
-# To save you need to bind your custom Contact and Lead models to the client.
-# Now whenever you ask for Leads or Contacts
-# you will get the bound object returned with all the custom fields automatically transposed.
-client = CloseClient(
-    api_key=CLOSE_API_KEY,
-    contact_model=PostCustomerContactModel,
-    lead_model=CustomLead
-)
+client = CloseClient(api_key=CLOSE_API_KEY)
 
+# Save the new lead with our custom fields
 client.save(new_lead)
 
+# Fetch Leads from a smartview using the custom Resource.
+leads = client.get_from_smartview(
+    resource=CustomLead,
+    smartview_name="People to follow up with",
+    max_results=10
+)
+# We now have lead score!
+print(leads[0].lead_score)
+
+
+```
+
+#### Working with Opportunities
+
+Opportunities behave like any other resource and also has support for custom fields.
+
+```python
+from close_dot_io import Opportunity
+from pydantic import Field
+
+
+class CustomOpportunity(Opportunity):
+    my_custom_opp_field:str | None = Field(default=None, alias="custom.cf_xxx")
+
+```
+
+Extending the custom lead example from earlier we can set our CustomOpportunity class
+so that whenever we fetch or interact with the Close API this is the model we are working with.
+
+```python
+from close_dot_io import Opportunity, Lead, CloseClient
+from pydantic import Field
+
+class CustomLead(Lead):
+    lead_score: int | None = Field(alias="custom.cf_xxx", default=None)
+    # Set the type of opportunities you want
+    # to have a full Lead representation.
+    opportunities: list[CustomOpportunity] = []
+
+```
+Just like contacts, opportunities are automatically saved when updating a Lead in the Close API.
+
+Adding and updating a new opportunity to a lead.
+```python
+CLOSE_API_KEY = "MY-KEY-HERE"
+
+client = CloseClient(api_key=CLOSE_API_KEY)
+
+# First get an instance of a Lead
+lead = client.get(resource=CustomLead, resource_id="lead_xxx")
+
+# Update the note of the first opportunity
+lead.opportunities[0].note = "Updated note from the API"
+
+# Now create your opportunity
+my_opp_data = {
+    "note": "i hope this deal closes...",
+    "confidence": 90,
+    "lead_id": lead.id,
+    "value_period": "monthly",
+    "status": "Active",
+    "value": 500,
+    "my_custom_opp_field": "My custom value"
+}
+new_opp = CustomOpportunity(**my_opp_data)
+
+# Add the opportunity to the lead
+lead.opportunities.append(new_opp)
+
+# Save it
+client.save(lead)
 ```
 
+Deleting all opportunities on a lead.
+```python
+CLOSE_API_KEY = "MY-KEY-HERE"
+
+client = CloseClient(api_key=CLOSE_API_KEY)
+
+# First get an instance of a Lead
+lead = client.get(resource=CustomLead, resource_id="lead_xxx")
+
+# Set the opportunities to an empty list.
+lead.opportunities = []
+
+# Save it
+client.save(lead)
+```
+
+Deleting all opportunities on a lead that are closed-lost
+```python
+CLOSE_API_KEY = "MY-KEY-HERE"
+
+client = CloseClient(api_key=CLOSE_API_KEY)
+
+# First get an instance of a Lead
+lead = client.get(resource=CustomLead, resource_id="lead_xxx")
+
+# Set the opportunities to only ones that are not closed lost.
+lead.opportunities = [opp for opp in lead.opportunities if not opp.is_lost]
+
+# Save it
+client.save(lead)
+```
 
 > Huge thank you to the Close team for creating a best-in-class product and API!
 
 Close API documentation: https://developer.close.com/
 
 
 ## License
```

