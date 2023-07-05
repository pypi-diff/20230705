# Comparing `tmp/sdccli-0.7.8.tar.gz` & `tmp/sdccli-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdccli-0.7.8.tar", max compression
+gzip compressed data, was "sdccli-0.7.9.tar", max compression
```

## Comparing `sdccli-0.7.8.tar` & `sdccli-0.7.9.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0     1067 2021-04-08 11:13:57.987774 sdccli-0.7.8/LICENSE.txt
--rw-r--r--   0        0        0      937 2021-04-08 11:14:09.867775 sdccli-0.7.8/pyproject.toml
--rw-r--r--   0        0        0       21 2021-04-08 11:14:09.867775 sdccli-0.7.8/sdccli/__init__.py
--rw-r--r--   0        0        0     2127 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/__init__.py
--rw-r--r--   0        0        0     5291 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/alert.py
--rw-r--r--   0        0        0     9160 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/backup.py
--rw-r--r--   0        0        0     5549 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/capture.py
--rw-r--r--   0        0        0     3924 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/command.py
--rw-r--r--   0        0        0     8177 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/compliance.py
--rw-r--r--   0        0        0     7144 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/dashboard/__init__.py
--rw-r--r--   0        0        0     5036 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/dashboard/panel.py
--rw-r--r--   0        0        0     7872 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/dashboardv2.py
--rw-r--r--   0        0        0     4617 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/event.py
--rw-r--r--   0        0        0     4406 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/eventv1.py
--rw-r--r--   0        0        0        0 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/formatter/__init__.py
--rw-r--r--   0        0        0      139 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/formatter/json_formatter/__init__.py
--rw-r--r--   0        0        0      841 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/formatter/text_formatter/__init__.py
--rw-r--r--   0        0        0      464 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/formatter/text_formatter/alert.py
--rw-r--r--   0        0        0      887 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/formatter/text_formatter/dashboard.py
--rw-r--r--   0        0        0     1017 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/formatter/text_formatter/panel.py
--rw-r--r--   0        0        0     1962 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/formatter/text_formatter/policy_events.py
--rw-r--r--   0        0        0        0 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/formatter/text_formatter/scanning/__init__.py
--rw-r--r--   0        0        0      537 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/formatter/text_formatter/scanning/alert.py
--rw-r--r--   0        0        0     4288 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/formatter/text_formatter/scanning/image.py
--rw-r--r--   0        0        0     3583 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/formatter/text_formatter/scanning/vulnerability.py
--rw-r--r--   0        0        0    18732 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/policy/__init__.py
--rw-r--r--   0        0        0     3528 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/policy/falco_list.py
--rw-r--r--   0        0        0     3548 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/policy/falco_macro.py
--rw-r--r--   0        0        0    10159 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/policy/rule.py
--rw-r--r--   0        0        0     6687 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/profile.py
--rw-r--r--   0        0        0      884 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/scanning/__init__.py
--rw-r--r--   0        0        0     3788 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/scanning/alert.py
--rw-r--r--   0        0        0     7778 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/scanning/cve_report.py
--rw-r--r--   0        0        0     8244 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/scanning/image.py
--rw-r--r--   0        0        0     3925 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/scanning/policy.py
--rw-r--r--   0        0        0     3702 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/scanning/query.py
--rw-r--r--   0        0        0     4148 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/scanning/registry.py
--rw-r--r--   0        0        0     3419 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/scanning/repo.py
--rw-r--r--   0        0        0     1470 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/scanning/runtime.py
--rw-r--r--   0        0        0     2484 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/scanning/subscription.py
--rw-r--r--   0        0        0     4079 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/scanning/vulnerability/__init__.py
--rw-r--r--   0        0        0     1848 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/scanning/vulnerability/bundle.py
--rw-r--r--   0        0        0      587 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/settings/__init__.py
--rw-r--r--   0        0        0     1893 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/settings/access_key.py
--rw-r--r--   0        0        0     3071 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/settings/notification.py
--rw-r--r--   0        0        0     7376 2021-04-08 11:13:57.991774 sdccli-0.7.8/sdccli/cli/settings/team.py
--rw-r--r--   0        0        0     3749 2021-04-08 11:13:57.995774 sdccli-0.7.8/sdccli/cli/settings/user.py
--rw-r--r--   0        0        0     5394 2021-04-08 11:13:57.995774 sdccli-0.7.8/sdccli/config.py
--rw-r--r--   0        0        0     8316 2021-04-08 11:13:57.995774 sdccli-0.7.8/sdccli/drop.py
--rw-r--r--   0        0        0     2804 2021-04-08 11:13:57.995774 sdccli-0.7.8/sdccli/falco_macro.py
--rw-r--r--   0        0        0      639 2021-04-08 11:13:57.995774 sdccli-0.7.8/sdccli/helpers.py
--rw-r--r--   0        0        0      796 2021-04-08 11:13:57.995774 sdccli-0.7.8/sdccli/printer.py
--rw-r--r--   0        0        0    20309 2021-04-08 11:13:57.995774 sdccli-0.7.8/sdccli/restore.py
--rw-r--r--   0        0        0     1493 2021-04-08 11:13:57.995774 sdccli-0.7.8/sdccli/time.py
--rw-r--r--   0        0        0        0 2021-04-08 11:13:57.995774 sdccli-0.7.8/sdccli/usecases/__init__.py
--rw-r--r--   0        0        0     2379 2021-04-08 11:13:57.995774 sdccli-0.7.8/sdccli/usecases/alert.py
--rw-r--r--   0        0        0        0 2021-04-08 11:13:57.995774 sdccli-0.7.8/sdccli/usecases/backup/Pipfile
--rw-r--r--   0        0        0       42 2021-04-08 11:13:57.995774 sdccli-0.7.8/sdccli/usecases/backup/__init__.py
--rw-r--r--   0        0        0    12512 2021-04-08 11:13:57.995774 sdccli-0.7.8/sdccli/usecases/backup/dump.py
--rw-r--r--   0        0        0    13838 2021-04-08 11:13:57.995774 sdccli-0.7.8/sdccli/usecases/backup/restore.py
--rw-r--r--   0        0        0        0 2021-04-08 11:13:57.995774 sdccli-0.7.8/sdccli/usecases/dashboard/__init__.py
--rw-r--r--   0        0        0     5161 2021-04-08 11:13:57.995774 sdccli-0.7.8/sdccli/usecases/dashboard/dashboard_v2.py
--rw-r--r--   0        0        0     6105 2021-04-08 11:13:57.995774 sdccli-0.7.8/sdccli/usecases/dashboard/dashboard_v3.py
--rw-r--r--   0        0        0     6903 2021-04-08 11:13:57.995774 sdccli-0.7.8/sdccli/usecases/dashboard/panel.py
--rw-r--r--   0        0        0        0 2021-04-08 11:13:57.995774 sdccli-0.7.8/sdccli/usecases/policy/__init__.py
--rw-r--r--   0        0        0     2247 2021-04-08 11:13:57.995774 sdccli-0.7.8/sdccli/usecases/policy/events.py
--rw-r--r--   0        0        0        0 2021-04-08 11:13:57.995774 sdccli-0.7.8/sdccli/usecases/scanning/__init__.py
--rw-r--r--   0        0        0     1137 2021-04-08 11:13:57.995774 sdccli-0.7.8/sdccli/usecases/scanning/alert.py
--rw-r--r--   0        0        0     3259 2021-04-08 11:13:57.995774 sdccli-0.7.8/sdccli/usecases/scanning/image.py
--rw-r--r--   0        0        0     3781 2021-04-08 11:13:57.995774 sdccli-0.7.8/sdccli/usecases/scanning/vulnerability.py
--rw-r--r--   0        0        0        0 2021-04-08 11:13:57.995774 sdccli-0.7.8/sdccli/usecases/settings/__init__.py
--rw-r--r--   0        0        0      530 2021-04-08 11:13:57.995774 sdccli-0.7.8/sdccli/usecases/settings/team.py
--rw-r--r--   0        0        0     1341 2021-04-08 11:14:10.379449 sdccli-0.7.8/setup.py
--rw-r--r--   0        0        0      872 2021-04-08 11:14:10.379796 sdccli-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2021-04-14 09:50:37.618261 sdccli-0.7.9/LICENSE.txt
+-rw-r--r--   0        0        0      937 2021-04-14 09:50:48.366396 sdccli-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0       21 2021-04-14 09:50:48.366396 sdccli-0.7.9/sdccli/__init__.py
+-rw-r--r--   0        0        0     2127 2021-04-14 09:50:37.618261 sdccli-0.7.9/sdccli/cli/__init__.py
+-rw-r--r--   0        0        0     5291 2021-04-14 09:50:37.618261 sdccli-0.7.9/sdccli/cli/alert.py
+-rw-r--r--   0        0        0     9160 2021-04-14 09:50:37.618261 sdccli-0.7.9/sdccli/cli/backup.py
+-rw-r--r--   0        0        0     5549 2021-04-14 09:50:37.618261 sdccli-0.7.9/sdccli/cli/capture.py
+-rw-r--r--   0        0        0     3924 2021-04-14 09:50:37.618261 sdccli-0.7.9/sdccli/cli/command.py
+-rw-r--r--   0        0        0     8177 2021-04-14 09:50:37.618261 sdccli-0.7.9/sdccli/cli/compliance.py
+-rw-r--r--   0        0        0     7144 2021-04-14 09:50:37.618261 sdccli-0.7.9/sdccli/cli/dashboard/__init__.py
+-rw-r--r--   0        0        0     5036 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/dashboard/panel.py
+-rw-r--r--   0        0        0     7872 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/dashboardv2.py
+-rw-r--r--   0        0        0     4617 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/event.py
+-rw-r--r--   0        0        0     4406 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/eventv1.py
+-rw-r--r--   0        0        0        0 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/formatter/__init__.py
+-rw-r--r--   0        0        0      139 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/formatter/json_formatter/__init__.py
+-rw-r--r--   0        0        0      841 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/formatter/text_formatter/__init__.py
+-rw-r--r--   0        0        0      464 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/formatter/text_formatter/alert.py
+-rw-r--r--   0        0        0      887 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/formatter/text_formatter/dashboard.py
+-rw-r--r--   0        0        0     1017 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/formatter/text_formatter/panel.py
+-rw-r--r--   0        0        0     1962 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/formatter/text_formatter/policy_events.py
+-rw-r--r--   0        0        0        0 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/formatter/text_formatter/scanning/__init__.py
+-rw-r--r--   0        0        0      537 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/formatter/text_formatter/scanning/alert.py
+-rw-r--r--   0        0        0     4497 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/formatter/text_formatter/scanning/image.py
+-rw-r--r--   0        0        0     3583 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/formatter/text_formatter/scanning/vulnerability.py
+-rw-r--r--   0        0        0    18732 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/policy/__init__.py
+-rw-r--r--   0        0        0     3528 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/policy/falco_list.py
+-rw-r--r--   0        0        0     3548 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/policy/falco_macro.py
+-rw-r--r--   0        0        0    10159 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/policy/rule.py
+-rw-r--r--   0        0        0     6687 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/profile.py
+-rw-r--r--   0        0        0      884 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/scanning/__init__.py
+-rw-r--r--   0        0        0     3788 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/scanning/alert.py
+-rw-r--r--   0        0        0     7778 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/scanning/cve_report.py
+-rw-r--r--   0        0        0     8439 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/scanning/image.py
+-rw-r--r--   0        0        0     3925 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/scanning/policy.py
+-rw-r--r--   0        0        0     3702 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/scanning/query.py
+-rw-r--r--   0        0        0     4148 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/scanning/registry.py
+-rw-r--r--   0        0        0     3419 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/scanning/repo.py
+-rw-r--r--   0        0        0     1470 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/scanning/runtime.py
+-rw-r--r--   0        0        0     2484 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/scanning/subscription.py
+-rw-r--r--   0        0        0     4079 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/scanning/vulnerability/__init__.py
+-rw-r--r--   0        0        0     1848 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/scanning/vulnerability/bundle.py
+-rw-r--r--   0        0        0      587 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/settings/__init__.py
+-rw-r--r--   0        0        0     1893 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/settings/access_key.py
+-rw-r--r--   0        0        0     3071 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/settings/notification.py
+-rw-r--r--   0        0        0     7376 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/settings/team.py
+-rw-r--r--   0        0        0     3749 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/settings/user.py
+-rw-r--r--   0        0        0     5394 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/config.py
+-rw-r--r--   0        0        0     8316 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/drop.py
+-rw-r--r--   0        0        0     2804 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/falco_macro.py
+-rw-r--r--   0        0        0      639 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/helpers.py
+-rw-r--r--   0        0        0      796 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/printer.py
+-rw-r--r--   0        0        0    20309 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/restore.py
+-rw-r--r--   0        0        0     1493 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/time.py
+-rw-r--r--   0        0        0        0 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/__init__.py
+-rw-r--r--   0        0        0     2379 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/alert.py
+-rw-r--r--   0        0        0        0 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/backup/Pipfile
+-rw-r--r--   0        0        0       42 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/backup/__init__.py
+-rw-r--r--   0        0        0    12512 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/backup/dump.py
+-rw-r--r--   0        0        0    13838 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/backup/restore.py
+-rw-r--r--   0        0        0        0 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/dashboard/__init__.py
+-rw-r--r--   0        0        0     5161 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/dashboard/dashboard_v2.py
+-rw-r--r--   0        0        0     6105 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/dashboard/dashboard_v3.py
+-rw-r--r--   0        0        0     6903 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/dashboard/panel.py
+-rw-r--r--   0        0        0        0 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/policy/__init__.py
+-rw-r--r--   0        0        0     2247 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/policy/events.py
+-rw-r--r--   0        0        0        0 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/scanning/__init__.py
+-rw-r--r--   0        0        0     1137 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/scanning/alert.py
+-rw-r--r--   0        0        0     4084 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/scanning/image.py
+-rw-r--r--   0        0        0     3781 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/scanning/vulnerability.py
+-rw-r--r--   0        0        0        0 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/settings/__init__.py
+-rw-r--r--   0        0        0      530 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/settings/team.py
+-rw-r--r--   0        0        0     1341 2021-04-14 09:50:48.895765 sdccli-0.7.9/setup.py
+-rw-r--r--   0        0        0      872 2021-04-14 09:50:48.896160 sdccli-0.7.9/PKG-INFO
```

### Comparing `sdccli-0.7.8/LICENSE.txt` & `sdccli-0.7.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/pyproject.toml` & `sdccli-0.7.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdccli"
-version = "0.7.8"
+version = "0.7.9"
 description = "CLI client for Sysdig Cloud"
 authors = ["Sysdig Inc. <info@sysdig.com>"]
 license = "MIT"
 maintainers = [
     "Nestor Salceda <nestor.salceda@sysdig.com>",
     "Federico Barcelona <fede.barcelona@sysdig.com>"
 ]
```

### Comparing `sdccli-0.7.8/sdccli/cli/__init__.py` & `sdccli-0.7.9/sdccli/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/alert.py` & `sdccli-0.7.9/sdccli/cli/alert.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/backup.py` & `sdccli-0.7.9/sdccli/cli/backup.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/capture.py` & `sdccli-0.7.9/sdccli/cli/capture.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/command.py` & `sdccli-0.7.9/sdccli/cli/command.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/compliance.py` & `sdccli-0.7.9/sdccli/cli/compliance.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/dashboard/__init__.py` & `sdccli-0.7.9/sdccli/cli/dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/dashboard/panel.py` & `sdccli-0.7.9/sdccli/cli/dashboard/panel.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/dashboardv2.py` & `sdccli-0.7.9/sdccli/cli/dashboardv2.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/event.py` & `sdccli-0.7.9/sdccli/cli/event.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/eventv1.py` & `sdccli-0.7.9/sdccli/cli/eventv1.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/formatter/text_formatter/__init__.py` & `sdccli-0.7.9/sdccli/cli/formatter/text_formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/formatter/text_formatter/dashboard.py` & `sdccli-0.7.9/sdccli/cli/formatter/text_formatter/dashboard.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/formatter/text_formatter/panel.py` & `sdccli-0.7.9/sdccli/cli/formatter/text_formatter/panel.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/formatter/text_formatter/policy_events.py` & `sdccli-0.7.9/sdccli/cli/formatter/text_formatter/policy_events.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/formatter/text_formatter/scanning/alert.py` & `sdccli-0.7.9/sdccli/cli/formatter/text_formatter/scanning/alert.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/formatter/text_formatter/scanning/image.py` & `sdccli-0.7.9/sdccli/cli/formatter/text_formatter/scanning/image.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,14 +55,19 @@
         'npm': ['package', 'version', 'location'],
         'gem': ['package', 'version', 'location'],
         'python': ['package', 'version', 'location'],
         'java': ['package', 'specification-version', 'implementation-version', 'location']
     }
     if query_type in keys:
         print_list(content, keys[query_type])
+    elif query_type in ['all', 'all+files']:
+        for elem in content:
+            content_type = elem["content_type"]
+            print(f"# {content_type}:")
+            _print_query((elem, content_type))
     else:
         print_list(content, content[0].keys())
 
 
 def _print_vuln(res):
     res, query_type = res
     if "vulnerabilities" not in res:
```

### Comparing `sdccli-0.7.8/sdccli/cli/formatter/text_formatter/scanning/vulnerability.py` & `sdccli-0.7.9/sdccli/cli/formatter/text_formatter/scanning/vulnerability.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/policy/__init__.py` & `sdccli-0.7.9/sdccli/cli/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/policy/falco_list.py` & `sdccli-0.7.9/sdccli/cli/policy/falco_list.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/policy/falco_macro.py` & `sdccli-0.7.9/sdccli/cli/policy/falco_macro.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/policy/rule.py` & `sdccli-0.7.9/sdccli/cli/policy/rule.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/profile.py` & `sdccli-0.7.9/sdccli/cli/profile.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/scanning/__init__.py` & `sdccli-0.7.9/sdccli/cli/scanning/__init__.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/scanning/alert.py` & `sdccli-0.7.9/sdccli/cli/scanning/alert.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/scanning/cve_report.py` & `sdccli-0.7.9/sdccli/cli/scanning/cve_report.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/scanning/image.py` & `sdccli-0.7.9/sdccli/cli/scanning/image.py`

 * *Files 9% similar despite different names*

```diff
@@ -79,29 +79,37 @@
     except Exception as ex:
         print(f"Error: {str(ex)}")
         sys.exit(1)
 
 
 @image.command(name='content', short_help="Get contents of image")
 @click.argument('input_image', nargs=1)
-@click.argument('content_type', nargs=1, required=False)
+@click.argument('content_type', nargs=1, required=True)
 @click.pass_obj
 def query_content(cnf, input_image, content_type):
     """
     INPUT_IMAGE: Input image can be in the following formats: Image Digest, ImageID or registry/repo:tag
 
     CONTENT_TYPE: The content type can be one of the following types:
 
       - os: Operating System Packages
 
+      - files: Files
+
       - npm: Node.JS NPM Module
 
       - gem: Ruby GEM
 
-      - files: Files
+      - python: Python modules
+
+      - java: Java packages
+
+      - all: includes [os, npm, gem, python, java] contents
+
+      - all+files: includes [os, npm, gem, python, java, files] contents
     """
     try:
         res = use_case.query_image_content(cnf.sdscanning, input_image, content_type)
         cnf.formatter.format((res, content_type), "scanningQueryImage")
     except Exception as ex:
         print(f"Error: {str(ex)}")
         sys.exit(1)
```

### Comparing `sdccli-0.7.8/sdccli/cli/scanning/policy.py` & `sdccli-0.7.9/sdccli/cli/scanning/policy.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/scanning/query.py` & `sdccli-0.7.9/sdccli/cli/scanning/query.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/scanning/registry.py` & `sdccli-0.7.9/sdccli/cli/scanning/registry.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/scanning/repo.py` & `sdccli-0.7.9/sdccli/cli/scanning/repo.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/scanning/runtime.py` & `sdccli-0.7.9/sdccli/cli/scanning/runtime.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/scanning/subscription.py` & `sdccli-0.7.9/sdccli/cli/scanning/subscription.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/scanning/vulnerability/__init__.py` & `sdccli-0.7.9/sdccli/cli/scanning/vulnerability/__init__.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/scanning/vulnerability/bundle.py` & `sdccli-0.7.9/sdccli/cli/scanning/vulnerability/bundle.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/settings/__init__.py` & `sdccli-0.7.9/sdccli/cli/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/settings/access_key.py` & `sdccli-0.7.9/sdccli/cli/settings/access_key.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/settings/notification.py` & `sdccli-0.7.9/sdccli/cli/settings/notification.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/settings/team.py` & `sdccli-0.7.9/sdccli/cli/settings/team.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/cli/settings/user.py` & `sdccli-0.7.9/sdccli/cli/settings/user.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/config.py` & `sdccli-0.7.9/sdccli/config.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/drop.py` & `sdccli-0.7.9/sdccli/drop.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/falco_macro.py` & `sdccli-0.7.9/sdccli/falco_macro.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/helpers.py` & `sdccli-0.7.9/sdccli/helpers.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/printer.py` & `sdccli-0.7.9/sdccli/printer.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/restore.py` & `sdccli-0.7.9/sdccli/restore.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/time.py` & `sdccli-0.7.9/sdccli/time.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/usecases/alert.py` & `sdccli-0.7.9/sdccli/usecases/alert.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/usecases/backup/dump.py` & `sdccli-0.7.9/sdccli/usecases/backup/dump.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/usecases/backup/restore.py` & `sdccli-0.7.9/sdccli/usecases/backup/restore.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/usecases/dashboard/dashboard_v2.py` & `sdccli-0.7.9/sdccli/usecases/dashboard/dashboard_v2.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/usecases/dashboard/dashboard_v3.py` & `sdccli-0.7.9/sdccli/usecases/dashboard/dashboard_v3.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/usecases/dashboard/panel.py` & `sdccli-0.7.9/sdccli/usecases/dashboard/panel.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/usecases/policy/events.py` & `sdccli-0.7.9/sdccli/usecases/policy/events.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/usecases/scanning/alert.py` & `sdccli-0.7.9/sdccli/usecases/scanning/alert.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/usecases/scanning/image.py` & `sdccli-0.7.9/sdccli/usecases/scanning/image.py`

 * *Files 26% similar despite different names*

```diff
@@ -50,21 +50,44 @@
     if not ok:
         raise Exception(res)
 
     return res[0]
 
 
 def query_image_content(scanning: SdScanningClient, input_image, content_type):
-    if content_type not in ["os", "npm", "gem", "files"]:
-        raise ValueError(f"Incorrect content type provided '{content_type}', must be one of: [os, npm, gem, files]")
-    ok, res = scanning.query_image_content(input_image, content_type)
-    if not ok:
-        raise Exception(res)
+    supported_content_types = ["os", "npm", "gem", "files", "java", "python", "all", "all+files"]
+    content_type = content_type.lower()
+
+    if content_type not in supported_content_types:
+        raise ValueError(f"Incorrect content type provided '{content_type}', must be one of: {supported_content_types}")
+
+    if content_type not in ["all", "all+files"]:
+        ok, res = scanning.query_image_content(input_image, content_type)
+        if not ok:
+            raise Exception(res)
+
+        return res
+
+    if content_type == "all":
+        result = {"content": [], "content_type": "all"}
+
+        for type in ["os", "npm", "gem", "java", "python"]:
+            result["content"].append(query_image_content(scanning, input_image, type))
+
+        return result
+
+    if content_type == "all+files":
+        result = {"content": [], "content_type": "all+files"}
+
+        for type in ["os", "npm", "gem", "java", "python", "files"]:
+            result["content"].append(query_image_content(scanning, input_image, type))
+
+        return result
 
-    return res
+    raise Exception("unreachable code reached! report this to the CLI maintainers")
 
 
 def query_image_metadata(scanning: SdScanningClient, input_image, metadata_type):
     if metadata_type not in ["manifest", "dockerfile", "docker_history"]:
         raise ValueError(
             "Incorrect metadata type provided 'foo', must be one of: [manifest, dockerfile, docker_history]")
     ok, res = scanning.query_image_metadata(input_image, metadata_type)
```

### Comparing `sdccli-0.7.8/sdccli/usecases/scanning/vulnerability.py` & `sdccli-0.7.9/sdccli/usecases/scanning/vulnerability.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/sdccli/usecases/settings/team.py` & `sdccli-0.7.9/sdccli/usecases/settings/team.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.8/setup.py` & `sdccli-0.7.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
  'sdcclient>=0.15.1,<0.16.0']
 
 entry_points = \
 {'console_scripts': ['sdc-cli = sdccli.cli:cli']}
 
 setup_kwargs = {
     'name': 'sdccli',
-    'version': '0.7.8',
+    'version': '0.7.9',
     'description': 'CLI client for Sysdig Cloud',
     'long_description': None,
     'author': 'Sysdig Inc.',
     'author_email': 'info@sysdig.com',
     'maintainer': 'Nestor Salceda',
     'maintainer_email': 'nestor.salceda@sysdig.com',
     'url': None,
```

### Comparing `sdccli-0.7.8/PKG-INFO` & `sdccli-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdccli
-Version: 0.7.8
+Version: 0.7.9
 Summary: CLI client for Sysdig Cloud
 License: MIT
 Author: Sysdig Inc.
 Author-email: info@sysdig.com
 Maintainer: Nestor Salceda
 Maintainer-email: nestor.salceda@sysdig.com
 Requires-Python: >=3.6,<4.0
```

