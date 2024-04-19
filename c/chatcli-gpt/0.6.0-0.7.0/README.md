# Comparing `tmp/chatcli_gpt-0.6.0.tar.gz` & `tmp/chatcli_gpt-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatcli_gpt-0.6.0.tar", max compression
+gzip compressed data, was "chatcli_gpt-0.7.0.tar", max compression
```

## Comparing `chatcli_gpt-0.6.0.tar` & `chatcli_gpt-0.7.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1067 2023-04-02 09:18:53.460518 chatcli_gpt-0.6.0/LICENSE
--rw-r--r--   0        0        0     9105 2023-11-23 15:38:44.412950 chatcli_gpt-0.6.0/README.md
--rw-r--r--   0        0        0        0 2023-03-26 16:42:53.990448 chatcli_gpt-0.6.0/chatcli_gpt/__init__.py
--rw-r--r--   0        0        0       30 2023-04-15 05:23:10.942580 chatcli_gpt-0.6.0/chatcli_gpt/__main__.py
--rw-r--r--   0        0        0    14514 2023-11-23 15:38:44.408950 chatcli_gpt-0.6.0/chatcli_gpt/cli.py
--rw-r--r--   0        0        0     4863 2023-11-23 15:38:44.400950 chatcli_gpt-0.6.0/chatcli_gpt/conversation.py
--rw-r--r--   0        0        0     3956 2023-11-10 12:26:15.489784 chatcli_gpt-0.6.0/chatcli_gpt/data/default_log
--rw-r--r--   0        0        0     4375 2023-11-22 10:38:22.658912 chatcli_gpt-0.6.0/chatcli_gpt/log.py
--rw-r--r--   0        0        0     2318 2023-11-23 15:38:44.408950 chatcli_gpt-0.6.0/chatcli_gpt/models.py
--rw-r--r--   0        0        0     4785 2023-08-25 15:40:16.066624 chatcli_gpt-0.6.0/chatcli_gpt/plugins.py
--rw-r--r--   0        0        0     1381 2023-11-23 15:38:44.412950 chatcli_gpt-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    10218 1970-01-01 00:00:00.000000 chatcli_gpt-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-21 20:21:46.075305 chatcli_gpt-0.7.0/LICENSE
+-rw-r--r--   0        0        0     9105 2023-11-29 19:04:14.386492 chatcli_gpt-0.7.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-21 20:23:44.371665 chatcli_gpt-0.7.0/chatcli_gpt/__init__.py
+-rw-r--r--   0        0        0       30 2023-04-21 20:23:51.363683 chatcli_gpt-0.7.0/chatcli_gpt/__main__.py
+-rw-r--r--   0        0        0    16205 2024-04-19 13:26:55.346080 chatcli_gpt-0.7.0/chatcli_gpt/cli.py
+-rw-r--r--   0        0        0     5467 2024-04-18 16:53:58.548713 chatcli_gpt-0.7.0/chatcli_gpt/conversation.py
+-rw-r--r--   0        0        0     3956 2023-11-29 19:04:14.386492 chatcli_gpt-0.7.0/chatcli_gpt/data/default_log
+-rw-r--r--   0        0        0     4479 2024-04-14 07:52:10.247599 chatcli_gpt-0.7.0/chatcli_gpt/log.py
+-rw-r--r--   0        0        0     2394 2024-04-19 13:27:54.878504 chatcli_gpt-0.7.0/chatcli_gpt/models.py
+-rw-r--r--   0        0        0     4871 2024-04-14 07:52:10.311601 chatcli_gpt-0.7.0/chatcli_gpt/plugins.py
+-rw-r--r--   0        0        0     1322 2024-04-19 14:02:18.360717 chatcli_gpt-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    10218 1970-01-01 00:00:00.000000 chatcli_gpt-0.7.0/PKG-INFO
```

### Comparing `chatcli_gpt-0.6.0/LICENSE` & `chatcli_gpt-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chatcli_gpt-0.6.0/README.md` & `chatcli_gpt-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `chatcli_gpt-0.6.0/chatcli_gpt/cli.py` & `chatcli_gpt-0.7.0/chatcli_gpt/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,43 +12,53 @@
 
 from .log import (
     write_log,
     search_conversations,
     conversation_log,
     create_initial_log,
 )
-from .conversation import Conversation
+from .conversation import Conversation, is_personality
 from . import models
 
-from .models import MODELS
+from .models import get_models
 
 MESSAGE_COLORS = {
     "user": (186, 85, 211),
     "system": (100, 150, 200),
     "assistant": None,
 }
 
 DEFAULT_MODEL = "gpt-3.5-turbo-1106"
 
 
-class PartialChoice(click.Choice):
+class PartialChoice(click.types.ParamType):
+    def __init__(self, name, get_choices, **kwargs):
+        self.name = name
+        self._get_choices = get_choices
+        super().__init__(**kwargs)
+
+    @property
+    def choices(self):
+        return self._get_choices()
+
     def convert(self, value, param, ctx):
         for choice in self.choices:
             if value in choice:
                 return choice
         return self.fail(
             f"invalid choice: {value}. (choose from {', '.join(self.choices)})",
             param,
             ctx,
         )
 
 
-MODEL_CHOICE = PartialChoice([model["id"] for model in MODELS])
-
-USAGE_COSTS = {model["id"]: model["pricing"] for model in MODELS}
+MODEL_CHOICE = PartialChoice(
+    name="MODEL",
+    get_choices=lambda: [model["id"] for model in get_models()],
+)
 
 
 def coro(f):
     @functools.wraps(f)
     def wrapper(*args, **kwargs):
         return asyncio.run(f(*args, **kwargs))
 
@@ -71,15 +81,17 @@
             offset = 1
         if kwargs.get("select_personality") and not (tag or search or offset):
             tag = "^" + kwargs["select_personality"]
         kwargs.pop("select_personality", None)
         if kwargs.get("new") and not (tag or search or offset):
             conversation = Conversation({})
         else:
-            conversation = get_logged_conversation(offset=offset, search=search, tag=tag)
+            conversation = get_logged_conversation(
+                offset=offset, search=search, tag=tag
+            )
         return command(
             *args,
             conversation=conversation,
             **kwargs,
         )
 
     return wrapper
@@ -100,79 +112,106 @@
             **kwargs,
         )
 
     return wrapper
 
 
 @cli.command(help="Ask a question of ChatGPT.")
-@click.option("-q", "--quick", is_flag=True, help="Just handle a one single-line question.")
+@click.option(
+    "-q", "--quick", is_flag=True, help="Just handle a one single-line question."
+)
 @click.option(
     "-c",
     "--continue_conversation",
     "--continue",
     is_flag=True,
     help="Continue previous conversation.",
 )
-@click.option("-p", "--personality", "select_personality", default="default", help="Personality to use.")
+@click.option(
+    "-p",
+    "--personality",
+    "select_personality",
+    default="default",
+    help="Personality to use.",
+)
 @click.option(
     "-f",
     "--file",
     type=click.Path(exists=True),
     multiple=True,
     help="Add a file to the conversation for context.",
 )
 @click.option("-r", "--retry", is_flag=True, help="Retry previous question")
 @click.option("--stream/--sync", default=True, help="Stream or sync mode.")
-@click.option("-m", "--model", type=MODEL_CHOICE)
+@click.option(
+    "-m",
+    "--model",
+    type=MODEL_CHOICE,
+    help="Model to use. Run `chatcli models list` to see available models.",
+)
 @click.option("--plugin", "additional_plugins", multiple=True, help="Load a plugin.")
 @select_conversation
 def chat(conversation, **kwargs):
+    conversation = conversation.clone()
+
     for filename in kwargs["file"]:
         with Path(filename).open(encoding="utf-8") as fh:
             file_contents = fh.read()
 
-        conversation.append("user", f"The file {filename!r} contains:\n```\n{file_contents}```")
-
-    tags = conversation.tags
-    tags_to_apply = [tags[-1]] if tags and not is_personality(tags[-1]) else []
+        conversation.append(
+            "user", f"The file {filename!r} contains:\n```\n{file_contents}```"
+        )
 
     conversation.plugins.extend(kwargs["additional_plugins"])
-    conversation.tags = tags_to_apply
     conversation.model = kwargs["model"] or conversation.model or DEFAULT_MODEL
 
     quick = kwargs["quick"] or not os.isatty(0)
     multiline = not quick
 
     if kwargs["retry"]:
         conversation.messages.pop()
         add_answer(conversation, stream=kwargs["stream"])
         if kwargs["quick"]:
             return
 
-    run_conversation(conversation, multiline=multiline, quick=quick, stream=kwargs["stream"])
+    run_conversation(
+        conversation, multiline=multiline, quick=quick, stream=kwargs["stream"]
+    )
 
 
 @cli.command(help="Create initial conversation log.")
-@click.option("-r", "--reinit", is_flag=True, help="re-initialize the personalities to default values")
+@click.option(
+    "-r",
+    "--reinit",
+    is_flag=True,
+    help="re-initialize the personalities to default values",
+)
 def init(reinit):
     try:
         create_initial_log(reinit)
     except FileExistsError as error:
         click.echo(f"{error}: Conversation log already exists.", file=sys.stderr)
         sys.exit(1)
 
 
 @cli.command(help="Add a message to a new or existing conversation.")
 @click.option("--multiline/--singleline", default=True)
 @click.option("-p", "--personality", help="")
-@click.option("--role", type=click.Choice(["system", "user", "assistant"]), default="system")
+@click.option(
+    "--role", type=click.Choice(["system", "user", "assistant"]), default="system"
+)
 @click.option("--plugin", multiple="True", help="Activate plugins.")
 @click.option("-m", "--model", type=MODEL_CHOICE)
 @click.option("--plugin", "additional_plugins", multiple=True, help="Load a plugin.")
-@click.option("--new/--continue", "-n/-c", default=True, help="Create a new conversation or continue.")
+@click.option(
+    "--new/--continue",
+    "-n/-c",
+    default=True,
+    help="Create a new conversation or continue.",
+)
 @select_conversation
 def add(conversation, personality, role, multiline, **kwargs):
     tags = conversation.tags
     tags_to_apply = [tags[-1]] if tags and not is_personality(tags[-1]) else []
 
     conversation.plugins.extend(kwargs["additional_plugins"])
     conversation.tags = tags_to_apply
@@ -190,14 +229,50 @@
 
 def merge_list(input_list, additions):
     for item in additions:
         if item not in input_list:
             input_list.append(item)
 
 
+@cli.command(help="Edit the last message in a conversation.")
+@click.option("-m", "--model", type=MODEL_CHOICE)
+@click.option("--prompt/--no-prompt", default=True)
+@click.option(
+    "-p",
+    "--personality",
+    "select_personality",
+    default="default",
+    help="Personality to use.",
+)
+@select_conversation
+def edit(conversation, **kwargs):
+    if kwargs["prompt"]:
+        content = prompt(
+            multiline=True,
+            default=conversation.messages[-1]["content"],
+        )
+
+        conversation.messages[-1]["content"] = content
+
+    if kwargs.get("model"):
+        conversation.model = kwargs["model"]
+
+    if kwargs.get("personality"):
+        conversation.add_tag(f"^{kwargs['personality']}")
+
+    write_log(conversation)
+
+
+@cli.command(help="Remove the last message in a conversation.")
+@select_conversation
+def drop(conversation):
+    conversation.messages.pop()
+    write_log(conversation)
+
+
 @cli.command(help="Create a new conversation by merging existing conversations.")
 @click.option("-p", "--personality", help="Set personality for new conversation.")
 @filter_conversations
 def merge(conversations, personality):
     merged_conversation = {
         "messages": [],
         "tags": [],
@@ -205,27 +280,29 @@
         "model": None,
     }
     if personality:
         merged_conversation["tags"].append("^" + personality)
 
     for _, item in reversed(list(conversations)):
         merge_list(merged_conversation["messages"], item.messages)
-        merge_list(merged_conversation["tags"], (tag for tag in item.tags if not is_personality(tag)))
+        merge_list(
+            merged_conversation["tags"],
+            (tag for tag in item.tags if not is_personality(tag)),
+        )
         merge_list(merged_conversation["plugins"], item.plugins)
         merged_conversation["model"] = item.model or merged_conversation["model"]
 
     write_log(Conversation(merged_conversation))
 
 
 @cli.command(help="List tags.", name="tags")
 def list_tags():
     tags = set()
     for conversation in conversation_log():
-        for tag in conversation.tags:
-            tags.add(tag)
+        tags |= set(conversation.tags)
     for tag in sorted(tags):
         click.echo(tag)
 
 
 @cli.command(help="List personalities.", name="personalities")
 def list_personalities():
     personalities = set()
@@ -237,18 +314,15 @@
         click.echo(personality)
 
 
 @cli.command(help="Add tags to an conversation.", name="tag")
 @click.argument("new_tag")
 @select_conversation
 def add_tag(new_tag, conversation):
-    new_tags = [tag for tag in conversation.tags if tag != new_tag]
-    new_tags.append(new_tag)
-    conversation.tags = new_tags
-
+    conversation.add_tag(new_tag)
     write_log(conversation)
 
 
 @cli.command(help="Remove tags from an conversation.")
 @click.argument("tag_to_remove")
 @select_conversation
 def untag(tag_to_remove, conversation):
@@ -260,61 +334,81 @@
 @select_conversation
 def show_tag(conversation):
     if conversation.tags:
         click.echo(conversation.tags[-1])
 
 
 @cli.command(help="Show a conversation.")
-@click.option("-p", "--personality", "select_personality", help="Select conversation by personality.")
+@click.option(
+    "-p",
+    "--personality",
+    "select_personality",
+    help="Select conversation by personality.",
+)
 @select_conversation
 @click.option(
     "-l/-s",
     "--long/--short",
     help="Show full conversation or just the most recent message.",
 )
-@click.option("--format-json", "--json", is_flag=True, help="Output conversation in JSON format.")
+@click.option(
+    "--format-json", "--json", is_flag=True, help="Output conversation in JSON format."
+)
 def show(long, conversation, format_json):
     if format_json:
         click.echo(conversation.to_json())
         return
 
     messages = conversation.messages if long else conversation.messages[-1:]
 
     for message in messages:
         prefix = ""
         if message["role"] == "user":
             prefix = ">> "
-        click.echo(click.style(prefix + message["content"], fg=MESSAGE_COLORS[message["role"]]))
+        click.echo(
+            click.style(prefix + message["content"], fg=MESSAGE_COLORS[message["role"]])
+        )
 
 
 @cli.command(help="Display conversation log.")
-@click.option("-p", "--personality", "select_personality", help="Select conversation by personality.")
+@click.option(
+    "-p",
+    "--personality",
+    "select_personality",
+    help="Select conversation by personality.",
+)
 @filter_conversations
 @click.option("--limit", "-l", type=int, help="Limit number of results")
 @click.option("--usage", "-u", is_flag=True, help="Show token usage")
 @click.option("--cost", is_flag=True, help="Show token cost")
 @click.option("--plugins", is_flag=True, help="Show enabled plugins")
 @click.option("-m", "--model", is_flag=True, help="Show model")
-@click.option("--json", "format_json", is_flag=True, help="Output conversation in JSON format.")
+@click.option(
+    "--json", "format_json", is_flag=True, help="Output conversation in JSON format."
+)
 def log(conversations, limit, format_json, **kwargs):
     for offset, conversation in reversed(list(itertools.islice(conversations, limit))):
         if format_json:
             click.echo(conversation.to_json())
             continue
         try:
-            question = conversation.find(lambda message: message["role"] != "assistant")["content"]
+            question = conversation.find(
+                lambda message: message["role"] != "assistant"
+            )["content"]
         except ValueError:
             question = conversation.messages[-1]["content"]
         trimmed_message = question.strip().split("\n", 1)[0][:80]
 
         fields = []
         fields.append(click.style(f"{offset: 4d}:", fg="blue"))
 
         if kwargs["usage"]:
-            total_tokens = conversation.usage["total_tokens"] if conversation.usage else 0
+            total_tokens = (
+                conversation.usage["total_tokens"] if conversation.usage else 0
+            )
             fields.append(f"{total_tokens: 5d}")
 
         if kwargs["cost"]:
             fields.append(f"${conversation_cost(conversation): 2.3f}")
 
         fields.append(trimmed_message)
         if conversation.tags:
@@ -343,72 +437,96 @@
         conversation.append("user", question)
         add_answer(conversation, stream=stream)
 
         if quick:
             break
 
 
-def prompt(*, multiline=True):
+def prompt(*, multiline=True, **kwargs):
     if os.isatty(0):
         try:
-            return prompt_toolkit.prompt(">> ", multiline=multiline, prompt_continuation=".. ").strip()
+            return prompt_toolkit.prompt(
+                ">> ",
+                multiline=multiline,
+                prompt_continuation=".. ",
+                **kwargs,
+            ).strip()
         except EOFError:
             return None
     else:
         return sys.stdin.read().strip()
 
 
 @cli.command(help="Add an answer to a question")
 @click.option("--stream/--sync", default=True, help="Stream or sync mode.")
+@click.option("-m", "--model", type=MODEL_CHOICE)
 @select_conversation
-def answer(conversation, stream):
+def answer(conversation, stream, **kwargs):
+    conversation = conversation.clone(**kwargs)
     add_answer(conversation, stream=stream)
 
 
 @coro
 async def add_answer(conversation, *, stream=True):
     while True:
-        response = await conversation.complete(stream=stream, callback=lambda token: click.echo(token, nl=False))
+        response = await conversation.complete(
+            stream=stream, callback=lambda token: click.echo(token, nl=False)
+        )
         click.echo()
-        write_log(conversation, completion=conversation.completion, usage=conversation.usage)
+        write_log(
+            conversation, completion=conversation.completion, usage=conversation.usage
+        )
         from . import plugins
 
-        plugin_response = plugins.evaluate_plugins(response["content"], conversation.plugins)
+        plugin_response = plugins.evaluate_plugins(
+            response["content"], conversation.plugins
+        )
         if not plugin_response:
             break
         click.echo(click.style(plugin_response, fg=(200, 180, 90)))
         conversation.append("user", plugin_response)
 
 
 def conversation_cost(conversation):
+    usage_costs = {model["id"]: model["pricing"] for model in get_models()}
+
     if not conversation.usage:
         return 0
     model = conversation.completion["model"]
     model_price = (
-        USAGE_COSTS.get(model) or USAGE_COSTS.get("-".join(model.split("-")[:-1])) or USAGE_COSTS["openrouter/" + model]
+        usage_costs.get(model)
+        or usage_costs.get("-".join(model.split("-")[:-1]))
+        or usage_costs["openrouter/" + model]
     )
 
     usage = conversation.usage
     return (
-        float(model_price["prompt"]) * usage["prompt_tokens"] / 1000
-        + float(model_price["completion"]) * usage["completion_tokens"] / 1000
+        float(model_price["prompt"]) * usage["prompt_tokens"]
+        + float(model_price["completion"]) * usage["completion_tokens"]
     )
 
 
 @cli.command(help="Display number of tokens and token cost.", name="usage")
 @click.option("--today", is_flag=True, help="Show usage for today only.")
 def show_usage(today):
     conversations = conversation_log()
 
     def is_today(conversation):
-        return dateutil.parser.parse(conversation.timestamp).date() == datetime.now(tz=timezone.utc).date()
+        return (
+            dateutil.parser.parse(conversation.timestamp).date()
+            == datetime.now(tz=timezone.utc).date()
+        )
 
     if today:
         conversations = [c for c in conversations if is_today(c)]
-    tokens = sum(conversation.usage["total_tokens"] for conversation in conversations if conversation.usage)
+    tokens = sum(
+        conversation.usage["total_tokens"]
+        for conversation in conversations
+        if conversation.usage
+    )
 
     total_cost = sum(conversation_cost(conversation) for conversation in conversations)
     click.echo(f"Tokens: {tokens}")
     click.echo(f"Cost: ${total_cost:.2f}")
 
 
 def get_logged_conversation(offset, search=None, tag=None):
@@ -416,18 +534,14 @@
     try:
         return next(search_conversations(offsets, search, tag))[1]
     except StopIteration:
         click.echo("Matching conversation not found", file=sys.stderr)
         sys.exit(1)
 
 
-def is_personality(tag):
-    return tag.startswith("^")
-
-
 def main():
     try:
         cli()
     except FileNotFoundError as error:
         click.echo(f"{error}: Chatcli not initialized. Run `chatcli init` first.")
         sys.exit(1)
```

### Comparing `chatcli_gpt-0.6.0/chatcli_gpt/conversation.py` & `chatcli_gpt-0.7.0/chatcli_gpt/conversation.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,19 @@
         self.completion = conversation_data.get("completion")
         self.timestamp = conversation_data.get("timestamp")
 
     def append(self, role, content):
         self.messages.append({"role": role, "content": content})
 
     def __contains__(self, search_term):
-        question = self.messages[-2]["content"] if len(self.messages) > 1 else self.messages[-1]["content"]
+        question = (
+            self.messages[-2]["content"]
+            if len(self.messages) > 1
+            else self.messages[-1]["content"]
+        )
         return search_term in question
 
     def to_json(self):
         return json.dumps(self.__dict__)
 
     def find(self, predicate):
         for message in reversed(self.messages):
@@ -44,29 +48,54 @@
         response_message = completion["choices"][0]["message"]
         self.append(**response_message)
         self.completion = completion
         self.usage = completion_usage(self.messages[:-1], self.model, completion)
 
         return response_message
 
+    def add_tag(self, tag):
+        self.tags = [t for t in self.tags if t != tag]
+        self.tags.append(tag)
+
+    def clone(self, *, model=None):
+        data = copy(self.__dict__)
+        data["tags"] = (
+            [data["tags"][-1]]
+            if data["tags"] and not is_personality(data["tags"][-1])
+            else []
+        )
+        data.pop("completion", None)
+        if model:
+            data["model"] = model
+        return type(self)(data)
+
+
+def is_personality(tag):
+    return tag.startswith("^")
+
 
 def completion_usage(request_messages, model, completion):
     if "usage" in completion:
         return completion["usage"]
 
     import tiktoken
 
     try:
         encoding = tiktoken.encoding_for_model(model)
     except KeyError:
         encoding = tiktoken.encoding_for_model("gpt-3.5-turbo")
 
-    request_text = " ".join("role: " + x["role"] + " content: " + x["content"] + "\n" for x in request_messages)
+    request_text = " ".join(
+        "role: " + x["role"] + " content: " + x["content"] + "\n"
+        for x in request_messages
+    )
     request_tokens = len(encoding.encode(request_text))
-    completion_tokens = len(encoding.encode(completion["choices"][0]["message"]["content"]))
+    completion_tokens = len(
+        encoding.encode(completion["choices"][0]["message"]["content"])
+    )
     return {
         "prompt_tokens": request_tokens,
         "completion_tokens": completion_tokens,
         "total_tokens": request_tokens + completion_tokens,
     }
```

### Comparing `chatcli_gpt-0.6.0/chatcli_gpt/data/default_log` & `chatcli_gpt-0.7.0/chatcli_gpt/data/default_log`

 * *Files identical despite different names*

### Comparing `chatcli_gpt-0.6.0/chatcli_gpt/log.py` & `chatcli_gpt-0.7.0/chatcli_gpt/log.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,15 +106,20 @@
                 del usage["request_tokens"]
 
             tags = data.get("tags", [])
             completion = data.get("completion") or data.get("response")
 
             timestamp = (
                 data.get("timestamp")
-                or (completion and datetime.fromtimestamp(completion.get("created"), tz=timezone.utc).isoformat())
+                or (
+                    completion
+                    and datetime.fromtimestamp(
+                        completion.get("created"), tz=timezone.utc
+                    ).isoformat()
+                )
                 or datetime.now(tz=timezone.utc).isoformat()
             )
 
             assert isinstance(messages, list), data
             assert isinstance(tags, list), data
             assert isinstance(completion, dict) or completion is None, (
                 completion,
```

### Comparing `chatcli_gpt-0.6.0/chatcli_gpt/models.py` & `chatcli_gpt-0.7.0/chatcli_gpt/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,49 +4,59 @@
 import json
 
 import click
 from click_default_group import DefaultGroup
 
 OPENROUTER_API_KEY = os.environ.get("OPENROUTER_API_KEY")
 
-MODEL_CACHE = Path("/home/akelly/.chatcli.models.json")
+MODEL_CACHE = Path.home() / ".chatcli.models.json"
 
 OPENAI_MODELS = [
-    "gpt-4-1106-preview",
-    "gpt-3.5-turbo-1106",
-    "gpt-4",
-    "gpt-3.5-turbo",
-]
-
-# Create the above LIST but in the format [{ "id": "gpt-4-1106-preview" }, ...]
-OPENAI_MODELS = [
     {
         "id": "gpt-4-1106-preview",
-        "pricing": {"prompt": 0.01, "completion": 0.03},
+        "pricing": {"prompt": 0.01 / 1000, "completion": 0.03 / 1000},
     },
     {
         "id": "gpt-3.5-turbo-1106",
-        "pricing": {"prompt": 0.001, "completion": 0.002},
+        "pricing": {"prompt": 0.001 / 1000, "completion": 0.002 / 1000},
     },
     {
         "id": "gpt-4",
-        "pricing": {"prompt": 0.03, "completion": 0.06},
+        "pricing": {"prompt": 0.03 / 1000, "completion": 0.06 / 1000},
     },
     {
         "id": "gpt-3.5-turbo",
-        "pricing": {"prompt": 0.002, "completion": 0.002},
+        "pricing": {"prompt": 0.002 / 1000, "completion": 0.002 / 1000},
     },
 ]
 
-MODELS = OPENAI_MODELS
-if MODEL_CACHE.exists():
-    MODELS += json.load(MODEL_CACHE.open())
+
+_MODELS = None
+
+
+def get_models():
+    global _MODELS  # noqa: PLW0603
+
+    if _MODELS is None:
+        _MODELS = []
+        _MODELS.extend(OPENAI_MODELS)
+        if MODEL_CACHE.exists():
+            _MODELS += json.load(MODEL_CACHE.open())
+    return _MODELS
+
+
+MODELS = get_models()
 
 
-@click.group(cls=DefaultGroup, default="list", default_if_no_args=True, help="View and manage models")
+@click.group(
+    cls=DefaultGroup,
+    default="list",
+    default_if_no_args=True,
+    help="View and manage models",
+)
 def models():
     pass
 
 
 @models.command(name="list", help="List available models")
 def list_models():
     for model in MODELS:
```

### Comparing `chatcli_gpt-0.6.0/chatcli_gpt/plugins.py` & `chatcli_gpt-0.7.0/chatcli_gpt/plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,17 @@
 
 
 def extract_blocks(response_text, plugin):
     return re.findall(BLOCK_PATTERNS[plugin], response_text, re.DOTALL)
 
 
 def exec_bash(code):
-    result = subprocess.run(["/bin/bash", "-c", code], capture_output=True, text=True, check=False)
+    result = subprocess.run(
+        ["/bin/bash", "-c", code], capture_output=True, text=True, check=False
+    )
 
     return {
         "result": result.stdout.strip(),
         "error": result.stderr.strip(),
     }
 
 
@@ -102,21 +104,27 @@
     return {
         "result": stdout.getvalue().strip(),
         "error": stderr.getvalue().strip(),
     }
 
 
 def exec_duckduckgo(search_term):
-    return {"result": json.dumps(duckduckgo_search.ddg(search_term, max_results=5), indent=2)}
+    return {
+        "result": json.dumps(
+            duckduckgo_search.ddg(search_term, max_results=5), indent=2
+        )
+    }
 
 
 def exec_wolfram(query):
     api_key = os.environ.get("WOLFRAM_ALPHA_API_KEY")
     if not api_key:
-        return {"error": "WOLFRAM_ALPHA_API_KEY is not configured. (Set as an environment variable.)"}
+        return {
+            "error": "WOLFRAM_ALPHA_API_KEY is not configured. (Set as an environment variable.)"
+        }
     client = wolframalpha.Client(api_key)
     result = client.query(query)
     return {"result": next(result.results).text}
 
 
 def generate_image(prompt):
     image_api_response = openai.Image.create(prompt=prompt, n=1, size="256x256")
@@ -133,9 +141,11 @@
     if output.get("error"):
         output_blocks.append(f"ERROR:\n```\n{output['error']}\n```")
     return "\n".join(output_blocks)
 
 
 if __name__ == "__main__":
     print("(Finish input with <Alt-Enter> or <Esc><Enter>)")
-    input_text = prompt_toolkit.prompt(multiline=True, prompt=">>> ", continuation_prompt="... ")
+    input_text = prompt_toolkit.prompt(
+        multiline=True, prompt=">>> ", continuation_prompt="... "
+    )
     print(evaluate_plugins(input_text, sys.argv[1:]))
```

### Comparing `chatcli_gpt-0.6.0/pyproject.toml` & `chatcli_gpt-0.7.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chatcli-gpt"
-version = "0.6.0"
+version = "0.7.0"
 description = "A command line interface for interacting with GPT-3. It's orientated around an append only chat log so you get a complete history of your conversations."
 readme = "README.md"
 license = "MIT"
 authors = ["Adam Kelly <adam@cthulahoops.org>"]
 repository = "https://github.com/cthulahoops/chatcli"
 
 [tool.poetry.dependencies]
@@ -23,24 +23,20 @@
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 pytest = "^7.2.2"
 pytest-mock = "^3.10.0"
 pytest-cov = "^4.0.0"
-ruff = "^0.0.261"
-pytest-asyncio = "^0.21.1"
+ruff = "^0.3.7"
+pytest-asyncio = "^0.23.6"
 
 [tool.poetry.scripts]
 chatcli = "chatcli_gpt.cli:main"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
-select = ["A", "B", "C","E", "F", "G", "I", "N", "Q", "T", "W", "ARG", "BLE", "COM", "DJ", "DTZ", "EM", "ERA", "EXE", "FBT", "ICN", "INP", "ISC", "NPY", "PD", "PGH", "PIE", "PL", "PT", "PTH", "PYI", "RET", "RSE", "RUF", "SIM", "SLF", "TCH", "TID", "UP", "YTT"]
+select = ["A", "B", "C","E", "F", "G", "I", "N", "Q", "T", "W", "ARG", "BLE", "DJ", "DTZ", "EM", "ERA", "EXE", "FBT", "ICN", "INP", "ISC", "NPY", "PD", "PGH", "PIE", "PL", "PT", "PTH", "PYI", "RET", "RSE", "RUF", "SIM", "SLF", "TCH", "TID", "UP", "YTT"]
 ignore = ["INP001", "I001", "PLR2004", "T201", "EM101", "EM102", "PGH001"]
-line-length = 120
-
-[tool.black]
-line-length = 120
```

### Comparing `chatcli_gpt-0.6.0/PKG-INFO` & `chatcli_gpt-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcli-gpt
-Version: 0.6.0
+Version: 0.7.0
 Summary: A command line interface for interacting with GPT-3. It's orientated around an append only chat log so you get a complete history of your conversations.
 Home-page: https://github.com/cthulahoops/chatcli
 License: MIT
 Author: Adam Kelly
 Author-email: adam@cthulahoops.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

