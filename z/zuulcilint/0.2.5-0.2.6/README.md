# Comparing `tmp/zuulcilint-0.2.5.tar.gz` & `tmp/zuulcilint-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zuulcilint-0.2.5.tar", max compression
+gzip compressed data, was "zuulcilint-0.2.6.tar", max compression
```

## Comparing `zuulcilint-0.2.5.tar` & `zuulcilint-0.2.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2024-02-18 21:36:40.677909 zuulcilint-0.2.5/LICENSE
--rw-r--r--   0        0        0     2211 2024-02-18 21:36:40.677909 zuulcilint-0.2.5/README.md
--rw-r--r--   0        0        0     2466 2024-02-18 21:36:40.681909 zuulcilint-0.2.5/pyproject.toml
--rw-r--r--   0        0        0       32 2024-02-18 21:36:40.681909 zuulcilint-0.2.5/zuulcilint/__init__.py
--rw-r--r--   0        0        0    11463 2024-02-18 21:36:40.681909 zuulcilint-0.2.5/zuulcilint/__main__.py
--rw-r--r--   0        0        0     3450 2024-02-18 21:36:40.681909 zuulcilint-0.2.5/zuulcilint/checker.py
--rw-r--r--   0        0        0     5802 2024-02-18 21:36:40.681909 zuulcilint-0.2.5/zuulcilint/utils.py
--rw-r--r--   0        0        0   154600 2024-02-18 21:36:40.681909 zuulcilint-0.2.5/zuulcilint/zuul-schema.json
--rw-r--r--   0        0        0     3062 1970-01-01 00:00:00.000000 zuulcilint-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-18 23:28:15.746281 zuulcilint-0.2.6/LICENSE
+-rw-r--r--   0        0        0     2211 2024-04-18 23:28:15.746281 zuulcilint-0.2.6/README.md
+-rw-r--r--   0        0        0     2476 2024-04-18 23:28:15.746281 zuulcilint-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0       32 2024-04-18 23:28:15.746281 zuulcilint-0.2.6/zuulcilint/__init__.py
+-rw-r--r--   0        0        0    11463 2024-04-18 23:28:15.746281 zuulcilint-0.2.6/zuulcilint/__main__.py
+-rw-r--r--   0        0        0     3450 2024-04-18 23:28:15.746281 zuulcilint-0.2.6/zuulcilint/checker.py
+-rw-r--r--   0        0        0     5802 2024-04-18 23:28:15.746281 zuulcilint-0.2.6/zuulcilint/utils.py
+-rw-r--r--   0        0        0   163833 2024-04-18 23:28:15.746281 zuulcilint-0.2.6/zuulcilint/zuul-schema.json
+-rw-r--r--   0        0        0     3062 1970-01-01 00:00:00.000000 zuulcilint-0.2.6/PKG-INFO
```

### Comparing `zuulcilint-0.2.5/LICENSE` & `zuulcilint-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `zuulcilint-0.2.5/README.md` & `zuulcilint-0.2.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 ## Validate with pre-commit
 
 Add the code below to your `.pre-commit-config.yaml` file:
 
 ```yaml
   - repo: https://github.com/codesquadnest/zuulcilint.git
-    rev: "0.2.5"
+    rev: "0.2.6"
     hooks:
       - id: zuulcilint
 ```
 
 
 ## Validate with VS Code
```

### Comparing `zuulcilint-0.2.5/pyproject.toml` & `zuulcilint-0.2.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zuulcilint"
-version = "0.2.5"
+version = "0.2.6"
 description = "Zuul CI linter"
 authors = ["Pedro Baptista <pedro.miguel.baptista@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["zuul", "ci", "linter"]
 repository = "https://github.com/codesquadnest/zuulcilint"
 include = ["pyproject.toml", "LICENSE", "README.md", "zuulcilint/zuul-schema.yaml"]
@@ -20,16 +20,16 @@
 jsonschema = "^4.21.0"
 six = "^1.16.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.5.0"
 pytest = ">=7.4.4,<9.0.0"
 tox = "^4.12.0"
-pytest-cov = "^4.1.0"
-ruff = ">=0.1.13,<0.3.0"
+pytest-cov = ">=4.1,<6.0"
+ruff = ">=0.1.13,<0.4.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 # Configurations for black
 [tool.black]
@@ -100,15 +100,15 @@
         poetry install -v
         poetry run pytest --cov=zuulcilint --cov-report=term-missing
 
     [testenv:lint]
     deps =
         ruff
     commands =
-        ruff zuulcilint tests
+        ruff check zuulcilint tests
 
     [testenv:pre-commit]
     skip_install = true
     deps = pre-commit
     commands = pre-commit run --all-files --show-diff-on-failure
 
 """
```

### Comparing `zuulcilint-0.2.5/zuulcilint/__main__.py` & `zuulcilint-0.2.6/zuulcilint/__main__.py`

 * *Files identical despite different names*

### Comparing `zuulcilint-0.2.5/zuulcilint/checker.py` & `zuulcilint-0.2.6/zuulcilint/checker.py`

 * *Files identical despite different names*

### Comparing `zuulcilint-0.2.5/zuulcilint/utils.py` & `zuulcilint-0.2.6/zuulcilint/utils.py`

 * *Files identical despite different names*

### Comparing `zuulcilint-0.2.5/zuulcilint/zuul-schema.json` & `zuulcilint-0.2.6/zuulcilint/zuul-schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8726892672686107%*

 * *Differences: {"'definitions'": "{'anonymous-job': {'properties': {'allowed-projects': {'type': ['string', "*

 * *                  "'array']}, 'ansible-version': {'default': '8', 'enum': ['8', '9', 8, 9], "*

 * *                  "delete: ['type']}, 'branches': {'anyOf': [OrderedDict([('$ref', "*

 * *                  "'#/definitions/regular-expression'), ('description', 'A regular expression (or "*

 * *                  'list of regular expressions) which describe on what branches a job should run '*

 * *                  '(or in the case of v […]*

```diff
@@ -50,54 +50,64 @@
                     "examples": [
                         "https://zuul-ci.org/docs/zuul/latest/config/job.html#attr-job.allowed-projects"
                     ],
                     "items": {
                         "type": "string"
                     },
                     "title": "job.allowed-projects",
-                    "type": "array"
+                    "type": [
+                        "string",
+                        "array"
+                    ]
                 },
                 "ansible-split-streams": {
                     "default": false,
                     "description": "Keep stdout/stderr of command and shell tasks separate (the Ansible default behavior) instead of merging stdout and stderr.\nSince version 3, Zuul has combined the stdout and stderr streams in Ansible command tasks, but will soon switch to using the normal Ansible behavior. In an upcoming release of Zuul, this default will change to True, and in a later release, this option will be removed altogether.\nThis option may be used in the interim to verify playbook compatibility and facilitate upgrading to the new behavior.",
                     "title": "job.ansible-split-streams",
                     "type": "boolean"
                 },
                 "ansible-version": {
-                    "default": 6,
+                    "default": "8",
                     "description": "The ansible version to use for all playbooks of the job.",
+                    "enum": [
+                        "8",
+                        "9",
+                        8,
+                        9
+                    ],
                     "examples": [
                         "https://zuul-ci.org/docs/zuul/latest/config/job.html#attr-job.ansible-version"
                     ],
-                    "title": "job.ansible-version",
-                    "type": [
-                        "string",
-                        "number"
-                    ]
+                    "title": "job.ansible-version"
                 },
                 "attempts": {
                     "default": 3,
                     "description": "When Zuul encounters an error running a job's pre-run playbook, Zuul will stop and restart the job. Errors during the main or post-run -playbook phase of a job are not affected by this parameter (they are reported immediately). This parameter controls the number of attempts to make before an error is reported.",
                     "minimum": 0,
                     "title": "job.attempts",
                     "type": "integer"
                 },
                 "branches": {
+                    "anyOf": [
+                        {
+                            "$ref": "#/definitions/regular-expression",
+                            "description": "A regular expression (or list of regular expressions) which describe on what branches a job should run (or in the case of variants, to alter the behavior of a job for a certain branch).\nThis attribute is not inherited in the usual manner. Instead, it is used to determine whether each variant on which it appears will be used when running the job."
+                        },
+                        {
+                            "items": {
+                                "$ref": "#/definitions/regular-expression"
+                            },
+                            "type": "array"
+                        }
+                    ],
                     "description": "A regular expression (or list of regular expressions) which describe on what branches a job should run (or in the case of variants, to alter the behavior of a job for a certain branch).\nThis attribute is not inherited in the usual manner. Instead, it is used to determine whether each variant on which it appears will be used when running the job.",
                     "examples": [
                         "https://zuul-ci.org/docs/zuul/latest/config/job.html#attr-job.branches"
                     ],
-                    "items": {
-                        "type": "string"
-                    },
-                    "title": "job.branches",
-                    "type": [
-                        "string",
-                        "array"
-                    ]
+                    "title": "job.branches"
                 },
                 "cleanup-run": {
                     "allOf": [
                         {
                             "description": "The name of a playbook or list of playbooks to run after job execution. Values are either a string describing the full path to the playbook in the repo where the job is defined, or a dictionary.\nThe cleanup phase is performed regardless of the job's result, even when the job is canceled. Cleanup results are not taken into account when reporting the job result.\nWhen a job inherits from a parent, the child's cleanup-run playbooks are run before the parent's.",
                             "title": "job.cleanup-run"
                         },
@@ -167,33 +177,37 @@
                 "failure-message": {
                     "default": "FAILURE",
                     "description": "Normally when a job fails, the string FAILURE is reported as the result for the job. If set, this option may be used to supply a different string.",
                     "title": "job.failure-message",
                     "type": "string"
                 },
                 "failure-output": {
-                    "description": "A regular expression (or list of regular expressions) that should be matched against job output to determine if the job is going to fail. Matches are performed line-by-line (multiline regular expressions will not be effective).\nThis option is not required; job failure is determined by the result code from its Ansible playbooks. However, if this option is supplied, and one of the regular expressions matches a line in the streaming output from the job, Zuul will be able to anticipate the failure before the completion of the playbook. In this case, it will be able to restart jobs for changes behind it in a dependent pipeline.\nWhen inheriting or applying variants this option is combined so that regular expressions from all parents and variants used will be applied.\nUse caution when specifying this option. If an early failure is triggered, the job result will be recorded as FAILURE even if the job playbooks ultimately succeed.",
+                    "description": "A regular expression string (or list of regular expression strings) that should be matched against job output to determine if the job is going to fail. Matches are performed line-by-line (multiline regular expressions will not be effective).\nThis option is not required; job failure is determined by the result code from its Ansible playbooks. However, if this option is supplied, and one of the regular expressions matches a line in the streaming output from the job, Zuul will be able to anticipate the failure before the completion of the playbook. In this case, it will be able to restart jobs for changes behind it in a dependent pipeline.\nWhen inheriting or applying variants this option is combined so that regular expressions from all parents and variants used will be applied.\nUse caution when specifying this option. If an early failure is triggered, the job result will be recorded as FAILURE even if the job playbooks ultimately succeed.",
+                    "format": "regex",
                     "items": {
+                        "format": "regex",
                         "type": "string"
                     },
                     "title": "job.failure-output",
                     "type": [
-                        "string",
-                        "array"
+                        "array",
+                        "string"
                     ]
                 },
                 "failure-url": {
                     "deprecated": true,
                     "description": "When a job fails, this URL is reported along with the result. Otherwise behaves the same as success-url.",
                     "title": "job.failure-url",
                     "type": "string"
                 },
                 "files": {
-                    "description": "This is a regular expression or list of regular expressions. This indicates that the job should only run on changes where the specified files are modified. Unlike branches, this value is subject to inheritance and overriding, so only the final value is used to determine if the job should run.",
+                    "description": "This is a regular expression or list of regular expression strings. This indicates that the job should only run on changes where the specified files are modified. Unlike branches, this value is subject to inheritance and overriding, so only the final value is used to determine if the job should run.",
+                    "format": "regex",
                     "items": {
+                        "format": "regex",
                         "type": "string"
                     },
                     "title": "job.files",
                     "type": [
                         "array",
                         "string"
                     ]
@@ -225,22 +239,24 @@
                 "intermediate": {
                     "default": false,
                     "description": "An intermediate job must be inherited by an abstract job; it can not be inherited by a final job. All intermediate jobs must also be abstract; a configuration error will be raised if not.\nOnce this is set to true in a job it cannot be reset to false within the same job by other variants; however jobs which inherit from it can (and by default do) reset it to false.\nFor example, you may define a base abstract job foo and create two abstract jobs that inherit from foo called foo-production and foo-development. If it would be an error to accidentally inherit from the base job foo instead of choosing one of the two variants, foo could be marked as intermediate.",
                     "title": "job.intermediate",
                     "type": "boolean"
                 },
                 "irrelevant-files": {
-                    "description": "A regular expression or list of regular expressions. It indicates that the job should run unless all of the files changed match this list. In other words, if the regular expression docs/.* is supplied, then this job will not run if the only files changed are in the docs directory.\nThis is a negative complement of files.",
+                    "description": "This is a regular expression or list of regular expression strings. It indicates that the job should run unless all of the files changed match this list. In other words, if the regular expression docs/.* is supplied, then this job will not run if the only files changed are in the docs directory.\nThis is a negative complement of files.",
+                    "format": "regex",
                     "items": {
+                        "format": "regex",
                         "type": "string"
                     },
                     "title": "job.irrelevant-files",
                     "type": [
-                        "string",
-                        "array"
+                        "array",
+                        "string"
                     ]
                 },
                 "match-on-config-updates": {
                     "default": true,
                     "description": "If this is set to true (the default), then the job\u2019s file matchers are ignored if a change alters the job\u2019s configuration. This means that changes to jobs with file matchers will be self-testing without requiring that the file matchers include the Zuul configuration file defining the job.",
                     "title": "job.match-on-config-updates",
                     "type": "boolean"
@@ -446,14 +462,15 @@
                 "secrets": {
                     "description": "A list of secrets which may be used by the job. A Secret is a named collection of private information defined separately in the configuration. The secrets that appear here must be defined in the same project as this job definition.\nEach item in the list may may be supplied either as a string, in which case it references the name of a Secret definition, or as a dict.",
                     "oneOf": [
                         {
                             "type": "string"
                         },
                         {
+                            "additionalProperties": false,
                             "properties": {
                                 "name": {
                                     "description": "The name to use for the Ansible variable into which the secret content will be placed.",
                                     "title": "job.secrets.name",
                                     "type": "string"
                                 },
                                 "pass-to-parent": {
@@ -475,18 +492,21 @@
                                 "name",
                                 "secret"
                             ],
                             "type": "object"
                         },
                         {
                             "items": {
-                                "$ref": "#/definitions/anonymous-job/properties/secrets/oneOf/1",
-                                "type": [
-                                    "string",
-                                    "object"
+                                "anyOf": [
+                                    {
+                                        "type": "string"
+                                    },
+                                    {
+                                        "$ref": "#/definitions/anonymous-job/properties/secrets/oneOf/1"
+                                    }
                                 ]
                             },
                             "type": "array"
                         }
                     ],
                     "title": "job.secrets"
                 },
@@ -1104,14 +1124,30 @@
                 "array",
                 "integer"
             ]
         },
         "gerrit-trigger": {
             "items": {
                 "properties": {
+                    "added": {
+                        "anyOf": [
+                            {
+                                "$ref": "#/definitions/regular-expression",
+                                "description": "This is only used for hashtags-changed events. It accepts a regex or list of regexes that are searched for in the list of hashtags added to the change in this event. If any of these regexes match a portion of any of the added hashtags, the trigger is matched."
+                            },
+                            {
+                                "items": {
+                                    "$ref": "#/definitions/regular-expression"
+                                },
+                                "type": "array"
+                            }
+                        ],
+                        "description": "This is only used for hashtags-changed events. It accepts a regex or list of regexes that are searched for in the list of hashtags added to the change in this event. If any of these regexes match a portion of any of the added hashtags, the trigger is matched.",
+                        "title": "pipeline.trigger.&lt;gerrit source&gt;.added"
+                    },
                     "approval": {
                         "description": "This is only used for comment-added events. It only matches if the event has a matching approval associated with it. Example: Code-Review: 2 matches a +2 vote on the code review category. Multiple approvals may be listed.",
                         "items": {
                             "additionalProperties": false,
                             "patternProperties": {
                                 "^(?!(event$|branch$|ref$|ignore-deletes$|email$|username$|comment$|require-approval$|reject-approval$|require$|reject$).*)": {
                                     "allOf": [
@@ -1124,65 +1160,77 @@
                             },
                             "type": "object"
                         },
                         "title": "pipeline.trigger.&lt;gerrit source&gt;.approval",
                         "type": "array"
                     },
                     "branch": {
+                        "anyOf": [
+                            {
+                                "$ref": "#/definitions/regular-expression",
+                                "description": "The branch associated with the event. Example: master. This field is treated as a regular expression, and multiple branches may be listed."
+                            },
+                            {
+                                "items": {
+                                    "$ref": "#/definitions/regular-expression"
+                                },
+                                "type": "array"
+                            }
+                        ],
                         "description": "The branch associated with the event. Example: master. This field is treated as a regular expression, and multiple branches may be listed.",
                         "examples": [
                             "master"
                         ],
-                        "items": {
-                            "type": "string"
-                        },
-                        "title": "pipeline.trigger.&lt;gerrit source&gt;.branch",
-                        "type": [
-                            "string",
-                            "array"
-                        ]
+                        "title": "pipeline.trigger.&lt;gerrit source&gt;.branch"
                     },
                     "comment": {
+                        "anyOf": [
+                            {
+                                "$ref": "#/definitions/regular-expression",
+                                "description": "This is only used for comment-added events. It accepts a list of regexes that are searched for in the comment string. If any of these regexes matches a portion of the comment string the trigger is matched. comment: retrigger will match when comments containing retrigger somewhere in the comment text are added to a change."
+                            },
+                            {
+                                "items": {
+                                    "$ref": "#/definitions/regular-expression"
+                                },
+                                "type": "array"
+                            }
+                        ],
                         "description": "This is only used for comment-added events. It accepts a list of regexes that are searched for in the comment string. If any of these regexes matches a portion of the comment string the trigger is matched. comment: retrigger will match when comments containing retrigger somewhere in the comment text are added to a change.",
-                        "format": "regex",
-                        "items": {
-                            "format": "regex",
-                            "type": "string"
-                        },
-                        "title": "pipeline.trigger.&lt;gerrit source&gt;.comment",
-                        "type": [
-                            "string",
-                            "array"
-                        ]
+                        "title": "pipeline.trigger.&lt;gerrit source&gt;.comment"
                     },
                     "email": {
+                        "anyOf": [
+                            {
+                                "$ref": "#/definitions/regular-expression",
+                                "description": "This is used for any event. It takes a regex applied on the performer email, i.e. Gerrit account email address. If you want to specify several email filters, you must use a YAML list. Make sure to use non greedy matchers and to escapes dots!"
+                            },
+                            {
+                                "items": {
+                                    "$ref": "#/definitions/regular-expression"
+                                },
+                                "type": "array"
+                            }
+                        ],
                         "description": "This is used for any event. It takes a regex applied on the performer email, i.e. Gerrit account email address. If you want to specify several email filters, you must use a YAML list. Make sure to use non greedy matchers and to escapes dots!",
                         "examples": [
                             "email: ^.*?@example\\.org$"
                         ],
-                        "format": "regex",
-                        "items": {
-                            "format": "regex",
-                            "type": "string"
-                        },
-                        "title": "pipeline.trigger.&lt;gerrit source&gt;.email",
-                        "type": [
-                            "string",
-                            "array"
-                        ]
+                        "title": "pipeline.trigger.&lt;gerrit source&gt;.email"
                     },
                     "event": {
                         "description": "The event name from gerrit.\nThis field is treated as a regular expression.",
                         "enum": [
                             "patchset-created",
                             "comment-added",
                             "ref-updated",
                             "change-restored",
                             "draft-published",
-                            "change-merged"
+                            "change-merged",
+                            "hashtags-changed"
                         ],
                         "examples": [
                             "patchset-created",
                             "comment-added",
                             "ref-updated"
                         ],
                         "title": "pipeline.trigger.&lt;gerrit source&gt;.event",
@@ -1191,23 +1239,28 @@
                     "ignore-deletes": {
                         "default": true,
                         "description": "When a branch is deleted, a ref-updated event is emitted with a newrev of all zeros specified. The ignore-deletes field is a boolean value that describes whether or not these newrevs trigger ref-updated events.",
                         "title": "pipeline.trigger.&lt;gerrit source&gt;.ignore-deletes",
                         "type": "boolean"
                     },
                     "ref": {
+                        "anyOf": [
+                            {
+                                "$ref": "#/definitions/regular-expression",
+                                "description": "On ref-updated events, the branch parameter is not used, instead the ref is provided. Currently Gerrit has the somewhat idiosyncratic behavior of specifying bare refs for branch names (e.g., master), but full ref names for other kinds of refs (e.g., refs/tags/foo). Zuul matches this value exactly against what Gerrit provides. This field is treated as a regular expression, and multiple refs may be listed."
+                            },
+                            {
+                                "items": {
+                                    "$ref": "#/definitions/regular-expression"
+                                },
+                                "type": "array"
+                            }
+                        ],
                         "description": "On ref-updated events, the branch parameter is not used, instead the ref is provided. Currently Gerrit has the somewhat idiosyncratic behavior of specifying bare refs for branch names (e.g., master), but full ref names for other kinds of refs (e.g., refs/tags/foo). Zuul matches this value exactly against what Gerrit provides. This field is treated as a regular expression, and multiple refs may be listed.",
-                        "items": {
-                            "type": "string"
-                        },
-                        "title": "pipeline.trigger.&lt;gerrit source&gt;.ref",
-                        "type": [
-                            "string",
-                            "array"
-                        ]
+                        "title": "pipeline.trigger.&lt;gerrit source&gt;.ref"
                     },
                     "reject": {
                         "allOf": [
                             {
                                 "description": "This may be used for any event and is the mirror of pipeline.trigger.<gerrit source>.require. It describes conditions that when met by the change cause the trigger event not to match. Those conditions may be satisfied by the event in question. It follows the same syntax as Requirements Configuration.",
                                 "title": "pipeline.trigger.&lt;gerrit source&gt;.reject"
                             },
@@ -1219,14 +1272,30 @@
                     },
                     "reject-approval": {
                         "deprecated": true,
                         "description": "This is deprecated and will be removed in a future version. Use pipeline.trigger.<gerrit source>.reject instead.\nThis takes a list of approvals in the same format as pipeline.trigger.<gerrit source>.require-approval but the item will fail to enter the pipeline if there is a matching approval.\nThis is ignored if the pipeline.trigger.<gerrit source>.reject attribute is present.",
                         "title": "pipeline.trigger.&lt;gerrit source&gt;.reject-approval",
                         "type": "object"
                     },
+                    "removed": {
+                        "anyOf": [
+                            {
+                                "$ref": "#/definitions/regular-expression",
+                                "description": "This is only used for hashtags-changed events. It accepts a regex or list of regexes that are searched for in the list of hashtags removed to the change in this event. If any of these regexes match a portion of any of the removed hashtags, the trigger is matched."
+                            },
+                            {
+                                "items": {
+                                    "$ref": "#/definitions/regular-expression"
+                                },
+                                "type": "array"
+                            }
+                        ],
+                        "description": "This is only used for hashtags-changed events. It accepts a regex or list of regexes that are searched for in the list of hashtags removed to the change in this event. If any of these regexes match a portion of any of the removed hashtags, the trigger is matched.",
+                        "title": "pipeline.trigger.&lt;gerrit source&gt;.removed"
+                    },
                     "require": {
                         "allOf": [
                             {
                                 "description": "This may be used for any event. It describes conditions that must be met by the change in order for the trigger event to match. Those conditions may be satisfied by the event in question. It follows the same syntax as Requirements Configuration.",
                                 "title": "pipeline.trigger.&lt;gerrit source&gt;.require"
                             },
                             {
@@ -1238,28 +1307,31 @@
                     "require-approval": {
                         "deprecated": true,
                         "description": "This is deprecated and will be removed in a future version. Use pipeline.trigger.<gerrit source>.require instead.\nThis may be used for any event. It requires that a certain kind of approval be present for the current patchset of the change (the approval could be added by the event in question). It follows the same syntax as pipeline.require.<gerrit source>.approval. For each specified criteria there must exist a matching approval.\nThis is ignored if the pipeline.trigger.<gerrit source>.require attribute is present.",
                         "title": "pipeline.trigger.&lt;gerrit source&gt;.require-approval",
                         "type": "object"
                     },
                     "username": {
+                        "anyOf": [
+                            {
+                                "$ref": "#/definitions/regular-expression",
+                                "description": "This is used for any event. It takes a regex applied on the performer username, i.e. Gerrit account name. If you want to specify several username filters, you must use a YAML list. Make sure to use non greedy matchers and to escapes dots."
+                            },
+                            {
+                                "items": {
+                                    "$ref": "#/definitions/regular-expression"
+                                },
+                                "type": "array"
+                            }
+                        ],
                         "description": "This is used for any event. It takes a regex applied on the performer username, i.e. Gerrit account name. If you want to specify several username filters, you must use a YAML list. Make sure to use non greedy matchers and to escapes dots.",
                         "examples": [
                             "username: ^zuul$"
                         ],
-                        "format": "regex",
-                        "items": {
-                            "format": "regex",
-                            "type": "string"
-                        },
-                        "title": "pipeline.trigger.&lt;gerrit source&gt;.username",
-                        "type": [
-                            "string",
-                            "array"
-                        ]
+                        "title": "pipeline.trigger.&lt;gerrit source&gt;.username"
                     }
                 },
                 "required": [
                     "event"
                 ],
                 "type": "object"
             },
@@ -1588,15 +1660,15 @@
                                     "reopened",
                                     "comment",
                                     "labeled",
                                     "unlabeled",
                                     "status",
                                     "submitted",
                                     "dismissed",
-                                    "requested",
+                                    "rerequested",
                                     "completed"
                                 ],
                                 "type": "string"
                             },
                             {
                                 "items": {
                                     "enum": [
@@ -1606,60 +1678,66 @@
                                         "reopened",
                                         "comment",
                                         "labeled",
                                         "unlabeled",
                                         "status",
                                         "submitted",
                                         "dismissed",
-                                        "requested",
+                                        "rerequested",
                                         "completed"
                                     ],
                                     "type": "string"
                                 },
                                 "type": "array"
                             }
                         ],
                         "title": "pipeline.trigger.&lt;github source&gt;.action"
                     },
                     "branch": {
+                        "anyOf": [
+                            {
+                                "$ref": "#/definitions/regular-expression",
+                                "description": "The branch associated with the event. Example: master. This field is treated as a regular expression, and multiple branches may be listed. Used for pull_request and pull_request_review events."
+                            },
+                            {
+                                "items": {
+                                    "$ref": "#/definitions/regular-expression"
+                                },
+                                "type": "array"
+                            }
+                        ],
                         "description": "The branch associated with the event. Example: master. This field is treated as a regular expression, and multiple branches may be listed. Used for pull_request and pull_request_review events.",
-                        "format": "regex",
-                        "items": {
-                            "format": "regex",
-                            "type": "string"
-                        },
-                        "title": "pipeline.trigger.&lt;github source&gt;.branch",
-                        "type": [
-                            "string",
-                            "array"
-                        ]
+                        "title": "pipeline.trigger.&lt;github source&gt;.branch"
                     },
                     "check": {
                         "description": "This is only used for check_run events. It works similar to the status attribute and accepts a list of strings each of which matches the app requesting or updating the check run, the check run\u2019s name and the conclusion in the format of app:name::conclusion. To make Zuul properly interact with Github\u2019s checks API, each pipeline that is using the checks API should have at least one trigger that matches the pipeline\u2019s name regardless of the result, e.g. zuul:cool-pipeline:.*. This will enable the cool-pipeline to trigger whenever a user requests the cool-pipeline check run as part of the zuul check suite. Additionally, one could use .*:success to trigger a pipeline whenever a successful check run is reported (e.g. useful for gating).",
                         "items": {
                             "type": "string"
                         },
                         "title": "pipeline.trigger.&lt;github source&gt;.check",
                         "type": [
                             "string",
                             "array"
                         ]
                     },
                     "comment": {
+                        "anyOf": [
+                            {
+                                "$ref": "#/definitions/regular-expression",
+                                "description": "This is only used for pull_request comment actions. It accepts a list of regexes that are searched for in the comment string. If any of these regexes matches a portion of the comment string the trigger is matched. comment: retrigger will match when comments containing 'retrigger' somewhere in the comment text are added to a pull request."
+                            },
+                            {
+                                "items": {
+                                    "$ref": "#/definitions/regular-expression"
+                                },
+                                "type": "array"
+                            }
+                        ],
                         "description": "This is only used for pull_request comment actions. It accepts a list of regexes that are searched for in the comment string. If any of these regexes matches a portion of the comment string the trigger is matched. comment: retrigger will match when comments containing 'retrigger' somewhere in the comment text are added to a pull request.",
-                        "format": "regex",
-                        "items": {
-                            "format": "regex",
-                            "type": "string"
-                        },
-                        "title": "pipeline.trigger.&lt;github source&gt;.comment",
-                        "type": [
-                            "string",
-                            "array"
-                        ]
+                        "title": "pipeline.trigger.&lt;github source&gt;.comment"
                     },
                     "event": {
                         "description": "The event from github. Supported events are:\r\n\r\n- pull_request\r\n- pull_request_review\r\n- push\r\n- check_run",
                         "enum": [
                             "pull_request",
                             "pull_request_review",
                             "push",
@@ -1673,23 +1751,28 @@
                         "items": {
                             "type": "string"
                         },
                         "title": "pipeline.trigger.&lt;github source&gt;.label",
                         "type": "array"
                     },
                     "ref": {
+                        "anyOf": [
+                            {
+                                "$ref": "#/definitions/regular-expression",
+                                "description": "This is only used for push events. This field is treated as a regular expression and multiple refs may be listed. GitHub always sends full ref name, eg. refs/tags/bar and this string is matched against the regular expression."
+                            },
+                            {
+                                "items": {
+                                    "$ref": "#/definitions/regular-expression"
+                                },
+                                "type": "array"
+                            }
+                        ],
                         "description": "This is only used for push events. This field is treated as a regular expression and multiple refs may be listed. GitHub always sends full ref name, eg. refs/tags/bar and this string is matched against the regular expression.",
-                        "items": {
-                            "type": "string"
-                        },
-                        "title": "pipeline.trigger.&lt;github source&gt;.ref",
-                        "type": [
-                            "string",
-                            "array"
-                        ]
+                        "title": "pipeline.trigger.&lt;github source&gt;.ref"
                     },
                     "reject": {
                         "allOf": [
                             {
                                 "description": "This may be used for any event and is the mirror of pipeline.trigger.<github source>.require. It describes conditions that when met by the PR cause the trigger event not to match. Those conditions may be satisfied by the event in question. It follows the same syntax as Requirements Configuration.",
                                 "title": "pipeline.trigger.&lt;github source&gt;.reject"
                             },
@@ -1791,14 +1874,17 @@
                 },
                 "topic": {
                     "description": "The MQTT topic to publish messages. The topic can be a format string that can use the following parameters: tenant, pipeline, project, branch, change, patchset and ref. MQTT topic can have hierarchy separated by '/'.",
                     "title": "pipeline.&lt;reporter&gt;.&lt;mqtt source&gt;.topic",
                     "type": "string"
                 }
             },
+            "required": [
+                "topic"
+            ],
             "title": "pipeline.&lt;reporter&gt;.&lt;mqtt source&gt;",
             "type": "object"
         },
         "nodeset": {
             "allOf": [
                 {
                     "properties": {
@@ -2209,15 +2295,15 @@
                 },
                 "implied-branches": {
                     "description": "This is a list of regular expressions, just as job.branches, which may be used to supply the value of the implied branch matcher for all jobs and project-templates in a file.\nThis may be useful if two projects share jobs but have dissimilar branch names.",
                     "examples": [
                         "https://zuul-ci.org/docs/zuul/latest/config/pragma.html#attr-pragma.implied-branches"
                     ],
                     "items": {
-                        "type": "string"
+                        "$ref": "#/definitions/regular-expression"
                     },
                     "title": "pragma.implied-branches",
                     "type": "array"
                 }
             },
             "title": "Pragma",
             "type": "object"
@@ -2386,14 +2472,45 @@
             },
             "required": [
                 "name"
             ],
             "title": "Queue",
             "type": "object"
         },
+        "regular-expression": {
+            "anyOf": [
+                {
+                    "format": "regex",
+                    "type": "string"
+                },
+                {
+                    "additionalProperties": false,
+                    "properties": {
+                        "negate": {
+                            "default": false,
+                            "description": "Whether to negate the match.",
+                            "title": "<regular-expression>.negate",
+                            "type": "boolean"
+                        },
+                        "regex": {
+                            "description": "The pattern for the regular expression. This uses the RE2 syntax.",
+                            "format": "regex",
+                            "title": "<regular-expression>.regex",
+                            "type": "string"
+                        }
+                    },
+                    "required": [
+                        "regex"
+                    ],
+                    "type": "object"
+                }
+            ],
+            "description": "Many options accept literal strings or regular expressions. In these cases, the regular expression matching starts at the beginning of the string as if there were an implicit ^ at the start of the regular expression. To match at an arbitrary position, prepend .* to the regular expression.\nZuul uses the RE2 library which has a restricted regular expression syntax compared to PCRE.\nSome options may be specified for regular expressions. To do so, use a dictionary to specify the regular expression in the YAML configuration.",
+            "title": "<regular-expression>"
+        },
         "run-type": {
             "anyOf": [
                 {
                     "type": "string"
                 },
                 {
                     "$ref": "#/definitions/run-type-object"
@@ -2616,11 +2733,11 @@
             "semaphore": {
                 "$ref": "#/definitions/semaphore",
                 "type": "object"
             }
         },
         "type": "object"
     },
-    "title": "JSON/YAML schema for Zuul CI 9.3.0 configuration files",
+    "title": "JSON/YAML schema for Zuul CI 10.0.0 configuration files",
     "type": "array",
-    "version": "1.0.2"
+    "version": "1.1.1"
 }
```

### Comparing `zuulcilint-0.2.5/PKG-INFO` & `zuulcilint-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zuulcilint
-Version: 0.2.5
+Version: 0.2.6
 Summary: Zuul CI linter
 Home-page: https://github.com/codesquadnest/zuulcilint
 License: MIT
 Keywords: zuul,ci,linter
 Author: Pedro Baptista
 Author-email: pedro.miguel.baptista@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -51,15 +51,15 @@
 
 ## Validate with pre-commit
 
 Add the code below to your `.pre-commit-config.yaml` file:
 
 ```yaml
   - repo: https://github.com/codesquadnest/zuulcilint.git
-    rev: "0.2.5"
+    rev: "0.2.6"
     hooks:
       - id: zuulcilint
 ```
 
 
 ## Validate with VS Code
```

