# Comparing `tmp/fds.sdk.StreetAccountNews-0.20.4-py3-none-any.whl.zip` & `tmp/fds.sdk.StreetAccountNews-0.40.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,70 +1,87 @@
-Zip file size: 218905 bytes, number of entries: 68
+Zip file size: 253577 bytes, number of entries: 85
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-19 09:33 fds/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-19 09:33 fds/sdk/__init__.py
--rw-r--r--  2.0 unx     2302 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/__init__.py
--rw-r--r--  2.0 unx    41311 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/api_client.py
--rw-r--r--  2.0 unx    19869 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/configuration.py
--rw-r--r--  2.0 unx     6535 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/exceptions.py
--rw-r--r--  2.0 unx    83930 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model_utils.py
--rw-r--r--  2.0 unx    15670 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/rest.py
+-rw-r--r--  2.0 unx     1527 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/__init__.py
+-rw-r--r--  2.0 unx    40536 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/api_client.py
+-rw-r--r--  2.0 unx    19088 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/configuration.py
+-rw-r--r--  2.0 unx     5760 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/exceptions.py
+-rw-r--r--  2.0 unx    83155 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model_utils.py
+-rw-r--r--  2.0 unx    14895 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/rest.py
 -rw-r--r--  2.0 unx      229 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/api/__init__.py
--rw-r--r--  2.0 unx    16694 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/api/filters_api.py
--rw-r--r--  2.0 unx    27575 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/api/headlines_api.py
--rw-r--r--  2.0 unx    44273 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/api/street_account_historical_stories_api.py
--rw-r--r--  2.0 unx    49409 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/api/views_api.py
--rw-r--r--  2.0 unx      722 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/apis/__init__.py
+-rw-r--r--  2.0 unx    82012 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/api/filters_api.py
+-rw-r--r--  2.0 unx    26993 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/api/headlines_api.py
+-rw-r--r--  2.0 unx    68780 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/api/views_api.py
+-rw-r--r--  2.0 unx      608 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/apis/__init__.py
 -rw-r--r--  2.0 unx      348 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/__init__.py
--rw-r--r--  2.0 unx    14532 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/checkstatus.py
--rw-r--r--  2.0 unx    13022 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/checkstatus_response.py
--rw-r--r--  2.0 unx    12905 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/create_edit_delete_view_response.py
--rw-r--r--  2.0 unx    13150 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/create_edit_delete_view_response_data.py
--rw-r--r--  2.0 unx    12583 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/create_edit_delete_view_response_data_message.py
--rw-r--r--  2.0 unx    12825 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/create_or_edit_view_body.py
--rw-r--r--  2.0 unx    14081 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/create_or_edit_view_body_data.py
--rw-r--r--  2.0 unx    13098 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/create_or_edit_view_tickers.py
--rw-r--r--  2.0 unx    13077 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/error.py
--rw-r--r--  2.0 unx    12850 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/error_object.py
--rw-r--r--  2.0 unx    12762 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/filter_response.py
--rw-r--r--  2.0 unx    13252 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/filter_response_data.py
--rw-r--r--  2.0 unx    14795 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/flattened_filters.py
--rw-r--r--  2.0 unx    12751 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/flattened_filters_categories_object.py
--rw-r--r--  2.0 unx    12748 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/flattened_filters_regions_object.py
--rw-r--r--  2.0 unx    12748 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/flattened_filters_sectors_object.py
--rw-r--r--  2.0 unx    12739 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/flattened_filters_topics_object.py
--rw-r--r--  2.0 unx    12923 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/flattened_filters_watchlists_object.py
--rw-r--r--  2.0 unx    14383 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/getfiles.py
--rw-r--r--  2.0 unx    12992 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/getfiles_response.py
--rw-r--r--  2.0 unx    12534 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/is_partial_one.py
--rw-r--r--  2.0 unx    13076 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/meta_one.py
--rw-r--r--  2.0 unx    14200 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/pagination_one.py
--rw-r--r--  2.0 unx    12973 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/requestfiles_response.py
--rw-r--r--  2.0 unx    13200 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/sa_headlines_request.py
--rw-r--r--  2.0 unx    13262 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/sa_headlines_request_by_view.py
--rw-r--r--  2.0 unx    12939 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/sa_headlines_request_by_view_data.py
--rw-r--r--  2.0 unx    14419 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/sa_headlines_request_data.py
--rw-r--r--  2.0 unx    13492 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/sa_headlines_request_data_search_date.py
--rw-r--r--  2.0 unx    12916 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/sa_headlines_request_meta.py
--rw-r--r--  2.0 unx    13159 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/sa_headlines_request_meta_pagination.py
--rw-r--r--  2.0 unx    13218 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/sa_headlines_request_tickers_object.py
--rw-r--r--  2.0 unx    13130 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/search_response.py
--rw-r--r--  2.0 unx    14251 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/search_response_array_object.py
--rw-r--r--  2.0 unx    12845 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/search_response_data.py
--rw-r--r--  2.0 unx    13092 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/search_response_meta.py
--rw-r--r--  2.0 unx    12804 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/search_response_meta_pagination.py
--rw-r--r--  2.0 unx    12782 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/street_account_status.py
--rw-r--r--  2.0 unx    14833 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/structured_filters.py
--rw-r--r--  2.0 unx    13304 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/structured_filters_categories_object.py
--rw-r--r--  2.0 unx    12748 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/structured_filters_children_object.py
--rw-r--r--  2.0 unx    12751 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/structured_filters_regions_object.py
--rw-r--r--  2.0 unx    13307 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/structured_filters_sectors_object.py
--rw-r--r--  2.0 unx    13292 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/structured_filters_topics_object.py
--rw-r--r--  2.0 unx    12926 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/structured_filters_watchlists_object.py
--rw-r--r--  2.0 unx    12691 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/views.py
--rw-r--r--  2.0 unx    13738 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/views_object.py
--rw-r--r--  2.0 unx     4739 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/models/__init__.py
--rw-r--r--  2.0 unx    11358 b- defN 24-Apr-19 09:33 fds.sdk.StreetAccountNews-0.20.4.dist-info/LICENSE
--rw-r--r--  2.0 unx    20925 b- defN 24-Apr-19 09:33 fds.sdk.StreetAccountNews-0.20.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-19 09:33 fds.sdk.StreetAccountNews-0.20.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 24-Apr-19 09:33 fds.sdk.StreetAccountNews-0.20.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     7554 b- defN 24-Apr-19 09:33 fds.sdk.StreetAccountNews-0.20.4.dist-info/RECORD
-68 files, 975637 bytes uncompressed, 206337 bytes compressed:  78.9%
+-rw-r--r--  2.0 unx    12050 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/create_or_edit_view_body.py
+-rw-r--r--  2.0 unx    14298 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/create_or_edit_view_body_data.py
+-rw-r--r--  2.0 unx    12323 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/create_or_edit_view_tickers.py
+-rw-r--r--  2.0 unx    12028 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/create_view_response.py
+-rw-r--r--  2.0 unx    11819 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/create_view_response_data.py
+-rw-r--r--  2.0 unx    11988 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/delete_view_body.py
+-rw-r--r--  2.0 unx    11819 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/delete_view_body_data.py
+-rw-r--r--  2.0 unx    11926 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/error.py
+-rw-r--r--  2.0 unx    12075 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/error_object.py
+-rw-r--r--  2.0 unx    12088 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/filter_categories_response.py
+-rw-r--r--  2.0 unx    12571 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/filter_categories_response_data.py
+-rw-r--r--  2.0 unx    12058 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/filter_regions_response.py
+-rw-r--r--  2.0 unx    12520 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/filter_regions_response_data.py
+-rw-r--r--  2.0 unx    11987 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/filter_response.py
+-rw-r--r--  2.0 unx    12399 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/filter_response_data.py
+-rw-r--r--  2.0 unx    12058 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/filter_sectors_response.py
+-rw-r--r--  2.0 unx    12520 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/filter_sectors_response_data.py
+-rw-r--r--  2.0 unx    12038 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/filter_topic_response.py
+-rw-r--r--  2.0 unx    12500 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/filter_topic_response_data.py
+-rw-r--r--  2.0 unx    12088 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/filter_watchlists_response.py
+-rw-r--r--  2.0 unx    12571 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/filter_watchlists_response_data.py
+-rw-r--r--  2.0 unx    14020 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/flattened_filters.py
+-rw-r--r--  2.0 unx    12158 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/flattened_filters_categories.py
+-rw-r--r--  2.0 unx    12164 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/flattened_filters_categories_object.py
+-rw-r--r--  2.0 unx    12113 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/flattened_filters_regions.py
+-rw-r--r--  2.0 unx    12161 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/flattened_filters_regions_object.py
+-rw-r--r--  2.0 unx    12113 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/flattened_filters_sectors.py
+-rw-r--r--  2.0 unx    12169 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/flattened_filters_sectors_object.py
+-rw-r--r--  2.0 unx    12098 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/flattened_filters_topics.py
+-rw-r--r--  2.0 unx    12138 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/flattened_filters_topics_object.py
+-rw-r--r--  2.0 unx    12158 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/flattened_filters_watchlists.py
+-rw-r--r--  2.0 unx    12336 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/flattened_filters_watchlists_object.py
+-rw-r--r--  2.0 unx    12389 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/headlines_request.py
+-rw-r--r--  2.0 unx    12495 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/headlines_request_by_view.py
+-rw-r--r--  2.0 unx    13266 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/headlines_request_by_view_data.py
+-rw-r--r--  2.0 unx    12138 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/headlines_request_by_view_meta.py
+-rw-r--r--  2.0 unx    16799 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/headlines_request_data.py
+-rw-r--r--  2.0 unx    12741 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/headlines_request_data_search_time.py
+-rw-r--r--  2.0 unx    12946 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/headlines_request_meta.py
+-rw-r--r--  2.0 unx    12378 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/headlines_request_meta_pagination.py
+-rw-r--r--  2.0 unx    12517 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/headlines_request_tickers_object.py
+-rw-r--r--  2.0 unx    12441 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/headlines_response.py
+-rw-r--r--  2.0 unx    12533 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/headlines_response_meta.py
+-rw-r--r--  2.0 unx    12038 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/headlines_response_meta_pagination.py
+-rw-r--r--  2.0 unx    11998 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/quick_alerts_body.py
+-rw-r--r--  2.0 unx    11852 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/quick_alerts_body_data.py
+-rw-r--r--  2.0 unx    12010 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/quick_alerts_response.py
+-rw-r--r--  2.0 unx    13853 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/search_response_array_object.py
+-rw-r--r--  2.0 unx    14058 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/structured_filters.py
+-rw-r--r--  2.0 unx    12168 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/structured_filters_categories.py
+-rw-r--r--  2.0 unx    12716 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/structured_filters_categories_object.py
+-rw-r--r--  2.0 unx    12057 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/structured_filters_children_object_categories.py
+-rw-r--r--  2.0 unx    12048 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/structured_filters_children_object_regions.py
+-rw-r--r--  2.0 unx    12054 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/structured_filters_children_object_sectors.py
+-rw-r--r--  2.0 unx    12045 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/structured_filters_children_object_topics.py
+-rw-r--r--  2.0 unx    12123 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/structured_filters_regions.py
+-rw-r--r--  2.0 unx    12682 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/structured_filters_regions_object.py
+-rw-r--r--  2.0 unx    12123 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/structured_filters_sectors.py
+-rw-r--r--  2.0 unx    12985 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/structured_filters_sectors_object.py
+-rw-r--r--  2.0 unx    12108 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/structured_filters_topics.py
+-rw-r--r--  2.0 unx    12664 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/structured_filters_topics_object.py
+-rw-r--r--  2.0 unx    12168 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/structured_filters_watchlists.py
+-rw-r--r--  2.0 unx    12339 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/structured_filters_watchlists_object.py
+-rw-r--r--  2.0 unx    11916 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/views.py
+-rw-r--r--  2.0 unx    13780 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/model/views_object.py
+-rw-r--r--  2.0 unx     6628 b- defN 24-Apr-19 09:33 fds/sdk/StreetAccountNews/models/__init__.py
+-rw-r--r--  2.0 unx    11358 b- defN 24-Apr-19 09:33 fds.sdk.StreetAccountNews-0.40.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    23664 b- defN 24-Apr-19 09:33 fds.sdk.StreetAccountNews-0.40.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-19 09:33 fds.sdk.StreetAccountNews-0.40.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 24-Apr-19 09:33 fds.sdk.StreetAccountNews-0.40.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     9653 b- defN 24-Apr-19 09:33 fds.sdk.StreetAccountNews-0.40.0.dist-info/RECORD
+85 files, 1205110 bytes uncompressed, 237491 bytes compressed:  80.3%
```

## zipnote {}

```diff
@@ -27,179 +27,230 @@
 
 Filename: fds/sdk/StreetAccountNews/api/filters_api.py
 Comment: 
 
 Filename: fds/sdk/StreetAccountNews/api/headlines_api.py
 Comment: 
 
-Filename: fds/sdk/StreetAccountNews/api/street_account_historical_stories_api.py
-Comment: 
-
 Filename: fds/sdk/StreetAccountNews/api/views_api.py
 Comment: 
 
 Filename: fds/sdk/StreetAccountNews/apis/__init__.py
 Comment: 
 
 Filename: fds/sdk/StreetAccountNews/model/__init__.py
 Comment: 
 
-Filename: fds/sdk/StreetAccountNews/model/checkstatus.py
+Filename: fds/sdk/StreetAccountNews/model/create_or_edit_view_body.py
 Comment: 
 
-Filename: fds/sdk/StreetAccountNews/model/checkstatus_response.py
+Filename: fds/sdk/StreetAccountNews/model/create_or_edit_view_body_data.py
 Comment: 
 
-Filename: fds/sdk/StreetAccountNews/model/create_edit_delete_view_response.py
+Filename: fds/sdk/StreetAccountNews/model/create_or_edit_view_tickers.py
 Comment: 
 
-Filename: fds/sdk/StreetAccountNews/model/create_edit_delete_view_response_data.py
+Filename: fds/sdk/StreetAccountNews/model/create_view_response.py
 Comment: 
 
-Filename: fds/sdk/StreetAccountNews/model/create_edit_delete_view_response_data_message.py
+Filename: fds/sdk/StreetAccountNews/model/create_view_response_data.py
 Comment: 
 
-Filename: fds/sdk/StreetAccountNews/model/create_or_edit_view_body.py
+Filename: fds/sdk/StreetAccountNews/model/delete_view_body.py
 Comment: 
 
-Filename: fds/sdk/StreetAccountNews/model/create_or_edit_view_body_data.py
-Comment: 
-
-Filename: fds/sdk/StreetAccountNews/model/create_or_edit_view_tickers.py
+Filename: fds/sdk/StreetAccountNews/model/delete_view_body_data.py
 Comment: 
 
 Filename: fds/sdk/StreetAccountNews/model/error.py
 Comment: 
 
 Filename: fds/sdk/StreetAccountNews/model/error_object.py
 Comment: 
 
+Filename: fds/sdk/StreetAccountNews/model/filter_categories_response.py
+Comment: 
+
+Filename: fds/sdk/StreetAccountNews/model/filter_categories_response_data.py
+Comment: 
+
+Filename: fds/sdk/StreetAccountNews/model/filter_regions_response.py
+Comment: 
+
+Filename: fds/sdk/StreetAccountNews/model/filter_regions_response_data.py
+Comment: 
+
 Filename: fds/sdk/StreetAccountNews/model/filter_response.py
 Comment: 
 
 Filename: fds/sdk/StreetAccountNews/model/filter_response_data.py
 Comment: 
 
+Filename: fds/sdk/StreetAccountNews/model/filter_sectors_response.py
+Comment: 
+
+Filename: fds/sdk/StreetAccountNews/model/filter_sectors_response_data.py
+Comment: 
+
+Filename: fds/sdk/StreetAccountNews/model/filter_topic_response.py
+Comment: 
+
+Filename: fds/sdk/StreetAccountNews/model/filter_topic_response_data.py
+Comment: 
+
+Filename: fds/sdk/StreetAccountNews/model/filter_watchlists_response.py
+Comment: 
+
+Filename: fds/sdk/StreetAccountNews/model/filter_watchlists_response_data.py
+Comment: 
+
 Filename: fds/sdk/StreetAccountNews/model/flattened_filters.py
 Comment: 
 
+Filename: fds/sdk/StreetAccountNews/model/flattened_filters_categories.py
+Comment: 
+
 Filename: fds/sdk/StreetAccountNews/model/flattened_filters_categories_object.py
 Comment: 
 
+Filename: fds/sdk/StreetAccountNews/model/flattened_filters_regions.py
+Comment: 
+
 Filename: fds/sdk/StreetAccountNews/model/flattened_filters_regions_object.py
 Comment: 
 
+Filename: fds/sdk/StreetAccountNews/model/flattened_filters_sectors.py
+Comment: 
+
 Filename: fds/sdk/StreetAccountNews/model/flattened_filters_sectors_object.py
 Comment: 
 
+Filename: fds/sdk/StreetAccountNews/model/flattened_filters_topics.py
+Comment: 
+
 Filename: fds/sdk/StreetAccountNews/model/flattened_filters_topics_object.py
 Comment: 
 
+Filename: fds/sdk/StreetAccountNews/model/flattened_filters_watchlists.py
+Comment: 
+
 Filename: fds/sdk/StreetAccountNews/model/flattened_filters_watchlists_object.py
 Comment: 
 
-Filename: fds/sdk/StreetAccountNews/model/getfiles.py
+Filename: fds/sdk/StreetAccountNews/model/headlines_request.py
 Comment: 
 
-Filename: fds/sdk/StreetAccountNews/model/getfiles_response.py
+Filename: fds/sdk/StreetAccountNews/model/headlines_request_by_view.py
 Comment: 
 
-Filename: fds/sdk/StreetAccountNews/model/is_partial_one.py
+Filename: fds/sdk/StreetAccountNews/model/headlines_request_by_view_data.py
 Comment: 
 
-Filename: fds/sdk/StreetAccountNews/model/meta_one.py
+Filename: fds/sdk/StreetAccountNews/model/headlines_request_by_view_meta.py
 Comment: 
 
-Filename: fds/sdk/StreetAccountNews/model/pagination_one.py
+Filename: fds/sdk/StreetAccountNews/model/headlines_request_data.py
 Comment: 
 
-Filename: fds/sdk/StreetAccountNews/model/requestfiles_response.py
+Filename: fds/sdk/StreetAccountNews/model/headlines_request_data_search_time.py
 Comment: 
 
-Filename: fds/sdk/StreetAccountNews/model/sa_headlines_request.py
+Filename: fds/sdk/StreetAccountNews/model/headlines_request_meta.py
 Comment: 
 
-Filename: fds/sdk/StreetAccountNews/model/sa_headlines_request_by_view.py
+Filename: fds/sdk/StreetAccountNews/model/headlines_request_meta_pagination.py
 Comment: 
 
-Filename: fds/sdk/StreetAccountNews/model/sa_headlines_request_by_view_data.py
+Filename: fds/sdk/StreetAccountNews/model/headlines_request_tickers_object.py
 Comment: 
 
-Filename: fds/sdk/StreetAccountNews/model/sa_headlines_request_data.py
+Filename: fds/sdk/StreetAccountNews/model/headlines_response.py
 Comment: 
 
-Filename: fds/sdk/StreetAccountNews/model/sa_headlines_request_data_search_date.py
+Filename: fds/sdk/StreetAccountNews/model/headlines_response_meta.py
 Comment: 
 
-Filename: fds/sdk/StreetAccountNews/model/sa_headlines_request_meta.py
+Filename: fds/sdk/StreetAccountNews/model/headlines_response_meta_pagination.py
 Comment: 
 
-Filename: fds/sdk/StreetAccountNews/model/sa_headlines_request_meta_pagination.py
+Filename: fds/sdk/StreetAccountNews/model/quick_alerts_body.py
 Comment: 
 
-Filename: fds/sdk/StreetAccountNews/model/sa_headlines_request_tickers_object.py
+Filename: fds/sdk/StreetAccountNews/model/quick_alerts_body_data.py
 Comment: 
 
-Filename: fds/sdk/StreetAccountNews/model/search_response.py
+Filename: fds/sdk/StreetAccountNews/model/quick_alerts_response.py
 Comment: 
 
 Filename: fds/sdk/StreetAccountNews/model/search_response_array_object.py
 Comment: 
 
-Filename: fds/sdk/StreetAccountNews/model/search_response_data.py
+Filename: fds/sdk/StreetAccountNews/model/structured_filters.py
 Comment: 
 
-Filename: fds/sdk/StreetAccountNews/model/search_response_meta.py
+Filename: fds/sdk/StreetAccountNews/model/structured_filters_categories.py
 Comment: 
 
-Filename: fds/sdk/StreetAccountNews/model/search_response_meta_pagination.py
+Filename: fds/sdk/StreetAccountNews/model/structured_filters_categories_object.py
 Comment: 
 
-Filename: fds/sdk/StreetAccountNews/model/street_account_status.py
+Filename: fds/sdk/StreetAccountNews/model/structured_filters_children_object_categories.py
 Comment: 
 
-Filename: fds/sdk/StreetAccountNews/model/structured_filters.py
+Filename: fds/sdk/StreetAccountNews/model/structured_filters_children_object_regions.py
 Comment: 
 
-Filename: fds/sdk/StreetAccountNews/model/structured_filters_categories_object.py
+Filename: fds/sdk/StreetAccountNews/model/structured_filters_children_object_sectors.py
+Comment: 
+
+Filename: fds/sdk/StreetAccountNews/model/structured_filters_children_object_topics.py
 Comment: 
 
-Filename: fds/sdk/StreetAccountNews/model/structured_filters_children_object.py
+Filename: fds/sdk/StreetAccountNews/model/structured_filters_regions.py
 Comment: 
 
 Filename: fds/sdk/StreetAccountNews/model/structured_filters_regions_object.py
 Comment: 
 
+Filename: fds/sdk/StreetAccountNews/model/structured_filters_sectors.py
+Comment: 
+
 Filename: fds/sdk/StreetAccountNews/model/structured_filters_sectors_object.py
 Comment: 
 
+Filename: fds/sdk/StreetAccountNews/model/structured_filters_topics.py
+Comment: 
+
 Filename: fds/sdk/StreetAccountNews/model/structured_filters_topics_object.py
 Comment: 
 
+Filename: fds/sdk/StreetAccountNews/model/structured_filters_watchlists.py
+Comment: 
+
 Filename: fds/sdk/StreetAccountNews/model/structured_filters_watchlists_object.py
 Comment: 
 
 Filename: fds/sdk/StreetAccountNews/model/views.py
 Comment: 
 
 Filename: fds/sdk/StreetAccountNews/model/views_object.py
 Comment: 
 
 Filename: fds/sdk/StreetAccountNews/models/__init__.py
 Comment: 
 
-Filename: fds.sdk.StreetAccountNews-0.20.4.dist-info/LICENSE
+Filename: fds.sdk.StreetAccountNews-0.40.0.dist-info/LICENSE
 Comment: 
 
-Filename: fds.sdk.StreetAccountNews-0.20.4.dist-info/METADATA
+Filename: fds.sdk.StreetAccountNews-0.40.0.dist-info/METADATA
 Comment: 
 
-Filename: fds.sdk.StreetAccountNews-0.20.4.dist-info/WHEEL
+Filename: fds.sdk.StreetAccountNews-0.40.0.dist-info/WHEEL
 Comment: 
 
-Filename: fds.sdk.StreetAccountNews-0.20.4.dist-info/top_level.txt
+Filename: fds.sdk.StreetAccountNews-0.40.0.dist-info/top_level.txt
 Comment: 
 
-Filename: fds.sdk.StreetAccountNews-0.20.4.dist-info/RECORD
+Filename: fds.sdk.StreetAccountNews-0.40.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fds/sdk/StreetAccountNews/__init__.py

```diff
@@ -1,21 +1,21 @@
 # flake8: noqa
 
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.20.4"
+__version__ = "0.40.0"
 
 # import ApiClient
 from fds.sdk.StreetAccountNews.api_client import ApiClient
 
 # import Configuration
 from fds.sdk.StreetAccountNews.configuration import Configuration
```

## fds/sdk/StreetAccountNews/api_client.py

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
@@ -102,15 +102,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'fds-sdk/python/StreetAccountNews/0.20.4'
+        self.user_agent = 'fds-sdk/python/StreetAccountNews/0.40.0'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

## fds/sdk/StreetAccountNews/configuration.py

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import copy
 import logging
@@ -116,15 +116,15 @@
                  server_index=None, server_variables=None,
                  server_operation_index=None, server_operation_variables=None,
                  ssl_ca_cert=None, verify_ssl=True,
                  proxy=None, proxy_headers=None,
                  ):
         """Constructor
         """
-        self._base_path = "https://api.factset.com/research/news/v0" if host is None else host
+        self._base_path = "https://api.factset.com/streetaccount/v1" if host is None else host
         """Default Base url
         """
         self.server_index = 0 if server_index is None and host is None else server_index
         self.server_operation_index = server_operation_index or {}
         """Default server index
         """
         self.server_variables = server_variables or {}
@@ -425,27 +425,27 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.0\n"\
-               "SDK Package Version: 0.20.4".\
+               "Version of the API: 1.0.0\n"\
+               "SDK Package Version: 0.40.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
         return [
             {
-                'url': "https://api.factset.com/research/news/v0",
-                'description': "No description provided",
+                'url': "https://api.factset.com/streetaccount/v1",
+                'description': "Production Server",
             }
         ]
 
     def get_host_from_settings(self, index, variables=None, servers=None):
         """Gets host URL based on the index and variables
         :param index: array index of the host settings
         :param variables: hash of variable and the corresponding value
```

## fds/sdk/StreetAccountNews/exceptions.py

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 
 class OpenApiException(Exception):
```

## fds/sdk/StreetAccountNews/model_utils.py

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
```

## fds/sdk/StreetAccountNews/rest.py

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
```

## fds/sdk/StreetAccountNews/api/filters_api.py

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -22,15 +22,20 @@
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
 from fds.sdk.StreetAccountNews.exceptions import ApiException
 from fds.sdk.StreetAccountNews.model.error import Error
+from fds.sdk.StreetAccountNews.model.filter_categories_response import FilterCategoriesResponse
+from fds.sdk.StreetAccountNews.model.filter_regions_response import FilterRegionsResponse
 from fds.sdk.StreetAccountNews.model.filter_response import FilterResponse
+from fds.sdk.StreetAccountNews.model.filter_sectors_response import FilterSectorsResponse
+from fds.sdk.StreetAccountNews.model.filter_topic_response import FilterTopicResponse
+from fds.sdk.StreetAccountNews.model.filter_watchlists_response import FilterWatchlistsResponse
 
 
 
 
 
 class FiltersApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
@@ -50,52 +55,389 @@
                   { 200: (FilterResponse,), 400: (Error,), 401: (Error,), 404: (Error,),  },
                   None
                 ),
                 'auth': [
                     'FactSetApiKey',
                     'FactSetOAuth2'
                 ],
-                'endpoint_path': '/streetaccount/filters',
+                'endpoint_path': '/filters',
                 'operation_id': 'get_street_account_filters',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'structured',
-                    'flattened',
+                    'attributes',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
+                    'attributes',
                 ],
                 'validation': [
+                    'attributes',
                 ]
             },
             root_map={
                 'validations': {
+                    ('attributes',): {
+
+                        'max_items': 2,
+                    },
+                },
+                'allowed_values': {
+                    ('attributes',): {
+
+                        "STRUCTURED": "structured",
+                        "FLATTENED": "flattened"
+                    },
+                },
+                'openapi_types': {
+                    'attributes':
+                        ([str],),
+                },
+                'attribute_map': {
+                    'attributes': '_attributes',
+                },
+                'location_map': {
+                    'attributes': 'query',
+                },
+                'collection_format_map': {
+                    'attributes': 'csv',
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+
+        self.get_street_account_filters_categories_endpoint = _Endpoint(
+            settings={
+                'response_type': (
+                  { 200: (FilterCategoriesResponse,), 400: (Error,), 401: (Error,), 404: (Error,),  },
+                  None
+                ),
+                'auth': [
+                    'FactSetApiKey',
+                    'FactSetOAuth2'
+                ],
+                'endpoint_path': '/filters/categories',
+                'operation_id': 'get_street_account_filters_categories',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'attributes',
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                    'attributes',
+                ],
+                'validation': [
+                    'attributes',
+                ]
+            },
+            root_map={
+                'validations': {
+                    ('attributes',): {
+
+                        'max_items': 2,
+                    },
+                },
+                'allowed_values': {
+                    ('attributes',): {
+
+                        "STRUCTURED": "structured",
+                        "FLATTENED": "flattened"
+                    },
+                },
+                'openapi_types': {
+                    'attributes':
+                        ([str],),
+                },
+                'attribute_map': {
+                    'attributes': '_attributes',
+                },
+                'location_map': {
+                    'attributes': 'query',
+                },
+                'collection_format_map': {
+                    'attributes': 'csv',
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+
+        self.get_street_account_filters_regions_endpoint = _Endpoint(
+            settings={
+                'response_type': (
+                  { 200: (FilterRegionsResponse,), 400: (Error,), 401: (Error,), 404: (Error,),  },
+                  None
+                ),
+                'auth': [
+                    'FactSetApiKey',
+                    'FactSetOAuth2'
+                ],
+                'endpoint_path': '/filters/regions',
+                'operation_id': 'get_street_account_filters_regions',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'attributes',
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                    'attributes',
+                ],
+                'validation': [
+                    'attributes',
+                ]
+            },
+            root_map={
+                'validations': {
+                    ('attributes',): {
+
+                        'max_items': 2,
+                    },
                 },
                 'allowed_values': {
+                    ('attributes',): {
+
+                        "STRUCTURED": "structured",
+                        "FLATTENED": "flattened"
+                    },
                 },
                 'openapi_types': {
-                    'structured':
-                        (bool,),
-                    'flattened':
-                        (bool,),
+                    'attributes':
+                        ([str],),
                 },
                 'attribute_map': {
-                    'structured': 'structured',
-                    'flattened': 'flattened',
+                    'attributes': '_attributes',
                 },
                 'location_map': {
-                    'structured': 'query',
-                    'flattened': 'query',
+                    'attributes': 'query',
                 },
                 'collection_format_map': {
+                    'attributes': 'csv',
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+
+        self.get_street_account_filters_sectors_endpoint = _Endpoint(
+            settings={
+                'response_type': (
+                  { 200: (FilterSectorsResponse,), 400: (Error,), 401: (Error,), 404: (Error,),  },
+                  None
+                ),
+                'auth': [
+                    'FactSetApiKey',
+                    'FactSetOAuth2'
+                ],
+                'endpoint_path': '/filters/sectors',
+                'operation_id': 'get_street_account_filters_sectors',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'attributes',
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                    'attributes',
+                ],
+                'validation': [
+                    'attributes',
+                ]
+            },
+            root_map={
+                'validations': {
+                    ('attributes',): {
+
+                        'max_items': 2,
+                    },
+                },
+                'allowed_values': {
+                    ('attributes',): {
+
+                        "STRUCTURED": "structured",
+                        "FLATTENED": "flattened"
+                    },
+                },
+                'openapi_types': {
+                    'attributes':
+                        ([str],),
+                },
+                'attribute_map': {
+                    'attributes': '_attributes',
+                },
+                'location_map': {
+                    'attributes': 'query',
+                },
+                'collection_format_map': {
+                    'attributes': 'csv',
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+
+        self.get_street_account_filters_topics_endpoint = _Endpoint(
+            settings={
+                'response_type': (
+                  { 200: (FilterTopicResponse,), 400: (Error,), 401: (Error,), 404: (Error,),  },
+                  None
+                ),
+                'auth': [
+                    'FactSetApiKey',
+                    'FactSetOAuth2'
+                ],
+                'endpoint_path': '/filters/topics',
+                'operation_id': 'get_street_account_filters_topics',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'attributes',
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                    'attributes',
+                ],
+                'validation': [
+                    'attributes',
+                ]
+            },
+            root_map={
+                'validations': {
+                    ('attributes',): {
+
+                        'max_items': 2,
+                    },
+                },
+                'allowed_values': {
+                    ('attributes',): {
+
+                        "STRUCTURED": "structured",
+                        "FLATTENED": "flattened"
+                    },
+                },
+                'openapi_types': {
+                    'attributes':
+                        ([str],),
+                },
+                'attribute_map': {
+                    'attributes': '_attributes',
+                },
+                'location_map': {
+                    'attributes': 'query',
+                },
+                'collection_format_map': {
+                    'attributes': 'csv',
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+
+        self.get_street_account_filters_watchlists_endpoint = _Endpoint(
+            settings={
+                'response_type': (
+                  { 200: (FilterWatchlistsResponse,), 400: (Error,), 401: (Error,), 404: (Error,),  },
+                  None
+                ),
+                'auth': [
+                    'FactSetApiKey',
+                    'FactSetOAuth2'
+                ],
+                'endpoint_path': '/filters/watchlists',
+                'operation_id': 'get_street_account_filters_watchlists',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'attributes',
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                    'attributes',
+                ],
+                'validation': [
+                    'attributes',
+                ]
+            },
+            root_map={
+                'validations': {
+                    ('attributes',): {
+
+                        'max_items': 2,
+                    },
+                },
+                'allowed_values': {
+                    ('attributes',): {
+
+                        "STRUCTURED": "structured",
+                        "FLATTENED": "flattened"
+                    },
+                },
+                'openapi_types': {
+                    'attributes':
+                        ([str],),
+                },
+                'attribute_map': {
+                    'attributes': '_attributes',
+                },
+                'location_map': {
+                    'attributes': 'query',
+                },
+                'collection_format_map': {
+                    'attributes': 'csv',
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
@@ -119,21 +461,20 @@
 
     def get_street_account_filters(
         self,
         **kwargs
     ) -> FilterResponse:
         """Retrieve all StreetAccount filters  # noqa: E501
 
-        Add StreetAccount filters (watchlists, company filters, market topics, regions and sectors) to filter down StreetAccount headlines by the relevant categories. Set the structured and/or flattened flag. If structured flag is set, parent and child filter information will be returned. If flattened flag is set, flattened filters will be returned which can be used with the headlines and createView endpoints. Both flags can be set to return both sets of filters.  If no params are provided it will return both  # noqa: E501
+        If structured flag is set, parent and child filter information will be returned. If flattened flag is set, flattened filters will be returned which can be used with the headlines and createView endpoints. Both flags can be set to return both sets of filters.  If no params are provided it will return both.  # noqa: E501
         This method makes a synchronous HTTP request. Returns the http data only
 
 
         Keyword Args:
-            structured (bool): Pass structured to generate a structured view of the available filters.. [optional]
-            flattened (bool): Pass flattened to generate a structured view of the available filters.. [optional]
+            attributes ([str]): Pass a list of filters to return the respective type of filter. Accepted list values are \"structured\" and/or \"flattened\". If no _atrributes are specified, all filters will be returned in the response (this is the default response). . [optional]
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True. NOTE: if this API returns a file, it is the responsibility
                 of the caller to close the file stream.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -163,21 +504,20 @@
 
     def get_street_account_filters_with_http_info(
         self,
         **kwargs
     ) -> typing.Tuple[FilterResponse, int, typing.MutableMapping]:
         """Retrieve all StreetAccount filters  # noqa: E501
 
-        Add StreetAccount filters (watchlists, company filters, market topics, regions and sectors) to filter down StreetAccount headlines by the relevant categories. Set the structured and/or flattened flag. If structured flag is set, parent and child filter information will be returned. If flattened flag is set, flattened filters will be returned which can be used with the headlines and createView endpoints. Both flags can be set to return both sets of filters.  If no params are provided it will return both  # noqa: E501
+        If structured flag is set, parent and child filter information will be returned. If flattened flag is set, flattened filters will be returned which can be used with the headlines and createView endpoints. Both flags can be set to return both sets of filters.  If no params are provided it will return both.  # noqa: E501
         This method makes a synchronous HTTP request. Returns http data, http status and headers
 
 
         Keyword Args:
-            structured (bool): Pass structured to generate a structured view of the available filters.. [optional]
-            flattened (bool): Pass flattened to generate a structured view of the available filters.. [optional]
+            attributes ([str]): Pass a list of filters to return the respective type of filter. Accepted list values are \"structured\" and/or \"flattened\". If no _atrributes are specified, all filters will be returned in the response (this is the default response). . [optional]
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True. NOTE: if this API returns a file, it is the responsibility
                 of the caller to close the file stream.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -211,21 +551,20 @@
 
     def get_street_account_filters_async(
         self,
         **kwargs
     ) -> "ApplyResult[FilterResponse]":
         """Retrieve all StreetAccount filters  # noqa: E501
 
-        Add StreetAccount filters (watchlists, company filters, market topics, regions and sectors) to filter down StreetAccount headlines by the relevant categories. Set the structured and/or flattened flag. If structured flag is set, parent and child filter information will be returned. If flattened flag is set, flattened filters will be returned which can be used with the headlines and createView endpoints. Both flags can be set to return both sets of filters.  If no params are provided it will return both  # noqa: E501
+        If structured flag is set, parent and child filter information will be returned. If flattened flag is set, flattened filters will be returned which can be used with the headlines and createView endpoints. Both flags can be set to return both sets of filters.  If no params are provided it will return both.  # noqa: E501
         This method makes a asynchronous HTTP request. Returns the http data, wrapped in ApplyResult
 
 
         Keyword Args:
-            structured (bool): Pass structured to generate a structured view of the available filters.. [optional]
-            flattened (bool): Pass flattened to generate a structured view of the available filters.. [optional]
+            attributes ([str]): Pass a list of filters to return the respective type of filter. Accepted list values are \"structured\" and/or \"flattened\". If no _atrributes are specified, all filters will be returned in the response (this is the default response). . [optional]
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True. NOTE: if this API returns a file, it is the responsibility
                 of the caller to close the file stream.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -254,21 +593,20 @@
 
     def get_street_account_filters_with_http_info_async(
         self,
         **kwargs
     ) -> "ApplyResult[typing.Tuple[FilterResponse, int, typing.MutableMapping]]":
         """Retrieve all StreetAccount filters  # noqa: E501
 
-        Add StreetAccount filters (watchlists, company filters, market topics, regions and sectors) to filter down StreetAccount headlines by the relevant categories. Set the structured and/or flattened flag. If structured flag is set, parent and child filter information will be returned. If flattened flag is set, flattened filters will be returned which can be used with the headlines and createView endpoints. Both flags can be set to return both sets of filters.  If no params are provided it will return both  # noqa: E501
+        If structured flag is set, parent and child filter information will be returned. If flattened flag is set, flattened filters will be returned which can be used with the headlines and createView endpoints. Both flags can be set to return both sets of filters.  If no params are provided it will return both.  # noqa: E501
         This method makes a asynchronous HTTP request. Returns http data, http status and headers, wrapped in ApplyResult
 
 
         Keyword Args:
-            structured (bool): Pass structured to generate a structured view of the available filters.. [optional]
-            flattened (bool): Pass flattened to generate a structured view of the available filters.. [optional]
+            attributes ([str]): Pass a list of filters to return the respective type of filter. Accepted list values are \"structured\" and/or \"flattened\". If no _atrributes are specified, all filters will be returned in the response (this is the default response). . [optional]
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True. NOTE: if this API returns a file, it is the responsibility
                 of the caller to close the file stream.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -292,7 +630,882 @@
         Returns:
             ApplyResult[(FilterResponse, int, typing.Dict)]
         """
         self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=True)
         return self.get_street_account_filters_endpoint.call_with_http_info(**kwargs)
 
 
+    def get_street_account_filters_categories(
+        self,
+        **kwargs
+    ) -> FilterCategoriesResponse:
+        """Retrieve all StreetAccount filter categories  # noqa: E501
+
+        If structured flag is set, parent and child filter information will be returned. If flattened flag is set, flattened filters will be returned which can be used with the headlines and createView endpoints. Both flags can be set to return both sets of filters.  If no params are provided it will return both.  # noqa: E501
+        This method makes a synchronous HTTP request. Returns the http data only
+
+
+        Keyword Args:
+            attributes ([str]): Pass a list of filters to return the respective type of filter categories. Accepted list values are \"structured\" and/or \"flattened\". If no _atrributes are specified, all filters will be returned in the response (this is the default response). . [optional]
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True. NOTE: if this API returns a file, it is the responsibility
+                of the caller to close the file stream.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+        Returns:
+            FilterCategoriesResponse
+                Response Object
+        """
+        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=False)
+        return self.get_street_account_filters_categories_endpoint.call_with_http_info(**kwargs)
+
+    def get_street_account_filters_categories_with_http_info(
+        self,
+        **kwargs
+    ) -> typing.Tuple[FilterCategoriesResponse, int, typing.MutableMapping]:
+        """Retrieve all StreetAccount filter categories  # noqa: E501
+
+        If structured flag is set, parent and child filter information will be returned. If flattened flag is set, flattened filters will be returned which can be used with the headlines and createView endpoints. Both flags can be set to return both sets of filters.  If no params are provided it will return both.  # noqa: E501
+        This method makes a synchronous HTTP request. Returns http data, http status and headers
+
+
+        Keyword Args:
+            attributes ([str]): Pass a list of filters to return the respective type of filter categories. Accepted list values are \"structured\" and/or \"flattened\". If no _atrributes are specified, all filters will be returned in the response (this is the default response). . [optional]
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True. NOTE: if this API returns a file, it is the responsibility
+                of the caller to close the file stream.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+        Returns:
+            FilterCategoriesResponse
+                Response Object
+            int
+                Http Status Code
+            dict
+                Dictionary of the response headers
+        """
+        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=False)
+        return self.get_street_account_filters_categories_endpoint.call_with_http_info(**kwargs)
+
+    def get_street_account_filters_categories_async(
+        self,
+        **kwargs
+    ) -> "ApplyResult[FilterCategoriesResponse]":
+        """Retrieve all StreetAccount filter categories  # noqa: E501
+
+        If structured flag is set, parent and child filter information will be returned. If flattened flag is set, flattened filters will be returned which can be used with the headlines and createView endpoints. Both flags can be set to return both sets of filters.  If no params are provided it will return both.  # noqa: E501
+        This method makes a asynchronous HTTP request. Returns the http data, wrapped in ApplyResult
+
+
+        Keyword Args:
+            attributes ([str]): Pass a list of filters to return the respective type of filter categories. Accepted list values are \"structured\" and/or \"flattened\". If no _atrributes are specified, all filters will be returned in the response (this is the default response). . [optional]
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True. NOTE: if this API returns a file, it is the responsibility
+                of the caller to close the file stream.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+        Returns:
+            ApplyResult[FilterCategoriesResponse]
+        """
+        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=True)
+        return self.get_street_account_filters_categories_endpoint.call_with_http_info(**kwargs)
+
+    def get_street_account_filters_categories_with_http_info_async(
+        self,
+        **kwargs
+    ) -> "ApplyResult[typing.Tuple[FilterCategoriesResponse, int, typing.MutableMapping]]":
+        """Retrieve all StreetAccount filter categories  # noqa: E501
+
+        If structured flag is set, parent and child filter information will be returned. If flattened flag is set, flattened filters will be returned which can be used with the headlines and createView endpoints. Both flags can be set to return both sets of filters.  If no params are provided it will return both.  # noqa: E501
+        This method makes a asynchronous HTTP request. Returns http data, http status and headers, wrapped in ApplyResult
+
+
+        Keyword Args:
+            attributes ([str]): Pass a list of filters to return the respective type of filter categories. Accepted list values are \"structured\" and/or \"flattened\". If no _atrributes are specified, all filters will be returned in the response (this is the default response). . [optional]
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True. NOTE: if this API returns a file, it is the responsibility
+                of the caller to close the file stream.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+        Returns:
+            ApplyResult[(FilterCategoriesResponse, int, typing.Dict)]
+        """
+        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=True)
+        return self.get_street_account_filters_categories_endpoint.call_with_http_info(**kwargs)
+
+
+    def get_street_account_filters_regions(
+        self,
+        **kwargs
+    ) -> FilterRegionsResponse:
+        """Retrieve all StreetAccount filter regions  # noqa: E501
+
+        If structured flag is set, parent and child filter information will be returned. If flattened flag is set, flattened filters will be returned which can be used with the headlines and createView endpoints. Both flags can be set to return both sets of filters.  If no params are provided it will return both.  # noqa: E501
+        This method makes a synchronous HTTP request. Returns the http data only
+
+
+        Keyword Args:
+            attributes ([str]): Pass a list of filters to return the respective type of filter Regions. Accepted list values are \"structured\" and/or \"flattened\". If no _atrributes are specified, all filters will be returned in the response (this is the default response). . [optional]
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True. NOTE: if this API returns a file, it is the responsibility
+                of the caller to close the file stream.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+        Returns:
+            FilterRegionsResponse
+                Response Object
+        """
+        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=False)
+        return self.get_street_account_filters_regions_endpoint.call_with_http_info(**kwargs)
+
+    def get_street_account_filters_regions_with_http_info(
+        self,
+        **kwargs
+    ) -> typing.Tuple[FilterRegionsResponse, int, typing.MutableMapping]:
+        """Retrieve all StreetAccount filter regions  # noqa: E501
+
+        If structured flag is set, parent and child filter information will be returned. If flattened flag is set, flattened filters will be returned which can be used with the headlines and createView endpoints. Both flags can be set to return both sets of filters.  If no params are provided it will return both.  # noqa: E501
+        This method makes a synchronous HTTP request. Returns http data, http status and headers
+
+
+        Keyword Args:
+            attributes ([str]): Pass a list of filters to return the respective type of filter Regions. Accepted list values are \"structured\" and/or \"flattened\". If no _atrributes are specified, all filters will be returned in the response (this is the default response). . [optional]
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True. NOTE: if this API returns a file, it is the responsibility
+                of the caller to close the file stream.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+        Returns:
+            FilterRegionsResponse
+                Response Object
+            int
+                Http Status Code
+            dict
+                Dictionary of the response headers
+        """
+        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=False)
+        return self.get_street_account_filters_regions_endpoint.call_with_http_info(**kwargs)
+
+    def get_street_account_filters_regions_async(
+        self,
+        **kwargs
+    ) -> "ApplyResult[FilterRegionsResponse]":
+        """Retrieve all StreetAccount filter regions  # noqa: E501
+
+        If structured flag is set, parent and child filter information will be returned. If flattened flag is set, flattened filters will be returned which can be used with the headlines and createView endpoints. Both flags can be set to return both sets of filters.  If no params are provided it will return both.  # noqa: E501
+        This method makes a asynchronous HTTP request. Returns the http data, wrapped in ApplyResult
+
+
+        Keyword Args:
+            attributes ([str]): Pass a list of filters to return the respective type of filter Regions. Accepted list values are \"structured\" and/or \"flattened\". If no _atrributes are specified, all filters will be returned in the response (this is the default response). . [optional]
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True. NOTE: if this API returns a file, it is the responsibility
+                of the caller to close the file stream.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+        Returns:
+            ApplyResult[FilterRegionsResponse]
+        """
+        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=True)
+        return self.get_street_account_filters_regions_endpoint.call_with_http_info(**kwargs)
+
+    def get_street_account_filters_regions_with_http_info_async(
+        self,
+        **kwargs
+    ) -> "ApplyResult[typing.Tuple[FilterRegionsResponse, int, typing.MutableMapping]]":
+        """Retrieve all StreetAccount filter regions  # noqa: E501
+
+        If structured flag is set, parent and child filter information will be returned. If flattened flag is set, flattened filters will be returned which can be used with the headlines and createView endpoints. Both flags can be set to return both sets of filters.  If no params are provided it will return both.  # noqa: E501
+        This method makes a asynchronous HTTP request. Returns http data, http status and headers, wrapped in ApplyResult
+
+
+        Keyword Args:
+            attributes ([str]): Pass a list of filters to return the respective type of filter Regions. Accepted list values are \"structured\" and/or \"flattened\". If no _atrributes are specified, all filters will be returned in the response (this is the default response). . [optional]
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True. NOTE: if this API returns a file, it is the responsibility
+                of the caller to close the file stream.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+        Returns:
+            ApplyResult[(FilterRegionsResponse, int, typing.Dict)]
+        """
+        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=True)
+        return self.get_street_account_filters_regions_endpoint.call_with_http_info(**kwargs)
+
+
+    def get_street_account_filters_sectors(
+        self,
+        **kwargs
+    ) -> FilterSectorsResponse:
+        """Retrieve all StreetAccount filter sectors  # noqa: E501
+
+        If structured flag is set, parent and child filter information will be returned. If flattened flag is set, flattened filters will be returned which can be used with the headlines and createView endpoints. Both flags can be set to return both sets of filters.  If no params are provided it will return both.  # noqa: E501
+        This method makes a synchronous HTTP request. Returns the http data only
+
+
+        Keyword Args:
+            attributes ([str]): Pass a list of filters to return the respective type of filter Sectors. Accepted list values are \"structured\" and/or \"flattened\". If no _atrributes are specified, all filters will be returned in the response (this is the default response). . [optional]
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True. NOTE: if this API returns a file, it is the responsibility
+                of the caller to close the file stream.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+        Returns:
+            FilterSectorsResponse
+                Response Object
+        """
+        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=False)
+        return self.get_street_account_filters_sectors_endpoint.call_with_http_info(**kwargs)
+
+    def get_street_account_filters_sectors_with_http_info(
+        self,
+        **kwargs
+    ) -> typing.Tuple[FilterSectorsResponse, int, typing.MutableMapping]:
+        """Retrieve all StreetAccount filter sectors  # noqa: E501
+
+        If structured flag is set, parent and child filter information will be returned. If flattened flag is set, flattened filters will be returned which can be used with the headlines and createView endpoints. Both flags can be set to return both sets of filters.  If no params are provided it will return both.  # noqa: E501
+        This method makes a synchronous HTTP request. Returns http data, http status and headers
+
+
+        Keyword Args:
+            attributes ([str]): Pass a list of filters to return the respective type of filter Sectors. Accepted list values are \"structured\" and/or \"flattened\". If no _atrributes are specified, all filters will be returned in the response (this is the default response). . [optional]
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True. NOTE: if this API returns a file, it is the responsibility
+                of the caller to close the file stream.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+        Returns:
+            FilterSectorsResponse
+                Response Object
+            int
+                Http Status Code
+            dict
+                Dictionary of the response headers
+        """
+        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=False)
+        return self.get_street_account_filters_sectors_endpoint.call_with_http_info(**kwargs)
+
+    def get_street_account_filters_sectors_async(
+        self,
+        **kwargs
+    ) -> "ApplyResult[FilterSectorsResponse]":
+        """Retrieve all StreetAccount filter sectors  # noqa: E501
+
+        If structured flag is set, parent and child filter information will be returned. If flattened flag is set, flattened filters will be returned which can be used with the headlines and createView endpoints. Both flags can be set to return both sets of filters.  If no params are provided it will return both.  # noqa: E501
+        This method makes a asynchronous HTTP request. Returns the http data, wrapped in ApplyResult
+
+
+        Keyword Args:
+            attributes ([str]): Pass a list of filters to return the respective type of filter Sectors. Accepted list values are \"structured\" and/or \"flattened\". If no _atrributes are specified, all filters will be returned in the response (this is the default response). . [optional]
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True. NOTE: if this API returns a file, it is the responsibility
+                of the caller to close the file stream.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+        Returns:
+            ApplyResult[FilterSectorsResponse]
+        """
+        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=True)
+        return self.get_street_account_filters_sectors_endpoint.call_with_http_info(**kwargs)
+
+    def get_street_account_filters_sectors_with_http_info_async(
+        self,
+        **kwargs
+    ) -> "ApplyResult[typing.Tuple[FilterSectorsResponse, int, typing.MutableMapping]]":
+        """Retrieve all StreetAccount filter sectors  # noqa: E501
+
+        If structured flag is set, parent and child filter information will be returned. If flattened flag is set, flattened filters will be returned which can be used with the headlines and createView endpoints. Both flags can be set to return both sets of filters.  If no params are provided it will return both.  # noqa: E501
+        This method makes a asynchronous HTTP request. Returns http data, http status and headers, wrapped in ApplyResult
+
+
+        Keyword Args:
+            attributes ([str]): Pass a list of filters to return the respective type of filter Sectors. Accepted list values are \"structured\" and/or \"flattened\". If no _atrributes are specified, all filters will be returned in the response (this is the default response). . [optional]
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True. NOTE: if this API returns a file, it is the responsibility
+                of the caller to close the file stream.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+        Returns:
+            ApplyResult[(FilterSectorsResponse, int, typing.Dict)]
+        """
+        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=True)
+        return self.get_street_account_filters_sectors_endpoint.call_with_http_info(**kwargs)
+
+
+    def get_street_account_filters_topics(
+        self,
+        **kwargs
+    ) -> FilterTopicResponse:
+        """Retrieve all StreetAccount filter topics  # noqa: E501
+
+        If structured flag is set, parent and child filter information will be returned. If flattened flag is set, flattened filters will be returned which can be used with the headlines and createView endpoints. Both flags can be set to return both sets of filters.  If no params are provided it will return both.  # noqa: E501
+        This method makes a synchronous HTTP request. Returns the http data only
+
+
+        Keyword Args:
+            attributes ([str]): Pass a list of filters to return the respective type of filter topics. Accepted list values are \"structured\" and/or \"flattened\". If no _atrributes are specified, all filters will be returned in the response (this is the default response). . [optional]
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True. NOTE: if this API returns a file, it is the responsibility
+                of the caller to close the file stream.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+        Returns:
+            FilterTopicResponse
+                Response Object
+        """
+        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=False)
+        return self.get_street_account_filters_topics_endpoint.call_with_http_info(**kwargs)
+
+    def get_street_account_filters_topics_with_http_info(
+        self,
+        **kwargs
+    ) -> typing.Tuple[FilterTopicResponse, int, typing.MutableMapping]:
+        """Retrieve all StreetAccount filter topics  # noqa: E501
+
+        If structured flag is set, parent and child filter information will be returned. If flattened flag is set, flattened filters will be returned which can be used with the headlines and createView endpoints. Both flags can be set to return both sets of filters.  If no params are provided it will return both.  # noqa: E501
+        This method makes a synchronous HTTP request. Returns http data, http status and headers
+
+
+        Keyword Args:
+            attributes ([str]): Pass a list of filters to return the respective type of filter topics. Accepted list values are \"structured\" and/or \"flattened\". If no _atrributes are specified, all filters will be returned in the response (this is the default response). . [optional]
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True. NOTE: if this API returns a file, it is the responsibility
+                of the caller to close the file stream.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+        Returns:
+            FilterTopicResponse
+                Response Object
+            int
+                Http Status Code
+            dict
+                Dictionary of the response headers
+        """
+        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=False)
+        return self.get_street_account_filters_topics_endpoint.call_with_http_info(**kwargs)
+
+    def get_street_account_filters_topics_async(
+        self,
+        **kwargs
+    ) -> "ApplyResult[FilterTopicResponse]":
+        """Retrieve all StreetAccount filter topics  # noqa: E501
+
+        If structured flag is set, parent and child filter information will be returned. If flattened flag is set, flattened filters will be returned which can be used with the headlines and createView endpoints. Both flags can be set to return both sets of filters.  If no params are provided it will return both.  # noqa: E501
+        This method makes a asynchronous HTTP request. Returns the http data, wrapped in ApplyResult
+
+
+        Keyword Args:
+            attributes ([str]): Pass a list of filters to return the respective type of filter topics. Accepted list values are \"structured\" and/or \"flattened\". If no _atrributes are specified, all filters will be returned in the response (this is the default response). . [optional]
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True. NOTE: if this API returns a file, it is the responsibility
+                of the caller to close the file stream.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+        Returns:
+            ApplyResult[FilterTopicResponse]
+        """
+        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=True)
+        return self.get_street_account_filters_topics_endpoint.call_with_http_info(**kwargs)
+
+    def get_street_account_filters_topics_with_http_info_async(
+        self,
+        **kwargs
+    ) -> "ApplyResult[typing.Tuple[FilterTopicResponse, int, typing.MutableMapping]]":
+        """Retrieve all StreetAccount filter topics  # noqa: E501
+
+        If structured flag is set, parent and child filter information will be returned. If flattened flag is set, flattened filters will be returned which can be used with the headlines and createView endpoints. Both flags can be set to return both sets of filters.  If no params are provided it will return both.  # noqa: E501
+        This method makes a asynchronous HTTP request. Returns http data, http status and headers, wrapped in ApplyResult
+
+
+        Keyword Args:
+            attributes ([str]): Pass a list of filters to return the respective type of filter topics. Accepted list values are \"structured\" and/or \"flattened\". If no _atrributes are specified, all filters will be returned in the response (this is the default response). . [optional]
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True. NOTE: if this API returns a file, it is the responsibility
+                of the caller to close the file stream.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+        Returns:
+            ApplyResult[(FilterTopicResponse, int, typing.Dict)]
+        """
+        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=True)
+        return self.get_street_account_filters_topics_endpoint.call_with_http_info(**kwargs)
+
+
+    def get_street_account_filters_watchlists(
+        self,
+        **kwargs
+    ) -> FilterWatchlistsResponse:
+        """Retrieve all StreetAccount filter watchlists  # noqa: E501
+
+        If structured flag is set, parent and child filter information will be returned. If flattened flag is set, flattened filters will be returned which can be used with the headlines and createView endpoints. Both flags can be set to return both sets of filters.  If no params are provided it will return both.  # noqa: E501
+        This method makes a synchronous HTTP request. Returns the http data only
+
+
+        Keyword Args:
+            attributes ([str]): Pass a list of filters to return the respective type of filter Watchlists. Accepted list values are \"structured\" and/or \"flattened\". If no _atrributes are specified, all filters will be returned in the response (this is the default response). . [optional]
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True. NOTE: if this API returns a file, it is the responsibility
+                of the caller to close the file stream.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+        Returns:
+            FilterWatchlistsResponse
+                Response Object
+        """
+        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=False)
+        return self.get_street_account_filters_watchlists_endpoint.call_with_http_info(**kwargs)
+
+    def get_street_account_filters_watchlists_with_http_info(
+        self,
+        **kwargs
+    ) -> typing.Tuple[FilterWatchlistsResponse, int, typing.MutableMapping]:
+        """Retrieve all StreetAccount filter watchlists  # noqa: E501
+
+        If structured flag is set, parent and child filter information will be returned. If flattened flag is set, flattened filters will be returned which can be used with the headlines and createView endpoints. Both flags can be set to return both sets of filters.  If no params are provided it will return both.  # noqa: E501
+        This method makes a synchronous HTTP request. Returns http data, http status and headers
+
+
+        Keyword Args:
+            attributes ([str]): Pass a list of filters to return the respective type of filter Watchlists. Accepted list values are \"structured\" and/or \"flattened\". If no _atrributes are specified, all filters will be returned in the response (this is the default response). . [optional]
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True. NOTE: if this API returns a file, it is the responsibility
+                of the caller to close the file stream.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+        Returns:
+            FilterWatchlistsResponse
+                Response Object
+            int
+                Http Status Code
+            dict
+                Dictionary of the response headers
+        """
+        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=False)
+        return self.get_street_account_filters_watchlists_endpoint.call_with_http_info(**kwargs)
+
+    def get_street_account_filters_watchlists_async(
+        self,
+        **kwargs
+    ) -> "ApplyResult[FilterWatchlistsResponse]":
+        """Retrieve all StreetAccount filter watchlists  # noqa: E501
+
+        If structured flag is set, parent and child filter information will be returned. If flattened flag is set, flattened filters will be returned which can be used with the headlines and createView endpoints. Both flags can be set to return both sets of filters.  If no params are provided it will return both.  # noqa: E501
+        This method makes a asynchronous HTTP request. Returns the http data, wrapped in ApplyResult
+
+
+        Keyword Args:
+            attributes ([str]): Pass a list of filters to return the respective type of filter Watchlists. Accepted list values are \"structured\" and/or \"flattened\". If no _atrributes are specified, all filters will be returned in the response (this is the default response). . [optional]
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True. NOTE: if this API returns a file, it is the responsibility
+                of the caller to close the file stream.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+        Returns:
+            ApplyResult[FilterWatchlistsResponse]
+        """
+        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=True)
+        return self.get_street_account_filters_watchlists_endpoint.call_with_http_info(**kwargs)
+
+    def get_street_account_filters_watchlists_with_http_info_async(
+        self,
+        **kwargs
+    ) -> "ApplyResult[typing.Tuple[FilterWatchlistsResponse, int, typing.MutableMapping]]":
+        """Retrieve all StreetAccount filter watchlists  # noqa: E501
+
+        If structured flag is set, parent and child filter information will be returned. If flattened flag is set, flattened filters will be returned which can be used with the headlines and createView endpoints. Both flags can be set to return both sets of filters.  If no params are provided it will return both.  # noqa: E501
+        This method makes a asynchronous HTTP request. Returns http data, http status and headers, wrapped in ApplyResult
+
+
+        Keyword Args:
+            attributes ([str]): Pass a list of filters to return the respective type of filter Watchlists. Accepted list values are \"structured\" and/or \"flattened\". If no _atrributes are specified, all filters will be returned in the response (this is the default response). . [optional]
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True. NOTE: if this API returns a file, it is the responsibility
+                of the caller to close the file stream.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+        Returns:
+            ApplyResult[(FilterWatchlistsResponse, int, typing.Dict)]
+        """
+        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=True)
+        return self.get_street_account_filters_watchlists_endpoint.call_with_http_info(**kwargs)
+
+
```

## fds/sdk/StreetAccountNews/api/headlines_api.py

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -22,17 +22,17 @@
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
 from fds.sdk.StreetAccountNews.exceptions import ApiException
 from fds.sdk.StreetAccountNews.model.error import Error
-from fds.sdk.StreetAccountNews.model.sa_headlines_request import SaHeadlinesRequest
-from fds.sdk.StreetAccountNews.model.sa_headlines_request_by_view import SaHeadlinesRequestByView
-from fds.sdk.StreetAccountNews.model.search_response import SearchResponse
+from fds.sdk.StreetAccountNews.model.headlines_request import HeadlinesRequest
+from fds.sdk.StreetAccountNews.model.headlines_request_by_view import HeadlinesRequestByView
+from fds.sdk.StreetAccountNews.model.headlines_response import HeadlinesResponse
 
 
 
 
 
 class HeadlinesApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
@@ -45,29 +45,29 @@
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
         self.get_street_account_headlines_endpoint = _Endpoint(
             settings={
                 'response_type': (
-                  { 200: (SearchResponse,), 400: (Error,), 401: (Error,), 404: (Error,),  },
+                  { 200: (HeadlinesResponse,), 400: (Error,), 401: (Error,), 404: (Error,),  },
                   None
                 ),
                 'auth': [
                     'FactSetApiKey',
                     'FactSetOAuth2'
                 ],
-                'endpoint_path': '/streetaccount/headlines',
+                'endpoint_path': '/headlines',
                 'operation_id': 'get_street_account_headlines',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'sa_headlines_request',
+                    'headlines_request',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
@@ -75,21 +75,21 @@
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'sa_headlines_request':
-                        (SaHeadlinesRequest,),
+                    'headlines_request':
+                        (HeadlinesRequest,),
                 },
                 'attribute_map': {
                 },
                 'location_map': {
-                    'sa_headlines_request': 'body',
+                    'headlines_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
@@ -100,58 +100,51 @@
             },
             api_client=api_client
         )
 
         self.get_street_account_headlines_by_view_endpoint = _Endpoint(
             settings={
                 'response_type': (
-                  { 200: (SearchResponse,), 400: (Error,), 401: (Error,), 404: (Error,),  },
+                  { 200: (HeadlinesResponse,), 400: (Error,), 401: (Error,), 404: (Error,),  },
                   None
                 ),
                 'auth': [
                     'FactSetApiKey',
                     'FactSetOAuth2'
                 ],
-                'endpoint_path': '/streetaccount/views/{id}/headlines',
+                'endpoint_path': '/headlines/view',
                 'operation_id': 'get_street_account_headlines_by_view',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'id',
-                    'sa_headlines_request_by_view',
-                ],
-                'required': [
-                    'id',
+                    'headlines_request_by_view',
                 ],
+                'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'id':
-                        (str,),
-                    'sa_headlines_request_by_view':
-                        (SaHeadlinesRequestByView,),
+                    'headlines_request_by_view':
+                        (HeadlinesRequestByView,),
                 },
                 'attribute_map': {
-                    'id': 'id',
                 },
                 'location_map': {
-                    'id': 'path',
-                    'sa_headlines_request_by_view': 'body',
+                    'headlines_request_by_view': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
@@ -176,23 +169,23 @@
         kwargs["_content_type"] = kwargs.get("_content_type")
         kwargs["_host_index"] = kwargs.get("_host_index")
 
 
     def get_street_account_headlines(
         self,
         **kwargs
-    ) -> SearchResponse:
+    ) -> HeadlinesResponse:
         """Retrieve StreetAccount headlines for given filters  # noqa: E501
 
-        This endpoint will pull all headlines produced by StreetAccount and the full story body will be returned by the data set. Filters can be specified via the endpoint below.  # noqa: E501
+        This endpoint will pull all headlines produced by StreetAccount and the full story body will be returned by the data set. Filters can be specified via the endpoint below. The attributes field in the request body can be used to specify which fields are returned in the response. If attributes are empty or not specified, the response does not omit attributes.  # noqa: E501
         This method makes a synchronous HTTP request. Returns the http data only
 
 
         Keyword Args:
-            sa_headlines_request (SaHeadlinesRequest): Filter Body which needs to be sent with request. [optional]
+            headlines_request (HeadlinesRequest): /filters endpoint contains the filters associated with the optional parameters in the request body.. [optional]
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True. NOTE: if this API returns a file, it is the responsibility
                 of the caller to close the file stream.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -210,32 +203,32 @@
             _content_type (str/None): force body content-type.
                 Default is None and content-type will be predicted by allowed
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
         Returns:
-            SearchResponse
+            HeadlinesResponse
                 Response Object
         """
         self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=False)
         return self.get_street_account_headlines_endpoint.call_with_http_info(**kwargs)
 
     def get_street_account_headlines_with_http_info(
         self,
         **kwargs
-    ) -> typing.Tuple[SearchResponse, int, typing.MutableMapping]:
+    ) -> typing.Tuple[HeadlinesResponse, int, typing.MutableMapping]:
         """Retrieve StreetAccount headlines for given filters  # noqa: E501
 
-        This endpoint will pull all headlines produced by StreetAccount and the full story body will be returned by the data set. Filters can be specified via the endpoint below.  # noqa: E501
+        This endpoint will pull all headlines produced by StreetAccount and the full story body will be returned by the data set. Filters can be specified via the endpoint below. The attributes field in the request body can be used to specify which fields are returned in the response. If attributes are empty or not specified, the response does not omit attributes.  # noqa: E501
         This method makes a synchronous HTTP request. Returns http data, http status and headers
 
 
         Keyword Args:
-            sa_headlines_request (SaHeadlinesRequest): Filter Body which needs to be sent with request. [optional]
+            headlines_request (HeadlinesRequest): /filters endpoint contains the filters associated with the optional parameters in the request body.. [optional]
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True. NOTE: if this API returns a file, it is the responsibility
                 of the caller to close the file stream.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -253,36 +246,36 @@
             _content_type (str/None): force body content-type.
                 Default is None and content-type will be predicted by allowed
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
         Returns:
-            SearchResponse
+            HeadlinesResponse
                 Response Object
             int
                 Http Status Code
             dict
                 Dictionary of the response headers
         """
         self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=False)
         return self.get_street_account_headlines_endpoint.call_with_http_info(**kwargs)
 
     def get_street_account_headlines_async(
         self,
         **kwargs
-    ) -> "ApplyResult[SearchResponse]":
+    ) -> "ApplyResult[HeadlinesResponse]":
         """Retrieve StreetAccount headlines for given filters  # noqa: E501
 
-        This endpoint will pull all headlines produced by StreetAccount and the full story body will be returned by the data set. Filters can be specified via the endpoint below.  # noqa: E501
+        This endpoint will pull all headlines produced by StreetAccount and the full story body will be returned by the data set. Filters can be specified via the endpoint below. The attributes field in the request body can be used to specify which fields are returned in the response. If attributes are empty or not specified, the response does not omit attributes.  # noqa: E501
         This method makes a asynchronous HTTP request. Returns the http data, wrapped in ApplyResult
 
 
         Keyword Args:
-            sa_headlines_request (SaHeadlinesRequest): Filter Body which needs to be sent with request. [optional]
+            headlines_request (HeadlinesRequest): /filters endpoint contains the filters associated with the optional parameters in the request body.. [optional]
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True. NOTE: if this API returns a file, it is the responsibility
                 of the caller to close the file stream.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -300,31 +293,31 @@
             _content_type (str/None): force body content-type.
                 Default is None and content-type will be predicted by allowed
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
         Returns:
-            ApplyResult[SearchResponse]
+            ApplyResult[HeadlinesResponse]
         """
         self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=True)
         return self.get_street_account_headlines_endpoint.call_with_http_info(**kwargs)
 
     def get_street_account_headlines_with_http_info_async(
         self,
         **kwargs
-    ) -> "ApplyResult[typing.Tuple[SearchResponse, int, typing.MutableMapping]]":
+    ) -> "ApplyResult[typing.Tuple[HeadlinesResponse, int, typing.MutableMapping]]":
         """Retrieve StreetAccount headlines for given filters  # noqa: E501
 
-        This endpoint will pull all headlines produced by StreetAccount and the full story body will be returned by the data set. Filters can be specified via the endpoint below.  # noqa: E501
+        This endpoint will pull all headlines produced by StreetAccount and the full story body will be returned by the data set. Filters can be specified via the endpoint below. The attributes field in the request body can be used to specify which fields are returned in the response. If attributes are empty or not specified, the response does not omit attributes.  # noqa: E501
         This method makes a asynchronous HTTP request. Returns http data, http status and headers, wrapped in ApplyResult
 
 
         Keyword Args:
-            sa_headlines_request (SaHeadlinesRequest): Filter Body which needs to be sent with request. [optional]
+            headlines_request (HeadlinesRequest): /filters endpoint contains the filters associated with the optional parameters in the request body.. [optional]
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True. NOTE: if this API returns a file, it is the responsibility
                 of the caller to close the file stream.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -342,35 +335,32 @@
             _content_type (str/None): force body content-type.
                 Default is None and content-type will be predicted by allowed
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
         Returns:
-            ApplyResult[(SearchResponse, int, typing.Dict)]
+            ApplyResult[(HeadlinesResponse, int, typing.Dict)]
         """
         self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=True)
         return self.get_street_account_headlines_endpoint.call_with_http_info(**kwargs)
 
 
     def get_street_account_headlines_by_view(
         self,
-        id,
         **kwargs
-    ) -> SearchResponse:
+    ) -> HeadlinesResponse:
         """Retrieve StreetAccount headlines for given view  # noqa: E501
 
         This endpoint allows you to pull all headlines produced by StreetAccount for a saved view. The full story body will be returned by the data set. Views can be created via the ‘Create Views’ endpoint.  # noqa: E501
         This method makes a synchronous HTTP request. Returns the http data only
 
-        Args:
-            id (str): view id of the view to return headlines for
 
         Keyword Args:
-            sa_headlines_request_by_view (SaHeadlinesRequestByView): View body which needs to be sent with request. [optional]
+            headlines_request_by_view (HeadlinesRequestByView): View body which needs to be sent with request. [optional]
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True. NOTE: if this API returns a file, it is the responsibility
                 of the caller to close the file stream.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -388,37 +378,32 @@
             _content_type (str/None): force body content-type.
                 Default is None and content-type will be predicted by allowed
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
         Returns:
-            SearchResponse
+            HeadlinesResponse
                 Response Object
         """
         self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=False)
-        kwargs['id'] = \
-            id
         return self.get_street_account_headlines_by_view_endpoint.call_with_http_info(**kwargs)
 
     def get_street_account_headlines_by_view_with_http_info(
         self,
-        id,
         **kwargs
-    ) -> typing.Tuple[SearchResponse, int, typing.MutableMapping]:
+    ) -> typing.Tuple[HeadlinesResponse, int, typing.MutableMapping]:
         """Retrieve StreetAccount headlines for given view  # noqa: E501
 
         This endpoint allows you to pull all headlines produced by StreetAccount for a saved view. The full story body will be returned by the data set. Views can be created via the ‘Create Views’ endpoint.  # noqa: E501
         This method makes a synchronous HTTP request. Returns http data, http status and headers
 
-        Args:
-            id (str): view id of the view to return headlines for
 
         Keyword Args:
-            sa_headlines_request_by_view (SaHeadlinesRequestByView): View body which needs to be sent with request. [optional]
+            headlines_request_by_view (HeadlinesRequestByView): View body which needs to be sent with request. [optional]
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True. NOTE: if this API returns a file, it is the responsibility
                 of the caller to close the file stream.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -436,41 +421,36 @@
             _content_type (str/None): force body content-type.
                 Default is None and content-type will be predicted by allowed
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
         Returns:
-            SearchResponse
+            HeadlinesResponse
                 Response Object
             int
                 Http Status Code
             dict
                 Dictionary of the response headers
         """
         self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=False)
-        kwargs['id'] = \
-            id
         return self.get_street_account_headlines_by_view_endpoint.call_with_http_info(**kwargs)
 
     def get_street_account_headlines_by_view_async(
         self,
-        id,
         **kwargs
-    ) -> "ApplyResult[SearchResponse]":
+    ) -> "ApplyResult[HeadlinesResponse]":
         """Retrieve StreetAccount headlines for given view  # noqa: E501
 
         This endpoint allows you to pull all headlines produced by StreetAccount for a saved view. The full story body will be returned by the data set. Views can be created via the ‘Create Views’ endpoint.  # noqa: E501
         This method makes a asynchronous HTTP request. Returns the http data, wrapped in ApplyResult
 
-        Args:
-            id (str): view id of the view to return headlines for
 
         Keyword Args:
-            sa_headlines_request_by_view (SaHeadlinesRequestByView): View body which needs to be sent with request. [optional]
+            headlines_request_by_view (HeadlinesRequestByView): View body which needs to be sent with request. [optional]
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True. NOTE: if this API returns a file, it is the responsibility
                 of the caller to close the file stream.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -488,36 +468,31 @@
             _content_type (str/None): force body content-type.
                 Default is None and content-type will be predicted by allowed
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
         Returns:
-            ApplyResult[SearchResponse]
+            ApplyResult[HeadlinesResponse]
         """
         self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=True)
-        kwargs['id'] = \
-            id
         return self.get_street_account_headlines_by_view_endpoint.call_with_http_info(**kwargs)
 
     def get_street_account_headlines_by_view_with_http_info_async(
         self,
-        id,
         **kwargs
-    ) -> "ApplyResult[typing.Tuple[SearchResponse, int, typing.MutableMapping]]":
+    ) -> "ApplyResult[typing.Tuple[HeadlinesResponse, int, typing.MutableMapping]]":
         """Retrieve StreetAccount headlines for given view  # noqa: E501
 
         This endpoint allows you to pull all headlines produced by StreetAccount for a saved view. The full story body will be returned by the data set. Views can be created via the ‘Create Views’ endpoint.  # noqa: E501
         This method makes a asynchronous HTTP request. Returns http data, http status and headers, wrapped in ApplyResult
 
-        Args:
-            id (str): view id of the view to return headlines for
 
         Keyword Args:
-            sa_headlines_request_by_view (SaHeadlinesRequestByView): View body which needs to be sent with request. [optional]
+            headlines_request_by_view (HeadlinesRequestByView): View body which needs to be sent with request. [optional]
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True. NOTE: if this API returns a file, it is the responsibility
                 of the caller to close the file stream.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -535,15 +510,13 @@
             _content_type (str/None): force body content-type.
                 Default is None and content-type will be predicted by allowed
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
         Returns:
-            ApplyResult[(SearchResponse, int, typing.Dict)]
+            ApplyResult[(HeadlinesResponse, int, typing.Dict)]
         """
         self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=True)
-        kwargs['id'] = \
-            id
         return self.get_street_account_headlines_by_view_endpoint.call_with_http_info(**kwargs)
```

## fds/sdk/StreetAccountNews/api/views_api.py

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -21,17 +21,20 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
 from fds.sdk.StreetAccountNews.exceptions import ApiException
-from fds.sdk.StreetAccountNews.model.create_edit_delete_view_response import CreateEditDeleteViewResponse
 from fds.sdk.StreetAccountNews.model.create_or_edit_view_body import CreateOrEditViewBody
+from fds.sdk.StreetAccountNews.model.create_view_response import CreateViewResponse
+from fds.sdk.StreetAccountNews.model.delete_view_body import DeleteViewBody
 from fds.sdk.StreetAccountNews.model.error import Error
+from fds.sdk.StreetAccountNews.model.quick_alerts_body import QuickAlertsBody
+from fds.sdk.StreetAccountNews.model.quick_alerts_response import QuickAlertsResponse
 from fds.sdk.StreetAccountNews.model.views import Views
 
 
 
 
 
 class ViewsApi(object):
@@ -42,60 +45,108 @@
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
+        self.create_quick_alert_for_view_endpoint = _Endpoint(
+            settings={
+                'response_type': (
+                  { 201: (QuickAlertsResponse,), 400: (Error,), 404: (Error,), 500: (Error,),  },
+                  None
+                ),
+                'auth': [
+                    'FactSetApiKey',
+                    'FactSetOAuth2'
+                ],
+                'endpoint_path': '/quick-alert/create',
+                'operation_id': 'create_quick_alert_for_view',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'quick_alerts_body',
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'quick_alerts_body':
+                        (QuickAlertsBody,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'quick_alerts_body': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+
         self.create_street_account_view_endpoint = _Endpoint(
             settings={
                 'response_type': (
-                  { 200: (CreateEditDeleteViewResponse,), 400: (Error,), 401: (Error,), 500: (Error,),  },
+                  { 201: (CreateViewResponse,), 400: (Error,), 401: (Error,), 500: (Error,),  },
                   None
                 ),
                 'auth': [
                     'FactSetApiKey',
                     'FactSetOAuth2'
                 ],
-                'endpoint_path': '/streetaccount/views/{id}',
+                'endpoint_path': '/views/create',
                 'operation_id': 'create_street_account_view',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'id',
                     'create_or_edit_view_body',
                 ],
-                'required': [
-                    'id',
-                ],
+                'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'id':
-                        (str,),
                     'create_or_edit_view_body':
                         (CreateOrEditViewBody,),
                 },
                 'attribute_map': {
-                    'id': 'id',
                 },
                 'location_map': {
-                    'id': 'path',
                     'create_or_edit_view_body': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
@@ -104,116 +155,154 @@
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
 
+        self.delete_quickalert_view_endpoint = _Endpoint(
+            settings={
+                'response_type': None,
+                'auth': [
+                    'FactSetApiKey',
+                    'FactSetOAuth2'
+                ],
+                'endpoint_path': '/quick-alert/delete',
+                'operation_id': 'delete_quickalert_view',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'quick_alerts_body',
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'quick_alerts_body':
+                        (QuickAlertsBody,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'quick_alerts_body': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+
         self.delete_street_account_view_endpoint = _Endpoint(
             settings={
-                'response_type': (
-                  { 200: (CreateEditDeleteViewResponse,), 400: (Error,), 401: (Error,), 500: (Error,),  },
-                  None
-                ),
+                'response_type': None,
                 'auth': [
                     'FactSetApiKey',
                     'FactSetOAuth2'
                 ],
-                'endpoint_path': '/streetaccount/views/{id}',
+                'endpoint_path': '/views/delete',
                 'operation_id': 'delete_street_account_view',
-                'http_method': 'DELETE',
+                'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'id',
-                ],
-                'required': [
-                    'id',
+                    'delete_view_body',
                 ],
+                'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'id':
-                        (str,),
+                    'delete_view_body':
+                        (DeleteViewBody,),
                 },
                 'attribute_map': {
-                    'id': 'id',
                 },
                 'location_map': {
-                    'id': 'path',
+                    'delete_view_body': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
-                'content_type': [],
+                'content_type': [
+                    'application/json'
+                ]
             },
             api_client=api_client
         )
 
         self.edit_street_account_view_endpoint = _Endpoint(
             settings={
-                'response_type': (
-                  { 200: (CreateEditDeleteViewResponse,), 400: (Error,), 401: (Error,), 500: (Error,),  },
-                  None
-                ),
+                'response_type': None,
                 'auth': [
                     'FactSetApiKey',
                     'FactSetOAuth2'
                 ],
-                'endpoint_path': '/streetaccount/views/{id}',
+                'endpoint_path': '/views/update',
                 'operation_id': 'edit_street_account_view',
-                'http_method': 'PUT',
+                'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'id',
                     'create_or_edit_view_body',
                 ],
-                'required': [
-                    'id',
-                ],
+                'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'id':
-                        (str,),
                     'create_or_edit_view_body':
                         (CreateOrEditViewBody,),
                 },
                 'attribute_map': {
-                    'id': 'id',
                 },
                 'location_map': {
-                    'id': 'path',
                     'create_or_edit_view_body': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
@@ -232,15 +321,15 @@
                   { 200: (Views,), 400: (Error,), 401: (Error,), 500: (Error,),  },
                   None
                 ),
                 'auth': [
                     'FactSetApiKey',
                     'FactSetOAuth2'
                 ],
-                'endpoint_path': '/streetaccount/views',
+                'endpoint_path': '/views',
                 'operation_id': 'get_street_account_views',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                 ],
@@ -285,26 +374,198 @@
         kwargs["_check_input_type"] = kwargs.get("_check_input_type", True)
         kwargs["_check_return_type"] = kwargs.get("_check_return_type", True)
         kwargs["_spec_property_naming"] = kwargs.get("_spec_property_naming", False)
         kwargs["_content_type"] = kwargs.get("_content_type")
         kwargs["_host_index"] = kwargs.get("_host_index")
 
 
+    def create_quick_alert_for_view(
+        self,
+        **kwargs
+    ) -> QuickAlertsResponse:
+        """Creates a quick-alert for given saved view  # noqa: E501
+
+        This endpoint takes in a view name and provides realtime email updates on new stories coming in for the view. Only one quick alert can be enabled for a view at a time.    # noqa: E501
+        This method makes a synchronous HTTP request. Returns the http data only
+
+
+        Keyword Args:
+            quick_alerts_body (QuickAlertsBody): View name to get an alert. [optional]
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True. NOTE: if this API returns a file, it is the responsibility
+                of the caller to close the file stream.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+        Returns:
+            QuickAlertsResponse
+                Response Object
+        """
+        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=False)
+        return self.create_quick_alert_for_view_endpoint.call_with_http_info(**kwargs)
+
+    def create_quick_alert_for_view_with_http_info(
+        self,
+        **kwargs
+    ) -> typing.Tuple[QuickAlertsResponse, int, typing.MutableMapping]:
+        """Creates a quick-alert for given saved view  # noqa: E501
+
+        This endpoint takes in a view name and provides realtime email updates on new stories coming in for the view. Only one quick alert can be enabled for a view at a time.    # noqa: E501
+        This method makes a synchronous HTTP request. Returns http data, http status and headers
+
+
+        Keyword Args:
+            quick_alerts_body (QuickAlertsBody): View name to get an alert. [optional]
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True. NOTE: if this API returns a file, it is the responsibility
+                of the caller to close the file stream.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+        Returns:
+            QuickAlertsResponse
+                Response Object
+            int
+                Http Status Code
+            dict
+                Dictionary of the response headers
+        """
+        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=False)
+        return self.create_quick_alert_for_view_endpoint.call_with_http_info(**kwargs)
+
+    def create_quick_alert_for_view_async(
+        self,
+        **kwargs
+    ) -> "ApplyResult[QuickAlertsResponse]":
+        """Creates a quick-alert for given saved view  # noqa: E501
+
+        This endpoint takes in a view name and provides realtime email updates on new stories coming in for the view. Only one quick alert can be enabled for a view at a time.    # noqa: E501
+        This method makes a asynchronous HTTP request. Returns the http data, wrapped in ApplyResult
+
+
+        Keyword Args:
+            quick_alerts_body (QuickAlertsBody): View name to get an alert. [optional]
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True. NOTE: if this API returns a file, it is the responsibility
+                of the caller to close the file stream.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+        Returns:
+            ApplyResult[QuickAlertsResponse]
+        """
+        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=True)
+        return self.create_quick_alert_for_view_endpoint.call_with_http_info(**kwargs)
+
+    def create_quick_alert_for_view_with_http_info_async(
+        self,
+        **kwargs
+    ) -> "ApplyResult[typing.Tuple[QuickAlertsResponse, int, typing.MutableMapping]]":
+        """Creates a quick-alert for given saved view  # noqa: E501
+
+        This endpoint takes in a view name and provides realtime email updates on new stories coming in for the view. Only one quick alert can be enabled for a view at a time.    # noqa: E501
+        This method makes a asynchronous HTTP request. Returns http data, http status and headers, wrapped in ApplyResult
+
+
+        Keyword Args:
+            quick_alerts_body (QuickAlertsBody): View name to get an alert. [optional]
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True. NOTE: if this API returns a file, it is the responsibility
+                of the caller to close the file stream.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+        Returns:
+            ApplyResult[(QuickAlertsResponse, int, typing.Dict)]
+        """
+        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=True)
+        return self.create_quick_alert_for_view_endpoint.call_with_http_info(**kwargs)
+
+
     def create_street_account_view(
         self,
-        id,
         **kwargs
-    ) -> CreateEditDeleteViewResponse:
+    ) -> CreateViewResponse:
         """Creates and saves a StreetAccount view  # noqa: E501
 
         This endpoint allows you to create a new StreetAccount view. Select watchlists/tickers and filters of your choice to create and save a view.  # noqa: E501
         This method makes a synchronous HTTP request. Returns the http data only
 
-        Args:
-            id (str): view id of the view which is the be created
 
         Keyword Args:
             create_or_edit_view_body (CreateOrEditViewBody): Create or Edit View Body which needs to be sent with request. [optional]
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True. NOTE: if this API returns a file, it is the responsibility
                 of the caller to close the file stream.
@@ -325,34 +586,29 @@
             _content_type (str/None): force body content-type.
                 Default is None and content-type will be predicted by allowed
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
         Returns:
-            CreateEditDeleteViewResponse
+            CreateViewResponse
                 Response Object
         """
         self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=False)
-        kwargs['id'] = \
-            id
         return self.create_street_account_view_endpoint.call_with_http_info(**kwargs)
 
     def create_street_account_view_with_http_info(
         self,
-        id,
         **kwargs
-    ) -> typing.Tuple[CreateEditDeleteViewResponse, int, typing.MutableMapping]:
+    ) -> typing.Tuple[CreateViewResponse, int, typing.MutableMapping]:
         """Creates and saves a StreetAccount view  # noqa: E501
 
         This endpoint allows you to create a new StreetAccount view. Select watchlists/tickers and filters of your choice to create and save a view.  # noqa: E501
         This method makes a synchronous HTTP request. Returns http data, http status and headers
 
-        Args:
-            id (str): view id of the view which is the be created
 
         Keyword Args:
             create_or_edit_view_body (CreateOrEditViewBody): Create or Edit View Body which needs to be sent with request. [optional]
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True. NOTE: if this API returns a file, it is the responsibility
                 of the caller to close the file stream.
@@ -373,38 +629,33 @@
             _content_type (str/None): force body content-type.
                 Default is None and content-type will be predicted by allowed
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
         Returns:
-            CreateEditDeleteViewResponse
+            CreateViewResponse
                 Response Object
             int
                 Http Status Code
             dict
                 Dictionary of the response headers
         """
         self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=False)
-        kwargs['id'] = \
-            id
         return self.create_street_account_view_endpoint.call_with_http_info(**kwargs)
 
     def create_street_account_view_async(
         self,
-        id,
         **kwargs
-    ) -> "ApplyResult[CreateEditDeleteViewResponse]":
+    ) -> "ApplyResult[CreateViewResponse]":
         """Creates and saves a StreetAccount view  # noqa: E501
 
         This endpoint allows you to create a new StreetAccount view. Select watchlists/tickers and filters of your choice to create and save a view.  # noqa: E501
         This method makes a asynchronous HTTP request. Returns the http data, wrapped in ApplyResult
 
-        Args:
-            id (str): view id of the view which is the be created
 
         Keyword Args:
             create_or_edit_view_body (CreateOrEditViewBody): Create or Edit View Body which needs to be sent with request. [optional]
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True. NOTE: if this API returns a file, it is the responsibility
                 of the caller to close the file stream.
@@ -425,33 +676,28 @@
             _content_type (str/None): force body content-type.
                 Default is None and content-type will be predicted by allowed
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
         Returns:
-            ApplyResult[CreateEditDeleteViewResponse]
+            ApplyResult[CreateViewResponse]
         """
         self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=True)
-        kwargs['id'] = \
-            id
         return self.create_street_account_view_endpoint.call_with_http_info(**kwargs)
 
     def create_street_account_view_with_http_info_async(
         self,
-        id,
         **kwargs
-    ) -> "ApplyResult[typing.Tuple[CreateEditDeleteViewResponse, int, typing.MutableMapping]]":
+    ) -> "ApplyResult[typing.Tuple[CreateViewResponse, int, typing.MutableMapping]]":
         """Creates and saves a StreetAccount view  # noqa: E501
 
         This endpoint allows you to create a new StreetAccount view. Select watchlists/tickers and filters of your choice to create and save a view.  # noqa: E501
         This method makes a asynchronous HTTP request. Returns http data, http status and headers, wrapped in ApplyResult
 
-        Args:
-            id (str): view id of the view which is the be created
 
         Keyword Args:
             create_or_edit_view_body (CreateOrEditViewBody): Create or Edit View Body which needs to be sent with request. [optional]
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True. NOTE: if this API returns a file, it is the responsibility
                 of the caller to close the file stream.
@@ -472,36 +718,207 @@
             _content_type (str/None): force body content-type.
                 Default is None and content-type will be predicted by allowed
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
         Returns:
-            ApplyResult[(CreateEditDeleteViewResponse, int, typing.Dict)]
+            ApplyResult[(CreateViewResponse, int, typing.Dict)]
         """
         self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=True)
-        kwargs['id'] = \
-            id
         return self.create_street_account_view_endpoint.call_with_http_info(**kwargs)
 
 
+    def delete_quickalert_view(
+        self,
+        **kwargs
+    ) -> None:
+        """Deletes an existing quick alert for a view.  # noqa: E501
+
+        This endpoint allows you to delete a quick alert from a previously saved view.  # noqa: E501
+        This method makes a synchronous HTTP request. Returns the http data only
+
+
+        Keyword Args:
+            quick_alerts_body (QuickAlertsBody): View name to get an alert. [optional]
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True. NOTE: if this API returns a file, it is the responsibility
+                of the caller to close the file stream.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+        Returns:
+            None
+                Response Object
+        """
+        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=False)
+        return self.delete_quickalert_view_endpoint.call_with_http_info(**kwargs)
+
+    def delete_quickalert_view_with_http_info(
+        self,
+        **kwargs
+    ) -> typing.Tuple[None, int, typing.MutableMapping]:
+        """Deletes an existing quick alert for a view.  # noqa: E501
+
+        This endpoint allows you to delete a quick alert from a previously saved view.  # noqa: E501
+        This method makes a synchronous HTTP request. Returns http data, http status and headers
+
+
+        Keyword Args:
+            quick_alerts_body (QuickAlertsBody): View name to get an alert. [optional]
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True. NOTE: if this API returns a file, it is the responsibility
+                of the caller to close the file stream.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+        Returns:
+            None
+                Response Object
+            int
+                Http Status Code
+            dict
+                Dictionary of the response headers
+        """
+        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=False)
+        return self.delete_quickalert_view_endpoint.call_with_http_info(**kwargs)
+
+    def delete_quickalert_view_async(
+        self,
+        **kwargs
+    ) -> "ApplyResult[None]":
+        """Deletes an existing quick alert for a view.  # noqa: E501
+
+        This endpoint allows you to delete a quick alert from a previously saved view.  # noqa: E501
+        This method makes a asynchronous HTTP request. Returns the http data, wrapped in ApplyResult
+
+
+        Keyword Args:
+            quick_alerts_body (QuickAlertsBody): View name to get an alert. [optional]
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True. NOTE: if this API returns a file, it is the responsibility
+                of the caller to close the file stream.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+        Returns:
+            ApplyResult[None]
+        """
+        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=True)
+        return self.delete_quickalert_view_endpoint.call_with_http_info(**kwargs)
+
+    def delete_quickalert_view_with_http_info_async(
+        self,
+        **kwargs
+    ) -> "ApplyResult[typing.Tuple[None, int, typing.MutableMapping]]":
+        """Deletes an existing quick alert for a view.  # noqa: E501
+
+        This endpoint allows you to delete a quick alert from a previously saved view.  # noqa: E501
+        This method makes a asynchronous HTTP request. Returns http data, http status and headers, wrapped in ApplyResult
+
+
+        Keyword Args:
+            quick_alerts_body (QuickAlertsBody): View name to get an alert. [optional]
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True. NOTE: if this API returns a file, it is the responsibility
+                of the caller to close the file stream.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+        Returns:
+            ApplyResult[(None, int, typing.Dict)]
+        """
+        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=True)
+        return self.delete_quickalert_view_endpoint.call_with_http_info(**kwargs)
+
+
     def delete_street_account_view(
         self,
-        id,
         **kwargs
-    ) -> CreateEditDeleteViewResponse:
+    ) -> None:
         """Deletes an existing StreetAccount view  # noqa: E501
 
         This endpoint allows you to delete a previously saved StreetAccount view.  # noqa: E501
         This method makes a synchronous HTTP request. Returns the http data only
 
-        Args:
-            id (str): view id of the view to be deleted
 
         Keyword Args:
+            delete_view_body (DeleteViewBody): Delete View Body which needs to be sent with request. [optional]
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True. NOTE: if this API returns a file, it is the responsibility
                 of the caller to close the file stream.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -519,36 +936,32 @@
             _content_type (str/None): force body content-type.
                 Default is None and content-type will be predicted by allowed
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
         Returns:
-            CreateEditDeleteViewResponse
+            None
                 Response Object
         """
         self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=False)
-        kwargs['id'] = \
-            id
         return self.delete_street_account_view_endpoint.call_with_http_info(**kwargs)
 
     def delete_street_account_view_with_http_info(
         self,
-        id,
         **kwargs
-    ) -> typing.Tuple[CreateEditDeleteViewResponse, int, typing.MutableMapping]:
+    ) -> typing.Tuple[None, int, typing.MutableMapping]:
         """Deletes an existing StreetAccount view  # noqa: E501
 
         This endpoint allows you to delete a previously saved StreetAccount view.  # noqa: E501
         This method makes a synchronous HTTP request. Returns http data, http status and headers
 
-        Args:
-            id (str): view id of the view to be deleted
 
         Keyword Args:
+            delete_view_body (DeleteViewBody): Delete View Body which needs to be sent with request. [optional]
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True. NOTE: if this API returns a file, it is the responsibility
                 of the caller to close the file stream.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -566,40 +979,36 @@
             _content_type (str/None): force body content-type.
                 Default is None and content-type will be predicted by allowed
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
         Returns:
-            CreateEditDeleteViewResponse
+            None
                 Response Object
             int
                 Http Status Code
             dict
                 Dictionary of the response headers
         """
         self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=False)
-        kwargs['id'] = \
-            id
         return self.delete_street_account_view_endpoint.call_with_http_info(**kwargs)
 
     def delete_street_account_view_async(
         self,
-        id,
         **kwargs
-    ) -> "ApplyResult[CreateEditDeleteViewResponse]":
+    ) -> "ApplyResult[None]":
         """Deletes an existing StreetAccount view  # noqa: E501
 
         This endpoint allows you to delete a previously saved StreetAccount view.  # noqa: E501
         This method makes a asynchronous HTTP request. Returns the http data, wrapped in ApplyResult
 
-        Args:
-            id (str): view id of the view to be deleted
 
         Keyword Args:
+            delete_view_body (DeleteViewBody): Delete View Body which needs to be sent with request. [optional]
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True. NOTE: if this API returns a file, it is the responsibility
                 of the caller to close the file stream.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -617,35 +1026,31 @@
             _content_type (str/None): force body content-type.
                 Default is None and content-type will be predicted by allowed
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
         Returns:
-            ApplyResult[CreateEditDeleteViewResponse]
+            ApplyResult[None]
         """
         self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=True)
-        kwargs['id'] = \
-            id
         return self.delete_street_account_view_endpoint.call_with_http_info(**kwargs)
 
     def delete_street_account_view_with_http_info_async(
         self,
-        id,
         **kwargs
-    ) -> "ApplyResult[typing.Tuple[CreateEditDeleteViewResponse, int, typing.MutableMapping]]":
+    ) -> "ApplyResult[typing.Tuple[None, int, typing.MutableMapping]]":
         """Deletes an existing StreetAccount view  # noqa: E501
 
         This endpoint allows you to delete a previously saved StreetAccount view.  # noqa: E501
         This method makes a asynchronous HTTP request. Returns http data, http status and headers, wrapped in ApplyResult
 
-        Args:
-            id (str): view id of the view to be deleted
 
         Keyword Args:
+            delete_view_body (DeleteViewBody): Delete View Body which needs to be sent with request. [optional]
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True. NOTE: if this API returns a file, it is the responsibility
                 of the caller to close the file stream.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
@@ -663,34 +1068,29 @@
             _content_type (str/None): force body content-type.
                 Default is None and content-type will be predicted by allowed
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
         Returns:
-            ApplyResult[(CreateEditDeleteViewResponse, int, typing.Dict)]
+            ApplyResult[(None, int, typing.Dict)]
         """
         self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=True)
-        kwargs['id'] = \
-            id
         return self.delete_street_account_view_endpoint.call_with_http_info(**kwargs)
 
 
     def edit_street_account_view(
         self,
-        id,
         **kwargs
-    ) -> CreateEditDeleteViewResponse:
+    ) -> None:
         """Edits and saves an existing StreetAccount view  # noqa: E501
 
         This endpoint allows you to edit the criteria used for a previously saved StreetAccount view.  # noqa: E501
         This method makes a synchronous HTTP request. Returns the http data only
 
-        Args:
-            id (str): view id of the view to be edited
 
         Keyword Args:
             create_or_edit_view_body (CreateOrEditViewBody): Create or Edit View Body which needs to be sent with request. [optional]
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True. NOTE: if this API returns a file, it is the responsibility
                 of the caller to close the file stream.
@@ -711,34 +1111,29 @@
             _content_type (str/None): force body content-type.
                 Default is None and content-type will be predicted by allowed
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
         Returns:
-            CreateEditDeleteViewResponse
+            None
                 Response Object
         """
         self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=False)
-        kwargs['id'] = \
-            id
         return self.edit_street_account_view_endpoint.call_with_http_info(**kwargs)
 
     def edit_street_account_view_with_http_info(
         self,
-        id,
         **kwargs
-    ) -> typing.Tuple[CreateEditDeleteViewResponse, int, typing.MutableMapping]:
+    ) -> typing.Tuple[None, int, typing.MutableMapping]:
         """Edits and saves an existing StreetAccount view  # noqa: E501
 
         This endpoint allows you to edit the criteria used for a previously saved StreetAccount view.  # noqa: E501
         This method makes a synchronous HTTP request. Returns http data, http status and headers
 
-        Args:
-            id (str): view id of the view to be edited
 
         Keyword Args:
             create_or_edit_view_body (CreateOrEditViewBody): Create or Edit View Body which needs to be sent with request. [optional]
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True. NOTE: if this API returns a file, it is the responsibility
                 of the caller to close the file stream.
@@ -759,38 +1154,33 @@
             _content_type (str/None): force body content-type.
                 Default is None and content-type will be predicted by allowed
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
         Returns:
-            CreateEditDeleteViewResponse
+            None
                 Response Object
             int
                 Http Status Code
             dict
                 Dictionary of the response headers
         """
         self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=False)
-        kwargs['id'] = \
-            id
         return self.edit_street_account_view_endpoint.call_with_http_info(**kwargs)
 
     def edit_street_account_view_async(
         self,
-        id,
         **kwargs
-    ) -> "ApplyResult[CreateEditDeleteViewResponse]":
+    ) -> "ApplyResult[None]":
         """Edits and saves an existing StreetAccount view  # noqa: E501
 
         This endpoint allows you to edit the criteria used for a previously saved StreetAccount view.  # noqa: E501
         This method makes a asynchronous HTTP request. Returns the http data, wrapped in ApplyResult
 
-        Args:
-            id (str): view id of the view to be edited
 
         Keyword Args:
             create_or_edit_view_body (CreateOrEditViewBody): Create or Edit View Body which needs to be sent with request. [optional]
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True. NOTE: if this API returns a file, it is the responsibility
                 of the caller to close the file stream.
@@ -811,33 +1201,28 @@
             _content_type (str/None): force body content-type.
                 Default is None and content-type will be predicted by allowed
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
         Returns:
-            ApplyResult[CreateEditDeleteViewResponse]
+            ApplyResult[None]
         """
         self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=True)
-        kwargs['id'] = \
-            id
         return self.edit_street_account_view_endpoint.call_with_http_info(**kwargs)
 
     def edit_street_account_view_with_http_info_async(
         self,
-        id,
         **kwargs
-    ) -> "ApplyResult[typing.Tuple[CreateEditDeleteViewResponse, int, typing.MutableMapping]]":
+    ) -> "ApplyResult[typing.Tuple[None, int, typing.MutableMapping]]":
         """Edits and saves an existing StreetAccount view  # noqa: E501
 
         This endpoint allows you to edit the criteria used for a previously saved StreetAccount view.  # noqa: E501
         This method makes a asynchronous HTTP request. Returns http data, http status and headers, wrapped in ApplyResult
 
-        Args:
-            id (str): view id of the view to be edited
 
         Keyword Args:
             create_or_edit_view_body (CreateOrEditViewBody): Create or Edit View Body which needs to be sent with request. [optional]
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True. NOTE: if this API returns a file, it is the responsibility
                 of the caller to close the file stream.
@@ -858,19 +1243,17 @@
             _content_type (str/None): force body content-type.
                 Default is None and content-type will be predicted by allowed
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
         Returns:
-            ApplyResult[(CreateEditDeleteViewResponse, int, typing.Dict)]
+            ApplyResult[(None, int, typing.Dict)]
         """
         self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=True)
-        kwargs['id'] = \
-            id
         return self.edit_street_account_view_endpoint.call_with_http_info(**kwargs)
 
 
     def get_street_account_views(
         self,
         **kwargs
     ) -> Views:
```

## fds/sdk/StreetAccountNews/apis/__init__.py

```diff
@@ -12,9 +12,8 @@
 #
 #   import sys
 #   sys.setrecursionlimit(n)
 
 # Import APIs into API package:
 from fds.sdk.StreetAccountNews.api.filters_api import FiltersApi
 from fds.sdk.StreetAccountNews.api.headlines_api import HeadlinesApi
-from fds.sdk.StreetAccountNews.api.street_account_historical_stories_api import StreetAccountHistoricalStoriesApi
 from fds.sdk.StreetAccountNews.api.views_api import ViewsApi
```

## fds/sdk/StreetAccountNews/model/create_or_edit_view_body.py

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/StreetAccountNews/model/create_or_edit_view_body_data.py

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -84,35 +84,37 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
+            'name': (str,),  # noqa: E501
             'tickers': ([CreateOrEditViewTickers],),  # noqa: E501
+            'is_primary': (bool,),  # noqa: E501
             'categories': ([str],),  # noqa: E501
-            'regions': ([str],),  # noqa: E501
             'topics': ([str],),  # noqa: E501
+            'regions': ([str],),  # noqa: E501
             'sectors': ([str],),  # noqa: E501
-            'is_primary': (bool,),  # noqa: E501
             'quick_alert': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'name': 'name',  # noqa: E501
         'tickers': 'tickers',  # noqa: E501
+        'is_primary': 'isPrimary',  # noqa: E501
         'categories': 'categories',  # noqa: E501
-        'regions': 'regions',  # noqa: E501
         'topics': 'topics',  # noqa: E501
+        'regions': 'regions',  # noqa: E501
         'sectors': 'sectors',  # noqa: E501
-        'is_primary': 'isPrimary',  # noqa: E501
         'quick_alert': 'quickAlert',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
@@ -149,21 +151,22 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            tickers ([CreateOrEditViewTickers]): [optional]  # noqa: E501
+            name (str): The name of the view.. [optional]  # noqa: E501
+            tickers ([CreateOrEditViewTickers]): An array of ticker objects associated with the view.. [optional]  # noqa: E501
+            is_primary (bool): If true, then only stories with the provided ticker as a primary symbol will be returned. Otherwise, all stories with the ticker as a primary symbol or related symbol will be returned. . [optional]  # noqa: E501
             categories ([str]): [optional]  # noqa: E501
-            regions ([str]): [optional]  # noqa: E501
             topics ([str]): [optional]  # noqa: E501
+            regions ([str]): [optional]  # noqa: E501
             sectors ([str]): [optional]  # noqa: E501
-            is_primary (bool): [optional]  # noqa: E501
-            quick_alert (bool): [optional]  # noqa: E501
+            quick_alert (bool): Indicates whether quick alerts are enabled for the view. A value of 'true' means quick alerts are enabled, while 'false' means they are not. . [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -237,21 +240,22 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            tickers ([CreateOrEditViewTickers]): [optional]  # noqa: E501
+            name (str): The name of the view.. [optional]  # noqa: E501
+            tickers ([CreateOrEditViewTickers]): An array of ticker objects associated with the view.. [optional]  # noqa: E501
+            is_primary (bool): If true, then only stories with the provided ticker as a primary symbol will be returned. Otherwise, all stories with the ticker as a primary symbol or related symbol will be returned. . [optional]  # noqa: E501
             categories ([str]): [optional]  # noqa: E501
-            regions ([str]): [optional]  # noqa: E501
             topics ([str]): [optional]  # noqa: E501
+            regions ([str]): [optional]  # noqa: E501
             sectors ([str]): [optional]  # noqa: E501
-            is_primary (bool): [optional]  # noqa: E501
-            quick_alert (bool): [optional]  # noqa: E501
+            quick_alert (bool): Indicates whether quick alerts are enabled for the view. A value of 'true' means quick alerts are enabled, while 'false' means they are not. . [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## fds/sdk/StreetAccountNews/model/create_or_edit_view_tickers.py

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/StreetAccountNews/model/error.py

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -84,25 +84,23 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'meta': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
             'errors': ([ErrorObject],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'meta': 'meta',  # noqa: E501
         'errors': 'errors',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
@@ -139,15 +137,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
             errors ([ErrorObject]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -222,15 +219,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
             errors ([ErrorObject]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

## fds/sdk/StreetAccountNews/model/error_object.py

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/StreetAccountNews/model/filter_response.py

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/StreetAccountNews/model/filter_response_data.py

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -86,26 +86,26 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'structured_filters': (StructuredFilters,),  # noqa: E501
-            'flattened_filters': (FlattenedFilters,),  # noqa: E501
+            'structured': (StructuredFilters,),  # noqa: E501
+            'flattened': (FlattenedFilters,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'structured_filters': 'structuredFilters',  # noqa: E501
-        'flattened_filters': 'flattenedFilters',  # noqa: E501
+        'structured': 'structured',  # noqa: E501
+        'flattened': 'flattened',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -141,16 +141,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            structured_filters (StructuredFilters): [optional]  # noqa: E501
-            flattened_filters (FlattenedFilters): [optional]  # noqa: E501
+            structured (StructuredFilters): [optional]  # noqa: E501
+            flattened (FlattenedFilters): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -224,16 +224,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            structured_filters (StructuredFilters): [optional]  # noqa: E501
-            flattened_filters (FlattenedFilters): [optional]  # noqa: E501
+            structured (StructuredFilters): [optional]  # noqa: E501
+            flattened (FlattenedFilters): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## fds/sdk/StreetAccountNews/model/flattened_filters.py

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/StreetAccountNews/model/flattened_filters_categories_object.py

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -133,16 +133,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
-            value ([str]): [optional]  # noqa: E501
+            name (str): The name of the category.. [optional]  # noqa: E501
+            value ([str]): An array containing a single value associated with the category. . [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -216,16 +216,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
-            value ([str]): [optional]  # noqa: E501
+            name (str): The name of the category.. [optional]  # noqa: E501
+            value ([str]): An array containing a single value associated with the category. . [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## fds/sdk/StreetAccountNews/model/flattened_filters_regions_object.py

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -79,15 +79,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'name': (str,),  # noqa: E501
-            'value': ([float],),  # noqa: E501
+            'value': ([str],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -133,16 +133,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
-            value ([float]): [optional]  # noqa: E501
+            name (str): The name of the region.. [optional]  # noqa: E501
+            value ([str]): An array containing a single numeric value associated with the region.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -216,16 +216,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
-            value ([float]): [optional]  # noqa: E501
+            name (str): The name of the region.. [optional]  # noqa: E501
+            value ([str]): An array containing a single numeric value associated with the region.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## fds/sdk/StreetAccountNews/model/flattened_filters_sectors_object.py

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -133,16 +133,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
-            value ([float]): [optional]  # noqa: E501
+            name (str): The name of the sector.. [optional]  # noqa: E501
+            value ([float]): An array containing a single numeric value associated with the sector. . [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -216,16 +216,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
-            value ([float]): [optional]  # noqa: E501
+            name (str): The name of the sector.. [optional]  # noqa: E501
+            value ([float]): An array containing a single numeric value associated with the sector. . [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## fds/sdk/StreetAccountNews/model/flattened_filters_topics_object.py

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -133,16 +133,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
-            value ([str]): [optional]  # noqa: E501
+            name (str): The name of the topic.. [optional]  # noqa: E501
+            value ([str]): An array containing a single value associated with the topic.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -216,16 +216,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
-            value ([str]): [optional]  # noqa: E501
+            name (str): The name of the topic.. [optional]  # noqa: E501
+            value ([str]): An array containing a single value associated with the topic.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## fds/sdk/StreetAccountNews/model/flattened_filters_watchlists_object.py

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -135,17 +135,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
-            type (str): [optional]  # noqa: E501
-            value (str): [optional]  # noqa: E501
+            name (str): The name of the watchlist.. [optional]  # noqa: E501
+            type (str): The type of watchlist.. [optional]  # noqa: E501
+            value (str): The value associated with the watchlist.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -219,17 +219,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
-            type (str): [optional]  # noqa: E501
-            value (str): [optional]  # noqa: E501
+            name (str): The name of the watchlist.. [optional]  # noqa: E501
+            type (str): The type of watchlist.. [optional]  # noqa: E501
+            value (str): The value associated with the watchlist.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## fds/sdk/StreetAccountNews/model/search_response_array_object.py

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -78,38 +78,40 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'docs_story_date_and_time': (str,),  # noqa: E501
-            'docs_headlines': (str,),  # noqa: E501
-            'docs_id': (str,),  # noqa: E501
-            'docs_primary_symbols': ([str],),  # noqa: E501
-            'docs_symbols': ([str],),  # noqa: E501
-            'docs_subjects': ([str],),  # noqa: E501
-            'docs_story_body': (str,),  # noqa: E501
-            'docs_reference_uris': (str,),  # noqa: E501
+            'story_time': (datetime,),  # noqa: E501
+            'headlines': (str,),  # noqa: E501
+            'id': (str,),  # noqa: E501
+            'primary_symbols': ([str],),  # noqa: E501
+            'symbols': ([str],),  # noqa: E501
+            'subjects': ([str],),  # noqa: E501
+            'story_body': (str,),  # noqa: E501
+            'reference_uris': (str,),  # noqa: E501
+            'url': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'docs_story_date_and_time': 'docsStoryDateAndTime',  # noqa: E501
-        'docs_headlines': 'docsHeadlines',  # noqa: E501
-        'docs_id': 'docsId',  # noqa: E501
-        'docs_primary_symbols': 'docsPrimarySymbols',  # noqa: E501
-        'docs_symbols': 'docsSymbols',  # noqa: E501
-        'docs_subjects': 'docsSubjects',  # noqa: E501
-        'docs_story_body': 'docsStoryBody',  # noqa: E501
-        'docs_reference_uris': 'docsReferenceUris',  # noqa: E501
+        'story_time': 'storyTime',  # noqa: E501
+        'headlines': 'headlines',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'primary_symbols': 'primarySymbols',  # noqa: E501
+        'symbols': 'symbols',  # noqa: E501
+        'subjects': 'subjects',  # noqa: E501
+        'story_body': 'storyBody',  # noqa: E501
+        'reference_uris': 'referenceUris',  # noqa: E501
+        'url': 'url',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -145,22 +147,23 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            docs_story_date_and_time (str): [optional]  # noqa: E501
-            docs_headlines (str): [optional]  # noqa: E501
-            docs_id (str): [optional]  # noqa: E501
-            docs_primary_symbols ([str]): [optional]  # noqa: E501
-            docs_symbols ([str]): [optional]  # noqa: E501
-            docs_subjects ([str]): [optional]  # noqa: E501
-            docs_story_body (str): [optional]  # noqa: E501
-            docs_reference_uris (str): [optional]  # noqa: E501
+            story_time (datetime): The timestamp when the story was published.. [optional]  # noqa: E501
+            headlines (str): The headline of the story.. [optional]  # noqa: E501
+            id (str): The unique identifier for the story.. [optional]  # noqa: E501
+            primary_symbols ([str]): [optional]  # noqa: E501
+            symbols ([str]): [optional]  # noqa: E501
+            subjects ([str]): [optional]  # noqa: E501
+            story_body (str): The sample body of the story.. [optional]  # noqa: E501
+            reference_uris (str): The reference URIs associated with the story.. [optional]  # noqa: E501
+            url (str): The URL of the story.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -234,22 +237,23 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            docs_story_date_and_time (str): [optional]  # noqa: E501
-            docs_headlines (str): [optional]  # noqa: E501
-            docs_id (str): [optional]  # noqa: E501
-            docs_primary_symbols ([str]): [optional]  # noqa: E501
-            docs_symbols ([str]): [optional]  # noqa: E501
-            docs_subjects ([str]): [optional]  # noqa: E501
-            docs_story_body (str): [optional]  # noqa: E501
-            docs_reference_uris (str): [optional]  # noqa: E501
+            story_time (datetime): The timestamp when the story was published.. [optional]  # noqa: E501
+            headlines (str): The headline of the story.. [optional]  # noqa: E501
+            id (str): The unique identifier for the story.. [optional]  # noqa: E501
+            primary_symbols ([str]): [optional]  # noqa: E501
+            symbols ([str]): [optional]  # noqa: E501
+            subjects ([str]): [optional]  # noqa: E501
+            story_body (str): The sample body of the story.. [optional]  # noqa: E501
+            reference_uris (str): The reference URIs associated with the story.. [optional]  # noqa: E501
+            url (str): The URL of the story.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## fds/sdk/StreetAccountNews/model/structured_filters.py

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/StreetAccountNews/model/structured_filters_categories_object.py

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,16 +27,16 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.StreetAccountNews.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fds.sdk.StreetAccountNews.model.structured_filters_children_object import StructuredFiltersChildrenObject
-    globals()['StructuredFiltersChildrenObject'] = StructuredFiltersChildrenObject
+    from fds.sdk.StreetAccountNews.model.structured_filters_children_object_categories import StructuredFiltersChildrenObjectCategories
+    globals()['StructuredFiltersChildrenObjectCategories'] = StructuredFiltersChildrenObjectCategories
 
 
 class StructuredFiltersCategoriesObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -86,15 +86,15 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
             'value': ([str],),  # noqa: E501
-            'children': ([StructuredFiltersChildrenObject],),  # noqa: E501
+            'children': ([StructuredFiltersChildrenObjectCategories],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -141,17 +141,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
+            name (str): The name of the category.. [optional]  # noqa: E501
             value ([str]): [optional]  # noqa: E501
-            children ([StructuredFiltersChildrenObject]): [optional]  # noqa: E501
+            children ([StructuredFiltersChildrenObjectCategories]): An array of children objects.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -225,17 +225,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
+            name (str): The name of the category.. [optional]  # noqa: E501
             value ([str]): [optional]  # noqa: E501
-            children ([StructuredFiltersChildrenObject]): [optional]  # noqa: E501
+            children ([StructuredFiltersChildrenObjectCategories]): An array of children objects.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## fds/sdk/StreetAccountNews/model/structured_filters_regions_object.py

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -26,14 +26,18 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.StreetAccountNews.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from fds.sdk.StreetAccountNews.model.structured_filters_children_object_regions import StructuredFiltersChildrenObjectRegions
+    globals()['StructuredFiltersChildrenObjectRegions'] = StructuredFiltersChildrenObjectRegions
+
 
 class StructuredFiltersRegionsObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
@@ -63,41 +67,45 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
             'name': (str,),  # noqa: E501
-            'value': ([float],),  # noqa: E501
+            'value': ([str],),  # noqa: E501
+            'children': ([StructuredFiltersChildrenObjectRegions],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'value': 'value',  # noqa: E501
+        'children': 'children',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -133,16 +141,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
-            value ([float]): [optional]  # noqa: E501
+            name (str): The name of the region.. [optional]  # noqa: E501
+            value ([str]): [optional]  # noqa: E501
+            children ([StructuredFiltersChildrenObjectRegions]): An array of children objects.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -216,16 +225,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
-            value ([float]): [optional]  # noqa: E501
+            name (str): The name of the region.. [optional]  # noqa: E501
+            value ([str]): [optional]  # noqa: E501
+            children ([StructuredFiltersChildrenObjectRegions]): An array of children objects.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## fds/sdk/StreetAccountNews/model/structured_filters_sectors_object.py

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,16 +27,16 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.StreetAccountNews.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fds.sdk.StreetAccountNews.model.structured_filters_children_object import StructuredFiltersChildrenObject
-    globals()['StructuredFiltersChildrenObject'] = StructuredFiltersChildrenObject
+    from fds.sdk.StreetAccountNews.model.structured_filters_children_object_sectors import StructuredFiltersChildrenObjectSectors
+    globals()['StructuredFiltersChildrenObjectSectors'] = StructuredFiltersChildrenObjectSectors
 
 
 class StructuredFiltersSectorsObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -86,26 +86,28 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
             'expanded': (bool,),  # noqa: E501
-            'children': ([StructuredFiltersChildrenObject],),  # noqa: E501
+            'children': ([StructuredFiltersChildrenObjectSectors],),  # noqa: E501
+            'value': ([float],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'expanded': 'expanded',  # noqa: E501
         'children': 'children',  # noqa: E501
+        'value': 'value',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -141,17 +143,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
-            expanded (bool): [optional]  # noqa: E501
-            children ([StructuredFiltersChildrenObject]): [optional]  # noqa: E501
+            name (str): The name of the sector. [optional]  # noqa: E501
+            expanded (bool): It returns the boolean value.. [optional]  # noqa: E501
+            children ([StructuredFiltersChildrenObjectSectors]): An array of child objects representing sectors.. [optional]  # noqa: E501
+            value ([float]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -225,17 +228,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
-            expanded (bool): [optional]  # noqa: E501
-            children ([StructuredFiltersChildrenObject]): [optional]  # noqa: E501
+            name (str): The name of the sector. [optional]  # noqa: E501
+            expanded (bool): It returns the boolean value.. [optional]  # noqa: E501
+            children ([StructuredFiltersChildrenObjectSectors]): An array of child objects representing sectors.. [optional]  # noqa: E501
+            value ([float]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## fds/sdk/StreetAccountNews/model/structured_filters_topics_object.py

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,16 +27,16 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.StreetAccountNews.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fds.sdk.StreetAccountNews.model.structured_filters_children_object import StructuredFiltersChildrenObject
-    globals()['StructuredFiltersChildrenObject'] = StructuredFiltersChildrenObject
+    from fds.sdk.StreetAccountNews.model.structured_filters_children_object_topics import StructuredFiltersChildrenObjectTopics
+    globals()['StructuredFiltersChildrenObjectTopics'] = StructuredFiltersChildrenObjectTopics
 
 
 class StructuredFiltersTopicsObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -86,15 +86,15 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
             'value': ([str],),  # noqa: E501
-            'children': ([StructuredFiltersChildrenObject],),  # noqa: E501
+            'children': ([StructuredFiltersChildrenObjectTopics],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -141,17 +141,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
+            name (str): The name of the topic.. [optional]  # noqa: E501
             value ([str]): [optional]  # noqa: E501
-            children ([StructuredFiltersChildrenObject]): [optional]  # noqa: E501
+            children ([StructuredFiltersChildrenObjectTopics]): An array of child objects.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -225,17 +225,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
+            name (str): The name of the topic.. [optional]  # noqa: E501
             value ([str]): [optional]  # noqa: E501
-            children ([StructuredFiltersChildrenObject]): [optional]  # noqa: E501
+            children ([StructuredFiltersChildrenObjectTopics]): An array of child objects.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## fds/sdk/StreetAccountNews/model/structured_filters_watchlists_object.py

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -135,17 +135,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
-            type (str): [optional]  # noqa: E501
-            value (str): [optional]  # noqa: E501
+            name (str): The name of the watchlist.. [optional]  # noqa: E501
+            type (str): The type of watchlist.. [optional]  # noqa: E501
+            value (str): The value associated with the watchlist.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -219,17 +219,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
-            type (str): [optional]  # noqa: E501
-            value (str): [optional]  # noqa: E501
+            name (str): The name of the watchlist.. [optional]  # noqa: E501
+            type (str): The type of watchlist.. [optional]  # noqa: E501
+            value (str): The value associated with the watchlist.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## fds/sdk/StreetAccountNews/model/views.py

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/StreetAccountNews/model/views_object.py

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -26,14 +26,18 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.StreetAccountNews.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from fds.sdk.StreetAccountNews.model.create_or_edit_view_tickers import CreateOrEditViewTickers
+    globals()['CreateOrEditViewTickers'] = CreateOrEditViewTickers
+
 
 class ViewsObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
@@ -63,51 +67,53 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'view_name': (str,),  # noqa: E501
-            'tickers': ([str],),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'tickers': ([CreateOrEditViewTickers],),  # noqa: E501
+            'is_primary': (bool,),  # noqa: E501
             'categories': ([str],),  # noqa: E501
             'topics': ([str],),  # noqa: E501
             'regions': ([str],),  # noqa: E501
             'sectors': ([str],),  # noqa: E501
-            'is_primary': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'view_name': 'viewName',  # noqa: E501
+        'name': 'name',  # noqa: E501
         'tickers': 'tickers',  # noqa: E501
+        'is_primary': 'isPrimary',  # noqa: E501
         'categories': 'categories',  # noqa: E501
         'topics': 'topics',  # noqa: E501
         'regions': 'regions',  # noqa: E501
         'sectors': 'sectors',  # noqa: E501
-        'is_primary': 'isPrimary',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -143,21 +149,21 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            view_name (str): [optional]  # noqa: E501
-            tickers ([str]): [optional]  # noqa: E501
+            name (str): The name of the view.. [optional]  # noqa: E501
+            tickers ([CreateOrEditViewTickers]): An array of ticker symbols associated with the view.. [optional]  # noqa: E501
+            is_primary (bool): If true, then only stories with the provided ticker as a primary symbol will be returned. Otherwise, all stories with the ticker as a primary symbol or related symbol will be returned.            . [optional]  # noqa: E501
             categories ([str]): [optional]  # noqa: E501
             topics ([str]): [optional]  # noqa: E501
             regions ([str]): [optional]  # noqa: E501
             sectors ([str]): [optional]  # noqa: E501
-            is_primary (bool): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -231,21 +237,21 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            view_name (str): [optional]  # noqa: E501
-            tickers ([str]): [optional]  # noqa: E501
+            name (str): The name of the view.. [optional]  # noqa: E501
+            tickers ([CreateOrEditViewTickers]): An array of ticker symbols associated with the view.. [optional]  # noqa: E501
+            is_primary (bool): If true, then only stories with the provided ticker as a primary symbol will be returned. Otherwise, all stories with the ticker as a primary symbol or related symbol will be returned.            . [optional]  # noqa: E501
             categories ([str]): [optional]  # noqa: E501
             topics ([str]): [optional]  # noqa: E501
             regions ([str]): [optional]  # noqa: E501
             sectors ([str]): [optional]  # noqa: E501
-            is_primary (bool): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## fds/sdk/StreetAccountNews/models/__init__.py

```diff
@@ -5,54 +5,72 @@
 # raise a RecursionError
 # to avoid this, import only the models that you directly need like:
 # from from fds.sdk.StreetAccountNews.model.pet import Pet
 # or import this package, but before doing it, use:
 # import sys
 # sys.setrecursionlimit(n)
 
-from fds.sdk.StreetAccountNews.model.checkstatus import Checkstatus
-from fds.sdk.StreetAccountNews.model.checkstatus_response import CheckstatusResponse
-from fds.sdk.StreetAccountNews.model.create_edit_delete_view_response import CreateEditDeleteViewResponse
-from fds.sdk.StreetAccountNews.model.create_edit_delete_view_response_data import CreateEditDeleteViewResponseData
-from fds.sdk.StreetAccountNews.model.create_edit_delete_view_response_data_message import CreateEditDeleteViewResponseDataMessage
 from fds.sdk.StreetAccountNews.model.create_or_edit_view_body import CreateOrEditViewBody
 from fds.sdk.StreetAccountNews.model.create_or_edit_view_body_data import CreateOrEditViewBodyData
 from fds.sdk.StreetAccountNews.model.create_or_edit_view_tickers import CreateOrEditViewTickers
+from fds.sdk.StreetAccountNews.model.create_view_response import CreateViewResponse
+from fds.sdk.StreetAccountNews.model.create_view_response_data import CreateViewResponseData
+from fds.sdk.StreetAccountNews.model.delete_view_body import DeleteViewBody
+from fds.sdk.StreetAccountNews.model.delete_view_body_data import DeleteViewBodyData
 from fds.sdk.StreetAccountNews.model.error import Error
 from fds.sdk.StreetAccountNews.model.error_object import ErrorObject
+from fds.sdk.StreetAccountNews.model.filter_categories_response import FilterCategoriesResponse
+from fds.sdk.StreetAccountNews.model.filter_categories_response_data import FilterCategoriesResponseData
+from fds.sdk.StreetAccountNews.model.filter_regions_response import FilterRegionsResponse
+from fds.sdk.StreetAccountNews.model.filter_regions_response_data import FilterRegionsResponseData
 from fds.sdk.StreetAccountNews.model.filter_response import FilterResponse
 from fds.sdk.StreetAccountNews.model.filter_response_data import FilterResponseData
+from fds.sdk.StreetAccountNews.model.filter_sectors_response import FilterSectorsResponse
+from fds.sdk.StreetAccountNews.model.filter_sectors_response_data import FilterSectorsResponseData
+from fds.sdk.StreetAccountNews.model.filter_topic_response import FilterTopicResponse
+from fds.sdk.StreetAccountNews.model.filter_topic_response_data import FilterTopicResponseData
+from fds.sdk.StreetAccountNews.model.filter_watchlists_response import FilterWatchlistsResponse
+from fds.sdk.StreetAccountNews.model.filter_watchlists_response_data import FilterWatchlistsResponseData
 from fds.sdk.StreetAccountNews.model.flattened_filters import FlattenedFilters
+from fds.sdk.StreetAccountNews.model.flattened_filters_categories import FlattenedFiltersCategories
 from fds.sdk.StreetAccountNews.model.flattened_filters_categories_object import FlattenedFiltersCategoriesObject
+from fds.sdk.StreetAccountNews.model.flattened_filters_regions import FlattenedFiltersRegions
 from fds.sdk.StreetAccountNews.model.flattened_filters_regions_object import FlattenedFiltersRegionsObject
+from fds.sdk.StreetAccountNews.model.flattened_filters_sectors import FlattenedFiltersSectors
 from fds.sdk.StreetAccountNews.model.flattened_filters_sectors_object import FlattenedFiltersSectorsObject
+from fds.sdk.StreetAccountNews.model.flattened_filters_topics import FlattenedFiltersTopics
 from fds.sdk.StreetAccountNews.model.flattened_filters_topics_object import FlattenedFiltersTopicsObject
+from fds.sdk.StreetAccountNews.model.flattened_filters_watchlists import FlattenedFiltersWatchlists
 from fds.sdk.StreetAccountNews.model.flattened_filters_watchlists_object import FlattenedFiltersWatchlistsObject
-from fds.sdk.StreetAccountNews.model.getfiles import Getfiles
-from fds.sdk.StreetAccountNews.model.getfiles_response import GetfilesResponse
-from fds.sdk.StreetAccountNews.model.is_partial_one import IsPartialOne
-from fds.sdk.StreetAccountNews.model.meta_one import MetaOne
-from fds.sdk.StreetAccountNews.model.pagination_one import PaginationOne
-from fds.sdk.StreetAccountNews.model.requestfiles_response import RequestfilesResponse
-from fds.sdk.StreetAccountNews.model.sa_headlines_request import SaHeadlinesRequest
-from fds.sdk.StreetAccountNews.model.sa_headlines_request_by_view import SaHeadlinesRequestByView
-from fds.sdk.StreetAccountNews.model.sa_headlines_request_by_view_data import SaHeadlinesRequestByViewData
-from fds.sdk.StreetAccountNews.model.sa_headlines_request_data import SaHeadlinesRequestData
-from fds.sdk.StreetAccountNews.model.sa_headlines_request_data_search_date import SaHeadlinesRequestDataSearchDate
-from fds.sdk.StreetAccountNews.model.sa_headlines_request_meta import SaHeadlinesRequestMeta
-from fds.sdk.StreetAccountNews.model.sa_headlines_request_meta_pagination import SaHeadlinesRequestMetaPagination
-from fds.sdk.StreetAccountNews.model.sa_headlines_request_tickers_object import SaHeadlinesRequestTickersObject
-from fds.sdk.StreetAccountNews.model.search_response import SearchResponse
+from fds.sdk.StreetAccountNews.model.headlines_request import HeadlinesRequest
+from fds.sdk.StreetAccountNews.model.headlines_request_by_view import HeadlinesRequestByView
+from fds.sdk.StreetAccountNews.model.headlines_request_by_view_data import HeadlinesRequestByViewData
+from fds.sdk.StreetAccountNews.model.headlines_request_by_view_meta import HeadlinesRequestByViewMeta
+from fds.sdk.StreetAccountNews.model.headlines_request_data import HeadlinesRequestData
+from fds.sdk.StreetAccountNews.model.headlines_request_data_search_time import HeadlinesRequestDataSearchTime
+from fds.sdk.StreetAccountNews.model.headlines_request_meta import HeadlinesRequestMeta
+from fds.sdk.StreetAccountNews.model.headlines_request_meta_pagination import HeadlinesRequestMetaPagination
+from fds.sdk.StreetAccountNews.model.headlines_request_tickers_object import HeadlinesRequestTickersObject
+from fds.sdk.StreetAccountNews.model.headlines_response import HeadlinesResponse
+from fds.sdk.StreetAccountNews.model.headlines_response_meta import HeadlinesResponseMeta
+from fds.sdk.StreetAccountNews.model.headlines_response_meta_pagination import HeadlinesResponseMetaPagination
+from fds.sdk.StreetAccountNews.model.quick_alerts_body import QuickAlertsBody
+from fds.sdk.StreetAccountNews.model.quick_alerts_body_data import QuickAlertsBodyData
+from fds.sdk.StreetAccountNews.model.quick_alerts_response import QuickAlertsResponse
 from fds.sdk.StreetAccountNews.model.search_response_array_object import SearchResponseArrayObject
-from fds.sdk.StreetAccountNews.model.search_response_data import SearchResponseData
-from fds.sdk.StreetAccountNews.model.search_response_meta import SearchResponseMeta
-from fds.sdk.StreetAccountNews.model.search_response_meta_pagination import SearchResponseMetaPagination
-from fds.sdk.StreetAccountNews.model.street_account_status import StreetAccountStatus
 from fds.sdk.StreetAccountNews.model.structured_filters import StructuredFilters
+from fds.sdk.StreetAccountNews.model.structured_filters_categories import StructuredFiltersCategories
 from fds.sdk.StreetAccountNews.model.structured_filters_categories_object import StructuredFiltersCategoriesObject
-from fds.sdk.StreetAccountNews.model.structured_filters_children_object import StructuredFiltersChildrenObject
+from fds.sdk.StreetAccountNews.model.structured_filters_children_object_categories import StructuredFiltersChildrenObjectCategories
+from fds.sdk.StreetAccountNews.model.structured_filters_children_object_regions import StructuredFiltersChildrenObjectRegions
+from fds.sdk.StreetAccountNews.model.structured_filters_children_object_sectors import StructuredFiltersChildrenObjectSectors
+from fds.sdk.StreetAccountNews.model.structured_filters_children_object_topics import StructuredFiltersChildrenObjectTopics
+from fds.sdk.StreetAccountNews.model.structured_filters_regions import StructuredFiltersRegions
 from fds.sdk.StreetAccountNews.model.structured_filters_regions_object import StructuredFiltersRegionsObject
+from fds.sdk.StreetAccountNews.model.structured_filters_sectors import StructuredFiltersSectors
 from fds.sdk.StreetAccountNews.model.structured_filters_sectors_object import StructuredFiltersSectorsObject
+from fds.sdk.StreetAccountNews.model.structured_filters_topics import StructuredFiltersTopics
 from fds.sdk.StreetAccountNews.model.structured_filters_topics_object import StructuredFiltersTopicsObject
+from fds.sdk.StreetAccountNews.model.structured_filters_watchlists import StructuredFiltersWatchlists
 from fds.sdk.StreetAccountNews.model.structured_filters_watchlists_object import StructuredFiltersWatchlistsObject
 from fds.sdk.StreetAccountNews.model.views import Views
 from fds.sdk.StreetAccountNews.model.views_object import ViewsObject
```

## Comparing `fds/sdk/StreetAccountNews/model/checkstatus.py` & `fds/sdk/StreetAccountNews/model/headlines_request_by_view_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.StreetAccountNews.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from fds.sdk.StreetAccountNews.model.headlines_request_data_search_time import HeadlinesRequestDataSearchTime
+    globals()['HeadlinesRequestDataSearchTime'] = HeadlinesRequestDataSearchTime
 
-class Checkstatus(ModelNormal):
+
+class HeadlinesRequestByViewData(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -52,73 +56,80 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('predefined_range',): {
+            'TODAY': "today",
+            'TWODAYS': "twoDays",
+            'ONEWEEK': "oneWeek",
+            'ONEMONTH': "oneMonth",
+            'THREEMONTHS': "threeMonths",
+            'SIXMONTHS': "sixMonths",
+            'ONEYEAR': "oneYear",
+            'THREEYEARS': "threeYears",
+            'FIVEYEARS': "fiveYears",
+            'TENYEARS': "tenYears",
+            'ALLAVAILABLE': "allAvailable",
+        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'product': (str,),  # noqa: E501
-            'job_id': (str,),  # noqa: E501
-            'status': (str,),  # noqa: E501
-            'percent_done': (int,),  # noqa: E501
-            'start_date': (date,),  # noqa: E501
-            'end_date': (date,),  # noqa: E501
-            'part': (int,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'predefined_range': (str,),  # noqa: E501
+            'search_time': (HeadlinesRequestDataSearchTime,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'product': 'product',  # noqa: E501
-        'job_id': 'jobID',  # noqa: E501
-        'status': 'status',  # noqa: E501
-        'percent_done': 'percentDone',  # noqa: E501
-        'start_date': 'startDate',  # noqa: E501
-        'end_date': 'endDate',  # noqa: E501
-        'part': 'part',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'predefined_range': 'predefinedRange',  # noqa: E501
+        'search_time': 'searchTime',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Checkstatus - a model defined in OpenAPI
+        """HeadlinesRequestByViewData - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -143,21 +154,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            product (str): Defines the name of the product. [optional]  # noqa: E501
-            job_id (str): Unique id to get the xml files for the requested date. [optional]  # noqa: E501
-            status (str): Returns any of the 2 results Submitted ->Running->Completed and Failed. [optional]  # noqa: E501
-            percent_done (int): Returns how much percentage of  task is completed for the requested jobID. [optional]  # noqa: E501
-            start_date (date): The date from which the data is required in YYYY-MM-DDTHH:MM:SSZ format. [optional]  # noqa: E501
-            end_date (date): The date until which the data is fetched in YYYY-MM-DDTHH:MM:SSZ format. [optional]  # noqa: E501
-            part (int): Returns the part number of the jobID. [optional]  # noqa: E501
+            name (str): View name of the view to return headlines for. [optional]  # noqa: E501
+            predefined_range (str): see list of valid date ranges. Date range is mutually exlusive to start/end time. [optional]  # noqa: E501
+            search_time (HeadlinesRequestDataSearchTime): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -198,15 +205,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """Checkstatus - a model defined in OpenAPI
+        """HeadlinesRequestByViewData - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -231,21 +238,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            product (str): Defines the name of the product. [optional]  # noqa: E501
-            job_id (str): Unique id to get the xml files for the requested date. [optional]  # noqa: E501
-            status (str): Returns any of the 2 results Submitted ->Running->Completed and Failed. [optional]  # noqa: E501
-            percent_done (int): Returns how much percentage of  task is completed for the requested jobID. [optional]  # noqa: E501
-            start_date (date): The date from which the data is required in YYYY-MM-DDTHH:MM:SSZ format. [optional]  # noqa: E501
-            end_date (date): The date until which the data is fetched in YYYY-MM-DDTHH:MM:SSZ format. [optional]  # noqa: E501
-            part (int): Returns the part number of the jobID. [optional]  # noqa: E501
+            name (str): View name of the view to return headlines for. [optional]  # noqa: E501
+            predefined_range (str): see list of valid date ranges. Date range is mutually exlusive to start/end time. [optional]  # noqa: E501
+            search_time (HeadlinesRequestDataSearchTime): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## Comparing `fds/sdk/StreetAccountNews/model/checkstatus_response.py` & `fds/sdk/StreetAccountNews/model/headlines_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,21 +27,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.StreetAccountNews.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fds.sdk.StreetAccountNews.model.checkstatus import Checkstatus
-    from fds.sdk.StreetAccountNews.model.meta_one import MetaOne
-    globals()['Checkstatus'] = Checkstatus
-    globals()['MetaOne'] = MetaOne
+    from fds.sdk.StreetAccountNews.model.headlines_response_meta import HeadlinesResponseMeta
+    from fds.sdk.StreetAccountNews.model.search_response_array_object import SearchResponseArrayObject
+    globals()['HeadlinesResponseMeta'] = HeadlinesResponseMeta
+    globals()['SearchResponseArrayObject'] = SearchResponseArrayObject
 
 
-class CheckstatusResponse(ModelNormal):
+class HeadlinesResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -86,16 +86,16 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': ([Checkstatus],),  # noqa: E501
-            'meta': (MetaOne,),  # noqa: E501
+            'data': ([SearchResponseArrayObject],),  # noqa: E501
+            'meta': (HeadlinesResponseMeta,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -108,15 +108,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """CheckstatusResponse - a model defined in OpenAPI
+        """HeadlinesResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -141,16 +141,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([Checkstatus]): [optional]  # noqa: E501
-            meta (MetaOne): [optional]  # noqa: E501
+            data ([SearchResponseArrayObject]): [optional]  # noqa: E501
+            meta (HeadlinesResponseMeta): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -191,15 +191,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """CheckstatusResponse - a model defined in OpenAPI
+        """HeadlinesResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -224,16 +224,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([Checkstatus]): [optional]  # noqa: E501
-            meta (MetaOne): [optional]  # noqa: E501
+            data ([SearchResponseArrayObject]): [optional]  # noqa: E501
+            meta (HeadlinesResponseMeta): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## Comparing `fds/sdk/StreetAccountNews/model/create_edit_delete_view_response.py` & `fds/sdk/StreetAccountNews/model/headlines_response_meta.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.StreetAccountNews.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fds.sdk.StreetAccountNews.model.create_edit_delete_view_response_data import CreateEditDeleteViewResponseData
-    globals()['CreateEditDeleteViewResponseData'] = CreateEditDeleteViewResponseData
+    from fds.sdk.StreetAccountNews.model.headlines_response_meta_pagination import HeadlinesResponseMetaPagination
+    globals()['HeadlinesResponseMetaPagination'] = HeadlinesResponseMetaPagination
 
 
-class CreateEditDeleteViewResponse(ModelNormal):
+class HeadlinesResponseMeta(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,35 +84,37 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (CreateEditDeleteViewResponseData,),  # noqa: E501
+            'request_guid': (str,),  # noqa: E501
+            'pagination': (HeadlinesResponseMetaPagination,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
+        'request_guid': 'requestGuid',  # noqa: E501
+        'pagination': 'pagination',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """CreateEditDeleteViewResponse - a model defined in OpenAPI
+        """HeadlinesResponseMeta - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -137,15 +139,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (CreateEditDeleteViewResponseData): [optional]  # noqa: E501
+            request_guid (str): Identifier to get general information about the request that produced that search response.. [optional]  # noqa: E501
+            pagination (HeadlinesResponseMetaPagination): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -186,15 +189,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """CreateEditDeleteViewResponse - a model defined in OpenAPI
+        """HeadlinesResponseMeta - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -219,15 +222,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (CreateEditDeleteViewResponseData): [optional]  # noqa: E501
+            request_guid (str): Identifier to get general information about the request that produced that search response.. [optional]  # noqa: E501
+            pagination (HeadlinesResponseMetaPagination): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## Comparing `fds/sdk/StreetAccountNews/model/create_edit_delete_view_response_data.py` & `fds/sdk/StreetAccountNews/model/filter_categories_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.StreetAccountNews.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fds.sdk.StreetAccountNews.model.create_edit_delete_view_response_data_message import CreateEditDeleteViewResponseDataMessage
-    globals()['CreateEditDeleteViewResponseDataMessage'] = CreateEditDeleteViewResponseDataMessage
+    from fds.sdk.StreetAccountNews.model.filter_categories_response_data import FilterCategoriesResponseData
+    globals()['FilterCategoriesResponseData'] = FilterCategoriesResponseData
 
 
-class CreateEditDeleteViewResponseData(ModelNormal):
+class FilterCategoriesResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,37 +84,35 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'id': (str,),  # noqa: E501
-            'message': (CreateEditDeleteViewResponseDataMessage,),  # noqa: E501
+            'data': (FilterCategoriesResponseData,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
-        'message': 'message',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """CreateEditDeleteViewResponseData - a model defined in OpenAPI
+        """FilterCategoriesResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -139,16 +137,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
-            message (CreateEditDeleteViewResponseDataMessage): [optional]  # noqa: E501
+            data (FilterCategoriesResponseData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -189,15 +186,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """CreateEditDeleteViewResponseData - a model defined in OpenAPI
+        """FilterCategoriesResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -222,16 +219,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
-            message (CreateEditDeleteViewResponseDataMessage): [optional]  # noqa: E501
+            data (FilterCategoriesResponseData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## Comparing `fds/sdk/StreetAccountNews/model/create_edit_delete_view_response_data_message.py` & `fds/sdk/StreetAccountNews/model/headlines_request_by_view_meta.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.StreetAccountNews.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from fds.sdk.StreetAccountNews.model.headlines_request_meta_pagination import HeadlinesRequestMetaPagination
+    globals()['HeadlinesRequestMetaPagination'] = HeadlinesRequestMetaPagination
 
-class CreateEditDeleteViewResponseDataMessage(ModelNormal):
+
+class HeadlinesRequestByViewMeta(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,50 +67,52 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'view': (str,),  # noqa: E501
+            'pagination': (HeadlinesRequestMetaPagination,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'view': 'view',  # noqa: E501
+        'pagination': 'pagination',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """CreateEditDeleteViewResponseDataMessage - a model defined in OpenAPI
+        """HeadlinesRequestByViewMeta - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -131,15 +137,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            view (str): [optional]  # noqa: E501
+            pagination (HeadlinesRequestMetaPagination): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -180,15 +186,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """CreateEditDeleteViewResponseDataMessage - a model defined in OpenAPI
+        """HeadlinesRequestByViewMeta - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -213,15 +219,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            view (str): [optional]  # noqa: E501
+            pagination (HeadlinesRequestMetaPagination): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## Comparing `fds/sdk/StreetAccountNews/model/getfiles.py` & `fds/sdk/StreetAccountNews/model/headlines_response_meta_pagination.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.StreetAccountNews.exceptions import ApiAttributeError
 
 
 
-class Getfiles(ModelNormal):
+class HeadlinesResponseMetaPagination(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,47 +78,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'product': (str,),  # noqa: E501
-            'start_date': (date,),  # noqa: E501
-            'end_date': (date,),  # noqa: E501
-            'job_id': (str,),  # noqa: E501
-            'status': (str,),  # noqa: E501
-            'url': (str,),  # noqa: E501
-            'part': (int,),  # noqa: E501
+            'total': (int,),  # noqa: E501
+            'is_estimated_total': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'product': 'product',  # noqa: E501
-        'start_date': 'startDate',  # noqa: E501
-        'end_date': 'endDate',  # noqa: E501
-        'job_id': 'jobID',  # noqa: E501
-        'status': 'status',  # noqa: E501
-        'url': 'url',  # noqa: E501
-        'part': 'part',  # noqa: E501
+        'total': 'total',  # noqa: E501
+        'is_estimated_total': 'isEstimatedTotal',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Getfiles - a model defined in OpenAPI
+        """HeadlinesResponseMetaPagination - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -143,21 +133,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            product (str): Defines the name of the product. [optional]  # noqa: E501
-            start_date (date): The startDate from which the data is required in YYYY-MM-DDTHH:MM:SSZ format. [optional]  # noqa: E501
-            end_date (date): The endDate until which the data is fetched in YYYY-MM-DDTHH:MM:SSZ format. [optional]  # noqa: E501
-            job_id (str): Unique id to get the xml files for the requested date. [optional]  # noqa: E501
-            status (str): Defines the status of the request. [optional]  # noqa: E501
-            url (str): Link to download the zip file which contains xml files. [optional]  # noqa: E501
-            part (int): Returns the part number of the jobID. [optional]  # noqa: E501
+            total (int): [optional]  # noqa: E501
+            is_estimated_total (bool): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -198,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """Getfiles - a model defined in OpenAPI
+        """HeadlinesResponseMetaPagination - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -231,21 +216,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            product (str): Defines the name of the product. [optional]  # noqa: E501
-            start_date (date): The startDate from which the data is required in YYYY-MM-DDTHH:MM:SSZ format. [optional]  # noqa: E501
-            end_date (date): The endDate until which the data is fetched in YYYY-MM-DDTHH:MM:SSZ format. [optional]  # noqa: E501
-            job_id (str): Unique id to get the xml files for the requested date. [optional]  # noqa: E501
-            status (str): Defines the status of the request. [optional]  # noqa: E501
-            url (str): Link to download the zip file which contains xml files. [optional]  # noqa: E501
-            part (int): Returns the part number of the jobID. [optional]  # noqa: E501
+            total (int): [optional]  # noqa: E501
+            is_estimated_total (bool): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## Comparing `fds/sdk/StreetAccountNews/model/getfiles_response.py` & `fds/sdk/StreetAccountNews/model/headlines_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,21 +27,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.StreetAccountNews.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fds.sdk.StreetAccountNews.model.getfiles import Getfiles
-    from fds.sdk.StreetAccountNews.model.meta_one import MetaOne
-    globals()['Getfiles'] = Getfiles
-    globals()['MetaOne'] = MetaOne
+    from fds.sdk.StreetAccountNews.model.headlines_request_data import HeadlinesRequestData
+    from fds.sdk.StreetAccountNews.model.headlines_request_meta import HeadlinesRequestMeta
+    globals()['HeadlinesRequestData'] = HeadlinesRequestData
+    globals()['HeadlinesRequestMeta'] = HeadlinesRequestMeta
 
 
-class GetfilesResponse(ModelNormal):
+class HeadlinesRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -86,16 +86,16 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': ([Getfiles],),  # noqa: E501
-            'meta': (MetaOne,),  # noqa: E501
+            'data': (HeadlinesRequestData,),  # noqa: E501
+            'meta': (HeadlinesRequestMeta,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -108,15 +108,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """GetfilesResponse - a model defined in OpenAPI
+        """HeadlinesRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -141,16 +141,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([Getfiles]): [optional]  # noqa: E501
-            meta (MetaOne): [optional]  # noqa: E501
+            data (HeadlinesRequestData): [optional]  # noqa: E501
+            meta (HeadlinesRequestMeta): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -191,15 +191,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """GetfilesResponse - a model defined in OpenAPI
+        """HeadlinesRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -224,16 +224,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([Getfiles]): [optional]  # noqa: E501
-            meta (MetaOne): [optional]  # noqa: E501
+            data (HeadlinesRequestData): [optional]  # noqa: E501
+            meta (HeadlinesRequestMeta): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## Comparing `fds/sdk/StreetAccountNews/model/is_partial_one.py` & `fds/sdk/StreetAccountNews/model/delete_view_body.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.StreetAccountNews.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from fds.sdk.StreetAccountNews.model.delete_view_body_data import DeleteViewBodyData
+    globals()['DeleteViewBodyData'] = DeleteViewBodyData
 
-class IsPartialOne(ModelNormal):
+
+class DeleteViewBody(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,50 +67,52 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'is_partial': (bool,),  # noqa: E501
+            'data': (DeleteViewBodyData,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'is_partial': 'isPartial',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """IsPartialOne - a model defined in OpenAPI
+        """DeleteViewBody - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -131,15 +137,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            is_partial (bool): [optional]  # noqa: E501
+            data (DeleteViewBodyData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -180,15 +186,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """IsPartialOne - a model defined in OpenAPI
+        """DeleteViewBody - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -213,15 +219,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            is_partial (bool): [optional]  # noqa: E501
+            data (DeleteViewBodyData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## Comparing `fds/sdk/StreetAccountNews/model/meta_one.py` & `fds/sdk/StreetAccountNews/model/filter_topic_response_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,21 +27,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.StreetAccountNews.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fds.sdk.StreetAccountNews.model.is_partial_one import IsPartialOne
-    from fds.sdk.StreetAccountNews.model.pagination_one import PaginationOne
-    globals()['IsPartialOne'] = IsPartialOne
-    globals()['PaginationOne'] = PaginationOne
+    from fds.sdk.StreetAccountNews.model.flattened_filters_topics import FlattenedFiltersTopics
+    from fds.sdk.StreetAccountNews.model.structured_filters_topics import StructuredFiltersTopics
+    globals()['FlattenedFiltersTopics'] = FlattenedFiltersTopics
+    globals()['StructuredFiltersTopics'] = StructuredFiltersTopics
 
 
-class MetaOne(ModelNormal):
+class FilterTopicResponseData(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -86,37 +86,37 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'pagination': (PaginationOne,),  # noqa: E501
-            'partial': (IsPartialOne,),  # noqa: E501
+            'structured': (StructuredFiltersTopics,),  # noqa: E501
+            'flattened': (FlattenedFiltersTopics,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'pagination': 'pagination',  # noqa: E501
-        'partial': 'partial',  # noqa: E501
+        'structured': 'structured',  # noqa: E501
+        'flattened': 'flattened',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """MetaOne - a model defined in OpenAPI
+        """FilterTopicResponseData - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -141,16 +141,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            pagination (PaginationOne): [optional]  # noqa: E501
-            partial (IsPartialOne): [optional]  # noqa: E501
+            structured (StructuredFiltersTopics): [optional]  # noqa: E501
+            flattened (FlattenedFiltersTopics): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -191,15 +191,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """MetaOne - a model defined in OpenAPI
+        """FilterTopicResponseData - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -224,16 +224,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            pagination (PaginationOne): [optional]  # noqa: E501
-            partial (IsPartialOne): [optional]  # noqa: E501
+            structured (StructuredFiltersTopics): [optional]  # noqa: E501
+            flattened (FlattenedFiltersTopics): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## Comparing `fds/sdk/StreetAccountNews/model/pagination_one.py` & `fds/sdk/StreetAccountNews/model/headlines_request_meta_pagination.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.StreetAccountNews.exceptions import ApiAttributeError
 
 
 
-class PaginationOne(ModelNormal):
+class HeadlinesRequestMetaPagination(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,41 +78,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'total': (int,),  # noqa: E501
-            'is_estimated_total': (bool,),  # noqa: E501
             'limit': (int,),  # noqa: E501
             'offset': (int,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'total': 'total',  # noqa: E501
-        'is_estimated_total': 'isEstimatedTotal',  # noqa: E501
         'limit': 'limit',  # noqa: E501
         'offset': 'offset',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """PaginationOne - a model defined in OpenAPI
+        """HeadlinesRequestMetaPagination - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -137,18 +133,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            total (int): Total number of files the API returns for a particular query. [optional]  # noqa: E501
-            is_estimated_total (bool): Boolean value that represents whether the total count of files returned is exact or an estimate. This is defaulted to “False” as the API should always return the exact count. [optional]  # noqa: E501
-            limit (int): Number of results returned per page. [optional]  # noqa: E501
-            offset (int): The flag indicating the position in the results array if additional results are available beyond the default value or the value in paginationLimit parameter (if used). This value is passed in the _paginationOffset parameter to retreieve subsequent results. [optional]  # noqa: E501
+            limit (int): Non-negative maximum number of entries to return.. [optional] if omitted the server will use the default value of 500  # noqa: E501
+            offset (int): Non-negative number of entries to skip.. [optional] if omitted the server will use the default value of 0  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -189,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """PaginationOne - a model defined in OpenAPI
+        """HeadlinesRequestMetaPagination - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -222,18 +216,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            total (int): Total number of files the API returns for a particular query. [optional]  # noqa: E501
-            is_estimated_total (bool): Boolean value that represents whether the total count of files returned is exact or an estimate. This is defaulted to “False” as the API should always return the exact count. [optional]  # noqa: E501
-            limit (int): Number of results returned per page. [optional]  # noqa: E501
-            offset (int): The flag indicating the position in the results array if additional results are available beyond the default value or the value in paginationLimit parameter (if used). This value is passed in the _paginationOffset parameter to retreieve subsequent results. [optional]  # noqa: E501
+            limit (int): Non-negative maximum number of entries to return.. [optional] if omitted the server will use the default value of 500  # noqa: E501
+            offset (int): Non-negative number of entries to skip.. [optional] if omitted the server will use the default value of 0  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## Comparing `fds/sdk/StreetAccountNews/model/requestfiles_response.py` & `fds/sdk/StreetAccountNews/model/headlines_request_tickers_object.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.StreetAccountNews.exceptions import ApiAttributeError
 
 
 
-class RequestfilesResponse(ModelNormal):
+class HeadlinesRequestTickersObject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -52,14 +52,23 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('type',): {
+            'INDEX': "Index",
+            'ETF': "ETF",
+            'MUTUAL_FUND': "Mutual_Fund",
+            'PORTFOLIOS': "Portfolios",
+            'EQUITY': "Equity",
+            'PRIVATECOMPANIES': "privateCompanies",
+            'FIXED_INCOME': "Fixed_Income",
+        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -78,37 +87,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'job_id': (str,),  # noqa: E501
-            'status': (str,),  # noqa: E501
+            'value': (str,),  # noqa: E501
+            'type': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'job_id': 'jobID',  # noqa: E501
-        'status': 'status',  # noqa: E501
+        'value': 'value',  # noqa: E501
+        'type': 'type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """RequestfilesResponse - a model defined in OpenAPI
+        """HeadlinesRequestTickersObject - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -133,16 +142,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            job_id (str): Unique id to get the xml files for the requested date. [optional]  # noqa: E501
-            status (str): Returns the value as submitted. Tells the request has been submitted. [optional]  # noqa: E501
+            value (str): The ticker symbol. It also supports an listing and regional suffix (ex:AAPL-US). [optional]  # noqa: E501
+            type (str): The type of asset associated with the ticker. . [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +192,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """RequestfilesResponse - a model defined in OpenAPI
+        """HeadlinesRequestTickersObject - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,16 +225,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            job_id (str): Unique id to get the xml files for the requested date. [optional]  # noqa: E501
-            status (str): Returns the value as submitted. Tells the request has been submitted. [optional]  # noqa: E501
+            value (str): The ticker symbol. It also supports an listing and regional suffix (ex:AAPL-US). [optional]  # noqa: E501
+            type (str): The type of asset associated with the ticker. . [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## Comparing `fds/sdk/StreetAccountNews/model/sa_headlines_request.py` & `fds/sdk/StreetAccountNews/model/headlines_request_by_view.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,21 +27,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.StreetAccountNews.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fds.sdk.StreetAccountNews.model.sa_headlines_request_data import SaHeadlinesRequestData
-    from fds.sdk.StreetAccountNews.model.sa_headlines_request_meta import SaHeadlinesRequestMeta
-    globals()['SaHeadlinesRequestData'] = SaHeadlinesRequestData
-    globals()['SaHeadlinesRequestMeta'] = SaHeadlinesRequestMeta
+    from fds.sdk.StreetAccountNews.model.headlines_request_by_view_data import HeadlinesRequestByViewData
+    from fds.sdk.StreetAccountNews.model.headlines_request_by_view_meta import HeadlinesRequestByViewMeta
+    globals()['HeadlinesRequestByViewData'] = HeadlinesRequestByViewData
+    globals()['HeadlinesRequestByViewMeta'] = HeadlinesRequestByViewMeta
 
 
-class SaHeadlinesRequest(ModelNormal):
+class HeadlinesRequestByView(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -86,16 +86,16 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (SaHeadlinesRequestData,),  # noqa: E501
-            'meta': (SaHeadlinesRequestMeta,),  # noqa: E501
+            'data': (HeadlinesRequestByViewData,),  # noqa: E501
+            'meta': (HeadlinesRequestByViewMeta,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -108,15 +108,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SaHeadlinesRequest - a model defined in OpenAPI
+        """HeadlinesRequestByView - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -141,16 +141,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (SaHeadlinesRequestData): [optional]  # noqa: E501
-            meta (SaHeadlinesRequestMeta): [optional]  # noqa: E501
+            data (HeadlinesRequestByViewData): [optional]  # noqa: E501
+            meta (HeadlinesRequestByViewMeta): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -191,15 +191,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """SaHeadlinesRequest - a model defined in OpenAPI
+        """HeadlinesRequestByView - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -224,16 +224,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (SaHeadlinesRequestData): [optional]  # noqa: E501
-            meta (SaHeadlinesRequestMeta): [optional]  # noqa: E501
+            data (HeadlinesRequestByViewData): [optional]  # noqa: E501
+            meta (HeadlinesRequestByViewMeta): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## Comparing `fds/sdk/StreetAccountNews/model/sa_headlines_request_by_view.py` & `fds/sdk/StreetAccountNews/model/filter_categories_response_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,21 +27,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.StreetAccountNews.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fds.sdk.StreetAccountNews.model.sa_headlines_request_by_view_data import SaHeadlinesRequestByViewData
-    from fds.sdk.StreetAccountNews.model.sa_headlines_request_meta import SaHeadlinesRequestMeta
-    globals()['SaHeadlinesRequestByViewData'] = SaHeadlinesRequestByViewData
-    globals()['SaHeadlinesRequestMeta'] = SaHeadlinesRequestMeta
+    from fds.sdk.StreetAccountNews.model.flattened_filters_categories import FlattenedFiltersCategories
+    from fds.sdk.StreetAccountNews.model.structured_filters_categories import StructuredFiltersCategories
+    globals()['FlattenedFiltersCategories'] = FlattenedFiltersCategories
+    globals()['StructuredFiltersCategories'] = StructuredFiltersCategories
 
 
-class SaHeadlinesRequestByView(ModelNormal):
+class FilterCategoriesResponseData(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -86,37 +86,37 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (SaHeadlinesRequestByViewData,),  # noqa: E501
-            'meta': (SaHeadlinesRequestMeta,),  # noqa: E501
+            'structured': (StructuredFiltersCategories,),  # noqa: E501
+            'flattened': (FlattenedFiltersCategories,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
-        'meta': 'meta',  # noqa: E501
+        'structured': 'structured',  # noqa: E501
+        'flattened': 'flattened',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SaHeadlinesRequestByView - a model defined in OpenAPI
+        """FilterCategoriesResponseData - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -141,16 +141,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (SaHeadlinesRequestByViewData): [optional]  # noqa: E501
-            meta (SaHeadlinesRequestMeta): [optional]  # noqa: E501
+            structured (StructuredFiltersCategories): [optional]  # noqa: E501
+            flattened (FlattenedFiltersCategories): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -191,15 +191,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """SaHeadlinesRequestByView - a model defined in OpenAPI
+        """FilterCategoriesResponseData - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -224,16 +224,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (SaHeadlinesRequestByViewData): [optional]  # noqa: E501
-            meta (SaHeadlinesRequestMeta): [optional]  # noqa: E501
+            structured (StructuredFiltersCategories): [optional]  # noqa: E501
+            flattened (FlattenedFiltersCategories): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## Comparing `fds/sdk/StreetAccountNews/model/sa_headlines_request_by_view_data.py` & `fds/sdk/StreetAccountNews/model/headlines_request_meta.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.StreetAccountNews.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fds.sdk.StreetAccountNews.model.sa_headlines_request_data_search_date import SaHeadlinesRequestDataSearchDate
-    globals()['SaHeadlinesRequestDataSearchDate'] = SaHeadlinesRequestDataSearchDate
+    from fds.sdk.StreetAccountNews.model.headlines_request_meta_pagination import HeadlinesRequestMetaPagination
+    globals()['HeadlinesRequestMetaPagination'] = HeadlinesRequestMetaPagination
 
 
-class SaHeadlinesRequestByViewData(ModelNormal):
+class HeadlinesRequestMeta(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -56,14 +56,25 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('attributes',): {
+            'HEADLINES': "headlines",
+            'STORYTIME': "storyTime",
+            'ID': "id",
+            'PRIMARYSYMBOLS': "primarySymbols",
+            'SYMBOLS': "symbols",
+            'SUBJECTS': "subjects",
+            'STORYBODY': "storyBody",
+            'REFERENCEURIS': "referenceUris",
+            'URL': "url",
+        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -84,35 +95,37 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'search_date': (SaHeadlinesRequestDataSearchDate,),  # noqa: E501
+            'pagination': (HeadlinesRequestMetaPagination,),  # noqa: E501
+            'attributes': ([str],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'search_date': 'searchDate',  # noqa: E501
+        'pagination': 'pagination',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SaHeadlinesRequestByViewData - a model defined in OpenAPI
+        """HeadlinesRequestMeta - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -137,15 +150,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            search_date (SaHeadlinesRequestDataSearchDate): [optional]  # noqa: E501
+            pagination (HeadlinesRequestMetaPagination): [optional]  # noqa: E501
+            attributes ([str]): A specific set of attributes to return in the response. If empty or not specified, the response does not omit attributes.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -186,15 +200,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """SaHeadlinesRequestByViewData - a model defined in OpenAPI
+        """HeadlinesRequestMeta - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -219,15 +233,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            search_date (SaHeadlinesRequestDataSearchDate): [optional]  # noqa: E501
+            pagination (HeadlinesRequestMetaPagination): [optional]  # noqa: E501
+            attributes ([str]): A specific set of attributes to return in the response. If empty or not specified, the response does not omit attributes.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## Comparing `fds/sdk/StreetAccountNews/model/sa_headlines_request_data.py` & `fds/sdk/StreetAccountNews/model/filter_sectors_response_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,21 +27,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.StreetAccountNews.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fds.sdk.StreetAccountNews.model.sa_headlines_request_data_search_date import SaHeadlinesRequestDataSearchDate
-    from fds.sdk.StreetAccountNews.model.sa_headlines_request_tickers_object import SaHeadlinesRequestTickersObject
-    globals()['SaHeadlinesRequestDataSearchDate'] = SaHeadlinesRequestDataSearchDate
-    globals()['SaHeadlinesRequestTickersObject'] = SaHeadlinesRequestTickersObject
+    from fds.sdk.StreetAccountNews.model.flattened_filters_sectors import FlattenedFiltersSectors
+    from fds.sdk.StreetAccountNews.model.structured_filters_sectors import StructuredFiltersSectors
+    globals()['FlattenedFiltersSectors'] = FlattenedFiltersSectors
+    globals()['StructuredFiltersSectors'] = StructuredFiltersSectors
 
 
-class SaHeadlinesRequestData(ModelNormal):
+class FilterSectorsResponseData(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -86,47 +86,37 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'tickers': ([SaHeadlinesRequestTickersObject],),  # noqa: E501
-            'categories': ([str],),  # noqa: E501
-            'regions': ([str],),  # noqa: E501
-            'topics': ([str],),  # noqa: E501
-            'sectors': ([str],),  # noqa: E501
-            'is_primary': (bool,),  # noqa: E501
-            'search_date': (SaHeadlinesRequestDataSearchDate,),  # noqa: E501
+            'structured': (StructuredFiltersSectors,),  # noqa: E501
+            'flattened': (FlattenedFiltersSectors,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'tickers': 'tickers',  # noqa: E501
-        'categories': 'categories',  # noqa: E501
-        'regions': 'regions',  # noqa: E501
-        'topics': 'topics',  # noqa: E501
-        'sectors': 'sectors',  # noqa: E501
-        'is_primary': 'isPrimary',  # noqa: E501
-        'search_date': 'searchDate',  # noqa: E501
+        'structured': 'structured',  # noqa: E501
+        'flattened': 'flattened',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SaHeadlinesRequestData - a model defined in OpenAPI
+        """FilterSectorsResponseData - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -151,21 +141,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            tickers ([SaHeadlinesRequestTickersObject]): [optional]  # noqa: E501
-            categories ([str]): [optional]  # noqa: E501
-            regions ([str]): [optional]  # noqa: E501
-            topics ([str]): [optional]  # noqa: E501
-            sectors ([str]): [optional]  # noqa: E501
-            is_primary (bool): [optional]  # noqa: E501
-            search_date (SaHeadlinesRequestDataSearchDate): [optional]  # noqa: E501
+            structured (StructuredFiltersSectors): [optional]  # noqa: E501
+            flattened (FlattenedFiltersSectors): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -206,15 +191,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """SaHeadlinesRequestData - a model defined in OpenAPI
+        """FilterSectorsResponseData - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -239,21 +224,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            tickers ([SaHeadlinesRequestTickersObject]): [optional]  # noqa: E501
-            categories ([str]): [optional]  # noqa: E501
-            regions ([str]): [optional]  # noqa: E501
-            topics ([str]): [optional]  # noqa: E501
-            sectors ([str]): [optional]  # noqa: E501
-            is_primary (bool): [optional]  # noqa: E501
-            search_date (SaHeadlinesRequestDataSearchDate): [optional]  # noqa: E501
+            structured (StructuredFiltersSectors): [optional]  # noqa: E501
+            flattened (FlattenedFiltersSectors): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## Comparing `fds/sdk/StreetAccountNews/model/sa_headlines_request_data_search_date.py` & `fds/sdk/StreetAccountNews/model/headlines_request_data_search_time.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.StreetAccountNews.exceptions import ApiAttributeError
 
 
 
-class SaHeadlinesRequestDataSearchDate(ModelNormal):
+class HeadlinesRequestDataSearchTime(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,16 +78,16 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'start': (str,),  # noqa: E501
-            'end': (str,),  # noqa: E501
+            'start': (datetime,),  # noqa: E501
+            'end': (datetime,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -100,15 +100,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SaHeadlinesRequestDataSearchDate - a model defined in OpenAPI
+        """HeadlinesRequestDataSearchTime - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -133,16 +133,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            start (str): Start time for custom search. startTime must follow the ISO 8601 standard format, YYYY-MM-DDTHH:mm:ssZ (UTC). It also supports offsets ±[hh]:[mm]. [optional]  # noqa: E501
-            end (str): End time for custom search. If end time is not present end time is automatically set to the time of the search. endTime must follow the ISO 8601 standard format, YYYY-MM-DDTHH:mm:ssZ (UTC). It also supports offsets ±[hh]:[mm]. [optional]  # noqa: E501
+            start (datetime): Start time for custom search. startTime must follow the ISO 8601 standard format, YYYY-MM-DDTHH:mm:ssZ (UTC). It also supports offsets ±[hh]:[mm]. [optional]  # noqa: E501
+            end (datetime): End time for custom search. If end time is not present end time is automatically set to the time of the search. endTime must follow the ISO 8601 standard format, YYYY-MM-DDTHH:mm:ssZ (UTC). It also supports offsets ±[hh]:[mm]. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """SaHeadlinesRequestDataSearchDate - a model defined in OpenAPI
+        """HeadlinesRequestDataSearchTime - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,16 +216,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            start (str): Start time for custom search. startTime must follow the ISO 8601 standard format, YYYY-MM-DDTHH:mm:ssZ (UTC). It also supports offsets ±[hh]:[mm]. [optional]  # noqa: E501
-            end (str): End time for custom search. If end time is not present end time is automatically set to the time of the search. endTime must follow the ISO 8601 standard format, YYYY-MM-DDTHH:mm:ssZ (UTC). It also supports offsets ±[hh]:[mm]. [optional]  # noqa: E501
+            start (datetime): Start time for custom search. startTime must follow the ISO 8601 standard format, YYYY-MM-DDTHH:mm:ssZ (UTC). It also supports offsets ±[hh]:[mm]. [optional]  # noqa: E501
+            end (datetime): End time for custom search. If end time is not present end time is automatically set to the time of the search. endTime must follow the ISO 8601 standard format, YYYY-MM-DDTHH:mm:ssZ (UTC). It also supports offsets ±[hh]:[mm]. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## Comparing `fds/sdk/StreetAccountNews/model/sa_headlines_request_meta.py` & `fds/sdk/StreetAccountNews/model/flattened_filters_categories.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.StreetAccountNews.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fds.sdk.StreetAccountNews.model.sa_headlines_request_meta_pagination import SaHeadlinesRequestMetaPagination
-    globals()['SaHeadlinesRequestMetaPagination'] = SaHeadlinesRequestMetaPagination
+    from fds.sdk.StreetAccountNews.model.flattened_filters_categories_object import FlattenedFiltersCategoriesObject
+    globals()['FlattenedFiltersCategoriesObject'] = FlattenedFiltersCategoriesObject
 
 
-class SaHeadlinesRequestMeta(ModelNormal):
+class FlattenedFiltersCategories(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,35 +84,35 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'pagination': (SaHeadlinesRequestMetaPagination,),  # noqa: E501
+            'categories': ([FlattenedFiltersCategoriesObject],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'pagination': 'pagination',  # noqa: E501
+        'categories': 'categories',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SaHeadlinesRequestMeta - a model defined in OpenAPI
+        """FlattenedFiltersCategories - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -137,15 +137,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            pagination (SaHeadlinesRequestMetaPagination): [optional]  # noqa: E501
+            categories ([FlattenedFiltersCategoriesObject]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -186,15 +186,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """SaHeadlinesRequestMeta - a model defined in OpenAPI
+        """FlattenedFiltersCategories - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -219,15 +219,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            pagination (SaHeadlinesRequestMetaPagination): [optional]  # noqa: E501
+            categories ([FlattenedFiltersCategoriesObject]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## Comparing `fds/sdk/StreetAccountNews/model/sa_headlines_request_meta_pagination.py` & `fds/sdk/StreetAccountNews/model/filter_regions_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.StreetAccountNews.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from fds.sdk.StreetAccountNews.model.filter_regions_response_data import FilterRegionsResponseData
+    globals()['FilterRegionsResponseData'] = FilterRegionsResponseData
 
-class SaHeadlinesRequestMetaPagination(ModelNormal):
+
+class FilterRegionsResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,52 +67,52 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'limit': (int,),  # noqa: E501
-            'offset': (int,),  # noqa: E501
+            'data': (FilterRegionsResponseData,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'limit': 'limit',  # noqa: E501
-        'offset': 'offset',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SaHeadlinesRequestMetaPagination - a model defined in OpenAPI
+        """FilterRegionsResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -133,16 +137,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            limit (int): Non-negative maximum number of entries to return.. [optional] if omitted the server will use the default value of 500  # noqa: E501
-            offset (int): Non-negative number of entries to skip.. [optional] if omitted the server will use the default value of 0  # noqa: E501
+            data (FilterRegionsResponseData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +186,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """SaHeadlinesRequestMetaPagination - a model defined in OpenAPI
+        """FilterRegionsResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,16 +219,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            limit (int): Non-negative maximum number of entries to return.. [optional] if omitted the server will use the default value of 500  # noqa: E501
-            offset (int): Non-negative number of entries to skip.. [optional] if omitted the server will use the default value of 0  # noqa: E501
+            data (FilterRegionsResponseData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## Comparing `fds/sdk/StreetAccountNews/model/sa_headlines_request_tickers_object.py` & `fds/sdk/StreetAccountNews/model/structured_filters_children_object_regions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.StreetAccountNews.exceptions import ApiAttributeError
 
 
 
-class SaHeadlinesRequestTickersObject(ModelNormal):
+class StructuredFiltersChildrenObjectRegions(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -52,23 +52,14 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('type',): {
-            'INDEX': "Index",
-            'ETF': "ETF",
-            'MUTUAL_FUND': "Mutual_Fund",
-            'PORTFOLIOS': "Portfolios",
-            'EQUITY': "Equity",
-            'PRIVATECOMPANIES': "privateCompanies",
-            'FIXED_INCOME': "Fixed_Income",
-        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -88,38 +79,36 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'name': (str,),  # noqa: E501
-            'value': (str,),  # noqa: E501
-            'type': (str,),  # noqa: E501
+            'value': ([str],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'value': 'value',  # noqa: E501
-        'type': 'type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SaHeadlinesRequestTickersObject - a model defined in OpenAPI
+        """StructuredFiltersChildrenObjectRegions - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -144,17 +133,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
-            value (str): [optional]  # noqa: E501
-            type (str): [optional]  # noqa: E501
+            name (str): The name of the children.. [optional]  # noqa: E501
+            value ([str]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -195,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """SaHeadlinesRequestTickersObject - a model defined in OpenAPI
+        """StructuredFiltersChildrenObjectRegions - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -228,17 +216,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
-            value (str): [optional]  # noqa: E501
-            type (str): [optional]  # noqa: E501
+            name (str): The name of the children.. [optional]  # noqa: E501
+            value ([str]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## Comparing `fds/sdk/StreetAccountNews/model/search_response.py` & `fds/sdk/StreetAccountNews/model/filter_regions_response_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,21 +27,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.StreetAccountNews.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fds.sdk.StreetAccountNews.model.search_response_data import SearchResponseData
-    from fds.sdk.StreetAccountNews.model.search_response_meta import SearchResponseMeta
-    globals()['SearchResponseData'] = SearchResponseData
-    globals()['SearchResponseMeta'] = SearchResponseMeta
+    from fds.sdk.StreetAccountNews.model.flattened_filters_regions import FlattenedFiltersRegions
+    from fds.sdk.StreetAccountNews.model.structured_filters_regions import StructuredFiltersRegions
+    globals()['FlattenedFiltersRegions'] = FlattenedFiltersRegions
+    globals()['StructuredFiltersRegions'] = StructuredFiltersRegions
 
 
-class SearchResponse(ModelNormal):
+class FilterRegionsResponseData(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -86,37 +86,37 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (SearchResponseData,),  # noqa: E501
-            'meta': (SearchResponseMeta,),  # noqa: E501
+            'structured': (StructuredFiltersRegions,),  # noqa: E501
+            'flattened': (FlattenedFiltersRegions,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
-        'meta': 'meta',  # noqa: E501
+        'structured': 'structured',  # noqa: E501
+        'flattened': 'flattened',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SearchResponse - a model defined in OpenAPI
+        """FilterRegionsResponseData - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -141,16 +141,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (SearchResponseData): [optional]  # noqa: E501
-            meta (SearchResponseMeta): [optional]  # noqa: E501
+            structured (StructuredFiltersRegions): [optional]  # noqa: E501
+            flattened (FlattenedFiltersRegions): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -191,15 +191,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """SearchResponse - a model defined in OpenAPI
+        """FilterRegionsResponseData - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -224,16 +224,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (SearchResponseData): [optional]  # noqa: E501
-            meta (SearchResponseMeta): [optional]  # noqa: E501
+            structured (StructuredFiltersRegions): [optional]  # noqa: E501
+            flattened (FlattenedFiltersRegions): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## Comparing `fds/sdk/StreetAccountNews/model/search_response_data.py` & `fds/sdk/StreetAccountNews/model/structured_filters_regions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.StreetAccountNews.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fds.sdk.StreetAccountNews.model.search_response_array_object import SearchResponseArrayObject
-    globals()['SearchResponseArrayObject'] = SearchResponseArrayObject
+    from fds.sdk.StreetAccountNews.model.structured_filters_regions_object import StructuredFiltersRegionsObject
+    globals()['StructuredFiltersRegionsObject'] = StructuredFiltersRegionsObject
 
 
-class SearchResponseData(ModelNormal):
+class StructuredFiltersRegions(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,35 +84,35 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'results': ([SearchResponseArrayObject],),  # noqa: E501
+            'regions': ([StructuredFiltersRegionsObject],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'results': 'results',  # noqa: E501
+        'regions': 'regions',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SearchResponseData - a model defined in OpenAPI
+        """StructuredFiltersRegions - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -137,15 +137,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            results ([SearchResponseArrayObject]): [optional]  # noqa: E501
+            regions ([StructuredFiltersRegionsObject]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -186,15 +186,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """SearchResponseData - a model defined in OpenAPI
+        """StructuredFiltersRegions - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -219,15 +219,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            results ([SearchResponseArrayObject]): [optional]  # noqa: E501
+            regions ([StructuredFiltersRegionsObject]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## Comparing `fds/sdk/StreetAccountNews/model/search_response_meta.py` & `fds/sdk/StreetAccountNews/model/quick_alerts_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.StreetAccountNews.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fds.sdk.StreetAccountNews.model.search_response_meta_pagination import SearchResponseMetaPagination
-    globals()['SearchResponseMetaPagination'] = SearchResponseMetaPagination
+    from fds.sdk.StreetAccountNews.model.quick_alerts_body_data import QuickAlertsBodyData
+    globals()['QuickAlertsBodyData'] = QuickAlertsBodyData
 
 
-class SearchResponseMeta(ModelNormal):
+class QuickAlertsResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,37 +84,35 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'request_guid': (str,),  # noqa: E501
-            'pagination': (SearchResponseMetaPagination,),  # noqa: E501
+            'data': (QuickAlertsBodyData,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'request_guid': 'requestGuid',  # noqa: E501
-        'pagination': 'pagination',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SearchResponseMeta - a model defined in OpenAPI
+        """QuickAlertsResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -139,16 +137,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            request_guid (str): [optional]  # noqa: E501
-            pagination (SearchResponseMetaPagination): [optional]  # noqa: E501
+            data (QuickAlertsBodyData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -189,15 +186,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """SearchResponseMeta - a model defined in OpenAPI
+        """QuickAlertsResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -222,16 +219,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            request_guid (str): [optional]  # noqa: E501
-            pagination (SearchResponseMetaPagination): [optional]  # noqa: E501
+            data (QuickAlertsBodyData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## Comparing `fds/sdk/StreetAccountNews/model/search_response_meta_pagination.py` & `fds/sdk/StreetAccountNews/model/structured_filters_categories.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.StreetAccountNews.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from fds.sdk.StreetAccountNews.model.structured_filters_categories_object import StructuredFiltersCategoriesObject
+    globals()['StructuredFiltersCategoriesObject'] = StructuredFiltersCategoriesObject
 
-class SearchResponseMetaPagination(ModelNormal):
+
+class StructuredFiltersCategories(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,52 +67,52 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'total': (int,),  # noqa: E501
-            'is_estimated_total': (bool,),  # noqa: E501
+            'categories': ([StructuredFiltersCategoriesObject],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'total': 'total',  # noqa: E501
-        'is_estimated_total': 'isEstimatedTotal',  # noqa: E501
+        'categories': 'categories',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SearchResponseMetaPagination - a model defined in OpenAPI
+        """StructuredFiltersCategories - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -133,16 +137,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            total (int): [optional]  # noqa: E501
-            is_estimated_total (bool): [optional]  # noqa: E501
+            categories ([StructuredFiltersCategoriesObject]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +186,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """SearchResponseMetaPagination - a model defined in OpenAPI
+        """StructuredFiltersCategories - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,16 +219,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            total (int): [optional]  # noqa: E501
-            is_estimated_total (bool): [optional]  # noqa: E501
+            categories ([StructuredFiltersCategoriesObject]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## Comparing `fds/sdk/StreetAccountNews/model/street_account_status.py` & `fds/sdk/StreetAccountNews/model/create_view_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.StreetAccountNews.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from fds.sdk.StreetAccountNews.model.create_view_response_data import CreateViewResponseData
+    globals()['CreateViewResponseData'] = CreateViewResponseData
 
-class StreetAccountStatus(ModelNormal):
+
+class CreateViewResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,52 +67,52 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'id': (str,),  # noqa: E501
-            'error_message': (str,),  # noqa: E501
+            'data': (CreateViewResponseData,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
-        'error_message': 'error_message',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """StreetAccountStatus - a model defined in OpenAPI
+        """CreateViewResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -133,16 +137,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
-            error_message (str): Textual error message. [optional]  # noqa: E501
+            data (CreateViewResponseData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +186,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """StreetAccountStatus - a model defined in OpenAPI
+        """CreateViewResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,16 +219,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
-            error_message (str): Textual error message. [optional]  # noqa: E501
+            data (CreateViewResponseData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

## Comparing `fds/sdk/StreetAccountNews/model/structured_filters_children_object.py` & `fds/sdk/StreetAccountNews/model/structured_filters_children_object_categories.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     StreetAccount News API
 
-    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  **StreetAccount Historical Stories:**  These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.  Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.  The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.  # noqa: E501
+    The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.  **StreetAccount Filters, Headlines, and Views:**  These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 1.0.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fds.sdk.StreetAccountNews.exceptions import ApiAttributeError
 
 
 
-class StructuredFiltersChildrenObject(ModelNormal):
+class StructuredFiltersChildrenObjectCategories(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -100,15 +100,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """StructuredFiltersChildrenObject - a model defined in OpenAPI
+        """StructuredFiltersChildrenObjectCategories - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -133,15 +133,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
+            name (str): The name of the children.. [optional]  # noqa: E501
             value ([str]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -183,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """StructuredFiltersChildrenObject - a model defined in OpenAPI
+        """StructuredFiltersChildrenObjectCategories - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,15 +216,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
+            name (str): The name of the children.. [optional]  # noqa: E501
             value ([str]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

## Comparing `fds.sdk.StreetAccountNews-0.20.4.dist-info/LICENSE` & `fds.sdk.StreetAccountNews-0.40.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fds.sdk.StreetAccountNews-0.20.4.dist-info/METADATA` & `fds.sdk.StreetAccountNews-0.40.0.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: fds.sdk.StreetAccountNews
-Version: 0.20.4
+Version: 0.40.0
 Summary: StreetAccount News client library for Python
-Home-page: https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0
+Home-page: https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1
 Author: FactSet Research Systems
 License: Apache License, Version 2.0
 Keywords: FactSet,API,SDK
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -21,48 +21,40 @@
 [![PyPi](https://img.shields.io/pypi/v/fds.sdk.StreetAccountNews)](https://pypi.org/project/fds.sdk.StreetAccountNews/)
 [![Apache-2 license](https://img.shields.io/badge/license-Apache2-brightgreen.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 
 The StreetAccount News API provides access to FactSet's proprietary news provider, StreetAccount. StreetAccount, is a premium real-time market intelligence news service that delivers comprehensive U.S., Canadian, and European coverage (and expanding Asia coverage). All possible sources for corporate news are scanned and key story facts are highlighted and presented in an easy-to-read format.
 
 **StreetAccount Filters, Headlines, and Views:**
 
-These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Company Filters, Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.
-
-**StreetAccount Historical Stories:**
-
-These endpoints provide access to historical StreetAccount (SA) news. The API delivers SA stories in XML format based on user-specified date input parameters. Output files are securely available to users through a URL. This API has three endpoints: Request Files, Check Status, and Get Files.
-
-Please note that this API only supports adhoc requests for historical files and does not support real-time files. If real-time push is required, consider using other methods such as SFTP, QNT account, or Azure Storage. Both historical and real-time Street Account news can be delivered via SFTP, QNT account, or Azure Storage.
-
-The files delivered contain both metadata and content body, eliminating the need for multiple requests through multiple services to retrieve all the information.
+These endpoints allow for the retrieval of news headlines using filters such as Watchlists/Indices/Tickers, Categories (the equivalent of 'Subjects' within the Workstation), Market Topics, Regions, and Sectors.  Headlines can also be retrieved based on saved views within the Workstation.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.0
-- Package version: 0.20.4
+- API version: 1.0.0
+- Package version: 0.40.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 For more information, please visit [https://developer.factset.com/contact](https://developer.factset.com/contact)
 
 ## Requirements
 
 * Python >= 3.7
 
 ## Installation
 
 ### Poetry
 
 ```shell
-poetry add fds.sdk.utils fds.sdk.StreetAccountNews==0.20.4
+poetry add fds.sdk.utils fds.sdk.StreetAccountNews==0.40.0
 ```
 
 ### pip
 
 ```shell
-pip install fds.sdk.utils fds.sdk.StreetAccountNews==0.20.4
+pip install fds.sdk.utils fds.sdk.StreetAccountNews==0.40.0
 ```
 
 ## Usage
 
 1. [Generate authentication credentials](../../../../README.md#authentication).
 2. Setup Python environment.
    1. Install and activate python 3.7+. If you're using [pyenv](https://github.com/pyenv/pyenv):
@@ -114,54 +106,55 @@
 #     password='API-KEY'
 # )
 
 # Enter a context with an instance of the API client
 with fds.sdk.StreetAccountNews.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = filters_api.FiltersApi(api_client)
-    structured = True # bool | Pass structured to generate a structured view of the available filters. (optional)
-    flattened = True # bool | Pass flattened to generate a structured view of the available filters. (optional)
+    attributes = [
+        "structured",
+    ] # [str] | Pass a list of filters to return the respective type of filter. Accepted list values are \"structured\" and/or \"flattened\". If no _atrributes are specified, all filters will be returned in the response (this is the default response).  (optional)
 
     try:
         # Retrieve all StreetAccount filters
         # example passing only required values which don't have defaults set
         # and optional values
-        api_response = api_instance.get_street_account_filters(structured=structured, flattened=flattened)
+        api_response = api_instance.get_street_account_filters(attributes=attributes)
 
         pprint(api_response)
     except fds.sdk.StreetAccountNews.ApiException as e:
         print("Exception when calling FiltersApi->get_street_account_filters: %s\n" % e)
 
     # # Get response, http status code and response headers
     # try:
     #     # Retrieve all StreetAccount filters
-    #     api_response, http_status_code, response_headers = api_instance.get_street_account_filters_with_http_info(structured=structured, flattened=flattened)
+    #     api_response, http_status_code, response_headers = api_instance.get_street_account_filters_with_http_info(attributes=attributes)
 
 
     #     pprint(api_response)
     #     pprint(http_status_code)
     #     pprint(response_headers)
     # except fds.sdk.StreetAccountNews.ApiException as e:
     #     print("Exception when calling FiltersApi->get_street_account_filters: %s\n" % e)
 
     # # Get response asynchronous
     # try:
     #     # Retrieve all StreetAccount filters
-    #     async_result = api_instance.get_street_account_filters_async(structured=structured, flattened=flattened)
+    #     async_result = api_instance.get_street_account_filters_async(attributes=attributes)
     #     api_response = async_result.get()
 
 
     #     pprint(api_response)
     # except fds.sdk.StreetAccountNews.ApiException as e:
     #     print("Exception when calling FiltersApi->get_street_account_filters: %s\n" % e)
 
     # # Get response, http status code and response headers asynchronous
     # try:
     #     # Retrieve all StreetAccount filters
-    #     async_result = api_instance.get_street_account_filters_with_http_info_async(structured=structured, flattened=flattened)
+    #     async_result = api_instance.get_street_account_filters_with_http_info_async(attributes=attributes)
     #     api_response, http_status_code, response_headers = async_result.get()
 
 
     #     pprint(api_response)
     #     pprint(http_status_code)
     #     pprint(response_headers)
     # except fds.sdk.StreetAccountNews.ApiException as e:
@@ -236,79 +229,101 @@
     ssl_ca_cert='/path/to/ca.pem'
 )
 ```
 
 
 ## Documentation for API Endpoints
 
-All URIs are relative to *https://api.factset.com/research/news/v0*
+All URIs are relative to *https://api.factset.com/streetaccount/v1*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
-*FiltersApi* | [**get_street_account_filters**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/FiltersApi.md#get_street_account_filters) | **GET** /streetaccount/filters | Retrieve all StreetAccount filters
-*HeadlinesApi* | [**get_street_account_headlines**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/HeadlinesApi.md#get_street_account_headlines) | **POST** /streetaccount/headlines | Retrieve StreetAccount headlines for given filters
-*HeadlinesApi* | [**get_street_account_headlines_by_view**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/HeadlinesApi.md#get_street_account_headlines_by_view) | **POST** /streetaccount/views/{id}/headlines | Retrieve StreetAccount headlines for given view
-*StreetAccountHistoricalStoriesApi* | [**streetaccount_historical_check_status_get**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/StreetAccountHistoricalStoriesApi.md#streetaccount_historical_check_status_get) | **GET** /streetaccount/historical/check-status | Returns the status and percentage of completion for the requested jobID
-*StreetAccountHistoricalStoriesApi* | [**streetaccount_historical_get_files_get**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/StreetAccountHistoricalStoriesApi.md#streetaccount_historical_get_files_get) | **GET** /streetaccount/historical/get-files | Returns the StreetAccount XML files for the specified date range
-*StreetAccountHistoricalStoriesApi* | [**streetaccount_historical_request_files_get**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/StreetAccountHistoricalStoriesApi.md#streetaccount_historical_request_files_get) | **GET** /streetaccount/historical/request-files | Returns the jobID
-*ViewsApi* | [**create_street_account_view**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/ViewsApi.md#create_street_account_view) | **POST** /streetaccount/views/{id} | Creates and saves a StreetAccount view
-*ViewsApi* | [**delete_street_account_view**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/ViewsApi.md#delete_street_account_view) | **DELETE** /streetaccount/views/{id} | Deletes an existing StreetAccount view
-*ViewsApi* | [**edit_street_account_view**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/ViewsApi.md#edit_street_account_view) | **PUT** /streetaccount/views/{id} | Edits and saves an existing StreetAccount view
-*ViewsApi* | [**get_street_account_views**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/ViewsApi.md#get_street_account_views) | **GET** /streetaccount/views | Retrieves StreetAccount search views
+*FiltersApi* | [**get_street_account_filters**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/FiltersApi.md#get_street_account_filters) | **GET** /filters | Retrieve all StreetAccount filters
+*FiltersApi* | [**get_street_account_filters_categories**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/FiltersApi.md#get_street_account_filters_categories) | **GET** /filters/categories | Retrieve all StreetAccount filter categories
+*FiltersApi* | [**get_street_account_filters_regions**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/FiltersApi.md#get_street_account_filters_regions) | **GET** /filters/regions | Retrieve all StreetAccount filter regions
+*FiltersApi* | [**get_street_account_filters_sectors**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/FiltersApi.md#get_street_account_filters_sectors) | **GET** /filters/sectors | Retrieve all StreetAccount filter sectors
+*FiltersApi* | [**get_street_account_filters_topics**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/FiltersApi.md#get_street_account_filters_topics) | **GET** /filters/topics | Retrieve all StreetAccount filter topics
+*FiltersApi* | [**get_street_account_filters_watchlists**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/FiltersApi.md#get_street_account_filters_watchlists) | **GET** /filters/watchlists | Retrieve all StreetAccount filter watchlists
+*HeadlinesApi* | [**get_street_account_headlines**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/HeadlinesApi.md#get_street_account_headlines) | **POST** /headlines | Retrieve StreetAccount headlines for given filters
+*HeadlinesApi* | [**get_street_account_headlines_by_view**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/HeadlinesApi.md#get_street_account_headlines_by_view) | **POST** /headlines/view | Retrieve StreetAccount headlines for given view
+*ViewsApi* | [**create_quick_alert_for_view**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/ViewsApi.md#create_quick_alert_for_view) | **POST** /quick-alert/create | Creates a quick-alert for given saved view
+*ViewsApi* | [**create_street_account_view**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/ViewsApi.md#create_street_account_view) | **POST** /views/create | Creates and saves a StreetAccount view
+*ViewsApi* | [**delete_quickalert_view**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/ViewsApi.md#delete_quickalert_view) | **POST** /quick-alert/delete | Deletes an existing quick alert for a view.
+*ViewsApi* | [**delete_street_account_view**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/ViewsApi.md#delete_street_account_view) | **POST** /views/delete | Deletes an existing StreetAccount view
+*ViewsApi* | [**edit_street_account_view**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/ViewsApi.md#edit_street_account_view) | **POST** /views/update | Edits and saves an existing StreetAccount view
+*ViewsApi* | [**get_street_account_views**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/ViewsApi.md#get_street_account_views) | **GET** /views | Retrieves StreetAccount search views
 
 
 ## Documentation For Models
 
- - [Checkstatus](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/Checkstatus.md)
- - [CheckstatusResponse](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/CheckstatusResponse.md)
- - [CreateEditDeleteViewResponse](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/CreateEditDeleteViewResponse.md)
- - [CreateEditDeleteViewResponseData](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/CreateEditDeleteViewResponseData.md)
- - [CreateEditDeleteViewResponseDataMessage](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/CreateEditDeleteViewResponseDataMessage.md)
- - [CreateOrEditViewBody](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/CreateOrEditViewBody.md)
- - [CreateOrEditViewBodyData](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/CreateOrEditViewBodyData.md)
- - [CreateOrEditViewTickers](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/CreateOrEditViewTickers.md)
- - [Error](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/Error.md)
- - [ErrorObject](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/ErrorObject.md)
- - [FilterResponse](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/FilterResponse.md)
- - [FilterResponseData](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/FilterResponseData.md)
- - [FlattenedFilters](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/FlattenedFilters.md)
- - [FlattenedFiltersCategoriesObject](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/FlattenedFiltersCategoriesObject.md)
- - [FlattenedFiltersRegionsObject](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/FlattenedFiltersRegionsObject.md)
- - [FlattenedFiltersSectorsObject](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/FlattenedFiltersSectorsObject.md)
- - [FlattenedFiltersTopicsObject](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/FlattenedFiltersTopicsObject.md)
- - [FlattenedFiltersWatchlistsObject](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/FlattenedFiltersWatchlistsObject.md)
- - [Getfiles](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/Getfiles.md)
- - [GetfilesResponse](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/GetfilesResponse.md)
- - [IsPartialOne](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/IsPartialOne.md)
- - [MetaOne](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/MetaOne.md)
- - [PaginationOne](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/PaginationOne.md)
- - [RequestfilesResponse](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/RequestfilesResponse.md)
- - [SaHeadlinesRequest](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/SaHeadlinesRequest.md)
- - [SaHeadlinesRequestByView](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/SaHeadlinesRequestByView.md)
- - [SaHeadlinesRequestByViewData](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/SaHeadlinesRequestByViewData.md)
- - [SaHeadlinesRequestData](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/SaHeadlinesRequestData.md)
- - [SaHeadlinesRequestDataSearchDate](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/SaHeadlinesRequestDataSearchDate.md)
- - [SaHeadlinesRequestMeta](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/SaHeadlinesRequestMeta.md)
- - [SaHeadlinesRequestMetaPagination](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/SaHeadlinesRequestMetaPagination.md)
- - [SaHeadlinesRequestTickersObject](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/SaHeadlinesRequestTickersObject.md)
- - [SearchResponse](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/SearchResponse.md)
- - [SearchResponseArrayObject](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/SearchResponseArrayObject.md)
- - [SearchResponseData](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/SearchResponseData.md)
- - [SearchResponseMeta](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/SearchResponseMeta.md)
- - [SearchResponseMetaPagination](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/SearchResponseMetaPagination.md)
- - [StreetAccountStatus](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/StreetAccountStatus.md)
- - [StructuredFilters](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/StructuredFilters.md)
- - [StructuredFiltersCategoriesObject](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/StructuredFiltersCategoriesObject.md)
- - [StructuredFiltersChildrenObject](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/StructuredFiltersChildrenObject.md)
- - [StructuredFiltersRegionsObject](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/StructuredFiltersRegionsObject.md)
- - [StructuredFiltersSectorsObject](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/StructuredFiltersSectorsObject.md)
- - [StructuredFiltersTopicsObject](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/StructuredFiltersTopicsObject.md)
- - [StructuredFiltersWatchlistsObject](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/StructuredFiltersWatchlistsObject.md)
- - [Views](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/Views.md)
- - [ViewsObject](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v0/docs/ViewsObject.md)
+ - [CreateOrEditViewBody](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/CreateOrEditViewBody.md)
+ - [CreateOrEditViewBodyData](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/CreateOrEditViewBodyData.md)
+ - [CreateOrEditViewTickers](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/CreateOrEditViewTickers.md)
+ - [CreateViewResponse](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/CreateViewResponse.md)
+ - [CreateViewResponseData](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/CreateViewResponseData.md)
+ - [DeleteViewBody](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/DeleteViewBody.md)
+ - [DeleteViewBodyData](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/DeleteViewBodyData.md)
+ - [Error](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/Error.md)
+ - [ErrorObject](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/ErrorObject.md)
+ - [FilterCategoriesResponse](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/FilterCategoriesResponse.md)
+ - [FilterCategoriesResponseData](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/FilterCategoriesResponseData.md)
+ - [FilterRegionsResponse](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/FilterRegionsResponse.md)
+ - [FilterRegionsResponseData](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/FilterRegionsResponseData.md)
+ - [FilterResponse](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/FilterResponse.md)
+ - [FilterResponseData](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/FilterResponseData.md)
+ - [FilterSectorsResponse](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/FilterSectorsResponse.md)
+ - [FilterSectorsResponseData](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/FilterSectorsResponseData.md)
+ - [FilterTopicResponse](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/FilterTopicResponse.md)
+ - [FilterTopicResponseData](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/FilterTopicResponseData.md)
+ - [FilterWatchlistsResponse](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/FilterWatchlistsResponse.md)
+ - [FilterWatchlistsResponseData](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/FilterWatchlistsResponseData.md)
+ - [FlattenedFilters](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/FlattenedFilters.md)
+ - [FlattenedFiltersCategories](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/FlattenedFiltersCategories.md)
+ - [FlattenedFiltersCategoriesObject](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/FlattenedFiltersCategoriesObject.md)
+ - [FlattenedFiltersRegions](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/FlattenedFiltersRegions.md)
+ - [FlattenedFiltersRegionsObject](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/FlattenedFiltersRegionsObject.md)
+ - [FlattenedFiltersSectors](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/FlattenedFiltersSectors.md)
+ - [FlattenedFiltersSectorsObject](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/FlattenedFiltersSectorsObject.md)
+ - [FlattenedFiltersTopics](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/FlattenedFiltersTopics.md)
+ - [FlattenedFiltersTopicsObject](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/FlattenedFiltersTopicsObject.md)
+ - [FlattenedFiltersWatchlists](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/FlattenedFiltersWatchlists.md)
+ - [FlattenedFiltersWatchlistsObject](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/FlattenedFiltersWatchlistsObject.md)
+ - [HeadlinesRequest](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/HeadlinesRequest.md)
+ - [HeadlinesRequestByView](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/HeadlinesRequestByView.md)
+ - [HeadlinesRequestByViewData](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/HeadlinesRequestByViewData.md)
+ - [HeadlinesRequestByViewMeta](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/HeadlinesRequestByViewMeta.md)
+ - [HeadlinesRequestData](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/HeadlinesRequestData.md)
+ - [HeadlinesRequestDataSearchTime](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/HeadlinesRequestDataSearchTime.md)
+ - [HeadlinesRequestMeta](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/HeadlinesRequestMeta.md)
+ - [HeadlinesRequestMetaPagination](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/HeadlinesRequestMetaPagination.md)
+ - [HeadlinesRequestTickersObject](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/HeadlinesRequestTickersObject.md)
+ - [HeadlinesResponse](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/HeadlinesResponse.md)
+ - [HeadlinesResponseMeta](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/HeadlinesResponseMeta.md)
+ - [HeadlinesResponseMetaPagination](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/HeadlinesResponseMetaPagination.md)
+ - [QuickAlertsBody](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/QuickAlertsBody.md)
+ - [QuickAlertsBodyData](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/QuickAlertsBodyData.md)
+ - [QuickAlertsResponse](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/QuickAlertsResponse.md)
+ - [SearchResponseArrayObject](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/SearchResponseArrayObject.md)
+ - [StructuredFilters](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/StructuredFilters.md)
+ - [StructuredFiltersCategories](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/StructuredFiltersCategories.md)
+ - [StructuredFiltersCategoriesObject](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/StructuredFiltersCategoriesObject.md)
+ - [StructuredFiltersChildrenObjectCategories](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/StructuredFiltersChildrenObjectCategories.md)
+ - [StructuredFiltersChildrenObjectRegions](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/StructuredFiltersChildrenObjectRegions.md)
+ - [StructuredFiltersChildrenObjectSectors](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/StructuredFiltersChildrenObjectSectors.md)
+ - [StructuredFiltersChildrenObjectTopics](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/StructuredFiltersChildrenObjectTopics.md)
+ - [StructuredFiltersRegions](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/StructuredFiltersRegions.md)
+ - [StructuredFiltersRegionsObject](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/StructuredFiltersRegionsObject.md)
+ - [StructuredFiltersSectors](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/StructuredFiltersSectors.md)
+ - [StructuredFiltersSectorsObject](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/StructuredFiltersSectorsObject.md)
+ - [StructuredFiltersTopics](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/StructuredFiltersTopics.md)
+ - [StructuredFiltersTopicsObject](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/StructuredFiltersTopicsObject.md)
+ - [StructuredFiltersWatchlists](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/StructuredFiltersWatchlists.md)
+ - [StructuredFiltersWatchlistsObject](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/StructuredFiltersWatchlistsObject.md)
+ - [Views](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/Views.md)
+ - [ViewsObject](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/StreetAccountNews/v1/docs/ViewsObject.md)
 
 
 ## Documentation For Authorization
 
 
 ## FactSetApiKey
```

## Comparing `fds.sdk.StreetAccountNews-0.20.4.dist-info/RECORD` & `fds.sdk.StreetAccountNews-0.40.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,68 +1,85 @@
 fds/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fds/sdk/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-fds/sdk/StreetAccountNews/__init__.py,sha256=3vmEBAH0w4aiohHcfa5R1JbTb0LHO_b5ArtXNfdENmw,2302
-fds/sdk/StreetAccountNews/api_client.py,sha256=HGpsLw2GF_LOcPcLd-NtFS4lX0SVqUpwXK4gvIkrm00,41311
-fds/sdk/StreetAccountNews/configuration.py,sha256=SQ7plL2SfsVaFM5D6S1JMbYtYOpfMbqD_urTRzywGMc,19869
-fds/sdk/StreetAccountNews/exceptions.py,sha256=RDwWax16wClPc8ZVES3txZa17ydbF8JZzD3CJn9xVDg,6535
-fds/sdk/StreetAccountNews/model_utils.py,sha256=T5LRNxlRClvwfjkFtjhLzpL2xh0M2aaaPObi4SjejP0,83930
-fds/sdk/StreetAccountNews/rest.py,sha256=DTa9QspAtpi1UVhrymWYJMPv4Bp88IllMPtz1zvq7B8,15670
+fds/sdk/StreetAccountNews/__init__.py,sha256=fNB0hDO4MW2G5RmmAo8X6nnj7n-T5ZZGi8wkBC57_1A,1527
+fds/sdk/StreetAccountNews/api_client.py,sha256=J8dfapo0WhKg0fzO3Jk4OatRIY7nJ2SBkvCHBUMEqIs,40536
+fds/sdk/StreetAccountNews/configuration.py,sha256=4xKGgvnwR33W2zO0jNH4az01v5PSr9J4_5LETNnTSGs,19088
+fds/sdk/StreetAccountNews/exceptions.py,sha256=lRnT7nPBzml4rRGmRJz6nJBV9dJtBEvyTtNdZW0HsQY,5760
+fds/sdk/StreetAccountNews/model_utils.py,sha256=X1JotRxQkmEdbTkYdMXejn05VELGi0hfb77kyEusBO4,83155
+fds/sdk/StreetAccountNews/rest.py,sha256=dwFtL5kL4B5W4T2HVtW9_Eb1n4CbV1Hl_NXR1mzDNcA,14895
 fds/sdk/StreetAccountNews/api/__init__.py,sha256=vXHnPz_Fg8jJH0DxCBeLcgJgr_2wpRMif2IG8zjxtK0,229
-fds/sdk/StreetAccountNews/api/filters_api.py,sha256=0PPzg193y-nWqD-roFop2ZsqyNtiMQPnfPk2etjGZDQ,16694
-fds/sdk/StreetAccountNews/api/headlines_api.py,sha256=BiSHrlJaYDzTUpPguXbJgGgNvgOUKlBOJUsNLgwxqu8,27575
-fds/sdk/StreetAccountNews/api/street_account_historical_stories_api.py,sha256=ZbQXlGAgd5EUPIzZAmKwW1mr8AbfOWuJYPwXzNvwYUU,44273
-fds/sdk/StreetAccountNews/api/views_api.py,sha256=yLx4EMrGk6IFUNpzrUsUGECJf8TTP62r4gWvaW0Y58o,49409
-fds/sdk/StreetAccountNews/apis/__init__.py,sha256=JOb6bU4bsB6LoaNCIpZmTOZAVhF_g9vQMCYpuJfRYM0,722
+fds/sdk/StreetAccountNews/api/filters_api.py,sha256=OtHxU1E7jBKkOCiWmj1FCAFVGg78F7XuKvPSDxbghkY,82012
+fds/sdk/StreetAccountNews/api/headlines_api.py,sha256=Zw2jakS5Zvp8GjTkBcheNLIPTORhmNZSPrhugB_qRnc,26993
+fds/sdk/StreetAccountNews/api/views_api.py,sha256=1BlwNMExYBV4aLgO-qm9asLC437imzqja1aA6zqVx-8,68780
+fds/sdk/StreetAccountNews/apis/__init__.py,sha256=t_KDEaY3MYssNqmm3_Liy7XLo7NvCugKIwD0gyTDUaA,608
 fds/sdk/StreetAccountNews/model/__init__.py,sha256=N49d9K35V_Hd5lOHWcMeVRl0Iy_-L-03rZgfKXwlESM,348
-fds/sdk/StreetAccountNews/model/checkstatus.py,sha256=csNkteJHX_BInx_1sRM5VVg10OYah7q1zqNwi2yAqMw,14532
-fds/sdk/StreetAccountNews/model/checkstatus_response.py,sha256=eU_NozKDATUnodZdRLozSYwQ0WoMFKBbk1-ydUJNwus,13022
-fds/sdk/StreetAccountNews/model/create_edit_delete_view_response.py,sha256=vn8W2gPVCjoiyNhPg_1-j0VEuAtwER2lI5gtaD8DRCM,12905
-fds/sdk/StreetAccountNews/model/create_edit_delete_view_response_data.py,sha256=DQd_7W3v3MuZzi7nz8yTl3G4pBs-W_Ex45h4qq3lC34,13150
-fds/sdk/StreetAccountNews/model/create_edit_delete_view_response_data_message.py,sha256=XDE7GXuji1JxaT7DQhoFPNa4ZFsbhJA2b82jXuN3zic,12583
-fds/sdk/StreetAccountNews/model/create_or_edit_view_body.py,sha256=K2uQK1N4Qoki7OWTJVEvWanXXjhmqrudth22qL2AORc,12825
-fds/sdk/StreetAccountNews/model/create_or_edit_view_body_data.py,sha256=Oz5OJmIkddta-x2YxkP0FR4uRG_NvxzAJ4ywMWJW9JA,14081
-fds/sdk/StreetAccountNews/model/create_or_edit_view_tickers.py,sha256=vSTg-Zd_Xz8KVB7B37vfXOFHt0VzVBjbkyj6ItbZo-E,13098
-fds/sdk/StreetAccountNews/model/error.py,sha256=fO3YATdjSRdW7iA_4cZZjKh0jnqBQQ7ziyssctX2Igc,13077
-fds/sdk/StreetAccountNews/model/error_object.py,sha256=fS-Awe-eYqce7ez2wyVjAiBPc6D1DgG40anAFXVAM8A,12850
-fds/sdk/StreetAccountNews/model/filter_response.py,sha256=p11VXbs1pmjauPUOdmRdUMgBK9p8xS-Y2gUIvXiNHLc,12762
-fds/sdk/StreetAccountNews/model/filter_response_data.py,sha256=tIx3_7Y5a5Ch9Wv-SwcYXYbpgFtcx48IRc82GAm0L7s,13252
-fds/sdk/StreetAccountNews/model/flattened_filters.py,sha256=EIKgAvPm6OpiHZddH16yjOOWAM9LfTQZ0jdvXsALDEY,14795
-fds/sdk/StreetAccountNews/model/flattened_filters_categories_object.py,sha256=4gGAdE9Y2RZl4hm8JHC9YouTTVG50x6WMayp61kwXo0,12751
-fds/sdk/StreetAccountNews/model/flattened_filters_regions_object.py,sha256=-aGAGkN3MuFhDfX4KLg_3OerRH5e0wzXSBBwmgNAnLg,12748
-fds/sdk/StreetAccountNews/model/flattened_filters_sectors_object.py,sha256=eSpLgx-RZ_1ZaEStv3kGzvMu15skVkT9_IXXNZ-W5ew,12748
-fds/sdk/StreetAccountNews/model/flattened_filters_topics_object.py,sha256=7D1BLtw2UAY67lhty3SPzm9YoiIOjmnlsh-5KHP5VG0,12739
-fds/sdk/StreetAccountNews/model/flattened_filters_watchlists_object.py,sha256=dYnH8TmV9El7QgIXQQBDHYz4r8qqTohoS3ewZDiXhCo,12923
-fds/sdk/StreetAccountNews/model/getfiles.py,sha256=bcF1yuH0q_ui1qCPcPxBEJ_1teMYB9dLgNvQyWziHak,14383
-fds/sdk/StreetAccountNews/model/getfiles_response.py,sha256=kU1mFxtZJ3Z2_8JziSeqwyAPXZefMGzxXGb_ggLdwwE,12992
-fds/sdk/StreetAccountNews/model/is_partial_one.py,sha256=tq-r3apyhPAzRK3abYf9BlZ9TwjgE4CbRy6EQ4NyFb8,12534
-fds/sdk/StreetAccountNews/model/meta_one.py,sha256=Xnl-Y4-y68_vrgknj474q1UHjbkmXYT0ExZvzp262q0,13076
-fds/sdk/StreetAccountNews/model/pagination_one.py,sha256=JOnPEgup6OjO6JtKEE_lV6o_5u2wfnbFxme2yvWsasQ,14200
-fds/sdk/StreetAccountNews/model/requestfiles_response.py,sha256=6N3Vrn_a-I-8j1D5W052f7sI-UhGcMI8SU3ky19-s84,12973
-fds/sdk/StreetAccountNews/model/sa_headlines_request.py,sha256=B4-8FiNJddTvcnc3kxdIDATOBdwUzvPViGsn3LIrTXI,13200
-fds/sdk/StreetAccountNews/model/sa_headlines_request_by_view.py,sha256=9dBQurfZXNxUnk1i4I9-tS_lOZVe-lKGwXvlp9PCtps,13262
-fds/sdk/StreetAccountNews/model/sa_headlines_request_by_view_data.py,sha256=12GFZpm7f0u9vHi7rT3zxv21KXL61UX8jqEOKjbgSY8,12939
-fds/sdk/StreetAccountNews/model/sa_headlines_request_data.py,sha256=7G6PUvKUjyUFS9r9wJAV10EbNLXXeS2dNxdr9srrvCs,14419
-fds/sdk/StreetAccountNews/model/sa_headlines_request_data_search_date.py,sha256=HH7vVQwfP3S2U0M-MFLVDybM8KsTZPCd5-dxh1SGFiM,13492
-fds/sdk/StreetAccountNews/model/sa_headlines_request_meta.py,sha256=2gvxbxH459Mr-IaGtxkmk1KxpLhl2pwiklwETPUyxHo,12916
-fds/sdk/StreetAccountNews/model/sa_headlines_request_meta_pagination.py,sha256=J98Mcq2PJaMRrjgiwHnn3pFNRqyYJ02LqWE5tyIyBgo,13159
-fds/sdk/StreetAccountNews/model/sa_headlines_request_tickers_object.py,sha256=xxjE8ZBN84hGuV5odrnlINpdte0ds8HzqrfmP3wvC30,13218
-fds/sdk/StreetAccountNews/model/search_response.py,sha256=MCH0Qum-7m9Ik8XiSQ-5eatEWCdZvnQ3uPoLSWu4c3o,13130
-fds/sdk/StreetAccountNews/model/search_response_array_object.py,sha256=3ykDm0jlmmVLetBOTmAx2TegQHgmqB0RccNvNrBlVCg,14251
-fds/sdk/StreetAccountNews/model/search_response_data.py,sha256=qmBhOB4CXGUnDL2YtUhv76q5rkyRFI2RpC-NtCkXHF0,12845
-fds/sdk/StreetAccountNews/model/search_response_meta.py,sha256=hOq-5ubW8Mbt2gup5IDim-edz_zpfRo-gcNZAtvAw6o,13092
-fds/sdk/StreetAccountNews/model/search_response_meta_pagination.py,sha256=MQ578tlLDS_4xtPAFwzE3KdEqvC7qAME2UyamYmQXX0,12804
-fds/sdk/StreetAccountNews/model/street_account_status.py,sha256=Fh7ncYZFBc89Sg8mBaNQM6w9iEOtfbGWGPEmAyIgDrk,12782
-fds/sdk/StreetAccountNews/model/structured_filters.py,sha256=36Lbk0H_Mn4DnhkOvhiTHXJeHrUn5bQixcOstc7yRDc,14833
-fds/sdk/StreetAccountNews/model/structured_filters_categories_object.py,sha256=tmt77qLs_zIDxbRjIkEId4ukn_KD5Ikz-vNks9kde0A,13304
-fds/sdk/StreetAccountNews/model/structured_filters_children_object.py,sha256=_OqUYefoKBOK8e1jHdIo1xMrKE3NnOnZH9IKgaKPmBI,12748
-fds/sdk/StreetAccountNews/model/structured_filters_regions_object.py,sha256=wJTfCn1sZKu6Z0y-hhEpsqBt6xuorbyn3ExxFoYbjiQ,12751
-fds/sdk/StreetAccountNews/model/structured_filters_sectors_object.py,sha256=SD7huAik5q4sGSnXzE9ickDDlDHdF_1Jh7AzgubA6hk,13307
-fds/sdk/StreetAccountNews/model/structured_filters_topics_object.py,sha256=ZK5v-QDQ87g7SzqxkMJ-x2XpURs7tIhjUqkqZJiMHdE,13292
-fds/sdk/StreetAccountNews/model/structured_filters_watchlists_object.py,sha256=F41bjsF5BOWQoDpyWKudbPGuYd2lCH44HYG3P8QtFsQ,12926
-fds/sdk/StreetAccountNews/model/views.py,sha256=8sD269s--OdkxHWeMfyX-tsH5dyJFYFkF-QIg2mGjNo,12691
-fds/sdk/StreetAccountNews/model/views_object.py,sha256=0olPMf0OVXTsbqUh4BT728lFE-_iAyS9Zcn2IyLL5kU,13738
-fds/sdk/StreetAccountNews/models/__init__.py,sha256=g_w6edFYiXYQR4gUfMNjLn3bYJbDt2TlAXFAbCEXT_o,4739
-fds.sdk.StreetAccountNews-0.20.4.dist-info/LICENSE,sha256=o360nv5Th1nES3Sbtp01thapHTMCT0CzuS7uq_ro8fw,11358
-fds.sdk.StreetAccountNews-0.20.4.dist-info/METADATA,sha256=3r-LZ3WWQAzJMuy8RnshH_m5_pEVdydqVtI08Ct8Vr4,20925
-fds.sdk.StreetAccountNews-0.20.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-fds.sdk.StreetAccountNews-0.20.4.dist-info/top_level.txt,sha256=52v1bB-782Xh07STWqzml3q9GVhwaqsY3NCEMiH3Hnc,4
-fds.sdk.StreetAccountNews-0.20.4.dist-info/RECORD,,
+fds/sdk/StreetAccountNews/model/create_or_edit_view_body.py,sha256=RqDpGJzix5aRh8YXHxV7axq1OgSx1GncjCQHtviXerQ,12050
+fds/sdk/StreetAccountNews/model/create_or_edit_view_body_data.py,sha256=YUE9kSaYPfPJPqQ6nHQtVKGh55y6twO5l3Mh06Jf-bM,14298
+fds/sdk/StreetAccountNews/model/create_or_edit_view_tickers.py,sha256=JN0WlCafSL8AdVisuLeMvX-L_Bnlycr5qNV_rfB8ai8,12323
+fds/sdk/StreetAccountNews/model/create_view_response.py,sha256=p3iBl2_mOQeWQLkC1VoLnwAFsO_DpfXIYcIGyG_8Imw,12028
+fds/sdk/StreetAccountNews/model/create_view_response_data.py,sha256=rDkgtjxX1pnxfCdYi4uRrq27dn7uTJsoCsWFtqDSNq4,11819
+fds/sdk/StreetAccountNews/model/delete_view_body.py,sha256=Co74EF9WrnYHZiq8yQ3bKYiMDLwnSz2A9aCuFCuj0fc,11988
+fds/sdk/StreetAccountNews/model/delete_view_body_data.py,sha256=N5gCF5e-7x4Vj_QwQxeIIYj_xFG4OkYF941sHL_asGA,11819
+fds/sdk/StreetAccountNews/model/error.py,sha256=MTZU5YXcsa1CIdZ1onYE6n7AcLvEQL3iAd2LtQTW8Nw,11926
+fds/sdk/StreetAccountNews/model/error_object.py,sha256=mixiC3NGlsbB_CBTsE1iZghRzEPcTM1UCKIahJNM540,12075
+fds/sdk/StreetAccountNews/model/filter_categories_response.py,sha256=3oIIkoWkXS7QNCYmWMKoaCSXmMzWFab2lTMpo5QuoTg,12088
+fds/sdk/StreetAccountNews/model/filter_categories_response_data.py,sha256=ntTp4TRd5SBIjECpqORQtY-CxY3GBzLIVX3ibvxKYng,12571
+fds/sdk/StreetAccountNews/model/filter_regions_response.py,sha256=OG0roGQNx4rXWQoZ6rCM9oUo-30gjHSfIsh0Xd8g2qE,12058
+fds/sdk/StreetAccountNews/model/filter_regions_response_data.py,sha256=87-8GXummL4qt0zpvxlLnnk5ZcEyjqmg6zG23irdV-c,12520
+fds/sdk/StreetAccountNews/model/filter_response.py,sha256=OC2cNwszVYSvS8DRAuUkLsjh2RKbFG7O1T3vziUPC88,11987
+fds/sdk/StreetAccountNews/model/filter_response_data.py,sha256=VjbB4jF5YY3Syj7UT7WHBFIwofo3MA0SE51R7s82dQE,12399
+fds/sdk/StreetAccountNews/model/filter_sectors_response.py,sha256=6rpDjndC7Lerx15AYE9ULujRG6CzLQzYrazrP1vmJIM,12058
+fds/sdk/StreetAccountNews/model/filter_sectors_response_data.py,sha256=SgW1XWX_XQUYp_znscEUV0ibyUNc7pc1fWrwPFYrDN0,12520
+fds/sdk/StreetAccountNews/model/filter_topic_response.py,sha256=gP8ZyOcAvQ47A_hKdCTl4zMYOYuk_of4n_RWvBk-4ec,12038
+fds/sdk/StreetAccountNews/model/filter_topic_response_data.py,sha256=FaIt6OGl7qEcLcODb-jTG2QAXiykWJ0hwTjjO3jRnUE,12500
+fds/sdk/StreetAccountNews/model/filter_watchlists_response.py,sha256=Kc9ycE3AorjXC52Bt-pgrw1wYHdb_UeIQ-RQByl727w,12088
+fds/sdk/StreetAccountNews/model/filter_watchlists_response_data.py,sha256=Pg-lOQ3GBxU7nH7E6XF0_P66Y5ASZ4eO-hbiEkkfrwE,12571
+fds/sdk/StreetAccountNews/model/flattened_filters.py,sha256=MhnJ1T8I00ef7_OrJKA7BZCyv6gDg7e1Q8s0m0UscAA,14020
+fds/sdk/StreetAccountNews/model/flattened_filters_categories.py,sha256=tUhRFrFJ_KAweamWLiOBPXUDisJfFqrQlfdUYuVVDaI,12158
+fds/sdk/StreetAccountNews/model/flattened_filters_categories_object.py,sha256=pw1wxHER21t4UVVyq18WmRG8tj51Hj8VNnqWubMqFko,12164
+fds/sdk/StreetAccountNews/model/flattened_filters_regions.py,sha256=-oaAHwilSbbx6MnaIFTtWNvz3VMTWqHLA5LXOXjp5PM,12113
+fds/sdk/StreetAccountNews/model/flattened_filters_regions_object.py,sha256=87mJI9VvxTCGpAgk_QuG0Ixks5Pf2t7zFEr33gZ6b6c,12161
+fds/sdk/StreetAccountNews/model/flattened_filters_sectors.py,sha256=ff4RZYcD58G6g1J4U9VqYE9MAlEkxrxrCk2828M9HEg,12113
+fds/sdk/StreetAccountNews/model/flattened_filters_sectors_object.py,sha256=0nBvVcqkWStZeYNNgEQwfPzsCngkt40AMHVVHjx-BqU,12169
+fds/sdk/StreetAccountNews/model/flattened_filters_topics.py,sha256=8Aym37MRsZgKxWh759zKYZ_yaS4teeZy0J8w_8hXSnI,12098
+fds/sdk/StreetAccountNews/model/flattened_filters_topics_object.py,sha256=rAylq0wo0ydv5-XRaUPCuKN5I3GEAiT9HPyvtETYv_I,12138
+fds/sdk/StreetAccountNews/model/flattened_filters_watchlists.py,sha256=quV-HafjIYVnWl69xVvjI3clLxgM5yDcK3KaOviUYEo,12158
+fds/sdk/StreetAccountNews/model/flattened_filters_watchlists_object.py,sha256=3XxLLv06seuncW_Pf8uva7RCGjFfdDvlb8ZCLrRkwg4,12336
+fds/sdk/StreetAccountNews/model/headlines_request.py,sha256=R_Yqnvjn0tUBj-TIX-NtGQBfa9ik1tOmxxK4Qj8Ewjo,12389
+fds/sdk/StreetAccountNews/model/headlines_request_by_view.py,sha256=LGIPkS9FNQqa0R07W-hReq5eAt-FVfAihW-dbofPiVM,12495
+fds/sdk/StreetAccountNews/model/headlines_request_by_view_data.py,sha256=kdfB8oNYiqIKM7CUP6gaCyJl1irWfTalfduDaG9AjH4,13266
+fds/sdk/StreetAccountNews/model/headlines_request_by_view_meta.py,sha256=gGQwPvGx6uVxef9CWpHUUDrjVp2D0eZNVSah34gdcaU,12138
+fds/sdk/StreetAccountNews/model/headlines_request_data.py,sha256=CkdOGoqgYW8idWHjvi6cCC2z682CvzPCXreYWnEwxG8,16799
+fds/sdk/StreetAccountNews/model/headlines_request_data_search_time.py,sha256=e6r_rFA1CCoxyRpZUX4uJSN_3njdrbYR5R7-l2vsBec,12741
+fds/sdk/StreetAccountNews/model/headlines_request_meta.py,sha256=FVTITVnvVnHVy6O0mFUACbSKy0uFiZ3T6JkVhkaR2go,12946
+fds/sdk/StreetAccountNews/model/headlines_request_meta_pagination.py,sha256=blEBRMhPOqmdsy0ffBDYADrffNmLO6EftERuiwab_aI,12378
+fds/sdk/StreetAccountNews/model/headlines_request_tickers_object.py,sha256=MvC-BdKJd93ud7KdH9TG-aXaxu9XuEwZHR7_p4MqYT0,12517
+fds/sdk/StreetAccountNews/model/headlines_response.py,sha256=EpqNaIYHdrxBVqtKk3MxHJieai-kmrF9h6OSV-eN2bg,12441
+fds/sdk/StreetAccountNews/model/headlines_response_meta.py,sha256=ntnCqTd0BEr37fJWx7Gp8EHGCB39t-h_JdS85aJGtCU,12533
+fds/sdk/StreetAccountNews/model/headlines_response_meta_pagination.py,sha256=Iec0-UgYPsqAmB-vEm2hxFBLVF5tyUW6-NpBwWjQIfo,12038
+fds/sdk/StreetAccountNews/model/quick_alerts_body.py,sha256=AcyJ60eoU5EM3BRzMC_4w3t6dSrYyXQWmXgigCfOhAk,11998
+fds/sdk/StreetAccountNews/model/quick_alerts_body_data.py,sha256=Tl83njYMet_QKWnawgFFpjtNrAFfmP-AH9WaDxNHgI0,11852
+fds/sdk/StreetAccountNews/model/quick_alerts_response.py,sha256=KfQkRwMO33Y0QCxUgf_gWQjb_5djFhU2W8cLFY87TRE,12010
+fds/sdk/StreetAccountNews/model/search_response_array_object.py,sha256=cCXPsCnRW3_guTx6iVeqUJ2x_Az1optGPHpzMdBqxps,13853
+fds/sdk/StreetAccountNews/model/structured_filters.py,sha256=1NNWuhN40I6rCqvJ25d2WmjehvNd3oE63kPy2pQkbOw,14058
+fds/sdk/StreetAccountNews/model/structured_filters_categories.py,sha256=sF8tWRSf1NlXMD5d9wJJpXpXc-AtJr7i-JwG9l8TX8g,12168
+fds/sdk/StreetAccountNews/model/structured_filters_categories_object.py,sha256=miQW17Rp_b6MEUxTd4gOw-0a_vQyIuAd1hhBwo9tyLw,12716
+fds/sdk/StreetAccountNews/model/structured_filters_children_object_categories.py,sha256=V1uGVSF-IFXegmyi2mFXhAtnBNWVp_apJ3wugPzR444,12057
+fds/sdk/StreetAccountNews/model/structured_filters_children_object_regions.py,sha256=HxSqjodvKuhHsjA9mxfN22dEAkC4qZPL3aIK-fbwSLs,12048
+fds/sdk/StreetAccountNews/model/structured_filters_children_object_sectors.py,sha256=f09-uqew_UHo785P6vK_iLMHh7Bg72HwQWJBvjngXvg,12054
+fds/sdk/StreetAccountNews/model/structured_filters_children_object_topics.py,sha256=Ma-Vp17lDDhMqE-32DhURuwqZoJ-t5-y0FymSu6mX9g,12045
+fds/sdk/StreetAccountNews/model/structured_filters_regions.py,sha256=vjgnCy34iQNGJMe4SO9vdthrj5mymFJZlXKoBl8N26I,12123
+fds/sdk/StreetAccountNews/model/structured_filters_regions_object.py,sha256=xTDssDolcwQgTcpF6iGPOrmsEINZLFusmH_GajoVYEQ,12682
+fds/sdk/StreetAccountNews/model/structured_filters_sectors.py,sha256=gGCCauk6sAXkFWZCX_WMSg_0BZyVAUy1AzPi73Qu5LA,12123
+fds/sdk/StreetAccountNews/model/structured_filters_sectors_object.py,sha256=oxHgASG547eNW5KqyRaleyUpyZliXsDW4l_4y6q5gDY,12985
+fds/sdk/StreetAccountNews/model/structured_filters_topics.py,sha256=mZL9NjOMnWsDlDYc2m2O0HF9qUMB5-wrBsAuDTbhJ9A,12108
+fds/sdk/StreetAccountNews/model/structured_filters_topics_object.py,sha256=wvWoHysV1zHqV3yShmARhQDyVAfJlguYy_mpqhjg8ks,12664
+fds/sdk/StreetAccountNews/model/structured_filters_watchlists.py,sha256=s5ybiSSEUMvzZybQDTaLo5XSmphNv73rkjL1OwEIfuE,12168
+fds/sdk/StreetAccountNews/model/structured_filters_watchlists_object.py,sha256=20YF68akXAqsgQ56GNRECQ9la9UG-aL1YJ1i_mcp93s,12339
+fds/sdk/StreetAccountNews/model/views.py,sha256=mTbmWuKyYuNLfEZN1tDvm8H9_mGFiAgrCMQEHIJ1Z1s,11916
+fds/sdk/StreetAccountNews/model/views_object.py,sha256=v-eqMB-csQXP4NLfhOqbLNPaBvWRcJCiCLtKHertvRg,13780
+fds/sdk/StreetAccountNews/models/__init__.py,sha256=rb2ITaPVGHUXDJqh5df0_sMw6Mfoi5XrA6Xx4ruVkoU,6628
+fds.sdk.StreetAccountNews-0.40.0.dist-info/LICENSE,sha256=o360nv5Th1nES3Sbtp01thapHTMCT0CzuS7uq_ro8fw,11358
+fds.sdk.StreetAccountNews-0.40.0.dist-info/METADATA,sha256=kIkJn0NvGTeMh4Rq2JhnqaGslvIvSHuE-Lm5X9fC9PQ,23664
+fds.sdk.StreetAccountNews-0.40.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+fds.sdk.StreetAccountNews-0.40.0.dist-info/top_level.txt,sha256=52v1bB-782Xh07STWqzml3q9GVhwaqsY3NCEMiH3Hnc,4
+fds.sdk.StreetAccountNews-0.40.0.dist-info/RECORD,,
```

