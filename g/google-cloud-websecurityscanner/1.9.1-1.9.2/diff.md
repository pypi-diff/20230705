# Comparing `tmp/google-cloud-websecurityscanner-1.9.1.tar.gz` & `tmp/google-cloud-websecurityscanner-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-websecurityscanner-1.9.1.tar", last modified: Tue Oct  4 00:47:36 2022, max compression
+gzip compressed data, was "google-cloud-websecurityscanner-1.9.2.tar", last modified: Mon Oct 10 16:14:35 2022, max compression
```

## Comparing `google-cloud-websecurityscanner-1.9.1.tar` & `google-cloud-websecurityscanner-1.9.2.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:47:36.386155 google-cloud-websecurityscanner-1.9.1/
--rw-rw-r--   0 root         (0)     1003    11358 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4964 2022-10-04 00:47:36.386155 google-cloud-websecurityscanner-1.9.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4036 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:47:36.370154 google-cloud-websecurityscanner-1.9.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:47:36.370154 google-cloud-websecurityscanner-1.9.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:47:36.370154 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner/
--rw-rw-r--   0 root         (0)     1003     3288 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner/__init__.py
--rw-rw-r--   0 root         (0)     1003       92 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:47:36.374155 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/
--rw-rw-r--   0 root         (0)     1003     2761 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3811 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       92 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:47:36.374155 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:47:36.374155 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/services/web_security_scanner/
--rw-rw-r--   0 root         (0)     1003      785 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/services/web_security_scanner/__init__.py
--rw-rw-r--   0 root         (0)     1003    54256 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/services/web_security_scanner/async_client.py
--rw-rw-r--   0 root         (0)     1003    62158 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/services/web_security_scanner/client.py
--rw-rw-r--   0 root         (0)     1003    21558 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/services/web_security_scanner/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:47:36.374155 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/services/web_security_scanner/transports/
--rw-rw-r--   0 root         (0)     1003     1237 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/services/web_security_scanner/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    15532 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/services/web_security_scanner/transports/base.py
--rw-rw-r--   0 root         (0)     1003    26035 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/services/web_security_scanner/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    26609 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/services/web_security_scanner/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:47:36.378155 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/types/
--rw-rw-r--   0 root         (0)     1003     2513 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     1638 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/types/crawled_url.py
--rw-rw-r--   0 root         (0)     1003     6265 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/types/finding.py
--rw-rw-r--   0 root         (0)     1003     6096 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/types/finding_addon.py
--rw-rw-r--   0 root         (0)     1003     1387 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/types/finding_type_stats.py
--rw-rw-r--   0 root         (0)     1003    11458 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/types/scan_config.py
--rw-rw-r--   0 root         (0)     1003     3656 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/types/scan_config_error.py
--rw-rw-r--   0 root         (0)     1003     5180 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/types/scan_run.py
--rw-rw-r--   0 root         (0)     1003     2493 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/types/scan_run_error_trace.py
--rw-rw-r--   0 root         (0)     1003     2639 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/types/scan_run_log.py
--rw-rw-r--   0 root         (0)     1003     1631 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/types/scan_run_warning_trace.py
--rw-rw-r--   0 root         (0)     1003    13738 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/types/web_security_scanner.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:47:36.378155 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/
--rw-rw-r--   0 root         (0)     1003     2410 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/__init__.py
--rw-rw-r--   0 root         (0)     1003     3821 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       92 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:47:36.378155 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:47:36.378155 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/
--rw-rw-r--   0 root         (0)     1003      785 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/__init__.py
--rw-rw-r--   0 root         (0)     1003    71298 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/async_client.py
--rw-rw-r--   0 root         (0)     1003    80311 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/client.py
--rw-rw-r--   0 root         (0)     1003    21723 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:47:36.378155 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/transports/
--rw-rw-r--   0 root         (0)     1003     1237 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    15735 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/transports/base.py
--rw-rw-r--   0 root         (0)     1003    26318 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    26892 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:47:36.378155 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/types/
--rw-rw-r--   0 root         (0)     1003     2186 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     1643 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/types/crawled_url.py
--rw-rw-r--   0 root         (0)     1003     5379 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/types/finding.py
--rw-rw-r--   0 root         (0)     1003     3849 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/types/finding_addon.py
--rw-rw-r--   0 root         (0)     1003     1523 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/types/finding_type_stats.py
--rw-rw-r--   0 root         (0)     1003     8231 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/types/scan_config.py
--rw-rw-r--   0 root         (0)     1003     4170 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/types/scan_run.py
--rw-rw-r--   0 root         (0)     1003    13820 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/types/web_security_scanner.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:47:36.382155 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/
--rw-rw-r--   0 root         (0)     1003     2680 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003     3819 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       92 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:47:36.382155 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:47:36.382155 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/
--rw-rw-r--   0 root         (0)     1003      785 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/__init__.py
--rw-rw-r--   0 root         (0)     1003    71292 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/async_client.py
--rw-rw-r--   0 root         (0)     1003    80305 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/client.py
--rw-rw-r--   0 root         (0)     1003    21690 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:47:36.382155 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/transports/
--rw-rw-r--   0 root         (0)     1003     1237 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    15731 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/transports/base.py
--rw-rw-r--   0 root         (0)     1003    26301 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    26875 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:47:36.382155 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/types/
--rw-rw-r--   0 root         (0)     1003     2438 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     1603 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/types/crawled_url.py
--rw-rw-r--   0 root         (0)     1003     5289 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/types/finding.py
--rw-rw-r--   0 root         (0)     1003     4348 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/types/finding_addon.py
--rw-rw-r--   0 root         (0)     1003     1353 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/types/finding_type_stats.py
--rw-rw-r--   0 root         (0)     1003     9458 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/types/scan_config.py
--rw-rw-r--   0 root         (0)     1003     3638 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/types/scan_config_error.py
--rw-rw-r--   0 root         (0)     1003     5025 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/types/scan_run.py
--rw-rw-r--   0 root         (0)     1003     2458 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/types/scan_run_error_trace.py
--rw-rw-r--   0 root         (0)     1003     1575 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/types/scan_run_warning_trace.py
--rw-rw-r--   0 root         (0)     1003    13808 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/types/web_security_scanner.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:47:36.386155 google-cloud-websecurityscanner-1.9.1/google_cloud_websecurityscanner.egg-info/
--rw-r--r--   0 root         (0)     1003     4964 2022-10-04 00:47:36.000000 google-cloud-websecurityscanner-1.9.1/google_cloud_websecurityscanner.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     5655 2022-10-04 00:47:36.000000 google-cloud-websecurityscanner-1.9.1/google_cloud_websecurityscanner.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-04 00:47:36.000000 google-cloud-websecurityscanner-1.9.1/google_cloud_websecurityscanner.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2022-10-04 00:47:36.000000 google-cloud-websecurityscanner-1.9.1/google_cloud_websecurityscanner.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-04 00:47:36.000000 google-cloud-websecurityscanner-1.9.1/google_cloud_websecurityscanner.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      160 2022-10-04 00:47:36.000000 google-cloud-websecurityscanner-1.9.1/google_cloud_websecurityscanner.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2022-10-04 00:47:36.000000 google-cloud-websecurityscanner-1.9.1/google_cloud_websecurityscanner.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:47:36.386155 google-cloud-websecurityscanner-1.9.1/scripts/
--rw-rw-r--   0 root         (0)     1003     6616 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/scripts/fixup_websecurityscanner_v1alpha_keywords.py
--rw-rw-r--   0 root         (0)     1003     6616 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/scripts/fixup_websecurityscanner_v1beta_keywords.py
--rw-rw-r--   0 root         (0)     1003       67 2022-10-04 00:47:36.390155 google-cloud-websecurityscanner-1.9.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3008 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:47:36.386155 google-cloud-websecurityscanner-1.9.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:47:36.386155 google-cloud-websecurityscanner-1.9.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:47:36.386155 google-cloud-websecurityscanner-1.9.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:47:36.386155 google-cloud-websecurityscanner-1.9.1/tests/unit/gapic/websecurityscanner_v1/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/tests/unit/gapic/websecurityscanner_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   162468 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/tests/unit/gapic/websecurityscanner_v1/test_web_security_scanner.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:47:36.386155 google-cloud-websecurityscanner-1.9.1/tests/unit/gapic/websecurityscanner_v1alpha/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/tests/unit/gapic/websecurityscanner_v1alpha/__init__.py
--rw-rw-r--   0 root         (0)     1003   200315 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/tests/unit/gapic/websecurityscanner_v1alpha/test_web_security_scanner.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:47:36.386155 google-cloud-websecurityscanner-1.9.1/tests/unit/gapic/websecurityscanner_v1beta/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/tests/unit/gapic/websecurityscanner_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003   202728 2022-10-04 00:44:49.000000 google-cloud-websecurityscanner-1.9.1/tests/unit/gapic/websecurityscanner_v1beta/test_web_security_scanner.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:14:35.987449 google-cloud-websecurityscanner-1.9.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4964 2022-10-10 16:14:35.991449 google-cloud-websecurityscanner-1.9.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4036 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:14:35.959449 google-cloud-websecurityscanner-1.9.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:14:35.959449 google-cloud-websecurityscanner-1.9.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:14:35.963449 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner/
+-rw-rw-r--   0 root         (0)     1003     3288 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner/__init__.py
+-rw-rw-r--   0 root         (0)     1003       92 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:14:35.963449 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/
+-rw-rw-r--   0 root         (0)     1003     2761 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3811 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       92 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:14:35.963449 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:14:35.963449 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/services/web_security_scanner/
+-rw-rw-r--   0 root         (0)     1003      785 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/services/web_security_scanner/__init__.py
+-rw-rw-r--   0 root         (0)     1003    54256 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/services/web_security_scanner/async_client.py
+-rw-rw-r--   0 root         (0)     1003    62158 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/services/web_security_scanner/client.py
+-rw-rw-r--   0 root         (0)     1003    21558 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/services/web_security_scanner/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:14:35.967449 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/services/web_security_scanner/transports/
+-rw-rw-r--   0 root         (0)     1003     1237 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/services/web_security_scanner/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15532 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/services/web_security_scanner/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    26035 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/services/web_security_scanner/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    26609 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/services/web_security_scanner/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:14:35.971449 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2513 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1638 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/types/crawled_url.py
+-rw-rw-r--   0 root         (0)     1003     6265 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/types/finding.py
+-rw-rw-r--   0 root         (0)     1003     6096 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/types/finding_addon.py
+-rw-rw-r--   0 root         (0)     1003     1387 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/types/finding_type_stats.py
+-rw-rw-r--   0 root         (0)     1003    11458 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/types/scan_config.py
+-rw-rw-r--   0 root         (0)     1003     3656 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/types/scan_config_error.py
+-rw-rw-r--   0 root         (0)     1003     5180 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/types/scan_run.py
+-rw-rw-r--   0 root         (0)     1003     2493 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/types/scan_run_error_trace.py
+-rw-rw-r--   0 root         (0)     1003     2639 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/types/scan_run_log.py
+-rw-rw-r--   0 root         (0)     1003     1631 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/types/scan_run_warning_trace.py
+-rw-rw-r--   0 root         (0)     1003    13738 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/types/web_security_scanner.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:14:35.971449 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/
+-rw-rw-r--   0 root         (0)     1003     2410 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3821 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       92 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:14:35.971449 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:14:35.971449 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/
+-rw-rw-r--   0 root         (0)     1003      785 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/__init__.py
+-rw-rw-r--   0 root         (0)     1003    71298 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/async_client.py
+-rw-rw-r--   0 root         (0)     1003    80311 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/client.py
+-rw-rw-r--   0 root         (0)     1003    21723 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:14:35.971449 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/transports/
+-rw-rw-r--   0 root         (0)     1003     1237 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15735 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    26318 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    26892 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:14:35.975449 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/types/
+-rw-rw-r--   0 root         (0)     1003     2186 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1643 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/types/crawled_url.py
+-rw-rw-r--   0 root         (0)     1003     5379 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/types/finding.py
+-rw-rw-r--   0 root         (0)     1003     3849 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/types/finding_addon.py
+-rw-rw-r--   0 root         (0)     1003     1523 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/types/finding_type_stats.py
+-rw-rw-r--   0 root         (0)     1003     8231 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/types/scan_config.py
+-rw-rw-r--   0 root         (0)     1003     4170 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/types/scan_run.py
+-rw-rw-r--   0 root         (0)     1003    13820 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/types/web_security_scanner.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:14:35.975449 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/
+-rw-rw-r--   0 root         (0)     1003     2680 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3819 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       92 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:14:35.975449 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:14:35.979449 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/
+-rw-rw-r--   0 root         (0)     1003      785 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/__init__.py
+-rw-rw-r--   0 root         (0)     1003    71292 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/async_client.py
+-rw-rw-r--   0 root         (0)     1003    80305 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/client.py
+-rw-rw-r--   0 root         (0)     1003    21690 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:14:35.979449 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/transports/
+-rw-rw-r--   0 root         (0)     1003     1237 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15731 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    26301 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    26875 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:14:35.983449 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/types/
+-rw-rw-r--   0 root         (0)     1003     2438 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1603 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/types/crawled_url.py
+-rw-rw-r--   0 root         (0)     1003     5289 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/types/finding.py
+-rw-rw-r--   0 root         (0)     1003     4348 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/types/finding_addon.py
+-rw-rw-r--   0 root         (0)     1003     1353 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/types/finding_type_stats.py
+-rw-rw-r--   0 root         (0)     1003     9458 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/types/scan_config.py
+-rw-rw-r--   0 root         (0)     1003     3638 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/types/scan_config_error.py
+-rw-rw-r--   0 root         (0)     1003     5025 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/types/scan_run.py
+-rw-rw-r--   0 root         (0)     1003     2458 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/types/scan_run_error_trace.py
+-rw-rw-r--   0 root         (0)     1003     1575 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/types/scan_run_warning_trace.py
+-rw-rw-r--   0 root         (0)     1003    13808 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/types/web_security_scanner.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:14:35.983449 google-cloud-websecurityscanner-1.9.2/google_cloud_websecurityscanner.egg-info/
+-rw-r--r--   0 root         (0)     1003     4964 2022-10-10 16:14:35.000000 google-cloud-websecurityscanner-1.9.2/google_cloud_websecurityscanner.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     5655 2022-10-10 16:14:35.000000 google-cloud-websecurityscanner-1.9.2/google_cloud_websecurityscanner.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-10-10 16:14:35.000000 google-cloud-websecurityscanner-1.9.2/google_cloud_websecurityscanner.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2022-10-10 16:14:35.000000 google-cloud-websecurityscanner-1.9.2/google_cloud_websecurityscanner.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-10-10 16:14:35.000000 google-cloud-websecurityscanner-1.9.2/google_cloud_websecurityscanner.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      232 2022-10-10 16:14:35.000000 google-cloud-websecurityscanner-1.9.2/google_cloud_websecurityscanner.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2022-10-10 16:14:35.000000 google-cloud-websecurityscanner-1.9.2/google_cloud_websecurityscanner.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:14:35.983449 google-cloud-websecurityscanner-1.9.2/scripts/
+-rw-rw-r--   0 root         (0)     1003     6616 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/scripts/fixup_websecurityscanner_v1alpha_keywords.py
+-rw-rw-r--   0 root         (0)     1003     6616 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/scripts/fixup_websecurityscanner_v1beta_keywords.py
+-rw-rw-r--   0 root         (0)     1003       67 2022-10-10 16:14:35.991449 google-cloud-websecurityscanner-1.9.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3077 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:14:35.983449 google-cloud-websecurityscanner-1.9.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:14:35.983449 google-cloud-websecurityscanner-1.9.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:14:35.983449 google-cloud-websecurityscanner-1.9.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:14:35.987449 google-cloud-websecurityscanner-1.9.2/tests/unit/gapic/websecurityscanner_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/tests/unit/gapic/websecurityscanner_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   162468 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/tests/unit/gapic/websecurityscanner_v1/test_web_security_scanner.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:14:35.987449 google-cloud-websecurityscanner-1.9.2/tests/unit/gapic/websecurityscanner_v1alpha/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/tests/unit/gapic/websecurityscanner_v1alpha/__init__.py
+-rw-rw-r--   0 root         (0)     1003   200315 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/tests/unit/gapic/websecurityscanner_v1alpha/test_web_security_scanner.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:14:35.987449 google-cloud-websecurityscanner-1.9.2/tests/unit/gapic/websecurityscanner_v1beta/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/tests/unit/gapic/websecurityscanner_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003   202728 2022-10-10 16:11:49.000000 google-cloud-websecurityscanner-1.9.2/tests/unit/gapic/websecurityscanner_v1beta/test_web_security_scanner.py
```

### Comparing `google-cloud-websecurityscanner-1.9.1/LICENSE` & `google-cloud-websecurityscanner-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/MANIFEST.in` & `google-cloud-websecurityscanner-1.9.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/PKG-INFO` & `google-cloud-websecurityscanner-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-websecurityscanner
-Version: 1.9.1
+Version: 1.9.2
 Summary: ('Google Cloud Web Security Scanner API client library',)
 Home-page: https://github.com/googleapis/python-websecurityscanner
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-websecurityscanner-1.9.1/README.rst` & `google-cloud-websecurityscanner-1.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner/__init__.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/__init__.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/gapic_metadata.json` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/services/__init__.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/services/web_security_scanner/__init__.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/services/web_security_scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/services/web_security_scanner/async_client.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/services/web_security_scanner/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/services/web_security_scanner/client.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/services/web_security_scanner/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/services/web_security_scanner/pagers.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/services/web_security_scanner/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/services/web_security_scanner/transports/__init__.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/services/web_security_scanner/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/services/web_security_scanner/transports/base.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/services/web_security_scanner/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/services/web_security_scanner/transports/grpc.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/services/web_security_scanner/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/services/web_security_scanner/transports/grpc_asyncio.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/services/web_security_scanner/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/types/__init__.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/types/crawled_url.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/types/crawled_url.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/types/finding.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/types/finding.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/types/finding_addon.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/types/finding_addon.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/types/finding_type_stats.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/types/finding_type_stats.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/types/scan_config.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/types/scan_config.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/types/scan_config_error.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/types/scan_config_error.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/types/scan_run.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/types/scan_run.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/types/scan_run_error_trace.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/types/scan_run_error_trace.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/types/scan_run_log.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/types/scan_run_log.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/types/scan_run_warning_trace.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/types/scan_run_warning_trace.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1/types/web_security_scanner.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1/types/web_security_scanner.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/__init__.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/gapic_metadata.json` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/services/__init__.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/__init__.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/async_client.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/client.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/pagers.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/transports/__init__.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/transports/base.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/transports/grpc.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/transports/grpc_asyncio.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/services/web_security_scanner/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/types/__init__.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/types/crawled_url.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/types/crawled_url.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/types/finding.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/types/finding.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/types/finding_addon.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/types/finding_addon.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/types/finding_type_stats.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/types/finding_type_stats.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/types/scan_config.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/types/scan_config.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/types/scan_run.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/types/scan_run.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1alpha/types/web_security_scanner.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1alpha/types/web_security_scanner.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/__init__.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/gapic_metadata.json` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/services/__init__.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/__init__.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/async_client.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/client.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/pagers.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/transports/__init__.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/transports/base.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/transports/grpc.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/transports/grpc_asyncio.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/services/web_security_scanner/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/types/__init__.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/types/crawled_url.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/types/crawled_url.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/types/finding.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/types/finding.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/types/finding_addon.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/types/finding_addon.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/types/finding_type_stats.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/types/finding_type_stats.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/types/scan_config.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/types/scan_config.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/types/scan_config_error.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/types/scan_config_error.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/types/scan_run.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/types/scan_run.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/types/scan_run_error_trace.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/types/scan_run_error_trace.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/types/scan_run_warning_trace.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/types/scan_run_warning_trace.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google/cloud/websecurityscanner_v1beta/types/web_security_scanner.py` & `google-cloud-websecurityscanner-1.9.2/google/cloud/websecurityscanner_v1beta/types/web_security_scanner.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/google_cloud_websecurityscanner.egg-info/PKG-INFO` & `google-cloud-websecurityscanner-1.9.2/google_cloud_websecurityscanner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-websecurityscanner
-Version: 1.9.1
+Version: 1.9.2
 Summary: ('Google Cloud Web Security Scanner API client library',)
 Home-page: https://github.com/googleapis/python-websecurityscanner
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-websecurityscanner-1.9.1/google_cloud_websecurityscanner.egg-info/SOURCES.txt` & `google-cloud-websecurityscanner-1.9.2/google_cloud_websecurityscanner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/scripts/fixup_websecurityscanner_v1alpha_keywords.py` & `google-cloud-websecurityscanner-1.9.2/scripts/fixup_websecurityscanner_v1alpha_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/scripts/fixup_websecurityscanner_v1beta_keywords.py` & `google-cloud-websecurityscanner-1.9.2/scripts/fixup_websecurityscanner_v1beta_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/setup.py` & `google-cloud-websecurityscanner-1.9.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,24 +17,24 @@
 
 import setuptools
 
 # Package metadata.
 
 name = "google-cloud-websecurityscanner"
 description = ("Google Cloud Web Security Scanner API client library",)
-version = "1.9.1"
+version = "1.9.2"
 # Should be one of:
 # 'Development Status :: 3 - Alpha'
 # 'Development Status :: 4 - Beta'
 # 'Development Status :: 5 - Production/Stable'
 release_status = "Development Status :: 5 - Production/Stable"
 dependencies = [
     "google-api-core[grpc] >= 1.32.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
-    "protobuf >= 3.20.2, <5.0.0dev",
+    "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
 extras = {}
 
 
 # Setup boilerplate below this line.
 
 package_root = os.path.abspath(os.path.dirname(__file__))
```

### Comparing `google-cloud-websecurityscanner-1.9.1/tests/__init__.py` & `google-cloud-websecurityscanner-1.9.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/tests/unit/__init__.py` & `google-cloud-websecurityscanner-1.9.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/tests/unit/gapic/__init__.py` & `google-cloud-websecurityscanner-1.9.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/tests/unit/gapic/websecurityscanner_v1/__init__.py` & `google-cloud-websecurityscanner-1.9.2/tests/unit/gapic/websecurityscanner_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/tests/unit/gapic/websecurityscanner_v1/test_web_security_scanner.py` & `google-cloud-websecurityscanner-1.9.2/tests/unit/gapic/websecurityscanner_v1/test_web_security_scanner.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/tests/unit/gapic/websecurityscanner_v1alpha/__init__.py` & `google-cloud-websecurityscanner-1.9.2/tests/unit/gapic/websecurityscanner_v1alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/tests/unit/gapic/websecurityscanner_v1alpha/test_web_security_scanner.py` & `google-cloud-websecurityscanner-1.9.2/tests/unit/gapic/websecurityscanner_v1alpha/test_web_security_scanner.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/tests/unit/gapic/websecurityscanner_v1beta/__init__.py` & `google-cloud-websecurityscanner-1.9.2/tests/unit/gapic/websecurityscanner_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-websecurityscanner-1.9.1/tests/unit/gapic/websecurityscanner_v1beta/test_web_security_scanner.py` & `google-cloud-websecurityscanner-1.9.2/tests/unit/gapic/websecurityscanner_v1beta/test_web_security_scanner.py`

 * *Files identical despite different names*

