# Comparing `tmp/spanish_chat_sdk-0.1.8.tar.gz` & `tmp/spanish_chat_sdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spanish_chat_sdk-0.1.8.tar", max compression
+gzip compressed data, was "spanish_chat_sdk-0.1.9.tar", max compression
```

## Comparing `spanish_chat_sdk-0.1.8.tar` & `spanish_chat_sdk-0.1.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     5009 2024-02-29 19:31:38.268414 spanish_chat_sdk-0.1.8/README.md
--rw-r--r--   0        0        0      591 2024-04-19 17:42:52.063661 spanish_chat_sdk-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      151 2024-04-19 18:43:48.890155 spanish_chat_sdk-0.1.8/spanish_chat_sdk/__init__.py
--rw-r--r--   0        0        0       47 2024-04-19 18:43:48.773486 spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 18:43:48.836820 spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/chat/__init__.py
--rw-r--r--   0        0        0     3640 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/chat/get_placement_test_chat_get_placement_test_get.py
--rw-r--r--   0        0        0     5136 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/chat/send_message_chat_send_message_post.py
--rw-r--r--   0        0        0        0 2024-04-19 18:43:48.836820 spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/conversations/__init__.py
--rw-r--r--   0        0        0     2187 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/conversations/end_all_user_conversations_conversations_end_all_get.py
--rw-r--r--   0        0        0     2164 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/conversations/end_conversation_conversations_end_post.py
--rw-r--r--   0        0        0     4979 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/conversations/get_current_conversation_messages_conversations_active_messages_post.py
--rw-r--r--   0        0        0     3380 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/conversations/start_conversation_conversations_start_post.py
--rw-r--r--   0        0        0        0 2024-04-19 18:43:48.846821 spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/default/__init__.py
--rw-r--r--   0        0        0     2085 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/default/welcome_get.py
--rw-r--r--   0        0        0        0 2024-04-19 18:43:48.840154 spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/grammar/__init__.py
--rw-r--r--   0        0        0     4401 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/grammar/check_grammar_grammar_check_post.py
--rw-r--r--   0        0        0     4443 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/grammar/check_grammar_v2_grammar_check_v2_post.py
--rw-r--r--   0        0        0     4447 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/grammar/translate_message_grammar_translate_post.py
--rw-r--r--   0        0        0        0 2024-04-19 18:43:48.796819 spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/users/__init__.py
--rw-r--r--   0        0        0     2174 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/users/get_current_cefr_level_users_cefr_level_get.py
--rw-r--r--   0        0        0     3281 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/users/get_me_users_me_get.py
--rw-r--r--   0        0        0     3624 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/users/get_users_users_get.py
--rw-r--r--   0        0        0     4757 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/users/login_for_access_token_users_token_post.py
--rw-r--r--   0        0        0     5822 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/users/register_account_users_register_post.py
--rw-r--r--   0        0        0    12131 2024-04-19 18:43:48.896822 spanish_chat_sdk-0.1.8/spanish_chat_sdk/client.py
--rw-r--r--   0        0        0      470 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.8/spanish_chat_sdk/errors.py
--rw-r--r--   0        0        0     1691 2024-04-19 18:43:48.863488 spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/__init__.py
--rw-r--r--   0        0        0     4255 2024-04-19 18:43:48.896822 spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/body_login_for_access_token_users_token_post.py
--rw-r--r--   0        0        0     3004 2024-04-19 18:43:48.896822 spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/conversation.py
--rw-r--r--   0        0        0     3734 2024-04-19 18:43:48.896822 spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/grammar_error.py
--rw-r--r--   0        0        0     2510 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/grammar_error_v2.py
--rw-r--r--   0        0        0     1900 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/grammar_errors.py
--rw-r--r--   0        0        0     1951 2024-04-19 18:43:48.896822 spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/grammar_errors_v2.py
--rw-r--r--   0        0        0     2193 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/http_validation_error.py
--rw-r--r--   0        0        0     2710 2024-04-19 18:43:48.896822 spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/message.py
--rw-r--r--   0        0        0     1655 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/placement_test_answer.py
--rw-r--r--   0        0        0     2267 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/placement_test_follow_up_question.py
--rw-r--r--   0        0        0     4760 2024-04-19 18:43:48.896822 spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/placement_test_question.py
--rw-r--r--   0        0        0      179 2024-04-19 18:43:48.863488 spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/placement_test_question_type.py
--rw-r--r--   0        0        0     2101 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/placement_test_questions.py
--rw-r--r--   0        0        0     1960 2024-04-19 18:43:48.896822 spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/send_message_chat_send_message_post_response_send_message_chat_send_message_post.py
--rw-r--r--   0        0        0     1667 2024-04-19 18:43:48.896822 spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/token.py
--rw-r--r--   0        0        0     1683 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/translation_usage_example.py
--rw-r--r--   0        0        0     2662 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/user.py
--rw-r--r--   0        0        0     2153 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/validation_error.py
--rw-r--r--   0        0        0     2400 2024-04-19 18:43:48.896822 spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/word_translation.py
--rw-r--r--   0        0        0       25 2024-04-19 18:43:48.656816 spanish_chat_sdk-0.1.8/spanish_chat_sdk/py.typed
--rw-r--r--   0        0        0      986 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.8/spanish_chat_sdk/types.py
--rw-r--r--   0        0        0     5679 1970-01-01 00:00:00.000000 spanish_chat_sdk-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     5009 2024-02-29 19:31:38.268414 spanish_chat_sdk-0.1.9/README.md
+-rw-r--r--   0        0        0      591 2024-04-19 18:45:05.148754 spanish_chat_sdk-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      151 2024-04-19 18:43:48.890155 spanish_chat_sdk-0.1.9/spanish_chat_sdk/__init__.py
+-rw-r--r--   0        0        0       47 2024-04-19 18:43:48.773486 spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 18:43:48.836820 spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/chat/__init__.py
+-rw-r--r--   0        0        0     3640 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/chat/get_placement_test_chat_get_placement_test_get.py
+-rw-r--r--   0        0        0     5136 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/chat/send_message_chat_send_message_post.py
+-rw-r--r--   0        0        0        0 2024-04-19 18:43:48.836820 spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/conversations/__init__.py
+-rw-r--r--   0        0        0     2187 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/conversations/end_all_user_conversations_conversations_end_all_get.py
+-rw-r--r--   0        0        0     2164 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/conversations/end_conversation_conversations_end_post.py
+-rw-r--r--   0        0        0     4979 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/conversations/get_current_conversation_messages_conversations_active_messages_post.py
+-rw-r--r--   0        0        0     3380 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/conversations/start_conversation_conversations_start_post.py
+-rw-r--r--   0        0        0        0 2024-04-19 18:43:48.846821 spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/default/__init__.py
+-rw-r--r--   0        0        0     2085 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/default/welcome_get.py
+-rw-r--r--   0        0        0        0 2024-04-19 18:43:48.840154 spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/grammar/__init__.py
+-rw-r--r--   0        0        0     4401 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/grammar/check_grammar_grammar_check_post.py
+-rw-r--r--   0        0        0     4443 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/grammar/check_grammar_v2_grammar_check_v2_post.py
+-rw-r--r--   0        0        0     4447 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/grammar/translate_message_grammar_translate_post.py
+-rw-r--r--   0        0        0        0 2024-04-19 18:43:48.796819 spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/users/__init__.py
+-rw-r--r--   0        0        0     2174 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/users/get_current_cefr_level_users_cefr_level_get.py
+-rw-r--r--   0        0        0     3281 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/users/get_me_users_me_get.py
+-rw-r--r--   0        0        0     3624 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/users/get_users_users_get.py
+-rw-r--r--   0        0        0     4757 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/users/login_for_access_token_users_token_post.py
+-rw-r--r--   0        0        0     5822 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/users/register_account_users_register_post.py
+-rw-r--r--   0        0        0    12131 2024-04-19 18:43:48.896822 spanish_chat_sdk-0.1.9/spanish_chat_sdk/client.py
+-rw-r--r--   0        0        0      470 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.9/spanish_chat_sdk/errors.py
+-rw-r--r--   0        0        0     1691 2024-04-19 18:43:48.863488 spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/__init__.py
+-rw-r--r--   0        0        0     4255 2024-04-19 18:43:48.896822 spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/body_login_for_access_token_users_token_post.py
+-rw-r--r--   0        0        0     3004 2024-04-19 18:43:48.896822 spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/conversation.py
+-rw-r--r--   0        0        0     3734 2024-04-19 18:43:48.896822 spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/grammar_error.py
+-rw-r--r--   0        0        0     2510 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/grammar_error_v2.py
+-rw-r--r--   0        0        0     1900 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/grammar_errors.py
+-rw-r--r--   0        0        0     1951 2024-04-19 18:43:48.896822 spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/grammar_errors_v2.py
+-rw-r--r--   0        0        0     2193 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/http_validation_error.py
+-rw-r--r--   0        0        0     2710 2024-04-19 18:43:48.896822 spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/message.py
+-rw-r--r--   0        0        0     1655 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/placement_test_answer.py
+-rw-r--r--   0        0        0     2267 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/placement_test_follow_up_question.py
+-rw-r--r--   0        0        0     4760 2024-04-19 18:43:48.896822 spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/placement_test_question.py
+-rw-r--r--   0        0        0      179 2024-04-19 18:43:48.863488 spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/placement_test_question_type.py
+-rw-r--r--   0        0        0     2101 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/placement_test_questions.py
+-rw-r--r--   0        0        0     1960 2024-04-19 18:43:48.896822 spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/send_message_chat_send_message_post_response_send_message_chat_send_message_post.py
+-rw-r--r--   0        0        0     1667 2024-04-19 18:43:48.896822 spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/token.py
+-rw-r--r--   0        0        0     1683 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/translation_usage_example.py
+-rw-r--r--   0        0        0     2662 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/user.py
+-rw-r--r--   0        0        0     2153 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/validation_error.py
+-rw-r--r--   0        0        0     2400 2024-04-19 18:43:48.896822 spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/word_translation.py
+-rw-r--r--   0        0        0       25 2024-04-19 18:43:48.656816 spanish_chat_sdk-0.1.9/spanish_chat_sdk/py.typed
+-rw-r--r--   0        0        0      986 2024-04-19 18:43:48.893489 spanish_chat_sdk-0.1.9/spanish_chat_sdk/types.py
+-rw-r--r--   0        0        0     5679 1970-01-01 00:00:00.000000 spanish_chat_sdk-0.1.9/PKG-INFO
```

### Comparing `spanish_chat_sdk-0.1.8/README.md` & `spanish_chat_sdk-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/pyproject.toml` & `spanish_chat_sdk-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spanish-chat-sdk"
-version = "0.1.8"
+version = "0.1.9"
 description = "A client library for accessing the Spanish chat API"
 authors = ["Marshall Bruner <brunerm99@gmail.com>"]
 readme = "README.md"
 packages = [
     {include = "spanish_chat_sdk"},
 ]
 include = ["CHANGELOG.md", "spanish_chat_sdk/py.typed"]
```

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/chat/get_placement_test_chat_get_placement_test_get.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/chat/get_placement_test_chat_get_placement_test_get.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/chat/send_message_chat_send_message_post.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/chat/send_message_chat_send_message_post.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/conversations/end_all_user_conversations_conversations_end_all_get.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/conversations/end_all_user_conversations_conversations_end_all_get.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/conversations/end_conversation_conversations_end_post.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/conversations/end_conversation_conversations_end_post.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/conversations/get_current_conversation_messages_conversations_active_messages_post.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/conversations/get_current_conversation_messages_conversations_active_messages_post.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/conversations/start_conversation_conversations_start_post.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/conversations/start_conversation_conversations_start_post.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/default/welcome_get.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/default/welcome_get.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/grammar/check_grammar_grammar_check_post.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/grammar/check_grammar_grammar_check_post.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/grammar/check_grammar_v2_grammar_check_v2_post.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/grammar/check_grammar_v2_grammar_check_v2_post.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/grammar/translate_message_grammar_translate_post.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/grammar/translate_message_grammar_translate_post.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/users/get_current_cefr_level_users_cefr_level_get.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/users/get_current_cefr_level_users_cefr_level_get.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/users/get_me_users_me_get.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/users/get_me_users_me_get.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/users/get_users_users_get.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/users/get_users_users_get.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/users/login_for_access_token_users_token_post.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/users/login_for_access_token_users_token_post.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/api/users/register_account_users_register_post.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/api/users/register_account_users_register_post.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/client.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/client.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/__init__.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/body_login_for_access_token_users_token_post.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/body_login_for_access_token_users_token_post.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/conversation.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/conversation.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/grammar_error.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/grammar_error.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/grammar_error_v2.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/grammar_error_v2.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/grammar_errors.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/grammar_errors.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/grammar_errors_v2.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/grammar_errors_v2.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/http_validation_error.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/message.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/message.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/placement_test_answer.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/placement_test_answer.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/placement_test_follow_up_question.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/placement_test_follow_up_question.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/placement_test_question.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/placement_test_question.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/placement_test_questions.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/placement_test_questions.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/send_message_chat_send_message_post_response_send_message_chat_send_message_post.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/send_message_chat_send_message_post_response_send_message_chat_send_message_post.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/token.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/token.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/translation_usage_example.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/translation_usage_example.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/user.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/user.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/validation_error.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/models/word_translation.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/models/word_translation.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/spanish_chat_sdk/types.py` & `spanish_chat_sdk-0.1.9/spanish_chat_sdk/types.py`

 * *Files identical despite different names*

### Comparing `spanish_chat_sdk-0.1.8/PKG-INFO` & `spanish_chat_sdk-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spanish-chat-sdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: A client library for accessing the Spanish chat API
 Author: Marshall Bruner
 Author-email: brunerm99@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

