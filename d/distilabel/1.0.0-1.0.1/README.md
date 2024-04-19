# Comparing `tmp/distilabel-1.0.0.tar.gz` & `tmp/distilabel-1.0.1.tar.gz`

## Comparing `distilabel-1.0.0.tar` & `distilabel-1.0.1.tar`

### file list

```diff
@@ -1,253 +1,256 @@
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 distilabel-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 distilabel-1.0.0/Makefile
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 distilabel-1.0.0/mkdocs.yml
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 distilabel-1.0.0/.github/ISSUE_TEMPLATE/blank-issue-template.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 distilabel-1.0.0/.github/ISSUE_TEMPLATE/🆕-feature-request.md
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 distilabel-1.0.0/.github/ISSUE_TEMPLATE/🐛-bug-report.md
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 distilabel-1.0.0/.github/ISSUE_TEMPLATE/📚-documentation-update.md
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 distilabel-1.0.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 distilabel-1.0.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 distilabel-1.0.0/.github/workflows/test.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/CNAME
--rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/index.md
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/overview.md
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/cli.md
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/llms/anthropic.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/llms/anyscale.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/llms/azure.md
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/llms/huggingface.md
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/llms/litellm.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/llms/llamacpp.md
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/llms/mistral.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/llms/ollama.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/llms/openai.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/llms/together.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/llms/vertexai.md
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/llms/vllm.md
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/pipeline/pipeline.md
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/steps/argilla.md
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/steps/decorator.md
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/steps/extra.md
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/steps/steps.md
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/steps/generator_steps/generator_steps.md
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/steps/global_steps/global_steps.md
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/steps/tasks/embeddings.md
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/steps/tasks/preference_tasks.md
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/steps/tasks/text_generation.md
--rw-r--r--   0        0        0    16279 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/distilabel-badge-dark.png
--rw-r--r--   0        0        0    15551 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/distilabel-badge-light.png
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/distilabel-icon.svg
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/logo.svg
--rw-r--r--   0        0        0    47284 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/images/distilabel-diagram-dark.svg
--rw-r--r--   0        0        0    47244 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/images/distilabel-diagram.svg
--rw-r--r--   0        0        0   301103 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/images/sections/caching/caching_pipe_1.png
--rw-r--r--   0        0        0   329256 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/images/sections/caching/caching_pipe_2.png
--rw-r--r--   0        0        0   129190 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/images/sections/caching/caching_pipe_3.png
--rw-r--r--   0        0        0    24695 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/images/sections/caching/caching_pipe_4.png
--rw-r--r--   0        0        0   368245 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/images/sections/cli/cli_pipe.png
--rw-r--r--   0        0        0  1290074 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/images/sections/learn/steps/argilla/preference.png
--rw-r--r--   0        0        0  1014081 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/images/sections/learn/steps/argilla/text_generation.png
--rw-r--r--   0        0        0   173971 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/tutorials-assets/instrucion_dataset_notus_ui.png
--rw-r--r--   0        0        0   356586 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/tutorials-assets/preference_dataset_notus_ui.png
--rw-r--r--   0        0        0    19151 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/tutorials-assets/deita/datasets.png
--rw-r--r--   0        0        0    96338 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/tutorials-assets/deita/diversity.png
--rw-r--r--   0        0        0   191403 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/tutorials-assets/deita/overview.png
--rw-r--r--   0        0        0    94813 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/tutorials-assets/deita/results.png
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/scripts/gen_ref_pages.py
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/learn/caching.md
--rw-r--r--   0        0        0     7963 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/learn/cli.md
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/learn/distiset.md
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/learn/index.md
--rw-r--r--   0        0        0     7708 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/learn/llms/index.md
--rw-r--r--   0        0        0    14338 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/learn/pipelines/index.md
--rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/learn/steps/argilla.md
--rw-r--r--   0        0        0     8669 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/learn/steps/general_steps.md
--rw-r--r--   0        0        0     6941 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/learn/steps/generator_steps.md
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/learn/steps/global_steps.md
--rw-r--r--   0        0        0     8491 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/learn/steps/index.md
--rw-r--r--   0        0        0     7803 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/learn/tasks/feedback_tasks.md
--rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/learn/tasks/index.md
--rw-r--r--   0        0        0     5887 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/learn/tasks/special_tasks.md
--rw-r--r--   0        0        0    16125 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/learn/tasks/text_generation.md
--rw-r--r--   0        0        0    21822 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/papers/deita.md
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/papers/index.md
--rw-r--r--   0        0        0     5921 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/papers/instruction_backtranslation.md
--rw-r--r--   0        0        0     6730 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/papers/ultrafeedback.md
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/stylesheets/extra.css
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/__init__.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/__main__.py
--rw-r--r--   0        0        0     9461 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/distiset.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/cli/__init__.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/cli/app.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/cli/pipeline/__init__.py
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/cli/pipeline/app.py
--rw-r--r--   0        0        0     8197 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/cli/pipeline/utils.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/__init__.py
--rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/anthropic.py
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/anyscale.py
--rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/azure.py
--rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/base.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/chat_templates.py
--rw-r--r--   0        0        0     9147 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/cohere.py
--rw-r--r--   0        0        0     8176 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/litellm.py
--rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/llamacpp.py
--rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/mistral.py
--rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/mixins.py
--rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/ollama.py
--rw-r--r--   0        0        0     6609 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/openai.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/together.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/typing.py
--rw-r--r--   0        0        0     6905 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/vertexai.py
--rw-r--r--   0        0        0     7200 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/vllm.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/huggingface/__init__.py
--rw-r--r--   0        0        0    15077 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/huggingface/inference_endpoints.py
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/huggingface/transformers.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/mixins/__init__.py
--rw-r--r--   0        0        0     6971 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/mixins/runtime_parameters.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/pipeline/__init__.py
--rw-r--r--   0        0        0    17954 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/pipeline/_dag.py
--rw-r--r--   0        0        0    37076 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/pipeline/base.py
--rw-r--r--   0        0        0    32476 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/pipeline/local.py
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/pipeline/utils.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/__init__.py
--rw-r--r--   0        0        0    19355 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/base.py
--rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/combine.py
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/conversation.py
--rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/decorator.py
--rw-r--r--   0        0        0     9152 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/deita.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/expand.py
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/keep.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/typing.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/argilla/__init__.py
--rw-r--r--   0        0        0     5690 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/argilla/base.py
--rw-r--r--   0        0        0    10934 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/argilla/preference.py
--rw-r--r--   0        0        0     6705 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/argilla/text_generation.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/generators/__init__.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/generators/data.py
--rw-r--r--   0        0        0     7256 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/generators/huggingface.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/globals/__init__.py
--rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/globals/huggingface.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/__init__.py
--rw-r--r--   0        0        0     6966 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/base.py
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/complexity_scorer.py
--rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/generate_embeddings.py
--rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/instruction_backtranslation.py
--rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/pair_rm.py
--rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/quality_scorer.py
--rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/self_instruct.py
--rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/text_generation.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/typing.py
--rw-r--r--   0        0        0     9452 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/ultrafeedback.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/evol_instruct/__init__.py
--rw-r--r--   0        0        0    12081 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/evol_instruct/base.py
--rw-r--r--   0        0        0    10714 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/evol_instruct/english_nouns.txt
--rw-r--r--   0        0        0    12857 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/evol_instruct/generator.py
--rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/evol_instruct/utils.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/evol_instruct/evol_complexity/__init__.py
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/evol_instruct/evol_complexity/base.py
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/evol_instruct/evol_complexity/generator.py
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/evol_instruct/evol_complexity/utils.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/evol_quality/__init__.py
--rw-r--r--   0        0        0     9098 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/evol_quality/base.py
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/evol_quality/utils.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/templates/instruction-backtranslation.jinja2
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/templates/self-instruct.jinja2
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/templates/ultrafeedback/helpfulness.jinja2
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/templates/ultrafeedback/honesty.jinja2
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/templates/ultrafeedback/instruction-following.jinja2
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/templates/ultrafeedback/overall-rating.jinja2
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/templates/ultrafeedback/truthfulness.jinja2
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/utils/__init__.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/utils/chat.py
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/utils/dicts.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/utils/docstring.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/utils/files.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/utils/itertools.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/utils/lists.py
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/utils/logging.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/utils/notebook.py
--rw-r--r--   0        0        0    10480 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/utils/serialization.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/utils/typing_.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/utils/card/__init__.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/utils/card/dataset_card.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/utils/card/distilabel_template.md
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/integration/test_pipe_llms.py
--rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/integration/test_pipe_simple.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/__init__.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/test_distiset.py
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/test_imports.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/cli/__init__.py
--rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/cli/test_pipeline.yaml
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/cli/utils.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/cli/pipeline/__init__.py
--rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/cli/pipeline/test_app.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/cli/pipeline/utils.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/llms/__init__.py
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/llms/test_anthropic.py
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/llms/test_anyscale.py
--rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/llms/test_azure.py
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/llms/test_cohere.py
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/llms/test_litellm.py
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/llms/test_llamacpp.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/llms/test_mistral.py
--rw-r--r--   0        0        0     5748 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/llms/test_mixins.py
--rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/llms/test_ollama.py
--rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/llms/test_openai.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/llms/test_together.py
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/llms/test_vertexai.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/llms/huggingface/__init__.py
--rw-r--r--   0        0        0     6669 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/llms/huggingface/test_inference_endpoints.py
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/llms/huggingface/test_transformers.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/mixins/__init__.py
--rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/mixins/test_runtime_parameters.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/pipeline/__init__.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/pipeline/conftest.py
--rw-r--r--   0        0        0    44539 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/pipeline/test_base.py
--rw-r--r--   0        0        0    17227 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/pipeline/test_dag.py
--rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/pipeline/test_local.py
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/pipeline/utils.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/__init__.py
--rw-r--r--   0        0        0     9554 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/test_base.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/test_combine.py
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/test_conversation.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/test_decorator.py
--rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/test_deita.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/test_expand.py
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/test_keep.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/argilla/__init__.py
--rw-r--r--   0        0        0     5814 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/argilla/test_base.py
--rw-r--r--   0        0        0     5725 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/argilla/test_preference.py
--rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/argilla/test_text_generation.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/generators/test_data.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/__init__.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/conftest.py
--rw-r--r--   0        0        0     6065 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/test_base.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/test_complexity_scorer.py
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/test_generate_embeddings.py
--rw-r--r--   0        0        0     5289 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/test_instruction_backtranslation.py
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/test_pair_rm.py
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/test_quality_scorer.py
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/test_self_instruct.py
--rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/test_text_generation.py
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/test_ultrafeedback.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/utils.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/evol_instruct/__init__.py
--rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/evol_instruct/test_base.py
--rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/evol_instruct/test_generator.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/__init__.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_base.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_generator.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/evol_quality/__init__.py
--rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/evol_quality/test_base.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/utils/__init__.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/utils/test_chat.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/utils/test_docstring.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/utils/test_lists.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/utils/test_typing.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 distilabel-1.0.0/.gitignore
--rw-r--r--   0        0        0    11355 2020-02-02 00:00:00.000000 distilabel-1.0.0/LICENSE
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 distilabel-1.0.0/LICENSE_HEADER
--rw-r--r--   0        0        0     9299 2020-02-02 00:00:00.000000 distilabel-1.0.0/README.md
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 distilabel-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    12494 2020-02-02 00:00:00.000000 distilabel-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 distilabel-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 distilabel-1.0.1/Makefile
+-rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 distilabel-1.0.1/mkdocs.yml
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 distilabel-1.0.1/.github/ISSUE_TEMPLATE/blank-issue-template.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 distilabel-1.0.1/.github/ISSUE_TEMPLATE/🆕-feature-request.md
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 distilabel-1.0.1/.github/ISSUE_TEMPLATE/🐛-bug-report.md
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 distilabel-1.0.1/.github/ISSUE_TEMPLATE/📚-documentation-update.md
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 distilabel-1.0.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 distilabel-1.0.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 distilabel-1.0.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/CNAME
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/index.md
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/overview.md
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/cli.md
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/llms/anthropic.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/llms/anyscale.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/llms/azure.md
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/llms/huggingface.md
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/llms/index.md
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/llms/litellm.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/llms/llamacpp.md
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/llms/mistral.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/llms/ollama.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/llms/openai.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/llms/together.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/llms/vertexai.md
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/llms/vllm.md
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/pipeline/pipeline.md
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/steps/argilla.md
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/steps/decorator.md
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/steps/extra.md
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/steps/index.md
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/steps/generator_steps/generator_steps.md
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/steps/global_steps/global_steps.md
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/steps/tasks/embeddings.md
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/steps/tasks/preference_tasks.md
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/api/steps/tasks/text_generation.md
+-rw-r--r--   0        0        0    16279 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/distilabel-badge-dark.png
+-rw-r--r--   0        0        0    15551 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/distilabel-badge-light.png
+-rw-r--r--   0        0        0    11187 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/distilabel-black.png
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/distilabel-icon.svg
+-rw-r--r--   0        0        0     7678 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/distilabel-white.png
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/logo.svg
+-rw-r--r--   0        0        0    47284 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/images/distilabel-diagram-dark.svg
+-rw-r--r--   0        0        0    47244 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/images/distilabel-diagram.svg
+-rw-r--r--   0        0        0   301103 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/images/sections/caching/caching_pipe_1.png
+-rw-r--r--   0        0        0   329256 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/images/sections/caching/caching_pipe_2.png
+-rw-r--r--   0        0        0   129190 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/images/sections/caching/caching_pipe_3.png
+-rw-r--r--   0        0        0    24695 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/images/sections/caching/caching_pipe_4.png
+-rw-r--r--   0        0        0   368245 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/images/sections/cli/cli_pipe.png
+-rw-r--r--   0        0        0  1290074 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/images/sections/learn/steps/argilla/preference.png
+-rw-r--r--   0        0        0  1014081 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/images/sections/learn/steps/argilla/text_generation.png
+-rw-r--r--   0        0        0   173971 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/tutorials-assets/instrucion_dataset_notus_ui.png
+-rw-r--r--   0        0        0   356586 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/tutorials-assets/preference_dataset_notus_ui.png
+-rw-r--r--   0        0        0    19151 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/tutorials-assets/deita/datasets.png
+-rw-r--r--   0        0        0    96338 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/tutorials-assets/deita/diversity.png
+-rw-r--r--   0        0        0   191403 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/tutorials-assets/deita/overview.png
+-rw-r--r--   0        0        0    94813 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/assets/tutorials-assets/deita/results.png
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/scripts/gen_ref_pages.py
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/learn/caching.md
+-rw-r--r--   0        0        0     7963 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/learn/cli.md
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/learn/distiset.md
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/learn/index.md
+-rw-r--r--   0        0        0     7708 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/learn/llms/index.md
+-rw-r--r--   0        0        0    14701 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/learn/pipelines/index.md
+-rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/learn/steps/argilla.md
+-rw-r--r--   0        0        0     8669 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/learn/steps/general_steps.md
+-rw-r--r--   0        0        0     6941 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/learn/steps/generator_steps.md
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/learn/steps/global_steps.md
+-rw-r--r--   0        0        0     8491 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/learn/steps/index.md
+-rw-r--r--   0        0        0     7803 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/learn/tasks/feedback_tasks.md
+-rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/learn/tasks/index.md
+-rw-r--r--   0        0        0     5887 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/learn/tasks/special_tasks.md
+-rw-r--r--   0        0        0    16125 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/learn/tasks/text_generation.md
+-rw-r--r--   0        0        0    21822 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/papers/deita.md
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/papers/index.md
+-rw-r--r--   0        0        0     5921 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/papers/instruction_backtranslation.md
+-rw-r--r--   0        0        0     6730 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/sections/papers/ultrafeedback.md
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 distilabel-1.0.1/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/__init__.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/__main__.py
+-rw-r--r--   0        0        0     9461 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/distiset.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/cli/__init__.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/cli/app.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/cli/pipeline/__init__.py
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/cli/pipeline/app.py
+-rw-r--r--   0        0        0     8197 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/cli/pipeline/utils.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/__init__.py
+-rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/anthropic.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/anyscale.py
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/azure.py
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/base.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/chat_templates.py
+-rw-r--r--   0        0        0     9147 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/cohere.py
+-rw-r--r--   0        0        0     8176 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/litellm.py
+-rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/llamacpp.py
+-rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/mistral.py
+-rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/mixins.py
+-rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/ollama.py
+-rw-r--r--   0        0        0     6609 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/openai.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/together.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/typing.py
+-rw-r--r--   0        0        0     6905 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/vertexai.py
+-rw-r--r--   0        0        0     7200 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/vllm.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/huggingface/__init__.py
+-rw-r--r--   0        0        0    15717 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/huggingface/inference_endpoints.py
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/llms/huggingface/transformers.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/mixins/__init__.py
+-rw-r--r--   0        0        0     6971 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/mixins/runtime_parameters.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/pipeline/__init__.py
+-rw-r--r--   0        0        0    17954 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/pipeline/_dag.py
+-rw-r--r--   0        0        0    37076 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/pipeline/base.py
+-rw-r--r--   0        0        0    32476 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/pipeline/local.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/pipeline/utils.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/__init__.py
+-rw-r--r--   0        0        0    19355 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/base.py
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/combine.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/conversation.py
+-rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/decorator.py
+-rw-r--r--   0        0        0     9152 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/deita.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/expand.py
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/keep.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/typing.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/argilla/__init__.py
+-rw-r--r--   0        0        0     5690 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/argilla/base.py
+-rw-r--r--   0        0        0    10934 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/argilla/preference.py
+-rw-r--r--   0        0        0     6705 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/argilla/text_generation.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/generators/__init__.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/generators/data.py
+-rw-r--r--   0        0        0     7256 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/generators/huggingface.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/globals/__init__.py
+-rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/globals/huggingface.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/__init__.py
+-rw-r--r--   0        0        0     6966 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/base.py
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/complexity_scorer.py
+-rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/generate_embeddings.py
+-rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/instruction_backtranslation.py
+-rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/pair_rm.py
+-rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/quality_scorer.py
+-rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/self_instruct.py
+-rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/text_generation.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/typing.py
+-rw-r--r--   0        0        0     9452 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/ultrafeedback.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/__init__.py
+-rw-r--r--   0        0        0    12081 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/base.py
+-rw-r--r--   0        0        0    10714 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/english_nouns.txt
+-rw-r--r--   0        0        0    12857 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/generator.py
+-rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/evol_complexity/__init__.py
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/evol_complexity/base.py
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/evol_complexity/generator.py
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/evol_complexity/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/evol_quality/__init__.py
+-rw-r--r--   0        0        0     9098 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/evol_quality/base.py
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/evol_quality/utils.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/templates/instruction-backtranslation.jinja2
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/templates/self-instruct.jinja2
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/templates/ultrafeedback/helpfulness.jinja2
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/templates/ultrafeedback/honesty.jinja2
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/templates/ultrafeedback/instruction-following.jinja2
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/templates/ultrafeedback/overall-rating.jinja2
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/steps/tasks/templates/ultrafeedback/truthfulness.jinja2
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/utils/__init__.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/utils/chat.py
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/utils/dicts.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/utils/docstring.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/utils/files.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/utils/itertools.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/utils/lists.py
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/utils/logging.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/utils/notebook.py
+-rw-r--r--   0        0        0    10480 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/utils/serialization.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/utils/typing_.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/utils/card/__init__.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/utils/card/dataset_card.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 distilabel-1.0.1/src/distilabel/utils/card/distilabel_template.md
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/integration/test_pipe_llms.py
+-rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/integration/test_pipe_simple.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/__init__.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/test_distiset.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/test_imports.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/cli/__init__.py
+-rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/cli/test_pipeline.yaml
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/cli/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/cli/pipeline/__init__.py
+-rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/cli/pipeline/test_app.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/cli/pipeline/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/llms/__init__.py
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/llms/test_anthropic.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/llms/test_anyscale.py
+-rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/llms/test_azure.py
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/llms/test_cohere.py
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/llms/test_litellm.py
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/llms/test_llamacpp.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/llms/test_mistral.py
+-rw-r--r--   0        0        0     5748 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/llms/test_mixins.py
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/llms/test_ollama.py
+-rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/llms/test_openai.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/llms/test_together.py
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/llms/test_vertexai.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/llms/huggingface/__init__.py
+-rw-r--r--   0        0        0     6669 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/llms/huggingface/test_inference_endpoints.py
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/llms/huggingface/test_transformers.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/mixins/__init__.py
+-rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/mixins/test_runtime_parameters.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/pipeline/__init__.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/pipeline/conftest.py
+-rw-r--r--   0        0        0    44539 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/pipeline/test_base.py
+-rw-r--r--   0        0        0    17227 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/pipeline/test_dag.py
+-rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/pipeline/test_local.py
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/pipeline/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/__init__.py
+-rw-r--r--   0        0        0     9554 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/test_base.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/test_combine.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/test_conversation.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/test_decorator.py
+-rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/test_deita.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/test_expand.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/test_keep.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/argilla/__init__.py
+-rw-r--r--   0        0        0     5814 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/argilla/test_base.py
+-rw-r--r--   0        0        0     5725 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/argilla/test_preference.py
+-rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/argilla/test_text_generation.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/generators/test_data.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/__init__.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/conftest.py
+-rw-r--r--   0        0        0     6065 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/test_base.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/test_complexity_scorer.py
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/test_generate_embeddings.py
+-rw-r--r--   0        0        0     5289 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/test_instruction_backtranslation.py
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/test_pair_rm.py
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/test_quality_scorer.py
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/test_self_instruct.py
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/test_text_generation.py
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/test_ultrafeedback.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/evol_instruct/__init__.py
+-rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/evol_instruct/test_base.py
+-rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/evol_instruct/test_generator.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/__init__.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_base.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_generator.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/evol_quality/__init__.py
+-rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/steps/tasks/evol_quality/test_base.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/utils/__init__.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/utils/test_chat.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/utils/test_docstring.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/utils/test_lists.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 distilabel-1.0.1/tests/unit/utils/test_typing.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 distilabel-1.0.1/.gitignore
+-rw-r--r--   0        0        0    11355 2020-02-02 00:00:00.000000 distilabel-1.0.1/LICENSE
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 distilabel-1.0.1/LICENSE_HEADER
+-rw-r--r--   0        0        0     8989 2020-02-02 00:00:00.000000 distilabel-1.0.1/README.md
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 distilabel-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    12184 2020-02-02 00:00:00.000000 distilabel-1.0.1/PKG-INFO
```

### Comparing `distilabel-1.0.0/.pre-commit-config.yaml` & `distilabel-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/mkdocs.yml` & `distilabel-1.0.1/mkdocs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -132,23 +132,24 @@
           - "What Makes Good Data for Alignment? A Comprehensive Study of Automatic Data Selection in Instruction Tuning": "sections/papers/deita.md"
           - "Self-Alignment with Instruction Backtranslation": "sections/papers/instruction_backtranslation.md"
           - "UltraFeedback: Boosting Language Models with High-quality Feedback": "sections/papers/ultrafeedback.md"
   - API Reference:
       - Pipeline:
           - "api/pipeline/pipeline.md"
       - Steps:
-          - "api/steps/steps.md"
+          - "api/steps/index.md"
           - Generator Steps: "api/steps/generator_steps/generator_steps.md"
           - Global Steps: "api/steps/global_steps/global_steps.md"
           - Tasks:
               - "api/steps/tasks/text_generation.md"
               - "api/steps/tasks/preference_tasks.md"
               - "api/steps/tasks/embeddings.md"
           - "api/steps/decorator.md"
       - LLMs:
+          - "api/llms/index.md"
           - "api/llms/anthropic.md"
           - "api/llms/anyscale.md"
           - "api/llms/huggingface.md"
           - "api/llms/litellm.md"
           - "api/llms/llamacpp.md"
           - "api/llms/mistral.md"
           - "api/llms/ollama.md"
```

### Comparing `distilabel-1.0.0/.github/ISSUE_TEMPLATE/🆕-feature-request.md` & `distilabel-1.0.1/.github/ISSUE_TEMPLATE/🆕-feature-request.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/.github/ISSUE_TEMPLATE/🐛-bug-report.md` & `distilabel-1.0.1/.github/ISSUE_TEMPLATE/🐛-bug-report.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/.github/ISSUE_TEMPLATE/📚-documentation-update.md` & `distilabel-1.0.1/.github/ISSUE_TEMPLATE/📚-documentation-update.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/.github/workflows/docs.yml` & `distilabel-1.0.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/.github/workflows/release.yml` & `distilabel-1.0.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/.github/workflows/test.yml` & `distilabel-1.0.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/index.md` & `distilabel-1.0.1/docs/index.md`

 * *Files 11% similar despite different names*

```diff
@@ -30,38 +30,42 @@
 - `ollama`: for using [Ollama](https://ollama.com/) and their available models via `OllamaLLM` integration.
 - `openai`: for using [OpenAI API](https://openai.com/blog/openai-api) models via the `OpenAILLM` integration, or the rest of the integrations based on OpenAI and relying on its client as `AnyscaleLLM`, `AzureOpenAILLM`, and `TogetherLLM`.
 - `vertexai`: for using [Google Vertex AI](https://cloud.google.com/vertex-ai) proprietary models via the `VertexAILLM` integration.
 - `vllm`: for using [vllm](https://github.com/vllm-project/vllm) serving engine via the `vLLM` integration.
 
 ## Quick example
 
+To run the following example you must install `distilabel` with both `openai` extra:
+
+```sh
+pip install "distilabel[openai]" --upgrade
+```
+
+Then run:
+
 ```python
 from distilabel.llms import OpenAILLM
 from distilabel.pipeline import Pipeline
-from distilabel.steps import LoadHubDataset, TextGenerationToArgilla
+from distilabel.steps import LoadHubDataset
 from distilabel.steps.tasks import TextGeneration
 
 with Pipeline(
     name="simple-text-generation-pipeline",
     description="A simple text generation pipeline",
 ) as pipeline:
     load_dataset = LoadHubDataset(
         name="load_dataset",
         output_mappings={"prompt": "instruction"},
     )
 
     generate_with_openai = TextGeneration(
-        name="generate_with_gpt3.5", llm=OpenAILLM(model="gpt-3.5-turbo")
+        name="generate_with_gpt35", llm=OpenAILLM(model="gpt-3.5-turbo")
     )
 
-    to_argilla = TextGenerationToArgilla(name="to_argilla")
-
     load_dataset.connect(generate_with_openai)
-    generate_with_openai.connect(to_argilla)
-
 
 if __name__ == "__main__":
     distiset = pipeline.run(
         parameters={
             "load_dataset": {
                 "repo_id": "distilabel-internal-testing/instruction-dataset-mini",
                 "split": "test",
@@ -70,17 +74,10 @@
                 "llm": {
                     "generation_kwargs": {
                         "temperature": 0.7,
                         "max_new_tokens": 512,
                     }
                 }
             },
-            "to_argilla": {
-                "dataset_name": "text-generations-with-gpt35",
-                "dataset_workspace": "admin",
-            },
         },
     )
-    distiset.push_to_hub(
-        "distilabel-internal-testing/instruction-dataset-mini-with-generations"
-    )
 ```
```

### Comparing `distilabel-1.0.0/docs/api/steps/tasks/text_generation.md` & `distilabel-1.0.1/docs/api/steps/tasks/text_generation.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Tasks
 
+This section contains the API reference for the distilabel tasks. For an example on how to create and use a task, see the [Tutorial - Tasks](../../../sections/learn/tasks/index.md).
+
 ::: distilabel.steps.tasks.base
 
 ## General Text Generation
 
 ::: distilabel.steps.tasks.text_generation
 
 ## Evol Instruct
```

### Comparing `distilabel-1.0.0/docs/assets/distilabel-badge-dark.png` & `distilabel-1.0.1/docs/assets/distilabel-badge-dark.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/assets/distilabel-badge-light.png` & `distilabel-1.0.1/docs/assets/distilabel-badge-light.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/assets/distilabel-icon.svg` & `distilabel-1.0.1/docs/assets/distilabel-icon.svg`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/assets/logo.svg` & `distilabel-1.0.1/docs/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/assets/images/distilabel-diagram-dark.svg` & `distilabel-1.0.1/docs/assets/images/distilabel-diagram-dark.svg`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/assets/images/distilabel-diagram.svg` & `distilabel-1.0.1/docs/assets/images/distilabel-diagram.svg`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/assets/images/sections/caching/caching_pipe_1.png` & `distilabel-1.0.1/docs/assets/images/sections/caching/caching_pipe_1.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/assets/images/sections/caching/caching_pipe_2.png` & `distilabel-1.0.1/docs/assets/images/sections/caching/caching_pipe_2.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/assets/images/sections/caching/caching_pipe_3.png` & `distilabel-1.0.1/docs/assets/images/sections/caching/caching_pipe_3.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/assets/images/sections/caching/caching_pipe_4.png` & `distilabel-1.0.1/docs/assets/images/sections/caching/caching_pipe_4.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/assets/images/sections/cli/cli_pipe.png` & `distilabel-1.0.1/docs/assets/images/sections/cli/cli_pipe.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/assets/images/sections/learn/steps/argilla/preference.png` & `distilabel-1.0.1/docs/assets/images/sections/learn/steps/argilla/preference.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/assets/images/sections/learn/steps/argilla/text_generation.png` & `distilabel-1.0.1/docs/assets/images/sections/learn/steps/argilla/text_generation.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/assets/tutorials-assets/instrucion_dataset_notus_ui.png` & `distilabel-1.0.1/docs/assets/tutorials-assets/instrucion_dataset_notus_ui.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/assets/tutorials-assets/preference_dataset_notus_ui.png` & `distilabel-1.0.1/docs/assets/tutorials-assets/preference_dataset_notus_ui.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/assets/tutorials-assets/deita/datasets.png` & `distilabel-1.0.1/docs/assets/tutorials-assets/deita/datasets.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/assets/tutorials-assets/deita/diversity.png` & `distilabel-1.0.1/docs/assets/tutorials-assets/deita/diversity.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/assets/tutorials-assets/deita/overview.png` & `distilabel-1.0.1/docs/assets/tutorials-assets/deita/overview.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/assets/tutorials-assets/deita/results.png` & `distilabel-1.0.1/docs/assets/tutorials-assets/deita/results.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/scripts/gen_ref_pages.py` & `distilabel-1.0.1/docs/scripts/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/sections/learn/caching.md` & `distilabel-1.0.1/docs/sections/learn/caching.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/sections/learn/cli.md` & `distilabel-1.0.1/docs/sections/learn/cli.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/sections/learn/distiset.md` & `distilabel-1.0.1/docs/sections/learn/distiset.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/sections/learn/llms/index.md` & `distilabel-1.0.1/docs/sections/learn/llms/index.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/sections/learn/pipelines/index.md` & `distilabel-1.0.1/docs/sections/learn/pipelines/index.md`

 * *Files 1% similar despite different names*

```diff
@@ -107,33 +107,39 @@
 if __name__ == "__main__":
     distiset = pipeline.run(
         parameters={
             "load_dataset": {
                 "repo_id": "distilabel-internal-testing/instruction-dataset-mini",
                 "split": "test",
             },
-            "text_generation_with_openai-gpt-4-0125-preview": {
-                "generation_kwargs": {
-                    "temperature": 0.7,
-                    "max_new_tokens": 512,
+            "text_generation_with_gpt-4-0125-preview": {
+                "llm": {
+                    "generation_kwargs": {
+                        "temperature": 0.7,
+                        "max_new_tokens": 512,
+                    }
                 }
             },
             "text_generation_with_mistral-large-2402": {
-                "generation_kwargs": {
-                    "temperature": 0.7,
-                    "max_new_tokens": 512,
+                "llm": {
+                    "generation_kwargs": {
+                        "temperature": 0.7,
+                        "max_new_tokens": 512,
+                    }
                 }
             },
-            "text_generation_with_vertexai-gemini-1.5-pro": {
-                "generation_kwargs": {
-                    "temperature": 0.7,
-                    "max_new_tokens": 512,
+            "text_generation_with_gemini-1.0-pro": {
+                "llm": {
+                    "generation_kwargs": {
+                        "temperature": 0.7,
+                        "max_new_tokens": 512,
+                    }
                 }
             },
-        }
+        },
     )
 ```
 
 But if we run it, we will see that the `run` method will fail:
 
 ```
 ValueError: Step 'text_generation_with_gpt-4-0125-preview' requires inputs ['instruction'] which are not available when the step gets to be executed in the pipeline. Please make sure previous steps to 'text_generation_with_gpt-4-0125-preview' are 
@@ -272,29 +278,35 @@
         distiset = pipeline.run(
             parameters={
                 "load_dataset": {
                     "repo_id": "distilabel-internal-testing/instruction-dataset-mini",
                     "split": "test",
                 },
                 "text_generation_with_gpt-4-0125-preview": {
-                    "generation_kwargs": {
-                        "temperature": 0.7,
-                        "max_new_tokens": 512,
+                    "llm": {
+                        "generation_kwargs": {
+                            "temperature": 0.7,
+                            "max_new_tokens": 512,
+                        }
                     }
                 },
                 "text_generation_with_mistral-large-2402": {
-                    "generation_kwargs": {
-                        "temperature": 0.7,
-                        "max_new_tokens": 512,
+                    "llm": {
+                        "generation_kwargs": {
+                            "temperature": 0.7,
+                            "max_new_tokens": 512,
+                        }
                     }
                 },
                 "text_generation_with_gemini-1.0-pro": {
-                    "generation_kwargs": {
-                        "temperature": 0.7,
-                        "max_new_tokens": 512,
+                    "llm": {
+                        "generation_kwargs": {
+                            "temperature": 0.7,
+                            "max_new_tokens": 512,
+                        }
                     }
                 },
             },
         )
         distiset.push_to_hub(
             "distilabel-internal-testing/instruction-dataset-mini-with-generations"
         )
```

### Comparing `distilabel-1.0.0/docs/sections/learn/steps/argilla.md` & `distilabel-1.0.1/docs/sections/learn/steps/argilla.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/sections/learn/steps/general_steps.md` & `distilabel-1.0.1/docs/sections/learn/steps/general_steps.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/sections/learn/steps/generator_steps.md` & `distilabel-1.0.1/docs/sections/learn/steps/generator_steps.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/sections/learn/steps/global_steps.md` & `distilabel-1.0.1/docs/sections/learn/steps/global_steps.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/sections/learn/steps/index.md` & `distilabel-1.0.1/docs/sections/learn/steps/index.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/sections/learn/tasks/feedback_tasks.md` & `distilabel-1.0.1/docs/sections/learn/tasks/feedback_tasks.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/sections/learn/tasks/index.md` & `distilabel-1.0.1/docs/sections/learn/tasks/index.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/sections/learn/tasks/special_tasks.md` & `distilabel-1.0.1/docs/sections/learn/tasks/special_tasks.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/sections/learn/tasks/text_generation.md` & `distilabel-1.0.1/docs/sections/learn/tasks/text_generation.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/sections/papers/deita.md` & `distilabel-1.0.1/docs/sections/papers/deita.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/sections/papers/instruction_backtranslation.md` & `distilabel-1.0.1/docs/sections/papers/instruction_backtranslation.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/docs/sections/papers/ultrafeedback.md` & `distilabel-1.0.1/docs/sections/papers/ultrafeedback.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/__init__.py` & `distilabel-1.0.1/src/distilabel/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,10 +10,10 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from rich import traceback as rich_traceback
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 rich_traceback.install(show_locals=True)
```

### Comparing `distilabel-1.0.0/src/distilabel/__main__.py` & `distilabel-1.0.1/src/distilabel/__main__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/distiset.py` & `distilabel-1.0.1/src/distilabel/distiset.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/cli/__init__.py` & `distilabel-1.0.1/src/distilabel/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/cli/app.py` & `distilabel-1.0.1/src/distilabel/cli/app.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/cli/pipeline/__init__.py` & `distilabel-1.0.1/src/distilabel/cli/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/cli/pipeline/app.py` & `distilabel-1.0.1/src/distilabel/cli/pipeline/app.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/cli/pipeline/utils.py` & `distilabel-1.0.1/src/distilabel/cli/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/llms/__init__.py` & `distilabel-1.0.1/src/distilabel/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/llms/anthropic.py` & `distilabel-1.0.1/src/distilabel/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/llms/anyscale.py` & `distilabel-1.0.1/src/distilabel/llms/anyscale.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/llms/azure.py` & `distilabel-1.0.1/src/distilabel/llms/azure.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/llms/base.py` & `distilabel-1.0.1/src/distilabel/llms/base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/llms/chat_templates.py` & `distilabel-1.0.1/src/distilabel/llms/chat_templates.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/llms/cohere.py` & `distilabel-1.0.1/src/distilabel/llms/cohere.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/llms/litellm.py` & `distilabel-1.0.1/src/distilabel/llms/litellm.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/llms/llamacpp.py` & `distilabel-1.0.1/src/distilabel/llms/llamacpp.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/llms/mistral.py` & `distilabel-1.0.1/src/distilabel/llms/mistral.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/llms/mixins.py` & `distilabel-1.0.1/src/distilabel/llms/mixins.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/llms/ollama.py` & `distilabel-1.0.1/src/distilabel/llms/ollama.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/llms/openai.py` & `distilabel-1.0.1/src/distilabel/llms/openai.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/llms/together.py` & `distilabel-1.0.1/src/distilabel/llms/together.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/llms/typing.py` & `distilabel-1.0.1/src/distilabel/llms/typing.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/llms/vertexai.py` & `distilabel-1.0.1/src/distilabel/llms/vertexai.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/llms/vllm.py` & `distilabel-1.0.1/src/distilabel/llms/vllm.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/llms/huggingface/__init__.py` & `distilabel-1.0.1/src/distilabel/llms/huggingface/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/llms/huggingface/inference_endpoints.py` & `distilabel-1.0.1/src/distilabel/llms/huggingface/inference_endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,14 @@
         model_display_name: the model display name to use for the LLM. Defaults to `None`.
         use_openai_client: whether to use the OpenAI client instead of the Hugging Face client.
 
     Examples:
         ```python
         from distilabel.llms.huggingface import InferenceEndpointsLLM
 
-
         # Free serverless Inference API
         llm = InferenceEndpointsLLM(
             model_id="mistralai/Mistral-7B-Instruct-v0.2",
         )
 
         # Dedicated Inference Endpoints
         llm = InferenceEndpointsLLM(
@@ -119,29 +118,38 @@
     _api_key_env_var: str = PrivateAttr(_INFERENCE_ENDPOINTS_API_KEY_ENV_VAR_NAME)
     _aclient: Optional[Union["AsyncInferenceClient", "AsyncOpenAI"]] = PrivateAttr(...)
 
     @model_validator(mode="after")  # type: ignore
     def only_one_of_model_id_endpoint_name_or_base_url_provided(
         self,
     ) -> "InferenceEndpointsLLM":
-        """Validates that only one of `model_id`, `endpoint_name`, or `base_url` is provided."""
+        """Validates that only one of `model_id` or `endpoint_name` is provided; and if `base_url` is also
+        provided, a warning will be shown informing the user that the provided `base_url` will be ignored in
+        favour of the dynamically calculated one.."""
+
+        if self.base_url and (self.model_id or self.endpoint_name):
+            self._logger.warning(  # type: ignore
+                f"Since the `base_url={self.base_url}` is available and either one of `model_id` or `endpoint_name`"
+                " is also provided, the `base_url` will either be ignored or overwritten with the one generated"
+                " from either of those args, for serverless or dedicated inference endpoints, respectively."
+            )
 
-        if self.model_id and (not self.endpoint_name and not self.base_url):
+        if self.base_url and not (self.model_id or self.endpoint_name):
             return self
 
-        if self.endpoint_name and (not self.model_id and not self.base_url):
+        if self.model_id and not self.endpoint_name:
             return self
 
-        if self.base_url and (not self.model_id and not self.endpoint_name):
+        if self.endpoint_name and not self.model_id:
             return self
 
         raise ValidationError(
-            "Only one of `model_id`, `endpoint_name`, or `base_url` must be provided. Found"
-            f" `model_id`={self.model_id}, `endpoint_name`={self.endpoint_name}, and"
-            f" `base_url`={self.base_url}."
+            "Only one of `model_id` or `endpoint_name` must be provided. If `base_url` is provided too,"
+            " it will be overwritten instead. Found `model_id`={self.model_id}, `endpoint_name`={self.endpoint_name},"
+            f" and `base_url`={self.base_url}."
         )
 
     def load(self) -> None:  # noqa: C901
         """Loads the either the `AsyncInferenceClient` or the `AsyncOpenAI` client to benefit
         from async requests, running the Hugging Face Inference Endpoint underneath via the
         `/v1/chat/completions` endpoint, exposed for the models running on TGI using the
         `text-generation` task.
```

### Comparing `distilabel-1.0.0/src/distilabel/llms/huggingface/transformers.py` & `distilabel-1.0.1/src/distilabel/llms/huggingface/transformers.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/mixins/__init__.py` & `distilabel-1.0.1/src/distilabel/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/mixins/runtime_parameters.py` & `distilabel-1.0.1/src/distilabel/mixins/runtime_parameters.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/pipeline/__init__.py` & `distilabel-1.0.1/src/distilabel/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/pipeline/_dag.py` & `distilabel-1.0.1/src/distilabel/pipeline/_dag.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/pipeline/base.py` & `distilabel-1.0.1/src/distilabel/pipeline/base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/pipeline/local.py` & `distilabel-1.0.1/src/distilabel/pipeline/local.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/pipeline/utils.py` & `distilabel-1.0.1/src/distilabel/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/__init__.py` & `distilabel-1.0.1/src/distilabel/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/base.py` & `distilabel-1.0.1/src/distilabel/steps/base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/combine.py` & `distilabel-1.0.1/src/distilabel/steps/combine.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/conversation.py` & `distilabel-1.0.1/src/distilabel/steps/conversation.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/decorator.py` & `distilabel-1.0.1/src/distilabel/steps/decorator.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/deita.py` & `distilabel-1.0.1/src/distilabel/steps/deita.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/expand.py` & `distilabel-1.0.1/src/distilabel/steps/expand.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/keep.py` & `distilabel-1.0.1/src/distilabel/steps/keep.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/typing.py` & `distilabel-1.0.1/src/distilabel/steps/typing.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/argilla/__init__.py` & `distilabel-1.0.1/src/distilabel/steps/argilla/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/argilla/base.py` & `distilabel-1.0.1/src/distilabel/steps/argilla/base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/argilla/preference.py` & `distilabel-1.0.1/src/distilabel/steps/argilla/preference.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/argilla/text_generation.py` & `distilabel-1.0.1/src/distilabel/steps/argilla/text_generation.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/generators/__init__.py` & `distilabel-1.0.1/src/distilabel/steps/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/generators/data.py` & `distilabel-1.0.1/src/distilabel/steps/generators/data.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/generators/huggingface.py` & `distilabel-1.0.1/src/distilabel/steps/generators/huggingface.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/globals/__init__.py` & `distilabel-1.0.1/src/distilabel/steps/globals/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/globals/huggingface.py` & `distilabel-1.0.1/src/distilabel/steps/globals/huggingface.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/tasks/__init__.py` & `distilabel-1.0.1/src/distilabel/steps/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/tasks/base.py` & `distilabel-1.0.1/src/distilabel/steps/tasks/base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/tasks/complexity_scorer.py` & `distilabel-1.0.1/src/distilabel/steps/tasks/complexity_scorer.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/tasks/generate_embeddings.py` & `distilabel-1.0.1/src/distilabel/steps/tasks/generate_embeddings.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/tasks/instruction_backtranslation.py` & `distilabel-1.0.1/src/distilabel/steps/tasks/instruction_backtranslation.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/tasks/pair_rm.py` & `distilabel-1.0.1/src/distilabel/steps/tasks/pair_rm.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/tasks/quality_scorer.py` & `distilabel-1.0.1/src/distilabel/steps/tasks/quality_scorer.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/tasks/self_instruct.py` & `distilabel-1.0.1/src/distilabel/steps/tasks/self_instruct.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/tasks/text_generation.py` & `distilabel-1.0.1/src/distilabel/steps/tasks/text_generation.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/tasks/typing.py` & `distilabel-1.0.1/src/distilabel/steps/tasks/typing.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/tasks/ultrafeedback.py` & `distilabel-1.0.1/src/distilabel/steps/tasks/ultrafeedback.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/tasks/evol_instruct/__init__.py` & `distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/tasks/evol_instruct/base.py` & `distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/tasks/evol_instruct/english_nouns.txt` & `distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/english_nouns.txt`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/tasks/evol_instruct/generator.py` & `distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/generator.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/tasks/evol_instruct/utils.py` & `distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/tasks/evol_instruct/evol_complexity/__init__.py` & `distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/evol_complexity/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/tasks/evol_instruct/evol_complexity/base.py` & `distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/evol_complexity/base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/tasks/evol_instruct/evol_complexity/generator.py` & `distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/evol_complexity/generator.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/tasks/evol_instruct/evol_complexity/utils.py` & `distilabel-1.0.1/src/distilabel/steps/tasks/evol_instruct/evol_complexity/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/tasks/evol_quality/__init__.py` & `distilabel-1.0.1/src/distilabel/steps/tasks/evol_quality/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/tasks/evol_quality/base.py` & `distilabel-1.0.1/src/distilabel/steps/tasks/evol_quality/base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/tasks/evol_quality/utils.py` & `distilabel-1.0.1/src/distilabel/steps/tasks/evol_quality/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/tasks/templates/instruction-backtranslation.jinja2` & `distilabel-1.0.1/src/distilabel/steps/tasks/templates/instruction-backtranslation.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/tasks/templates/ultrafeedback/helpfulness.jinja2` & `distilabel-1.0.1/src/distilabel/steps/tasks/templates/ultrafeedback/helpfulness.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/tasks/templates/ultrafeedback/honesty.jinja2` & `distilabel-1.0.1/src/distilabel/steps/tasks/templates/ultrafeedback/honesty.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/tasks/templates/ultrafeedback/instruction-following.jinja2` & `distilabel-1.0.1/src/distilabel/steps/tasks/templates/ultrafeedback/instruction-following.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/tasks/templates/ultrafeedback/overall-rating.jinja2` & `distilabel-1.0.1/src/distilabel/steps/tasks/templates/ultrafeedback/overall-rating.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/steps/tasks/templates/ultrafeedback/truthfulness.jinja2` & `distilabel-1.0.1/src/distilabel/steps/tasks/templates/ultrafeedback/truthfulness.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/utils/__init__.py` & `distilabel-1.0.1/src/distilabel/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/utils/chat.py` & `distilabel-1.0.1/src/distilabel/utils/chat.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/utils/dicts.py` & `distilabel-1.0.1/src/distilabel/utils/dicts.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/utils/docstring.py` & `distilabel-1.0.1/src/distilabel/utils/docstring.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/utils/files.py` & `distilabel-1.0.1/src/distilabel/utils/files.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/utils/itertools.py` & `distilabel-1.0.1/src/distilabel/utils/itertools.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/utils/lists.py` & `distilabel-1.0.1/src/distilabel/utils/lists.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/utils/logging.py` & `distilabel-1.0.1/src/distilabel/utils/logging.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/utils/notebook.py` & `distilabel-1.0.1/src/distilabel/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/utils/serialization.py` & `distilabel-1.0.1/src/distilabel/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/utils/typing_.py` & `distilabel-1.0.1/src/distilabel/utils/typing_.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/utils/card/__init__.py` & `distilabel-1.0.1/src/distilabel/utils/card/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/utils/card/dataset_card.py` & `distilabel-1.0.1/src/distilabel/utils/card/dataset_card.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/src/distilabel/utils/card/distilabel_template.md` & `distilabel-1.0.1/src/distilabel/utils/card/distilabel_template.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/__init__.py` & `distilabel-1.0.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/integration/test_pipe_llms.py` & `distilabel-1.0.1/tests/integration/test_pipe_llms.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/integration/test_pipe_simple.py` & `distilabel-1.0.1/tests/integration/test_pipe_simple.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/__init__.py` & `distilabel-1.0.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/test_distiset.py` & `distilabel-1.0.1/tests/unit/test_distiset.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/test_imports.py` & `distilabel-1.0.1/tests/unit/test_imports.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/cli/__init__.py` & `distilabel-1.0.1/tests/unit/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/cli/test_pipeline.yaml` & `distilabel-1.0.1/tests/unit/cli/test_pipeline.yaml`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/cli/utils.py` & `distilabel-1.0.1/tests/unit/cli/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/cli/pipeline/__init__.py` & `distilabel-1.0.1/tests/unit/cli/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/cli/pipeline/test_app.py` & `distilabel-1.0.1/tests/unit/cli/pipeline/test_app.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/cli/pipeline/utils.py` & `distilabel-1.0.1/tests/unit/cli/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/llms/__init__.py` & `distilabel-1.0.1/tests/unit/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/llms/test_anthropic.py` & `distilabel-1.0.1/tests/unit/llms/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/llms/test_anyscale.py` & `distilabel-1.0.1/tests/unit/llms/test_anyscale.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/llms/test_azure.py` & `distilabel-1.0.1/tests/unit/llms/test_azure.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/llms/test_cohere.py` & `distilabel-1.0.1/tests/unit/llms/test_cohere.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/llms/test_litellm.py` & `distilabel-1.0.1/tests/unit/llms/test_litellm.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/llms/test_llamacpp.py` & `distilabel-1.0.1/tests/unit/llms/test_llamacpp.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/llms/test_mistral.py` & `distilabel-1.0.1/tests/unit/llms/test_mistral.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/llms/test_mixins.py` & `distilabel-1.0.1/tests/unit/llms/test_mixins.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/llms/test_ollama.py` & `distilabel-1.0.1/tests/unit/llms/test_ollama.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/llms/test_openai.py` & `distilabel-1.0.1/tests/unit/llms/test_openai.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/llms/test_together.py` & `distilabel-1.0.1/tests/unit/llms/test_together.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/llms/test_vertexai.py` & `distilabel-1.0.1/tests/unit/llms/test_vertexai.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/llms/huggingface/__init__.py` & `distilabel-1.0.1/tests/unit/llms/huggingface/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/llms/huggingface/test_inference_endpoints.py` & `distilabel-1.0.1/tests/unit/llms/huggingface/test_inference_endpoints.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/llms/huggingface/test_transformers.py` & `distilabel-1.0.1/tests/unit/llms/huggingface/test_transformers.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/mixins/__init__.py` & `distilabel-1.0.1/tests/unit/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/mixins/test_runtime_parameters.py` & `distilabel-1.0.1/tests/unit/mixins/test_runtime_parameters.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/pipeline/__init__.py` & `distilabel-1.0.1/tests/unit/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/pipeline/conftest.py` & `distilabel-1.0.1/tests/unit/pipeline/conftest.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/pipeline/test_base.py` & `distilabel-1.0.1/tests/unit/pipeline/test_base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/pipeline/test_dag.py` & `distilabel-1.0.1/tests/unit/pipeline/test_dag.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/pipeline/test_local.py` & `distilabel-1.0.1/tests/unit/pipeline/test_local.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/pipeline/utils.py` & `distilabel-1.0.1/tests/unit/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/steps/__init__.py` & `distilabel-1.0.1/tests/unit/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/steps/test_base.py` & `distilabel-1.0.1/tests/unit/steps/test_base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/steps/test_combine.py` & `distilabel-1.0.1/tests/unit/steps/test_combine.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/steps/test_conversation.py` & `distilabel-1.0.1/tests/unit/steps/test_conversation.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/steps/test_decorator.py` & `distilabel-1.0.1/tests/unit/steps/test_decorator.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/steps/test_deita.py` & `distilabel-1.0.1/tests/unit/steps/test_deita.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/steps/test_expand.py` & `distilabel-1.0.1/tests/unit/steps/test_expand.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/steps/test_keep.py` & `distilabel-1.0.1/tests/unit/steps/test_keep.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/steps/argilla/__init__.py` & `distilabel-1.0.1/tests/unit/steps/argilla/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/steps/argilla/test_base.py` & `distilabel-1.0.1/tests/unit/steps/argilla/test_base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/steps/argilla/test_preference.py` & `distilabel-1.0.1/tests/unit/steps/argilla/test_preference.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/steps/argilla/test_text_generation.py` & `distilabel-1.0.1/tests/unit/steps/argilla/test_text_generation.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/steps/generators/test_data.py` & `distilabel-1.0.1/tests/unit/steps/generators/test_data.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/steps/tasks/__init__.py` & `distilabel-1.0.1/tests/unit/steps/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/steps/tasks/conftest.py` & `distilabel-1.0.1/tests/unit/steps/tasks/conftest.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/steps/tasks/test_base.py` & `distilabel-1.0.1/tests/unit/steps/tasks/test_base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/steps/tasks/test_complexity_scorer.py` & `distilabel-1.0.1/tests/unit/steps/tasks/test_complexity_scorer.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/steps/tasks/test_generate_embeddings.py` & `distilabel-1.0.1/tests/unit/steps/tasks/test_generate_embeddings.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/steps/tasks/test_instruction_backtranslation.py` & `distilabel-1.0.1/tests/unit/steps/tasks/test_instruction_backtranslation.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/steps/tasks/test_pair_rm.py` & `distilabel-1.0.1/tests/unit/steps/tasks/test_pair_rm.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/steps/tasks/test_quality_scorer.py` & `distilabel-1.0.1/tests/unit/steps/tasks/test_quality_scorer.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/steps/tasks/test_self_instruct.py` & `distilabel-1.0.1/tests/unit/steps/tasks/test_self_instruct.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/steps/tasks/test_text_generation.py` & `distilabel-1.0.1/tests/unit/steps/tasks/test_text_generation.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/steps/tasks/test_ultrafeedback.py` & `distilabel-1.0.1/tests/unit/steps/tasks/test_ultrafeedback.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/steps/tasks/utils.py` & `distilabel-1.0.1/tests/unit/steps/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/steps/tasks/evol_instruct/__init__.py` & `distilabel-1.0.1/tests/unit/steps/tasks/evol_instruct/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/steps/tasks/evol_instruct/test_base.py` & `distilabel-1.0.1/tests/unit/steps/tasks/evol_instruct/test_base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/steps/tasks/evol_instruct/test_generator.py` & `distilabel-1.0.1/tests/unit/steps/tasks/evol_instruct/test_generator.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/__init__.py` & `distilabel-1.0.1/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_base.py` & `distilabel-1.0.1/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_generator.py` & `distilabel-1.0.1/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_generator.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/steps/tasks/evol_quality/__init__.py` & `distilabel-1.0.1/tests/unit/steps/tasks/evol_quality/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/steps/tasks/evol_quality/test_base.py` & `distilabel-1.0.1/tests/unit/steps/tasks/evol_quality/test_base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/utils/__init__.py` & `distilabel-1.0.1/tests/unit/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/utils/test_chat.py` & `distilabel-1.0.1/tests/unit/utils/test_chat.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/utils/test_docstring.py` & `distilabel-1.0.1/tests/unit/utils/test_docstring.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/utils/test_lists.py` & `distilabel-1.0.1/tests/unit/utils/test_lists.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/tests/unit/utils/test_typing.py` & `distilabel-1.0.1/tests/unit/utils/test_typing.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/.gitignore` & `distilabel-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/LICENSE` & `distilabel-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/LICENSE_HEADER` & `distilabel-1.0.1/LICENSE_HEADER`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/README.md` & `distilabel-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 <div align="center">
-  <h1>⚗️ distilabel</h1>
+  <picture>
+    <source media="(prefers-color-scheme: dark)" srcset="https://github.com/argilla-io/distilabel/blob/main/docs/assets/distilabel-white.png?raw=true">
+    <img alt="Distilabel Logo" src="https://raw.githubusercontent.com/argilla-io/distilabel/main/docs/assets/distilabel-black.png">
+  </picture>
 </div>
 <h3 align="center">Synthesize data for AI and add feedback on the fly!</h2>
 
 <p align="center">
 <a  href="https://pypi.org/project/distilabel/">
 <img alt="CI" src="https://img.shields.io/pypi/v/distilabel.svg?style=flat-round&logo=pypi&logoColor=white">
 </a>
@@ -84,46 +87,42 @@
 - `ollama`: for using [Ollama](https://ollama.com/) and their available models via `OllamaLLM` integration.
 - `openai`: for using [OpenAI API](https://openai.com/blog/openai-api) models via the `OpenAILLM` integration, or the rest of the integrations based on OpenAI and relying on its client as `AnyscaleLLM`, `AzureOpenAILLM`, and `TogetherLLM`.
 - `vertexai`: for using [Google Vertex AI](https://cloud.google.com/vertex-ai) proprietary models via the `VertexAILLM` integration.
 - `vllm`: for using [vllm](https://github.com/vllm-project/vllm) serving engine via the `vLLM` integration.
 
 ### Example
 
-To run the following example you must install `distilabel` with both `openai` and `argilla` extras:
+To run the following example you must install `distilabel` with both `openai` extra:
 
 ```sh
-pip install "distilabel[openai,argilla]" --upgrade
+pip install "distilabel[openai]" --upgrade
 ```
 
-Then run the following example:
+Then run:
 
 ```python
 from distilabel.llms import OpenAILLM
 from distilabel.pipeline import Pipeline
-from distilabel.steps import LoadHubDataset, TextGenerationToArgilla
+from distilabel.steps import LoadHubDataset
 from distilabel.steps.tasks import TextGeneration
 
 with Pipeline(
     name="simple-text-generation-pipeline",
     description="A simple text generation pipeline",
 ) as pipeline:
     load_dataset = LoadHubDataset(
         name="load_dataset",
         output_mappings={"prompt": "instruction"},
     )
 
     generate_with_openai = TextGeneration(
-        name="generate_with_gpt3.5", llm=OpenAILLM(model="gpt-3.5-turbo")
+        name="generate_with_gpt35", llm=OpenAILLM(model="gpt-3.5-turbo")
     )
 
-    to_argilla = TextGenerationToArgilla(name="to_argilla")
-
     load_dataset.connect(generate_with_openai)
-    generate_with_openai.connect(to_argilla)
-
 
 if __name__ == "__main__":
     distiset = pipeline.run(
         parameters={
             "load_dataset": {
                 "repo_id": "distilabel-internal-testing/instruction-dataset-mini",
                 "split": "test",
@@ -132,28 +131,18 @@
                 "llm": {
                     "generation_kwargs": {
                         "temperature": 0.7,
                         "max_new_tokens": 512,
                     }
                 }
             },
-            "to_argilla": {
-                "dataset_name": "text-generations-with-gpt35",
-                "dataset_workspace": "admin",
-            },
         },
     )
-    distiset.push_to_hub(
-        "distilabel-internal-testing/instruction-dataset-mini-with-generations"
-    )
 ```
 
-Distilabel integrates smoothly with Argilla and provides all the necessary configurations to make giving a final human touch as easy as possible.
-
-
 ## Badges
 
 If you build something cool with `distilabel` consider adding one of these badges to your dataset or model card.
 
     [<img src="https://raw.githubusercontent.com/argilla-io/distilabel/main/docs/assets/distilabel-badge-light.png" alt="Built with Distilabel" width="200" height="32"/>](https://github.com/argilla-io/distilabel)
 
 [<img src="https://raw.githubusercontent.com/argilla-io/distilabel/main/docs/assets/distilabel-badge-light.png" alt="Built with Distilabel" width="200" height="32"/>](https://github.com/argilla-io/distilabel)
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope__8j9xkut_/tmpx7m9wqpd_TarContainer/0/250.md", line 4, column 75: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-                        ************ ?â???ï?¸? ddiissttiillaabbeell ************
+                               [Distilabel Logo]
          ******** SSyynntthheessiizzee ddaattaa ffoorr AAII aanndd aadddd ffeeeeddbbaacckk oonn tthhee ffllyy!! ********
                                    _[_C_I_]_[_C_I_]
   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_t_w_i_t_t_e_r_-_b_l_a_c_k_?_l_o_g_o_=_x_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
     _b_a_d_g_e_/_l_i_n_k_e_d_i_n_-_b_l_u_e_?_l_o_g_o_=_l_i_n_k_e_d_i_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_s_l_a_c_k_-
                               _p_u_r_p_l_e_?_l_o_g_o_=_s_l_a_c_k_]
 Distilabel is the **framework for synthetic data and AI feedback for AI
 engineers** that require **high-quality outputs, full data ownership, and
@@ -68,35 +68,29 @@
 [OpenAI API](https://openai.com/blog/openai-api) models via the `OpenAILLM`
 integration, or the rest of the integrations based on OpenAI and relying on its
 client as `AnyscaleLLM`, `AzureOpenAILLM`, and `TogetherLLM`. - `vertexai`: for
 using [Google Vertex AI](https://cloud.google.com/vertex-ai) proprietary models
 via the `VertexAILLM` integration. - `vllm`: for using [vllm](https://
 github.com/vllm-project/vllm) serving engine via the `vLLM` integration. ###
 Example To run the following example you must install `distilabel` with both
-`openai` and `argilla` extras: ```sh pip install "distilabel[openai,argilla]" -
--upgrade ``` Then run the following example: ```python from distilabel.llms
-import OpenAILLM from distilabel.pipeline import Pipeline from distilabel.steps
-import LoadHubDataset, TextGenerationToArgilla from distilabel.steps.tasks
-import TextGeneration with Pipeline( name="simple-text-generation-pipeline",
-description="A simple text generation pipeline", ) as pipeline: load_dataset =
-LoadHubDataset( name="load_dataset", output_mappings={"prompt": "instruction"},
-) generate_with_openai = TextGeneration( name="generate_with_gpt3.5",
-llm=OpenAILLM(model="gpt-3.5-turbo") ) to_argilla = TextGenerationToArgilla
-(name="to_argilla") load_dataset.connect(generate_with_openai)
-generate_with_openai.connect(to_argilla) if __name__ == "__main__": distiset =
-pipeline.run( parameters={ "load_dataset": { "repo_id": "distilabel-internal-
+`openai` extra: ```sh pip install "distilabel[openai]" --upgrade ``` Then run:
+```python from distilabel.llms import OpenAILLM from distilabel.pipeline import
+Pipeline from distilabel.steps import LoadHubDataset from
+distilabel.steps.tasks import TextGeneration with Pipeline( name="simple-text-
+generation-pipeline", description="A simple text generation pipeline", ) as
+pipeline: load_dataset = LoadHubDataset( name="load_dataset", output_mappings=
+{"prompt": "instruction"}, ) generate_with_openai = TextGeneration
+( name="generate_with_gpt35", llm=OpenAILLM(model="gpt-3.5-turbo") )
+load_dataset.connect(generate_with_openai) if __name__ == "__main__": distiset
+= pipeline.run( parameters={ "load_dataset": { "repo_id": "distilabel-internal-
 testing/instruction-dataset-mini", "split": "test", }, "generate_with_gpt35":
 { "llm": { "generation_kwargs": { "temperature": 0.7, "max_new_tokens": 512, }
-} }, "to_argilla": { "dataset_name": "text-generations-with-gpt35",
-"dataset_workspace": "admin", }, }, ) distiset.push_to_hub( "distilabel-
-internal-testing/instruction-dataset-mini-with-generations" ) ``` Distilabel
-integrates smoothly with Argilla and provides all the necessary configurations
-to make giving a final human touch as easy as possible. ## Badges If you build
-something cool with `distilabel` consider adding one of these badges to your
-dataset or model card. [[Built with Distilabel]](https://github.com/argilla-io/
-distilabel) [[Built with Distilabel]](https://github.com/argilla-io/distilabel)
-[[Built with Distilabel]](https://github.com/argilla-io/distilabel) [[Built
-with Distilabel]](https://github.com/argilla-io/distilabel) ## Contribute To
+} }, }, ) ``` ## Badges If you build something cool with `distilabel` consider
+adding one of these badges to your dataset or model card. [[Built with
+Distilabel]](https://github.com/argilla-io/distilabel) [[Built with
+Distilabel]](https://github.com/argilla-io/distilabel) [[Built with
+Distilabel]](https://github.com/argilla-io/distilabel) [[Built with
+Distilabel]](https://github.com/argilla-io/distilabel) ## Contribute To
 directly contribute with `distilabel`, check our [good first issues](https://
 github.com/argilla-io/distilabel/
 issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22) or [open a new
 one](https://github.com/argilla-io/distilabel/issues/new/choose).
```

### Comparing `distilabel-1.0.0/pyproject.toml` & `distilabel-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.0/PKG-INFO` & `distilabel-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: distilabel
-Version: 1.0.0
+Version: 1.0.1
 Summary: AI Feedback (AIF) framework
 Project-URL: Documentation, https://distilabel.argilla.io/
 Project-URL: Issues, https://github.com/argilla/distilabel/issues
 Project-URL: Source, https://github.com/argilla/distilabel
 Author-email: Argilla <admin@argilla.io>
 License-Expression: MIT
 License-File: LICENSE
@@ -73,15 +73,18 @@
 Requires-Dist: google-cloud-aiplatform>=1.38.0; extra == 'vertexai'
 Provides-Extra: vllm
 Requires-Dist: filelock>=3.13.4; extra == 'vllm'
 Requires-Dist: vllm>=0.2.1; extra == 'vllm'
 Description-Content-Type: text/markdown
 
 <div align="center">
-  <h1>⚗️ distilabel</h1>
+  <picture>
+    <source media="(prefers-color-scheme: dark)" srcset="https://github.com/argilla-io/distilabel/blob/main/docs/assets/distilabel-white.png?raw=true">
+    <img alt="Distilabel Logo" src="https://raw.githubusercontent.com/argilla-io/distilabel/main/docs/assets/distilabel-black.png">
+  </picture>
 </div>
 <h3 align="center">Synthesize data for AI and add feedback on the fly!</h2>
 
 <p align="center">
 <a  href="https://pypi.org/project/distilabel/">
 <img alt="CI" src="https://img.shields.io/pypi/v/distilabel.svg?style=flat-round&logo=pypi&logoColor=white">
 </a>
@@ -162,46 +165,42 @@
 - `ollama`: for using [Ollama](https://ollama.com/) and their available models via `OllamaLLM` integration.
 - `openai`: for using [OpenAI API](https://openai.com/blog/openai-api) models via the `OpenAILLM` integration, or the rest of the integrations based on OpenAI and relying on its client as `AnyscaleLLM`, `AzureOpenAILLM`, and `TogetherLLM`.
 - `vertexai`: for using [Google Vertex AI](https://cloud.google.com/vertex-ai) proprietary models via the `VertexAILLM` integration.
 - `vllm`: for using [vllm](https://github.com/vllm-project/vllm) serving engine via the `vLLM` integration.
 
 ### Example
 
-To run the following example you must install `distilabel` with both `openai` and `argilla` extras:
+To run the following example you must install `distilabel` with both `openai` extra:
 
 ```sh
-pip install "distilabel[openai,argilla]" --upgrade
+pip install "distilabel[openai]" --upgrade
 ```
 
-Then run the following example:
+Then run:
 
 ```python
 from distilabel.llms import OpenAILLM
 from distilabel.pipeline import Pipeline
-from distilabel.steps import LoadHubDataset, TextGenerationToArgilla
+from distilabel.steps import LoadHubDataset
 from distilabel.steps.tasks import TextGeneration
 
 with Pipeline(
     name="simple-text-generation-pipeline",
     description="A simple text generation pipeline",
 ) as pipeline:
     load_dataset = LoadHubDataset(
         name="load_dataset",
         output_mappings={"prompt": "instruction"},
     )
 
     generate_with_openai = TextGeneration(
-        name="generate_with_gpt3.5", llm=OpenAILLM(model="gpt-3.5-turbo")
+        name="generate_with_gpt35", llm=OpenAILLM(model="gpt-3.5-turbo")
     )
 
-    to_argilla = TextGenerationToArgilla(name="to_argilla")
-
     load_dataset.connect(generate_with_openai)
-    generate_with_openai.connect(to_argilla)
-
 
 if __name__ == "__main__":
     distiset = pipeline.run(
         parameters={
             "load_dataset": {
                 "repo_id": "distilabel-internal-testing/instruction-dataset-mini",
                 "split": "test",
@@ -210,28 +209,18 @@
                 "llm": {
                     "generation_kwargs": {
                         "temperature": 0.7,
                         "max_new_tokens": 512,
                     }
                 }
             },
-            "to_argilla": {
-                "dataset_name": "text-generations-with-gpt35",
-                "dataset_workspace": "admin",
-            },
         },
     )
-    distiset.push_to_hub(
-        "distilabel-internal-testing/instruction-dataset-mini-with-generations"
-    )
 ```
 
-Distilabel integrates smoothly with Argilla and provides all the necessary configurations to make giving a final human touch as easy as possible.
-
-
 ## Badges
 
 If you build something cool with `distilabel` consider adding one of these badges to your dataset or model card.
 
     [<img src="https://raw.githubusercontent.com/argilla-io/distilabel/main/docs/assets/distilabel-badge-light.png" alt="Built with Distilabel" width="200" height="32"/>](https://github.com/argilla-io/distilabel)
 
 [<img src="https://raw.githubusercontent.com/argilla-io/distilabel/main/docs/assets/distilabel-badge-light.png" alt="Built with Distilabel" width="200" height="32"/>](https://github.com/argilla-io/distilabel)
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope__8j9xkut_/tmpx7m9wqpd_TarContainer/0/252", line 82, column 75: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: distilabel Version: 1.0.0 Summary: AI Feedback
+Metadata-Version: 2.3 Name: distilabel Version: 1.0.1 Summary: AI Feedback
 (AIF) framework Project-URL: Documentation, https://distilabel.argilla.io/
 Project-URL: Issues, https://github.com/argilla/distilabel/issues Project-URL:
 Source, https://github.com/argilla/distilabel Author-email: Argilla
 argilla.io> License-Expression: MIT License-File: LICENSE License-File:
 LICENSE_HEADER Keywords: alignment,annotation,data,llm,rlaif,synthetic
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3.8 Classifier:
@@ -36,15 +36,15 @@
 ollama Requires-Dist: ollama>=0.1.7; extra == 'ollama' Provides-Extra: openai
 Requires-Dist: openai>=1.0.0; extra == 'openai' Provides-Extra: tests Requires-
 Dist: nest-asyncio; extra == 'tests' Requires-Dist: pytest-asyncio; extra ==
 'tests' Requires-Dist: pytest>=7.4.0; extra == 'tests' Provides-Extra: vertexai
 Requires-Dist: google-cloud-aiplatform>=1.38.0; extra == 'vertexai' Provides-
 Extra: vllm Requires-Dist: filelock>=3.13.4; extra == 'vllm' Requires-Dist:
 vllm>=0.2.1; extra == 'vllm' Description-Content-Type: text/markdown
-                        ************ ?â???ï?¸? ddiissttiillaabbeell ************
+                               [Distilabel Logo]
          ******** SSyynntthheessiizzee ddaattaa ffoorr AAII aanndd aadddd ffeeeeddbbaacckk oonn tthhee ffllyy!! ********
                                    _[_C_I_]_[_C_I_]
   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_t_w_i_t_t_e_r_-_b_l_a_c_k_?_l_o_g_o_=_x_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
     _b_a_d_g_e_/_l_i_n_k_e_d_i_n_-_b_l_u_e_?_l_o_g_o_=_l_i_n_k_e_d_i_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_s_l_a_c_k_-
                               _p_u_r_p_l_e_?_l_o_g_o_=_s_l_a_c_k_]
 Distilabel is the **framework for synthetic data and AI feedback for AI
 engineers** that require **high-quality outputs, full data ownership, and
@@ -110,35 +110,29 @@
 [OpenAI API](https://openai.com/blog/openai-api) models via the `OpenAILLM`
 integration, or the rest of the integrations based on OpenAI and relying on its
 client as `AnyscaleLLM`, `AzureOpenAILLM`, and `TogetherLLM`. - `vertexai`: for
 using [Google Vertex AI](https://cloud.google.com/vertex-ai) proprietary models
 via the `VertexAILLM` integration. - `vllm`: for using [vllm](https://
 github.com/vllm-project/vllm) serving engine via the `vLLM` integration. ###
 Example To run the following example you must install `distilabel` with both
-`openai` and `argilla` extras: ```sh pip install "distilabel[openai,argilla]" -
--upgrade ``` Then run the following example: ```python from distilabel.llms
-import OpenAILLM from distilabel.pipeline import Pipeline from distilabel.steps
-import LoadHubDataset, TextGenerationToArgilla from distilabel.steps.tasks
-import TextGeneration with Pipeline( name="simple-text-generation-pipeline",
-description="A simple text generation pipeline", ) as pipeline: load_dataset =
-LoadHubDataset( name="load_dataset", output_mappings={"prompt": "instruction"},
-) generate_with_openai = TextGeneration( name="generate_with_gpt3.5",
-llm=OpenAILLM(model="gpt-3.5-turbo") ) to_argilla = TextGenerationToArgilla
-(name="to_argilla") load_dataset.connect(generate_with_openai)
-generate_with_openai.connect(to_argilla) if __name__ == "__main__": distiset =
-pipeline.run( parameters={ "load_dataset": { "repo_id": "distilabel-internal-
+`openai` extra: ```sh pip install "distilabel[openai]" --upgrade ``` Then run:
+```python from distilabel.llms import OpenAILLM from distilabel.pipeline import
+Pipeline from distilabel.steps import LoadHubDataset from
+distilabel.steps.tasks import TextGeneration with Pipeline( name="simple-text-
+generation-pipeline", description="A simple text generation pipeline", ) as
+pipeline: load_dataset = LoadHubDataset( name="load_dataset", output_mappings=
+{"prompt": "instruction"}, ) generate_with_openai = TextGeneration
+( name="generate_with_gpt35", llm=OpenAILLM(model="gpt-3.5-turbo") )
+load_dataset.connect(generate_with_openai) if __name__ == "__main__": distiset
+= pipeline.run( parameters={ "load_dataset": { "repo_id": "distilabel-internal-
 testing/instruction-dataset-mini", "split": "test", }, "generate_with_gpt35":
 { "llm": { "generation_kwargs": { "temperature": 0.7, "max_new_tokens": 512, }
-} }, "to_argilla": { "dataset_name": "text-generations-with-gpt35",
-"dataset_workspace": "admin", }, }, ) distiset.push_to_hub( "distilabel-
-internal-testing/instruction-dataset-mini-with-generations" ) ``` Distilabel
-integrates smoothly with Argilla and provides all the necessary configurations
-to make giving a final human touch as easy as possible. ## Badges If you build
-something cool with `distilabel` consider adding one of these badges to your
-dataset or model card. [[Built with Distilabel]](https://github.com/argilla-io/
-distilabel) [[Built with Distilabel]](https://github.com/argilla-io/distilabel)
-[[Built with Distilabel]](https://github.com/argilla-io/distilabel) [[Built
-with Distilabel]](https://github.com/argilla-io/distilabel) ## Contribute To
+} }, }, ) ``` ## Badges If you build something cool with `distilabel` consider
+adding one of these badges to your dataset or model card. [[Built with
+Distilabel]](https://github.com/argilla-io/distilabel) [[Built with
+Distilabel]](https://github.com/argilla-io/distilabel) [[Built with
+Distilabel]](https://github.com/argilla-io/distilabel) [[Built with
+Distilabel]](https://github.com/argilla-io/distilabel) ## Contribute To
 directly contribute with `distilabel`, check our [good first issues](https://
 github.com/argilla-io/distilabel/
 issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22) or [open a new
 one](https://github.com/argilla-io/distilabel/issues/new/choose).
```

