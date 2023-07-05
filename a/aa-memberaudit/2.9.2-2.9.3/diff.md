# Comparing `tmp/aa_memberaudit-2.9.2.tar.gz` & `tmp/aa_memberaudit-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_memberaudit-2.9.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aa_memberaudit-2.9.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aa_memberaudit-2.9.2.tar` & `aa_memberaudit-2.9.3.tar`

### file list

```diff
@@ -1,241 +1,239 @@
--rw-r--r--   0        0        0     1070 2023-06-23 12:09:49.027656 aa_memberaudit-2.9.2/LICENSE
--rw-r--r--   0        0        0     5782 2023-06-23 12:09:49.027656 aa_memberaudit-2.9.2/README.md
--rw-r--r--   0        0        0      240 2023-06-30 12:57:32.000784 aa_memberaudit-2.9.2/memberaudit/__init__.py
--rw-r--r--   0        0        0    24333 2023-06-23 12:09:49.035656 aa_memberaudit-2.9.2/memberaudit/admin.py
--rw-r--r--   0        0        0     4548 2023-06-23 12:09:49.035656 aa_memberaudit-2.9.2/memberaudit/app_settings.py
--rw-r--r--   0        0        0      407 2023-06-23 12:09:49.035656 aa_memberaudit-2.9.2/memberaudit/apps.py
--rw-r--r--   0        0        0     1251 2023-06-23 12:09:49.035656 aa_memberaudit-2.9.2/memberaudit/auth_hooks.py
--rw-r--r--   0        0        0     1271 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/checks.py
--rw-r--r--   0        0        0     1704 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/constants.py
--rw-r--r--   0        0        0        0 2023-06-30 13:31:50.428699 aa_memberaudit-2.9.2/memberaudit/core/__init__.py
--rw-r--r--   0        0        0    11526 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/core/data_exporters.py
--rw-r--r--   0        0        0    19456 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/core/eft_parser.py
--rw-r--r--   0        0        0     5563 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/core/fittings.py
--rw-r--r--   0        0        0     2244 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/core/skill_plans.py
--rw-r--r--   0        0        0     5362 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/core/skills.py
--rw-r--r--   0        0        0     3159 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/core/xml_converter.py
--rw-r--r--   0        0        0     2430 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/decorators.py
--rw-r--r--   0        0        0     3740 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/forms.py
--rw-r--r--   0        0        0     1820 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/helpers.py
--rw-r--r--   0        0        0      384 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43105 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    43046 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/locale/django.pot
--rw-r--r--   0        0        0    43093 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      380 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43093 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      450 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43171 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      438 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43159 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43100 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      391 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43112 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    26859 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    54952 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      609 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43330 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      373 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43086 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      102 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/management/commands/__init__.py
--rw-r--r--   0        0        0     1443 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/management/commands/memberaudit_data_export.py
--rw-r--r--   0        0        0     1374 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/management/commands/memberaudit_load_eve.py
--rw-r--r--   0        0        0     3859 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/management/commands/memberaudit_reset_characters.py
--rw-r--r--   0        0        0      740 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/management/commands/memberaudit_stats.py
--rw-r--r--   0        0        0     1941 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/management/commands/memberaudit_update_characters.py
--rw-r--r--   0        0        0        0 2023-06-30 13:31:50.428699 aa_memberaudit-2.9.2/memberaudit/managers/__init__.py
--rw-r--r--   0        0        0    13017 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/managers/character.py
--rw-r--r--   0        0        0    26850 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/managers/character_sections_1.py
--rw-r--r--   0        0        0    29910 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/managers/character_sections_2.py
--rw-r--r--   0        0        0    25043 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/managers/character_sections_3.py
--rw-r--r--   0        0        0    24472 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/managers/general.py
--rw-r--r--   0        0        0    65995 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/migrations/0001_initial_new.py
--rw-r--r--   0        0        0     3444 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/migrations/0002_add_mining_ledger.py
--rw-r--r--   0        0        0     1478 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/migrations/0003_add_notify_permission.py
--rw-r--r--   0        0        0      513 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/migrations/0004_character_is_disabled.py
--rw-r--r--   0        0        0     3819 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/migrations/0005_add_fw_stats.py
--rw-r--r--   0        0        0     5969 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/migrations/0006_add_localizations.py
--rw-r--r--   0        0        0     2129 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/migrations/0007_add_localization_2.py
--rw-r--r--   0        0        0     2727 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/migrations/0008_improve_skill_sets.py
--rw-r--r--   0        0        0     3274 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/migrations/0009_add_planetary_industry.py
--rw-r--r--   0        0        0        0 2023-06-30 13:31:50.428699 aa_memberaudit-2.9.2/memberaudit/migrations/__init__.py
--rw-r--r--   0        0        0     1117 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/models/__init__.py
--rw-r--r--   0        0        0    15243 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/models/character_sections_1.py
--rw-r--r--   0        0        0    13506 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/models/character_sections_2.py
--rw-r--r--   0        0        0    13923 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/models/character_sections_3.py
--rw-r--r--   0        0        0    26983 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/models/characters.py
--rw-r--r--   0        0        0      108 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/models/constants.py
--rw-r--r--   0        0        0    17213 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/models/general.py
--rw-r--r--   0        0        0      299 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/providers.py
--rw-r--r--   0        0        0      542 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/signals.py
--rw-r--r--   0        0        0      191 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/admin.css
--rw-r--r--   0        0        0      174 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/character_finder.css
--rw-r--r--   0        0        0     5736 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/character_viewer.css
--rw-r--r--   0        0        0     2540 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/character_viewer.min.css
--rw-r--r--   0        0        0       94 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/data_export.css
--rw-r--r--   0        0        0     1538 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/global.css
--rw-r--r--   0        0        0      646 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/global.min.css
--rw-r--r--   0        0        0     4331 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/launcher.css
--rw-r--r--   0        0        0     2765 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/launcher.min.css
--rw-r--r--   0        0        0     1363 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/memberaudit.css
--rw-r--r--   0        0        0      617 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/memberaudit.min.css
--rw-r--r--   0        0        0      611 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/reports.css
--rw-r--r--   0        0        0    43262 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif
--rw-r--r--   0        0        0    43381 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif
--rw-r--r--   0        0        0     1862 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/charisma.png
--rw-r--r--   0        0        0      694 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/eve-prism.png
--rw-r--r--   0        0        0      220 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/evelogo.png
--rw-r--r--   0        0        0      595 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/evesearch.png
--rw-r--r--   0        0        0     1966 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/intelligence.png
--rw-r--r--   0        0        0     1809 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/memory.png
--rw-r--r--   0        0        0     1803 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/perception.png
--rw-r--r--   0        0        0     1782 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/willpower.png
--rw-r--r--   0        0        0      259 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/zkillboard.png
--rw-r--r--   0        0        0     5573 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js
--rw-r--r--   0        0        0     3908 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js
--rw-r--r--   0        0        0     2529 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js
--rw-r--r--   0        0        0      384 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.bootstrap.min.css
--rw-r--r--   0        0        0      384 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.dataTables.min.css
--rw-r--r--   0        0        0    69950 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/vendor/moment/moment.min.js
--rw-r--r--   0        0        0   881821 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/swagger.json
--rw-r--r--   0        0        0    40513 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/tasks.py
--rw-r--r--   0        0        0      687 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html
--rw-r--r--   0        0        0      488 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/admin/memberaudit/skillset/change_list.html
--rw-r--r--   0        0        0      848 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/admin/memberaudit/skillset/import_skills.html
--rw-r--r--   0        0        0      367 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/base.html
--rw-r--r--   0        0        0     4801 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/character_finder.html
--rw-r--r--   0        0        0    29413 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/character_viewer.html
--rw-r--r--   0        0        0     2932 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/data_export.html
--rw-r--r--   0        0        0     8515 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/launcher.html
--rw-r--r--   0        0        0     1238 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html
--rw-r--r--   0        0        0     4307 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html
--rw-r--r--   0        0        0     1713 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html
--rw-r--r--   0        0        0     1246 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/contract.html
--rw-r--r--   0        0        0     8075 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html
--rw-r--r--   0        0        0      658 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html
--rw-r--r--   0        0        0     1375 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/mail.html
--rw-r--r--   0        0        0      382 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/mail_content.html
--rw-r--r--   0        0        0     3880 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html
--rw-r--r--   0        0        0     9005 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/overview.html
--rw-r--r--   0        0        0     1451 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html
--rw-r--r--   0        0        0      637 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html
--rw-r--r--   0        0        0     1256 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html
--rw-r--r--   0        0        0      560 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes.html
--rw-r--r--   0        0        0     2604 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html
--rw-r--r--   0        0        0      314 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_bio.html
--rw-r--r--   0        0        0      848 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html
--rw-r--r--   0        0        0      960 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html
--rw-r--r--   0        0        0      582 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html
--rw-r--r--   0        0        0      894 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html
--rw-r--r--   0        0        0      549 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats.html
--rw-r--r--   0        0        0     2786 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html
--rw-r--r--   0        0        0      563 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/implants.html
--rw-r--r--   0        0        0      721 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html
--rw-r--r--   0        0        0      148 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/last_updated.html
--rw-r--r--   0        0        0      611 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html
--rw-r--r--   0        0        0     2878 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html
--rw-r--r--   0        0        0      779 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html
--rw-r--r--   0        0        0      885 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/planets.html
--rw-r--r--   0        0        0      669 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html
--rw-r--r--   0        0        0      882 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html
--rw-r--r--   0        0        0      592 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html
--rw-r--r--   0        0        0      907 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html
--rw-r--r--   0        0        0      916 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html
--rw-r--r--   0        0        0     3941 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html
--rw-r--r--   0        0        0     2674 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/menu.html
--rw-r--r--   0        0        0      292 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/reports/tabs/_compliance_color_code.html
--rw-r--r--   0        0        0      684 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html
--rw-r--r--   0        0        0      760 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html
--rw-r--r--   0        0        0      775 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html
--rw-r--r--   0        0        0      691 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html
--rw-r--r--   0        0        0      709 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/solar_system.html
--rw-r--r--   0        0        0     9420 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/reports.html
--rw-r--r--   0        0        0        0 2023-06-30 13:31:50.436699 aa_memberaudit-2.9.2/memberaudit/templatetags/__init__.py
--rw-r--r--   0        0        0      355 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templatetags/memberaudit.py
--rw-r--r--   0        0        0        0 2023-06-30 13:31:50.436699 aa_memberaudit-2.9.2/memberaudit/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 13:31:50.436699 aa_memberaudit-2.9.2/memberaudit/tests/core/__init__.py
--rw-r--r--   0        0        0     6350 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/tests/core/test_core_xml_converter.py
--rw-r--r--   0        0        0    12725 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/tests/core/test_data_exporters.py
--rw-r--r--   0        0        0    22366 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/tests/core/test_eft_parser.py
--rw-r--r--   0        0        0     6371 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/tests/core/test_fittings.py
--rw-r--r--   0        0        0     4082 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/tests/core/test_skill_plans.py
--rw-r--r--   0        0        0     2458 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/tests/core/test_skills.py
--rw-r--r--   0        0        0        0 2023-06-30 13:31:50.436699 aa_memberaudit-2.9.2/memberaudit/tests/managers/__init__.py
--rw-r--r--   0        0        0    18357 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/tests/managers/test_character.py
--rw-r--r--   0        0        0    30687 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/tests/managers/test_character_sections_1.py
--rw-r--r--   0        0        0    37493 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/tests/managers/test_character_sections_2.py
--rw-r--r--   0        0        0    24751 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/tests/managers/test_character_sections_3.py
--rw-r--r--   0        0        0    46675 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/managers/test_general.py
--rw-r--r--   0        0        0        0 2023-06-30 13:31:50.436699 aa_memberaudit-2.9.2/memberaudit/tests/models/__init__.py
--rw-r--r--   0        0        0     2963 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/models/test_character_sections.py
--rw-r--r--   0        0        0    36073 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/models/test_characters_1.py
--rw-r--r--   0        0        0    23158 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/models/test_characters_2.py
--rw-r--r--   0        0        0    10969 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/models/test_general.py
--rw-r--r--   0        0        0    15428 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/test_admin.py
--rw-r--r--   0        0        0     1807 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/test_auth_hooks.py
--rw-r--r--   0        0        0     1314 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/test_checks.py
--rw-r--r--   0        0        0     3487 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/test_commands.py
--rw-r--r--   0        0        0     4119 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/test_decorators.py
--rw-r--r--   0        0        0      900 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/test_factories.py
--rw-r--r--   0        0        0     3516 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/test_forms.py
--rw-r--r--   0        0        0     1476 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/test_helpers.py
--rw-r--r--   0        0        0    15643 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/test_integration.py
--rw-r--r--   0        0        0     1215 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/test_signals.py
--rw-r--r--   0        0        0    38340 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/test_tasks.py
--rw-r--r--   0        0        0      968 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/test_templatetags.py
--rw-r--r--   0        0        0     3822 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/test_utils.py
--rw-r--r--   0        0        0      267 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/testdata/__init__.py
--rw-r--r--   0        0        0     4432 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/testdata/create_eveuniverse.py
--rw-r--r--   0        0        0     4350 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/testdata/entities.json
--rw-r--r--   0        0        0     5298 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/testdata/esi_client_stub.py
--rw-r--r--   0        0        0    41017 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/testdata/esi_testdata.json
--rw-r--r--   0        0        0  1225856 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/eveuniverse.json
--rw-r--r--   0        0        0    13508 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/factories.py
--rw-r--r--   0        0        0      799 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_archon.txt
--rw-r--r--   0        0        0      889 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_archon_max.txt
--rw-r--r--   0        0        0      231 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_empty.txt
--rw-r--r--   0        0        0      503 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_eve_celestis_no_high_slots.txt
--rw-r--r--   0        0        0      193 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_eve_tristan_3.txt
--rw-r--r--   0        0        0      377 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_eve_tristian.txt
--rw-r--r--   0        0        0      293 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_eve_tristian_2.txt
--rw-r--r--   0        0        0       96 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_eve_tristian_empty.txt
--rw-r--r--   0        0        0      583 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_svipul.txt
--rw-r--r--   0        0        0      432 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_svipul_2.txt
--rw-r--r--   0        0        0      700 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_tengu.txt
--rw-r--r--   0        0        0      459 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_tristan.txt
--rw-r--r--   0        0        0      332 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_tristan_missing_rigs.txt
--rw-r--r--   0        0        0      410 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_tristan_no_title.txt
--rw-r--r--   0        0        0      460 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_tristan_unknown_types.txt
--rw-r--r--   0        0        0      455 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_unknown_ship_type.txt
--rw-r--r--   0        0        0     4268 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/generate_character.py
--rw-r--r--   0        0        0     3859 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/generate_doctrines.py
--rw-r--r--   0        0        0     3680 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/load_entities.py
--rw-r--r--   0        0        0      478 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/load_eveuniverse.py
--rw-r--r--   0        0        0     1188 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/load_locations.py
--rw-r--r--   0        0        0     1097 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/pilot_esi_error_handling.py
--rw-r--r--   0        0        0      838 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/profiler_toolbox.py
--rw-r--r--   0        0        0     5744 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/utils.py
--rw-r--r--   0        0        0        0 2023-06-30 13:31:50.440699 aa_memberaudit-2.9.2/memberaudit/tests/views/__init__.py
--rw-r--r--   0        0        0     9299 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/views/test_admin.py
--rw-r--r--   0        0        0     7089 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/views/test_character_finder.py
--rw-r--r--   0        0        0    32680 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/views/test_character_viewer_1.py
--rw-r--r--   0        0        0    24561 2023-06-23 12:09:49.067655 aa_memberaudit-2.9.2/memberaudit/tests/views/test_character_viewer_2.py
--rw-r--r--   0        0        0    14594 2023-06-23 12:09:49.067655 aa_memberaudit-2.9.2/memberaudit/tests/views/test_characters.py
--rw-r--r--   0        0        0     4101 2023-06-23 12:09:49.067655 aa_memberaudit-2.9.2/memberaudit/tests/views/test_data_export.py
--rw-r--r--   0        0        0    16249 2023-06-23 12:09:49.067655 aa_memberaudit-2.9.2/memberaudit/tests/views/test_reports.py
--rw-r--r--   0        0        0      710 2023-06-23 12:09:49.067655 aa_memberaudit-2.9.2/memberaudit/tools/clear_celery_once_locks.py
--rw-r--r--   0        0        0     3051 2023-06-23 12:09:49.067655 aa_memberaudit-2.9.2/memberaudit/tools/drop_tables.sql
--rw-r--r--   0        0        0      329 2023-06-23 12:09:49.067655 aa_memberaudit-2.9.2/memberaudit/tools/total_size.sql
--rw-r--r--   0        0        0     7242 2023-06-23 12:09:49.067655 aa_memberaudit-2.9.2/memberaudit/urls.py
--rw-r--r--   0        0        0     2367 2023-06-23 12:09:49.067655 aa_memberaudit-2.9.2/memberaudit/utils.py
--rw-r--r--   0        0        0        0 2023-06-30 13:31:50.440699 aa_memberaudit-2.9.2/memberaudit/views/__init__.py
--rw-r--r--   0        0        0     1539 2023-06-23 12:09:49.067655 aa_memberaudit-2.9.2/memberaudit/views/_common.py
--rw-r--r--   0        0        0     3510 2023-06-23 12:09:49.067655 aa_memberaudit-2.9.2/memberaudit/views/admin.py
--rw-r--r--   0        0        0    12637 2023-06-23 12:09:49.067655 aa_memberaudit-2.9.2/memberaudit/views/character_finder.py
--rw-r--r--   0        0        0    24043 2023-06-23 12:09:49.067655 aa_memberaudit-2.9.2/memberaudit/views/character_viewer_1.py
--rw-r--r--   0        0        0    24147 2023-06-30 12:57:32.000784 aa_memberaudit-2.9.2/memberaudit/views/character_viewer_2.py
--rw-r--r--   0        0        0     8029 2023-06-23 12:09:49.067655 aa_memberaudit-2.9.2/memberaudit/views/characters.py
--rw-r--r--   0        0        0     2222 2023-06-23 12:09:49.067655 aa_memberaudit-2.9.2/memberaudit/views/data_export.py
--rw-r--r--   0        0        0    13139 2023-06-23 12:09:49.067655 aa_memberaudit-2.9.2/memberaudit/views/reports.py
--rw-r--r--   0        0        0     2285 2023-06-30 12:57:32.000784 aa_memberaudit-2.9.2/pyproject.toml
--rw-r--r--   0        0        0     7374 1970-01-01 00:00:00.000000 aa_memberaudit-2.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-05 11:03:39.217293 aa_memberaudit-2.9.3/LICENSE
+-rw-r--r--   0        0        0     5782 2023-07-05 11:03:39.217293 aa_memberaudit-2.9.3/README.md
+-rw-r--r--   0        0        0      240 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/__init__.py
+-rw-r--r--   0        0        0    24112 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/admin.py
+-rw-r--r--   0        0        0     4548 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/app_settings.py
+-rw-r--r--   0        0        0      407 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/apps.py
+-rw-r--r--   0        0        0     1251 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/auth_hooks.py
+-rw-r--r--   0        0        0     1271 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/checks.py
+-rw-r--r--   0        0        0     1812 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/constants.py
+-rw-r--r--   0        0        0        0 2023-07-05 11:09:35.048957 aa_memberaudit-2.9.3/memberaudit/core/__init__.py
+-rw-r--r--   0        0        0    11526 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/core/data_exporters.py
+-rw-r--r--   0        0        0    19456 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/core/eft_parser.py
+-rw-r--r--   0        0        0     5563 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/core/fittings.py
+-rw-r--r--   0        0        0     2244 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/core/skill_plans.py
+-rw-r--r--   0        0        0     5362 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/core/skills.py
+-rw-r--r--   0        0        0     3159 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/core/xml_converter.py
+-rw-r--r--   0        0        0     3166 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/decorators.py
+-rw-r--r--   0        0        0     3740 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/forms.py
+-rw-r--r--   0        0        0     1820 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/helpers.py
+-rw-r--r--   0        0        0      384 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    43105 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.3/memberaudit/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    43046 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.3/memberaudit/locale/django.pot
+-rw-r--r--   0        0        0    43093 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.3/memberaudit/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      380 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.3/memberaudit/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    43093 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.3/memberaudit/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      450 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.3/memberaudit/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    43171 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.3/memberaudit/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      438 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.3/memberaudit/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    43159 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.3/memberaudit/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.3/memberaudit/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    43100 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.3/memberaudit/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      391 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.3/memberaudit/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    43112 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.3/memberaudit/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    26859 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.3/memberaudit/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    54952 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.3/memberaudit/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      609 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.3/memberaudit/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    43330 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.3/memberaudit/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      373 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.3/memberaudit/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    43086 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.3/memberaudit/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      102 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.3/memberaudit/management/commands/__init__.py
+-rw-r--r--   0        0        0     1443 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.3/memberaudit/management/commands/memberaudit_data_export.py
+-rw-r--r--   0        0        0     1374 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.3/memberaudit/management/commands/memberaudit_load_eve.py
+-rw-r--r--   0        0        0     3859 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.3/memberaudit/management/commands/memberaudit_reset_characters.py
+-rw-r--r--   0        0        0      740 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.3/memberaudit/management/commands/memberaudit_stats.py
+-rw-r--r--   0        0        0     1941 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.3/memberaudit/management/commands/memberaudit_update_characters.py
+-rw-r--r--   0        0        0        0 2023-07-05 11:09:35.052957 aa_memberaudit-2.9.3/memberaudit/managers/__init__.py
+-rw-r--r--   0        0        0    13017 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.3/memberaudit/managers/character.py
+-rw-r--r--   0        0        0    26850 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.3/memberaudit/managers/character_sections_1.py
+-rw-r--r--   0        0        0    29910 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.3/memberaudit/managers/character_sections_2.py
+-rw-r--r--   0        0        0    25043 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/managers/character_sections_3.py
+-rw-r--r--   0        0        0    24472 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/managers/general.py
+-rw-r--r--   0        0        0    65995 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/migrations/0001_initial_new.py
+-rw-r--r--   0        0        0     3444 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/migrations/0002_add_mining_ledger.py
+-rw-r--r--   0        0        0     1478 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/migrations/0003_add_notify_permission.py
+-rw-r--r--   0        0        0      513 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/migrations/0004_character_is_disabled.py
+-rw-r--r--   0        0        0     3819 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/migrations/0005_add_fw_stats.py
+-rw-r--r--   0        0        0     5969 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/migrations/0006_add_localizations.py
+-rw-r--r--   0        0        0     2129 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/migrations/0007_add_localization_2.py
+-rw-r--r--   0        0        0     2727 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/migrations/0008_improve_skill_sets.py
+-rw-r--r--   0        0        0     3274 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/migrations/0009_add_planetary_industry.py
+-rw-r--r--   0        0        0        0 2023-07-05 11:09:35.052957 aa_memberaudit-2.9.3/memberaudit/migrations/__init__.py
+-rw-r--r--   0        0        0     1117 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/models/__init__.py
+-rw-r--r--   0        0        0    15243 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/models/character_sections_1.py
+-rw-r--r--   0        0        0    13506 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/models/character_sections_2.py
+-rw-r--r--   0        0        0    13923 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/models/character_sections_3.py
+-rw-r--r--   0        0        0    26983 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/models/characters.py
+-rw-r--r--   0        0        0      108 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/models/constants.py
+-rw-r--r--   0        0        0    17213 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/models/general.py
+-rw-r--r--   0        0        0      196 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/providers.py
+-rw-r--r--   0        0        0      542 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/signals.py
+-rw-r--r--   0        0        0      191 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/admin.css
+-rw-r--r--   0        0        0      174 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/character_finder.css
+-rw-r--r--   0        0        0     5820 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/character_viewer.css
+-rw-r--r--   0        0        0       94 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/data_export.css
+-rw-r--r--   0        0        0     1538 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/global.css
+-rw-r--r--   0        0        0      646 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/global.min.css
+-rw-r--r--   0        0        0     4331 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/launcher.css
+-rw-r--r--   0        0        0     2765 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/launcher.min.css
+-rw-r--r--   0        0        0     1363 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/memberaudit.css
+-rw-r--r--   0        0        0      617 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/memberaudit.min.css
+-rw-r--r--   0        0        0      611 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/reports.css
+-rw-r--r--   0        0        0    43262 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif
+-rw-r--r--   0        0        0    43381 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif
+-rw-r--r--   0        0        0     1862 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/charisma.png
+-rw-r--r--   0        0        0      694 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/eve-prism.png
+-rw-r--r--   0        0        0      220 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/evelogo.png
+-rw-r--r--   0        0        0      595 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/evesearch.png
+-rw-r--r--   0        0        0     1966 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/intelligence.png
+-rw-r--r--   0        0        0     1809 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/memory.png
+-rw-r--r--   0        0        0     1803 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/perception.png
+-rw-r--r--   0        0        0     1782 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/willpower.png
+-rw-r--r--   0        0        0      259 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/zkillboard.png
+-rw-r--r--   0        0        0     5573 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js
+-rw-r--r--   0        0        0     3908 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js
+-rw-r--r--   0        0        0     2529 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js
+-rw-r--r--   0        0        0      384 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.bootstrap.min.css
+-rw-r--r--   0        0        0      384 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.dataTables.min.css
+-rw-r--r--   0        0        0    69950 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/vendor/moment/moment.min.js
+-rw-r--r--   0        0        0    40015 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/tasks.py
+-rw-r--r--   0        0        0      687 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html
+-rw-r--r--   0        0        0      488 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/templates/admin/memberaudit/skillset/change_list.html
+-rw-r--r--   0        0        0      848 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/templates/admin/memberaudit/skillset/import_skills.html
+-rw-r--r--   0        0        0      367 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/base.html
+-rw-r--r--   0        0        0     4801 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/character_finder.html
+-rw-r--r--   0        0        0    29413 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/character_viewer.html
+-rw-r--r--   0        0        0     2932 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/data_export.html
+-rw-r--r--   0        0        0     8515 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/launcher.html
+-rw-r--r--   0        0        0     1238 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html
+-rw-r--r--   0        0        0     4307 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html
+-rw-r--r--   0        0        0     1713 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html
+-rw-r--r--   0        0        0     1246 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/contract.html
+-rw-r--r--   0        0        0     8075 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html
+-rw-r--r--   0        0        0      658 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html
+-rw-r--r--   0        0        0     1375 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/mail.html
+-rw-r--r--   0        0        0      382 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/mail_content.html
+-rw-r--r--   0        0        0     3880 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html
+-rw-r--r--   0        0        0     9005 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/overview.html
+-rw-r--r--   0        0        0     1451 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html
+-rw-r--r--   0        0        0      637 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html
+-rw-r--r--   0        0        0     1256 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html
+-rw-r--r--   0        0        0      560 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes.html
+-rw-r--r--   0        0        0     2604 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html
+-rw-r--r--   0        0        0      314 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_bio.html
+-rw-r--r--   0        0        0      848 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html
+-rw-r--r--   0        0        0      960 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html
+-rw-r--r--   0        0        0      582 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html
+-rw-r--r--   0        0        0      894 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html
+-rw-r--r--   0        0        0      549 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats.html
+-rw-r--r--   0        0        0     2786 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html
+-rw-r--r--   0        0        0      563 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/implants.html
+-rw-r--r--   0        0        0      721 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html
+-rw-r--r--   0        0        0      148 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/last_updated.html
+-rw-r--r--   0        0        0      611 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html
+-rw-r--r--   0        0        0     2878 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html
+-rw-r--r--   0        0        0      779 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html
+-rw-r--r--   0        0        0      885 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/planets.html
+-rw-r--r--   0        0        0      669 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html
+-rw-r--r--   0        0        0      882 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html
+-rw-r--r--   0        0        0      592 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html
+-rw-r--r--   0        0        0      907 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html
+-rw-r--r--   0        0        0      916 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html
+-rw-r--r--   0        0        0     3941 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html
+-rw-r--r--   0        0        0     2674 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/menu.html
+-rw-r--r--   0        0        0      292 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/reports/tabs/_compliance_color_code.html
+-rw-r--r--   0        0        0      684 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html
+-rw-r--r--   0        0        0      760 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html
+-rw-r--r--   0        0        0      775 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html
+-rw-r--r--   0        0        0      691 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html
+-rw-r--r--   0        0        0      709 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/solar_system.html
+-rw-r--r--   0        0        0     9420 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/reports.html
+-rw-r--r--   0        0        0        0 2023-07-05 11:09:35.060958 aa_memberaudit-2.9.3/memberaudit/templatetags/__init__.py
+-rw-r--r--   0        0        0      355 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.3/memberaudit/templatetags/memberaudit.py
+-rw-r--r--   0        0        0        0 2023-07-05 11:09:35.060958 aa_memberaudit-2.9.3/memberaudit/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 11:09:35.060958 aa_memberaudit-2.9.3/memberaudit/tests/core/__init__.py
+-rw-r--r--   0        0        0     6350 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.3/memberaudit/tests/core/test_core_xml_converter.py
+-rw-r--r--   0        0        0    12725 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.3/memberaudit/tests/core/test_data_exporters.py
+-rw-r--r--   0        0        0    22366 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.3/memberaudit/tests/core/test_eft_parser.py
+-rw-r--r--   0        0        0     6371 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.3/memberaudit/tests/core/test_fittings.py
+-rw-r--r--   0        0        0     4082 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.3/memberaudit/tests/core/test_skill_plans.py
+-rw-r--r--   0        0        0     2458 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.3/memberaudit/tests/core/test_skills.py
+-rw-r--r--   0        0        0        0 2023-07-05 11:09:35.060958 aa_memberaudit-2.9.3/memberaudit/tests/managers/__init__.py
+-rw-r--r--   0        0        0    18357 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.3/memberaudit/tests/managers/test_character.py
+-rw-r--r--   0        0        0    30687 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.3/memberaudit/tests/managers/test_character_sections_1.py
+-rw-r--r--   0        0        0    37493 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.3/memberaudit/tests/managers/test_character_sections_2.py
+-rw-r--r--   0        0        0    24751 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.3/memberaudit/tests/managers/test_character_sections_3.py
+-rw-r--r--   0        0        0    46675 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.3/memberaudit/tests/managers/test_general.py
+-rw-r--r--   0        0        0        0 2023-07-05 11:09:35.060958 aa_memberaudit-2.9.3/memberaudit/tests/models/__init__.py
+-rw-r--r--   0        0        0     2963 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/models/test_character_sections.py
+-rw-r--r--   0        0        0    36073 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/models/test_characters_1.py
+-rw-r--r--   0        0        0    23158 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/models/test_characters_2.py
+-rw-r--r--   0        0        0    10969 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/models/test_general.py
+-rw-r--r--   0        0        0    15428 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/test_admin.py
+-rw-r--r--   0        0        0     1807 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0     1314 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/test_checks.py
+-rw-r--r--   0        0        0     3487 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/test_commands.py
+-rw-r--r--   0        0        0     5266 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/test_decorators.py
+-rw-r--r--   0        0        0      900 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/test_factories.py
+-rw-r--r--   0        0        0     3516 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/test_forms.py
+-rw-r--r--   0        0        0     1476 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/test_helpers.py
+-rw-r--r--   0        0        0    15465 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/test_integration.py
+-rw-r--r--   0        0        0     1215 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/test_signals.py
+-rw-r--r--   0        0        0    36377 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/test_tasks.py
+-rw-r--r--   0        0        0      968 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/test_templatetags.py
+-rw-r--r--   0        0        0     3822 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/test_utils.py
+-rw-r--r--   0        0        0      267 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/testdata/__init__.py
+-rw-r--r--   0        0        0     4432 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/testdata/create_eveuniverse.py
+-rw-r--r--   0        0        0     4350 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/testdata/entities.json
+-rw-r--r--   0        0        0     5298 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/testdata/esi_client_stub.py
+-rw-r--r--   0        0        0    41017 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/testdata/esi_testdata.json
+-rw-r--r--   0        0        0  1225856 2023-07-05 11:03:39.269295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/eveuniverse.json
+-rw-r--r--   0        0        0    13508 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/factories.py
+-rw-r--r--   0        0        0      799 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_archon.txt
+-rw-r--r--   0        0        0      889 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_archon_max.txt
+-rw-r--r--   0        0        0      231 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_empty.txt
+-rw-r--r--   0        0        0      503 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_eve_celestis_no_high_slots.txt
+-rw-r--r--   0        0        0      193 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_eve_tristan_3.txt
+-rw-r--r--   0        0        0      377 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_eve_tristian.txt
+-rw-r--r--   0        0        0      293 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_eve_tristian_2.txt
+-rw-r--r--   0        0        0       96 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_eve_tristian_empty.txt
+-rw-r--r--   0        0        0      583 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_svipul.txt
+-rw-r--r--   0        0        0      432 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_svipul_2.txt
+-rw-r--r--   0        0        0      700 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_tengu.txt
+-rw-r--r--   0        0        0      459 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_tristan.txt
+-rw-r--r--   0        0        0      332 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_tristan_missing_rigs.txt
+-rw-r--r--   0        0        0      410 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_tristan_no_title.txt
+-rw-r--r--   0        0        0      460 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_tristan_unknown_types.txt
+-rw-r--r--   0        0        0      455 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_unknown_ship_type.txt
+-rw-r--r--   0        0        0     4268 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/generate_character.py
+-rw-r--r--   0        0        0     3859 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/generate_doctrines.py
+-rw-r--r--   0        0        0     3680 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/load_entities.py
+-rw-r--r--   0        0        0      478 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/load_eveuniverse.py
+-rw-r--r--   0        0        0     1188 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/load_locations.py
+-rw-r--r--   0        0        0     1097 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/pilot_esi_error_handling.py
+-rw-r--r--   0        0        0      838 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/profiler_toolbox.py
+-rw-r--r--   0        0        0     5744 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/utils.py
+-rw-r--r--   0        0        0        0 2023-07-05 11:09:35.064958 aa_memberaudit-2.9.3/memberaudit/tests/views/__init__.py
+-rw-r--r--   0        0        0     9299 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/views/test_admin.py
+-rw-r--r--   0        0        0     7089 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/views/test_character_finder.py
+-rw-r--r--   0        0        0    32680 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/views/test_character_viewer_1.py
+-rw-r--r--   0        0        0    24561 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/views/test_character_viewer_2.py
+-rw-r--r--   0        0        0    14594 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/views/test_characters.py
+-rw-r--r--   0        0        0     4101 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/views/test_data_export.py
+-rw-r--r--   0        0        0    16249 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/views/test_reports.py
+-rw-r--r--   0        0        0      710 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tools/clear_celery_once_locks.py
+-rw-r--r--   0        0        0     3051 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tools/drop_tables.sql
+-rw-r--r--   0        0        0      329 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tools/total_size.sql
+-rw-r--r--   0        0        0     7242 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/urls.py
+-rw-r--r--   0        0        0     2367 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/utils.py
+-rw-r--r--   0        0        0        0 2023-07-05 11:09:35.064958 aa_memberaudit-2.9.3/memberaudit/views/__init__.py
+-rw-r--r--   0        0        0     1539 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/views/_common.py
+-rw-r--r--   0        0        0     3510 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/views/admin.py
+-rw-r--r--   0        0        0    12637 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/views/character_finder.py
+-rw-r--r--   0        0        0    24043 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/views/character_viewer_1.py
+-rw-r--r--   0        0        0    24147 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/views/character_viewer_2.py
+-rw-r--r--   0        0        0     8029 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/views/characters.py
+-rw-r--r--   0        0        0     2222 2023-07-05 11:03:39.277295 aa_memberaudit-2.9.3/memberaudit/views/data_export.py
+-rw-r--r--   0        0        0    13139 2023-07-05 11:03:39.277295 aa_memberaudit-2.9.3/memberaudit/views/reports.py
+-rw-r--r--   0        0        0     2285 2023-07-05 11:03:39.277295 aa_memberaudit-2.9.3/pyproject.toml
+-rw-r--r--   0        0        0     7374 1970-01-01 00:00:00.000000 aa_memberaudit-2.9.3/PKG-INFO
```

### Comparing `aa_memberaudit-2.9.2/LICENSE` & `aa_memberaudit-2.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/README.md` & `aa_memberaudit-2.9.3/README.md`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/admin.py` & `aa_memberaudit-2.9.3/memberaudit/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -394,24 +394,15 @@
                 priority=MEMBERAUDIT_TASKS_NORMAL_PRIORITY,
             )  # type: ignore
             self.message_user(
                 request, _("Started updating assets for character %s.") % obj
             )
 
     @admin.display(
-        description=(
-            _(
-                "Update %s for selected characters from EVE server"
-                % {
-                    Character.UpdateSection.display_name(
-                        Character.UpdateSection.LOCATION
-                    )
-                }
-            )
-        )
+        description=(_("Update location for selected characters from EVE server"))
     )
     def update_location(self, request, queryset):
         section = Character.UpdateSection.LOCATION
         for obj in queryset:
             tasks.update_character_section.apply_async(
                 kwargs={"character_pk": obj.pk, "section": section},
                 priority=MEMBERAUDIT_TASKS_NORMAL_PRIORITY,
```

### Comparing `aa_memberaudit-2.9.2/memberaudit/app_settings.py` & `aa_memberaudit-2.9.3/memberaudit/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/auth_hooks.py` & `aa_memberaudit-2.9.3/memberaudit/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/checks.py` & `aa_memberaudit-2.9.3/memberaudit/checks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/constants.py` & `aa_memberaudit-2.9.3/memberaudit/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Shared constants for Member Audit."""
 
+import sys
 from enum import IntEnum
 
 
 class EveCategoryId(IntEnum):
     """Eve Online named category IDs"""
 
     ASTEROID = 25
@@ -75,7 +76,10 @@
 """Map to convert arabic to roman numbers (1 to 5 only)"""
 
 DATETIME_FORMAT = "%Y-%b-%d %H:%M"
 MY_DATETIME_FORMAT = "Y-M-d H:i"
 DEFAULT_ICON_SIZE = 32
 SKILL_SET_DEFAULT_ICON_TYPE_ID = 3327
 MAIL_LABEL_ID_ALL_MAILS = 0
+
+IS_TESTING = sys.argv[1:2] == ["test"]
+"""True when tests are currently running, else False."""
```

### Comparing `aa_memberaudit-2.9.2/memberaudit/core/data_exporters.py` & `aa_memberaudit-2.9.3/memberaudit/core/data_exporters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/core/eft_parser.py` & `aa_memberaudit-2.9.3/memberaudit/core/eft_parser.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/core/fittings.py` & `aa_memberaudit-2.9.3/memberaudit/core/fittings.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/core/skill_plans.py` & `aa_memberaudit-2.9.3/memberaudit/core/skill_plans.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/core/skills.py` & `aa_memberaudit-2.9.3/memberaudit/core/skills.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/core/xml_converter.py` & `aa_memberaudit-2.9.3/memberaudit/core/xml_converter.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/decorators.py` & `aa_memberaudit-2.9.3/memberaudit/decorators.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Decorators for Member Audit."""
 
 from functools import wraps
 
 from django.http import HttpResponseForbidden, HttpResponseNotFound
 
 from allianceauth.services.hooks import get_extension_logger
+from app_utils.esi import EsiDailyDowntime, fetch_esi_status
 from app_utils.logging import LoggerAddTag
 
 from memberaudit import __title__
+from memberaudit.constants import IS_TESTING
 
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
 
 def fetch_character_if_allowed(*args_select_related):
     """Asserts the current user has access to the character
     and loads the given character if it exists
@@ -71,7 +73,30 @@
                 func.__name__,
             )
             return func(self, character, token, *args, **kwargs)
 
         return _wrapped_view
 
     return decorator
+
+
+def when_esi_is_available(func):
+    """Makes sure the decorated task only runs when esi is available.
+
+    Raised exception when ESI is offline.
+    Completes the task without running it when downtime is detected.
+
+    Automatically disabled during tests.
+    """
+
+    @wraps(func)
+    def outer(*args, **kwargs):
+        if IS_TESTING is not True:
+            try:
+                fetch_esi_status().raise_for_status()
+            except EsiDailyDowntime:
+                logger.info("Daily Downtime detected. Aborting.")
+                return  # function will not run
+
+        return func(*args, **kwargs)
+
+    return outer
```

### Comparing `aa_memberaudit-2.9.2/memberaudit/forms.py` & `aa_memberaudit-2.9.3/memberaudit/forms.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/helpers.py` & `aa_memberaudit-2.9.3/memberaudit/helpers.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/locale/de/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.3/memberaudit/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/locale/django.pot` & `aa_memberaudit-2.9.3/memberaudit/locale/django.pot`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/locale/en/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.3/memberaudit/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/locale/es/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.3/memberaudit/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/locale/fr_FR/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.3/memberaudit/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/locale/it_IT/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.3/memberaudit/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/locale/ja/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.3/memberaudit/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/locale/ko_KR/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.3/memberaudit/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/locale/ru/LC_MESSAGES/django.mo` & `aa_memberaudit-2.9.3/memberaudit/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/locale/ru/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.3/memberaudit/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/locale/uk/LC_MESSAGES/django.mo` & `aa_memberaudit-2.9.3/memberaudit/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/locale/uk/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.3/memberaudit/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.3/memberaudit/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/management/commands/memberaudit_data_export.py` & `aa_memberaudit-2.9.3/memberaudit/management/commands/memberaudit_data_export.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/management/commands/memberaudit_load_eve.py` & `aa_memberaudit-2.9.3/memberaudit/management/commands/memberaudit_load_eve.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/management/commands/memberaudit_reset_characters.py` & `aa_memberaudit-2.9.3/memberaudit/management/commands/memberaudit_reset_characters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/management/commands/memberaudit_stats.py` & `aa_memberaudit-2.9.3/memberaudit/management/commands/memberaudit_stats.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/management/commands/memberaudit_update_characters.py` & `aa_memberaudit-2.9.3/memberaudit/management/commands/memberaudit_update_characters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/managers/character.py` & `aa_memberaudit-2.9.3/memberaudit/managers/character.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/managers/character_sections_1.py` & `aa_memberaudit-2.9.3/memberaudit/managers/character_sections_1.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/managers/character_sections_2.py` & `aa_memberaudit-2.9.3/memberaudit/managers/character_sections_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/managers/character_sections_3.py` & `aa_memberaudit-2.9.3/memberaudit/managers/character_sections_3.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/managers/general.py` & `aa_memberaudit-2.9.3/memberaudit/managers/general.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/migrations/0001_initial_new.py` & `aa_memberaudit-2.9.3/memberaudit/migrations/0001_initial_new.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/migrations/0002_add_mining_ledger.py` & `aa_memberaudit-2.9.3/memberaudit/migrations/0002_add_mining_ledger.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/migrations/0003_add_notify_permission.py` & `aa_memberaudit-2.9.3/memberaudit/migrations/0003_add_notify_permission.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/migrations/0004_character_is_disabled.py` & `aa_memberaudit-2.9.3/memberaudit/migrations/0004_character_is_disabled.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/migrations/0005_add_fw_stats.py` & `aa_memberaudit-2.9.3/memberaudit/migrations/0005_add_fw_stats.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/migrations/0006_add_localizations.py` & `aa_memberaudit-2.9.3/memberaudit/migrations/0006_add_localizations.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/migrations/0007_add_localization_2.py` & `aa_memberaudit-2.9.3/memberaudit/migrations/0007_add_localization_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/migrations/0008_improve_skill_sets.py` & `aa_memberaudit-2.9.3/memberaudit/migrations/0008_improve_skill_sets.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/migrations/0009_add_planetary_industry.py` & `aa_memberaudit-2.9.3/memberaudit/migrations/0009_add_planetary_industry.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/models/__init__.py` & `aa_memberaudit-2.9.3/memberaudit/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/models/character_sections_1.py` & `aa_memberaudit-2.9.3/memberaudit/models/character_sections_1.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/models/character_sections_2.py` & `aa_memberaudit-2.9.3/memberaudit/models/character_sections_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/models/character_sections_3.py` & `aa_memberaudit-2.9.3/memberaudit/models/character_sections_3.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/models/characters.py` & `aa_memberaudit-2.9.3/memberaudit/models/characters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/models/general.py` & `aa_memberaudit-2.9.3/memberaudit/models/general.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/signals.py` & `aa_memberaudit-2.9.3/memberaudit/signals.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/character_viewer.css` & `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/character_viewer.css`

 * *Files 1% similar despite different names*

```diff
@@ -230,25 +230,28 @@
     }
 
     /* sidebar */
     .sidebar_characters {
         list-style-type: none;
         margin: 0;
         padding: 0;
+        overflow-x: auto;
     }
 
     .sidebar_character {
         margin: 0.2rem 0;
+        white-space: nowrap;
     }
 
     .sidebar_character_disabled {
         margin: 0.2rem 0;
         display: block;
         padding: 0.2rem 0.4rem;
         text-decoration: none;
+        white-space: nowrap;
     }
 
     .sidebar_character>a {
         display: block;
         padding: 0.2rem 0.4rem;
         text-decoration: none;
     }
```

### Comparing `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/global.css` & `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/global.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/global.min.css` & `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/global.min.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/launcher.css` & `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/launcher.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/launcher.min.css` & `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/launcher.min.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/memberaudit.css` & `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/memberaudit.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/memberaudit.min.css` & `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/memberaudit.min.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/reports.css` & `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/reports.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif` & `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif` & `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/charisma.png` & `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/charisma.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/eve-prism.png` & `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/eve-prism.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/evesearch.png` & `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/evesearch.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/intelligence.png` & `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/intelligence.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/memory.png` & `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/memory.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/perception.png` & `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/perception.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/willpower.png` & `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/willpower.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js` & `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js` & `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js` & `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/vendor/moment/moment.min.js` & `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/vendor/moment/moment.min.js`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tasks.py` & `aa_memberaudit-2.9.3/memberaudit/tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,34 +12,30 @@
 from esi.models import Token
 from eveuniverse.constants import POST_UNIVERSE_NAMES_MAX_ITEMS
 from eveuniverse.models import EveEntity, EveMarketPrice
 
 from allianceauth.notifications import notify
 from allianceauth.services.hooks import get_extension_logger
 from allianceauth.services.tasks import QueueOnce
-from app_utils.esi import (
-    EsiDailyDowntime,
-    EsiErrorLimitExceeded,
-    EsiOffline,
-    fetch_esi_status,
-)
+from app_utils.esi import EsiErrorLimitExceeded, EsiOffline
 from app_utils.logging import LoggerAddTag
 
 from memberaudit import __title__, utils
 from memberaudit.app_settings import (
     MEMBERAUDIT_BULK_METHODS_BATCH_SIZE,
     MEMBERAUDIT_LOG_UPDATE_STATS,
     MEMBERAUDIT_TASKS_LOW_PRIORITY,
     MEMBERAUDIT_TASKS_MAX_ASSETS_PER_PASS,
     MEMBERAUDIT_TASKS_NORMAL_PRIORITY,
     MEMBERAUDIT_TASKS_OBJECT_CACHE_TIMEOUT,
     MEMBERAUDIT_TASKS_TIME_LIMIT,
     MEMBERAUDIT_UPDATE_STALE_RING_2,
 )
 from memberaudit.core import data_exporters
+from memberaudit.decorators import when_esi_is_available
 from memberaudit.models import (
     Character,
     CharacterAsset,
     CharacterContract,
     CharacterMail,
     CharacterUpdateStatus,
     ComplianceGroupDesignation,
@@ -77,25 +73,21 @@
     if ComplianceGroupDesignation.objects.exists():
         update_compliance_groups_for_all.apply_async(
             priority=MEMBERAUDIT_TASKS_NORMAL_PRIORITY
         )
 
 
 @shared_task(**TASK_DEFAULTS_BIND_ONCE)
+@when_esi_is_available
 def update_all_characters(self, force_update: bool = False) -> None:
     """Start the update of all registered characters
 
     Args:
     - force_update: When set to True will always update regardless of stale status
     """
-    try:
-        fetch_esi_status().raise_for_status()
-    except EsiDailyDowntime:
-        logger.info("Daily Downtime detected. Aborting.")
-        return
     if MEMBERAUDIT_LOG_UPDATE_STATS:
         stats = CharacterUpdateStatus.objects.statistics()
         logger.info(f"Update statistics: {stats}")
 
     # disable characters without owner
     orphaned_characters = Character.objects.filter(
         eve_character__character_ownership__isnull=True
@@ -270,25 +262,25 @@
             "once": {
                 "keys": ["character_pk", "section", "force_update"],
                 "graceful": True,
             }
         },
     }
 )
+@when_esi_is_available
 def update_character_section(
     self,
     character_pk: int,
     section: str,
     force_update: bool = False,
     root_task_id: Optional[str] = None,
     parent_task_id: Optional[str] = None,
     **kwargs,
 ) -> None:
     """Task that updates the section of a character"""
-    fetch_esi_status().raise_for_status()
     character = Character.objects.get_cached(
         pk=character_pk, timeout=MEMBERAUDIT_TASKS_OBJECT_CACHE_TIMEOUT
     )
     character.reset_update_section(section, root_task_id, parent_task_id)
     logger.info(
         "%s: Updating %s", character, Character.UpdateSection.display_name(section)
     )
@@ -345,17 +337,17 @@
         character=character,
         section=section,
         defaults={"is_success": True, "last_error_message": "", "finished_at": now()},
     )
 
 
 @shared_task(**TASK_DEFAULTS_ONCE)
+@when_esi_is_available
 def update_unresolved_eve_entities() -> None:
     """Bulk resolved all unresolved EveEntity objects in database."""
-    fetch_esi_status().raise_for_status()
     unresolved_ids = EveEntity.objects.filter(name="")[
         :POST_UNIVERSE_NAMES_MAX_ITEMS
     ].values_list("id", flat=True)
     if unresolved_ids:
         updated_count = EveEntity.objects.update_from_esi_by_id(unresolved_ids)
         logger.info("Updating %d unresolved entities from ESI", updated_count)
 
@@ -395,19 +387,19 @@
         assets_build_list_from_esi.s(character.pk, force_update).set(priority=priority),
         assets_preload_objects.s(character.pk).set(priority=priority),
         assets_create_parents.s(character.pk).set(priority=priority),
     ).delay()
 
 
 @shared_task(**TASK_DEFAULTS_BIND_ONCE)
+@when_esi_is_available
 def assets_build_list_from_esi(
     self, character_pk: int, force_update: bool = False
 ) -> dict:
     """Building asset list"""
-    fetch_esi_status().raise_for_status()
     character = Character.objects.get_cached(
         pk=character_pk, timeout=MEMBERAUDIT_TASKS_OBJECT_CACHE_TIMEOUT
     )
     asset_list = _character_update_with_error_logging(
         self,
         character,
         Character.UpdateSection.ASSETS,
@@ -642,83 +634,83 @@
         ),
         update_character_mail_bodies.si(character.pk).set(priority=priority),
         update_unresolved_eve_entities.si().set(priority=priority),
     ).delay()
 
 
 @shared_task(**TASK_DEFAULTS_BIND_ONCE)
+@when_esi_is_available
 def update_character_mailing_lists(
     self, character_pk: int, force_update: bool = False
 ) -> None:
-    fetch_esi_status().raise_for_status()
     character = Character.objects.get_cached(
         pk=character_pk, timeout=MEMBERAUDIT_TASKS_OBJECT_CACHE_TIMEOUT
     )
     _character_update_with_error_logging(
         self,
         character,
         Character.UpdateSection.MAILS,
         character.update_mailing_lists,
         force_update=force_update,
     )
 
 
 @shared_task(**TASK_DEFAULTS_BIND_ONCE)
+@when_esi_is_available
 def update_character_mail_labels(
     self, character_pk: int, force_update: bool = False
 ) -> None:
-    fetch_esi_status().raise_for_status()
     character = Character.objects.get_cached(
         pk=character_pk, timeout=MEMBERAUDIT_TASKS_OBJECT_CACHE_TIMEOUT
     )
     _character_update_with_error_logging(
         self,
         character,
         Character.UpdateSection.MAILS,
         character.update_mail_labels,
         force_update=force_update,
     )
 
 
 @shared_task(**TASK_DEFAULTS_BIND_ONCE)
+@when_esi_is_available
 def update_character_mail_headers(
     self, character_pk: int, force_update: bool = False
 ) -> None:
-    fetch_esi_status().raise_for_status()
     character = Character.objects.get_cached(
         pk=character_pk, timeout=MEMBERAUDIT_TASKS_OBJECT_CACHE_TIMEOUT
     )
     _character_update_with_error_logging(
         self,
         character,
         Character.UpdateSection.MAILS,
         character.update_mail_headers,
         force_update=force_update,
     )
 
 
 @shared_task(**TASK_DEFAULTS_BIND_ONCE)
+@when_esi_is_available
 def update_mail_body_esi(self, character_pk: int, mail_pk: int):
     """Task for updating the body of a mail from ESI"""
-    fetch_esi_status().raise_for_status()
     character = Character.objects.get_cached(
         pk=character_pk, timeout=MEMBERAUDIT_TASKS_OBJECT_CACHE_TIMEOUT
     )
     mail = CharacterMail.objects.get(pk=mail_pk)
     _character_update_with_error_logging(
         self,
         character,
         Character.UpdateSection.MAILS,
         character.update_mail_body,
         mail,
     )
 
 
 @shared_task(**TASK_DEFAULTS_BIND_ONCE)
-def update_character_mail_bodies(self, character_pk: int) -> None:
+def update_character_mail_bodies(self, character_pk: int, *args, **kwargs) -> None:
     character = Character.objects.get_cached(
         pk=character_pk, timeout=MEMBERAUDIT_TASKS_OBJECT_CACHE_TIMEOUT
     )
     mails_without_body_qs = character.mails.filter(body="")
     mails_without_body_count = mails_without_body_qs.count()
 
     if mails_without_body_count > 0:
@@ -770,35 +762,35 @@
             priority=priority
         ),
         update_unresolved_eve_entities.si().set(priority=priority),
     ).delay()
 
 
 @shared_task(**TASK_DEFAULTS_BIND)
+@when_esi_is_available
 def update_character_contact_labels(
     self, character_pk: int, force_update: bool = False
 ) -> None:
-    fetch_esi_status().raise_for_status()
     character = Character.objects.get_cached(
         pk=character_pk, timeout=MEMBERAUDIT_TASKS_OBJECT_CACHE_TIMEOUT
     )
     _character_update_with_error_logging(
         self,
         character,
         Character.UpdateSection.CONTACTS,
         character.update_contact_labels,
         force_update=force_update,
     )
 
 
 @shared_task(**TASK_DEFAULTS_BIND)
+@when_esi_is_available
 def update_character_contacts_2(
     self, character_pk: int, force_update: bool = False
 ) -> None:
-    fetch_esi_status().raise_for_status()
     character = Character.objects.get_cached(
         pk=character_pk, timeout=MEMBERAUDIT_TASKS_OBJECT_CACHE_TIMEOUT
     )
     _character_update_with_error_logging(
         self,
         character,
         Character.UpdateSection.CONTACTS,
@@ -843,18 +835,18 @@
         update_character_contracts_items.si(character.pk).set(priority=priority),
         update_character_contracts_bids.si(character.pk).set(priority=priority),
         update_unresolved_eve_entities.si().set(priority=priority),
     ).delay()
 
 
 @shared_task(**TASK_DEFAULTS_BIND_ONCE)
+@when_esi_is_available
 def update_character_contract_headers(
     self, character_pk: int, force_update: bool = False
 ):
-    fetch_esi_status().raise_for_status()
     character = Character.objects.get_cached(
         pk=character_pk, timeout=MEMBERAUDIT_TASKS_OBJECT_CACHE_TIMEOUT
     )
     _character_update_with_error_logging(
         self,
         character,
         Character.UpdateSection.CONTRACTS,
@@ -890,17 +882,17 @@
             )
 
     else:
         logger.info("%s: No items to update", character)
 
 
 @shared_task(**TASK_DEFAULTS_ONCE)
+@when_esi_is_available
 def update_contract_items_esi(character_pk: int, contract_pk: int):
     """Task for updating the items of a contract from ESI"""
-    fetch_esi_status().raise_for_status()
     character = Character.objects.get_cached(
         pk=character_pk, timeout=MEMBERAUDIT_TASKS_OBJECT_CACHE_TIMEOUT
     )
     contract = CharacterContract.objects.get(pk=contract_pk)
     character.update_contract_items(contract)
 
 
@@ -929,17 +921,17 @@
 
     else:
         logger.info("%s: No bids to update", character)
     _log_character_update_success(character, Character.UpdateSection.CONTRACTS)
 
 
 @shared_task(**TASK_DEFAULTS_ONCE)
+@when_esi_is_available
 def update_contract_bids_esi(character_pk: int, contract_pk: int):
     """Task for updating the bids of a contract from ESI"""
-    fetch_esi_status().raise_for_status()
     character = Character.objects.get_cached(
         pk=character_pk, timeout=MEMBERAUDIT_TASKS_OBJECT_CACHE_TIMEOUT
     )
     contract = CharacterContract.objects.get(pk=contract_pk)
     character.update_contract_bids(contract)
 
 
@@ -973,16 +965,16 @@
     chain(
         update_character_wallet_journal_entries.si(character.pk).set(priority=priority),
         update_unresolved_eve_entities.si().set(priority=priority),
     ).delay()
 
 
 @shared_task(**TASK_DEFAULTS_BIND_ONCE)
+@when_esi_is_available
 def update_character_wallet_journal_entries(self, character_pk: int) -> None:
-    fetch_esi_status().raise_for_status()
     character = Character.objects.get_cached(
         pk=character_pk, timeout=MEMBERAUDIT_TASKS_OBJECT_CACHE_TIMEOUT
     )
     _character_update_with_error_logging(
         self,
         character,
         Character.UpdateSection.WALLET_JOURNAL,
@@ -991,21 +983,17 @@
     _log_character_update_success(character, Character.UpdateSection.WALLET_JOURNAL)
 
 
 # Tasks for other objects
 
 
 @shared_task(**TASK_DEFAULTS_BIND_ONCE)
+@when_esi_is_available
 def update_market_prices(self):
     """Update market prices from ESI"""
-    try:
-        fetch_esi_status().raise_for_status()
-    except EsiDailyDowntime:
-        logger.info("Daily Downtime detected. Aborting.")
-        return
     EveMarketPrice.objects.update_from_esi(
         minutes_until_stale=MEMBERAUDIT_UPDATE_STALE_RING_2
     )
 
 
 @shared_task(
     **{
```

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html` & `aa_memberaudit-2.9.3/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/admin/memberaudit/skillset/import_skills.html` & `aa_memberaudit-2.9.3/memberaudit/templates/admin/memberaudit/skillset/import_skills.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/character_finder.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/character_finder.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/character_viewer.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/character_viewer.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/data_export.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/data_export.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/launcher.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/launcher.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/contract.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/contract.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/mail.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/mail.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/overview.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/overview.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/implants.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/implants.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/planets.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/planets.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/menu.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/menu.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/solar_system.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/solar_system.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/reports.html` & `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/reports.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/core/test_core_xml_converter.py` & `aa_memberaudit-2.9.3/memberaudit/tests/core/test_core_xml_converter.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/core/test_data_exporters.py` & `aa_memberaudit-2.9.3/memberaudit/tests/core/test_data_exporters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/core/test_eft_parser.py` & `aa_memberaudit-2.9.3/memberaudit/tests/core/test_eft_parser.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/core/test_fittings.py` & `aa_memberaudit-2.9.3/memberaudit/tests/core/test_fittings.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/core/test_skill_plans.py` & `aa_memberaudit-2.9.3/memberaudit/tests/core/test_skill_plans.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/core/test_skills.py` & `aa_memberaudit-2.9.3/memberaudit/tests/core/test_skills.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/managers/test_character.py` & `aa_memberaudit-2.9.3/memberaudit/tests/managers/test_character.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/managers/test_character_sections_1.py` & `aa_memberaudit-2.9.3/memberaudit/tests/managers/test_character_sections_1.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/managers/test_character_sections_2.py` & `aa_memberaudit-2.9.3/memberaudit/tests/managers/test_character_sections_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/managers/test_character_sections_3.py` & `aa_memberaudit-2.9.3/memberaudit/tests/managers/test_character_sections_3.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/managers/test_general.py` & `aa_memberaudit-2.9.3/memberaudit/tests/managers/test_general.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/models/test_character_sections.py` & `aa_memberaudit-2.9.3/memberaudit/tests/models/test_character_sections.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/models/test_characters_1.py` & `aa_memberaudit-2.9.3/memberaudit/tests/models/test_characters_1.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/models/test_characters_2.py` & `aa_memberaudit-2.9.3/memberaudit/tests/models/test_characters_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/models/test_general.py` & `aa_memberaudit-2.9.3/memberaudit/tests/models/test_general.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/test_admin.py` & `aa_memberaudit-2.9.3/memberaudit/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/test_auth_hooks.py` & `aa_memberaudit-2.9.3/memberaudit/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/test_checks.py` & `aa_memberaudit-2.9.3/memberaudit/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/test_commands.py` & `aa_memberaudit-2.9.3/memberaudit/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/test_factories.py` & `aa_memberaudit-2.9.3/memberaudit/tests/test_factories.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/test_forms.py` & `aa_memberaudit-2.9.3/memberaudit/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/test_helpers.py` & `aa_memberaudit-2.9.3/memberaudit/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/test_integration.py` & `aa_memberaudit-2.9.3/memberaudit/tests/test_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import datetime as dt
-from unittest.mock import MagicMock, patch
+from unittest.mock import patch
 
 from django.test import TestCase, override_settings
 from django.urls import reverse
 from django.utils.dateparse import parse_datetime
 from django.utils.timezone import now
 from django_webtest import WebTest
 from eveuniverse.models import EveEntity, EveType
 
 from allianceauth.tests.auth_utils import AuthUtils
-from app_utils.esi import EsiStatus, fetch_esi_status
+from app_utils.esi import EsiStatus
 from app_utils.testing import NoSocketsTestCase
 
 from memberaudit import tasks
 from memberaudit.models import (
     Character,
     CharacterAsset,
     CharacterContract,
@@ -37,15 +37,14 @@
 )
 
 MANAGERS_PATH = "memberaudit.managers"
 MODELS_PATH = "memberaudit.models"
 TASKS_PATH = "memberaudit.tasks"
 
 
-@patch(TASKS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
 class TestUILauncher(WebTest):
     fixtures = ["disable_analytics.json"]
 
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
         load_eveuniverse()
@@ -328,15 +327,14 @@
         self.assertIn(body_text, mail_details.text)
 
 
 @patch(
     TASKS_PATH + ".Character.objects.get_cached",
     lambda pk, timeout: Character.objects.get(pk=pk),
 )
-@patch(TASKS_PATH + ".fetch_esi_status", lambda: EsiStatus(True, 99, 60))
 @patch(MANAGERS_PATH + ".general.fetch_esi_status", lambda: EsiStatus(True, 99, 60))
 @patch(TASKS_PATH + ".MEMBERAUDIT_LOG_UPDATE_STATS", False)
 @patch(MANAGERS_PATH + ".character_sections_1.data_retention_cutoff", lambda: None)
 @patch(MANAGERS_PATH + ".character_sections_2.data_retention_cutoff", lambda: None)
 @patch(MANAGERS_PATH + ".character_sections_3.data_retention_cutoff", lambda: None)
 @patch(MANAGERS_PATH + ".character_sections_1.esi", esi_stub)
 @patch(MANAGERS_PATH + ".character_sections_2.esi", esi_stub)
```

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/test_signals.py` & `aa_memberaudit-2.9.3/memberaudit/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/test_tasks.py` & `aa_memberaudit-2.9.3/memberaudit/tests/test_tasks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 import datetime as dt
 from unittest import skipIf
-from unittest.mock import MagicMock, patch
+from unittest.mock import patch
 
 from celery.exceptions import Retry as CeleryRetry
 
 from django.test import override_settings
 from django.utils.timezone import now
 from esi.models import Token
 from eveuniverse.models import EveSolarSystem, EveType
 from eveuniverse.tests.testdata.factories import create_eve_entity
 
 from allianceauth.eveonline.models import EveCharacter
-from app_utils.esi import (
-    EsiDailyDowntime,
-    EsiErrorLimitExceeded,
-    EsiOffline,
-    EsiStatus,
-    fetch_esi_status,
-)
+from app_utils.esi import EsiErrorLimitExceeded, EsiOffline, EsiStatus
 from app_utils.esi_testing import build_http_error
 from app_utils.testing import (
     NoSocketsTestCase,
     create_authgroup,
     create_user_from_evecharacter,
     generate_invalid_pk,
 )
@@ -80,24 +74,22 @@
         tasks.run_regular_updates()
         # then
         self.assertTrue(mock_update_market_prices.apply_async.called)
         self.assertTrue(mock_update_all_characters.apply_async.called)
         self.assertTrue(mock_update_compliance_groups_for_all.apply_async.called)
 
 
-@patch(TASKS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
 class TestOtherTasks(TestCaseTasks):
     @patch(TASKS_PATH + ".EveMarketPrice.objects.update_from_esi", spec=True)
     def test_update_market_prices(self, mock_update_from_esi):
         tasks.update_market_prices()
         self.assertTrue(mock_update_from_esi.called)
 
 
 @override_settings(CELERY_ALWAYS_EAGER=True)  # need to ignore exceptions
-@patch(TASKS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
 @patch(MANAGERS_PATH + ".character_sections_1.esi")
 class TestUpdateCharacterAssets(TestCaseTasks):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_eveuniverse()
         load_entities()
@@ -379,15 +371,14 @@
         status = self.character_1001.update_status_set.get(
             section=Character.UpdateSection.ASSETS
         )
         self.assertTrue(status.is_success)
 
 
 @override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
-@patch(TASKS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
 @patch(MANAGERS_PATH + ".general.fetch_esi_status", lambda: EsiStatus(True, 99, 60))
 @patch(MANAGERS_PATH + ".character_sections_1.esi")
 class TestUpdateCharacterContacts(TestCaseTasks):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_eveuniverse()
@@ -427,15 +418,14 @@
                 status.last_error_message, "HTTPBadGateway: 502 Test exception"
             )
         else:
             self.assertTrue(False)  # Hack to ensure the test fails when it gets here
 
 
 @override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
-@patch(TASKS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
 @patch(MANAGERS_PATH + ".general.fetch_esi_status", lambda: EsiStatus(True, 99, 60))
 @patch(MANAGERS_PATH + ".character_sections_1.esi")
 class TestUpdateCharacterContracts(TestCaseTasks):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_eveuniverse()
@@ -476,15 +466,14 @@
                 status.last_error_message, "HTTPBadGateway: 502 Test exception"
             )
         else:
             self.assertTrue(False)  # Hack to ensure the test fails when it gets here
 
 
 @override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
-@patch(TASKS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
 @patch(MANAGERS_PATH + ".general.fetch_esi_status", lambda: EsiStatus(True, 99, 60))
 @patch(MANAGERS_PATH + ".character_sections_2.esi")
 @patch(MANAGERS_PATH + ".general.esi")
 class TestUpdateCharacterMails(TestCaseTasks):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
@@ -528,15 +517,14 @@
                 status.last_error_message, "HTTPBadGateway: 502 Test exception"
             )
         else:
             self.assertTrue(False)  # Hack to ensure the test fails when it gets here
 
 
 @override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
-@patch(TASKS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
 @patch(MANAGERS_PATH + ".general.fetch_esi_status", lambda: EsiStatus(True, 99, 60))
 @patch(MANAGERS_PATH + ".character_sections_3.esi")
 class TestUpdateCharacterWalletJournal(TestCaseTasks):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_eveuniverse()
@@ -575,15 +563,14 @@
             self.assertEqual(
                 status.last_error_message, "HTTPBadGateway: 502 Test exception"
             )
         else:
             self.assertTrue(False)  # Hack to ensure the test fails when it gets here
 
 
-@patch(TASKS_PATH + ".fetch_esi_status", lambda: EsiStatus(True, 99, 60))
 @patch(MANAGERS_PATH + ".general.fetch_esi_status", lambda: EsiStatus(True, 99, 60))
 @patch(MANAGERS_PATH + ".character_sections_1.data_retention_cutoff", lambda: None)
 @patch(MANAGERS_PATH + ".character_sections_2.data_retention_cutoff", lambda: None)
 @patch(MANAGERS_PATH + ".character_sections_3.data_retention_cutoff", lambda: None)
 @patch(MANAGERS_PATH + ".character_sections_1.esi", esi_stub)
 @patch(MANAGERS_PATH + ".character_sections_2.esi", esi_stub)
 @patch(MANAGERS_PATH + ".character_sections_3.esi", esi_stub)
@@ -688,15 +675,14 @@
         # when
         result = tasks.update_character(character.pk)
         # then
         self.assertFalse(result)
         self.assertIsNone(character.is_update_status_ok())
 
 
-@patch(TASKS_PATH + ".fetch_esi_status", lambda: EsiStatus(True, 99, 60))
 @patch(MANAGERS_PATH + ".general.fetch_esi_status", lambda: EsiStatus(True, 99, 60))
 @patch(MANAGERS_PATH + ".character_sections_1.data_retention_cutoff", lambda: None)
 @patch(MANAGERS_PATH + ".character_sections_2.data_retention_cutoff", lambda: None)
 @patch(MANAGERS_PATH + ".character_sections_3.data_retention_cutoff", lambda: None)
 @patch(MANAGERS_PATH + ".character_sections_1.esi", esi_error_stub)
 @patch(MANAGERS_PATH + ".character_sections_2.esi", esi_error_stub)
 @patch(MANAGERS_PATH + ".character_sections_3.esi", esi_error_stub)
@@ -724,15 +710,14 @@
         ).first()
         self.assertEqual(
             status.last_error_message, "HTTPBadGateway: 502 Test exception"
         )
         self.assertTrue(status.finished_at)
 
 
-@patch(TASKS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
 @patch(MANAGERS_PATH + ".general.fetch_esi_status", lambda: EsiStatus(True, 99, 60))
 @patch(TASKS_PATH + ".Location.objects.structure_update_or_create_esi", spec=True)
 class TestUpdateStructureEsi(TestCaseTasks):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_entities()
@@ -795,15 +780,14 @@
         """When ESI error limit reached, then abort"""
         mock_update_or_create_esi.side_effect = EsiErrorLimitExceeded(5)
 
         with self.assertRaises(EsiErrorLimitExceeded):
             tasks.update_mail_entity_esi(1001)
 
 
-@patch(TASKS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
 @patch(MANAGERS_PATH + ".general.fetch_esi_status", lambda: EsiStatus(True, 99, 60))
 @override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
 class TestUpdateCharactersDoctrines(TestCaseTasks):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_entities()
@@ -882,15 +866,14 @@
         )
         # when
         tasks.update_compliance_groups_for_user(user.pk)
         # then
         self.assertTrue(mock_update_user.called)
 
 
-@patch(TASKS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
 @patch(TASKS_PATH + ".update_character", spec=True)
 class TestUpdateAllCharacters(TestCaseTasks):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_eveuniverse()
         load_entities()
@@ -923,44 +906,14 @@
         # then
         character_1001.refresh_from_db()
         self.assertFalse(character_1001.is_disabled)
         character_1002.refresh_from_db()
         self.assertTrue(character_1002.is_disabled)
 
 
-@patch(TASKS_PATH + ".fetch_esi_status", spec=True)
-class TestAbortMainTaskDuringDailyDowntime(TestCaseTasks):
-    @patch(TASKS_PATH + ".update_character", spec=True)
-    def test_should_abort_update_all_characters(
-        self, mock_update_character, mock_fetch_esi_status
-    ):
-        # given
-        mock_fetch_esi_status.return_value.raise_for_status.side_effect = (
-            EsiDailyDowntime
-        )
-        # when/then
-        tasks.update_all_characters()
-        # then
-        self.assertFalse(mock_update_character.apply_async.called)
-
-    @patch(TASKS_PATH + ".EveMarketPrice.objects.update_from_esi")
-    def test_should_abort_update_market_prices(
-        self, mock_update_from_esi, mock_fetch_esi_status
-    ):
-        # given
-        mock_fetch_esi_status.return_value.raise_for_status.side_effect = (
-            EsiDailyDowntime
-        )
-        # when/then
-        tasks.update_market_prices()
-        # then
-        self.assertFalse(mock_update_from_esi.called)
-
-
-@patch(TASKS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
 @patch(TASKS_PATH + ".EveEntity.objects.update_from_esi_by_id", spec=True)
 class TestUpdateUnresolvedEveEntities(TestCaseTasks):
     def test_should_not_attempt_to_update_when_no_unresolved_entities(
         self, mock_update_from_esi_by_id
     ):
         # given
         create_eve_entity(id=1, name="alpha")
```

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/test_templatetags.py` & `aa_memberaudit-2.9.3/memberaudit/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/test_utils.py` & `aa_memberaudit-2.9.3/memberaudit/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/testdata/create_eveuniverse.py` & `aa_memberaudit-2.9.3/memberaudit/tests/testdata/create_eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/testdata/entities.json` & `aa_memberaudit-2.9.3/memberaudit/tests/testdata/entities.json`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/testdata/esi_client_stub.py` & `aa_memberaudit-2.9.3/memberaudit/tests/testdata/esi_client_stub.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/testdata/esi_testdata.json` & `aa_memberaudit-2.9.3/memberaudit/tests/testdata/esi_testdata.json`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/testdata/eveuniverse.json` & `aa_memberaudit-2.9.3/memberaudit/tests/testdata/eveuniverse.json`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/testdata/factories.py` & `aa_memberaudit-2.9.3/memberaudit/tests/testdata/factories.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_archon.txt` & `aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_archon.txt`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_archon_max.txt` & `aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_archon_max.txt`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_svipul.txt` & `aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_svipul.txt`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_tengu.txt` & `aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_tengu.txt`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/testdata/generate_character.py` & `aa_memberaudit-2.9.3/memberaudit/tests/testdata/generate_character.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/testdata/generate_doctrines.py` & `aa_memberaudit-2.9.3/memberaudit/tests/testdata/generate_doctrines.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/testdata/load_entities.py` & `aa_memberaudit-2.9.3/memberaudit/tests/testdata/load_entities.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/testdata/load_locations.py` & `aa_memberaudit-2.9.3/memberaudit/tests/testdata/load_locations.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/testdata/pilot_esi_error_handling.py` & `aa_memberaudit-2.9.3/memberaudit/tests/testdata/pilot_esi_error_handling.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/testdata/profiler_toolbox.py` & `aa_memberaudit-2.9.3/memberaudit/tests/testdata/profiler_toolbox.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/utils.py` & `aa_memberaudit-2.9.3/memberaudit/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/views/test_admin.py` & `aa_memberaudit-2.9.3/memberaudit/tests/views/test_admin.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/views/test_character_finder.py` & `aa_memberaudit-2.9.3/memberaudit/tests/views/test_character_finder.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/views/test_character_viewer_1.py` & `aa_memberaudit-2.9.3/memberaudit/tests/views/test_character_viewer_1.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/views/test_character_viewer_2.py` & `aa_memberaudit-2.9.3/memberaudit/tests/views/test_character_viewer_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/views/test_characters.py` & `aa_memberaudit-2.9.3/memberaudit/tests/views/test_characters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/views/test_data_export.py` & `aa_memberaudit-2.9.3/memberaudit/tests/views/test_data_export.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tests/views/test_reports.py` & `aa_memberaudit-2.9.3/memberaudit/tests/views/test_reports.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tools/clear_celery_once_locks.py` & `aa_memberaudit-2.9.3/memberaudit/tools/clear_celery_once_locks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/tools/drop_tables.sql` & `aa_memberaudit-2.9.3/memberaudit/tools/drop_tables.sql`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/urls.py` & `aa_memberaudit-2.9.3/memberaudit/urls.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/utils.py` & `aa_memberaudit-2.9.3/memberaudit/utils.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/views/_common.py` & `aa_memberaudit-2.9.3/memberaudit/views/_common.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/views/admin.py` & `aa_memberaudit-2.9.3/memberaudit/views/admin.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/views/character_finder.py` & `aa_memberaudit-2.9.3/memberaudit/views/character_finder.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/views/character_viewer_1.py` & `aa_memberaudit-2.9.3/memberaudit/views/character_viewer_1.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/views/character_viewer_2.py` & `aa_memberaudit-2.9.3/memberaudit/views/character_viewer_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/views/characters.py` & `aa_memberaudit-2.9.3/memberaudit/views/characters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/views/data_export.py` & `aa_memberaudit-2.9.3/memberaudit/views/data_export.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/memberaudit/views/reports.py` & `aa_memberaudit-2.9.3/memberaudit/views/reports.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/pyproject.toml` & `aa_memberaudit-2.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.2/PKG-INFO` & `aa_memberaudit-2.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-memberaudit
-Version: 2.9.2
+Version: 2.9.3
 Summary: "An Alliance Auth app that provides full access to Eve characters
 Keywords: allianceauth,eveonline,memberaudit
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>, Peter Pfeufer <develop@ppfeufer.de>, Rebecca Murphy <rebecca@rcmurphy.me>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

