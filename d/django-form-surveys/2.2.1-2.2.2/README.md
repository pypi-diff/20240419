# Comparing `tmp/django-form-surveys-2.2.1.tar.gz` & `tmp/django-form-surveys-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-form-surveys-2.2.1.tar", last modified: Mon Mar 18 07:08:46 2024, max compression
+gzip compressed data, was "django-form-surveys-2.2.2.tar", last modified: Fri Apr 19 03:04:51 2024, max compression
```

## Comparing `django-form-surveys-2.2.1.tar` & `django-form-surveys-2.2.2.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-03-18 07:08:46.221471 django-form-surveys-2.2.1/
--rw-r--r--   0 irfanpule   (501) staff       (20)     1059 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/LICENSE
--rw-r--r--   0 irfanpule   (501) staff       (20)      158 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/MANIFEST.in
--rw-r--r--   0 irfanpule   (501) staff       (20)     7828 2024-03-18 07:08:46.221291 django-form-surveys-2.2.1/PKG-INFO
--rw-r--r--   0 irfanpule   (501) staff       (20)     6580 2024-03-15 06:26:40.000000 django-form-surveys-2.2.1/README.md
-drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-03-18 07:08:46.186300 django-form-surveys-2.2.1/django_form_surveys.egg-info/
--rw-r--r--   0 irfanpule   (501) staff       (20)     7828 2024-03-18 07:08:46.000000 django-form-surveys-2.2.1/django_form_surveys.egg-info/PKG-INFO
--rw-r--r--   0 irfanpule   (501) staff       (20)     4943 2024-03-18 07:08:46.000000 django-form-surveys-2.2.1/django_form_surveys.egg-info/SOURCES.txt
--rw-r--r--   0 irfanpule   (501) staff       (20)        1 2024-03-18 07:08:46.000000 django-form-surveys-2.2.1/django_form_surveys.egg-info/dependency_links.txt
--rw-r--r--   0 irfanpule   (501) staff       (20)        1 2023-05-02 07:50:06.000000 django-form-surveys-2.2.1/django_form_surveys.egg-info/not-zip-safe
--rw-r--r--   0 irfanpule   (501) staff       (20)       17 2024-03-18 07:08:46.000000 django-form-surveys-2.2.1/django_form_surveys.egg-info/requires.txt
--rw-r--r--   0 irfanpule   (501) staff       (20)      101 2024-03-18 07:08:46.000000 django-form-surveys-2.2.1/django_form_surveys.egg-info/top_level.txt
-drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-03-18 07:08:46.191013 django-form-surveys-2.2.1/djf_surveys/
--rw-r--r--   0 irfanpule   (501) staff       (20)       81 2024-03-18 07:08:05.000000 django-form-surveys-2.2.1/djf_surveys/__init__.py
--rw-r--r--   0 irfanpule   (501) staff       (20)      983 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/djf_surveys/admin.py
-drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-03-18 07:08:46.191734 django-form-surveys-2.2.1/djf_surveys/admins/
--rw-r--r--   0 irfanpule   (501) staff       (20)        0 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/djf_surveys/admins/__init__.py
--rw-r--r--   0 irfanpule   (501) staff       (20)     1387 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/djf_surveys/admins/urls.py
-drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-03-18 07:08:46.192719 django-form-surveys-2.2.1/djf_surveys/admins/v2/
--rw-r--r--   0 irfanpule   (501) staff       (20)        0 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/djf_surveys/admins/v2/__init__.py
--rw-r--r--   0 irfanpule   (501) staff       (20)     1685 2024-03-15 06:25:03.000000 django-form-surveys-2.2.1/djf_surveys/admins/v2/forms.py
--rw-r--r--   0 irfanpule   (501) staff       (20)     4229 2024-03-18 07:07:22.000000 django-form-surveys-2.2.1/djf_surveys/admins/v2/views.py
--rw-r--r--   0 irfanpule   (501) staff       (20)     8028 2024-02-27 06:22:45.000000 django-form-surveys-2.2.1/djf_surveys/admins/views.py
--rw-r--r--   0 irfanpule   (501) staff       (20)     2363 2024-03-15 06:25:03.000000 django-form-surveys-2.2.1/djf_surveys/app_settings.py
--rw-r--r--   0 irfanpule   (501) staff       (20)      194 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/djf_surveys/apps.py
--rw-r--r--   0 irfanpule   (501) staff       (20)      399 2024-03-15 06:25:03.000000 django-form-surveys-2.2.1/djf_surveys/context_processors.py
--rw-r--r--   0 irfanpule   (501) staff       (20)     7936 2024-03-18 07:07:22.000000 django-form-surveys-2.2.1/djf_surveys/forms.py
-drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-03-18 07:08:46.182966 django-form-surveys-2.2.1/djf_surveys/locale/
-drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-03-18 07:08:46.182733 django-form-surveys-2.2.1/djf_surveys/locale/en/
-drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-03-18 07:08:46.193012 django-form-surveys-2.2.1/djf_surveys/locale/en/LC_MESSAGES/
--rw-r--r--   0 irfanpule   (501) staff       (20)     5632 2023-12-13 09:57:48.000000 django-form-surveys-2.2.1/djf_surveys/locale/en/LC_MESSAGES/django.mo
-drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-03-18 07:08:46.182883 django-form-surveys-2.2.1/djf_surveys/locale/fr/
-drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-03-18 07:08:46.193201 django-form-surveys-2.2.1/djf_surveys/locale/fr/LC_MESSAGES/
--rw-r--r--   0 irfanpule   (501) staff       (20)     6132 2023-12-13 09:57:48.000000 django-form-surveys-2.2.1/djf_surveys/locale/fr/LC_MESSAGES/django.mo
-drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-03-18 07:08:46.183024 django-form-surveys-2.2.1/djf_surveys/locale/id/
-drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-03-18 07:08:46.193687 django-form-surveys-2.2.1/djf_surveys/locale/id/LC_MESSAGES/
--rw-r--r--   0 irfanpule   (501) staff       (20)     5906 2023-12-13 09:57:48.000000 django-form-surveys-2.2.1/djf_surveys/locale/id/LC_MESSAGES/django.mo
-drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-03-18 07:08:46.197426 django-form-surveys-2.2.1/djf_surveys/migrations/
--rw-r--r--   0 irfanpule   (501) staff       (20)     3775 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/djf_surveys/migrations/0001_initial.py
--rw-r--r--   0 irfanpule   (501) staff       (20)      860 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/djf_surveys/migrations/0002_auto_20220330_1033.py
--rw-r--r--   0 irfanpule   (501) staff       (20)      553 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/djf_surveys/migrations/0003_auto_20220330_1036.py
--rw-r--r--   0 irfanpule   (501) staff       (20)      850 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/djf_surveys/migrations/0004_auto_20220330_1112.py
--rw-r--r--   0 irfanpule   (501) staff       (20)      377 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/djf_surveys/migrations/0005_auto_20220404_1518.py
--rw-r--r--   0 irfanpule   (501) staff       (20)      451 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/djf_surveys/migrations/0006_survey_private_response.py
--rw-r--r--   0 irfanpule   (501) staff       (20)      895 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/djf_surveys/migrations/0007_auto_20220525_1126.py
--rw-r--r--   0 irfanpule   (501) staff       (20)      520 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/djf_surveys/migrations/0008_auto_20220721_0935.py
--rw-r--r--   0 irfanpule   (501) staff       (20)      784 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/djf_surveys/migrations/0009_auto_20220803_0927.py
--rw-r--r--   0 irfanpule   (501) staff       (20)     8956 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/djf_surveys/migrations/0010_model_translation.py
--rw-r--r--   0 irfanpule   (501) staff       (20)      662 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/djf_surveys/migrations/0011_alter_question_key.py
--rw-r--r--   0 irfanpule   (501) staff       (20)      510 2024-02-27 06:22:45.000000 django-form-surveys-2.2.1/djf_surveys/migrations/0012_survey_notification_to.py
--rw-r--r--   0 irfanpule   (501) staff       (20)      610 2024-03-15 06:25:03.000000 django-form-surveys-2.2.1/djf_surveys/migrations/0013_survey_success_page_content.py
--rw-r--r--   0 irfanpule   (501) staff       (20)        0 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/djf_surveys/migrations/__init__.py
--rw-r--r--   0 irfanpule   (501) staff       (20)      611 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/djf_surveys/mixin.py
--rw-r--r--   0 irfanpule   (501) staff       (20)     7958 2024-03-18 07:07:22.000000 django-form-surveys-2.2.1/djf_surveys/models.py
-drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-03-18 07:08:46.183246 django-form-surveys-2.2.1/djf_surveys/static/
-drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-03-18 07:08:46.183475 django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/
-drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-03-18 07:08:46.198427 django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/css/
--rw-r--r--   0 irfanpule   (501) staff       (20)      389 2024-02-07 10:57:48.000000 django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/css/rating.css
--rw-r--r--   0 irfanpule   (501) staff       (20)   356448 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/css/tailwindcss-3.3.1.js
--rw-r--r--   0 irfanpule   (501) staff       (20)   455935 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/css/tailwindcss-plugin-3.3.1.js
-drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-03-18 07:08:46.199415 django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/images/
--rw-r--r--   0 irfanpule   (501) staff       (20)     2962 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/images/star-border.png
--rw-r--r--   0 irfanpule   (501) staff       (20)     2729 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/images/star-fill.png
-drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-03-18 07:08:46.183619 django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/te-starter/
-drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-03-18 07:08:46.202108 django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/te-starter/css/
--rw-r--r--   0 irfanpule   (501) staff       (20)   198463 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/te-starter/css/tw-elements.min.css
--rw-r--r--   0 irfanpule   (501) staff       (20)      121 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/te-starter/css/tw-elements.min.css.map
-drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-03-18 07:08:46.207441 django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/te-starter/js/
--rw-r--r--   0 irfanpule   (501) staff       (20)   270873 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/te-starter/js/chart.es.js
--rw-r--r--   0 irfanpule   (501) staff       (20)   783041 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/te-starter/js/chart.es.js.map
--rw-r--r--   0 irfanpule   (501) staff       (20)    12217 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/te-starter/js/chartjs-plugin-datalabels.es.js
--rw-r--r--   0 irfanpule   (501) staff       (20)    50339 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/te-starter/js/chartjs-plugin-datalabels.es.js.map
--rw-r--r--   0 irfanpule   (501) staff       (20)   425275 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.es.min.js
--rw-r--r--   0 irfanpule   (501) staff       (20)  1151819 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.es.min.js.map
--rw-r--r--   0 irfanpule   (501) staff       (20)   539120 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.umd.min.js
--rw-r--r--   0 irfanpule   (501) staff       (20)  1929935 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.umd.min.js.map
--rw-r--r--   0 irfanpule   (501) staff       (20)     7569 2024-03-18 07:07:22.000000 django-form-surveys-2.2.1/djf_surveys/summary.py
-drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-03-18 07:08:46.183775 django-form-surveys-2.2.1/djf_surveys/templates/
-drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-03-18 07:08:46.211305 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/
-drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-03-18 07:08:46.213477 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/admins/
--rw-r--r--   0 irfanpule   (501) staff       (20)     1761 2024-02-06 15:05:01.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/admins/form.html
--rw-r--r--   0 irfanpule   (501) staff       (20)     7165 2024-02-06 15:05:01.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/admins/form_preview.html
--rw-r--r--   0 irfanpule   (501) staff       (20)     1132 2024-02-06 15:05:01.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/admins/master.html
--rw-r--r--   0 irfanpule   (501) staff       (20)      702 2024-02-06 15:05:01.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/admins/question_form.html
--rw-r--r--   0 irfanpule   (501) staff       (20)       45 2024-02-06 15:05:01.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/admins/question_form_v2.html
--rw-r--r--   0 irfanpule   (501) staff       (20)     1790 2024-02-06 15:05:01.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/admins/summary.html
--rw-r--r--   0 irfanpule   (501) staff       (20)     1490 2024-02-06 15:05:01.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/admins/survey_list.html
--rw-r--r--   0 irfanpule   (501) staff       (20)     4237 2024-02-06 15:05:01.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/answer_list.html
-drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-03-18 07:08:46.214652 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/buttons/
--rw-r--r--   0 irfanpule   (501) staff       (20)      292 2024-02-06 15:05:01.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/buttons/add_button.html
--rw-r--r--   0 irfanpule   (501) staff       (20)      343 2024-02-06 15:05:01.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/buttons/delete_button.html
--rw-r--r--   0 irfanpule   (501) staff       (20)      309 2024-02-06 15:05:01.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/buttons/edit_button.html
--rw-r--r--   0 irfanpule   (501) staff       (20)      457 2024-02-06 15:05:01.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/buttons/share_button.html
-drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-03-18 07:08:46.218886 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/components/
--rw-r--r--   0 irfanpule   (501) staff       (20)     1638 2024-02-06 15:05:01.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/components/alert.html
--rw-r--r--   0 irfanpule   (501) staff       (20)      326 2024-02-06 15:05:01.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/components/alert_js.html
--rw-r--r--   0 irfanpule   (501) staff       (20)     2967 2024-03-15 03:01:39.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/components/card_list_answer.html
--rw-r--r--   0 irfanpule   (501) staff       (20)     2872 2024-02-06 15:09:24.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/components/card_list_survey.html
--rw-r--r--   0 irfanpule   (501) staff       (20)      347 2024-02-06 15:05:01.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/components/empty_state.html
--rw-r--r--   0 irfanpule   (501) staff       (20)     3324 2024-02-06 15:05:01.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/components/header_nav.html
--rw-r--r--   0 irfanpule   (501) staff       (20)     3622 2024-02-06 15:05:01.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/components/modal_choice_field_type.html
--rw-r--r--   0 irfanpule   (501) staff       (20)     3073 2024-02-06 15:05:01.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/components/modal_delete.html
--rw-r--r--   0 irfanpule   (501) staff       (20)      777 2024-02-06 15:05:01.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/components/modal_delete_js.html
--rw-r--r--   0 irfanpule   (501) staff       (20)     3552 2024-02-06 15:05:01.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/components/pagination.html
--rw-r--r--   0 irfanpule   (501) staff       (20)      968 2024-02-06 15:05:01.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/components/search_form.html
--rw-r--r--   0 irfanpule   (501) staff       (20)      570 2024-02-06 15:05:01.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/components/section_welcome.html
--rw-r--r--   0 irfanpule   (501) staff       (20)      557 2024-02-06 15:05:01.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/components/share_link_button_js.html
--rw-r--r--   0 irfanpule   (501) staff       (20)      557 2024-02-06 15:05:01.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/components/star_border.html
--rw-r--r--   0 irfanpule   (501) staff       (20)        0 2024-02-06 15:05:01.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/components/star_fill.html
--rw-r--r--   0 irfanpule   (501) staff       (20)      889 2024-02-06 15:05:01.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/detail_result.html
--rw-r--r--   0 irfanpule   (501) staff       (20)     2014 2024-02-06 15:05:01.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/form.html
--rw-r--r--   0 irfanpule   (501) staff       (20)      792 2024-02-06 15:05:01.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/master.html
--rw-r--r--   0 irfanpule   (501) staff       (20)     1633 2024-03-15 06:25:03.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/success-page.html
--rw-r--r--   0 irfanpule   (501) staff       (20)     1189 2024-02-06 15:05:01.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/survey_list.html
-drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-03-18 07:08:46.220313 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/widgets/
--rw-r--r--   0 irfanpule   (501) staff       (20)      247 2024-02-06 15:05:01.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/widgets/attrs_exclude_id.html
--rw-r--r--   0 irfanpule   (501) staff       (20)      538 2024-02-06 15:05:01.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/widgets/checkbox_option.html
--rw-r--r--   0 irfanpule   (501) staff       (20)      324 2024-02-06 16:37:27.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/widgets/datepicker.html
--rw-r--r--   0 irfanpule   (501) staff       (20)     5069 2024-02-06 15:05:01.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/widgets/inline_choices.html
--rw-r--r--   0 irfanpule   (501) staff       (20)      520 2024-02-06 15:05:01.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/widgets/radio_option.html
--rw-r--r--   0 irfanpule   (501) staff       (20)     1805 2024-02-06 15:05:15.000000 django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/widgets/star_rating.html
-drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-03-18 07:08:46.220831 django-form-surveys-2.2.1/djf_surveys/templatetags/
--rw-r--r--   0 irfanpule   (501) staff       (20)        0 2023-12-13 04:15:23.000000 django-form-surveys-2.2.1/djf_surveys/templatetags/__init__.py
--rw-r--r--   0 irfanpule   (501) staff       (20)      537 2024-02-06 15:05:15.000000 django-form-surveys-2.2.1/djf_surveys/templatetags/djf_survey_tags.py
--rw-r--r--   0 irfanpule   (501) staff       (20)      469 2024-02-06 15:05:15.000000 django-form-surveys-2.2.1/djf_surveys/tests.py
--rw-r--r--   0 irfanpule   (501) staff       (20)      887 2024-03-15 06:25:03.000000 django-form-surveys-2.2.1/djf_surveys/urls.py
--rw-r--r--   0 irfanpule   (501) staff       (20)     3750 2024-02-06 15:05:15.000000 django-form-surveys-2.2.1/djf_surveys/utils.py
--rw-r--r--   0 irfanpule   (501) staff       (20)      696 2024-02-06 15:05:15.000000 django-form-surveys-2.2.1/djf_surveys/validators.py
--rw-r--r--   0 irfanpule   (501) staff       (20)    10253 2024-03-18 07:07:22.000000 django-form-surveys-2.2.1/djf_surveys/views.py
--rw-r--r--   0 irfanpule   (501) staff       (20)     1298 2024-02-06 15:05:15.000000 django-form-surveys-2.2.1/djf_surveys/widgets.py
--rw-r--r--   0 irfanpule   (501) staff       (20)       38 2024-03-18 07:08:46.221545 django-form-surveys-2.2.1/setup.cfg
--rw-r--r--   0 irfanpule   (501) staff       (20)     3070 2024-02-28 09:21:30.000000 django-form-surveys-2.2.1/setup.py
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-04-19 03:04:51.315537 django-form-surveys-2.2.2/
+-rw-r--r--   0 irfanpule   (501) staff       (20)     1059 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/LICENSE
+-rw-r--r--   0 irfanpule   (501) staff       (20)      158 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/MANIFEST.in
+-rw-r--r--   0 irfanpule   (501) staff       (20)     7828 2024-04-19 03:04:51.315345 django-form-surveys-2.2.2/PKG-INFO
+-rw-r--r--   0 irfanpule   (501) staff       (20)     6580 2024-03-15 06:26:40.000000 django-form-surveys-2.2.2/README.md
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-04-19 03:04:51.283948 django-form-surveys-2.2.2/django_form_surveys.egg-info/
+-rw-r--r--   0 irfanpule   (501) staff       (20)     7828 2024-04-19 03:04:51.000000 django-form-surveys-2.2.2/django_form_surveys.egg-info/PKG-INFO
+-rw-r--r--   0 irfanpule   (501) staff       (20)     4943 2024-04-19 03:04:51.000000 django-form-surveys-2.2.2/django_form_surveys.egg-info/SOURCES.txt
+-rw-r--r--   0 irfanpule   (501) staff       (20)        1 2024-04-19 03:04:51.000000 django-form-surveys-2.2.2/django_form_surveys.egg-info/dependency_links.txt
+-rw-r--r--   0 irfanpule   (501) staff       (20)        1 2023-05-02 07:50:06.000000 django-form-surveys-2.2.2/django_form_surveys.egg-info/not-zip-safe
+-rw-r--r--   0 irfanpule   (501) staff       (20)       17 2024-04-19 03:04:51.000000 django-form-surveys-2.2.2/django_form_surveys.egg-info/requires.txt
+-rw-r--r--   0 irfanpule   (501) staff       (20)      101 2024-04-19 03:04:51.000000 django-form-surveys-2.2.2/django_form_surveys.egg-info/top_level.txt
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-04-19 03:04:51.287675 django-form-surveys-2.2.2/djf_surveys/
+-rw-r--r--   0 irfanpule   (501) staff       (20)       81 2024-04-19 03:04:29.000000 django-form-surveys-2.2.2/djf_surveys/__init__.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      983 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/djf_surveys/admin.py
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-04-19 03:04:51.288198 django-form-surveys-2.2.2/djf_surveys/admins/
+-rw-r--r--   0 irfanpule   (501) staff       (20)        0 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/djf_surveys/admins/__init__.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)     1387 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/djf_surveys/admins/urls.py
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-04-19 03:04:51.288909 django-form-surveys-2.2.2/djf_surveys/admins/v2/
+-rw-r--r--   0 irfanpule   (501) staff       (20)        0 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/djf_surveys/admins/v2/__init__.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)     1685 2024-03-15 06:25:03.000000 django-form-surveys-2.2.2/djf_surveys/admins/v2/forms.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)     4229 2024-03-18 07:07:22.000000 django-form-surveys-2.2.2/djf_surveys/admins/v2/views.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)     8028 2024-02-27 06:22:45.000000 django-form-surveys-2.2.2/djf_surveys/admins/views.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)     2363 2024-03-15 06:25:03.000000 django-form-surveys-2.2.2/djf_surveys/app_settings.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      194 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/djf_surveys/apps.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      399 2024-03-15 06:25:03.000000 django-form-surveys-2.2.2/djf_surveys/context_processors.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)     7936 2024-03-18 07:07:22.000000 django-form-surveys-2.2.2/djf_surveys/forms.py
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-04-19 03:04:51.281215 django-form-surveys-2.2.2/djf_surveys/locale/
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-04-19 03:04:51.281001 django-form-surveys-2.2.2/djf_surveys/locale/en/
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-04-19 03:04:51.289064 django-form-surveys-2.2.2/djf_surveys/locale/en/LC_MESSAGES/
+-rw-r--r--   0 irfanpule   (501) staff       (20)     5632 2023-12-13 09:57:48.000000 django-form-surveys-2.2.2/djf_surveys/locale/en/LC_MESSAGES/django.mo
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-04-19 03:04:51.281141 django-form-surveys-2.2.2/djf_surveys/locale/fr/
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-04-19 03:04:51.289202 django-form-surveys-2.2.2/djf_surveys/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 irfanpule   (501) staff       (20)     6132 2023-12-13 09:57:48.000000 django-form-surveys-2.2.2/djf_surveys/locale/fr/LC_MESSAGES/django.mo
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-04-19 03:04:51.281272 django-form-surveys-2.2.2/djf_surveys/locale/id/
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-04-19 03:04:51.289453 django-form-surveys-2.2.2/djf_surveys/locale/id/LC_MESSAGES/
+-rw-r--r--   0 irfanpule   (501) staff       (20)     5906 2023-12-13 09:57:48.000000 django-form-surveys-2.2.2/djf_surveys/locale/id/LC_MESSAGES/django.mo
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-04-19 03:04:51.293621 django-form-surveys-2.2.2/djf_surveys/migrations/
+-rw-r--r--   0 irfanpule   (501) staff       (20)     3775 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/djf_surveys/migrations/0001_initial.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      860 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/djf_surveys/migrations/0002_auto_20220330_1033.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      553 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/djf_surveys/migrations/0003_auto_20220330_1036.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      850 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/djf_surveys/migrations/0004_auto_20220330_1112.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      377 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/djf_surveys/migrations/0005_auto_20220404_1518.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      451 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/djf_surveys/migrations/0006_survey_private_response.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      895 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/djf_surveys/migrations/0007_auto_20220525_1126.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      520 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/djf_surveys/migrations/0008_auto_20220721_0935.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      784 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/djf_surveys/migrations/0009_auto_20220803_0927.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)     8956 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/djf_surveys/migrations/0010_model_translation.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      662 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/djf_surveys/migrations/0011_alter_question_key.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      510 2024-02-27 06:22:45.000000 django-form-surveys-2.2.2/djf_surveys/migrations/0012_survey_notification_to.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      610 2024-03-15 06:25:03.000000 django-form-surveys-2.2.2/djf_surveys/migrations/0013_survey_success_page_content.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)        0 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/djf_surveys/migrations/__init__.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      611 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/djf_surveys/mixin.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)     7958 2024-03-18 07:07:22.000000 django-form-surveys-2.2.2/djf_surveys/models.py
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-04-19 03:04:51.281474 django-form-surveys-2.2.2/djf_surveys/static/
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-04-19 03:04:51.281679 django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-04-19 03:04:51.294669 django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/css/
+-rw-r--r--   0 irfanpule   (501) staff       (20)      389 2024-02-07 10:57:48.000000 django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/css/rating.css
+-rw-r--r--   0 irfanpule   (501) staff       (20)   356448 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/css/tailwindcss-3.3.1.js
+-rw-r--r--   0 irfanpule   (501) staff       (20)   455935 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/css/tailwindcss-plugin-3.3.1.js
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-04-19 03:04:51.296400 django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/images/
+-rw-r--r--   0 irfanpule   (501) staff       (20)     2962 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/images/star-border.png
+-rw-r--r--   0 irfanpule   (501) staff       (20)     2729 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/images/star-fill.png
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-04-19 03:04:51.281808 django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/te-starter/
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-04-19 03:04:51.296786 django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/te-starter/css/
+-rw-r--r--   0 irfanpule   (501) staff       (20)   198463 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/te-starter/css/tw-elements.min.css
+-rw-r--r--   0 irfanpule   (501) staff       (20)      121 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/te-starter/css/tw-elements.min.css.map
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-04-19 03:04:51.301955 django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/te-starter/js/
+-rw-r--r--   0 irfanpule   (501) staff       (20)   270873 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/te-starter/js/chart.es.js
+-rw-r--r--   0 irfanpule   (501) staff       (20)   783041 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/te-starter/js/chart.es.js.map
+-rw-r--r--   0 irfanpule   (501) staff       (20)    12217 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/te-starter/js/chartjs-plugin-datalabels.es.js
+-rw-r--r--   0 irfanpule   (501) staff       (20)    50339 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/te-starter/js/chartjs-plugin-datalabels.es.js.map
+-rw-r--r--   0 irfanpule   (501) staff       (20)   425275 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.es.min.js
+-rw-r--r--   0 irfanpule   (501) staff       (20)  1151819 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.es.min.js.map
+-rw-r--r--   0 irfanpule   (501) staff       (20)   539120 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.umd.min.js
+-rw-r--r--   0 irfanpule   (501) staff       (20)  1929935 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.umd.min.js.map
+-rw-r--r--   0 irfanpule   (501) staff       (20)     7569 2024-03-18 07:07:22.000000 django-form-surveys-2.2.2/djf_surveys/summary.py
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-04-19 03:04:51.281935 django-form-surveys-2.2.2/djf_surveys/templates/
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-04-19 03:04:51.306113 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-04-19 03:04:51.307957 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/admins/
+-rw-r--r--   0 irfanpule   (501) staff       (20)     1761 2024-02-06 15:05:01.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/admins/form.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)     7165 2024-02-06 15:05:01.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/admins/form_preview.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)     1132 2024-02-06 15:05:01.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/admins/master.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)      702 2024-02-06 15:05:01.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/admins/question_form.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)       45 2024-02-06 15:05:01.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/admins/question_form_v2.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)     1790 2024-02-06 15:05:01.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/admins/summary.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)     1490 2024-02-06 15:05:01.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/admins/survey_list.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)     4237 2024-02-06 15:05:01.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/answer_list.html
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-04-19 03:04:51.309145 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/buttons/
+-rw-r--r--   0 irfanpule   (501) staff       (20)      292 2024-02-06 15:05:01.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/buttons/add_button.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)      343 2024-02-06 15:05:01.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/buttons/delete_button.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)      309 2024-02-06 15:05:01.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/buttons/edit_button.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)      457 2024-02-06 15:05:01.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/buttons/share_button.html
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-04-19 03:04:51.312904 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/components/
+-rw-r--r--   0 irfanpule   (501) staff       (20)     1638 2024-02-06 15:05:01.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/components/alert.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)      326 2024-02-06 15:05:01.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/components/alert_js.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)     2967 2024-03-15 03:01:39.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/components/card_list_answer.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)     2872 2024-02-06 15:09:24.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/components/card_list_survey.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)      347 2024-02-06 15:05:01.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/components/empty_state.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)     3324 2024-02-06 15:05:01.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/components/header_nav.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)     3622 2024-02-06 15:05:01.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/components/modal_choice_field_type.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)     3073 2024-02-06 15:05:01.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/components/modal_delete.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)      777 2024-02-06 15:05:01.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/components/modal_delete_js.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)     3552 2024-02-06 15:05:01.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/components/pagination.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)      968 2024-02-06 15:05:01.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/components/search_form.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)      570 2024-02-06 15:05:01.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/components/section_welcome.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)      557 2024-02-06 15:05:01.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/components/share_link_button_js.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)      557 2024-02-06 15:05:01.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/components/star_border.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)        0 2024-02-06 15:05:01.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/components/star_fill.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)      889 2024-02-06 15:05:01.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/detail_result.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)     2014 2024-02-06 15:05:01.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/form.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)      792 2024-02-06 15:05:01.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/master.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)     1633 2024-03-15 06:25:03.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/success-page.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)     1189 2024-02-06 15:05:01.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/survey_list.html
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-04-19 03:04:51.314406 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/widgets/
+-rw-r--r--   0 irfanpule   (501) staff       (20)      247 2024-02-06 15:05:01.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/widgets/attrs_exclude_id.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)      538 2024-02-06 15:05:01.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/widgets/checkbox_option.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)      324 2024-02-06 16:37:27.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/widgets/datepicker.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)     5069 2024-02-06 15:05:01.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/widgets/inline_choices.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)      520 2024-02-06 15:05:01.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/widgets/radio_option.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)     1827 2024-04-19 03:03:50.000000 django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/widgets/star_rating.html
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2024-04-19 03:04:51.314731 django-form-surveys-2.2.2/djf_surveys/templatetags/
+-rw-r--r--   0 irfanpule   (501) staff       (20)        0 2023-12-13 04:15:23.000000 django-form-surveys-2.2.2/djf_surveys/templatetags/__init__.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      537 2024-02-06 15:05:15.000000 django-form-surveys-2.2.2/djf_surveys/templatetags/djf_survey_tags.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      469 2024-02-06 15:05:15.000000 django-form-surveys-2.2.2/djf_surveys/tests.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      887 2024-03-15 06:25:03.000000 django-form-surveys-2.2.2/djf_surveys/urls.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)     3750 2024-02-06 15:05:15.000000 django-form-surveys-2.2.2/djf_surveys/utils.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      696 2024-02-06 15:05:15.000000 django-form-surveys-2.2.2/djf_surveys/validators.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)    10253 2024-03-18 07:07:22.000000 django-form-surveys-2.2.2/djf_surveys/views.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)     1298 2024-02-06 15:05:15.000000 django-form-surveys-2.2.2/djf_surveys/widgets.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)       38 2024-04-19 03:04:51.315604 django-form-surveys-2.2.2/setup.cfg
+-rw-r--r--   0 irfanpule   (501) staff       (20)     3070 2024-02-28 09:21:30.000000 django-form-surveys-2.2.2/setup.py
```

### Comparing `django-form-surveys-2.2.1/LICENSE` & `django-form-surveys-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/PKG-INFO` & `django-form-surveys-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-form-surveys
-Version: 2.2.1
+Version: 2.2.2
 Summary: A simple Django app to conduct Web-based survey
 Home-page: https://irfanpule.github.io/django-form-surveys
 Author: irfanpule
 Author-email: irfan.pule2@gmail.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `django-form-surveys-2.2.1/README.md` & `django-form-surveys-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/django_form_surveys.egg-info/PKG-INFO` & `django-form-surveys-2.2.2/django_form_surveys.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-form-surveys
-Version: 2.2.1
+Version: 2.2.2
 Summary: A simple Django app to conduct Web-based survey
 Home-page: https://irfanpule.github.io/django-form-surveys
 Author: irfanpule
 Author-email: irfan.pule2@gmail.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `django-form-surveys-2.2.1/django_form_surveys.egg-info/SOURCES.txt` & `django-form-surveys-2.2.2/django_form_surveys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/admin.py` & `django-form-surveys-2.2.2/djf_surveys/admin.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/admins/urls.py` & `django-form-surveys-2.2.2/djf_surveys/admins/urls.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/admins/v2/forms.py` & `django-form-surveys-2.2.2/djf_surveys/admins/v2/forms.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/admins/v2/views.py` & `django-form-surveys-2.2.2/djf_surveys/admins/v2/views.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/admins/views.py` & `django-form-surveys-2.2.2/djf_surveys/admins/views.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/app_settings.py` & `django-form-surveys-2.2.2/djf_surveys/app_settings.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/forms.py` & `django-form-surveys-2.2.2/djf_surveys/forms.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/locale/en/LC_MESSAGES/django.mo` & `django-form-surveys-2.2.2/djf_surveys/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/locale/fr/LC_MESSAGES/django.mo` & `django-form-surveys-2.2.2/djf_surveys/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/locale/id/LC_MESSAGES/django.mo` & `django-form-surveys-2.2.2/djf_surveys/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/migrations/0001_initial.py` & `django-form-surveys-2.2.2/djf_surveys/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/migrations/0002_auto_20220330_1033.py` & `django-form-surveys-2.2.2/djf_surveys/migrations/0002_auto_20220330_1033.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/migrations/0003_auto_20220330_1036.py` & `django-form-surveys-2.2.2/djf_surveys/migrations/0003_auto_20220330_1036.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/migrations/0004_auto_20220330_1112.py` & `django-form-surveys-2.2.2/djf_surveys/migrations/0004_auto_20220330_1112.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/migrations/0007_auto_20220525_1126.py` & `django-form-surveys-2.2.2/djf_surveys/migrations/0007_auto_20220525_1126.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/migrations/0008_auto_20220721_0935.py` & `django-form-surveys-2.2.2/djf_surveys/migrations/0008_auto_20220721_0935.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/migrations/0009_auto_20220803_0927.py` & `django-form-surveys-2.2.2/djf_surveys/migrations/0009_auto_20220803_0927.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/migrations/0010_model_translation.py` & `django-form-surveys-2.2.2/djf_surveys/migrations/0010_model_translation.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/migrations/0011_alter_question_key.py` & `django-form-surveys-2.2.2/djf_surveys/migrations/0011_alter_question_key.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/migrations/0013_survey_success_page_content.py` & `django-form-surveys-2.2.2/djf_surveys/migrations/0013_survey_success_page_content.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/mixin.py` & `django-form-surveys-2.2.2/djf_surveys/mixin.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/models.py` & `django-form-surveys-2.2.2/djf_surveys/models.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/css/tailwindcss-3.3.1.js` & `django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/css/tailwindcss-3.3.1.js`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/css/tailwindcss-plugin-3.3.1.js` & `django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/css/tailwindcss-plugin-3.3.1.js`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/images/star-border.png` & `django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/images/star-border.png`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/images/star-fill.png` & `django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/images/star-fill.png`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/te-starter/css/tw-elements.min.css` & `django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/te-starter/css/tw-elements.min.css`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/te-starter/js/chart.es.js` & `django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/te-starter/js/chart.es.js`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/te-starter/js/chart.es.js.map` & `django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/te-starter/js/chart.es.js.map`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/te-starter/js/chartjs-plugin-datalabels.es.js` & `django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/te-starter/js/chartjs-plugin-datalabels.es.js`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/te-starter/js/chartjs-plugin-datalabels.es.js.map` & `django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/te-starter/js/chartjs-plugin-datalabels.es.js.map`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.es.min.js` & `django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.es.min.js`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.es.min.js.map` & `django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.es.min.js.map`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.umd.min.js` & `django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.umd.min.js`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.umd.min.js.map` & `django-form-surveys-2.2.2/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.umd.min.js.map`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/summary.py` & `django-form-surveys-2.2.2/djf_surveys/summary.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/admins/form.html` & `django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/admins/form.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/admins/form_preview.html` & `django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/admins/form_preview.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/admins/master.html` & `django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/admins/master.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/admins/question_form.html` & `django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/admins/question_form.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/admins/summary.html` & `django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/admins/summary.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/admins/survey_list.html` & `django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/admins/survey_list.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/answer_list.html` & `django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/answer_list.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/components/alert.html` & `django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/components/alert.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/components/card_list_answer.html` & `django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/components/card_list_answer.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/components/card_list_survey.html` & `django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/components/card_list_survey.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/components/header_nav.html` & `django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/components/header_nav.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/components/modal_choice_field_type.html` & `django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/components/modal_choice_field_type.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/components/modal_delete.html` & `django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/components/modal_delete.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/components/modal_delete_js.html` & `django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/components/modal_delete_js.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/components/pagination.html` & `django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/components/pagination.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/components/search_form.html` & `django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/components/search_form.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/components/section_welcome.html` & `django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/components/section_welcome.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/components/share_link_button_js.html` & `django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/components/share_link_button_js.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/components/star_border.html` & `django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/components/star_border.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/detail_result.html` & `django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/detail_result.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/form.html` & `django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/form.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/master.html` & `django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/master.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/success-page.html` & `django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/success-page.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/survey_list.html` & `django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/survey_list.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/widgets/checkbox_option.html` & `django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/widgets/checkbox_option.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/widgets/inline_choices.html` & `django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/widgets/inline_choices.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/widgets/radio_option.html` & `django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/widgets/radio_option.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/templates/djf_surveys/widgets/star_rating.html` & `django-form-surveys-2.2.2/djf_surveys/templates/djf_surveys/widgets/star_rating.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% load static djf_survey_tags %}
 
-<input type="{{ widget.type }}" name="{{ widget.name }}"{% if widget.value != None %} value="{{ widget.value }}"{% endif %}{% include "django/forms/widgets/attrs.html" %}>
+<input type="{{ widget.type }}" name="{{ widget.name }}"{% if widget.value != None %} value="{{ widget.value }}" {% else %} value="0" {% endif %}{% include "django/forms/widgets/attrs.html" %}>
 {% if widget.value != None %}
     {% create_star widget.value widget.attrs.id widget.num_ratings %}
 {% else %}
     {% create_star "0" widget.attrs.id widget.num_ratings %}
 {% endif %}
 
 <script>
```

#### html2text {}

```diff
@@ -1,5 +1,5 @@
 {% load static djf_survey_tags %}
-% if widget.value != None %} value="{{ widget.value }}"{% endif %}{% include
-"django/forms/widgets/attrs.html" %}> {% if widget.value != None %} {%
-create_star widget.value widget.attrs.id widget.num_ratings %} {% else %} {%
-create_star "0" widget.attrs.id widget.num_ratings %} {% endif %}
+% if widget.value != None %} value="{{ widget.value }}" {% else %} value="0" {%
+endif %}{% include "django/forms/widgets/attrs.html" %}> {% if widget.value !=
+None %} {% create_star widget.value widget.attrs.id widget.num_ratings %} {%
+else %} {% create_star "0" widget.attrs.id widget.num_ratings %} {% endif %}
```

### Comparing `django-form-surveys-2.2.1/djf_surveys/templatetags/djf_survey_tags.py` & `django-form-surveys-2.2.2/djf_surveys/templatetags/djf_survey_tags.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/urls.py` & `django-form-surveys-2.2.2/djf_surveys/urls.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/utils.py` & `django-form-surveys-2.2.2/djf_surveys/utils.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/validators.py` & `django-form-surveys-2.2.2/djf_surveys/validators.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/views.py` & `django-form-surveys-2.2.2/djf_surveys/views.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/djf_surveys/widgets.py` & `django-form-surveys-2.2.2/djf_surveys/widgets.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.2.1/setup.py` & `django-form-surveys-2.2.2/setup.py`

 * *Files identical despite different names*

