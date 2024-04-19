# Comparing `tmp/newscatcherapi_python_sdk-6.0.3.tar.gz` & `tmp/newscatcherapi_python_sdk-6.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newscatcherapi_python_sdk-6.0.3.tar", max compression
+gzip compressed data, was "newscatcherapi_python_sdk-6.0.4.tar", max compression
```

## Comparing `newscatcherapi_python_sdk-6.0.3.tar` & `newscatcherapi_python_sdk-6.0.4.tar`

### file list

```diff
@@ -1,239 +1,239 @@
--rw-r--r--   0        0        0     1081 2024-04-15 17:14:53.857576 newscatcherapi_python_sdk-6.0.3/LICENSE
--rw-r--r--   0        0        0    75510 2024-04-15 17:18:13.390065 newscatcherapi_python_sdk-6.0.3/README.md
--rw-r--r--   0        0        0     1059 2024-04-15 17:18:13.390276 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/__init__.py
--rw-r--r--   0        0        0    77304 2024-04-15 17:18:13.390586 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/api_client.py
--rw-r--r--   0        0        0      663 2024-04-15 17:14:53.814746 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/api_response.py
--rw-r--r--   0        0        0      214 2024-04-15 17:14:53.814890 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/__init__.py
--rw-r--r--   0        0        0     1432 2024-04-15 17:14:53.815013 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/path_to_api.py
--rw-r--r--   0        0        0      248 2024-04-15 17:14:53.815202 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/paths/__init__.py
--rw-r--r--   0        0        0      197 2024-04-15 17:14:53.815333 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/paths/api_authors.py
--rw-r--r--   0        0        0      223 2024-04-15 17:14:53.815446 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/paths/api_latest_headlines.py
--rw-r--r--   0        0        0      194 2024-04-15 17:14:53.815563 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/paths/api_search.py
--rw-r--r--   0        0        0      216 2024-04-15 17:14:53.815683 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/paths/api_search_by_link.py
--rw-r--r--   0        0        0      217 2024-04-15 17:14:53.815806 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/paths/api_search_similar.py
--rw-r--r--   0        0        0      197 2024-04-15 17:14:53.815913 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/paths/api_sources.py
--rw-r--r--   0        0        0      212 2024-04-15 17:14:53.816025 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/paths/api_subscription.py
--rw-r--r--   0        0        0     1339 2024-04-15 17:14:53.816145 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tag_to_api.py
--rw-r--r--   0        0        0      507 2024-04-15 17:14:53.816302 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/__init__.py
--rw-r--r--   0        0        0      902 2024-04-15 17:14:53.816410 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/authors_api.py
--rw-r--r--   0        0        0      705 2024-04-15 17:14:53.816516 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/authors_api_raw.py
--rw-r--r--   0        0        0      961 2024-04-15 17:14:53.816626 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/latest_headlines_api.py
--rw-r--r--   0        0        0      731 2024-04-15 17:14:53.816733 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/latest_headlines_api_raw.py
--rw-r--r--   0        0        0      895 2024-04-15 17:14:53.816845 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/search_api.py
--rw-r--r--   0        0        0      702 2024-04-15 17:14:53.816950 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/search_api_raw.py
--rw-r--r--   0        0        0      932 2024-04-15 17:14:53.817060 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/search_link_api.py
--rw-r--r--   0        0        0      722 2024-04-15 17:14:53.817181 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/search_link_api_raw.py
--rw-r--r--   0        0        0      947 2024-04-15 17:14:53.817302 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/search_similar_api.py
--rw-r--r--   0        0        0      725 2024-04-15 17:14:53.817419 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/search_similar_api_raw.py
--rw-r--r--   0        0        0      902 2024-04-15 17:14:53.817524 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/sources_api.py
--rw-r--r--   0        0        0      705 2024-04-15 17:14:53.817634 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/sources_api_raw.py
--rw-r--r--   0        0        0      937 2024-04-15 17:14:53.817747 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/subscription_api.py
--rw-r--r--   0        0        0      720 2024-04-15 17:14:53.817867 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/subscription_api_raw.py
--rw-r--r--   0        0        0     2114 2024-04-15 17:14:53.817992 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/client.py
--rw-r--r--   0        0        0     2114 2024-04-15 17:14:53.818125 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/client.pyi
--rw-r--r--   0        0        0      950 2024-04-15 17:14:53.818250 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/client_custom.py
--rw-r--r--   0        0        0    18272 2024-04-15 17:18:13.390856 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/configuration.py
--rw-r--r--   0        0        0     7953 2024-04-15 17:14:53.818574 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/exceptions.py
--rw-r--r--   0        0        0     2274 2024-04-15 17:14:53.818717 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/exceptions_base.py
--rw-r--r--   0        0        0      355 2024-04-15 17:14:53.818935 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/__init__.py
--rw-r--r--   0        0        0     3747 2024-04-15 17:14:53.819072 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/additional_source_info.py
--rw-r--r--   0        0        0     3747 2024-04-15 17:14:53.819207 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/additional_source_info.pyi
--rw-r--r--   0        0        0    31468 2024-04-15 17:18:13.391130 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/author_search_request.py
--rw-r--r--   0        0        0    31152 2024-04-15 17:18:13.391406 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/author_search_request.pyi
--rw-r--r--   0        0        0     2575 2024-04-15 17:14:53.819638 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/authors_get_response.py
--rw-r--r--   0        0        0     2575 2024-04-15 17:14:53.819784 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/authors_get_response.pyi
--rw-r--r--   0        0        0     2577 2024-04-15 17:14:53.819936 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/authors_post_response.py
--rw-r--r--   0        0        0     2577 2024-04-15 17:14:53.820063 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/authors_post_response.pyi
--rw-r--r--   0        0        0     3902 2024-04-15 17:14:53.820192 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/cluster.py
--rw-r--r--   0        0        0     3902 2024-04-15 17:14:53.820315 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/cluster.pyi
--rw-r--r--   0        0        0     1483 2024-04-15 17:14:53.820452 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/cluster_articles.py
--rw-r--r--   0        0        0     1483 2024-04-15 17:14:53.820577 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/cluster_articles.pyi
--rw-r--r--   0        0        0     7566 2024-04-15 17:14:53.820718 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/clustering_search_response.py
--rw-r--r--   0        0        0     7566 2024-04-15 17:14:53.820856 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/clustering_search_response.pyi
--rw-r--r--   0        0        0    31356 2024-04-15 17:14:53.821010 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_author_search_response_article_result.py
--rw-r--r--   0        0        0    31356 2024-04-15 17:14:53.821176 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_author_search_response_article_result.pyi
--rw-r--r--   0        0        0     7190 2024-04-15 17:14:53.821335 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_author_search_response_failed_search_response.py
--rw-r--r--   0        0        0     7190 2024-04-15 17:14:53.821484 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_author_search_response_failed_search_response.pyi
--rw-r--r--   0        0        0     6467 2024-04-15 17:14:53.821621 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_author_search_response_search_response.py
--rw-r--r--   0        0        0     6467 2024-04-15 17:14:53.821766 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_author_search_response_search_response.pyi
--rw-r--r--   0        0        0     1561 2024-04-15 17:14:53.821896 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_author_search_response_search_response_articles.py
--rw-r--r--   0        0        0     1561 2024-04-15 17:14:53.822026 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_author_search_response_search_response_articles.pyi
--rw-r--r--   0        0        0    32982 2024-04-15 17:14:53.822180 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_more_like_this_response_article_result.py
--rw-r--r--   0        0        0    32982 2024-04-15 17:14:53.822359 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_more_like_this_response_article_result.pyi
--rw-r--r--   0        0        0     7191 2024-04-15 17:14:53.822515 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_more_like_this_response_failed_search_response.py
--rw-r--r--   0        0        0     7191 2024-04-15 17:14:53.822648 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_more_like_this_response_failed_search_response.pyi
--rw-r--r--   0        0        0     6468 2024-04-15 17:14:53.822785 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response.py
--rw-r--r--   0        0        0     6468 2024-04-15 17:14:53.822915 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response.pyi
--rw-r--r--   0        0        0     1561 2024-04-15 17:14:53.823030 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response_articles.py
--rw-r--r--   0        0        0     1561 2024-04-15 17:14:53.823157 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response_articles.pyi
--rw-r--r--   0        0        0     6406 2024-04-15 17:14:53.823288 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_search_response_search_response.py
--rw-r--r--   0        0        0     6406 2024-04-15 17:14:53.823406 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_search_response_search_response.pyi
--rw-r--r--   0        0        0     1549 2024-04-15 17:14:53.823525 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_search_response_search_response_articles.py
--rw-r--r--   0        0        0     1549 2024-04-15 17:14:53.823655 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_search_response_search_response_articles.pyi
--rw-r--r--   0        0        0     3525 2024-04-15 17:14:53.823783 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/http_validation_error.py
--rw-r--r--   0        0        0     3525 2024-04-15 17:14:53.823904 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/http_validation_error.pyi
--rw-r--r--   0        0        0     2429 2024-04-15 17:14:53.824028 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_get_response.py
--rw-r--r--   0        0        0     2429 2024-04-15 17:14:53.824139 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_get_response.pyi
--rw-r--r--   0        0        0     2431 2024-04-15 17:14:53.824258 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_post_response.py
--rw-r--r--   0        0        0     2431 2024-04-15 17:14:53.824381 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_post_response.pyi
--rw-r--r--   0        0        0    28236 2024-04-15 17:18:13.391685 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_request.py
--rw-r--r--   0        0        0    27920 2024-04-15 17:18:13.391954 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_request.pyi
--rw-r--r--   0        0        0     6233 2024-04-15 17:14:53.824809 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_response.py
--rw-r--r--   0        0        0     6233 2024-04-15 17:14:53.824930 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_response.pyi
--rw-r--r--   0        0        0     1515 2024-04-15 17:14:53.825034 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_response_articles.py
--rw-r--r--   0        0        0     1515 2024-04-15 17:14:53.825143 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_response_articles.pyi
--rw-r--r--   0        0        0    32225 2024-04-15 17:14:53.825269 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/more_like_this_request.py
--rw-r--r--   0        0        0    31830 2024-04-15 17:14:53.825416 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/more_like_this_request.pyi
--rw-r--r--   0        0        0     2465 2024-04-15 17:14:53.825541 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_get_response.py
--rw-r--r--   0        0        0     2465 2024-04-15 17:14:53.825653 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_get_response.pyi
--rw-r--r--   0        0        0     2467 2024-04-15 17:14:53.825775 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_post_response.py
--rw-r--r--   0        0        0     2467 2024-04-15 17:14:53.825877 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_post_response.pyi
--rw-r--r--   0        0        0    36733 2024-04-15 17:18:13.393918 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_request.py
--rw-r--r--   0        0        0    36417 2024-04-15 17:18:13.395611 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_request.pyi
--rw-r--r--   0        0        0     2589 2024-04-15 17:14:53.826283 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_similar_get_response.py
--rw-r--r--   0        0        0     2589 2024-04-15 17:14:53.826403 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_similar_get_response.pyi
--rw-r--r--   0        0        0     2591 2024-04-15 17:14:53.826518 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_similar_post_response.py
--rw-r--r--   0        0        0     2591 2024-04-15 17:14:53.826631 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_similar_post_response.pyi
--rw-r--r--   0        0        0     4688 2024-04-15 17:14:53.826748 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_url_request.py
--rw-r--r--   0        0        0     4530 2024-04-15 17:14:53.826871 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_url_request.pyi
--rw-r--r--   0        0        0     4012 2024-04-15 17:14:53.826972 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/similar_document.py
--rw-r--r--   0        0        0     4012 2024-04-15 17:14:53.827076 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/similar_document.pyi
--rw-r--r--   0        0        0     4460 2024-04-15 17:14:53.827191 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/source_info.py
--rw-r--r--   0        0        0     4460 2024-04-15 17:14:53.827313 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/source_info.pyi
--rw-r--r--   0        0        0     3881 2024-04-15 17:14:53.827424 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/source_response.py
--rw-r--r--   0        0        0     3881 2024-04-15 17:14:53.827546 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/source_response.pyi
--rw-r--r--   0        0        0     3437 2024-04-15 17:14:53.827665 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/source_response_sources.py
--rw-r--r--   0        0        0     3437 2024-04-15 17:14:53.827776 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/source_response_sources.pyi
--rw-r--r--   0        0        0     6829 2024-04-15 17:14:53.827889 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/sources_request.py
--rw-r--r--   0        0        0     6829 2024-04-15 17:14:53.828002 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/sources_request.pyi
--rw-r--r--   0        0        0     5882 2024-04-15 17:14:53.828117 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/subscription_response.py
--rw-r--r--   0        0        0     5882 2024-04-15 17:14:53.828229 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/subscription_response.pyi
--rw-r--r--   0        0        0     3626 2024-04-15 17:14:53.828343 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/validation_error.py
--rw-r--r--   0        0        0     3626 2024-04-15 17:14:53.828470 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/validation_error.pyi
--rw-r--r--   0        0        0     3408 2024-04-15 17:14:53.828574 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/validation_error_loc.py
--rw-r--r--   0        0        0     3408 2024-04-15 17:14:53.828676 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/validation_error_loc.pyi
--rw-r--r--   0        0        0     4137 2024-04-15 17:14:53.828797 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/models/__init__.py
--rw-r--r--   0        0        0    25039 2024-04-15 17:18:13.395926 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/operation_parameter_map.py
--rw-r--r--   0        0        0      582 2024-04-15 17:14:53.829074 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/__init__.py
--rw-r--r--   0        0        0      323 2024-04-15 17:14:53.829193 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_authors/__init__.py
--rw-r--r--   0        0        0    66916 2024-04-15 17:18:13.396293 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_authors/get.py
--rw-r--r--   0        0        0    66607 2024-04-15 17:18:13.396664 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_authors/get.pyi
--rw-r--r--   0        0        0    47473 2024-04-15 17:18:13.396987 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_authors/post.py
--rw-r--r--   0        0        0    47336 2024-04-15 17:18:13.397275 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_authors/post.pyi
--rw-r--r--   0        0        0      341 2024-04-15 17:14:53.830874 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_latest_headlines/__init__.py
--rw-r--r--   0        0        0    66032 2024-04-15 17:18:13.397593 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_latest_headlines/get.py
--rw-r--r--   0        0        0    65723 2024-04-15 17:18:13.397880 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_latest_headlines/get.pyi
--rw-r--r--   0        0        0    49192 2024-04-15 17:18:13.398145 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_latest_headlines/post.py
--rw-r--r--   0        0        0    49055 2024-04-15 17:18:13.398420 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_latest_headlines/post.pyi
--rw-r--r--   0        0        0      321 2024-04-15 17:14:53.832084 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search/__init__.py
--rw-r--r--   0        0        0    77343 2024-04-15 17:18:13.398812 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search/get.py
--rw-r--r--   0        0        0    77034 2024-04-15 17:18:13.399319 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search/get.pyi
--rw-r--r--   0        0        0    54404 2024-04-15 17:18:13.399637 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search/post.py
--rw-r--r--   0        0        0    54267 2024-04-15 17:18:13.399936 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search/post.pyi
--rw-r--r--   0        0        0      337 2024-04-15 17:14:53.832957 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_by_link/__init__.py
--rw-r--r--   0        0        0    19293 2024-04-15 17:14:53.833078 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_by_link/get.py
--rw-r--r--   0        0        0    19070 2024-04-15 17:14:53.833225 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_by_link/get.pyi
--rw-r--r--   0        0        0    17699 2024-04-15 17:14:53.833367 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_by_link/post.py
--rw-r--r--   0        0        0    17562 2024-04-15 17:14:53.835150 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_by_link/post.pyi
--rw-r--r--   0        0        0      337 2024-04-15 17:14:53.835338 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_similar/__init__.py
--rw-r--r--   0        0        0    67713 2024-04-15 17:14:53.835596 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_similar/get.py
--rw-r--r--   0        0        0    67361 2024-04-15 17:14:53.835865 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_similar/get.pyi
--rw-r--r--   0        0        0    47930 2024-04-15 17:14:53.836031 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_similar/post.py
--rw-r--r--   0        0        0    47793 2024-04-15 17:14:53.836857 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_similar/post.pyi
--rw-r--r--   0        0        0      323 2024-04-15 17:14:53.837014 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_sources/__init__.py
--rw-r--r--   0        0        0    22889 2024-04-15 17:14:53.837139 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_sources/get.py
--rw-r--r--   0        0        0    22752 2024-04-15 17:14:53.837285 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_sources/get.pyi
--rw-r--r--   0        0        0    19936 2024-04-15 17:14:53.837427 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_sources/post.py
--rw-r--r--   0        0        0    19799 2024-04-15 17:14:53.837562 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_sources/post.pyi
--rw-r--r--   0        0        0      333 2024-04-15 17:14:53.837697 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_subscription/__init__.py
--rw-r--r--   0        0        0    12067 2024-04-15 17:14:53.837806 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_subscription/get.py
--rw-r--r--   0        0        0    11930 2024-04-15 17:14:53.837986 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_subscription/get.pyi
--rw-r--r--   0        0        0    12093 2024-04-15 17:14:53.838240 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_subscription/post.py
--rw-r--r--   0        0        0    11956 2024-04-15 17:14:53.838448 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_subscription/post.pyi
--rw-r--r--   0        0        0        0 2024-04-15 17:14:53.838623 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/__init__.py
--rw-r--r--   0        0        0      987 2024-04-15 17:14:53.838734 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/additional_source_info.py
--rw-r--r--   0        0        0     4726 2024-04-15 17:18:13.400226 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/author_search_request.py
--rw-r--r--   0        0        0     1061 2024-04-15 17:14:53.838987 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/authors_get_response.py
--rw-r--r--   0        0        0     1062 2024-04-15 17:14:53.839092 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/authors_post_response.py
--rw-r--r--   0        0        0      995 2024-04-15 17:14:53.839196 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/cluster.py
--rw-r--r--   0        0        0      665 2024-04-15 17:14:53.839308 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/cluster_articles.py
--rw-r--r--   0        0        0     1336 2024-04-15 17:14:53.839415 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/clustering_search_response.py
--rw-r--r--   0        0        0     3052 2024-04-15 17:14:53.839522 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_author_search_response_article_result.py
--rw-r--r--   0        0        0     1542 2024-04-15 17:14:53.839632 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_author_search_response_failed_search_response.py
--rw-r--r--   0        0        0     1436 2024-04-15 17:14:53.839747 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_author_search_response_search_response.py
--rw-r--r--   0        0        0      704 2024-04-15 17:14:53.839863 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_author_search_response_search_response_articles.py
--rw-r--r--   0        0        0     3239 2024-04-15 17:14:53.839972 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_article_result.py
--rw-r--r--   0        0        0     1543 2024-04-15 17:14:53.840077 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_failed_search_response.py
--rw-r--r--   0        0        0     1437 2024-04-15 17:14:53.840183 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_search_response.py
--rw-r--r--   0        0        0      704 2024-04-15 17:14:53.840297 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_search_response_articles.py
--rw-r--r--   0        0        0     1411 2024-04-15 17:14:53.840402 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_search_response_search_response.py
--rw-r--r--   0        0        0      698 2024-04-15 17:14:53.840505 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_search_response_search_response_articles.py
--rw-r--r--   0        0        0      937 2024-04-15 17:14:53.840610 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/http_validation_error.py
--rw-r--r--   0        0        0      907 2024-04-15 17:14:53.840719 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/latest_headlines_get_response.py
--rw-r--r--   0        0        0      908 2024-04-15 17:14:53.840826 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/latest_headlines_post_response.py
--rw-r--r--   0        0        0     4897 2024-04-15 17:18:13.400461 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/latest_headlines_request.py
--rw-r--r--   0        0        0     1340 2024-04-15 17:14:53.841066 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/latest_headlines_response.py
--rw-r--r--   0        0        0      681 2024-04-15 17:14:53.841165 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/latest_headlines_response_articles.py
--rw-r--r--   0        0        0     4721 2024-04-15 17:14:53.841277 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/more_like_this_request.py
--rw-r--r--   0        0        0      952 2024-04-15 17:14:53.841381 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/search_get_response.py
--rw-r--r--   0        0        0      953 2024-04-15 17:14:53.841482 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/search_post_response.py
--rw-r--r--   0        0        0     5539 2024-04-15 17:18:13.400762 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/search_request.py
--rw-r--r--   0        0        0     1069 2024-04-15 17:14:53.841699 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/search_similar_get_response.py
--rw-r--r--   0        0        0     1070 2024-04-15 17:14:53.841804 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/search_similar_post_response.py
--rw-r--r--   0        0        0     1151 2024-04-15 17:14:53.841902 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/search_url_request.py
--rw-r--r--   0        0        0      937 2024-04-15 17:14:53.842004 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/similar_document.py
--rw-r--r--   0        0        0     1132 2024-04-15 17:14:53.842116 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/source_info.py
--rw-r--r--   0        0        0     1093 2024-04-15 17:14:53.842221 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/source_response.py
--rw-r--r--   0        0        0      760 2024-04-15 17:14:53.842321 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/source_response_sources.py
--rw-r--r--   0        0        0     1432 2024-04-15 17:14:53.842420 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/sources_request.py
--rw-r--r--   0        0        0     1216 2024-04-15 17:14:53.842520 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/subscription_response.py
--rw-r--r--   0        0        0      973 2024-04-15 17:14:53.842622 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/validation_error.py
--rw-r--r--   0        0        0      684 2024-04-15 17:14:53.842723 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/validation_error_loc.py
--rw-r--r--   0        0        0      913 2024-04-15 17:14:53.842835 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/request_after_hook.py
--rw-r--r--   0        0        0      971 2024-04-15 17:14:53.842937 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/request_before_hook.py
--rw-r--r--   0        0        0      936 2024-04-15 17:14:53.843037 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/request_before_url_hook.py
--rw-r--r--   0        0        0    11233 2024-04-15 17:14:53.843143 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/rest.py
--rw-r--r--   0        0        0    96391 2024-04-15 17:14:53.843395 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/schemas.py
--rw-r--r--   0        0        0        0 2024-04-15 17:14:53.843546 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/__init__.py
--rw-r--r--   0        0        0      842 2024-04-15 17:14:53.843655 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/additional_source_info.py
--rw-r--r--   0        0        0     2699 2024-04-15 17:18:13.401083 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/author_search_request.py
--rw-r--r--   0        0        0      992 2024-04-15 17:14:53.843869 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/authors_get_response.py
--rw-r--r--   0        0        0      993 2024-04-15 17:14:53.843982 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/authors_post_response.py
--rw-r--r--   0        0        0      862 2024-04-15 17:14:53.844086 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/cluster.py
--rw-r--r--   0        0        0      604 2024-04-15 17:14:53.844195 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/cluster_articles.py
--rw-r--r--   0        0        0     1106 2024-04-15 17:14:53.844317 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/clustering_search_response.py
--rw-r--r--   0        0        0     1778 2024-04-15 17:14:53.844424 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_author_search_response_article_result.py
--rw-r--r--   0        0        0     1341 2024-04-15 17:14:53.844534 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_author_search_response_failed_search_response.py
--rw-r--r--   0        0        0     1326 2024-04-15 17:14:53.844641 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_author_search_response_search_response.py
--rw-r--r--   0        0        0      643 2024-04-15 17:14:53.844750 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_author_search_response_search_response_articles.py
--rw-r--r--   0        0        0     1903 2024-04-15 17:14:53.844857 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_more_like_this_response_article_result.py
--rw-r--r--   0        0        0     1342 2024-04-15 17:14:53.844980 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_more_like_this_response_failed_search_response.py
--rw-r--r--   0        0        0     1327 2024-04-15 17:14:53.845092 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_more_like_this_response_search_response.py
--rw-r--r--   0        0        0      643 2024-04-15 17:14:53.845204 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_more_like_this_response_search_response_articles.py
--rw-r--r--   0        0        0     1277 2024-04-15 17:14:53.845312 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_search_response_search_response.py
--rw-r--r--   0        0        0      637 2024-04-15 17:14:53.845423 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_search_response_search_response_articles.py
--rw-r--r--   0        0        0      889 2024-04-15 17:14:53.845526 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/http_validation_error.py
--rw-r--r--   0        0        0      838 2024-04-15 17:14:53.845628 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/latest_headlines_get_response.py
--rw-r--r--   0        0        0      839 2024-04-15 17:14:53.845736 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/latest_headlines_post_response.py
--rw-r--r--   0        0        0     2812 2024-04-15 17:18:13.401318 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/latest_headlines_request.py
--rw-r--r--   0        0        0     1138 2024-04-15 17:14:53.845939 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/latest_headlines_response.py
--rw-r--r--   0        0        0      620 2024-04-15 17:14:53.846038 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/latest_headlines_response_articles.py
--rw-r--r--   0        0        0     2616 2024-04-15 17:14:53.846135 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/more_like_this_request.py
--rw-r--r--   0        0        0      883 2024-04-15 17:14:53.846241 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/search_get_response.py
--rw-r--r--   0        0        0      884 2024-04-15 17:14:53.846342 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/search_post_response.py
--rw-r--r--   0        0        0     3031 2024-04-15 17:18:13.401517 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/search_request.py
--rw-r--r--   0        0        0     1000 2024-04-15 17:14:53.846554 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/search_similar_get_response.py
--rw-r--r--   0        0        0     1001 2024-04-15 17:14:53.846668 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/search_similar_post_response.py
--rw-r--r--   0        0        0      957 2024-04-15 17:14:53.846769 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/search_url_request.py
--rw-r--r--   0        0        0      836 2024-04-15 17:14:53.846875 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/similar_document.py
--rw-r--r--   0        0        0      904 2024-04-15 17:14:53.846974 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/source_info.py
--rw-r--r--   0        0        0      994 2024-04-15 17:14:53.847077 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/source_response.py
--rw-r--r--   0        0        0      695 2024-04-15 17:14:53.847175 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/source_response_sources.py
--rw-r--r--   0        0        0      996 2024-04-15 17:14:53.847270 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/sources_request.py
--rw-r--r--   0        0        0      925 2024-04-15 17:14:53.847369 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/subscription_response.py
--rw-r--r--   0        0        0      892 2024-04-15 17:14:53.847472 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/validation_error.py
--rw-r--r--   0        0        0      623 2024-04-15 17:14:53.847570 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/validation_error_loc.py
--rw-r--r--   0        0        0      758 2024-04-15 17:14:53.847687 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type_util.py
--rw-r--r--   0        0        0     3177 2024-04-15 17:14:53.847810 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/validation_metadata.py
--rw-r--r--   0        0        0      791 2024-04-15 17:18:13.401672 newscatcherapi_python_sdk-6.0.3/pyproject.toml
--rw-r--r--   0        0        0    76476 1970-01-01 00:00:00.000000 newscatcherapi_python_sdk-6.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-19 17:40:04.230921 newscatcherapi_python_sdk-6.0.4/LICENSE
+-rw-r--r--   0        0        0    75510 2024-04-19 17:53:34.550018 newscatcherapi_python_sdk-6.0.4/README.md
+-rw-r--r--   0        0        0     1059 2024-04-19 17:53:34.550527 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/__init__.py
+-rw-r--r--   0        0        0    77304 2024-04-19 17:53:34.550739 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/api_client.py
+-rw-r--r--   0        0        0      663 2024-04-19 17:40:04.188946 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/api_response.py
+-rw-r--r--   0        0        0      214 2024-04-19 17:40:04.189051 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/__init__.py
+-rw-r--r--   0        0        0     1432 2024-04-19 17:40:04.189144 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/path_to_api.py
+-rw-r--r--   0        0        0      248 2024-04-19 17:40:04.189238 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/paths/__init__.py
+-rw-r--r--   0        0        0      197 2024-04-19 17:40:04.189332 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/paths/api_authors.py
+-rw-r--r--   0        0        0      223 2024-04-19 17:40:04.189422 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/paths/api_latest_headlines.py
+-rw-r--r--   0        0        0      194 2024-04-19 17:40:04.189513 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/paths/api_search.py
+-rw-r--r--   0        0        0      216 2024-04-19 17:40:04.189603 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/paths/api_search_by_link.py
+-rw-r--r--   0        0        0      217 2024-04-19 17:40:04.189689 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/paths/api_search_similar.py
+-rw-r--r--   0        0        0      197 2024-04-19 17:40:04.189774 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/paths/api_sources.py
+-rw-r--r--   0        0        0      212 2024-04-19 17:40:04.189860 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/paths/api_subscription.py
+-rw-r--r--   0        0        0     1339 2024-04-19 17:40:04.189947 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tag_to_api.py
+-rw-r--r--   0        0        0      507 2024-04-19 17:40:04.190038 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/__init__.py
+-rw-r--r--   0        0        0      902 2024-04-19 17:40:04.190127 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/authors_api.py
+-rw-r--r--   0        0        0      705 2024-04-19 17:40:04.190213 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/authors_api_raw.py
+-rw-r--r--   0        0        0      961 2024-04-19 17:40:04.190302 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/latest_headlines_api.py
+-rw-r--r--   0        0        0      731 2024-04-19 17:40:04.190396 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/latest_headlines_api_raw.py
+-rw-r--r--   0        0        0      895 2024-04-19 17:40:04.190488 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/search_api.py
+-rw-r--r--   0        0        0      702 2024-04-19 17:40:04.190574 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/search_api_raw.py
+-rw-r--r--   0        0        0      932 2024-04-19 17:40:04.190662 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/search_link_api.py
+-rw-r--r--   0        0        0      722 2024-04-19 17:40:04.190759 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/search_link_api_raw.py
+-rw-r--r--   0        0        0      947 2024-04-19 17:40:04.191017 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/search_similar_api.py
+-rw-r--r--   0        0        0      725 2024-04-19 17:40:04.191118 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/search_similar_api_raw.py
+-rw-r--r--   0        0        0      902 2024-04-19 17:40:04.191214 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/sources_api.py
+-rw-r--r--   0        0        0      705 2024-04-19 17:40:04.191312 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/sources_api_raw.py
+-rw-r--r--   0        0        0      937 2024-04-19 17:40:04.191418 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/subscription_api.py
+-rw-r--r--   0        0        0      720 2024-04-19 17:40:04.191515 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/subscription_api_raw.py
+-rw-r--r--   0        0        0     2114 2024-04-19 17:40:04.191614 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/client.py
+-rw-r--r--   0        0        0     2114 2024-04-19 17:40:04.191708 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/client.pyi
+-rw-r--r--   0        0        0      950 2024-04-19 17:40:04.191800 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/client_custom.py
+-rw-r--r--   0        0        0    18272 2024-04-19 17:53:34.550892 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/configuration.py
+-rw-r--r--   0        0        0     7953 2024-04-19 17:40:04.192038 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/exceptions.py
+-rw-r--r--   0        0        0     2274 2024-04-19 17:40:04.192134 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/exceptions_base.py
+-rw-r--r--   0        0        0      355 2024-04-19 17:40:04.192269 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/__init__.py
+-rw-r--r--   0        0        0     3784 2024-04-19 17:53:34.551018 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/additional_source_info.py
+-rw-r--r--   0        0        0     3784 2024-04-19 17:53:34.551120 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/additional_source_info.pyi
+-rw-r--r--   0        0        0    31500 2024-04-19 17:53:34.551253 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/author_search_request.py
+-rw-r--r--   0        0        0    31184 2024-04-19 17:53:34.551385 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/author_search_request.pyi
+-rw-r--r--   0        0        0     2575 2024-04-19 17:40:04.192995 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/authors_get_response.py
+-rw-r--r--   0        0        0     2575 2024-04-19 17:40:04.193195 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/authors_get_response.pyi
+-rw-r--r--   0        0        0     2577 2024-04-19 17:40:04.193606 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/authors_post_response.py
+-rw-r--r--   0        0        0     2577 2024-04-19 17:40:04.193821 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/authors_post_response.pyi
+-rw-r--r--   0        0        0     3926 2024-04-19 17:53:34.551510 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/cluster.py
+-rw-r--r--   0        0        0     3926 2024-04-19 17:53:34.551640 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/cluster.pyi
+-rw-r--r--   0        0        0     1483 2024-04-19 17:40:04.194616 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/cluster_articles.py
+-rw-r--r--   0        0        0     1483 2024-04-19 17:40:04.195127 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/cluster_articles.pyi
+-rw-r--r--   0        0        0     7607 2024-04-19 17:53:34.551759 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/clustering_search_response.py
+-rw-r--r--   0        0        0     7607 2024-04-19 17:53:34.551864 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/clustering_search_response.pyi
+-rw-r--r--   0        0        0    31387 2024-04-19 17:53:34.552013 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_author_search_response_article_result.py
+-rw-r--r--   0        0        0    31387 2024-04-19 17:53:34.552136 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_author_search_response_article_result.pyi
+-rw-r--r--   0        0        0     7229 2024-04-19 17:53:34.552268 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_author_search_response_failed_search_response.py
+-rw-r--r--   0        0        0     7229 2024-04-19 17:53:34.552403 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_author_search_response_failed_search_response.pyi
+-rw-r--r--   0        0        0     6499 2024-04-19 17:53:34.552527 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_author_search_response_search_response.py
+-rw-r--r--   0        0        0     6499 2024-04-19 17:53:34.552640 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_author_search_response_search_response.pyi
+-rw-r--r--   0        0        0     1561 2024-04-19 17:40:04.198114 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_author_search_response_search_response_articles.py
+-rw-r--r--   0        0        0     1561 2024-04-19 17:40:04.198247 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_author_search_response_search_response_articles.pyi
+-rw-r--r--   0        0        0    33012 2024-04-19 17:53:34.552766 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_more_like_this_response_article_result.py
+-rw-r--r--   0        0        0    33012 2024-04-19 17:53:34.553052 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_more_like_this_response_article_result.pyi
+-rw-r--r--   0        0        0     7228 2024-04-19 17:53:34.553181 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_more_like_this_response_failed_search_response.py
+-rw-r--r--   0        0        0     7228 2024-04-19 17:53:34.553301 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_more_like_this_response_failed_search_response.pyi
+-rw-r--r--   0        0        0     6499 2024-04-19 17:53:34.553419 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response.py
+-rw-r--r--   0        0        0     6499 2024-04-19 17:53:34.553529 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response.pyi
+-rw-r--r--   0        0        0     1561 2024-04-19 17:40:04.199081 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response_articles.py
+-rw-r--r--   0        0        0     1561 2024-04-19 17:40:04.199176 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response_articles.pyi
+-rw-r--r--   0        0        0     6437 2024-04-19 17:53:34.553634 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_search_response_search_response.py
+-rw-r--r--   0        0        0     6437 2024-04-19 17:53:34.553734 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_search_response_search_response.pyi
+-rw-r--r--   0        0        0     1549 2024-04-19 17:40:04.200663 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_search_response_search_response_articles.py
+-rw-r--r--   0        0        0     1549 2024-04-19 17:40:04.201373 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_search_response_search_response_articles.pyi
+-rw-r--r--   0        0        0     3525 2024-04-19 17:40:04.202603 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/http_validation_error.py
+-rw-r--r--   0        0        0     3525 2024-04-19 17:40:04.203006 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/http_validation_error.pyi
+-rw-r--r--   0        0        0     2429 2024-04-19 17:40:04.203802 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_get_response.py
+-rw-r--r--   0        0        0     2429 2024-04-19 17:40:04.204002 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_get_response.pyi
+-rw-r--r--   0        0        0     2431 2024-04-19 17:40:04.205533 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_post_response.py
+-rw-r--r--   0        0        0     2431 2024-04-19 17:40:04.205813 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_post_response.pyi
+-rw-r--r--   0        0        0    28271 2024-04-19 17:53:34.553852 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_request.py
+-rw-r--r--   0        0        0    27955 2024-04-19 17:53:34.553982 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_request.pyi
+-rw-r--r--   0        0        0     6273 2024-04-19 17:53:34.554213 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_response.py
+-rw-r--r--   0        0        0     6273 2024-04-19 17:53:34.554310 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_response.pyi
+-rw-r--r--   0        0        0     1515 2024-04-19 17:40:04.206400 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_response_articles.py
+-rw-r--r--   0        0        0     1515 2024-04-19 17:40:04.206501 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_response_articles.pyi
+-rw-r--r--   0        0        0    32258 2024-04-19 17:53:34.554432 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/more_like_this_request.py
+-rw-r--r--   0        0        0    31863 2024-04-19 17:53:34.554559 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/more_like_this_request.pyi
+-rw-r--r--   0        0        0     2465 2024-04-19 17:40:04.206847 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_get_response.py
+-rw-r--r--   0        0        0     2465 2024-04-19 17:40:04.206937 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_get_response.pyi
+-rw-r--r--   0        0        0     2467 2024-04-19 17:40:04.207028 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_post_response.py
+-rw-r--r--   0        0        0     2467 2024-04-19 17:40:04.207123 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_post_response.pyi
+-rw-r--r--   0        0        0    36757 2024-04-19 17:53:34.554689 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_request.py
+-rw-r--r--   0        0        0    36441 2024-04-19 17:53:34.554831 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_request.pyi
+-rw-r--r--   0        0        0     2589 2024-04-19 17:40:04.207461 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_similar_get_response.py
+-rw-r--r--   0        0        0     2589 2024-04-19 17:40:04.207554 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_similar_get_response.pyi
+-rw-r--r--   0        0        0     2591 2024-04-19 17:40:04.207642 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_similar_post_response.py
+-rw-r--r--   0        0        0     2591 2024-04-19 17:40:04.207765 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_similar_post_response.pyi
+-rw-r--r--   0        0        0     4717 2024-04-19 17:53:34.554953 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_url_request.py
+-rw-r--r--   0        0        0     4559 2024-04-19 17:53:34.555058 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_url_request.pyi
+-rw-r--r--   0        0        0     4044 2024-04-19 17:53:34.555160 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/similar_document.py
+-rw-r--r--   0        0        0     4044 2024-04-19 17:53:34.555261 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/similar_document.pyi
+-rw-r--r--   0        0        0     4488 2024-04-19 17:53:34.555374 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/source_info.py
+-rw-r--r--   0        0        0     4488 2024-04-19 17:53:34.555471 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/source_info.pyi
+-rw-r--r--   0        0        0     3912 2024-04-19 17:53:34.555575 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/source_response.py
+-rw-r--r--   0        0        0     3912 2024-04-19 17:53:34.555667 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/source_response.pyi
+-rw-r--r--   0        0        0     3437 2024-04-19 17:40:04.208700 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/source_response_sources.py
+-rw-r--r--   0        0        0     3437 2024-04-19 17:40:04.208800 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/source_response_sources.pyi
+-rw-r--r--   0        0        0     6854 2024-04-19 17:53:34.555778 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/sources_request.py
+-rw-r--r--   0        0        0     6854 2024-04-19 17:53:34.555874 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/sources_request.pyi
+-rw-r--r--   0        0        0     5919 2024-04-19 17:53:34.555978 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/subscription_response.py
+-rw-r--r--   0        0        0     5919 2024-04-19 17:53:34.556077 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/subscription_response.pyi
+-rw-r--r--   0        0        0     3626 2024-04-19 17:40:04.209362 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/validation_error.py
+-rw-r--r--   0        0        0     3626 2024-04-19 17:40:04.209457 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/validation_error.pyi
+-rw-r--r--   0        0        0     3408 2024-04-19 17:40:04.209553 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/validation_error_loc.py
+-rw-r--r--   0        0        0     3408 2024-04-19 17:40:04.209653 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/validation_error_loc.pyi
+-rw-r--r--   0        0        0     4137 2024-04-19 17:40:04.209761 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/models/__init__.py
+-rw-r--r--   0        0        0    25039 2024-04-19 17:53:34.556234 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/operation_parameter_map.py
+-rw-r--r--   0        0        0      582 2024-04-19 17:40:04.210000 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/__init__.py
+-rw-r--r--   0        0        0      323 2024-04-19 17:40:04.210101 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_authors/__init__.py
+-rw-r--r--   0        0        0    66916 2024-04-19 17:53:34.556468 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_authors/get.py
+-rw-r--r--   0        0        0    66607 2024-04-19 17:53:34.557062 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_authors/get.pyi
+-rw-r--r--   0        0        0    47473 2024-04-19 17:53:34.557217 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_authors/post.py
+-rw-r--r--   0        0        0    47336 2024-04-19 17:53:34.557365 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_authors/post.pyi
+-rw-r--r--   0        0        0      341 2024-04-19 17:40:04.210787 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_latest_headlines/__init__.py
+-rw-r--r--   0        0        0    66032 2024-04-19 17:53:34.557727 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_latest_headlines/get.py
+-rw-r--r--   0        0        0    65723 2024-04-19 17:53:34.557902 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_latest_headlines/get.pyi
+-rw-r--r--   0        0        0    49192 2024-04-19 17:53:34.558070 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_latest_headlines/post.py
+-rw-r--r--   0        0        0    49055 2024-04-19 17:53:34.558264 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_latest_headlines/post.pyi
+-rw-r--r--   0        0        0      321 2024-04-19 17:40:04.211502 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search/__init__.py
+-rw-r--r--   0        0        0    77343 2024-04-19 17:53:34.558463 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search/get.py
+-rw-r--r--   0        0        0    77034 2024-04-19 17:53:34.558675 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search/get.pyi
+-rw-r--r--   0        0        0    54404 2024-04-19 17:53:34.558843 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search/post.py
+-rw-r--r--   0        0        0    54267 2024-04-19 17:53:34.559013 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search/post.pyi
+-rw-r--r--   0        0        0      337 2024-04-19 17:40:04.212230 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_by_link/__init__.py
+-rw-r--r--   0        0        0    19293 2024-04-19 17:40:04.212336 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_by_link/get.py
+-rw-r--r--   0        0        0    19070 2024-04-19 17:40:04.212460 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_by_link/get.pyi
+-rw-r--r--   0        0        0    17699 2024-04-19 17:40:04.212610 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_by_link/post.py
+-rw-r--r--   0        0        0    17562 2024-04-19 17:40:04.212731 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_by_link/post.pyi
+-rw-r--r--   0        0        0      337 2024-04-19 17:40:04.212849 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_similar/__init__.py
+-rw-r--r--   0        0        0    67713 2024-04-19 17:40:04.212991 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_similar/get.py
+-rw-r--r--   0        0        0    67361 2024-04-19 17:40:04.213152 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_similar/get.pyi
+-rw-r--r--   0        0        0    47930 2024-04-19 17:40:04.213293 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_similar/post.py
+-rw-r--r--   0        0        0    47793 2024-04-19 17:40:04.213423 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_similar/post.pyi
+-rw-r--r--   0        0        0      323 2024-04-19 17:40:04.213538 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_sources/__init__.py
+-rw-r--r--   0        0        0    22889 2024-04-19 17:40:04.213643 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_sources/get.py
+-rw-r--r--   0        0        0    22752 2024-04-19 17:40:04.213786 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_sources/get.pyi
+-rw-r--r--   0        0        0    19936 2024-04-19 17:40:04.214231 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_sources/post.py
+-rw-r--r--   0        0        0    19799 2024-04-19 17:40:04.214365 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_sources/post.pyi
+-rw-r--r--   0        0        0      333 2024-04-19 17:40:04.214491 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_subscription/__init__.py
+-rw-r--r--   0        0        0    12067 2024-04-19 17:40:04.214601 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_subscription/get.py
+-rw-r--r--   0        0        0    11930 2024-04-19 17:40:04.214745 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_subscription/get.pyi
+-rw-r--r--   0        0        0    12093 2024-04-19 17:40:04.214878 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_subscription/post.py
+-rw-r--r--   0        0        0    11956 2024-04-19 17:40:04.215531 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_subscription/post.pyi
+-rw-r--r--   0        0        0        0 2024-04-19 17:40:04.215957 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/__init__.py
+-rw-r--r--   0        0        0      987 2024-04-19 17:40:04.216048 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/additional_source_info.py
+-rw-r--r--   0        0        0     4726 2024-04-19 17:53:34.559173 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/author_search_request.py
+-rw-r--r--   0        0        0     1061 2024-04-19 17:40:04.216235 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/authors_get_response.py
+-rw-r--r--   0        0        0     1062 2024-04-19 17:40:04.216330 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/authors_post_response.py
+-rw-r--r--   0        0        0      995 2024-04-19 17:40:04.216415 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/cluster.py
+-rw-r--r--   0        0        0      665 2024-04-19 17:40:04.216499 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/cluster_articles.py
+-rw-r--r--   0        0        0     1336 2024-04-19 17:40:04.216592 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/clustering_search_response.py
+-rw-r--r--   0        0        0     3052 2024-04-19 17:40:04.216694 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_author_search_response_article_result.py
+-rw-r--r--   0        0        0     1542 2024-04-19 17:40:04.216809 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_author_search_response_failed_search_response.py
+-rw-r--r--   0        0        0     1436 2024-04-19 17:40:04.216907 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_author_search_response_search_response.py
+-rw-r--r--   0        0        0      704 2024-04-19 17:40:04.217000 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_author_search_response_search_response_articles.py
+-rw-r--r--   0        0        0     3239 2024-04-19 17:40:04.217091 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_article_result.py
+-rw-r--r--   0        0        0     1543 2024-04-19 17:40:04.217184 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_failed_search_response.py
+-rw-r--r--   0        0        0     1437 2024-04-19 17:40:04.217278 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_search_response.py
+-rw-r--r--   0        0        0      704 2024-04-19 17:40:04.217372 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_search_response_articles.py
+-rw-r--r--   0        0        0     1411 2024-04-19 17:40:04.217462 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_search_response_search_response.py
+-rw-r--r--   0        0        0      698 2024-04-19 17:40:04.217553 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_search_response_search_response_articles.py
+-rw-r--r--   0        0        0      937 2024-04-19 17:40:04.217648 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/http_validation_error.py
+-rw-r--r--   0        0        0      907 2024-04-19 17:40:04.217740 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/latest_headlines_get_response.py
+-rw-r--r--   0        0        0      908 2024-04-19 17:40:04.217825 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/latest_headlines_post_response.py
+-rw-r--r--   0        0        0     4897 2024-04-19 17:53:34.559286 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/latest_headlines_request.py
+-rw-r--r--   0        0        0     1340 2024-04-19 17:40:04.218013 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/latest_headlines_response.py
+-rw-r--r--   0        0        0      681 2024-04-19 17:40:04.218099 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/latest_headlines_response_articles.py
+-rw-r--r--   0        0        0     4721 2024-04-19 17:40:04.218191 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/more_like_this_request.py
+-rw-r--r--   0        0        0      952 2024-04-19 17:40:04.218275 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/search_get_response.py
+-rw-r--r--   0        0        0      953 2024-04-19 17:40:04.218368 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/search_post_response.py
+-rw-r--r--   0        0        0     5539 2024-04-19 17:53:34.559396 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/search_request.py
+-rw-r--r--   0        0        0     1069 2024-04-19 17:40:04.218549 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/search_similar_get_response.py
+-rw-r--r--   0        0        0     1070 2024-04-19 17:40:04.218635 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/search_similar_post_response.py
+-rw-r--r--   0        0        0     1151 2024-04-19 17:40:04.218724 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/search_url_request.py
+-rw-r--r--   0        0        0      937 2024-04-19 17:40:04.218812 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/similar_document.py
+-rw-r--r--   0        0        0     1132 2024-04-19 17:40:04.218895 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/source_info.py
+-rw-r--r--   0        0        0     1093 2024-04-19 17:40:04.218981 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/source_response.py
+-rw-r--r--   0        0        0      760 2024-04-19 17:40:04.219074 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/source_response_sources.py
+-rw-r--r--   0        0        0     1432 2024-04-19 17:40:04.219159 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/sources_request.py
+-rw-r--r--   0        0        0     1216 2024-04-19 17:40:04.219243 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/subscription_response.py
+-rw-r--r--   0        0        0      973 2024-04-19 17:40:04.219330 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/validation_error.py
+-rw-r--r--   0        0        0      684 2024-04-19 17:40:04.219432 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/validation_error_loc.py
+-rw-r--r--   0        0        0      913 2024-04-19 17:40:04.219528 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/request_after_hook.py
+-rw-r--r--   0        0        0      971 2024-04-19 17:40:04.219616 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/request_before_hook.py
+-rw-r--r--   0        0        0      936 2024-04-19 17:40:04.219710 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/request_before_url_hook.py
+-rw-r--r--   0        0        0    11233 2024-04-19 17:40:04.219818 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/rest.py
+-rw-r--r--   0        0        0    96391 2024-04-19 17:40:04.220036 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/schemas.py
+-rw-r--r--   0        0        0        0 2024-04-19 17:40:04.220150 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/__init__.py
+-rw-r--r--   0        0        0      842 2024-04-19 17:40:04.220245 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/additional_source_info.py
+-rw-r--r--   0        0        0     2699 2024-04-19 17:53:34.559523 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/author_search_request.py
+-rw-r--r--   0        0        0      992 2024-04-19 17:40:04.220450 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/authors_get_response.py
+-rw-r--r--   0        0        0      993 2024-04-19 17:40:04.220582 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/authors_post_response.py
+-rw-r--r--   0        0        0      862 2024-04-19 17:40:04.220720 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/cluster.py
+-rw-r--r--   0        0        0      604 2024-04-19 17:40:04.220873 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/cluster_articles.py
+-rw-r--r--   0        0        0     1106 2024-04-19 17:40:04.221004 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/clustering_search_response.py
+-rw-r--r--   0        0        0     1778 2024-04-19 17:40:04.221103 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_author_search_response_article_result.py
+-rw-r--r--   0        0        0     1341 2024-04-19 17:40:04.221202 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_author_search_response_failed_search_response.py
+-rw-r--r--   0        0        0     1326 2024-04-19 17:40:04.221302 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_author_search_response_search_response.py
+-rw-r--r--   0        0        0      643 2024-04-19 17:40:04.221400 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_author_search_response_search_response_articles.py
+-rw-r--r--   0        0        0     1903 2024-04-19 17:40:04.221494 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_more_like_this_response_article_result.py
+-rw-r--r--   0        0        0     1342 2024-04-19 17:40:04.221596 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_more_like_this_response_failed_search_response.py
+-rw-r--r--   0        0        0     1327 2024-04-19 17:40:04.221690 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_more_like_this_response_search_response.py
+-rw-r--r--   0        0        0      643 2024-04-19 17:40:04.221790 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_more_like_this_response_search_response_articles.py
+-rw-r--r--   0        0        0     1277 2024-04-19 17:40:04.221884 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_search_response_search_response.py
+-rw-r--r--   0        0        0      637 2024-04-19 17:40:04.221980 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_search_response_search_response_articles.py
+-rw-r--r--   0        0        0      889 2024-04-19 17:40:04.222070 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/http_validation_error.py
+-rw-r--r--   0        0        0      838 2024-04-19 17:40:04.222159 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/latest_headlines_get_response.py
+-rw-r--r--   0        0        0      839 2024-04-19 17:40:04.222247 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/latest_headlines_post_response.py
+-rw-r--r--   0        0        0     2812 2024-04-19 17:53:34.559640 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/latest_headlines_request.py
+-rw-r--r--   0        0        0     1138 2024-04-19 17:40:04.222498 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/latest_headlines_response.py
+-rw-r--r--   0        0        0      620 2024-04-19 17:40:04.222605 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/latest_headlines_response_articles.py
+-rw-r--r--   0        0        0     2616 2024-04-19 17:40:04.222814 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/more_like_this_request.py
+-rw-r--r--   0        0        0      883 2024-04-19 17:40:04.222912 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/search_get_response.py
+-rw-r--r--   0        0        0      884 2024-04-19 17:40:04.223013 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/search_post_response.py
+-rw-r--r--   0        0        0     3031 2024-04-19 17:53:34.559747 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/search_request.py
+-rw-r--r--   0        0        0     1000 2024-04-19 17:40:04.223198 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/search_similar_get_response.py
+-rw-r--r--   0        0        0     1001 2024-04-19 17:40:04.223427 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/search_similar_post_response.py
+-rw-r--r--   0        0        0      957 2024-04-19 17:40:04.223520 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/search_url_request.py
+-rw-r--r--   0        0        0      836 2024-04-19 17:40:04.223627 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/similar_document.py
+-rw-r--r--   0        0        0      904 2024-04-19 17:40:04.223710 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/source_info.py
+-rw-r--r--   0        0        0      994 2024-04-19 17:40:04.223795 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/source_response.py
+-rw-r--r--   0        0        0      695 2024-04-19 17:40:04.223883 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/source_response_sources.py
+-rw-r--r--   0        0        0      996 2024-04-19 17:40:04.223964 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/sources_request.py
+-rw-r--r--   0        0        0      925 2024-04-19 17:40:04.224045 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/subscription_response.py
+-rw-r--r--   0        0        0      892 2024-04-19 17:40:04.224127 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/validation_error.py
+-rw-r--r--   0        0        0      623 2024-04-19 17:40:04.224211 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/validation_error_loc.py
+-rw-r--r--   0        0        0      758 2024-04-19 17:40:04.224296 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type_util.py
+-rw-r--r--   0        0        0     3177 2024-04-19 17:40:04.224385 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/validation_metadata.py
+-rw-r--r--   0        0        0      791 2024-04-19 17:53:34.559852 newscatcherapi_python_sdk-6.0.4/pyproject.toml
+-rw-r--r--   0        0        0    76527 1970-01-01 00:00:00.000000 newscatcherapi_python_sdk-6.0.4/PKG-INFO
```

### Comparing `newscatcherapi_python_sdk-6.0.3/LICENSE` & `newscatcherapi_python_sdk-6.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/README.md` & `newscatcherapi_python_sdk-6.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # newscatcherapi-python-sdk<a id="newscatcherapi-python-sdk"></a>
 
 <img src='https://uploads-ssl.webflow.com/6429857b17973b636c2195c5/646c6f1eb774ff2f2997bec5_newscatcher_.svg' width='286' height='35' /> <br>  <br>Visit our website  <a href='https://newscatcherapi.com'>https://newscatcherapi.com</a>
 
 
-[![PyPI](https://img.shields.io/badge/PyPI-v6.0.3-blue)](https://pypi.org/project/newscatcherapi-python-sdk/6.0.3)
+[![PyPI](https://img.shields.io/badge/PyPI-v6.0.4-blue)](https://pypi.org/project/newscatcherapi-python-sdk/6.0.4)
 [![README.md](https://img.shields.io/badge/README-Click%20Here-green)](https://github.com/konfig-dev/newscatcher-sdks/tree/main/v3/python#readme)
 
 ## Table of Contents<a id="table-of-contents"></a>
 
 <!-- toc -->
 
 - [Requirements](#requirements)
@@ -36,15 +36,15 @@
 ## Requirements<a id="requirements"></a>
 
 Python >=3.7
 
 ## Installation<a id="installation"></a>
 
 ```sh
-pip install newscatcherapi-python-sdk==6.0.3
+pip install newscatcherapi-python-sdk==6.0.4
 ```
 
 ## Getting Started<a id="getting-started"></a>
 
 ```python
 from pprint import pprint
 from newscatcherapi_client import Newscatcher, ApiException
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/__init__.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     <img src='https://uploads-ssl.webflow.com/6429857b17973b636c2195c5/646c6f1eb774ff2f2997bec5_newscatcher_.svg' width='286' height='35' /> <br>  <br>Visit our website  <a href='https://newscatcherapi.com'>https://newscatcherapi.com</a>
 
     The version of the OpenAPI document: 3.2.16
     Contact: maksym@newscatcherapi.com
     Generated by: https://konfigthis.com
 """
 
-__version__ = "6.0.3"
+__version__ = "6.0.4"
 
 # import ApiClient
 from newscatcherapi_client.api_client import ApiClient
 
 # import Configuration
 from newscatcherapi_client.configuration import Configuration
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8 # flake8: noqa """ NewsCatcher-V3 Production API [https://
 uploads-ssl.webflow.com/6429857b17973b636c2195c5/
 646c6f1eb774ff2f2997bec5_newscatcher_.svg]
 
 Visit our website _h_t_t_p_s_:_/_/_n_e_w_s_c_a_t_c_h_e_r_a_p_i_._c_o_m The version of the OpenAPI
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
-konfigthis.com """ __version__ = "6.0.3" # import ApiClient from
+konfigthis.com """ __version__ = "6.0.4" # import ApiClient from
 newscatcherapi_client.api_client import ApiClient # import Configuration from
 newscatcherapi_client.configuration import Configuration # import exceptions
 from newscatcherapi_client.exceptions import OpenApiException from
 newscatcherapi_client.exceptions import ApiAttributeError from
 newscatcherapi_client.exceptions import ApiTypeError from
 newscatcherapi_client.exceptions import ApiValueError from
 newscatcherapi_client.exceptions import ApiKeyError from
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/api_client.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2984,15 +2984,15 @@
 0000ba70: 655d 203d 2068 6561 6465 725f 7661 6c75  e] = header_valu
 0000ba80: 650a 2020 2020 2020 2020 7365 6c66 2e63  e.        self.c
 0000ba90: 6f6f 6b69 6520 3d20 636f 6f6b 6965 0a20  ookie = cookie. 
 0000baa0: 2020 2020 2020 2023 2053 6574 2064 6566         # Set def
 0000bab0: 6175 6c74 2055 7365 722d 4167 656e 742e  ault User-Agent.
 0000bac0: 0a20 2020 2020 2020 2073 656c 662e 7573  .        self.us
 0000bad0: 6572 5f61 6765 6e74 203d 2027 4b6f 6e66  er_agent = 'Konf
-0000bae0: 6967 2f36 2e30 2e33 2f70 7974 686f 6e27  ig/6.0.3/python'
+0000bae0: 6967 2f36 2e30 2e34 2f70 7974 686f 6e27  ig/6.0.4/python'
 0000baf0: 0a0a 2020 2020 6465 6620 5f5f 656e 7465  ..    def __ente
 0000bb00: 725f 5f28 7365 6c66 293a 0a20 2020 2020  r__(self):.     
 0000bb10: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
 0000bb20: 2020 2020 6465 6620 5f5f 6578 6974 5f5f      def __exit__
 0000bb30: 2873 656c 662c 2065 7863 5f74 7970 652c  (self, exc_type,
 0000bb40: 2065 7863 5f76 616c 7565 2c20 7472 6163   exc_value, trac
 0000bb50: 6562 6163 6b29 3a0a 2020 2020 2020 2020  eback):.
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/api_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/api_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/path_to_api.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tag_to_api.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tag_to_api.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/authors_api.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/authors_api.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/authors_api_raw.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/authors_api_raw.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/latest_headlines_api.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/latest_headlines_api.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/latest_headlines_api_raw.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/latest_headlines_api_raw.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/search_api.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/search_api.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/search_api_raw.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/search_api_raw.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/search_link_api.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/search_link_api.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/search_link_api_raw.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/search_link_api_raw.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/search_similar_api.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/search_similar_api.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/search_similar_api_raw.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/search_similar_api_raw.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/sources_api.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/sources_api.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/sources_api_raw.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/sources_api_raw.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/subscription_api.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/subscription_api.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/subscription_api_raw.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/subscription_api_raw.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/client.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/client.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/client.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/client.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/client_custom.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/client_custom.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/configuration.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,15 +404,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 3.2.16\n"\
-               "SDK Package Version: 6.0.3".\
+               "SDK Package Version: 6.0.4".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/exceptions.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/exceptions_base.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/exceptions_base.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/additional_source_info.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/additional_source_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class AdditionalSourceInfo(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    AdditionalSourceInfo DTO class.
     """
 
 
     class MetaOapg:
         
         class properties:
             nb_articles_for_7d = schemas.IntSchema
```

#### html2text {}

```diff
@@ -6,19 +6,19 @@
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
 newscatcherapi_client import schemas # noqa: F401 class AdditionalSourceInfo
 ( schemas.DictSchema ): """ This class is auto generated by Konfig (https://
-konfigthis.com) """ class MetaOapg: class properties: nb_articles_for_7d =
-schemas.IntSchema country = schemas.StrSchema rank = schemas.IntSchema
-__annotations__ = { "nb_articles_for_7d": nb_articles_for_7d, "country":
-country, "rank": rank, } @typing.overload def __getitem__(self, name:
-typing_extensions.Literal["nb_articles_for_7d"]) -
+konfigthis.com) AdditionalSourceInfo DTO class. """ class MetaOapg: class
+properties: nb_articles_for_7d = schemas.IntSchema country = schemas.StrSchema
+rank = schemas.IntSchema __annotations__ = { "nb_articles_for_7d":
+nb_articles_for_7d, "country": country, "rank": rank, } @typing.overload def
+__getitem__(self, name: typing_extensions.Literal["nb_articles_for_7d"]) -
 > MetaOapg.properties.nb_articles_for_7d: ... @typing.overload def __getitem__
 (self, name: typing_extensions.Literal["country"]) -
 > MetaOapg.properties.country: ... @typing.overload def __getitem__(self, name:
 typing_extensions.Literal["rank"]) -> MetaOapg.properties.rank: ...
 @typing.overload def __getitem__(self, name: str) -
 > schemas.UnsetAnyTypeSchema: ... def __getitem__(self, name: typing.Union
 [typing_extensions.Literal["nb_articles_for_7d", "country", "rank", ], str]): #
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/additional_source_info.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/additional_source_info.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class AdditionalSourceInfo(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    AdditionalSourceInfo DTO class.
     """
 
 
     class MetaOapg:
         
         class properties:
             nb_articles_for_7d = schemas.IntSchema
```

#### html2text {}

```diff
@@ -6,19 +6,19 @@
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
 newscatcherapi_client import schemas # noqa: F401 class AdditionalSourceInfo
 ( schemas.DictSchema ): """ This class is auto generated by Konfig (https://
-konfigthis.com) """ class MetaOapg: class properties: nb_articles_for_7d =
-schemas.IntSchema country = schemas.StrSchema rank = schemas.IntSchema
-__annotations__ = { "nb_articles_for_7d": nb_articles_for_7d, "country":
-country, "rank": rank, } @typing.overload def __getitem__(self, name:
-typing_extensions.Literal["nb_articles_for_7d"]) -
+konfigthis.com) AdditionalSourceInfo DTO class. """ class MetaOapg: class
+properties: nb_articles_for_7d = schemas.IntSchema country = schemas.StrSchema
+rank = schemas.IntSchema __annotations__ = { "nb_articles_for_7d":
+nb_articles_for_7d, "country": country, "rank": rank, } @typing.overload def
+__getitem__(self, name: typing_extensions.Literal["nb_articles_for_7d"]) -
 > MetaOapg.properties.nb_articles_for_7d: ... @typing.overload def __getitem__
 (self, name: typing_extensions.Literal["country"]) -
 > MetaOapg.properties.country: ... @typing.overload def __getitem__(self, name:
 typing_extensions.Literal["rank"]) -> MetaOapg.properties.rank: ...
 @typing.overload def __getitem__(self, name: str) -
 > schemas.UnsetAnyTypeSchema: ... def __getitem__(self, name: typing.Union
 [typing_extensions.Literal["nb_articles_for_7d", "country", "rank", ], str]): #
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/author_search_request.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/author_search_request.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class AuthorSearchRequest(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    Author search request DTO.
     """
 
 
     class MetaOapg:
         required = {
             "author_name",
         }
@@ -137,45 +139,33 @@
             all_links = schemas.AnyTypeSchema
             all_domain_links = schemas.AnyTypeSchema
             
             
             class word_count_min(
                 schemas.IntSchema
             ):
-            
-            
-                class MetaOapg:
-                    inclusive_minimum = 0
+                pass
             
             
             class word_count_max(
                 schemas.IntSchema
             ):
-            
-            
-                class MetaOapg:
-                    inclusive_minimum = 0
+                pass
             
             
             class page(
                 schemas.IntSchema
             ):
-            
-            
-                class MetaOapg:
-                    inclusive_minimum = 0
+                pass
             
             
             class page_size(
                 schemas.IntSchema
             ):
-            
-            
-                class MetaOapg:
-                    inclusive_minimum = 0
+                pass
             include_nlp_data = schemas.BoolSchema
             has_nlp = schemas.BoolSchema
             theme = schemas.StrSchema
             not_theme = schemas.StrSchema
             ner_name = schemas.StrSchema
             title_sentiment_min = schemas.NumberSchema
             title_sentiment_max = schemas.NumberSchema
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/author_search_request.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/author_search_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class AuthorSearchRequest(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    Author search request DTO.
     """
 
 
     class MetaOapg:
         required = {
             "author_name",
         }
@@ -137,33 +139,45 @@
             all_links = schemas.AnyTypeSchema
             all_domain_links = schemas.AnyTypeSchema
             
             
             class word_count_min(
                 schemas.IntSchema
             ):
-                pass
+            
+            
+                class MetaOapg:
+                    inclusive_minimum = 0
             
             
             class word_count_max(
                 schemas.IntSchema
             ):
-                pass
+            
+            
+                class MetaOapg:
+                    inclusive_minimum = 0
             
             
             class page(
                 schemas.IntSchema
             ):
-                pass
+            
+            
+                class MetaOapg:
+                    inclusive_minimum = 0
             
             
             class page_size(
                 schemas.IntSchema
             ):
-                pass
+            
+            
+                class MetaOapg:
+                    inclusive_minimum = 0
             include_nlp_data = schemas.BoolSchema
             has_nlp = schemas.BoolSchema
             theme = schemas.StrSchema
             not_theme = schemas.StrSchema
             ner_name = schemas.StrSchema
             title_sentiment_min = schemas.NumberSchema
             title_sentiment_max = schemas.NumberSchema
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/authors_get_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/authors_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/authors_get_response.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/authors_get_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/authors_post_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/authors_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/authors_post_response.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/authors_post_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/cluster.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class Cluster(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    Cluster DTO class.
     """
 
 
     class MetaOapg:
         required = {
             "cluster_id",
             "cluster_size",
```

#### html2text {}

```diff
@@ -6,26 +6,27 @@
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
 newscatcherapi_client import schemas # noqa: F401 class Cluster
 ( schemas.DictSchema ): """ This class is auto generated by Konfig (https://
-konfigthis.com) """ class MetaOapg: required = { "cluster_id", "cluster_size",
-"articles", } class properties: cluster_id = schemas.StrSchema cluster_size =
-schemas.IntSchema @staticmethod def articles() -> typing.Type
-['ClusterArticles']: return ClusterArticles __annotations__ = { "cluster_id":
-cluster_id, "cluster_size": cluster_size, "articles": articles, } cluster_id:
-MetaOapg.properties.cluster_id cluster_size: MetaOapg.properties.cluster_size
-articles: 'ClusterArticles' @typing.overload def __getitem__(self, name:
-typing_extensions.Literal["cluster_id"]) -> MetaOapg.properties.cluster_id: ...
-@typing.overload def __getitem__(self, name: typing_extensions.Literal
-["cluster_size"]) -> MetaOapg.properties.cluster_size: ... @typing.overload def
-__getitem__(self, name: typing_extensions.Literal["articles"]) -
-> 'ClusterArticles': ... @typing.overload def __getitem__(self, name: str) -
+konfigthis.com) Cluster DTO class. """ class MetaOapg: required =
+{ "cluster_id", "cluster_size", "articles", } class properties: cluster_id =
+schemas.StrSchema cluster_size = schemas.IntSchema @staticmethod def articles()
+-> typing.Type['ClusterArticles']: return ClusterArticles __annotations__ =
+{ "cluster_id": cluster_id, "cluster_size": cluster_size, "articles": articles,
+} cluster_id: MetaOapg.properties.cluster_id cluster_size:
+MetaOapg.properties.cluster_size articles: 'ClusterArticles' @typing.overload
+def __getitem__(self, name: typing_extensions.Literal["cluster_id"]) -
+> MetaOapg.properties.cluster_id: ... @typing.overload def __getitem__(self,
+name: typing_extensions.Literal["cluster_size"]) -
+> MetaOapg.properties.cluster_size: ... @typing.overload def __getitem__(self,
+name: typing_extensions.Literal["articles"]) -> 'ClusterArticles': ...
+@typing.overload def __getitem__(self, name: str) -
 > schemas.UnsetAnyTypeSchema: ... def __getitem__(self, name: typing.Union
 [typing_extensions.Literal["cluster_id", "cluster_size", "articles", ], str]):
 # dict_instance[name] accessor return super().__getitem__(name)
 @typing.overload def get_item_oapg(self, name: typing_extensions.Literal
 ["cluster_id"]) -> MetaOapg.properties.cluster_id: ... @typing.overload def
 get_item_oapg(self, name: typing_extensions.Literal["cluster_size"]) -
 > MetaOapg.properties.cluster_size: ... @typing.overload def get_item_oapg
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/cluster.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/cluster.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class Cluster(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    Cluster DTO class.
     """
 
 
     class MetaOapg:
         required = {
             "cluster_id",
             "cluster_size",
```

#### html2text {}

```diff
@@ -6,26 +6,27 @@
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
 newscatcherapi_client import schemas # noqa: F401 class Cluster
 ( schemas.DictSchema ): """ This class is auto generated by Konfig (https://
-konfigthis.com) """ class MetaOapg: required = { "cluster_id", "cluster_size",
-"articles", } class properties: cluster_id = schemas.StrSchema cluster_size =
-schemas.IntSchema @staticmethod def articles() -> typing.Type
-['ClusterArticles']: return ClusterArticles __annotations__ = { "cluster_id":
-cluster_id, "cluster_size": cluster_size, "articles": articles, } cluster_id:
-MetaOapg.properties.cluster_id cluster_size: MetaOapg.properties.cluster_size
-articles: 'ClusterArticles' @typing.overload def __getitem__(self, name:
-typing_extensions.Literal["cluster_id"]) -> MetaOapg.properties.cluster_id: ...
-@typing.overload def __getitem__(self, name: typing_extensions.Literal
-["cluster_size"]) -> MetaOapg.properties.cluster_size: ... @typing.overload def
-__getitem__(self, name: typing_extensions.Literal["articles"]) -
-> 'ClusterArticles': ... @typing.overload def __getitem__(self, name: str) -
+konfigthis.com) Cluster DTO class. """ class MetaOapg: required =
+{ "cluster_id", "cluster_size", "articles", } class properties: cluster_id =
+schemas.StrSchema cluster_size = schemas.IntSchema @staticmethod def articles()
+-> typing.Type['ClusterArticles']: return ClusterArticles __annotations__ =
+{ "cluster_id": cluster_id, "cluster_size": cluster_size, "articles": articles,
+} cluster_id: MetaOapg.properties.cluster_id cluster_size:
+MetaOapg.properties.cluster_size articles: 'ClusterArticles' @typing.overload
+def __getitem__(self, name: typing_extensions.Literal["cluster_id"]) -
+> MetaOapg.properties.cluster_id: ... @typing.overload def __getitem__(self,
+name: typing_extensions.Literal["cluster_size"]) -
+> MetaOapg.properties.cluster_size: ... @typing.overload def __getitem__(self,
+name: typing_extensions.Literal["articles"]) -> 'ClusterArticles': ...
+@typing.overload def __getitem__(self, name: str) -
 > schemas.UnsetAnyTypeSchema: ... def __getitem__(self, name: typing.Union
 [typing_extensions.Literal["cluster_id", "cluster_size", "articles", ], str]):
 # dict_instance[name] accessor return super().__getitem__(name)
 @typing.overload def get_item_oapg(self, name: typing_extensions.Literal
 ["cluster_id"]) -> MetaOapg.properties.cluster_id: ... @typing.overload def
 get_item_oapg(self, name: typing_extensions.Literal["cluster_size"]) -
 > MetaOapg.properties.cluster_size: ... @typing.overload def get_item_oapg
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/cluster_articles.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/cluster_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/cluster_articles.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/cluster_articles.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/clustering_search_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/clustering_search_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class ClusteringSearchResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    ClusteringSearchResponse DTO class.
     """
 
 
     class MetaOapg:
         required = {
             "total_hits",
             "user_input",
```

#### html2text {}

```diff
@@ -6,41 +6,41 @@
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
 newscatcherapi_client import schemas # noqa: F401 class
 ClusteringSearchResponse( schemas.DictSchema ): """ This class is auto
-generated by Konfig (https://konfigthis.com) """ class MetaOapg: required =
-{ "total_hits", "user_input", "page", "total_pages", "clusters_count",
-"clusters", "page_size", } class properties: total_hits = schemas.IntSchema
-page = schemas.IntSchema total_pages = schemas.IntSchema page_size =
-schemas.IntSchema clusters_count = schemas.IntSchema class clusters
-( schemas.ListSchema ): class MetaOapg: @staticmethod def items() -
-> typing.Type['Cluster']: return Cluster def __new__( cls, arg: typing.Union
-[typing.Tuple['Cluster'], typing.List['Cluster']], _configuration:
-typing.Optional[schemas.Configuration] = None, ) -> 'clusters': return super
-().__new__( cls, arg, _configuration=_configuration, ) def __getitem__(self, i:
-int) -> 'Cluster': return super().__getitem__(i) user_input =
-schemas.DictSchema status = schemas.StrSchema __annotations__ = { "total_hits":
-total_hits, "page": page, "total_pages": total_pages, "page_size": page_size,
-"clusters_count": clusters_count, "clusters": clusters, "user_input":
-user_input, "status": status, } total_hits: MetaOapg.properties.total_hits
-user_input: MetaOapg.properties.user_input page: MetaOapg.properties.page
-total_pages: MetaOapg.properties.total_pages clusters_count:
-MetaOapg.properties.clusters_count clusters: MetaOapg.properties.clusters
-page_size: MetaOapg.properties.page_size @typing.overload def __getitem__(self,
-name: typing_extensions.Literal["total_hits"]) -
-> MetaOapg.properties.total_hits: ... @typing.overload def __getitem__(self,
-name: typing_extensions.Literal["page"]) -> MetaOapg.properties.page: ...
+generated by Konfig (https://konfigthis.com) ClusteringSearchResponse DTO
+class. """ class MetaOapg: required = { "total_hits", "user_input", "page",
+"total_pages", "clusters_count", "clusters", "page_size", } class properties:
+total_hits = schemas.IntSchema page = schemas.IntSchema total_pages =
+schemas.IntSchema page_size = schemas.IntSchema clusters_count =
+schemas.IntSchema class clusters( schemas.ListSchema ): class MetaOapg:
+@staticmethod def items() -> typing.Type['Cluster']: return Cluster def __new__
+( cls, arg: typing.Union[typing.Tuple['Cluster'], typing.List['Cluster']],
+_configuration: typing.Optional[schemas.Configuration] = None, ) -> 'clusters':
+return super().__new__( cls, arg, _configuration=_configuration, ) def
+__getitem__(self, i: int) -> 'Cluster': return super().__getitem__(i)
+user_input = schemas.DictSchema status = schemas.StrSchema __annotations__ =
+{ "total_hits": total_hits, "page": page, "total_pages": total_pages,
+"page_size": page_size, "clusters_count": clusters_count, "clusters": clusters,
+"user_input": user_input, "status": status, } total_hits:
+MetaOapg.properties.total_hits user_input: MetaOapg.properties.user_input page:
+MetaOapg.properties.page total_pages: MetaOapg.properties.total_pages
+clusters_count: MetaOapg.properties.clusters_count clusters:
+MetaOapg.properties.clusters page_size: MetaOapg.properties.page_size
 @typing.overload def __getitem__(self, name: typing_extensions.Literal
-["total_pages"]) -> MetaOapg.properties.total_pages: ... @typing.overload def
-__getitem__(self, name: typing_extensions.Literal["page_size"]) -
-> MetaOapg.properties.page_size: ... @typing.overload def __getitem__(self,
-name: typing_extensions.Literal["clusters_count"]) -
+["total_hits"]) -> MetaOapg.properties.total_hits: ... @typing.overload def
+__getitem__(self, name: typing_extensions.Literal["page"]) -
+> MetaOapg.properties.page: ... @typing.overload def __getitem__(self, name:
+typing_extensions.Literal["total_pages"]) -> MetaOapg.properties.total_pages:
+... @typing.overload def __getitem__(self, name: typing_extensions.Literal
+["page_size"]) -> MetaOapg.properties.page_size: ... @typing.overload def
+__getitem__(self, name: typing_extensions.Literal["clusters_count"]) -
 > MetaOapg.properties.clusters_count: ... @typing.overload def __getitem__
 (self, name: typing_extensions.Literal["clusters"]) -
 > MetaOapg.properties.clusters: ... @typing.overload def __getitem__(self,
 name: typing_extensions.Literal["user_input"]) -
 > MetaOapg.properties.user_input: ... @typing.overload def __getitem__(self,
 name: typing_extensions.Literal["status"]) -> MetaOapg.properties.status: ...
 @typing.overload def __getitem__(self, name: str) -
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/clustering_search_response.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/clustering_search_response.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class ClusteringSearchResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    ClusteringSearchResponse DTO class.
     """
 
 
     class MetaOapg:
         required = {
             "total_hits",
             "user_input",
```

#### html2text {}

```diff
@@ -6,41 +6,41 @@
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
 newscatcherapi_client import schemas # noqa: F401 class
 ClusteringSearchResponse( schemas.DictSchema ): """ This class is auto
-generated by Konfig (https://konfigthis.com) """ class MetaOapg: required =
-{ "total_hits", "user_input", "page", "total_pages", "clusters_count",
-"clusters", "page_size", } class properties: total_hits = schemas.IntSchema
-page = schemas.IntSchema total_pages = schemas.IntSchema page_size =
-schemas.IntSchema clusters_count = schemas.IntSchema class clusters
-( schemas.ListSchema ): class MetaOapg: @staticmethod def items() -
-> typing.Type['Cluster']: return Cluster def __new__( cls, arg: typing.Union
-[typing.Tuple['Cluster'], typing.List['Cluster']], _configuration:
-typing.Optional[schemas.Configuration] = None, ) -> 'clusters': return super
-().__new__( cls, arg, _configuration=_configuration, ) def __getitem__(self, i:
-int) -> 'Cluster': return super().__getitem__(i) user_input =
-schemas.DictSchema status = schemas.StrSchema __annotations__ = { "total_hits":
-total_hits, "page": page, "total_pages": total_pages, "page_size": page_size,
-"clusters_count": clusters_count, "clusters": clusters, "user_input":
-user_input, "status": status, } total_hits: MetaOapg.properties.total_hits
-user_input: MetaOapg.properties.user_input page: MetaOapg.properties.page
-total_pages: MetaOapg.properties.total_pages clusters_count:
-MetaOapg.properties.clusters_count clusters: MetaOapg.properties.clusters
-page_size: MetaOapg.properties.page_size @typing.overload def __getitem__(self,
-name: typing_extensions.Literal["total_hits"]) -
-> MetaOapg.properties.total_hits: ... @typing.overload def __getitem__(self,
-name: typing_extensions.Literal["page"]) -> MetaOapg.properties.page: ...
+generated by Konfig (https://konfigthis.com) ClusteringSearchResponse DTO
+class. """ class MetaOapg: required = { "total_hits", "user_input", "page",
+"total_pages", "clusters_count", "clusters", "page_size", } class properties:
+total_hits = schemas.IntSchema page = schemas.IntSchema total_pages =
+schemas.IntSchema page_size = schemas.IntSchema clusters_count =
+schemas.IntSchema class clusters( schemas.ListSchema ): class MetaOapg:
+@staticmethod def items() -> typing.Type['Cluster']: return Cluster def __new__
+( cls, arg: typing.Union[typing.Tuple['Cluster'], typing.List['Cluster']],
+_configuration: typing.Optional[schemas.Configuration] = None, ) -> 'clusters':
+return super().__new__( cls, arg, _configuration=_configuration, ) def
+__getitem__(self, i: int) -> 'Cluster': return super().__getitem__(i)
+user_input = schemas.DictSchema status = schemas.StrSchema __annotations__ =
+{ "total_hits": total_hits, "page": page, "total_pages": total_pages,
+"page_size": page_size, "clusters_count": clusters_count, "clusters": clusters,
+"user_input": user_input, "status": status, } total_hits:
+MetaOapg.properties.total_hits user_input: MetaOapg.properties.user_input page:
+MetaOapg.properties.page total_pages: MetaOapg.properties.total_pages
+clusters_count: MetaOapg.properties.clusters_count clusters:
+MetaOapg.properties.clusters page_size: MetaOapg.properties.page_size
 @typing.overload def __getitem__(self, name: typing_extensions.Literal
-["total_pages"]) -> MetaOapg.properties.total_pages: ... @typing.overload def
-__getitem__(self, name: typing_extensions.Literal["page_size"]) -
-> MetaOapg.properties.page_size: ... @typing.overload def __getitem__(self,
-name: typing_extensions.Literal["clusters_count"]) -
+["total_hits"]) -> MetaOapg.properties.total_hits: ... @typing.overload def
+__getitem__(self, name: typing_extensions.Literal["page"]) -
+> MetaOapg.properties.page: ... @typing.overload def __getitem__(self, name:
+typing_extensions.Literal["total_pages"]) -> MetaOapg.properties.total_pages:
+... @typing.overload def __getitem__(self, name: typing_extensions.Literal
+["page_size"]) -> MetaOapg.properties.page_size: ... @typing.overload def
+__getitem__(self, name: typing_extensions.Literal["clusters_count"]) -
 > MetaOapg.properties.clusters_count: ... @typing.overload def __getitem__
 (self, name: typing_extensions.Literal["clusters"]) -
 > MetaOapg.properties.clusters: ... @typing.overload def __getitem__(self,
 name: typing_extensions.Literal["user_input"]) -
 > MetaOapg.properties.user_input: ... @typing.overload def __getitem__(self,
 name: typing_extensions.Literal["status"]) -> MetaOapg.properties.status: ...
 @typing.overload def __getitem__(self, name: str) -
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_author_search_response_article_result.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_author_search_response_article_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class DtoResponsesAuthorSearchResponseArticleResult(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    Article result data model
     """
 
 
     class MetaOapg:
         required = {
             "score",
             "extraction_data",
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_author_search_response_article_result.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_author_search_response_article_result.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class DtoResponsesAuthorSearchResponseArticleResult(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    Article result data model
     """
 
 
     class MetaOapg:
         required = {
             "score",
             "extraction_data",
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_author_search_response_failed_search_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_author_search_response_failed_search_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class DtoResponsesAuthorSearchResponseFailedSearchResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    Failed search response data model
     """
 
 
     class MetaOapg:
         required = {
             "user_input",
         }
```

#### html2text {}

```diff
@@ -6,21 +6,21 @@
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
 newscatcherapi_client import schemas # noqa: F401 class
 DtoResponsesAuthorSearchResponseFailedSearchResponse( schemas.DictSchema ): """
-This class is auto generated by Konfig (https://konfigthis.com) """ class
-MetaOapg: required = { "user_input", } class properties: user_input =
-schemas.DictSchema status = schemas.StrSchema total_hits = schemas.IntSchema
-page = schemas.IntSchema total_pages = schemas.IntSchema page_size =
-schemas.IntSchema class articles( schemas.ListSchema ): class MetaOapg:
-@staticmethod def items() -> typing.Type
-['DtoResponsesAuthorSearchResponseArticleResult']: return
+This class is auto generated by Konfig (https://konfigthis.com) Failed search
+response data model """ class MetaOapg: required = { "user_input", } class
+properties: user_input = schemas.DictSchema status = schemas.StrSchema
+total_hits = schemas.IntSchema page = schemas.IntSchema total_pages =
+schemas.IntSchema page_size = schemas.IntSchema class articles
+( schemas.ListSchema ): class MetaOapg: @staticmethod def items() -
+> typing.Type['DtoResponsesAuthorSearchResponseArticleResult']: return
 DtoResponsesAuthorSearchResponseArticleResult def __new__( cls, arg:
 typing.Union[typing.Tuple['DtoResponsesAuthorSearchResponseArticleResult'],
 typing.List['DtoResponsesAuthorSearchResponseArticleResult']], _configuration:
 typing.Optional[schemas.Configuration] = None, ) -> 'articles': return super
 ().__new__( cls, arg, _configuration=_configuration, ) def __getitem__(self, i:
 int) -> 'DtoResponsesAuthorSearchResponseArticleResult': return super
 ().__getitem__(i) __annotations__ = { "user_input": user_input, "status":
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_author_search_response_failed_search_response.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_author_search_response_failed_search_response.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class DtoResponsesAuthorSearchResponseFailedSearchResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    Failed search response data model
     """
 
 
     class MetaOapg:
         required = {
             "user_input",
         }
```

#### html2text {}

```diff
@@ -6,21 +6,21 @@
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
 newscatcherapi_client import schemas # noqa: F401 class
 DtoResponsesAuthorSearchResponseFailedSearchResponse( schemas.DictSchema ): """
-This class is auto generated by Konfig (https://konfigthis.com) """ class
-MetaOapg: required = { "user_input", } class properties: user_input =
-schemas.DictSchema status = schemas.StrSchema total_hits = schemas.IntSchema
-page = schemas.IntSchema total_pages = schemas.IntSchema page_size =
-schemas.IntSchema class articles( schemas.ListSchema ): class MetaOapg:
-@staticmethod def items() -> typing.Type
-['DtoResponsesAuthorSearchResponseArticleResult']: return
+This class is auto generated by Konfig (https://konfigthis.com) Failed search
+response data model """ class MetaOapg: required = { "user_input", } class
+properties: user_input = schemas.DictSchema status = schemas.StrSchema
+total_hits = schemas.IntSchema page = schemas.IntSchema total_pages =
+schemas.IntSchema page_size = schemas.IntSchema class articles
+( schemas.ListSchema ): class MetaOapg: @staticmethod def items() -
+> typing.Type['DtoResponsesAuthorSearchResponseArticleResult']: return
 DtoResponsesAuthorSearchResponseArticleResult def __new__( cls, arg:
 typing.Union[typing.Tuple['DtoResponsesAuthorSearchResponseArticleResult'],
 typing.List['DtoResponsesAuthorSearchResponseArticleResult']], _configuration:
 typing.Optional[schemas.Configuration] = None, ) -> 'articles': return super
 ().__new__( cls, arg, _configuration=_configuration, ) def __getitem__(self, i:
 int) -> 'DtoResponsesAuthorSearchResponseArticleResult': return super
 ().__getitem__(i) __annotations__ = { "user_input": user_input, "status":
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_author_search_response_search_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_author_search_response_search_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class DtoResponsesAuthorSearchResponseSearchResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    Search response data model
     """
 
 
     class MetaOapg:
         required = {
             "total_hits",
             "user_input",
```

#### html2text {}

```diff
@@ -6,19 +6,19 @@
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
 newscatcherapi_client import schemas # noqa: F401 class
 DtoResponsesAuthorSearchResponseSearchResponse( schemas.DictSchema ): """ This
-class is auto generated by Konfig (https://konfigthis.com) """ class MetaOapg:
-required = { "total_hits", "user_input", "page", "total_pages", "articles",
-"page_size", } class properties: total_hits = schemas.IntSchema page =
-schemas.IntSchema total_pages = schemas.IntSchema page_size = schemas.IntSchema
-@staticmethod def articles() -> typing.Type
+class is auto generated by Konfig (https://konfigthis.com) Search response data
+model """ class MetaOapg: required = { "total_hits", "user_input", "page",
+"total_pages", "articles", "page_size", } class properties: total_hits =
+schemas.IntSchema page = schemas.IntSchema total_pages = schemas.IntSchema
+page_size = schemas.IntSchema @staticmethod def articles() -> typing.Type
 ['DtoResponsesAuthorSearchResponseSearchResponseArticles']: return
 DtoResponsesAuthorSearchResponseSearchResponseArticles user_input =
 schemas.DictSchema status = schemas.StrSchema __annotations__ = { "total_hits":
 total_hits, "page": page, "total_pages": total_pages, "page_size": page_size,
 "articles": articles, "user_input": user_input, "status": status, } total_hits:
 MetaOapg.properties.total_hits user_input: MetaOapg.properties.user_input page:
 MetaOapg.properties.page total_pages: MetaOapg.properties.total_pages articles:
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_author_search_response_search_response.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_author_search_response_search_response.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class DtoResponsesAuthorSearchResponseSearchResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    Search response data model
     """
 
 
     class MetaOapg:
         required = {
             "total_hits",
             "user_input",
```

#### html2text {}

```diff
@@ -6,19 +6,19 @@
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
 newscatcherapi_client import schemas # noqa: F401 class
 DtoResponsesAuthorSearchResponseSearchResponse( schemas.DictSchema ): """ This
-class is auto generated by Konfig (https://konfigthis.com) """ class MetaOapg:
-required = { "total_hits", "user_input", "page", "total_pages", "articles",
-"page_size", } class properties: total_hits = schemas.IntSchema page =
-schemas.IntSchema total_pages = schemas.IntSchema page_size = schemas.IntSchema
-@staticmethod def articles() -> typing.Type
+class is auto generated by Konfig (https://konfigthis.com) Search response data
+model """ class MetaOapg: required = { "total_hits", "user_input", "page",
+"total_pages", "articles", "page_size", } class properties: total_hits =
+schemas.IntSchema page = schemas.IntSchema total_pages = schemas.IntSchema
+page_size = schemas.IntSchema @staticmethod def articles() -> typing.Type
 ['DtoResponsesAuthorSearchResponseSearchResponseArticles']: return
 DtoResponsesAuthorSearchResponseSearchResponseArticles user_input =
 schemas.DictSchema status = schemas.StrSchema __annotations__ = { "total_hits":
 total_hits, "page": page, "total_pages": total_pages, "page_size": page_size,
 "articles": articles, "user_input": user_input, "status": status, } total_hits:
 MetaOapg.properties.total_hits user_input: MetaOapg.properties.user_input page:
 MetaOapg.properties.page total_pages: MetaOapg.properties.total_pages articles:
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_author_search_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_author_search_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_author_search_response_search_response_articles.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_author_search_response_search_response_articles.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_more_like_this_response_article_result.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_more_like_this_response_article_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class DtoResponsesMoreLikeThisResponseArticleResult(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    ArticleResult DTO class.
     """
 
 
     class MetaOapg:
         required = {
             "score",
             "extraction_data",
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_more_like_this_response_article_result.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_more_like_this_response_article_result.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class DtoResponsesMoreLikeThisResponseArticleResult(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    ArticleResult DTO class.
     """
 
 
     class MetaOapg:
         required = {
             "score",
             "extraction_data",
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_more_like_this_response_failed_search_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_more_like_this_response_failed_search_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class DtoResponsesMoreLikeThisResponseFailedSearchResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    FailedSearchResponse DTO class.
     """
 
 
     class MetaOapg:
         required = {
             "user_input",
         }
```

#### html2text {}

```diff
@@ -6,21 +6,21 @@
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
 newscatcherapi_client import schemas # noqa: F401 class
 DtoResponsesMoreLikeThisResponseFailedSearchResponse( schemas.DictSchema ): """
-This class is auto generated by Konfig (https://konfigthis.com) """ class
-MetaOapg: required = { "user_input", } class properties: user_input =
-schemas.DictSchema status = schemas.StrSchema total_hits = schemas.IntSchema
-page = schemas.IntSchema total_pages = schemas.IntSchema page_size =
-schemas.IntSchema class articles( schemas.ListSchema ): class MetaOapg:
-@staticmethod def items() -> typing.Type
-['DtoResponsesMoreLikeThisResponseArticleResult']: return
+This class is auto generated by Konfig (https://konfigthis.com)
+FailedSearchResponse DTO class. """ class MetaOapg: required = { "user_input",
+} class properties: user_input = schemas.DictSchema status = schemas.StrSchema
+total_hits = schemas.IntSchema page = schemas.IntSchema total_pages =
+schemas.IntSchema page_size = schemas.IntSchema class articles
+( schemas.ListSchema ): class MetaOapg: @staticmethod def items() -
+> typing.Type['DtoResponsesMoreLikeThisResponseArticleResult']: return
 DtoResponsesMoreLikeThisResponseArticleResult def __new__( cls, arg:
 typing.Union[typing.Tuple['DtoResponsesMoreLikeThisResponseArticleResult'],
 typing.List['DtoResponsesMoreLikeThisResponseArticleResult']], _configuration:
 typing.Optional[schemas.Configuration] = None, ) -> 'articles': return super
 ().__new__( cls, arg, _configuration=_configuration, ) def __getitem__(self, i:
 int) -> 'DtoResponsesMoreLikeThisResponseArticleResult': return super
 ().__getitem__(i) __annotations__ = { "user_input": user_input, "status":
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_more_like_this_response_failed_search_response.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_more_like_this_response_failed_search_response.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class DtoResponsesMoreLikeThisResponseFailedSearchResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    FailedSearchResponse DTO class.
     """
 
 
     class MetaOapg:
         required = {
             "user_input",
         }
```

#### html2text {}

```diff
@@ -6,21 +6,21 @@
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
 newscatcherapi_client import schemas # noqa: F401 class
 DtoResponsesMoreLikeThisResponseFailedSearchResponse( schemas.DictSchema ): """
-This class is auto generated by Konfig (https://konfigthis.com) """ class
-MetaOapg: required = { "user_input", } class properties: user_input =
-schemas.DictSchema status = schemas.StrSchema total_hits = schemas.IntSchema
-page = schemas.IntSchema total_pages = schemas.IntSchema page_size =
-schemas.IntSchema class articles( schemas.ListSchema ): class MetaOapg:
-@staticmethod def items() -> typing.Type
-['DtoResponsesMoreLikeThisResponseArticleResult']: return
+This class is auto generated by Konfig (https://konfigthis.com)
+FailedSearchResponse DTO class. """ class MetaOapg: required = { "user_input",
+} class properties: user_input = schemas.DictSchema status = schemas.StrSchema
+total_hits = schemas.IntSchema page = schemas.IntSchema total_pages =
+schemas.IntSchema page_size = schemas.IntSchema class articles
+( schemas.ListSchema ): class MetaOapg: @staticmethod def items() -
+> typing.Type['DtoResponsesMoreLikeThisResponseArticleResult']: return
 DtoResponsesMoreLikeThisResponseArticleResult def __new__( cls, arg:
 typing.Union[typing.Tuple['DtoResponsesMoreLikeThisResponseArticleResult'],
 typing.List['DtoResponsesMoreLikeThisResponseArticleResult']], _configuration:
 typing.Optional[schemas.Configuration] = None, ) -> 'articles': return super
 ().__new__( cls, arg, _configuration=_configuration, ) def __getitem__(self, i:
 int) -> 'DtoResponsesMoreLikeThisResponseArticleResult': return super
 ().__getitem__(i) __annotations__ = { "user_input": user_input, "status":
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class DtoResponsesMoreLikeThisResponseSearchResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    SearchResponse DTO class.
     """
 
 
     class MetaOapg:
         required = {
             "total_hits",
             "user_input",
```

#### html2text {}

```diff
@@ -6,19 +6,19 @@
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
 newscatcherapi_client import schemas # noqa: F401 class
 DtoResponsesMoreLikeThisResponseSearchResponse( schemas.DictSchema ): """ This
-class is auto generated by Konfig (https://konfigthis.com) """ class MetaOapg:
-required = { "total_hits", "user_input", "page", "total_pages", "articles",
-"page_size", } class properties: total_hits = schemas.IntSchema page =
-schemas.IntSchema total_pages = schemas.IntSchema page_size = schemas.IntSchema
-@staticmethod def articles() -> typing.Type
+class is auto generated by Konfig (https://konfigthis.com) SearchResponse DTO
+class. """ class MetaOapg: required = { "total_hits", "user_input", "page",
+"total_pages", "articles", "page_size", } class properties: total_hits =
+schemas.IntSchema page = schemas.IntSchema total_pages = schemas.IntSchema
+page_size = schemas.IntSchema @staticmethod def articles() -> typing.Type
 ['DtoResponsesMoreLikeThisResponseSearchResponseArticles']: return
 DtoResponsesMoreLikeThisResponseSearchResponseArticles user_input =
 schemas.DictSchema status = schemas.StrSchema __annotations__ = { "total_hits":
 total_hits, "page": page, "total_pages": total_pages, "page_size": page_size,
 "articles": articles, "user_input": user_input, "status": status, } total_hits:
 MetaOapg.properties.total_hits user_input: MetaOapg.properties.user_input page:
 MetaOapg.properties.page total_pages: MetaOapg.properties.total_pages articles:
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class DtoResponsesMoreLikeThisResponseSearchResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    SearchResponse DTO class.
     """
 
 
     class MetaOapg:
         required = {
             "total_hits",
             "user_input",
```

#### html2text {}

```diff
@@ -6,19 +6,19 @@
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
 newscatcherapi_client import schemas # noqa: F401 class
 DtoResponsesMoreLikeThisResponseSearchResponse( schemas.DictSchema ): """ This
-class is auto generated by Konfig (https://konfigthis.com) """ class MetaOapg:
-required = { "total_hits", "user_input", "page", "total_pages", "articles",
-"page_size", } class properties: total_hits = schemas.IntSchema page =
-schemas.IntSchema total_pages = schemas.IntSchema page_size = schemas.IntSchema
-@staticmethod def articles() -> typing.Type
+class is auto generated by Konfig (https://konfigthis.com) SearchResponse DTO
+class. """ class MetaOapg: required = { "total_hits", "user_input", "page",
+"total_pages", "articles", "page_size", } class properties: total_hits =
+schemas.IntSchema page = schemas.IntSchema total_pages = schemas.IntSchema
+page_size = schemas.IntSchema @staticmethod def articles() -> typing.Type
 ['DtoResponsesMoreLikeThisResponseSearchResponseArticles']: return
 DtoResponsesMoreLikeThisResponseSearchResponseArticles user_input =
 schemas.DictSchema status = schemas.StrSchema __annotations__ = { "total_hits":
 total_hits, "page": page, "total_pages": total_pages, "page_size": page_size,
 "articles": articles, "user_input": user_input, "status": status, } total_hits:
 MetaOapg.properties.total_hits user_input: MetaOapg.properties.user_input page:
 MetaOapg.properties.page total_pages: MetaOapg.properties.total_pages articles:
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response_articles.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response_articles.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_search_response_search_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_search_response_search_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class DtoResponsesSearchResponseSearchResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    SearchResponse DTO class.
     """
 
 
     class MetaOapg:
         required = {
             "total_hits",
             "user_input",
```

#### html2text {}

```diff
@@ -6,19 +6,19 @@
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
 newscatcherapi_client import schemas # noqa: F401 class
 DtoResponsesSearchResponseSearchResponse( schemas.DictSchema ): """ This class
-is auto generated by Konfig (https://konfigthis.com) """ class MetaOapg:
-required = { "total_hits", "user_input", "page", "total_pages", "articles",
-"page_size", } class properties: total_hits = schemas.IntSchema page =
-schemas.IntSchema total_pages = schemas.IntSchema page_size = schemas.IntSchema
-@staticmethod def articles() -> typing.Type
+is auto generated by Konfig (https://konfigthis.com) SearchResponse DTO class.
+""" class MetaOapg: required = { "total_hits", "user_input", "page",
+"total_pages", "articles", "page_size", } class properties: total_hits =
+schemas.IntSchema page = schemas.IntSchema total_pages = schemas.IntSchema
+page_size = schemas.IntSchema @staticmethod def articles() -> typing.Type
 ['DtoResponsesSearchResponseSearchResponseArticles']: return
 DtoResponsesSearchResponseSearchResponseArticles user_input =
 schemas.DictSchema status = schemas.StrSchema __annotations__ = { "total_hits":
 total_hits, "page": page, "total_pages": total_pages, "page_size": page_size,
 "articles": articles, "user_input": user_input, "status": status, } total_hits:
 MetaOapg.properties.total_hits user_input: MetaOapg.properties.user_input page:
 MetaOapg.properties.page total_pages: MetaOapg.properties.total_pages articles:
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_search_response_search_response.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_search_response_search_response.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class DtoResponsesSearchResponseSearchResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    SearchResponse DTO class.
     """
 
 
     class MetaOapg:
         required = {
             "total_hits",
             "user_input",
```

#### html2text {}

```diff
@@ -6,19 +6,19 @@
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
 newscatcherapi_client import schemas # noqa: F401 class
 DtoResponsesSearchResponseSearchResponse( schemas.DictSchema ): """ This class
-is auto generated by Konfig (https://konfigthis.com) """ class MetaOapg:
-required = { "total_hits", "user_input", "page", "total_pages", "articles",
-"page_size", } class properties: total_hits = schemas.IntSchema page =
-schemas.IntSchema total_pages = schemas.IntSchema page_size = schemas.IntSchema
-@staticmethod def articles() -> typing.Type
+is auto generated by Konfig (https://konfigthis.com) SearchResponse DTO class.
+""" class MetaOapg: required = { "total_hits", "user_input", "page",
+"total_pages", "articles", "page_size", } class properties: total_hits =
+schemas.IntSchema page = schemas.IntSchema total_pages = schemas.IntSchema
+page_size = schemas.IntSchema @staticmethod def articles() -> typing.Type
 ['DtoResponsesSearchResponseSearchResponseArticles']: return
 DtoResponsesSearchResponseSearchResponseArticles user_input =
 schemas.DictSchema status = schemas.StrSchema __annotations__ = { "total_hits":
 total_hits, "page": page, "total_pages": total_pages, "page_size": page_size,
 "articles": articles, "user_input": user_input, "status": status, } total_hits:
 MetaOapg.properties.total_hits user_input: MetaOapg.properties.user_input page:
 MetaOapg.properties.page total_pages: MetaOapg.properties.total_pages articles:
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_search_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_search_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_search_response_search_response_articles.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_search_response_search_response_articles.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/http_validation_error.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/http_validation_error.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/http_validation_error.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_get_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_get_response.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_get_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_post_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_post_response.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_post_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_request.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class LatestHeadlinesRequest(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    Latest headlines request DTO.
     """
 
 
     class MetaOapg:
         
         class properties:
             when = schemas.StrSchema
```

#### html2text {}

```diff
@@ -6,40 +6,40 @@
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
 newscatcherapi_client import schemas # noqa: F401 class LatestHeadlinesRequest
 ( schemas.DictSchema ): """ This class is auto generated by Konfig (https://
-konfigthis.com) """ class MetaOapg: class properties: when = schemas.StrSchema
-by_parse_date = schemas.BoolSchema lang = schemas.AnyTypeSchema not_lang =
-schemas.AnyTypeSchema countries = schemas.AnyTypeSchema not_countries =
-schemas.AnyTypeSchema sources = schemas.AnyTypeSchema predefined_sources =
-schemas.AnyTypeSchema not_sources = schemas.AnyTypeSchema not_author_name =
-schemas.AnyTypeSchema ranked_only = schemas.StrSchema is_headline =
-schemas.BoolSchema is_paid_content = schemas.BoolSchema parent_url =
-schemas.AnyTypeSchema all_links = schemas.AnyTypeSchema all_domain_links =
-schemas.AnyTypeSchema class word_count_min( schemas.IntSchema ): class
-MetaOapg: inclusive_minimum = 0 class word_count_max( schemas.IntSchema ):
-class MetaOapg: inclusive_minimum = 0 class page( schemas.IntSchema ): class
-MetaOapg: inclusive_minimum = 0 class page_size( schemas.IntSchema ): class
-MetaOapg: inclusive_minimum = 0 clustering_variable = schemas.StrSchema
-clustering_enabled = schemas.BoolSchema clustering_threshold =
-schemas.NumberSchema include_nlp_data = schemas.BoolSchema has_nlp =
-schemas.BoolSchema theme = schemas.StrSchema not_theme = schemas.StrSchema
-ORG_entity_name = schemas.StrSchema PER_entity_name = schemas.StrSchema
-LOC_entity_name = schemas.StrSchema MISC_entity_name = schemas.StrSchema
-title_sentiment_min = schemas.NumberSchema title_sentiment_max =
-schemas.NumberSchema content_sentiment_min = schemas.NumberSchema
-content_sentiment_max = schemas.NumberSchema iptc_tags = schemas.AnyTypeSchema
-not_iptc_tags = schemas.AnyTypeSchema iab_tags = schemas.AnyTypeSchema
-not_iab_tags = schemas.AnyTypeSchema __annotations__ = { "when": when,
-"by_parse_date": by_parse_date, "lang": lang, "not_lang": not_lang,
-"countries": countries, "not_countries": not_countries, "sources": sources,
-"predefined_sources": predefined_sources, "not_sources": not_sources,
+konfigthis.com) Latest headlines request DTO. """ class MetaOapg: class
+properties: when = schemas.StrSchema by_parse_date = schemas.BoolSchema lang =
+schemas.AnyTypeSchema not_lang = schemas.AnyTypeSchema countries =
+schemas.AnyTypeSchema not_countries = schemas.AnyTypeSchema sources =
+schemas.AnyTypeSchema predefined_sources = schemas.AnyTypeSchema not_sources =
+schemas.AnyTypeSchema not_author_name = schemas.AnyTypeSchema ranked_only =
+schemas.StrSchema is_headline = schemas.BoolSchema is_paid_content =
+schemas.BoolSchema parent_url = schemas.AnyTypeSchema all_links =
+schemas.AnyTypeSchema all_domain_links = schemas.AnyTypeSchema class
+word_count_min( schemas.IntSchema ): class MetaOapg: inclusive_minimum = 0
+class word_count_max( schemas.IntSchema ): class MetaOapg: inclusive_minimum =
+0 class page( schemas.IntSchema ): class MetaOapg: inclusive_minimum = 0 class
+page_size( schemas.IntSchema ): class MetaOapg: inclusive_minimum = 0
+clustering_variable = schemas.StrSchema clustering_enabled = schemas.BoolSchema
+clustering_threshold = schemas.NumberSchema include_nlp_data =
+schemas.BoolSchema has_nlp = schemas.BoolSchema theme = schemas.StrSchema
+not_theme = schemas.StrSchema ORG_entity_name = schemas.StrSchema
+PER_entity_name = schemas.StrSchema LOC_entity_name = schemas.StrSchema
+MISC_entity_name = schemas.StrSchema title_sentiment_min = schemas.NumberSchema
+title_sentiment_max = schemas.NumberSchema content_sentiment_min =
+schemas.NumberSchema content_sentiment_max = schemas.NumberSchema iptc_tags =
+schemas.AnyTypeSchema not_iptc_tags = schemas.AnyTypeSchema iab_tags =
+schemas.AnyTypeSchema not_iab_tags = schemas.AnyTypeSchema __annotations__ =
+{ "when": when, "by_parse_date": by_parse_date, "lang": lang, "not_lang":
+not_lang, "countries": countries, "not_countries": not_countries, "sources":
+sources, "predefined_sources": predefined_sources, "not_sources": not_sources,
 "not_author_name": not_author_name, "ranked_only": ranked_only, "is_headline":
 is_headline, "is_paid_content": is_paid_content, "parent_url": parent_url,
 "all_links": all_links, "all_domain_links": all_domain_links, "word_count_min":
 word_count_min, "word_count_max": word_count_max, "page": page, "page_size":
 page_size, "clustering_variable": clustering_variable, "clustering_enabled":
 clustering_enabled, "clustering_threshold": clustering_threshold,
 "include_nlp_data": include_nlp_data, "has_nlp": has_nlp, "theme": theme,
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_request.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_request.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class LatestHeadlinesRequest(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    Latest headlines request DTO.
     """
 
 
     class MetaOapg:
         
         class properties:
             when = schemas.StrSchema
```

#### html2text {}

```diff
@@ -6,27 +6,28 @@
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
 newscatcherapi_client import schemas # noqa: F401 class LatestHeadlinesRequest
 ( schemas.DictSchema ): """ This class is auto generated by Konfig (https://
-konfigthis.com) """ class MetaOapg: class properties: when = schemas.StrSchema
-by_parse_date = schemas.BoolSchema lang = schemas.AnyTypeSchema not_lang =
-schemas.AnyTypeSchema countries = schemas.AnyTypeSchema not_countries =
-schemas.AnyTypeSchema sources = schemas.AnyTypeSchema predefined_sources =
-schemas.AnyTypeSchema not_sources = schemas.AnyTypeSchema not_author_name =
-schemas.AnyTypeSchema ranked_only = schemas.StrSchema is_headline =
-schemas.BoolSchema is_paid_content = schemas.BoolSchema parent_url =
-schemas.AnyTypeSchema all_links = schemas.AnyTypeSchema all_domain_links =
-schemas.AnyTypeSchema class word_count_min( schemas.IntSchema ): pass class
-word_count_max( schemas.IntSchema ): pass class page( schemas.IntSchema ): pass
-class page_size( schemas.IntSchema ): pass clustering_variable =
-schemas.StrSchema clustering_enabled = schemas.BoolSchema clustering_threshold
-= schemas.NumberSchema include_nlp_data = schemas.BoolSchema has_nlp =
+konfigthis.com) Latest headlines request DTO. """ class MetaOapg: class
+properties: when = schemas.StrSchema by_parse_date = schemas.BoolSchema lang =
+schemas.AnyTypeSchema not_lang = schemas.AnyTypeSchema countries =
+schemas.AnyTypeSchema not_countries = schemas.AnyTypeSchema sources =
+schemas.AnyTypeSchema predefined_sources = schemas.AnyTypeSchema not_sources =
+schemas.AnyTypeSchema not_author_name = schemas.AnyTypeSchema ranked_only =
+schemas.StrSchema is_headline = schemas.BoolSchema is_paid_content =
+schemas.BoolSchema parent_url = schemas.AnyTypeSchema all_links =
+schemas.AnyTypeSchema all_domain_links = schemas.AnyTypeSchema class
+word_count_min( schemas.IntSchema ): pass class word_count_max
+( schemas.IntSchema ): pass class page( schemas.IntSchema ): pass class
+page_size( schemas.IntSchema ): pass clustering_variable = schemas.StrSchema
+clustering_enabled = schemas.BoolSchema clustering_threshold =
+schemas.NumberSchema include_nlp_data = schemas.BoolSchema has_nlp =
 schemas.BoolSchema theme = schemas.StrSchema not_theme = schemas.StrSchema
 ORG_entity_name = schemas.StrSchema PER_entity_name = schemas.StrSchema
 LOC_entity_name = schemas.StrSchema MISC_entity_name = schemas.StrSchema
 title_sentiment_min = schemas.NumberSchema title_sentiment_max =
 schemas.NumberSchema content_sentiment_min = schemas.NumberSchema
 content_sentiment_max = schemas.NumberSchema iptc_tags = schemas.AnyTypeSchema
 not_iptc_tags = schemas.AnyTypeSchema iab_tags = schemas.AnyTypeSchema
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class LatestHeadlinesResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    LatestHeadlinesResponse DTO class.
     """
 
 
     class MetaOapg:
         required = {
             "total_hits",
             "user_input",
```

#### html2text {}

```diff
@@ -6,34 +6,34 @@
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
 newscatcherapi_client import schemas # noqa: F401 class LatestHeadlinesResponse
 ( schemas.DictSchema ): """ This class is auto generated by Konfig (https://
-konfigthis.com) """ class MetaOapg: required = { "total_hits", "user_input",
-"page", "total_pages", "articles", "page_size", } class properties: total_hits
-= schemas.IntSchema page = schemas.IntSchema total_pages = schemas.IntSchema
-page_size = schemas.IntSchema @staticmethod def articles() -> typing.Type
-['LatestHeadlinesResponseArticles']: return LatestHeadlinesResponseArticles
-user_input = schemas.DictSchema status = schemas.StrSchema __annotations__ =
-{ "total_hits": total_hits, "page": page, "total_pages": total_pages,
-"page_size": page_size, "articles": articles, "user_input": user_input,
-"status": status, } total_hits: MetaOapg.properties.total_hits user_input:
-MetaOapg.properties.user_input page: MetaOapg.properties.page total_pages:
-MetaOapg.properties.total_pages articles: 'LatestHeadlinesResponseArticles'
-page_size: MetaOapg.properties.page_size @typing.overload def __getitem__(self,
-name: typing_extensions.Literal["total_hits"]) -
-> MetaOapg.properties.total_hits: ... @typing.overload def __getitem__(self,
-name: typing_extensions.Literal["page"]) -> MetaOapg.properties.page: ...
+konfigthis.com) LatestHeadlinesResponse DTO class. """ class MetaOapg: required
+= { "total_hits", "user_input", "page", "total_pages", "articles", "page_size",
+} class properties: total_hits = schemas.IntSchema page = schemas.IntSchema
+total_pages = schemas.IntSchema page_size = schemas.IntSchema @staticmethod def
+articles() -> typing.Type['LatestHeadlinesResponseArticles']: return
+LatestHeadlinesResponseArticles user_input = schemas.DictSchema status =
+schemas.StrSchema __annotations__ = { "total_hits": total_hits, "page": page,
+"total_pages": total_pages, "page_size": page_size, "articles": articles,
+"user_input": user_input, "status": status, } total_hits:
+MetaOapg.properties.total_hits user_input: MetaOapg.properties.user_input page:
+MetaOapg.properties.page total_pages: MetaOapg.properties.total_pages articles:
+'LatestHeadlinesResponseArticles' page_size: MetaOapg.properties.page_size
 @typing.overload def __getitem__(self, name: typing_extensions.Literal
-["total_pages"]) -> MetaOapg.properties.total_pages: ... @typing.overload def
-__getitem__(self, name: typing_extensions.Literal["page_size"]) -
-> MetaOapg.properties.page_size: ... @typing.overload def __getitem__(self,
-name: typing_extensions.Literal["articles"]) -
+["total_hits"]) -> MetaOapg.properties.total_hits: ... @typing.overload def
+__getitem__(self, name: typing_extensions.Literal["page"]) -
+> MetaOapg.properties.page: ... @typing.overload def __getitem__(self, name:
+typing_extensions.Literal["total_pages"]) -> MetaOapg.properties.total_pages:
+... @typing.overload def __getitem__(self, name: typing_extensions.Literal
+["page_size"]) -> MetaOapg.properties.page_size: ... @typing.overload def
+__getitem__(self, name: typing_extensions.Literal["articles"]) -
 > 'LatestHeadlinesResponseArticles': ... @typing.overload def __getitem__(self,
 name: typing_extensions.Literal["user_input"]) -
 > MetaOapg.properties.user_input: ... @typing.overload def __getitem__(self,
 name: typing_extensions.Literal["status"]) -> MetaOapg.properties.status: ...
 @typing.overload def __getitem__(self, name: str) -
 > schemas.UnsetAnyTypeSchema: ... def __getitem__(self, name: typing.Union
 [typing_extensions.Literal["total_hits", "page", "total_pages", "page_size",
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_response.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_response.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class LatestHeadlinesResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    LatestHeadlinesResponse DTO class.
     """
 
 
     class MetaOapg:
         required = {
             "total_hits",
             "user_input",
```

#### html2text {}

```diff
@@ -6,34 +6,34 @@
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
 newscatcherapi_client import schemas # noqa: F401 class LatestHeadlinesResponse
 ( schemas.DictSchema ): """ This class is auto generated by Konfig (https://
-konfigthis.com) """ class MetaOapg: required = { "total_hits", "user_input",
-"page", "total_pages", "articles", "page_size", } class properties: total_hits
-= schemas.IntSchema page = schemas.IntSchema total_pages = schemas.IntSchema
-page_size = schemas.IntSchema @staticmethod def articles() -> typing.Type
-['LatestHeadlinesResponseArticles']: return LatestHeadlinesResponseArticles
-user_input = schemas.DictSchema status = schemas.StrSchema __annotations__ =
-{ "total_hits": total_hits, "page": page, "total_pages": total_pages,
-"page_size": page_size, "articles": articles, "user_input": user_input,
-"status": status, } total_hits: MetaOapg.properties.total_hits user_input:
-MetaOapg.properties.user_input page: MetaOapg.properties.page total_pages:
-MetaOapg.properties.total_pages articles: 'LatestHeadlinesResponseArticles'
-page_size: MetaOapg.properties.page_size @typing.overload def __getitem__(self,
-name: typing_extensions.Literal["total_hits"]) -
-> MetaOapg.properties.total_hits: ... @typing.overload def __getitem__(self,
-name: typing_extensions.Literal["page"]) -> MetaOapg.properties.page: ...
+konfigthis.com) LatestHeadlinesResponse DTO class. """ class MetaOapg: required
+= { "total_hits", "user_input", "page", "total_pages", "articles", "page_size",
+} class properties: total_hits = schemas.IntSchema page = schemas.IntSchema
+total_pages = schemas.IntSchema page_size = schemas.IntSchema @staticmethod def
+articles() -> typing.Type['LatestHeadlinesResponseArticles']: return
+LatestHeadlinesResponseArticles user_input = schemas.DictSchema status =
+schemas.StrSchema __annotations__ = { "total_hits": total_hits, "page": page,
+"total_pages": total_pages, "page_size": page_size, "articles": articles,
+"user_input": user_input, "status": status, } total_hits:
+MetaOapg.properties.total_hits user_input: MetaOapg.properties.user_input page:
+MetaOapg.properties.page total_pages: MetaOapg.properties.total_pages articles:
+'LatestHeadlinesResponseArticles' page_size: MetaOapg.properties.page_size
 @typing.overload def __getitem__(self, name: typing_extensions.Literal
-["total_pages"]) -> MetaOapg.properties.total_pages: ... @typing.overload def
-__getitem__(self, name: typing_extensions.Literal["page_size"]) -
-> MetaOapg.properties.page_size: ... @typing.overload def __getitem__(self,
-name: typing_extensions.Literal["articles"]) -
+["total_hits"]) -> MetaOapg.properties.total_hits: ... @typing.overload def
+__getitem__(self, name: typing_extensions.Literal["page"]) -
+> MetaOapg.properties.page: ... @typing.overload def __getitem__(self, name:
+typing_extensions.Literal["total_pages"]) -> MetaOapg.properties.total_pages:
+... @typing.overload def __getitem__(self, name: typing_extensions.Literal
+["page_size"]) -> MetaOapg.properties.page_size: ... @typing.overload def
+__getitem__(self, name: typing_extensions.Literal["articles"]) -
 > 'LatestHeadlinesResponseArticles': ... @typing.overload def __getitem__(self,
 name: typing_extensions.Literal["user_input"]) -
 > MetaOapg.properties.user_input: ... @typing.overload def __getitem__(self,
 name: typing_extensions.Literal["status"]) -> MetaOapg.properties.status: ...
 @typing.overload def __getitem__(self, name: str) -
 > schemas.UnsetAnyTypeSchema: ... def __getitem__(self, name: typing.Union
 [typing_extensions.Literal["total_hits", "page", "total_pages", "page_size",
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_response_articles.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_response_articles.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_response_articles.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/more_like_this_request.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/more_like_this_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class MoreLikeThisRequest(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    More like this request DTO.
     """
 
 
     class MetaOapg:
         required = {
             "q",
         }
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/more_like_this_request.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/more_like_this_request.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class MoreLikeThisRequest(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    More like this request DTO.
     """
 
 
     class MetaOapg:
         required = {
             "q",
         }
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_get_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_get_response.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_get_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_post_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_post_response.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_post_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_request.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class SearchRequest(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    Search request DTO
     """
 
 
     class MetaOapg:
         required = {
             "q",
         }
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_request.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_request.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class SearchRequest(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    Search request DTO
     """
 
 
     class MetaOapg:
         required = {
             "q",
         }
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_similar_get_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_similar_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_similar_get_response.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_similar_get_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_similar_post_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_similar_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_similar_post_response.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_similar_post_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_url_request.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_url_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class SearchURLRequest(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    Search URL Request DTO.
     """
 
 
     class MetaOapg:
         
         class properties:
             ids = schemas.AnyTypeSchema
```

#### html2text {}

```diff
@@ -6,16 +6,16 @@
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
 newscatcherapi_client import schemas # noqa: F401 class SearchURLRequest
 ( schemas.DictSchema ): """ This class is auto generated by Konfig (https://
-konfigthis.com) """ class MetaOapg: class properties: ids =
-schemas.AnyTypeSchema links = schemas.AnyTypeSchema class page
+konfigthis.com) Search URL Request DTO. """ class MetaOapg: class properties:
+ids = schemas.AnyTypeSchema links = schemas.AnyTypeSchema class page
 ( schemas.IntSchema ): class MetaOapg: inclusive_minimum = 0 class page_size
 ( schemas.IntSchema ): class MetaOapg: inclusive_minimum = 0 __annotations__ =
 { "ids": ids, "links": links, "page": page, "page_size": page_size, }
 @typing.overload def __getitem__(self, name: typing_extensions.Literal["ids"])
 -> MetaOapg.properties.ids: ... @typing.overload def __getitem__(self, name:
 typing_extensions.Literal["links"]) -> MetaOapg.properties.links: ...
 @typing.overload def __getitem__(self, name: typing_extensions.Literal["page"])
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_url_request.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_url_request.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class SearchURLRequest(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    Search URL Request DTO.
     """
 
 
     class MetaOapg:
         
         class properties:
             ids = schemas.AnyTypeSchema
```

#### html2text {}

```diff
@@ -6,16 +6,16 @@
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
 newscatcherapi_client import schemas # noqa: F401 class SearchURLRequest
 ( schemas.DictSchema ): """ This class is auto generated by Konfig (https://
-konfigthis.com) """ class MetaOapg: class properties: ids =
-schemas.AnyTypeSchema links = schemas.AnyTypeSchema class page
+konfigthis.com) Search URL Request DTO. """ class MetaOapg: class properties:
+ids = schemas.AnyTypeSchema links = schemas.AnyTypeSchema class page
 ( schemas.IntSchema ): pass class page_size( schemas.IntSchema ): pass
 __annotations__ = { "ids": ids, "links": links, "page": page, "page_size":
 page_size, } @typing.overload def __getitem__(self, name:
 typing_extensions.Literal["ids"]) -> MetaOapg.properties.ids: ...
 @typing.overload def __getitem__(self, name: typing_extensions.Literal
 ["links"]) -> MetaOapg.properties.links: ... @typing.overload def __getitem__
 (self, name: typing_extensions.Literal["page"]) -> MetaOapg.properties.page:
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/similar_document.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/similar_document.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class SimilarDocument(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    SimilarDocument DTO class.
     """
 
 
     class MetaOapg:
         required = {
             "score",
             "link",
```

#### html2text {}

```diff
@@ -6,19 +6,19 @@
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
 newscatcherapi_client import schemas # noqa: F401 class SimilarDocument
 ( schemas.DictSchema ): """ This class is auto generated by Konfig (https://
-konfigthis.com) """ class MetaOapg: required = { "score", "link", "id",
-"title", } class properties: title = schemas.StrSchema id = schemas.StrSchema
-score = schemas.NumberSchema link = schemas.StrSchema __annotations__ =
-{ "title": title, "id": id, "score": score, "link": link, } score:
-MetaOapg.properties.score link: MetaOapg.properties.link id:
+konfigthis.com) SimilarDocument DTO class. """ class MetaOapg: required =
+{ "score", "link", "id", "title", } class properties: title = schemas.StrSchema
+id = schemas.StrSchema score = schemas.NumberSchema link = schemas.StrSchema
+__annotations__ = { "title": title, "id": id, "score": score, "link": link, }
+score: MetaOapg.properties.score link: MetaOapg.properties.link id:
 MetaOapg.properties.id title: MetaOapg.properties.title @typing.overload def
 __getitem__(self, name: typing_extensions.Literal["title"]) -
 > MetaOapg.properties.title: ... @typing.overload def __getitem__(self, name:
 typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
 @typing.overload def __getitem__(self, name: typing_extensions.Literal
 ["score"]) -> MetaOapg.properties.score: ... @typing.overload def __getitem__
 (self, name: typing_extensions.Literal["link"]) -> MetaOapg.properties.link:
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/similar_document.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/similar_document.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class SimilarDocument(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    SimilarDocument DTO class.
     """
 
 
     class MetaOapg:
         required = {
             "score",
             "link",
```

#### html2text {}

```diff
@@ -6,19 +6,19 @@
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
 newscatcherapi_client import schemas # noqa: F401 class SimilarDocument
 ( schemas.DictSchema ): """ This class is auto generated by Konfig (https://
-konfigthis.com) """ class MetaOapg: required = { "score", "link", "id",
-"title", } class properties: title = schemas.StrSchema id = schemas.StrSchema
-score = schemas.NumberSchema link = schemas.StrSchema __annotations__ =
-{ "title": title, "id": id, "score": score, "link": link, } score:
-MetaOapg.properties.score link: MetaOapg.properties.link id:
+konfigthis.com) SimilarDocument DTO class. """ class MetaOapg: required =
+{ "score", "link", "id", "title", } class properties: title = schemas.StrSchema
+id = schemas.StrSchema score = schemas.NumberSchema link = schemas.StrSchema
+__annotations__ = { "title": title, "id": id, "score": score, "link": link, }
+score: MetaOapg.properties.score link: MetaOapg.properties.link id:
 MetaOapg.properties.id title: MetaOapg.properties.title @typing.overload def
 __getitem__(self, name: typing_extensions.Literal["title"]) -
 > MetaOapg.properties.title: ... @typing.overload def __getitem__(self, name:
 typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
 @typing.overload def __getitem__(self, name: typing_extensions.Literal
 ["score"]) -> MetaOapg.properties.score: ... @typing.overload def __getitem__
 (self, name: typing_extensions.Literal["link"]) -> MetaOapg.properties.link:
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/source_info.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/source_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class SourceInfo(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    "SourceInfo DTO class.
     """
 
 
     class MetaOapg:
         required = {
             "domain_url",
         }
```

#### html2text {}

```diff
@@ -6,20 +6,20 @@
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
 newscatcherapi_client import schemas # noqa: F401 class SourceInfo
 ( schemas.DictSchema ): """ This class is auto generated by Konfig (https://
-konfigthis.com) """ class MetaOapg: required = { "domain_url", } class
-properties: domain_url = schemas.StrSchema name_source = schemas.StrSchema logo
-= schemas.StrSchema @staticmethod def additional_info() -> typing.Type
-['AdditionalSourceInfo']: return AdditionalSourceInfo __annotations__ =
-{ "domain_url": domain_url, "name_source": name_source, "logo": logo,
-"additional_info": additional_info, } domain_url:
+konfigthis.com) "SourceInfo DTO class. """ class MetaOapg: required =
+{ "domain_url", } class properties: domain_url = schemas.StrSchema name_source
+= schemas.StrSchema logo = schemas.StrSchema @staticmethod def additional_info
+() -> typing.Type['AdditionalSourceInfo']: return AdditionalSourceInfo
+__annotations__ = { "domain_url": domain_url, "name_source": name_source,
+"logo": logo, "additional_info": additional_info, } domain_url:
 MetaOapg.properties.domain_url @typing.overload def __getitem__(self, name:
 typing_extensions.Literal["domain_url"]) -> MetaOapg.properties.domain_url: ...
 @typing.overload def __getitem__(self, name: typing_extensions.Literal
 ["name_source"]) -> MetaOapg.properties.name_source: ... @typing.overload def
 __getitem__(self, name: typing_extensions.Literal["logo"]) -
 > MetaOapg.properties.logo: ... @typing.overload def __getitem__(self, name:
 typing_extensions.Literal["additional_info"]) -> 'AdditionalSourceInfo': ...
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/source_info.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/source_info.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class SourceInfo(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    "SourceInfo DTO class.
     """
 
 
     class MetaOapg:
         required = {
             "domain_url",
         }
```

#### html2text {}

```diff
@@ -6,20 +6,20 @@
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
 newscatcherapi_client import schemas # noqa: F401 class SourceInfo
 ( schemas.DictSchema ): """ This class is auto generated by Konfig (https://
-konfigthis.com) """ class MetaOapg: required = { "domain_url", } class
-properties: domain_url = schemas.StrSchema name_source = schemas.StrSchema logo
-= schemas.StrSchema @staticmethod def additional_info() -> typing.Type
-['AdditionalSourceInfo']: return AdditionalSourceInfo __annotations__ =
-{ "domain_url": domain_url, "name_source": name_source, "logo": logo,
-"additional_info": additional_info, } domain_url:
+konfigthis.com) "SourceInfo DTO class. """ class MetaOapg: required =
+{ "domain_url", } class properties: domain_url = schemas.StrSchema name_source
+= schemas.StrSchema logo = schemas.StrSchema @staticmethod def additional_info
+() -> typing.Type['AdditionalSourceInfo']: return AdditionalSourceInfo
+__annotations__ = { "domain_url": domain_url, "name_source": name_source,
+"logo": logo, "additional_info": additional_info, } domain_url:
 MetaOapg.properties.domain_url @typing.overload def __getitem__(self, name:
 typing_extensions.Literal["domain_url"]) -> MetaOapg.properties.domain_url: ...
 @typing.overload def __getitem__(self, name: typing_extensions.Literal
 ["name_source"]) -> MetaOapg.properties.name_source: ... @typing.overload def
 __getitem__(self, name: typing_extensions.Literal["logo"]) -
 > MetaOapg.properties.logo: ... @typing.overload def __getitem__(self, name:
 typing_extensions.Literal["additional_info"]) -> 'AdditionalSourceInfo': ...
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/source_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/source_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class SourceResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    SourceResponse DTO class.
     """
 
 
     class MetaOapg:
         required = {
             "sources",
             "user_input",
```

#### html2text {}

```diff
@@ -6,39 +6,40 @@
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
 newscatcherapi_client import schemas # noqa: F401 class SourceResponse
 ( schemas.DictSchema ): """ This class is auto generated by Konfig (https://
-konfigthis.com) """ class MetaOapg: required = { "sources", "user_input",
-"message", } class properties: message = schemas.StrSchema @staticmethod def
-sources() -> typing.Type['SourceResponseSources']: return SourceResponseSources
-user_input = schemas.DictSchema __annotations__ = { "message": message,
-"sources": sources, "user_input": user_input, } sources:
-'SourceResponseSources' user_input: MetaOapg.properties.user_input message:
-MetaOapg.properties.message @typing.overload def __getitem__(self, name:
-typing_extensions.Literal["message"]) -> MetaOapg.properties.message: ...
+konfigthis.com) SourceResponse DTO class. """ class MetaOapg: required =
+{ "sources", "user_input", "message", } class properties: message =
+schemas.StrSchema @staticmethod def sources() -> typing.Type
+['SourceResponseSources']: return SourceResponseSources user_input =
+schemas.DictSchema __annotations__ = { "message": message, "sources": sources,
+"user_input": user_input, } sources: 'SourceResponseSources' user_input:
+MetaOapg.properties.user_input message: MetaOapg.properties.message
 @typing.overload def __getitem__(self, name: typing_extensions.Literal
-["sources"]) -> 'SourceResponseSources': ... @typing.overload def __getitem__
-(self, name: typing_extensions.Literal["user_input"]) -
-> MetaOapg.properties.user_input: ... @typing.overload def __getitem__(self,
-name: str) -> schemas.UnsetAnyTypeSchema: ... def __getitem__(self, name:
-typing.Union[typing_extensions.Literal["message", "sources", "user_input", ],
-str]): # dict_instance[name] accessor return super().__getitem__(name)
-@typing.overload def get_item_oapg(self, name: typing_extensions.Literal
 ["message"]) -> MetaOapg.properties.message: ... @typing.overload def
-get_item_oapg(self, name: typing_extensions.Literal["sources"]) -
-> 'SourceResponseSources': ... @typing.overload def get_item_oapg(self, name:
+__getitem__(self, name: typing_extensions.Literal["sources"]) -
+> 'SourceResponseSources': ... @typing.overload def __getitem__(self, name:
 typing_extensions.Literal["user_input"]) -> MetaOapg.properties.user_input: ...
-@typing.overload def get_item_oapg(self, name: str) -> typing.Union
-[schemas.UnsetAnyTypeSchema, schemas.Unset]: ... def get_item_oapg(self, name:
-typing.Union[typing_extensions.Literal["message", "sources", "user_input", ],
-str]): return super().get_item_oapg(name) def __new__( cls, *args: typing.Union
-[dict, frozendict.frozendict, ], sources: 'SourceResponseSources', user_input:
+@typing.overload def __getitem__(self, name: str) -
+> schemas.UnsetAnyTypeSchema: ... def __getitem__(self, name: typing.Union
+[typing_extensions.Literal["message", "sources", "user_input", ], str]): #
+dict_instance[name] accessor return super().__getitem__(name) @typing.overload
+def get_item_oapg(self, name: typing_extensions.Literal["message"]) -
+> MetaOapg.properties.message: ... @typing.overload def get_item_oapg(self,
+name: typing_extensions.Literal["sources"]) -> 'SourceResponseSources': ...
+@typing.overload def get_item_oapg(self, name: typing_extensions.Literal
+["user_input"]) -> MetaOapg.properties.user_input: ... @typing.overload def
+get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema,
+schemas.Unset]: ... def get_item_oapg(self, name: typing.Union
+[typing_extensions.Literal["message", "sources", "user_input", ], str]): return
+super().get_item_oapg(name) def __new__( cls, *args: typing.Union[dict,
+frozendict.frozendict, ], sources: 'SourceResponseSources', user_input:
 typing.Union[MetaOapg.properties.user_input, dict, frozendict.frozendict, ],
 message: typing.Union[MetaOapg.properties.message, str, ], _configuration:
 typing.Optional[schemas.Configuration] = None, **kwargs: typing.Union
 [schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime,
 uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes], ) -
 > 'SourceResponse': return super().__new__( cls, *args, sources=sources,
 user_input=user_input, message=message, _configuration=_configuration,
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/source_response.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/source_response.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class SourceResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    SourceResponse DTO class.
     """
 
 
     class MetaOapg:
         required = {
             "sources",
             "user_input",
```

#### html2text {}

```diff
@@ -6,39 +6,40 @@
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
 newscatcherapi_client import schemas # noqa: F401 class SourceResponse
 ( schemas.DictSchema ): """ This class is auto generated by Konfig (https://
-konfigthis.com) """ class MetaOapg: required = { "sources", "user_input",
-"message", } class properties: message = schemas.StrSchema @staticmethod def
-sources() -> typing.Type['SourceResponseSources']: return SourceResponseSources
-user_input = schemas.DictSchema __annotations__ = { "message": message,
-"sources": sources, "user_input": user_input, } sources:
-'SourceResponseSources' user_input: MetaOapg.properties.user_input message:
-MetaOapg.properties.message @typing.overload def __getitem__(self, name:
-typing_extensions.Literal["message"]) -> MetaOapg.properties.message: ...
+konfigthis.com) SourceResponse DTO class. """ class MetaOapg: required =
+{ "sources", "user_input", "message", } class properties: message =
+schemas.StrSchema @staticmethod def sources() -> typing.Type
+['SourceResponseSources']: return SourceResponseSources user_input =
+schemas.DictSchema __annotations__ = { "message": message, "sources": sources,
+"user_input": user_input, } sources: 'SourceResponseSources' user_input:
+MetaOapg.properties.user_input message: MetaOapg.properties.message
 @typing.overload def __getitem__(self, name: typing_extensions.Literal
-["sources"]) -> 'SourceResponseSources': ... @typing.overload def __getitem__
-(self, name: typing_extensions.Literal["user_input"]) -
-> MetaOapg.properties.user_input: ... @typing.overload def __getitem__(self,
-name: str) -> schemas.UnsetAnyTypeSchema: ... def __getitem__(self, name:
-typing.Union[typing_extensions.Literal["message", "sources", "user_input", ],
-str]): # dict_instance[name] accessor return super().__getitem__(name)
-@typing.overload def get_item_oapg(self, name: typing_extensions.Literal
 ["message"]) -> MetaOapg.properties.message: ... @typing.overload def
-get_item_oapg(self, name: typing_extensions.Literal["sources"]) -
-> 'SourceResponseSources': ... @typing.overload def get_item_oapg(self, name:
+__getitem__(self, name: typing_extensions.Literal["sources"]) -
+> 'SourceResponseSources': ... @typing.overload def __getitem__(self, name:
 typing_extensions.Literal["user_input"]) -> MetaOapg.properties.user_input: ...
-@typing.overload def get_item_oapg(self, name: str) -> typing.Union
-[schemas.UnsetAnyTypeSchema, schemas.Unset]: ... def get_item_oapg(self, name:
-typing.Union[typing_extensions.Literal["message", "sources", "user_input", ],
-str]): return super().get_item_oapg(name) def __new__( cls, *args: typing.Union
-[dict, frozendict.frozendict, ], sources: 'SourceResponseSources', user_input:
+@typing.overload def __getitem__(self, name: str) -
+> schemas.UnsetAnyTypeSchema: ... def __getitem__(self, name: typing.Union
+[typing_extensions.Literal["message", "sources", "user_input", ], str]): #
+dict_instance[name] accessor return super().__getitem__(name) @typing.overload
+def get_item_oapg(self, name: typing_extensions.Literal["message"]) -
+> MetaOapg.properties.message: ... @typing.overload def get_item_oapg(self,
+name: typing_extensions.Literal["sources"]) -> 'SourceResponseSources': ...
+@typing.overload def get_item_oapg(self, name: typing_extensions.Literal
+["user_input"]) -> MetaOapg.properties.user_input: ... @typing.overload def
+get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema,
+schemas.Unset]: ... def get_item_oapg(self, name: typing.Union
+[typing_extensions.Literal["message", "sources", "user_input", ], str]): return
+super().get_item_oapg(name) def __new__( cls, *args: typing.Union[dict,
+frozendict.frozendict, ], sources: 'SourceResponseSources', user_input:
 typing.Union[MetaOapg.properties.user_input, dict, frozendict.frozendict, ],
 message: typing.Union[MetaOapg.properties.message, str, ], _configuration:
 typing.Optional[schemas.Configuration] = None, **kwargs: typing.Union
 [schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime,
 uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes], ) -
 > 'SourceResponse': return super().__new__( cls, *args, sources=sources,
 user_input=user_input, message=message, _configuration=_configuration,
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/source_response_sources.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/source_response_sources.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/source_response_sources.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/source_response_sources.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/sources_request.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/sources_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class SourcesRequest(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    Sources request DTO
     """
 
 
     class MetaOapg:
         
         class properties:
             lang = schemas.StrSchema
```

#### html2text {}

```diff
@@ -6,38 +6,39 @@
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
 newscatcherapi_client import schemas # noqa: F401 class SourcesRequest
 ( schemas.DictSchema ): """ This class is auto generated by Konfig (https://
-konfigthis.com) """ class MetaOapg: class properties: lang = schemas.StrSchema
-countries = schemas.StrSchema predefined_sources = schemas.StrSchema
-include_additional_info = schemas.BoolSchema from_rank = schemas.IntSchema
-to_rank = schemas.IntSchema source_name = schemas.AnyTypeSchema source_url =
-schemas.StrSchema __annotations__ = { "lang": lang, "countries": countries,
-"predefined_sources": predefined_sources, "include_additional_info":
-include_additional_info, "from_rank": from_rank, "to_rank": to_rank,
-"source_name": source_name, "source_url": source_url, } @typing.overload def
-__getitem__(self, name: typing_extensions.Literal["lang"]) -
-> MetaOapg.properties.lang: ... @typing.overload def __getitem__(self, name:
-typing_extensions.Literal["countries"]) -> MetaOapg.properties.countries: ...
+konfigthis.com) Sources request DTO """ class MetaOapg: class properties: lang
+= schemas.StrSchema countries = schemas.StrSchema predefined_sources =
+schemas.StrSchema include_additional_info = schemas.BoolSchema from_rank =
+schemas.IntSchema to_rank = schemas.IntSchema source_name =
+schemas.AnyTypeSchema source_url = schemas.StrSchema __annotations__ =
+{ "lang": lang, "countries": countries, "predefined_sources":
+predefined_sources, "include_additional_info": include_additional_info,
+"from_rank": from_rank, "to_rank": to_rank, "source_name": source_name,
+"source_url": source_url, } @typing.overload def __getitem__(self, name:
+typing_extensions.Literal["lang"]) -> MetaOapg.properties.lang: ...
 @typing.overload def __getitem__(self, name: typing_extensions.Literal
-["predefined_sources"]) -> MetaOapg.properties.predefined_sources: ...
+["countries"]) -> MetaOapg.properties.countries: ... @typing.overload def
+__getitem__(self, name: typing_extensions.Literal["predefined_sources"]) -
+> MetaOapg.properties.predefined_sources: ... @typing.overload def __getitem__
+(self, name: typing_extensions.Literal["include_additional_info"]) -
+> MetaOapg.properties.include_additional_info: ... @typing.overload def
+__getitem__(self, name: typing_extensions.Literal["from_rank"]) -
+> MetaOapg.properties.from_rank: ... @typing.overload def __getitem__(self,
+name: typing_extensions.Literal["to_rank"]) -> MetaOapg.properties.to_rank: ...
 @typing.overload def __getitem__(self, name: typing_extensions.Literal
-["include_additional_info"]) -> MetaOapg.properties.include_additional_info:
-... @typing.overload def __getitem__(self, name: typing_extensions.Literal
-["from_rank"]) -> MetaOapg.properties.from_rank: ... @typing.overload def
-__getitem__(self, name: typing_extensions.Literal["to_rank"]) -
-> MetaOapg.properties.to_rank: ... @typing.overload def __getitem__(self, name:
-typing_extensions.Literal["source_name"]) -> MetaOapg.properties.source_name:
-... @typing.overload def __getitem__(self, name: typing_extensions.Literal
-["source_url"]) -> MetaOapg.properties.source_url: ... @typing.overload def
-__getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ... def __getitem__
-(self, name: typing.Union[typing_extensions.Literal["lang", "countries",
+["source_name"]) -> MetaOapg.properties.source_name: ... @typing.overload def
+__getitem__(self, name: typing_extensions.Literal["source_url"]) -
+> MetaOapg.properties.source_url: ... @typing.overload def __getitem__(self,
+name: str) -> schemas.UnsetAnyTypeSchema: ... def __getitem__(self, name:
+typing.Union[typing_extensions.Literal["lang", "countries",
 "predefined_sources", "include_additional_info", "from_rank", "to_rank",
 "source_name", "source_url", ], str]): # dict_instance[name] accessor return
 super().__getitem__(name) @typing.overload def get_item_oapg(self, name:
 typing_extensions.Literal["lang"]) -> typing.Union[MetaOapg.properties.lang,
 schemas.Unset]: ... @typing.overload def get_item_oapg(self, name:
 typing_extensions.Literal["countries"]) -> typing.Union
 [MetaOapg.properties.countries, schemas.Unset]: ... @typing.overload def
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/sources_request.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/sources_request.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class SourcesRequest(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    Sources request DTO
     """
 
 
     class MetaOapg:
         
         class properties:
             lang = schemas.StrSchema
```

#### html2text {}

```diff
@@ -6,38 +6,39 @@
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
 newscatcherapi_client import schemas # noqa: F401 class SourcesRequest
 ( schemas.DictSchema ): """ This class is auto generated by Konfig (https://
-konfigthis.com) """ class MetaOapg: class properties: lang = schemas.StrSchema
-countries = schemas.StrSchema predefined_sources = schemas.StrSchema
-include_additional_info = schemas.BoolSchema from_rank = schemas.IntSchema
-to_rank = schemas.IntSchema source_name = schemas.AnyTypeSchema source_url =
-schemas.StrSchema __annotations__ = { "lang": lang, "countries": countries,
-"predefined_sources": predefined_sources, "include_additional_info":
-include_additional_info, "from_rank": from_rank, "to_rank": to_rank,
-"source_name": source_name, "source_url": source_url, } @typing.overload def
-__getitem__(self, name: typing_extensions.Literal["lang"]) -
-> MetaOapg.properties.lang: ... @typing.overload def __getitem__(self, name:
-typing_extensions.Literal["countries"]) -> MetaOapg.properties.countries: ...
+konfigthis.com) Sources request DTO """ class MetaOapg: class properties: lang
+= schemas.StrSchema countries = schemas.StrSchema predefined_sources =
+schemas.StrSchema include_additional_info = schemas.BoolSchema from_rank =
+schemas.IntSchema to_rank = schemas.IntSchema source_name =
+schemas.AnyTypeSchema source_url = schemas.StrSchema __annotations__ =
+{ "lang": lang, "countries": countries, "predefined_sources":
+predefined_sources, "include_additional_info": include_additional_info,
+"from_rank": from_rank, "to_rank": to_rank, "source_name": source_name,
+"source_url": source_url, } @typing.overload def __getitem__(self, name:
+typing_extensions.Literal["lang"]) -> MetaOapg.properties.lang: ...
 @typing.overload def __getitem__(self, name: typing_extensions.Literal
-["predefined_sources"]) -> MetaOapg.properties.predefined_sources: ...
+["countries"]) -> MetaOapg.properties.countries: ... @typing.overload def
+__getitem__(self, name: typing_extensions.Literal["predefined_sources"]) -
+> MetaOapg.properties.predefined_sources: ... @typing.overload def __getitem__
+(self, name: typing_extensions.Literal["include_additional_info"]) -
+> MetaOapg.properties.include_additional_info: ... @typing.overload def
+__getitem__(self, name: typing_extensions.Literal["from_rank"]) -
+> MetaOapg.properties.from_rank: ... @typing.overload def __getitem__(self,
+name: typing_extensions.Literal["to_rank"]) -> MetaOapg.properties.to_rank: ...
 @typing.overload def __getitem__(self, name: typing_extensions.Literal
-["include_additional_info"]) -> MetaOapg.properties.include_additional_info:
-... @typing.overload def __getitem__(self, name: typing_extensions.Literal
-["from_rank"]) -> MetaOapg.properties.from_rank: ... @typing.overload def
-__getitem__(self, name: typing_extensions.Literal["to_rank"]) -
-> MetaOapg.properties.to_rank: ... @typing.overload def __getitem__(self, name:
-typing_extensions.Literal["source_name"]) -> MetaOapg.properties.source_name:
-... @typing.overload def __getitem__(self, name: typing_extensions.Literal
-["source_url"]) -> MetaOapg.properties.source_url: ... @typing.overload def
-__getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ... def __getitem__
-(self, name: typing.Union[typing_extensions.Literal["lang", "countries",
+["source_name"]) -> MetaOapg.properties.source_name: ... @typing.overload def
+__getitem__(self, name: typing_extensions.Literal["source_url"]) -
+> MetaOapg.properties.source_url: ... @typing.overload def __getitem__(self,
+name: str) -> schemas.UnsetAnyTypeSchema: ... def __getitem__(self, name:
+typing.Union[typing_extensions.Literal["lang", "countries",
 "predefined_sources", "include_additional_info", "from_rank", "to_rank",
 "source_name", "source_url", ], str]): # dict_instance[name] accessor return
 super().__getitem__(name) @typing.overload def get_item_oapg(self, name:
 typing_extensions.Literal["lang"]) -> typing.Union[MetaOapg.properties.lang,
 schemas.Unset]: ... @typing.overload def get_item_oapg(self, name:
 typing_extensions.Literal["countries"]) -> typing.Union
 [MetaOapg.properties.countries, schemas.Unset]: ... @typing.overload def
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/subscription_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/subscription_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class SubscriptionResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    SubscriptionResponse DTO class.
     """
 
 
     class MetaOapg:
         required = {
             "active",
             "plan_name",
```

#### html2text {}

```diff
@@ -6,24 +6,25 @@
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
 newscatcherapi_client import schemas # noqa: F401 class SubscriptionResponse
 ( schemas.DictSchema ): """ This class is auto generated by Konfig (https://
-konfigthis.com) """ class MetaOapg: required = { "active", "plan_name", } class
-properties: active = schemas.BoolSchema plan_name = schemas.StrSchema
-calls_per_seconds = schemas.IntSchema usage_assigned_calls = schemas.IntSchema
-usage_remaining_calls = schemas.IntSchema historical_days = schemas.IntSchema
-__annotations__ = { "active": active, "plan_name": plan_name,
-"calls_per_seconds": calls_per_seconds, "usage_assigned_calls":
-usage_assigned_calls, "usage_remaining_calls": usage_remaining_calls,
-"historical_days": historical_days, } active: MetaOapg.properties.active
-plan_name: MetaOapg.properties.plan_name @typing.overload def __getitem__(self,
-name: typing_extensions.Literal["active"]) -> MetaOapg.properties.active: ...
+konfigthis.com) SubscriptionResponse DTO class. """ class MetaOapg: required =
+{ "active", "plan_name", } class properties: active = schemas.BoolSchema
+plan_name = schemas.StrSchema calls_per_seconds = schemas.IntSchema
+usage_assigned_calls = schemas.IntSchema usage_remaining_calls =
+schemas.IntSchema historical_days = schemas.IntSchema __annotations__ =
+{ "active": active, "plan_name": plan_name, "calls_per_seconds":
+calls_per_seconds, "usage_assigned_calls": usage_assigned_calls,
+"usage_remaining_calls": usage_remaining_calls, "historical_days":
+historical_days, } active: MetaOapg.properties.active plan_name:
+MetaOapg.properties.plan_name @typing.overload def __getitem__(self, name:
+typing_extensions.Literal["active"]) -> MetaOapg.properties.active: ...
 @typing.overload def __getitem__(self, name: typing_extensions.Literal
 ["plan_name"]) -> MetaOapg.properties.plan_name: ... @typing.overload def
 __getitem__(self, name: typing_extensions.Literal["calls_per_seconds"]) -
 > MetaOapg.properties.calls_per_seconds: ... @typing.overload def __getitem__
 (self, name: typing_extensions.Literal["usage_assigned_calls"]) -
 > MetaOapg.properties.usage_assigned_calls: ... @typing.overload def
 __getitem__(self, name: typing_extensions.Literal["usage_remaining_calls"]) -
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/subscription_response.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/subscription_response.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class SubscriptionResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
+
+    SubscriptionResponse DTO class.
     """
 
 
     class MetaOapg:
         required = {
             "active",
             "plan_name",
```

#### html2text {}

```diff
@@ -6,24 +6,25 @@
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
 konfigthis.com """ from datetime import date, datetime # noqa: F401 import
 decimal # noqa: F401 import functools # noqa: F401 import io # noqa: F401
 import re # noqa: F401 import typing # noqa: F401 import typing_extensions #
 noqa: F401 import uuid # noqa: F401 import frozendict # noqa: F401 from
 newscatcherapi_client import schemas # noqa: F401 class SubscriptionResponse
 ( schemas.DictSchema ): """ This class is auto generated by Konfig (https://
-konfigthis.com) """ class MetaOapg: required = { "active", "plan_name", } class
-properties: active = schemas.BoolSchema plan_name = schemas.StrSchema
-calls_per_seconds = schemas.IntSchema usage_assigned_calls = schemas.IntSchema
-usage_remaining_calls = schemas.IntSchema historical_days = schemas.IntSchema
-__annotations__ = { "active": active, "plan_name": plan_name,
-"calls_per_seconds": calls_per_seconds, "usage_assigned_calls":
-usage_assigned_calls, "usage_remaining_calls": usage_remaining_calls,
-"historical_days": historical_days, } active: MetaOapg.properties.active
-plan_name: MetaOapg.properties.plan_name @typing.overload def __getitem__(self,
-name: typing_extensions.Literal["active"]) -> MetaOapg.properties.active: ...
+konfigthis.com) SubscriptionResponse DTO class. """ class MetaOapg: required =
+{ "active", "plan_name", } class properties: active = schemas.BoolSchema
+plan_name = schemas.StrSchema calls_per_seconds = schemas.IntSchema
+usage_assigned_calls = schemas.IntSchema usage_remaining_calls =
+schemas.IntSchema historical_days = schemas.IntSchema __annotations__ =
+{ "active": active, "plan_name": plan_name, "calls_per_seconds":
+calls_per_seconds, "usage_assigned_calls": usage_assigned_calls,
+"usage_remaining_calls": usage_remaining_calls, "historical_days":
+historical_days, } active: MetaOapg.properties.active plan_name:
+MetaOapg.properties.plan_name @typing.overload def __getitem__(self, name:
+typing_extensions.Literal["active"]) -> MetaOapg.properties.active: ...
 @typing.overload def __getitem__(self, name: typing_extensions.Literal
 ["plan_name"]) -> MetaOapg.properties.plan_name: ... @typing.overload def
 __getitem__(self, name: typing_extensions.Literal["calls_per_seconds"]) -
 > MetaOapg.properties.calls_per_seconds: ... @typing.overload def __getitem__
 (self, name: typing_extensions.Literal["usage_assigned_calls"]) -
 > MetaOapg.properties.usage_assigned_calls: ... @typing.overload def
 __getitem__(self, name: typing_extensions.Literal["usage_remaining_calls"]) -
```

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/validation_error.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/validation_error.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/validation_error.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/validation_error.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/validation_error_loc.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/validation_error_loc.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/validation_error_loc.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/validation_error_loc.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/models/__init__.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/operation_parameter_map.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/operation_parameter_map.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/__init__.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_authors/get.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_authors/get.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_authors/get.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_authors/get.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_authors/post.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_authors/post.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_authors/post.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_authors/post.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_latest_headlines/get.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_latest_headlines/get.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_latest_headlines/get.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_latest_headlines/get.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_latest_headlines/post.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_latest_headlines/post.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_latest_headlines/post.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_latest_headlines/post.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search/get.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search/get.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search/get.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search/get.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search/post.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search/post.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search/post.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search/post.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_by_link/get.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_by_link/get.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_by_link/get.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_by_link/get.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_by_link/post.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_by_link/post.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_by_link/post.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_by_link/post.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_similar/get.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_similar/get.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_similar/get.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_similar/get.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_similar/post.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_similar/post.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_similar/post.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_similar/post.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_sources/get.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_sources/get.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_sources/get.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_sources/get.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_sources/post.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_sources/post.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_sources/post.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_sources/post.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_subscription/get.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_subscription/get.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_subscription/get.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_subscription/get.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_subscription/post.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_subscription/post.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_subscription/post.pyi` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_subscription/post.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/additional_source_info.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/additional_source_info.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/author_search_request.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/author_search_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/authors_get_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/authors_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/authors_post_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/authors_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/cluster.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/cluster.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/cluster_articles.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/cluster_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/clustering_search_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/clustering_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_author_search_response_article_result.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_author_search_response_article_result.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_author_search_response_failed_search_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_author_search_response_failed_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_author_search_response_search_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_author_search_response_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_author_search_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_author_search_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_article_result.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_article_result.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_failed_search_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_failed_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_search_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_search_response_search_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_search_response_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_search_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_search_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/http_validation_error.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/latest_headlines_get_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/latest_headlines_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/latest_headlines_post_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/latest_headlines_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/latest_headlines_request.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/latest_headlines_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/latest_headlines_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/latest_headlines_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/latest_headlines_response_articles.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/latest_headlines_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/more_like_this_request.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/more_like_this_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/search_get_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/search_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/search_post_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/search_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/search_request.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/search_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/search_similar_get_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/search_similar_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/search_similar_post_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/search_similar_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/search_url_request.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/search_url_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/similar_document.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/similar_document.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/source_info.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/source_info.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/source_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/source_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/source_response_sources.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/source_response_sources.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/sources_request.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/sources_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/subscription_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/subscription_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/validation_error.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/validation_error.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/validation_error_loc.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/validation_error_loc.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/request_after_hook.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/request_after_hook.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/request_before_hook.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/request_before_hook.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/request_before_url_hook.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/request_before_url_hook.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/rest.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/schemas.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/schemas.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/additional_source_info.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/additional_source_info.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/author_search_request.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/author_search_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/authors_get_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/authors_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/authors_post_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/authors_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/cluster.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/cluster.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/cluster_articles.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/cluster_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/clustering_search_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/clustering_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_author_search_response_article_result.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_author_search_response_article_result.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_author_search_response_failed_search_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_author_search_response_failed_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_author_search_response_search_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_author_search_response_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_author_search_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_author_search_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_more_like_this_response_article_result.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_more_like_this_response_article_result.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_more_like_this_response_failed_search_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_more_like_this_response_failed_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_more_like_this_response_search_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_more_like_this_response_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_more_like_this_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_more_like_this_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_search_response_search_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_search_response_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_search_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_search_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/http_validation_error.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/latest_headlines_get_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/latest_headlines_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/latest_headlines_post_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/latest_headlines_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/latest_headlines_request.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/latest_headlines_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/latest_headlines_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/latest_headlines_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/latest_headlines_response_articles.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/latest_headlines_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/more_like_this_request.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/more_like_this_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/search_get_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/search_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/search_post_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/search_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/search_request.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/search_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/search_similar_get_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/search_similar_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/search_similar_post_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/search_similar_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/search_url_request.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/search_url_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/similar_document.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/similar_document.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/source_info.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/source_info.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/source_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/source_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/source_response_sources.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/source_response_sources.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/sources_request.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/sources_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/subscription_response.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/subscription_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/validation_error.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/validation_error.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/validation_error_loc.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/validation_error_loc.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type_util.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type_util.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/validation_metadata.py` & `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/validation_metadata.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.3/pyproject.toml` & `newscatcherapi_python_sdk-6.0.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "newscatcherapi-python-sdk"
-version = "6.0.3"
+version = "6.0.4"
 description = "Client for NewsCatcher-V3 Production API"
 authors = ["Maksym Sugonyaka <maksym@newscatcherapi.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "newscatcherapi_client"}]
 
 [tool.poetry.dependencies]
```

### Comparing `newscatcherapi_python_sdk-6.0.3/PKG-INFO` & `newscatcherapi_python_sdk-6.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: newscatcherapi-python-sdk
-Version: 6.0.3
+Version: 6.0.4
 Summary: Client for NewsCatcher-V3 Production API
 License: MIT
 Author: Maksym Sugonyaka
 Author-email: maksym@newscatcherapi.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: certifi (>=2023.7.22)
 Requires-Dist: cryptography (>=42.0.5,<43.0.0)
 Requires-Dist: frozendict (>=2.3.4,<3.0.0)
 Requires-Dist: pydantic (>=2.4.2,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: typing_extensions (>=4.3.0,<5.0.0)
@@ -24,15 +25,15 @@
 Description-Content-Type: text/markdown
 
 # newscatcherapi-python-sdk<a id="newscatcherapi-python-sdk"></a>
 
 <img src='https://uploads-ssl.webflow.com/6429857b17973b636c2195c5/646c6f1eb774ff2f2997bec5_newscatcher_.svg' width='286' height='35' /> <br>  <br>Visit our website  <a href='https://newscatcherapi.com'>https://newscatcherapi.com</a>
 
 
-[![PyPI](https://img.shields.io/badge/PyPI-v6.0.3-blue)](https://pypi.org/project/newscatcherapi-python-sdk/6.0.3)
+[![PyPI](https://img.shields.io/badge/PyPI-v6.0.4-blue)](https://pypi.org/project/newscatcherapi-python-sdk/6.0.4)
 [![README.md](https://img.shields.io/badge/README-Click%20Here-green)](https://github.com/konfig-dev/newscatcher-sdks/tree/main/v3/python#readme)
 
 ## Table of Contents<a id="table-of-contents"></a>
 
 <!-- toc -->
 
 - [Requirements](#requirements)
@@ -61,15 +62,15 @@
 ## Requirements<a id="requirements"></a>
 
 Python >=3.7
 
 ## Installation<a id="installation"></a>
 
 ```sh
-pip install newscatcherapi-python-sdk==6.0.3
+pip install newscatcherapi-python-sdk==6.0.4
 ```
 
 ## Getting Started<a id="getting-started"></a>
 
 ```python
 from pprint import pprint
 from newscatcherapi_client import Newscatcher, ApiException
```

